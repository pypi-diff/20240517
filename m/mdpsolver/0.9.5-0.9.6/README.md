# Comparing `tmp/mdpsolver-0.9.5.tar.gz` & `tmp/mdpsolver-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdpsolver-0.9.5.tar", last modified: Sun May 12 13:16:29 2024, max compression
+gzip compressed data, was "mdpsolver-0.9.6.tar", last modified: Fri May 17 14:46:58 2024, max compression
```

## Comparing `mdpsolver-0.9.5.tar` & `mdpsolver-0.9.6.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-12 13:16:29.940960 mdpsolver-0.9.5/
--rw-rw-r--   0 anders    (1000) anders    (1000)     1106 2024-04-28 23:39:54.000000 mdpsolver-0.9.5/LICENSE
--rw-rw-r--   0 anders    (1000) anders    (1000)       37 2024-04-28 23:19:52.000000 mdpsolver-0.9.5/MANIFEST.in
--rw-r--r--   0 anders    (1000) anders    (1000)     4384 2024-05-12 13:16:29.940960 mdpsolver-0.9.5/PKG-INFO
--rw-rw-r--   0 anders    (1000) anders    (1000)     3777 2024-05-12 13:14:16.000000 mdpsolver-0.9.5/README.md
--rw-rw-r--   0 anders    (1000) anders    (1000)      789 2024-05-12 13:00:23.000000 mdpsolver-0.9.5/pyproject.toml
--rw-rw-r--   0 anders    (1000) anders    (1000)       38 2024-05-12 13:16:29.940960 mdpsolver-0.9.5/setup.cfg
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-12 13:16:29.932960 mdpsolver-0.9.5/src/
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-12 13:16:29.936960 mdpsolver-0.9.5/src/mdpsolver/
--rw-rw-r--   0 anders    (1000) anders    (1000)       33 2024-04-28 23:39:54.000000 mdpsolver-0.9.5/src/mdpsolver/__init__.py
--rw-rw-r--   0 anders    (1000) anders    (1000)     4754 2024-05-10 15:54:49.000000 mdpsolver-0.9.5/src/mdpsolver/model.py
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-12 13:16:29.940960 mdpsolver-0.9.5/src/mdpsolver/problems/
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-12 13:16:29.940960 mdpsolver-0.9.5/src/mdpsolver/problems/__pycache__/
--rw-rw-r--   0 anders    (1000) anders    (1000)     1208 2024-05-12 12:59:13.000000 mdpsolver-0.9.5/src/mdpsolver/problems/__pycache__/cbmaux.cpython-310.pyc
--rw-rw-r--   0 anders    (1000) anders    (1000)     1208 2024-05-12 12:59:13.000000 mdpsolver-0.9.5/src/mdpsolver/problems/__pycache__/tbmaux.cpython-310.pyc
--rw-rw-r--   0 anders    (1000) anders    (1000)     1371 2024-04-28 23:39:54.000000 mdpsolver-0.9.5/src/mdpsolver/problems/cbmaux.py
--rw-rw-r--   0 anders    (1000) anders    (1000)     1366 2024-04-28 23:39:54.000000 mdpsolver-0.9.5/src/mdpsolver/problems/tbmaux.py
--rw-r--r--   0 anders    (1000) anders    (1000)   256512 2024-05-12 12:51:09.000000 mdpsolver-0.9.5/src/mdpsolver/solvermodule.cp310-win_amd64.pyd
--rw-r--r--   0 anders    (1000) anders    (1000)   258560 2024-05-12 12:51:09.000000 mdpsolver-0.9.5/src/mdpsolver/solvermodule.cp311-win_amd64.pyd
--rw-r--r--   0 anders    (1000) anders    (1000)   260608 2024-05-12 12:26:21.000000 mdpsolver-0.9.5/src/mdpsolver/solvermodule.cp312-win_amd64.pyd
--rwxrwxr-x   0 anders    (1000) anders    (1000)   455592 2024-05-12 11:55:05.000000 mdpsolver-0.9.5/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so
-drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-12 13:16:29.940960 mdpsolver-0.9.5/src/mdpsolver.egg-info/
--rw-r--r--   0 anders    (1000) anders    (1000)     4384 2024-05-12 13:16:29.000000 mdpsolver-0.9.5/src/mdpsolver.egg-info/PKG-INFO
--rw-rw-r--   0 anders    (1000) anders    (1000)      623 2024-05-12 13:16:29.000000 mdpsolver-0.9.5/src/mdpsolver.egg-info/SOURCES.txt
--rw-rw-r--   0 anders    (1000) anders    (1000)        1 2024-05-12 13:16:29.000000 mdpsolver-0.9.5/src/mdpsolver.egg-info/dependency_links.txt
--rw-rw-r--   0 anders    (1000) anders    (1000)       10 2024-05-12 13:16:29.000000 mdpsolver-0.9.5/src/mdpsolver.egg-info/top_level.txt
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-17 14:46:58.977307 mdpsolver-0.9.6/
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1106 2024-04-28 23:39:54.000000 mdpsolver-0.9.6/LICENSE
+-rw-rw-r--   0 anders    (1000) anders    (1000)       37 2024-04-28 23:19:52.000000 mdpsolver-0.9.6/MANIFEST.in
+-rw-r--r--   0 anders    (1000) anders    (1000)     4713 2024-05-17 14:46:58.973307 mdpsolver-0.9.6/PKG-INFO
+-rw-rw-r--   0 anders    (1000) anders    (1000)     4106 2024-05-17 10:28:01.000000 mdpsolver-0.9.6/README.md
+-rw-rw-r--   0 anders    (1000) anders    (1000)      789 2024-05-17 14:45:51.000000 mdpsolver-0.9.6/pyproject.toml
+-rw-rw-r--   0 anders    (1000) anders    (1000)       38 2024-05-17 14:46:58.977307 mdpsolver-0.9.6/setup.cfg
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-17 14:46:58.969307 mdpsolver-0.9.6/src/
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-17 14:46:58.973307 mdpsolver-0.9.6/src/mdpsolver/
+-rw-rw-r--   0 anders    (1000) anders    (1000)       33 2024-04-28 23:39:54.000000 mdpsolver-0.9.6/src/mdpsolver/__init__.py
+-rw-rw-r--   0 anders    (1000) anders    (1000)     4754 2024-05-12 13:19:50.000000 mdpsolver-0.9.6/src/mdpsolver/model.py
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-17 14:46:58.973307 mdpsolver-0.9.6/src/mdpsolver/problems/
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-17 14:46:58.973307 mdpsolver-0.9.6/src/mdpsolver/problems/__pycache__/
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1208 2024-05-12 12:59:13.000000 mdpsolver-0.9.6/src/mdpsolver/problems/__pycache__/cbmaux.cpython-310.pyc
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1208 2024-05-12 12:59:13.000000 mdpsolver-0.9.6/src/mdpsolver/problems/__pycache__/tbmaux.cpython-310.pyc
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1371 2024-04-28 23:39:54.000000 mdpsolver-0.9.6/src/mdpsolver/problems/cbmaux.py
+-rw-rw-r--   0 anders    (1000) anders    (1000)     1366 2024-04-28 23:39:54.000000 mdpsolver-0.9.6/src/mdpsolver/problems/tbmaux.py
+-rw-rw-r--   0 anders    (1000) anders    (1000)   256512 2024-05-12 13:19:50.000000 mdpsolver-0.9.6/src/mdpsolver/solvermodule.cp310-win_amd64.pyd
+-rw-rw-r--   0 anders    (1000) anders    (1000)   258560 2024-05-12 13:19:50.000000 mdpsolver-0.9.6/src/mdpsolver/solvermodule.cp311-win_amd64.pyd
+-rw-rw-r--   0 anders    (1000) anders    (1000)   260608 2024-05-12 13:19:50.000000 mdpsolver-0.9.6/src/mdpsolver/solvermodule.cp312-win_amd64.pyd
+-rw-rw-r--   0 anders    (1000) anders    (1000)   455592 2024-05-12 13:19:50.000000 mdpsolver-0.9.6/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so
+-rwxr-xr-x   0 anders    (1000) anders    (1000)   437312 2024-05-17 14:15:59.000000 mdpsolver-0.9.6/src/mdpsolver/solvermodule.cpython-311-x86_64-linux-gnu.so
+-rwxr-xr-x   0 anders    (1000) anders    (1000)   436736 2024-05-17 14:22:05.000000 mdpsolver-0.9.6/src/mdpsolver/solvermodule.cpython-312-x86_64-linux-gnu.so
+drwxrwxr-x   0 anders    (1000) anders    (1000)        0 2024-05-17 14:46:58.973307 mdpsolver-0.9.6/src/mdpsolver.egg-info/
+-rw-r--r--   0 anders    (1000) anders    (1000)     4713 2024-05-17 14:46:58.000000 mdpsolver-0.9.6/src/mdpsolver.egg-info/PKG-INFO
+-rw-rw-r--   0 anders    (1000) anders    (1000)      741 2024-05-17 14:46:58.000000 mdpsolver-0.9.6/src/mdpsolver.egg-info/SOURCES.txt
+-rw-rw-r--   0 anders    (1000) anders    (1000)        1 2024-05-17 14:46:58.000000 mdpsolver-0.9.6/src/mdpsolver.egg-info/dependency_links.txt
+-rw-rw-r--   0 anders    (1000) anders    (1000)       10 2024-05-17 14:46:58.000000 mdpsolver-0.9.6/src/mdpsolver.egg-info/top_level.txt
```

### Comparing `mdpsolver-0.9.5/LICENSE` & `mdpsolver-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.5/PKG-INFO` & `mdpsolver-0.9.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdpsolver
-Version: 0.9.5
+Version: 0.9.6
 Summary: A fast solver for Markov Decision Processes
 Author-email: Anders Reenberg Andersen <andersra@live.dk>, Jesper Fink Andersen <jfan@dtu.dk>
 Project-URL: Homepage, https://github.com/areenberg/MDPSolver
 Project-URL: Issues, https://github.com/areenberg/MDPSolver/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,26 +23,40 @@
 
 * Fast solver: Our C++-based solver is substantially faster than other MDP packages available for Python. See details in the documentation.
 * Three optimization algorithms: *Value iteration*, *Policy iteration*, and *Modified policy iteration*.
 * Three value-update methods: *Standard*, *Gauss–Seidel*, *Successive over-relaxation*.
 * Supports sparse matrices.
 * Employs parallel computing.
 
