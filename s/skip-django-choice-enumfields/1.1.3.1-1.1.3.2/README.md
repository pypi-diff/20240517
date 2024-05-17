# Comparing `tmp/skip-django-choice-enumfields-1.1.3.1.tar.gz` & `tmp/skip-django-choice-enumfields-1.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-choice-enumfields-1.1.3.1.tar", last modified: Thu Jan 12 13:25:58 2023, max compression
+gzip compressed data, was "skip-django-choice-enumfields-1.1.3.2.tar", last modified: Thu Jan 12 15:12:51 2023, max compression
```

## Comparing `skip-django-choice-enumfields-1.1.3.1.tar` & `skip-django-choice-enumfields-1.1.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:25:58.747570 skip-django-choice-enumfields-1.1.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-01-12 13:25:58.747570 skip-django-choice-enumfields-1.1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:25:58.747570 skip-django-choice-enumfields-1.1.3.1/enumfields/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:25:58.747570 skip-django-choice-enumfields-1.1.3.1/enumfields/drf/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/drf/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/drf/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/enumfields/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-12 13:25:58.751570 skip-django-choice-enumfields-1.1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-01-12 13:25:47.000000 skip-django-choice-enumfields-1.1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 13:25:58.747570 skip-django-choice-enumfields-1.1.3.1/skip_django_choice_enumfields.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-01-12 13:25:58.000000 skip-django-choice-enumfields-1.1.3.1/skip_django_choice_enumfields.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-12 13:25:58.000000 skip-django-choice-enumfields-1.1.3.1/skip_django_choice_enumfields.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 13:25:58.000000 skip-django-choice-enumfields-1.1.3.1/skip_django_choice_enumfields.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 13:25:58.000000 skip-django-choice-enumfields-1.1.3.1/skip_django_choice_enumfields.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-12 13:25:58.000000 skip-django-choice-enumfields-1.1.3.1/skip_django_choice_enumfields.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:12:51.751741 skip-django-choice-enumfields-1.1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-01-12 15:12:51.751741 skip-django-choice-enumfields-1.1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:12:51.751741 skip-django-choice-enumfields-1.1.3.2/enumfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:12:51.751741 skip-django-choice-enumfields-1.1.3.2/enumfields/drf/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/drf/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/drf/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/enumfields/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-12 15:12:51.751741 skip-django-choice-enumfields-1.1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-01-12 15:12:42.000000 skip-django-choice-enumfields-1.1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:12:51.751741 skip-django-choice-enumfields-1.1.3.2/skip_django_choice_enumfields.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-01-12 15:12:51.000000 skip-django-choice-enumfields-1.1.3.2/skip_django_choice_enumfields.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-12 15:12:51.000000 skip-django-choice-enumfields-1.1.3.2/skip_django_choice_enumfields.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:12:51.000000 skip-django-choice-enumfields-1.1.3.2/skip_django_choice_enumfields.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:12:51.000000 skip-django-choice-enumfields-1.1.3.2/skip_django_choice_enumfields.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-12 15:12:51.000000 skip-django-choice-enumfields-1.1.3.2/skip_django_choice_enumfields.egg-info/top_level.txt
```

### Comparing `skip-django-choice-enumfields-1.1.3.1/LICENSE` & `skip-django-choice-enumfields-1.1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/PKG-INFO` & `skip-django-choice-enumfields-1.1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: skip-django-choice-enumfields
-Version: 1.1.3.1
+Version: 1.1.3.2
 Summary: Real Python Enums for Django.
-Home-page: https://github.com/druids/django-choice-enumfields
+Home-page: https://github.com/skip-pay/django-choice-enumfields
 Author: HZDG, Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
```

### Comparing `skip-django-choice-enumfields-1.1.3.1/README.rst` & `skip-django-choice-enumfields-1.1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/enumfields/admin.py` & `skip-django-choice-enumfields-1.1.3.2/enumfields/admin.py`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/enumfields/drf/fields.py` & `skip-django-choice-enumfields-1.1.3.2/enumfields/drf/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/enumfields/drf/serializers.py` & `skip-django-choice-enumfields-1.1.3.2/enumfields/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/enumfields/enums.py` & `skip-django-choice-enumfields-1.1.3.2/enumfields/enums.py`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/enumfields/fields.py` & `skip-django-choice-enumfields-1.1.3.2/enumfields/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/enumfields/forms.py` & `skip-django-choice-enumfields-1.1.3.2/enumfields/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/setup.cfg` & `skip-django-choice-enumfields-1.1.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `skip-django-choice-enumfields-1.1.3.1/setup.py` & `skip-django-choice-enumfields-1.1.3.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,20 +25,20 @@
         os.environ['DJANGO_SETTINGS_MODULE'] = 'tests.settings'
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 setup(
     name='skip-django-choice-enumfields',
-    version='1.1.3.1',
+    version='1.1.3.2',
     author='HZDG, Lubos Matl',
     author_email='matllubos@gmail.com',
     description='Real Python Enums for Django.',
     license='MIT',
-    url='https://github.com/druids/django-choice-enumfields',
+    url='https://github.com/skip-pay/django-choice-enumfields',
     long_description=README,
     packages=find_packages(exclude=['tests*']),
     zip_safe=False,
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 3.1',
```

### Comparing `skip-django-choice-enumfields-1.1.3.1/skip_django_choice_enumfields.egg-info/PKG-INFO` & `skip-django-choice-enumfields-1.1.3.2/skip_django_choice_enumfields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: skip-django-choice-enumfields
-Version: 1.1.3.1
+Version: 1.1.3.2
 Summary: Real Python Enums for Django.
-Home-page: https://github.com/druids/django-choice-enumfields
+Home-page: https://github.com/skip-pay/django-choice-enumfields
 Author: HZDG, Lubos Matl
 Author-email: matllubos@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
```

