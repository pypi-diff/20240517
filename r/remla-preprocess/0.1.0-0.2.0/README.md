# Comparing `tmp/remla_preprocess-0.1.0.tar.gz` & `tmp/remla_preprocess-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla_preprocess-0.1.0.tar", max compression
+gzip compressed data, was "remla_preprocess-0.2.0.tar", max compression
```

## Comparing `remla_preprocess-0.1.0.tar` & `remla_preprocess-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1072 2024-05-13 11:15:32.463915 remla_preprocess-0.1.0/LICENSE
--rw-r--r--   0        0        0     1346 2024-05-13 11:15:32.463915 remla_preprocess-0.1.0/README.md
--rw-r--r--   0        0        0      623 2024-05-13 11:16:17.948275 remla_preprocess-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 11:15:32.463915 remla_preprocess-0.1.0/remla_preprocess/__init__.py
--rw-r--r--   0        0        0     3998 2024-05-13 11:15:32.463915 remla_preprocess-0.1.0/remla_preprocess/pre_processing.py
--rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 remla_preprocess-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-17 21:39:38.729625 remla_preprocess-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1361 2024-05-17 21:39:38.729625 remla_preprocess-0.2.0/README.md
+-rw-r--r--   0        0        0      666 2024-05-17 21:40:22.918142 remla_preprocess-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 21:39:38.729625 remla_preprocess-0.2.0/remla_preprocess/__init__.py
+-rw-r--r--   0        0        0     4365 2024-05-17 21:39:38.729625 remla_preprocess-0.2.0/remla_preprocess/pre_processing.py
+-rw-r--r--   0        0        0     2144 1970-01-01 00:00:00.000000 remla_preprocess-0.2.0/PKG-INFO
```

### Comparing `remla_preprocess-0.1.0/LICENSE` & `remla_preprocess-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `remla_preprocess-0.1.0/README.md` & `remla_preprocess-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # lib-ml
 
-This Python library is tailored for preprocessing text data in machine learning. It provides functions for tokenizing data, padding sequences, and encoding labels, all essential for training ML models. Additionally, it enables data downloading from Google Drive and facilitates storing and loading data in various formats from disk. The library is accessible on PyPI and can be seamlessly integrated into your projects.
+This Python library is designed for preprocessing text data in machine learning. It provides functions for tokenizing data, padding sequences, and encoding labels, all essential for training ML models. Additionally, it enables data downloading from Google Drive and facilitates storing and loading data in various formats from disk. The library is accessible on PyPI and can be seamlessly integrated into your projects.
 
 ## Features
 
 - **Data Tokenization:** Convert text into sequences of integers.
 - **Sequence Padding:** Pad sequences to a consistent fixed length. 
 - **Label Encoding:** Convert labels into numerical format.
 - **Data Storage:** Store data to given path under selected format.
@@ -19,15 +19,15 @@
 ```
 
 ## Usage 
 
 Example of how to use `lib-ml` for text processing: 
 
 ```python
-from remla_preprocessing import MLPreprocessor
+from remla_preprocessing.pre_processing import MLPreprocessor
 
 # Instantiate the MLPreprocessor class
 preprocessor = MLPreprocessor()
 
 # Now you can use the functions of the MLPreprocessor class
 preprocessor.tokenize_pad_encode_data(train_data, validation_data, test_data)
 ```
