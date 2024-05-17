# Comparing `tmp/gspread-6.1.1.tar.gz` & `tmp/gspread-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gspread-6.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gspread-6.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gspread-6.1.1.tar` & `gspread-6.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    39852 2024-05-15 23:22:07.109393 gspread-6.1.1/HISTORY.rst
--rw-r--r--   0        0        0     1064 2024-05-15 23:22:07.109393 gspread-6.1.1/LICENSE.txt
--rw-r--r--   0        0        0     9779 2024-05-15 23:22:07.109393 gspread-6.1.1/README.md
--rw-r--r--   0        0        0     1301 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/_templates/layout.html
--rw-r--r--   0        0        0     2310 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/advanced.rst
--rw-r--r--   0        0        0       53 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/auth.rst
--rw-r--r--   0        0        0       58 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/client.rst
--rw-r--r--   0        0        0      472 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/exceptions.rst
--rw-r--r--   0        0        0      258 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/http_client.rst
--rw-r--r--   0        0        0      144 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/index.rst
--rw-r--r--   0        0        0       57 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/cell.rst
--rw-r--r--   0        0        0      432 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/index.rst
--rw-r--r--   0        0        0       85 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/spreadsheet.rst
--rw-r--r--   0        0        0      179 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/models/worksheet.rst
--rw-r--r--   0        0        0      128 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/top-level.rst
--rw-r--r--   0        0        0       75 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/api/utils.rst
--rw-r--r--   0        0        0     9539 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/conf.py
--rw-r--r--   0        0        0     2306 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/index.rst
--rw-r--r--   0        0        0    11204 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/oauth2.rst
--rw-r--r--   0        0        0       46 2024-05-15 23:22:07.109393 gspread-6.1.1/docs/requirements.txt
--rw-r--r--   0        0        0    11159 2024-05-15 23:22:07.113393 gspread-6.1.1/docs/user-guide.rst
--rw-r--r--   0        0        0      560 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/__init__.py
--rw-r--r--   0        0        0    14310 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/auth.py
--rw-r--r--   0        0        0     2407 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/cell.py
--rw-r--r--   0        0        0    16121 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/client.py
--rw-r--r--   0        0        0     1713 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/exceptions.py
--rw-r--r--   0        0        0    22653 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/http_client.py
--rw-r--r--   0        0        0        0 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/py.typed
--rw-r--r--   0        0        0    29058 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/spreadsheet.py
--rw-r--r--   0        0        0     1287 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/urls.py
--rw-r--r--   0        0        0    28495 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/utils.py
--rw-r--r--   0        0        0   119486 2024-05-15 23:22:07.113393 gspread-6.1.1/gspread/worksheet.py
--rw-r--r--   0        0        0     1512 2024-05-15 23:22:07.113393 gspread-6.1.1/pyproject.toml
--rw-r--r--   0        0        0    11072 1970-01-01 00:00:00.000000 gspread-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0    40089 2024-05-17 21:30:41.947034 gspread-6.1.2/HISTORY.rst
+-rw-r--r--   0        0        0     1064 2024-05-17 21:30:41.947034 gspread-6.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     9779 2024-05-17 21:30:41.947034 gspread-6.1.2/README.md
+-rw-r--r--   0        0        0     1301 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/_templates/layout.html
+-rw-r--r--   0        0        0     2310 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/advanced.rst
+-rw-r--r--   0        0        0       53 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/auth.rst
+-rw-r--r--   0        0        0       58 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/client.rst
+-rw-r--r--   0        0        0      472 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/exceptions.rst
+-rw-r--r--   0        0        0      258 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/http_client.rst
+-rw-r--r--   0        0        0      144 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/index.rst
+-rw-r--r--   0        0        0       57 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/models/cell.rst
+-rw-r--r--   0        0        0      432 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/models/index.rst
+-rw-r--r--   0        0        0       85 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/models/spreadsheet.rst
+-rw-r--r--   0        0        0      179 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/models/worksheet.rst
+-rw-r--r--   0        0        0      128 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/top-level.rst
+-rw-r--r--   0        0        0       75 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/api/utils.rst
+-rw-r--r--   0        0        0     9539 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/conf.py
+-rw-r--r--   0        0        0     2306 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/index.rst
+-rw-r--r--   0        0        0    11204 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/oauth2.rst
+-rw-r--r--   0        0        0       46 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0    11159 2024-05-17 21:30:41.947034 gspread-6.1.2/docs/user-guide.rst
+-rw-r--r--   0        0        0      560 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/__init__.py
+-rw-r--r--   0        0        0    14310 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/auth.py
+-rw-r--r--   0        0        0     2407 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/cell.py
+-rw-r--r--   0        0        0    16121 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/client.py
+-rw-r--r--   0        0        0     1713 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/exceptions.py
+-rw-r--r--   0        0        0    22653 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/http_client.py
+-rw-r--r--   0        0        0        0 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/py.typed
+-rw-r--r--   0        0        0    29058 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/spreadsheet.py
+-rw-r--r--   0        0        0     1287 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/urls.py
+-rw-r--r--   0        0        0    28495 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/utils.py
+-rw-r--r--   0        0        0   120067 2024-05-17 21:30:41.947034 gspread-6.1.2/gspread/worksheet.py
+-rw-r--r--   0        0        0     1512 2024-05-17 21:30:41.947034 gspread-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11072 1970-01-01 00:00:00.000000 gspread-6.1.2/PKG-INFO
```

### Comparing `gspread-6.1.1/HISTORY.rst` & `gspread-6.1.2/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Release History
 ===============
 
