# Comparing `tmp/fastapi_oidc_backend-0.3.0.tar.gz` & `tmp/fastapi_oidc_backend-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_oidc_backend-0.3.0.tar", max compression
+gzip compressed data, was "fastapi_oidc_backend-0.4.0.tar", max compression
```

## Comparing `fastapi_oidc_backend-0.3.0.tar` & `fastapi_oidc_backend-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1106 2024-05-13 13:07:43.056065 fastapi_oidc_backend-0.3.0/LICENSE
--rwxr-xr-x   0        0        0     1466 2024-05-13 13:07:43.056065 fastapi_oidc_backend-0.3.0/README.md
--rwxr-xr-x   0        0        0     1399 2024-05-13 13:07:43.056065 fastapi_oidc_backend-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 13:07:43.056065 fastapi_oidc_backend-0.3.0/src/__init__.py
--rwxr-xr-x   0        0        0     5249 2024-05-13 13:07:43.056065 fastapi_oidc_backend-0.3.0/src/fastapi_resource_server.py
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 fastapi_oidc_backend-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1106 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/LICENSE
+-rwxr-xr-x   0        0        0     1371 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/README.md
+-rwxr-xr-x   0        0        0     1422 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/exceptions.py
+-rw-r--r--   0        0        0     1521 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/models.py
+-rwxr-xr-x   0        0        0     4665 2024-05-17 11:42:33.371825 fastapi_oidc_backend-0.4.0/src/fastapi_oidc_backend/security.py
+-rw-r--r--   0        0        0     2705 1970-01-01 00:00:00.000000 fastapi_oidc_backend-0.4.0/PKG-INFO
```

### Comparing `fastapi_oidc_backend-0.3.0/LICENSE` & `fastapi_oidc_backend-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_oidc_backend-0.3.0/README.md` & `fastapi_oidc_backend-0.4.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -7,42 +7,41 @@
 Fork of fastapi-resource-server
 
 # Usage
 
 Run keycloak on port 8888:
 
 ```sh
-docker container run --name auth-server -d -p 8888:8080 \
+docker container run --name auth-server -d -p 8080:8080 \
     -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin \
     quay.io/keycloak/keycloak:latest
 ```
 
 Install dependencies
 
 ```sh
-pip install fastapi fastapi_resource_server uvicorn
+pip install fastapi fastapi_oidc_backend uvicorn
 ```
 
 Create the main.py module
 
 ```python
 from fastapi import Depends, FastAPI, Security
 from pydantic import BaseModel
 
-from fastapi_resource_server import JwtDecodeOptions, OidcResourceServer
+from fastapi_oidc_backend.security import OidcResourceServer
+from fastapi_oidc_backend.models import JwtKwargs
 
-decode_options = JwtDecodeOptions(require_aud=True, require_issuer=True)
-decode_kwargs = JwtKwargs(audience="my-client", issuer="http://localhost:8888/auth/realms/master")
+oidc_config = JwtKwargs(audience="myclient", issuer="http://localhost:8888/realms/myrealm")
 
-app = FastAPI(swagger_ui_init_oauth={"clientId": decode_kwargs.audience})
+app = FastAPI(swagger_ui_init_oauth={"clientId": oidc_config.audience})
 
 auth_scheme = OidcResourceServer(
-    decode_kwargs.issuer,
+    oidc_config,
     scheme_name="Keycloak",
-    jwt_decode_options=decode_options,
 )
 
 
 class User(BaseModel):
     username: str
     given_name: str
     family_name: str
```

### Comparing `fastapi_oidc_backend-0.3.0/pyproject.toml` & `fastapi_oidc_backend-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "fastapi-oidc-backend"
-version = "0.3.0"
+version = "0.4.0"
 description = "Build resource servers with FastAPI"
-authors = ["Felix Gustavsson <github@0b1.se>"]
+authors = ["Felix Gustavsson <felix@0b1.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/BlackVoid/fastapi-oidc-backend"
 keywords = [ "fastapi", "authentication", "oidc", "openidconnect" ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
@@ -26,21 +26,22 @@
 packages = [
     { include = "*", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11.2"
 fastapi = "^0"
-python-jose = "^3.2"
+python-jose = "^3.3.0"
+httpx = "^0.27.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2"
-pytest-cov = "^2.12.0"
-pytest-mock = "^3.6.1"
-black = "^21.5b1"
-flake8 = "^3.9.2"
-mypy = "^0.812"
-isort = "^5.8.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
+black = "^24.4.2"
+flake8 = "^7.0.0"
+mypy = "^1.10.0"
+isort = "^5.13.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fastapi_oidc_backend-0.3.0/PKG-INFO` & `fastapi_oidc_backend-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi-oidc-backend
-Version: 0.3.0
+Version: 0.4.0
 Summary: Build resource servers with FastAPI
 Home-page: https://github.com/BlackVoid/fastapi-oidc-backend
 License: MIT
 Keywords: fastapi,authentication,oidc,openidconnect
 Author: Felix Gustavsson
-Author-email: github@0b1.se
+Author-email: felix@0b1.se
 Requires-Python: >=3.11.2,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,16 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fastapi (>=0,<1)
-Requires-Dist: python-jose (>=3.2,<4.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Project-URL: Repository, https://github.com/BlackVoid/fastapi-oidc-backend
 Description-Content-Type: text/markdown
 
 # FastAPI Resource Backend
 
 Build an OIDC resource server using FastAPI.
 
@@ -37,42 +38,41 @@
 Fork of fastapi-resource-server
 
 # Usage
 
 Run keycloak on port 8888:
 
 ```sh
-docker container run --name auth-server -d -p 8888:8080 \
+docker container run --name auth-server -d -p 8080:8080 \
     -e KEYCLOAK_USER=admin -e KEYCLOAK_PASSWORD=admin \
     quay.io/keycloak/keycloak:latest
 ```
 
 Install dependencies
 
 ```sh
-pip install fastapi fastapi_resource_server uvicorn
+pip install fastapi fastapi_oidc_backend uvicorn
 ```
 
 Create the main.py module
 
 ```python
 from fastapi import Depends, FastAPI, Security
 from pydantic import BaseModel
 
-from fastapi_resource_server import JwtDecodeOptions, OidcResourceServer
+from fastapi_oidc_backend.security import OidcResourceServer
+from fastapi_oidc_backend.models import JwtKwargs
 
-decode_options = JwtDecodeOptions(require_aud=True, require_issuer=True)
-decode_kwargs = JwtKwargs(audience="my-client", issuer="http://localhost:8888/auth/realms/master")
+oidc_config = JwtKwargs(audience="myclient", issuer="http://localhost:8888/realms/myrealm")
 
-app = FastAPI(swagger_ui_init_oauth={"clientId": decode_kwargs.audience})
+app = FastAPI(swagger_ui_init_oauth={"clientId": oidc_config.audience})
 
 auth_scheme = OidcResourceServer(
-    decode_kwargs.issuer,
+    oidc_config,
     scheme_name="Keycloak",
-    jwt_decode_options=decode_options,
 )
 
 
 class User(BaseModel):
     username: str
     given_name: str
     family_name: str
```

