# Comparing `tmp/socketsecurity-0.0.66.tar.gz` & `tmp/socketsecurity-0.0.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.66.tar", last modified: Thu May 16 11:43:04 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.67.tar", last modified: Fri May 17 19:35:03 2024, max compression
```

## Comparing `socketsecurity-0.0.66.tar` & `socketsecurity-0.0.67.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:43:04.915116 socketsecurity-0.0.66/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 11:43:04.914923 socketsecurity-0.0.66/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)       21 2024-05-15 04:22:36.000000 socketsecurity-0.0.66/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-16 11:43:00.000000 socketsecurity-0.0.66/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 11:43:04.915156 socketsecurity-0.0.66/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:43:04.901987 socketsecurity-0.0.66/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.66/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:43:04.914402 socketsecurity-0.0.66/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26207 2024-05-16 11:42:54.000000 socketsecurity-0.0.66/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.66/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      785 2024-05-16 11:28:29.000000 socketsecurity-0.0.66/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.66/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11041 2024-05-16 11:03:01.000000 socketsecurity-0.0.66/socketsecurity/core/gitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.66/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.66/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.66/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5975 2024-05-16 10:18:06.000000 socketsecurity-0.0.66/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-16 11:43:04.914681 socketsecurity-0.0.66/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)      771 2024-05-16 11:43:04.000000 socketsecurity-0.0.66/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      560 2024-05-16 11:43:04.000000 socketsecurity-0.0.66/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-16 11:43:04.000000 socketsecurity-0.0.66/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-16 11:43:04.000000 socketsecurity-0.0.66/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-16 11:43:04.000000 socketsecurity-0.0.66/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-16 11:43:04.000000 socketsecurity-0.0.66/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-17 19:35:03.800377 socketsecurity-0.0.67/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1066 2024-05-17 19:27:22.000000 socketsecurity-0.0.67/LICENSE
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-17 19:35:03.800193 socketsecurity-0.0.67/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4136 2024-05-17 19:24:12.000000 socketsecurity-0.0.67/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-17 19:29:29.000000 socketsecurity-0.0.67/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-17 19:35:03.800413 socketsecurity-0.0.67/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-17 19:35:03.789550 socketsecurity-0.0.67/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.67/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-17 19:35:03.799682 socketsecurity-0.0.67/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26209 2024-05-17 19:29:42.000000 socketsecurity-0.0.67/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.67/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      785 2024-05-16 11:28:29.000000 socketsecurity-0.0.67/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.67/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11041 2024-05-16 11:03:01.000000 socketsecurity-0.0.67/socketsecurity/core/gitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.67/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.67/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.67/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5912 2024-05-17 19:20:19.000000 socketsecurity-0.0.67/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-17 19:35:03.799880 socketsecurity-0.0.67/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-17 19:35:03.000000 socketsecurity-0.0.67/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      568 2024-05-17 19:35:03.000000 socketsecurity-0.0.67/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-17 19:35:03.000000 socketsecurity-0.0.67/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-17 19:35:03.000000 socketsecurity-0.0.67/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-17 19:35:03.000000 socketsecurity-0.0.67/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-17 19:35:03.000000 socketsecurity-0.0.67/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.66/pyproject.toml` & `socketsecurity-0.0.67/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.66"
+version = "0.0.67"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.66/socketsecurity/core/__init__.py` & `socketsecurity-0.0.67/socketsecurity/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.66'
+__version__ = '0.0.67'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
 
 
@@ -200,16 +200,16 @@
         path = f"orgs/{org_slug}/full-scans/{full_scan_id}"
         response = do_request(path)
         results = []
         try:
             data = response.json()
             results = data.get("sbom_artifacts") or []
         except Exception as error:
-            log.info("Failed with old style full-scan API using new format")
-            log.info(error)
+            log.debug("Failed with old style full-scan API using new format")
+            log.debug(error)
             data = response.text
             data.strip('"')
             data.strip()
             for line in data.split("\n"):
                 if line != '"' and line != "" and line is not None:
                     item = json.loads(line)
                     results.append(item)
```

### Comparing `socketsecurity-0.0.66/socketsecurity/core/classes.py` & `socketsecurity-0.0.67/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.66/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.67/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.66/socketsecurity/core/github.py` & `socketsecurity-0.0.67/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.66/socketsecurity/core/gitlab.py` & `socketsecurity-0.0.67/socketsecurity/core/gitlab.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.66/socketsecurity/core/issues.py` & `socketsecurity-0.0.67/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.66/socketsecurity/core/licenses.py` & `socketsecurity-0.0.67/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.66/socketsecurity/core/messages.py` & `socketsecurity-0.0.67/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.66/socketsecurity/socketcli.py` & `socketsecurity-0.0.67/socketsecurity/socketcli.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 parser.add_argument(
     '--commit_message',
     help='Commit or build message for the run',
     required=False
 )
 parser.add_argument(
     '--default_branch',
-    default=1,
+    default=False,
+    action='store_true',
     help='Whether this is the default/head for run'
 )
 parser.add_argument(
     '--target_path',
     default='./',
     help='Path to look for manifest files',
     required=False
@@ -86,14 +87,15 @@
 parser.add_argument(
     '--enable-debug',
     help='Enable debug mode',
     action='store_true',
     default=False
 )
 
+
 def output_console_comments(diff_report) -> None:
     console_security_comment = Messages.create_console_security_alert_table(diff_report)
     if len(diff_report.new_alerts) > 0:
         log.info("Security issues detected by Socket Security")
         log.info(console_security_comment)
         sys.exit(1)
     else:
@@ -105,18 +107,15 @@
     debug = arguments.enable_debug
     if debug:
         logging.basicConfig(level=logging.DEBUG)
     repo = arguments.repo
     branch = arguments.branch
     commit_message = arguments.commit_message
     committer = arguments.committer
-    default_branch_int = arguments.default_branch
-    default_branch = False
-    if default_branch_int == 1:
-        default_branch = True
+    default_branch = arguments.default_branch
     pr_number = arguments.pr_number
     target_path = arguments.target_path
     scm_type = arguments.scm
     license_mode = arguments.generate_license
     license_file = f"{repo}"
     if branch is not None:
         license_file += f"_{branch}"
```

### Comparing `socketsecurity-0.0.66/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.67/socketsecurity.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 socketsecurity/__init__.py
 socketsecurity/socketcli.py
 socketsecurity.egg-info/PKG-INFO
 socketsecurity.egg-info/SOURCES.txt
 socketsecurity.egg-info/dependency_links.txt
```

