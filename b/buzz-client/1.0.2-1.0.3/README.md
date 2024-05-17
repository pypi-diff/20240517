# Comparing `tmp/buzz_client-1.0.2.tar.gz` & `tmp/buzz_client-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buzz_client-1.0.2.tar", max compression
+gzip compressed data, was "buzz_client-1.0.3.tar", max compression
```

## Comparing `buzz_client-1.0.2.tar` & `buzz_client-1.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2174 2024-05-16 13:37:23.631928 buzz_client-1.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.2/buzz_client/__init__.py
--rwxr-xr-x   0        0        0     3891 2024-05-16 17:03:13.771299 buzz_client-1.0.2/buzz_client/cli.py
--rw-r--r--   0        0        0     2021 2024-05-15 16:36:50.757253 buzz_client-1.0.2/buzz_client/client.py
--rw-r--r--   0        0        0      451 2024-05-16 17:03:43.514357 buzz_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 buzz_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2174 2024-05-16 13:37:23.631928 buzz_client-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.3/buzz_client/__init__.py
+-rwxr-xr-x   0        0        0     4171 2024-05-17 10:38:15.599424 buzz_client-1.0.3/buzz_client/cli.py
+-rw-r--r--   0        0        0     2674 2024-05-17 10:30:15.232087 buzz_client-1.0.3/buzz_client/client.py
+-rw-r--r--   0        0        0      451 2024-05-17 11:01:19.987636 buzz_client-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 buzz_client-1.0.3/PKG-INFO
```

### Comparing `buzz_client-1.0.2/README.md` & `buzz_client-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `buzz_client-1.0.2/buzz_client/cli.py` & `buzz_client-1.0.3/buzz_client/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 Options:
     -h  --help                   show this help message and exit
     -d
     -q
 
     -v --version                 show version and exit
 
-    -s URL --server=URL          API URL
+    -a URL --api=URL             API URL
     -t TOKEN --token=TOKEN       API Auth token
 
     --recipient <recipient>      the recipient of the notification,
                                  must be valid for the notifier chosen
     --title <title>              the title of the notification. [default: You received a buzz]
     --severity <severity>        the severity of the message. [default: info]
                                  One of: 'info', 'success', 'warning', 'failure'
@@ -30,16 +30,16 @@
 
     <notifier>                   the notifier you want to use,
                                  you can see the available notifiers using `list` command
 
     <body>                       Content of the notification,
                                  if not specified read from stdin
 Environment variables:
-    - BC_API         API URL, overrides command line argument
-    - BC_TOKEN       API token, overrides command line argument
+    - BUZZ_API         API URL, overrides command line argument
+    - BUZZ_TOKEN       API token, overrides command line argument
 """
 import sys
 import signal
 from docopt import docopt
 from buzz_client.client import BuzzClient
 from scriptonite.configuration import Configuration
 from scriptonite.logging import Logger
@@ -80,36 +80,43 @@
         print(">> arguments")
         for k, v in arguments.items():
             print(f"{k:15}: {str(v):20}")
         print("")
 
     client_configuration = Configuration()
     client_configuration.from_mapping(
-        dict(api=arguments.get('--server'), token=arguments.get('--token')))
-    client_configuration.from_environ(prefix="BC")
+        dict(api=arguments.get('--api'), token=arguments.get('--token')))
+    client_configuration.from_environ(prefix="BUZZ")
 
     client = BuzzClient(client_configuration)
 
     if client.api is None or client.settings.token is None:
-        message = "Missing values for Server URL or TOKEN"
-        print()
-        print(f"** {message}")
-        print()
-        exit(2)
+        print(f"\n** Missing values for API URL or TOKEN")
+        sys.exit(2)
+
+    # Check connection
+    check = client.check()
+    if not check.get('api_ok'):
+        print(f"\nERROR: connection to '{client.api}' failed.\n")
+        sys.exit(2)
+    if not check.get('token_ok'):
+        print(f"\nERROR: authentication failed while connecting to '{
+              client.api}'\n")
+        sys.exit(3)
 
     if arguments.version:
         banner(client)
-        exit(0)
+        sys.exit(0)
 
     if arguments.list:
         print("Available notifiers")
         print("-" * len("Available notifiers"))
         for notifier in client.notifiers:
             print(notifier)
-        exit(0)
+        sys.exit(0)
 
     if arguments.send:
         if arguments.get('<body>'):
             body = [" ".join(arguments.get('<body>'))]  # type: ignore
         else:
             body = []
             for line in sys.stdin:
@@ -122,12 +129,12 @@
             body="\n".join(body),
             severity=arguments.get('--severity'),  # type: ignore
             attach=arguments.get('--attach')  # type: ignore
         )
         print(
             f"{r.json().get('detail')} [{r.status_code}]")
 
-        exit(int(not (r)))
+        sys.exit(int(not (r)))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `buzz_client-1.0.2/buzz_client/client.py` & `buzz_client-1.0.3/buzz_client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from email.policy import HTTP
 from functools import cached_property
 import re
