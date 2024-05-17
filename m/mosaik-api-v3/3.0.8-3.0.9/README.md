# Comparing `tmp/mosaik-api-v3-3.0.8.tar.gz` & `tmp/mosaik-api-v3-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaik-api-v3-3.0.8.tar", last modified: Mon Mar 25 10:16:04 2024, max compression
+gzip compressed data, was "mosaik-api-v3-3.0.9.tar", last modified: Thu Mar 28 14:20:53 2024, max compression
```

## Comparing `mosaik-api-v3-3.0.8.tar` & `mosaik-api-v3-3.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 10:16:04.690556 mosaik-api-v3-3.0.8/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/AUTHORS.txt
--rw-rw-rw-   0 root         (0) root         (0)     2247 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/CHANGES.txt
--rw-rw-rw-   0 root         (0) root         (0)     1080 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5665 2024-03-25 10:16:04.690556 mosaik-api-v3-3.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2015 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 10:16:04.688556 mosaik-api-v3-3.0.8/example_mas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/example_mas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2295 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/example_mas/mosaik.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 10:16:04.688556 mosaik-api-v3-3.0.8/example_sim/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/example_sim/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/example_sim/mosaik.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/example_sim/simulator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 10:16:04.689556 mosaik-api-v3-3.0.8/mosaik_api_v3/
--rw-rw-rw-   0 root         (0) root         (0)    20841 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/mosaik_api_v3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7527 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/mosaik_api_v3/connection.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/mosaik_api_v3/datetime.py
--rw-rw-rw-   0 root         (0) root         (0)     3054 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/mosaik_api_v3/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-25 10:16:04.690556 mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5665 2024-03-25 10:16:04.000000 mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      546 2024-03-25 10:16:04.000000 mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-25 10:16:04.000000 mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       97 2024-03-25 10:16:04.000000 mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       53 2024-03-25 10:16:04.000000 mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-25 10:16:04.000000 mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      261 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-03-25 10:16:04.691556 mosaik-api-v3-3.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-25 10:15:42.000000 mosaik-api-v3-3.0.8/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 14:20:53.358873 mosaik-api-v3-3.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/AUTHORS.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2491 2024-03-28 14:20:19.000000 mosaik-api-v3-3.0.9/CHANGES.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5909 2024-03-28 14:20:53.358873 mosaik-api-v3-3.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2015 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 14:20:53.354873 mosaik-api-v3-3.0.9/example_mas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 14:20:24.000000 mosaik-api-v3-3.0.9/example_mas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2295 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/example_mas/mosaik.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 14:20:53.358873 mosaik-api-v3-3.0.9/example_sim/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 14:20:24.000000 mosaik-api-v3-3.0.9/example_sim/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/example_sim/mosaik.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/example_sim/simulator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 14:20:53.358873 mosaik-api-v3-3.0.9/mosaik_api_v3/
+-rw-rw-rw-   0 root         (0) root         (0)    20845 2024-03-28 14:20:19.000000 mosaik-api-v3-3.0.9/mosaik_api_v3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7527 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/mosaik_api_v3/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/mosaik_api_v3/datetime.py
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/mosaik_api_v3/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 14:20:53.358873 mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5909 2024-03-28 14:20:53.000000 mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      546 2024-03-28 14:20:53.000000 mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 14:20:53.000000 mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2024-03-28 14:20:53.000000 mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2024-03-28 14:20:53.000000 mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-28 14:20:53.000000 mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      261 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-03-28 14:20:53.358873 mosaik-api-v3-3.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-03-28 14:20:19.000000 mosaik-api-v3-3.0.9/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-26 15:46:48.000000 mosaik-api-v3-3.0.9/tox.ini
```

### Comparing `mosaik-api-v3-3.0.8/CHANGES.txt` & `mosaik-api-v3-3.0.9/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+3.0.9 - 2024-03-28
+------------------
+
+- [CHANGE] We don't overwrite the logging system in `start_simulation`
+  anymore, except when the user explicitly sets `--log-level` on the
+  command line. This also changed the default level to `debug`.
+
 3.0.8 - 2024-03-25
 ------------------
 
 - [FIX] Enable yielding coroutines in finalize
 
 3.0.7 - 2023-12-19
 ------------------
```

### Comparing `mosaik-api-v3-3.0.8/LICENSE.txt` & `mosaik-api-v3-3.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/PKG-INFO` & `mosaik-api-v3-3.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-api-v3
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python implementation of the mosaik API version 3.
 Home-page: https://mosaik.offis.de
 Author: mosaik development team
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -105,14 +105,21 @@
 <https://mosaik.readthedocs.org/en/latest/dev/setup.html>`_ contains more
 details.
 
 
 Changelog
 =========
 
+3.0.9 - 2024-03-28
+------------------
+
+- [CHANGE] We don't overwrite the logging system in `start_simulation`
+  anymore, except when the user explicitly sets `--log-level` on the
+  command line. This also changed the default level to `debug`.
+
 3.0.8 - 2024-03-25
 ------------------
 
 - [FIX] Enable yielding coroutines in finalize
 
 3.0.7 - 2023-12-19
 ------------------
