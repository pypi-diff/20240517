# Comparing `tmp/hikconnect-1.1.0.tar.gz` & `tmp/hikconnect-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikconnect-1.1.0.tar", max compression
+gzip compressed data, was "hikconnect-1.2.0.tar", max compression
```

## Comparing `hikconnect-1.1.0.tar` & `hikconnect-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2093 2023-08-25 18:54:43.224565 hikconnect-1.1.0/README.md
--rw-r--r--   0        0        0      185 2021-09-16 21:47:39.000000 hikconnect-1.1.0/hikconnect/__init__.py
--rw-r--r--   0        0        0    11438 2023-08-25 18:47:34.464397 hikconnect-1.1.0/hikconnect/api.py
--rw-r--r--   0        0        0      150 2022-07-27 21:43:49.000000 hikconnect-1.1.0/hikconnect/exceptions.py
--rw-r--r--   0        0        0     1400 2023-08-25 18:56:11.740639 hikconnect-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3170 1970-01-01 00:00:00.000000 hikconnect-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2093 2023-08-25 18:54:43.224565 hikconnect-1.2.0/README.md
+-rw-r--r--   0        0        0       73 2023-08-30 22:30:49.093845 hikconnect-1.2.0/hikconnect/__init__.py
+-rw-r--r--   0        0        0    12510 2023-10-12 06:17:49.894336 hikconnect-1.2.0/hikconnect/api.py
+-rw-r--r--   0        0        0      150 2022-07-27 21:43:49.000000 hikconnect-1.2.0/hikconnect/exceptions.py
+-rw-r--r--   0        0        0     1455 2023-10-12 06:18:02.007109 hikconnect-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3170 1970-01-01 00:00:00.000000 hikconnect-1.2.0/PKG-INFO
```

### Comparing `hikconnect-1.1.0/README.md` & `hikconnect-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hikconnect-1.1.0/hikconnect/api.py` & `hikconnect-1.2.0/hikconnect/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -91,19 +91,19 @@
             new_api_domain = res_json["loginArea"]["apiDomain"]
             self.BASE_URL = f"https://{new_api_domain}"
             log.debug("Switching API domain to '%s'", self.BASE_URL)
             return await self.login(username, password)
 
         try:
             session_id = res_json["loginSession"]["sessionId"]
-        except KeyError as e:
+        except KeyError as e:  # pragma: no cover
             raise LoginError("Unable to parse session_id from response.") from e
         try:
             refresh_session_id = res_json["loginSession"]["rfSessionId"]
-        except KeyError as e:
+        except KeyError as e:  # pragma: no cover
             raise LoginError("Unable to parse refresh_session_id from response.") from e
 
         self._handle_login_response(session_id, refresh_session_id)
 
         log.info("Login successful as username '%s'", username)
 
     async def refresh_login(self):
@@ -117,19 +117,19 @@
                 f"{self.BASE_URL}/v3/apigateway/login", data=data
             ) as res:
                 res_json = await res.json()
         log.debug("Got refresh login response '%s'", res_json)
 
         try:
             session_id = res_json["sessionInfo"]["sessionId"]
-        except KeyError as e:
+        except KeyError as e:  # pragma: no cover
             raise LoginError("Unable to parse session_id from response.") from e
         try:
             refresh_session_id = res_json["sessionInfo"]["refreshSessionId"]
-        except KeyError as e:
+        except KeyError as e:  # pragma: no cover
             raise LoginError("Unable to parse refresh_session_id from response.") from e
 
         self._handle_login_response(session_id, refresh_session_id)
 
         log.info("Login refreshed successfuly")
 
     def _handle_login_response(self, session_id, refresh_session_id):
@@ -248,29 +248,52 @@
                 log.debug("Missing caller info key: %s", in_key)
 
         return {
             "status": status,
             "info": info,
         }
 
+    async def answer_call(self, device_serial: str):
+        """
+        Send answer call request.
+
+        The `device_serial` parameter can be obtained from `get_devices()` and/or `get_cameras()`.
+        """
+        async with self.client.put(
+            f"{self.BASE_URL}/v3/devconfig/v1/call/{device_serial}/operation?cmdId=2"
+        ) as res:
+            res_json = await res.json()
+        log.debug("Got answer_call response '%s'", res_json)
+        log.info("Answer call to device '%s'", device_serial)
+
     async def cancel_call(self, device_serial: str):
         """
         Send cancel call request.
 
         The `device_serial` parameter can be obtained from `get_devices()` and/or `get_cameras()`.
         """
         async with self.client.put(
-                f"{self.BASE_URL}/v3/devconfig/v1/call/{device_serial}/operation?cmdId=3"
+            f"{self.BASE_URL}/v3/devconfig/v1/call/{device_serial}/operation?cmdId=3"
         ) as res:
             res_json = await res.json()
         log.debug("Got cancel_call response '%s'", res_json)
