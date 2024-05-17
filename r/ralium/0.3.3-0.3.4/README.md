# Comparing `tmp/ralium-0.3.3.tar.gz` & `tmp/ralium-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-0.3.3.tar", last modified: Fri May 17 19:38:56 2024, max compression
+gzip compressed data, was "ralium-0.3.4.tar", last modified: Fri May 17 20:28:25 2024, max compression
```

## Comparing `ralium-0.3.3.tar` & `ralium-0.3.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 19:38:56.626027 ralium-0.3.3/
--rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.3.3/LICENSE
--rw-rw-rw-   0        0        0    41876 2024-05-17 19:38:56.624719 ralium-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.3.3/README.md
--rw-rw-rw-   0        0        0     1018 2024-05-17 19:37:32.000000 ralium-0.3.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-17 19:38:56.604291 ralium-0.3.3/ralium/
--rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.3.3/ralium/__init__.py
--rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.3.3/ralium/_util.py
--rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.3.3/ralium/_util.pyi
--rw-rw-rw-   0        0        0     6579 2024-05-17 19:36:07.000000 ralium-0.3.3/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.3.3/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.3.3/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.3.3/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.3.3/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.3.3/ralium/config.pyi
--rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.3.3/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.3.3/ralium/element.pyi
--rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.3.3/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.3.3/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1086 2024-05-16 17:41:03.000000 ralium-0.3.3/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-16 15:25:16.000000 ralium-0.3.3/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.3.3/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.3.3/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.3.3/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     3952 2024-05-13 23:29:31.000000 ralium-0.3.3/ralium/setup.py
--rw-rw-rw-   0        0        0      559 2024-05-13 23:23:01.000000 ralium-0.3.3/ralium/setup.pyi
--rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.3.3/ralium/webpage.py
--rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.3.3/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6031 2024-05-16 19:45:52.000000 ralium-0.3.3/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-16 17:42:01.000000 ralium-0.3.3/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-17 19:38:56.622716 ralium-0.3.3/ralium.egg-info/
--rw-rw-rw-   0        0        0    41876 2024-05-17 19:38:56.000000 ralium-0.3.3/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      612 2024-05-17 19:38:56.000000 ralium-0.3.3/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 19:38:56.000000 ralium-0.3.3/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-17 19:38:56.000000 ralium-0.3.3/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 19:38:56.000000 ralium-0.3.3/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 19:38:56.626027 ralium-0.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 20:28:25.110911 ralium-0.3.4/
+-rw-rw-rw-   0        0        0    35823 2024-04-24 23:35:07.000000 ralium-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0    41876 2024-05-17 20:28:25.109703 ralium-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-04-24 23:35:07.000000 ralium-0.3.4/README.md
+-rw-rw-rw-   0        0        0     1018 2024-05-17 20:19:34.000000 ralium-0.3.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-17 20:28:25.093457 ralium-0.3.4/ralium/
+-rw-rw-rw-   0        0        0      185 2024-05-13 23:24:25.000000 ralium-0.3.4/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1816 2024-05-14 21:40:48.000000 ralium-0.3.4/ralium/_util.py
+-rw-rw-rw-   0        0        0      634 2024-05-14 21:32:03.000000 ralium-0.3.4/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     6579 2024-05-17 19:36:07.000000 ralium-0.3.4/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-13 23:23:35.000000 ralium-0.3.4/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-02 17:00:29.000000 ralium-0.3.4/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-13 23:23:27.000000 ralium-0.3.4/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-13 22:21:52.000000 ralium-0.3.4/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-01 22:26:47.000000 ralium-0.3.4/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6194 2024-05-14 05:14:25.000000 ralium-0.3.4/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-14 05:14:09.000000 ralium-0.3.4/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4401 2024-05-13 21:17:30.000000 ralium-0.3.4/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-13 23:23:13.000000 ralium-0.3.4/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1086 2024-05-16 17:41:03.000000 ralium-0.3.4/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-16 15:25:16.000000 ralium-0.3.4/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-16 14:59:59.000000 ralium-0.3.4/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-14 21:31:14.000000 ralium-0.3.4/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-04-29 20:44:02.000000 ralium-0.3.4/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     3945 2024-05-17 20:13:42.000000 ralium-0.3.4/ralium/setup.py
+-rw-rw-rw-   0        0        0      587 2024-05-17 20:14:19.000000 ralium-0.3.4/ralium/setup.pyi
+-rw-rw-rw-   0        0        0     5738 2024-05-14 21:32:26.000000 ralium-0.3.4/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1250 2024-05-13 23:22:49.000000 ralium-0.3.4/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6031 2024-05-17 19:51:41.000000 ralium-0.3.4/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-16 17:42:01.000000 ralium-0.3.4/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-17 20:28:25.108209 ralium-0.3.4/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41876 2024-05-17 20:28:25.000000 ralium-0.3.4/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2024-05-17 20:28:25.000000 ralium-0.3.4/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 20:28:25.000000 ralium-0.3.4/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-17 20:28:25.000000 ralium-0.3.4/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 20:28:25.000000 ralium-0.3.4/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 20:28:25.110911 ralium-0.3.4/setup.cfg
```

### Comparing `ralium-0.3.3/LICENSE` & `ralium-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/PKG-INFO` & `ralium-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.3.3
+Version: 0.3.4
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.3.3/pyproject.toml` & `ralium-0.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "0.3.3"
+version = "0.3.4"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-0.3.3/ralium/_util.py` & `ralium-0.3.4/ralium/_util.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/_util.pyi` & `ralium-0.3.4/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/api.py` & `ralium-0.3.4/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/api.pyi` & `ralium-0.3.4/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/builtins.py` & `ralium-0.3.4/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/builtins.pyi` & `ralium-0.3.4/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/config.py` & `ralium-0.3.4/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/element.py` & `ralium-0.3.4/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/element.pyi` & `ralium-0.3.4/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/engine.py` & `ralium-0.3.4/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/engine.pyi` & `ralium-0.3.4/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/errors.py` & `ralium-0.3.4/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/listener.py` & `ralium-0.3.4/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/listener.pyi` & `ralium-0.3.4/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/navigation.py` & `ralium-0.3.4/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/setup.py` & `ralium-0.3.4/ralium/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from ralium.errors import DisableWarnings
 import PyInstaller.__main__
 import sys
 import os
 
 HTML_FILE_EXTENSIONS = [".htm", ".html"]
