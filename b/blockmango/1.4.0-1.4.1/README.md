# Comparing `tmp/blockmango-1.4.0.tar.gz` & `tmp/blockmango-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.0.tar", last modified: Thu May 16 20:10:55 2024, max compression
+gzip compressed data, was "blockmango-1.4.1.tar", last modified: Thu May 16 20:29:39 2024, max compression
```

## Comparing `blockmango-1.4.0.tar` & `blockmango-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:10:55.001166 blockmango-1.4.0/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.0/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 20:10:55.001166 blockmango-1.4.0/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.0/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:10:54.977167 blockmango-1.4.0/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 19:13:31.000000 blockmango-1.4.0/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     5953 2024-05-16 20:08:47.000000 blockmango-1.4.0/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     1848 2024-05-16 20:09:05.000000 blockmango-1.4.0/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     3608 2024-05-16 20:09:31.000000 blockmango-1.4.0/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     4327 2024-05-16 20:09:47.000000 blockmango-1.4.0/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     3383 2024-05-16 20:10:06.000000 blockmango-1.4.0/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:10:54.997166 blockmango-1.4.0/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 20:10:54.000000 blockmango-1.4.0/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      330 2024-05-16 20:10:54.000000 blockmango-1.4.0/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 20:10:54.000000 blockmango-1.4.0/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 20:10:54.000000 blockmango-1.4.0/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 20:10:54.000000 blockmango-1.4.0/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 20:10:55.001166 blockmango-1.4.0/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 20:08:12.000000 blockmango-1.4.0/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:29:39.433166 blockmango-1.4.1/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.1/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 20:29:39.429166 blockmango-1.4.1/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      834 2024-05-16 17:43:12.000000 blockmango-1.4.1/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:29:39.409166 blockmango-1.4.1/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      172 2024-05-16 20:23:50.000000 blockmango-1.4.1/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     5961 2024-05-16 20:24:58.000000 blockmango-1.4.1/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      747 2024-05-16 20:23:50.000000 blockmango-1.4.1/blockmango/constants.py
+-rw-------   0 userland  (2000) userland  (2000)     1856 2024-05-16 20:27:18.000000 blockmango-1.4.1/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     3616 2024-05-16 20:27:59.000000 blockmango-1.4.1/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     4336 2024-05-16 20:28:32.000000 blockmango-1.4.1/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     3391 2024-05-16 20:28:52.000000 blockmango-1.4.1/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-16 20:29:39.425166 blockmango-1.4.1/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)      430 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      354 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-16 20:29:38.000000 blockmango-1.4.1/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-16 20:29:39.433166 blockmango-1.4.1/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)      503 2024-05-16 20:29:22.000000 blockmango-1.4.1/setup.py
```

### Comparing `blockmango-1.4.0/LICENSE.md` & `blockmango-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.0/README.md` & `blockmango-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.0/blockmango/clan.py` & `blockmango-1.4.1/blockmango/clan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
-from constant.constants import BASE_URL, BASE_URL_V2, BASE_URL_V3, HEADERS_TEMPLATE
+import constants
+from constants import BASE_URL, BASE_URL_V2, BASE_URL_V3, HEADERS_TEMPLATE
 
 class Clan:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
             "Access-Token": access_token
```

### Comparing `blockmango-1.4.0/blockmango/decoration.py` & `blockmango-1.4.1/blockmango/decoration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
-from constant.constants import BASE_URL_DECORATION, BASE_URL_SHOP, BASE_URL_USER, HEADERS_TEMPLATE
+import constants
+from constants import BASE_URL_DECORATION, BASE_URL_SHOP, BASE_URL_USER, HEADERS_TEMPLATE
 
 class Decoration:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
             "Access-Token": access_token
```

### Comparing `blockmango-1.4.0/blockmango/friends.py` & `blockmango-1.4.1/blockmango/friends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
-from constant.constants import BASE_URL_FRIEND, BASE_URL_DECORATION, HEADERS_TEMPLATE
+import constants
+from constants import BASE_URL_FRIEND, BASE_URL_DECORATION, HEADERS_TEMPLATE
 
 class Friends:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
             "Access-Token": access_token
```

### Comparing `blockmango-1.4.0/blockmango/groupchat.py` & `blockmango-1.4.1/blockmango/groupchat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import request
-from constant.constants import BASE_URL_GROUP, BASE_URL_GROUP_V2, HEADERS_TEMPLATE
+import requests
+import constants
+from constants import BASE_URL_GROUP, BASE_URL_GROUP_V2, HEADERS_TEMPLATE
 
 class Group:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
             "Access-Token": access_token
```

### Comparing `blockmango-1.4.0/blockmango/user.py` & `blockmango-1.4.1/blockmango/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
-from constant.constants import BASE_URL_USER, BASE_URL_ROUTE, HEADERS_TEMPLATE
+import constants
+from constants import BASE_URL_USER, BASE_URL_ROUTE, HEADERS_TEMPLATE
 
 class User:
     def __init__(self, user_id, access_token):
         self.headers = {
             **HEADERS_TEMPLATE,
             "userId": user_id,
             "Access-Token": access_token
```

