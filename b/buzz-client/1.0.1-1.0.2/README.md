# Comparing `tmp/buzz_client-1.0.1.tar.gz` & `tmp/buzz_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buzz_client-1.0.1.tar", max compression
+gzip compressed data, was "buzz_client-1.0.2.tar", max compression
```

## Comparing `buzz_client-1.0.1.tar` & `buzz_client-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2174 2024-05-16 13:37:23.631928 buzz_client-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.1/buzz_client/__init__.py
--rwxr-xr-x   0        0        0     3760 2024-05-16 14:11:49.741838 buzz_client-1.0.1/buzz_client/cli.py
--rw-r--r--   0        0        0     2021 2024-05-15 16:36:50.757253 buzz_client-1.0.1/buzz_client/client.py
--rw-r--r--   0        0        0      451 2024-05-16 14:11:43.940420 buzz_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 buzz_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2174 2024-05-16 13:37:23.631928 buzz_client-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 12:39:43.660459 buzz_client-1.0.2/buzz_client/__init__.py
+-rwxr-xr-x   0        0        0     3891 2024-05-16 17:03:13.771299 buzz_client-1.0.2/buzz_client/cli.py
+-rw-r--r--   0        0        0     2021 2024-05-15 16:36:50.757253 buzz_client-1.0.2/buzz_client/client.py
+-rw-r--r--   0        0        0      451 2024-05-16 17:03:43.514357 buzz_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2819 1970-01-01 00:00:00.000000 buzz_client-1.0.2/PKG-INFO
```

### Comparing `buzz_client-1.0.1/README.md` & `buzz_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `buzz_client-1.0.1/buzz_client/cli.py` & `buzz_client-1.0.2/buzz_client/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,21 @@
     client_configuration = Configuration()
     client_configuration.from_mapping(
         dict(api=arguments.get('--server'), token=arguments.get('--token')))
     client_configuration.from_environ(prefix="BC")
 
     client = BuzzClient(client_configuration)
 
+    if client.api is None or client.settings.token is None:
+        message = "Missing values for Server URL or TOKEN"
+        print()
+        print(f"** {message}")
+        print()
+        exit(2)
+
     if arguments.version:
         banner(client)
         exit(0)
 
     if arguments.list:
         print("Available notifiers")
         print("-" * len("Available notifiers"))
@@ -107,19 +114,19 @@
             body = []
             for line in sys.stdin:
                 body.append(line.rstrip())
 
         r = client.send(notifier=arguments.get('<notifier>'),  # type: ignore
                         title=arguments.get('--title'),  # type: ignore
                         recipient=arguments.get(
-                            '--recipient'),  # type: ignore
-                        body="\n".join(body),
-                        severity=arguments.get('--severity'),  # type: ignore
-                        attach=arguments.get('--attach')  # type: ignore
-                        )
+            '--recipient'),  # type: ignore
+            body="\n".join(body),
+            severity=arguments.get('--severity'),  # type: ignore
+            attach=arguments.get('--attach')  # type: ignore
+        )
         print(
             f"{r.json().get('detail')} [{r.status_code}]")
 
         exit(int(not (r)))
 
 
 if __name__ == "__main__":
```

### Comparing `buzz_client-1.0.1/buzz_client/client.py` & `buzz_client-1.0.2/buzz_client/client.py`

 * *Files identical despite different names*

### Comparing `buzz_client-1.0.1/PKG-INFO` & `buzz_client-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buzz-client
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: buzz-client Version: 1.0.1 Summary: A client for
+Metadata-Version: 2.1 Name: buzz-client Version: 1.0.2 Summary: A client for
 Buzz API License: GPL Author: Andrea Mistrali Author-email: andrea@mistrali.pw
 Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: docopt-ng
 (>=0.9.0,<0.10.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-Dist:
 requests (>=2.31.0,<3.0.0) Requires-Dist: scriptonite (>=1.0.3,<2.0.0)
```

