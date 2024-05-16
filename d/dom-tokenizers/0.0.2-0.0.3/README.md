# Comparing `tmp/dom_tokenizers-0.0.2.tar.gz` & `tmp/dom_tokenizers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_tokenizers-0.0.2.tar", last modified: Thu May 16 00:40:32 2024, max compression
+gzip compressed data, was "dom_tokenizers-0.0.3.tar", last modified: Thu May 16 09:34:50 2024, max compression
```

## Comparing `dom_tokenizers-0.0.2.tar` & `dom_tokenizers-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.796277 dom_tokenizers-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-16 00:40:32.796277 dom_tokenizers-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:40:32.796277 dom_tokenizers-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/dom_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:50.437112 dom_tokenizers-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-16 09:34:50.433112 dom_tokenizers-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:34:50.437112 dom_tokenizers-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:50.433112 dom_tokenizers-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:50.433112 dom_tokenizers-0.0.3/src/dom_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/src/dom_tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:50.433112 dom_tokenizers-0.0.3/src/dom_tokenizers/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/src/dom_tokenizers/pre_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-05-16 09:34:21.000000 dom_tokenizers-0.0.3/src/dom_tokenizers/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:50.433112 dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-16 09:34:50.000000 dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-16 09:34:50.000000 dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:34:50.000000 dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 09:34:50.000000 dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 09:34:50.000000 dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 09:34:50.000000 dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/top_level.txt
```

### Comparing `dom_tokenizers-0.0.2/LICENSE` & `dom_tokenizers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.2/PKG-INFO` & `dom_tokenizers-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dom-tokenizers
-Version: 0.0.2
-Summary: DOM-aware tokenizers for Hugging Face language models
+Version: 0.0.3
+Summary: DOM-aware tokenizers for 🤗 Hugging Face language models
 Author: Gary Benson
-License: Apache Software License (Apache-2.0)
+License: Apache-2.0
 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -40,20 +40,20 @@
     <a href="https://github.com/gbenson/dom-tokenizers/blob/master/LICENSE">
         <img alt="GitHub" src="https://img.shields.io/github/license/gbenson/dom-tokenizers.svg?color=blue">
     </a>
 </p>
 
 # DOM tokenizers
 
-DOM-aware tokenizers for [🤗 Hugging Face](https://huggingface.co/)
-language models.
+DOM-aware tokenizers for Hugging Face language models.
 
 ## Installation
 
 ### With PIP
+
 ```sh
 pip install dom-tokenizers[train]
 ```
 
 ### From sources
 
 ```sh
@@ -61,11 +61,27 @@
 cd dom-tokenizers
 python3 -m venv .venv
 . .venv/bin/activate
 pip install --upgrade pip
 pip install -e .[dev,train]
 ```
 
-## Train a tokenizer
+## Load a pretrained tokenizer from the Hub
+
+## Train your own
+
+### On the command line
+
+Check everything's working using a small dataset of around 300 examples:
+
+```sh
+train-tokenizer gbenson/interesting-dom-snapshots
+```
+
+Train a tokenizer with a 10,000-token vocabulary using a dataset of
+4,536 examples and upload it to the Hub:
+
 ```sh
-train-tokenizer gbenson/interesting-dom-snapshots -n 10000
+train-tokenizer gbenson/webui-dom-snapshots -n 10000 -N 4536
+huggingface-cli login
+huggingface-cli upload dom-tokenizer-10k
 ```
```

#### html2text {}

```diff
@@ -1,27 +1,31 @@
-Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.2 Summary: DOM-aware
-tokenizers for HuggingÂ Face language models Author: Gary Benson License:
-Apache Software License (Apache-2.0) Project-URL: Homepage, https://github.com/
-gbenson/dom-tokenizers Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Internet :: WWW/HTTP Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Scientific/Engineering :: Information
-Analysis Classifier: Topic :: Text Processing :: Markup :: HTML Requires-
-Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: python-magic Requires-Dist: tokenizers Requires-Dist:
-transformers Provides-Extra: dev Requires-Dist: build; extra == "dev" Requires-
-Dist: flake8; extra == "dev" Provides-Extra: train Requires-Dist: datasets;
-extra == "train" Requires-Dist: pillow; extra == "train"
+Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.3 Summary: DOM-aware
+tokenizers for ð¤Â HuggingÂ Face language models Author: Gary Benson License:
+Apache-2.0 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Education Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
+HTTP Classifier: Topic :: Software Development :: Libraries Classifier: Topic
+:: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Information Analysis Classifier: Topic :: Text
+Processing :: Markup :: HTML Requires-Python: >=3.10 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: python-magic Requires-Dist:
+tokenizers Requires-Dist: transformers Provides-Extra: dev Requires-Dist:
+build; extra == "dev" Requires-Dist: flake8; extra == "dev" Provides-Extra:
+train Requires-Dist: datasets; extra == "train" Requires-Dist: pillow; extra ==
+"train"
 _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]
