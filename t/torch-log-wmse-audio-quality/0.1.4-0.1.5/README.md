# Comparing `tmp/torch_log_wmse_audio_quality-0.1.4.tar.gz` & `tmp/torch_log_wmse_audio_quality-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_log_wmse_audio_quality-0.1.4.tar", last modified: Thu May 16 18:13:05 2024, max compression
+gzip compressed data, was "torch_log_wmse_audio_quality-0.1.5.tar", last modified: Fri May 17 19:10:28 2024, max compression
```

## Comparing `torch_log_wmse_audio_quality-0.1.4.tar` & `torch_log_wmse_audio_quality-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 18:13:05.558204 torch_log_wmse_audio_quality-0.1.4/
--rw-r--r--   0 chris      (501) staff       (20)    11370 2024-05-15 20:08:40.000000 torch_log_wmse_audio_quality-0.1.4/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)     7472 2024-05-16 18:13:05.558074 torch_log_wmse_audio_quality-0.1.4/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     6643 2024-05-16 18:12:59.000000 torch_log_wmse_audio_quality-0.1.4/README.md
--rw-r--r--   0 chris      (501) staff       (20)      103 2024-05-15 21:20:06.000000 torch_log_wmse_audio_quality-0.1.4/pyproject.toml
--rw-r--r--   0 chris      (501) staff       (20)     1006 2024-05-16 18:13:05.558651 torch_log_wmse_audio_quality-0.1.4/setup.cfg
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 18:13:05.552656 torch_log_wmse_audio_quality-0.1.4/tests/
--rw-r--r--   0 chris      (501) staff       (20)     4159 2024-05-16 17:08:03.000000 torch_log_wmse_audio_quality-0.1.4/tests/test_metric.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 18:13:05.555618 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/
--rw-r--r--   0 chris      (501) staff       (20)       51 2024-05-15 20:27:31.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      599 2024-03-29 20:25:42.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/constants.py
--rw-r--r--   0 chris      (501) staff       (20)    32151 2024-03-28 21:53:42.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/filter_ir.pkl
--rw-r--r--   0 chris      (501) staff       (20)     5747 2024-05-16 16:39:36.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/freq_weighting_filter.py
--rw-r--r--   0 chris      (501) staff       (20)     5473 2024-05-16 17:39:28.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/metric.py
--rw-r--r--   0 chris      (501) staff       (20)      947 2024-05-15 18:39:32.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/utils.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2024-05-16 18:13:05.557460 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     7472 2024-05-16 18:13:05.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      579 2024-05-16 18:13:05.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2024-05-16 18:13:05.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)       45 2024-05-16 18:13:05.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       29 2024-05-16 18:13:05.000000 torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.149312 torch_log_wmse_audio_quality-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/tests/test_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.149312 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32151 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/filter_ir.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/freq_weighting_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-17 19:10:23.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:10:28.153313 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7572 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 19:10:28.000000 torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/top_level.txt
```

### Comparing `torch_log_wmse_audio_quality-0.1.4/LICENSE` & `torch_log_wmse_audio_quality-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.4/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.4
+Version: 0.1.5
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.8.0
 Requires-Dist: torchaudio>=1.8.0
 Requires-Dist: numpy>=1.23.5
 
