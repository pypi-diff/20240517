# Comparing `tmp/bsphud-1.0.1.tar.gz` & `tmp/bsphud-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsphud-1.0.1.tar", last modified: Thu May 16 21:40:41 2024, max compression
+gzip compressed data, was "bsphud-1.0.2.tar", last modified: Thu May 16 23:12:15 2024, max compression
```

## Comparing `bsphud-1.0.1.tar` & `bsphud-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.088881 bsphud-1.0.1/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    35150 2024-05-16 21:32:03.000000 bsphud-1.0.1/LICENSE.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    44903 2024-05-16 21:40:41.088881 bsphud-1.0.1/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)     4067 2024-05-16 21:39:45.000000 bsphud-1.0.1/README.md
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      483 2024-05-16 21:40:05.000000 bsphud-1.0.1/pyproject.toml
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       38 2024-05-16 21:40:41.088881 bsphud-1.0.1/setup.cfg
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.085881 bsphud-1.0.1/src/
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.086881 bsphud-1.0.1/src/bsphud/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-16 20:10:27.000000 bsphud-1.0.1/src/bsphud/__init__.py
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)       36 2024-05-16 20:11:13.000000 bsphud-1.0.1/src/bsphud/__main__.py
--rwxr-xr-x   0 maybetree  (1000) maybetree  (1000)     5565 2024-05-16 21:25:00.000000 bsphud-1.0.1/src/bsphud/bsphud.py
-drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 21:40:41.087881 bsphud-1.0.1/src/bsphud.egg-info/
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)    44903 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/PKG-INFO
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)      239 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/SOURCES.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/dependency_links.txt
--rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-16 21:40:41.000000 bsphud-1.0.1/src/bsphud.egg-info/top_level.txt
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 23:12:15.538842 bsphud-1.0.2/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    11326 2024-05-16 23:09:48.000000 bsphud-1.0.2/LICENSE.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    16669 2024-05-16 23:12:15.538842 bsphud-1.0.2/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)     3441 2024-05-16 23:07:46.000000 bsphud-1.0.2/README.md
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      483 2024-05-16 23:08:16.000000 bsphud-1.0.2/pyproject.toml
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       38 2024-05-16 23:12:15.538842 bsphud-1.0.2/setup.cfg
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 23:12:15.535842 bsphud-1.0.2/src/
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 23:12:15.536842 bsphud-1.0.2/src/bsphud/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       29 2024-05-16 20:10:27.000000 bsphud-1.0.2/src/bsphud/__init__.py
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)       36 2024-05-16 20:11:13.000000 bsphud-1.0.2/src/bsphud/__main__.py
+-rwxr-xr-x   0 maybetree  (1000) maybetree  (1000)     5565 2024-05-16 21:25:00.000000 bsphud-1.0.2/src/bsphud/bsphud.py
+drwxr-xr-x   0 maybetree  (1000) maybetree  (1000)        0 2024-05-16 23:12:15.537842 bsphud-1.0.2/src/bsphud.egg-info/
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)    16669 2024-05-16 23:12:15.000000 bsphud-1.0.2/src/bsphud.egg-info/PKG-INFO
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)      239 2024-05-16 23:12:15.000000 bsphud-1.0.2/src/bsphud.egg-info/SOURCES.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        1 2024-05-16 23:12:15.000000 bsphud-1.0.2/src/bsphud.egg-info/dependency_links.txt
+-rw-r--r--   0 maybetree  (1000) maybetree  (1000)        7 2024-05-16 23:12:15.000000 bsphud-1.0.2/src/bsphud.egg-info/top_level.txt
```

### Comparing `bsphud-1.0.1/README.md` & `bsphud-1.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -122,22 +122,7 @@
 launching it, it might crash.
 Working on it!
 
 - BSPHUD is inspired by the venerable [XFCE](https://xfce.org/)
 desktop envrionment,
 which has a comparable feature built-in.
 
-
-## License
-
-This program is free software: you can redistribute it and/or modify it under
-the terms of the GNU General Public License as published by the Free Software
-Foundation, either version 3 of the License, or (at your option) any later
-version.
-
-This program is distributed in the hope that it will be useful, but WITHOUT ANY
-WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
-PARTICULAR PURPOSE. See the GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License along with
-this program. If not, see <https://www.gnu.org/licenses/>. 
-
```

### Comparing `bsphud-1.0.1/src/bsphud/bsphud.py` & `bsphud-1.0.2/src/bsphud/bsphud.py`

 * *Files identical despite different names*

