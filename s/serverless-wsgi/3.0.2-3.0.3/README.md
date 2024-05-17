# Comparing `tmp/serverless-wsgi-3.0.2.tar.gz` & `tmp/serverless-wsgi-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serverless-wsgi-3.0.2.tar", last modified: Sat Feb 25 07:17:41 2023, max compression
+gzip compressed data, was "serverless-wsgi-3.0.3.tar", last modified: Thu Oct  5 09:32:39 2023, max compression
```

## Comparing `serverless-wsgi-3.0.2.tar` & `serverless-wsgi-3.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 logan      (501) staff       (20)        0 2023-02-25 07:17:41.819405 serverless-wsgi-3.0.2/
--rw-r--r--   0 logan      (501) staff       (20)     9972 2023-02-25 07:08:37.000000 serverless-wsgi-3.0.2/CHANGELOG.md
--rw-r--r--   0 logan      (501) staff       (20)     1069 2016-10-13 11:18:07.000000 serverless-wsgi-3.0.2/LICENSE
--rw-r--r--   0 logan      (501) staff       (20)       37 2018-08-02 22:20:40.000000 serverless-wsgi-3.0.2/MANIFEST.in
--rw-r--r--   0 logan      (501) staff       (20)    16625 2023-02-25 07:17:41.819483 serverless-wsgi-3.0.2/PKG-INFO
--rw-r--r--   0 logan      (501) staff       (20)    15973 2022-04-04 08:05:28.000000 serverless-wsgi-3.0.2/README.md
-drwxr-xr-x   0 logan      (501) staff       (20)        0 2023-02-25 07:17:41.819313 serverless-wsgi-3.0.2/serverless_wsgi.egg-info/
--rw-r--r--   0 logan      (501) staff       (20)    16625 2023-02-25 07:17:41.000000 serverless-wsgi-3.0.2/serverless_wsgi.egg-info/PKG-INFO
--rw-r--r--   0 logan      (501) staff       (20)      274 2023-02-25 07:17:41.000000 serverless-wsgi-3.0.2/serverless_wsgi.egg-info/SOURCES.txt
--rw-r--r--   0 logan      (501) staff       (20)        1 2023-02-25 07:17:41.000000 serverless-wsgi-3.0.2/serverless_wsgi.egg-info/dependency_links.txt
--rw-r--r--   0 logan      (501) staff       (20)       11 2023-02-25 07:17:41.000000 serverless-wsgi-3.0.2/serverless_wsgi.egg-info/requires.txt
--rw-r--r--   0 logan      (501) staff       (20)       16 2023-02-25 07:17:41.000000 serverless-wsgi-3.0.2/serverless_wsgi.egg-info/top_level.txt
--rw-r--r--   0 logan      (501) staff       (20)    11683 2023-02-25 07:11:21.000000 serverless-wsgi-3.0.2/serverless_wsgi.py
--rw-r--r--   0 logan      (501) staff       (20)      102 2023-02-25 07:17:41.819744 serverless-wsgi-3.0.2/setup.cfg
--rw-r--r--   0 logan      (501) staff       (20)      867 2023-02-25 07:08:57.000000 serverless-wsgi-3.0.2/setup.py
+drwxr-xr-x   0 logan      (501) staff       (20)        0 2023-10-05 09:32:39.940457 serverless-wsgi-3.0.3/
+-rw-r--r--   0 logan      (501) staff       (20)    10102 2023-10-05 09:24:52.000000 serverless-wsgi-3.0.3/CHANGELOG.md
+-rw-r--r--   0 logan      (501) staff       (20)     1069 2023-10-05 08:50:26.000000 serverless-wsgi-3.0.3/LICENSE
+-rw-r--r--   0 logan      (501) staff       (20)       37 2023-10-05 08:50:26.000000 serverless-wsgi-3.0.3/MANIFEST.in
+-rw-r--r--   0 logan      (501) staff       (20)    16588 2023-10-05 09:32:39.940562 serverless-wsgi-3.0.3/PKG-INFO
+-rw-r--r--   0 logan      (501) staff       (20)    15973 2023-10-05 08:50:26.000000 serverless-wsgi-3.0.3/README.md
+drwxr-xr-x   0 logan      (501) staff       (20)        0 2023-10-05 09:32:39.940333 serverless-wsgi-3.0.3/serverless_wsgi.egg-info/
+-rw-r--r--   0 logan      (501) staff       (20)    16588 2023-10-05 09:32:39.000000 serverless-wsgi-3.0.3/serverless_wsgi.egg-info/PKG-INFO
+-rw-r--r--   0 logan      (501) staff       (20)      274 2023-10-05 09:32:39.000000 serverless-wsgi-3.0.3/serverless_wsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 logan      (501) staff       (20)        1 2023-10-05 09:32:39.000000 serverless-wsgi-3.0.3/serverless_wsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 logan      (501) staff       (20)       11 2023-10-05 09:32:39.000000 serverless-wsgi-3.0.3/serverless_wsgi.egg-info/requires.txt
+-rw-r--r--   0 logan      (501) staff       (20)       16 2023-10-05 09:32:39.000000 serverless-wsgi-3.0.3/serverless_wsgi.egg-info/top_level.txt
+-rw-r--r--   0 logan      (501) staff       (20)    11690 2023-10-05 09:17:14.000000 serverless-wsgi-3.0.3/serverless_wsgi.py
+-rw-r--r--   0 logan      (501) staff       (20)      102 2023-10-05 09:32:39.940885 serverless-wsgi-3.0.3/setup.cfg
+-rw-r--r--   0 logan      (501) staff       (20)      867 2023-10-05 09:25:07.000000 serverless-wsgi-3.0.3/setup.py
```

### Comparing `serverless-wsgi-3.0.2/CHANGELOG.md` & `serverless-wsgi-3.0.3/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# 3.0.3
+
+## Features
+
+- As of Werkzeug 3.0.0, url_encode is no longer available, use the urllib counterparts
+
+  _Ryan Whittaker_
+
 # 3.0.2
 
 ## Features
 
 - Support base path stripping for v2 events
 - Default to https when protocol not specified in event
 - Add blacklist entries
