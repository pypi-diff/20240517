# Comparing `tmp/shadowfinder-0.1.1.tar.gz` & `tmp/shadowfinder-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowfinder-0.1.1.tar", max compression
+gzip compressed data, was "shadowfinder-0.2.0.tar", max compression
```

## Comparing `shadowfinder-0.1.1.tar` & `shadowfinder-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2024-05-13 09:45:09.967971 shadowfinder-0.1.1/LICENSE
--rw-r--r--   0        0        0      483 2024-05-13 09:45:09.967971 shadowfinder-0.1.1/README.md
--rw-r--r--   0        0        0      981 2024-05-13 09:45:09.967971 shadowfinder-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 09:45:09.967971 shadowfinder-0.1.1/shadowfinder/__init__.py
--rw-r--r--   0        0        0     1509 2024-05-13 09:45:09.967971 shadowfinder-0.1.1/shadowfinder/cli.py
--rw-r--r--   0        0        0      164 2024-05-13 09:45:09.967971 shadowfinder-0.1.1/shadowfinder/main.py
--rw-r--r--   0        0        0     2947 2024-05-13 09:45:09.967971 shadowfinder-0.1.1/shadowfinder/shadowfinder.py
--rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 shadowfinder-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/LICENSE
+-rw-r--r--   0        0        0      483 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/README.md
+-rw-r--r--   0        0        0     1051 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/__init__.py
+-rw-r--r--   0        0        0     1509 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/cli.py
+-rw-r--r--   0        0        0      164 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/main.py
+-rw-r--r--   0        0        0     6500 2024-05-17 15:55:35.988639 shadowfinder-0.2.0/shadowfinder/shadowfinder.py
+-rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 shadowfinder-0.2.0/PKG-INFO
```

### Comparing `shadowfinder-0.1.1/LICENSE` & `shadowfinder-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowfinder-0.1.1/pyproject.toml` & `shadowfinder-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ShadowFinder"
-version = "0.1.1"
+version = "0.2.0"
 description = "Find possible locations of shadows."
 authors = ["Bellingcat"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/bellingcat/ShadowFinder"
 classifiers = [
   "Intended Audience :: Developers",
@@ -24,14 +24,18 @@
 
 [tool.poetry.dependencies]
 python =  ">=3.9,<3.13"
 matplotlib = "^3.8"
 basemap = "^1.4"
 suncalc = "^0.1.3"
 fire = "^0.5"
+timezonefinder = "^6.5"
+pandas = "^2.2"
+numpy = "^1"
+pytz = "^2024.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `shadowfinder-0.1.1/shadowfinder/cli.py` & `shadowfinder-0.2.0/shadowfinder/cli.py`

 * *Files identical despite different names*

### Comparing `shadowfinder-0.1.1/PKG-INFO` & `shadowfinder-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ShadowFinder
-Version: 0.1.1
+Version: 0.2.0
 Summary: Find possible locations of shadows.
 Home-page: https://github.com/bellingcat/ShadowFinder
 License: MIT
 Keywords: shadow,finder,locator,map
 Author: Bellingcat
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 3 - Alpha
@@ -16,15 +16,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: basemap (>=1.4,<2.0)
 Requires-Dist: fire (>=0.5,<0.6)
 Requires-Dist: matplotlib (>=3.8,<4.0)
+Requires-Dist: numpy (>=1,<2)
+Requires-Dist: pandas (>=2.2,<3.0)
+Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: suncalc (>=0.1.3,<0.2.0)
+Requires-Dist: timezonefinder (>=6.5,<7.0)
 Project-URL: Bug Tracker, https://github.com/bellingcat/ShadowFinder/issues
 Project-URL: Repository, https://github.com/bellingcat/ShadowFinder
 Description-Content-Type: text/markdown
 
 # ShadowFinder
 
 A lightweight tool and Google Colab notebook for estimating the points on the Earth's surface where a shadow of a particular length could occur, for geolocation purposes.
```

