# Comparing `tmp/deps_rocker-0.1.1.tar.gz` & `tmp/deps_rocker-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps_rocker-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deps_rocker-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deps_rocker-0.1.1.tar` & `deps_rocker-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1288 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/__init__.py
--rw-r--r--   0        0        0     8012 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/dependencies.py
--rw-r--r--   0        0        0      127 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/deps.yaml
--rw-r--r--   0        0        0      226 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
--rw-r--r--   0        0        0      205 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/apt_snippet.Dockerfile
--rw-r--r--   0        0        0     1422 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/dependencies_snippet.Dockerfile
--rw-r--r--   0        0        0       85 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/env_snippet.Dockerfile
--rw-r--r--   0        0        0      118 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/pip_snippet.Dockerfile
--rw-r--r--   0        0        0      104 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/pyproject_snippet.Dockerfile
--rw-r--r--   0        0        0       99 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/run_snippet.Dockerfile
--rw-r--r--   0        0        0       77 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/templates/script_snippet.Dockerfile
--rw-r--r--   0        0        0      152 2024-05-17 10:53:28.551559 deps_rocker-0.1.1/deps_rocker/toposort.py
--rw-r--r--   0        0        0     2059 2024-05-17 10:53:28.555559 deps_rocker-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 deps_rocker-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1288 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/__init__.py
+-rw-r--r--   0        0        0     8012 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/dependencies.py
+-rw-r--r--   0        0        0      127 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/deps.yaml
+-rw-r--r--   0        0        0      226 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
+-rw-r--r--   0        0        0      205 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/apt_snippet.Dockerfile
+-rw-r--r--   0        0        0     1422 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/dependencies_snippet.Dockerfile
+-rw-r--r--   0        0        0       85 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/env_snippet.Dockerfile
+-rw-r--r--   0        0        0      118 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/pip_snippet.Dockerfile
+-rw-r--r--   0        0        0      104 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/templates/pyproject_snippet.Dockerfile
+-rw-r--r--   0        0        0       99 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/templates/run_snippet.Dockerfile
+-rw-r--r--   0        0        0       77 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/templates/script_snippet.Dockerfile
+-rw-r--r--   0        0        0      152 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/toposort.py
+-rw-r--r--   0        0        0     2059 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 deps_rocker-0.1.2/PKG-INFO
```

### Comparing `deps_rocker-0.1.1/README.md` & `deps_rocker-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.1/deps_rocker/dependencies.py` & `deps_rocker-0.1.2/deps_rocker/dependencies.py`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.1/deps_rocker/templates/dependencies_snippet.Dockerfile` & `deps_rocker-0.1.2/deps_rocker/templates/dependencies_snippet.Dockerfile`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.1/pyproject.toml` & `deps_rocker-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deps_rocker"
-version = "0.1.1"
+version = "0.1.2"
 
 authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
 description = "A python package template"
 readme = "README.md"
 
 requires-python = ">=3.10"
```

### Comparing `deps_rocker-0.1.1/PKG-INFO` & `deps_rocker-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deps_rocker
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package template
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: rocker
 Requires-Dist: pyyaml
 Requires-Dist: off-your-rocker
```

