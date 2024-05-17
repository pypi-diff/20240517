# Comparing `tmp/bilbyai_source_label_map-0.2.5.tar.gz` & `tmp/bilbyai_source_label_map-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilbyai_source_label_map-0.2.5.tar", max compression
+gzip compressed data, was "bilbyai_source_label_map-0.2.6.tar", max compression
```

## Comparing `bilbyai_source_label_map-0.2.5.tar` & `bilbyai_source_label_map-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3452 2024-05-16 07:09:01.493211 bilbyai_source_label_map-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-05-16 07:09:01.493211 bilbyai_source_label_map-0.2.5/bilbyai/__init__.py
--rw-r--r--   0        0        0      132 2024-05-16 07:09:01.493211 bilbyai_source_label_map-0.2.5/bilbyai/source_label_map/__init__.py
--rw-r--r--   0        0        0    18400 2024-05-16 07:09:01.493211 bilbyai_source_label_map-0.2.5/bilbyai/source_label_map/source_label_map.py
--rw-r--r--   0        0        0      629 2024-05-16 07:09:01.493211 bilbyai_source_label_map-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3947 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     3881 2024-05-17 10:16:35.587593 bilbyai_source_label_map-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 10:16:35.587593 bilbyai_source_label_map-0.2.6/bilbyai/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-17 10:16:35.587593 bilbyai_source_label_map-0.2.6/bilbyai/source_label_map/__init__.py
+-rw-r--r--   0        0        0    18400 2024-05-17 10:16:35.587593 bilbyai_source_label_map-0.2.6/bilbyai/source_label_map/source_label_map.py
+-rw-r--r--   0        0        0      629 2024-05-17 10:16:35.587593 bilbyai_source_label_map-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 bilbyai_source_label_map-0.2.6/PKG-INFO
```

### Comparing `bilbyai_source_label_map-0.2.5/README.md` & `bilbyai_source_label_map-0.2.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,24 +21,29 @@
 
 get_source_labels("ben")
 # 'Beijing Evening News'
 
 get_source_labels(["gmwnews", "ben"]) 
 # ['Enlightenment Daily', 'Beijing Evening News']
 
-get_source_labels("cannot-be-found") 
+# Since the key 'cannot-be-found' is not in the dictionary, it returns the original input.
+get_source_labels("cannot-be-found")
+get_source_labels("cannot-be-found", when_not_found="preserve") # this is the default.
 # 'cannot-be-found'
 
-get_source_labels("cannot-be-found", when_not_found="set_none") 
+# When the option is set to 'set_none', the function returns None when the key is not found.
+get_source_labels("cannot-be-found", when_not_found="set_none")
 # None
 
+# When the option is set to 'set_unknown', the function returns the string "unknown".
 get_source_labels("cannot-be-found", when_not_found="set_unknown") 
 # 'unknown'
 
-get_source_labels("ben", when_not_found="throw_error") 
+# When the option is set to 'raise_error', the function raises a ValueError.
+get_source_labels("ben", when_not_found="raise_error") 
 # raises ValueError
 ```
 
 ### Using `get_source_labels` with DataFrames 
 
 ```python
 import pandas as pd
@@ -70,15 +75,15 @@
 # Name: source_label, dtype: object
 ```
 
 
 # Function Specs
 Get source labels for a list of inputs.
 
-### Args:
+### Args
 
 `source` (`str | Iterable[str]`): The string or list of strings to get source labels for.
   
 `when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
 - `"preserve"`: Preserve the source name as the source label. 
 - `"set_none"`: Set the source label to None. 
 - `"set_unknown"`: Set the source label to "unknown". 
@@ -90,21 +95,21 @@
     "gmwnews": "Enlightenment Daily",
     "sina_news": "Sina News",
     "xueqiu": "Xueqiu (Snowball Finance)",
     "peoplenews": "People's Daily",
 }
 ```
 
-### Returns:
+### Returns
   A list of source labels for the inputs.
 
-### Raises:
+### Raises
   `ValueError`: If the when_not_found value is not recognized.
   `ValueError`: If the inputs are not a string or iterable of strings.
-  `ValueError`: If when_not_found is set to "throw_error" and a source label is not found.
+  `ValueError`: If when_not_found is set to "raise_error" and a source label is not found.
 
 The project owner is [@leetdavid](https://github.com/leetdavid).
 
 ## Development
 
 If not already in a virtual environement, create and use one.
 Read about it in the Python documentation: [venv — Creation of virtual environments](https://docs.python.org/3/library/venv.html).
```

