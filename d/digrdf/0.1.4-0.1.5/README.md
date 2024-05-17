# Comparing `tmp/digrdf-0.1.4.tar.gz` & `tmp/digrdf-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digrdf-0.1.4.tar", max compression
+gzip compressed data, was "digrdf-0.1.5.tar", max compression
```

## Comparing `digrdf-0.1.4.tar` & `digrdf-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1143 2024-05-03 05:56:07.796450 digrdf-0.1.4/README.md
--rw-r--r--   0        0        0       35 2024-05-03 02:30:07.231145 digrdf-0.1.4/digrdf/__init__.py
--rw-r--r--   0        0        0     5111 2024-05-03 05:57:57.684489 digrdf-0.1.4/digrdf/__main__.py
--rw-r--r--   0        0        0      101 2024-05-03 05:49:19.197611 digrdf-0.1.4/digrdf/instance_query.sparql
--rw-r--r--   0        0        0      658 2024-05-03 00:07:38.359667 digrdf-0.1.4/digrdf/prefixes.py
--rw-r--r--   0        0        0      289 2024-05-03 05:49:20.734434 digrdf-0.1.4/digrdf/schema_query.sparql
--rw-r--r--   0        0        0      409 2024-05-03 05:50:57.664313 digrdf-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 digrdf-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1143 2024-05-03 05:56:07.796450 digrdf-0.1.5/README.md
+-rw-r--r--   0        0        0       35 2024-05-03 02:30:07.231145 digrdf-0.1.5/digrdf/__init__.py
+-rw-r--r--   0        0        0     5567 2024-05-17 06:40:47.789395 digrdf-0.1.5/digrdf/__main__.py
+-rw-r--r--   0        0        0      101 2024-05-03 05:49:19.197611 digrdf-0.1.5/digrdf/instance_query.sparql
+-rw-r--r--   0        0        0      703 2024-05-15 11:51:48.620609 digrdf-0.1.5/digrdf/prefixes.py
+-rw-r--r--   0        0        0      289 2024-05-03 05:49:20.734434 digrdf-0.1.5/digrdf/schema_query.sparql
+-rw-r--r--   0        0        0      409 2024-05-17 06:55:02.911094 digrdf-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 digrdf-0.1.5/PKG-INFO
```

### Comparing `digrdf-0.1.4/README.md` & `digrdf-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `digrdf-0.1.4/digrdf/__main__.py` & `digrdf-0.1.5/digrdf/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 from pathlib import Path
 from subprocess import check_output
 from urllib.parse import urlparse
 
 import requests
+import networkx as nx
 from pyvis.network import Network
 
 try:
     from .prefixes import prefix_map
 except ImportError:
     from prefixes import prefix_map
 
@@ -36,15 +37,15 @@
     output_dir: Path = Path("./"),
     height: str = "800px",
     return_json: bool = False,
     iri: str | None = None,
 ):
     schema_query_path = Path(__file__).parent / "schema_query.sparql"
     instance_query_path = Path(__file__).parent / "instance_query.sparql"
-    parsed_input_path = urlparse(input_path)
+    parsed_input_path = urlparse(str(input_path))
     # does it look like a url ?
     if not all([parsed_input_path.scheme, parsed_input_path.netloc]):
         # if not, assume its a local dir/file path
         input_path = Path(input_path)
         if input_path.is_dir():
             datastrs = [
                 f"--data={path}" for path in input_path.glob(f"*.{input_format}")
@@ -63,15 +64,15 @@
         # otherwise assume it is a sparql endpoint
         if not (parsed_input_path.path.endswith("sparql") or parsed_input_path.path.endswith("sparql/")):
             raise ValueError(f"{input_path} must be a sparql endpoint ending with 'sparql' or 'sparql/'")
         if iri:
             query_str = instance_query_path.read_text().replace("{}", iri)
         else:
             query_str = schema_query_path.read_text()
-        response = requests.get(input_path, headers={"Accept": "text/csv"}, params={"query": query_str})
+        response = requests.get(str(input_path), headers={"Accept": "text/csv"}, params={"query": query_str})
         query_results = response.content.decode()
     bool_map = {"true": True, "false": False}
     net = Network(
         height=height,
         width="100%",
         neighborhood_highlight=True,
         directed=True,
@@ -80,18 +81,27 @@
     )
     for line in query_results.splitlines()[1:]:
         row = line.split(",")
         prop_label = get_label(row[0])
         is_literal = True if row[2] == "" else bool_map[row[3]]
         domain_label = get_label(row[1])
         range_label = get_label(row[2])
-        net.add_node(domain_label, label=domain_label)
         shape = "box" if is_literal else "dot"
+        net.add_node(domain_label, label=domain_label)
         net.add_node(range_label, label=range_label, shape=shape)
-        net.add_edge(domain_label, range_label, title=prop_label)
+        edges = net.get_edges()
+        duplicate_edge = False
+        for edge in edges:
+            if edge['from'] == domain_label and edge['to'] == range_label:
+                duplicate_edge = True
+                edge['title'] += f"\n{prop_label}"
+                edge['width'] += .2
+        if not duplicate_edge:
+            net.add_edge(domain_label, range_label, title=prop_label, physics=False, width=1)
+    net.set_edge_smooth('cubicBezier')
     if return_json:
         print(net.to_json())
     else:
         net.show(str(output_dir / "diagram.html"), notebook=False)
 
 
 if __name__ == "__main__":
@@ -146,15 +156,15 @@
         "-s",
         "--subject",
         action="store",
         type=str,
         required=False,
         dest="iri",
         default=None,
-        help="IRI of subject to generate a graph for."
+        help="IRI of subject to generate a graph for. Do not include surrounding <> tags."
     )
     args = parser.parse_args()
     input_path = args.input_path
     input_format = args.format
     output_dir = Path(args.output_dir)
     height = str(args.height) + "px"
     return_json = args.return_json
```

### Comparing `digrdf-0.1.4/digrdf/prefixes.py` & `digrdf-0.1.5/digrdf/prefixes.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,9 @@
     "http://schema.org/": "sdo",
     "https://schema.org/": "sdo",
     "http://www.ontoweb.org/ontology/1#": "ow",
     "http://www.w3.org/2006/time#": "time",
     "http://www.opengis.net/ont/geosparql#": "geo",
     "http://www.w3.org/ns/dcat#": "dcat",
     "http://www.w3.org/2002/07/owl#": "owl",
+    "http://purl.org/ontology/bibo/": "bibo"
 }
```

### Comparing `digrdf-0.1.4/PKG-INFO` & `digrdf-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digrdf
-Version: 0.1.4
+Version: 0.1.5
 Summary: RDF Schema Diagram creation tool
 Author: Lawson Lewis
 Author-email: lawson@kurrawong.ai
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