```

### Comparing `serverless-wsgi-3.0.2/LICENSE` & `serverless-wsgi-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `serverless-wsgi-3.0.2/PKG-INFO` & `serverless-wsgi-3.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: serverless-wsgi
-Version: 3.0.2
+Version: 3.0.3
 Summary: Amazon AWS API Gateway WSGI wrapper
 Home-page: https://github.com/logandk/serverless-wsgi
 Author: Logan Raarup
 Author-email: logan@logan.dk
-License: UNKNOWN
 Keywords: wsgi serverless aws lambda api gateway apigw flask django pyramid
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
@@ -554,9 +552,7 @@
 # Thanks
 
 Thanks to [Zappa](https://github.com/Miserlou/Zappa), which has been both the
 inspiration and source of several implementations that went into this project.
 
 Thanks to [chalice](https://github.com/awslabs/chalice) for the
 requirement packaging implementation.
-
-
```

### Comparing `serverless-wsgi-3.0.2/README.md` & `serverless-wsgi-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `serverless-wsgi-3.0.2/serverless_wsgi.egg-info/PKG-INFO` & `serverless-wsgi-3.0.3/serverless_wsgi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: serverless-wsgi
-Version: 3.0.2
+Version: 3.0.3
 Summary: Amazon AWS API Gateway WSGI wrapper
 Home-page: https://github.com/logandk/serverless-wsgi
 Author: Logan Raarup
 Author-email: logan@logan.dk