-# DOMÂ tokenizers DOM-aware tokenizers for [ð¤Â HuggingÂ Face](https://
-huggingface.co/) language models. ## Installation ### With PIP ```sh pip
-install dom-tokenizers[train] ``` ### From sources ```sh git clone https://
-github.com/gbenson/dom-tokenizers.git cd dom-tokenizers python3 -m venv .venv .
-.venv/bin/activate pip install --upgrade pip pip install -e .[dev,train] ``` ##
-Train a tokenizer ```sh train-tokenizer gbenson/interesting-dom-snapshots -
-n 10000 ```
+# DOMÂ tokenizers DOM-aware tokenizers for HuggingÂ Face language models. ##
+Installation ### With PIP ```sh pip install dom-tokenizers[train] ``` ### From
+sources ```sh git clone https://github.com/gbenson/dom-tokenizers.git cd dom-
+tokenizers python3 -m venv .venv . .venv/bin/activate pip install --upgrade pip
+pip install -e .[dev,train] ``` ## Load a pretrained tokenizer from the Hub ##
+Train your own ### On the command line Check everything's working using a small
+dataset of around 300Â examples: ```sh train-tokenizer gbenson/interesting-dom-
+snapshots ``` Train a tokenizer with a 10,000-token vocabulary using a dataset
+of 4,536Â examples and upload it to the Hub: ```sh train-tokenizer gbenson/
+webui-dom-snapshots -n 10000 -N 4536 huggingface-cli login huggingface-cli
+upload dom-tokenizer-10k ```
```

### Comparing `dom_tokenizers-0.0.2/pyproject.toml` & `dom_tokenizers-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "dom-tokenizers"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Gary Benson" }]
-description = "DOM-aware tokenizers for Hugging Face language models"
+description = "DOM-aware tokenizers for 🤗 Hugging Face language models"
 readme = "README.md"
-license = { text = "Apache Software License (Apache-2.0)" }
+license = { text = "Apache-2.0" }
 requires-python = ">=3.10"  # match..case
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py` & `dom_tokenizers-0.0.3/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.2/src/dom_tokenizers/train.py` & `dom_tokenizers-0.0.3/src/dom_tokenizers/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,27 +65,37 @@
 
     # Try and get a dataset length, for the progress tracker.
     if corpus_size is None:
         try:
             corpus_size = len(training_dataset)
         except TypeError:
             pass
+    cs = f"{corpus_size:,}" if corpus_size else "an unknown number of"
+    print(f"Generating {vocab_size:,} tokens from {cs} examples:")
 
     # Train the new tokenizer.
     new_tokenizer = base_tokenizer.train_new_from_iterator(
         text_iterator=get_training_corpus(),
         vocab_size=vocab_size,
         new_special_tokens=new_special_tokens,
         length=corpus_size,
         show_progress=True,
     )
+    new_tokenizer.name_or_path = _pretty_name(new_tokenizer)
 
     return new_tokenizer
 
 
+def _pretty_name(tokenizer=None, *, vocab_size=None, prefix="dom-tokenizer-"):
+    if vocab_size is None:
+        vocab_size = tokenizer.vocab_size
+    pretty_size = _round_and_prefix(vocab_size)
+    return f"{prefix}{pretty_size}"
+
+
 def _round_and_prefix(value):
     """314159 -> '314k'."""
     whole, frac = divmod(log10(value), 1)
     unit_index, whole = divmod(floor(whole), 3)
     value = round(10 ** (whole + frac))
     unit = ([""] + list("kMBTQ"))[unit_index]
     return f"{value}{unit}"
@@ -119,16 +129,15 @@
         "-o", "--output", metavar="DIR", dest="save_directory",
         help=("directory to save the trained tokenizer into"
               " [default: something based on targeted vocabulary size]"))
     args = p.parse_args()
 
     save_directory = args.save_directory
     if save_directory is None:
