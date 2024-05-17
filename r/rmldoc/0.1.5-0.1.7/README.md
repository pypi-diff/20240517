# Comparing `tmp/rmldoc-0.1.5.tar.gz` & `tmp/rmldoc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rmldoc-0.1.5.tar", last modified: Fri Mar  8 15:46:26 2024, max compression
+gzip compressed data, was "rmldoc-0.1.7.tar", last modified: Fri May 17 09:27:09 2024, max compression
```

## Comparing `rmldoc-0.1.5.tar` & `rmldoc-0.1.7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:46:26.001834 rmldoc-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-08 15:46:15.000000 rmldoc-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-08 15:46:26.001834 rmldoc-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-03-08 15:46:15.000000 rmldoc-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 15:46:26.001834 rmldoc-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-03-08 15:46:15.000000 rmldoc-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:46:25.997835 rmldoc-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:46:25.997835 rmldoc-0.1.5/src/Templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/Templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:46:25.997835 rmldoc-0.1.5/src/rmldoc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:46:26.001834 rmldoc-0.1.5/src/rmldoc/Templates/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/TriplesMap.md
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/base.md
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/diagram.md
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/function.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/predicate_object.md
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/rmd.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/source.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/Templates/subject.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-08 15:46:15.000000 rmldoc-0.1.5/src/rmldoc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:46:26.001834 rmldoc-0.1.5/src/rmldoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-08 15:46:25.000000 rmldoc-0.1.5/src/rmldoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-08 15:46:25.000000 rmldoc-0.1.5/src/rmldoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 15:46:25.000000 rmldoc-0.1.5/src/rmldoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-08 15:46:25.000000 rmldoc-0.1.5/src/rmldoc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 15:46:25.000000 rmldoc-0.1.5/src/rmldoc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-08 15:46:25.000000 rmldoc-0.1.5/src/rmldoc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-08 15:46:25.000000 rmldoc-0.1.5/src/rmldoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:27:09.102901 rmldoc-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 09:26:58.000000 rmldoc-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-17 09:27:09.102901 rmldoc-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-17 09:26:58.000000 rmldoc-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:27:09.102901 rmldoc-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-17 09:26:58.000000 rmldoc-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:27:09.098901 rmldoc-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:27:09.098901 rmldoc-0.1.7/src/Templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/Templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:27:09.098901 rmldoc-0.1.7/src/rmldoc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:27:09.102901 rmldoc-0.1.7/src/rmldoc/Templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/TriplesMap.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/base.md
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/diagram.md
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/function.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/named_graph.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/predicate_object.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/rmd.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/source.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/Templates/subject.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 09:26:58.000000 rmldoc-0.1.7/src/rmldoc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:27:09.102901 rmldoc-0.1.7/src/rmldoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-17 09:27:09.000000 rmldoc-0.1.7/src/rmldoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 09:27:09.000000 rmldoc-0.1.7/src/rmldoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:27:09.000000 rmldoc-0.1.7/src/rmldoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 09:27:09.000000 rmldoc-0.1.7/src/rmldoc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:27:09.000000 rmldoc-0.1.7/src/rmldoc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-17 09:27:09.000000 rmldoc-0.1.7/src/rmldoc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 09:27:09.000000 rmldoc-0.1.7/src/rmldoc.egg-info/top_level.txt
```

### Comparing `rmldoc-0.1.5/LICENSE` & `rmldoc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/PKG-INFO` & `rmldoc-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmldoc
-Version: 0.1.5
+Version: 0.1.7
 Summary: Rmldoc is a tool that generates documentation of RML mappings
 Home-page: https://github.com/oeg-upm/rmldoc
 Author: Jhon Toledo
 Author-email: ja.toledo@upm.es
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdflib>=6.0.2
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: yatter>=1.1.2
 
