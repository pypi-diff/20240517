# Comparing `tmp/minecraft-launcher-lib-6.3.tar.gz` & `tmp/minecraft-launcher-lib-6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft-launcher-lib-6.3.tar", last modified: Mon Oct 16 13:22:16 2023, max compression
+gzip compressed data, was "minecraft-launcher-lib-6.4.tar", last modified: Sat Dec  9 18:33:42 2023, max compression
```

## Comparing `minecraft-launcher-lib-6.3.tar` & `minecraft-launcher-lib-6.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 13:22:16.429748 minecraft-launcher-lib-6.3/
--rw-r--r--   0 root         (0) root         (0)     1318 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      117 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5010 2023-10-16 13:22:16.429748 minecraft-launcher-lib-6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3258 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 13:22:16.425748 minecraft-launcher-lib-6.3/minecraft_launcher_lib/
--rw-r--r--   0 root         (0) root         (0)      350 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10461 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 13:22:16.425748 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/forge_types.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/helper_types.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/install_types.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/mrpack_types.py
--rw-r--r--   0 root         (0) root         (0)      815 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/runtime_types.py
--rw-r--r--   0 root         (0) root         (0)     2587 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/shared_types.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/vanilla_launcher_types.py
--rw-r--r--   0 root         (0) root         (0)    11036 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/command.py
--rw-r--r--   0 root         (0) root         (0)     4251 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5508 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/fabric.py
--rw-r--r--   0 root         (0) root         (0)    10749 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/forge.py
--rw-r--r--   0 root         (0) root         (0)     9389 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/install.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/java_utils.py
--rw-r--r--   0 root         (0) root         (0)    14781 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/microsoft_account.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/microsoft_types.py
--rw-r--r--   0 root         (0) root         (0)     8050 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/mrpack.py
--rw-r--r--   0 root         (0) root         (0)     3607 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/natives.py
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/py.typed
--rw-r--r--   0 root         (0) root         (0)     5710 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/quilt.py
--rw-r--r--   0 root         (0) root         (0)     8028 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/runtime.py
--rw-r--r--   0 root         (0) root         (0)     3602 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/types.py
--rw-r--r--   0 root         (0) root         (0)     7274 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/utils.py
--rw-r--r--   0 root         (0) root         (0)     9062 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/vanilla_launcher.py
--rw-r--r--   0 root         (0) root         (0)        4 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 13:22:16.425748 minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5010 2023-10-16 13:22:16.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1692 2023-10-16 13:22:16.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 13:22:16.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-10-16 13:22:16.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-10-16 13:22:16.000000 minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1845 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-16 13:22:16.429748 minecraft-launcher-lib-6.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 13:22:16.429748 minecraft-launcher-lib-6.3/tests/
--rw-r--r--   0 root         (0) root         (0)    10227 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_command.py
--rw-r--r--   0 root         (0) root         (0)     2392 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     3667 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_fabric.py
--rw-r--r--   0 root         (0) root         (0)     4342 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_forge.py
--rw-r--r--   0 root         (0) root         (0)     4746 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_install.py
--rw-r--r--   0 root         (0) root         (0)     3301 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_java_utils.py
--rw-r--r--   0 root         (0) root         (0)     7813 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_microsoft_account.py
--rw-r--r--   0 root         (0) root         (0)     8500 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_mrpack.py
--rw-r--r--   0 root         (0) root         (0)     4400 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_natives.py
--rw-r--r--   0 root         (0) root         (0)     3588 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_quilt.py
--rw-r--r--   0 root         (0) root         (0)     7327 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_runtime.py
--rw-r--r--   0 root         (0) root         (0)    10207 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     8138 2023-10-16 13:21:48.000000 minecraft-launcher-lib-6.3/tests/test_vanilla_launcher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-09 18:33:42.964630 minecraft-launcher-lib-6.4/
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      117 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-12-09 18:33:42.964630 minecraft-launcher-lib-6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3258 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-09 18:33:42.960630 minecraft-launcher-lib-6.4/minecraft_launcher_lib/
+-rw-r--r--   0 root         (0) root         (0)      350 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10461 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-09 18:33:42.960630 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/forge_types.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/helper_types.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/install_types.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/mrpack_types.py
+-rw-r--r--   0 root         (0) root         (0)      815 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/runtime_types.py
+-rw-r--r--   0 root         (0) root         (0)     2587 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/shared_types.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/vanilla_launcher_types.py
+-rw-r--r--   0 root         (0) root         (0)    11036 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/command.py
+-rw-r--r--   0 root         (0) root         (0)     4594 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5508 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/fabric.py
+-rw-r--r--   0 root         (0) root         (0)    10749 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/forge.py
+-rw-r--r--   0 root         (0) root         (0)     9389 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/install.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/java_utils.py
+-rw-r--r--   0 root         (0) root         (0)    15076 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/microsoft_account.py
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/microsoft_types.py
+-rw-r--r--   0 root         (0) root         (0)     8050 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/mrpack.py
+-rw-r--r--   0 root         (0) root         (0)     3607 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/natives.py
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5727 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/quilt.py
+-rw-r--r--   0 root         (0) root         (0)     8028 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/runtime.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/types.py
+-rw-r--r--   0 root         (0) root         (0)     7274 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/vanilla_launcher.py
+-rw-r--r--   0 root         (0) root         (0)        4 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-09 18:33:42.960630 minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5061 2023-12-09 18:33:42.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-12-09 18:33:42.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-09 18:33:42.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-12-09 18:33:42.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-12-09 18:33:42.000000 minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-09 18:33:42.964630 minecraft-launcher-lib-6.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-09 18:33:42.960630 minecraft-launcher-lib-6.4/tests/
+-rw-r--r--   0 root         (0) root         (0)    10227 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_command.py
+-rw-r--r--   0 root         (0) root         (0)     2392 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_fabric.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_forge.py
+-rw-r--r--   0 root         (0) root         (0)     5366 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_install.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_java_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8918 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_microsoft_account.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_mrpack.py
+-rw-r--r--   0 root         (0) root         (0)     4400 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_natives.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_quilt.py
+-rw-r--r--   0 root         (0) root         (0)     7181 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_runtime.py
+-rw-r--r--   0 root         (0) root         (0)    10207 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8138 2023-12-09 18:33:14.000000 minecraft-launcher-lib-6.4/tests/test_vanilla_launcher.py
```

### Comparing `minecraft-launcher-lib-6.3/LICENSE` & `minecraft-launcher-lib-6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/PKG-INFO` & `minecraft-launcher-lib-6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-launcher-lib
-Version: 6.3
+Version: 6.4
 Summary: A library for creating a custom Minecraft launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://minecraft-launcher-lib.readthedocs.io/en/stable/index.html
 Project-URL: Issues, https://codeberg.org/JakobDev/minecraft-launcher-lib/issues
 Project-URL: Source, https://codeberg.org/JakobDev/minecraft-launcher-lib
 Project-URL: Changelog, https://minecraft-launcher-lib.readthedocs.io/en/stable/changelog.html
