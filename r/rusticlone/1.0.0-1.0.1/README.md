# Comparing `tmp/rusticlone-1.0.0.tar.gz` & `tmp/rusticlone-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rusticlone-1.0.0.tar", last modified: Wed May 15 10:36:46 2024, max compression
+gzip compressed data, was "rusticlone-1.0.1.tar", last modified: Fri May 17 08:52:02 2024, max compression
```

## Comparing `rusticlone-1.0.0.tar` & `rusticlone-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:36:46.425828 rusticlone-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 10:36:36.000000 rusticlone-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-15 10:36:46.421828 rusticlone-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-05-15 10:36:36.000000 rusticlone-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-15 10:36:36.000000 rusticlone-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:36:46.417828 rusticlone-1.0.0/rusticlone/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3164 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:36:46.421828 rusticlone-1.0.0/rusticlone/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/helpers/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/helpers/custom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/helpers/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/helpers/rclone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/helpers/rustic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/helpers/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:36:46.421828 rusticlone-1.0.0/rusticlone/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/processing/atomic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/processing/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    21586 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/processing/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6306 2024-05-15 10:36:36.000000 rusticlone-1.0.0/rusticlone/processing/sequential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:36:46.421828 rusticlone-1.0.0/rusticlone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-05-15 10:36:46.000000 rusticlone-1.0.0/rusticlone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-15 10:36:46.000000 rusticlone-1.0.0/rusticlone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:36:46.000000 rusticlone-1.0.0/rusticlone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-15 10:36:46.000000 rusticlone-1.0.0/rusticlone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 10:36:46.000000 rusticlone-1.0.0/rusticlone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 10:36:46.000000 rusticlone-1.0.0/rusticlone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:36:46.425828 rusticlone-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:52:02.362989 rusticlone-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 08:51:46.000000 rusticlone-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-05-17 08:52:02.362989 rusticlone-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-17 08:51:46.000000 rusticlone-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-17 08:51:46.000000 rusticlone-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:52:02.358988 rusticlone-1.0.1/rusticlone/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3164 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:52:02.358988 rusticlone-1.0.1/rusticlone/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/helpers/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/helpers/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/helpers/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/helpers/rclone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/helpers/rustic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/helpers/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:52:02.362989 rusticlone-1.0.1/rusticlone/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/processing/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/processing/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23765 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/processing/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-17 08:51:46.000000 rusticlone-1.0.1/rusticlone/processing/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:52:02.362989 rusticlone-1.0.1/rusticlone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11003 2024-05-17 08:52:02.000000 rusticlone-1.0.1/rusticlone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-17 08:52:02.000000 rusticlone-1.0.1/rusticlone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:52:02.000000 rusticlone-1.0.1/rusticlone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 08:52:02.000000 rusticlone-1.0.1/rusticlone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-17 08:52:02.000000 rusticlone-1.0.1/rusticlone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 08:52:02.000000 rusticlone-1.0.1/rusticlone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:52:02.362989 rusticlone-1.0.1/setup.cfg
```

### Comparing `rusticlone-1.0.0/LICENSE` & `rusticlone-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/PKG-INFO` & `rusticlone-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,21 @@
-Metadata-Version: 2.1
-Name: rusticlone
-Version: 1.0.0
-Summary: 3-2-1 backups using Rustic and RClone
-Author: AlphaJack
-Project-URL: Homepage, https://github.com/AlphaJack/rusticlone
-Project-URL: Issues, https://github.com/AlphaJack/rusticlone/issues
-Project-URL: Repository, https://github.com/AlphaJack/rusticlone
-Project-URL: Changelog, https://github.com/AlphaJack/rusticlone/blob/master/CHANGELOG.md
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: System :: Archiving :: Backup
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: importlib_metadata
-
 # Rusticlone
 
 <p style='text-align: center;'>
 <strong>3-2-1 backups using Rustic and RClone</strong>
 </p>
 
 <div style='text-align: left;'>
