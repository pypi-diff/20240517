# Comparing `tmp/deps_rocker-0.1.2.tar.gz` & `tmp/deps_rocker-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps_rocker-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deps_rocker-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deps_rocker-0.1.2.tar` & `deps_rocker-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1288 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/__init__.py
--rw-r--r--   0        0        0     8012 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/dependencies.py
--rw-r--r--   0        0        0      127 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/deps.yaml
--rw-r--r--   0        0        0      226 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
--rw-r--r--   0        0        0      205 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/apt_snippet.Dockerfile
--rw-r--r--   0        0        0     1422 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/dependencies_snippet.Dockerfile
--rw-r--r--   0        0        0       85 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/env_snippet.Dockerfile
--rw-r--r--   0        0        0      118 2024-05-17 10:54:09.435171 deps_rocker-0.1.2/deps_rocker/templates/pip_snippet.Dockerfile
--rw-r--r--   0        0        0      104 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/templates/pyproject_snippet.Dockerfile
--rw-r--r--   0        0        0       99 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/templates/run_snippet.Dockerfile
--rw-r--r--   0        0        0       77 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/templates/script_snippet.Dockerfile
--rw-r--r--   0        0        0      152 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/deps_rocker/toposort.py
--rw-r--r--   0        0        0     2059 2024-05-17 10:54:09.439171 deps_rocker-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 deps_rocker-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1288 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/__init__.py
+-rw-r--r--   0        0        0     8012 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/dependencies.py
+-rw-r--r--   0        0        0      127 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/deps.yaml
+-rw-r--r--   0        0        0      226 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
+-rw-r--r--   0        0        0      205 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/apt_snippet.Dockerfile
+-rw-r--r--   0        0        0     1422 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/dependencies_snippet.Dockerfile
+-rw-r--r--   0        0        0       85 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/env_snippet.Dockerfile
+-rw-r--r--   0        0        0      118 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/pip_snippet.Dockerfile
+-rw-r--r--   0        0        0      104 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/pyproject_snippet.Dockerfile
+-rw-r--r--   0        0        0       99 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/run_snippet.Dockerfile
+-rw-r--r--   0        0        0       77 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/script_snippet.Dockerfile
+-rw-r--r--   0        0        0      152 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/toposort.py
+-rw-r--r--   0        0        0     2216 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 deps_rocker-0.1.3/PKG-INFO
```

### Comparing `deps_rocker-0.1.2/README.md` & `deps_rocker-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.2/deps_rocker/dependencies.py` & `deps_rocker-0.1.3/deps_rocker/dependencies.py`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.2/deps_rocker/templates/dependencies_snippet.Dockerfile` & `deps_rocker-0.1.3/deps_rocker/templates/dependencies_snippet.Dockerfile`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.2/pyproject.toml` & `deps_rocker-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [project]
 name = "deps_rocker"
-version = "0.1.2"
+version = "0.1.3"
+license = { text = "MIT" }
 
 authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
-description = "A python package template"
+description = "A rocker plugin to help installing apt and pip dependencies"
 readme = "README.md"
 
 requires-python = ">=3.10"
 
 dependencies = ["rocker","pyyaml","off-your-rocker","toml"]
 
 [project.optional-dependencies]
@@ -21,25 +22,26 @@
   "coverage>=7.2.7,<=7.5.1",
 ]
 
 [project.urls]
 Source = "https://github.com/blooop/deps_rocker"
 Home = "https://github.com/blooop/deps_rocker"
 
-
-[tool.flit.module]
-name = "deps_rocker"
-
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
+[tool.flit.sdist]
+include = ["deps_rocker/templates/*.Dockerfile"]
+
+[project.entrypoints."rocker.extensions"]
+"odeps_dependencies" = "deps_rocker.dependencies:Dependencies"
+
 
 [tool.pylint]
-extension-pkg-whitelist = ["numpy"]
 jobs = 16                           #detect number of cores
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = "C,logging-fstring-interpolation,line-too-long,fixme,broad-exception-caught,missing-module-docstring,too-many-instance-attributes,too-few-public-methods,too-many-arguments,too-many-locals,too-many-branches,too-many-statements,use-dict-literal,cyclic-import,duplicate-code,too-many-public-methods"
 enable = "no-else-return,consider-using-in"
 
 [tool.black]
```

### Comparing `deps_rocker-0.1.2/PKG-INFO` & `deps_rocker-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: deps_rocker
-Version: 0.1.2
-Summary: A python package template
+Version: 0.1.3
+Summary: A rocker plugin to help installing apt and pip dependencies
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: rocker
 Requires-Dist: pyyaml
 Requires-Dist: off-your-rocker
 Requires-Dist: toml
```

