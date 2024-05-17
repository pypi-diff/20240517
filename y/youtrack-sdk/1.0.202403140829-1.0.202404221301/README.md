# Comparing `tmp/youtrack_sdk-1.0.202403140829.tar.gz` & `tmp/youtrack_sdk-1.0.202404221301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtrack_sdk-1.0.202403140829.tar", max compression
+gzip compressed data, was "youtrack_sdk-1.0.202404221301.tar", max compression
```

## Comparing `youtrack_sdk-1.0.202403140829.tar` & `youtrack_sdk-1.0.202404221301.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2024-03-14 08:29:09.241510 youtrack_sdk-1.0.202403140829/LICENSE
--rw-r--r--   0        0        0     1598 2024-03-14 08:29:09.241510 youtrack_sdk-1.0.202403140829/README.md
--rw-r--r--   0        0        0       41 2024-03-14 08:29:24.877603 youtrack_sdk-1.0.202403140829/VERSION.txt
--rw-r--r--   0        0        0      992 2024-03-14 08:29:24.877603 youtrack_sdk-1.0.202403140829/pyproject.toml
--rw-r--r--   0        0        0       49 2024-03-14 08:29:09.245510 youtrack_sdk-1.0.202403140829/youtrack_sdk/__init__.py
--rw-r--r--   0        0        0    22665 2024-03-14 08:29:09.245510 youtrack_sdk-1.0.202403140829/youtrack_sdk/client.py
--rw-r--r--   0        0        0    14325 2024-03-14 08:29:09.245510 youtrack_sdk-1.0.202403140829/youtrack_sdk/entities.py
--rw-r--r--   0        0        0      157 2024-03-14 08:29:09.245510 youtrack_sdk-1.0.202403140829/youtrack_sdk/exceptions.py
--rw-r--r--   0        0        0     5519 2024-03-14 08:29:09.245510 youtrack_sdk-1.0.202403140829/youtrack_sdk/helpers.py
--rw-r--r--   0        0        0     1233 2024-03-14 08:29:09.245510 youtrack_sdk-1.0.202403140829/youtrack_sdk/types.py
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 youtrack_sdk-1.0.202403140829/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-22 13:01:24.152963 youtrack_sdk-1.0.202404221301/LICENSE
+-rw-r--r--   0        0        0     1598 2024-04-22 13:01:24.152963 youtrack_sdk-1.0.202404221301/README.md
+-rw-r--r--   0        0        0       41 2024-04-22 13:01:39.880789 youtrack_sdk-1.0.202404221301/VERSION.txt
+-rw-r--r--   0        0        0      991 2024-04-22 13:01:39.876789 youtrack_sdk-1.0.202404221301/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-04-22 13:01:24.156963 youtrack_sdk-1.0.202404221301/youtrack_sdk/__init__.py
+-rw-r--r--   0        0        0    22665 2024-04-22 13:01:24.156963 youtrack_sdk-1.0.202404221301/youtrack_sdk/client.py
+-rw-r--r--   0        0        0    14325 2024-04-22 13:01:24.156963 youtrack_sdk-1.0.202404221301/youtrack_sdk/entities.py
+-rw-r--r--   0        0        0      157 2024-04-22 13:01:24.156963 youtrack_sdk-1.0.202404221301/youtrack_sdk/exceptions.py
+-rw-r--r--   0        0        0     5519 2024-04-22 13:01:24.156963 youtrack_sdk-1.0.202404221301/youtrack_sdk/helpers.py
+-rw-r--r--   0        0        0     1233 2024-04-22 13:01:24.156963 youtrack_sdk-1.0.202404221301/youtrack_sdk/types.py
+-rw-r--r--   0        0        0     2344 1970-01-01 00:00:00.000000 youtrack_sdk-1.0.202404221301/PKG-INFO
```

### Comparing `youtrack_sdk-1.0.202403140829/LICENSE` & `youtrack_sdk-1.0.202404221301/LICENSE`

 * *Files identical despite different names*

### Comparing `youtrack_sdk-1.0.202403140829/README.md` & `youtrack_sdk-1.0.202404221301/README.md`

 * *Files identical despite different names*

### Comparing `youtrack_sdk-1.0.202403140829/pyproject.toml` & `youtrack_sdk-1.0.202404221301/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "youtrack-sdk"
-version = "1.0.202403140829"
+version = "1.0.202404221301"
 description = "YouTrack SDK"
 authors = ["moneymeets <service@moneymeets.com>"]
 readme = "README.md"
 repository = "https://github.com/moneymeets/youtrack-sdk"
 packages = [
     { include = "youtrack_sdk" },
 ]
@@ -19,15 +19,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "~3.12"
 requests = "*"
-pydantic = "^2"
+pydantic = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-cov = "*"
 
 requests-mock = "*"
```

### Comparing `youtrack_sdk-1.0.202403140829/youtrack_sdk/client.py` & `youtrack_sdk-1.0.202404221301/youtrack_sdk/client.py`

 * *Files identical despite different names*

### Comparing `youtrack_sdk-1.0.202403140829/youtrack_sdk/entities.py` & `youtrack_sdk-1.0.202404221301/youtrack_sdk/entities.py`

 * *Files identical despite different names*

### Comparing `youtrack_sdk-1.0.202403140829/youtrack_sdk/helpers.py` & `youtrack_sdk-1.0.202404221301/youtrack_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `youtrack_sdk-1.0.202403140829/youtrack_sdk/types.py` & `youtrack_sdk-1.0.202404221301/youtrack_sdk/types.py`

 * *Files identical despite different names*

### Comparing `youtrack_sdk-1.0.202403140829/PKG-INFO` & `youtrack_sdk-1.0.202404221301/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: youtrack-sdk
-Version: 1.0.202403140829
+Version: 1.0.202404221301
 Summary: YouTrack SDK
 Home-page: https://github.com/moneymeets/youtrack-sdk
 License: MIT
 Keywords: youtrack,sdk
 Author: moneymeets
 Author-email: service@moneymeets.com
 Requires-Python: >=3.12,<3.13
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: pydantic (>=2,<3)
+Requires-Dist: pydantic
 Requires-Dist: requests
 Project-URL: Repository, https://github.com/moneymeets/youtrack-sdk
 Description-Content-Type: text/markdown
 
 # YouTrack REST API Client
 
 A client library for accessing YouTrack REST API.
```