+from httpx import HTTPError
 import requests
 import logging
 from scriptonite.configuration import Configuration, yaml_load
 from scriptonite.utilities import dictObj
 from scriptonite.logging import Logger
 
 
@@ -15,36 +17,54 @@
     settings: dictObj
 
     def __init__(self, settings) -> None:
 
         # Load config
         self.settings = settings
         self.api = settings.api
+        self.headers = {'x-auth-token': self.settings.token}
 
     def get(self, endpoint: str):
-        response = requests.get(f"{self.settings.api}{endpoint}",
-                                headers={"x-auth-token":
-                                         self.settings.token})
+        response = requests.get(f"{self.api}{endpoint}",
+                                headers=self.headers)
         return response
 
+    def check(self):
+        try:
+            api_info = self.get('/')
+        except requests.exceptions.ConnectionError:
+            return dict(api_ok=False, token_ok=False)
+        if api_info.ok:
+            api_path = api_info.json().get('api_path')
+            token_check = self.get(f"{api_path}/check")
+
+            if token_check.ok:
+                return dict(api_ok=True, token_ok=True)
+            else:
+                return dict(api_ok=True, token_ok=False)
+
     @cached_property
     def api_info(self) -> dict:
         return self.get('/').json()
 
     @cached_property
     def api_path(self) -> str | None:
         return self.api_info.get('api_path')
 
     @cached_property
     def api_version(self) -> str | None:
         return self.api_info.get('app_version')
 
     @cached_property
     def notifiers(self):
-        return self.get(f'{self.api_path}/notifiers').json().get('notifiers')
+        response = self.get(f'{self.api_path}/notifiers')
+        if response.ok:
+            return self.get(f'{self.api_path}/notifiers').json().get('notifiers')
+        else:
+            return []
 
     def send(self, notifier: str,
              recipient: str,
              body: str = "The body",
              title: str = "You got a buzz",
              severity: str = "info",
              attach: str = ''):
@@ -58,16 +78,17 @@
             log.debug(f"attaching {attach}...")
             files = {'attach': open(attach, 'rb')}
 
         response = requests.post(
             f"{self.settings.api}{self.api_path}/send/{notifier}",
             data=data,
             files=files,
-            headers={"x-auth-token": self.settings.token})
+            headers=self.headers)
 
+        response.raise_for_status()
         return response
 
 
 if __name__ == "__main__":
     c = Configuration()
     c.from_file(filename='settings.yaml', load=yaml_load)  # type: ignore
     c.from_environ(prefix="BC")
```

### Comparing `buzz_client-1.0.2/PKG-INFO` & `buzz_client-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buzz-client
-Version: 1.0.2
+Version: 1.0.3
 Summary: A client for Buzz API
 License: GPL
 Author: Andrea Mistrali
 Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: buzz-client Version: 1.0.2 Summary: A client for
+Metadata-Version: 2.1 Name: buzz-client Version: 1.0.3 Summary: A client for
 Buzz API License: GPL Author: Andrea Mistrali Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: docopt-ng
 (>=0.9.0,<0.10.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
 requests (>=2.31.0,<3.0.0) Requires-Dist: scriptonite (>=1.0.3,<2.0.0)
```

