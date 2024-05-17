# Comparing `tmp/django-exception-logger-0.1.tar.gz` & `tmp/django-exception-logger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-exception-logger-0.1.tar", last modified: Fri May 17 14:29:49 2024, max compression
+gzip compressed data, was "django-exception-logger-0.1.3.tar", last modified: Fri May 17 14:46:57 2024, max compression
```

## Comparing `django-exception-logger-0.1.tar` & `django-exception-logger-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:29:49.090254 django-exception-logger-0.1/
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1065 2024-05-17 09:26:59.000000 django-exception-logger-0.1/LICENSE
--rwxrwxrwx   0 titov     (1000) titov     (1000)      341 2024-05-17 14:18:21.000000 django-exception-logger-0.1/MANIFEST.in
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1677 2024-05-17 14:29:49.089258 django-exception-logger-0.1/PKG-INFO
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1351 2024-05-17 12:38:32.000000 django-exception-logger-0.1/README.md
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:29:48.815340 django-exception-logger-0.1/django_exception_logger.egg-info/
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1677 2024-05-17 14:29:48.000000 django-exception-logger-0.1/django_exception_logger.egg-info/PKG-INFO
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1035 2024-05-17 14:29:48.000000 django-exception-logger-0.1/django_exception_logger.egg-info/SOURCES.txt
--rwxrwxrwx   0 titov     (1000) titov     (1000)        1 2024-05-17 14:29:48.000000 django-exception-logger-0.1/django_exception_logger.egg-info/dependency_links.txt
--rwxrwxrwx   0 titov     (1000) titov     (1000)       12 2024-05-17 14:29:48.000000 django-exception-logger-0.1/django_exception_logger.egg-info/requires.txt
--rwxrwxrwx   0 titov     (1000) titov     (1000)       17 2024-05-17 14:29:48.000000 django-exception-logger-0.1/django_exception_logger.egg-info/top_level.txt
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:29:48.867512 django-exception-logger-0.1/exception_logger/
--rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/__init__.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:29:48.929612 django-exception-logger-0.1/exception_logger/admin/
--rwxrwxrwx   0 titov     (1000) titov     (1000)      193 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/admin/__init__.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1764 2024-05-17 09:33:45.000000 django-exception-logger-0.1/exception_logger/admin/celery_exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     2028 2024-05-17 12:38:32.000000 django-exception-logger-0.1/exception_logger/admin/exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      741 2024-05-17 12:38:32.000000 django-exception-logger-0.1/exception_logger/admin/request_time.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      253 2024-05-17 09:33:45.000000 django-exception-logger-0.1/exception_logger/apps.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      391 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/forms.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:29:48.976414 django-exception-logger-0.1/exception_logger/middlewares/
--rwxrwxrwx   0 titov     (1000) titov     (1000)      106 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/middlewares/__init__.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1235 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/middlewares/exception_logger.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      620 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/middlewares/request_time.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:29:49.010144 django-exception-logger-0.1/exception_logger/migrations/
--rwxrwxrwx   0 titov     (1000) titov     (1000)     6640 2024-05-17 09:46:17.000000 django-exception-logger-0.1/exception_logger/migrations/0001_initial.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      381 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/migrations/0002_alter_exceptionmodel_exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/migrations/__init__.py
-drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:29:49.073019 django-exception-logger-0.1/exception_logger/models/
--rwxrwxrwx   0 titov     (1000) titov     (1000)      235 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/models/__init__.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     2366 2024-05-17 09:44:15.000000 django-exception-logger-0.1/exception_logger/models/celery_exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      215 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/models/enums.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     2791 2024-05-17 09:44:15.000000 django-exception-logger-0.1/exception_logger/models/exception.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1702 2024-05-17 09:46:43.000000 django-exception-logger-0.1/exception_logger/models/request_time.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)     1457 2024-05-06 12:59:31.000000 django-exception-logger-0.1/exception_logger/signals.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)      388 2024-05-17 09:03:36.000000 django-exception-logger-0.1/exception_logger/utils.py
--rwxrwxrwx   0 titov     (1000) titov     (1000)       38 2024-05-17 14:29:49.091687 django-exception-logger-0.1/setup.cfg
--rwxrwxrwx   0 titov     (1000) titov     (1000)      633 2024-05-17 14:29:44.000000 django-exception-logger-0.1/setup.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.488410 django-exception-logger-0.1.3/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1065 2024-05-17 09:26:59.000000 django-exception-logger-0.1.3/LICENSE
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      341 2024-05-17 14:18:21.000000 django-exception-logger-0.1.3/MANIFEST.in
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1679 2024-05-17 14:46:57.479411 django-exception-logger-0.1.3/PKG-INFO
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1351 2024-05-17 12:38:32.000000 django-exception-logger-0.1.3/README.md
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:56.944409 django-exception-logger-0.1.3/django_exception_logger.egg-info/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1679 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/PKG-INFO
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1035 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/SOURCES.txt
+-rwxrwxrwx   0 titov     (1000) titov     (1000)        1 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/dependency_links.txt
+-rwxrwxrwx   0 titov     (1000) titov     (1000)       12 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/requires.txt
+-rwxrwxrwx   0 titov     (1000) titov     (1000)       17 2024-05-17 14:46:56.000000 django-exception-logger-0.1.3/django_exception_logger.egg-info/top_level.txt
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.049565 django-exception-logger-0.1.3/exception_logger/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/__init__.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.141933 django-exception-logger-0.1.3/exception_logger/admin/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      193 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/admin/__init__.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1764 2024-05-17 09:33:45.000000 django-exception-logger-0.1.3/exception_logger/admin/celery_exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     2028 2024-05-17 12:38:32.000000 django-exception-logger-0.1.3/exception_logger/admin/exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      741 2024-05-17 12:38:32.000000 django-exception-logger-0.1.3/exception_logger/admin/request_time.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      253 2024-05-17 09:33:45.000000 django-exception-logger-0.1.3/exception_logger/apps.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      391 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/forms.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.212536 django-exception-logger-0.1.3/exception_logger/middlewares/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      106 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/middlewares/__init__.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1235 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/middlewares/exception_logger.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      620 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/middlewares/request_time.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.278745 django-exception-logger-0.1.3/exception_logger/migrations/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     6640 2024-05-17 09:46:17.000000 django-exception-logger-0.1.3/exception_logger/migrations/0001_initial.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      381 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/migrations/0002_alter_exceptionmodel_exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/migrations/__init__.py
+drwxrwxrwx   0 titov     (1000) titov     (1000)        0 2024-05-17 14:46:57.431801 django-exception-logger-0.1.3/exception_logger/models/
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      235 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/models/__init__.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     2366 2024-05-17 09:44:15.000000 django-exception-logger-0.1.3/exception_logger/models/celery_exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      215 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/models/enums.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     2791 2024-05-17 09:44:15.000000 django-exception-logger-0.1.3/exception_logger/models/exception.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1702 2024-05-17 09:46:43.000000 django-exception-logger-0.1.3/exception_logger/models/request_time.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)     1457 2024-05-06 12:59:31.000000 django-exception-logger-0.1.3/exception_logger/signals.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      387 2024-05-17 14:41:04.000000 django-exception-logger-0.1.3/exception_logger/utils.py
+-rwxrwxrwx   0 titov     (1000) titov     (1000)       38 2024-05-17 14:46:57.489429 django-exception-logger-0.1.3/setup.cfg
+-rwxrwxrwx   0 titov     (1000) titov     (1000)      636 2024-05-17 14:46:14.000000 django-exception-logger-0.1.3/setup.py
```

### Comparing `django-exception-logger-0.1/LICENSE` & `django-exception-logger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/PKG-INFO` & `django-exception-logger-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-exception-logger
-Version: 0.1
+Version: 0.1.3
 Summary: Adds error logging to the admin panel
 Home-page: https://github.com/Leonid-T/django-exception-logger/
 Author: Titov Leonid
 Author-email: titov281@yandex.ru
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django-exception-logger-0.1/README.md` & `django-exception-logger-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/django_exception_logger.egg-info/PKG-INFO` & `django-exception-logger-0.1.3/django_exception_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-exception-logger
-Version: 0.1
+Version: 0.1.3
 Summary: Adds error logging to the admin panel
 Home-page: https://github.com/Leonid-T/django-exception-logger/
 Author: Titov Leonid
 Author-email: titov281@yandex.ru
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `django-exception-logger-0.1/django_exception_logger.egg-info/SOURCES.txt` & `django-exception-logger-0.1.3/django_exception_logger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/admin/celery_exception.py` & `django-exception-logger-0.1.3/exception_logger/admin/celery_exception.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/admin/exception.py` & `django-exception-logger-0.1.3/exception_logger/admin/exception.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/admin/request_time.py` & `django-exception-logger-0.1.3/exception_logger/admin/request_time.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/middlewares/exception_logger.py` & `django-exception-logger-0.1.3/exception_logger/middlewares/exception_logger.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/middlewares/request_time.py` & `django-exception-logger-0.1.3/exception_logger/middlewares/request_time.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/migrations/0001_initial.py` & `django-exception-logger-0.1.3/exception_logger/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/models/celery_exception.py` & `django-exception-logger-0.1.3/exception_logger/models/celery_exception.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/models/exception.py` & `django-exception-logger-0.1.3/exception_logger/models/exception.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/models/request_time.py` & `django-exception-logger-0.1.3/exception_logger/models/request_time.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/exception_logger/signals.py` & `django-exception-logger-0.1.3/exception_logger/signals.py`

 * *Files identical despite different names*

### Comparing `django-exception-logger-0.1/setup.py` & `django-exception-logger-0.1.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
-README = open(os.path.join(here, 'README.md')).read()
+README = open(os.path.join(here, "README.md")).read()
 
 
 setup(
-    name='django-exception-logger',
-    version='0.1',
-    packages=find_packages(exclude=['tests*']),
-    description='Adds error logging to the admin panel',
+    name="django-exception-logger",
+    version="0.1.3",
+    packages=find_packages(exclude=["tests*"]),
+    description="Adds error logging to the admin panel",
     long_description=README,
-    long_description_content_type='text/markdown',
-    author='Titov Leonid',
-    author_email='titov281@yandex.ru',
-    url='https://github.com/Leonid-T/django-exception-logger/',
-    license='MIT',
+    long_description_content_type="text/markdown",
+    author="Titov Leonid",
+    author_email="titov281@yandex.ru",
+    url="https://github.com/Leonid-T/django-exception-logger/",
+    license="MIT",
     install_requires=[
-        'Django>=4.0',
-    ]
+        "Django>=4.0",
+    ],
 )
```

