# Comparing `tmp/txt2udp-0.1.2.tar.gz` & `tmp/txt2udp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt2udp-0.1.2.tar", last modified: Thu May 16 12:26:28 2024, max compression
+gzip compressed data, was "txt2udp-0.1.3.tar", last modified: Fri May 17 14:03:27 2024, max compression
```

## Comparing `txt2udp-0.1.2.tar` & `txt2udp-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:26:28.547591 txt2udp-0.1.2/
--rw-rw-rw-   0        0        0    11560 2024-05-15 12:52:07.000000 txt2udp-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2861 2024-05-16 12:26:28.545077 txt2udp-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2218 2024-05-15 12:46:37.000000 txt2udp-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:26:28.547591 txt2udp-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      944 2024-05-16 12:25:53.000000 txt2udp-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:26:28.522874 txt2udp-0.1.2/txt2udp/
--rw-rw-rw-   0        0        0        0 2024-05-13 01:53:18.000000 txt2udp-0.1.2/txt2udp/__init__.py
--rw-rw-rw-   0        0        0     2218 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/cli.py
--rw-rw-rw-   0        0        0     3169 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/client.py
--rw-rw-rw-   0        0        0     1127 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/config.py
--rw-rw-rw-   0        0        0     1844 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/conn.py
--rw-rw-rw-   0        0        0      977 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/datagram.py
--rw-rw-rw-   0        0        0     1579 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/main.py
--rw-rw-rw-   0        0        0      330 2024-05-13 07:34:38.000000 txt2udp-0.1.2/txt2udp/messages.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:26:28.541075 txt2udp-0.1.2/txt2udp/plugins/
--rw-rw-rw-   0        0        0      621 2024-05-13 10:51:17.000000 txt2udp-0.1.2/txt2udp/plugins/__init__.py
--rw-rw-rw-   0        0        0     3783 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/plugins/mitm.py
--rw-rw-rw-   0        0        0     1530 2024-05-16 12:25:42.000000 txt2udp-0.1.2/txt2udp/plugins/stdio.py
--rw-rw-rw-   0        0        0     3032 2024-05-15 12:12:05.000000 txt2udp-0.1.2/txt2udp/server.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:26:28.543078 txt2udp-0.1.2/txt2udp.egg-info/
--rw-rw-rw-   0        0        0     2861 2024-05-16 12:26:28.000000 txt2udp-0.1.2/txt2udp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      452 2024-05-16 12:26:28.000000 txt2udp-0.1.2/txt2udp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:26:28.000000 txt2udp-0.1.2/txt2udp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-16 12:26:28.000000 txt2udp-0.1.2/txt2udp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-05-16 12:26:28.000000 txt2udp-0.1.2/txt2udp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 12:26:28.000000 txt2udp-0.1.2/txt2udp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 14:03:27.928658 txt2udp-0.1.3/
+-rw-rw-rw-   0        0        0    11560 2024-05-15 12:52:07.000000 txt2udp-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2861 2024-05-17 14:03:27.926498 txt2udp-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2218 2024-05-15 12:46:37.000000 txt2udp-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 14:03:27.929654 txt2udp-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      944 2024-05-17 14:03:14.000000 txt2udp-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:03:27.902895 txt2udp-0.1.3/txt2udp/
+-rw-rw-rw-   0        0        0        0 2024-05-13 01:53:18.000000 txt2udp-0.1.3/txt2udp/__init__.py
+-rw-rw-rw-   0        0        0     2218 2024-05-15 12:12:05.000000 txt2udp-0.1.3/txt2udp/cli.py
+-rw-rw-rw-   0        0        0     3169 2024-05-15 12:12:05.000000 txt2udp-0.1.3/txt2udp/client.py
+-rw-rw-rw-   0        0        0     1127 2024-05-15 12:12:05.000000 txt2udp-0.1.3/txt2udp/config.py
+-rw-rw-rw-   0        0        0     1844 2024-05-15 12:12:05.000000 txt2udp-0.1.3/txt2udp/conn.py
+-rw-rw-rw-   0        0        0      977 2024-05-15 12:12:05.000000 txt2udp-0.1.3/txt2udp/datagram.py
+-rw-rw-rw-   0        0        0     1579 2024-05-15 12:12:05.000000 txt2udp-0.1.3/txt2udp/main.py
+-rw-rw-rw-   0        0        0      330 2024-05-13 07:34:38.000000 txt2udp-0.1.3/txt2udp/messages.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:03:27.921498 txt2udp-0.1.3/txt2udp/plugins/
+-rw-rw-rw-   0        0        0      621 2024-05-13 10:51:17.000000 txt2udp-0.1.3/txt2udp/plugins/__init__.py
+-rw-rw-rw-   0        0        0     3909 2024-05-17 14:02:23.000000 txt2udp-0.1.3/txt2udp/plugins/mitm.py
+-rw-rw-rw-   0        0        0     1530 2024-05-16 12:25:42.000000 txt2udp-0.1.3/txt2udp/plugins/stdio.py
+-rw-rw-rw-   0        0        0     3032 2024-05-15 12:12:05.000000 txt2udp-0.1.3/txt2udp/server.py
+drwxrwxrwx   0        0        0        0 2024-05-17 14:03:27.925527 txt2udp-0.1.3/txt2udp.egg-info/
+-rw-rw-rw-   0        0        0     2861 2024-05-17 14:03:27.000000 txt2udp-0.1.3/txt2udp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      452 2024-05-17 14:03:27.000000 txt2udp-0.1.3/txt2udp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 14:03:27.000000 txt2udp-0.1.3/txt2udp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-17 14:03:27.000000 txt2udp-0.1.3/txt2udp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-05-17 14:03:27.000000 txt2udp-0.1.3/txt2udp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 14:03:27.000000 txt2udp-0.1.3/txt2udp.egg-info/top_level.txt
```

### Comparing `txt2udp-0.1.2/LICENSE` & `txt2udp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/PKG-INFO` & `txt2udp-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2udp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple tool for forwarding UDP datagrams through a text-only protocol/interface.
 Home-page: https://github.com/mirrorange/TXT2UDP
 Author: Orange
 Author-email: orange@icedeer.net
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `txt2udp-0.1.2/README.md` & `txt2udp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/setup.py` & `txt2udp-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="txt2udp",
-    version="0.1.2",
+    version="0.1.3",
     description="A simple tool for forwarding UDP datagrams through a text-only protocol/interface.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mirrorange/TXT2UDP",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
```