-    <img alt="backup process divided in archive and upload" src="images/process-backup.png" style="width: 43%; vertical-align: top;"/>
-    <img alt="output of rusticlone backup parallel" src="images/parallel-backup.png" style="width: 40%; vertical-align: top;"/>
-    <img alt="output of rusticlone backup sequential" src="images/sequential-backup.png" style="width: 14%; vertical-align: top;"/>
+    <img alt="backup process divided in archive and upload" src="https://github.com/AlphaJack/rusticlone/raw/master/images/process-backup.png" style="width: 43%; vertical-align: top;"/>
+    <img alt="output of rusticlone backup parallel" src="https://github.com/AlphaJack/rusticlone/raw/master/images/parallel-backup.png" style="width: 40%; vertical-align: top;"/>
+    <img alt="output of rusticlone backup sequential" src="https://github.com/AlphaJack/rusticlone/raw/master/images/sequential-backup.png" style="width: 14%; vertical-align: top;"/>
     <br/>
-    <img alt="restore process divided in download and extract" src="images/process-restore.png" style="width: 43%; vertical-align: top;"/>
-    <img alt="output of rusticlone restore parallel" src="images/parallel-restore.png" style="width: 40%; vertical-align: top;"/>
-    <img alt="output of rusticlone restore sequential" src="images/sequential-restore.png" style="width: 14%; vertical-align: top;"/>
+    <img alt="restore process divided in download and extract" src="https://github.com/AlphaJack/rusticlone/raw/master/images/process-restore.png" style="width: 43%; vertical-align: top;"/>
+    <img alt="output of rusticlone restore parallel" src="https://github.com/AlphaJack/rusticlone/raw/master/images/parallel-restore.png" style="width: 40%; vertical-align: top;"/>
+    <img alt="output of rusticlone restore sequential" src="https://github.com/AlphaJack/rusticlone/raw/master/images/sequential-restore.png" style="width: 14%; vertical-align: top;"/>
 </div>
 
 ## Motivation
 
 [Rustic](https://rustic.cli.rs/) comes with [native support](https://rustic.cli.rs/docs/commands/init/rclone.html) for [RClone](https://rclone.org/)'s built-in [Restic server](https://rclone.org/commands/rclone_serve_restic/).
 After trying this feature, I experienced an abysmally low backup speed, much lower than my upload bandwidth: the bottleneck was the synchronous RClone server, as Rustic was waiting for a response before sending other data.
 
@@ -263,18 +242,18 @@
 
 ```ini
 [Unit]
 Description=Rusticlone service
 
 [Service]
 Type=oneshot
-ExecStart=rusticlone --ignore-pattern "common" --remote "gdrive:/PC" backup
+ExecStart=rusticlone --ignore "common" --remote "gdrive:/PC" backup
 ```
 
-Adjust your `--ignore-pattern` and `--remote` as needed.
+Adjust your `--ignore` and `--remote` as needed.
 
 Apply your changes and enable the timer:
 
 ```bash
 sudo systemctl daemon-reload
 sudo systemctl enable --now rusticlone.timer
 ```
```

### Comparing `rusticlone-1.0.0/README.md` & `rusticlone-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,42 @@
+Metadata-Version: 2.1
+Name: rusticlone
+Version: 1.0.1
+Summary: 3-2-1 backups using Rustic and RClone
+Author: AlphaJack
+Project-URL: Homepage, https://github.com/AlphaJack/rusticlone
+Project-URL: Issues, https://github.com/AlphaJack/rusticlone/issues
+Project-URL: Repository, https://github.com/AlphaJack/rusticlone
+Project-URL: Changelog, https://github.com/AlphaJack/rusticlone/blob/master/CHANGELOG.md
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Topic :: System :: Archiving :: Backup
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: importlib_metadata
+
 # Rusticlone
 
 <p style='text-align: center;'>
 <strong>3-2-1 backups using Rustic and RClone</strong>
 </p>
 
 <div style='text-align: left;'>
-    <img alt="backup process divided in archive and upload" src="images/process-backup.png" style="width: 43%; vertical-align: top;"/>
-    <img alt="output of rusticlone backup parallel" src="images/parallel-backup.png" style="width: 40%; vertical-align: top;"/>
-    <img alt="output of rusticlone backup sequential" src="images/sequential-backup.png" style="width: 14%; vertical-align: top;"/>
+    <img alt="backup process divided in archive and upload" src="https://github.com/AlphaJack/rusticlone/raw/master/images/process-backup.png" style="width: 43%; vertical-align: top;"/>
+    <img alt="output of rusticlone backup parallel" src="https://github.com/AlphaJack/rusticlone/raw/master/images/parallel-backup.png" style="width: 40%; vertical-align: top;"/>
+    <img alt="output of rusticlone backup sequential" src="https://github.com/AlphaJack/rusticlone/raw/master/images/sequential-backup.png" style="width: 14%; vertical-align: top;"/>
     <br/>
-    <img alt="restore process divided in download and extract" src="images/process-restore.png" style="width: 43%; vertical-align: top;"/>
-    <img alt="output of rusticlone restore parallel" src="images/parallel-restore.png" style="width: 40%; vertical-align: top;"/>
-    <img alt="output of rusticlone restore sequential" src="images/sequential-restore.png" style="width: 14%; vertical-align: top;"/>
+    <img alt="restore process divided in download and extract" src="https://github.com/AlphaJack/rusticlone/raw/master/images/process-restore.png" style="width: 43%; vertical-align: top;"/>
+    <img alt="output of rusticlone restore parallel" src="https://github.com/AlphaJack/rusticlone/raw/master/images/parallel-restore.png" style="width: 40%; vertical-align: top;"/>
+    <img alt="output of rusticlone restore sequential" src="https://github.com/AlphaJack/rusticlone/raw/master/images/sequential-restore.png" style="width: 14%; vertical-align: top;"/>
 </div>
 
 ## Motivation
 
 [Rustic](https://rustic.cli.rs/) comes with [native support](https://rustic.cli.rs/docs/commands/init/rclone.html) for [RClone](https://rclone.org/)'s built-in [Restic server](https://rclone.org/commands/rclone_serve_restic/).
 After trying this feature, I experienced an abysmally low backup speed, much lower than my upload bandwidth: the bottleneck was the synchronous RClone server, as Rustic was waiting for a response before sending other data.
 
@@ -242,18 +263,18 @@
 
 ```ini
 [Unit]
 Description=Rusticlone service
 
 [Service]
 Type=oneshot
-ExecStart=rusticlone --ignore-pattern "common" --remote "gdrive:/PC" backup
+ExecStart=rusticlone --ignore "common" --remote "gdrive:/PC" backup
 ```
 
-Adjust your `--ignore-pattern` and `--remote` as needed.
+Adjust your `--ignore` and `--remote` as needed.
 
 Apply your changes and enable the timer:
 
 ```bash
 sudo systemctl daemon-reload
 sudo systemctl enable --now rusticlone.timer
 ```
```

### Comparing `rusticlone-1.0.0/pyproject.toml` & `rusticlone-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [tool.setuptools]
 packages = ["rusticlone", "rusticlone.helpers", "rusticlone.processing"]
 
 # ################################################################ Project
 
 [project]
 name = "rusticlone"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="AlphaJack" },
 ]
 description = "3-2-1 backups using Rustic and RClone"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `rusticlone-1.0.0/rusticlone/cli.py` & `rusticlone-1.0.1/rusticlone/cli.py`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/rusticlone/helpers/action.py` & `rusticlone-1.0.1/rusticlone/helpers/action.py`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/rusticlone/helpers/custom.py` & `rusticlone-1.0.1/rusticlone/helpers/custom.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # os and hostname
 import platform
 
 # exit
 import sys
 
 # rusticlone
-from rusticlone.helpers.formatting import print_stats
+from rusticlone.helpers.action import Action
 from rusticlone.processing.parallel import (
     system_backup_parallel,
     system_archive_parallel,
     system_upload_parallel,
     system_restore_parallel,
     system_download_parallel,
     system_extract_parallel,
@@ -89,51 +89,54 @@
         else:
             self.profiles = []
 
     def check_log_file(self):
         """
         Create log file parent folders if missing, delete old log file
         """
-        print_stats("Checking log file", "")
+        action = Action("Checking log file")
         if self.log_file != self.default_log_file:
             used_log = self.log_file
             self.log_file.parents[0].mkdir(parents=True, exist_ok=True)
             self.log_file.unlink(missing_ok=True)
             self.log_file.touch()
         else:
             # if not defined in Rustic profiles, "./rusticlone.log" is used
             used_log = "defined in Rustic profiles"
-        print_stats(f"Log file: {used_log}", "")
+        action.stop(f"Log file: {used_log}", "")
 
 
 # ################################################################ FUNCTIONS
 
 
 def list_profiles(
     profiles_dirs: list, profiles: list, ignore_pattern: str = "🫣🫣🫣"
 ) -> list:
     """
     Scan profiles from directories if none have been provided explicitely
+    Don't scan from /etc/rustic if ~/.config/rustic has some profiles'
     """
+    action = Action("Reading profiles")
     if not profiles:
         for profiles_dir in profiles_dirs:
-            if profiles_dir.exists() and profiles_dir.is_dir():
+            if len(profiles) == 0 and profiles_dir.exists() and profiles_dir.is_dir():
+                action.stop(f'Scanning "{profiles_dir}"', "")
                 files = sorted(list(profiles_dir.glob("*.toml")))
                 for file in files:
                     if (
                         file.is_file()
                         and ignore_pattern not in file.stem
                         and file.stem not in profiles
                     ):
                         profiles.append(file.stem)
     if len(profiles) == 0:
-        print("Could not find any rustic profile, aborting")
+        action.abort("Could not find any rustic profile")
         sys.exit(1)
     else:
-        print("Profiles:", profiles)
+        action.stop(f"Profiles: {str(profiles)}", "")
         return profiles
 
 
 def process_profiles(
     profiles: list,
     parallel: bool,
     command: str,
```

