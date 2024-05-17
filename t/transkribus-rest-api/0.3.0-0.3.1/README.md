# Comparing `tmp/transkribus_rest_api-0.3.0.tar.gz` & `tmp/transkribus_rest_api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transkribus_rest_api-0.3.0.tar", last modified: Thu Apr 25 14:52:43 2024, max compression
+gzip compressed data, was "transkribus_rest_api-0.3.1.tar", last modified: Fri May 17 08:13:49 2024, max compression
```

## Comparing `transkribus_rest_api-0.3.0.tar` & `transkribus_rest_api-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/transkribus_rest_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-25 14:52:32.000000 transkribus_rest_api-0.3.0/transkribus_rest_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:52:43.769941 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-25 14:52:43.000000 transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:13:49.325691 transkribus_rest_api-0.3.1/transkribus_rest_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-17 08:13:35.000000 transkribus_rest_api-0.3.1/transkribus_rest_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:13:49.329691 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-17 08:13:49.000000 transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/top_level.txt
```

### Comparing `transkribus_rest_api-0.3.0/LICENSE` & `transkribus_rest_api-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.3.0/PKG-INFO` & `transkribus_rest_api-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transkribus_rest_api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Transkribus Metagrapho API Client.
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/transkribus_rest_api
 Project-URL: Bug Tracker, http://github.com/jnphilipp/transkribus_rest_api/issues
 Keywords: transkribus,api
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `transkribus_rest_api-0.3.0/pyproject.toml` & `transkribus_rest_api-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "transkribus_rest_api"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     {name = "J. Nathanael Philipp", email = "nathanael@philipp.land"}
 ]
 description="Transkribus Metagrapho API Client."
 readme = "README.md"
 license = {text = "GPLv3+"}
 requires-python = ">=3.10"
```

### Comparing `transkribus_rest_api-0.3.0/transkribus_rest_api/__init__.py` & `transkribus_rest_api-0.3.1/transkribus_rest_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 __all__ = ["TranskribusRestApi", "transkribus_rest_api"]
 
 __app_name__ = "transkribus-rest-api"
 __author__ = "J. Nathanael Philipp"
 __email__ = "nathanael@philipp.land"
 __copyright__ = "Copyright 2024 J. Nathanael Philipp (jnphilipp)"
 __license__ = "GPLv3"
-__version_info__ = (0, 3, 0)
+__version_info__ = (0, 3, 1)
 __version__ = ".".join(str(e) for e in __version_info__)
 __github__ = "https://github.com/jnphilipp/transkribus-rest-api"
 VERSION = (
     f"%(prog)s v{__version__}\n{__copyright__}\n"
     + "License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>."
     + "\nThis is free software: you are free to change and redistribute it.\n"
     + "There is NO WARRANTY, to the extent permitted by law.\n\n"
```

### Comparing `transkribus_rest_api-0.3.0/transkribus_rest_api/api.py` & `transkribus_rest_api-0.3.1/transkribus_rest_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,15 +380,15 @@
 
     def upload_document(
         self,
         collection_id: int,
         title: str,
         pages: list[UploadPage],
         metadata: dict = {},
-    ):
+    ) -> int:
         """Upload a document.
 
         Args:
          * collection_id: collection to upload document to
          * title: title of the document
          * pages: pages to upload
          * metadata: extra metadata for the document
@@ -415,14 +415,15 @@
         }
 
         doc = self.uploads.create_upload_doc_structure(collection_id, data)
         upload_id = int(doc.xpath("//uploadId/text()")[0])
 
         for page in pages:
             self.uploads.upload_page(upload_id, page.image, page.page_xml)
+        return int(doc.xpath("//docId/text()")[0])
 
     def download_document(
         self,
         collection_id: int,
         document_id: int,
         target: str | Path,
     ) -> None:
@@ -444,27 +445,37 @@
                     "ns2": "http://www.w3.org/1999/xlink",
                     "ns3": "http://www.loc.gov/METS/",
                 },
             )
         ):
             e.attrib["LOCTYPE"] = "OTHER"
             e.attrib["OTHERLOCTYPE"] = "FILE"
-            e.attrib["{http://www.w3.org/1999/xlink}href"] = pages[1]["tsList"][
+            e.attrib["{http://www.w3.org/1999/xlink}href"] = pages[i]["tsList"][
                 "transcripts"
             ][0]["fileName"]
 
+        etree.indent(mets, space=" " * 4)
         with open(target / "mets.xml", "wb") as f:
             f.write(etree.tostring(mets, xml_declaration=True, pretty_print=True))
 
         for page in pages:
             doc = self.collections.get_transcript(
                 collection_id, document_id, page["pageNr"]
             )
+            etree.indent(doc, space=" " * 4)
             with open(target / page["tsList"]["transcripts"][0]["fileName"], "wb") as f:
-                f.write(etree.tostring(doc, xml_declaration=True, pretty_print=True))
+                f.write(
+                    etree.tostring(
+                        doc,
+                        encoding="utf-8",
+                        xml_declaration=True,
+                        pretty_print=True,
+                        standalone=True,
+                    )
+                )
 
 
 @contextmanager
 def transkribus_rest_api(username: str, password: str) -> Generator:
     """Context manager for Transkribus rest API.
 
     Args:
```

### Comparing `transkribus_rest_api-0.3.0/transkribus_rest_api/types.py` & `transkribus_rest_api-0.3.1/transkribus_rest_api/types.py`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.3.0/transkribus_rest_api/utils.py` & `transkribus_rest_api-0.3.1/transkribus_rest_api/utils.py`

 * *Files identical despite different names*

### Comparing `transkribus_rest_api-0.3.0/transkribus_rest_api.egg-info/PKG-INFO` & `transkribus_rest_api-0.3.1/transkribus_rest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transkribus_rest_api
-Version: 0.3.0
+Version: 0.3.1
 Summary: Transkribus Metagrapho API Client.
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/transkribus_rest_api
 Project-URL: Bug Tracker, http://github.com/jnphilipp/transkribus_rest_api/issues
 Keywords: transkribus,api
 Classifier: Development Status :: 5 - Production/Stable
```

