# Comparing `tmp/django_includes-0.3.0.tar.gz` & `tmp/django_includes-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django_includes-0.3.0.tar", last modified: Thu Jan  2 08:05:28 2020, max compression
+gzip compressed data, was "dist/django_includes-0.3.1.tar", last modified: Thu Jan  2 08:06:57 2020, max compression
```

## Comparing `django_includes-0.3.0.tar` & `django_includes-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rd         (501) staff       (20)        0 2020-01-02 08:05:28.000000 django_includes-0.3.0/
--rw-r--r--   0 rd         (501) staff       (20)       14 2020-01-02 08:02:02.000000 django_includes-0.3.0/MANIFEST.in
--rw-r--r--   0 rd         (501) staff       (20)     2427 2020-01-02 08:05:28.000000 django_includes-0.3.0/PKG-INFO
--rw-r--r--   0 rd         (501) staff       (20)     1525 2020-01-02 08:02:02.000000 django_includes-0.3.0/README.rst
--rw-r--r--   0 rd         (501) staff       (20)        0 2020-01-02 08:02:02.000000 django_includes-0.3.0/classifiers.txt
-drwxr-xr-x   0 rd         (501) staff       (20)        0 2020-01-02 08:05:28.000000 django_includes-0.3.0/django_includes/
--rw-r--r--   0 rd         (501) staff       (20)       76 2020-01-02 08:02:02.000000 django_includes-0.3.0/django_includes/__init__.py
--rw-r--r--   0 rd         (501) staff       (20)       22 2020-01-02 08:02:02.000000 django_includes-0.3.0/django_includes/_version.py
--rw-r--r--   0 rd         (501) staff       (20)     3156 2020-01-02 08:02:02.000000 django_includes-0.3.0/django_includes/jinja2.py
--rw-r--r--   0 rd         (501) staff       (20)     1306 2020-01-02 08:02:02.000000 django_includes-0.3.0/django_includes/middleware.py
--rw-r--r--   0 rd         (501) staff       (20)       23 2020-01-02 08:02:02.000000 django_includes-0.3.0/django_includes/settings.py
--rw-r--r--   0 rd         (501) staff       (20)      358 2020-01-02 08:02:02.000000 django_includes-0.3.0/django_includes/utils.py
--rw-r--r--   0 rd         (501) staff       (20)     2899 2020-01-02 08:02:02.000000 django_includes-0.3.0/django_includes/views.py
-drwxr-xr-x   0 rd         (501) staff       (20)        0 2020-01-02 08:05:28.000000 django_includes-0.3.0/django_includes.egg-info/
--rw-r--r--   0 rd         (501) staff       (20)     2427 2020-01-02 08:05:28.000000 django_includes-0.3.0/django_includes.egg-info/PKG-INFO
--rw-r--r--   0 rd         (501) staff       (20)      491 2020-01-02 08:05:28.000000 django_includes-0.3.0/django_includes.egg-info/SOURCES.txt
--rw-r--r--   0 rd         (501) staff       (20)        1 2020-01-02 08:05:28.000000 django_includes-0.3.0/django_includes.egg-info/dependency_links.txt
--rw-r--r--   0 rd         (501) staff       (20)      130 2020-01-02 08:05:28.000000 django_includes-0.3.0/django_includes.egg-info/requires.txt
--rw-r--r--   0 rd         (501) staff       (20)       16 2020-01-02 08:05:28.000000 django_includes-0.3.0/django_includes.egg-info/top_level.txt
--rw-r--r--   0 rd         (501) staff       (20)      233 2020-01-02 08:02:02.000000 django_includes-0.3.0/requirements-dev.txt
--rw-r--r--   0 rd         (501) staff       (20)      223 2020-01-02 08:02:02.000000 django_includes-0.3.0/requirements.txt
--rw-r--r--   0 rd         (501) staff       (20)      107 2020-01-02 08:05:28.000000 django_includes-0.3.0/setup.cfg
--rw-r--r--   0 rd         (501) staff       (20)     2125 2020-01-02 08:02:02.000000 django_includes-0.3.0/setup.py
--rw-r--r--   0 rd         (501) staff       (20)        6 2020-01-02 08:02:02.000000 django_includes-0.3.0/version.txt
+drwxr-xr-x   0 rd         (501) staff       (20)        0 2020-01-02 08:06:57.425597 django_includes-0.3.1/
+-rw-r--r--   0 rd         (501) staff       (20)       14 2020-01-02 08:06:44.000000 django_includes-0.3.1/MANIFEST.in
+-rw-r--r--   0 rd         (501) staff       (20)     2427 2020-01-02 08:06:57.425780 django_includes-0.3.1/PKG-INFO
+-rw-r--r--   0 rd         (501) staff       (20)     1525 2020-01-02 08:06:44.000000 django_includes-0.3.1/README.rst
+-rw-r--r--   0 rd         (501) staff       (20)        0 2020-01-02 08:06:44.000000 django_includes-0.3.1/classifiers.txt
+drwxr-xr-x   0 rd         (501) staff       (20)        0 2020-01-02 08:06:57.423597 django_includes-0.3.1/django_includes/
+-rw-r--r--   0 rd         (501) staff       (20)       76 2020-01-02 08:06:44.000000 django_includes-0.3.1/django_includes/__init__.py
+-rw-r--r--   0 rd         (501) staff       (20)       22 2020-01-02 08:06:44.000000 django_includes-0.3.1/django_includes/_version.py
+-rw-r--r--   0 rd         (501) staff       (20)     3156 2020-01-02 08:06:44.000000 django_includes-0.3.1/django_includes/jinja2.py
+-rw-r--r--   0 rd         (501) staff       (20)     1306 2020-01-02 08:06:44.000000 django_includes-0.3.1/django_includes/middleware.py
+-rw-r--r--   0 rd         (501) staff       (20)       23 2020-01-02 08:06:44.000000 django_includes-0.3.1/django_includes/settings.py
+-rw-r--r--   0 rd         (501) staff       (20)      358 2020-01-02 08:06:44.000000 django_includes-0.3.1/django_includes/utils.py
+-rw-r--r--   0 rd         (501) staff       (20)     2899 2020-01-02 08:06:44.000000 django_includes-0.3.1/django_includes/views.py
+drwxr-xr-x   0 rd         (501) staff       (20)        0 2020-01-02 08:06:57.425264 django_includes-0.3.1/django_includes.egg-info/
+-rw-r--r--   0 rd         (501) staff       (20)     2427 2020-01-02 08:06:57.000000 django_includes-0.3.1/django_includes.egg-info/PKG-INFO
+-rw-r--r--   0 rd         (501) staff       (20)      491 2020-01-02 08:06:57.000000 django_includes-0.3.1/django_includes.egg-info/SOURCES.txt
+-rw-r--r--   0 rd         (501) staff       (20)        1 2020-01-02 08:06:57.000000 django_includes-0.3.1/django_includes.egg-info/dependency_links.txt
+-rw-r--r--   0 rd         (501) staff       (20)      130 2020-01-02 08:06:57.000000 django_includes-0.3.1/django_includes.egg-info/requires.txt
+-rw-r--r--   0 rd         (501) staff       (20)       16 2020-01-02 08:06:57.000000 django_includes-0.3.1/django_includes.egg-info/top_level.txt
+-rw-r--r--   0 rd         (501) staff       (20)      233 2020-01-02 08:06:44.000000 django_includes-0.3.1/requirements-dev.txt
+-rw-r--r--   0 rd         (501) staff       (20)      223 2020-01-02 08:06:44.000000 django_includes-0.3.1/requirements.txt
+-rw-r--r--   0 rd         (501) staff       (20)      107 2020-01-02 08:06:57.426349 django_includes-0.3.1/setup.cfg
+-rw-r--r--   0 rd         (501) staff       (20)     2125 2020-01-02 08:06:44.000000 django_includes-0.3.1/setup.py
+-rw-r--r--   0 rd         (501) staff       (20)        6 2020-01-02 08:06:44.000000 django_includes-0.3.1/version.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django_includes-0.3.0/PKG-INFO` & `django_includes-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django_includes
-Version: 0.3.0
+Version: 0.3.1
 Summary: Include django views as a subparts of other django views, using either HTTP (with esi or hinclude) or direct render.
 Home-page: https://github.com/hartym/django-includes
 Author: Romain Dorgueil
 Author-email: romain@dorgueil.net
 License: Apache License, Version 2.0