### Comparing `rusticlone-1.0.0/rusticlone/helpers/formatting.py` & `rusticlone-1.0.1/rusticlone/helpers/formatting.py`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/rusticlone/helpers/rclone.py` & `rusticlone-1.0.1/rusticlone/helpers/rclone.py`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/rusticlone/helpers/rustic.py` & `rusticlone-1.0.1/rusticlone/helpers/rustic.py`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/rusticlone/helpers/timer.py` & `rusticlone-1.0.1/rusticlone/helpers/timer.py`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/rusticlone/processing/atomic.py` & `rusticlone-1.0.1/rusticlone/processing/atomic.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,11 +106,12 @@
     timer = Timer(parallel)
     profile = Profile(name, parallel)
     profile.read_rustic_config()
     profile.parse_rustic_config()
     profile.set_log_file(log_file)
     profile.check_local_repo_exists()
     profile.latest()
+    profile.check_source_type()
     profile.restore()
     timer.stop()
     # print_stats("", "")
     return profile.result, timer.duration
```

### Comparing `rusticlone-1.0.0/rusticlone/processing/parallel.py` & `rusticlone-1.0.1/rusticlone/processing/parallel.py`

 * *Files identical despite different names*

### Comparing `rusticlone-1.0.0/rusticlone/processing/profile.py` & `rusticlone-1.0.1/rusticlone/processing/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,22 @@
         """
         Default values for each Rustic profile
         """
         self.profile_name = profile
         self.parallel = parallel
         self.source = ""
         self.repo = ""
