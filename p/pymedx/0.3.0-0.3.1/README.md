# Comparing `tmp/pymedx-0.3.0.tar.gz` & `tmp/pymedx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymedx-0.3.0.tar", max compression
+gzip compressed data, was "pymedx-0.3.1.tar", max compression
```

## Comparing `pymedx-0.3.0.tar` & `pymedx-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1925 2024-02-09 16:58:49.917217 pymedx-0.3.0/docs/index.md
--rw-r--r--   0        0        0     1909 2024-02-09 17:00:10.381749 pymedx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      496 2024-02-09 17:00:10.377750 pymedx-0.3.0/src/pymedx/__init__.py
--rw-r--r--   0        0        0    11739 2024-02-09 16:58:49.921217 pymedx-0.3.0/src/pymedx/api.py
--rw-r--r--   0        0        0    13063 2024-02-09 16:58:49.921217 pymedx-0.3.0/src/pymedx/article.py
--rw-r--r--   0        0        0     6004 2024-02-09 16:58:49.921217 pymedx-0.3.0/src/pymedx/book.py
--rw-r--r--   0        0        0     4552 2024-02-09 16:58:49.921217 pymedx-0.3.0/src/pymedx/helpers.py
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 pymedx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1925 2024-02-14 13:32:43.925454 pymedx-0.3.1/docs/index.md
+-rw-r--r--   0        0        0     1909 2024-02-14 13:34:23.302568 pymedx-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-02-14 13:34:23.298568 pymedx-0.3.1/src/pymedx/__init__.py
+-rw-r--r--   0        0        0    11739 2024-02-14 13:32:43.929454 pymedx-0.3.1/src/pymedx/api.py
+-rw-r--r--   0        0        0    13221 2024-02-14 13:32:43.929454 pymedx-0.3.1/src/pymedx/article.py
+-rw-r--r--   0        0        0     6004 2024-02-14 13:32:43.929454 pymedx-0.3.1/src/pymedx/book.py
+-rw-r--r--   0        0        0     4552 2024-02-14 13:32:43.929454 pymedx-0.3.1/src/pymedx/helpers.py
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 pymedx-0.3.1/PKG-INFO
```

### Comparing `pymedx-0.3.0/docs/index.md` & `pymedx-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pymedx-0.3.0/pyproject.toml` & `pymedx-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymedx"
-version = "0.3.0"  # semantic-release
+version = "0.3.1"  # semantic-release
 description = "PyMedX is a tool set for handling multimedia files."
 readme = "docs/index.md"
 authors = ["Gijs Wobben <gijswobben@gmail.com>", "Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 packages = [
   {include = "pymedx", from="src"},
 ]
 license = "MIT"
```

### Comparing `pymedx-0.3.0/src/pymedx/api.py` & `pymedx-0.3.1/src/pymedx/api.py`

 * *Files identical despite different names*

### Comparing `pymedx-0.3.0/src/pymedx/article.py` & `pymedx-0.3.1/src/pymedx/article.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,27 +281,32 @@
         self, xml_element: _Element
     ) -> Optional[datetime.date]:
         # Get the publication date
 
         # Get the publication elements
         publication_date = xml_element.find(".//pub-date[@pub-type='epub']")
 
-        if not publication_date:  # Check this part
+        if publication_date is None:
             publication_date = xml_element.find(".//pub-date")
 
         if publication_date is not None:
             publication_year = getContent(publication_date, ".//year", None)
 
+            if not publication_year or publication_year is None:
+                return None
+
             publication_month = getContent(publication_date, ".//month", "1")
 
             publication_day = getContent(publication_date, ".//day", "1")
 
             # Construct a datetime object from the info
             date_str: str = (
-                f"{publication_year}/{publication_month}/{publication_day}"
+                f"{str(publication_year).strip()}/"
+                f"{str(publication_month).strip()}/"
+                f"{str(publication_day).strip()}"
             )
 
             return datetime.datetime.strptime(date_str, "%Y/%m/%d")
 
         # Unable to parse the datetime
         return None
```

### Comparing `pymedx-0.3.0/src/pymedx/book.py` & `pymedx-0.3.1/src/pymedx/book.py`

 * *Files identical despite different names*

### Comparing `pymedx-0.3.0/src/pymedx/helpers.py` & `pymedx-0.3.1/src/pymedx/helpers.py`

 * *Files identical despite different names*

### Comparing `pymedx-0.3.0/PKG-INFO` & `pymedx-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymedx
-Version: 0.3.0
+Version: 0.3.1
 Summary: PyMedX is a tool set for handling multimedia files.
 License: MIT
 Author: Gijs Wobben
 Author-email: gijswobben@gmail.com
 Requires-Python: >3.8.1,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

