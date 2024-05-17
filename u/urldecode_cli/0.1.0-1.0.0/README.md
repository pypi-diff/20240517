# Comparing `tmp/urldecode_cli-0.1.0.tar.gz` & `tmp/urldecode_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urldecode_cli-0.1.0.tar", max compression
+gzip compressed data, was "urldecode_cli-1.0.0.tar", max compression
```

## Comparing `urldecode_cli-0.1.0.tar` & `urldecode_cli-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       60 2024-05-14 16:41:40.760167 urldecode_cli-0.1.0/README.md
--rw-r--r--   0        0        0      493 2024-05-14 16:58:48.842546 urldecode_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      203 2024-05-14 17:29:45.306035 urldecode_cli-0.1.0/urldecode_cli/__init__.py
--rw-r--r--   0        0        0       95 2024-05-14 17:29:47.873947 urldecode_cli-0.1.0/urldecode_cli/__main__.py
--rw-r--r--   0        0        0      201 2024-05-14 17:29:50.467055 urldecode_cli-0.1.0/urldecode_cli/cli.py
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 urldecode_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       60 2024-05-14 16:41:40.760167 urldecode_cli-1.0.0/README.md
+-rw-r--r--   0        0        0      493 2024-05-17 17:54:44.089134 urldecode_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      203 2024-05-14 17:29:45.306035 urldecode_cli-1.0.0/urldecode_cli/__init__.py
+-rw-r--r--   0        0        0       95 2024-05-14 17:29:47.873947 urldecode_cli-1.0.0/urldecode_cli/__main__.py
+-rw-r--r--   0        0        0      201 2024-05-14 17:29:50.467055 urldecode_cli-1.0.0/urldecode_cli/cli.py
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 urldecode_cli-1.0.0/PKG-INFO
```

### Comparing `urldecode_cli-0.1.0/PKG-INFO` & `urldecode_cli-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: urldecode_cli
-Version: 0.1.0
+Version: 1.0.0
 Summary: CLI tool to quickly decode URL encoded strings
 Home-page: https://github.com/annie444/urldecode
 License: GPL-3.0-or-later
 Author: Annie Ehler
 Author-email: annie.ehler.4@gmail.com
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Project-URL: Repository, https://github.com/annie444/urldecode
 Description-Content-Type: text/markdown
 
 # urldecode
```

