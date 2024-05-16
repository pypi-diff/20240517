# Comparing `tmp/helipad-1.6.tar.gz` & `tmp/helipad-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helipad-1.6.tar", last modified: Thu Jun 15 20:21:25 2023, max compression
+gzip compressed data, was "helipad-1.6.1.tar", last modified: Thu May 16 22:23:10 2024, max compression
```

## Comparing `helipad-1.6.tar` & `helipad-1.6.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.900558 helipad-1.6/
--rw-r--r--   0 charwick   (501) staff       (20)     1066 2023-01-08 22:00:03.000000 helipad-1.6/LICENSE
--rw-r--r--   0 charwick   (501) staff       (20)     6054 2023-06-15 20:21:25.900186 helipad-1.6/PKG-INFO
--rw-r--r--   0 charwick   (501) staff       (20)     3974 2023-06-15 19:09:24.000000 helipad-1.6/README.md
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.889691 helipad-1.6/helipad/
--rw-r--r--   0 charwick   (501) staff       (20)   379036 2022-06-27 21:28:10.000000 helipad-1.6/helipad/Helipad.png
--rw-r--r--   0 charwick   (501) staff       (20)      383 2023-05-29 03:23:08.000000 helipad-1.6/helipad/__init__.py
--rw-r--r--   0 charwick   (501) staff       (20)    33987 2023-06-15 19:07:40.000000 helipad-1.6/helipad/agent.py
--rw-r--r--   0 charwick   (501) staff       (20)    13252 2023-05-29 20:05:24.000000 helipad-1.6/helipad/cpanelJupyter.py
--rw-r--r--   0 charwick   (501) staff       (20)    27019 2023-05-29 20:19:00.000000 helipad-1.6/helipad/cpanelTkinter.py
--rw-r--r--   0 charwick   (501) staff       (20)     8676 2023-05-29 20:34:22.000000 helipad-1.6/helipad/data.py
--rw-r--r--   0 charwick   (501) staff       (20)     3878 2023-06-15 19:39:17.000000 helipad-1.6/helipad/helpers.py
--rw-r--r--   0 charwick   (501) staff       (20)     3414 2022-08-23 03:14:37.000000 helipad-1.6/helipad/ipy-styles.css
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.891778 helipad-1.6/helipad/locales/
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.884293 helipad-1.6/helipad/locales/en/
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.892171 helipad-1.6/helipad/locales/en/LC_MESSAGES/
--rw-r--r--   0 charwick   (501) staff       (20)      434 2023-06-15 20:17:44.000000 helipad-1.6/helipad/locales/en/LC_MESSAGES/helipad.mo
--rw-r--r--   0 charwick   (501) staff       (20)     8160 2023-06-15 20:15:08.000000 helipad-1.6/helipad/locales/helipad.pot
--rw-r--r--   0 charwick   (501) staff       (20)    32130 2023-06-01 03:30:48.000000 helipad-1.6/helipad/model.py
--rw-r--r--   0 charwick   (501) staff       (20)    25379 2023-05-29 21:10:59.000000 helipad-1.6/helipad/param.py
--rw-r--r--   0 charwick   (501) staff       (20)    20367 2023-06-15 19:39:26.000000 helipad-1.6/helipad/spatial.py
--rw-r--r--   0 charwick   (501) staff       (20)     5617 2023-05-30 03:50:59.000000 helipad-1.6/helipad/utility.py
--rw-r--r--   0 charwick   (501) staff       (20)    41377 2023-06-15 19:49:19.000000 helipad-1.6/helipad/visualize.py
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.891381 helipad-1.6/helipad.egg-info/
--rw-r--r--   0 charwick   (501) staff       (20)     6054 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/PKG-INFO
--rw-r--r--   0 charwick   (501) staff       (20)     1047 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/SOURCES.txt
--rw-r--r--   0 charwick   (501) staff       (20)        1 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/dependency_links.txt
--rw-r--r--   0 charwick   (501) staff       (20)       88 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/requires.txt
--rw-r--r--   0 charwick   (501) staff       (20)       39 2023-06-15 20:21:25.000000 helipad-1.6/helipad.egg-info/top_level.txt
--rw-r--r--   0 charwick   (501) staff       (20)     1205 2023-06-15 20:01:21.000000 helipad-1.6/pyproject.toml
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.897241 helipad-1.6/sample-models/
--rw-r--r--   0 charwick   (501) staff       (20)    10781 2023-06-01 03:41:45.000000 helipad-1.6/sample-models/Cities.py
--rw-r--r--   0 charwick   (501) staff       (20)    14160 2023-06-01 03:38:03.000000 helipad-1.6/sample-models/Helicopter-OMO.py
--rw-r--r--   0 charwick   (501) staff       (20)    15767 2023-06-01 03:38:38.000000 helipad-1.6/sample-models/Helicopter.py
--rw-r--r--   0 charwick   (501) staff       (20)     7017 2023-05-21 00:37:25.000000 helipad-1.6/sample-models/axelrod.py
--rw-r--r--   0 charwick   (501) staff       (20)     2756 2023-06-01 03:49:58.000000 helipad-1.6/sample-models/bootstrap.py
--rw-r--r--   0 charwick   (501) staff       (20)     4937 2023-06-15 19:44:12.000000 helipad-1.6/sample-models/cpanel-test.py
--rw-r--r--   0 charwick   (501) staff       (20)     1409 2023-05-22 22:18:00.000000 helipad-1.6/sample-models/crime.py
--rw-r--r--   0 charwick   (501) staff       (20)     5074 2023-05-20 18:33:31.000000 helipad-1.6/sample-models/criticalperiod.py
--rw-r--r--   0 charwick   (501) staff       (20)     3801 2023-06-01 03:40:50.000000 helipad-1.6/sample-models/demeSelection.py
--rw-r--r--   0 charwick   (501) staff       (20)     1534 2023-06-01 03:56:20.000000 helipad-1.6/sample-models/gameoflife.py
--rw-r--r--   0 charwick   (501) staff       (20)     5307 2023-05-30 03:17:05.000000 helipad-1.6/sample-models/grass.py
--rw-r--r--   0 charwick   (501) staff       (20)     3011 2023-06-01 03:40:38.000000 helipad-1.6/sample-models/pricediscover.py
--rw-r--r--   0 charwick   (501) staff       (20)     2491 2023-05-18 14:28:27.000000 helipad-1.6/sample-models/prisoners.py
-drwxr-xr-x   0 charwick   (501) staff       (20)        0 2023-06-15 20:21:25.899494 helipad-1.6/sample-notebooks/
--rw-r--r--   0 charwick   (501) staff       (20)    10516 2023-05-18 14:28:45.000000 helipad-1.6/sample-notebooks/axelrod.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)     6015 2023-05-20 22:52:11.000000 helipad-1.6/sample-notebooks/cpanel-test.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)    20909 2023-06-01 03:39:28.000000 helipad-1.6/sample-notebooks/helicopter.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)    91616 2023-06-15 19:25:59.000000 helipad-1.6/sample-notebooks/pricediscover.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)    86511 2023-06-01 03:54:49.000000 helipad-1.6/sample-notebooks/viz-tutorial.ipynb
--rw-r--r--   0 charwick   (501) staff       (20)       38 2023-06-15 20:21:25.900654 helipad-1.6/setup.cfg
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.786418 helipad-1.6.1/
+-rw-r--r--   0 charwick   (501) staff       (20)     1065 2024-01-13 21:00:47.000000 helipad-1.6.1/LICENSE
+-rw-r--r--   0 charwick   (501) staff       (20)     6300 2024-05-16 22:23:10.785774 helipad-1.6.1/PKG-INFO
+-rw-r--r--   0 charwick   (501) staff       (20)     3974 2023-06-15 19:09:24.000000 helipad-1.6.1/README.md
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.765866 helipad-1.6.1/helipad/
+-rw-r--r--   0 charwick   (501) staff       (20)   379036 2022-06-27 21:28:10.000000 helipad-1.6.1/helipad/Helipad.png
+-rw-r--r--   0 charwick   (501) staff       (20)      385 2024-05-16 22:17:59.000000 helipad-1.6.1/helipad/__init__.py
+-rw-r--r--   0 charwick   (501) staff       (20)    33968 2024-05-16 04:47:50.000000 helipad-1.6.1/helipad/agent.py
+-rw-r--r--   0 charwick   (501) staff       (20)    13423 2023-12-12 01:46:22.000000 helipad-1.6.1/helipad/cpanelJupyter.py
+-rw-r--r--   0 charwick   (501) staff       (20)    27454 2024-03-10 19:12:04.000000 helipad-1.6.1/helipad/cpanelTkinter.py
+-rw-r--r--   0 charwick   (501) staff       (20)     8676 2023-12-12 01:51:23.000000 helipad-1.6.1/helipad/data.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3878 2023-11-01 03:24:15.000000 helipad-1.6.1/helipad/helpers.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3479 2023-12-11 22:34:56.000000 helipad-1.6.1/helipad/ipy-styles.css
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.768923 helipad-1.6.1/helipad/locales/
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.757116 helipad-1.6.1/helipad/locales/en/
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.769801 helipad-1.6.1/helipad/locales/en/LC_MESSAGES/
+-rw-r--r--   0 charwick   (501) staff       (20)      434 2023-06-15 20:17:44.000000 helipad-1.6.1/helipad/locales/en/LC_MESSAGES/helipad.mo
+-rw-r--r--   0 charwick   (501) staff       (20)     7988 2024-03-10 20:05:05.000000 helipad-1.6.1/helipad/locales/helipad.pot
+-rw-r--r--   0 charwick   (501) staff       (20)    32451 2024-05-16 22:19:36.000000 helipad-1.6.1/helipad/model.py
+-rw-r--r--   0 charwick   (501) staff       (20)    25824 2024-05-16 22:20:16.000000 helipad-1.6.1/helipad/param.py
+-rw-r--r--   0 charwick   (501) staff       (20)    18694 2023-12-11 23:37:41.000000 helipad-1.6.1/helipad/spatial.py
+-rw-r--r--   0 charwick   (501) staff       (20)     5617 2023-05-30 03:50:59.000000 helipad-1.6.1/helipad/utility.py
+-rw-r--r--   0 charwick   (501) staff       (20)    41630 2024-05-16 04:52:13.000000 helipad-1.6.1/helipad/visualize.py
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.784387 helipad-1.6.1/helipad.egg-info/
+-rw-r--r--   0 charwick   (501) staff       (20)     6300 2024-05-16 22:23:10.000000 helipad-1.6.1/helipad.egg-info/PKG-INFO
+-rw-r--r--   0 charwick   (501) staff       (20)     1047 2024-05-16 22:23:10.000000 helipad-1.6.1/helipad.egg-info/SOURCES.txt
+-rw-r--r--   0 charwick   (501) staff       (20)        1 2024-05-16 22:23:10.000000 helipad-1.6.1/helipad.egg-info/dependency_links.txt
+-rw-r--r--   0 charwick   (501) staff       (20)       88 2024-05-16 22:23:10.000000 helipad-1.6.1/helipad.egg-info/requires.txt
+-rw-r--r--   0 charwick   (501) staff       (20)       39 2024-05-16 22:23:10.000000 helipad-1.6.1/helipad.egg-info/top_level.txt
+-rw-r--r--   0 charwick   (501) staff       (20)     1207 2024-05-16 22:19:07.000000 helipad-1.6.1/pyproject.toml
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.777057 helipad-1.6.1/sample-models/
+-rw-r--r--   0 charwick   (501) staff       (20)    10801 2024-03-10 20:13:36.000000 helipad-1.6.1/sample-models/Cities.py
+-rw-r--r--   0 charwick   (501) staff       (20)    14135 2023-12-12 02:11:40.000000 helipad-1.6.1/sample-models/Helicopter-OMO.py
+-rw-r--r--   0 charwick   (501) staff       (20)    15622 2024-05-16 04:47:46.000000 helipad-1.6.1/sample-models/Helicopter.py
+-rw-r--r--   0 charwick   (501) staff       (20)     7017 2023-05-21 00:37:25.000000 helipad-1.6.1/sample-models/axelrod.py
+-rw-r--r--   0 charwick   (501) staff       (20)     2756 2023-06-01 03:49:58.000000 helipad-1.6.1/sample-models/bootstrap.py
+-rw-r--r--   0 charwick   (501) staff       (20)     4944 2023-11-17 16:55:12.000000 helipad-1.6.1/sample-models/cpanel-test.py
+-rw-r--r--   0 charwick   (501) staff       (20)     1409 2023-05-22 22:18:00.000000 helipad-1.6.1/sample-models/crime.py
+-rw-r--r--   0 charwick   (501) staff       (20)     5067 2023-11-01 03:43:28.000000 helipad-1.6.1/sample-models/criticalperiod.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3800 2023-12-12 02:16:48.000000 helipad-1.6.1/sample-models/demeSelection.py
+-rw-r--r--   0 charwick   (501) staff       (20)     1534 2023-06-01 03:56:20.000000 helipad-1.6.1/sample-models/gameoflife.py
+-rw-r--r--   0 charwick   (501) staff       (20)     5307 2024-05-16 04:54:46.000000 helipad-1.6.1/sample-models/grass.py
+-rw-r--r--   0 charwick   (501) staff       (20)     3011 2023-06-01 03:40:38.000000 helipad-1.6.1/sample-models/pricediscover.py
+-rw-r--r--   0 charwick   (501) staff       (20)     2491 2023-05-18 14:28:27.000000 helipad-1.6.1/sample-models/prisoners.py
+drwxr-xr-x   0 charwick   (501) staff       (20)        0 2024-05-16 22:23:10.782296 helipad-1.6.1/sample-notebooks/
+-rw-r--r--   0 charwick   (501) staff       (20)    10516 2023-05-18 14:28:45.000000 helipad-1.6.1/sample-notebooks/axelrod.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)     6014 2023-12-12 01:31:55.000000 helipad-1.6.1/sample-notebooks/cpanel-test.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)    20795 2023-12-11 23:28:21.000000 helipad-1.6.1/sample-notebooks/helicopter.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)    91616 2023-06-15 19:25:59.000000 helipad-1.6.1/sample-notebooks/pricediscover.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)    86511 2023-06-01 03:54:49.000000 helipad-1.6.1/sample-notebooks/viz-tutorial.ipynb
+-rw-r--r--   0 charwick   (501) staff       (20)       38 2024-05-16 22:23:10.786563 helipad-1.6.1/setup.cfg
```

### Comparing `helipad-1.6/LICENSE` & `helipad-1.6.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 C Harwick
+Copyright (c) 2024 C Harwick
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `helipad-1.6/PKG-INFO` & `helipad-1.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: helipad
-Version: 1.6
+Version: 1.6.1
 Summary: An agent-based modeling framework for Python with a shallow learning curve and powerful visualization capabilities.
 Author-email: C Harwick <cameron@cameronharwick.com>
 License: MIT License
         
-        Copyright (c) 2023 C Harwick
+        Copyright (c) 2024 C Harwick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -20,29 +20,35 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-        
 Project-URL: Homepage, https://helipad.dev
 Project-URL: Documentation, https://helipad.dev/functions/
 Project-URL: Source Code, https://github.com/charwick/helipad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: networkx
 Provides-Extra: notebook
+Requires-Dist: jupyterlab; extra == "notebook"
+Requires-Dist: ipywidgets>=8.0; extra == "notebook"
+Requires-Dist: ipympl; extra == "notebook"
 Provides-Extra: geo
-License-File: LICENSE
+Requires-Dist: shapely; extra == "geo"
 
 # Helipad
 
 Helipad is an agent-based modeling framework for Python with powerful visualization capabilities and a shallow learning curve. Documentation and API reference can be found at [helipad.dev](https://helipad.dev).
 
 ## Features
```

### Comparing `helipad-1.6/README.md` & `helipad-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `helipad-1.6/helipad/Helipad.png` & `helipad-1.6.1/helipad/Helipad.png`

 * *Files identical despite different names*

