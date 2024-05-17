# Comparing `tmp/mauth_client-1.6.4.tar.gz` & `tmp/mauth_client-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mauth_client-1.6.4.tar", max compression
+gzip compressed data, was "mauth_client-1.6.5.tar", max compression
```

## Comparing `mauth_client-1.6.4.tar` & `mauth_client-1.6.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1062 2024-02-08 22:40:52.067518 mauth_client-1.6.4/LICENSE.txt
--rw-r--r--   0        0        0     6084 2024-02-08 22:40:52.067518 mauth_client-1.6.4/README.md
--rw-r--r--   0        0        0      146 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/__init__.py
--rw-r--r--   0        0        0     9672 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/authenticator.py
--rw-r--r--   0        0        0      434 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/config.py
--rw-r--r--   0        0        0      479 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/consts.py
--rw-r--r--   0        0        0      633 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/exceptions.py
--rw-r--r--   0        0        0     2046 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/key_holder.py
--rw-r--r--   0        0        0       54 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/lambda_authenticator/__init__.py
--rw-r--r--   0        0        0      761 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/lambda_authenticator/lambda_authenticator.py
--rw-r--r--   0        0        0      700 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/lambda_helper.py
--rw-r--r--   0        0        0       76 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/middlewares/__init__.py
--rw-r--r--   0        0        0     4147 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/middlewares/asgi.py
--rw-r--r--   0        0        0     4978 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/middlewares/wsgi.py
--rw-r--r--   0        0        0       26 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/requests_mauth/__init__.py
--rw-r--r--   0        0        0     1304 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/requests_mauth/client.py
--rw-r--r--   0        0        0     2795 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/rsa_signer.py
--rw-r--r--   0        0        0     2324 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/rsa_verifier.py
--rw-r--r--   0        0        0     6196 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/signable.py
--rw-r--r--   0        0        0     1731 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/signed.py
--rw-r--r--   0        0        0     2849 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/signer.py
--rw-r--r--   0        0        0      820 2024-02-08 22:40:52.071518 mauth_client-1.6.4/mauth_client/utils.py
--rw-r--r--   0        0        0     1381 2024-02-08 22:40:52.071518 mauth_client-1.6.4/pyproject.toml
--rw-r--r--   0        0        0     7329 1970-01-01 00:00:00.000000 mauth_client-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-17 01:47:02.368022 mauth_client-1.6.5/LICENSE.txt
+-rw-r--r--   0        0        0     5922 2024-05-17 01:47:02.368022 mauth_client-1.6.5/README.md
+-rw-r--r--   0        0        0      146 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/__init__.py
+-rw-r--r--   0        0        0     9672 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/authenticator.py
+-rw-r--r--   0        0        0      434 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/config.py
+-rw-r--r--   0        0        0      479 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/consts.py
+-rw-r--r--   0        0        0      633 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/exceptions.py
+-rw-r--r--   0        0        0     2046 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/key_holder.py
+-rw-r--r--   0        0        0       54 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/lambda_authenticator/__init__.py
+-rw-r--r--   0        0        0      761 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/lambda_authenticator/lambda_authenticator.py
+-rw-r--r--   0        0        0      700 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/lambda_helper.py
+-rw-r--r--   0        0        0       76 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/middlewares/__init__.py
+-rw-r--r--   0        0        0     4147 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/middlewares/asgi.py
+-rw-r--r--   0        0        0     4978 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/middlewares/wsgi.py
+-rw-r--r--   0        0        0       26 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/requests_mauth/__init__.py
+-rw-r--r--   0        0        0     1304 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/requests_mauth/client.py
+-rw-r--r--   0        0        0     2795 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/rsa_signer.py
+-rw-r--r--   0        0        0     2324 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/rsa_verifier.py
+-rw-r--r--   0        0        0     6196 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/signable.py
+-rw-r--r--   0        0        0     1731 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/signed.py
+-rw-r--r--   0        0        0     2849 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/signer.py
+-rw-r--r--   0        0        0      820 2024-05-17 01:47:02.368022 mauth_client-1.6.5/mauth_client/utils.py
+-rw-r--r--   0        0        0     1418 2024-05-17 01:47:02.372022 mauth_client-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0     7175 1970-01-01 00:00:00.000000 mauth_client-1.6.5/PKG-INFO
```

### Comparing `mauth_client-1.6.4/LICENSE.txt` & `mauth_client-1.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/README.md` & `mauth_client-1.6.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # MAuth Client Python
-[![Build
-Status](https://travis-ci.com/mdsol/mauth-client-python.svg?token=YCqgqZjJBpwz6GCprYaV&branch=develop)](https://travis-ci.com/mdsol/mauth-client-python)
 
 MAuth Client Python is an authentication library to manage the information needed to both sign and authenticate requests and responses for Medidata's MAuth authentication system.
 
 
 ## Pre-requisites
 
 To use MAuth Authenticator you will need:
```

### Comparing `mauth_client-1.6.4/mauth_client/authenticator.py` & `mauth_client-1.6.5/mauth_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/exceptions.py` & `mauth_client-1.6.5/mauth_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/key_holder.py` & `mauth_client-1.6.5/mauth_client/key_holder.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/lambda_authenticator/lambda_authenticator.py` & `mauth_client-1.6.5/mauth_client/lambda_authenticator/lambda_authenticator.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/lambda_helper.py` & `mauth_client-1.6.5/mauth_client/lambda_helper.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/middlewares/asgi.py` & `mauth_client-1.6.5/mauth_client/middlewares/asgi.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/middlewares/wsgi.py` & `mauth_client-1.6.5/mauth_client/middlewares/wsgi.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/requests_mauth/client.py` & `mauth_client-1.6.5/mauth_client/requests_mauth/client.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/rsa_signer.py` & `mauth_client-1.6.5/mauth_client/rsa_signer.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/rsa_verifier.py` & `mauth_client-1.6.5/mauth_client/rsa_verifier.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/signable.py` & `mauth_client-1.6.5/mauth_client/signable.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/signed.py` & `mauth_client-1.6.5/mauth_client/signed.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/signer.py` & `mauth_client-1.6.5/mauth_client/signer.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/mauth_client/utils.py` & `mauth_client-1.6.5/mauth_client/utils.py`

 * *Files identical despite different names*

### Comparing `mauth_client-1.6.4/pyproject.toml` & `mauth_client-1.6.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mauth-client"
-version = "1.6.4"
+version = "1.6.5"
 description = "MAuth Client for Python"
 repository = "https://github.com/mdsol/mauth-client-python"
 authors = ["Medidata Solutions <support@mdsol.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -20,32 +20,32 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "^2.23"
-cachetools = "^5.3"
-rsa = "^4.0"
-asgiref = "^3.5.2"
-charset-normalizer = "^3.1.0"
+requests = "^2.31.0"
+cachetools = "^5.3.3"
+rsa = "^4.9"
+asgiref = "^3.8.1"
+charset-normalizer = "^3.3.2"
 
 [tool.poetry.dev-dependencies]
-boto3 = "^1.24"
-flask = "^2"
-python-dateutil = "^2.8"
-requests-mock = "^1.7"
-pytest = "^7"
-pytest-cov = "^4"
+boto3 = "^1.34.106"
+flask = "^2.3.3"
+python-dateutil = "^2.9.0.post0"
+requests-mock = "^1.12.1"
+pytest = "^7.4.4"
+pytest-cov = "^4.1.0"
 pytest-freezer = "^0.4"
-pytest-randomly = "^3.11"
+pytest-randomly = "^3.15.0"
 pytest-subtests = "^0.10"
-flake8 = "^3.7"
-tox = "^3.28"
+flake8 = "^3.9.2"
+tox = "^4.15.0"
 fastapi = "^0.109.0"
 httpx = "^0.26.0"
 
 [tool.black]
 line-length = 120
 
 [build-system]
```

### Comparing `mauth_client-1.6.4/PKG-INFO` & `mauth_client-1.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mauth-client
-Version: 1.6.4
+Version: 1.6.5
 Summary: MAuth Client for Python
 Home-page: https://github.com/mdsol/mauth-client-python
 License: MIT
 Author: Medidata Solutions
 Author-email: support@mdsol.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -17,25 +17,23 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: asgiref (>=3.5.2,<4.0.0)
-Requires-Dist: cachetools (>=5.3,<6.0)
-Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
-Requires-Dist: requests (>=2.23,<3.0)
-Requires-Dist: rsa (>=4.0,<5.0)
+Requires-Dist: asgiref (>=3.8.1,<4.0.0)
+Requires-Dist: cachetools (>=5.3.3,<6.0.0)
+Requires-Dist: charset-normalizer (>=3.3.2,<4.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rsa (>=4.9,<5.0)
 Project-URL: Repository, https://github.com/mdsol/mauth-client-python
 Description-Content-Type: text/markdown
 
 # MAuth Client Python
-[![Build
-Status](https://travis-ci.com/mdsol/mauth-client-python.svg?token=YCqgqZjJBpwz6GCprYaV&branch=develop)](https://travis-ci.com/mdsol/mauth-client-python)
 
 MAuth Client Python is an authentication library to manage the information needed to both sign and authenticate requests and responses for Medidata's MAuth authentication system.
 
 
 ## Pre-requisites
 
 To use MAuth Authenticator you will need:
```

