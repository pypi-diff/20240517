# Comparing `tmp/weedata-0.2.6.tar.gz` & `tmp/weedata-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weedata-0.2.6.tar", last modified: Tue Apr 30 19:07:03 2024, max compression
+gzip compressed data, was "weedata-0.2.7.tar", last modified: Fri May 17 00:18:04 2024, max compression
```

## Comparing `weedata-0.2.6.tar` & `weedata-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.225186 weedata-0.2.6/
--rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    19300 2024-04-30 19:07:03.214186 weedata-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    16310 2024-04-30 18:09:55.000000 weedata-0.2.6/README.md
--rw-rw-rw-   0        0        0     1417 2024-04-30 18:10:10.000000 weedata-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 19:07:03.226186 weedata-0.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.065186 weedata-0.2.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.104186 weedata-0.2.6/src/weedata/
--rw-rw-rw-   0        0        0      497 2024-04-20 12:22:59.000000 weedata-0.2.6/src/weedata/__init__.py
--rw-rw-rw-   0        0        0    32289 2024-04-30 18:36:56.000000 weedata-0.2.6/src/weedata/client.py
--rw-rw-rw-   0        0        0    15767 2024-04-30 18:36:13.000000 weedata-0.2.6/src/weedata/fields.py
--rw-rw-rw-   0        0        0     9863 2024-04-20 12:22:08.000000 weedata-0.2.6/src/weedata/model.py
--rw-rw-rw-   0        0        0     8132 2024-04-19 12:41:56.000000 weedata-0.2.6/src/weedata/queries.py
-drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.211186 weedata-0.2.6/src/weedata.egg-info/
--rw-rw-rw-   0        0        0    19300 2024-04-30 19:07:02.000000 weedata-0.2.6/src/weedata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2024-04-30 19:07:03.000000 weedata-0.2.6/src/weedata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 19:07:03.000000 weedata-0.2.6/src/weedata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-30 19:07:03.000000 weedata-0.2.6/src/weedata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 19:07:03.191186 weedata-0.2.6/tests/
--rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.6/tests/test_base.py
--rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.6/tests/test_connection.py
--rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.6/tests/test_delete.py
--rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.6/tests/test_fields.py
--rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.6/tests/test_queries.py
--rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.6/tests/test_save.py
--rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.6/tests/test_update.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:18:04.465259 weedata-0.2.7/
+-rw-rw-rw-   0        0        0     1084 2024-02-06 11:15:24.000000 weedata-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    19349 2024-05-17 00:18:04.460259 weedata-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    16356 2024-05-17 00:13:27.000000 weedata-0.2.7/README.md
+-rw-rw-rw-   0        0        0     1417 2024-05-17 00:13:34.000000 weedata-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 00:18:04.466259 weedata-0.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 00:18:04.155259 weedata-0.2.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 00:18:04.239259 weedata-0.2.7/src/weedata/
+-rw-rw-rw-   0        0        0      497 2024-04-20 12:22:59.000000 weedata-0.2.7/src/weedata/__init__.py
+-rw-rw-rw-   0        0        0    32289 2024-04-30 18:36:56.000000 weedata-0.2.7/src/weedata/client.py
+-rw-rw-rw-   0        0        0    15767 2024-04-30 18:36:13.000000 weedata-0.2.7/src/weedata/fields.py
+-rw-rw-rw-   0        0        0     9863 2024-04-20 12:22:08.000000 weedata-0.2.7/src/weedata/model.py
+-rw-rw-rw-   0        0        0     8176 2024-05-17 00:12:14.000000 weedata-0.2.7/src/weedata/queries.py
+drwxrwxrwx   0        0        0        0 2024-05-17 00:18:04.456259 weedata-0.2.7/src/weedata.egg-info/
+-rw-rw-rw-   0        0        0    19349 2024-05-17 00:18:04.000000 weedata-0.2.7/src/weedata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2024-05-17 00:18:04.000000 weedata-0.2.7/src/weedata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 00:18:04.000000 weedata-0.2.7/src/weedata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 00:18:04.000000 weedata-0.2.7/src/weedata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 00:18:04.426259 weedata-0.2.7/tests/
+-rw-rw-rw-   0        0        0     4294 2024-03-16 22:05:45.000000 weedata-0.2.7/tests/test_base.py
+-rw-rw-rw-   0        0        0     3366 2024-02-24 09:33:45.000000 weedata-0.2.7/tests/test_connection.py
+-rw-rw-rw-   0        0        0     3085 2024-02-25 15:24:02.000000 weedata-0.2.7/tests/test_delete.py
+-rw-rw-rw-   0        0        0     9765 2024-02-25 23:41:43.000000 weedata-0.2.7/tests/test_fields.py
+-rw-rw-rw-   0        0        0     9033 2024-02-26 00:16:26.000000 weedata-0.2.7/tests/test_queries.py
+-rw-rw-rw-   0        0        0     1017 2024-02-24 09:34:08.000000 weedata-0.2.7/tests/test_save.py
+-rw-rw-rw-   0        0        0     5398 2024-02-25 17:34:27.000000 weedata-0.2.7/tests/test_update.py
```

### Comparing `weedata-0.2.6/LICENSE` & `weedata-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/PKG-INFO` & `weedata-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.6
+Version: 0.2.7
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -478,14 +478,17 @@
 
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
+* v0.2.7
+1. bugfix: fix query.dicts function
+
 
 * v0.2.6
 1. bugfix: Compatible with peewee, store datetime without timezone info.
 
 
 * v0.2.5
 1. bugfix: The compatibility problem of get_or_none().
