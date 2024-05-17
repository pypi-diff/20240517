# Comparing `tmp/lambkid-0.2.1.tar.gz` & `tmp/lambkid-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambkid-0.2.1.tar", last modified: Wed May 15 08:33:56 2024, max compression
+gzip compressed data, was "lambkid-0.2.2.tar", last modified: Fri May 17 01:57:05 2024, max compression
```

## Comparing `lambkid-0.2.1.tar` & `lambkid-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.271175 lambkid-0.2.1/
--rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2094 2024-05-15 08:33:56.269184 lambkid-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.107612 lambkid-0.2.1/docs/
--rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.1/docs/cli.md
--rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.1/docs/csv.md
--rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.1/docs/install.md
--rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.1/docs/log.md
--rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.1/docs/sshclient.md
--rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.1/docs/utils.md
-drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.110604 lambkid-0.2.1/lambkid/
--rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.1/lambkid/__init__.py
--rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.1/lambkid/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.202358 lambkid-0.2.1/lambkid/libs/
--rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.1/lambkid/libs/__init__.py
--rw-rw-rw-   0        0        0     1514 2024-04-29 07:44:19.000000 lambkid-0.2.1/lambkid/libs/log.py
--rw-rw-rw-   0        0        0      825 2024-04-08 02:45:19.000000 lambkid-0.2.1/lambkid/libs/minio_client.py
--rw-rw-rw-   0        0        0     7346 2024-05-15 08:32:56.000000 lambkid-0.2.1/lambkid/libs/ssh.py
--rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.1/lambkid/libs/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:33:56.240257 lambkid-0.2.1/lambkid.egg-info/
--rw-rw-rw-   0        0        0     2094 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 08:33:55.000000 lambkid-0.2.1/lambkid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 08:33:56.271175 lambkid-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1834 2024-05-15 08:32:56.000000 lambkid-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 01:57:05.993481 lambkid-0.2.2/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 01:13:02.000000 lambkid-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       27 2024-04-01 08:22:25.000000 lambkid-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2094 2024-05-17 01:57:05.991487 lambkid-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      717 2024-04-24 02:44:24.000000 lambkid-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 01:57:05.941621 lambkid-0.2.2/docs/
+-rw-rw-rw-   0        0        0      371 2024-04-08 03:30:43.000000 lambkid-0.2.2/docs/cli.md
+-rw-rw-rw-   0        0        0      221 2024-04-24 02:42:57.000000 lambkid-0.2.2/docs/csv.md
+-rw-rw-rw-   0        0        0       54 2024-03-31 06:58:42.000000 lambkid-0.2.2/docs/install.md
+-rw-rw-rw-   0        0        0      778 2024-04-07 15:20:10.000000 lambkid-0.2.2/docs/log.md
+-rw-rw-rw-   0        0        0     1878 2024-04-01 07:39:19.000000 lambkid-0.2.2/docs/sshclient.md
+-rw-rw-rw-   0        0        0       36 2024-04-25 02:05:46.000000 lambkid-0.2.2/docs/utils.md
+drwxrwxrwx   0        0        0        0 2024-05-17 01:57:05.943643 lambkid-0.2.2/lambkid/
+-rw-rw-rw-   0        0        0      188 2024-04-25 02:53:27.000000 lambkid-0.2.2/lambkid/__init__.py
+-rw-rw-rw-   0        0        0      969 2024-04-08 15:55:58.000000 lambkid-0.2.2/lambkid/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-17 01:57:05.977524 lambkid-0.2.2/lambkid/libs/
+-rw-rw-rw-   0        0        0        0 2024-03-31 06:59:08.000000 lambkid-0.2.2/lambkid/libs/__init__.py
+-rw-rw-rw-   0        0        0     1514 2024-04-29 07:44:19.000000 lambkid-0.2.2/lambkid/libs/log.py
+-rw-rw-rw-   0        0        0     1793 2024-05-17 01:55:15.000000 lambkid-0.2.2/lambkid/libs/minio_client.py
+-rw-rw-rw-   0        0        0     7346 2024-05-15 08:32:56.000000 lambkid-0.2.2/lambkid/libs/ssh.py
+-rw-rw-rw-   0        0        0     2259 2024-04-28 05:47:19.000000 lambkid-0.2.2/lambkid/libs/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 01:57:05.990489 lambkid-0.2.2/lambkid.egg-info/
+-rw-rw-rw-   0        0        0     2094 2024-05-17 01:57:05.000000 lambkid-0.2.2/lambkid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-05-17 01:57:05.000000 lambkid-0.2.2/lambkid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 01:57:05.000000 lambkid-0.2.2/lambkid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-17 01:57:05.000000 lambkid-0.2.2/lambkid.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-05-17 01:57:05.000000 lambkid-0.2.2/lambkid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 01:57:05.000000 lambkid-0.2.2/lambkid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 01:57:05.993481 lambkid-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1834 2024-05-17 01:56:26.000000 lambkid-0.2.2/setup.py
```

### Comparing `lambkid-0.2.1/LICENSE` & `lambkid-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/PKG-INFO` & `lambkid-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.1
+Version: 0.2.2
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.1/README.md` & `lambkid-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/docs/log.md` & `lambkid-0.2.2/docs/log.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/docs/sshclient.md` & `lambkid-0.2.2/docs/sshclient.md`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/lambkid/cli.py` & `lambkid-0.2.2/lambkid/cli.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/lambkid/libs/log.py` & `lambkid-0.2.2/lambkid/libs/log.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/lambkid/libs/ssh.py` & `lambkid-0.2.2/lambkid/libs/ssh.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/lambkid/libs/utils.py` & `lambkid-0.2.2/lambkid/libs/utils.py`

 * *Files identical despite different names*

### Comparing `lambkid-0.2.1/lambkid.egg-info/PKG-INFO` & `lambkid-0.2.2/lambkid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambkid
-Version: 0.2.1
+Version: 0.2.2
 Summary: lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.
 Home-page: https://github.com/redrose2100/lambkid
 Author: redrose2100
 Author-email: hitredrose@163.com
 Maintainer: redrose2100
 Maintainer-email: hitredrose@163.com
 License: MIT
```

### Comparing `lambkid-0.2.1/setup.py` & `lambkid-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         long_desc=f.read()
 except:
     long_desc=""
 
 
 setup(
     name="lambkid",
-    version="0.2.1",
+    version="0.2.2",
     description="lambkid is an advance abstract from some common pyton lib, it aim to make you write python more easily and more fewer code.",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     author="redrose2100",
     author_email="hitredrose@163.com",
     maintainer="redrose2100",
     maintainer_email="hitredrose@163.com",
```

