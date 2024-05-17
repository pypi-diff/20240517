# Comparing `tmp/directory_healthcheck-3.5-py3-none-any.whl.zip` & `tmp/directory_healthcheck-3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5582 bytes, number of entries: 10
--rw-r--r--  2.0 unx       68 b- defN 24-Mar-05 14:21 directory_healthcheck/__init__.py
--rw-r--r--  2.0 unx      324 b- defN 24-Mar-05 14:21 directory_healthcheck/apps.py
--rw-r--r--  2.0 unx     2244 b- defN 24-Mar-05 14:21 directory_healthcheck/backends.py
--rw-r--r--  2.0 unx     1176 b- defN 24-Mar-05 14:21 directory_healthcheck/views.py
--rw-r--r--  2.0 unx      339 b- defN 24-Mar-05 14:21 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
--rw-r--r--  2.0 unx     1091 b- defN 24-Mar-05 14:21 directory_healthcheck-3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4069 b- defN 24-Mar-05 14:21 directory_healthcheck-3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-05 14:21 directory_healthcheck-3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-05 14:21 directory_healthcheck-3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      922 b- defN 24-Mar-05 14:21 directory_healthcheck-3.5.dist-info/RECORD
-10 files, 10347 bytes uncompressed, 3972 bytes compressed:  61.6%
+Zip file size: 5583 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       68 b- defN 24-May-17 13:37 directory_healthcheck/__init__.py
+-rw-r--r--  2.0 unx      324 b- defN 24-May-17 13:37 directory_healthcheck/apps.py
+-rw-r--r--  2.0 unx     2244 b- defN 24-May-17 13:37 directory_healthcheck/backends.py
+-rw-r--r--  2.0 unx     1176 b- defN 24-May-17 13:37 directory_healthcheck/views.py
+-rw-r--r--  2.0 unx      339 b- defN 24-May-17 13:37 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
+-rw-r--r--  2.0 unx     1091 b- defN 24-May-17 13:37 directory_healthcheck-3.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4069 b- defN 24-May-17 13:37 directory_healthcheck-3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 13:37 directory_healthcheck-3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 24-May-17 13:37 directory_healthcheck-3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      922 b- defN 24-May-17 13:37 directory_healthcheck-3.6.dist-info/RECORD
+10 files, 10347 bytes uncompressed, 3973 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_healthcheck/views.py
 Comment: 
 
 Filename: directory_healthcheck/templates/directory_healthcheck/healthcheck.html
 Comment: 
 
-Filename: directory_healthcheck-3.5.dist-info/LICENSE
+Filename: directory_healthcheck-3.6.dist-info/LICENSE
 Comment: 
 
-Filename: directory_healthcheck-3.5.dist-info/METADATA
+Filename: directory_healthcheck-3.6.dist-info/METADATA
 Comment: 
 
-Filename: directory_healthcheck-3.5.dist-info/WHEEL
+Filename: directory_healthcheck-3.6.dist-info/WHEEL
 Comment: 
 
-Filename: directory_healthcheck-3.5.dist-info/top_level.txt
+Filename: directory_healthcheck-3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_healthcheck-3.5.dist-info/RECORD
+Filename: directory_healthcheck-3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `directory_healthcheck-3.5.dist-info/LICENSE` & `directory_healthcheck-3.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_healthcheck-3.5.dist-info/METADATA` & `directory_healthcheck-3.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-healthcheck
-Version: 3.5
+Version: 3.6
 Summary: Library to streamline healthchecks for Directory apps.
 Home-page: https://github.com/uktrade/directory-healthcheck
 Author: Department for International Trade
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -20,15 +20,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django-health-check ==3.18.1
+Requires-Dist: django-health-check ==3.18.2
 Requires-Dist: django <5.0,>=4.2.10
 Provides-Extra: test
 Requires-Dist: pytest >=4.6.0 ; extra == 'test'
 Requires-Dist: pytest-cov >=2.11.0 ; extra == 'test'
 Requires-Dist: pytest-django ==4.8.0 ; extra == 'test'
 Requires-Dist: flake8 ==5.0.4 ; extra == 'test'
 Requires-Dist: codecov >=2.0.16 ; extra == 'test'
```

