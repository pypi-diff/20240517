# Comparing `tmp/dom_tokenizers-0.0.4.tar.gz` & `tmp/dom_tokenizers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_tokenizers-0.0.4.tar", last modified: Thu May 16 22:33:05 2024, max compression
+gzip compressed data, was "dom_tokenizers-0.0.5.tar", last modified: Fri May 17 09:42:28 2024, max compression
```

## Comparing `dom_tokenizers-0.0.4.tar` & `dom_tokenizers-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.889274 dom_tokenizers-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.889274 dom_tokenizers-0.0.4/src/dom_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/src/dom_tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/src/dom_tokenizers/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/src/dom_tokenizers/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/src/dom_tokenizers/internal/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/src/dom_tokenizers/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/src/dom_tokenizers/pre_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/src/dom_tokenizers/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-16 22:33:05.000000 dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-16 22:33:05.000000 dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:33:05.000000 dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 22:33:05.000000 dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 22:33:05.000000 dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 22:33:05.000000 dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:33:05.893274 dom_tokenizers-0.0.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/tests/resources/svg-in-base64.html
--rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/tests/resources/svg-in-base64.json
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/tests/test_train_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-16 22:32:30.000000 dom_tokenizers-0.0.4/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.046356 dom_tokenizers-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-17 09:42:28.046356 dom_tokenizers-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:42:28.046356 dom_tokenizers-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.038356 dom_tokenizers-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.038356 dom_tokenizers-0.0.5/src/dom_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/src/dom_tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.042356 dom_tokenizers-0.0.5/src/dom_tokenizers/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/src/dom_tokenizers/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/src/dom_tokenizers/internal/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.042356 dom_tokenizers-0.0.5/src/dom_tokenizers/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/src/dom_tokenizers/pre_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6010 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/src/dom_tokenizers/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.042356 dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-17 09:42:28.000000 dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-17 09:42:28.000000 dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:42:28.000000 dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-17 09:42:28.000000 dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-17 09:42:28.000000 dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 09:42:28.000000 dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.042356 dom_tokenizers-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.042356 dom_tokenizers-0.0.5/tests/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/pre_tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.042356 dom_tokenizers-0.0.5/tests/pre_tokenizers/dom_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/pre_tokenizers/dom_snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/pre_tokenizers/dom_snapshot/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:42:28.042356 dom_tokenizers-0.0.5/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/resources/raw-browser-response.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/resources/raw-browser-response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47499 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/resources/svg-in-base64.html
+-rw-r--r--   0 runner    (1001) docker     (127)    48905 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/resources/svg-in-base64.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/test_train_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-17 09:41:44.000000 dom_tokenizers-0.0.5/tests/util.py
```

### Comparing `dom_tokenizers-0.0.4/LICENSE` & `dom_tokenizers-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.4/PKG-INFO` & `dom_tokenizers-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom-tokenizers
-Version: 0.0.4
+Version: 0.0.5
 Summary: DOM-aware tokenizers for 🤗 Hugging Face language models
 Author: Gary Benson
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -27,14 +27,15 @@
 Requires-Dist: tokenizers
 Requires-Dist: transformers
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: datasets; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: train
 Requires-Dist: datasets; extra == "train"
 Requires-Dist: pillow; extra == "train"
 
 <p style="float: right">
     <a href="https://badge.fury.io/py/dom-tokenizers">
          <img alt="Build" src="https://badge.fury.io/py/dom-tokenizers.svg">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.4 Summary: DOM-aware
+Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.5 Summary: DOM-aware
 tokenizers for ð¤Â HuggingÂ Face language models Author: Gary Benson License:
 Apache-2.0 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -11,17 +11,17 @@
 HTTP Classifier: Topic :: Software Development :: Libraries Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Text
 Processing :: Markup :: HTML Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: python-magic Requires-Dist:
 tokenizers Requires-Dist: transformers Provides-Extra: dev Requires-Dist:
 build; extra == "dev" Requires-Dist: datasets; extra == "dev" Requires-Dist:
-flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Provides-Extra:
-train Requires-Dist: datasets; extra == "train" Requires-Dist: pillow; extra ==
-"train"
+flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
+pytest-cov; extra == "dev" Provides-Extra: train Requires-Dist: datasets; extra
+== "train" Requires-Dist: pillow; extra == "train"
 _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]
 # DOMÂ tokenizers DOM-aware tokenizers for HuggingÂ Face language models. ##
 Installation ### With PIP ```sh pip install dom-tokenizers[train] ``` ### From
 sources ```sh git clone https://github.com/gbenson/dom-tokenizers.git cd dom-
 tokenizers python3 -m venv .venv . .venv/bin/activate pip install --upgrade pip
 pip install -e .[dev,train] ``` ## Load a pretrained tokenizer from the Hub ##
 Train your own ### On the command line Check everything's working using a small
```

### Comparing `dom_tokenizers-0.0.4/README.md` & `dom_tokenizers-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.4/pyproject.toml` & `dom_tokenizers-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dom-tokenizers"
-version = "0.0.4"
+version = "0.0.5"
 authors = [{ name = "Gary Benson" }]
 description = "DOM-aware tokenizers for 🤗 Hugging Face language models"
 readme = "README.md"
 license = { text = "Apache-2.0" }
 requires-python = ">=3.10"  # match..case
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -35,25 +35,27 @@
 
 [project.optional-dependencies]
 dev = [
     "build",
     "datasets",
     "flake8",
     "pytest",
+    "pytest-cov",
 ]
 train = [
     "datasets",
     "pillow",
 ]
 
 [project.scripts]
 train-tokenizer = "dom_tokenizers.train:main"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
