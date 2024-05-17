# Comparing `tmp/nadeo_api-0.1.0.tar.gz` & `tmp/nadeo_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadeo_api-0.1.0.tar", last modified: Thu May 16 00:26:47 2024, max compression
+gzip compressed data, was "nadeo_api-0.2.0.tar", last modified: Fri May 17 19:20:49 2024, max compression
```

## Comparing `nadeo_api-0.1.0.tar` & `nadeo_api-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.178122 nadeo_api-0.1.0/
--rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3365 2024-05-16 00:26:47.177122 nadeo_api-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1493 2024-05-15 20:11:16.000000 nadeo_api-0.1.0/README.md
--rw-rw-rw-   0        0        0      671 2024-05-16 00:12:55.000000 nadeo_api-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 00:26:47.178122 nadeo_api-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.138748 nadeo_api-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.150898 nadeo_api-0.1.0/src/nadeo_api/
--rw-rw-rw-   0        0        0      240 2024-05-16 00:13:14.000000 nadeo_api-0.1.0/src/nadeo_api/__init__.py
--rw-rw-rw-   0        0        0     9931 2024-05-15 23:21:32.000000 nadeo_api-0.1.0/src/nadeo_api/auth.py
--rw-rw-rw-   0        0        0     2139 2024-05-16 00:07:27.000000 nadeo_api-0.1.0/src/nadeo_api/core.py
--rw-rw-rw-   0        0        0     2941 2024-05-16 00:07:12.000000 nadeo_api-0.1.0/src/nadeo_api/live.py
--rw-rw-rw-   0        0        0        0 2024-05-15 05:36:16.000000 nadeo_api-0.1.0/src/nadeo_api/meet.py
--rw-rw-rw-   0        0        0        0 2024-05-15 05:36:21.000000 nadeo_api-0.1.0/src/nadeo_api/oauth.py
-drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.176123 nadeo_api-0.1.0/src/nadeo_api.egg-info/
--rw-rw-rw-   0        0        0     3365 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-16 00:26:47.000000 nadeo_api-0.1.0/src/nadeo_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-16 00:26:47.175123 nadeo_api-0.1.0/tests/
--rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.1.0/tests/test_auth.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:20:49.029984 nadeo_api-0.2.0/
+-rw-rw-rw-   0        0        0     1064 2024-05-07 17:58:02.000000 nadeo_api-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3506 2024-05-17 19:20:49.029480 nadeo_api-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1633 2024-05-17 18:39:02.000000 nadeo_api-0.2.0/README.md
+-rw-rw-rw-   0        0        0      671 2024-05-17 19:16:41.000000 nadeo_api-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 19:20:49.029984 nadeo_api-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 19:20:48.987919 nadeo_api-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 19:20:49.007008 nadeo_api-0.2.0/src/nadeo_api/
+-rw-rw-rw-   0        0        0      240 2024-05-17 19:16:46.000000 nadeo_api-0.2.0/src/nadeo_api/__init__.py
+-rw-rw-rw-   0        0        0    10109 2024-05-16 23:12:13.000000 nadeo_api-0.2.0/src/nadeo_api/auth.py
+-rw-rw-rw-   0        0        0     2046 2024-05-16 23:18:12.000000 nadeo_api-0.2.0/src/nadeo_api/core.py
+-rw-rw-rw-   0        0        0     2848 2024-05-16 23:18:18.000000 nadeo_api-0.2.0/src/nadeo_api/live.py
+-rw-rw-rw-   0        0        0     1627 2024-05-16 23:18:23.000000 nadeo_api-0.2.0/src/nadeo_api/meet.py
+-rw-rw-rw-   0        0        0     2881 2024-05-17 19:15:57.000000 nadeo_api-0.2.0/src/nadeo_api/oauth.py
+drwxrwxrwx   0        0        0        0 2024-05-17 19:20:49.028975 nadeo_api-0.2.0/src/nadeo_api.egg-info/
+-rw-rw-rw-   0        0        0     3506 2024-05-17 19:20:48.000000 nadeo_api-0.2.0/src/nadeo_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-17 19:20:48.000000 nadeo_api-0.2.0/src/nadeo_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 19:20:48.000000 nadeo_api-0.2.0/src/nadeo_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-17 19:20:48.000000 nadeo_api-0.2.0/src/nadeo_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 19:20:48.000000 nadeo_api-0.2.0/src/nadeo_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 19:20:49.028048 nadeo_api-0.2.0/tests/
+-rw-rw-rw-   0        0        0      257 2024-05-12 19:21:20.000000 nadeo_api-0.2.0/tests/test_auth.py
```

### Comparing `nadeo_api-0.1.0/LICENSE.txt` & `nadeo_api-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nadeo_api-0.1.0/PKG-INFO` & `nadeo_api-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,15 +44,16 @@
 
 A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
 
 The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
 The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
 Most of these endpoints are not documented at all, but you may help supplement the documentation [here](https://github.com/openplanet-nl/nadeoapi-docs).
 
-The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).
+The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).\
+There is also community-driven documentation [here](https://webservices.openplanet.dev/oauth/reference) which should be a bit more useful.
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
```

### Comparing `nadeo_api-0.1.0/README.md` & `nadeo_api-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
 
 The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
 The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
 Most of these endpoints are not documented at all, but you may help supplement the documentation [here](https://github.com/openplanet-nl/nadeoapi-docs).
 
-The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).
+The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).\
+There is also community-driven documentation [here](https://webservices.openplanet.dev/oauth/reference) which should be a bit more useful.
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
```

### Comparing `nadeo_api-0.1.0/pyproject.toml` & `nadeo_api-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nadeo-api"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Ezio416", email="e@e416.dev" },
 ]
 description = "Access Nadeo's web services API and the public Trackmania API"
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.12"
```

### Comparing `nadeo_api-0.1.0/src/nadeo_api/auth.py` & `nadeo_api-0.2.0/src/nadeo_api/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-07
-| Modified: 2024-05-15
+| Modified: 2024-05-16
 
 - Functions for interacting with authentication tokens to use with the API
 - Also contains variables and functions intended for internal use
 '''
 
 from base64 import b64encode, urlsafe_b64decode
 from dataclasses import dataclass
@@ -194,37 +194,39 @@
 
     if req.status_code >= 400:
         raise ConnectionError(f'Bad response from {base_name} API: code {req.status_code}, response {req.text}')
 
     return req.json()
 
 
-def get_token(audience: str, agent: str, username: str, password: str, server_account: bool = False) -> Token:
+def get_token(audience: str, username: str, password: str, agent: str = '', server_account: bool = False) -> Token:
     '''
     - requests an authentication token for a given audience
 
     Parameters
     ----------
     audience: str
         - desired audience for token use
         - capitalization is ignored
         - valid: `NadeoServices`/`core`/`prod`, `NadeoLiveServices`/`live`/`meet`/`club`, `OAuth`/`OAuth2`
 