### Comparing `helipad-1.6/helipad/agent.py` & `helipad-1.6.1/helipad/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,34 +180,33 @@
 		Keys of `mutate` correspond to property names, which will mutate either a property value retrieved from `inherit` or the initial value otherwise. Dict values can be either (1) a function (which takes a value and returns a value), (2) a std dev by which to mutate the value in a normal distribution with mean of the initial value, or (3) a tuple, the first item of which is a stdev and the second is either `'log'` or `'linear'` (i.e. to sample from a lognormal distribution).
 
 		https://helipad.dev/functions/baseagent/reproduce/"""
 		if self.fixed: raise NotImplementedError(ï('Fixed primitives cannot reproduce.'))
 
 		maxid = 0
 		for a in self.model.agents.all:
-			if a.id > maxid:
-				maxid = a.id
+			maxid = max(maxid, a.id)
 		newagent = type(self)(self.breed, maxid+1, self.model)
 
 		parents = [self] + partners
 		for a in inherit:
 			stat = None
 			if isinstance(a, tuple): a, stat = a
 			v = [getattr(p,a) for p in parents if hasattr(p,a)] #List of values, filtering those without
-			if len(v)==0: continue
+			if not v: continue
 
 			#Default statistic if unspecified. 'mean' for numbers, and 'first' for non-numbers.
 			if stat is None:
 				stat = 'mean' if isinstance(v[0], (int, float, complex)) and not isinstance(v[0], bool) else 'first'
 
 			if stat=='mean': n = np.mean(v)
 			elif stat=='sum': n = sum(v)
 			elif stat=='gmean': n = np.exp(np.log(v).sum()/len(v))
 			elif stat=='first': n = v[0]
-			elif stat=='last': n = v[len(v)-1]
+			elif stat=='last': n = v[-1]
 			elif stat in ('rand', 'random'): n = choice(v)
 			elif stat=='max': n = max(v)
 			elif stat=='min': n = min(v)
 			elif callable(stat): n = stat(v)
 			else: raise ValueError(ï('Invalid statistic {}.').format(stat))
 
 			setattr(newagent, a, n)
@@ -372,16 +371,16 @@
 				self.startpoint = agent1 if direction==agent2 else agent2
 			else: raise ValueError(ï('Direction must be either int, bool, or agent.'))
 		if not self.directed:
 			self.endpoint, self.startpoint, self.directed = (None, None, False)
 
 		#Add object to each agent, and to the model
 		for agent in self.vertices:
-			if not kind in agent.edges: agent.edges[kind] = []
-			if not self in agent.edges[kind]: agent.edges[kind].append(self) #Don't add self-links twice
+			if kind not in agent.edges: agent.edges[kind] = []
+			if self not in agent.edges[kind]: agent.edges[kind].append(self) #Don't add self-links twice
 
 		agent1.model.doHooks('edgeInit', [self, kind, agent1, agent2])
 
 	def __repr__(self):
 		pair, arrow = (self.vertices, '—') if not self.directed else ((self.startpoint, self.endpoint), '→')
 		return f'<{self.__class__.__name__}: {pair[0].__class__.__name__} {pair[0].id} {arrow} {pair[1].__class__.__name__} {pair[1].id}>'
 
@@ -546,15 +545,15 @@
 
 		#Add agents
 		if diff > 0:
 			maxid = max(ids) if (ids := [a.id for a in self.all]) else 0 #Figure out maximum existing ID
 			for aId in range(maxid+1, maxid+int(diff)+1):
 				breed = self.model.doHooks([prim+'DecideBreed', 'decideBreed'], [aId, self[prim].breeds.keys(), self.model])
 				if breed is None: breed = list(self[prim].breeds.keys())[aId%len(self[prim].breeds)]
-				if not breed in self[prim].breeds:
+				if breed not in self[prim].breeds:
 					raise ValueError(ï('Breed \'{0}\' is not registered for the \'{1}\' primitive.').format(breed, prim))
 				new = self[prim].class_(breed, aId, self.model)
 				array.append(new)
 
 		#Remove agents
 		elif diff < 0:
 			shuffle(array) #Delete agents at random
@@ -629,15 +628,15 @@
 		for p in paramDict.values(): p.addKey(name)
 
 		return self[name]
 
 	def remove(self, name: str):
 		"""Remove an item."""
 		if isinstance(name, (list, tuple)): return [self.remove(n) for n in name]
-		if not name in self: return False
+		if name not in self: return False
 
 		#Also delete per-item parameters
 		pdict = self.model.params.perBreed if isinstance(self, Breeds) else self.model.params.perGood
 		for param in pdict.values():
 			del param.value[name]
 			if getattr(param, 'elements', False):
 				if not isNotebook(): param.elements[name].destroy()
@@ -702,25 +701,25 @@
 	def __getitem__(self, val): return [e for e in self.all if e.kind==val]
 	def __contains__(self, val) -> bool: return val in list(self.keys())
 	def items(self): yield from self._dict.items()
 	def values(self): yield from self._dict.values()
 	def keys(self):
 		ks = []
 		for e in self.all:
-			if not e.kind in ks: ks.append(e.kind)
+			if e.kind not in ks: ks.append(e.kind)
 		yield from ks
 	__iter__ = keys
 	def __repr__(self): return self._dict.__repr__()
 
 	@property
 	def _dict(self):
 		es = {}
 		for e in self.all:
-			if not e.kind in es: es[e.kind] = []
-			if not e in es[e.kind]: es[e.kind].append(e)
+			if e.kind not in es: es[e.kind] = []
+			if e not in es[e.kind]: es[e.kind].append(e)
 		return es
 
 	@property
 	def all(self) -> list:
 		"""A list of all network edges in the model."""
 		es = []
 		for a in self.agents.all: es += a.edges.all
```

### Comparing `helipad-1.6/helipad/cpanelJupyter.py` & `helipad-1.6.1/helipad/cpanelJupyter.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 		#CSS for goods and breeds, since Ipywidgets ≥8.0 oversanitizes HTML in description attributes
 		for n,c in ChainMap(*[{f'breed_{p}_{k}': v.color.hex for k,v in d.breeds.items()} for p,d in model.agents.items()]+[{'good_'+k: v.color.hex for k,v in model.goods.items()}]).items():
 			css += f'.helipad_{n} .widget-label::before {{ background: {c} }}'
 
 		self.children += HTML(value='<style type="text/css">'+css+'</style>'),
 
 		#Callback function generator for Jupyter elements
+		#Attaches to the `param` object, so the param argument is a `self`
 		def setVar(param, item=None):
 			def sv(val): #Ipywidgets bases on the function signature, so can't use more than one here…
 				if param.type=='checkgrid': param.set(item, val, updateGUI=False)
 				else: param.set(val, item, updateGUI=False)
 
 				if callable(param.callback):
 					if param.per is None:
@@ -58,146 +59,65 @@
 						sv(val)
 					except: els.children[1].value = str(param.get())
 
 				return sv2
 			else: return sv
 		Param.setVar = setVar
 
-		def renderParam(param, func, title: str, val, circle=None):
-			i=None
-			if param.type=='slider':
-				if isinstance(param.opts, dict): i = interactive(func, val=(param.opts['low'],param.opts['high'], param.opts['step']))
-				else:
-					s = interactive(func, val=(0, len(param.opts)-1, 1))
-					s.children[0].readout = False
-					l = Label(value=str(param.opts[0]), layout=Layout(margin='0 0 0 15px'))
-					i = HBox([s.children[0],l])
-
-			elif param.type=='check':
-				i = interactive(func, val=val)
-			elif param.type=='menu':
-				i = interactive(func, val=[(k[1], k[0]) for k in param.opts.items()])
-			elif param.type=='checkentry':
-				defaults = (
-					(isinstance(val, param.entryType) or val) if not (param.name=='stopafter' and param.event) else True,				#Bool
-					(str(val) if isinstance(val, param.entryType) else '') if not (param.name=='stopafter' and param.event) else 'Event: '+val	#Str
-				)
-				i = interactive(func, b=defaults[0], s=defaults[1])
-				if param.per is None:
-					i = HBox(i.children)
-					i.children[0].layout = Layout(width='150px')
-				if val is False: i.children[1].disabled = True
-				i.children[1].description = ''
-
-				if param.name=='stopafter' and param.event:
-					i.children[0].disabled = True
-					i.children[1].disabled = True
-					i.add_class('helipad_checkentry_func')
-			elif param.type=='checkgrid':
-				param.elements = {}
-				for k,v in param.opts.items():
-					if not isinstance(v, (tuple, list)): v = (v, None)
-					elif len(v) < 2: v = (v[0], None)
-					param.elements[k] = interactive(param.setVar(k), val=param.vars[k])
-					param.elements[k].children[0].description = v[0]
-					param.elements[k].children[0].description_tooltip = v[1] if v[1] is not None else '' #Not working, not sure why
-
-				#Toggle-all button
-				#Would like to put it in .p-Collapse-header, but I don't think I can place an element in there
-				#So append it to the children and we'll absolutely position it to the right place
-				param.elements['toggleAll'] = Button(icon='check')
-				def toggleAll(b=None):
-					v = False if [c.children[0].value for c in param.element.children[0].children if not isinstance(c, Button) and c.children[0].value] else True
-					for c in param.element.children[0].children:
-						if not isinstance(c, Button) and not c.children[0].disabled: c.children[0].value = v
-				param.elements['toggleAll'].on_click(toggleAll)
-				param.elements['toggleAll'].add_class('helipad_toggleAll')
-
-				param.containerElement = HBox(list(param.elements.values()))
-				i = Accordion(children=[param.containerElement], selected_index=0)
-				i.set_title(0, title)
-				i.add_class('helipad_checkgrid')
-
-			if i is not None and param.type!='checkgrid':
-				if param.per is not None:
-					n = (f'{param.prim}_' if param.per=='breed' else '')+title.lower()
-					i.children[0].add_class(f'helipad_{param.per}_{n}')
-					i.children[0].add_class('helipad_per_item')
-				i.children[0].description = title
-				i.children[0].style = {'description_width': 'initial'} #Don't truncate the label
-				i.children[0].description_tooltip = param.desc if param.desc is not None else ''
-				if param.type=='slider' and isinstance(param.opts, list):
-					i.children[0].add_class('widget-logslider')
-					i.children[1].value = str(val)
-					if val in param.opts: val=param.opts.index(val)
-				if param.type!='checkentry': i.children[0].value = val
-
-			return i
-
-		def constructAccordion(param, itemList: dict):
-			param.elements = {}
-			for item, good in itemList.items():
-				param.elements[item] = renderParam(param, param.setVar(item), item.title(), param.get(item), circle=good.color)
-
-			accordion = Accordion(children=[HBox(list(param.elements.values()))], selected_index=0)
-			accordion.set_title(0, param.title)
-			accordion.add_class('helipad_param_peritem helipad_paramgroup')
-			return accordion
-
 		ctop = self.model.doHooks('CpanelTop', [self, None])
 		if ctop: self.children += ctop,
 
 		#Global config
 		for n,param in model.params.items():
 			if not getattr(param, 'config', False) or param.type=='checkgrid': continue
-			param.element = renderParam(param, param.setVar(), param.title, param.get())
+			param.element = self.renderParam(param)
 			if param.element is not None: self.children += (param.element,)
 			if param.name=='csv': param.set(ï('filename'))
 			if n=='stopafter' and not param.event and not param.get(): param.element.children[1].value = '10000'
 			if param.type=='checkentry' and getattr(param, 'config', False) and not (n=='stopafter' and param.event): param.set(False)
 
 		caip = self.model.doHooks('CpanelAboveItemParams', [self, None])
 		if caip: self.children += caip,
 
 		#Per-good parameters
 		for param in model.params.perGood.values():
-			param.element = constructAccordion(param, model.goods.nonmonetary)
+			param.element = self.renderParam(param)
 			self.children += param.element,
 
 		#Per-breed parameters
 		for param in model.params.perBreed.values():
-			param.element = constructAccordion(param, param.pKeys)
+			param.element = self.renderParam(param)
 			self.children += param.element,
 
 		cap = self.model.doHooks('CpanelAboveParams', [self, None])
 		if cap: self.children += cap,
 
 		#Pull out grouped parameters
 		groups = []
 		for group in self.model.params.groups: groups += list(group.members.keys())
 
 		#Global parameters
 		for k, param in model.params.globals.items():
 			if getattr(param, 'config', False) or k in groups or param.type=='checkgrid': continue
-			param.element = renderParam(param, param.setVar(), param.title, param.get())
+			param.element = self.renderParam(param)
 			if param.element is not None: self.children += param.element,
 
 		#Param groups
 		for group in model.params.groups:
 			for param in group.members.values():
-				param.element = renderParam(param, param.setVar(), param.title, param.get())
+				param.element = self.renderParam(param)
 			group.element = Accordion(children=[HBox([p.element for p in group.members.values()])], selected_index=0 if group.open else None)
 			group.element.set_title(0, group.title)
 			group.element.add_class('helipad_paramgroup')
 			self.children += group.element,
 
 		#Checkgrids
 		for param in model.params.values():
 			if param.type!='checkgrid' or param.name=='shocks': continue
-			param.element = renderParam(param, None, param.title, None)
+			param.element = self.renderParam(param)
 			if param.element is not None: self.children += param.element,
 
 		cas = self.model.doHooks('CpanelAboveShocks', [self, None])
 		if cas: self.children += cas,
 
 		#Shocks
 		if len(model.shocks):
@@ -283,14 +203,102 @@
 				display(pbararea)
 
 			@model.hook('terminate')
 			def cpanel_terminate(model, data):
 				self.postinstruct.layout = Layout(display='inline-block')
 				self.stopbutton.layout.visibility = 'hidden'
 
+	def renderParam(self, param, item=None):
+		"""Constructs an Ipywidget from a `Param` object. https://helipad.dev/functions/cpanel/renderparam/"""
+		i=None
+
+		#Generate an accordion for per-item parameters
+		if param.per is not None and item is None:
+			param.elements = {}
+			for name, good in param.pKeys.items():
+				if getattr(good, 'money', False): continue
+				param.elements[name] = self.renderParam(param, item=name)
+
+			accordion = Accordion(children=[HBox(list(param.elements.values()))], selected_index=0)
+			accordion.set_title(0, param.title)
+			accordion.add_class('helipad_param_peritem helipad_paramgroup')
+			return accordion
+
+		elif param.type=='slider':
+			if isinstance(param.opts, dict): i = interactive(param.setVar(item), val=(param.opts['low'],param.opts['high'], param.opts['step']))
+			else:
+				s = interactive(param.setVar(item), val=(0, len(param.opts)-1, 1))
+				s.children[0].readout = False
+				l = Label(value=str(param.opts[0]), layout=Layout(margin='0 0 0 15px'))
+				i = HBox([s.children[0],l])
+
+		elif param.type=='check':
+			i = interactive(param.setVar(item), val=param.get(item))
+		elif param.type=='menu':
+			i = interactive(param.setVar(item), val=[(k[1], k[0]) for k in param.opts.items()])
+		elif param.type=='checkentry':
+			val = param.get(item)
+			defaults = (
+				(isinstance(val, param.entryType) or val) if not (param.name=='stopafter' and param.event) else True,				#Bool
+				(str(val) if isinstance(val, param.entryType) else '') if not (param.name=='stopafter' and param.event) else 'Event: '+val	#Str
+			)
+			i = interactive(param.setVar(item), b=defaults[0], s=defaults[1])
+			if param.per is None:
+				i = HBox(i.children)
+				i.children[0].layout = Layout(width='150px')
+			if val is False: i.children[1].disabled = True
+			i.children[1].description = ''
+
+			if param.name=='stopafter' and param.event:
+				i.children[0].disabled = True
+				i.children[1].disabled = True
+				i.add_class('helipad_checkentry_func')
+		elif param.type=='checkgrid':
+			param.elements = {}
+			for k,v in param.opts.items():
+				if not isinstance(v, (tuple, list)): v = (v, None)
+				elif len(v) < 2: v = (v[0], None)
+				param.elements[k] = interactive(param.setVar(k), val=param.vars[k])
+				param.elements[k].children[0].description = v[0]
+				param.elements[k].children[0].description_tooltip = v[1] if v[1] is not None else '' #Not working, not sure why
+
+			#Toggle-all button
+			#Would like to put it in .p-Collapse-header, but I don't think I can place an element in there
+			#So append it to the children and we'll absolutely position it to the right place
+			param.elements['toggleAll'] = Button(icon='check')
+			def toggleAll(b=None):
+				v = not [c.children[0].value for c in param.element.children[0].children if not isinstance(c, Button) and c.children[0].value]
+				for c in param.element.children[0].children:
+					if not isinstance(c, Button) and not c.children[0].disabled: c.children[0].value = v
+			param.elements['toggleAll'].on_click(toggleAll)
+			param.elements['toggleAll'].add_class('helipad_toggleAll')
+
+			param.containerElement = HBox(list(param.elements.values()))
+			i = Accordion(children=[param.containerElement], selected_index=0)
+			i.set_title(0, param.title if not item else item.title())
+			i.add_class('helipad_checkgrid')
+
+		if i is not None and param.type!='checkgrid':
+			title = param.title if not item else item.title()
+			if param.per is not None:
+				n = (f'{param.prim}_' if param.per=='breed' else '')+title.lower()
+				i.children[0].add_class(f'helipad_{param.per}_{n}')
+				i.children[0].add_class('helipad_per_item')
+			i.children[0].description = title
+			i.children[0].style = {'description_width': 'initial'} #Don't truncate the label
+			i.children[0].description_tooltip = param.desc if param.desc is not None else ''
+			val = param.get(item)
+			if param.type=='slider' and isinstance(param.opts, list):
+				i.children[0].add_class('widget-logslider')
+				i.children[1].value = str(val)
+				if val in param.opts: val=param.opts.index(val)
+			if param.type!='checkentry': i.children[0].value = val
+
+		return i
+
 	def displayAlert(self, text: str, inCpanel: bool=True):
 		"""Display an alert element in the Jupyter notebook."""
 		element = HTML(value=text)
 		element.add_class('helipad_info') #Latter applies some built-in styles to the contents
 		if inCpanel: self.children += element,
 		else: display(element)
 		return element