```

### Comparing `weedata-0.2.6/README.md` & `weedata-0.2.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -428,14 +428,17 @@
 
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
+* v0.2.7
+1. bugfix: fix query.dicts function
+
 
 * v0.2.6
 1. bugfix: Compatible with peewee, store datetime without timezone info.
 
 
 * v0.2.5
 1. bugfix: The compatibility problem of get_or_none().
```

### Comparing `weedata-0.2.6/pyproject.toml` & `weedata-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "weedata"
-version = "0.2.6"
+version = "0.2.7"
 description = "an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 keywords = ["peewee", "ORM", "ODM", "google cloud datastore", "MongoDB", "redis"]
 dependencies = [
 #  "google-cloud-datastore",
```

### Comparing `weedata-0.2.6/src/weedata/client.py` & `weedata-0.2.7/src/weedata/client.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/src/weedata/fields.py` & `weedata-0.2.7/src/weedata/fields.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/src/weedata/model.py` & `weedata-0.2.7/src/weedata/model.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/src/weedata/queries.py` & `weedata-0.2.7/src/weedata/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self._distinct = [distinct_field]
         return self
 
     #the parameter limit will override the property of query object
     def execute(self, page_size=500, parent_key=None, limit=None):
         return self.client.execute(self, page_size=page_size, parent_key=parent_key, limit=limit)
     
-    def dicts(self):
+    def dicts(self, page_size=500, parent_key=None, limit=None):
         return self.client.execute(self, page_size=page_size, parent_key=parent_key, as_dict=True)
 
     def get(self):
         result = None
         try:
             result = next(self.execute(page_size=1, limit=1))
         except (TypeError, StopIteration):
```

### Comparing `weedata-0.2.6/src/weedata.egg-info/PKG-INFO` & `weedata-0.2.7/src/weedata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weedata
-Version: 0.2.6
+Version: 0.2.7
 Summary: an ORM/ODM for Google Cloud Datastore/MongoDB/redis, featuring a compatible interface with Peewee.
 Author-email: cdhigh <akindleear@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 cdhigh
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -478,14 +478,17 @@
 
 User.replace(name='python', score=100, birthdate=datetime.datetime(2024,1,1)).execute()
 
 ```
 
 
 # Changelog  
+* v0.2.7
+1. bugfix: fix query.dicts function
+
 
 * v0.2.6
 1. bugfix: Compatible with peewee, store datetime without timezone info.
 
 
 * v0.2.5
 1. bugfix: The compatibility problem of get_or_none().
```

### Comparing `weedata-0.2.6/tests/test_base.py` & `weedata-0.2.7/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/tests/test_connection.py` & `weedata-0.2.7/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/tests/test_delete.py` & `weedata-0.2.7/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/tests/test_fields.py` & `weedata-0.2.7/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/tests/test_queries.py` & `weedata-0.2.7/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/tests/test_save.py` & `weedata-0.2.7/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `weedata-0.2.6/tests/test_update.py` & `weedata-0.2.7/tests/test_update.py`

 * *Files identical despite different names*