+addopts = "--cov=dom_tokenizers"
 filterwarnings = [
     "error",
     "ignore:`resume_download` is deprecated:FutureWarning",
 ]
```

### Comparing `dom_tokenizers-0.0.4/src/dom_tokenizers/internal/transformers.py` & `dom_tokenizers-0.0.5/src/dom_tokenizers/internal/transformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 __orig_val = os.environ.get(__var_name)
 os.environ[__var_name] = "1"
 try:
     from transformers import AutoTokenizer  # noqa: F401
 finally:
     if __orig_val is None:
         os.environ.pop(__var_name)
-    else:
+    else:  # pragma: no cover
         os.environ[__var_name] = __orig_val
     del __var_name, __orig_val, os
```

### Comparing `dom_tokenizers-0.0.4/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py` & `dom_tokenizers-0.0.5/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,19 @@
     def pre_tokenize(self, pretok: PreTokenizedString):
         """Pre-tokenize a :class:`~tokenizers.PyPreTokenizedString` in-place.
         """
         pretok.split(self._split_json)
 
     def _split_json(self, i: int, s: NormalizedString) -> List[NormalizedString]:
         snapshot = json.loads(s.normalized)
+
+        # Unpack the snapshot if what we have is a raw browser response
+        if not any(key in snapshot for key in ("documents", "strings")):
+            snapshot = snapshot.get("result", snapshot)
+
         return list(chain.from_iterable(self._split_serialized(snapshot)))
 
     def _split_serialized(self, snapshot: dict) -> Iterable[List[NormalizedString]]:
         emitter = TokenEmitter(self, snapshot)
         elem_token = [NormalizedString(self.elem_token)]
         attr_token = [NormalizedString(self.attr_token)]
```

### Comparing `dom_tokenizers-0.0.4/src/dom_tokenizers/train.py` & `dom_tokenizers-0.0.5/src/dom_tokenizers/train.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/PKG-INFO` & `dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dom-tokenizers
-Version: 0.0.4
+Version: 0.0.5
 Summary: DOM-aware tokenizers for 🤗 Hugging Face language models
 Author: Gary Benson
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -27,14 +27,15 @@
 Requires-Dist: tokenizers
 Requires-Dist: transformers
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: datasets; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
 Provides-Extra: train
 Requires-Dist: datasets; extra == "train"
 Requires-Dist: pillow; extra == "train"
 
 <p style="float: right">
     <a href="https://badge.fury.io/py/dom-tokenizers">
          <img alt="Build" src="https://badge.fury.io/py/dom-tokenizers.svg">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.4 Summary: DOM-aware
+Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.5 Summary: DOM-aware
 tokenizers for ð¤Â HuggingÂ Face language models Author: Gary Benson License:
 Apache-2.0 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -11,17 +11,17 @@
 HTTP Classifier: Topic :: Software Development :: Libraries Classifier: Topic
 :: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
 Scientific/Engineering :: Information Analysis Classifier: Topic :: Text
 Processing :: Markup :: HTML Requires-Python: >=3.10 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: python-magic Requires-Dist:
 tokenizers Requires-Dist: transformers Provides-Extra: dev Requires-Dist:
 build; extra == "dev" Requires-Dist: datasets; extra == "dev" Requires-Dist:
-flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Provides-Extra:
-train Requires-Dist: datasets; extra == "train" Requires-Dist: pillow; extra ==
-"train"
+flake8; extra == "dev" Requires-Dist: pytest; extra == "dev" Requires-Dist:
+pytest-cov; extra == "dev" Provides-Extra: train Requires-Dist: datasets; extra
+== "train" Requires-Dist: pillow; extra == "train"
 _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]
 # DOMÂ tokenizers DOM-aware tokenizers for HuggingÂ Face language models. ##
 Installation ### With PIP ```sh pip install dom-tokenizers[train] ``` ### From
 sources ```sh git clone https://github.com/gbenson/dom-tokenizers.git cd dom-
 tokenizers python3 -m venv .venv . .venv/bin/activate pip install --upgrade pip
 pip install -e .[dev,train] ``` ## Load a pretrained tokenizer from the Hub ##
 Train your own ### On the command line Check everything's working using a small
```

### Comparing `dom_tokenizers-0.0.4/src/dom_tokenizers.egg-info/SOURCES.txt` & `dom_tokenizers-0.0.5/src/dom_tokenizers.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,9 +15,15 @@
 src/dom_tokenizers/internal/transformers.py
 src/dom_tokenizers/pre_tokenizers/__init__.py
 src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
 tests/__init__.py
 tests/conftest.py
 tests/test_train_tokenizer.py
 tests/util.py
+tests/pre_tokenizers/__init__.py
+tests/pre_tokenizers/dom_snapshot/__init__.py
+tests/pre_tokenizers/dom_snapshot/conftest.py
+tests/pre_tokenizers/dom_snapshot/test_pre_tokenizer.py
+tests/resources/raw-browser-response.html
+tests/resources/raw-browser-response.json
 tests/resources/svg-in-base64.html
 tests/resources/svg-in-base64.json
```

### Comparing `dom_tokenizers-0.0.4/tests/resources/svg-in-base64.html` & `dom_tokenizers-0.0.5/tests/resources/svg-in-base64.html`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.4/tests/resources/svg-in-base64.json` & `dom_tokenizers-0.0.5/tests/resources/svg-in-base64.json`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.4/tests/util.py` & `dom_tokenizers-0.0.5/tests/util.py`

 * *Files identical despite different names*

