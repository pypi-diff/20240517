# Comparing `tmp/fizzysearch-0.2.tar.gz` & `tmp/fizzysearch-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fizzysearch-0.2.tar", max compression
+gzip compressed data, was "fizzysearch-0.3.tar", max compression
```

## Comparing `fizzysearch-0.2.tar` & `fizzysearch-0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1152 2024-02-29 13:36:33.804542 fizzysearch-0.2/LICENSE
--rw-r--r--   0        0        0     1959 2024-03-27 15:37:51.706422 fizzysearch-0.2/README.md
--rw-r--r--   0        0        0     3006 2024-03-27 15:38:23.013527 fizzysearch-0.2/fizzysearch.py
--rw-r--r--   0        0        0      304 2024-03-27 15:38:23.014054 fizzysearch-0.2/pyproject.toml
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 fizzysearch-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1152 2024-02-29 13:36:33.804542 fizzysearch-0.3/LICENSE
+-rw-r--r--   0        0        0     1959 2024-05-17 02:53:44.403985 fizzysearch-0.3/README.md
+-rw-r--r--   0        0        0     3063 2024-05-17 21:53:37.774091 fizzysearch-0.3/fizzysearch.py
+-rw-r--r--   0        0        0      304 2024-05-17 21:54:10.410300 fizzysearch-0.3/pyproject.toml
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 fizzysearch-0.3/PKG-INFO
```

### Comparing `fizzysearch-0.2/LICENSE` & `fizzysearch-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fizzysearch-0.2/README.md` & `fizzysearch-0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # FIZzysearch
 
 ## A SPARQL rewriter that performs enhanced searches
 
 This is an extension of the work that was started at the [2023 HackaLOD](https://github.com/ISE-FIZKarlsruhe/hackaLOD23) event in Gouda.
 The package provides a SPARQL rewriting framework which can be used to implement different enhanced search facilities like full-text searches or embeddings based searches. The re-writing can be used as a "front-end" to existing SPARQL endpoints, or integrated as a software library.
-One of the benefits are enabling easier searches for existing triplestires in which it might be cumbersome to install or configure enhanced search facilities.
+One of the benefits are enabling easier searches for existing triplestores in which it might be cumbersome to install or configure enhanced search facilities.
 
 ✨ This library gives you ["fizzy"](https://en.wiktionary.org/wiki/fizzy) searches! ✨
 
 (and it was made by the [FIZ ISE](https://www.fiz-karlsruhe.de/en/forschung/information-service-engineering) group)
 
 ## Example
 
@@ -28,10 +28,10 @@
 }
 ```
 
 This demo is from [SHMARQL](https://github.com/epoz/shmarql) which uses FIZzysearch to add fulltext searches to the triplestore.
 
 ## TODO
 
-- [ ] Add a sample FTS implementation as demo
+- [x] Add a sample FTS implementation as demo
 
 - [ ] Add documentation on how to build the dependencies and where to fetch the SPARQL grammar
```

### Comparing `fizzysearch-0.2/fizzysearch.py` & `fizzysearch-0.3/fizzysearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,17 @@
     start_byte = end_byte = 0
     var_name = q_object = None
     predicate = None
     for n, name in q.captures(tree.root_node):
         if name == "tss":
             if start_byte > 0 and end_byte > start_byte:
                 if var_name is not None and q_object is not None and found:
-                    found_vars.append((start_byte, end_byte, var_name, q_object))
+                    found_vars.append(
+                        (start_byte, end_byte, var_name, q_object, predicate)
+                    )
             start_byte = n.start_byte
             end_byte = n.end_byte
             var_name = q_object = None
             found = False
         if name in ("q_object_literal", "q_object_iri"):
             q_object = n.text.decode("utf8")
         if name == "predicate" and n.text.decode("utf8") in PREDICATE_MAP:
```

### Comparing `fizzysearch-0.2/PKG-INFO` & `fizzysearch-0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fizzysearch
-Version: 0.2
+Version: 0.3
 Summary: A SPARQL rewriter that performs enhanced searches
 Home-page: https://github.com/ISE-FIZKarlsruhe/fizzysearch
 License: MIT
 Author: Etienne Posthumus
 Author-email: ep@epoz.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 
 # FIZzysearch
 
 ## A SPARQL rewriter that performs enhanced searches
 
 This is an extension of the work that was started at the [2023 HackaLOD](https://github.com/ISE-FIZKarlsruhe/hackaLOD23) event in Gouda.
 The package provides a SPARQL rewriting framework which can be used to implement different enhanced search facilities like full-text searches or embeddings based searches. The re-writing can be used as a "front-end" to existing SPARQL endpoints, or integrated as a software library.
-One of the benefits are enabling easier searches for existing triplestires in which it might be cumbersome to install or configure enhanced search facilities.
+One of the benefits are enabling easier searches for existing triplestores in which it might be cumbersome to install or configure enhanced search facilities.
 
 ✨ This library gives you ["fizzy"](https://en.wiktionary.org/wiki/fizzy) searches! ✨
 
 (and it was made by the [FIZ ISE](https://www.fiz-karlsruhe.de/en/forschung/information-service-engineering) group)
 
 ## Example
 
@@ -47,11 +47,11 @@
 }
 ```
 
 This demo is from [SHMARQL](https://github.com/epoz/shmarql) which uses FIZzysearch to add fulltext searches to the triplestore.
 
 ## TODO
 
-- [ ] Add a sample FTS implementation as demo
+- [x] Add a sample FTS implementation as demo
 
 - [ ] Add documentation on how to build the dependencies and where to fetch the SPARQL grammar
```