@@ -298,13 +306,13 @@
 	def invalidate(self, message: str=ï('Model parameters changed, please re-launch the control panel with launchCpanel().')):
 		"""Prevent the user from interacting with a control panel. A control panel is invalidated when another is launched."""
 		self.valid = False
 		self.add_class('invalid')
 		warning = Label(value=message)
 		warning.add_class('helipad_modal')
 		self.children += warning,
-		for p in self.model.params.values(): del p.element
+		for p in self.model.params.values(): p.element = None
 		return warning
 
 #https://stackoverflow.com/questions/24005221/ipython-notebook-early-exit-from-cell
 class SilentExit(Exception):
 	def _render_traceback_(self): pass
```

### Comparing `helipad-1.6/helipad/cpanelTkinter.py` & `helipad-1.6.1/helipad/cpanelTkinter.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from math import ceil
 from tkinter.ttk import Progressbar
 from helipad.helpers import Color, ï
 from helipad.param import Param
 
 class Cpanel(tk.Tk):
 	"""The Tkinter-based control panel class for use in standalone models. https://helipad.dev/functions/cpanel/"""
+	font = ('Lucida Grande', 16) if sys.platform=='darwin' else ('Calibri', 14)
+
 	def __init__(self, model):
 		self.model = model
 		super().__init__()
 		self.protocol("WM_DELETE_WINDOW", self.cpanelClose)
 
 		#Set application name
 		self.setAppIcon()
@@ -93,195 +95,87 @@
 				self2['text'] = ï('New Model')
 				self2['command'] = self.model.launchVisual
 
 		#
 		# CONSTRUCT CONTROL PANEL INTERFACE
 		#
 
-		def drawCircle(frame, color, bg):
-			circle = tk.Canvas(frame, width=17, height=12, bg=bg, highlightthickness=0)
-			circle.create_oval(0,0,12,12,fill=color, outline='')
-			return circle
-
-		def renderParam(frame, param, item=None, bg='#EEEEEE'):
-			if param.type in ['hidden', 'checkgrid']: return
-
-			#Parent frame for per-item parameters
-			if param.per is not None and item is None:
-				param.element = expandableFrame(frame, bg=bg, padx=5, pady=10, text=param.title, fg="#333", font=font)
-				efSub = param.element.subframe
-				i=0
-				param.elements = {}
-				for name, b in param.pKeys.items():
-					if hasattr(b, 'money') and b.money: continue
-
-					#Do this separately because they should all be stacked
-					f = renderParam(efSub, param, item=name, bg=bg)
-					if param.type == 'checkentry':
-						f.grid(row=i, column=0)
-						efSub.columnconfigure(0,weight=1)
-
-					#Everything else goes in the two-column format
-					else:
-						f.grid(row=ceil((i+1)/2)*2, column=i%2)
-						for c in range(2): efSub.columnconfigure(c, weight=1)
-
-					i+=1
-				return param.element
-
-			#Single parameters, including the individual per-item parameters
-			else:
-				title = param.title if item is None else item.title()
-				wrap = tk.Frame(frame, bg=bg, padx=10 if item is None and not getattr(param,'config',False) else 0, pady=8 if item is None and not getattr(param,'config',False) else 0)
-
-				#Get .value directly rather than .get because we need the Var() items
-				#Except for checkentry since it doesn't store its values in .value
-				if param.value is not None:
-					val = param.value if item is None else param.value[item]
-
-				#These put the circle beside the widget
-				if param.type in ['check', 'checkentry']:
-					if param.type=='check':
-						v = tk.BooleanVar(value=val)
-						el = tk.Checkbutton(wrap, text=title, var=v, onvalue=True, offvalue=False, command=param.setVar(item), bg=bg)
-						el.BooleanVar = v
-					elif param.type=='checkentry':
-						dflt = param.get(item)
-						el = checkEntry(wrap, title, bg=bg, width=15, padx=0 if getattr(param,'config',False) else 10, pady=0 if getattr(param,'config',False) else 5, datatype='int' if param.entryType is int else 'string', command=param.setVar(item))
-						if param.name=='stopafter' and param.event:
-							el.disable()
-							el.entryValue.set('Event: '+param.get())
-							el.checkVar.set(True)
-							el.textbox.config(font=('Helvetica Neue', 12,'italic')) #Lucida doesn't have an italic?
-						else: el.set(dflt)
-
-					if item is not None:
-						el.grid(row=0, column=1)
-						drawCircle(wrap, param.pKeys[item].color.hex, bg).grid(row=0, column=0)
-					else: el.pack(anchor='center' if param.type=='check' else 'w')
-
-				#These need a separate label
-				else:
-					if param.type == 'menu':
-						v = tk.StringVar(value=param.opts[val])
-						el = tk.OptionMenu(wrap, v, *param.opts.values(), command=param.setVar(item))
-						el.StringVar = v #Save to set later
-						el.config(bg=bg)
-					elif param.type == 'slider':
-						if isinstance(param.opts, dict): el = tk.Scale(wrap, from_=param.opts['low'], to=param.opts['high'], resolution=param.opts['step'], orient='horizontal', length=150, highlightthickness=0, command=param.setVar(item), bg=bg)
-						else: el = logSlider(wrap, title=title if getattr(param, 'config', False) else None, orient='horizontal', values=param.opts, length=150, command=param.setVar(item), bg=bg)
-						el.set(param.get(item))
-
-					if item is None and not getattr(param, 'config', False):
-						tk.Label(wrap, text=title, fg="#333", bg=bg).pack(side='left', padx=8, pady=3)
-						el.pack(side='right')
-					elif getattr(param, 'config', False): el.pack()
-					else:
-						lframe = tk.Frame(wrap, bg=bg, padx=0, pady=0)
-						tk.Label(lframe, text=title, fg="#333", bg=bg).grid(row=0, column=1, pady=(0,8))
-						drawCircle(lframe, param.pKeys[item].color.hex, bg).grid(row=0, column=0, pady=(0,8))
-						lframe.grid(row=1, column=0)
-						el.grid(row=0,column=0)
-
-				if param.desc is not None: Tooltip(wrap, param.desc)
-
-				if item is None: param.element = el
-				else: param.elements[item] = el
-				return wrap
+		self.tiers = { 'config': tk.Frame(self, padx=10, pady=10, bg=bgcolors[fnum%2]) }
 
 		ctop = self.model.doHooks('CpanelTop', [self, bgcolors[fnum%2]])
 		if ctop:
 			ctop.pack(fill='x', side='top')
 			fnum += 1
 
-		frame1 = tk.Frame(self, padx=10, pady=10, bg=bgcolors[fnum%2])
-		renderParam(frame1, self.model.params['stopafter'], bg=bgcolors[fnum%2]).grid(row=0,column=0, columnspan=3, sticky='w')
-		renderParam(frame1, self.model.params['csv'], bg=bgcolors[fnum%2]).grid(row=1,column=0, columnspan=3, sticky='w')
+		self.renderParam(self.model.params['stopafter']).grid(row=0,column=0, columnspan=3, sticky='w')
+		self.renderParam(self.model.params['csv']).grid(row=1,column=0, columnspan=3, sticky='w')
 		if not self.model.params['stopafter'].event and not self.model.param('stopafter'): self.model.params['stopafter'].element.entryValue.set(10000)
 		self.model.params['csv'].set(ï('filename'))
 		self.model.params['csv'].set(False)
 
-		font = ('Lucida Grande', 16) if sys.platform=='darwin' else ('Calibri', 14)
-
-		renderParam(frame1, self.model.params['refresh'], bg=bgcolors[fnum%2]).grid(row=2, column=0, columnspan=2, pady=(10,0))
-		self.runButton = runButton(frame1, bgcolors[fnum%2])
+		self.renderParam(self.model.params['refresh']).grid(row=2, column=0, columnspan=2, pady=(10,0))
+		self.runButton = runButton(self.tiers['config'])
 		self.runButton.grid(row=2, column=2, pady=(15,0))
 
-		for c in range(2): frame1.columnconfigure(c, weight=1)
-		frame1.pack(fill='x', side='top')
+		for c in range(2): self.tiers['config'].columnconfigure(c, weight=1)
+		self.tiers['config'].pack(fill='x', side='top')
 		fnum += 1
 
 		#Can't change the background color of a progress bar on Mac, so we have to put a gray stripe on top :-/
 		frame0 = tk.Frame(self, padx=10, pady=0, bg=bgcolors[1])
 		self.progress = progressBar(root=frame0)
 		self.progress.grid(row=0, column=0)
 		frame0.columnconfigure(0,weight=1)
 		frame0.pack(fill='x', side='top')
 
 		caip = self.model.doHooks('CpanelAboveItemParams', [self, bgcolors[fnum%2]])
 		if caip:
 			caip.pack(fill='x', side='top')
 			fnum += 1
 
-		#Per-good and per-breed parameters
-		for k, param in model.params.perGood.items():
-			e = renderParam(None, param, bg=bgcolors[fnum%2])
-			if e is not None: e.pack(fill='x')
-		if len(model.params.perGood): fnum += 1 #Only increment the stripe counter if we had any good params to draw
-		for k, param in model.params.perBreed.items():
-			e = renderParam(None, param, bg=bgcolors[fnum%2])
-			if e is not None: e.pack(fill='x')
-		if len(model.params.perBreed): fnum += 1
+		#Tiers for per-good and per-breed parameters
+		self.tiers['pergood'] = tk.Frame(self, bg=bgcolors[fnum%2])
+		self.tiers['pergood'].pack(fill='x', side='top')
+		if model.params.perGood: fnum += 1 #Only increment the stripe counter if we had any good params to draw
+		self.tiers['perbreed'] = tk.Frame(self, bg=bgcolors[fnum%2])
+		self.tiers['perbreed'].pack(fill='x', side='top')
+		if model.params.perBreed: fnum += 1
 
 		cap = self.model.doHooks('CpanelAboveParams', [self, bgcolors[fnum%2]])
 		if cap:
 			cap.pack(fill='x', side='top')
 			fnum += 1
 
-		#Pull out grouped parameters
-		groups = []
-		for group in self.model.params.groups: groups += list(group.members.keys())
-
-		#Global parameters
-		for k, param in self.model.params.globals.items():
-			if getattr(param, 'config', False) or k in groups: continue
-			e = renderParam(self, param, bg=bgcolors[fnum%2])
-			if e is not None: e.pack(fill='x')
-		fnum += 1
+		#Set up tiers for global, grouped, and checkgrid parameters
+		self.tiers['global'] = tk.Frame(self, bg=bgcolors[fnum%2])
+		self.tiers['global'].pack(fill='x', side='top')
+		if model.params.globals: fnum += 1
 
-		#Param groups
 		for group in self.model.params.groups:
-			group.element = expandableFrame(self, bg=bgcolors[fnum%2], padx=5, pady=10, text=group.title, fg="#333", font=font, startOpen=group.open)
-			i=0
-			for p in group.members.values():
-				f = renderParam(group.element.subframe, p, bg=bgcolors[fnum%2])
-				f.pack(fill='x')
-				i += 1
+			group.element = expandableFrame(self, bg=bgcolors[fnum%2], padx=5, pady=10, text=group.title, fg="#333", font=self.font, startOpen=group.open)
 			if group.element is not None: group.element.pack(fill='x')
 			fnum += 1
 
-		#Checkgrid parameters
-		for p in self.model.params.values():
-			if p.type!='checkgrid' or p.name=='shocks': continue
-			p.element = checkGrid(parent=self, text=p.title, columns=getattr(p, 'columns', 3), bg=bgcolors[fnum%2], callback=p.setVar())
-			for k,v in p.opts.items():
-				if not isinstance(v, (tuple, list)): v = (v, None)
-				elif len(v) < 2: v = (v[0], None)
-				p.element.addCheck(k, v[0], p.vars[k], v[1])
-			p.element.pack(fill='both')
-			fnum += 1
+		self.tiers['checkgrids'] = tk.Frame(self, bg=bgcolors[fnum%2])
+		self.tiers['checkgrids'].pack(fill='x', side='top')
+		if [p for p in self.model.params.values() if p.type=='checkgrid' and p.name!='shocks']: fnum += 1
+
+		#Fill in tiers with parameters
+		for k, param in [(k,p) for k,p in self.model.params.items() if not getattr(p, 'config', False) or p.name=='plots']:
+			e = self.renderParam(param)
+			if e is not None: e.pack(fill='x')
 
 		cas = self.model.doHooks('CpanelAboveShocks', [self, bgcolors[fnum%2]])
 		if cas:
 			cas.pack(fill='x', side='top')
 			fnum += 1
 
 		#Shock checkboxes and buttons
 		if len(self.model.shocks):
-			self.model.shocks.element = expandableFrame(self, text=self.model.shocks.title, padx=5, pady=8, font=font, bg=bgcolors[fnum%2])
+			self.model.shocks.element = expandableFrame(self, text=self.model.shocks.title, padx=5, pady=8, font=self.font, bg=bgcolors[fnum%2])
 			self.model.shocks.element.checks = {}
 			self.model.params['shocks'].element = self.model.shocks.element
 			for shock in self.model.shocks.shocksExceptButtons.values():
 				bv = tk.BooleanVar(value=shock.selected)
 				shock.element = tk.Checkbutton(self.model.shocks.element.subframe, text=shock.name, var=bv, onvalue=True, offvalue=False, bg=bgcolors[fnum%2], anchor='w', command=shock.setCallback)
 				shock.element.BooleanVar = bv #To set via the shock object
 				self.model.shocks.element.checks[shock.name] = bv #To set via the shock parameter
@@ -301,14 +195,123 @@
 			self.model.shocks.element.pack(fill='x', side='top')
 
 		cbot = self.model.doHooks('CpanelBottom', [self, bgcolors[fnum%2]])
 		if cbot:
 			cbot.pack(fill='x', side='top')
 			fnum += 1
 