### Comparing `txt2udp-0.1.2/txt2udp/cli.py` & `txt2udp-0.1.3/txt2udp/cli.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/client.py` & `txt2udp-0.1.3/txt2udp/client.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/config.py` & `txt2udp-0.1.3/txt2udp/config.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/conn.py` & `txt2udp-0.1.3/txt2udp/conn.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/datagram.py` & `txt2udp-0.1.3/txt2udp/datagram.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/main.py` & `txt2udp-0.1.3/txt2udp/main.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/plugins/__init__.py` & `txt2udp-0.1.3/txt2udp/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/plugins/mitm.py` & `txt2udp-0.1.3/txt2udp/plugins/mitm.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,17 @@
         if self._working_flow != flow:
             return
 
         # Handle messages
         if not last_message.from_client:
             # Handle stdout
             if message_type == "stdout":
-                await self.input_queue.put(message_text)
+                lines = [line.strip() for line in message_text.split("\n") if line.strip()]
+                for line in lines:
+                    await self.output_queue.put(line)
         elif message_type == "stdin" and message_text == "\u0003":
             # Stop terminal
             self._working_flow = None
             return
 
         # Drop message
         last_message.drop()
```

### Comparing `txt2udp-0.1.2/txt2udp/plugins/stdio.py` & `txt2udp-0.1.3/txt2udp/plugins/stdio.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp/server.py` & `txt2udp-0.1.3/txt2udp/server.py`

 * *Files identical despite different names*

### Comparing `txt2udp-0.1.2/txt2udp.egg-info/PKG-INFO` & `txt2udp-0.1.3/txt2udp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txt2udp
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple tool for forwarding UDP datagrams through a text-only protocol/interface.
 Home-page: https://github.com/mirrorange/TXT2UDP
 Author: Orange
 Author-email: orange@icedeer.net
 License: Apache-2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