-        self.log_file = Path("")
+        self.log_file = Path("rusticlone.log")
         self.password_provided = ""
         self.rclone_config = ""
         self.rclone_config_pass = ""
         self.rclone_config_pass_comm = ""
         self.backup_output = ""
         self.source_exists = False
+        self.source_type = "dir"
         self.local_repo_exists = False
         self.remote_repo_exists = False
         self.snapshot_exists = False
         self.result = True
         self.hostname = platform.node()
         self.config = ""
         # self.repo_info = ""
@@ -131,15 +132,17 @@
                         "Could not parse source in config:\n", self.config
                     )
                 case self.repo:
                     self.result = action.abort(
                         "Could not parse repo in config:\n", self.config
                     )
                 case str(self.log_file):
-                    self.result = action.abort("Invalid log file")
+                    self.result = action.abort(
+                        f'Invalid log file: "{str(self.log_file)}"'
+                    )
                 case self.password_provided:
                     self.result = action.abort(
                         "Could not parse password in config:\n", self.config
                     )
                 case _:
                     action.stop("Rustic configuration parsed")
 
@@ -179,34 +182,44 @@
                 self.result = action.abort("Empty rustic config")
 
     def set_log_file(self, passed_log_file: Path) -> None:
         """
         set rclone log file
         if not default has been passed, use it, otherwise use the one in conf
         if there are no matches in conf, use the default one
+        rustic fails if it cannot find the parent folder of the log file when parsing the conf,
+        so it must be created before Profile.read_rustic_config() is run
         from now on, use self.log_file in Profile.upload() and Profile.download()
         """
         if self.result:
