# Comparing `tmp/ai_project_setup-0.2.0.tar.gz` & `tmp/ai_project_setup-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_project_setup-0.2.0.tar", last modified: Fri May 17 01:12:46 2024, max compression
+gzip compressed data, was "ai_project_setup-0.2.1.tar", last modified: Fri May 17 01:20:19 2024, max compression
```

## Comparing `ai_project_setup-0.2.0.tar` & `ai_project_setup-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.940650 ai_project_setup-0.2.0/
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-17 01:12:46.939650 ai_project_setup-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 00:50:04.000000 ai_project_setup-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.938650 ai_project_setup-0.2.0/ai_project_setup.egg-info/
--rw-r--r--   0 root         (0) root         (0)      610 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.939650 ai_project_setup-0.2.0/git_clone/
--rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.0/git_clone/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9249 2024-05-17 00:53:07.000000 ai_project_setup-0.2.0/git_clone/git_clone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.939650 ai_project_setup-0.2.0/project_setup/
--rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.0/project_setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.0/project_setup/project_setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 01:12:46.940650 ai_project_setup-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      894 2024-05-17 01:11:15.000000 ai_project_setup-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:20:19.487548 ai_project_setup-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-17 01:20:19.487548 ai_project_setup-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3159 2024-05-17 01:19:44.000000 ai_project_setup-0.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:20:19.486548 ai_project_setup-0.2.1/ai_project_setup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-17 01:20:19.000000 ai_project_setup-0.2.1/ai_project_setup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 01:20:19.000000 ai_project_setup-0.2.1/ai_project_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 01:20:19.000000 ai_project_setup-0.2.1/ai_project_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 01:20:19.000000 ai_project_setup-0.2.1/ai_project_setup.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:20:19.486548 ai_project_setup-0.2.1/git_clone/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.1/git_clone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9249 2024-05-17 00:53:07.000000 ai_project_setup-0.2.1/git_clone/git_clone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:20:19.486548 ai_project_setup-0.2.1/project_setup/
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.1/project_setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.1/project_setup/project_setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 01:20:19.487548 ai_project_setup-0.2.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-17 01:20:08.000000 ai_project_setup-0.2.1/setup.py
```

### Comparing `ai_project_setup-0.2.0/PKG-INFO` & `ai_project_setup-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
 Name: ai_project_setup
-Version: 0.2.0
+Version: 0.2.1
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
```

### Comparing `ai_project_setup-0.2.0/ai_project_setup.egg-info/PKG-INFO` & `ai_project_setup-0.2.1/ai_project_setup.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Metadata-Version: 2.1
 Name: ai-project-setup
-Version: 0.2.0
+Version: 0.2.1
 Summary: A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.
 Author: Patrick Ogbuitepu
 Author-email: pat2echo@gmail.com
 Keywords: AI,utility package,project structure,Git integration,Google Colab integration,collaborative projects,ease of use,streamlined workflow,automation,project management,project,setup,structure,ai,artificial intelligence,research,data science,machine learning
```

### Comparing `ai_project_setup-0.2.0/git_clone/git_clone.py` & `ai_project_setup-0.2.1/git_clone/git_clone.py`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.0/project_setup/project_setup.py` & `ai_project_setup-0.2.1/project_setup/project_setup.py`

 * *Files identical despite different names*

### Comparing `ai_project_setup-0.2.0/setup.py` & `ai_project_setup-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ai_project_setup',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     description='A versatile utility package designed to streamline the setup of AI project structures while seamlessly integrating with Git repositories and Google Colab, simplifying the process of building collaborative AI projects.',
     author='Patrick Ogbuitepu',
     author_email='pat2echo@gmail.com',
     keywords=['AI', 'utility package', 'project structure', 'Git integration', 'Google Colab integration', 'collaborative projects', 'ease of use', 'streamlined workflow', 'automation', 'project management', 'project', 'setup', 'structure', 'ai', 'artificial intelligence', 'research', 'data science', 'machine learning'],
     install_requires=[
         # Any dependencies the package might have, e.g.,
```