+	def renderParam(self, param, item=None, frame=None):
+		"""Constructs a Tkinter widget from a `Param` object. https://helipad.dev/functions/cpanel/renderparam/"""
+		if param.type=='hidden': return
+
+		#Parent frame for per-item parameters
+		if param.per is not None and item is None:
+			param.element = expandableFrame(self.tiers['per'+param.per], bg=self.tiers['per'+param.per].cget('bg'), padx=5, pady=10, text=param.title, fg="#333", font=self.font)
+			efSub = param.element.subframe
+			i=0
+			param.elements = {}
+			for name, b in param.pKeys.items():
+				if getattr(b, 'money', False): continue
+
+				#Do this separately because they should all be stacked
+				f = self.renderParam(param, item=name, frame=efSub)
+				if param.type == 'checkentry':
+					f.grid(row=i, column=0)
+					efSub.columnconfigure(0,weight=1)
+
+				#Everything else goes in the two-column format
+				else:
+					f.grid(row=ceil((i+1)/2)*2, column=i%2)
+					for c in range(2): efSub.columnconfigure(c, weight=1)
+
+				i+=1
+			return param.element
+
+		elif param.type=='checkgrid':
+			param.element = checkGrid(self.tiers['checkgrids'], text=param.title, columns=getattr(param, 'columns', 3), bg=self.tiers['checkgrids'].cget('bg'), callback=param.setVar())
+			for k,v in param.opts.items():
+				if not isinstance(v, (tuple, list)): v = (v, None)
+				elif len(v) < 2: v = (v[0], None)
+				param.element.addCheck(k, v[0], param.vars[k], v[1])
+			return param.element
+
+		#Single parameters, including the individual per-item parameters
+		else:
+			def drawCircle(frame, color):
+				circle = tk.Canvas(frame, width=17, height=12, bg=frame.cget('bg'), highlightthickness=0)
+				circle.create_oval(0,0,12,12,fill=color, outline='')
+				return circle
+
+			title = param.title if item is None else item.title()
+
+			#Find the right frame to attach it to
+			if getattr(param,'config',False): frame = self.tiers['config']
+			elif frame is None:
+				frame = self.tiers['global']
+				for group in self.model.params.groups:
+					if param.name in group.members:
+						frame = group.element.subframe
+						break
+			wrap = tk.Frame(frame, bg=frame.cget('bg'), padx=10 if item is None and not getattr(param,'config',False) else 0, pady=8 if item is None and not getattr(param,'config',False) else 0)
+
+			#Get .value directly rather than .get because we need the Var() items
+			#Except for checkentry since it doesn't store its values in .value
+			if param.value is not None:
+				val = param.value if item is None else param.value[item]
+
+			#These put the circle beside the widget
+			if param.type in ['check', 'checkentry']:
+				if param.type=='check':
+					v = tk.BooleanVar(value=val)
+					el = tk.Checkbutton(wrap, text=title, var=v, onvalue=True, offvalue=False, command=param.setVar(item), bg=wrap.cget('bg'))
+					el.BooleanVar = v
+				elif param.type=='checkentry':
+					dflt = param.get(item)
+					el = checkEntry(wrap, title, bg=wrap.cget('bg'), width=15, padx=0 if getattr(param,'config',False) else 10, pady=0 if getattr(param,'config',False) else 5, datatype='int' if param.entryType is int else 'string', command=param.setVar(item))
+					if param.name=='stopafter' and param.event:
+						el.disable()
+						el.entryValue.set('Event: '+param.get())
+						el.checkVar.set(True)
+						el.textbox.config(font=('Helvetica Neue', 12,'italic')) #Lucida doesn't have an italic?
+					else: el.set(dflt)
+
+				if item is not None:
+					el.grid(row=0, column=1)
+					drawCircle(wrap, param.pKeys[item].color.hex).grid(row=0, column=0)
+				else: el.pack(anchor='center' if param.type=='check' else 'w')
+
+			#These need a separate label
+			else:
+				if param.type == 'menu':
+					v = tk.StringVar(value=param.opts[val])
+					el = tk.OptionMenu(wrap, v, *param.opts.values(), command=param.setVar(item))
+					el.StringVar = v #Save to set later
+					el.config(bg=wrap.cget('bg'))
+				elif param.type == 'slider':
+					if isinstance(param.opts, dict): el = tk.Scale(wrap, from_=param.opts['low'], to=param.opts['high'], resolution=param.opts['step'], orient='horizontal', length=150, highlightthickness=0, command=param.setVar(item), bg=wrap.cget('bg'))
+					else: el = logSlider(wrap, title=title if getattr(param, 'config', False) else None, orient='horizontal', values=param.opts, length=150, command=param.setVar(item), bg=wrap.cget('bg'))
+					el.set(param.get(item))
+
+				if item is None and not getattr(param, 'config', False):
+					tk.Label(wrap, text=title, fg="#333", bg=wrap.cget('bg')).pack(side='left', padx=8, pady=3)
+					el.pack(side='right')
+				elif getattr(param, 'config', False): el.pack()
+				else:
+					lframe = tk.Frame(wrap, bg=wrap.cget('bg'), padx=0, pady=0)
+					tk.Label(lframe, text=title, fg="#333", bg=lframe.cget('bg')).grid(row=0, column=1, pady=(0,8))
+					drawCircle(lframe, param.pKeys[item].color.hex).grid(row=0, column=0, pady=(0,8))
+					lframe.grid(row=1, column=0)
+					el.grid(row=0,column=0)
+
+			if param.desc is not None: Tooltip(wrap, param.desc)
+
+			if item is None: param.element = el
+			else: param.elements[item] = el
+			return wrap
+
 	#Separate function so we can call it again when MPL tries to override
 	def setAppIcon(self):
 		"""Set the dock/taskbar icon to the Helipad icon."""
 		try:
 			__location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 			icon = os.path.join(__location__, 'Helipad.png')
 			pi = tk.PhotoImage(file=icon, master=self)
@@ -524,15 +527,15 @@
 
 		self.checkVar = tk.BooleanVar()
 		self.checkbox = tk.Checkbutton(self, text=title, bg=bg, var=self.checkVar, onvalue=True, offvalue=False, command=self.disableTextfield)
 		self.checkbox.grid(row=0, column=0)
 
 	def disableTextfield(self):
 		"""Update the enabled state of the text field to correspond to the value of the checkbox. https://helipad.dev/functions/checkentry/disabletextfield/"""
-		self.textbox.config(state='disabled' if not self.checkVar.get() else 'normal')
+		self.textbox.config(state='normal' if self.checkVar.get() else 'disabled')
 		if callable(self.callback): self.callback(self.get())
 
 	def get(self):
 		"""Retrieve the value of the combined input. Returns `False` if the checkbox is unchecked, and the value of the textbox otherwise. https://helipad.dev/functions/checkentry/get/"""
 		if not self.checkVar.get(): return False
 		v = self.entryValue.get()
 		if self.datatype=='int':
@@ -562,16 +565,16 @@
 		self.enabled = not disable
 
 	#Here for compatibility with other Tkinter widgets
 	def configure(self, state): self.disabled(state=='disabled')
 
 class checkGrid(expandableFrame):
 	"""An `expandableFrame` full of `textCheck`s, with setters and getters. https://helipad.dev/functions/checkentry/"""
-	def __init__(self, parent=None, text: str='', columns: int=3, fg='#333', bg='#FFF', padx: int=8, pady: int=5, font=('Lucida Grande', 16) if sys.platform=='darwin' else ('Calibri', 14), startOpen=True, callback=None):
-		super().__init__(parent=parent, text=text, fg=fg, bg=bg, padx=padx, pady=pady, font=font, startOpen=startOpen)
+	def __init__(self, parent=None, text: str='', columns: int=3, fg='#333', bg='#FFF', padx: int=8, pady: int=5, startOpen=True, callback=None):
+		super().__init__(parent=parent, text=text, fg=fg, bg=bg, padx=padx, pady=pady, font=Cpanel.font, startOpen=startOpen)
 		self.bg = bg
 		self.columns = columns
 		self.checks = {}
 		self._index=0
 		self.callback = callback
 
 		for i in range(columns): self.subframe.columnconfigure(i, weight=1)
```

### Comparing `helipad-1.6/helipad/data.py` & `helipad-1.6.1/helipad/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Classes for collecting and exporting data from model runs. This module should not be imported directly; interface with the `model.data` container object instead. See https://helipad.dev/functions/data/
 """
 
-import pandas, os.path
-import numpy as np
+import os.path
+import pandas, numpy as np
 from helipad.helpers import Item, ï
 
 #Don't try to subclass Pandas.dataframe; substantially slower and doesn't scale
 class Data:
 	"""Interface for collecting, storing, and accessing data generated during model runs. The object is subscriptable: `data[key]` will return the column of the data labelled `key`. Stored in `model.data`. https://helipad.dev/functions/data/"""
 	def __init__(self, model):
 		self.reporters = {}
```

### Comparing `helipad-1.6/helipad/helpers.py` & `helipad-1.6.1/helipad/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 		return True
 	except NameError: return False
 
 def isNotebook() -> bool:
 	"""Check whether Helipad is running in an interactive notebook."""
 	#get_ipython() comes back undefined inside callbacks. So cache the value once, the first time it runs.
 	#Can try @functools.cache when Python 3.9 is required
-	if not '__helipad_ipy' in globals():
+	if '__helipad_ipy' not in globals():
 		try:
 			globals()['__helipad_ipy'] = 'InteractiveShell' in get_ipython().__class__.__name__
 		except NameError: globals()['__helipad_ipy'] = False
 
 	return __helipad_ipy
 
 def isBuffered() -> bool:
```

### Comparing `helipad-1.6/helipad/ipy-styles.css` & `helipad-1.6.1/helipad/ipy-styles.css`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 .helipad_checkgrid .widget-label-basic input:enabled + span:hover { background: #DBDBDB; }
 .helipad_checkgrid .widget-label-basic input:checked:enabled + span:hover { background: #1c87f8 }
 .helipad_checkgrid .widget-label { display: none; }
 .helipad_checkgrid .widget-checkbox {
 	width: auto; height: auto;
 	margin: 0 2px 2px 0;
 }
-.helipad_checkgrid .widget-box, .helipad_paramgroup .widget-box {
-	overflow: visible;
+.helipad_checkgrid .lm-Panel, .helipad_paramgroup .lm-Panel { overflow: visible; }
+.helipad_checkgrid .widget-vbox, .helipad_paramgroup .widget-vbox {
 	display: block;
 	float: left;
 }
 .helipad_param_peritem .widget-inline-hbox { padding-right: 15px; }
 .helipad_checkgrid .widget-label-basic input:disabled + span {
 	opacity: 0.5;
 	cursor: default;
@@ -47,16 +47,15 @@
 .helipad_checkgrid .p-Panel { /* Position toggle-all correctly */
 	overflow: visible;
 	position: static;
 }
 
 .helipad_toggleAll {
 	position: absolute;
-	right: 2px;
-	top: 2px;
+	right: 0; top: -3.5em;
 	background: none;
 	color: #999;
 	width: auto;
 	border-radius: 5px;
 	cursor: pointer;
 }
 .helipad_toggleAll:hover {
```

### Comparing `helipad-1.6/helipad/locales/helipad.pot` & `helipad-1.6.1/helipad/locales/helipad.pot`

 * *Files 10% similar despite different names*

```diff
@@ -241,14 +241,18 @@
 msgid "Money good already specified as {}. Overriding…"
 msgstr ""
 
 #: model.py:652 visualize.py:146
 msgid "Money"
 msgstr ""
 
+#: model.py:116 param.py:540
+msgid "Three-item parameter tuple identifiers have been deprecated. The second item can be removed."
+msgstr ""
+
 #: param.py:36 param.py:110 param.py:129
 #: param.py:178
 msgid "A {} whose parameter value to set must be specified."
 msgstr ""
 
 #: param.py:93
 msgid "Can't add keys to a global parameter…"
@@ -282,39 +286,18 @@
 msgid "Shocks"
 msgstr ""
 
 #: param.py:579
 msgid "randn() argument must be between 0 and 100."
 msgstr ""
 
-#: spatial.py:25
-msgid "The `diag` argument is deprecated. Use the `corners` argument instead."
-msgstr ""
-
 #: spatial.py:34
 msgid "Patch number cannot be set directly. Set the dim parameter instead."
 msgstr ""
 
-#: spatial.py:41 spatial.py:44 spatial.py:48
-#: spatial.py:51
-msgid "The {0} parameter is deprecated. Use {1} instead."
-msgstr ""
-
-#: spatial.py:54
-msgid "Map Width"
-msgstr ""
-
-#: spatial.py:55
-msgid "Map Height"
-msgstr ""
-
-#: spatial.py:56
-msgid "Wrap"
-msgstr ""
-
 #: spatial.py:65
 msgid "Agent is not on a patch."
 msgstr ""
 
 #: spatial.py:98
 msgid "There is no patch at ({0}, {1})."
 msgstr ""
@@ -357,14 +340,18 @@
 
 #: visualize.py:133
 msgid ""
 "model.visual.plots is deprecated. Plots can be accessed by indexing the "
 "visualization object directly."
 msgstr ""
 
+#: visualize.py:230
+msgid "Replacing plot '{}'"
+msgstr ""
+
 #: visualize.py:245 visualize.py:348
 msgid "Cannot remove plots after control panel is drawn."
 msgstr ""
 
 #: visualize.py:251 visualize.py:354
 msgid "No plot '{}' to remove."
 msgstr ""
```

### Comparing `helipad-1.6/helipad/model.py` & `helipad-1.6.1/helipad/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 import os, sys, warnings, asyncio, time
 import gettext
 from random import shuffle, choice
 #from memory_profiler import profile
 
-from helipad.visualize import BaseVisualization, Charts, TimeSeries
+from helipad.visualize import BaseVisualization, TimeSeries
 from helipad.helpers import *
 from helipad.param import Params, Shocks
 from helipad.data import Data
 from helipad.agent import *
 
 class Helipad:
 	"""The main model object. https://helipad.dev/functions/model/"""
@@ -105,31 +105,37 @@
 		else: return '<Helipad object>'
 
 	def addButton(self, text: str, func, desc=None):
 		"""Add a button to the control panel, in the shocks section, that runs `func` when pressed. This method is aliased by the `@model.button` function decorator, which is preferred. https://helipad.dev/functions/model/addbutton/"""
 		self.shocks.add(text, None, func, 'button', True, desc)
 
 	def param(self, param, val=None):
-		"""Get or set a model parameter, depending on whether there are two or three arguments. https://helipad.dev/functions/model/param/"""
-		item = param[2] if isinstance(param, tuple) and len(param)>2 else None
+		"""Get or set a model parameter, depending on whether there is one or two arguments. https://helipad.dev/functions/model/param/"""
+		if isinstance(param, tuple):
+			#Deprecated in Helipad 1.6.1, remove in 1.8
+			if len(param) > 1 and param[1] in ['breed', 'good']:
+				warnings.warn(ï('Three-item parameter tuple identifiers have been deprecated. The second item can be removed.'), FutureWarning, 2)
+				item = param[2]
+			else: item = param[1] if len(param)>1 else None
+		else: item = None
 		param = self.params[param[0]] if isinstance(param, tuple) else self.params[param]
 
 		if val is not None: param.set(val, item)
 		else: return param.get(item)
 
 	def doHooks(self, place: str, args: list):
 		"""Execute registered hooks at various places in the model and return the value of the last function in the list. https://helipad.dev/functions/model/dohooks/"""
 		#Take a list of hooks; go until we get a response
 		if isinstance(place, list):
 			for f in place:
 				r = self.doHooks(f, args)
 				if r is not None: return r
 			return None
 
-		if not place in self.hooks: return None
+		if place not in self.hooks: return None
 		for f in self.hooks[place]: r = f(*args)
 		return r
 
 	def useVisual(self, viz: BaseVisualization):
 		"""Register a visualization class for live model visualization. Visualization classes can be imported from `helipad.visualize`, or custom visualization classes can be subclassed from `BaseVisualization`. The visualization can then be launched later using model.launchVisual(). https://helipad.dev/functions/model/usevisual/"""
 		if hasattr(self, 'breed'):
 			warnings.warn(ï('Visualizations can only be registered on the top-level model.'), None, 2)