-License: UNKNOWN
 Keywords: wsgi serverless aws lambda api gateway apigw flask django pyramid
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
@@ -554,9 +552,7 @@
 # Thanks
 
 Thanks to [Zappa](https://github.com/Miserlou/Zappa), which has been both the
 inspiration and source of several implementations that went into this project.
 
 Thanks to [chalice](https://github.com/awslabs/chalice) for the
 requirement packaging implementation.
-
-
```

### Comparing `serverless-wsgi-3.0.2/serverless_wsgi.py` & `serverless-wsgi-3.0.3/serverless_wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 Author: Logan Raarup <logan@logan.dk>
 """
 import base64
 import io
 import json
 import os
 import sys
-from werkzeug.datastructures import Headers, iter_multi_items, MultiDict
-from werkzeug.wrappers import Response
-from werkzeug.urls import url_encode, url_unquote, url_unquote_plus
-from werkzeug.http import HTTP_STATUS_CODES
+from urllib.parse import urlencode, unquote, unquote_plus
 
+from werkzeug.datastructures import Headers, iter_multi_items
+from werkzeug.http import HTTP_STATUS_CODES
+from werkzeug.wrappers import Response
 
 # List of MIME types that should not be base64 encoded. MIME types within `text/*`
 # are included by default.
 TEXT_MIME_TYPES = [
     "application/json",
     "application/javascript",
     "application/xml",
@@ -86,19 +86,19 @@
     if not params:
         params = event.get("queryStringParameters")
     if not params:
         params = event.get("query")
     if not params:
         params = ""
     if is_alb_event(event):
-        params = MultiDict(
-            (url_unquote_plus(k), url_unquote_plus(v))
+        params = [
+            (unquote_plus(k), unquote_plus(v))
             for k, v in iter_multi_items(params)
-        )
-    return url_encode(params)
+        ]
+    return urlencode(params, doseq=True)
 
 
 def get_script_name(headers, request_context):
     strip_stage_path = os.environ.get("STRIP_STAGE_PATH", "").lower().strip() in [
         "yes",
         "y",
         "true",
@@ -147,20 +147,21 @@
             response.status_code,
             HTTP_STATUS_CODES[response.status_code],
         )
 
     if response.data:
         mimetype = response.mimetype or "text/plain"
         if (
-            mimetype.startswith("text/") or mimetype in TEXT_MIME_TYPES
+                mimetype.startswith("text/") or mimetype in TEXT_MIME_TYPES
         ) and not response.headers.get("Content-Encoding", ""):
             returndict["body"] = response.get_data(as_text=True)
             returndict["isBase64Encoded"] = False
         else:
-            returndict["body"] = base64.b64encode(response.data).decode("utf-8")
+            returndict["body"] = base64.b64encode(
+                response.data).decode("utf-8")
             returndict["isBase64Encoded"] = True
 
     return returndict
 
 
 def strip_express_gateway_query_params(path):
     """Contrary to regular AWS lambda HTTP events, Express Gateway
@@ -174,18 +175,18 @@
 
 def handle_request(app, event, context):
     if event.get("source") in ["aws.events", "serverless-plugin-warmup"]:
         print("Lambda warming event received, skipping handler")
         return {}
 
     if (
-        event.get("version") is None
-        and event.get("isBase64Encoded") is None
-        and event.get("requestPath") is not None
-        and not is_alb_event(event)
+            event.get("version") is None
+            and event.get("isBase64Encoded") is None
+            and event.get("requestPath") is not None
+            and not is_alb_event(event)
     ):
         return handle_lambda_integration(app, event, context)
 
     if event.get("version") == "2.0":
         return handle_payload_v2(app, event, context)
 
     return handle_payload_v1(app, event, context)
@@ -204,23 +205,23 @@
     # environment variable.
     path_info = strip_express_gateway_query_params(event["path"])
     base_path = os.environ.get("API_GATEWAY_BASE_PATH")
     if base_path:
         script_name = "/" + base_path
 
         if path_info.startswith(script_name):
-            path_info = path_info[len(script_name) :]
+            path_info = path_info[len(script_name):]
 
     body = event.get("body") or ""
     body = get_body_bytes(event, body)
 
     environ = {
         "CONTENT_LENGTH": str(len(body)),
         "CONTENT_TYPE": headers.get("Content-Type", ""),
-        "PATH_INFO": url_unquote(path_info),
+        "PATH_INFO": unquote(path_info),
         "QUERY_STRING": encode_query_string(event),
         "REMOTE_ADDR": event.get("requestContext", {})
         .get("identity", {})
         .get("sourceIp", ""),
         "REMOTE_USER": (event.get("requestContext", {})
                         .get("authorizer") or {})
         .get("principalId", ""),
@@ -256,25 +257,25 @@
 
     path_info = strip_express_gateway_query_params(event["rawPath"])
     base_path = os.environ.get("API_GATEWAY_BASE_PATH")
     if base_path:
         script_name = "/" + base_path
 
         if path_info.startswith(script_name):
-            path_info = path_info[len(script_name) :]
+            path_info = path_info[len(script_name):]
 
     body = event.get("body", "")
     body = get_body_bytes(event, body)
 
     headers["Cookie"] = "; ".join(event.get("cookies", []))
 
     environ = {
         "CONTENT_LENGTH": str(len(body or "")),
         "CONTENT_TYPE": headers.get("Content-Type", ""),
-        "PATH_INFO": url_unquote(path_info),
+        "PATH_INFO": unquote(path_info),
         "QUERY_STRING": event.get("rawQueryString", ""),
         "REMOTE_ADDR": event.get("requestContext", {})
         .get("http", {})
         .get("sourceIp", ""),
         "REMOTE_USER": event.get("requestContext", {})
         .get("authorizer", {})
         .get("principalId", ""),
@@ -320,16 +321,16 @@
     body = event.get("body", {})
     body = json.dumps(body) if body else ""
     body = get_body_bytes(event, body)
 
     environ = {
         "CONTENT_LENGTH": str(len(body or "")),
         "CONTENT_TYPE": headers.get("Content-Type", ""),
-        "PATH_INFO": url_unquote(path_info),
-        "QUERY_STRING": url_encode(event.get("query", {})),
+        "PATH_INFO": unquote(path_info),
+        "QUERY_STRING": urlencode(event.get("query", {}), doseq=True),
         "REMOTE_ADDR": event.get("identity", {}).get("sourceIp", ""),
         "REMOTE_USER": event.get("principalId", ""),
         "REQUEST_METHOD": event.get("method", ""),
         "SCRIPT_NAME": script_name,
         "SERVER_NAME": headers.get("Host", "lambda"),
         "SERVER_PORT": headers.get("X-Forwarded-Port", "443"),
         "SERVER_PROTOCOL": "HTTP/1.1",
```

### Comparing `serverless-wsgi-3.0.2/setup.py` & `serverless-wsgi-3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="serverless-wsgi",
-    version="3.0.2",
+    version="3.0.3",
     python_requires=">3.6",
     author="Logan Raarup",
     author_email="logan@logan.dk",
     description="Amazon AWS API Gateway WSGI wrapper",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/logandk/serverless-wsgi",
```

