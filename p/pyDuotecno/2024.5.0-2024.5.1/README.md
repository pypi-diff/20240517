# Comparing `tmp/pyduotecno-2024.5.0.tar.gz` & `tmp/pyduotecno-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyduotecno-2024.5.0.tar", last modified: Tue May 14 16:43:28 2024, max compression
+gzip compressed data, was "pyduotecno-2024.5.1.tar", last modified: Fri May 17 14:59:31 2024, max compression
```

## Comparing `pyduotecno-2024.5.0.tar` & `pyduotecno-2024.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:28.925104 pyduotecno-2024.5.0/duotecno/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11193 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/duotecno/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/pyDuotecno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 16:43:28.000000 pyduotecno-2024.5.0/pyDuotecno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 16:43:28.929105 pyduotecno-2024.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-14 16:43:22.000000 pyduotecno-2024.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:31.807910 pyduotecno-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-17 14:59:31.807910 pyduotecno-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:31.807910 pyduotecno-2024.5.1/duotecno/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/duotecno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/duotecno/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/duotecno/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/duotecno/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11002 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/duotecno/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/duotecno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/duotecno/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:31.807910 pyduotecno-2024.5.1/pyDuotecno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-17 14:59:31.000000 pyduotecno-2024.5.1/pyDuotecno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 14:59:31.000000 pyduotecno-2024.5.1/pyDuotecno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:59:31.000000 pyduotecno-2024.5.1/pyDuotecno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:59:31.000000 pyduotecno-2024.5.1/pyDuotecno.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 14:59:31.000000 pyduotecno-2024.5.1/pyDuotecno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:59:31.807910 pyduotecno-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-17 14:59:27.000000 pyduotecno-2024.5.1/setup.py
```

### Comparing `pyduotecno-2024.5.0/LICENSE` & `pyduotecno-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyduotecno-2024.5.0/PKG-INFO` & `pyduotecno-2024.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyduotecno-2024.5.0/duotecno/controller.py` & `pyduotecno-2024.5.1/duotecno/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         else:
             # in case of skipload we do want to request the status again
             self._log.info("Requesting unit status")
             for node in self.nodes.values():
                 for unit in node.get_units():
                     self._log.debug(f"Unit: {unit}")
                     await unit.requestStatus()
+        await asyncio.sleep(5)
         self.hbTask = asyncio.Task(self.heartbeatTask())
         await self.enableAllUnits()
 
     async def write(self, msg: str) -> None:
         """Send a message."""
         if not self.writer:
             return
```

### Comparing `pyduotecno-2024.5.0/duotecno/node.py` & `pyduotecno-2024.5.1/duotecno/node.py`

 * *Files identical despite different names*

### Comparing `pyduotecno-2024.5.0/duotecno/protocol.py` & `pyduotecno-2024.5.1/duotecno/protocol.py`

 * *Files identical despite different names*

### Comparing `pyduotecno-2024.5.0/duotecno/unit.py` & `pyduotecno-2024.5.1/duotecno/unit.py`

 * *Files identical despite different names*

### Comparing `pyduotecno-2024.5.0/pyDuotecno.egg-info/PKG-INFO` & `pyduotecno-2024.5.1/pyDuotecno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDuotecno
-Version: 2024.5.0
+Version: 2024.5.1
 Summary: Open-source home automation platform running on Python 3.
 Author-email: Maikel Punie <maikel.punie@gmail.com>
 License: Apache
 Project-URL: Source Code, https://github.com/Cereal2nd/pyDuotecno
 Project-URL: Bug Reports, https://github.com/Cereal2nd/pyDuotecno/issues
 Keywords: home,duotecno,automation
 Platform: any
```

### Comparing `pyduotecno-2024.5.0/pyproject.toml` & `pyduotecno-2024.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "pyDuotecno"
 license = {text = "Apache"}
-version = "2024.5.0"
+version = "2024.5.1"
 description = "Open-source home automation platform running on Python 3."
 readme = "README.md"
 authors = [
     {name = "Maikel Punie", email = "maikel.punie@gmail.com"}
 ]
 keywords = ["home", "duotecno", "automation"]
 classifiers = [
@@ -37,15 +37,15 @@
 zip-safe  = false
 include-package-data = true
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "tests.*", "examples", "examples/*"]
 
 [tool.bumpver]
-current_version = "2024.5.0"
+current_version = "2024.5.1"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