-# Quick start guide
+# Installation
 
-The following shows how to get quickly started with `mdpsolver`.
+## Linux
+
+Install directly from PyPI with:
+
+```
+pip install mdpsolver
+```
 
-## Installation
+After the installation, MDPSolver works *out of the box*.
 
-Download and install `mdpsolver` directly from PyPI. 
+## Windows
+
+Requires [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) (17.9) with MSVC C++ compiler and libraries installed.
+
+After installing Visual Studio (incl. MSVC C++ compiler and libraries), install directly from PyPI with:
 
 ```
 pip install mdpsolver
 ```
 
+# Quick start guide
+
+The following shows how to get quickly started with `mdpsolver`.
+
 ## Usage
 
 Start by specifying the reward function and transition probabilities as lists. The following is an example of a simple MDP containing **three states** and **two actions in each state**.
 
 ```python
 #Import packages
 import mdpsolver
```

### Comparing `mdpsolver-0.9.5/README.md` & `mdpsolver-0.9.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,26 +8,40 @@
 
 * Fast solver: Our C++-based solver is substantially faster than other MDP packages available for Python. See details in the documentation.
 * Three optimization algorithms: *Value iteration*, *Policy iteration*, and *Modified policy iteration*.
 * Three value-update methods: *Standard*, *Gauss–Seidel*, *Successive over-relaxation*.
 * Supports sparse matrices.
 * Employs parallel computing.
 