-    agent: str
-        - user agent with your program's name and a way to contact you
-        - Ubisoft can block your request without this being properly set
-
     username: str
         - Ubisoft/dedicated server account username
         - for OAuth2, this is the identifier
 
     password: str
         - Ubisoft/dedicated server account password
         - for OAuth2, this is the secret
 
+    agent: str
+        - user agent with your program's name and a way to contact you
+        - Ubisoft can block your request without this being properly set
+        - not required for OAuth2
+        - default: `''` (empty)
+
     server_account: bool
         - whether you're using a dedicated server account instead of a Ubisoft account
         - ignored when using OAuth2
         - default: `False`
     '''
 
     aud_lower: str = audience.lower()
@@ -251,14 +253,17 @@
 
         if req.status_code >= 400:
             raise ConnectionError(f'Bad response getting token for {audience}: code {req.status_code}, response {req.text}')
 
         json: dict = req.json()
         return Token(json['access_token'], audience, expiration=int(time.time()) + json['expires_in'])
 
+    if agent == '':
+        raise ValueError('For web services endpoints, you must specify a user agent')
+
     req: requests.Response = requests.post(
         f'{url_core}/v2/authentication/token/basic' if server_account else 'https://public-ubiservices.ubi.com/v3/profiles/sessions',
         headers={
             'Authorization': f'Basic {b64encode(f'{username}:{password}'.encode('utf-8')).decode('ascii')}',
             'Content-Type':  'application/json',
             'Ubi-AppId':     tmnext_app_id,
             'User-Agent':    agent,
```

### Comparing `nadeo_api-0.1.0/src/nadeo_api/core.py` & `nadeo_api-0.2.0/src/nadeo_api/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-14
-| Modified: 2024-05-15
+| Modified: 2024-05-16
 
 - Functions for interacting with the web services Core API
 '''
 
 import auth
 
 
@@ -19,15 +19,14 @@
         - authentication token gotten from `auth.get_token`
 
     endpoint: str
         - desired endpoint
         - base URL is optional
         - leading forward slash is optional
         - trailing parameters are optional, i.e. `?param1=true&param2=0`
-        - it is your responsibility to ensure there are no invalid characters such as commas
 
     params: dict
         - parameters for request if applicable
         - if you specified parameters at the end of the `endpoint`, do not specify them here else they will be duplicated
 
     Returns
     -------
```

### Comparing `nadeo_api-0.1.0/src/nadeo_api/live.py` & `nadeo_api-0.2.0/src/nadeo_api/live.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 | Author:   Ezio416
 | Created:  2024-05-15
-| Modified: 2024-05-15
+| Modified: 2024-05-16
 
 - Functions for interacting with the web services Live API
 '''
 
 import auth
 
 
@@ -19,15 +19,14 @@
         - authentication token gotten from `auth.get_token`
 
     endpoint: str
         - desired endpoint
         - base URL is optional
         - leading forward slash is optional
         - trailing parameters are optional, i.e. `?param1=true&param2=0`
-        - it is your responsibility to ensure there are no invalid characters such as commas
 
     params: dict
         - parameters for request if applicable
         - if you specified parameters at the end of the `endpoint`, do not specify them here else they will be duplicated
 
     Returns
     -------
```

### Comparing `nadeo_api-0.1.0/src/nadeo_api.egg-info/PKG-INFO` & `nadeo_api-0.2.0/src/nadeo_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadeo-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: Access Nadeo's web services API and the public Trackmania API
 Author-email: Ezio416 <e@e416.dev>
 License: MIT License
         
         Copyright (c) 2024 Ezio416
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -44,15 +44,16 @@
 
 A library to assist with accessing Nadeo's web services API and the public Trackmania API (OAuth2).
 
 The web services API has community-driven documentation [here](https://webservices.openplanet.dev/).\
 The main section of this API (named "Core") has an up-to-date list of valid endpoints being kept [here](https://github.com/openplanet-nl/core-api-tracking).\
 Most of these endpoints are not documented at all, but you may help supplement the documentation [here](https://github.com/openplanet-nl/nadeoapi-docs).
 
-The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).
+The public Trackmania API has official documentation [here](https://api.trackmania.com/doc).\
+There is also community-driven documentation [here](https://webservices.openplanet.dev/oauth/reference) which should be a bit more useful.
 
 Installing the package from PyPI:
 ```
 python -m pip install nadeo-api
 ```
 
 Using the package:
```