```

### Comparing `mosaik-api-v3-3.0.8/README.rst` & `mosaik-api-v3-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/example_mas/mosaik.py` & `mosaik-api-v3-3.0.9/example_mas/mosaik.py`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/example_sim/mosaik.py` & `mosaik-api-v3-3.0.9/example_sim/mosaik.py`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/example_sim/simulator.py` & `mosaik-api-v3-3.0.9/example_sim/simulator.py`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/mosaik_api_v3/__init__.py` & `mosaik-api-v3-3.0.9/mosaik_api_v3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Time,
 )
 from .connection import Channel
 
 import docopt
 
 
-__version__ = '3.0.8'
+__version__ = '3.0.9'
 __api_version__ = __version__
 __all__ = [
     "__version__",
     "__api_version__",
     "Simulator",
     "start_simulation",
     "MosaikProxy",
@@ -61,22 +61,23 @@
 
 Usage:
     %(prog)s [options] HOST:PORT
 
 Options:
     HOST:PORT   Connect to this address
     -l LEVEL, --log-level LEVEL
-                Log level for simulator (%(levels)s) [default: info]
+                Log level for simulator (%(levels)s)
     -r, --remote
                 Simulator is to be started on a machine remote from mosaik
     -t TIME, --timeout TIME
                 Timeout in seconds for mosaik handshake [default: 60]
 %(extra_opts)s
 """
 _LOG_LEVELS = {
+    'trace': 'TRACE',
     'debug': 'DEBUG',
     'info': 'INFO',
     'warning': 'WARNING',
     'error': 'ERROR',
     'critical': 'CRITICAL',
 }
 
@@ -385,16 +386,18 @@
     OK, ERR = 0, 1
 
     args = _parse_args(
         description or 'Start the simulation service.',
         extra_options or [],
     )
 
-    logger.remove()
-    logger.add(sys.stderr, level=args['--log-level'])
+    log_level = args.get("--log-level")
+    if log_level:
+        logger.remove()
+        logger.add(sys.stderr, level=_LOG_LEVELS[log_level])
     remote_flag = args['--remote'] if '--remote' in args.keys() else False
     sim_name = simulator.__class__.__name__
 
     # Check if simulator has implemented *time_resolution* and *max_advance*:
     global api_compliant
     api_compliant = check_api_compliance(simulator)
 
@@ -568,15 +571,14 @@
         'desc': desc,
         'prog': sys.argv[0],
         'levels': ', '.join(_LOG_LEVELS.keys()),
         'extra_opts': '\n'.join('    %s' % opt
                                 for opt in extra_options),
     }
     args = docopt.docopt(msg)
-    args['--log-level'] = _LOG_LEVELS[args.get('--log-level', 'info')]
     args['--timeout'] = args.get('--timeout', 60)
     return args
 
 
 def _parse_addr(addr):
     """Parse ``addr`` and returns a ``('host', port)`` tuple.
```

### Comparing `mosaik-api-v3-3.0.8/mosaik_api_v3/connection.py` & `mosaik-api-v3-3.0.9/mosaik_api_v3/connection.py`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/mosaik_api_v3/datetime.py` & `mosaik-api-v3-3.0.9/mosaik_api_v3/datetime.py`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/mosaik_api_v3/types.py` & `mosaik-api-v3-3.0.9/mosaik_api_v3/types.py`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/PKG-INFO` & `mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaik-api-v3
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python implementation of the mosaik API version 3.
 Home-page: https://mosaik.offis.de
 Author: mosaik development team
 Author-email: mosaik@offis.de
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -105,14 +105,21 @@
 <https://mosaik.readthedocs.org/en/latest/dev/setup.html>`_ contains more
 details.
 
 
 Changelog
 =========
 
+3.0.9 - 2024-03-28
+------------------
+
+- [CHANGE] We don't overwrite the logging system in `start_simulation`
+  anymore, except when the user explicitly sets `--log-level` on the
+  command line. This also changed the default level to `debug`.
+
 3.0.8 - 2024-03-25
 ------------------
 
 - [FIX] Enable yielding coroutines in finalize
 
 3.0.7 - 2023-12-19
 ------------------
```

### Comparing `mosaik-api-v3-3.0.8/mosaik_api_v3.egg-info/SOURCES.txt` & `mosaik-api-v3-3.0.9/mosaik_api_v3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaik-api-v3-3.0.8/setup.py` & `mosaik-api-v3-3.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='mosaik-api-v3',
-    version='3.0.8',
+    version='3.0.9',
     author='mosaik development team',
     author_email='mosaik@offis.de',
     description='Python implementation of the mosaik API version 3.',
     long_description='\n\n'.join(
         open(f, 'rb').read().decode('utf-8')
         for f in ['README.rst', 'CHANGES.txt', 'AUTHORS.txt']),
     long_description_content_type='text/x-rst',
```