-        log.info(
-            "Cancel call to device '%s'",
-            device_serial
-        )
+        log.info("Cancel call to device '%s'", device_serial)
+
+    async def hangup_call(self, device_serial: str):
+        """
+        Send hangup call request.
+
+        The `device_serial` parameter can be obtained from `get_devices()` and/or `get_cameras()`.
+        """
+        async with self.client.put(
+            f"{self.BASE_URL}/v3/devconfig/v1/call/{device_serial}/operation?cmdId=5"
+        ) as res:
+            res_json = await res.json()
+        log.debug("Got hangup_call response '%s'", res_json)
+        log.info("Hangup call to device '%s'", device_serial)
 
     @staticmethod
     def _decode_jwt_expiration(jwt):
         # decode JWT manually because of PyJWT version incompatibility with HomeAssistant
         parts = jwt.split(".")
         claims_raw = parts[1]
         missing_padding = len(claims_raw) % 4
```

### Comparing `hikconnect-1.1.0/pyproject.toml` & `hikconnect-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "hikconnect"
-version = "1.1.0"
+version = "1.2.0"
 description = "Communicate with Hikvision smart doorbells via Hik-Connect cloud."
 
 license = "MIT"
 
 authors = ["Tomas Bedrich <ja@tbedrich.cz>"]
 
 readme = "README.md"
@@ -26,47 +26,47 @@
     "Topic :: System :: Hardware",
     "Topic :: Home Automation",
 ]
 
 [tool.poetry.dependencies]
 
 python = "^3.8"
-aiohttp = "^3.7.4"
-
+aiohttp = "^3.8.5"
 
 [tool.poetry.dev-dependencies]
 
-python-dotenv = "^0.19.0"
+python-dotenv = "^1.0.0"
 
 # Formatters
-black = "=20.8b1"
-isort = "^5.6.3"
+black = "^23.7.0"
+isort = "^5.12.0"
 
 # Linters
-mypy = "*"
-pydocstyle = "*"
-pylint = "^2.6.0"
+mypy = "^1.5.1"
+pydocstyle = "^6.3.0"
+pylint = "^2.17.5"
 
 # Testing
-pytest = "^6.1.1"
-pytest-cov = "*"
-pytest-describe = "^2.0.0"
-pytest-expecter = "^2.1"
-pytest-random = "*"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+pytest-describe = "^2.1.0"
+pytest-expecter = "^3.0"
+pytest-random = "^0.02"
 pytest-asyncio = "^0.14.0"
 pytest-dotenv = "^0.5.2"
+aioresponses = "^0.7.4"
 
 # Reports
-coveragespace = "^3.1.1"
+coveragespace = "^6.0.2"
 
 # Documentation
-mkdocs = "^1.1.2"
-mkdocs-material = "*"
-mkdocstrings = "*"
-pygments = "^2.5.2"
+mkdocs = "^1.5.2"
+mkdocs-material = "^9.2.5"
+mkdocstrings = "^0.22.0"
+pygments = "^2.16.1"
 
 [tool.black]
 
 target-version = ["py36", "py37", "py38"]
 
 [build-system]
```

### Comparing `hikconnect-1.1.0/PKG-INFO` & `hikconnect-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikconnect
-Version: 1.1.0
+Version: 1.2.0
 Summary: Communicate with Hikvision smart doorbells via Hik-Connect cloud.
 Home-page: https://pypi.org/project/hikconnect
 License: MIT
 Author: Tomas Bedrich
 Author-email: ja@tbedrich.cz
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Home Automation
 Classifier: Topic :: System :: Hardware
 Classifier: Topic :: System :: Networking
-Requires-Dist: aiohttp (>=3.7.4,<4.0.0)
+Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Project-URL: Documentation, https://hikconnect.readthedocs.io
 Project-URL: Repository, https://github.com/tomasbedrich/hikconnect
 Description-Content-Type: text/markdown
 
 # Usage
 
 ```python
```