-# torch-log-wmse-audio-quality
+![torch-log-wmse-audio-quality-logo](https://raw.githubusercontent.com/crlandsc/torch-log-wmse-audio-quality/main/images/logo.png)
 
 [![LICENSE](https://img.shields.io/github/license/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/blob/main/LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/stargazers) [![GitHub forks](https://img.shields.io/github/forks/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/forks)
 
 This repository contains the torch implementation of an audio quality metric, [logWMSE](https://github.com/nomonosound/log-wmse-audio-quality), originally proposed by [Iver Jordal](https://github.com/iver56) of [Nomono](https://nomono.co/). In addition to the original metric, this implementation can also be used as a loss function for training audio separation and denoising models.
 
 logWMSE is a custom metric and loss function for audio signals that calculates the logarithm (log) of a frequency-weighted (W) Mean Squared Error (MSE). It is designed to address several shortcomings of common audio metrics, most importantly the lack of support for digital silence targets.
```

### Comparing `torch_log_wmse_audio_quality-0.1.4/README.md` & `torch_log_wmse_audio_quality-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# torch-log-wmse-audio-quality
+![torch-log-wmse-audio-quality-logo](https://raw.githubusercontent.com/crlandsc/torch-log-wmse-audio-quality/main/images/logo.png)
 
 [![LICENSE](https://img.shields.io/github/license/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/blob/main/LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/stargazers) [![GitHub forks](https://img.shields.io/github/forks/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/forks)
 
 This repository contains the torch implementation of an audio quality metric, [logWMSE](https://github.com/nomonosound/log-wmse-audio-quality), originally proposed by [Iver Jordal](https://github.com/iver56) of [Nomono](https://nomono.co/). In addition to the original metric, this implementation can also be used as a loss function for training audio separation and denoising models.
 
 logWMSE is a custom metric and loss function for audio signals that calculates the logarithm (log) of a frequency-weighted (W) Mean Squared Error (MSE). It is designed to address several shortcomings of common audio metrics, most importantly the lack of support for digital silence targets.
```

### Comparing `torch_log_wmse_audio_quality-0.1.4/setup.cfg` & `torch_log_wmse_audio_quality-0.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch-log-wmse-audio-quality
-version = 0.1.4
+version = 0.1.5
 author = Christopher Landschoot
 author_email = crlandschoot@gmail.com
 license = Apache License 2.0
 description = logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/crlandsc/torch-log-wmse-audio-quality
```

### Comparing `torch_log_wmse_audio_quality-0.1.4/tests/test_metric.py` & `torch_log_wmse_audio_quality-0.1.5/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/constants.py` & `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/constants.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/filter_ir.pkl` & `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/filter_ir.pkl`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/freq_weighting_filter.py` & `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/freq_weighting_filter.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/metric.py` & `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/metric.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality/utils.py` & `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality/utils.py`

 * *Files identical despite different names*

### Comparing `torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/PKG-INFO` & `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-log-wmse-audio-quality
-Version: 0.1.4
+Version: 0.1.5
 Summary: logWMSE is an audio quality metric & loss function with support for digital silence target. Useful for training and evaluating audio source separation systems.
 Home-page: https://github.com/crlandsc/torch-log-wmse-audio-quality
 Author: Christopher Landschoot
 Author-email: crlandschoot@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/crlandsc/torch-log-wmse-audio-quality/issues
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.8.0
 Requires-Dist: torchaudio>=1.8.0
 Requires-Dist: numpy>=1.23.5
 
-# torch-log-wmse-audio-quality
+![torch-log-wmse-audio-quality-logo](https://raw.githubusercontent.com/crlandsc/torch-log-wmse-audio-quality/main/images/logo.png)
 
 [![LICENSE](https://img.shields.io/github/license/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/blob/main/LICENSE) [![GitHub Repo stars](https://img.shields.io/github/stars/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/stargazers) [![GitHub forks](https://img.shields.io/github/forks/crlandsc/torch-log-wmse-audio-quality)](https://github.com/crlandsc/torch-log-wmse-audio-quality/forks)
 
 This repository contains the torch implementation of an audio quality metric, [logWMSE](https://github.com/nomonosound/log-wmse-audio-quality), originally proposed by [Iver Jordal](https://github.com/iver56) of [Nomono](https://nomono.co/). In addition to the original metric, this implementation can also be used as a loss function for training audio separation and denoising models.
 
 logWMSE is a custom metric and loss function for audio signals that calculates the logarithm (log) of a frequency-weighted (W) Mean Squared Error (MSE). It is designed to address several shortcomings of common audio metrics, most importantly the lack of support for digital silence targets.
```

### Comparing `torch_log_wmse_audio_quality-0.1.4/torch_log_wmse_audio_quality.egg-info/SOURCES.txt` & `torch_log_wmse_audio_quality-0.1.5/torch_log_wmse_audio_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

