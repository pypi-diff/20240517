# Comparing `tmp/Flask-Static-Digest-0.4.0.tar.gz` & `tmp/flask_static_digest-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Static-Digest-0.4.0.tar", last modified: Sun May 14 23:30:16 2023, max compression
+gzip compressed data, was "flask_static_digest-0.4.1.tar", last modified: Fri May 17 16:03:46 2024, max compression
```

## Comparing `Flask-Static-Digest-0.4.0.tar` & `flask_static_digest-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)      871 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)      434 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       58 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-05-14 23:30:09.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/not-zip-safe
--rw-r--r--   0 nick      (1000) nick      (1000)       35 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/requires.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       20 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/top_level.txt
--rw-r--r--   0 nick      (1000) nick      (1000)     1115 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/LICENSE
--rw-r--r--   0 nick      (1000) nick      (1000)      871 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    24264 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/README.md
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/flask_static_digest/
--rw-r--r--   0 nick      (1000) nick      (1000)     3024 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/flask_static_digest/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     2132 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/flask_static_digest/cli.py
--rw-r--r--   0 nick      (1000) nick      (1000)     5650 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/flask_static_digest/digester.py
--rw-r--r--   0 nick      (1000) nick      (1000)      104 2023-03-17 01:03:17.000000 Flask-Static-Digest-0.4.0/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)       38 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/setup.cfg
--rw-r--r--   0 nick      (1000) nick      (1000)     1197 2023-05-14 23:25:07.000000 Flask-Static-Digest-0.4.0/setup.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-17 16:03:46.693506 flask_static_digest-0.4.1/
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-17 16:03:46.693506 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)      935 2024-05-17 16:03:46.000000 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)      434 2024-05-17 16:03:46.000000 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/SOURCES.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2024-05-17 16:03:46.000000 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/dependency_links.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)       57 2024-05-17 16:03:46.000000 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/entry_points.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2024-05-17 16:01:58.000000 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/not-zip-safe
+-rw-r--r--   0 nick      (1000) nick      (1000)       35 2024-05-17 16:03:46.000000 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/requires.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)       20 2024-05-17 16:03:46.000000 flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/top_level.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)     1115 2023-05-14 23:23:06.000000 flask_static_digest-0.4.1/LICENSE
+-rw-r--r--   0 nick      (1000) nick      (1000)      935 2024-05-17 16:03:46.693506 flask_static_digest-0.4.1/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    24264 2023-05-14 23:23:06.000000 flask_static_digest-0.4.1/README.md
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-17 16:03:46.693506 flask_static_digest-0.4.1/flask_static_digest/
+-rw-r--r--   0 nick      (1000) nick      (1000)     3199 2024-05-17 15:53:10.000000 flask_static_digest-0.4.1/flask_static_digest/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2132 2023-05-14 23:23:06.000000 flask_static_digest-0.4.1/flask_static_digest/cli.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5650 2023-05-14 23:23:06.000000 flask_static_digest-0.4.1/flask_static_digest/digester.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      104 2023-03-17 01:03:17.000000 flask_static_digest-0.4.1/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)       38 2024-05-17 16:03:46.693506 flask_static_digest-0.4.1/setup.cfg
+-rw-r--r--   0 nick      (1000) nick      (1000)     1224 2024-05-17 15:59:31.000000 flask_static_digest-0.4.1/setup.py
```

### Comparing `Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/PKG-INFO` & `flask_static_digest-0.4.1/Flask_Static_Digest.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Static-Digest
-Version: 0.4.0
+Version: 0.4.1
 Summary: Flask extension for md5 tagging and compressing (gzip / brotli) static files.
 Home-page: https://github.com/nickjj/flask-static-digest
 Author: Nick Janetakis
 Author-email: nick.janetakis@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -14,12 +14,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Compression
 Requires-Python: >=3.6
-Provides-Extra: brotli
 License-File: LICENSE