-        pretty_size = _round_and_prefix(args.vocab_size)
-        save_directory = f"dom-tokenizer-{pretty_size}"
+        save_directory = _pretty_name(vocab_size=args.vocab_size)
         print(f"Output directory: {save_directory}\n")
 
     warnings.filterwarnings("ignore", message=r".*resume_download.*")
 
     tokenizer = train_tokenizer(
         load_dataset(
             args.dataset,
```

### Comparing `dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/PKG-INFO` & `dom_tokenizers-0.0.3/src/dom_tokenizers.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: dom-tokenizers
-Version: 0.0.2
-Summary: DOM-aware tokenizers for Hugging Face language models
+Version: 0.0.3
+Summary: DOM-aware tokenizers for 🤗 Hugging Face language models
 Author: Gary Benson
-License: Apache Software License (Apache-2.0)
+License: Apache-2.0
 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -40,20 +40,20 @@
     <a href="https://github.com/gbenson/dom-tokenizers/blob/master/LICENSE">
         <img alt="GitHub" src="https://img.shields.io/github/license/gbenson/dom-tokenizers.svg?color=blue">
     </a>
 </p>
 
 # DOM tokenizers
 
-DOM-aware tokenizers for [🤗 Hugging Face](https://huggingface.co/)
-language models.
+DOM-aware tokenizers for Hugging Face language models.
 
 ## Installation
 
 ### With PIP
+
 ```sh
 pip install dom-tokenizers[train]
 ```
 
 ### From sources
 
 ```sh
@@ -61,11 +61,27 @@
 cd dom-tokenizers
 python3 -m venv .venv
 . .venv/bin/activate
 pip install --upgrade pip
 pip install -e .[dev,train]
 ```
 
-## Train a tokenizer
+## Load a pretrained tokenizer from the Hub
+
+## Train your own
+
+### On the command line
+
+Check everything's working using a small dataset of around 300 examples:
+
+```sh
+train-tokenizer gbenson/interesting-dom-snapshots
+```
+
+Train a tokenizer with a 10,000-token vocabulary using a dataset of
+4,536 examples and upload it to the Hub:
+
 ```sh
-train-tokenizer gbenson/interesting-dom-snapshots -n 10000
+train-tokenizer gbenson/webui-dom-snapshots -n 10000 -N 4536
+huggingface-cli login
+huggingface-cli upload dom-tokenizer-10k
 ```
```

#### html2text {}

```diff
@@ -1,27 +1,31 @@
-Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.2 Summary: DOM-aware
-tokenizers for HuggingÂ Face language models Author: Gary Benson License:
-Apache Software License (Apache-2.0) Project-URL: Homepage, https://github.com/
-gbenson/dom-tokenizers Classifier: Development Status :: 4 - Beta Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: Apache Software License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
-Topic :: Internet :: WWW/HTTP Classifier: Topic :: Software Development ::
-Libraries Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Scientific/Engineering :: Information
-Analysis Classifier: Topic :: Text Processing :: Markup :: HTML Requires-
-Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
-Requires-Dist: python-magic Requires-Dist: tokenizers Requires-Dist:
-transformers Provides-Extra: dev Requires-Dist: build; extra == "dev" Requires-
-Dist: flake8; extra == "dev" Provides-Extra: train Requires-Dist: datasets;
-extra == "train" Requires-Dist: pillow; extra == "train"
+Metadata-Version: 2.1 Name: dom-tokenizers Version: 0.0.3 Summary: DOM-aware
+tokenizers for ð¤Â HuggingÂ Face language models Author: Gary Benson License:
+Apache-2.0 Project-URL: Homepage, https://github.com/gbenson/dom-tokenizers
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
+Developers Classifier: Intended Audience :: Education Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Programming Language :: Python :: 3.12 Classifier: Topic :: Internet :: WWW/
+HTTP Classifier: Topic :: Software Development :: Libraries Classifier: Topic
+:: Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
+Scientific/Engineering :: Information Analysis Classifier: Topic :: Text
+Processing :: Markup :: HTML Requires-Python: >=3.10 Description-Content-Type:
+text/markdown License-File: LICENSE Requires-Dist: python-magic Requires-Dist:
+tokenizers Requires-Dist: transformers Provides-Extra: dev Requires-Dist:
+build; extra == "dev" Requires-Dist: flake8; extra == "dev" Provides-Extra:
+train Requires-Dist: datasets; extra == "train" Requires-Dist: pillow; extra ==
+"train"
 _[_B_u_i_l_d_]_[_G_i_t_H_u_b_]
-# DOMÂ tokenizers DOM-aware tokenizers for [ð¤Â HuggingÂ Face](https://
-huggingface.co/) language models. ## Installation ### With PIP ```sh pip
-install dom-tokenizers[train] ``` ### From sources ```sh git clone https://
-github.com/gbenson/dom-tokenizers.git cd dom-tokenizers python3 -m venv .venv .
-.venv/bin/activate pip install --upgrade pip pip install -e .[dev,train] ``` ##
-Train a tokenizer ```sh train-tokenizer gbenson/interesting-dom-snapshots -
-n 10000 ```
+# DOMÂ tokenizers DOM-aware tokenizers for HuggingÂ Face language models. ##
+Installation ### With PIP ```sh pip install dom-tokenizers[train] ``` ### From
+sources ```sh git clone https://github.com/gbenson/dom-tokenizers.git cd dom-
+tokenizers python3 -m venv .venv . .venv/bin/activate pip install --upgrade pip
+pip install -e .[dev,train] ``` ## Load a pretrained tokenizer from the Hub ##
+Train your own ### On the command line Check everything's working using a small
+dataset of around 300Â examples: ```sh train-tokenizer gbenson/interesting-dom-
+snapshots ``` Train a tokenizer with a 10,000-token vocabulary using a dataset
+of 4,536Â examples and upload it to the Hub: ```sh train-tokenizer gbenson/
+webui-dom-snapshots -n 10000 -N 4536 huggingface-cli login huggingface-cli
+upload dom-tokenizer-10k ```
```

