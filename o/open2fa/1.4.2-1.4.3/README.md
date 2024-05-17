# Comparing `tmp/open2fa-1.4.2-py3-none-any.whl.zip` & `tmp/open2fa-1.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20672 bytes, number of entries: 17
+Zip file size: 20694 bytes, number of entries: 17
 -rw-r--r--  2.0 unx      113 b- defN 24-Feb-12 01:03 open2fa/__init__.py
--rw-r--r--  2.0 unx    10069 b- defN 24-Mar-25 23:32 open2fa/cli.py
+-rw-r--r--  2.0 unx    10180 b- defN 24-May-17 12:35 open2fa/cli.py
 -rw-r--r--  2.0 unx     4747 b- defN 24-Apr-27 23:38 open2fa/cli_utils.py
 -rw-r--r--  2.0 unx     4334 b- defN 24-Mar-24 22:21 open2fa/common.py
 -rw-r--r--  2.0 unx      660 b- defN 24-Apr-11 22:49 open2fa/config.py
 -rw-r--r--  2.0 unx      923 b- defN 24-Mar-21 19:32 open2fa/ex.py
 -rw-r--r--  2.0 unx    17991 b- defN 24-Apr-28 22:53 open2fa/main.py
 -rw-r--r--  2.0 unx     1814 b- defN 24-Apr-28 22:58 open2fa/msgs.py
 -rw-r--r--  2.0 unx     2248 b- defN 24-Apr-16 18:10 open2fa/totp.py
 -rw-r--r--  2.0 unx     2139 b- defN 24-Mar-21 19:36 open2fa/utils.py
--rw-r--r--  2.0 unx       22 b- defN 24-May-13 05:50 open2fa/version.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    11088 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1284 b- defN 24-May-13 08:19 open2fa-1.4.2.dist-info/RECORD
-17 files, 58652 bytes uncompressed, 18602 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx       22 b- defN 24-May-17 12:38 open2fa/version.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-17 14:59 open2fa-1.4.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx    11133 b- defN 24-May-17 14:59 open2fa-1.4.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 14:59 open2fa-1.4.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 24-May-17 14:59 open2fa-1.4.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-May-17 14:59 open2fa-1.4.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1284 b- defN 24-May-17 14:59 open2fa-1.4.3.dist-info/RECORD
+17 files, 58808 bytes uncompressed, 18624 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: open2fa/utils.py
 Comment: 
 
 Filename: open2fa/version.py
 Comment: 
 
-Filename: open2fa-1.4.2.dist-info/LICENSE
+Filename: open2fa-1.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: open2fa-1.4.2.dist-info/METADATA
+Filename: open2fa-1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: open2fa-1.4.2.dist-info/WHEEL
+Filename: open2fa-1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: open2fa-1.4.2.dist-info/entry_points.txt
+Filename: open2fa-1.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: open2fa-1.4.2.dist-info/top_level.txt
+Filename: open2fa-1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: open2fa-1.4.2.dist-info/RECORD
+Filename: open2fa-1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## open2fa/cli.py

```diff
@@ -146,28 +146,30 @@
         'remote', help='Remote operations', aliases=['r']
     )
     remote_subparsers = parser_remote.add_subparsers(
         dest='remote_command', required=True, help='Remote operations'
     )
 
     remote_list = remote_subparsers.add_parser(
-        'list', help='List remote secrets'
+        'list', aliases=['l'], help='List remote secrets'
     )
     remote_list.add_argument(
         '-s',
         '--secrets',
         '--secret',
         dest='show_secrets',
         action='store_true',
         help='Show full secrets',
         default=False,
     )
 
     # Init remote command
-    remote_subparsers.add_parser('init', help='Initialize remote capabilities')
+    remote_subparsers.add_parser(
+        'init', help='Initialize remote capabilities', aliases=['i']
+    )
 
     # Info/Status remote command
     parser_info = subparsers.add_parser(
         'info', help='Show Open2FA info/status', aliases=['i']
     )
 
     parser_info.add_argument(
@@ -176,17 +178,21 @@
         '--secrets',
         help='Show all info/status info without censorship',
         dest='show_secrets',
         action='store_true',
         default=False,
     )
     # Push remote command
-    remote_subparsers.add_parser('push', help='Push secrets to remote')
+    remote_subparsers.add_parser(
+        'push', help='Push secrets to remote', aliases=['pus']
+    )
     # Pull remote command
-    remote_subparsers.add_parser('pull', help='Pull secrets from remote')
+    remote_subparsers.add_parser(
+        'pull', help='Pull secrets from remote', aliases=['pul']
+    )
 
     # Delete remote command
     del_parser = remote_subparsers.add_parser(
         'delete', help='Delete remote secrets', aliases=['d']
     )
     del_parser.add_argument(
         'secret', type=str, help='The TOTP secret key to delete', nargs='?'
@@ -198,15 +204,15 @@
         help='Name of the secret to delete',
         dest='name',
     )
 
     return parser
 
 
-def _print_secrets(secrets: list[TOTPSecret], show_secrets: bool = False):
+def _print_secrets(secrets: TYPE.List[TOTPSecret], show_secrets: bool = False):
     """Prints a list of TOTPSecrets to the console."""
     max_name, max_secret = 4, 6
     if len(secrets) > 0:
         max_name = max([len(str(s.name)) for s in secrets])
         max_secret = max(
             [
                 (
```

## open2fa/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.4.2"
+__version__ = "1.4.3"
```

## Comparing `open2fa-1.4.2.dist-info/LICENSE` & `open2fa-1.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `open2fa-1.4.2.dist-info/METADATA` & `open2fa-1.4.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open2fa
-Version: 1.4.2
+Version: 1.4.3
 Summary: A 2FA CLI tool for generating 2FA codes using TOTP secrets, with an optional SECURE remote api, and an optional web ui enabling 2FA code generation from any device
 Author-email: Cary Carter <ccarterdev@gmail.com>
 Project-URL: Homepage, https://open2fa.liberfy.ai
 Project-URL: Repository, https://github.com/cc-d/open2fa
 Project-URL: Issues, https://github.com/cc-d/open2fa/issues
 Project-URL: Server, https://github.com/cc-d/open2fa-server
 Project-URL: Documentation, https://github.com/cc-d/open2fa
@@ -24,15 +24,16 @@
 Requires-Dist: logfunc <3.0.0
 Requires-Dist: cryptography <=41.0.7
 Requires-Dist: pyshared <1.6.0
 Requires-Dist: base58 ==2.1.1
 Provides-Extra: dev
 Requires-Dist: pytest ; extra == 'dev'
 Requires-Dist: pytest-cov ; extra == 'dev'
-Requires-Dist: pytest-mock ; extra == 'dev'
+Requires-Dist: pytest-xdist ; extra == 'dev'
+Requires-Dist: pytest-html ; extra == 'dev'
 Requires-Dist: black ; extra == 'dev'
 Requires-Dist: isort ; extra == 'dev'
 Requires-Dist: flake8 ; extra == 'dev'
 Requires-Dist: twine ; extra == 'dev'
 Requires-Dist: build ; extra == 'dev'
 Requires-Dist: pyshared ; extra == 'dev'
```

