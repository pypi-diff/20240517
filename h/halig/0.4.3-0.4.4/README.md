# Comparing `tmp/halig-0.4.3.tar.gz` & `tmp/halig-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halig-0.4.3.tar", last modified: Wed Nov 29 17:42:53 2023, max compression
+gzip compressed data, was "halig-0.4.4.tar", last modified: Sun Dec 10 10:22:47 2023, max compression
```

## Comparing `halig-0.4.3.tar` & `halig-0.4.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    34670 2023-06-19 16:50:30.000000 halig-0.4.3/LICENSE
--rw-r--r--   0        0        0     1635 2023-06-19 16:50:30.000000 halig-0.4.3/README.md
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.3/halig/__init__.py
--rw-r--r--   0        0        0       22 2023-11-29 17:41:47.891774 halig-0.4.3/halig/__version__.py
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.3/halig/commands/__init__.py
--rw-r--r--   0        0        0      385 2023-07-24 17:42:38.529912 halig-0.4.3/halig/commands/base.py
--rw-r--r--   0        0        0     2781 2023-06-19 16:50:47.000000 halig-0.4.3/halig/commands/edit.py
--rw-r--r--   0        0        0     1397 2023-06-19 16:50:47.000000 halig-0.4.3/halig/commands/import_unencrypted.py
--rw-r--r--   0        0        0     1128 2023-07-22 12:38:35.359342 halig-0.4.3/halig/commands/notebooks.py
--rw-r--r--   0        0        0      958 2023-11-29 17:05:03.788220 halig-0.4.3/halig/commands/reencrypt.py
--rw-r--r--   0        0        0     3780 2023-11-29 17:05:03.789219 halig-0.4.3/halig/commands/search.py
--rw-r--r--   0        0        0     1368 2023-11-29 17:05:03.789219 halig-0.4.3/halig/commands/show.py
--rw-r--r--   0        0        0     1468 2023-07-24 17:49:45.965214 halig-0.4.3/halig/encryption.py
--rw-r--r--   0        0        0     2262 2023-11-29 17:05:03.789219 halig-0.4.3/halig/literals.py
--rw-r--r--   0        0        0     4411 2023-11-29 17:05:03.789219 halig-0.4.3/halig/main.py
--rw-r--r--   0        0        0     4341 2023-11-29 17:14:56.563242 halig-0.4.3/halig/settings.py
--rw-r--r--   0        0        0      733 2023-06-19 16:50:47.000000 halig-0.4.3/halig/utils.py
--rw-r--r--   0        0        0     2780 2023-11-29 17:42:53.174176 halig-0.4.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.3/tests/commands/__init__.py
--rw-r--r--   0        0        0     2262 2023-11-29 17:05:03.791219 halig-0.4.3/tests/commands/conftest.py
--rw-r--r--   0        0        0     1177 2023-11-29 17:11:21.843414 halig-0.4.3/tests/commands/test_edit.py
--rw-r--r--   0        0        0     1476 2023-11-29 17:11:21.834415 halig-0.4.3/tests/commands/test_import.py
--rw-r--r--   0        0        0     1563 2023-06-19 16:50:47.000000 halig-0.4.3/tests/commands/test_notebooks.py
--rw-r--r--   0        0        0      426 2023-11-29 17:05:03.792219 halig-0.4.3/tests/commands/test_reencrypt.py
--rw-r--r--   0        0        0     1150 2023-11-29 17:11:21.845414 halig-0.4.3/tests/commands/test_show.py
--rw-r--r--   0        0        0     3527 2023-11-29 17:33:35.644381 halig-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0     2318 2023-11-29 17:32:13.310156 halig-0.4.3/tests/test_encryption.py
--rw-r--r--   0        0        0     1121 2023-11-29 17:33:54.514204 halig-0.4.3/tests/test_settings.py
--rw-r--r--   0        0        0     1516 2023-11-29 17:05:03.792219 halig-0.4.3/tests/test_utils.py
--rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 halig-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    34670 2023-06-19 16:50:30.000000 halig-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1635 2023-06-19 16:50:30.000000 halig-0.4.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/halig/__init__.py
+-rw-r--r--   0        0        0       22 2023-12-10 10:22:26.033716 halig-0.4.4/halig/__version__.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/halig/commands/__init__.py
+-rw-r--r--   0        0        0      385 2023-07-24 17:42:38.529912 halig-0.4.4/halig/commands/base.py
+-rw-r--r--   0        0        0     2781 2023-06-19 16:50:47.000000 halig-0.4.4/halig/commands/edit.py
+-rw-r--r--   0        0        0     1397 2023-06-19 16:50:47.000000 halig-0.4.4/halig/commands/import_unencrypted.py
+-rw-r--r--   0        0        0     1128 2023-07-22 12:38:35.359342 halig-0.4.4/halig/commands/notebooks.py
+-rw-r--r--   0        0        0      958 2023-11-29 17:05:03.788220 halig-0.4.4/halig/commands/reencrypt.py
+-rw-r--r--   0        0        0     3780 2023-11-29 17:05:03.789219 halig-0.4.4/halig/commands/search.py
+-rw-r--r--   0        0        0     1368 2023-11-29 17:05:03.789219 halig-0.4.4/halig/commands/show.py
+-rw-r--r--   0        0        0     1468 2023-07-24 17:49:45.965214 halig-0.4.4/halig/encryption.py
+-rw-r--r--   0        0        0     2262 2023-11-29 17:05:03.789219 halig-0.4.4/halig/literals.py
+-rw-r--r--   0        0        0     4411 2023-11-29 17:05:03.789219 halig-0.4.4/halig/main.py
+-rw-r--r--   0        0        0     4341 2023-11-29 17:14:56.563242 halig-0.4.4/halig/settings.py
+-rw-r--r--   0        0        0      733 2023-06-19 16:50:47.000000 halig-0.4.4/halig/utils.py
+-rw-r--r--   0        0        0     2780 2023-12-10 10:22:47.720482 halig-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-19 16:50:47.000000 halig-0.4.4/tests/commands/__init__.py
+-rw-r--r--   0        0        0     2262 2023-11-29 17:05:03.791219 halig-0.4.4/tests/commands/conftest.py
+-rw-r--r--   0        0        0     1177 2023-11-29 17:11:21.843414 halig-0.4.4/tests/commands/test_edit.py
+-rw-r--r--   0        0        0     1476 2023-11-29 17:11:21.834415 halig-0.4.4/tests/commands/test_import.py
+-rw-r--r--   0        0        0     1563 2023-06-19 16:50:47.000000 halig-0.4.4/tests/commands/test_notebooks.py
+-rw-r--r--   0        0        0      426 2023-11-29 17:05:03.792219 halig-0.4.4/tests/commands/test_reencrypt.py
+-rw-r--r--   0        0        0     1150 2023-11-29 17:11:21.845414 halig-0.4.4/tests/commands/test_show.py
+-rw-r--r--   0        0        0     3527 2023-11-29 17:33:35.644381 halig-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     2318 2023-11-29 17:32:13.310156 halig-0.4.4/tests/test_encryption.py
+-rw-r--r--   0        0        0     1121 2023-11-29 17:33:54.514204 halig-0.4.4/tests/test_settings.py
+-rw-r--r--   0        0        0     1516 2023-11-29 17:05:03.792219 halig-0.4.4/tests/test_utils.py
+-rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 halig-0.4.4/PKG-INFO
```

### Comparing `halig-0.4.3/LICENSE` & `halig-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/README.md` & `halig-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/commands/edit.py` & `halig-0.4.4/halig/commands/edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/commands/import_unencrypted.py` & `halig-0.4.4/halig/commands/import_unencrypted.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/commands/notebooks.py` & `halig-0.4.4/halig/commands/notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/commands/reencrypt.py` & `halig-0.4.4/halig/commands/reencrypt.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/commands/search.py` & `halig-0.4.4/halig/commands/search.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/commands/show.py` & `halig-0.4.4/halig/commands/show.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/encryption.py` & `halig-0.4.4/halig/encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/literals.py` & `halig-0.4.4/halig/literals.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/main.py` & `halig-0.4.4/halig/main.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/settings.py` & `halig-0.4.4/halig/settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/halig/utils.py` & `halig-0.4.4/halig/utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/pyproject.toml` & `halig-0.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Terminals",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
-version = "0.4.3"
+version = "0.4.4"
 
 [project.license]
 text = "GPL-3.0-or-later"
 
 [project.urls]
 Homepage = "https://git.roboces.dev/catalin/halig"
 Repository = "https://git.roboces.dev/catalin/halig"
```

### Comparing `halig-0.4.3/tests/commands/conftest.py` & `halig-0.4.4/tests/commands/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/commands/test_edit.py` & `halig-0.4.4/tests/commands/test_edit.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/commands/test_import.py` & `halig-0.4.4/tests/commands/test_import.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/commands/test_notebooks.py` & `halig-0.4.4/tests/commands/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/commands/test_show.py` & `halig-0.4.4/tests/commands/test_show.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/conftest.py` & `halig-0.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/test_encryption.py` & `halig-0.4.4/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/test_settings.py` & `halig-0.4.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/tests/test_utils.py` & `halig-0.4.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `halig-0.4.3/PKG-INFO` & `halig-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halig
-Version: 0.4.3
+Version: 0.4.4
 Summary: age-encrypted, file-based, note-taking CLI app
 Keywords: cli notes age rage encryption notebook
 Author-Email: cătălin <185504a9@duck.com>
 License: GPL-3.0-or-later
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