```

### Comparing `remla_preprocess-0.1.0/pyproject.toml` & `remla_preprocess-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "remla_preprocess"
-version = "v0.1.0"
+version = "v0.2.0"
 description = "Pre-processing library for ML models"
 authors = ["Razvan Mihai Popescu <R.Popescu-3@student.tudelft.nl>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
@@ -21,7 +21,10 @@
 [tool.poetry.group.dev.dependencies]
 flake8 = "^7.0.0"
 pylint = "^3.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pylint]
+disable = ["E0401", "R0914"]
```

### Comparing `remla_preprocess-0.1.0/remla_preprocess/pre_processing.py` & `remla_preprocess-0.2.0/remla_preprocess/pre_processing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# pylint: disable=E0401,R0914
-
 """
 Data preprocessing for ML model
 """
 
+import json
 import pickle
 import gdown
 import pandas as pd
 from tensorflow.keras.preprocessing.text import Tokenizer
 from sklearn.preprocessing import LabelEncoder
 from keras.preprocessing.sequence import pad_sequences
 
 
 class MLPreprocessor:
     """
     Class for preprocessing data for ML model
     """
+
     def __init__(self, seq_len=200, tok_path=None, enc_path=None):
         self.sequence_length = seq_len
         if tok_path:
-            self.tokenizer = MLPreprocessor.load_pkl_data(tok_path)
+            self.tokenizer = MLPreprocessor.load_pkl(tok_path)
         else:
             self.tokenizer = Tokenizer(lower=True,
                                        char_level=True,
                                        oov_token="-n-")
         if enc_path:
-            self.encoder = MLPreprocessor.load_pkl_data(enc_path)
+            self.encoder = MLPreprocessor.load_pkl(enc_path)
         else:
             self.encoder = LabelEncoder()
 
     def split_data_content(self, content):
         """
         Create dataframe from raw data
         """
@@ -93,45 +93,62 @@
     def get_data_from_gdrive(file_id, output):
         """
         Download data from Google Drive
         """
         gdown.download(file_id, output=output)
 
     @staticmethod
-    def save_data_as_pkl(data, path):
+    def save_pkl(data, path):
         """
         Save data to given path into pickle format
         """
-        with open(path, "wb", encoding="utf-8") as f:
+        with open(path, "wb") as f:
             pickle.dump(data, f)
 
     @staticmethod
     def save_csv(df, file_path, index=False):
         """
         Save a pandas DataFrame to a CSV file for a given path
         """
         df.to_csv(file_path, index=index)
 
     @staticmethod
-    def load_pkl_data(path):
+    def save_json(data, path, indent):
+        """
+        Save data to given path into json format
+        """
+        with open(path, "w", encoding="utf-8") as file:
+            json.dump(data, file, indent=indent)
+
+    @staticmethod
+    def load_pkl(path):
         """
         Load pickle data from given path
         """
-        with open(path, "rb", encoding="utf-8") as file:
+        with open(path, "rb") as file:
             return pickle.load(file)
 
     @staticmethod
-    def load_csv_data(path):
+    def load_csv(path):
         """
         Load csv data from given path
         """
         data = pd.read_csv(path)
         return data
 
     @staticmethod
-    def load_txt_data(path):
+    def load_txt(path):
         """
         Load txt data from given path
         """
         with open(path, "r", encoding="utf-8") as file:
             data = file.read()
         return data
+
+    @staticmethod
+    def load_json(path):
+        """
+        Load json data from given path
+        """
+        with open(path, "r", encoding="utf-8") as file:
+            data = json.load(file)
+        return data
```

### Comparing `remla_preprocess-0.1.0/PKG-INFO` & `remla_preprocess-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remla_preprocess
-Version: 0.1.0
+Version: 0.2.0
 Summary: Pre-processing library for ML models
 License: MIT
 Author: Razvan Mihai Popescu
 Author-email: R.Popescu-3@student.tudelft.nl
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,15 @@
 Requires-Dist: tensorflow (==2.8.0)
 Requires-Dist: tensorflow-io-gcs-filesystem (==0.24.0)
 Requires-Dist: twine (>=5.0.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # lib-ml
 
-This Python library is tailored for preprocessing text data in machine learning. It provides functions for tokenizing data, padding sequences, and encoding labels, all essential for training ML models. Additionally, it enables data downloading from Google Drive and facilitates storing and loading data in various formats from disk. The library is accessible on PyPI and can be seamlessly integrated into your projects.
+This Python library is designed for preprocessing text data in machine learning. It provides functions for tokenizing data, padding sequences, and encoding labels, all essential for training ML models. Additionally, it enables data downloading from Google Drive and facilitates storing and loading data in various formats from disk. The library is accessible on PyPI and can be seamlessly integrated into your projects.
 
 ## Features
 
 - **Data Tokenization:** Convert text into sequences of integers.
 - **Sequence Padding:** Pad sequences to a consistent fixed length. 
 - **Label Encoding:** Convert labels into numerical format.
 - **Data Storage:** Store data to given path under selected format.
@@ -41,15 +41,15 @@
 ```
 
 ## Usage 
 
 Example of how to use `lib-ml` for text processing: 
 
 ```python
-from remla_preprocessing import MLPreprocessor
+from remla_preprocessing.pre_processing import MLPreprocessor
 
 # Instantiate the MLPreprocessor class
 preprocessor = MLPreprocessor()
 
 # Now you can use the functions of the MLPreprocessor class
 preprocessor.tokenize_pad_encode_data(train_data, validation_data, test_data)
 ```
```

