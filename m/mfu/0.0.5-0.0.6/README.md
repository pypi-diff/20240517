# Comparing `tmp/mfu-0.0.5.tar.gz` & `tmp/mfu-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfu-0.0.5.tar", last modified: Mon Nov 21 09:19:56 2022, max compression
+gzip compressed data, was "mfu-0.0.6.tar", last modified: Fri May 17 08:44:27 2024, max compression
```

## Comparing `mfu-0.0.5.tar` & `mfu-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/
--rw-rw-r--   0 michael   (1000) michael   (1000)      514 2022-11-21 09:19:56.104891 mfu-0.0.5/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      321 2022-11-21 08:51:54.000000 mfu-0.0.5/README.md
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/mfu/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)       61 2022-11-21 08:51:54.000000 mfu-0.0.5/mfu/__main__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      194 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/main.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/mfu/scripts/
--rw-rw-r--   0 michael   (1000) michael   (1000)        0 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/scripts/__init__.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3651 2022-11-21 08:51:54.000000 mfu-0.0.5/mfu/scripts/doctor.py
--rw-rw-r--   0 michael   (1000) michael   (1000)     3693 2022-11-21 08:51:54.000000 mfu-0.0.5/mfu/scripts/sync.py
--rw-rw-r--   0 michael   (1000) michael   (1000)      756 2022-11-21 04:24:21.000000 mfu-0.0.5/mfu/utils.py
-drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2022-11-21 09:19:56.104891 mfu-0.0.5/mfu.egg-info/
--rw-rw-r--   0 michael   (1000) michael   (1000)      514 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/PKG-INFO
--rw-rw-r--   0 michael   (1000) michael   (1000)      320 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/SOURCES.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        1 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/dependency_links.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       37 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/entry_points.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)       66 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/requires.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)        4 2022-11-21 09:19:56.000000 mfu-0.0.5/mfu.egg-info/top_level.txt
--rw-rw-r--   0 michael   (1000) michael   (1000)      460 2022-11-21 09:15:37.000000 mfu-0.0.5/pyproject.toml
--rw-rw-r--   0 michael   (1000) michael   (1000)       38 2022-11-21 09:19:56.104891 mfu-0.0.5/setup.cfg
--rw-rw-r--   0 michael   (1000) michael   (1000)       68 2022-11-21 09:07:09.000000 mfu-0.0.5/setup.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-05-17 08:44:27.983802 mfu-0.0.6/PKG-INFO
+-rw-rw-r--   0 michael   (1000) michael   (1000)      444 2024-05-17 08:44:02.000000 mfu-0.0.6/README.md
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:51.000000 mfu-0.0.6/mfu/__init__.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)       61 2023-03-22 08:55:56.000000 mfu-0.0.6/mfu/__main__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      324 2024-05-17 08:42:36.000000 mfu-0.0.6/mfu/main.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu/scripts/
+-rw-rw-r--   0 michael   (1000) michael   (1000)        0 2023-03-22 08:55:45.000000 mfu-0.0.6/mfu/scripts/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4159 2024-04-12 11:30:45.000000 mfu-0.0.6/mfu/scripts/cluster.py
+-rw-rw-r--   0 michael   (1000) michael   (1000)     1199 2023-03-22 09:33:27.000000 mfu-0.0.6/mfu/scripts/config.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3748 2023-03-22 09:16:00.000000 mfu-0.0.6/mfu/scripts/doctor.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3715 2022-11-23 11:16:20.000000 mfu-0.0.6/mfu/scripts/sync.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu/utils/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        0 2022-11-23 11:12:20.000000 mfu-0.0.6/mfu/utils/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     2841 2022-11-23 11:15:13.000000 mfu-0.0.6/mfu/utils/forcelink.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3176 2023-06-20 13:21:08.000000 mfu-0.0.6/mfu/utils/general.py
+drwxrwxr-x   0 michael   (1000) michael   (1000)        0 2024-05-17 08:44:27.983802 mfu-0.0.6/mfu.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/PKG-INFO
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      418 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/SOURCES.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        1 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/dependency_links.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       37 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/entry_points.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       83 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/requires.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)        4 2024-05-17 08:44:27.000000 mfu-0.0.6/mfu.egg-info/top_level.txt
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      486 2024-05-17 08:43:25.000000 mfu-0.0.6/pyproject.toml
+-rw-rw-r--   0 michael   (1000) michael   (1000)       38 2024-05-17 08:44:27.983802 mfu-0.0.6/setup.cfg
+-rw-rw-r--   0 michael   (1000) michael   (1000)       68 2023-03-22 08:56:38.000000 mfu-0.0.6/setup.py
```

### Comparing `mfu-0.0.5/mfu/scripts/doctor.py` & `mfu-0.0.6/mfu/scripts/doctor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
+import platform
+import shutil
 from pathlib import Path
 
 import click