-            action = Action("Setting log file for rclone", self.parallel)
-            default_log_file = Path("rusticlone.log")
-            if passed_log_file != default_log_file or str(self.log_file) == ".":
+            action = Action("Setting log file", self.parallel)
+            if passed_log_file != Path("rusticlone.log"):
                 self.log_file = passed_log_file
-                action.stop("RClone uses specified log file")
-            else:
-                action.stop("RClone uses Rustic log file")
+            if self.parallel:
+                suffix_old = self.log_file.suffix
+                suffix_new = "-" + self.profile_name + ".log"
+                self.log_file = Path(str(self.log_file).replace(suffix_old, suffix_new))
+                # rustic fails anyway if it cannot find the path when parsing the conf
+                # self.log_file.parent.mkdir(parents=True, exist_ok=True)
+                # self.log_file.touch(exist_ok=True)
+            action.stop("Log file set")
 
     def check_source_exists(self) -> None:
         """
         Check if the source exists and handle accordingly.
         """
         if self.result:
             action = Action("Checking if source exists", self.parallel)
             # print(self.source)
-            folder = Path(self.source)
-            if folder.exists() and folder.is_dir():
+            source = Path(self.source)
+            if source.exists():
+                if source.is_dir():
+                    self.source_type = "dir"
+                else:
+                    self.source_type = "file"
                 self.source_exists = True
                 action.stop("Source exists")
             else:
                 # self.source_exists = False
                 self.result = action.abort("Source does not exist")
 
     def check_local_repo_exists(self) -> None:
@@ -228,15 +241,17 @@
         """
         Check remote repo folder with rclone
         """
         if self.result:
             if self.rclone_config:
                 action = Action("Checking if remote repo exists", self.parallel)
                 rclone_log_file = str(self.log_file)