-[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![License](https://camo.githubusercontent.com/db9dfde8049c5d66ba62fde707d2cfb30e26f9f26ff274c3442c0aec1ec410a4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d417061636865253230322e302d626c75652e737667)](https://github.com/oeg-upm/Mapeathor/blob/master/LICENSE) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10732487.svg)](https://doi.org/10.5281/zenodo.10732487)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![License](https://camo.githubusercontent.com/db9dfde8049c5d66ba62fde707d2cfb30e26f9f26ff274c3442c0aec1ec410a4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d417061636865253230322e302d626c75652e737667)](https://github.com/oeg-upm/Mapeathor/blob/master/LICENSE) ![DOI: 10.5281/zenodo.10797980](https://zenodo.org/badge/DOI/10.5281/zenodo.10797980.svg)
 
 # RMLdoc
 
 RMLdoc is a tool designed to simplify the process of generating documentation of mappings used for knowledge graph construction. It automates the documentation generation process, allowing users to easily understand the mapping transformation rules defined within their projects. Given an input mapping file written in R2RML, RML, or YARRRML, RMLdoc will generate a detailed Markdown documentation explaining each mapping with corresponding diagrams, in a human readable manner.
 
 ## Features
```

### Comparing `rmldoc-0.1.5/README.md` & `rmldoc-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![License](https://camo.githubusercontent.com/db9dfde8049c5d66ba62fde707d2cfb30e26f9f26ff274c3442c0aec1ec410a4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d417061636865253230322e302d626c75652e737667)](https://github.com/oeg-upm/Mapeathor/blob/master/LICENSE) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10732487.svg)](https://doi.org/10.5281/zenodo.10732487)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![License](https://camo.githubusercontent.com/db9dfde8049c5d66ba62fde707d2cfb30e26f9f26ff274c3442c0aec1ec410a4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d417061636865253230322e302d626c75652e737667)](https://github.com/oeg-upm/Mapeathor/blob/master/LICENSE) ![DOI: 10.5281/zenodo.10797980](https://zenodo.org/badge/DOI/10.5281/zenodo.10797980.svg)
 
 # RMLdoc
 
 RMLdoc is a tool designed to simplify the process of generating documentation of mappings used for knowledge graph construction. It automates the documentation generation process, allowing users to easily understand the mapping transformation rules defined within their projects. Given an input mapping file written in R2RML, RML, or YARRRML, RMLdoc will generate a detailed Markdown documentation explaining each mapping with corresponding diagrams, in a human readable manner.
 
 ## Features
```

### Comparing `rmldoc-0.1.5/setup.py` & `rmldoc-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     items = find_paths(dirname)
     return [os.path.relpath(path, dirname) for path in items]
 
 
 setup(
     name="rmldoc",
-    version="0.1.5",
+    version="0.1.7",
     author="Jhon Toledo",
     author_email="ja.toledo@upm.es",
     description="Rmldoc is a tool that generates documentation of RML mappings",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/oeg-upm/rmldoc",
     classifiers=[
```

### Comparing `rmldoc-0.1.5/src/Templates/__init__.py` & `rmldoc-0.1.7/src/Templates/__init__.py`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/src/rmldoc/Templates/__init__.py` & `rmldoc-0.1.7/src/rmldoc/Templates/__init__.py`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/src/rmldoc/Templates/base.md` & `rmldoc-0.1.7/src/rmldoc/Templates/base.md`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/src/rmldoc/Templates/rmd.md` & `rmldoc-0.1.7/src/rmldoc/Templates/rmd.md`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/src/rmldoc/__init__.py` & `rmldoc-0.1.7/src/rmldoc/__init__.py`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/src/rmldoc/__main__.py` & `rmldoc-0.1.7/src/rmldoc/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,14 +112,27 @@
         <""" + triples_map + """> rr:predicateObjectMap/rr:objectMap/rr:joinCondition[rr:child ?child; rr:parent ?parent; ^rr:joinCondition/rr:parentTriplesMap ?parentTriplesMap; ^rr:joinCondition/^rr:objectMap/rr:predicateMap/rr:constant ?predicate; ^rr:joinCondition/^rr:objectMap/^rr:predicateObjectMap/rr:subjectMap/rr:template   ?s_template ].
         ?parentTriplesMap rr:subjectMap/(rr:template|ns0:reference) ?o_template.
     }
     """
     return query
 
 
+def named_graph(triples_map):
+    query = """
+    PREFIX  rr: <http://www.w3.org/ns/r2rml#> 
+    PREFIX  rml: <http://w3id.org/rml/>
+    PREFIX  ns0: <http://semweb.mmlab.be/ns/rml#>
+    SELECT distinct ?graph
+    WHERE {
+        <""" + triples_map + """> rr:subjectMap/rr:graphMap/rr:constant ?graph .
+    }
+     """
+    return query
+
+
 def get_namespaces(g):
     g1 = rdflib.Graph()
     temp1 = g.namespaces()
     temp2 = g1.namespaces()
     return list(set(temp1) - set(temp2))
 
 
@@ -133,14 +146,15 @@
 
     template = environment.get_template("rmd.md")
     source_template = environment.get_template("source.md")
     subject_template = environment.get_template("subject.md")
     pom_template = environment.get_template("predicate_object.md")
     spo_diagram = environment.get_template("diagram.md")
     join_diagram = environment.get_template("function.md")
+    named_graph_template = environment.get_template("named_graph.md")
     # Version
     rml_version = g.query(dataset_version)
 
     rml_version = [{"version": str(vr.version), "license": str(vr.license), "description": str(vr.description),
                     "title": str(vr.title), "dateCreated": str(vr.dateCreated)} for vr in rml_version]
 
     # Prefix
@@ -195,14 +209,19 @@
              "child": str(i.child), "parent": str(i.parent), 'template': str(i.o_template).replace('"', "'"),
              'subject': str(i.s_template).replace('"', "'")} for i in
             g.query(join_condition(tp))]
 
         if join_condition_diagram:
             mapping_content += join_diagram.render(subject=tp.split('/')[-1], join_list=join_condition_diagram)
 
+        # named_graph
+        rml_graph = [{"graph": str(i.graph)} for i in g.query(named_graph(tp))]
+        if rml_graph:
+            mapping_content += named_graph_template.render(graph=rml_graph)
+
     # parse the content
     # content = template.render(authors=rmd_authors, prefixes=rmd_prefixes, mapping_content=mapping_content)
 
     content = template.render(version=rml_version, mapping_file=get_file_name(rdf_mapping_path),
                               authors=rmd_authors,
                               prefixes=rmd_prefixes,
                               mapping_content=mapping_content)
@@ -225,14 +244,15 @@
 
     template = environment.get_template("rmd.md")
     source_template = environment.get_template("source.md")
     subject_template = environment.get_template("subject.md")
     pom_template = environment.get_template("predicate_object.md")
     spo_diagram = environment.get_template("diagram.md")
     join_diagram = environment.get_template("function.md")
+    named_graph_template = environment.get_template("named_graph.md")
     # Version
     rml_version = g.query(dataset_version)
 
     rml_version = [{"version": str(vr.version), "license": str(vr.license), "description": str(vr.description),
                     "title": str(vr.title), "dateCreated": str(vr.dateCreated)} for vr in rml_version]
 
     # Prefix
@@ -287,14 +307,19 @@
              "child": str(i.child), "parent": str(i.parent), 'template': str(i.o_template).replace('"', "'"),
              'subject': str(i.s_template).replace('"', "'")} for i in
             g.query(join_condition(tp))]
 
         if join_condition_diagram:
             mapping_content += join_diagram.render(subject=tp.split('/')[-1], join_list=join_condition_diagram)
 
+        # named_graph
+        rml_graph = [{"graph": str(i.graph)} for i in g.query(named_graph(tp))]
+        if rml_graph:
+            mapping_content += named_graph_template.render(graph=rml_graph)
+
     content = template.render(version=rml_version, mapping_file=get_file_name(rdf_mapping_path),
                               authors=rmd_authors,
                               prefixes=rmd_prefixes,
                               mapping_content=mapping_content)
     # Write results
     write_doc(content, output_path)
 
@@ -307,14 +332,15 @@
                         help="Path to save the generated document. Default output output.md")
     parser.add_argument("-y", "--yatter", action='store_true',
                         help="Enable yatter option to read yarrrml mappings")
     return parser
 
 
 def main():
+
     args = define_args().parse_args()
     log.info("RML Documentation(RMLdoc)")
     log.info(args.input_mapping_path)
     if args.yatter:
         workflow_with_yatter(args.input_mapping_path, args.output_path)
     else:
         workflow(args.input_mapping_path, args.output_path)
```

### Comparing `rmldoc-0.1.5/src/rmldoc/queries.py` & `rmldoc-0.1.7/src/rmldoc/queries.py`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/src/rmldoc/utils.py` & `rmldoc-0.1.7/src/rmldoc/utils.py`

 * *Files identical despite different names*

### Comparing `rmldoc-0.1.5/src/rmldoc.egg-info/PKG-INFO` & `rmldoc-0.1.7/src/rmldoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rmldoc
-Version: 0.1.5
+Version: 0.1.7
 Summary: Rmldoc is a tool that generates documentation of RML mappings
 Home-page: https://github.com/oeg-upm/rmldoc
 Author: Jhon Toledo
 Author-email: ja.toledo@upm.es
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
@@ -14,15 +14,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rdflib>=6.0.2
 Requires-Dist: Jinja2>=3.1.2
 Requires-Dist: yatter>=1.1.2
 
-[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![License](https://camo.githubusercontent.com/db9dfde8049c5d66ba62fde707d2cfb30e26f9f26ff274c3442c0aec1ec410a4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d417061636865253230322e302d626c75652e737667)](https://github.com/oeg-upm/Mapeathor/blob/master/LICENSE) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10732487.svg)](https://doi.org/10.5281/zenodo.10732487)
+[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active) [![License](https://camo.githubusercontent.com/db9dfde8049c5d66ba62fde707d2cfb30e26f9f26ff274c3442c0aec1ec410a4/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f4c6963656e73652d417061636865253230322e302d626c75652e737667)](https://github.com/oeg-upm/Mapeathor/blob/master/LICENSE) ![DOI: 10.5281/zenodo.10797980](https://zenodo.org/badge/DOI/10.5281/zenodo.10797980.svg)
 
 # RMLdoc
 
 RMLdoc is a tool designed to simplify the process of generating documentation of mappings used for knowledge graph construction. It automates the documentation generation process, allowing users to easily understand the mapping transformation rules defined within their projects. Given an input mapping file written in R2RML, RML, or YARRRML, RMLdoc will generate a detailed Markdown documentation explaining each mapping with corresponding diagrams, in a human readable manner.
 
 ## Features
```

### Comparing `rmldoc-0.1.5/src/rmldoc.egg-info/SOURCES.txt` & `rmldoc-0.1.7/src/rmldoc.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 src/rmldoc.egg-info/requires.txt
 src/rmldoc.egg-info/top_level.txt
 src/rmldoc/Templates/TriplesMap.md
 src/rmldoc/Templates/__init__.py
 src/rmldoc/Templates/base.md
 src/rmldoc/Templates/diagram.md
 src/rmldoc/Templates/function.md
+src/rmldoc/Templates/named_graph.md
 src/rmldoc/Templates/predicate_object.md
 src/rmldoc/Templates/rmd.md
 src/rmldoc/Templates/source.md
 src/rmldoc/Templates/subject.md
```

