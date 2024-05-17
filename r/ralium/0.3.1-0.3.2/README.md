# Comparing `tmp/ralium-0.3.1.tar.gz` & `tmp/ralium-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-0.3.1.tar", last modified: Thu May 16 18:25:46 2024, max compression
+gzip compressed data, was "ralium-0.3.2.tar", last modified: Thu May 16 19:49:06 2024, max compression
```

## Comparing `ralium-0.3.1.tar` & `ralium-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:25:46.486711 ralium-0.3.1/
--rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.3.1/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-16 18:25:46.485244 ralium-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.3.1/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-16 18:25:24.000000 ralium-0.3.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-16 18:25:46.467350 ralium-0.3.1/ralium/
--rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.3.1/ralium/__init__.py
--rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.3.1/ralium/_util.py
--rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.3.1/ralium/_util.pyi
--rw-rw-rw-   0        0        0     6579 2024-05-16 18:23:22.000000 ralium-0.3.1/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.3.1/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.3.1/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.3.1/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.3.1/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.3.1/ralium/config.pyi
--rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.3.1/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.3.1/ralium/element.pyi
--rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.3.1/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.3.1/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1086 2024-05-16 17:41:03.000000 ralium-0.3.1/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-16 15:25:16.000000 ralium-0.3.1/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.3.1/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.3.1/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.3.1/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.3.1/ralium/setup.py
--rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.3.1/ralium/setup.pyi
--rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.3.1/ralium/webpage.py
--rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.3.1/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6022 2024-05-16 17:41:38.000000 ralium-0.3.1/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-16 17:42:01.000000 ralium-0.3.1/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-16 18:25:46.484241 ralium-0.3.1/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-16 18:25:46.000000 ralium-0.3.1/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-05-16 18:25:46.000000 ralium-0.3.1/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:25:46.000000 ralium-0.3.1/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-16 18:25:46.000000 ralium-0.3.1/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 18:25:46.000000 ralium-0.3.1/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:25:46.486711 ralium-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 19:49:06.236585 ralium-0.3.2/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-16 19:49:06.235469 ralium-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.3.2/README.md
+-rw-rw-rw-   0        0        0     1018 2024-05-16 19:48:33.000000 ralium-0.3.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-16 19:49:06.218456 ralium-0.3.2/ralium/
+-rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.3.2/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.3.2/ralium/_util.py
+-rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.3.2/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     6579 2024-05-16 18:23:22.000000 ralium-0.3.2/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.3.2/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.3.2/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.3.2/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.3.2/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.3.2/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.3.2/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.3.2/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.3.2/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.3.2/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1086 2024-05-16 17:41:03.000000 ralium-0.3.2/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-16 15:25:16.000000 ralium-0.3.2/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.3.2/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.3.2/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.3.2/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.3.2/ralium/setup.py
+-rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.3.2/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.3.2/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.3.2/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6031 2024-05-16 19:45:52.000000 ralium-0.3.2/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-16 17:42:01.000000 ralium-0.3.2/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-16 19:49:06.234377 ralium-0.3.2/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-16 19:49:06.000000 ralium-0.3.2/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2024-05-16 19:49:06.000000 ralium-0.3.2/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 19:49:06.000000 ralium-0.3.2/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-16 19:49:06.000000 ralium-0.3.2/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 19:49:06.000000 ralium-0.3.2/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 19:49:06.236585 ralium-0.3.2/setup.cfg
```

### Comparing `ralium-0.3.1/LICENSE` & `ralium-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/PKG-INFO` & `ralium-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.3.1
+Version: 0.3.2
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.3.1/pyproject.toml` & `ralium-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "0.3.1"
+version = "0.3.2"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-0.3.1/ralium/_util.py` & `ralium-0.3.2/ralium/_util.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/_util.pyi` & `ralium-0.3.2/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/api.py` & `ralium-0.3.2/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/api.pyi` & `ralium-0.3.2/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/builtins.py` & `ralium-0.3.2/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/builtins.pyi` & `ralium-0.3.2/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/config.py` & `ralium-0.3.2/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/element.py` & `ralium-0.3.2/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/element.pyi` & `ralium-0.3.2/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/engine.py` & `ralium-0.3.2/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/engine.pyi` & `ralium-0.3.2/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/errors.py` & `ralium-0.3.2/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/listener.py` & `ralium-0.3.2/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/listener.pyi` & `ralium-0.3.2/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/navigation.py` & `ralium-0.3.2/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/setup.py` & `ralium-0.3.2/ralium/setup.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/setup.pyi` & `ralium-0.3.2/ralium/setup.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/webpage.py` & `ralium-0.3.2/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/webpage.pyi` & `ralium-0.3.2/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium/window.py` & `ralium-0.3.2/ralium/window.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,21 +151,22 @@
         html = BeautifulSoup(webhook.html, features="lxml")
         webhook.elements = [create_ralium_id(element) for element in html.body.find_all()]
 
         create_element(html, "base", {"href": str(self.engine)})
         create_element(html, "script", string=str(self.engine.bridge))
         create_element(html, "style", string=webhook.css)
 
-        if self.running:
-            return self.render(html)
-        
-        self.webview.html = str(html)
+        self.render(html)
 
     def render(self, html):
         """Write HTML to the DOM."""
+        if not self.running:
+            self.webview.html = str(html)
+            return
+
         self.webview.evaluate_js(f"document.open();document.write(String.raw`{str(html)}`);document.close();")
     
     def start(self):
         """Starts the Ralium Window and officially displays the GUI."""
         if self.running: return
         
         self.running = True
```

### Comparing `ralium-0.3.1/ralium/window.pyi` & `ralium-0.3.2/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.1/ralium.egg-info/PKG-INFO` & `ralium-0.3.2/ralium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.3.1
+Version: 0.3.2
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.3.1/ralium.egg-info/SOURCES.txt` & `ralium-0.3.2/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

