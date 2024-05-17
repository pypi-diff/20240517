# Comparing `tmp/predibase-api-2024.4.8.tar.gz` & `tmp/predibase-api-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-api-2024.4.8.tar", last modified: Sat Apr 20 01:07:52 2024, max compression
+gzip compressed data, was "predibase-api-2024.5.1.tar", last modified: Fri May 17 00:14:20 2024, max compression
```

## Comparing `predibase-api-2024.4.8.tar` & `predibase-api-2024.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.352036 predibase-api-2024.4.8/predibase_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.352036 predibase-api-2024.4.8/predibase_api/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.352036 predibase-api-2024.4.8/predibase_api/artifacts/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/artifacts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-20 01:07:49.000000 predibase-api-2024.4.8/predibase_api/artifacts/v1/artifacts_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.352036 predibase-api-2024.4.8/predibase_api/foobar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/foobar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.352036 predibase-api-2024.4.8/predibase_api/foobar/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/foobar/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-20 01:07:47.000000 predibase-api-2024.4.8/predibase_api/foobar/v1/bar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-20 01:07:47.000000 predibase-api-2024.4.8/predibase_api/foobar/v1/foo_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/predibase_api/iterml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/iterml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/predibase_api/iterml/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/iterml/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-20 01:07:50.000000 predibase-api-2024.4.8/predibase_api/iterml/v1/iterml_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/predibase_api/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/profiles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/predibase_api/profiles/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/profiles/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-04-20 01:07:51.000000 predibase-api-2024.4.8/predibase_api/profiles/v1/dataset_profile_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/predibase_api/tenants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/tenants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/predibase_api/tenants/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/predibase_api/tenants/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-20 01:07:48.000000 predibase-api-2024.4.8/predibase_api/tenants/v1/tenants_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.352036 predibase-api-2024.4.8/predibase_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-20 01:07:52.000000 predibase-api-2024.4.8/predibase_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-20 01:07:52.000000 predibase-api-2024.4.8/predibase_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:07:52.000000 predibase-api-2024.4.8/predibase_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:07:06.000000 predibase-api-2024.4.8/predibase_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:07:52.000000 predibase-api-2024.4.8/predibase_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-20 01:07:52.000000 predibase-api-2024.4.8/predibase_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:07:52.356036 predibase-api-2024.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-20 01:06:03.000000 predibase-api-2024.4.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:07:45.000000 predibase-api-2024.4.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.785695 predibase-api-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/artifacts/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/artifacts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-17 00:14:18.000000 predibase-api-2024.5.1/predibase_api/artifacts/v1/artifacts_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/foobar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/foobar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/foobar/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/foobar/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-17 00:14:15.000000 predibase-api-2024.5.1/predibase_api/foobar/v1/bar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-17 00:14:14.000000 predibase-api-2024.5.1/predibase_api/foobar/v1/foo_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/iterml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/iterml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/iterml/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/iterml/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-17 00:14:16.000000 predibase-api-2024.5.1/predibase_api/iterml/v1/iterml_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/profiles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/profiles/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/profiles/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8016 2024-05-17 00:14:17.000000 predibase-api-2024.5.1/predibase_api/profiles/v1/dataset_profile_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/tenants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/tenants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api/tenants/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/predibase_api/tenants/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-17 00:14:19.000000 predibase-api-2024.5.1/predibase_api/tenants/v1/tenants_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:20.781695 predibase-api-2024.5.1/predibase_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-17 00:14:20.000000 predibase-api-2024.5.1/predibase_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-17 00:14:20.000000 predibase-api-2024.5.1/predibase_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:14:20.000000 predibase-api-2024.5.1/predibase_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:13:21.000000 predibase-api-2024.5.1/predibase_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 00:14:20.000000 predibase-api-2024.5.1/predibase_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 00:14:20.000000 predibase-api-2024.5.1/predibase_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 00:14:20.785695 predibase-api-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-17 00:11:52.000000 predibase-api-2024.5.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 00:14:13.000000 predibase-api-2024.5.1/version.txt
```

### Comparing `predibase-api-2024.4.8/predibase_api/artifacts/v1/artifacts_pb2.py` & `predibase-api-2024.5.1/predibase_api/artifacts/v1/artifacts_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.8/predibase_api/foobar/v1/bar_pb2.py` & `predibase-api-2024.5.1/predibase_api/foobar/v1/bar_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.8/predibase_api/foobar/v1/foo_pb2.py` & `predibase-api-2024.5.1/predibase_api/foobar/v1/foo_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.8/predibase_api/iterml/v1/iterml_pb2.py` & `predibase-api-2024.5.1/predibase_api/iterml/v1/iterml_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.8/predibase_api/profiles/v1/dataset_profile_pb2.py` & `predibase-api-2024.5.1/predibase_api/profiles/v1/dataset_profile_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.8/predibase_api/tenants/v1/tenants_pb2.py` & `predibase-api-2024.5.1/predibase_api/tenants/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.8/predibase_api.egg-info/SOURCES.txt` & `predibase-api-2024.5.1/predibase_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `predibase-api-2024.4.8/setup.py` & `predibase-api-2024.5.1/setup.py`

 * *Files identical despite different names*