@@ -171,32 +177,32 @@
 					self.data.addReporter(n+'-'+good, pReporter(p, good))
 			elif p.per == 'breed':
 				for breed in p.pKeys:
 					self.data.addReporter(p.prim+'-'+n+'-'+breed, pReporter(p, breed))
 
 		if self.goods.money is not None:
 			self.data.addReporter('M0', self.data.agentReporter('stocks', 'all', good=self.goods.money, stat='sum'))
-			if self.visual is not None and isinstance(self.visual, TimeSeries) and 'money' in self.visual:
+			if isinstance(self.visual, TimeSeries) and 'money' in self.visual:
 				self.visual['money'].addSeries('M0', ï('Monetary Base'), self.goods[self.goods.money].color)
 
 		#Unconditional variables to report
 		# self.data.addReporter('utility', self.data.agentReporter('utils', defPrim))
 
 		#Per-breed and per-good series and reporters
 		#Don't put lambda functions in here, or the variable pairs will be reported the same, for some reason.
 		for breed, b in self.agents[defPrim].breeds.items():
 			self.data.addReporter('utility-'+breed, self.data.agentReporter('utils', defPrim, breed=breed))
-			if self.visual is not None and self.visual.__class__.__name__=='TimeSeries':
+			if isinstance(self.visual, TimeSeries):
 				self.visual['utility'].addSeries('utility-'+breed, breed.title()+' '+ï('Utility'), b.color)
 
 		if len(self.goods) >= 2:
 			for good, g in self.goods.nonmonetary.items():
 				self.data.addReporter('demand-'+good, self.data.agentReporter('currentDemand', 'all', good=good, stat='sum'))
-				if self.visual is not None:
-					if 'demand' in self.visual: self.visual['demand'].addSeries('demand-'+good, good.title()+' '+ï('Demand'), g.color)
+				if isinstance(self.visual, TimeSeries) and 'demand' in self.visual:
+					self.visual['demand'].addSeries('demand-'+good, good.title()+' '+ï('Demand'), g.color)
 
 		#Initialize agents
 		for prim, ags in self.agents.items():
 			ags.clear()																	#Clear any surviving agents from last run
 			self.agents.initialize(self.param('num_'+prim), prim, self, force=True)		#Force is so we can call initialize() before instantiating hasModel
 
 		#Start progress bar
@@ -397,29 +403,29 @@
 		if not self.param('stopafter'): raise RuntimeError(ï('Can\'t do a parameter sweep without the value of the \'stopafter\' parameter set.'))
 
 		#Standardize format and get the Param objects
 		if not isinstance(param, list): param = [param]
 		params = {}
 		for p in param:
 			if not isinstance(p, tuple): p = (p,)
-			pobj = self.parseParamId(p)
+			pobj = self.params[p[0]]
 			params['-'.join(p)] = (p, pobj)
 
 		#Generate the parameter space, a list of dicts
 		from itertools import product
 		space = [{p[0]:run[k] for k,p in enumerate(params.items())} for run in product(*[p[1].range for p in params.values()])]
 
 		#Run the model
 		alldata = []
 		for i,run in enumerate(space):
 			print('Run',str(i+1)+'/'+str(len(space))+':',', '.join([k+'='+('\''+v+'\'' if isinstance(v, str) else str(v)) for k,v in run.items()])+'…')
 			for p in self.params.values():
 				if not getattr(p, 'config', False): p.reset()
 
-			for k,v in run.items(): params[k][1].set(v, params[k][0][2] if params[k][1].obj is not None else None)
+			for k,v in run.items(): params[k][1].set(v, params[k][0][2] if params[k][1].per is not None else None)
 			self.setup()
 			self.start()
 
 			if reporters is not None: data = pandas.DataFrame({k:self.data.all[k] for k in reporters})
 			else: data = self.data.dataframe
 
 			events = [Item(name=e.name, triggered=e.triggered, data=e.data) for e in self.events.values()]
@@ -436,16 +442,18 @@
 	def debugConsole(self):
 		"""Launch a REPL console to interact with the model after launch. Requires to be run in a buffered console. `self` will refer to the model object."""
 		if sys.platform=='darwin' and isBuffered():
 			try:
 				import code, readline # Readline doesn't look like it's doing anything here, but it enables certain console features
 				env = globals().copy()
 				env['self'] = self
-				code.interact(local=env)
+				self.console = code.InteractiveConsole(locals=env)
+				self.console.interact()
 			except ModuleNotFoundError: print(ï('Error initializing the debug console. Make sure the `readline` and `code` modules are installed.'))
+			except SystemExit: pass
 
 	def launchCpanel(self, console: bool=True):
 		"""Launch the control panel, either in a Tkinter or a Jupyter environment, as appropriate. https://helipad.dev/functions/model/launchcpanel/"""
 		if hasattr(self, 'breed'): warnings.warn(ï('Control panel can only be launched on the top-level model.'), None, 2)
 
 		self.doHooks('CpanelPreLaunch', [self])
 
@@ -457,26 +465,26 @@
 				if not l: continue
 				self.params['num_'+k].opts['low'] = makeDivisible(self.params['num_'+k].opts['low'], l, 'max')
 				self.params['num_'+k].opts['high'] = makeDivisible(self.params['num_'+k].opts['high'], l, 'max')
 				self.params['num_'+k].opts['step'] = makeDivisible(self.params['num_'+k].opts['low'], l, 'max')
 				self.params['num_'+k].value = makeDivisible(self.params['num_'+k].value, l, 'max')
 				self.params['num_'+k].default = makeDivisible(self.params['num_'+k].default, l, 'max')
 
-		if not isNotebook():
-			from helipad.cpanelTkinter import Cpanel
-			self.cpanel = Cpanel(self)
-			self.doHooks('CpanelPostInit', [self.cpanel]) #Want the cpanel property to be available here, so don't put in cpanel.py
-			if console: self.debugConsole()
-			self.cpanel.mainloop()		#Launch the control panel
-		else:
+		if isNotebook():
 			from helipad.cpanelJupyter import Cpanel, SilentExit
 			if self.cpanel: self.cpanel.invalidate(ï('Control panel was redrawn in another cell.'))
 			self.cpanel = Cpanel(self)
 			self.doHooks('CpanelPostInit', [self.cpanel])
 			raise SilentExit() #Don't blow past the cpanel if doing "run all"
+		else:
+			from helipad.cpanelTkinter import Cpanel
+			self.cpanel = Cpanel(self)
+			self.doHooks('CpanelPostInit', [self.cpanel]) #Want the cpanel property to be available here, so don't put in cpanel.py
+			if console: self.debugConsole()
+			self.cpanel.mainloop()		#Launch the control panel
 
 		self.doHooks('GUIClose', [self]) #This only executes after all GUI elements have closed
 
 	def launchVisual(self):
 		"""Launch the visualization window from the class registered in `model.useVisual()`, and start the model. https://helipad.dev/functions/model/launchvisual/"""
 		if self.visual is None or self.visual.isNull:
 			if not self.cpanel:
@@ -582,16 +590,16 @@
 	def summary(self, var, prim=None, breed=None, good=False):
 		"""Print summary statistics on an agent property. This method is deprecated; use `model.agents.summary()` instead."""
 		warnings.warn(ï('{0} is deprecated and has been replaced with {1}.').format('model.summary()', 'model.agents.summary()'), FutureWarning, 2)
 		return self.agents.summary(var, prim, breed, good)
 
 class MultiLevel(baseAgent, Helipad):
 	"""A class allowing multi-level agent-based models to be constructed, where the agents at one level are themselves full models with sub-agents. Inherits from both `baseAgent` and `Helipad`. https://helipad.dev/functions/multilevel/"""
-	def __init__(self, breed, id, parentModel):
-		super().__init__(breed, id, parentModel)
+	def __init__(self, breed, aId, parentModel):
+		super().__init__(breed, aId, parentModel)
 		self.setup()
 
 #==================
 # CONTAINER CLASSES
 #==================
 
 class Events(funcStore):
@@ -645,25 +653,23 @@
 			if self.money is not None:
 				print(ï('Money good already specified as {}. Overriding…').format(self.money))
 				self[self.money].money = False
 
 			#Add the M0 plot once we have a money good, only if we haven't done it before
 			elif (self.model.visual is None or self.model.visual.isNull) and hasattr(self.model.visual, 'plots'):
 				try:
-					if not 'money' in self.model.visual: self.model.visual.addPlot('money', ï('Money'), selected=False)
+					if 'money' not in self.model.visual: self.model.visual.addPlot('money', ï('Money'), selected=False)
 				except: pass #Can't add plot if re-drawing the cpanel
 
 		props['quantity'] = endowment
 		item = super().add('good', name, color, money=money, props=props)
 
-		#Add demand plot once we have at least 2 goods
+		#Add demand plot once we have at least 2 goods, but only if the cpanel hasn't been drawn yet
 		if len(self) == 2 and (self.model.visual is None or self.model.visual.isNull) and hasattr(self.model.visual, 'plots'):
-			try:
-				if not 'demand' in self.model.visual: self.model.visual.addPlot('demand', ï('Demand'), selected=False)
-			except: pass
+			if 'demand' not in self.model.visual: self.model.visual.addPlot('demand', ï('Demand'), selected=False)
 
 		return item
 
 	@property
 	def money(self):
 		"""The name of the good serving as a numeraire. This property is set by the `money` parameter of `Goods.add()`. https://helipad.dev/functions/goods/#money"""
 		for name,good in self.items():
@@ -677,10 +683,10 @@
 
 class Hooks(funcStore):
 	"""Interface to add and store hooks, allowing user-defined code to be inserted into the model. https://helipad.dev/functions/hooks/"""
 	multi: bool = True
 
 	def add(self, name: str, function, prioritize: bool=False):
 		"""Inserts a function into designated places in the model’s logic. See the Hooks Reference (https://helipad.dev/glossary/hooks/) for a complete list of possible hooks and the function signatures necessary to use them. This method is aliased by the `@model.hook` function decorator, which is the preferred way to hook functions. https://helipad.dev/functions/hooks/add/"""
-		if not name in self: self[name] = []
+		if name not in self: self[name] = []
 		if prioritize: self[name].insert(0, function)
 		else: self[name].append(function)
```

### Comparing `helipad-1.6/helipad/param.py` & `helipad-1.6.1/helipad/param.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Classes to abstract the interface between model parameters and GUI elements. This module should not be imported directly; use `model.params.add()` instead.
 """
 
 from itertools import combinations
-import warnings
-from helipad.helpers import *
 from numpy import arange, random
+from helipad.helpers import warnings, ï, isNotebook, Item, funcStore
 
 class Param(Item):
 	"""Base class defining a model parameter that can be set before or during runtime. https://helipad.dev/functions/param/"""
 	def __init__(self, **kwargs):
 		super().__init__(**kwargs)
 		if not hasattr(self, 'per'): self.per=None
 		if not hasattr(self, 'value'): self.value = {b:self.defaultVal for b in kwargs['pKeys']} if self.per else self.defaultVal
@@ -400,16 +399,19 @@
 		self._destroy(self[name])
 
 		del self[name]
 		return True
 
 	def _destroy(self, item):
 		if item.element:
-			if not isNotebook(): item.element.forget()
-			else: item.element.close()
+			if isNotebook(): item.element.close()
+			else:
+				#For global non-checkgrid parameters, delete the parent frame. Otherwise item.element is the whole thing
+				if getattr(item, 'per', True) or item.type=='checkgrid': item.element.forget()
+				else: item.element.master.forget()
 
 class Params(fStoreWithInterface):
 	"""Interface for storing, adding, and accessing model parameters. Stored in `model.params`. https://helipad.dev/functions/params/"""
 	multi = False
 
 	def __init__(self, model):
 		super().__init__()
@@ -502,42 +504,46 @@
 
 			def active(self2, val: bool, updateGUI: bool=True):
 				self.set(self2.name, bool(val))
 				if updateGUI and not isNotebook() and self2.element is not None:
 					self2.element.BooleanVar.set(val)
 
 			def do(self, model):
-				if self.param is not None:
+				if self.param is None: self.valFunc(model)
+				else:
 					newval = self.valFunc(self.param.get(self.item))	#Pass in current value
 					self.param.set(newval, self.item)
 					if hasattr(self.param, 'callback') and callable(self.param.callback):
 						if self.param.per is not None and self.item is not None:
 							self.param.callback(model, self.param.name, self.item, newval)
 						else:
 							self.param.callback(model, self.param.name, newval)
-				else:
-					self.valFunc(model)
 
 			#Updates the parameter value when the GUI element is clicked
 			#Can't do the regular setVar without a unified Tkinter element (like CheckGrid) to route the values
 			def setCallback(self, val=None):
 				if not isNotebook(): val = self.element.BooleanVar.get()
 				self.active(val, False)
 
 				if callable(model.params['shocks'].callback): model.params['shocks'].callback(model, 'shocks', (self.name, val))
 		self.Shock = Shock
 
 	def __repr__(self): return f'<{self.__class__.__name__}: {len(self)} shocks>'
 
 	def add(self, name: str, param, valFunc, timerFunc, active: bool=True, desc=None):
 		"""Register a shock to parameter `param`. `valFunc` takes the current value and returns a new value. `timerFunc` is a function that takes the current model time and returns `bool` (or the string `'button'`, in which case the value is shocked when a control panel button is pressed); `valFunc` will execute whenever `timerFunc` returns `True`. `param` can also be set to `None`, in which case `valFunc` receives the model object. https://helipad.dev/functions/shocks/add/"""
-		if param is not None:
-			item = param[2] if isinstance(param, tuple) and len(param)>2 else None	#The good or breed whose parameter to shock
+		if param is None: item=None
+		else:
+			if isinstance(param, tuple):
+				#Deprecated in Helipad 1.6.1, remove in 1.8
+				if len(param) > 1 and param[1] in ['breed', 'good']:
+					warnings.warn(ï('Three-item parameter tuple identifiers have been deprecated. The second item can be removed.'), FutureWarning, 2)
+					item = param[2]
+				else: item = param[1] if len(param)>1 else None
 			param = self.model.params[param[0]] if isinstance(param, tuple) else self.model.params[param]
