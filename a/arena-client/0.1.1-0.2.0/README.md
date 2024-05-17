# Comparing `tmp/arena_client-0.1.1.tar.gz` & `tmp/arena_client-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arena_client-0.1.1.tar", max compression
+gzip compressed data, was "arena_client-0.2.0.tar", max compression
```

## Comparing `arena_client-0.1.1.tar` & `arena_client-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      570 2024-05-07 10:32:25.378587 arena_client-0.1.1/README.md
--rw-r--r--   0        0        0     1330 2024-05-07 10:32:25.378587 arena_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      154 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/__init__.py
--rw-r--r--   0        0        0    11685 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/client.py
--rw-r--r--   0        0        0     1018 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/models/__init__.py
--rw-r--r--   0        0        0     3988 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/models/anthropic.py
--rw-r--r--   0        0        0     4364 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/models/chat_completion.py
--rw-r--r--   0        0        0      281 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/models/evaluation.py
--rw-r--r--   0        0        0     2393 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/models/mistral.py
--rw-r--r--   0        0        0     1882 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/models/openai.py
--rw-r--r--   0        0        0      204 2024-05-07 10:32:25.378587 arena_client-0.1.1/src/arena/models/settings.py
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 arena_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      570 2024-05-17 11:59:03.499076 arena_client-0.2.0/README.md
+-rw-r--r--   0        0        0     1330 2024-05-17 11:59:03.499076 arena_client-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      154 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/__init__.py
+-rw-r--r--   0        0        0    12669 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/client.py
+-rw-r--r--   0        0        0     1018 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/__init__.py
+-rw-r--r--   0        0        0     3988 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/anthropic.py
+-rw-r--r--   0        0        0     4364 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/chat_completion.py
+-rw-r--r--   0        0        0      281 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/evaluation.py
+-rw-r--r--   0        0        0     2393 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/mistral.py
+-rw-r--r--   0        0        0     1882 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/openai.py
+-rw-r--r--   0        0        0      204 2024-05-17 11:59:03.499076 arena_client-0.2.0/src/arena/models/settings.py
+-rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 arena_client-0.2.0/PKG-INFO
```

### Comparing `arena_client-0.1.1/README.md` & `arena_client-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `arena_client-0.1.1/pyproject.toml` & `arena_client-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arena-client"
-version = "0.1.1"
+version = "0.2.0"
 description = "A client to use arena AI"
 authors = ["Nicolas Grislain <ng@sarus.tech>"]
 license = "Apache-2"
 readme = "README.md"
 packages = [{from = "src", include = "arena"}]
 
 [tool.poetry.dependencies]
```

### Comparing `arena_client-0.1.1/src/arena/client.py` & `arena_client-0.2.0/src/arena/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,46 +8,75 @@
 import openai
 import mistralai
 import anthropic
 
 BASE_URL = "https://arena.sarus.app/api/v1"
 
 class Client:
-    def __init__(self, user: str | None = None, password: str | None = None, api_key: str | None = None, base_url: str = BASE_URL):
-        self.user = user
+    def __init__(self, username: str | None = None, password: str | None = None, api_key: str | None = None, base_url: str = BASE_URL):
+        self.username = username
         self.password = password
         self.api_key = api_key
         self.base_url = base_url
         self.timeout = 30.0
         if not self.api_key:
             self.login()
     
     
     def login(self):
         """Used internally to get a connection token from a user and a password"""
-        assert(self.user and self.password)
+        assert(self.username and self.password)
         with httpx.Client(timeout=self.timeout) as client:
             resp = client.post(
                 url = f"{self.base_url}/login/access-token",
                 headers =  {
                     "accept": "application/json",
                     "Content-Type": "application/x-www-form-urlencoded",
                 },
                 data = {
                     "grant_type": "",
-                    "username": self.user,
+                    "username": self.username,
                     "password": self.password,
                     "scope": "",
                     "client_id": "",
                     "client_secret": "",
                 },
             )
         self.api_key = resp.json()['access_token']
     
 
+    def user(self, email: str, password: str, full_name: str | None = None):
+        """Create a new user"""
+        with httpx.Client(timeout=self.timeout) as client:
+            client.post(
+                url = f"{self.base_url}/users/open",
+                headers = {
+                    "Authorization": f"Bearer {self.api_key}"
+                },
+                json={
+                    "email": email,
+                    "password": password,
+                    "full_name": full_name
+                },
+            )
+
+    @staticmethod
+    def user_open(email: str, password: str, full_name: str | None = None,  base_url=BASE_URL):
+        """Create a new user"""
+        with httpx.Client() as client:
+            client.post(
+                url = f"{base_url}/users/open",
+                json={
+                    "email": email,
+                    "password": password,
+                    "full_name": full_name
+                },
+            )
+
+
     def openai_api_key(self, api_key: str):
         """Set the OpenAI API token"""
         with httpx.Client(timeout=self.timeout) as client:
             client.post(
                 url = f"{self.base_url}/settings/",
                 headers = {
                     "Authorization": f"Bearer {self.api_key}"
@@ -102,15 +131,15 @@
             client.post(
                 url = f"{self.base_url}/settings/",
                 headers = {
                     "Authorization": f"Bearer {self.api_key}"
                 },
                 json={
                     "name": "LM_CONFIG",
-                    "content": lm_config.model_dump(mode="json")
+                    "content": lm_config.model_dump_json()
                 },
             )
 
 
     def chat_completions(self, **kwargs: Any) -> ChatCompletionResponse:
         """Abstract chat completion"""
         req = ChatCompletionRequest.model_validate(kwargs).model_dump(mode="json", exclude_none=True)
```

### Comparing `arena_client-0.1.1/src/arena/models/__init__.py` & `arena_client-0.2.0/src/arena/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.1.1/src/arena/models/anthropic.py` & `arena_client-0.2.0/src/arena/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.1.1/src/arena/models/chat_completion.py` & `arena_client-0.2.0/src/arena/models/chat_completion.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.1.1/src/arena/models/mistral.py` & `arena_client-0.2.0/src/arena/models/mistral.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.1.1/src/arena/models/openai.py` & `arena_client-0.2.0/src/arena/models/openai.py`

 * *Files identical despite different names*

### Comparing `arena_client-0.1.1/PKG-INFO` & `arena_client-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arena-client
-Version: 0.1.1
+Version: 0.2.0
 Summary: A client to use arena AI
 License: Apache-2
 Author: Nicolas Grislain
 Author-email: ng@sarus.tech
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