-                rclone_origin = remote_prefix + "/" + self.profile_name
+                # rclone_origin = remote_prefix + "/" + self.profile_name
+                repo_name = str(Path(self.repo).name)
+                rclone_origin = remote_prefix + "/" + repo_name
                 rclone_lsd = Rclone(
                     config=self.rclone_config,
                     config_pass=self.rclone_config_pass,
                     config_pass_command=self.rclone_config_pass_comm,
                     log_file=rclone_log_file,
                     action="lsd",
                     origin=rclone_origin,
@@ -398,42 +413,48 @@
         Uploads the local repository to a remote destination using rclone.
         """
         if self.result:
             action = Action("Uploading repo", self.parallel)
             if self.rclone_config != "" and self.local_repo_exists:
                 rclone_log_file = str(self.log_file)
                 rclone_origin = self.repo.replace("\\", "/").replace("//", "/")
-                rclone_destination = remote_prefix + "/" + self.profile_name
+                # rclone_destination = remote_prefix + "/" + self.profile_name
+                repo_name = str(Path(self.repo).name)
+                rclone_destination = remote_prefix + "/" + repo_name
                 # print(rclone_destination)
                 Rclone(
                     config=self.rclone_config,
                     config_pass=self.rclone_config_pass,
                     config_pass_command=self.rclone_config_pass_comm,
                     log_file=rclone_log_file,
                     action="sync",
                     origin=rclone_origin,
                     destination=rclone_destination,
                 )
                 # action.stop(f"Uploaded repo: {rclone_destination}")
                 action.stop("Uploaded repo")
             else:
-                action.stop("Rclone config missing or repository is already remote", "")
+                self.result = action.abort(
+                    "RClone config missing or local repo does not exist", ""
+                )
 
     def download(self, remote_prefix: str) -> None:
         """
         Uploads the remote repository to a local destination using rclone.
         """
         if self.result:
             if not self.repo.startswith("rclone:"):
                 action = Action("Downloading repo", self.parallel)
                 if not self.local_repo_exists:
                     if self.rclone_config is not None:
                         if self.remote_repo_exists:
                             rclone_log_file = str(self.log_file)
-                            rclone_origin = remote_prefix + "/" + self.profile_name
+                            # rclone_origin = remote_prefix + "/" + self.profile_name
+                            repo_name = str(Path(self.repo).name)
+                            rclone_origin = remote_prefix + "/" + repo_name
                             rclone_destination = self.repo
                             Rclone(
                                 config=self.rclone_config,
                                 config_pass=self.rclone_config_pass,
                                 config_pass_command=self.rclone_config_pass_comm,
                                 log_file=rclone_log_file,
                                 action="sync",
@@ -492,22 +513,49 @@
                         self.result = action.abort("Cannot parse timestamp")
                 else:
                     self.result = action.abort("Repo does not have snapshots")
         # else:
         #    self.snapshot_exists = False
         #    action.abort("Skipping non-existing repo")
 
+    def check_source_type(self) -> None:
+        """
+        Check if the source that needs to be restored is a directory or file
+        """
+        if self.result:
+            action = Action("Checking source type", self.parallel)
+            if self.local_repo_exists and self.snapshot_exists:
+                rustic = Rustic(
+                    self.profile_name,
+                    "ls",
+                    "latest",
+                    "--glob",
+                    f"{self.source}",
+                    "--long",
+                    "--log-file",
+                    str(self.log_file),
+                )
+                if rustic.stdout[0] == "d" or rustic.stdout.count("\n") > 1:
+                    self.source_type = "dir"
+                else:
+                    self.source_type = "file"
+                action.stop(f"Source is a {self.source_type}")
+
     def restore(self) -> None:
         """
         Extract files in the latest snapshot to the source location, after creating it if missing
-        self.source must exist, so rustic can create the folder inside it
+        if self.source is a directory, it is created if missing
+        if self.source is a file, its parent is created if missing
         """
         if self.result:
             action = Action("Extracting snapshot", self.parallel)
-            Path(self.source).mkdir(parents=True, exist_ok=True)
+            if self.source_type == "dir":
+                Path(self.source).mkdir(parents=True, exist_ok=True)
+            else:
+                Path(self.source).parent.mkdir(parents=True, exist_ok=True)
             if self.local_repo_exists and self.snapshot_exists:
                 Rustic(
                     self.profile_name,
                     "restore",
                     f"latest:{self.source}",
                     self.source,
                     "--log-file",
```

### Comparing `rusticlone-1.0.0/rusticlone/processing/sequential.py` & `rusticlone-1.0.1/rusticlone/processing/sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     for name in profiles:
         archive_success, duration = profile_archive(name=name, log_file=log_file)
         archive_results[name] = archive_success
         if archive_success:
             print_stats("", "")
         else:
             print_stats(f"Error archiving {name}", "")
+            print_stats("", "")
     return archive_results
 
 
 def system_upload_sequential(
     profiles: list,
     log_file: Path,
     remote_prefix: str,
@@ -109,14 +110,15 @@
             )
             if upload_success:
                 print_stats("", "")
             else:
                 print_stats(f"Error uploading {name}", "")
         else:
             print_stats(f"Not uploading {name} as archiving failed", "")
+            print_stats("", "")
 
 
 # ################################ RESTORE
 
 
 def system_restore_sequential(
     profiles: list, log_file: Path, remote_prefix: str
```

### Comparing `rusticlone-1.0.0/rusticlone.egg-info/PKG-INFO` & `rusticlone-1.0.1/rusticlone.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rusticlone
-Version: 1.0.0
+Version: 1.0.1
 Summary: 3-2-1 backups using Rustic and RClone
 Author: AlphaJack
 Project-URL: Homepage, https://github.com/AlphaJack/rusticlone
 Project-URL: Issues, https://github.com/AlphaJack/rusticlone/issues
 Project-URL: Repository, https://github.com/AlphaJack/rusticlone
 Project-URL: Changelog, https://github.com/AlphaJack/rusticlone/blob/master/CHANGELOG.md
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,21 +22,21 @@
 # Rusticlone
 
 <p style='text-align: center;'>
 <strong>3-2-1 backups using Rustic and RClone</strong>
 </p>
 
 <div style='text-align: left;'>
-    <img alt="backup process divided in archive and upload" src="images/process-backup.png" style="width: 43%; vertical-align: top;"/>
-    <img alt="output of rusticlone backup parallel" src="images/parallel-backup.png" style="width: 40%; vertical-align: top;"/>
-    <img alt="output of rusticlone backup sequential" src="images/sequential-backup.png" style="width: 14%; vertical-align: top;"/>
+    <img alt="backup process divided in archive and upload" src="https://github.com/AlphaJack/rusticlone/raw/master/images/process-backup.png" style="width: 43%; vertical-align: top;"/>
+    <img alt="output of rusticlone backup parallel" src="https://github.com/AlphaJack/rusticlone/raw/master/images/parallel-backup.png" style="width: 40%; vertical-align: top;"/>
+    <img alt="output of rusticlone backup sequential" src="https://github.com/AlphaJack/rusticlone/raw/master/images/sequential-backup.png" style="width: 14%; vertical-align: top;"/>
     <br/>
-    <img alt="restore process divided in download and extract" src="images/process-restore.png" style="width: 43%; vertical-align: top;"/>
-    <img alt="output of rusticlone restore parallel" src="images/parallel-restore.png" style="width: 40%; vertical-align: top;"/>
-    <img alt="output of rusticlone restore sequential" src="images/sequential-restore.png" style="width: 14%; vertical-align: top;"/>
+    <img alt="restore process divided in download and extract" src="https://github.com/AlphaJack/rusticlone/raw/master/images/process-restore.png" style="width: 43%; vertical-align: top;"/>
+    <img alt="output of rusticlone restore parallel" src="https://github.com/AlphaJack/rusticlone/raw/master/images/parallel-restore.png" style="width: 40%; vertical-align: top;"/>
+    <img alt="output of rusticlone restore sequential" src="https://github.com/AlphaJack/rusticlone/raw/master/images/sequential-restore.png" style="width: 14%; vertical-align: top;"/>
 </div>
 
 ## Motivation
 
 [Rustic](https://rustic.cli.rs/) comes with [native support](https://rustic.cli.rs/docs/commands/init/rclone.html) for [RClone](https://rclone.org/)'s built-in [Restic server](https://rclone.org/commands/rclone_serve_restic/).
 After trying this feature, I experienced an abysmally low backup speed, much lower than my upload bandwidth: the bottleneck was the synchronous RClone server, as Rustic was waiting for a response before sending other data.
 
@@ -263,18 +263,18 @@
 
 ```ini
 [Unit]
 Description=Rusticlone service
 
 [Service]
 Type=oneshot
-ExecStart=rusticlone --ignore-pattern "common" --remote "gdrive:/PC" backup
+ExecStart=rusticlone --ignore "common" --remote "gdrive:/PC" backup
 ```
 
-Adjust your `--ignore-pattern` and `--remote` as needed.
+Adjust your `--ignore` and `--remote` as needed.
 
 Apply your changes and enable the timer:
 
 ```bash
 sudo systemctl daemon-reload
 sudo systemctl enable --now rusticlone.timer
 ```
```

### Comparing `rusticlone-1.0.0/rusticlone.egg-info/SOURCES.txt` & `rusticlone-1.0.1/rusticlone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