-
-UNKNOWN
-
+Requires-Dist: Flask>=1.0
+Provides-Extra: brotli
+Requires-Dist: Brotli>=1.0.9; extra == "brotli"
```

### Comparing `Flask-Static-Digest-0.4.0/LICENSE` & `flask_static_digest-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Static-Digest-0.4.0/PKG-INFO` & `flask_static_digest-0.4.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Static-Digest
-Version: 0.4.0
+Version: 0.4.1
 Summary: Flask extension for md5 tagging and compressing (gzip / brotli) static files.
 Home-page: https://github.com/nickjj/flask-static-digest
 Author: Nick Janetakis
 Author-email: nick.janetakis@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
@@ -14,12 +14,11 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Compression
 Requires-Python: >=3.6
-Provides-Extra: brotli
 License-File: LICENSE
-
-UNKNOWN
-
+Requires-Dist: Flask>=1.0
+Provides-Extra: brotli
+Requires-Dist: Brotli>=1.0.9; extra == "brotli"
```

### Comparing `Flask-Static-Digest-0.4.0/README.md` & `flask_static_digest-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `Flask-Static-Digest-0.4.0/flask_static_digest/__init__.py` & `flask_static_digest-0.4.1/flask_static_digest/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import logging
 import os
-from urllib.parse import urljoin
 
 from flask import request
 from flask import url_for as flask_url_for
 
 
 class FlaskStaticDigest(object):
     def __init__(self, app=None):
@@ -51,18 +50,25 @@
         except json.JSONDecodeError:
             logging.warning(f"Couldn't decode file: {manifest_path}")
         except PermissionError:
             logging.warning(f"Couldn't access file: {manifest_path}")
         except (FileNotFoundError, Exception):
             pass
 
-    def _prepend_host_url(self, host, filename):
-        return urljoin(
-            self.host_url, "/".join([self.static_url_path, filename])
-        )
+    def _custom_url_join(self, url_path):
+        """
+        Join the host URL with another URL path.
+        :param url_path: The URL returned by url_for
+        :type url_path: str
+        :return: Joined URL
+        """
+        if self.host_url is None:
+            return url_path
+
+        return "/".join([self.host_url.rstrip("/"), url_path.lstrip("/")])
 
     def static_url_for(self, endpoint, **values):
         """
         This function uses Flask's url_for under the hood and accepts the
         same arguments. The only differences are it will prefix a host URL if
         one exists and if a manifest is available it will look up the filename
         from the manifest.
@@ -79,8 +85,8 @@
                 else:
                     endpoint = endpoint[1:]
 
         manifest = self.manifests.get(endpoint, {})
         filename = values.get("filename", None)
         values["filename"] = manifest.get(filename, filename)
 
-        return urljoin(self.host_url, flask_url_for(endpoint, **values))
+        return self._custom_url_join(flask_url_for(endpoint, **values))
```

### Comparing `Flask-Static-Digest-0.4.0/flask_static_digest/cli.py` & `flask_static_digest-0.4.1/flask_static_digest/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-Static-Digest-0.4.0/flask_static_digest/digester.py` & `flask_static_digest-0.4.1/flask_static_digest/digester.py`

 * *Files identical despite different names*

### Comparing `Flask-Static-Digest-0.4.0/setup.py` & `flask_static_digest-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup
 
 
 setup(
     name="Flask-Static-Digest",
-    version="0.4.0",
+    version="0.4.1",
     author="Nick Janetakis",
     author_email="nick.janetakis@gmail.com",
     url="https://github.com/nickjj/flask-static-digest",
-    description="Flask extension for md5 tagging and compressing (gzip / brotli) static files.",
+    description=(
+        "Flask extension for md5 tagging and compressing "
+        "(gzip / brotli) static files."
+    ),
     license="MIT",
     package_data={"Flask-Static-Digest": ["VERSION"]},
     packages=["flask_static_digest"],
     platforms="any",
     python_requires=">=3.6",
     zip_safe=False,
     install_requires=["Flask>=1.0"],
```