-# Quick start guide
+# Installation
 
-The following shows how to get quickly started with `mdpsolver`.
+## Linux
+
+Install directly from PyPI with:
+
+```
+pip install mdpsolver
+```
 
-## Installation
+After the installation, MDPSolver works *out of the box*.
 
-Download and install `mdpsolver` directly from PyPI. 
+## Windows
+
+Requires [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) (17.9) with MSVC C++ compiler and libraries installed.
+
+After installing Visual Studio (incl. MSVC C++ compiler and libraries), install directly from PyPI with:
 
 ```
 pip install mdpsolver
 ```
 
+# Quick start guide
+
+The following shows how to get quickly started with `mdpsolver`.
+
 ## Usage
 
 Start by specifying the reward function and transition probabilities as lists. The following is an example of a simple MDP containing **three states** and **two actions in each state**.
 
 ```python
 #Import packages
 import mdpsolver
```

### Comparing `mdpsolver-0.9.5/pyproject.toml` & `mdpsolver-0.9.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "mdpsolver"
-version = "0.9.5"
+version = "0.9.6"
 authors = [
   { name="Anders Reenberg Andersen", email="andersra@live.dk" },
   { name="Jesper Fink Andersen", email="jfan@dtu.dk" },
 ]
 description = "A fast solver for Markov Decision Processes"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mdpsolver-0.9.5/src/mdpsolver/model.py` & `mdpsolver-0.9.6/src/mdpsolver/model.py`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.5/src/mdpsolver/problems/__pycache__/cbmaux.cpython-310.pyc` & `mdpsolver-0.9.6/src/mdpsolver/problems/__pycache__/cbmaux.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.5/src/mdpsolver/problems/__pycache__/tbmaux.cpython-310.pyc` & `mdpsolver-0.9.6/src/mdpsolver/problems/__pycache__/tbmaux.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.5/src/mdpsolver/problems/cbmaux.py` & `mdpsolver-0.9.6/src/mdpsolver/problems/cbmaux.py`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.5/src/mdpsolver/problems/tbmaux.py` & `mdpsolver-0.9.6/src/mdpsolver/problems/tbmaux.py`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.5/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so` & `mdpsolver-0.9.6/src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `mdpsolver-0.9.5/src/mdpsolver.egg-info/PKG-INFO` & `mdpsolver-0.9.6/src/mdpsolver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mdpsolver
