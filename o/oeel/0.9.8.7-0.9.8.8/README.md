# Comparing `tmp/oeel-0.9.8.7.tar.gz` & `tmp/oeel-0.9.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oeel-0.9.8.7.tar", last modified: Wed May 15 08:03:34 2024, max compression
+gzip compressed data, was "oeel-0.9.8.8.tar", last modified: Fri May 17 05:33:51 2024, max compression
```

## Comparing `oeel-0.9.8.7.tar` & `oeel-0.9.8.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:34.672004 oeel-0.9.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-15 08:03:28.000000 oeel-0.9.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 08:03:34.672004 oeel-0.9.8.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:34.672004 oeel-0.9.8.7/oeel/
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/EE_node_server.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/external.py
--rw-r--r--   0 runner    (1001) docker     (127)    10877 2024-05-15 08:03:28.000000 oeel-0.9.8.7/oeel/oeel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:03:34.672004 oeel-0.9.8.7/oeel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 08:03:34.000000 oeel-0.9.8.7/oeel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:03:34.672004 oeel-0.9.8.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-15 08:03:28.000000 oeel-0.9.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:33:51.378514 oeel-0.9.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35146 2024-05-17 05:33:40.000000 oeel-0.9.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-17 05:33:51.378514 oeel-0.9.8.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:33:51.378514 oeel-0.9.8.8/oeel/
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-17 05:33:40.000000 oeel-0.9.8.8/oeel/EE_node_server.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:33:40.000000 oeel-0.9.8.8/oeel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-17 05:33:40.000000 oeel-0.9.8.8/oeel/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-05-17 05:33:40.000000 oeel-0.9.8.8/oeel/oeel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:33:51.378514 oeel-0.9.8.8/oeel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-17 05:33:51.000000 oeel-0.9.8.8/oeel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-17 05:33:51.000000 oeel-0.9.8.8/oeel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:33:51.000000 oeel-0.9.8.8/oeel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 05:33:51.000000 oeel-0.9.8.8/oeel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 05:33:51.000000 oeel-0.9.8.8/oeel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 05:33:51.378514 oeel-0.9.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-17 05:33:40.000000 oeel-0.9.8.8/setup.py
```

### Comparing `oeel-0.9.8.7/LICENSE` & `oeel-0.9.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `oeel-0.9.8.7/PKG-INFO` & `oeel-0.9.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oeel
-Version: 0.9.8.7
+Version: 0.9.8.8
 Summary: The Open Earth Engine Library Python interface
 Home-page: https://www.open-geocomputing.org/OpenEarthEngineLibrary/
 Author: Mathieu Gravey
 Author-email: research@mgravey.com
 License: GPLv3
 Keywords: Earth Engine,OEEL,Open Earth Engine Library
 Platform: UNKNOWN
```

### Comparing `oeel-0.9.8.7/oeel/EE_node_server.js` & `oeel-0.9.8.8/oeel/EE_node_server.js`

 * *Files identical despite different names*

### Comparing `oeel-0.9.8.7/oeel/external.py` & `oeel-0.9.8.8/oeel/external.py`

 * *Files identical despite different names*

### Comparing `oeel-0.9.8.7/oeel/oeel.py` & `oeel-0.9.8.8/oeel/oeel.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,19 +112,14 @@
 		pass
 	class oeelInitFailed(Exception):
 		pass
 	class oeelMissingRequireFile(Exception):
 		pass
 
 	def __init__(self):
-		# if(not ee.data._initialized and IN_COLAB):
-		# 	try:
-		# 		colab.AuthAndInitilize();
-		# 	except Exception as e:
-		# 		pass
 		self.nodeSocket=None;
 		self.loadOEELFunctions()
 		self.init();
 
 	def manageNodeRequest(self,message):
 		if(message['function']=='print'):
 			print(*(message['payload']))
@@ -291,14 +286,12 @@
 
 
 oeelManadger=oeelClass();
 oeelManadger.oeelLibInterface.init=oeelManadger.init;
 oeelManadger.oeelLibInterface.requireJS=oeelManadger.requireJS;
 oeelManadger.oeelLibInterface.setMap=oeelManadger.setMap;
 oeel=oeelManadger.oeelLibInterface
-oeel.colab=oeelParentDirectory({})
-oeel.colab.AuthAndInitilize=colab.AuthAndInitilize;
 
 for name in dir(oeel) :
 	globals()[name]=oeel[name];
 
 __all__=dir(oeel)
```

### Comparing `oeel-0.9.8.7/oeel.egg-info/PKG-INFO` & `oeel-0.9.8.8/oeel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oeel
-Version: 0.9.8.7
+Version: 0.9.8.8
 Summary: The Open Earth Engine Library Python interface
 Home-page: https://www.open-geocomputing.org/OpenEarthEngineLibrary/
 Author: Mathieu Gravey
 Author-email: research@mgravey.com
 License: GPLv3
 Keywords: Earth Engine,OEEL,Open Earth Engine Library
 Platform: UNKNOWN
```

### Comparing `oeel-0.9.8.7/setup.py` & `oeel-0.9.8.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='oeel',
-    version='0.9.8.7',
+    version='0.9.8.8',
     author='Mathieu Gravey',
     author_email='research@mgravey.com',
     url='https://www.open-geocomputing.org/OpenEarthEngineLibrary/',
     description='The Open Earth Engine Library Python interface',
     long_description='Python interface for the OpenEarthEngineLibrary and JS Earth Engine code.',
     classifiers=['Development Status :: 3 - Alpha','License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)','Programming Language :: Python :: 3','Programming Language :: JavaScript','Topic :: Scientific/Engineering :: GIS'],
     packages=['oeel'],
```