@@ -22,14 +22,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `minecraft-launcher-lib-6.3/README.md` & `minecraft-launcher-lib-6.4/README.md`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/_helper.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/_helper.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/forge_types.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/forge_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/mrpack_types.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/mrpack_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/runtime_types.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/runtime_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/_internal_types/shared_types.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/_internal_types/shared_types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/command.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/command.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/exceptions.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -123,7 +123,15 @@
 
 class PlatformNotSupported(Exception):
     """
     Raised, when the current Platform is not supported by a feature
     """
     def __init__(self) -> None:
         super().__init__("Your Platform is not supported")
+
+
+class AccountNotOwnMinecraft(Exception):
+    """
+    Raised by :func:`~minecraft_launcher_lib.microsoft_account.complete_login` and :func:`~minecraft_launcher_lib.microsoft_account.complete_login` when the Account does not own Minecraft
+    """
+    def __init__(self) -> None:
+        super().__init__("This Account does not own Minecraft")
```

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/fabric.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/fabric.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/forge.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/forge.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/install.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/install.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/java_utils.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/java_utils.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/microsoft_account.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/microsoft_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 microsoft_account contains functions for login with a Microsoft Account. Before using this module you need to `create a Azure application <https://docs.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app>`_.
 Many thanks to wiki.vg for it's `documentation of the login process <https://wiki.vg/Microsoft_Authentication_Scheme>`_.
 You may want to read the :doc:`/tutorial/microsoft_login` tutorial before using this module.
 For a list of all types see :doc:`microsoft_types`.
 """
 from .microsoft_types import AuthorizationTokenResponse, XBLResponse, XSTSResponse, MinecraftAuthenticateResponse, MinecraftStoreResponse, MinecraftProfileResponse, CompleteLoginResponse
-from .exceptions import InvalidRefreshToken, AzureAppNotPermitted
+from .exceptions import InvalidRefreshToken, AzureAppNotPermitted, AccountNotOwnMinecraft
 from ._helper import get_user_agent, assert_func
 from typing import Literal, Optional, Tuple, cast
 from base64 import urlsafe_b64encode
 from hashlib import sha256
 import urllib.parse
 import requests
 import secrets
@@ -297,14 +297,15 @@
 
     :param client_id: The Client ID of your Azure App
     :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
     :param redirect_uri: The Redirect URI of your Azure App
     :param auth_code: The Code you get from :func:`parse_auth_code_url`
     :param code_verifier: The 3rd entry in the Tuple you get from :func:`get_secure_login_data`
     :raises AzureAppNotPermitted: Your Azure App don't have the Permission to use the Minecraft API
+    :raises AccountNotOwnMinecraft: The Account does not own Minecraft
 
     It returns the following:
 
     .. code:: json
 
         {
             "id" : "The uuid",
@@ -334,15 +335,20 @@
     account_request = authenticate_with_minecraft(userhash, xsts_token)
 
     if "access_token" not in account_request:
         raise AzureAppNotPermitted()
 
     access_token = account_request["access_token"]
 
-    profile = cast(CompleteLoginResponse, get_profile(access_token))
+    profile = get_profile(access_token)
+
+    if "error" in profile and profile["error"] == "NOT_FOUND":
+        raise AccountNotOwnMinecraft()
+
+    profile = cast(CompleteLoginResponse, profile)
 
     profile["access_token"] = account_request["access_token"]
     profile["refresh_token"] = token_request["refresh_token"]
 
     return profile
 
 
@@ -351,16 +357,15 @@
     Do the complete login process with a refresh token. It returns the same as :func:`complete_login`.
 
     :param client_id: The Client ID of your Azure App
     :param client_secret: The Client Secret of your Azure App. This is deprecated and should not been used anymore.
     :param redirect_uri: The Redirect URI of Azure App. This Parameter only exists for backwards compatibility and is not used anymore.
     :param refresh_token: Your refresh token
     :raises InvalidRefreshToken: Your refresh token is not valid
-
-    Raises a :class:`~minecraft_launcher_lib.exceptions.InvalidRefreshToken` exception when the refresh token is invalid.
+    :raises AccountNotOwnMinecraft: The Account does not own Minecraft
     """
     token_request = refresh_authorization_token(client_id, client_secret, redirect_uri, refresh_token)
 
     if "error" in token_request:
         raise InvalidRefreshToken()
 
     token = token_request["access_token"]
@@ -371,13 +376,18 @@
 
     xsts_request = authenticate_with_xsts(xbl_token)
     xsts_token = xsts_request["Token"]
 
     account_request = authenticate_with_minecraft(userhash, xsts_token)
     access_token = account_request["access_token"]
 
-    profile = cast(CompleteLoginResponse, get_profile(access_token))
+    profile = get_profile(access_token)
+
+    if "error" in profile and profile["error"] == "NOT_FOUND":
+        raise AccountNotOwnMinecraft()
+
+    profile = cast(CompleteLoginResponse, profile)
 
     profile["access_token"] = account_request["access_token"]
     profile["refresh_token"] = token_request["refresh_token"]
 
     return profile
```

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/microsoft_types.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/microsoft_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,12 +69,14 @@
 
 
 class MinecraftProfileResponse(TypedDict):
     id: str
     name: str
     skins: List[_MinecraftProfileSkin]
     capes: List[_MinecraftProfileCape]
+    error: str
+    errorMessage: str
 
 
 class CompleteLoginResponse(MinecraftProfileResponse):
     access_token: str
     refresh_token: str
```

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/mrpack.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/mrpack.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/natives.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/natives.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/quilt.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/quilt.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     """
     Checks if a Minecraft version supported by Quilt
 
     :param version: A vanilla version
     """
     minecraft_versions = get_all_minecraft_versions()
     for i in minecraft_versions:
+        print(i)
         if i["version"] == version:
             return True
     return False
 
 
 def get_all_loader_versions() -> List[QuiltLoader]:
     """
```

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/runtime.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/runtime.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/types.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/types.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/utils.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/utils.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib/vanilla_launcher.py` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib/vanilla_launcher.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/PKG-INFO` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-launcher-lib
-Version: 6.3
+Version: 6.4
 Summary: A library for creating a custom Minecraft launcher
 Author-email: JakobDev <jakobdev@gmx.de>
 License: BSD-2-Clause
 Project-URL: Documentation, https://minecraft-launcher-lib.readthedocs.io/en/stable/index.html
 Project-URL: Issues, https://codeberg.org/JakobDev/minecraft-launcher-lib/issues
 Project-URL: Source, https://codeberg.org/JakobDev/minecraft-launcher-lib
 Project-URL: Changelog, https://minecraft-launcher-lib.readthedocs.io/en/stable/changelog.html
@@ -22,14 +22,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `minecraft-launcher-lib-6.3/minecraft_launcher_lib.egg-info/SOURCES.txt` & `minecraft-launcher-lib-6.4/minecraft_launcher_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/pyproject.toml` & `minecraft-launcher-lib-6.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -25,14 +25,15 @@
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Typing :: Typed"
 ]
 dependencies = [
   "requests"
@@ -46,8 +47,12 @@
 Changelog = "https://minecraft-launcher-lib.readthedocs.io/en/stable/changelog.html"
 Donation = "https://ko-fi.com/jakobdev"
 
 [tool.setuptools.dynamic]
 version = { file = "minecraft_launcher_lib/version.txt" }
 
 [tool.pytest.ini_options]
+addopts = "-v --basetemp=pytest-temp --durations=10 --cov=minecraft_launcher_lib --cov-report html --cov-report term --cov-report term-missing"
 testpaths = ["tests"]
+
+[tool.mypy]
+modules = ["minecraft_launcher_lib"]
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_command.py` & `minecraft-launcher-lib-6.4/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/tests/test_exceptions.py` & `minecraft-launcher-lib-6.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/tests/test_fabric.py` & `minecraft-launcher-lib-6.4/tests/test_fabric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from ._test_helper import prepare_test_versions, get_test_callbacks
+from ._test_helper import prepare_test_versions, get_test_callbacks, prepare_requests_mock
 import minecraft_launcher_lib
+import pytest_subtests
 import requests_mock
 import subprocess
 import platform
 import pathlib
 import pytest
 import shutil
 
@@ -45,34 +46,39 @@
     assert isinstance(minecraft_launcher_lib.fabric.get_latest_loader_version(), str)
 
 
 def test_fabric_get_latest_installer_version() -> None:
     assert isinstance(minecraft_launcher_lib.fabric.get_latest_installer_version(), str)
 
 
-def test_install_fabric(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
+def test_install_fabric(monkeypatch: pytest.MonkeyPatch, subtests: pytest_subtests.SubTests, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
     monkeypatch.setattr(minecraft_launcher_lib.fabric, "is_minecraft_version_supported", lambda version: True if version == "test1" else False)
     monkeypatch.setattr(minecraft_launcher_lib.fabric, "get_latest_installer_version", lambda: "testinstaller")
     monkeypatch.setattr(minecraft_launcher_lib.fabric, "get_latest_loader_version", lambda: "testloader")
     monkeypatch.setattr(subprocess, "run", lambda cmd, **kwargs: subprocess.CompletedProcess([], 0))
     monkeypatch.setattr(platform, "system", lambda: "Linux")
 
     requests_mock.get("https://maven.fabricmc.net/net/fabricmc/fabric-installer/testinstaller/fabric-installer-testinstaller.jar")
     requests_mock.real_http = True
 
     prepare_test_versions(tmp_path)
+    prepare_requests_mock(requests_mock)
 
     shutil.copytree(tmp_path / "versions" / "test1", tmp_path / "versions" / "fabric-loader-testloader-test1")
     (tmp_path / "versions" / "fabric-loader-testloader-test1" / "test1.json").rename(tmp_path / "versions" / "fabric-loader-testloader-test1" / "fabric-loader-testloader-test1.json")
 
-    minecraft_launcher_lib.fabric.install_fabric("test1", tmp_path, callback=get_test_callbacks())
+    with subtests.test("Install"):
+        minecraft_launcher_lib.fabric.install_fabric("test1", tmp_path, callback=get_test_callbacks())
 
-    monkeypatch.setattr(subprocess, "run", lambda cmd, **kwargs: subprocess.CompletedProcess([], 1))
+    with subtests.test("ExternalProgramError"):
+        monkeypatch.setattr(subprocess, "run", lambda cmd, **kwargs: subprocess.CompletedProcess([], 1))
 
-    with pytest.raises(minecraft_launcher_lib.exceptions.ExternalProgramError):
-        minecraft_launcher_lib.fabric.install_fabric("test1", tmp_path)
+        with pytest.raises(minecraft_launcher_lib.exceptions.ExternalProgramError):
+            minecraft_launcher_lib.fabric.install_fabric("test1", tmp_path)
 
-    with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
-        minecraft_launcher_lib.fabric.install_fabric("natives", tmp_path)
-
-    with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
-        minecraft_launcher_lib.fabric.install_fabric("invalid", tmp_path)
+    with subtests.test("UnsupportedVersion"):
+        with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
+            minecraft_launcher_lib.fabric.install_fabric("natives", tmp_path)
+
+    with subtests.test("VersionNotFound"):
+        with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
+            minecraft_launcher_lib.fabric.install_fabric("invalid", tmp_path)
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_forge.py` & `minecraft-launcher-lib-6.4/tests/test_forge.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._test_helper import prepare_test_versions, get_test_callbacks
+from ._test_helper import prepare_test_versions, get_test_callbacks, prepare_requests_mock
 import minecraft_launcher_lib
 import requests_mock
 import subprocess
 import platform
 import zipfile
 import pathlib
 import pytest
@@ -25,14 +25,15 @@
     requests_mock.real_http = True
 
     monkeypatch.setattr(platform, "system", lambda: "Linux")
     monkeypatch.setattr(platform, "architecture", lambda: ("64bit", "ELF"))
     monkeypatch.setattr(subprocess, "run", lambda cmd, **kwargs: None)
 
     prepare_test_versions(tmp_path)
+    prepare_requests_mock(requests_mock)
 
     minecraft_launcher_lib.forge.install_forge_version("forgetest1", tmp_path, callback=get_test_callbacks())
     minecraft_launcher_lib.forge.install_forge_version("forgetest2", tmp_path, callback=get_test_callbacks())
 
     assert (tmp_path / "libraries" / "net" / "minecraftforge" / "forge" / "forgetest1" / "forge-forgetest1.jar").is_file()
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_install.py` & `minecraft-launcher-lib-6.4/tests/test_install.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,57 +13,69 @@
 
     assert os.path.getsize(path) == size
 
     with open(path, "rb") as f:
         assert hashlib.sha1(f.read()).hexdigest() == hash
 
 
-def test_install_minecraft_version(monkeypatch: pytest.MonkeyPatch, tmp_path: pathlib.Path) -> None:
+def test_install_minecraft_version(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
     monkeypatch.setattr(platform, "system", lambda: "Linux")
 
     prepare_test_versions(tmp_path)
+    prepare_requests_mock(requests_mock)
 
     minecraft_launcher_lib.install.install_minecraft_version("test1", tmp_path)
 
-    _assert_downloaded_file(tmp_path / "libraries" / "ca" / "weblite" / "java-objc-bridge" / "1.1" / "java-objc-bridge-1.1.jar", 1318, "c02d7272de43e27c6b12b288d037608cc6d37f15")
-    _assert_downloaded_file(tmp_path / "libraries" / "org" / "slf4j" / "slf4j-api" / "2.0.1" / "slf4j-api-2.0.1.jar", 117, "c55c4428b2bec60461d3416b17a54fa8cfe20677")
+    _assert_downloaded_file(tmp_path / "libraries" / "ca" / "weblite" / "java-objc-bridge" / "1.1" / "java-objc-bridge-1.1.jar", 25, "2f8a26755f00bc8dc54cbf5e613f6d00f02a099e")
+    _assert_downloaded_file(tmp_path / "libraries" / "org" / "slf4j" / "slf4j-api" / "2.0.1" / "slf4j-api-2.0.1.jar", 20, "03b7e695aa5cd7ca418ee6710e304d64d0491929")
     _assert_downloaded_file(tmp_path / "assets" / "log_configs" / "client-1.12.xml", 888, "bd65e7d2e3c237be76cfbef4c2405033d7f91521")
-    _assert_downloaded_file(tmp_path / "versions" / "test1" / "test1.jar", 3259, "1a34a92bf766c61eb83edaf7ff632cf0c862f958")
+    _assert_downloaded_file(tmp_path / "versions" / "test1" / "test1.jar", 7, "173219a75174abb3e3a7bfd36148129df03f9123")
 
 
 def test_install_minecraft_version_assets(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
     monkeypatch.setattr(platform, "system", lambda: "Linux")
 
     prepare_test_versions(tmp_path)
-
     prepare_requests_mock(requests_mock)
 
     minecraft_launcher_lib.install.install_minecraft_version("assets", tmp_path)
 
     assert (tmp_path / "assets" / "objects" / "86" / "86f7e437faa5a7fce15d1ddcb9eaeaea377667b8").is_file()
     assert (tmp_path / "assets" / "objects" / "e9" / "e9d71f5ee7c92d6dc9e92ffdad17b8bd49418f98").is_file()
     assert (tmp_path / "assets" / "objects" / "84" / "84a516841ba77a5b4648de2cd0dfcb30ea46dbb4").is_file()
     assert os.listdir(tmp_path / "assets" / "log_configs") == ["client-1.12.xml"]
     assert os.listdir(tmp_path / "assets" / "indexes") == ["test.json"]
     assert len(os.listdir(tmp_path / "assets" / "objects")) == 3
 
 
-def test_install_minecraft_version_inherit(monkeypatch: pytest.MonkeyPatch, tmp_path: pathlib.Path) -> None:
+def test_install_minecraft_version_runtime(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
     monkeypatch.setattr(platform, "system", lambda: "Linux")
 
     prepare_test_versions(tmp_path)
+    prepare_requests_mock(requests_mock)
+
+    minecraft_launcher_lib.install.install_minecraft_version("runtime", tmp_path)
+
+    assert (tmp_path / "runtime" / "java-runtime-test" / "linux" / ".version").read_text().strip() == "17.0.3"
+
+
+def test_install_minecraft_version_inherit(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
+    monkeypatch.setattr(platform, "system", lambda: "Linux")
+
+    prepare_test_versions(tmp_path)
+    prepare_requests_mock(requests_mock)
 
     minecraft_launcher_lib.install.install_minecraft_version("inherit", tmp_path)
 
-    _assert_downloaded_file(tmp_path / "libraries" / "ca" / "weblite" / "java-objc-bridge" / "1.1" / "java-objc-bridge-1.1.jar", 1318, "c02d7272de43e27c6b12b288d037608cc6d37f15")
-    _assert_downloaded_file(tmp_path / "libraries" / "org" / "slf4j" / "slf4j-api" / "2.0.1" / "slf4j-api-2.0.1.jar", 117, "c55c4428b2bec60461d3416b17a54fa8cfe20677")
-    _assert_downloaded_file(tmp_path / "libraries" / "com" / "ibm" / "icu" / "icu4j" / "71.1" / "icu4j-71.1.jar", 1318, "c02d7272de43e27c6b12b288d037608cc6d37f15")
+    _assert_downloaded_file(tmp_path / "libraries" / "ca" / "weblite" / "java-objc-bridge" / "1.1" / "java-objc-bridge-1.1.jar", 25, "2f8a26755f00bc8dc54cbf5e613f6d00f02a099e")
+    _assert_downloaded_file(tmp_path / "libraries" / "org" / "slf4j" / "slf4j-api" / "2.0.1" / "slf4j-api-2.0.1.jar", 20, "03b7e695aa5cd7ca418ee6710e304d64d0491929")
+    _assert_downloaded_file(tmp_path / "libraries" / "com" / "ibm" / "icu" / "icu4j" / "71.1" / "icu4j-71.1.jar", 14, "78ef2a15d1afad3e435cdcaf12c502ac290ca707")
     _assert_downloaded_file(tmp_path / "assets" / "log_configs" / "client-1.12.xml", 888, "bd65e7d2e3c237be76cfbef4c2405033d7f91521")
-    _assert_downloaded_file(tmp_path / "versions" / "inherit" / "inherit.jar", 3259, "1a34a92bf766c61eb83edaf7ff632cf0c862f958")
-    _assert_downloaded_file(tmp_path / "versions" / "test1" / "test1.jar", 3259, "1a34a92bf766c61eb83edaf7ff632cf0c862f958")
+    _assert_downloaded_file(tmp_path / "versions" / "inherit" / "inherit.jar", 7, "173219a75174abb3e3a7bfd36148129df03f9123")
+    _assert_downloaded_file(tmp_path / "versions" / "test1" / "test1.jar", 7, "173219a75174abb3e3a7bfd36148129df03f9123")
 
 
 def test_install_minecraft_version_extended(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
     monkeypatch.setattr(platform, "system", lambda: "Linux")
 
     prepare_test_versions(tmp_path)
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_java_utils.py` & `minecraft-launcher-lib-6.4/tests/test_java_utils.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/tests/test_microsoft_account.py` & `minecraft-launcher-lib-6.4/tests/test_microsoft_account.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         self._mode = mode
 
     def get(self, url: str, **kwargs: dict) -> MicrosoftRequestsResponseMock:
         if url == "https://api.minecraftservices.com/minecraft/profile":
             if kwargs["headers"]["Authorization"] != "Bearer minecraft_access_token":
                 return MicrosoftRequestsResponseMock(500, {})
 
+            if self._mode == "not_own_minecraft":
+                return MicrosoftRequestsResponseMock(400, {"error": "NOT_FOUND", "errorMessage": "Not Found"})
+
             return MicrosoftRequestsResponseMock(200, {"id": "minecraft_uuid", "name": "minecraft_name", "skins": [], "capes": []})
 
         elif url == "https://api.minecraftservices.com/entitlements/mcstore":
             if kwargs["headers"]["Authorization"] != "Bearer minecraft_access_token":
                 return MicrosoftRequestsResponseMock(500, {})
 
             return MicrosoftRequestsResponseMock(200, {"items": [], "signature": "jwt sig", "keyId": "1"})
@@ -133,14 +136,24 @@
 
     assert login_data["id"] == "minecraft_uuid"
     assert login_data["name"] == "minecraft_name"
     assert login_data["access_token"] == "minecraft_access_token"
     assert login_data["refresh_token"] == "refresh_token"
 
 
+def test_complete_login_not_own_minecraft(monkeypatch: pytest.MonkeyPatch) -> None:
+    requests_mock = MicrosoftRequestsMock("not_own_minecraft")
+
+    monkeypatch.setattr(requests, "get", requests_mock.get)
+    monkeypatch.setattr(requests, "post", requests_mock.post)
+
+    with pytest.raises(minecraft_launcher_lib.exceptions.AccountNotOwnMinecraft):
+        minecraft_launcher_lib.microsoft_account.complete_login("client_id", None, "redirect_url", "auth_code")
+
+
 def test_complete_login_not_permitted_azure_app(monkeypatch: pytest.MonkeyPatch) -> None:
     requests_mock = MicrosoftRequestsMock("not_permitted_app")
 
     monkeypatch.setattr(requests, "get", requests_mock.get)
     monkeypatch.setattr(requests, "post", requests_mock.post)
 
     with pytest.raises(minecraft_launcher_lib.exceptions.AzureAppNotPermitted):
@@ -157,14 +170,24 @@
 
     assert login_data["id"] == "minecraft_uuid"
     assert login_data["name"] == "minecraft_name"
     assert login_data["access_token"] == "minecraft_access_token"
     assert login_data["refresh_token"] == "refresh_token"
 
 
+def test_complete_refresh_not_own_minecraft(monkeypatch: pytest.MonkeyPatch) -> None:
+    requests_mock = MicrosoftRequestsMock("not_own_minecraft")
+
+    monkeypatch.setattr(requests, "get", requests_mock.get)
+    monkeypatch.setattr(requests, "post", requests_mock.post)
+
+    with pytest.raises(minecraft_launcher_lib.exceptions.AccountNotOwnMinecraft):
+        minecraft_launcher_lib.microsoft_account.complete_refresh("client_id", "client_secret", None, "refresh_token")
+
+
 def test_complete_refresh_invalid_token(monkeypatch: pytest.MonkeyPatch) -> None:
     requests_mock = MicrosoftRequestsMock("default")
 
     monkeypatch.setattr(requests, "get", requests_mock.get)
     monkeypatch.setattr(requests, "post", requests_mock.post)
 
     with pytest.raises(minecraft_launcher_lib.exceptions.InvalidRefreshToken):
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_mrpack.py` & `minecraft-launcher-lib-6.4/tests/test_mrpack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from ._test_helper import prepare_test_versions, get_test_callbacks
+from ._test_helper import prepare_test_versions, get_test_callbacks, prepare_requests_mock
 from typing import List, Dict, Any
 import minecraft_launcher_lib
+import pytest_subtests
+import requests_mock
 import requests
 import hashlib
 import pathlib
 import zipfile
 import random
 import pytest
 import json
@@ -66,54 +68,56 @@
         "name": "Test",
         "versionId": "minecraft-launcher-lib.test",
         "files": [
             {
                 **{
                     "path": "a.txt"
                 },
-                **_generate_test_file("https://example.com")
+                **_generate_test_file("minecraft-launcher-lib-test://text.txt")
             },
             {
                 **{
                     "path": "b.txt",
                     "env": {
                         "client": "required",
                         "server": "required"
                     }
                 },
-                **_generate_test_file("https://example.com")
+                **_generate_test_file("minecraft-launcher-lib-test://text.txt")
             },
             {
                 **{
                     "path": "c.txt",
                     "env": {
                         "client": "optional",
                         "server": "optional"
                     }
                 },
-                **_generate_test_file("https://example.com")
+                **_generate_test_file("minecraft-launcher-lib-test://text.txt")
             },
             {
                 **{
                     "path": "d.txt",
                     "env": {
                         "client": "unsupported",
                         "server": "unsupported"
                     }
                 },
-                **_generate_test_file("https://example.com")
+                **_generate_test_file("minecraft-launcher-lib-test://text.txt")
             },
         ],
         "dependencies": {
             "minecraft": "test1"
         }
     }
 
 
-def test_get_mrpack_information(tmp_path: pathlib.Path) -> None:
+def test_get_mrpack_information(requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
+    prepare_requests_mock(requests_mock)
+
     index = _get_test_index()
 
     # Test without summary
     info = minecraft_launcher_lib.mrpack.get_mrpack_information(_create_test_index_pack(index, tmp_path))
 
     assert info["name"] == "Test"
     assert info["summary"] == ""
@@ -125,90 +129,99 @@
     # Test with summary
     index["summary"] = "Summary"
     info_summary = minecraft_launcher_lib.mrpack.get_mrpack_information(_create_test_index_pack(index, tmp_path))
 
     assert info_summary["summary"] == "Summary"
 
 
-def test_install_mrpack(tmp_path) -> None:
+def test_install_mrpack(subtests: pytest_subtests.SubTests, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
+    prepare_requests_mock(requests_mock)
+
     index = _get_test_index()
 
-    # Test without Optional File
-    first_dir = _create_test_dir(tmp_path)
-    minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path), first_dir, mrpack_install_options={"skipDependenciesInstall": True})
-    assert sorted(os.listdir(first_dir)) == sorted(["a.txt", "b.txt"])
-
-    # Test with Optional File
-    second_dir = _create_test_dir(tmp_path)
-    minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path), second_dir, mrpack_install_options={"skipDependenciesInstall": True, "optionalFiles": ["c.txt"]})
-    assert sorted(os.listdir(second_dir)) == sorted(["a.txt", "b.txt", "c.txt"])
-
-    # Test overides
-    third_dir = _create_test_dir(tmp_path)
-    minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path, overrides=["overrides.txt"], client_overrides=["client/test.txt"]), third_dir, mrpack_install_options={"skipDependenciesInstall": True})
-    assert sorted(os.listdir(third_dir)) == sorted(["a.txt", "b.txt", "overrides.txt", "client"])
-    assert sorted(os.listdir(os.path.join(third_dir, "client"))) == sorted(["test.txt"])
-
-    # Test FileOutsideMinecraftDirectory Exception with Files
-    fourth_dir = _create_test_dir(tmp_path)
-    exception_index = copy.deepcopy(index)
-    exception_index["files"].append({**{
-        "path": "../error.txt"
-    },
-        **_generate_test_file("https://example.com")
-    })
-    with pytest.raises(minecraft_launcher_lib.exceptions.FileOutsideMinecraftDirectory):
-        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(exception_index, tmp_path), fourth_dir, mrpack_install_options={"skipDependenciesInstall": True})
-
-    # Test FileOutsideMinecraftDirectory Exception with Overrides
-    fifth_dir = _create_test_dir(tmp_path)
-    with pytest.raises(minecraft_launcher_lib.exceptions.FileOutsideMinecraftDirectory):
-        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path, overrides=["../overrides.txt"]), fifth_dir, mrpack_install_options={"skipDependenciesInstall": True})
-
-    # Test with Modpack directory
-    sixth_dir = _create_test_dir(tmp_path)
-    modpack_dir = _create_test_dir(tmp_path)
-    minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path), sixth_dir, modpack_directory=modpack_dir, mrpack_install_options={"skipDependenciesInstall": True})
-    assert sorted(os.listdir(modpack_dir)) == sorted(["a.txt", "b.txt"])
-    assert not os.path.isdir(sixth_dir)
-
-    # Test with forge install
-    forge_dir = _create_test_dir(tmp_path)
-    forge_index = copy.deepcopy(index)
-    forge_index["dependencies"]["forge"] = "invalid"
-    prepare_test_versions(forge_dir)
-    with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
-        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(forge_index, tmp_path), forge_dir, callback=get_test_callbacks())
-
-    # Test with fabric install
-    fabric_dir = _create_test_dir(tmp_path)
-    fabric_index = copy.deepcopy(index)
-    fabric_index["dependencies"]["fabric-loader"] = "invalid"
-    prepare_test_versions(fabric_dir)
-    with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
-        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(fabric_index, tmp_path), fabric_dir, callback=get_test_callbacks())
-
-    # Test with quilt install
-    quilt_dir = _create_test_dir(tmp_path)
-    quilt_index = copy.deepcopy(index)
-    quilt_index["dependencies"]["quilt-loader"] = "invalid"
-    prepare_test_versions(quilt_dir)
-    with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
-        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(quilt_index, tmp_path), quilt_dir, callback=get_test_callbacks())
+    with subtests.test("Without optional file"):
+        first_dir = _create_test_dir(tmp_path)
+        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path), first_dir, mrpack_install_options={"skipDependenciesInstall": True})
+        assert sorted(os.listdir(first_dir)) == sorted(["a.txt", "b.txt"])
+
+    with subtests.test("With optional file"):
+        second_dir = _create_test_dir(tmp_path)
+        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path), second_dir, mrpack_install_options={"skipDependenciesInstall": True, "optionalFiles": ["c.txt"]})
+        assert sorted(os.listdir(second_dir)) == sorted(["a.txt", "b.txt", "c.txt"])
+
+    with subtests.test("Overrides"):
+        third_dir = _create_test_dir(tmp_path)
+        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path, overrides=["overrides.txt"], client_overrides=["client/test.txt"]), third_dir, mrpack_install_options={"skipDependenciesInstall": True})
+        assert sorted(os.listdir(third_dir)) == sorted(["a.txt", "b.txt", "overrides.txt", "client"])
+        assert sorted(os.listdir(os.path.join(third_dir, "client"))) == sorted(["test.txt"])
+
+    with subtests.test("FileOutsideMinecraftDirectory Exception with files"):
+        fourth_dir = _create_test_dir(tmp_path)
+        exception_index = copy.deepcopy(index)
+        exception_index["files"].append({**{
+            "path": "../error.txt"
+        },
+            **_generate_test_file("minecraft-launcher-lib-test://text.txt")
+        })
+        with pytest.raises(minecraft_launcher_lib.exceptions.FileOutsideMinecraftDirectory):
+            minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(exception_index, tmp_path), fourth_dir, mrpack_install_options={"skipDependenciesInstall": True})
+
+    with subtests.test("FileOutsideMinecraftDirectory Exception with overrides"):
+        fifth_dir = _create_test_dir(tmp_path)
+        with pytest.raises(minecraft_launcher_lib.exceptions.FileOutsideMinecraftDirectory):
+            minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path, overrides=["../overrides.txt"]), fifth_dir, mrpack_install_options={"skipDependenciesInstall": True})
+
+    with subtests.test("Modpack directory"):
+        sixth_dir = _create_test_dir(tmp_path)
+        modpack_dir = _create_test_dir(tmp_path)
+        minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(index, tmp_path), sixth_dir, modpack_directory=modpack_dir, mrpack_install_options={"skipDependenciesInstall": True})
+        assert sorted(os.listdir(modpack_dir)) == sorted(["a.txt", "b.txt"])
+        assert not os.path.isdir(sixth_dir)
+
+    with subtests.test("Forge"):
+        forge_dir = _create_test_dir(tmp_path)
+        forge_index = copy.deepcopy(index)
+        forge_index["dependencies"]["forge"] = "invalid"
+        prepare_test_versions(forge_dir)
+        requests_mock.get("https://files.minecraftforge.net/maven/net/minecraftforge/forge/test1-invalid/forge-test1-invalid-installer.jar", status_code=404)
+        with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
+            minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(forge_index, tmp_path), forge_dir, callback=get_test_callbacks())
+
+    with subtests.test("Fabric"):
+        fabric_dir = _create_test_dir(tmp_path)
+        fabric_index = copy.deepcopy(index)
+        fabric_index["dependencies"]["fabric-loader"] = "invalid"
+        prepare_test_versions(fabric_dir)
+        with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
+            minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(fabric_index, tmp_path), fabric_dir, callback=get_test_callbacks())
+
+    with subtests.test("Quilt"):
+        quilt_dir = _create_test_dir(tmp_path)
+        quilt_index = copy.deepcopy(index)
+        quilt_index["dependencies"]["quilt-loader"] = "invalid"
+        prepare_test_versions(quilt_dir)
+        with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
+            minecraft_launcher_lib.mrpack.install_mrpack(_create_test_index_pack(quilt_index, tmp_path), quilt_dir, callback=get_test_callbacks())
+
 
+def test_mrpack_launch_version(subtests: pytest_subtests.SubTests, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
+    prepare_requests_mock(requests_mock)
 
-def test_mrpack_launch_version(tmp_path) -> None:
     index = _get_test_index()
 
-    assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "test1"
+    with subtests.test("Vanilla"):
+        assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "test1"
 
-    index["dependencies"]["forge"] = "41.1.0"
-    assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "test1-forge-41.1.0"
-    del index["dependencies"]["forge"]
-
-    index["dependencies"]["fabric-loader"] = "0.14.15"
-    assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "fabric-loader-0.14.15-test1"
-    del index["dependencies"]["fabric-loader"]
-
-    index["dependencies"]["quilt-loader"] = "0.18.2"
-    assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "quilt-loader-0.18.2-test1"
-    del index["dependencies"]["quilt-loader"]
+    with subtests.test("Forge"):
+        index["dependencies"]["forge"] = "41.1.0"
+        assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "test1-forge-41.1.0"
+        del index["dependencies"]["forge"]
+
+    with subtests.test("Fabric"):
+        index["dependencies"]["fabric-loader"] = "0.14.15"
+        assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "fabric-loader-0.14.15-test1"
+        del index["dependencies"]["fabric-loader"]
+
+    with subtests.test("Quilt"):
+        index["dependencies"]["quilt-loader"] = "0.18.2"
+        assert minecraft_launcher_lib.mrpack.get_mrpack_launch_version(_create_test_index_pack(index, tmp_path)) == "quilt-loader-0.18.2-test1"
+        del index["dependencies"]["quilt-loader"]
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_natives.py` & `minecraft-launcher-lib-6.4/tests/test_natives.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/tests/test_quilt.py` & `minecraft-launcher-lib-6.4/tests/test_quilt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,51 @@
-from ._test_helper import prepare_test_versions, get_test_callbacks
+from ._test_helper import prepare_test_versions, get_test_callbacks, prepare_requests_mock
 import minecraft_launcher_lib
+import pytest_subtests
 import requests_mock
 import subprocess
 import platform
 import pathlib
 import pytest
 import shutil
 
 
-def test_quilt_get_all_minecraft_versions() -> None:
+def test_quilt_get_all_minecraft_versions(requests_mock: requests_mock.Mocker) -> None:
+    prepare_requests_mock(requests_mock)
+
     version_list = minecraft_launcher_lib.quilt.get_all_minecraft_versions()
     for i in version_list:
         assert isinstance(i["version"], str)
         assert isinstance(i["stable"], bool)
 
 
-def test_quilt_get_stable_minecraft_versions() -> None:
+def test_quilt_get_stable_minecraft_versions(requests_mock: requests_mock.Mocker) -> None:
+    prepare_requests_mock(requests_mock)
+
     version_list = minecraft_launcher_lib.quilt.get_stable_minecraft_versions()
     assert isinstance(version_list[0], str)
 
 
-def test_quilt_get_latest_minecraft_version() -> None:
-    assert isinstance(minecraft_launcher_lib.quilt.get_latest_minecraft_version(), str)
+def test_quilt_get_latest_minecraft_version(requests_mock: requests_mock.Mocker) -> None:
+    prepare_requests_mock(requests_mock)
+
+    assert minecraft_launcher_lib.quilt.get_latest_minecraft_version() == "unstable"
 
 
-def test_quilt_get_latest_stable_minecraft_version() -> None:
-    assert isinstance(minecraft_launcher_lib.quilt.get_latest_stable_minecraft_version(), str)
+def test_quilt_get_latest_stable_minecraft_version(requests_mock: requests_mock.Mocker) -> None:
+    prepare_requests_mock(requests_mock)
 
+    assert minecraft_launcher_lib.quilt.get_latest_stable_minecraft_version() == "test2"
 
-def test_quilt_is_minecraft_version_supported() -> None:
-    assert minecraft_launcher_lib.quilt.is_minecraft_version_supported("1.16") is True
-    assert minecraft_launcher_lib.quilt.is_minecraft_version_supported("1.0") is False
+
+def test_quilt_is_minecraft_version_supported(requests_mock: requests_mock.Mocker) -> None:
+    prepare_requests_mock(requests_mock)
+
+    assert minecraft_launcher_lib.quilt.is_minecraft_version_supported("test2") is True
+    assert minecraft_launcher_lib.quilt.is_minecraft_version_supported("test1") is False
 
 
 def test_quilt_get_all_loader_versions() -> None:
     version_list = minecraft_launcher_lib.quilt.get_all_loader_versions()
     for i in version_list:
         assert isinstance(i["separator"], str)
         assert isinstance(i["build"], int)
@@ -46,34 +57,39 @@
     assert isinstance(minecraft_launcher_lib.quilt.get_latest_loader_version(), str)
 
 
 def test_quilt_get_latest_installer_version() -> None:
     assert isinstance(minecraft_launcher_lib.quilt.get_latest_installer_version(), str)
 
 
-def test_install_quilt(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
+def test_install_quilt(monkeypatch: pytest.MonkeyPatch, subtests: pytest_subtests.SubTests, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
     monkeypatch.setattr(minecraft_launcher_lib.quilt, "is_minecraft_version_supported", lambda version: True if version == "test1" else False)
     monkeypatch.setattr(minecraft_launcher_lib.quilt, "get_latest_installer_version", lambda: "testinstaller")
     monkeypatch.setattr(minecraft_launcher_lib.quilt, "get_latest_loader_version", lambda: "testloader")
     monkeypatch.setattr(subprocess, "run", lambda cmd, **kwargs: subprocess.CompletedProcess([], 0))
     monkeypatch.setattr(platform, "system", lambda: "Linux")
 
     requests_mock.get("https://maven.quiltmc.org/repository/release/org/quiltmc/quilt-installer/testinstaller/quilt-installer-testinstaller.jar")
     requests_mock.real_http = True
 
     prepare_test_versions(tmp_path)
+    prepare_requests_mock(requests_mock)
 
     shutil.copytree(tmp_path / "versions" / "test1", tmp_path / "versions" / "quilt-loader-testloader-test1")
     (tmp_path / "versions" / "quilt-loader-testloader-test1" / "test1.json").rename(tmp_path / "versions" / "quilt-loader-testloader-test1" / "quilt-loader-testloader-test1.json")
 
-    minecraft_launcher_lib.quilt.install_quilt("test1", tmp_path, callback=get_test_callbacks())
-
-    monkeypatch.setattr(subprocess, "run", lambda cmd, **kwargs: subprocess.CompletedProcess([], 1))
+    with subtests.test("Install"):
+        minecraft_launcher_lib.quilt.install_quilt("test1", tmp_path, callback=get_test_callbacks())
 
-    with pytest.raises(minecraft_launcher_lib.exceptions.ExternalProgramError):
-        minecraft_launcher_lib.quilt.install_quilt("test1", tmp_path)
+    with subtests.test("ExternalProgramError"):
+        monkeypatch.setattr(subprocess, "run", lambda cmd, **kwargs: subprocess.CompletedProcess([], 1))
 
-    with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
-        minecraft_launcher_lib.quilt.install_quilt("natives", tmp_path)
+        with pytest.raises(minecraft_launcher_lib.exceptions.ExternalProgramError):
+            minecraft_launcher_lib.quilt.install_quilt("test1", tmp_path)
 
-    with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
-        minecraft_launcher_lib.quilt.install_quilt("invalid", tmp_path)
+    with subtests.test("UnsupportedVersion"):
+        with pytest.raises(minecraft_launcher_lib.exceptions.UnsupportedVersion):
+            minecraft_launcher_lib.quilt.install_quilt("natives", tmp_path)
+
+    with subtests.test("VersionNotFound"):
+        with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
+            minecraft_launcher_lib.quilt.install_quilt("invalid", tmp_path)
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_runtime.py` & `minecraft-launcher-lib-6.4/tests/test_runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from ._test_helper import prepare_requests_mock
 import minecraft_launcher_lib
+import pytest_subtests
 import requests_mock
 import subprocess
 import platform
 import datetime
 import pathlib
 import pytest
-import json
 import os
 
 
 def test_get_jvm_runtimes() -> None:
     runtime_list = minecraft_launcher_lib.runtime.get_jvm_runtimes()
     for i in runtime_list:
         assert isinstance(i, str)
@@ -22,88 +23,84 @@
         os.makedirs(os.path.join(tmp_path, "runtime", i))
 
     runtime_list = minecraft_launcher_lib.runtime.get_installed_jvm_runtimes(tmp_path)
     runtime_list.sort()
     assert runtime_list == ["a", "b", "c"]
 
 
-def test_install_jvm_runtime(monkeypatch: pytest.MonkeyPatch, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
-    with open(os.path.join(os.path.dirname(__file__), "data", "runtime", "list.json"), "r", encoding="utf-8") as f:
-        list_data = json.load(f)
-
-    with open(os.path.join(os.path.dirname(__file__), "data", "runtime", "runtime.json"), "r", encoding="utf-8") as f:
-        runtime_data = json.load(f)
-
-    with open(os.path.join(os.path.dirname(__file__), "data", "runtime", "error.json"), "r", encoding="utf-8") as f:
-        error_data = json.load(f)
-
+def test_install_jvm_runtime(monkeypatch: pytest.MonkeyPatch, subtests: pytest_subtests.SubTests, requests_mock: requests_mock.Mocker, tmp_path: pathlib.Path) -> None:
     monkeypatch.setattr(platform, "architecture", lambda: ("test",))
     monkeypatch.setattr(platform, "system", lambda: "Linux")
 
-    requests_mock.get("https://launchermeta.mojang.com/v1/products/java-runtime/2ec0cc96c44e5a76b9c8b7c39df7210883d12871/all.json", json=list_data)
-    requests_mock.get("https://test.json", json=runtime_data)
-    requests_mock.get("https://error.json", json=error_data)
-    requests_mock.real_http = True
-
-    with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
-        minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-invalid", tmp_path)
-
-    minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-empty", tmp_path)
-
-    assert len(os.listdir(tmp_path)) == 0
-
-    # This functions needs to be patched, so the test also works on non Unix Systems
-    monkeypatch.setattr(os, "symlink", lambda target, file: pathlib.Path(file).write_text(target), raising=False)
-    monkeypatch.setattr(subprocess, "run", lambda cmd: pathlib.Path(cmd[2] + ".execute").touch() if cmd[0] == "chmod" else None)
-
-    minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-test", tmp_path)
+    prepare_requests_mock(requests_mock)
 
-    assert (tmp_path / "runtime" / "java-runtime-test" / "linux" / ".version").read_text().strip() == "17.0.3"
-    assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test.sha1")
-    assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "COPYRIGHT")
-    assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "LICENSE")
-    assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "LICENSE.execute")
-    assert os.path.isdir(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "lib" / "desktop" / "mime")
-    assert (tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "links" / "testlink").read_text().strip() == "../target"
+    with subtests.test("Empty"):
+        minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-empty", tmp_path)
 
-    # Test, if the exceptions are handeld
-    monkeypatch.setattr(subprocess, "run", lambda cmd: exec("raise FileNotFoundError()"))
-    monkeypatch.setattr(os, "symlink", lambda target, file: exec("raise Exception()"), raising=False)
-    minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-test", tmp_path)
-
-    with pytest.raises(minecraft_launcher_lib.exceptions.FileOutsideMinecraftDirectory):
-        minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-error", tmp_path)
-
-
-def test_get_executable_path(monkeypatch: pytest.MonkeyPatch, tmp_path: pathlib.Path) -> None:
-    monkeypatch.setattr(platform, "architecture", lambda: ("test",))
-    monkeypatch.setattr(platform, "system", lambda: "Linux")
-    linux_java = (tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "bin" / "java")
-    os.makedirs(linux_java.parent)
-    linux_java.touch()
-    assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-test", tmp_path) == str(linux_java)
-
-    monkeypatch.undo()
-    monkeypatch.setattr(platform, "architecture", lambda: ("test",))
-    monkeypatch.setattr(platform, "system", lambda: "Windows")
-    windows_java = (tmp_path / "runtime" / "java-runtime-test" / "windows-x64" / "java-runtime-test" / "bin" / "java.exe")
-    os.makedirs(windows_java.parent)
-    windows_java.touch()
-    assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-test", tmp_path) == str(windows_java)
-
-    monkeypatch.undo()
-    monkeypatch.setattr(platform, "machine", lambda: "arm64")
-    monkeypatch.setattr(platform, "system", lambda: "Darwin")
-    mac_java = (tmp_path / "runtime" / "java-runtime-test" / "mac-os-arm64" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "bin" / "java")
-    os.makedirs(mac_java.parent)
-    mac_java.touch()
-    assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-test", tmp_path) == str(mac_java)
+        assert len(os.listdir(tmp_path)) == 0
 
-    monkeypatch.undo()
-    assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-invalid", tmp_path) is None
+    with subtests.test("Full"):
+        # This functions needs to be patched, so the test also works on non Unix Systems
+        monkeypatch.setattr(os, "symlink", lambda target, file: pathlib.Path(file).write_text(target), raising=False)
+        monkeypatch.setattr(subprocess, "run", lambda cmd: pathlib.Path(cmd[2] + ".execute").touch() if cmd[0] == "chmod" else None)
+
+        minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-test", tmp_path)
+
+        assert (tmp_path / "runtime" / "java-runtime-test" / "linux" / ".version").read_text().strip() == "17.0.3"
+        assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test.sha1")
+        assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "COPYRIGHT")
+        assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "LICENSE")
+        assert os.path.isfile(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "LICENSE.execute")
+        assert os.path.isdir(tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "lib" / "desktop" / "mime")
+        assert (tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "links" / "testlink").read_text().strip() == "../target"
+
+    with subtests.test("Invalid"):
+        with pytest.raises(minecraft_launcher_lib.exceptions.VersionNotFound):
+            minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-invalid", tmp_path)
+
+    with subtests.test("Exceptions"):
+        # Test, if the exceptions are handeld
+        monkeypatch.setattr(subprocess, "run", lambda cmd: exec("raise FileNotFoundError()"))
+        monkeypatch.setattr(os, "symlink", lambda target, file: exec("raise Exception()"), raising=False)
+        minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-test", tmp_path)
+
+        with pytest.raises(minecraft_launcher_lib.exceptions.FileOutsideMinecraftDirectory):
+            minecraft_launcher_lib.runtime.install_jvm_runtime("java-runtime-error", tmp_path)
+
+
+def test_get_executable_path(monkeypatch: pytest.MonkeyPatch, subtests: pytest_subtests.SubTests, tmp_path: pathlib.Path) -> None:
+    with subtests.test("Linux"):
+        monkeypatch.setattr(platform, "architecture", lambda: ("test",))
+        monkeypatch.setattr(platform, "system", lambda: "Linux")
+        linux_java = (tmp_path / "runtime" / "java-runtime-test" / "linux" / "java-runtime-test" / "bin" / "java")
+        os.makedirs(linux_java.parent)
+        linux_java.touch()
+        assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-test", tmp_path) == str(linux_java)
+
+    with subtests.test("Windows"):
+        monkeypatch.undo()
+        monkeypatch.setattr(platform, "architecture", lambda: ("test",))
+        monkeypatch.setattr(platform, "system", lambda: "Windows")
+        windows_java = (tmp_path / "runtime" / "java-runtime-test" / "windows-x64" / "java-runtime-test" / "bin" / "java.exe")
+        os.makedirs(windows_java.parent)
+        windows_java.touch()
+        assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-test", tmp_path) == str(windows_java)
+
+    with subtests.test("macOS"):
+        monkeypatch.undo()
+        monkeypatch.setattr(platform, "machine", lambda: "arm64")
+        monkeypatch.setattr(platform, "system", lambda: "Darwin")
+        mac_java = (tmp_path / "runtime" / "java-runtime-test" / "mac-os-arm64" / "java-runtime-test" / "jre.bundle" / "Contents" / "Home" / "bin" / "java")
+        os.makedirs(mac_java.parent)
+        mac_java.touch()
+        assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-test", tmp_path) == str(mac_java)
+
+    with subtests.test("Invalid"):
+        monkeypatch.undo()
+        assert minecraft_launcher_lib.runtime.get_executable_path("java-runtime-invalid", tmp_path) is None
 
 
 def _test_runtime_information() -> None:
     info = minecraft_launcher_lib.runtime.get_jvm_runtime_information("java-runtime-gamma")
     assert isinstance(info["released"], datetime.datetime)
     assert isinstance(info["name"], str)
     assert len(info) == 2
```

### Comparing `minecraft-launcher-lib-6.3/tests/test_utils.py` & `minecraft-launcher-lib-6.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `minecraft-launcher-lib-6.3/tests/test_vanilla_launcher.py` & `minecraft-launcher-lib-6.4/tests/test_vanilla_launcher.py`

 * *Files identical despite different names*

