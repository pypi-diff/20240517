# Comparing `tmp/pyvelop-2024.5.1.tar.gz` & `tmp/pyvelop-2024.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvelop-2024.5.1.tar", last modified: Sun May  5 19:27:45 2024, max compression
+gzip compressed data, was "pyvelop-2024.5.2.tar", last modified: Thu May 16 19:20:11 2024, max compression
```

## Comparing `pyvelop-2024.5.1.tar` & `pyvelop-2024.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:27:45.005392 pyvelop-2024.5.1/
--rw-rw-rw-   0        0        0     1720 2024-05-05 19:27:45.004384 pyvelop-2024.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-05 19:27:44.999127 pyvelop-2024.5.1/pyvelop/
--rw-rw-rw-   0        0        0      716 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/__init__.py
--rw-rw-rw-   0        0        0    37881 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/__main__.py
--rw-rw-rw-   0        0        0     7204 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/base.py
--rw-rw-rw-   0        0        0      226 2024-05-05 19:12:50.000000 pyvelop-2024.5.1/pyvelop/const.py
--rw-rw-rw-   0        0        0      598 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/decorators.py
--rw-rw-rw-   0        0        0    12640 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/device.py
--rw-rw-rw-   0        0        0     3139 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/exceptions.py
--rw-rw-rw-   0        0        0    12421 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/jnap.py
--rw-rw-rw-   0        0        0      788 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/pyvelop/logger.py
--rw-rw-rw-   0        0        0    63596 2024-05-05 19:12:36.000000 pyvelop-2024.5.1/pyvelop/mesh.py
--rw-rw-rw-   0        0        0     6258 2024-05-05 19:12:36.000000 pyvelop-2024.5.1/pyvelop/node.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:27:45.003027 pyvelop-2024.5.1/pyvelop.egg-info/
--rw-rw-rw-   0        0        0     1720 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-05 19:27:44.000000 pyvelop-2024.5.1/pyvelop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 19:27:45.005392 pyvelop-2024.5.1/setup.cfg
--rw-rw-rw-   0        0        0      738 2024-05-05 18:37:29.000000 pyvelop-2024.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:20:11.497378 pyvelop-2024.5.2/
+-rw-rw-rw-   0        0        0     1720 2024-05-16 19:20:11.496199 pyvelop-2024.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-16 19:20:11.491991 pyvelop-2024.5.2/pyvelop/
+-rw-rw-rw-   0        0        0      716 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/pyvelop/__init__.py
+-rw-rw-rw-   0        0        0    37881 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/pyvelop/__main__.py
+-rw-rw-rw-   0        0        0     7233 2024-05-16 19:19:37.000000 pyvelop-2024.5.2/pyvelop/base.py
+-rw-rw-rw-   0        0        0      264 2024-05-16 19:19:37.000000 pyvelop-2024.5.2/pyvelop/const.py
+-rw-rw-rw-   0        0        0      598 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/pyvelop/decorators.py
+-rw-rw-rw-   0        0        0    12640 2024-05-16 19:17:36.000000 pyvelop-2024.5.2/pyvelop/device.py
+-rw-rw-rw-   0        0        0     3139 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/pyvelop/exceptions.py
+-rw-rw-rw-   0        0        0    12421 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/pyvelop/jnap.py
+-rw-rw-rw-   0        0        0      788 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/pyvelop/logger.py
+-rw-rw-rw-   0        0        0    63596 2024-05-05 19:12:36.000000 pyvelop-2024.5.2/pyvelop/mesh.py
+-rw-rw-rw-   0        0        0     6258 2024-05-05 19:12:36.000000 pyvelop-2024.5.2/pyvelop/node.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:20:11.496199 pyvelop-2024.5.2/pyvelop.egg-info/
+-rw-rw-rw-   0        0        0     1720 2024-05-16 19:20:11.000000 pyvelop-2024.5.2/pyvelop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-05-16 19:20:11.000000 pyvelop-2024.5.2/pyvelop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 19:20:11.000000 pyvelop-2024.5.2/pyvelop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 19:20:11.000000 pyvelop-2024.5.2/pyvelop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 19:20:11.000000 pyvelop-2024.5.2/pyvelop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 19:20:11.497378 pyvelop-2024.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      738 2024-05-05 18:37:29.000000 pyvelop-2024.5.2/setup.py
```

### Comparing `pyvelop-2024.5.1/PKG-INFO` & `pyvelop-2024.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

### Comparing `pyvelop-2024.5.1/README.rst` & `pyvelop-2024.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/__init__.py` & `pyvelop-2024.5.2/pyvelop/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/__main__.py` & `pyvelop-2024.5.2/pyvelop/__main__.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/base.py` & `pyvelop-2024.5.2/pyvelop/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # region #-- imports --#
 from __future__ import annotations
 
 from typing import Any, Dict, List
 
 from . import signal_strength_to_text
-
+from .const import DEF_EMPTY_NAME
 # endregion
 
 
 class MeshDevice:
     """A class that manages the common properties between the devices in the Velop mesh network."""
 
     def __init__(self, **kwargs) -> None:
@@ -125,22 +125,22 @@
     def name(self) -> str:
         """Get the name of the device.
 
         Decision on the name to use is as follows: -
 
             - User set name
             - Friendly name
-            - "Network Device" if no name is found
+            - DEF_EMPTY_NAME if no name is found
 
         :return: A string containing the name of the device
         """
         return (
             self._get_user_property(name="userDeviceName")
             or self._attribs.get("friendlyName")
-            or "Network Device"
+            or DEF_EMPTY_NAME
         )
 
     @property
     def network(self) -> List[dict]:
         """Get all the adapters the device has installed.
 
         :return: List of dictionaries containing details of adapaters.
```

### Comparing `pyvelop-2024.5.1/pyvelop/decorators.py` & `pyvelop-2024.5.2/pyvelop/decorators.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/device.py` & `pyvelop-2024.5.2/pyvelop/device.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/exceptions.py` & `pyvelop-2024.5.2/pyvelop/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/jnap.py` & `pyvelop-2024.5.2/pyvelop/jnap.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/logger.py` & `pyvelop-2024.5.2/pyvelop/logger.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/mesh.py` & `pyvelop-2024.5.2/pyvelop/mesh.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop/node.py` & `pyvelop-2024.5.2/pyvelop/node.py`

 * *Files identical despite different names*

### Comparing `pyvelop-2024.5.1/pyvelop.egg-info/PKG-INFO` & `pyvelop-2024.5.2/pyvelop.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvelop
-Version: 2024.5.1
+Version: 2024.5.2
 Summary: A Python library for the Linksys Velop Mesh system
 Home-page: https://github.com/uvjim/pyvelop
 Author: uvjim
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
```

### Comparing `pyvelop-2024.5.1/setup.py` & `pyvelop-2024.5.2/setup.py`

 * *Files identical despite different names*

