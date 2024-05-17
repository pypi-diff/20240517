# Comparing `tmp/psychopy_cedrus-0.0.4.tar.gz` & `tmp/psychopy_cedrus-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy_cedrus-0.0.4.tar", last modified: Wed May  1 10:23:27 2024, max compression
+gzip compressed data, was "psychopy_cedrus-0.0.5.tar", last modified: Fri May 17 13:39:55 2024, max compression
```

## Comparing `psychopy_cedrus-0.0.4.tar` & `psychopy_cedrus-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/docs_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.424434 psychopy_cedrus-0.0.4/docs_src/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/
--rw-r--r--   0 runner    (1001) docker     (127)    65201 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Nottingham Supported.png
--rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.428434 psychopy_cedrus-0.0.4/psychopy_cedrus/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/cedrus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/
--rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrus@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrusBox.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox.png
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox.png
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/components/riponda.py
--rw-r--r--   0 runner    (1001) docker     (127)     9571 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/psychopy_cedrus/riponda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 10:23:27.000000 psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/tests/test_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/test_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/test_builder/test_ExampleComponent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:27.432434 psychopy_cedrus-0.0.4/tests/test_coder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 10:23:19.000000 psychopy_cedrus-0.0.4/tests/test_coder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.878431 psychopy_cedrus-0.0.5/docs_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/docs_src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/docs_src/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.874431 psychopy_cedrus-0.0.5/docs_src/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.874431 psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.878431 psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    65201 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/static/Nottingham Supported.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.878431 psychopy_cedrus-0.0.5/psychopy_cedrus/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/cedrus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.878431 psychopy_cedrus-0.0.5/psychopy_cedrus/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.878431 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/
+-rw-r--r--   0 runner    (1001) docker     (127)    13268 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/classic/cedrus@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/classic/cedrusBox.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/dark/cedrusBox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/dark/cedrusBox@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/light/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/light/cedrusBox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/light/cedrusBox@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/components/riponda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/psychopy_cedrus/riponda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-17 13:39:55.000000 psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-17 13:39:55.000000 psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:39:55.000000 psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 13:39:55.000000 psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 13:39:55.000000 psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 13:39:55.000000 psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/tests/test_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/tests/test_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/tests/test_builder/test_ExampleComponent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:55.882431 psychopy_cedrus-0.0.5/tests/test_coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:39:44.000000 psychopy_cedrus-0.0.5/tests/test_coder/__init__.py
```

### Comparing `psychopy_cedrus-0.0.4/LICENSE` & `psychopy_cedrus-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/PKG-INFO` & `psychopy_cedrus-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-cedrus
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extension package for PsychoPy which adds support for various hardware devices by the Cedrus Corporation.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>, Todd Parsons <todd@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://psychopy.github.io/psychopy-cedrus
 Project-URL: changelog, https://github.com/psychopy/psychopy-cedrus/blob/main/CHANGELOG.txt
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psychopy_cedrus-0.0.4/README.md` & `psychopy_cedrus-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/docs_src/conf.py` & `psychopy_cedrus-0.0.5/docs_src/conf.py`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/docs_src/favicon.png` & `psychopy_cedrus-0.0.5/docs_src/favicon.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Nottingham Supported.png` & `psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/static/Nottingham Supported.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png` & `psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png` & `psychopy_cedrus-0.0.5/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/cedrus.py` & `psychopy_cedrus-0.0.5/psychopy_cedrus/cedrus.py`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/__init__.py` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from psychopy.experiment.components import Param, _translate
 from psychopy.experiment.components.keyboard import KeyboardComponent
 from psychopy.experiment import CodeGenerationException, valid_var_re
 __author__ = 'Jon Peirce'
 
 
-class cedrusButtonBoxComponent(KeyboardComponent):
+class CedrusButtonBoxComponent(KeyboardComponent):
     """An event class for checking an Cedrus RBxxx button boxes
     using XID library
 
     This is based on keyboard component, several important differences:
     - no special response class analogous to event.BuilderKeyResponse()
     - enabled responses (active keys) are handled by the hardware device
 
@@ -36,15 +36,15 @@
                  useTimer=True, deviceNumber=0, allowedKeys="",
                  getReleaseTime=False,  # not yet supported
                  forceEndRoutine=True, storeCorrect=False, correctAns="",
                  discardPrev=True,
                  startType='time (s)', startVal=0.0,
                  stopType='duration (s)', stopVal=1.0,
                  startEstim='', durationEstim='',):
-        super(cedrusButtonBoxComponent, self).__init__(
+        super(CedrusButtonBoxComponent, self).__init__(
             exp, parentName, name=name,
             allowedKeys=allowedKeys, store=store, discardPrev=discardPrev,
             forceEndRoutine=forceEndRoutine, storeCorrect=storeCorrect,
             correctAns=correctAns, startType=startType, startVal=startVal,
             stopType=stopType, stopVal=stopVal,
             startEstim=startEstim, durationEstim=durationEstim)
```

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrus@2x.png` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/classic/cedrus@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/classic/cedrusBox.png` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/classic/cedrusBox.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox.png` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/dark/cedrusBox.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/dark/cedrusBox@2x.png` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/dark/cedrusBox@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox.png` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/light/cedrusBox.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/cedrusBox/light/cedrusBox@2x.png` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/cedrusBox/light/cedrusBox@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/components/riponda.py` & `psychopy_cedrus-0.0.5/psychopy_cedrus/components/riponda.py`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus/riponda.py` & `psychopy_cedrus-0.0.5/psychopy_cedrus/riponda.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 from psychopy.hardware import base, photodiode, button
-from psychopy.hardware.manager import deviceManager, DeviceManager
+from psychopy.hardware.manager import deviceManager, DeviceManager, ManagedDeviceError
 from psychopy import logging, layout
 import pyxid2
 
 
 class RipondaPhotodiodeGroup(photodiode.BasePhotodiodeGroup):
     def __init__(self, pad, channels=1):
-        _requestedPad = pad
-        # try to get associated riponda
-        if isinstance(_requestedPad, str):
-            # try getting by name
-            pad = DeviceManager.getDevice(pad)
-        # if still failed, make one
-        if pad is None or isinstance(pad, int):
-            pad = DeviceManager.addDevice(
-                deviceClass="psychopy_cedrus.riponda.Riponda",
-                deviceName=_requestedPad,
-                index=_requestedPad
-            )
-        # reference self in pad
-        pad.nodes.append(self)
+        # get parent
+        self.parent = Riponda.resolve(pad)
+        # reference self in parent
+        self.parent.nodes.append(self)
         # initialise base class
         photodiode.BasePhotodiodeGroup.__init__(self, channels=channels)
-        self.parent = pad
 
     def isSameDevice(self, other):
         """
         Determine whether this object represents the same physical device as a given other
         object.
 
         Parameters
@@ -59,22 +48,27 @@
                 'pad': profile['deviceName'],
                 'index': profile['index'],
                 'channels': 1,
             })
 
         return devices
 
-    def setThreshold(self, threshold, channels=(1, 2)):
+    def _setThreshold(self, threshold, channel=0):
+        if threshold is None:
+            return
         # store value
         self._threshold = threshold
         # convert from base 16
         thr = threshold / 255 * 100
-        # send commands
-        for n in channels:
-            self.parent.xid.con.send_xid_command(f"it{n}{thr}")
+        # send command
+        self.parent.xid.con.send_xid_command(f"it{channel}{thr}")
+        # dispatch
+        self.dispatchMessages()
+        # return True/False according to state
+        return self.getState(channel)
 
     def resetTimer(self, clock=logging.defaultClock):
         self.parent.resetTimer(clock=clock)
 
     def dispatchMessages(self):
         """
         Dispatch messages from parent Riponda to this photodiode group
@@ -93,32 +87,20 @@
         )
 
         return resp
 
 
 class RipondaButtonGroup(button.BaseButtonGroup):
     def __init__(self, pad=0, channels=7):
-        _requestedPad = pad
-        # try to get associated riponda
-        if isinstance(_requestedPad, str):
-            # try getting by name
-            pad = DeviceManager.getDevice(pad)
-        # if still failed, make one
-        if pad is None or isinstance(pad, int):
-            pad = DeviceManager.addDevice(
-                deviceClass="psychopy_cedrus.riponda.Riponda",
-                deviceName=_requestedPad,
-                index=_requestedPad
-            )
-
-        # reference self in pad
-        pad.nodes.append(self)
+        # get parent
+        self.parent = Riponda.resolve(pad)
+        # reference self in parent
+        self.parent.nodes.append(self)
         # initialise base class
         button.BaseButtonGroup.__init__(self, channels=channels)
-        self.parent = pad
 
     def isSameDevice(self, other):
         """
         Determine whether this object represents the same physical device as a given other
         object.
 
         Parameters
@@ -195,14 +177,50 @@
         # nodes
         self.nodes = []
         # dict of responses by timestamp
         self.messages = {}
         # reset timer
         self._lastTimerReset = None
         self.resetTimer()
+    
+    @classmethod
+    def resolve(cls, requested):
+        """
+        Take a value given to a device which has a Riponda as its parent and, from it, 
+        find/make the associated Riponda object.
+
+        Parameters
+        ----------
+        requested : str, int or Riponda
+            Value to resolve
+        """
+        # if requested is already a handle, return as is
+        if isinstance(requested, cls):
+            return requested
+        # try to get by name
+        if isinstance(requested, str):
+            pad = DeviceManager.getDevice(requested)
+            # if found, return
+            if pad is not None:
+                return pad
+        # try to get by index
+        if isinstance(requested, int):
+            pad = DeviceManager.getDeviceBy("index", requested, deviceClass="psychopy_cedrus.riponda.Riponda")
+            # if found, return
+            if pad is not None:
+                return pad
+        # if given an index of a not-yet setup device, set one up
+        if requested is None or isinstance(requested, int):
+            return DeviceManager.addDevice(
+                deviceClass="psychopy_cedrus.riponda.Riponda",
+                deviceName=f"Riponda@{requested}",
+                index=requested
+            )
+        # if still not found, raise error
+        raise ManagedDeviceError(f"Could not find/create any Riponda object from the value {requested}")
 
     def isSameDevice(self, other):
         """
         Determine whether this object represents the same physical button box as a given other
         object.
 
         Parameters
```

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/PKG-INFO` & `psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-cedrus
-Version: 0.0.4
+Version: 0.0.5
 Summary: Extension package for PsychoPy which adds support for various hardware devices by the Cedrus Corporation.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>, Todd Parsons <todd@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://psychopy.github.io/psychopy-cedrus
 Project-URL: changelog, https://github.com/psychopy/psychopy-cedrus/blob/main/CHANGELOG.txt
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `psychopy_cedrus-0.0.4/psychopy_cedrus.egg-info/SOURCES.txt` & `psychopy_cedrus-0.0.5/psychopy_cedrus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychopy_cedrus-0.0.4/pyproject.toml` & `psychopy_cedrus-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psychopy-cedrus"
-version = "0.0.4"
+version = "0.0.5"
 description = "Extension package for PsychoPy which adds support for various hardware devices by the Cedrus Corporation."
 readme = "README.md"
 requires-python = ">= 3.7"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 authors = [
   { name = "Jon Peirce", email = "jon@opensceincetools.org" },
   { name = "Matthew Cutone", email = "mcutone@opensceincetools.org" },
@@ -44,15 +44,15 @@
 [tool.setuptools.packages.find]
 where = ["",]
 
 [tool.setuptools.package-data]
 "*" = ["*.png",]
 
 [project.entry-points."psychopy.experiment.components"]
-cedrusButtonBoxComponent = "psychopy_cedrus.components.cedrusBox:cedrusButtonBoxComponent"
+CedrusButtonBoxComponent = "psychopy_cedrus.components.cedrusBox:CedrusButtonBoxComponent"
 RipondaButtonBoxBackend = "psychopy_cedrus.components.riponda:RipondaButtonBoxBackend"
 
 [project.entry-points."psychopy.hardware.cedrus"]
 RB730 = "psychopy_cedrus.cedrus:RB730"
 Riponda = "psychopy_cedrus.riponda:Riponda"
 RipondaPhotodiodeGroup = "psychopy_cedrus.riponda:RipondaPhotodiodeGroup"
 RipondaButtonGroup = "psychopy_cedrus.riponda:RipondaButtonGroup"
```

