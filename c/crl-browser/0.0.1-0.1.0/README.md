# Comparing `tmp/crl_browser-0.0.1.tar.gz` & `tmp/crl_browser-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crl_browser-0.0.1.tar", last modified: Fri May 17 18:29:25 2024, max compression
+gzip compressed data, was "crl_browser-0.1.0.tar", last modified: Fri May 17 18:19:17 2024, max compression
```

## Comparing `crl_browser-0.0.1.tar` & `crl_browser-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 goychay23  (1000) goychay23  (1000)        0 2024-05-17 18:29:25.875691 crl_browser-0.0.1/
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)     1448 2024-05-17 18:29:25.875691 crl_browser-0.0.1/PKG-INFO
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)      913 2024-05-17 18:12:55.000000 crl_browser-0.0.1/README.md
-drwxr-xr-x   0 goychay23  (1000) goychay23  (1000)        0 2024-05-17 18:29:25.875691 crl_browser-0.0.1/crl_browser.egg-info/
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)     1448 2024-05-17 18:29:25.000000 crl_browser-0.0.1/crl_browser.egg-info/PKG-INFO
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)      192 2024-05-17 18:29:25.000000 crl_browser-0.0.1/crl_browser.egg-info/SOURCES.txt
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)        1 2024-05-17 18:29:25.000000 crl_browser-0.0.1/crl_browser.egg-info/dependency_links.txt
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)       24 2024-05-17 18:29:25.000000 crl_browser-0.0.1/crl_browser.egg-info/requires.txt
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)        1 2024-05-17 18:29:25.000000 crl_browser-0.0.1/crl_browser.egg-info/top_level.txt
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)       38 2024-05-17 18:29:25.879025 crl_browser-0.0.1/setup.cfg
--rw-r--r--   0 goychay23  (1000) goychay23  (1000)      753 2024-05-17 18:29:21.000000 crl_browser-0.0.1/setup.py
+drwxr-xr-x   0 goychay23  (1000) goychay23  (1000)        0 2024-05-17 18:19:17.298047 crl_browser-0.1.0/
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)     1448 2024-05-17 18:19:17.298047 crl_browser-0.1.0/PKG-INFO
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)      913 2024-05-17 18:12:55.000000 crl_browser-0.1.0/README.md
+drwxr-xr-x   0 goychay23  (1000) goychay23  (1000)        0 2024-05-17 18:19:17.294713 crl_browser-0.1.0/crl_browser.egg-info/
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)     1448 2024-05-17 18:19:17.000000 crl_browser-0.1.0/crl_browser.egg-info/PKG-INFO
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)      192 2024-05-17 18:19:17.000000 crl_browser-0.1.0/crl_browser.egg-info/SOURCES.txt
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)        1 2024-05-17 18:19:17.000000 crl_browser-0.1.0/crl_browser.egg-info/dependency_links.txt
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)       24 2024-05-17 18:19:17.000000 crl_browser-0.1.0/crl_browser.egg-info/requires.txt
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)        1 2024-05-17 18:19:17.000000 crl_browser-0.1.0/crl_browser.egg-info/top_level.txt
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)       38 2024-05-17 18:19:17.298047 crl_browser-0.1.0/setup.cfg
+-rw-r--r--   0 goychay23  (1000) goychay23  (1000)      756 2024-05-17 18:19:14.000000 crl_browser-0.1.0/setup.py
```

### Comparing `crl_browser-0.0.1/PKG-INFO` & `crl_browser-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crl-browser
-Version: 0.0.1
+Version: 0.1.0
 Summary: crl net browsering
 Home-page: https://github.com/Goychay23/crlbrowsering
 Author: Goychay__23
 Author-email: goychaylii23@gmail.com
 License: LGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `crl_browser-0.0.1/README.md` & `crl_browser-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crl_browser-0.0.1/crl_browser.egg-info/PKG-INFO` & `crl_browser-0.1.0/crl_browser.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crl-browser
-Version: 0.0.1
+Version: 0.1.0
 Summary: crl net browsering
 Home-page: https://github.com/Goychay23/crlbrowsering
 Author: Goychay__23
 Author-email: goychaylii23@gmail.com
 License: LGPL-3.0-or-later
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `crl_browser-0.0.1/setup.py` & `crl_browser-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='crl-browser',
-    version='0.0.1',
+    version='0.1.0',
     author='Goychay__23',
     author_email='goychaylii23@gmail.com',
     description='crl net browsering',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Goychay23/crlbrowsering',
-    packages=find_packages('crl-browser'),
+    packages=find_packages('crl-browser.py'),
     license='LGPL-3.0-or-later',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.12',
```

