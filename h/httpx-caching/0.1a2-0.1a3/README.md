# Comparing `tmp/httpx-caching-0.1a2.tar.gz` & `tmp/httpx-caching-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx-caching-0.1a2.tar", last modified: Fri Mar 18 21:55:45 2022, max compression
+gzip compressed data, was "httpx-caching-0.1a3.tar", last modified: Wed Aug 23 21:09:49 2023, max compression
```

## Comparing `httpx-caching-0.1a2.tar` & `httpx-caching-0.1a3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:55:45.827581 httpx-caching-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-03-18 21:55:45.827581 httpx-caching-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:55:45.827581 httpx-caching-0.1a2/httpx_caching/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:55:45.827581 httpx-caching-0.1a2/httpx_caching/_async/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_async/_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     4512 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_async/_transport.py
--rw-r--r--   0 runner    (1001) docker     (121)     4426 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_heuristics.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    18873 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_policy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:55:45.827581 httpx-caching-0.1a2/httpx_caching/_sync/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_sync/_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     4347 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_sync/_transport.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     3063 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/httpx_caching/_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-18 21:55:45.827581 httpx-caching-0.1a2/httpx_caching.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-03-18 21:55:45.000000 httpx-caching-0.1a2/httpx_caching.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-03-18 21:55:45.000000 httpx-caching-0.1a2/httpx_caching.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 21:55:45.000000 httpx-caching-0.1a2/httpx_caching.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-18 21:55:44.000000 httpx-caching-0.1a2/httpx_caching.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-03-18 21:55:45.000000 httpx-caching-0.1a2/httpx_caching.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-03-18 21:55:45.000000 httpx-caching-0.1a2/httpx_caching.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-03-18 21:55:45.831581 httpx-caching-0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2214 2022-03-18 21:55:17.000000 httpx-caching-0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 21:09:49.145445 httpx-caching-0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-23 21:09:49.145445 httpx-caching-0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 21:09:49.141445 httpx-caching-0.1a3/httpx_caching/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 21:09:49.141445 httpx-caching-0.1a3/httpx_caching/_async/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_async/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_async/_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_heuristics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 21:09:49.145445 httpx-caching-0.1a3/httpx_caching/_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_sync/_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_sync/_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/httpx_caching/_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 21:09:49.141445 httpx-caching-0.1a3/httpx_caching.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-23 21:09:49.000000 httpx-caching-0.1a3/httpx_caching.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-08-23 21:09:49.000000 httpx-caching-0.1a3/httpx_caching.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 21:09:49.000000 httpx-caching-0.1a3/httpx_caching.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 21:09:48.000000 httpx-caching-0.1a3/httpx_caching.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-23 21:09:49.000000 httpx-caching-0.1a3/httpx_caching.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-23 21:09:49.000000 httpx-caching-0.1a3/httpx_caching.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-08-23 21:09:49.145445 httpx-caching-0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-08-23 21:09:26.000000 httpx-caching-0.1a3/setup.py
```

### Comparing `httpx-caching-0.1a2/PKG-INFO` & `httpx-caching-0.1a3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-caching
-Version: 0.1a2
+Version: 0.1a3
 Summary: Caching for HTTPX.
 Home-page: https://github.com/johtso/httpx-caching
 Author: Johannes (johtso)
 Author-email: johtso@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/johtso/httpx-caching
 Platform: UNKNOWN
@@ -25,14 +25,17 @@
 
 <p align="center">Caching for HTTPX.</em></p>
 
 <p align="center">
 <a href="https://github.com/johtso/httpx-caching/actions">
     <img src="https://github.com/johtso/httpx-caching/workflows/Test%20Suite/badge.svg" alt="Test Suite">
 </a>
