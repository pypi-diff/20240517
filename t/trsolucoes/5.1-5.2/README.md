# Comparing `tmp/trsolucoes-5.1.tar.gz` & `tmp/trsolucoes-5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trsolucoes-5.1.tar", last modified: Thu May 16 23:33:53 2024, max compression
+gzip compressed data, was "trsolucoes-5.2.tar", last modified: Thu May 16 23:45:23 2024, max compression
```

## Comparing `trsolucoes-5.1.tar` & `trsolucoes-5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 23:33:53.859453 trsolucoes-5.1/
--rw-rw-rw-   0        0        0      341 2024-05-16 23:33:53.859453 trsolucoes-5.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-16 23:33:53.860454 trsolucoes-5.1/setup.cfg
--rw-rw-rw-   0        0        0      701 2024-05-16 23:32:43.000000 trsolucoes-5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 23:33:53.858454 trsolucoes-5.1/trsolucoes.egg-info/
--rw-rw-rw-   0        0        0      341 2024-05-16 23:33:53.000000 trsolucoes-5.1/trsolucoes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-05-16 23:33:53.000000 trsolucoes-5.1/trsolucoes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 23:33:53.000000 trsolucoes-5.1/trsolucoes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-16 23:33:53.000000 trsolucoes-5.1/trsolucoes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 23:33:53.000000 trsolucoes-5.1/trsolucoes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 23:45:23.029460 trsolucoes-5.2/
+-rw-rw-rw-   0        0        0      341 2024-05-16 23:45:23.028953 trsolucoes-5.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-16 23:45:23.029460 trsolucoes-5.2/setup.cfg
+-rw-rw-rw-   0        0        0      701 2024-05-16 23:45:13.000000 trsolucoes-5.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 23:45:23.027953 trsolucoes-5.2/trsolucoes.egg-info/
+-rw-rw-rw-   0        0        0      341 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 23:45:22.000000 trsolucoes-5.2/trsolucoes.egg-info/top_level.txt
```

### Comparing `trsolucoes-5.1/setup.py` & `trsolucoes-5.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='trsolucoes',
-    version='5.1',
+    version='5.2',
     packages=find_packages(),
     install_requires=[
         'selenium',
     ],
     author='Tainan Ramos',
     author_email='tainan@trsolucoes.com.br',
     description='Uma biblioteca de auxílio para Selenium',
```