### Comparing `bilbyai_source_label_map-0.2.5/bilbyai/source_label_map/source_label_map.py` & `bilbyai_source_label_map-0.2.6/bilbyai/source_label_map/source_label_map.py`

 * *Files identical despite different names*

### Comparing `bilbyai_source_label_map-0.2.5/pyproject.toml` & `bilbyai_source_label_map-0.2.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "bilbyai-source-label-map"
 readme = "README.md"
-version = "0.2.5"
+version = "0.2.6"
 description = "Converts news sources into human-friendly labels" 
 authors = [
     "David Lee <leetdavidu@gmail.com>"
 ]
 packages = [
   { include = "bilbyai" }
 ]
```

### Comparing `bilbyai_source_label_map-0.2.5/PKG-INFO` & `bilbyai_source_label_map-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilbyai-source-label-map
-Version: 0.2.5
+Version: 0.2.6
 Summary: Converts news sources into human-friendly labels
 Author: David Lee
 Author-email: leetdavidu@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -35,24 +35,29 @@
 
 get_source_labels("ben")
 # 'Beijing Evening News'
 
 get_source_labels(["gmwnews", "ben"]) 
 # ['Enlightenment Daily', 'Beijing Evening News']
 
-get_source_labels("cannot-be-found") 
+# Since the key 'cannot-be-found' is not in the dictionary, it returns the original input.
+get_source_labels("cannot-be-found")
+get_source_labels("cannot-be-found", when_not_found="preserve") # this is the default.
 # 'cannot-be-found'
 
-get_source_labels("cannot-be-found", when_not_found="set_none") 
+# When the option is set to 'set_none', the function returns None when the key is not found.
+get_source_labels("cannot-be-found", when_not_found="set_none")
 # None
 
+# When the option is set to 'set_unknown', the function returns the string "unknown".
 get_source_labels("cannot-be-found", when_not_found="set_unknown") 
 # 'unknown'
 
-get_source_labels("ben", when_not_found="throw_error") 
+# When the option is set to 'raise_error', the function raises a ValueError.
+get_source_labels("ben", when_not_found="raise_error") 
 # raises ValueError
 ```
 
 ### Using `get_source_labels` with DataFrames 
 
 ```python
 import pandas as pd
@@ -84,15 +89,15 @@
 # Name: source_label, dtype: object
 ```
 
 
 # Function Specs
 Get source labels for a list of inputs.
 
-### Args:
+### Args
 
 `source` (`str | Iterable[str]`): The string or list of strings to get source labels for.
   
 `when_not_found`: The action to take when a source label is not found. Set to "preserve_source_name" by default.
 - `"preserve"`: Preserve the source name as the source label. 
 - `"set_none"`: Set the source label to None. 
 - `"set_unknown"`: Set the source label to "unknown". 
@@ -104,21 +109,21 @@
     "gmwnews": "Enlightenment Daily",
     "sina_news": "Sina News",
     "xueqiu": "Xueqiu (Snowball Finance)",
     "peoplenews": "People's Daily",
 }
 ```
 
-### Returns:
+### Returns
   A list of source labels for the inputs.
 
-### Raises:
+### Raises
   `ValueError`: If the when_not_found value is not recognized.
   `ValueError`: If the inputs are not a string or iterable of strings.
-  `ValueError`: If when_not_found is set to "throw_error" and a source label is not found.
+  `ValueError`: If when_not_found is set to "raise_error" and a source label is not found.
 
 The project owner is [@leetdavid](https://github.com/leetdavid).
 
 ## Development
 
 If not already in a virtual environement, create and use one.
 Read about it in the Python documentation: [venv — Creation of virtual environments](https://docs.python.org/3/library/venv.html).
```

