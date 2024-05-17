# Comparing `tmp/rahavard-0.0.14.tar.gz` & `tmp/rahavard-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rahavard-0.0.14.tar", last modified: Wed Apr 17 19:37:18 2024, max compression
+gzip compressed data, was "rahavard-0.0.15.tar", last modified: Fri May 17 04:22:00 2024, max compression
```

## Comparing `rahavard-0.0.14.tar` & `rahavard-0.0.15.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-17 19:37:18.385841 rahavard-0.0.14/
--rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-20 17:42:50.000000 rahavard-0.0.14/LICENSE
--rw-r--r--   0 nino      (1000) nino      (1000)      699 2024-04-17 19:37:18.385841 rahavard-0.0.14/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)       93 2024-03-20 17:41:56.000000 rahavard-0.0.14/README.md
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-17 19:37:18.382507 rahavard-0.0.14/rahavard/
--rw-r--r--   0 nino      (1000) nino      (1000)      379 2024-04-17 19:36:01.000000 rahavard-0.0.14/rahavard/__init__.py
--rw-r--r--   0 nino      (1000) nino      (1000)     9279 2024-04-17 19:34:24.000000 rahavard-0.0.14/rahavard/utils.py
-drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-04-17 19:37:18.385841 rahavard-0.0.14/rahavard.egg-info/
--rw-r--r--   0 nino      (1000) nino      (1000)      699 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/PKG-INFO
--rw-r--r--   0 nino      (1000) nino      (1000)      224 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/SOURCES.txt
--rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/dependency_links.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       34 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/requires.txt
--rw-r--r--   0 nino      (1000) nino      (1000)        9 2024-04-17 19:37:18.000000 rahavard-0.0.14/rahavard.egg-info/top_level.txt
--rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-04-17 19:37:18.385841 rahavard-0.0.14/setup.cfg
--rw-r--r--   0 nino      (1000) nino      (1000)     1182 2024-04-17 19:36:31.000000 rahavard-0.0.14/setup.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-05-17 04:22:00.953507 rahavard-0.0.15/
+-rw-r--r--   0 nino      (1000) nino      (1000)     1072 2024-03-20 17:42:50.000000 rahavard-0.0.15/LICENSE
+-rw-r--r--   0 nino      (1000) nino      (1000)      778 2024-05-17 04:22:00.953507 rahavard-0.0.15/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)       93 2024-03-20 17:41:56.000000 rahavard-0.0.15/README.md
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-05-17 04:22:00.950174 rahavard-0.0.15/rahavard/
+-rw-r--r--   0 nino      (1000) nino      (1000)      417 2024-05-17 04:15:45.000000 rahavard-0.0.15/rahavard/__init__.py
+-rw-r--r--   0 nino      (1000) nino      (1000)     9642 2024-05-17 04:15:17.000000 rahavard-0.0.15/rahavard/utils.py
+drwxr-xr-x   0 nino      (1000) nino      (1000)        0 2024-05-17 04:22:00.953507 rahavard-0.0.15/rahavard.egg-info/
+-rw-r--r--   0 nino      (1000) nino      (1000)      778 2024-05-17 04:22:00.000000 rahavard-0.0.15/rahavard.egg-info/PKG-INFO
+-rw-r--r--   0 nino      (1000) nino      (1000)      224 2024-05-17 04:22:00.000000 rahavard-0.0.15/rahavard.egg-info/SOURCES.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)        1 2024-05-17 04:22:00.000000 rahavard-0.0.15/rahavard.egg-info/dependency_links.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       34 2024-05-17 04:22:00.000000 rahavard-0.0.15/rahavard.egg-info/requires.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)        9 2024-05-17 04:22:00.000000 rahavard-0.0.15/rahavard.egg-info/top_level.txt
+-rw-r--r--   0 nino      (1000) nino      (1000)       38 2024-05-17 04:22:00.953507 rahavard-0.0.15/setup.cfg
+-rw-r--r--   0 nino      (1000) nino      (1000)     1182 2024-05-17 04:16:43.000000 rahavard-0.0.15/setup.py
```

### Comparing `rahavard-0.0.14/LICENSE` & `rahavard-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `rahavard-0.0.14/PKG-INFO` & `rahavard-0.0.15/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rahavard
-Version: 0.0.14
+Version: 0.0.15
 Summary: Re-Usable Utils
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,12 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: convert_numbers
+Requires-Dist: jdatetime
+Requires-Dist: natsort
 
 
 # rahavard
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
```