-Download-URL: https://github.com/hartym/django-includes/archive/0.3.0.tar.gz
+Download-URL: https://github.com/hartym/django-includes/archive/0.3.1.tar.gz
 Description: django-includes
         ===============
         
         Experimental software. There is no tests, no documentation, use it are your own risks (or don't).
         
         Currently testing that with django 2 and python 3.5+ only, which will be the only supported target.
```

### Comparing `django_includes-0.3.0/README.rst` & `django_includes-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `django_includes-0.3.0/django_includes/jinja2.py` & `django_includes-0.3.1/django_includes/jinja2.py`

 * *Files identical despite different names*

### Comparing `django_includes-0.3.0/django_includes/middleware.py` & `django_includes-0.3.1/django_includes/middleware.py`

 * *Files identical despite different names*

### Comparing `django_includes-0.3.0/django_includes/views.py` & `django_includes-0.3.1/django_includes/views.py`

 * *Files identical despite different names*

### Comparing `django_includes-0.3.0/django_includes.egg-info/PKG-INFO` & `django_includes-0.3.1/django_includes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: django-includes
-Version: 0.3.0
+Version: 0.3.1
 Summary: Include django views as a subparts of other django views, using either HTTP (with esi or hinclude) or direct render.
 Home-page: https://github.com/hartym/django-includes
 Author: Romain Dorgueil
 Author-email: romain@dorgueil.net
 License: Apache License, Version 2.0
-Download-URL: https://github.com/hartym/django-includes/archive/0.3.0.tar.gz
+Download-URL: https://github.com/hartym/django-includes/archive/0.3.1.tar.gz
 Description: django-includes
         ===============
         
         Experimental software. There is no tests, no documentation, use it are your own risks (or don't).
         
         Currently testing that with django 2 and python 3.5+ only, which will be the only supported target.
```

### Comparing `django_includes-0.3.0/setup.py` & `django_includes-0.3.1/setup.py`

 * *Files identical despite different names*

