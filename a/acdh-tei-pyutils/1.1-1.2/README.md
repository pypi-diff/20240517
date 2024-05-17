# Comparing `tmp/acdh-tei-pyutils-1.1.tar.gz` & `tmp/acdh-tei-pyutils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh-tei-pyutils-1.1.tar", last modified: Sun Jan 28 07:53:39 2024, max compression
+gzip compressed data, was "acdh-tei-pyutils-1.2.tar", last modified: Fri May 17 13:15:59 2024, max compression
```

## Comparing `acdh-tei-pyutils-1.1.tar` & `acdh-tei-pyutils-1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:53:39.262895 acdh-tei-pyutils-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-01-28 07:53:39.262895 acdh-tei-pyutils-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:53:39.258895 acdh-tei-pyutils-1.1/acdh_tei_pyutils/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16801 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:53:39.262895 acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/clean_markup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei_no_id.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei_no_ids.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei_trailing_slash.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/tei.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:53:39.262895 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-01-28 07:53:39.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-28 07:53:39.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 07:53:39.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-01-28 07:53:39.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-28 07:53:39.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-28 07:53:39.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-28 07:53:39.000000 acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-28 07:53:39.262895 acdh-tei-pyutils-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-28 07:53:39.262895 acdh-tei-pyutils-1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-01-28 07:53:17.000000 acdh-tei-pyutils-1.1/tests/test_tei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.090220 acdh-tei-pyutils-1.2/acdh_tei_pyutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16811 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/clean_markup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_id.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_ids.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_trailing_slash.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/tei.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 13:15:59.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 13:15:58.000000 acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:15:59.094220 acdh-tei-pyutils-1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-05-17 13:15:42.000000 acdh-tei-pyutils-1.2/tests/test_tei.py
```

### Comparing `acdh-tei-pyutils-1.1/LICENSE` & `acdh-tei-pyutils-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.1/PKG-INFO` & `acdh-tei-pyutils-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-tei-pyutils
-Version: 1.1
+Version: 1.2
 Summary: Utilty functions to work with TEI Documents
 Home-page: https://github.com/acdh-oeaw/acdh-tei-pyutils
 Author: Peter Andorfer, Daniel Stoxreiter
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Keywords: acdh-tei-pyutils
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,45 +18,47 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # acdh-tei-pyutils
 
 [![Github Workflow Tests Status](https://github.com/acdh-oeaw/acdh-tei-pyutils/workflows/Test/badge.svg)](https://github.com/acdh-oeaw/acdh-tei-pyutils/workflows/Test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/acdh-tei-pyutils.svg)](https://badge.fury.io/py/acdh-tei-pyutils)
-[![codecov](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils/branch/master/graph/badge.svg?token=y6HUg72XnH)](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils)
+[![codecov](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils/branch/main/graph/badge.svg?token=y6HUg72XnH)](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils)
 
 Utilty functions to work with TEI Documents
 
 ## install
 
 run `pip install acdh-tei-pyutils`
 
 ## usage
 
-parse an XML/TEI Document from and URL, string or file:
+some examples on how to use this package
+
+### parse an XML/TEI Document from and URL, string or file:
 
 ```python
 from acdh_tei_pyutils.tei import TeiReader
 
-doc = TeiReader("https://raw.githubusercontent.com/acdh-oeaw/acdh-tei-pyutils/master/acdh_tei_pyutils/files/tei.xml")
+doc = TeiReader("https://raw.githubusercontent.com/acdh-oeaw/acdh-tei-pyutils/main/acdh_tei_pyutils/files/tei.xml")
 print(doc.tree)
 >>> <Element {http://www.tei-c.org/ns/1.0}TEI at 0x7ffb926f9c40>
 
 doc = TeiReader("./acdh_tei_pyutils/files/tei.xml")
 doc.tree
 >>> <Element {http://www.tei-c.org/ns/1.0}TEI at 0x7ffb926f9c40>
 ```
 
-write the current XML/TEI tree object to file
+### write the current XML/TEI tree object to file
 ```python
 doc.tree_to_file("out.xml")
 >>> 'out.xml'
 ```
 
-see [acdh_tei_pyutils/cli.py](https://github.com/acdh-oeaw/acdh-tei-pyutils/blob/master/acdh_tei_pyutils/cli.py) for further examples
+see [acdh_tei_pyutils/cli.py](https://github.com/acdh-oeaw/acdh-tei-pyutils/blob/main/acdh_tei_pyutils/cli.py) for further examples
 
 ### command line scripts
 
 Batch process a collection of XML/Documents by adding xml:id, xml:base next and prev attributes to the documents root element run:
 
 ```bash
 add-attributes -g "/path/to/your/xmls/*.xml" -b "https://value/of-your/base.com"
```

### Comparing `acdh-tei-pyutils-1.1/README.md` & `acdh-tei-pyutils-1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # acdh-tei-pyutils
 
 [![Github Workflow Tests Status](https://github.com/acdh-oeaw/acdh-tei-pyutils/workflows/Test/badge.svg)](https://github.com/acdh-oeaw/acdh-tei-pyutils/workflows/Test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/acdh-tei-pyutils.svg)](https://badge.fury.io/py/acdh-tei-pyutils)
-[![codecov](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils/branch/master/graph/badge.svg?token=y6HUg72XnH)](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils)
+[![codecov](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils/branch/main/graph/badge.svg?token=y6HUg72XnH)](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils)
 
 Utilty functions to work with TEI Documents
 
 ## install
 
 run `pip install acdh-tei-pyutils`
 
 ## usage
 
-parse an XML/TEI Document from and URL, string or file:
+some examples on how to use this package
+
+### parse an XML/TEI Document from and URL, string or file:
 
 ```python
 from acdh_tei_pyutils.tei import TeiReader
 
-doc = TeiReader("https://raw.githubusercontent.com/acdh-oeaw/acdh-tei-pyutils/master/acdh_tei_pyutils/files/tei.xml")
+doc = TeiReader("https://raw.githubusercontent.com/acdh-oeaw/acdh-tei-pyutils/main/acdh_tei_pyutils/files/tei.xml")
 print(doc.tree)
 >>> <Element {http://www.tei-c.org/ns/1.0}TEI at 0x7ffb926f9c40>
 
 doc = TeiReader("./acdh_tei_pyutils/files/tei.xml")
 doc.tree
 >>> <Element {http://www.tei-c.org/ns/1.0}TEI at 0x7ffb926f9c40>
 ```
 
-write the current XML/TEI tree object to file
+### write the current XML/TEI tree object to file
 ```python
 doc.tree_to_file("out.xml")
 >>> 'out.xml'
 ```
 
-see [acdh_tei_pyutils/cli.py](https://github.com/acdh-oeaw/acdh-tei-pyutils/blob/master/acdh_tei_pyutils/cli.py) for further examples
+see [acdh_tei_pyutils/cli.py](https://github.com/acdh-oeaw/acdh-tei-pyutils/blob/main/acdh_tei_pyutils/cli.py) for further examples
 
 ### command line scripts
 
 Batch process a collection of XML/Documents by adding xml:id, xml:base next and prev attributes to the documents root element run:
 
 ```bash
 add-attributes -g "/path/to/your/xmls/*.xml" -b "https://value/of-your/base.com"
```

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/cli.py` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,29 +218,29 @@
         doc_base = doc.any_xpath("./@xml:base")[0]
         doc_id = doc.any_xpath("./@xml:id")[0]
         doc_uri = f"{doc_base}/{doc_id}"
         try:
             doc_title = doc.any_xpath(title_xpath)[0]
         except IndexError:
             doc_title = f"ERROR in title xpath of file: {doc_id}"
-            print(f"ERROR in title xpath of file: {doc_id}")
+            print(f"ERROR in -x title xpath of file: {doc_id}")
         if title_sec_xpath:
             try:
                 doc_title_sec = doc.any_xpath(title_sec_xpath)[0]
             except IndexError:
-                doc_title_sec = f"ERROR in secondary title xpath of file: {doc_id}"
+                doc_title_sec = f"ERROR in -xs secondary title xpath of file: {doc_id}"
                 print(f"ERROR in secondary title xpath of file: {doc_id}")
         else:
             doc_title_sec = None
         if date_xpath:
             try:
                 doc_date = doc.any_xpath(date_xpath)[0]
             except IndexError:
                 doc_date = f"ERROR in date xpath of file: {doc_id}"
-                print(f"ERROR in date xpath of file: {doc_id}")
+                print(f"ERROR in -d date xpath of file: {doc_id}")
         else:
             doc_date = None
         refs = doc.any_xpath(mention_xpath)
         for ref in set(refs):
             if ref.startswith("#") and len(ref.split(" ")) == 1:
                 ref = ref[1:]
             if ref.startswith("#") and len(ref.split(" ")) > 1:
```

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/clean_markup.xsl` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/clean_markup.xsl`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei.xml` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei_no_id.xml` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_id.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei_no_ids.xml` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_no_ids.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/files/tei_trailing_slash.xml` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/files/tei_trailing_slash.xml`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/tei.py` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/tei.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from lxml import etree as ET
 import re
 from acdh_xml_pyutils.xml import XMLReader
+from slugify import slugify
 
 
 class HandleAlreadyExist(Exception):
     pass
 
 
 NER_TAG_MAP = {
@@ -250,19 +251,24 @@
         :param mentions: a list of dicts with keys `doc_id` and `doc_title`
         :type mentions: noteGrp
 
         :return: a etree.element
         """
         tei_ns = f"{self.ns_tei['tei']}"
         node_root = ET.Element(f"{{{tei_ns}}}noteGrp")
+        mentions_added = {}
         for x in mentions:
-            note = ET.Element(f"{{{tei_ns}}}note")
-            note.attrib["target"] = x["doc_id"]
-            note.attrib["type"] = "mentions"
-            if x["doc_date"] is not None:
-                note.attrib["corresp"] = x["doc_date"]
-            if x["doc_title_sec"] is not None:
-                note.text = f"{x['doc_title']} {x['doc_title_sec']}"
-            else:
-                note.text = x["doc_title"]
-            node_root.append(note)
+            try:
+                mentions_added[slugify(x['doc_id'])]
+            except KeyError:
+                note = ET.Element(f"{{{tei_ns}}}note")
+                note.attrib['target'] = x['doc_id']
+                note.attrib['type'] = "mentions"
+                if x['doc_date'] is not None:
+                    note.attrib['corresp'] = x['doc_date']
+                if x['doc_title_sec'] is not None:
+                    note.text = f"{x['doc_title']} {x['doc_title_sec']}"
+                else:
+                    note.text = x['doc_title']
+                node_root.append(note)
+                mentions_added[slugify(x['doc_id'])] = True
         return node_root
```

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils/utils.py` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     prevs, items, nexts = tee(some_iterable, 3)
     prevs = chain([None], prevs)
     nexts = chain(islice(nexts, 1, None), [None])
     return zip(prevs, items, nexts)
 
 
 def normalize_string(string: str) -> str:
+    """ removese any superfluos whitespace from a given string"""
     return " ".join(" ".join(string.split()).split())
 
 
 def make_entity_label(
     name_node: ET.Element, default_msg="no label provided", default_lang="en"
 ) -> tuple[str, str]:
     """extracts labels from tei:persName|placeName|orgName"""
```

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/PKG-INFO` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-tei-pyutils
-Version: 1.1
+Version: 1.2
 Summary: Utilty functions to work with TEI Documents
 Home-page: https://github.com/acdh-oeaw/acdh-tei-pyutils
 Author: Peter Andorfer, Daniel Stoxreiter
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Keywords: acdh-tei-pyutils
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -18,45 +18,47 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # acdh-tei-pyutils
 
 [![Github Workflow Tests Status](https://github.com/acdh-oeaw/acdh-tei-pyutils/workflows/Test/badge.svg)](https://github.com/acdh-oeaw/acdh-tei-pyutils/workflows/Test/badge.svg)
 [![PyPI version](https://badge.fury.io/py/acdh-tei-pyutils.svg)](https://badge.fury.io/py/acdh-tei-pyutils)
-[![codecov](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils/branch/master/graph/badge.svg?token=y6HUg72XnH)](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils)
+[![codecov](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils/branch/main/graph/badge.svg?token=y6HUg72XnH)](https://codecov.io/gh/acdh-oeaw/acdh-tei-pyutils)
 
 Utilty functions to work with TEI Documents
 
 ## install
 
 run `pip install acdh-tei-pyutils`
 
 ## usage
 
-parse an XML/TEI Document from and URL, string or file:
+some examples on how to use this package
+
+### parse an XML/TEI Document from and URL, string or file:
 
 ```python
 from acdh_tei_pyutils.tei import TeiReader
 
-doc = TeiReader("https://raw.githubusercontent.com/acdh-oeaw/acdh-tei-pyutils/master/acdh_tei_pyutils/files/tei.xml")
+doc = TeiReader("https://raw.githubusercontent.com/acdh-oeaw/acdh-tei-pyutils/main/acdh_tei_pyutils/files/tei.xml")
 print(doc.tree)
 >>> <Element {http://www.tei-c.org/ns/1.0}TEI at 0x7ffb926f9c40>
 
 doc = TeiReader("./acdh_tei_pyutils/files/tei.xml")
 doc.tree
 >>> <Element {http://www.tei-c.org/ns/1.0}TEI at 0x7ffb926f9c40>
 ```
 
-write the current XML/TEI tree object to file
+### write the current XML/TEI tree object to file
 ```python
 doc.tree_to_file("out.xml")
 >>> 'out.xml'
 ```
 
-see [acdh_tei_pyutils/cli.py](https://github.com/acdh-oeaw/acdh-tei-pyutils/blob/master/acdh_tei_pyutils/cli.py) for further examples
+see [acdh_tei_pyutils/cli.py](https://github.com/acdh-oeaw/acdh-tei-pyutils/blob/main/acdh_tei_pyutils/cli.py) for further examples
 
 ### command line scripts
 
 Batch process a collection of XML/Documents by adding xml:id, xml:base next and prev attributes to the documents root element run:
 
 ```bash
 add-attributes -g "/path/to/your/xmls/*.xml" -b "https://value/of-your/base.com"
```

### Comparing `acdh-tei-pyutils-1.1/acdh_tei_pyutils.egg-info/SOURCES.txt` & `acdh-tei-pyutils-1.2/acdh_tei_pyutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acdh-tei-pyutils-1.1/setup.py` & `acdh-tei-pyutils-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     package_data={
         module.__name__: walker(os.path.dirname(module.__file__), "files"),
     },
     setup_requires=dev_requirements,
     test_suite="tests",
     tests_require=dev_requirements,
     url="https://github.com/acdh-oeaw/acdh-tei-pyutils",
-    version="v1.1",
+    version="v1.2",
     zip_safe=False,
 )
```

### Comparing `acdh-tei-pyutils-1.1/tests/test_tei.py` & `acdh-tei-pyutils-1.2/tests/test_tei.py`

 * *Files identical despite different names*