+<a href="https://pypi.org/project/httpx-caching/">
+    <img src="https://badge.fury.io/py/httpx-caching.svg" alt="Package version">
+</a>
 </p>
 
 **Note**: Early development / alpha, use at your own risk.
 
 This package adds caching functionality to [HTTPX](https://github.com/encode/httpx)
 
 Adapted from Eric Larson's fantastic [CacheControl](https://github.com/ionrock/cachecontrol) for [requests](https://requests.readthedocs.io/en/stable/).
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: httpx-caching Version: 0.1a2 Summary: Caching for
+Metadata-Version: 2.1 Name: httpx-caching Version: 0.1a3 Summary: Caching for
 HTTPX. Home-page: https://github.com/johtso/httpx-caching Author: Johannes
 (johtso) Author-email: johtso@gmail.com License: Apache-2.0 Project-URL:
 Source, https://github.com/johtso/httpx-caching Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3 :: Only Requires-Python: >=3.7 Description-
 Content-Type: text/markdown
                               Caching for HTTPX.
-                                 _[_T_e_s_t_ _S_u_i_t_e_]
+                         _[_T_e_s_t_ _S_u_i_t_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 **Note**: Early development / alpha, use at your own risk. This package adds
 caching functionality to [HTTPX](https://github.com/encode/httpx) Adapted from
 Eric Larson's fantastic [CacheControl](https://github.com/ionrock/cachecontrol)
 for [requests](https://requests.readthedocs.io/en/stable/). Project goals: -
 [x] Sans-io caching protocol - [x] Fully async compatible - [ ] Support
 multiple http clients (currently only supports httpx) Limitations: * Currently
 only has in-memory cache storage (async redis would be nice!) * Test suite was
```

### Comparing `httpx-caching-0.1a2/README.md` & `httpx-caching-0.1a3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 <p align="center">Caching for HTTPX.</em></p>
 
 <p align="center">
 <a href="https://github.com/johtso/httpx-caching/actions">
     <img src="https://github.com/johtso/httpx-caching/workflows/Test%20Suite/badge.svg" alt="Test Suite">
 </a>
+<a href="https://pypi.org/project/httpx-caching/">
+    <img src="https://badge.fury.io/py/httpx-caching.svg" alt="Package version">
+</a>
 </p>
 
 **Note**: Early development / alpha, use at your own risk.
 
 This package adds caching functionality to [HTTPX](https://github.com/encode/httpx)
 
 Adapted from Eric Larson's fantastic [CacheControl](https://github.com/ionrock/cachecontrol) for [requests](https://requests.readthedocs.io/en/stable/).
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
                               Caching for HTTPX.
-                                 _[_T_e_s_t_ _S_u_i_t_e_]
+                         _[_T_e_s_t_ _S_u_i_t_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 **Note**: Early development / alpha, use at your own risk. This package adds
 caching functionality to [HTTPX](https://github.com/encode/httpx) Adapted from
 Eric Larson's fantastic [CacheControl](https://github.com/ionrock/cachecontrol)
 for [requests](https://requests.readthedocs.io/en/stable/). Project goals: -
 [x] Sans-io caching protocol - [x] Fully async compatible - [ ] Support
 multiple http clients (currently only supports httpx) Limitations: * Currently
 only has in-memory cache storage (async redis would be nice!) * Test suite was
```

### Comparing `httpx-caching-0.1a2/httpx_caching/__init__.py` & `httpx-caching-0.1a3/httpx_caching/__init__.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching/_async/_cache.py` & `httpx-caching-0.1a3/httpx_caching/_async/_cache.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching/_async/_transport.py` & `httpx-caching-0.1a3/httpx_caching/_async/_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     @aio_handler.register
     async def _io_make_request(self, action: protocol.MakeRequest) -> Response:
         response = await self.transport.handle_async_request(action.request)  # type: ignore
         return Response(
             status_code=response.status_code,
             headers=response.headers,
             stream=response.stream,  # type: ignore
-            extensions=response.extensions,
+            extensions=response.extensions,  # type: ignore
         )
 
     @aio_handler.register
     async def _io_close_response_stream(
         self, action: protocol.CloseResponseStream
     ) -> None:
         await action.response.stream.aclose()
```

### Comparing `httpx-caching-0.1a2/httpx_caching/_heuristics.py` & `httpx-caching-0.1a3/httpx_caching/_heuristics.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching/_policy.py` & `httpx-caching-0.1a3/httpx_caching/_policy.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching/_serializer.py` & `httpx-caching-0.1a3/httpx_caching/_serializer.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching/_sync/_cache.py` & `httpx-caching-0.1a3/httpx_caching/_sync/_cache.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching/_sync/_transport.py` & `httpx-caching-0.1a3/httpx_caching/_sync/_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     @io_handler.register
     def _io_make_request(self, action: protocol.MakeRequest) -> Response:
         response = self.transport.handle_request(action.request)  # type: ignore
         return Response(
             status_code=response.status_code,
             headers=response.headers,
             stream=response.stream,  # type: ignore
-            extensions=response.extensions,
+            extensions=response.extensions,  # type: ignore
         )
 
     @io_handler.register
     def _io_close_response_stream(self, action: protocol.CloseResponseStream) -> None:
         action.response.stream.close()
         return None
```

### Comparing `httpx-caching-0.1a2/httpx_caching/_utils.py` & `httpx-caching-0.1a3/httpx_caching/_utils.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching/_wrapper.py` & `httpx-caching-0.1a3/httpx_caching/_wrapper.py`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/httpx_caching.egg-info/PKG-INFO` & `httpx-caching-0.1a3/httpx_caching.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx-caching
-Version: 0.1a2
+Version: 0.1a3
 Summary: Caching for HTTPX.
 Home-page: https://github.com/johtso/httpx-caching
 Author: Johannes (johtso)
 Author-email: johtso@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/johtso/httpx-caching
 Platform: UNKNOWN
@@ -25,14 +25,17 @@
 
 <p align="center">Caching for HTTPX.</em></p>
 
 <p align="center">
 <a href="https://github.com/johtso/httpx-caching/actions">
     <img src="https://github.com/johtso/httpx-caching/workflows/Test%20Suite/badge.svg" alt="Test Suite">
 </a>
+<a href="https://pypi.org/project/httpx-caching/">
+    <img src="https://badge.fury.io/py/httpx-caching.svg" alt="Package version">
+</a>
 </p>
 
 **Note**: Early development / alpha, use at your own risk.
 
 This package adds caching functionality to [HTTPX](https://github.com/encode/httpx)
 
 Adapted from Eric Larson's fantastic [CacheControl](https://github.com/ionrock/cachecontrol) for [requests](https://requests.readthedocs.io/en/stable/).
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: httpx-caching Version: 0.1a2 Summary: Caching for
+Metadata-Version: 2.1 Name: httpx-caching Version: 0.1a3 Summary: Caching for
 HTTPX. Home-page: https://github.com/johtso/httpx-caching Author: Johannes
 (johtso) Author-email: johtso@gmail.com License: Apache-2.0 Project-URL:
 Source, https://github.com/johtso/httpx-caching Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3 :: Only Requires-Python: >=3.7 Description-
 Content-Type: text/markdown
                               Caching for HTTPX.
-                                 _[_T_e_s_t_ _S_u_i_t_e_]
+                         _[_T_e_s_t_ _S_u_i_t_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 **Note**: Early development / alpha, use at your own risk. This package adds
 caching functionality to [HTTPX](https://github.com/encode/httpx) Adapted from
 Eric Larson's fantastic [CacheControl](https://github.com/ionrock/cachecontrol)
 for [requests](https://requests.readthedocs.io/en/stable/). Project goals: -
 [x] Sans-io caching protocol - [x] Fully async compatible - [ ] Support
 multiple http clients (currently only supports httpx) Limitations: * Currently
 only has in-memory cache storage (async redis would be nice!) * Test suite was
```

### Comparing `httpx-caching-0.1a2/httpx_caching.egg-info/SOURCES.txt` & `httpx-caching-0.1a3/httpx_caching.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpx-caching-0.1a2/setup.py` & `httpx-caching-0.1a3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     author="Johannes (johtso)",
     author_email="johtso@gmail.com",
     package_data={"httpx_caching": ["py.typed"]},
     packages=get_packages("httpx_caching"),
     include_package_data=True,
     zip_safe=False,
     install_requires=[
-        "httpx==0.22.*",
+        "httpx>=0.22.0,<0.24.0",
         "msgpack",  
         "anyio",
         "multimethod",
     ],
     extras_require={},
     classifiers=[
         "Development Status :: 3 - Alpha",
@@ -70,8 +70,8 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3 :: Only",
     ],
-)
+)
```

