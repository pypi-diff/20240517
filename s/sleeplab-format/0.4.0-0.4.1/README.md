# Comparing `tmp/sleeplab_format-0.4.0.tar.gz` & `tmp/sleeplab_format-0.4.1.tar.gz`

## Comparing `sleeplab_format-0.4.0.tar` & `sleeplab_format-0.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/concepts.md
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/contributing.md
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/index.md
--rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/smartsleeplab_logo.png
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/api/extractor.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/api/models.md
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/api/reader.md
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/api/writer.md
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/examples/automatic_sleep_staging.md
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/examples/edf_conversion.md
--rwxr-xr-x   0        0        0    13168 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/figures/fig1.svg
--rwxr-xr-x   0        0        0    39237 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/figures/fig2.svg
--rwxr-xr-x   0        0        0    75810 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/docs/figures/fig3.svg
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/benchmark/README.md
--rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/benchmark/benchmark.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/benchmark/benchmark_out.json
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/benchmark/requirements.txt
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/dod_sleep_staging/README.md
--rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/dod_sleep_staging/convert_data.py
--rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/dod_sleep_staging/dataset.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/dod_sleep_staging/download_data.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/dod_sleep_staging/extractor_config.yml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/dod_sleep_staging/requirements.txt
--rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/dod_sleep_staging/train.py
--rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/sleep_cassette_conversion/README.md
--rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/sleep_cassette_conversion/convert_data.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/examples/sleep_cassette_conversion/requirements.txt
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/__init__.py
--rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/models.py
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/reader.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/version.py
--rw-r--r--   0        0        0     8642 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/extractor/__init__.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/extractor/cli.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/extractor/config.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/extractor/preprocess.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/test_utils/__init__.py
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/src/sleeplab_format/test_utils/fixtures.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/create_datasets.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/test_models.py
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/test_reader.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/test_writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/extractor/__init__.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/extractor/test_extract.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/extractor/test_parse_config.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/tests/extractor/data/example_config.yml
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/LICENSE
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/README.md
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 sleeplab_format-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/concepts.md
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/contributing.md
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/index.md
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/smartsleeplab_logo.png
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/api/extractor.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/api/models.md
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/api/reader.md
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/api/writer.md
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/examples/automatic_sleep_staging.md
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/examples/edf_conversion.md
+-rwxr-xr-x   0        0        0    13168 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/figures/fig1.svg
+-rwxr-xr-x   0        0        0    39237 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/figures/fig2.svg
+-rwxr-xr-x   0        0        0    75810 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/docs/figures/fig3.svg
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/benchmark/README.md
+-rw-r--r--   0        0        0     9726 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/benchmark/benchmark.py
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/benchmark/benchmark_out.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/benchmark/requirements.txt
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/dod_sleep_staging/README.md
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/dod_sleep_staging/convert_data.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/dod_sleep_staging/dataset.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/dod_sleep_staging/download_data.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/dod_sleep_staging/extractor_config.yml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/dod_sleep_staging/requirements.txt
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/dod_sleep_staging/train.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/sleep_cassette_conversion/README.md
+-rw-r--r--   0        0        0     6244 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/sleep_cassette_conversion/convert_data.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/examples/sleep_cassette_conversion/requirements.txt
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/__init__.py
+-rw-r--r--   0        0        0     6488 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/models.py
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/reader.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/version.py
+-rw-r--r--   0        0        0     8750 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/extractor/__init__.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/extractor/cli.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/extractor/config.py
+-rw-r--r--   0        0        0     9503 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/extractor/preprocess.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/test_utils/__init__.py
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/src/sleeplab_format/test_utils/fixtures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/create_datasets.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/test_models.py
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/test_reader.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/test_writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/extractor/__init__.py
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/extractor/test_extract.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/extractor/test_parse_config.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/tests/extractor/data/example_config.yml
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/README.md
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 sleeplab_format-0.4.1/PKG-INFO
```

### Comparing `sleeplab_format-0.4.0/mkdocs.yml` & `sleeplab_format-0.4.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/concepts.md` & `sleeplab_format-0.4.1/docs/concepts.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/contributing.md` & `sleeplab_format-0.4.1/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/index.md` & `sleeplab_format-0.4.1/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Sleeplab-format v0.4.0
+# Sleeplab-format v0.4.1
 
 Sleeplab format (SLF) is a both machine and human-readable format to store and process polysomnography recordings. It provides reader and writer with built-in validation of the data types and structures. SLF was designed for harmonization of datasets from different sources to enable easier application of analysis and machine learning pipelines on multiple datasets.
 
 See [Concepts](concepts.md) and [the paper](https://arxiv.org/abs/2402.06702v1) for detailed description of the format.
 
 ## Installation
```

### Comparing `sleeplab_format-0.4.0/docs/smartsleeplab_logo.png` & `sleeplab_format-0.4.1/docs/smartsleeplab_logo.png`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/api/extractor.md` & `sleeplab_format-0.4.1/docs/api/extractor.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/examples/automatic_sleep_staging.md` & `sleeplab_format-0.4.1/docs/examples/automatic_sleep_staging.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/examples/edf_conversion.md` & `sleeplab_format-0.4.1/docs/examples/edf_conversion.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/figures/fig1.svg` & `sleeplab_format-0.4.1/docs/figures/fig1.svg`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/figures/fig2.svg` & `sleeplab_format-0.4.1/docs/figures/fig2.svg`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/docs/figures/fig3.svg` & `sleeplab_format-0.4.1/docs/figures/fig3.svg`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/benchmark/README.md` & `sleeplab_format-0.4.1/examples/benchmark/README.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/benchmark/benchmark.py` & `sleeplab_format-0.4.1/examples/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/benchmark/benchmark_out.json` & `sleeplab_format-0.4.1/examples/benchmark/benchmark_out.json`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/dod_sleep_staging/README.md` & `sleeplab_format-0.4.1/examples/dod_sleep_staging/README.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/dod_sleep_staging/convert_data.py` & `sleeplab_format-0.4.1/examples/dod_sleep_staging/convert_data.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/dod_sleep_staging/dataset.py` & `sleeplab_format-0.4.1/examples/dod_sleep_staging/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     },
     'emg': {
         'src_name': 'EMG_64Hz',
         'ctype': 'sample_array',
         'fs': 64.0
     },
     'hypnogram': {
-        'src_name': 'manual_consensus_hypnogram.a.parquet',
+        'src_name': 'manual_consensus_hypnogram.a.json',
         'ctype': 'annotation',
         'sampling_interval': 30,
         'return_type': 'segmentation_combined',
         'value_map': {
             'W': 0,
             'N1': 1,
             'N2': 2,
```

### Comparing `sleeplab_format-0.4.0/examples/dod_sleep_staging/download_data.py` & `sleeplab_format-0.4.1/examples/dod_sleep_staging/download_data.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/dod_sleep_staging/extractor_config.yml` & `sleeplab_format-0.4.1/examples/dod_sleep_staging/extractor_config.yml`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/dod_sleep_staging/train.py` & `sleeplab_format-0.4.1/examples/dod_sleep_staging/train.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/sleep_cassette_conversion/README.md` & `sleeplab_format-0.4.1/examples/sleep_cassette_conversion/README.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/examples/sleep_cassette_conversion/convert_data.py` & `sleeplab_format-0.4.1/examples/sleep_cassette_conversion/convert_data.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/src/sleeplab_format/models.py` & `sleeplab_format-0.4.1/src/sleeplab_format/models.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/src/sleeplab_format/reader.py` & `sleeplab_format-0.4.1/src/sleeplab_format/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     Returns:
         All sample arrays in a dictionary.
     """
     sarrs = {}
     for p in subject_dir.iterdir():
         if p.is_dir() and not p.name.startswith('.'):
             with open(p / 'attributes.json', 'rb') as f:
-                raw_data = f.read()
+                raw_data = f.read().decode('utf-8')
                 attributes = ArrayAttributes.model_validate_json(raw_data)
 
             if (p / 'data.npy').exists():
                 # Return a function that returns a memmapped numpy array
                 values_func = lambda _p=p / 'data.npy': np.load(
                     _p, mmap_mode='r', allow_pickle=False)
             elif (p / 'data.parquet').exists():
                 values_func = lambda _p=p / 'data.parquet': pq.read_table(
                     _p)['data'].to_numpy()
             elif (p / 'data.zarr').exists():
-                values_func = lambda _p=p / 'data.zarr': zarr.open(_p, mode='r')
+                values_func = lambda _p=p / 'data.zarr': zarr.load(_p)
             else:
-                raise FileNotFoundError(f'No data.npy or data.parquet in {p}')
+                raise FileNotFoundError(f'No data.npy, data.zarr, or data.parquet in {p}')
 
             assert p.name == attributes.name
             sarrs[p.name] = SampleArray(
                 attributes=attributes, values_func=values_func)
     return sarrs
 
 
@@ -63,21 +63,21 @@
     """
     annotations = {}
     for p in subject_dir.iterdir():
 
         if p.name.endswith(JSON_ANNOTATION_SUFFIX):            
             annotation_name = p.name.removesuffix(JSON_ANNOTATION_SUFFIX)
             with open(p, 'rb') as f:
-                raw_data = f.read()
+                raw_data = f.read().decode('utf-8')
                 annotations[annotation_name] = BaseAnnotations.model_validate_json(raw_data)
         elif p.name.endswith(PARQUET_ANNOTATION_SUFFIX):
             annotation_name = p.name.removesuffix(PARQUET_ANNOTATION_SUFFIX)
             annotation_meta_path = subject_dir / f'{annotation_name}{PARQUET_ANNOTATION_META_SUFFIX}'
 
-            with open(annotation_meta_path, 'r') as f:
+            with open(annotation_meta_path, 'r', encoding='utf-8') as f:
                 ann_dict = json.load(f)
 
             ann_df = pd.read_parquet(p)
             ann_dict['annotations'] = ann_df.to_dict('records')
 
             annotations[annotation_name] = BaseAnnotations.model_validate(ann_dict)
 
@@ -95,15 +95,15 @@
         subject_dir: The subject folder.
         include_annotations: Whether to include the annotations.
 
     Returns:
         The resulting subject.
     """
     with open(subject_dir / 'metadata.json', 'rb') as f:
-        raw_data = f.read()
+        raw_data = f.read().decode('utf-8')
         metadata = SubjectMetadata.model_validate_json(raw_data)
     
     sample_arrays = read_sample_arrays(subject_dir)
 
     if include_annotations:
         annotations = read_annotations(subject_dir)
     else:
@@ -147,15 +147,15 @@
         ds_dir: The dataset root folder.
         series_names: The series included in the resulting dataset.
         include_annotations: Whether to include annotations or only read the sample arrays.
 
     Returns:
         The resulting dataset.
     """
-    with open(ds_dir / 'metadata.json', 'r') as f:
+    with open(ds_dir / 'metadata.json', 'r', encoding='utf-8') as f:
         ds_meta = json.load(f)
 
     assert ds_meta['name'] == ds_dir.name
     if ds_meta['version'] != SLEEPLAB_FORMAT_VERSION:
         logger.warning(
             f'Reading dataset version {ds_meta["version"]} with sleeplab-format version {SLEEPLAB_FORMAT_VERSION}')
```

### Comparing `sleeplab_format-0.4.0/src/sleeplab_format/writer.py` & `sleeplab_format-0.4.1/src/sleeplab_format/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     Arguments:
         subject: The sleeplab_format.models.Subject whose metadata will be saved.
         subject_path: The path to the subject folder.
     """
     metadata_path = subject_path / 'metadata.json'
     metadata_path.write_text(
         subject.metadata.model_dump_json(indent=JSON_INDENT, exclude_none=True),
+        encoding='utf-8'
     )
 
 
 def write_sample_arrays(
         subject: Subject,
         subject_path: Path,
         format: str = 'numpy',
@@ -61,15 +62,15 @@
         assert name == sarr.attributes.name
         sarr_path = subject_path / f'{sarr.attributes.name}'
         sarr_path.mkdir(exist_ok=True)
         
         # Write the attributes
         attr_path = sarr_path / 'attributes.json'
         attr_path.write_text(
-            sarr.attributes.model_dump_json(indent=JSON_INDENT, exclude_none=True))
+            sarr.attributes.model_dump_json(indent=JSON_INDENT, exclude_none=True), encoding='utf-8')
 
         arr = sarr.values_func()
         if format == 'numpy':
             # Write the array
             arr_fname = 'data.npy'
             np.save(sarr_path / arr_fname, arr, allow_pickle=False)
         elif format == 'zarr':
@@ -115,15 +116,16 @@
     for k, v in subject.annotations.items():
         _msg = f'Annotation key should equal to "{v.scorer}_{v.type}", got "{k}"'
         assert k == f'{v.scorer}_{v.type}', _msg
         
         if format == 'json':
             json_path = subject_path / f'{k}{JSON_ANNOTATION_SUFFIX}'
             json_path.write_text(
-                v.model_dump_json(exclude_none=True, indent=JSON_INDENT)
+                v.model_dump_json(exclude_none=True, indent=JSON_INDENT),
+                encoding='utf-8'
             )
         else:
             # Write the actual annotations in parquet, metadata in json
             metadata_path = subject_path / f'{k}{PARQUET_ANNOTATION_META_SUFFIX}'
             pq_path = subject_path / f'{k}{PARQUET_ANNOTATION_SUFFIX}'
             
             ann_dict = v.model_dump()
@@ -210,15 +212,17 @@
     logger.info(f'Creating dataset dir {dataset_path}...')
     dataset_path.mkdir(parents=True, exist_ok=True)
 
     # Write the dataset metadata
     dataset.version = SLEEPLAB_FORMAT_VERSION
     metadata_path = dataset_path / 'metadata.json'
     metadata_path.write_text(
-        dataset.model_dump_json(exclude={'series'}, indent=JSON_INDENT))
+        dataset.model_dump_json(exclude={'series'}, indent=JSON_INDENT),
+        encoding='utf-8'
+    )
 
     # Write the series
     for name, series in dataset.series.items():
         assert name == series.name
         logger.info(f'Writing data for series {series.name}...')
         series_path = dataset_path / series.name
         series_path.mkdir(exist_ok=True)
```

### Comparing `sleeplab_format-0.4.0/src/sleeplab_format/extractor/cli.py` & `sleeplab_format-0.4.1/src/sleeplab_format/extractor/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """CLI for extracting and preprocessing a subset of data in sleeplab format."""
 import argparse
+import json
 import logging
 
 from pathlib import Path
 from sleeplab_format.extractor import config, preprocess
 from sleeplab_format import reader, writer
 
 
@@ -19,27 +20,35 @@
         cfg: The extractor config.
     """ 
     logger.info(f'Reading dataset from {src_dir}')
     series_names = [series_config.name for series_config in cfg.series_configs]
     ds = reader.read_dataset(src_dir, series_names=series_names)
     
     updated_series = {}
+    series_skipped = {}
 
     for series_config in cfg.series_configs:
         logger.info(f'Creating updated series {series_config.name}')
-        _series = preprocess.process_series(ds.series[series_config.name], series_config)
+        _series, _skipped = preprocess.process_series(ds.series[series_config.name], series_config)
         updated_series[series_config.name] = _series
+        series_skipped[series_config.name] = _skipped
     
     logger.info('Creating updated Dataset')
     ds = ds.model_copy(update={'name': cfg.new_dataset_name, 'series': updated_series})
 
     logger.info(f'Applying preprocessing and writing dataset to {dst_dir}')
     writer.write_dataset(
         ds, dst_dir, annotation_format=cfg.annotation_format, array_format=cfg.array_format)
 
+    if series_skipped != {}:
+        skipped_path = Path(dst_dir) / ds.name / '.extractor_skipped_subjects.json'
+        logger.info(f'Writing skipped subject IDs and reasons to {skipped_path}')
+        with open(skipped_path, 'w') as f:
+            json.dump(series_skipped, f, indent=2)
+
 
 def get_parser():
     parser = argparse.ArgumentParser()
 
     parser.add_argument('-s', '--src_dir', required=True)
     parser.add_argument('-d', '--dst_dir', required=True)
     parser.add_argument('-c', '--config_path', required=True)
```

### Comparing `sleeplab_format-0.4.0/src/sleeplab_format/extractor/config.py` & `sleeplab_format-0.4.1/src/sleeplab_format/extractor/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,35 +7,40 @@
 
 class ArrayAction(BaseModel, extra='forbid'):
     name: str
     method: str
 
     # The name of an optional reference signal
     ref_name: str | None = None
+    alt_ref_names: list[str] | None = None
     
     kwargs: dict[str, Any] = {}
     updated_attributes: dict[str, Any] | None = None
 
 
 class ArrayConfig(BaseModel, extra='forbid'):
     name: str
+    alt_names: list[str] | None = None
     actions: list[ArrayAction] | None = None
 
 
 class FilterCond(BaseModel, extra='forbid'):
     name: str
     method: str
     kwargs: dict[str, Any] | None = None
 
 
 class SeriesConfig(BaseModel, extra='forbid'):
     name: str
     array_configs: list[ArrayConfig]
     filter_conds: list[FilterCond] | None = None
 
+    # If given, ignore subjects who do not have all of these signals in the resulting dataset
+    required_result_array_names: list[str] | None = None
+
 
 class DatasetConfig(BaseModel, extra='forbid'):
     new_dataset_name: str
     series_configs: list[SeriesConfig]
     annotation_format: str = 'json'
     array_format: str = 'numpy'
```

### Comparing `sleeplab_format-0.4.0/src/sleeplab_format/extractor/preprocess.py` & `sleeplab_format-0.4.1/src/sleeplab_format/extractor/preprocess.py`

 * *Files 26% similar despite different names*

```diff
@@ -45,15 +45,23 @@
         cfg: ArrayConfig) -> SampleArray:
     """Process a SampleArray according to the actions defined in cfg."""
     # Create a deep copy not to modify the source dataset
     arr = arr_dict[cfg.name].model_copy(deep=True)
 
     for action in cfg.actions:
         if action.ref_name is not None:
