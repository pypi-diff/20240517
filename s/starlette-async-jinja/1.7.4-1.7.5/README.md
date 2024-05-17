# Comparing `tmp/starlette_async_jinja-1.7.4.tar.gz` & `tmp/starlette_async_jinja-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_async_jinja-1.7.4.tar", last modified: Sun Apr 28 09:08:08 2024, max compression
+gzip compressed data, was "starlette_async_jinja-1.7.5.tar", last modified: Fri May 17 14:27:10 2024, max compression
```

## Comparing `starlette_async_jinja-1.7.4.tar` & `starlette_async_jinja-1.7.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.4/LICENSE
--rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.4/README.md
--rw-r--r--   0        0        0     2353 2024-04-28 09:08:08.379025 starlette_async_jinja-1.7.4/pyproject.toml
--rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.7.4/starlette_async_jinja/__init__.py
--rw-r--r--   0        0        0     6344 2024-03-18 08:09:07.321729 starlette_async_jinja-1.7.4/starlette_async_jinja/responses.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.5/LICENSE
+-rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.5/README.md
+-rw-r--r--   0        0        0     2353 2024-05-17 14:27:10.694274 starlette_async_jinja-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.7.5/starlette_async_jinja/__init__.py
+-rw-r--r--   0        0        0     6344 2024-03-18 08:09:07.321729 starlette_async_jinja-1.7.5/starlette_async_jinja/responses.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.5/PKG-INFO
```

### Comparing `starlette_async_jinja-1.7.4/LICENSE` & `starlette_async_jinja-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.4/README.md` & `starlette_async_jinja-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.4/pyproject.toml` & `starlette_async_jinja-1.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,34 +37,34 @@
 
 [tool.creosote]
 paths = [
     "starlette_async_jinja",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "autotyping",
     "pre-commit",
-    "pdm-bump",
-    "python-ulid",
     "pdm",
+    "pdm-bump",
     "pytest",
+    "python-ulid",
+    "autotyping",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "starlette_async_jinja",
 ]
 skips = [
-    "B113",
     "B404",
-    "B603",
     "B403",
+    "B603",
+    "B113",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "starlette_async_jinja",
 ]
@@ -85,15 +85,15 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "starlette-async-jinja"
-version = "1.7.4"
+version = "1.7.5"
 description = ""
 dependencies = [
     "starlette>=0.34.0",
     "jinja2>=3.1.2",
     "jinja2-async-environment>=0.4.2",
 ]
 requires-python = ">=3.12"
```

### Comparing `starlette_async_jinja-1.7.4/starlette_async_jinja/responses.py` & `starlette_async_jinja-1.7.5/starlette_async_jinja/responses.py`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.4/PKG-INFO` & `starlette_async_jinja-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-async-jinja
-Version: 1.7.4
+Version: 1.7.5
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

