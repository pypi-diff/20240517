# Comparing `tmp/vipas-0.1.1.tar.gz` & `tmp/vipas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vipas-0.1.1.tar", last modified: Thu May 16 12:26:38 2024, max compression
+gzip compressed data, was "vipas-0.1.2.tar", last modified: Thu May 16 15:23:42 2024, max compression
```

## Comparing `vipas-0.1.1.tar` & `vipas-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.408251 vipas-0.1.1/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.1/LICENSE.md
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-16 12:26:38.408251 vipas-0.1.1/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.1/README.md
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.1/pyproject.toml
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-16 12:26:38.412251 vipas-0.1.1/setup.cfg
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-16 10:24:06.000000 vipas-0.1.1/setup.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.400251 vipas-0.1.1/test/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.1/test/test_model_client.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.404251 vipas-0.1.1/vipas/
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.1/vipas/__init__.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.1.1/vipas/_rest.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.1/vipas/config.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     3555 2024-05-01 08:36:27.000000 vipas-0.1.1/vipas/exceptions.py
--rw-rw-r--   0 aditya    (1001) aditya    (1001)     6864 2024-05-16 12:24:58.000000 vipas-0.1.1/vipas/model.py
-drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 12:26:38.408251 vipas-0.1.1/vipas.egg-info/
--rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/PKG-INFO
--rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/SOURCES.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/dependency_links.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/requires.txt
--rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-16 12:26:38.000000 vipas-0.1.1/vipas.egg-info/top_level.txt
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 15:23:42.512345 vipas-0.1.2/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2487 2024-04-30 05:46:43.000000 vipas-0.1.2/LICENSE.md
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-16 15:23:42.512345 vipas-0.1.2/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1598 2024-05-01 12:56:58.000000 vipas-0.1.2/README.md
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       91 2024-05-14 08:16:21.000000 vipas-0.1.2/pyproject.toml
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      443 2024-05-16 15:23:42.512345 vipas-0.1.2/setup.cfg
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     1273 2024-05-16 15:16:44.000000 vipas-0.1.2/setup.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 15:23:42.508345 vipas-0.1.2/test/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2818 2024-05-14 08:16:21.000000 vipas-0.1.2/test/test_model_client.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 15:23:42.512345 vipas-0.1.2/vipas/
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      725 2024-04-30 15:42:34.000000 vipas-0.1.2/vipas/__init__.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     2084 2024-05-02 09:27:49.000000 vipas-0.1.2/vipas/_rest.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     4145 2024-05-15 18:08:55.000000 vipas-0.1.2/vipas/config.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     3809 2024-05-16 15:16:24.000000 vipas-0.1.2/vipas/exceptions.py
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)     6864 2024-05-16 12:24:58.000000 vipas-0.1.2/vipas/model.py
+drwxrwxr-x   0 aditya    (1001) aditya    (1001)        0 2024-05-16 15:23:42.512345 vipas-0.1.2/vipas.egg-info/
+-rw-r--r--   0 aditya    (1001) aditya    (1001)      360 2024-05-16 15:23:42.000000 vipas-0.1.2/vipas.egg-info/PKG-INFO
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)      308 2024-05-16 15:23:42.000000 vipas-0.1.2/vipas.egg-info/SOURCES.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        1 2024-05-16 15:23:42.000000 vipas-0.1.2/vipas.egg-info/dependency_links.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)       65 2024-05-16 15:23:42.000000 vipas-0.1.2/vipas.egg-info/requires.txt
+-rw-rw-r--   0 aditya    (1001) aditya    (1001)        6 2024-05-16 15:23:42.000000 vipas-0.1.2/vipas.egg-info/top_level.txt
```

### Comparing `vipas-0.1.1/LICENSE.md` & `vipas-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.1/README.md` & `vipas-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vipas-0.1.1/setup.py` & `vipas-0.1.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "vipas"
-VERSION = "0.1.1"
+VERSION = "0.1.2"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3",
     "pydantic",
     "typing-extensions",
     "ratelimit",
     "pybreaker",
```

### Comparing `vipas-0.1.1/test/test_model_client.py` & `vipas-0.1.2/test/test_model_client.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.1/vipas/__init__.py` & `vipas-0.1.2/vipas/__init__.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.1/vipas/_rest.py` & `vipas-0.1.2/vipas/_rest.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.1/vipas/config.py` & `vipas-0.1.2/vipas/config.py`

 * *Files identical despite different names*

### Comparing `vipas-0.1.1/vipas/exceptions.py` & `vipas-0.1.2/vipas/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,14 +67,17 @@
             raise UnauthorizedException(status=http_resp.status_code, reason=http_resp.reason, http_resp=http_resp, body=body, data=data)
 
         if http_resp.status_code == 403:
             raise ForbiddenException(status=http_resp.status_code, reason=http_resp.reason, http_resp=http_resp, body=body, data=data)
 
         if http_resp.status_code == 404:
             raise NotFoundException(status=http_resp.status_code, reason=http_resp.reason, http_resp=http_resp, body=body, data=data)
+        
+        if http_resp.status_code == 429:
+            raise RateLimitExceededException(status=http_resp.status_code, reason=http_resp.reason, http_resp=http_resp, body=body, data=data)
 
         if 500 <= http_resp.status_code <= 599:
             raise ConnectionException(status=http_resp.status_code, reason=http_resp.reason, http_resp=http_resp, body=body, data=data)
         raise ClientException(status=http_resp.status_code, reason=http_resp.reason, http_resp=http_resp, body=body, data=data)
 
     def __str__(self):
         """Custom error messages for exception"""
@@ -104,7 +107,10 @@
 
 class ForbiddenException(ClientException):
     pass
 
 
 class ConnectionException(ClientException):
     pass
+
+class RateLimitExceededException(ClientException):
+    pass
```

### Comparing `vipas-0.1.1/vipas/model.py` & `vipas-0.1.2/vipas/model.py`

 * *Files identical despite different names*