+6.1.2 (2024-05-17)
+------------------
+
+* add note about runnings tests to contrib guide by @alifeee in https://github.com/burnash/gspread/pull/1465
+* Some updates on `get_notes` by @nbwzx in https://github.com/burnash/gspread/pull/1461
+
 6.1.1 (2024-05-16)
 ------------------
 
 * Add some missing typing in code by @lavigne958 in https://github.com/burnash/gspread/pull/1448
 * More fixes for `Worksheet.update` argument ordering & single cell updating (i.e. now `Worksheet.update_acell`) by @alexmalins in https://github.com/burnash/gspread/pull/1449
 * Added 'add_data_validation` to `Workhsheet` [Issue #1420] by @muddi900 in https://github.com/burnash/gspread/pull/1444
 * Bump typing-extensions from 4.10.0 to 4.11.0 by @dependabot in https://github.com/burnash/gspread/pull/1450
```

### Comparing `gspread-6.1.1/LICENSE.txt` & `gspread-6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/README.md` & `gspread-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/docs/_templates/layout.html` & `gspread-6.1.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/docs/advanced.rst` & `gspread-6.1.2/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/docs/conf.py` & `gspread-6.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/docs/index.rst` & `gspread-6.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/docs/oauth2.rst` & `gspread-6.1.2/docs/oauth2.rst`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/docs/user-guide.rst` & `gspread-6.1.2/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/__init__.py` & `gspread-6.1.2/gspread/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Google Spreadsheets Python API"""
 
-__version__ = "6.1.1"
+__version__ = "6.1.2"
 __author__ = "Anton Burnashev"
 
 
 from .auth import (
     api_key,
     authorize,
     oauth,
```

### Comparing `gspread-6.1.1/gspread/auth.py` & `gspread-6.1.2/gspread/auth.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/cell.py` & `gspread-6.1.2/gspread/cell.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/client.py` & `gspread-6.1.2/gspread/client.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/exceptions.py` & `gspread-6.1.2/gspread/exceptions.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/http_client.py` & `gspread-6.1.2/gspread/http_client.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/spreadsheet.py` & `gspread-6.1.2/gspread/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/urls.py` & `gspread-6.1.2/gspread/urls.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/utils.py` & `gspread-6.1.2/gspread/utils.py`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/gspread/worksheet.py` & `gspread-6.1.2/gspread/worksheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -2602,32 +2602,54 @@
                     },
                 },
             ]
         }
 
         return self.client.batch_update(self.spreadsheet_id, body)
 
-    def get_notes(self, default_empty_value: Optional[str] = None) -> List[List[str]]:
-        """Returns a list of lists containing all notes in the sheet, or the empty list if the
-        sheet does not have a note.
+    def get_notes(self, default_empty_value: Optional[str] = "") -> List[List[str]]:
+        """Returns a list of lists containing all notes in the sheet.
 
         .. note::
 
-            The resulting matrix is as long as the last row holding a note
-                (could be smaller than the last data row)
+            The resulting matrix is not necessarily square.
+            The matrix is as tall as the last row with a note,
+            and each row is only as long as the last column in that row with a note.
 
-            The resulting matrix is as large as the last column holding a note
-                (could be smaller than the last data column)
+
+            Please see the example below.
+            To ensure it is square, use `gspread.utils.fill_gaps`,
+            for example like `utils.fill_gaps(arr, len(arr), max(len(a) for a in arr), None)`
 
         :param str default_empty_value: (optional) Determines which value to use
             for cells without notes, defaults to None.
+
+        Examples::
+
+            # Note data:
+            #      A      B
+            # 1    A1     -
+            # 2    -      B2
+
+            # Read all notes from the sheet
+            >>> arr = worksheet.get_notes()
+            >>> print(arr)
+            [
+                ["A1"],
+                ["", "B2"]
+            ]
+            >>> print(gspread.utils.fill_gaps(arr, len(arr), max(len(a) for a in arr), None))
+            [
+                ["A1", ""],
+                ["", "B2"]
+            ]
         """
         params: ParamsType = {"fields": "sheets.data.rowData.values.note"}
         res = self.client.spreadsheets_get(self.spreadsheet_id, params)
-        data = res["sheets"][self.index]["data"][0].get("rowData", [])
+        data = res["sheets"][self.index]["data"][0].get("rowData", [{}])
         notes: List[List[str]] = []
         for row in data:
             notes.append([])
             for cell in row.get("values", []):
                 notes[-1].append(cell.get("note", default_empty_value))
 
         return notes
```

### Comparing `gspread-6.1.1/pyproject.toml` & `gspread-6.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gspread-6.1.1/PKG-INFO` & `gspread-6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gspread
-Version: 6.1.1
+Version: 6.1.2
 Summary: Google Spreadsheets Python API
 Keywords: spreadsheets,google-spreadsheets,google-sheets
 Author-email: Anton Burnashev <fuss.here@gmail.com>
 Maintainer-email: Alexandre Lavigne <lavigne958@gmail.com>, alifeee <alifeee.web@outlook.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
```

