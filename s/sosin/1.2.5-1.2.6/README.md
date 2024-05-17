# Comparing `tmp/sosin-1.2.5.tar.gz` & `tmp/sosin-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.2.5.tar", last modified: Sun Apr 21 11:01:02 2024, max compression
+gzip compressed data, was "sosin-1.2.6.tar", last modified: Fri May 17 13:31:51 2024, max compression
```

## Comparing `sosin-1.2.5.tar` & `sosin-1.2.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 11:01:02.736695 sosin-1.2.5/
--rw-rw-rw-   0        0        0     1083 2024-04-21 10:50:27.000000 sosin-1.2.5/LICENSE
--rw-rw-rw-   0        0        0     1328 2024-04-21 11:01:02.736695 sosin-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      863 2024-04-21 10:50:27.000000 sosin-1.2.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-21 11:01:02.736695 sosin-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      985 2024-04-21 10:59:54.000000 sosin-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-21 11:01:02.716199 sosin-1.2.5/sosin/
--rw-rw-rw-   0        0        0      302 2024-04-21 11:00:02.000000 sosin-1.2.5/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-21 11:01:02.725845 sosin-1.2.5/sosin/databases/
--rw-rw-rw-   0        0        0    13404 2024-04-21 10:59:25.000000 sosin-1.2.5/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2024-04-21 11:01:02.726842 sosin-1.2.5/sosin/rpa/
--rw-rw-rw-   0        0        0    12041 2024-04-21 10:54:40.000000 sosin-1.2.5/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2024-04-21 11:01:02.730551 sosin-1.2.5/sosin/utils/
--rw-rw-rw-   0        0        0     1797 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      422 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/utils/secret.py
--rw-rw-rw-   0        0        0      885 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/utils/zip.py
-drwxrwxrwx   0        0        0        0 2024-04-21 11:01:02.734932 sosin-1.2.5/sosin/web/
--rw-rw-rw-   0        0        0     1055 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/web/content.py
--rw-rw-rw-   0        0        0     6086 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/web/session.py
--rw-rw-rw-   0        0        0     1051 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4580 2024-04-21 10:50:27.000000 sosin-1.2.5/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2024-04-21 11:01:02.724847 sosin-1.2.5/sosin.egg-info/
--rw-rw-rw-   0        0        0     1328 2024-04-21 11:01:02.000000 sosin-1.2.5/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2024-04-21 11:01:02.000000 sosin-1.2.5/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 11:01:02.000000 sosin-1.2.5/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-21 11:01:02.000000 sosin-1.2.5/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-21 11:01:02.000000 sosin-1.2.5/sosin.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.578196 sosin-1.2.6/
+-rw-rw-rw-   0        0        0     1083 2024-05-17 13:30:25.000000 sosin-1.2.6/LICENSE
+-rw-rw-rw-   0        0        0     1269 2024-05-17 13:31:51.577110 sosin-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2024-05-17 13:30:25.000000 sosin-1.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 13:31:51.578196 sosin-1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      985 2024-05-17 13:31:12.000000 sosin-1.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.538398 sosin-1.2.6/sosin/
+-rw-rw-rw-   0        0        0      302 2024-05-17 13:31:04.000000 sosin-1.2.6/sosin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.561913 sosin-1.2.6/sosin/databases/
+-rw-rw-rw-   0        0        0    13404 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/databases/rdb.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.564954 sosin-1.2.6/sosin/rpa/
+-rw-rw-rw-   0        0        0    12041 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/rpa/email_mgr.py
+-rw-rw-rw-   0        0        0     3698 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/rpa/sms_mgr.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.569529 sosin-1.2.6/sosin/utils/
+-rw-rw-rw-   0        0        0     1797 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/currency.py
+-rw-rw-rw-   0        0        0      304 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/log.py
+-rw-rw-rw-   0        0        0      527 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/progress.py
+-rw-rw-rw-   0        0        0      422 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/secret.py
+-rw-rw-rw-   0        0        0      885 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/utils/zip.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.572792 sosin-1.2.6/sosin/web/
+-rw-rw-rw-   0        0        0     1055 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/web/content.py
+-rw-rw-rw-   0        0        0     6138 2024-05-17 13:30:49.000000 sosin-1.2.6/sosin/web/session.py
+-rw-rw-rw-   0        0        0     1051 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/web/translate.py
+-rw-rw-rw-   0        0        0     4580 2024-05-17 13:30:25.000000 sosin-1.2.6/sosin/web/virtual.py
+drwxrwxrwx   0        0        0        0 2024-05-17 13:31:51.560408 sosin-1.2.6/sosin.egg-info/
+-rw-rw-rw-   0        0        0     1269 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-17 13:31:51.000000 sosin-1.2.6/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.2.5/LICENSE` & `sosin-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/PKG-INFO` & `sosin-1.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.2.5
+Version: 1.2.6
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: sosincomp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: requests-toolbelt
 
 # sosin: easy to use Python utils for general works
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
 [![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
```

### Comparing `sosin-1.2.5/README.md` & `sosin-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/setup.py` & `sosin-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.2.5",
+    version                             = "1.2.6",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "sosincomp@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'requests-toolbelt'],
```

### Comparing `sosin-1.2.5/sosin/databases/rdb.py` & `sosin-1.2.6/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/rpa/email_mgr.py` & `sosin-1.2.6/sosin/rpa/email_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/rpa/sms_mgr.py` & `sosin-1.2.6/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/utils/currency.py` & `sosin-1.2.6/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/utils/progress.py` & `sosin-1.2.6/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/utils/zip.py` & `sosin-1.2.6/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/web/content.py` & `sosin-1.2.6/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/web/session.py` & `sosin-1.2.6/sosin/web/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,18 @@
     def _set_cookies(self, r:requests.Response) -> None:
         self._cookies.update(dict(r.cookies))
 
     def _reset_cookies(self, keys:list=[]) -> None:
         self._cookies = {k: self._cookies[k] for k in keys}
     
     def _save_cookies(self) -> None:
-        open(self._cookie_path, 'w').write('\n'.join(['{}={}'.format(k, v) for k, v in self._cookies.items()]))
+        try:
+            open(self._cookie_path, 'w').write('\n'.join(['{}={}'.format(k, v) for k, v in self._cookies.items()]))
+        except:
+            ...
         
     def _load_cookies(self) -> dict:
         for l in open(self._cookie_path, 'r').readlines():
             _idx = l.index('=')
             self._cookies.update({l[:_idx]: l[_idx+1:].rstrip()})
 
     # ------------------------------------------------------------------------
```

### Comparing `sosin-1.2.5/sosin/web/translate.py` & `sosin-1.2.6/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin/web/virtual.py` & `sosin-1.2.6/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.2.5/sosin.egg-info/PKG-INFO` & `sosin-1.2.6/sosin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: sosin
-Version: 1.2.5
+Version: 1.2.6
 Summary: Python utils for general works
 Home-page: https://github.com/devsosin/sosin
 Author: Jason Choi
 Author-email: sosincomp@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: requests-toolbelt
 
 # sosin: easy to use Python utils for general works
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
 [![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
```

