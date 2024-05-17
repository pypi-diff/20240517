# Comparing `tmp/mfu-0.0.6.tar.gz` & `tmp/mfu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfu-0.0.6.tar", last modified: Fri May 17 08:44:27 2024, max compression
+gzip compressed data, was "mfu-0.0.7.tar", last modified: Fri May 17 08:49:44 2024, max compression
```

## Comparing `mfu-0.0.6.tar` & `mfu-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-05-17 08:44:27.983802 mfu-0.0.6/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      444 2024-05-17 08:44:02.000000 mfu-0.0.6/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:51.000000 mfu-0.0.6/mfu/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)       61 2023-03-22 08:55:56.000000 mfu-0.0.6/mfu/__main__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)      324 2024-05-17 08:42:36.000000 mfu-0.0.6/mfu/main.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu/scripts/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:45.000000 mfu-0.0.6/mfu/scripts/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4159 2024-04-12 11:30:45.000000 mfu-0.0.6/mfu/scripts/cluster.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     1199 2023-03-22 09:33:27.000000 mfu-0.0.6/mfu/scripts/config.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3748 2023-03-22 09:16:00.000000 mfu-0.0.6/mfu/scripts/doctor.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3715 2022-11-23 11:16:20.000000 mfu-0.0.6/mfu/scripts/sync.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu/utils/
--rwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-23 11:12:20.000000 mfu-0.0.6/mfu/utils/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     2841 2022-11-23 11:15:13.000000 mfu-0.0.6/mfu/utils/forcelink.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3176 2023-06-20 13:21:08.000000 mfu-0.0.6/mfu/utils/general.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/PKG-INFO
--rwxr-xr-x   0 michael   (1000) michael   (1000)      418 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/SOURCES.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)        1 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/dependency_links.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)       37 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/entry_points.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/requires.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)        4 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/top_level.txt
--rwxr-xr-x   0 michael   (1000) michael   (1000)      486 2024-05-17 08:43:25.000000 mfu-0.0.6/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-17 08:44:27.983802 mfu-0.0.6/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)       68 2023-03-22 08:56:38.000000 mfu-0.0.6/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/
+-rw-r--r--   0 michael   (1000) michael   (1000)      827 2024-05-17 08:49:44.392214 mfu-0.0.7/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      476 2024-05-17 08:49:27.000000 mfu-0.0.7/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:51.000000 mfu-0.0.7/mfu/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)       61 2023-03-22 08:55:56.000000 mfu-0.0.7/mfu/__main__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      324 2024-05-17 08:42:36.000000 mfu-0.0.7/mfu/main.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu/scripts/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:45.000000 mfu-0.0.7/mfu/scripts/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4159 2024-04-12 11:30:45.000000 mfu-0.0.7/mfu/scripts/cluster.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1199 2023-03-22 09:33:27.000000 mfu-0.0.7/mfu/scripts/config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3748 2023-03-22 09:16:00.000000 mfu-0.0.7/mfu/scripts/doctor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3709 2024-05-17 08:49:07.000000 mfu-0.0.7/mfu/scripts/sync.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu/utils/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-23 11:12:20.000000 mfu-0.0.7/mfu/utils/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2841 2022-11-23 11:15:13.000000 mfu-0.0.7/mfu/utils/forcelink.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3176 2023-06-20 13:21:08.000000 mfu-0.0.7/mfu/utils/general.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:49:44.392214 mfu-0.0.7/mfu.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)      827 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/PKG-INFO
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      418 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/SOURCES.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        1 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/dependency_links.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       37 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/entry_points.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/requires.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        4 2024-05-17 08:49:44.000000 mfu-0.0.7/mfu.egg-info/top_level.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      486 2024-05-17 08:49:37.000000 mfu-0.0.7/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-17 08:49:44.392214 mfu-0.0.7/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)       68 2023-03-22 08:56:38.000000 mfu-0.0.7/setup.py
```

### Comparing `mfu-0.0.6/PKG-INFO` & `mfu-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfu
-Version: 0.0.6
+Version: 0.0.7
 Summary: Michael's fun utilities
 Author-email: Michael Botha <michael@408.co.za>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: Click>=8.1.3
 Requires-Dist: kubernetes>=25.3.0
 Requires-Dist: watchdog>=2.1.9
