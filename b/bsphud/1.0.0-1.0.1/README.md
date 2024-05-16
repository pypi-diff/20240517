# Comparing `tmp/bsphud-1.0.0.tar.gz` & `tmp/bsphud-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsphud-1.0.0.tar", last modified: Thu May 16 21:35:23 2024, max compression
+gzip compressed data, was "bsphud-1.0.1.tar", last modified: Thu May 16 21:40:41 2024, max compression
```

## Comparing `bsphud-1.0.0.tar` & `bsphud-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:35:23.439386 bsphud-1.0.0/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    35150 2024-05-16 21:32:03.000000 bsphud-1.0.0/LICENSE.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    44812 2024-05-16 21:35:23.438386 bsphud-1.0.0/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3976 2024-05-16 21:32:51.000000 bsphud-1.0.0/README.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      483 2024-05-16 21:29:52.000000 bsphud-1.0.0/pyproject.toml
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       38 2024-05-16 21:35:23.439386 bsphud-1.0.0/setup.cfg
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:35:23.436385 bsphud-1.0.0/src/
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:35:23.437385 bsphud-1.0.0/src/bsphud/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-16 20:10:27.000000 bsphud-1.0.0/src/bsphud/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       36 2024-05-16 20:11:13.000000 bsphud-1.0.0/src/bsphud/__main__.py
--rwxr-xr-x   0 maybetree  (1000) maybetree  (1000)     5565 2024-05-16 21:25:00.000000 bsphud-1.0.0/src/bsphud/bsphud.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:35:23.438386 bsphud-1.0.0/src/bsphud.egg-info/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    44812 2024-05-16 21:35:23.000000 bsphud-1.0.0/src/bsphud.egg-info/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      239 2024-05-16 21:35:23.000000 bsphud-1.0.0/src/bsphud.egg-info/SOURCES.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-16 21:35:23.000000 bsphud-1.0.0/src/bsphud.egg-info/dependency_links.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-16 21:35:23.000000 bsphud-1.0.0/src/bsphud.egg-info/top_level.txt
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.088881 bsphud-1.0.1/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    35150 2024-05-16 21:32:03.000000 bsphud-1.0.1/LICENSE.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    44903 2024-05-16 21:40:41.088881 bsphud-1.0.1/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4067 2024-05-16 21:39:45.000000 bsphud-1.0.1/README.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      483 2024-05-16 21:40:05.000000 bsphud-1.0.1/pyproject.toml
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       38 2024-05-16 21:40:41.088881 bsphud-1.0.1/setup.cfg
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.085881 bsphud-1.0.1/src/
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.086881 bsphud-1.0.1/src/bsphud/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-16 20:10:27.000000 bsphud-1.0.1/src/bsphud/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       36 2024-05-16 20:11:13.000000 bsphud-1.0.1/src/bsphud/__main__.py
+-rwxr-xr-x   0 maybetree  (1000) maybetree  (1000)     5565 2024-05-16 21:25:00.000000 bsphud-1.0.1/src/bsphud/bsphud.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.087881 bsphud-1.0.1/src/bsphud.egg-info/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    44903 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      239 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/SOURCES.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/dependency_links.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/top_level.txt
```

### Comparing `bsphud-1.0.0/LICENSE.txt` & `bsphud-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bsphud-1.0.0/PKG-INFO` & `bsphud-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsphud
-Version: 1.0.0
+Version: 1.0.1
 Summary: Desktop switcher popup for BSPWM
 Author-email: maybetree <maybetree48@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,14 +684,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # BSPHUD
 
 Desktop switcher popup for [bspwm](https://github.com/baskerville/bspwm).
 
+- PyPI: <https://pypi.org/project/bsphud/>
+- GitHub: <https://github.com/maybeetree/bsphud>
+
 ![BSPHUD screenshot](img/bsphud-scrot.png)
 
 BSPHUD is a window that pops up in the middle of your screen
 and gives an overview of the desktops on the currently focused monitor.
 Each desktop is represented by a black box.
 If the box is filled,
 there are windows on that desktop.
@@ -787,22 +790,22 @@
 - there needs to be a rule that tells bspwm to not manage
 the BSPHUD window.
 BSPHUD creates this rule automatically.
 Since the window is unmanaged, the border
 is actually drawn by BSPHUD itself,
 not by bspwm.
 BSPHUD queries your preferred border width and color
-using `bspc query`.
+using `bspc config`.
 
 - If you plan to run multiple instances of BSPHUD
 (e.g. multiuser system),
 it is wise to change the location of the PID file.
 For example:
 ```
-python -m bsphud.py --pidfile /var/run/user/$(id -u)/bsphud.pid
+python -m bsphud --pidfile /var/run/user/$(id -u)/bsphud.pid
 ```
 
 - bug: If you send a SIGUSR signal to BSPHUD immediately after
 launching it, it might crash.
 Working on it!
 
 - BSPHUD is inspired by the venerable [XFCE](https://xfce.org/)
```

### Comparing `bsphud-1.0.0/README.md` & `bsphud-1.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # BSPHUD
 
 Desktop switcher popup for [bspwm](https://github.com/baskerville/bspwm).
 
+- PyPI: <https://pypi.org/project/bsphud/>
+- GitHub: <https://github.com/maybeetree/bsphud>
+
 ![BSPHUD screenshot](img/bsphud-scrot.png)
 
 BSPHUD is a window that pops up in the middle of your screen
 and gives an overview of the desktops on the currently focused monitor.
 Each desktop is represented by a black box.
 If the box is filled,
 there are windows on that desktop.
@@ -101,22 +104,22 @@
 - there needs to be a rule that tells bspwm to not manage
 the BSPHUD window.
 BSPHUD creates this rule automatically.
 Since the window is unmanaged, the border
 is actually drawn by BSPHUD itself,
 not by bspwm.
 BSPHUD queries your preferred border width and color
-using `bspc query`.
+using `bspc config`.
 
 - If you plan to run multiple instances of BSPHUD
 (e.g. multiuser system),
 it is wise to change the location of the PID file.
 For example:
 ```
-python -m bsphud.py --pidfile /var/run/user/$(id -u)/bsphud.pid
+python -m bsphud --pidfile /var/run/user/$(id -u)/bsphud.pid
 ```
 
 - bug: If you send a SIGUSR signal to BSPHUD immediately after
 launching it, it might crash.
 Working on it!
 
 - BSPHUD is inspired by the venerable [XFCE](https://xfce.org/)
```

### Comparing `bsphud-1.0.0/src/bsphud/bsphud.py` & `bsphud-1.0.1/src/bsphud/bsphud.py`

 * *Files identical despite different names*

### Comparing `bsphud-1.0.0/src/bsphud.egg-info/PKG-INFO` & `bsphud-1.0.1/src/bsphud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsphud
-Version: 1.0.0
+Version: 1.0.1
 Summary: Desktop switcher popup for BSPWM
 Author-email: maybetree <maybetree48@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -684,14 +684,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # BSPHUD
 
 Desktop switcher popup for [bspwm](https://github.com/baskerville/bspwm).
 
+- PyPI: <https://pypi.org/project/bsphud/>
+- GitHub: <https://github.com/maybeetree/bsphud>
+
 ![BSPHUD screenshot](img/bsphud-scrot.png)
 
 BSPHUD is a window that pops up in the middle of your screen
 and gives an overview of the desktops on the currently focused monitor.
 Each desktop is represented by a black box.
 If the box is filled,
 there are windows on that desktop.
@@ -787,22 +790,22 @@
 - there needs to be a rule that tells bspwm to not manage
 the BSPHUD window.
 BSPHUD creates this rule automatically.
 Since the window is unmanaged, the border
 is actually drawn by BSPHUD itself,
 not by bspwm.
 BSPHUD queries your preferred border width and color
-using `bspc query`.
+using `bspc config`.
 
 - If you plan to run multiple instances of BSPHUD
 (e.g. multiuser system),
 it is wise to change the location of the PID file.
 For example:
 ```
-python -m bsphud.py --pidfile /var/run/user/$(id -u)/bsphud.pid
+python -m bsphud --pidfile /var/run/user/$(id -u)/bsphud.pid
 ```
 
 - bug: If you send a SIGUSR signal to BSPHUD immediately after
 launching it, it might crash.
 Working on it!
 
 - BSPHUD is inspired by the venerable [XFCE](https://xfce.org/)
```