-		else: item=None
 
 		super().add(name, self.Shock(
 			name=name,
 			desc=desc,
 			param=param,
 			item=item,
 			valFunc=valFunc,
```

### Comparing `helipad-1.6/helipad/spatial.py` & `helipad-1.6.1/helipad/spatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,50 +15,25 @@
 # SETUP
 # Create parameters, add functions, and so on
 #===============
 
 def spatialSetup(model, dim=10, corners=False, geometry: str='rect', offmap: bool=False, **kwargs):
 	"""Set up functions, properties, and methods for a spatial model. https://helipad.dev/functions/model/spatial/"""
 
-	# Backward compatibility
-	if 'diag' in kwargs:	#Remove in Helipad 1.7
-		corners = kwargs['diag']
-		warnings.warn(ï('The `diag` argument is deprecated. Use the `corners` argument instead.'), FutureWarning, 3)
-
 	#Initialize patch container and primitive
 	model.agents.addPrimitive('patch', Patch, hidden=True, priority=-10)
 	pClasses = {'rect': PatchesRect, 'polar': PatchesPolar, 'geo': PatchesGeo}
 	if not isinstance(geometry, str): #We're gonna throw an error anyway if it's not a class or a string
 		pClasses[geometry.geometry] = geometry
 		geometry = geometry.geometry
 	model.patches = pClasses[geometry](dim, corners=corners, offmap=offmap, **kwargs)
 	def npsetter(val, item): raise RuntimeError(ï('Patch number cannot be set directly. Set the dim parameter instead.'))
 	model.params['num_patch'].getter = lambda item: len(model.patches)
 	model.params['num_patch'].setter = npsetter
 
-	#Dimension parameters. Deprecated in Helipad 1.5; remove in Helipad 1.7
-	def dimgen(dim, action):
-		def dimget(name, model):
-			warnings.warn(ï("The {0} parameter is deprecated. Use {1} instead.").format(f"'{dim}'", "model.patches.dim"), FutureWarning, 5)
-			return model.patches.dim[0 if dim=='x' else 1]
-		def dimset(val, name, model):
-			warnings.warn(ï("The {0} parameter is deprecated. Use {1} instead.").format(f"'{dim}'", "model.patches.dim"), FutureWarning, 5)
-			model.patches.dim[0 if dim=='x' else 1] = val
-		return dimget if action=='get' else dimset
-	def wrapget(name, model):
-		warnings.warn(ï("The {0} parameter is deprecated. Use {1} instead.").format("'wrap'", "model.patches.wrap"), FutureWarning, 5)
-		return model.patches.wrap == (True, True)
-	def wrapset(val, name, model):
-		warnings.warn(ï("The {0} parameter is deprecated. Use {1} instead.").format("'wrap'", "model.patches.wrap"), FutureWarning, 5)
-		model.patches.wrap = val if isinstance(val, (tuple, list)) else (val, val)
-	wrap = kwargs['wrap'] if 'wrap' in kwargs else True
-	model.params.add('x', ï('Map Width'), 'hidden', dflt=model.patches.dim[0], setter=dimgen('x','set'), getter=dimgen('x','get'))
-	model.params.add('y', ï('Map Height'), 'hidden', dflt=model.patches.dim[1], setter=dimgen('y','set'), getter=dimgen('y','get'))
-	model.params.add('wrap', ï('Wrap'), 'hidden', dflt=(wrap is True), setter=wrapset, getter=wrapget) #Only checked at the beginning of a model
-
 	#Hook a positioning function or randomly position our agents
 	@model.hook(prioritize=True)
 	def baseAgentInit(agent, model):
 		if agent.primitive == 'patch': return #Patch position is fixed
 		p = model.doHooks(['baseAgentPosition', agent.primitive+'Position'], [agent, agent.model])
 		if p and len(p) >= 2:
 			agent.position = list(p)
```

### Comparing `helipad-1.6/helipad/utility.py` & `helipad-1.6.1/helipad/utility.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/helipad/visualize.py` & `helipad-1.6.1/helipad/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Base classes for visualizing Helipad models with Matplotlib, to be passed to `model.useVisual()`. Main visualizers are `TimeSeries` to display diachronic data, and `Charts` to display synchronic data.
 """
 
 import sys
 from abc import ABC, abstractmethod
 from math import sqrt, ceil, pi, isnan
 from numpy import ndarray, array, asanyarray, log10, linspace, newaxis, arange, full_like, linalg, ones, vstack
-import matplotlib, matplotlib.pyplot as plt, matplotlib.style as mlpstyle, matplotlib.cm as cm
+import matplotlib, matplotlib.pyplot as plt, matplotlib.style as mlpstyle
 from matplotlib.lines import Line2D
 from matplotlib.patches import Polygon
 from helipad.helpers import *
 mlpstyle.use('fast')
 
 #======================
 # TOP-LEVEL VISUALIZERS
@@ -102,35 +102,37 @@
 			else: width, height = self.dim
 
 			self.fig.set_size_inches(width/self.fig.dpi, height/self.fig.dpi)
 			fm.window.wm_geometry(f'+{self.pos[0]}+{self.pos[1]}')
 
 	#Save window dimensions and position
 	def terminate(self, model):
+		if self.isNull: return
 		fm = self.fig.canvas.manager
 		if hasattr(fm, 'window'):
 			self.dim = list(self.fig.get_size_inches()*self.fig.dpi)
 			pos = fm.window.wm_geometry().split('+')
 			self.pos = (pos[1], pos[2])
 
 	def addKeypress(self, key: str, fn):
 		"""Register a function to be run when `key` is pressed in a Matplotlib visualizer. `fn` will run if `key` is pressed at any time when the plot window is in focus. To narrow the focus to a particular plot, define `catchKeypress()` in a subclass of `ChartPlot`. https://helipad.dev/functions/mplvisualization/addkeypress/"""
-		if not key in self.keyListeners: self.keyListeners[key] = []
+		if key not in self.keyListeners: self.keyListeners[key] = []
 		self.keyListeners[key].append(fn)
 
 	@property
 	def activePlots(self) -> dict:
 		"""The subset of the plots containing the `Plot`s that are currently active. https://helipad.dev/functions/mplvisualization/#activePlots"""
 		return {k:plot for k,plot in self.items() if plot.selected}
 
 	@property
 	def isNull(self) -> bool:
 		"""`True` when the model should run as-if with no visualization, for example if all plots are unselected. `False` indicates the window can be launched. https://helipad.dev/functions/mplvisualization/#isNull"""
 		return not [plot for plot in self.values() if plot.selected]
 
+	#Deprecated in Helipad 1.6, remove in 1.8
 	@property
 	def plots(self):
 		"""A `dict` of plots. This property is deprecated; the visualization object can be indexed directly."""
 		warnings.warn(ï('model.visual.plots is deprecated. Plots can be accessed by indexing the visualization object directly.'), FutureWarning, 2)
 		return self
 
 class TimeSeries(MPLVisualization):
@@ -220,14 +222,15 @@
 		for plot in self.activePlots.values(): plot.draw(time) #Update the actual plots. Has to be after the new resolution is set
 		if self.fig.stale: self.fig.canvas.draw_idle()
 		self.fig.canvas.flush_events() #Listen for user input
 
 	def addPlot(self, name: str, label: str, position=None, selected: bool=True, logscale: bool=False, stack: bool=False):
 		"""Register a plot area in the `TimeSeries` plot area to which data series can be added. `position` Position is the number you want it to be, *not* the array position. https://helipad.dev/functions/timeseries/addplot/"""
 		plot = TimeSeriesPlot(viz=self, name=name, label=label, logscale=logscale, stack=stack)
+		if name in self: warnings.warn(ï("Replacing plot '{}'").format(name), None, 2)
 
 		self.selector.addItem(name, label, position, selected)
 		if position is None or position > len(self): self[name] = plot
 		else:		#Reconstruct the dicts because there's no insert method…
 			newplots, i = ({}, 1)
 			for k,v in self.items():
 				if position==i:
@@ -243,15 +246,15 @@
 	def removePlot(self, name, reassign=None):
 		"""Remove a plot or plots and optionally reassign their series to a different plot. https://helipad.dev/functions/timeseries/removeplot/"""
 		if self.model.cpanel: raise RuntimeError(ï('Cannot remove plots after control panel is drawn.'))
 		if isinstance(name, list):
 			for p in name: self.removePlot(p, reassign)
 			return
 
-		if not name in self:
+		if name not in self:
 			warnings.warn(ï('No plot \'{}\' to remove.').format(name), None, 2)
 			return False
 
 		if reassign is not None: self[reassign].series += self[name].series
 		del self[name]
 		del self.selector.opts[name]
 		del self.selector.vars[name]
@@ -267,14 +270,15 @@
 
 class Charts(MPLVisualization):
 	"""A Matplotlib-based visualizer for a variety of visualizations that display data that reflects a single point in time. https://helipad.dev/functions/charts/"""
 	def __init__(self, model):
 		super().__init__(model)
 		self.events = {}
 		self.plotTypes = {}
+		self.timeslider = None
 
 		for p in [BarChart, AgentsPlot, TimeSeriesPlot]: self.addPlotType(p)
 		model.params['refresh'].runtime=False
 		self.model = model # :(
 
 	def launch(self, title: str):
 		if not self.activePlots: return #Windowless mode
@@ -295,15 +299,15 @@
 			plots[i].subplot_position = (y,x,i+1)
 		super().launch(title)
 
 		#Time slider
 		ref = self.model.params['refresh'].get()
 		self.fig.subplots_adjust(bottom=0.12) #Make room for the slider
 		sax = self.fig.add_axes([0.1,0.01,.75,0.03], facecolor='#EEF')
-		self.timeslider = Slider(sax, 't=', 0, ref, ref, valstep=ref, closedmin=False)
+		self.timeslider = Slider(sax, 't=', 0, ref, valinit=ref, valstep=ref, closedmin=False)
 		self.timeslider.on_changed(self.scrub)
 
 		self.fig.canvas.draw_idle()
 		plt.show(block=False)
 
 	def refresh(self, data: dict):
 		data = {k:v[-1] for k,v in data.items()}
@@ -323,14 +327,15 @@
 		"""Update the visualizer with the values from model time `t`."""
 		self.scrubval = t
 		for c in self.activePlots.values(): c.draw(t)
 		self.fig.patch.set_facecolor(self.events[t] if t in self.events else 'white')
 
 	def addPlot(self, name: str, label: str, type=None, position=None, selected=True, **kwargs):
 		"""Adds a plot area to the Chart visualizer. Defaults to a bar chart, but can be set to any subclass of ChartPlot. Kwargs are passed to the `ChartPlot` object. https://helipad.dev/functions/charts/addplot/"""
+		if name in self: warnings.warn(ï("Replacing plot '{}'").format(name), None, 2)
 		self.selector.addItem(name, label, position, selected)
 		if type == 'network': #Deprecated in Helipad 1.6; remove in 1.8
 			warnings.warn(ï('The `network` plot type is deprecated. Use `agents` instead.'), FutureWarning, 2)
 			type = 'agents'
 		self.type = type if type is not None else 'bar'
 		if self.type not in self.plotTypes: raise KeyError(ï('\'{}\' is not a registered plot visualizer.').format(self.type))
 		self[name] = self.plotTypes[self.type](name=name, label=label, viz=self, selected=True, **kwargs)
@@ -346,15 +351,15 @@
 	def removePlot(self, name):
 		"""Remove a plot or plots and optionally reassign their series to a different plot. https://helipad.dev/functions/timeseries/removeplot/"""
 		if self.model.cpanel: raise RuntimeError(ï('Cannot remove plots after control panel is drawn.'))
 		if isinstance(name, list):
 			for p in name: self.removePlot(p)
 			return
 
-		if not name in self:
+		if name not in self:
 			warnings.warn(ï('No plot \'{}\' to remove.').format(name), None, 2)
 			return False
 
 		del self[name]
 		return True
 
 	def event(self, t: int, color='#FDC', **kwargs):
@@ -422,15 +427,15 @@
 		super().__init__(**kwargs)
 
 	def addSeries(self, reporter, label: str, color, style: str='-', visible: bool=True):
 		"""Register a reporter to be plotted during the model's runtime. https://helipad.dev/functions/timeseriesplot/addseries/"""
 		if not isinstance(color, Color): color = Color(color)
 
 		#Check against columns and not reporters so subseries work
-		if not callable(reporter) and not reporter in self.viz.model.data.columns:
+		if not callable(reporter) and reporter not in self.viz.model.data.columns:
 			raise KeyError(ï('Reporter \'{}\' does not exist. Be sure to register reporters before adding series.').format(reporter))
 
 		#Add subsidiary series (e.g. percentile bars)
 		subseries = []
 		if reporter in self.viz.model.data.reporters and self.viz.model.data.reporters[reporter].children:
 			for p in self.viz.model.data.reporters[reporter].children:
 				if '-unsmooth' in p: continue #Don't plot the unsmoothed series
@@ -543,15 +548,15 @@
 		return self.viz.resolution if hasattr(self.viz, 'resolution') else int(self.viz.model.param('refresh'))
 
 class BarChart(ChartPlot):
 	"""A plot type that displays live-updating bar charts. https://helipad.dev/functions/barchart/"""
 	type = 'bar'
 	def __init__(self, **kwargs):
 		for arg in ['horizontal', 'logscale']:
-			if not arg in kwargs: kwargs[arg] = False
+			if arg not in kwargs: kwargs[arg] = False
 		super().__init__(**kwargs)
 		self.bars = []
 
 	def addBar(self, reporter, label: str, color='blue', position=None):
 		"""Register a data reporter as a bar on the current plot. To display error bars, use the `std` or `percentiles` arguments when creating the agent reporter. https://helipad.dev/functions/barchart/addbar/"""
 		if not isinstance(color, Color): color = Color(color)
 		bar = Item(reporter=reporter, label=label, color=color)
@@ -759,15 +764,15 @@
 		self.axes.set_title(self.label, fontdict={'fontsize':10})
 		if self.layout != 'spatial' or self.viz.model.patches.geometry != 'geo':
 			self.axes.set_facecolor('white')
 			self.axes.set_aspect('auto')
 		self.pos = self.layouts[self.layout](self.ndata[t])
 
 		if self.layout == 'spatial':
-			cmap = cm.get_cmap(self.params['patchColormap'])
+			cmap = matplotlib.colormaps[self.params['patchColormap']]
 			if self.viz.model.patches.geometry == 'geo': pd = array([self.getPatchParamValue(p,t) for p in self.viz.model.patches])
 			else:
 				pd = array([[self.getPatchParamValue(p,t) for p in col] for col in self.viz.model.patches]).T #Transpose because numpy is indexed col, row
 			if self.projection=='polar':
 				self.axes.set_aspect('equal')
 				self.axes.set_ylim(0, self.viz.model.patches.dim[1])
 				norm = (pd - int(self.normal.vmin))/(rng if (rng:=(self.normal.vmax-int(self.normal.vmin))) else 1)
```

### Comparing `helipad-1.6/helipad.egg-info/PKG-INFO` & `helipad-1.6.1/helipad.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: helipad
-Version: 1.6
+Version: 1.6.1
 Summary: An agent-based modeling framework for Python with a shallow learning curve and powerful visualization capabilities.
 Author-email: C Harwick <cameron@cameronharwick.com>
 License: MIT License
         
-        Copyright (c) 2023 C Harwick
+        Copyright (c) 2024 C Harwick
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -20,29 +20,35 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-        
 Project-URL: Homepage, https://helipad.dev
 Project-URL: Documentation, https://helipad.dev/functions/
 Project-URL: Source Code, https://github.com/charwick/helipad
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: networkx
 Provides-Extra: notebook
+Requires-Dist: jupyterlab; extra == "notebook"
+Requires-Dist: ipywidgets>=8.0; extra == "notebook"
+Requires-Dist: ipympl; extra == "notebook"
 Provides-Extra: geo
-License-File: LICENSE
+Requires-Dist: shapely; extra == "geo"
 
 # Helipad
 
 Helipad is an agent-based modeling framework for Python with powerful visualization capabilities and a shallow learning curve. Documentation and API reference can be found at [helipad.dev](https://helipad.dev).
 
 ## Features
```

### Comparing `helipad-1.6/helipad.egg-info/SOURCES.txt` & `helipad-1.6.1/helipad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helipad-1.6/pyproject.toml` & `helipad-1.6.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "helipad"
-version = "1.6"
+version = "1.6.1"
 authors = [
 	{ name="C Harwick", email="cameron@cameronharwick.com" },
 ]
 description = "An agent-based modeling framework for Python with a shallow learning curve and powerful visualization capabilities."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `helipad-1.6/sample-models/Cities.py` & `helipad-1.6.1/sample-models/Cities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # A model of the long-run cyclical dynamics of urbanization and human capital.
 
-from math import sqrt, log, floor, exp
+from math import sqrt, floor
+from numpy import diff, random, log
 from helipad import Helipad
-from numpy import *
 heli = Helipad()
 
 #================
 # CONFIGURATION
 #================
 
 heli.agents.addBreed('urban', '#CC0000')
 heli.agents.addBreed('rural', '#00CC00')
 
 #Constrain the parameter space to values resulting in H* = 100
 def constrain(model, var, val):
-	if var=='city': model.params['rent'].disabled(val)
+	if var=='city':
+		model.params.hide('rent')
+		#model.params['rent'].disabled(val)
 	elif model.param('city'):
 		if var=='fixed':
 			model.params['rent'].enable() #Tkinter won't let you update the value of a disabled widget...
 			model.param('rent', .04+.037*val)
 			model.params['rent'].disable()
 		# if var=='rent':
 		# 	model.params['fixed'].enable() #Tkinter won't let you update the value of a disabled widget...
@@ -42,33 +44,33 @@
 
 class Land():
 	def __init__(self, loc):
 		self.loc = loc
 		self.input = 0
 		self.lastInput = 0
 		self.product = 0
-	
+
 	def produce(self):
 		self.product = popfactor*log(self.input) #if self.loc=='rural' else sqrt(self.input)	# = ln∑P (eq. 2)
 		self.lastInput = self.input
 		self.input = 0 #Reset productivity at the end of each period
 		return self.product
-	
+
 	def pop(self, model): return len(model.agents['agent'][self.loc])
-	
+
 	#The add argument calculates the productivity as if the agent were already there, if he's not
 	def agentProd(self, H, add=False):
 		if self.loc=='rural': return sqrt(150) * H
 		else:
 			if add:
 				return 1/sqrt(self.pop(heli)+1) * (heli.data.getLast('hsum')+H)
 				# return (heli.data.getLast('urbanH')*p+H)/(p+1) * log(heli.data.getLast('hsum')+H) #wtf was I doing here?
 			else: return 1/sqrt(self.pop(heli)) * heli.data.getLast('hsum')
 			# else: return heli.data.getLast('urbanH')*log(heli.data.getLast('hsum'))
-	
+
 	def expWage(self, H):
 		prod = self.agentProd(H, True)
 		potentialprod = log(self.lastInput+prod) #if self.loc=='rural' else sqrt(self.lastInput+prod)
 		return potentialprod *  prod/(self.lastInput+prod) #Your share of the product
 
 heli.land = {k: Land(k) for k in ['urban', 'rural']}
 heli.params['num_agent'].type = 'hidden'
@@ -84,26 +86,26 @@
 	model.movers = {b:0 for b in heli.agents['agent'].breeds}
 	model.births = {b:0 for b in heli.agents['agent'].breeds}
 	model.deaths = 0
 	for b in heli.agents['agent'].breeds:
 		setattr(model, 'moverate'+b, 0)
 		setattr(model, 'birthrate'+b, 0)
 	model.deathrate = 0
-	
+
 	#Mark the different phases of the Malthusian model
 	model.events.clear()
 	if not model.param('city'):
 		model.param('num_agent', 150)
 		@heli.event
 		def exp1(model):	return sum(diff(model.data.getLast('ruralPop', 20))) > 3
 		@heli.event
 		def stab2(model):	return model.events['exp1'].triggered and model.t > model.events['exp1'].triggered+1000 and sum(diff(model.data.getLast('ruralH', 3000))) < 0
 		@heli.event
 		def end3(model): return model.events['stab2'].triggered and model.t >= model.events['stab2'].triggered + burnout
-	
+
 	#Start with the equilibrium population
 	else: model.param('num_agent', floor(2.55-1.69*model.param('fixed'))*popfactor)
 
 @heli.hook
 def agentInit(agent, model):
 	agent.H = random.normal(100, 15) if model.param('city') else 10 #Human capital
 	agent.prod = 0
@@ -125,39 +127,39 @@
 
 @heli.hook
 def agentStep(agent, model, stage):
 	if stage==1:
 		if model.param('city'):
 			otherloc = 'urban' if agent.breed == 'rural' else 'rural'
 			agent.expwage = model.land[otherloc].expWage(agent.H)
-		
+
 			#Decide whether or not to move
 			mvc = model.param('movecost')
 			if agent.expwage > agent.lastWage*1.2 and agent.wealth > mvc and model.t > 2:
 			# if agent.prod[otherloc]-mvc > agent.prod[agent.breed] and agent.wealth > mvc: #and model.t > 10000:
 				# print('T=',model.t,', HC',agent.H,':',agent.breed,'wage=',agent.lastWage,',',otherloc,'wage=',otherwage)
 				agent.wealth -= mvc
 				model.movers[agent.breed] += 1
 				agent.breed = otherloc
-				
+
 		agent.prod = model.land[agent.breed].agentProd(agent.H)
 		model.land[agent.breed].input += agent.prod #Work
-		
+
 		#Reproduce
 		randn = random.normal(1, 0.2)
 		if random.random() < model.param('deathrate'): agent.die()
 		elif agent.wealth > model.param('breedThresh') * (randn if agent.breed=='rural' else agent.H/4):
 			child = agent.reproduce(
 				inherit=['H', ('wealth', lambda w: w[0]/2)],
 				mutate={'H': 14.25} if not model.param('lockH') else {} #See footnote 3 for derivation
 			)
 			agent.wealth -= agent.wealth/2 + 1 #-= breedThresh #Fixed cost
 			model.births[agent.breed] += 1
 			if child.H < 2: child.die()
-	
+
 	#Get paid in modelStep, then pay rent
 	elif stage==2:
 		agent.wealth -= model.param('rent') * agent.H + model.param('fixed')
 		if agent.wealth <= 0: agent.die()
 		return
 
 #Organize some data and pause if all agents are dead
@@ -172,16 +174,16 @@
 				setattr(model,'birthrate'+b, model.births[b]/pop)
 				model.movers[b] = 0
 				model.births[b] = 0
 		model.deathrate = model.deaths/len(model.agents['agent'])
 		model.deaths = 0
 
 @heli.hook
-def decideBreed(id, choices, model):
-	return 'rural';
+def decideBreed(aId, choices, model):
+	return 'rural'
 
 @heli.hook
 def agentDie(agent): heli.deaths += 1
 
 #================
 # REPORTERS AND PLOTS
 #================
@@ -189,15 +191,15 @@
 from helipad.visualize import TimeSeries
 viz = heli.useVisual(TimeSeries)
 
 # returns ln(∑H²)
 @heli.reporter
 def hsum(model, loc='urban'):
 	upop = model.agents['agent'][loc]
-	return sum([a.H for a in upop]) if len(upop) > 0 else 1
+	return sum(a.H for a in upop) if len(upop) > 0 else 1
 
 def perCapGdp(model, loc):
 	def tmp(model):
 		pop = model.land[loc].pop(model)
 		if pop==0: return 0
 		else: return model.land[loc].product/pop
 	return tmp
```

### Comparing `helipad-1.6/sample-models/Helicopter-OMO.py` & `helipad-1.6.1/sample-models/Helicopter-OMO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # A model of the relative price effects of monetary shocks via helicopter drop vs. by open market operations.
 # Includes a banking system to distribute OMOs. Requires the basic Helicopter.py in the same folder.
 # Download the paper at https://ssrn.com/abstract=2545488
 
-from numpy import isnan, mean, array #, std
+from numpy import mean, array #, std
 from Helicopter import * #Building on the basic Helicopter model
 heli = setup()
 
 #===============
 # BANK CLASS
 #===============
 
@@ -286,15 +286,15 @@
 	if model.param('num_bank') > 0 and agent.primitive != 'bank':
 		agent.bank = model.agents['bank'][0]
 		agent.bank.setupAccount(agent)
 
 @heli.hook
 def agentInit(agent, model):
 	if model.param('num_bank') > 0:
-		agent.liqPref = model.param(('liqPref', 'breed', agent.breed, 'agent'))
+		agent.liqPref = model.param(('liqPref', agent.breed))
 
 @heli.hook
 def agentStep(agent, model, stage):
 	#Deposit cash in the bank at the end of each period
 	if hasattr(agent, 'bank'):
 		tCash = agent.liqPref * (1/(1+agent.bank.i)) * agent.balance #Slightly interest-elastic
 		agent.bank.deposit(agent, agent.stocks[agent.model.goods.money]-tCash)
```

### Comparing `helipad-1.6/sample-models/Helicopter.py` & `helipad-1.6.1/sample-models/Helicopter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # A model of the relative price effects of monetary shocks via helicopter drop
 # Download the paper at https://ssrn.com/abstract=2545488
 
 #To generate IRFs, turn off the visualization, turn on stopafter, and one shock.
 
 from itertools import combinations
 from math import sqrt
+from numpy import random
 from helipad import *
-from numpy import random, isnan
 
 M0 = 120000
 
 #===============
 # STORE CLASS
 # Has to come before adding the primitive
 #===============
 
 class Store(baseAgent):
-	def __init__(self, breed, id, model):
-		super().__init__(breed, id, model)
+	def __init__(self, breed, aId, model):
+		super().__init__(breed, aId, model)
 
 		#Start with equilibrium prices. Not strictly necessary, but it eliminates the burn-in period. See eq. A7
-		sm=sum(1/sqrt(model.param(('prod','good',g))) for g in model.goods.nonmonetary) * M0/(model.param('num_agent')*(len(model.goods.nonmonetary)+sum(1+model.param(('rbd','breed',b,'agent')) for b in model.agents['agent'].breeds)))
-		self.price = {g:sm/(sqrt(model.param(('prod','good',g)))) for g in model.goods.nonmonetary}
+		sm=sum(1/sqrt(model.param(('prod',g))) for g in model.goods.nonmonetary) * M0/(model.param('num_agent')*(len(model.goods.nonmonetary)+sum(1+model.param(('rbd',b)) for b in model.agents['agent'].breeds)))
+		self.price = {g:sm/(sqrt(model.param(('prod',g)))) for g in model.goods.nonmonetary}
 
-		self.invTarget = {g:model.param(('prod','good',g))*model.param('num_agent')*2 for g in model.goods.nonmonetary}
+		self.invTarget = {g:model.param(('prod',g))*model.param('num_agent')*2 for g in model.goods.nonmonetary}
 		self.portion = {g:1/(len(model.goods.nonmonetary)) for g in model.goods.nonmonetary} #Capital allocation
 		self.wage = 0
 		self.cashDemand = 0
 
 	def step(self, stage):
 		super().step(stage)
 		N = self.model.param('num_agent')
@@ -49,19 +49,19 @@
 			labor += 1
 
 		tPrice = sum(self.price[good] for good in self.model.goods.nonmonetary)
 		avg, stdev = {},{} #Hang onto these for use with credit calculations
 		for i in self.model.goods.nonmonetary:
 
 			#Just have a fixed inventory target, but update if params do
-			self.invTarget = {g:self.model.param(('prod','good',g))*self.model.param('num_agent')*2 for g in self.model.goods.nonmonetary}
+			self.invTarget = {g:self.model.param(('prod',g))*self.model.param('num_agent')*2 for g in self.model.goods.nonmonetary}
 
 			#Produce stuff
 			self.portion[i] = (self.model.param('kImmob') * self.portion[i] + self.price[i]/tPrice) / (self.model.param('kImmob') + 1)	#Calculate capital allocation
-			self.stocks[i] = self.stocks[i] + self.portion[i] * labor * self.model.param(('prod', 'good', i))
+			self.stocks[i] = self.stocks[i] + self.portion[i] * labor * self.model.param(('prod', i))
 
 			#Set prices
 			#Change in the direction of hitting the inventory target
 			# self.price[i] += log(self.invTarget[i] / (self.inventory[i][0] + self.lastShortage[i])) #Jim's pricing rule?
 			self.price[i] += (self.invTarget[i] - self.stocks[i] + self.model.data.getLast('shortage-'+i))/100 #/150
 
 			#Adjust in proportion to the rate of inventory change
@@ -129,18 +129,18 @@
 
 	heli.params.add('rbd', 'Demand for Real Balances', 'slider', per='breed', dflt={'hobbit':7, 'dwarf': 35}, opts={'low':1, 'high': 50, 'step': 1}, prim='agent', callback=rbalUpdater)
 	heli.params.add('prod', 'Productivity', 'slider', per='good', dflt=1.75, opts={'low':0.1, 'high': 2, 'step': 0.1}) #If you shock productivity, make sure to call rbalupdater
 
 	#Takes as input the slider value, outputs b_g. See equation (A8) in the paper.
 	def rbaltodemand(breed):
 		def reporter(model):
-			rbd = model.param(('rbd', 'breed', breed, 'agent'))
+			rbd = model.param(('rbd', breed))
 			beta = rbd/(1+rbd)
 
-			return (beta/(1-beta)) * len(model.goods) * sqrt(model.param(('prod','good',AgentGoods[breed]))) / sum(1/sqrt(pr) for pr in model.param(('prod','good')).values())
+			return (beta/(1-beta)) * len(model.goods) * sqrt(model.param(('prod',AgentGoods[breed]))) / sum(1/sqrt(pr) for pr in model.param('prod').values())
 
 		return reporter
 
 #===============
 # DATA COLLECTION AND VISUALIZATION
 #===============
 
@@ -242,18 +242,18 @@
 
 	from helipad.utility import CES
 
 	@heli.hook
 	def agentInit(agent, model):
 		agent.store = model.agents['store'][0]
 		agent.item = AgentGoods[agent.breed]
-		rbd = model.param(('rbd', 'breed', agent.breed, 'agent'))
+		rbd = model.param(('rbd', agent.breed))
 		beta = rbd/(rbd+1)
 		agent.utility = CES({'good': 1-beta, 'rbal': beta }, agent.model.param('sigma'))
-		agent.expCons = model.param(('prod', 'good', agent.item))
+		agent.expCons = model.param(('prod', agent.item))
 
 		#Set cash endowment to equilibrium value based on parameters. Not strictly necessary but avoids the burn-in period.
 		agent.stocks[model.goods.money] = agent.store.price[agent.item] * rbaltodemand(agent.breed)(heli)
 
 	@heli.hook
 	def agentStep(agent, model, stage):
 		itemPrice = agent.store.price[agent.item]
@@ -290,15 +290,15 @@
 # SHOCKS
 #========
 
 	#Random shock to dwarf cash demand
 	def shock(v):
 		c = random.normal(v, 4)
 		return c if c >= 1 else 1
-	heli.shocks.add('Dwarf real balances', ('rbd','breed','dwarf','agent'), shock, heli.shocks.randn(2), active=False)
+	heli.shocks.add('Dwarf real balances', ('rbd','dwarf'), shock, heli.shocks.randn(2), active=False)
 
 	#Shock the money supply
 	def mshock(model):
 		pct = random.normal(3, 15) #High mean to counteract the downward bias of (1-%)(1+%)
 		m = model.cb.M0 * (1+pct/100)
 		m = max(m, 10000)		#Things get weird when there's a money shortage
 		model.cb.M0 = m
@@ -323,21 +323,21 @@
 #
 
 class CentralBank(baseAgent):
 	ngdpAvg = 0
 	ngdp = 0
 	primitive = 'cb'
 
-	def __init__(self, id, model):
-		super().__init__(None, id, model)
-		self.id = id
+	def __init__(self, aId, model):
+		super().__init__(None, aId, model)
+		self.id = aId
 		self.model = model
 		self.stocks[self.model.goods.money] = M0 #Has to have assets in order to contract
 
-		self.ngdpTarget = False if not model.param('ngdpTarget') else 10000
+		self.ngdpTarget = 10000 if model.param('ngdpTarget') else False
 
 	def step(self):
 
 		#Record macroeconomic vars at the end of the last stage
 		#Getting demand has it lagged one period…
 		self.ngdp = sum(self.model.data.getLast('demand-'+good) * self.model.agents['store'][0].price[good] for good in self.model.goods.nonmonetary)
 		if not self.ngdpAvg: self.ngdpAvg = self.ngdp
@@ -350,17 +350,16 @@
 
 	def expand(self, amount):
 		if self.model.param('dist') == 'lump':
 			amt = amount/self.model.param('num_agent')
 			for a in self.model.agents['agent']:
 				a.stocks[self.model.goods.money] += amt
 		else:
-			M0 = self.M0
 			for a in self.model.agents.all:
-				a.stocks[self.model.goods.money] += a.stocks[self.model.goods.money]/M0 * amount
+				a.stocks[self.model.goods.money] += a.stocks[self.model.goods.money]/self.M0 * amount
 
 	@property
 	def M0(self):
 		return self.model.data.agentReporter('stocks', 'all', good=self.model.goods.money, stat='sum')(self.model)
 
 	@M0.setter
 	def M0(self, value): self.expand(value - self.M0)
```

### Comparing `helipad-1.6/sample-models/axelrod.py` & `helipad-1.6.1/sample-models/axelrod.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-models/bootstrap.py` & `helipad-1.6.1/sample-models/bootstrap.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-models/cpanel-test.py` & `helipad-1.6.1/sample-models/cpanel-test.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,22 +91,22 @@
 
 #Cut one edge and create one edge
 @heli.hook
 def modelPostStep(model):
 	random.choice(model.agents.edges['edge']).cut()
 	newedge(model)
 
-net = viz.addPlot('net', 'Network Structure', type='agents', scatter=['s1', 's2'])
+net = viz.addPlot('net', 'Network Structure', type='agents') #scatter=['s1', 's2']
 bar1 = viz.addPlot('prop', 'Bar Chart')
 bar2 = viz.addPlot('prop2', 'Horizontal Bar Chart', horizontal=True)
 net.config({
 	'agentLabel': True,
  	'labelColor': '#FFFFFF',
 # 	'labelFamily': 'serif',
-	'agentMarker': 'H',
+#	'agentMarker': 'H',
 	'labelAlpha': 0.75,
 	'labelWeight': 'bold',
  	'labelSize': 8,
 	'regLine': True
 })
 
 gcolors = ['F00', 'F03', 'F06', 'F09', 'F0C', 'C0F', '90F', '60F', '30F', '00F']
@@ -117,15 +117,15 @@
 #Replace an agent, but only if we click during the current model time
 @heli.hook
 def agentClick(agents, plot, t):
 	if t != heli.t: return
 	
 	for agent in agents:
 		new = agent.reproduce()
-		enum = len(agent.edges[plot.kind]) if plot.kind in agent.edges else 0
+		enum = len(agent.edges[plot.network]) if plot.network in agent.edges else 0
 		agent.die()
 		for e in range(enum): newedge(heli)
 		print('Killing agent',agent.id,'and creating agent',new.id)
 	plot.update(None, t)
 	plot.draw(t, forceUpdate=True)
 
 #===============
```

### Comparing `helipad-1.6/sample-models/crime.py` & `helipad-1.6.1/sample-models/crime.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-models/criticalperiod.py` & `helipad-1.6.1/sample-models/criticalperiod.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 #Returns language capacity
 def capacity(self, gene=None, age=None):
 	if gene is None: gene = self.dominantLap
 	if age is None: age=self.age
 	
 	start = (10-self.model.param('pleio'))*age
 	l = sum(gene[start:start+10])
-	return 0 if l<0 else l
+	return max(0,l)
 Agent.capacity = capacity
 
 @heli.hook
 def modelPostSetup(model):
 	model.births = 0 #Keep track so we can mutate every 30
 	
 #Initialize agent variables
```

### Comparing `helipad-1.6/sample-models/demeSelection.py` & `helipad-1.6.1/sample-models/demeSelection.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 #===============
 # SETUP
 #===============
 
 from random import choice
 from math import exp
-from helipad import Helipad, MultiLevel
 import numpy.random as nprand
+from helipad import Helipad, MultiLevel
 
 heli = Helipad()
 heli.name = 'Deme Selection'
 heli.agents.order = ['linear', 'linear', 'match']
 heli.stages = 3 #Stage 1 for intra-demic competition, stage 2 for reproduction, stage 3 for war
 
 heli.agents.addPrimitive('deme', MultiLevel, dflt=20, priority=1)
@@ -71,16 +71,16 @@
 			for i in range(a.stocks['payoff']): a.reproduce()
 			a.die()
 
 #Normalize population at the beginning of stage 3
 @heli.hook
 def modelStep(model, stage):
 	if stage==3:
+		targetDpop = 20
 		for d in model.agents['deme']:
-			targetDpop = 20
 			while len(d.agents['agent']) > targetDpop: choice(d.agents['agent']).die()
 			while len(d.agents['agent']) < targetDpop: choice(d.agents['agent']).reproduce()
 
 #===============
 # DATA AND VISUALIZATION
 #===============
```

### Comparing `helipad-1.6/sample-models/gameoflife.py` & `helipad-1.6.1/sample-models/gameoflife.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-models/grass.py` & `helipad-1.6.1/sample-models/grass.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-models/pricediscover.py` & `helipad-1.6.1/sample-models/pricediscover.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-models/prisoners.py` & `helipad-1.6.1/sample-models/prisoners.py`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-notebooks/axelrod.ipynb` & `helipad-1.6.1/sample-notebooks/axelrod.ipynb`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-notebooks/cpanel-test.ipynb` & `helipad-1.6.1/sample-notebooks/cpanel-test.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99769069664903%*

 * *Differences: {"'cells'": '{5: {\'source\': {insert: [(27, "viz.addPlot(\'net\', \'Network Structure\', '*

 * *            'type=\'agents\', layout=\'spring\')\\n")], delete: [27]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.12.1'}}"}*

```diff
@@ -116,15 +116,15 @@
                 "def modelPostStep(model):\n",
                 "\trandom.choice(model.agents.edges['edge']).cut()\n",
                 "\t\n",
                 "\ta1, a2 = random.choice(model.agents['agent']), random.choice(model.agents['agent'])\n",
                 "\twhile a1.edges.With(a2): a1, a2 = random.choice(model.agents['agent']), random.choice(model.agents['agent'])\n",
                 "\ta1.edges.add(a2, direction=random.choice([True, False]), weight=random.choice([0.5,1,2,3]))\n",
                 "\n",
-                "viz.addPlot('net', 'Network Structure', type='network', layout='spring')\n",
+                "viz.addPlot('net', 'Network Structure', type='agents', layout='spring')\n",
                 "bar1 = viz.addPlot('prop', 'My Property')\n",
                 "bar2 = viz.addPlot('prop2', 'Horizontal Property', horizontal=True)\n",
                 "\n",
                 "gcolors = ['F00', 'F03', 'F06', 'F09', 'F0C', 'C0F', '90F', '60F', '30F', '00F']\n",
                 "for i in range(20):\n",
                 "\theli.data.addReporter('prop'+str(i), heli.data.agentReporter('prop'+str(i), std=0.1))\n",
                 "\t(bar1 if i<=10 else bar2).addBar('prop'+str(i), str(i), '#'+gcolors[i%10])"
@@ -168,13 +168,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.5"
+            "version": "3.12.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `helipad-1.6/sample-notebooks/helicopter.ipynb` & `helipad-1.6.1/sample-notebooks/helicopter.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974412433222726%*

 * *Differences: {"'cells'": '{3: {\'source\': {insert: [(5, "\\t\\tsm=sum(1/sqrt(model.param((\'prod\',g))) for g '*

 * *            'in model.goods.nonmonetary) * '*

 * *            "M0/(model.param('num_agent')*(len(model.goods.nonmonetary)+sum(1+model.param(('rbd',b,'agent')) "*

 * *            'for b in model.agents[\'agent\'].breeds)))\\n"), (6, "\\t\\tself.price = '*

 * *            '{g:sm/(sqrt(model.param((\'prod\',g)))) for g in model.goods.nonmonetary}\\n"), (8, '*

 * *            '"\\t\\tself.invTarget = {g:model.param((\'prod\',g))*mod […]*

```diff
@@ -45,18 +45,18 @@
             "outputs": [],
             "source": [
                 "class Store(baseAgent):\n",
                 "\tdef __init__(self, breed, id, model):\n",
                 "\t\tsuper().__init__(breed, id, model)\n",
                 "\n",
                 "\t\t#Start with equilibrium prices. Not strictly necessary, but it eliminates the burn-in period. See eq. A7\n",
-                "\t\tsm=sum(1/sqrt(model.param(('prod','good',g))) for g in model.goods.nonmonetary) * M0/(model.param('num_agent')*(len(model.goods.nonmonetary)+sum(1+model.param(('rbd','breed',b,'agent')) for b in model.primitives['agent'].breeds)))\n",
-                "\t\tself.price = {g:sm/(sqrt(model.param(('prod','good',g)))) for g in model.goods.nonmonetary}\n",
+                "\t\tsm=sum(1/sqrt(model.param(('prod',g))) for g in model.goods.nonmonetary) * M0/(model.param('num_agent')*(len(model.goods.nonmonetary)+sum(1+model.param(('rbd',b,'agent')) for b in model.agents['agent'].breeds)))\n",
+                "\t\tself.price = {g:sm/(sqrt(model.param(('prod',g)))) for g in model.goods.nonmonetary}\n",
                 "\n",
-                "\t\tself.invTarget = {g:model.param(('prod','good',g))*model.param('num_agent')*2 for g in model.goods.nonmonetary}\n",
+                "\t\tself.invTarget = {g:model.param(('prod',g))*model.param('num_agent')*2 for g in model.goods.nonmonetary}\n",
                 "\t\tself.portion = {g:1/(len(model.goods.nonmonetary)) for g in model.goods.nonmonetary} #Capital allocation\n",
                 "\t\tself.wage = 0\n",
                 "\t\tself.cashDemand = 0\n",
                 "\n",
                 "\tdef step(self, stage):\n",
                 "\t\tsuper().step(stage)\n",
                 "\t\tN = self.model.param('num_agent')\n",
@@ -78,19 +78,19 @@
                 "\t\t\tlabor += 1\n",
                 "\t\n",
                 "\t\ttPrice = sum(self.price[good] for good in self.model.goods.nonmonetary)\t\t\n",
                 "\t\tavg, stdev = {},{} #Hang onto these for use with credit calculations\n",
                 "\t\tfor i in self.model.goods.nonmonetary:\n",
                 "\n",
                 "\t\t\t#Just have a fixed inventory target, but update if params do\n",
-                "\t\t\tself.invTarget = {g:self.model.param(('prod','good',g))*self.model.param('num_agent')*2 for g in self.model.goods.nonmonetary}\n",
+                "\t\t\tself.invTarget = {g:self.model.param(('prod',g))*self.model.param('num_agent')*2 for g in self.model.goods.nonmonetary}\n",
                 "\n",
                 "\t\t\t#Produce stuff\n",
                 "\t\t\tself.portion[i] = (self.model.param('kImmob') * self.portion[i] + self.price[i]/tPrice) / (self.model.param('kImmob') + 1)\t#Calculate capital allocation\n",
-                "\t\t\tself.stocks[i] = self.stocks[i] + self.portion[i] * labor * self.model.param(('prod', 'good', i))\n",
+                "\t\t\tself.stocks[i] = self.stocks[i] + self.portion[i] * labor * self.model.param(('prod', i))\n",
                 "\n",
                 "\t\t\t#Set prices\n",
                 "\t\t\t#Change in the direction of hitting the inventory target\n",
                 "\t\t\t# self.price[i] += log(self.invTarget[i] / (self.inventory[i][0] + self.lastShortage[i])) #Jim's pricing rule?\n",
                 "\t\t\tself.price[i] += (self.invTarget[i] - self.stocks[i] + self.model.data.getLast('shortage-'+i))/100 #/150\n",
                 "\n",
                 "\t\t\t#Adjust in proportion to the rate of inventory change\n",
@@ -166,18 +166,18 @@
                 "\n",
                 "heli.params.add('rbd', 'Demand for Real Balances', 'slider', per='breed', dflt={'hobbit':7, 'dwarf': 35}, opts={'low':1, 'high': 50, 'step': 1}, prim='agent', callback=rbalUpdater)\n",
                 "heli.params.add('prod', 'Productivity', 'slider', per='good', dflt=1.75, opts={'low':0.1, 'high': 2, 'step': 0.1}) #If you shock productivity, make sure to call rbalupdater\n",
                 "\n",
                 "#Takes as input the slider value, outputs b_g. See equation (A8) in the paper.\n",
                 "def rbaltodemand(breed):\n",
                 "\tdef reporter(model):\n",
-                "\t\trbd = model.param(('rbd', 'breed', breed, 'agent'))\n",
+                "\t\trbd = model.param(('rbd', breed, 'agent'))\n",
                 "\t\tbeta = rbd/(1+rbd)\n",
                 "\t\t\n",
-                "\t\treturn (beta/(1-beta)) * len(model.goods) * sqrt(model.param(('prod','good',AgentGoods[breed]))) / sum(1/sqrt(pr) for pr in model.param(('prod','good')).values())\n",
+                "\t\treturn (beta/(1-beta)) * len(model.goods) * sqrt(model.param(('prod',AgentGoods[breed]))) / sum(1/sqrt(pr) for pr in model.param('prod').values())\n",
                 "\n",
                 "\treturn reporter"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -202,16 +202,16 @@
                 "viz.addPlot('wage', 'Wage', 11, selected=False)\n",
                 "viz.addPlot('shortage', 'Shortages', 6, selected=False)\n",
                 "\n",
                 "def shortageReporter(good):\n",
                 "\tdef reporter(model): return model.shortages[good]\n",
                 "\treturn reporter\n",
                 "\n",
-                "viz['capital'].addSeries(lambda t: 1/len(heli.primitives['agent'].breeds), '', '#CCCCCC')\n",
-                "for breed, d in heli.primitives['agent'].breeds.items():\n",
+                "viz['capital'].addSeries(lambda t: 1/len(heli.agents['agent'].breeds), '', '#CCCCCC')\n",
+                "for breed, d in heli.agents['agent'].breeds.items():\n",
                 "\theli.data.addReporter('rbalDemand-'+breed, rbaltodemand(breed))\n",
                 "\theli.data.addReporter('shortage-'+AgentGoods[breed], shortageReporter(AgentGoods[breed]))\n",
                 "\theli.data.addReporter('eCons-'+breed, heli.data.agentReporter('expCons', 'agent', breed=breed, stat='sum'))\n",
                 "\t# heli.data.addReporter('rWage-'+breed, lambda model: heli.data.agentReporter('wage', 'store')(model) / heli.data.agentReporter('price', 'store', good=b.good)(model))\n",
                 "\t# heli.data.addReporter('expWage', heli.data.agentReporter('expWage', 'agent'))\n",
                 "\theli.data.addReporter('rBal-'+breed, heli.data.agentReporter('realBalances', 'agent', breed=breed))\n",
                 "\theli.data.addReporter('invTarget-'+AgentGoods[breed], heli.data.agentReporter('invTarget', 'store', good=AgentGoods[breed]))\n",
@@ -277,18 +277,18 @@
                 "\n",
                 "from helipad.utility import CES\n",
                 "\n",
                 "@heli.hook\n",
                 "def agentInit(agent, model):\n",
                 "\tagent.store = model.agents['store'][0]\n",
                 "\tagent.item = AgentGoods[agent.breed]\n",
-                "\trbd = model.param(('rbd', 'breed', agent.breed, 'agent'))\n",
+                "\trbd = model.param(('rbd', agent.breed, 'agent'))\n",
                 "\tbeta = rbd/(rbd+1)\n",
                 "\tagent.utility = CES({'good': 1-beta, 'rbal': beta }, agent.model.param('sigma'))\n",
-                "\tagent.expCons = model.param(('prod', 'good', agent.item))\n",
+                "\tagent.expCons = model.param(('prod', agent.item))\n",
                 "\t\n",
                 "\t#Set cash endowment to equilibrium value based on parameters. Not strictly necessary but avoids the burn-in period.\n",
                 "\tagent.stocks[model.goods.money] = agent.store.price[agent.item] * rbaltodemand(agent.breed)(heli)\n",
                 "\n",
                 "@heli.hook\n",
                 "def agentStep(agent, model, stage):\n",
                 "\titemPrice = agent.store.price[agent.item]\n",
@@ -384,15 +384,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "def shock(v):\n",
                 "\tc = random.normal(v, 4)\n",
                 "\treturn c if c >= 1 else 1\n",
-                "heli.shocks.add('Dwarf real balances', ('rbd','breed','dwarf','agent'), shock, heli.shocks.randn(2))\n",
+                "heli.shocks.add('Dwarf real balances', ('rbd','dwarf'), shock, heli.shocks.randn(2))\n",
                 "\n",
                 "def mshock(model):\n",
                 "\tpct = random.normal(3, 15) #High mean to counteract the downward bias of (1-%)(1+%)\n",
                 "\tm = model.cb.M0 * (1+pct/100)\n",
                 "\tm = max(m, 10000)\t#Things get weird when there's a money shortage\n",
                 "\tmodel.cb.M0 = m\n",
                 "heli.shocks.add('M0 (2% prob)', None, mshock, heli.shocks.randn(2), desc=\"Shocks the money supply a random percentage (\u00b5=1, \u03c3=15) with 2% probability each period\")\n",
@@ -454,13 +454,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.5"
+            "version": "3.12.1"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `helipad-1.6/sample-notebooks/pricediscover.ipynb` & `helipad-1.6.1/sample-notebooks/pricediscover.ipynb`

 * *Files identical despite different names*

### Comparing `helipad-1.6/sample-notebooks/viz-tutorial.ipynb` & `helipad-1.6.1/sample-notebooks/viz-tutorial.ipynb`

 * *Files identical despite different names*

