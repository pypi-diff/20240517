# Comparing `tmp/souk-0.4.0.tar.gz` & `tmp/souk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "souk-0.4.0.tar", max compression
+gzip compressed data, was "souk-0.4.1.tar", max compression
```

## Comparing `souk-0.4.0.tar` & `souk-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1533 2024-03-12 16:57:02.953777 souk-0.4.0/LICENSE
--rw-r--r--   0        0        0     3654 2024-03-12 16:57:02.953777 souk-0.4.0/README.md
--rw-r--r--   0        0        0     4955 2024-03-12 16:57:02.957777 souk-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-12 16:57:02.957777 souk-0.4.0/src/souk/__init__.py
--rw-r--r--   0        0        0      406 2024-03-12 16:57:02.957777 souk-0.4.0/src/souk/htcondor_helper.py
--rwxr-xr-x   0        0        0    10024 2024-03-12 16:57:02.957777 souk-0.4.0/src/souk/system/arch_info.py
--rw-r--r--   0        0        0        0 2024-03-12 16:57:02.957777 souk-0.4.0/src/souk/util/__init__.py
--rw-r--r--   0        0        0        0 2024-03-12 16:57:02.957777 souk-0.4.0/src/souk/util/cli/__init__.py
--rw-r--r--   0        0        0      538 2024-03-12 16:57:02.957777 souk-0.4.0/src/souk/util/cli/arg_string.py
--rw-r--r--   0        0        0     1601 2024-03-12 16:57:02.957777 souk-0.4.0/src/souk/util/cli/ini_formatter.py
--rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 souk-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-05-17 13:02:03.256873 souk-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3654 2024-05-17 13:02:03.256873 souk-0.4.1/README.md
+-rw-r--r--   0        0        0     4955 2024-05-17 13:02:03.264873 souk-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-17 13:02:03.264873 souk-0.4.1/src/souk/__init__.py
+-rw-r--r--   0        0        0      406 2024-05-17 13:02:03.264873 souk-0.4.1/src/souk/htcondor_helper.py
+-rwxr-xr-x   0        0        0    10024 2024-05-17 13:02:03.264873 souk-0.4.1/src/souk/system/arch_info.py
+-rw-r--r--   0        0        0        0 2024-05-17 13:02:03.264873 souk-0.4.1/src/souk/util/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 13:02:03.264873 souk-0.4.1/src/souk/util/cli/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-17 13:02:03.264873 souk-0.4.1/src/souk/util/cli/arg_string.py
+-rw-r--r--   0        0        0     1601 2024-05-17 13:02:03.264873 souk-0.4.1/src/souk/util/cli/ini_formatter.py
+-rw-r--r--   0        0        0     5437 1970-01-01 00:00:00.000000 souk-0.4.1/PKG-INFO
```

### Comparing `souk-0.4.0/LICENSE` & `souk-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `souk-0.4.0/README.md` & `souk-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `souk-0.4.0/pyproject.toml` & `souk-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "souk"
-version = "0.4.0"
+version = "0.4.1"
 description = "SO:UK Data Centre documentation."
 license = "BSD-3-Clause"
 keywords = [
     "data centre",
     "HPC",
     "HTC",
     "SO:UK",
@@ -137,15 +137,15 @@
     '.eggs',
     'ci/templates',
     'build',
     'dist',
 ]
 
 [tool.bumpversion]
-current_version = "0.4.0"
+current_version = "0.4.1"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `souk-0.4.0/src/souk/system/arch_info.py` & `souk-0.4.1/src/souk/system/arch_info.py`

 * *Files identical despite different names*

### Comparing `souk-0.4.0/src/souk/util/cli/arg_string.py` & `souk-0.4.1/src/souk/util/cli/arg_string.py`

 * *Files identical despite different names*

### Comparing `souk-0.4.0/src/souk/util/cli/ini_formatter.py` & `souk-0.4.1/src/souk/util/cli/ini_formatter.py`

 * *Files identical despite different names*

### Comparing `souk-0.4.0/PKG-INFO` & `souk-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: souk
-Version: 0.4.0
+Version: 0.4.1
 Summary: SO:UK Data Centre documentation.
 Home-page: https://docs.souk.ac.uk
 License: BSD-3-Clause
 Keywords: data centre,HPC,HTC,SO:UK
 Author: Kolen Cheung
 Author-email: christian.kolen@gmail.com
 Requires-Python: >=3.9
```

