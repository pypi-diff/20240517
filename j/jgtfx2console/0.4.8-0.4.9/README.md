# Comparing `tmp/jgtfx2console-0.4.8.tar.gz` & `tmp/jgtfx2console-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgtfx2console-0.4.8.tar", last modified: Sun Apr 14 12:09:50 2024, max compression
+gzip compressed data, was "jgtfx2console-0.4.9.tar", last modified: Sun Apr 14 12:14:58 2024, max compression
```

## Comparing `jgtfx2console-0.4.8.tar` & `jgtfx2console-0.4.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:09:50.359333 jgtfx2console-0.4.8/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-03-16 22:23:35.000000 jgtfx2console-0.4.8/LICENSE
--rw-r--r--   0 jgi       (1000) jgi       (1000)     2224 2024-04-14 12:09:50.359333 jgtfx2console-0.4.8/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      696 2024-03-16 22:23:35.000000 jgtfx2console-0.4.8/README.md
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      205 2024-03-16 22:23:35.000000 jgtfx2console-0.4.8/README.rst
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:09:50.355333 jgtfx2console-0.4.8/jgtfx2console/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1610 2024-04-14 12:09:48.000000 jgtfx2console-0.4.8/jgtfx2console/__init__.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:09:50.359333 jgtfx2console-0.4.8/jgtfx2console/forexconnect/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1649 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/EachRowListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    25755 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/ForexConnect.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9925 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/LiveHistory.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8003 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/ResponseListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4783 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/SessionStatusListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5900 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/TableListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3121 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/TableManagerListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2125 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    19128 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/common.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      931 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/errors.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      437 2024-01-14 01:04:03.000000 jgtfx2console-0.4.8/jgtfx2console/forexconnect/x-pyd.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     7504 2024-04-14 11:54:49.000000 jgtfx2console-0.4.8/jgtfx2console/fxcli2console.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:09:50.355333 jgtfx2console-0.4.8/jgtfx2console.egg-info/
--rw-r--r--   0 jgi       (1000) jgi       (1000)     2224 2024-04-14 12:09:50.000000 jgtfx2console-0.4.8/jgtfx2console.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      817 2024-04-14 12:09:50.000000 jgtfx2console-0.4.8/jgtfx2console.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-14 12:09:50.000000 jgtfx2console-0.4.8/jgtfx2console.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       67 2024-04-14 12:09:50.000000 jgtfx2console-0.4.8/jgtfx2console.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      328 2024-04-14 12:09:50.000000 jgtfx2console-0.4.8/jgtfx2console.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-14 12:09:50.000000 jgtfx2console-0.4.8/jgtfx2console.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      693 2024-04-14 12:09:48.000000 jgtfx2console-0.4.8/pyproject.toml
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      103 2024-04-14 12:09:50.359333 jgtfx2console-0.4.8/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1814 2024-04-14 11:57:45.000000 jgtfx2console-0.4.8/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:14:58.485747 jgtfx2console-0.4.9/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-03-16 22:23:35.000000 jgtfx2console-0.4.9/LICENSE
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2224 2024-04-14 12:14:58.485747 jgtfx2console-0.4.9/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      696 2024-03-16 22:23:35.000000 jgtfx2console-0.4.9/README.md
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      205 2024-03-16 22:23:35.000000 jgtfx2console-0.4.9/README.rst
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:14:58.481747 jgtfx2console-0.4.9/jgtfx2console/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1610 2024-04-14 12:14:56.000000 jgtfx2console-0.4.9/jgtfx2console/__init__.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:14:58.485747 jgtfx2console-0.4.9/jgtfx2console/forexconnect/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1649 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/EachRowListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    25755 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/ForexConnect.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9925 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/LiveHistory.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8003 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/ResponseListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4783 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/SessionStatusListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5900 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/TableListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3121 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/TableManagerListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2125 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    19128 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/common.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      931 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/errors.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      437 2024-01-14 01:04:03.000000 jgtfx2console-0.4.9/jgtfx2console/forexconnect/x-pyd.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     7425 2024-04-14 12:14:47.000000 jgtfx2console-0.4.9/jgtfx2console/fxcli2console.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-04-14 12:14:58.481747 jgtfx2console-0.4.9/jgtfx2console.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2224 2024-04-14 12:14:58.000000 jgtfx2console-0.4.9/jgtfx2console.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      817 2024-04-14 12:14:58.000000 jgtfx2console-0.4.9/jgtfx2console.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-04-14 12:14:58.000000 jgtfx2console-0.4.9/jgtfx2console.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       67 2024-04-14 12:14:58.000000 jgtfx2console-0.4.9/jgtfx2console.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      328 2024-04-14 12:14:58.000000 jgtfx2console-0.4.9/jgtfx2console.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       14 2024-04-14 12:14:58.000000 jgtfx2console-0.4.9/jgtfx2console.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      693 2024-04-14 12:14:56.000000 jgtfx2console-0.4.9/pyproject.toml
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      103 2024-04-14 12:14:58.485747 jgtfx2console-0.4.9/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1814 2024-04-14 11:57:45.000000 jgtfx2console-0.4.9/setup.py
```

### Comparing `jgtfx2console-0.4.8/LICENSE` & `jgtfx2console-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/PKG-INFO` & `jgtfx2console-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtfx2console
-Version: 0.4.8
+Version: 0.4.9
 Summary: PDS Services
 Home-page: https://github.com/jgwill/jgtfx2console
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtfx2console
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtfx2console/issues
```

### Comparing `jgtfx2console-0.4.8/README.md` & `jgtfx2console-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/__init__.py` & `jgtfx2console-0.4.9/jgtfx2console/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
 import warnings
 
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=RuntimeWarning, module="importlib._bootstrap")
     # your code here
 
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
```

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/EachRowListener.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/EachRowListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/ForexConnect.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/ForexConnect.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/LiveHistory.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/LiveHistory.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/ResponseListener.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/ResponseListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/SessionStatusListener.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/SessionStatusListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/TableListener.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/TableListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/TableManagerListener.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/TableManagerListener.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/__init__.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/common.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/common.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/forexconnect/errors.py` & `jgtfx2console-0.4.9/jgtfx2console/forexconnect/errors.py`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/jgtfx2console/fxcli2console.py` & `jgtfx2console-0.4.9/jgtfx2console/fxcli2console.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     str_user_id = user_id#args.l
     str_password = password#args.p
     str_url = url#args.u
     
     keep_bid_ask = args.keepbidask
     #env variable bypass if env exist JGT_KEEP_BID_ASK=1, keep_bid_ask = True
     if os.getenv("JGT_KEEP_BID_ASK","0") == "1":
-        print("KEEP BID ASK ENV VAR ON (bypassing the --keepbidask argument)")
         keep_bid_ask = True
         
     using_tlid = False
     if args.tlidrange is not None:
       using_tlid= True
       tlid_range = args.tlidrange
       #print(tlid_range)
```

### Comparing `jgtfx2console-0.4.8/jgtfx2console.egg-info/PKG-INFO` & `jgtfx2console-0.4.9/jgtfx2console.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtfx2console
-Version: 0.4.8
+Version: 0.4.9
 Summary: PDS Services
 Home-page: https://github.com/jgwill/jgtfx2console
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtfx2console
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtfx2console/issues
```

### Comparing `jgtfx2console-0.4.8/jgtfx2console.egg-info/SOURCES.txt` & `jgtfx2console-0.4.9/jgtfx2console.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jgtfx2console-0.4.8/pyproject.toml` & `jgtfx2console-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jgtfx2console"
-version = "0.4.8"
+version = "0.4.9"
 authors = [
   { name="Guillaume Isabelle", email="jgi@jgwill.com" },
 ]
 
 description = "PDS Services"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `jgtfx2console-0.4.8/setup.py` & `jgtfx2console-0.4.9/setup.py`

 * *Files identical despite different names*

