# Comparing `tmp/ai_project_setup-0.1.0.tar.gz` & `tmp/ai_project_setup-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_project_setup-0.1.0.tar", last modified: Sat Apr 27 15:28:30 2024, max compression
+gzip compressed data, was "ai_project_setup-0.2.0.tar", last modified: Fri May 17 01:12:46 2024, max compression
```

## Comparing `ai_project_setup-0.1.0.tar` & `ai_project_setup-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:28:30.032402 ai_project_setup-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      284 2024-04-27 15:28:30.031402 ai_project_setup-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-27 15:22:16.000000 ai_project_setup-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:28:30.031402 ai_project_setup-0.1.0/ai_project_setup.egg-info/
--rw-r--r--   0 root         (0) root         (0)      284 2024-04-27 15:28:29.000000 ai_project_setup-0.1.0/ai_project_setup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-27 15:28:29.000000 ai_project_setup-0.1.0/ai_project_setup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 15:28:29.000000 ai_project_setup-0.1.0/ai_project_setup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 15:28:29.000000 ai_project_setup-0.1.0/ai_project_setup.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 15:28:30.031402 ai_project_setup-0.1.0/project_setup/
--rw-r--r--   0 root         (0) root         (0)       41 2024-04-27 15:22:16.000000 ai_project_setup-0.1.0/project_setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5173 2024-04-27 15:22:16.000000 ai_project_setup-0.1.0/project_setup/project_setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 15:28:30.032402 ai_project_setup-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      538 2024-04-27 15:22:16.000000 ai_project_setup-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.940650 ai_project_setup-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-17 01:12:46.939650 ai_project_setup-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-17 00:50:04.000000 ai_project_setup-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.938650 ai_project_setup-0.2.0/ai_project_setup.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      610 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 01:12:46.000000 ai_project_setup-0.2.0/ai_project_setup.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.939650 ai_project_setup-0.2.0/git_clone/
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-17 00:52:56.000000 ai_project_setup-0.2.0/git_clone/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9249 2024-05-17 00:53:07.000000 ai_project_setup-0.2.0/git_clone/git_clone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 01:12:46.939650 ai_project_setup-0.2.0/project_setup/
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 00:50:04.000000 ai_project_setup-0.2.0/project_setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-17 00:50:04.000000 ai_project_setup-0.2.0/project_setup/project_setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 01:12:46.940650 ai_project_setup-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      894 2024-05-17 01:11:15.000000 ai_project_setup-0.2.0/setup.py
```

### Comparing `ai_project_setup-0.1.0/project_setup/project_setup.py` & `ai_project_setup-0.2.0/project_setup/project_setup.py`

 * *Files identical despite different names*