-Version: 0.9.5
+Version: 0.9.6
 Summary: A fast solver for Markov Decision Processes
 Author-email: Anders Reenberg Andersen <andersra@live.dk>, Jesper Fink Andersen <jfan@dtu.dk>
 Project-URL: Homepage, https://github.com/areenberg/MDPSolver
 Project-URL: Issues, https://github.com/areenberg/MDPSolver/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,26 +23,40 @@
 
 * Fast solver: Our C++-based solver is substantially faster than other MDP packages available for Python. See details in the documentation.
 * Three optimization algorithms: *Value iteration*, *Policy iteration*, and *Modified policy iteration*.
 * Three value-update methods: *Standard*, *Gauss–Seidel*, *Successive over-relaxation*.
 * Supports sparse matrices.
 * Employs parallel computing.
 
-# Quick start guide
+# Installation
 
-The following shows how to get quickly started with `mdpsolver`.
+## Linux
+
+Install directly from PyPI with:
+
+```
+pip install mdpsolver
+```
 
-## Installation
+After the installation, MDPSolver works *out of the box*.
 
-Download and install `mdpsolver` directly from PyPI. 
+## Windows
+
+Requires [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) (17.9) with MSVC C++ compiler and libraries installed.
+
+After installing Visual Studio (incl. MSVC C++ compiler and libraries), install directly from PyPI with:
 
 ```
 pip install mdpsolver
 ```
 
+# Quick start guide
+
+The following shows how to get quickly started with `mdpsolver`.
+
 ## Usage
 
 Start by specifying the reward function and transition probabilities as lists. The following is an example of a simple MDP containing **three states** and **two actions in each state**.
 
 ```python
 #Import packages
 import mdpsolver
```

### Comparing `mdpsolver-0.9.5/src/mdpsolver.egg-info/SOURCES.txt` & `mdpsolver-0.9.6/src/mdpsolver.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 pyproject.toml
 src/mdpsolver/__init__.py
 src/mdpsolver/model.py
 src/mdpsolver/solvermodule.cp310-win_amd64.pyd
 src/mdpsolver/solvermodule.cp311-win_amd64.pyd
 src/mdpsolver/solvermodule.cp312-win_amd64.pyd
 src/mdpsolver/solvermodule.cpython-310-x86_64-linux-gnu.so
+src/mdpsolver/solvermodule.cpython-311-x86_64-linux-gnu.so
+src/mdpsolver/solvermodule.cpython-312-x86_64-linux-gnu.so
 src/mdpsolver.egg-info/PKG-INFO
 src/mdpsolver.egg-info/SOURCES.txt
 src/mdpsolver.egg-info/dependency_links.txt
 src/mdpsolver.egg-info/top_level.txt
 src/mdpsolver/problems/cbmaux.py
 src/mdpsolver/problems/tbmaux.py
 src/mdpsolver/problems/__pycache__/cbmaux.cpython-310.pyc
```