-            ref_func = arr_dict[action.ref_name].values_func
+            if action.ref_name not in arr_dict.keys() and action.alt_ref_names is not None:
+                alt_name_set = set(action.alt_ref_names).intersection(set(arr_dict.keys()))
+                if alt_name_set != set():
+                    action.ref_name = alt_name_set.pop()
+            try:
+                ref_func = arr_dict[action.ref_name].values_func
+            except KeyError:
+                logger.warning(f'Discarding {cfg.name} since reference {[action.ref_name] + (action.alt_ref_names or [])} was not found in {arr_dict.keys()}')
+                return None
         else:
             ref_func = None
 
         _values_func = chain_action(
             arr.values_func,
             arr.attributes,
             action,
@@ -63,45 +71,76 @@
 
     return arr
 
 
 def process_subject(subject: Subject, cfg: SeriesConfig) -> Subject | None:
     """Process all conditions and sample arrays for a single subject."""
     _sample_arrays = {}
+    _cfg = cfg.model_copy(deep=True)
 
-    if cfg.filter_conds is not None:
-        for cond in cfg.filter_conds:
+    if _cfg.filter_conds is not None:
+        for cond in _cfg.filter_conds:
             _func = import_function(cond.method)
             if cond.kwargs is None:
                 bool_keep = _func(subject)
             else:
                 bool_keep = _func(subject, **cond.kwargs)
 
             if not bool_keep:
-                logger.info(f'Skipping subject {subject.metadata.subject_id} due to filter_cond {cond.name}')
-                return None
+                _msg = f'Skipping subject {subject.metadata.subject_id} due to filter_cond {cond.name}'
+                logger.info(_msg)
+                return None, _msg
+
+    for array_cfg in _cfg.array_configs:
+        if array_cfg.alt_names is not None:
+            alt_name_set = set(array_cfg.alt_names).intersection(set(subject.sample_arrays.keys()))
+        else:
+            alt_name_set = set()
+
+        if array_cfg.name not in subject.sample_arrays.keys() and alt_name_set != set():
+            array_cfg.name = alt_name_set.pop()
 
-    for array_cfg in cfg.array_configs:
         if array_cfg.name in subject.sample_arrays.keys():
             _arr = process_array(subject.sample_arrays, array_cfg)
-            _sample_arrays[_arr.attributes.name] = _arr
+            if _arr is not None:
+                _sample_arrays[_arr.attributes.name] = _arr
         else:
-            logger.warn(f'{array_cfg.name} not in sample arrays for subject {subject.metadata.subject_id}')
+            logger.warning(f'{[array_cfg.name] + (array_cfg.alt_names or [])} not in sample arrays for subject {subject.metadata.subject_id}')
+
+    if cfg.required_result_array_names is not None:
+        # Ignore subjects with missing required arrays
+        array_names = set([a.attributes.name for a in _sample_arrays.values()])
+        required = set(_cfg.required_result_array_names)
+        if not required.issubset(array_names):
+            _msg = f'Skipping subject {subject.metadata.subject_id} with missing sample arrays. Required: {required}, missing: {required - array_names}'
+            logger.warning(_msg)
+            return None, _msg
 
     return subject.model_copy(update={'sample_arrays': _sample_arrays})
 
 
 def process_series(series: Series, cfg: SeriesConfig) -> Series:
+    # A handled skip is a subject for which process_subject returns None,
+    # unhandled is a subject for which process_subject throws an exception
+    skipped = {'handled': {}, 'unhandled': {}}
     updated_subjects = {}
     for sid, subj in series.subjects.items():
-        _subj = process_subject(subj, cfg)
-        if _subj is not None:
-            updated_subjects[sid] = _subj
+        try:
+            _subj = process_subject(subj, cfg)
+            match _subj:
+                case Subject():
+                    updated_subjects[sid] = _subj
+                case (None, str(msg)):
+                    skipped['handled'][sid] = msg
+                case _:
+                    skipped['unhandled'][sid] = f'process_subject(): incorrect return type {repr(_subj)}'
+        except Exception as e:
+            skipped['unhandled'][sid] = repr(e)
 
-    return series.model_copy(update={'subjects': updated_subjects})
+    return series.model_copy(update={'subjects': updated_subjects}), skipped
 
 
 def filter_by_tst(
         subject: Subject,
         hypnogram_key: str,
         min_tst_sec: float) -> bool:
     allowed_stages = [
```

### Comparing `sleeplab_format-0.4.0/src/sleeplab_format/test_utils/fixtures.py` & `sleeplab_format-0.4.1/src/sleeplab_format/test_utils/fixtures.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/tests/conftest.py` & `sleeplab_format-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/tests/create_datasets.py` & `sleeplab_format-0.4.1/tests/create_datasets.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/tests/test_models.py` & `sleeplab_format-0.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/tests/test_reader.py` & `sleeplab_format-0.4.1/tests/test_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -67,14 +67,22 @@
                          annotation_format='parquet',
                          array_format='parquet')
 
     ds_read = reader.read_dataset(ds_dir / dataset.name)
     _assert_datasets_equal(dataset, ds_read)
 
 
+def test_write_read_utf8(dataset: Dataset, tmp_path: Path):
+    ds_dir = tmp_path / 'datasets'
+    dataset.series['series1'].subjects['10001'].annotations['study_logs'].annotations[0].name = '\u0394'
+    writer.write_dataset(dataset, ds_dir)
+    ds_read = reader.read_dataset(ds_dir / dataset.name)
+    _assert_datasets_equal(dataset, ds_read)
+
+
 def test_read_write(tmp_path: Path):
     tests_ds_dir = Path(__file__).parent / 'datasets'
     ds_read = reader.read_dataset(tests_ds_dir / 'dataset1')
 
     ds_dir = tmp_path / 'datasets'
     writer.write_dataset(ds_read, ds_dir)
```

### Comparing `sleeplab_format-0.4.0/tests/test_writer.py` & `sleeplab_format-0.4.1/tests/test_writer.py`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/tests/extractor/data/example_config.yml` & `sleeplab_format-0.4.1/tests/extractor/data/example_config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # You must give a new name for the extracted dataset
 new_dataset_name: "dataset1_extracted"
 
 # annotation_format can be "parquet" or "json".
-annotation_format: "parquet"
+annotation_format: "json"
 
-# array_format can be "numpy" or "parquet".
+# array_format can be "numpy", "parquet" or "zarr".
 array_format: "numpy"
 
 # A separate config must be defined for each series that is desired to be extracted.
 series_configs:
 
   - name: "series1"
     
@@ -49,20 +49,20 @@
 
       - name: "s2"
         
         actions:
           - name: "resample"
             method: "sleeplab_format.extractor.preprocess.resample_polyphase"
             kwargs: {"fs_new": 32}
-            updated_attributes: {"sampling_rate": 32}
+            updated_attributes: {"sampling_rate": 32, "name": "s2s1_32Hz"}
 
           - name: "subtract_reference"
             method: "sleeplab_format.extractor.preprocess.sub_ref"
             ref_name: "s1"
-            updated_attributes: {"name": "s2s1_32Hz"}
+            #updated_attributes: {"name": "s2s1_32Hz"}
     
       - name: "s1"
         
         actions:
           - name: "upsample_linear"
             method: "sleeplab_format.extractor.preprocess.upsample_linear"
             kwargs: {"fs_new": 64}
```

### Comparing `sleeplab_format-0.4.0/.gitignore` & `sleeplab_format-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/LICENSE` & `sleeplab_format-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/README.md` & `sleeplab_format-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/pyproject.toml` & `sleeplab_format-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sleeplab_format-0.4.0/PKG-INFO` & `sleeplab_format-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sleeplab-format
-Version: 0.4.0
+Version: 0.4.1
 Summary: An interoperable and harmonized format for polysomnography recordings.
 Project-URL: Documentation, https://github.com/UEF-SmartSleepLab/sleeplab-format#readme
 Project-URL: Issues, https://github.com/UEF-SmartSleepLab/sleeplab-format/issues
 Project-URL: Source, https://github.com/UEF-SmartSleepLab/sleeplab-format
 Author-email: Riku Huttunen <riku.huttunen@uef.fi>
 License-Expression: MIT
 License-File: LICENSE
```

