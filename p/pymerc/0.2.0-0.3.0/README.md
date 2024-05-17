# Comparing `tmp/pymerc-0.2.0.tar.gz` & `tmp/pymerc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymerc-0.2.0.tar", max compression
+gzip compressed data, was "pymerc-0.3.0.tar", max compression
```

## Comparing `pymerc-0.2.0.tar` & `pymerc-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1096 2024-05-14 17:39:13.904595 pymerc-0.2.0/README.md
--rw-r--r--   0        0        0      381 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/base.py
--rw-r--r--   0        0        0      571 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/map.py
--rw-r--r--   0        0        0      264 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/models/common.py
--rw-r--r--   0        0        0      594 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/models/map.py
--rw-r--r--   0        0        0     2003 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/models/player.py
--rw-r--r--   0        0        0     2466 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/models/static.py
--rw-r--r--   0        0        0     3325 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/models/towns.py
--rw-r--r--   0        0        0      481 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/player.py
--rw-r--r--   0        0        0     2207 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/static.py
--rw-r--r--   0        0        0     1828 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/api/towns.py
--rw-r--r--   0        0        0     1282 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/client.py
--rw-r--r--   0        0        0      834 2024-05-14 17:39:13.904595 pymerc-0.2.0/pymerc/util/towns.py
--rw-r--r--   0        0        0      761 2024-05-14 17:39:13.904595 pymerc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 pymerc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-17 15:32:57.829331 pymerc-0.3.0/README.md
+-rw-r--r--   0        0        0      381 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/base.py
+-rw-r--r--   0        0        0      571 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/map.py
+-rw-r--r--   0        0        0      264 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/common.py
+-rw-r--r--   0        0        0      594 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/map.py
+-rw-r--r--   0        0        0     2003 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/player.py
+-rw-r--r--   0        0        0     2466 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/static.py
+-rw-r--r--   0        0        0     3285 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/models/towns.py
+-rw-r--r--   0        0        0      481 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/player.py
+-rw-r--r--   0        0        0     2204 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/static.py
+-rw-r--r--   0        0        0     1828 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/api/towns.py
+-rw-r--r--   0        0        0     1282 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/client.py
+-rw-r--r--   0        0        0     1585 2024-05-17 15:32:57.829331 pymerc-0.3.0/pymerc/util/towns.py
+-rw-r--r--   0        0        0      761 2024-05-17 15:32:57.829331 pymerc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 pymerc-0.3.0/PKG-INFO
```

### Comparing `pymerc-0.2.0/README.md` & `pymerc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pymerc-0.2.0/pymerc/api/map.py` & `pymerc-0.3.0/pymerc/api/map.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.2.0/pymerc/api/models/map.py` & `pymerc-0.3.0/pymerc/api/models/map.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.2.0/pymerc/api/models/player.py` & `pymerc-0.3.0/pymerc/api/models/player.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.2.0/pymerc/api/models/static.py` & `pymerc-0.3.0/pymerc/api/models/static.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.2.0/pymerc/api/models/towns.py` & `pymerc-0.3.0/pymerc/api/models/towns.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     """Represents the data for a town in the game."""
     id: str
     name: str
     location: Location
     region: int
     center_ids: list[int]
     domain: dict[str, TownDomain]
-    structures: dict[str, TownStrucure]
     household_ids: list[str]
     commoners: TownCommoners
     government: TownGovernment
     church: TownChurch
     navigation_zones: dict[int, int]
     culture: TownCulture
```

### Comparing `pymerc-0.2.0/pymerc/api/static.py` & `pymerc-0.3.0/pymerc/api/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,9 +64,9 @@
             The static data from the game.
         """
         response = await self.client.get(ROOT_URL)
         pattern = r"src=\"\/static\/js\/(.*?)\">"
         filename = re.search(pattern, response.text).group(1)
 
         response = await self.client.get(BASE_URL + filename)
-        pattern = r"Bt=JSON\.parse\('(.*?)'\)"
+        pattern = r"JSON\.parse\('(.*?)'\)"
         return json.loads(re.search(pattern, response.text).group(1).replace("\\", ""))
```

### Comparing `pymerc-0.2.0/pymerc/api/towns.py` & `pymerc-0.3.0/pymerc/api/towns.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.2.0/pymerc/client.py` & `pymerc-0.3.0/pymerc/client.py`

 * *Files identical despite different names*

### Comparing `pymerc-0.2.0/pyproject.toml` & `pymerc-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymerc"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Python library for interacting with the Mercatorio browser based game"
 authors = ["Joshua Gilman <joshuagilman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jmgilman/pymerc"
 keywords = ["mercatorio", "python", "library", "game"]
 packages = [{ include = "pymerc" }]
```

### Comparing `pymerc-0.2.0/PKG-INFO` & `pymerc-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymerc
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Python library for interacting with the Mercatorio browser based game
 Home-page: https://github.com/jmgilman/pymerc
 License: MIT
 Keywords: mercatorio,python,library,game
 Author: Joshua Gilman
 Author-email: joshuagilman@gmail.com
 Requires-Python: >=3.11,<4.0
```

