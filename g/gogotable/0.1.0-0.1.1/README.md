# Comparing `tmp/gogotable-0.1.0.tar.gz` & `tmp/gogotable-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gogotable-0.1.0.tar", max compression
+gzip compressed data, was "gogotable-0.1.1.tar", max compression
```

## Comparing `gogotable-0.1.0.tar` & `gogotable-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1211 2024-04-27 14:32:31.956850 gogotable-0.1.0/LICENSE
--rw-r--r--   0        0        0     1178 2024-04-27 14:32:31.957569 gogotable-0.1.0/README.md
--rw-r--r--   0        0        0      848 2024-05-10 12:55:41.355470 gogotable-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-27 14:32:31.961336 gogotable-0.1.0/src/gogotable/__init__.py
--rw-r--r--   0        0        0     1492 2024-05-10 12:52:39.471145 gogotable-0.1.0/src/gogotable/gogotable.py
--rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 gogotable-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-27 14:32:31.956850 gogotable-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1178 2024-04-27 14:32:31.957569 gogotable-0.1.1/README.md
+-rw-r--r--   0        0        0      848 2024-05-17 14:40:27.759263 gogotable-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-27 14:32:31.961336 gogotable-0.1.1/src/gogotable/__init__.py
+-rw-r--r--   0        0        0     1455 2024-05-17 14:39:24.799795 gogotable-0.1.1/src/gogotable/gogotable.py
+-rw-r--r--   0        0        0     1704 1970-01-01 00:00:00.000000 gogotable-0.1.1/PKG-INFO
```

### Comparing `gogotable-0.1.0/LICENSE` & `gogotable-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gogotable-0.1.0/README.md` & `gogotable-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gogotable-0.1.0/pyproject.toml` & `gogotable-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.poetry]
 name = "gogotable"
-version = "0.1.0"
+version = "0.1.1"
 description = "Convert structured data to a table"
 authors = ["Luís Miranda <luistm@gmail.com>"]
 license = "The Unlicense"
 readme = "README.md"
 packages = [{ include = "gogotable", from = "src" }]
 exclude = ["**/*_test.py"]
```

### Comparing `gogotable-0.1.0/src/gogotable/gogotable.py` & `gogotable-0.1.1/src/gogotable/gogotable.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,53 +3,49 @@
     Go Go Table
 
     :param headers: headers of the table
     :param rows: the data of the table
     :return: a list of strings representing the table
     """
 
-    table = []
-    skip_data = False
+    has_data_rows = True
 
     # Find the size of each column
     columns_length = []
     for i, _ in enumerate(headers):
+        column_length = 0
         try:
             column_length = max(len(str(row[i])) for row in rows)
         except IndexError:
-            column_length = 0
+            pass
         except ValueError:
             # There are no rows to calculate the max
-            column_length = 0
-            skip_data = True
+            has_data_rows = False
 
         # Sometimes, the header size is greater than the value
         if len(headers[i]) > column_length:
             column_length = len(headers[i])
 
         columns_length.append(column_length)
 
-    header_line = (
-        "|"
-        + "|".join(
-            f" {header:^{length}} " for header, length in zip(headers, columns_length)
-        )
-        + "|"
-    )
-    border = "|" + "-".join("-" * (length + 2) for length in columns_length) + "|"
-    table.extend([border, header_line, border])
+    # Vertical Border
+    vb = "|"
+    # Horizontal Border
+    hb = "-"
+
+    horizontal_border = vb + hb.join(hb * (1 + cl + 1) for cl in columns_length) + vb
+    header_cells = [
+        f" {header:^{length}} " for header, length in zip(headers, columns_length)
+    ]
+    header_line = vb + vb.join(header_cells) + vb
 
-    if not skip_data:
-        # Build the table data rows
+    table = [horizontal_border, header_line, horizontal_border]
+    if has_data_rows:
         for row in rows:
-            data_line = (
-                "|"
-                + "|".join(
-                    f" {data:>{length}} " for data, length in zip(row, columns_length)
-                )
-                + "|"
-            )
-            table.append(data_line)
+            data_cells = [
+                f" {data:>{length}} " for data, length in zip(row, columns_length)
+            ]
+            table.append(vb + vb.join(data_cells) + vb)
 
-    table.append(border)
+    table.append(horizontal_border)
 
     return table
```

### Comparing `gogotable-0.1.0/PKG-INFO` & `gogotable-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gogotable
-Version: 0.1.0
+Version: 0.1.1
 Summary: Convert structured data to a table
 License: Unlicense
 Author: Luís Miranda
 Author-email: luistm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

