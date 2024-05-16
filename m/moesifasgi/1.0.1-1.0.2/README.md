# Comparing `tmp/moesifasgi-1.0.1.tar.gz` & `tmp/moesifasgi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moesifasgi-1.0.1.tar", last modified: Wed May  8 23:35:03 2024, max compression
+gzip compressed data, was "moesifasgi-1.0.2.tar", last modified: Thu May 16 22:48:35 2024, max compression
```

## Comparing `moesifasgi-1.0.1.tar` & `moesifasgi-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:35:03.221683 moesifasgi-1.0.1/
--rw-r--r--   0 keyur      (501) staff       (20)    11908 2021-08-28 00:36:27.000000 moesifasgi-1.0.1/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2021-08-28 00:36:31.000000 moesifasgi-1.0.1/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-08 23:35:03.221842 moesifasgi-1.0.1/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)    12564 2024-01-10 01:16:32.000000 moesifasgi-1.0.1/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:35:03.218761 moesifasgi-1.0.1/moesifasgi/
--rw-r--r--   0 keyur      (501) staff       (20)       26 2024-04-15 15:48:48.000000 moesifasgi-1.0.1/moesifasgi/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)      301 2021-08-28 00:35:10.000000 moesifasgi-1.0.1/moesifasgi/async_iterator_wrapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     4843 2024-03-29 23:20:02.000000 moesifasgi-1.0.1/moesifasgi/client_ip.py
--rw-r--r--   0 keyur      (501) staff       (20)     3592 2024-04-15 17:25:00.000000 moesifasgi-1.0.1/moesifasgi/event_mapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     9087 2024-04-15 17:25:00.000000 moesifasgi-1.0.1/moesifasgi/logger_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)    11096 2024-05-08 23:32:29.000000 moesifasgi-1.0.1/moesifasgi/middleware.py
--rw-r--r--   0 keyur      (501) staff       (20)     2218 2024-05-08 23:16:09.000000 moesifasgi-1.0.1/moesifasgi/send_batch_events.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-08 23:35:03.221459 moesifasgi-1.0.1/moesifasgi.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-08 23:35:03.000000 moesifasgi-1.0.1/moesifasgi.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)      413 2024-05-08 23:35:03.000000 moesifasgi-1.0.1/moesifasgi.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2024-05-08 23:35:03.000000 moesifasgi-1.0.1/moesifasgi.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)       82 2024-05-08 23:35:03.000000 moesifasgi-1.0.1/moesifasgi.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       11 2024-05-08 23:35:03.000000 moesifasgi-1.0.1/moesifasgi.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2024-05-08 23:35:03.222657 moesifasgi-1.0.1/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3269 2024-05-08 23:32:29.000000 moesifasgi-1.0.1/setup.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-16 22:48:35.603078 moesifasgi-1.0.2/
+-rw-r--r--   0 keyur      (501) staff       (20)    11908 2021-08-28 00:36:27.000000 moesifasgi-1.0.2/LICENSE
+-rw-r--r--   0 keyur      (501) staff       (20)       61 2021-08-28 00:36:31.000000 moesifasgi-1.0.2/MANIFEST.in
+-rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-16 22:48:35.603284 moesifasgi-1.0.2/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)    12564 2024-01-10 01:16:32.000000 moesifasgi-1.0.2/README.md
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-16 22:48:35.600315 moesifasgi-1.0.2/moesifasgi/
+-rw-r--r--   0 keyur      (501) staff       (20)       26 2024-04-15 15:48:48.000000 moesifasgi-1.0.2/moesifasgi/__init__.py
+-rw-r--r--   0 keyur      (501) staff       (20)      301 2021-08-28 00:35:10.000000 moesifasgi-1.0.2/moesifasgi/async_iterator_wrapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     4957 2024-05-16 22:46:04.000000 moesifasgi-1.0.2/moesifasgi/client_ip.py
+-rw-r--r--   0 keyur      (501) staff       (20)     3592 2024-05-16 17:14:06.000000 moesifasgi-1.0.2/moesifasgi/event_mapper.py
+-rw-r--r--   0 keyur      (501) staff       (20)     9087 2024-05-16 17:13:31.000000 moesifasgi-1.0.2/moesifasgi/logger_helper.py
+-rw-r--r--   0 keyur      (501) staff       (20)    11096 2024-05-16 22:46:04.000000 moesifasgi-1.0.2/moesifasgi/middleware.py
+-rw-r--r--   0 keyur      (501) staff       (20)     2218 2024-05-16 22:45:23.000000 moesifasgi-1.0.2/moesifasgi/send_batch_events.py
+drwxr-xr-x   0 keyur      (501) staff       (20)        0 2024-05-16 22:48:35.602766 moesifasgi-1.0.2/moesifasgi.egg-info/
+-rw-r--r--   0 keyur      (501) staff       (20)    13688 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/PKG-INFO
+-rw-r--r--   0 keyur      (501) staff       (20)      413 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/SOURCES.txt
+-rw-r--r--   0 keyur      (501) staff       (20)        1 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/dependency_links.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       82 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/requires.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       11 2024-05-16 22:48:35.000000 moesifasgi-1.0.2/moesifasgi.egg-info/top_level.txt
+-rw-r--r--   0 keyur      (501) staff       (20)       67 2024-05-16 22:48:35.604123 moesifasgi-1.0.2/setup.cfg
+-rw-r--r--   0 keyur      (501) staff       (20)     3269 2024-05-16 22:46:04.000000 moesifasgi-1.0.2/setup.py
```

### Comparing `moesifasgi-1.0.1/LICENSE` & `moesifasgi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.1/PKG-INFO` & `moesifasgi-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifasgi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Moesif Middleware for Python ASGI based platforms (FastAPI & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-asgi/
 Author: Moesif, Inc
 Author-email: keyur@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug asgi fastapi http middleware
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifasgi-1.0.1/README.md` & `moesifasgi-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.1/moesifasgi/client_ip.py` & `moesifasgi-1.0.2/moesifasgi/client_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,24 @@
 class ClientIp:
 
     def __init__(self):
         pass
 
     @classmethod
     def is_ip(cls, value):
-        if not value is None:
-            ipv4 = r"^(?:(?:\d|[1-9]\d|1\d{2}|2[0-4]\d|25[0-5])\.){3}(?:\d|[1-9]\d|1\d{2}|2[0-4]\d|25[0-5])$"
-            ipv6 = r"^((?=.*::)(?!.*::.+::)(::)?([\dA-F]{1,4}:(:|\b)|){5}|([\dA-F]{1,4}:){6})((([\dA-F]{1,4}((?!\3)::|:\b|$))|(?!\2\3)){2}|(((2[0-4]|1\d|[1-9])?\d|25[0-5])\.?\b){4})$/i"
-            return re.match(ipv4, value) or re.match(ipv6, value)
+        try:
+            if not value is None:
+                ipv4 = r"^(?:(?:\d|[1-9]\d|1\d{2}|2[0-4]\d|25[0-5])\.){3}(?:\d|[1-9]\d|1\d{2}|2[0-4]\d|25[0-5])$"
+                ipv6 = r"^((?=.*::)(?!.*::.+::)(::)?([\dA-F]{1,4}:(:|\b)|){5}|([\dA-F]{1,4}:){6})((([\dA-F]{1,4}((?!\3)::|:\b|$))|(?!\2\3)){2}|(((2[0-4]|1\d|[1-9])?\d|25[0-5])\.?\b){4})$/i"
+                return re.match(ipv4, value) or re.match(ipv6, value)
+        except:
+            # Ignore any error
+            pass
+
+        return None
 
     def getClientIpFromXForwardedFor(self, value, debug = False):
         try:
 
             if not value or value is None:
                 return None
```

### Comparing `moesifasgi-1.0.1/moesifasgi/event_mapper.py` & `moesifasgi-1.0.2/moesifasgi/event_mapper.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.1/moesifasgi/logger_helper.py` & `moesifasgi-1.0.2/moesifasgi/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.1/moesifasgi/middleware.py` & `moesifasgi-1.0.2/moesifasgi/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         except Exception as ex:
             self.is_config_job_scheduled = False
             if self.DEBUG:
                 logger.info(f'Error while starting the config scheduler job in background: {str(ex)}')
 
     def initialize_config(self):
         Configuration.BASE_URI = self.settings.get("BASE_URI", "https://api.moesif.net")
-        Configuration.version = 'moesifasgi-python/1.0.1'
+        Configuration.version = 'moesifasgi-python/1.0.2'
         self.LOG_BODY = self.settings.get("LOG_BODY", True)
 
         self.app_config = AppConfig()
         self.config = ConfigUpdateManager(self.api_client, self.app_config, self.DEBUG)
         self.schedule_config_job()
 
     def initialize_worker_pool(self):
```

### Comparing `moesifasgi-1.0.1/moesifasgi/send_batch_events.py` & `moesifasgi-1.0.2/moesifasgi/send_batch_events.py`

 * *Files identical despite different names*

### Comparing `moesifasgi-1.0.1/moesifasgi.egg-info/PKG-INFO` & `moesifasgi-1.0.2/moesifasgi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moesifasgi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Moesif Middleware for Python ASGI based platforms (FastAPI & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-asgi/
 Author: Moesif, Inc
 Author-email: keyur@moesif.com
 License: Apache Software License
 Keywords: log analysis restful api development debug asgi fastapi http middleware
 Classifier: Development Status :: 4 - Beta
```

### Comparing `moesifasgi-1.0.1/setup.py` & `moesifasgi-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifasgi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.1',
+    version='1.0.2',
 
     description='Moesif Middleware for Python ASGI based platforms (FastAPI & Others)',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-asgi/',
```

