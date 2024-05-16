# Comparing `tmp/kbve-1.0.7.tar.gz` & `tmp/kbve-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kbve-1.0.7.tar", max compression
+gzip compressed data, was "kbve-1.0.8.tar", max compression
```

## Comparing `kbve-1.0.7.tar` & `kbve-1.0.8.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0       35 2024-04-17 13:56:58.189905 kbve-1.0.7/README.md
--rw-r--r--   0        0        0      161 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/OAI_CONFIG_LIST.json
--rw-r--r--   0        0        0       12 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/__init__.py
--rw-r--r--   0        0        0        9 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/__init__.py
--rw-r--r--   0        0        0     4075 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/api_connector.py
--rw-r--r--   0        0        0      240 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/__init__.py
--rw-r--r--   0        0        0     1998 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/coindesk_client.py
--rw-r--r--   0        0        0     1985 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/novnc_client.py
--rw-r--r--   0        0        0     1166 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/poetry_db_client.py
--rw-r--r--   0        0        0     1336 2024-04-17 13:56:58.189905 kbve-1.0.7/kbve_atlas/api/clients/screen_client.py
--rw-r--r--   0        0        0     2967 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/clients/websocket_echo_client.py
--rw-r--r--   0        0        0      234 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/broadcast_utils.py
--rw-r--r--   0        0        0     1088 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/cors_utils.py
--rw-r--r--   0        0        0     2350 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/image_utils.py
--rw-r--r--   0        0        0      823 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/kr_decorator.py
--rw-r--r--   0        0        0     3048 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/rss_utils.py
--rw-r--r--   0        0        0     1517 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/api/utils/theme_core.py
--rw-r--r--   0        0        0      940 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/atlas_autogen.py
--rw-r--r--   0        0        0      616 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/bigman.py
--rw-r--r--   0        0        0        0 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/__init__.py
--rw-r--r--   0        0        0     1480 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/doom.py
--rw-r--r--   0        0        0     1167 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/enter_the_matrix.py
--rw-r--r--   0        0        0     4640 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/memetris.py
--rw-r--r--   0        0        0     2012 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/pacman.py
--rw-r--r--   0        0        0     1379 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/snake.py
--rw-r--r--   0        0        0     2215 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/games/tetris.py
--rw-r--r--   0        0        0      473 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/hello.py
--rw-r--r--   0        0        0       11 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/__init__.py
--rw-r--r--   0        0        0      523 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/coindesk.py
--rw-r--r--   0        0        0      190 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/poem.py
--rw-r--r--   0        0        0     1434 2024-04-17 13:56:58.193904 kbve-1.0.7/kbve_atlas/models/rsps.py
--rw-r--r--   0        0        0      335 2024-04-17 13:56:58.197904 kbve-1.0.7/kbve_atlas/models/rss.py
--rw-r--r--   0        0        0    15477 2024-04-17 13:56:58.929907 kbve-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     8809 1970-01-01 00:00:00.000000 kbve-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-05-16 22:58:29.163511 kbve-1.0.8/README.md
+-rw-r--r--   0        0        0      161 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/OAI_CONFIG_LIST.json
+-rw-r--r--   0        0        0       12 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/__init__.py
+-rw-r--r--   0        0        0        9 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/__init__.py
+-rw-r--r--   0        0        0     4075 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/api_connector.py
+-rw-r--r--   0        0        0      283 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/__init__.py
+-rw-r--r--   0        0        0     1998 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/coindesk_client.py
+-rw-r--r--   0        0        0     1985 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/novnc_client.py
+-rw-r--r--   0        0        0     1166 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/poetry_db_client.py
+-rw-r--r--   0        0        0      982 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/runelite_client.py
+-rw-r--r--   0        0        0     1336 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/screen_client.py
+-rw-r--r--   0        0        0     2967 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/clients/websocket_echo_client.py
+-rw-r--r--   0        0        0      234 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/__init__.py
+-rw-r--r--   0        0        0     2315 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/broadcast_utils.py
+-rw-r--r--   0        0        0     1088 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/cors_utils.py
+-rw-r--r--   0        0        0     2350 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/image_utils.py
+-rw-r--r--   0        0        0      823 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/kr_decorator.py
+-rw-r--r--   0        0        0     3048 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/rss_utils.py
+-rw-r--r--   0        0        0     1517 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/api/utils/theme_core.py
+-rw-r--r--   0        0        0      940 2024-05-16 22:58:29.167511 kbve-1.0.8/kbve_atlas/atlas_autogen.py
+-rw-r--r--   0        0        0      616 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/bigman.py
+-rw-r--r--   0        0        0        0 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/__init__.py
+-rw-r--r--   0        0        0     1480 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/doom.py
+-rw-r--r--   0        0        0     1167 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/enter_the_matrix.py
+-rw-r--r--   0        0        0     4640 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/memetris.py
+-rw-r--r--   0        0        0     2012 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/pacman.py
+-rw-r--r--   0        0        0     1379 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/snake.py
+-rw-r--r--   0        0        0     2215 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/games/tetris.py
+-rw-r--r--   0        0        0      473 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/hello.py
+-rw-r--r--   0        0        0       11 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/coindesk.py
+-rw-r--r--   0        0        0      190 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/poem.py
+-rw-r--r--   0        0        0     1434 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/rsps.py
+-rw-r--r--   0        0        0      335 2024-05-16 22:58:29.171511 kbve-1.0.8/kbve_atlas/models/rss.py
+-rw-r--r--   0        0        0    15477 2024-05-16 22:58:29.923512 kbve-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8809 1970-01-01 00:00:00.000000 kbve-1.0.8/PKG-INFO
```

### Comparing `kbve-1.0.7/kbve_atlas/api/api_connector.py` & `kbve-1.0.8/kbve_atlas/api/api_connector.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/clients/coindesk_client.py` & `kbve-1.0.8/kbve_atlas/api/clients/coindesk_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/clients/novnc_client.py` & `kbve-1.0.8/kbve_atlas/api/clients/novnc_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/clients/poetry_db_client.py` & `kbve-1.0.8/kbve_atlas/api/clients/poetry_db_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/clients/screen_client.py` & `kbve-1.0.8/kbve_atlas/api/clients/screen_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/clients/websocket_echo_client.py` & `kbve-1.0.8/kbve_atlas/api/clients/websocket_echo_client.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/utils/broadcast_utils.py` & `kbve-1.0.8/kbve_atlas/api/utils/broadcast_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/utils/cors_utils.py` & `kbve-1.0.8/kbve_atlas/api/utils/cors_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/utils/image_utils.py` & `kbve-1.0.8/kbve_atlas/api/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/utils/kr_decorator.py` & `kbve-1.0.8/kbve_atlas/api/utils/kr_decorator.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/utils/rss_utils.py` & `kbve-1.0.8/kbve_atlas/api/utils/rss_utils.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/api/utils/theme_core.py` & `kbve-1.0.8/kbve_atlas/api/utils/theme_core.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/atlas_autogen.py` & `kbve-1.0.8/kbve_atlas/atlas_autogen.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/bigman.py` & `kbve-1.0.8/kbve_atlas/bigman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/games/doom.py` & `kbve-1.0.8/kbve_atlas/games/doom.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/games/enter_the_matrix.py` & `kbve-1.0.8/kbve_atlas/games/enter_the_matrix.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/games/memetris.py` & `kbve-1.0.8/kbve_atlas/games/memetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/games/pacman.py` & `kbve-1.0.8/kbve_atlas/games/pacman.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/games/snake.py` & `kbve-1.0.8/kbve_atlas/games/snake.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/games/tetris.py` & `kbve-1.0.8/kbve_atlas/games/tetris.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/models/coindesk.py` & `kbve-1.0.8/kbve_atlas/models/coindesk.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/kbve_atlas/models/rsps.py` & `kbve-1.0.8/kbve_atlas/models/rsps.py`

 * *Files identical despite different names*

### Comparing `kbve-1.0.7/pyproject.toml` & `kbve-1.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   stubPath = "typings"
   typingsPath = "typings"
   analyzeTypeshed = false
   autoSearchPaths = true
 
 [tool.poetry]
 name = "kbve"
-version = "1.0.7"
+version = "1.0.8"
 description = "ATLAS"
 authors = [ ]
 license = "Proprietary"
 readme = "README.md"
 
   [[tool.poetry.packages]]
   include = "kbve_atlas"
```

### Comparing `kbve-1.0.7/PKG-INFO` & `kbve-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kbve
-Version: 1.0.7
+Version: 1.0.8
 Summary: ATLAS
 License: Proprietary
 Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