@@ -14,17 +14,20 @@
 # MFU (Michael's Fun Utilities)
 
 A collection of utilities to make my life easier and hopefully others too.
 
 
 ## Release Notes
 
-### 0.0.6
+### 0.0.7
 - Fixed new acumen namespace.
 
+### 0.0.6
+- Fixed pypi config.
+
 ### 0.0.5
 - Moved to pyproject.toml rather than setup.py
 - Added wheel in upload
 
 ### 0.0.4
 - Getting sync listener to work on Windows.
```

### Comparing `mfu-0.0.6/mfu/scripts/cluster.py` & `mfu-0.0.7/mfu/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.6/mfu/scripts/config.py` & `mfu-0.0.7/mfu/scripts/config.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.6/mfu/scripts/doctor.py` & `mfu-0.0.7/mfu/scripts/doctor.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.6/mfu/scripts/sync.py` & `mfu-0.0.7/mfu/scripts/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,27 +34,27 @@
         def __init__(self, project_path, branch):
             self.project_path = project_path.replace("\\", "/")  # Remove windows mapping for pod
             self.branch = branch.lower()
             self.system = platform.system()
 
         def on_modified(self, event):
             if "WebContent" in event.src_path and "~" not in event.src_path and not event.is_directory:
-                pods = v1.list_namespaced_pod(f"forcelink-{self.branch}", label_selector=podlabel).items
+                pods = v1.list_namespaced_pod(f"acumen-{self.branch}", label_selector=podlabel).items
                 if pods:
                     pod = pods[0]
                     pod_name = pod.metadata.name
                     src_path = event.src_path.replace("\\", "/")
                     dest_path = src_path.replace(self.project_path + "/WebContent", "")
                     if self.system == "Windows":
                         Path(f"{Path.home()}/.mfu-temp/").mkdir(parents=True, exist_ok=True)
                         copy_path = f"{Path.home()}\.mfu-temp\{src_path.split('/')[-1]}"
                         click.echo(f"Creating temp file at {copy_path}")
                         shutil.copyfile(src_path, copy_path)
                         src_path = copy_path.replace("\\", "/").split(":")[-1]
-                    command = f"kubectl --context={context} --namespace=forcelink-{self.branch} cp {src_path} {pod_name}:{podroot}{dest_path}"
+                    command = f"kubectl --context={context} --namespace=acumen-{self.branch} cp {src_path} {pod_name}:{podroot}{dest_path}"
                     command_list = command.split(" ")
                     if run_command(command_list) == 0:
                         click.echo(
                             f"Synced: {event.src_path} to {pod_name}:{podroot}{event.src_path.replace(f'{self.project_path}/WebContent', '')}")
                 else:
                     click.echo(click.style('No pods were found', fg='red'))
                     click.echo(click.style(f'Search Details:', fg='red'))
```

### Comparing `mfu-0.0.6/mfu/utils/forcelink.py` & `mfu-0.0.7/mfu/utils/forcelink.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.6/mfu/utils/general.py` & `mfu-0.0.7/mfu/utils/general.py`

 * *Files identical despite different names*

### Comparing `mfu-0.0.6/mfu.egg-info/PKG-INFO` & `mfu-0.0.7/mfu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfu
-Version: 0.0.6
+Version: 0.0.7
 Summary: Michael's fun utilities
 Author-email: Michael Botha <michael@408.co.za>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: Click>=8.1.3
 Requires-Dist: kubernetes>=25.3.0
 Requires-Dist: watchdog>=2.1.9
@@ -14,17 +14,20 @@
 # MFU (Michael's Fun Utilities)
 
 A collection of utilities to make my life easier and hopefully others too.
 
 
 ## Release Notes
 
-### 0.0.6
+### 0.0.7
 - Fixed new acumen namespace.
 
+### 0.0.6
+- Fixed pypi config.
+
 ### 0.0.5
 - Moved to pyproject.toml rather than setup.py
 - Added wheel in upload
 
 ### 0.0.4
 - Getting sync listener to work on Windows.
```