### Comparing `rahavard-0.0.14/rahavard/utils.py` & `rahavard-0.0.15/rahavard/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     else:
         suff = ['B', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB']
     i = int(floor(math_log(size_in_bytes, 1024)))
     p = math_pow(1024, i)
     conv = f'{float(size_in_bytes / p):.1f}'
 
     ## remove trailing .0 or .00
-    reg = '^[0-9]+\.0+$'
+    reg = r'^[0-9]+\.0+$'
     if match(reg, conv):
-        conv = sub('\.0+$', '', conv)
+        conv = sub(r'\.0+$', '', conv)
 
     if to_persian:
         return f'{persianize(conv)} {suff[i]}'
 
     return f'{conv}{suff[i]}'
 
 
@@ -120,14 +120,32 @@
         result = sub(r'^0+:0([0-9]):', r'\1:', result)          ## 0:00:12 -> 0:12
                                                                 ## 0:08:12 -> 8:12
         result = sub(r'^0+:([1-9])([0-9]):', r'\1\2:', result)  ## 0:10:12 -> 10:12
 
     return result
 
 
+def convert_string_True_False_None_0(item):
+    '''
+        'True'  -> True
+        'False' -> False
+        'None'  -> None
+        '0'     -> 0
+    '''
+
+    if item in ['True', 'False', 'None', '0']:
+        return {
+            'True': True,
+            'False': False,
+            'None': None,
+            '0': 0,
+        }.get(item)
+    return item
+
+
 def convert_timestamp_to_jalali(tmstmp=None):
     '''
     takes timestamp, e.g. 1682598113
     and converts it to jalali in this format: چهارشنبه ۰۷:۰۶:۳۳ ۳۰-/۰۱/۱۴۰۲
     '''
 
     if not tmstmp:
@@ -215,15 +233,15 @@
             return '~۰'
         return '~0'
 
     _perc = int(_perc * 10) / 10  ## 99.95232355216523 -> 99.9
     ## NOTE we didn't use f'{_perc:.1f}'
     ##      because it turns 99.95232355216523 to 100.0
 
-    _perc = sub('\.0+$', '', str(_perc))  ## 97.0 -> 97
+    _perc = sub(r'\.0+$', '', str(_perc))  ## 97.0 -> 97
 
     if to_persian:
         return persianize(_perc)
 
     return _perc
 
 ## inspired by:
@@ -237,21 +255,21 @@
 
     commad = ''
     left = ''
     right = ''
     is_float = False
 
     ## JUMP_1 is float
-    if match('^[۱۲۳۴۵۶۷۸۹۰]+\.[۱۲۳۴۵۶۷۸۹۰]+$', num):
+    if match(r'^[۱۲۳۴۵۶۷۸۹۰]+\.[۱۲۳۴۵۶۷۸۹۰]+$', num):
         left, right = num.split('.')
         separator = '.'
         is_float = True
 
     ## JUMP_1 is float
-    elif match('^[۱۲۳۴۵۶۷۸۹۰]+\/[۱۲۳۴۵۶۷۸۹۰]+$', num):
+    elif match(r'^[۱۲۳۴۵۶۷۸۹۰]+\/[۱۲۳۴۵۶۷۸۹۰]+$', num):
         left, right = num.split('/')
         separator = '/'
         is_float = True
 
     else:
         left = num
 
@@ -267,15 +285,15 @@
 
     return commad
 
 def persianize(number):
     number = str(number)
 
     ## JUMP_1 is float
-    if match('^[0-9]+\.[0-9]+$', number):
+    if match(r'^[0-9]+\.[0-9]+$', number):
         _left, _right = number.split('.')
         if match('^0+$', _right):
             return english_to_persian(_left)
         return f'{english_to_persian(_left)}.{english_to_persian(_right[:2])}'
 
     return english_to_persian(int(number))
```

### Comparing `rahavard-0.0.14/rahavard.egg-info/PKG-INFO` & `rahavard-0.0.15/rahavard.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rahavard
-Version: 0.0.14
+Version: 0.0.15
 Summary: Re-Usable Utils
 Author: Davoud Arsalani
 Author-email: d_arsalani@yahoo.com
 Keywords: python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,12 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Utilities
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: convert_numbers
+Requires-Dist: jdatetime
+Requires-Dist: natsort
 
 
 # rahavard
 
 Under construction! Not ready for use yet! Currently experimenting and planning!
```

### Comparing `rahavard-0.0.14/setup.py` & `rahavard-0.0.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 here = path.abspath(path.dirname(__file__))
 with codecs.open(path.join(here, 'README.md'), encoding='utf-8') as opened:
     long_description = '\n' + opened.read()
 
 
-VERSION = '0.0.14'
+VERSION = '0.0.15'
 DESCRIPTION = 'Re-Usable Utils'
 LONG_DESCRIPTION = 'Re-Usable Utils to Be Used on Our Django Projects'
 
 setup(
     name='rahavard',
     version=VERSION,
     author='Davoud Arsalani',
```