+FILE_EXTENSIONS = [*HTML_FILE_EXTENSIONS, ".css", ".py"]
 
 def _exe_str_error(name, var):
     return TypeError(f"Expected executable {name} to be of type 'str', instead got '{type(var)}'")
 
 def _add_data_arg(src, dst):
     return f'--add-data={src}{os.pathsep}{dst}'
 
@@ -26,25 +27,25 @@
     cssfolder = os.path.join(webfolder, "styles")
     imgfolder = os.path.join(webfolder, "images")
     webfolder_name = os.path.basename(webfolder)
     
     if os.path.exists(webroutes):
         for root, _, files in os.walk(webroutes):
             dest = os.path.normpath(f"{webfolder_name}\\{root.removeprefix(webfolder)}")
-            webfiles.update({os.path.join(root, file): os.path.join(dest, file) for file in files if os.path.splitext(file)[-1] in HTML_FILE_EXTENSIONS})
+            webfiles.update({os.path.join(root, file): dest for file in files if os.path.splitext(file)[-1] in FILE_EXTENSIONS})
     
     if os.path.exists(cssfolder):
         for root, _, files in os.walk(cssfolder):
             dest = os.path.normpath(f"{webfolder_name}\\{root.removeprefix(webfolder)}")
-            webfiles.update({os.path.join(root, file): os.path.join(dest, file) for file in files if os.path.splitext(file)[-1] == ".css"})
+            webfiles.update({os.path.join(root, file): dest for file in files if os.path.splitext(file)[-1] == ".css"})
     
     if os.path.exists(imgfolder):
         for root, _, files in os.walk(imgfolder):
             dest = os.path.normpath(f"{webfolder_name}\\{root.removeprefix(webfolder)}")
-            webfiles.update({os.path.join(root, file): os.path.join(dest, file) for file in files})
+            webfiles.update({os.path.join(root, file): dest for file in files})
     
     return webfiles
 
 def setup(
     pyfile,
     name = None,
     icon = None,
```

### Comparing `ralium-0.3.3/ralium/setup.pyi` & `ralium-0.3.4/ralium/setup.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ralium._util import (
     FilePathStr,
     DirPathStr,
     Any
 )
 
 HTML_FILE_EXTENSIONS: list[str]
+FILE_EXTENSIONS: list[str]
 
 def _exe_str_error(name: str, var: Any) -> Exception: ...
 def _add_data_arg(src: FilePathStr, dst: FilePathStr) -> str: ...
 
 def collect_webfolder(webfolder: DirPathStr) -> dict[FilePathStr]: ...
 
 def setup(
```

### Comparing `ralium-0.3.3/ralium/webpage.py` & `ralium-0.3.4/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/webpage.pyi` & `ralium-0.3.4/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/window.py` & `ralium-0.3.4/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium/window.pyi` & `ralium-0.3.4/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-0.3.3/ralium.egg-info/PKG-INFO` & `ralium-0.3.4/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 0.3.3
+Version: 0.3.4
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-0.3.3/ralium.egg-info/SOURCES.txt` & `ralium-0.3.4/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

