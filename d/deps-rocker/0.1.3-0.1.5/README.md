# Comparing `tmp/deps_rocker-0.1.3.tar.gz` & `tmp/deps_rocker-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps_rocker-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deps_rocker-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deps_rocker-0.1.3.tar` & `deps_rocker-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1288 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/__init__.py
--rw-r--r--   0        0        0     8012 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/dependencies.py
--rw-r--r--   0        0        0      127 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/deps.yaml
--rw-r--r--   0        0        0      226 2024-05-17 11:29:19.629869 deps_rocker-0.1.3/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
--rw-r--r--   0        0        0      205 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/apt_snippet.Dockerfile
--rw-r--r--   0        0        0     1422 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/dependencies_snippet.Dockerfile
--rw-r--r--   0        0        0       85 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/env_snippet.Dockerfile
--rw-r--r--   0        0        0      118 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/pip_snippet.Dockerfile
--rw-r--r--   0        0        0      104 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/pyproject_snippet.Dockerfile
--rw-r--r--   0        0        0       99 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/run_snippet.Dockerfile
--rw-r--r--   0        0        0       77 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/templates/script_snippet.Dockerfile
--rw-r--r--   0        0        0      152 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/deps_rocker/toposort.py
--rw-r--r--   0        0        0     2216 2024-05-17 11:29:19.633870 deps_rocker-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 deps_rocker-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1288 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/__init__.py
+-rw-r--r--   0        0        0      128 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/dep_rocker_cli.py
+-rw-r--r--   0        0        0     8012 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/dependencies.py
+-rw-r--r--   0        0        0      127 2024-05-17 12:11:59.576516 deps_rocker-0.1.5/deps_rocker/deps.yaml
+-rw-r--r--   0        0        0      226 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/add-apt-repository_snippet.Dockerfile
+-rw-r--r--   0        0        0      205 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/apt_snippet.Dockerfile
+-rw-r--r--   0        0        0     1422 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/dependencies_snippet.Dockerfile
+-rw-r--r--   0        0        0       85 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/env_snippet.Dockerfile
+-rw-r--r--   0        0        0      118 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/pip_snippet.Dockerfile
+-rw-r--r--   0        0        0      104 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/pyproject_snippet.Dockerfile
+-rw-r--r--   0        0        0       99 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/run_snippet.Dockerfile
+-rw-r--r--   0        0        0       77 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/templates/script_snippet.Dockerfile
+-rw-r--r--   0        0        0      152 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/deps_rocker/toposort.py
+-rw-r--r--   0        0        0     2292 2024-05-17 12:11:59.580516 deps_rocker-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 deps_rocker-0.1.5/PKG-INFO
```

### Comparing `deps_rocker-0.1.3/README.md` & `deps_rocker-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.3/deps_rocker/dependencies.py` & `deps_rocker-0.1.5/deps_rocker/dependencies.py`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.3/deps_rocker/templates/dependencies_snippet.Dockerfile` & `deps_rocker-0.1.5/deps_rocker/templates/dependencies_snippet.Dockerfile`

 * *Files identical despite different names*

### Comparing `deps_rocker-0.1.3/pyproject.toml` & `deps_rocker-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "deps_rocker"
-version = "0.1.3"
+version = "0.1.5"
 license = { text = "MIT" }
 
 authors = [{ name = "Austin Gregg-Smith", email = "blooop@gmail.com" }]
 description = "A rocker plugin to help installing apt and pip dependencies"
 readme = "README.md"
 
 requires-python = ">=3.10"
@@ -29,16 +29,19 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.flit.sdist]
 include = ["deps_rocker/templates/*.Dockerfile"]
 
-[project.entrypoints."rocker.extensions"]
-"odeps_dependencies" = "deps_rocker.dependencies:Dependencies"
+[project.scripts]
+deps-rocker = "deps_rocker.dep_rocker_cli:gen_dockerfile"
+
+[project.entry-points."rocker.extensions"]
+odeps_dependencies = "deps_rocker.dependencies:Dependencies"
 
 
 [tool.pylint]
 jobs = 16                           #detect number of cores
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = "C,logging-fstring-interpolation,line-too-long,fixme,broad-exception-caught,missing-module-docstring,too-many-instance-attributes,too-few-public-methods,too-many-arguments,too-many-locals,too-many-branches,too-many-statements,use-dict-literal,cyclic-import,duplicate-code,too-many-public-methods"
```

### Comparing `deps_rocker-0.1.3/PKG-INFO` & `deps_rocker-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deps_rocker
-Version: 0.1.3
+Version: 0.1.5
 Summary: A rocker plugin to help installing apt and pip dependencies
 Author-email: Austin Gregg-Smith <blooop@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: rocker
 Requires-Dist: pyyaml
 Requires-Dist: off-your-rocker
```

