# Comparing `tmp/xontrib-cmd-durations-0.3.1.tar.gz` & `tmp/xontrib-cmd-durations-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-cmd-durations-0.3.1.tar", last modified: Sat Apr  6 14:22:55 2024, max compression
+gzip compressed data, was "xontrib-cmd-durations-0.3.2.tar", last modified: Fri May 17 16:03:19 2024, max compression
```

## Comparing `xontrib-cmd-durations-0.3.1.tar` & `xontrib-cmd-durations-0.3.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/LICENSE
--rw-r--r--   0        0        0     1872 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/README.md
--rw-r--r--   0        0        0     1424 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4302 2024-04-06 14:22:52.677982 xontrib-cmd-durations-0.3.1/xontrib/cmd_done.py
--rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 xontrib-cmd-durations-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-17 16:03:15.085397 xontrib-cmd-durations-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1872 2024-05-17 16:03:15.085397 xontrib-cmd-durations-0.3.2/README.md
+-rw-r--r--   0        0        0     1424 2024-05-17 16:03:15.085397 xontrib-cmd-durations-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4377 2024-05-17 16:03:15.085397 xontrib-cmd-durations-0.3.2/xontrib/cmd_done.py
+-rw-r--r--   0        0        0     3002 1970-01-01 00:00:00.000000 xontrib-cmd-durations-0.3.2/PKG-INFO
```

### Comparing `xontrib-cmd-durations-0.3.1/LICENSE` & `xontrib-cmd-durations-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-cmd-durations-0.3.1/README.md` & `xontrib-cmd-durations-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `xontrib-cmd-durations-0.3.1/pyproject.toml` & `xontrib-cmd-durations-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 requires-python = ">=3.7"
 dependencies = [
     "xonsh>=0.10",
     "notify-py>=0.3.3; python_version >= \"3.6\" and python_version < \"4.0\"",
 ]
 name = "xontrib-cmd-durations"
-version = "0.3.1"
+version = "0.3.2"
 description = "Send notification once long running command is finished. Add duration PROMP_FIELD."
 readme = "README.md"
 keywords = [
     "xontrib",
     "xonsh",
 ]
 classifiers = [
```

### Comparing `xontrib-cmd-durations-0.3.1/xontrib/cmd_done.py` & `xontrib-cmd-durations-0.3.2/xontrib/cmd_done.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 from xonsh.built_ins import XSH as xsh
 
 LONG_DURATION = xsh.env.get("XONTRIB_CD_LONG_DURATION", 5)  # seconds
 TRIGGER_NOTIFICATION = xsh.env.get("XONTRIB_CD_TRIGGER_NOTIFICATION", True)
 NOTIFICATION_APP_NAME = xsh.env.get("XONTRIB_CD_NOTIFICATION_APP_NAME", xsh.env.get("TITLE", "xonsh"))
 
+if isinstance(LONG_DURATION, str):
+    LONG_DURATION = int(LONG_DURATION)
+
 
 def _term_program_mapping() -> dict:
     """The app name doesn't match the $TERMPROGRAM . This is to map equivalent ones in OSX"""
     defaults = {"iterm.app": "iTerm2", "apple_terminal": "Terminal", "vscode": "Code", "pycharm": "PyCharm",
                  "kate": "Kate"}
     maps = xsh.env.get("XONTRIB_CD_TERM_PROGRAM_MAP", defaults)
     return {key.lower(): val for key, val in maps.items()}
```

### Comparing `xontrib-cmd-durations-0.3.1/PKG-INFO` & `xontrib-cmd-durations-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-cmd-durations
-Version: 0.3.1
+Version: 0.3.2
 Summary: Send notification once long running command is finished. Add duration PROMP_FIELD.
 License: MIT
 Keywords: xontrib,xonsh
 Author-email: Noortheen Raja J <jnoortheen@gmail.com>
 Requires-Python: >=3.7
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