-import platform
-import shutil
 
-from mfu.utils import run_command
+from mfu.utils.general import run_command
 
 
 @click.command(help="Check the status of the host machine to run all commands",
                short_help="Check the status of the host machine to run all commands")
 @click.option('--fix', is_flag=True, help='Try to fix issues on the machine detected by doctor.')
 def doctor(fix):
     click.echo(f"Starting the doctor")
@@ -19,15 +19,16 @@
     click.echo("Checking for a package manager")
     if os_system == "Darwin":
         if shutil.which("brew") is not None:
             click.echo(click.style('You\'ve got brew installed. Good job.', fg='green'))
         else:
             click.echo(click.style('You\'re gonna have some issues.', fg='red'))
             if fix:
-                command = ['/bin/bash', '-c', '"$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"']
+                command = ['/bin/bash', '-c',
+                           '"$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"']
                 run_command(command)
             else:
                 click.echo('Run with --fix to install it here')
     elif os_system == "Windows":
         if shutil.which("choco") is not None:
             click.echo(click.style('You\'ve got choco installed. Good job.', fg='green'))
         else:
@@ -48,20 +49,23 @@
         else:
             if fix:
                 if os_system == "Darwin":
                     command = ['brew', 'install', 'kubectl']
                     click.echo(click.style('Attempting to install kubectl.', fg='red'))
                     run_command(command)
                 elif os_system == "Linux":
-                    command = ['curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl" > /usr/local/bin/kubectl']
+                    command = [
+                        'curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl" > /usr/local/bin/kubectl']
                     click.echo(click.style('Attempting to install kubectl.', fg='red'))
                     run_command(command)
             else:
                 click.echo('Run with --fix to install it here')
 
     click.echo("Checking if kubeconfig file is on the machine")
     if os.path.isfile(f'{Path.home()}/.kube/config'):
         click.echo(click.style('You\'ve got a kubeconfig file. Good Job.', fg='green'))
-        click.echo(click.style('It doesn\'t mean you\'re out of the woods though. It is possible for the config to be broken', fg='green'))
+        click.echo(
+            click.style('It doesn\'t mean you\'re out of the woods though. It is possible for the config to be broken',
+                        fg='green'))
     else:
         click.echo(click.style('It doesn\'t look like you have a kubeconfig file.', fg='red'))
         click.echo(click.style('You should download one from https://rancher.acumensoft.net/', fg='red'))
```

### Comparing `mfu-0.0.5/mfu/scripts/sync.py` & `mfu-0.0.6/mfu/scripts/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,37 +5,38 @@
 
 import click
 from git import Repo
 from kubernetes import client, config
 from watchdog.events import FileSystemEventHandler
 from watchdog.observers import Observer
 
-from mfu.utils import run_command
+from mfu.utils.general import run_command
 
 
 @click.group(help="Command group to sync files to kubernetes pods",
-              short_help="Command group to sync files to kubernetes pods")
+             short_help="Command group to sync files to kubernetes pods")
 def sync():
     pass
 
 
 @sync.command(help="Run as a background process and write detected file changes to the forcelink-webapp pod",
               short_help="Run as a background process and write detected file changes to the forcelink-webapp pod")
 @click.option('--path', default=os.getcwd(), help='The path on which to listen for file changes')
 @click.option('--context', default='core', help='Kubernetes context of the cluster that the pod is running in')
-@click.option('--podlabel', default='app.kubernetes.io/instance=webapp-forcelink', help='Label on which to match the running forcelink pod')
+@click.option('--podlabel', default='app.kubernetes.io/instance=webapp-forcelink',
+              help='Label on which to match the running forcelink pod')
 @click.option('--podroot', default='/usr/local/tomcat/webapps/forcelink',
               help='The path within the pod that maps to the local path root.')
 def listen(path, context, podlabel, podroot):
     config.load_kube_config(context=context)
     v1 = client.CoreV1Api()
 
     class Handler(FileSystemEventHandler):
         def __init__(self, project_path, branch):
-            self.project_path = project_path.replace("\\", "/") # Remove windows mapping for pod
+            self.project_path = project_path.replace("\\", "/")  # Remove windows mapping for pod
             self.branch = branch.lower()
             self.system = platform.system()
 
         def on_modified(self, event):
             if "WebContent" in event.src_path and "~" not in event.src_path and not event.is_directory:
                 pods = v1.list_namespaced_pod(f"forcelink-{self.branch}", label_selector=podlabel).items
                 if pods:
```

