# Comparing `tmp/pyfilemaker2-0.2.5.tar.gz` & `tmp/pyfilemaker2-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfilemaker2-0.2.5.tar", last modified: Tue Feb 28 15:09:41 2023, max compression
+gzip compressed data, was "pyfilemaker2-0.2.6.tar", last modified: Fri May 17 20:09:03 2024, max compression
```

## Comparing `pyfilemaker2-0.2.5.tar` & `pyfilemaker2-0.2.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2023-02-28 15:09:41.976020 pyfilemaker2-0.2.5/
--rw-r--r--   0 jeremie    (503) staff       (20)     1491 2022-10-12 07:26:04.000000 pyfilemaker2-0.2.5/LICENSE.txt
--rw-r--r--   0 jeremie    (503) staff       (20)       74 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.5/MANIFEST.in
--rw-r--r--   0 jeremie    (503) staff       (20)     4526 2023-02-28 15:09:41.975433 pyfilemaker2-0.2.5/PKG-INFO
--rw-r--r--   0 jeremie    (503) staff       (20)     3608 2023-02-28 15:09:06.000000 pyfilemaker2-0.2.5/README.md
-drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2023-02-28 15:09:41.939583 pyfilemaker2-0.2.5/dummy/
--rw-r--r--   0 jeremie    (503) staff       (20)        0 2021-12-04 10:15:40.000000 pyfilemaker2-0.2.5/dummy/__init__.py
--rwxr-xr-x   0 jeremie    (503) staff       (20)     5689 2021-12-07 10:03:45.000000 pyfilemaker2-0.2.5/dummy/dummy.py
-drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2023-02-28 15:09:41.945621 pyfilemaker2-0.2.5/pyfilemaker2/
--rw-r--r--   0 jeremie    (503) staff       (20)      131 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.5/pyfilemaker2/__init__.py
--rw-r--r--   0 jeremie    (503) staff       (20)     3854 2023-02-28 15:06:46.000000 pyfilemaker2-0.2.5/pyfilemaker2/caster.py
--rw-r--r--   0 jeremie    (503) staff       (20)     1915 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.5/pyfilemaker2/data.py
-drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2023-02-28 15:09:41.959999 pyfilemaker2-0.2.5/pyfilemaker2/errors/
--rw-r--r--   0 jeremie    (503) staff       (20)      481 2021-12-07 10:06:23.000000 pyfilemaker2-0.2.5/pyfilemaker2/errors/__init__.py
--rw-r--r--   0 jeremie    (503) staff       (20)    14491 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.5/pyfilemaker2/errors/errors_fms17.py
--rw-r--r--   0 jeremie    (503) staff       (20)     8005 2023-02-28 15:07:16.000000 pyfilemaker2-0.2.5/pyfilemaker2/metadata.py
--rw-r--r--   0 jeremie    (503) staff       (20)     4794 2021-12-07 10:13:59.000000 pyfilemaker2-0.2.5/pyfilemaker2/parser.py
--rw-r--r--   0 jeremie    (503) staff       (20)    33552 2023-02-28 15:07:48.000000 pyfilemaker2-0.2.5/pyfilemaker2/server.py
-drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2023-02-28 15:09:41.974345 pyfilemaker2-0.2.5/pyfilemaker2/tests/
--rw-r--r--   0 jeremie    (503) staff       (20)        0 2018-09-01 05:40:35.000000 pyfilemaker2-0.2.5/pyfilemaker2/tests/__init__.py
-drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2023-02-28 15:09:41.974891 pyfilemaker2-0.2.5/pyfilemaker2/tests/ressources/
--rw-r--r--   0 jeremie    (503) staff       (20)        0 2018-11-20 20:15:34.000000 pyfilemaker2-0.2.5/pyfilemaker2/tests/ressources/__init__.py
--rw-r--r--   0 jeremie    (503) staff       (20)     1824 2021-12-07 10:06:23.000000 pyfilemaker2-0.2.5/pyfilemaker2/tests/test_caster.py
--rw-r--r--   0 jeremie    (503) staff       (20)     2022 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.5/pyfilemaker2/tests/test_data.py
--rw-r--r--   0 jeremie    (503) staff       (20)     3343 2021-12-07 10:06:23.000000 pyfilemaker2-0.2.5/pyfilemaker2/tests/test_metadata.py
--rw-r--r--   0 jeremie    (503) staff       (20)     4265 2022-10-12 07:38:01.000000 pyfilemaker2-0.2.5/pyfilemaker2/tests/test_server.py
-drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2023-02-28 15:09:41.950033 pyfilemaker2-0.2.5/pyfilemaker2.egg-info/
--rw-r--r--   0 jeremie    (503) staff       (20)     4526 2023-02-28 15:09:41.000000 pyfilemaker2-0.2.5/pyfilemaker2.egg-info/PKG-INFO
--rw-r--r--   0 jeremie    (503) staff       (20)      671 2023-02-28 15:09:41.000000 pyfilemaker2-0.2.5/pyfilemaker2.egg-info/SOURCES.txt
--rw-r--r--   0 jeremie    (503) staff       (20)        1 2023-02-28 15:09:41.000000 pyfilemaker2-0.2.5/pyfilemaker2.egg-info/dependency_links.txt
--rw-r--r--   0 jeremie    (503) staff       (20)       14 2023-02-28 15:09:41.000000 pyfilemaker2-0.2.5/pyfilemaker2.egg-info/requires.txt
--rw-r--r--   0 jeremie    (503) staff       (20)       13 2023-02-28 15:09:41.000000 pyfilemaker2-0.2.5/pyfilemaker2.egg-info/top_level.txt
--rw-r--r--   0 jeremie    (503) staff       (20)       38 2023-02-28 15:09:41.976184 pyfilemaker2-0.2.5/setup.cfg
--rwxr-xr-x   0 jeremie    (503) staff       (20)     1465 2023-02-28 15:02:33.000000 pyfilemaker2-0.2.5/setup.py
+drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2024-05-17 20:09:03.322782 pyfilemaker2-0.2.6/
+-rw-r--r--   0 jeremie    (503) staff       (20)     1491 2022-10-12 07:26:04.000000 pyfilemaker2-0.2.6/LICENSE.txt
+-rw-r--r--   0 jeremie    (503) staff       (20)       74 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.6/MANIFEST.in
+-rw-r--r--   0 jeremie    (503) staff       (20)     4748 2024-05-17 20:09:03.322167 pyfilemaker2-0.2.6/PKG-INFO
+-rw-r--r--   0 jeremie    (503) staff       (20)     3830 2023-03-02 07:38:38.000000 pyfilemaker2-0.2.6/README.md
+drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2024-05-17 20:09:03.298743 pyfilemaker2-0.2.6/dummy/
+-rw-r--r--   0 jeremie    (503) staff       (20)        0 2021-12-04 10:15:40.000000 pyfilemaker2-0.2.6/dummy/__init__.py
+-rwxr-xr-x   0 jeremie    (503) staff       (20)     3125 2024-05-16 15:48:00.000000 pyfilemaker2-0.2.6/dummy/dummy.py
+drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2024-05-17 20:09:03.305533 pyfilemaker2-0.2.6/pyfilemaker2/
+-rw-r--r--   0 jeremie    (503) staff       (20)      131 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.6/pyfilemaker2/__init__.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     4050 2024-05-16 15:10:57.000000 pyfilemaker2-0.2.6/pyfilemaker2/caster.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     1934 2024-05-16 15:56:16.000000 pyfilemaker2-0.2.6/pyfilemaker2/data.py
+drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2024-05-17 20:09:03.314745 pyfilemaker2-0.2.6/pyfilemaker2/errors/
+-rw-r--r--   0 jeremie    (503) staff       (20)      481 2021-12-07 10:06:23.000000 pyfilemaker2-0.2.6/pyfilemaker2/errors/__init__.py
+-rw-r--r--   0 jeremie    (503) staff       (20)    14491 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.6/pyfilemaker2/errors/errors_fms17.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     9931 2024-05-17 19:38:09.000000 pyfilemaker2-0.2.6/pyfilemaker2/metadata.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     5135 2024-05-17 06:37:50.000000 pyfilemaker2-0.2.6/pyfilemaker2/parser.py
+-rw-r--r--   0 jeremie    (503) staff       (20)    35548 2024-05-17 19:47:56.000000 pyfilemaker2-0.2.6/pyfilemaker2/server.py
+drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2024-05-17 20:09:03.320093 pyfilemaker2-0.2.6/pyfilemaker2/tests/
+-rw-r--r--   0 jeremie    (503) staff       (20)        0 2018-09-01 05:40:35.000000 pyfilemaker2-0.2.6/pyfilemaker2/tests/__init__.py
+drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2024-05-17 20:09:03.321144 pyfilemaker2-0.2.6/pyfilemaker2/tests/ressources/
+-rw-r--r--   0 jeremie    (503) staff       (20)        0 2018-11-20 20:15:34.000000 pyfilemaker2-0.2.6/pyfilemaker2/tests/ressources/__init__.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     1824 2021-12-07 10:06:23.000000 pyfilemaker2-0.2.6/pyfilemaker2/tests/test_caster.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     2022 2021-09-28 11:10:32.000000 pyfilemaker2-0.2.6/pyfilemaker2/tests/test_data.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     3339 2024-05-17 19:41:32.000000 pyfilemaker2-0.2.6/pyfilemaker2/tests/test_metadata.py
+-rw-r--r--   0 jeremie    (503) staff       (20)     4808 2024-05-17 06:22:59.000000 pyfilemaker2-0.2.6/pyfilemaker2/tests/test_server.py
+drwxr-xr-x   0 jeremie    (503) staff       (20)        0 2024-05-17 20:09:03.312738 pyfilemaker2-0.2.6/pyfilemaker2.egg-info/
+-rw-r--r--   0 jeremie    (503) staff       (20)     4748 2024-05-17 20:09:03.000000 pyfilemaker2-0.2.6/pyfilemaker2.egg-info/PKG-INFO
+-rw-r--r--   0 jeremie    (503) staff       (20)      671 2024-05-17 20:09:03.000000 pyfilemaker2-0.2.6/pyfilemaker2.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremie    (503) staff       (20)        1 2024-05-17 20:09:03.000000 pyfilemaker2-0.2.6/pyfilemaker2.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremie    (503) staff       (20)       14 2024-05-17 20:09:03.000000 pyfilemaker2-0.2.6/pyfilemaker2.egg-info/requires.txt
+-rw-r--r--   0 jeremie    (503) staff       (20)       13 2024-05-17 20:09:03.000000 pyfilemaker2-0.2.6/pyfilemaker2.egg-info/top_level.txt
+-rw-r--r--   0 jeremie    (503) staff       (20)       38 2024-05-17 20:09:03.322993 pyfilemaker2-0.2.6/setup.cfg
+-rwxr-xr-x   0 jeremie    (503) staff       (20)     1465 2024-05-17 19:51:18.000000 pyfilemaker2-0.2.6/setup.py
```

### Comparing `pyfilemaker2-0.2.5/LICENSE.txt` & `pyfilemaker2-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfilemaker2-0.2.5/PKG-INFO` & `pyfilemaker2-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilemaker2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python Object Wrapper for FileMaker Server XML Interface
 Home-page: https://github.com/jeremie-borel/pyfilemaker2/
 Author: Klokan Petr Pridal, Pieter Claerhout, Marcin Kawa, Jeremie Borel
 Author-email: klokan@klokan.cz, pieter@yellowduck.be, kawa.macin@gmail.com
 License: http://www.opensource.org/licenses/bsd-license.php
 Download-URL: https://github.com/jeremie-borel/pyfilemaker2/
 Keywords: FileMaker
@@ -107,15 +107,15 @@
 extensive docstring. Starts in particular with the server.py file. Moreover an
 FmServer object is likely the unique thing one will need to import from this
 package.
 
 ### 5. CHANGES
 
 0.2.5:
-- server_timezone parameter now requires a zoneinfo.ZoneInfo object or None.
+- BACKWARD INCOMPATIBLE: server_timezone parameter now requires a zoneinfo.ZoneInfo object or None. Timezones from pytz are not supported anymore. To use another package (e.g. pytz), one can overload the BackCast class from caster and define it as the :back_cast_class: static member of FmInstance.
 
 0.2.4:
 - Fix https://github.com/jeremie-borel/pyfilemaker2/issues/1 that prevented FMS 19 to work.
 
 0.2.3:
 -
```

### Comparing `pyfilemaker2-0.2.5/README.md` & `pyfilemaker2-0.2.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 extensive docstring. Starts in particular with the server.py file. Moreover an
 FmServer object is likely the unique thing one will need to import from this
 package.
 
 ### 5. CHANGES
 
 0.2.5:
-- server_timezone parameter now requires a zoneinfo.ZoneInfo object or None.
+- BACKWARD INCOMPATIBLE: server_timezone parameter now requires a zoneinfo.ZoneInfo object or None. Timezones from pytz are not supported anymore. To use another package (e.g. pytz), one can overload the BackCast class from caster and define it as the :back_cast_class: static member of FmInstance.
 
 0.2.4:
 - Fix https://github.com/jeremie-borel/pyfilemaker2/issues/1 that prevented FMS 19 to work.
 
 0.2.3:
 -
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/caster.py` & `pyfilemaker2-0.2.6/pyfilemaker2/caster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # -*- coding: utf-8 -*-
 import datetime
 import numbers
-from typing import Any, Optional
+from typing import Any, Optional, TYPE_CHECKING
 
-# from builtins import str
+
+if TYPE_CHECKING:
+    from .metadata import (
+        FmMeta,
+        FmFieldBase,
+        FmFieldData,
+    )
 
 __all__ = ['default_cast_map']
 
 FM_NUMBER = 'number'
 FM_TEXT = 'text'
 FM_DATE = 'date'
 FM_TIME = 'time'
 FM_TIMESTAMP = 'timestamp'
 
 
 class TypeCast:
     """Type caster, get's initiated with the corresponding FmFieldData"""
 
-    def __init__(self, fm_field, fm_meta):
+    def __init__(self, fm_field: 'FmFieldBase', fm_meta: 'FmMeta'):
         pass
 
     def __call__(self, value: str) -> Any:
         return value
 
 
 class NumberCast(TypeCast):
@@ -49,44 +55,44 @@
         return ''
 
 
 DummyCast = TextCast
 
 
 class DateCast(TypeCast):
-    def __init__(self, fm_field, fm_meta):
+    def __init__(self, fm_field: 'FmFieldData', fm_meta: 'FmMeta'):
         self.pat = fm_meta.date_pattern
 
     def __call__(self, value: str) -> Optional[datetime.date]:
         try:
             d = datetime.datetime.strptime(
                 value,
                 self.pat,
             )
             return d.date()
         except (ValueError, TypeError):
             return None
 
 
 class TimeCast(TypeCast):
-    def __init__(self, fm_field, fm_meta):
+    def __init__(self, fm_field, fm_meta: 'FmMeta'):
         self.pat = fm_meta.time_pattern
 
     def __call__(self, value: str) -> Optional[datetime.time]:
         try:
             return datetime.datetime.strptime(
                 value,
                 self.pat,
             ).time()
         except (ValueError, TypeError):
             return None
 
 
 class TimestampCast(TypeCast):
-    def __init__(self, fm_field, fm_meta):
+    def __init__(self, fm_field, fm_meta: 'FmMeta'):
         self.pat = fm_meta.timestamp_pattern
         self.tz = fm_meta.server_timezone
 
     def __call__(self, value: str) -> Optional[datetime.datetime]:
         try:
             d = datetime.datetime.strptime(
                 value,
@@ -136,14 +142,14 @@
 
         elif isinstance(value, numbers.Number):
             return value
 
         return str(value)
 
 
-default_cast_map = {
+default_cast_map: dict[str, type[TypeCast]] = {
     FM_NUMBER: NumberCast,
     FM_TEXT: TextCast,
     FM_DATE: DateCast,
     FM_TIME: TimeCast,
     FM_TIMESTAMP: TimestampCast,
 }
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/data.py` & `pyfilemaker2-0.2.6/pyfilemaker2/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,59 +3,64 @@
 __all__ = ['MutableDict']
 
 
 class MutableDict(dict):
     """
     Thin wrapper around dict that tracks keys that are set more than once.
 
-    It also keeps tracks the record_id and the mod_id is applicable
+    It can also keeps tracks the record_id and the mod_id when applicable
     """
     def __init__(self, *args, **kwargs):
-        super(MutableDict, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.__key_counter = Counter(self.keys())
         self.record_id = None
         self.mod_id = None
 
     def __setitem__(self, key, value):
         self.__key_counter[key] += 1
-        super(MutableDict, self).__setitem__(key, value)
+        super().__setitem__(key, value)
 
     def __delitem__(self, key):
-        super(MutableDict, self).__delitem__(key)
+        super().__delitem__(key)
         self.__key_counter[key] += 1
 
     def pop(self, key, default=None):
         if key in self.keys():
             self.__key_counter[key] += 1
-        return super(MutableDict, self).pop(key, default)
+        return super().pop(key, default)
 
     def popitem(self):
-        e = super(MutableDict, self).popitem()
+        e = super().popitem()
         self.__key_counter[e[0]] += 1
 
     def clear(self):
         for k in self.keys():
             self.__key_counter[k] += 1
-        return super(MutableDict, self).clear()
+        return super().clear()
 
     def update(self, other):
         # TODO: implement a more generic way of handling the :other: argument
         # WARNING: atm the x.update(a=22,b=35) syntax is not supported.
         if hasattr(other, 'keys'):
             for k in other.keys():
                 self.__key_counter[k] += 1
         else:
             try:
                 for k, v in other:
                     self.__key_counter[k] += 1
             except Exception:
                 pass
 
-        return super(MutableDict, self).update(other)
+        return super().update(other)
 
     def setdefault(self, key, default):
         if key in self.keys():
             self.__key_counter[key] += 1
-        return super(MutableDict, self).setdefault(key, default)
+        return super().setdefault(key, default)
+
+    def reset_all_counters(self):
+        """Mark all keys as untouched."""
+        for key in self.keys():
+            self.__key_counter[key] = 1
 
     def changed_keys(self):
         return tuple(k for k, v in self.__key_counter.items() if v > 1)
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/errors/errors_fms17.py` & `pyfilemaker2-0.2.6/pyfilemaker2/errors/errors_fms17.py`

 * *Files identical despite different names*

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/metadata.py` & `pyfilemaker2-0.2.6/pyfilemaker2/metadata.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,110 +1,133 @@
-#!/usr/bin/env python
+import logging
+from typing import Optional, TYPE_CHECKING, Union
+from zoneinfo import ZoneInfo
+
 
 from .data import MutableDict
 
 from .caster import (
     DummyCast,
     default_cast_map
 )
 
+if TYPE_CHECKING:
+    from lxml.etree import _Element
+    from .caster import TypeCast
+    from .server import FmQuery, FmRecord
+
 __all__ = ['FmMeta', 'metadata_parser', 'FmFieldBase', 'FmFieldData']
 
+log = logging.getLogger(__name__)
 
-class FmMeta():
+class FmMeta:
     """
     FmMeta objects hold all the information about an xml query to an FMS server
     - date, time and timestamp formats
     - fields definition and how to cast them into python objects
     - relatedset fields definition
-
     """
 
-    def __init__(self, cast_map=None, server_timezone=None):
+    def __init__(
+        self,
+        cast_map: dict[str, type['TypeCast']] = {},
+        server_timezone: Optional[ZoneInfo] = None
+    ):
         self.cast_map = default_cast_map
         if cast_map:
             self.cast_map.update(cast_map)
         self.server_timezone = server_timezone
 
-        self.ns = None
+        # namespace of the xml. http://www.filemaker.com/xml/fmresultset
+        self.ns: str = ''
+
         self._ns_length = 0
-        self.database = None
-        self.error = None
-        self.date_pattern = None
-        self.time_pattern = None
-        self.timestamp_pattern = None
-        self.db_name = None
-        self.layout = None
-        self.table = None
+        self.database: dict[str, str] = {}
+        self.error: Optional[int] = None
+        self.date_pattern: str = ''
+        self.time_pattern: str = ''
+        self.timestamp_pattern: str = ''
+        self.db_name: str = ''
+        self.layout: str = ''
+        self.table: str = ''
         self.encoding = 'utf8'
+        self.fms_version: str = ''
+        self.total_count: int = -1
+        self.fetch_count: int = -1
         self.fields = {}
+        self.query: Optional['FmQuery'] = None
 
-    def get_tagname(self, node):
+    def get_tagname(self, node) -> str:
         """Returns the tag name striped from the ns name at the begining"""
         return node.tag[self._ns_length:]
 
-    def add_field(self, field):
+    def add_field(self, field: 'FmFieldData'):
         """Adds an FmFieldBase object in the current context"""
-        # name = field.name
         raw_name = field.raw_name
         if not raw_name:
             return
 
         field.splitted_names = raw_name.split('::', 1)
         if field.table and field.table != field.splitted_names[0]:
-            field.splitted_names = tuple([field.table] + field.splitted_names)
-
+            field.splitted_names = list([field.table] + field.splitted_names)
         ukey = raw_name
         if field.table:
-            ukey = "{}__{}".format(field.table, raw_name)
+            ukey = f"{field.table}__{raw_name}"
+        if ukey in self.fields:
+            log.warning(
+                f"One field ({ukey}) exists twice in the layout. This is "
+                "a problem because the FmRecord value is set twice and so "
+                "will be considered as edited. If this field is a computed "
+                "value on FMS and one calls do_edit(record), the call will fail."
+            )
         self.fields[ukey] = field
 
-    def get_fm_field(self, raw_name, table):
-        if not table:
+    def get_fm_field(self, raw_name: str, related_table: str) -> 'FmFieldData':
+        if not related_table:
             return self.fields[raw_name]
-        return self.fields["{}__{}".format(table, raw_name)]
+        return self.fields[f"{related_table}__{raw_name}"]
 
     def set_context(self, name, field=None):
         if name is None or name == '':
             self._context = self.fields
             return
         if name not in self.fields:
             self.fields[name] = field
         self._context = self.fields[name]
 
-    def decode_attrs(self, value):
+    def decode_attrs(self, value: Union[bytes, str]) -> str:
         if not isinstance(value, str):
             return value.decode(self.encoding)
         return value
 
-    def decode_data(self, value):
+    def decode_data(self, value: Union[bytes, str, None]) -> Optional[str]:
         if value is not None:
             if not isinstance(value, str):
                 return value.decode(self.encoding)
             return value
         return None
 
     # def sanitize_field_identifier(self, value):
     #     val = unidecode(value)
     #     return val.replace('::','_')
 
-    def parse_fm_dates_formats(self, formats):
+    def parse_fm_dates_formats(self, formats: dict[str, str]) -> dict[str, str]:
         """
         Takes a dict build from the datasource node of an xml FMS result, e.g.
         <datasource
         ...
         date-format="MM/dd/yyyy"
         time-format="HH:mm:ss"
         timestamp-format="MM/dd/yyyy HH:mm:ss">
         </datasource>
 
         And converts all the datetime formats to formats that can be used in
         datetime.datetime.strptime
         """
-        def _build_one(stamp):
+        def _build_one(stamp) -> str:
             return (
                 stamp
                 .replace('yyyy', '%Y')
                 .replace('MM', '%m')
                 .replace('dd', '%d')
                 .replace('HH', '%H')
                 .replace('mm', '%M')
@@ -113,113 +136,142 @@
 
         return {
             'date': _build_one(formats.get('date-format', '')),
             'timestamp': _build_one(formats.get('timestamp-format', '')),
             'time': _build_one(formats.get('time-format', '')),
         }
 
-    def get_record_class(self):
+    def get_record_class(self) -> type[MutableDict]:
         return MutableDict
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "<{klass} ({x.db_name},layout:{x.layout}) {error} fields:({fields})>".format(
             klass=self.__class__.__name__,
             x=self,
             error=self.error if self.error else '',
             fields=", ".join(self.fields.keys()),
         )
 
-    def dump(self):
+    def dump(self) -> str:
         """Verbose representation of the object"""
         s = ["  " + field.dump() for field in self.fields.values()]
         return "{klass}(({x.db_name},layout:{x.layout}) {error}):\n{fields}".format(
             klass=self.__class__.__name__,
             x=self,
             error=self.error if self.error else '',
             fields="\n".join(s)
         )
 
 
-class FmFieldBase():
-    def __init__(self, raw_name, attrs=None, fm_meta=None, table=None):
+class FmFieldBase:
+    def __init__(
+        self,
+        raw_name: str,
+        attrs: dict[str, str] = {},
+        fm_meta: Optional[FmMeta] = None,
+        table: str = ''
+    ):
         self.raw_name = raw_name
         self.attrs = attrs
         self.fm_meta = fm_meta
         self.table = table
-        self.is_multi = 1  # means False. >1 is True.
+        # self.is_multi=1 means not a multi_value field (in the fms sens). >1 means multi_value.
+        self.is_multi = 1
+        self.splitted_names: list[str] = []
 
     def set_value(self, record, data_list):
         pass
 
-    def dump(self):
+    def dump(self) -> str:
         """Verbose representation of the object"""
         return "'{}'".format(self.raw_name)
 
 
 class FmFieldData(FmFieldBase):
-    def __init__(self, raw_name, attrs=None, fm_meta=None, table=None):
+    def __init__(
+        self,
+        raw_name: str,
+        attrs: dict[str, str] = {},
+        fm_meta: Optional[FmMeta] = None,
+        table: str = ''
+    ):
         super().__init__(
             raw_name=raw_name,
             attrs=attrs,
             fm_meta=fm_meta,
             table=table
         )
         self.is_multi = 0
         if fm_meta:
-            result = attrs.get('result', None)
+            result = attrs.get('result', '')
             caster_class = fm_meta.cast_map.get(result, DummyCast)
             self.caster = caster_class(
                 fm_field=self,
                 fm_meta=fm_meta,
             )
             self.is_multi = int(attrs.get('max-repeat', '1'))
 
-    def set_value(self, record, data_list):
+    def set_value(self, record: dict, data_list: list):
+        """
+        Set the value into the record.
+        """
         value = data_list
         if self.is_multi == 1:
             value = data_list[0]
 
         if len(self.splitted_names) == 1:
             record[self.splitted_names[0]] = value
         else:
-            ctxs = self.splitted_names[:-1]
-            if ctxs[0] == self.table:
-                ctxs = ctxs[1:]
-            name = self.splitted_names[-1]
+            # if self.splitted_names is ['a',''b','c'] we want to create
+            # {'a':{'b':'c': value}}
+            
+            # If path is ['a','b','c'] and table is 'a' we don't repeat 'a'.
+            path = []
+            if self.table:
+                path.append(self.table)
+                if self.splitted_names[0] == self.table:
+                    path.extend(self.splitted_names[1:])
+            else:
+                path = self.splitted_names[:]
+
+            name = path[-1]
+
             obj = record
-            for ctx in ctxs:
+            for ctx in path[:-1]:
                 try:
                     obj = obj[ctx]
                 except KeyError:
                     obj[ctx] = self.fm_meta.get_record_class()()
+                    obj = obj[ctx]
             obj[name] = value
 
-    def dump(self):
+    def dump(self) -> str:
         """Verbose representation of the object"""
         return f"{self.raw_name}: type:{self.caster.__class__.__name__}"
 
 
 class FmFieldContainer(FmFieldBase, dict):
-    def __init__(self, raw_name, attrs=None, fm_meta=None):
-        super().__init__(
-            raw_name=raw_name,
-            attrs=attrs,
-            fm_meta=fm_meta
-        )
+    def __init__(
+        self,
+        raw_name: str,
+        attrs: dict[str, str] = {},
+        fm_meta: Optional[FmMeta] = None,
+    ):
+        super().__init__(raw_name=raw_name,attrs=attrs,fm_meta=fm_meta)
 
     def dump(self):
         """Verbose representation of the object"""
         s = ["     " + field.dump() for field in self.values()]
         return "Container({})\n{}".format(
             self.raw_name,
             "\n".join(s),
         )
 
 
-def metadata_parser(node, fm_meta, table=None):
+def metadata_parser(node: '_Element', fm_meta: FmMeta, table: str = ''):
     """
     Parses the <metadata> node from the xml.
     :fm_meta: is the FmMeta object that is to be defined
     :node: is either the <metadata> node or a <relatedset-definition> subnode
     :table: is defined only when in a <realtedset-definition> node.
     """
     tag = fm_meta.get_tagname(node)
@@ -230,21 +282,20 @@
                 fm_meta=fm_meta,
                 table=table,
             )
     elif tag == 'field-definition':
         f = fm_meta.decode_attrs
         attrs = {f(k): f(v) for k, v in node.attrib.items()}
         raw_name = attrs['name']
-        f = FmFieldData(
+        fm_meta.add_field(FmFieldData(
             raw_name=raw_name,
             attrs=attrs,
             fm_meta=fm_meta,
             table=table
-        )
-        fm_meta.add_field(f)
+        ))
 
     elif tag == 'relatedset-definition':
         f = fm_meta.decode_attrs
         attrs = {f(k): f(v) for k, v in node.attrib.items()}
         table = attrs['table']
 
         f = FmFieldContainer(raw_name=table, fm_meta=fm_meta)
@@ -252,10 +303,10 @@
             for subnode in node:
                 metadata_parser(
                     node=subnode,
                     fm_meta=fm_meta,
                     table=table,
                 )
         except Exception as e:
-            raise e.with_traceback()
+            raise e
         finally:
-            table = None
+            table = ''
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/parser.py` & `pyfilemaker2-0.2.6/pyfilemaker2/parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,95 @@
-#!/usr/bin/env python
-# -*- coding: utf8 -*-
-
+from typing import Generator, Optional, TYPE_CHECKING
 from lxml import etree
 
+
 from .errors import FmError, XmlError
 
 from .metadata import (
     metadata_parser,
     FmMeta,
 )
 
+if TYPE_CHECKING:
+    from pyfilemaker2.data import MutableDict
+
+
 __all__ = ['parse']
 
 
-def parse(stream, fm_meta=None, only_meta=False):
+def parse(
+    stream,
+    fm_meta: Optional[FmMeta] = None,
+    only_meta: bool = False,
+) -> Generator[dict, None, None]:
     """
     Generator that parses an FMS xml response.
 
     :fm_meta: FmMeta instance or None.
 
     :stream: is either a file-like objects or a response.raw attribute from a
     request query.
     """
     if not fm_meta:
         fm_meta = FmMeta()
 
     tree = etree.iterparse(
         stream,
-        # events=("start", "end"),
         events=('start-ns', 'start', 'end'),
     )
 
     record = fm_meta.get_record_class()()
-    table = None  # related table
+    reltable = ''  # related table
     relatedset = []
     data_buffer = []
-    decode = fm_meta.decode_data
     caster = None
     super_record = None
 
     for event, elem in tree:
         if event == 'start-ns':
             fm_meta.ns = elem[1]
             fm_meta._ns_length = len(fm_meta.ns)+2
             continue
 
         elif event == 'end':
             tag = fm_meta.get_tagname(elem)
             if tag == 'data':
-                value = decode(elem.text)
+                value = fm_meta.decode_data(elem.text)
                 if caster:
                     data_buffer.append(caster.caster(value))
 
             elif tag == 'field':
-                raw_name = fm_meta.decode_attrs(elem.attrib.get('name', '')) or None
+                raw_name = fm_meta.decode_attrs(
+                    elem.attrib.get('name', '')
+                )
                 try:
                     field = fm_meta.get_fm_field(
                         raw_name=raw_name,
-                        table=table
+                        related_table=reltable
                     )
                     field.set_value(record=record, data_list=data_buffer)
                 except KeyError:
                     pass
                 data_buffer = []
 
             elif tag == 'record':
                 # end a record. Either in relatedset or not.
                 record.record_id = elem.attrib.get('record-id', None)
                 record.mod_id = elem.attrib.get('mod-id', None)
-                if not table:
+                if not reltable:
                     yield record
                     record = fm_meta.get_record_class()()
 
                 else:
                     relatedset.append(record)
+                    record = fm_meta.get_record_class()()
 
             elif tag == 'relatedset':
-                table = None
-                record = super_record
+                reltable = ''
+                record: 'MutableDict' = super_record
                 super_record = None
 
             elif tag == 'error':
                 fm_meta.error = elem.attrib.get('code', None)
                 if fm_meta.error is None:
                     raise XmlError("Badly formatted error code in the xml")
 
@@ -112,30 +120,33 @@
                 fm_meta.table = fm_meta.database['table']
 
             elif tag == 'metadata':
                 metadata_parser(node=elem, fm_meta=fm_meta)
                 if only_meta:
                     break
 
+            elif tag == 'product':
+                fm_meta.fms_version = elem.attrib.get('version', '')
+
         elif event == 'start':
             tag = fm_meta.get_tagname(elem)
 
             if tag == 'field':
                 try:
                     caster = fm_meta.get_fm_field(
                         raw_name=fm_meta.decode_attrs(elem.attrib['name']),
-                        table=table
+                        related_table=reltable
                     )
                 except KeyError:
                     pass
 
             elif tag == 'relatedset':
-                table = elem.attrib['table']
-                record[table] = []
-                relatedset = record[table]
+                reltable:str= elem.attrib['table']
+                record[reltable] = []
+                relatedset = record[reltable]
                 super_record = record
                 record = fm_meta.get_record_class()()
 
             elif tag == 'resultset':
                 try:
                     _count = int(elem.attrib['count'])
                     fetch_size = int(elem.attrib['fetch-size'])
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/server.py` & `pyfilemaker2-0.2.6/pyfilemaker2/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 
+from typing import Any, Generator, Iterable, Literal, Optional, TypeVar, Union, overload
 from urllib.parse import urlparse, urlencode
 from zoneinfo import ZoneInfo
 
 import requests
 import logging
 import copy
 from re import compile
@@ -10,23 +11,25 @@
 import threading
 import time
 
 from .metadata import FmMeta
 from .errors import FmError
 from .parser import parse
 from .data import MutableDict
-from .caster import BackCast
+from .caster import BackCast, TypeCast
 
+FmRecord = TypeVar('FmRecord', bound=dict)
+FmRecordStream = Generator[FmRecord, None, None]
 
 log = logging.getLogger(__name__)
 
 __all__ = ['FmServer']
 
 
-class FmServer():
+class FmServer:
     """
     Main class to interact with FM server instances.
 
     Note that all the static arguments can also be passed in the **kwargs from
     the FmServder.__init__'s method.
 
     Customize your FmServer instance:
@@ -46,35 +49,35 @@
     or you can pass the argument directly to the constructor:
 
     fm = FmServer(
         cast_map = { FM_NUMBER: CommaDecimalNumberCast }
     )
     """
     meta_class = FmMeta
-    cast_map = None
+    cast_map: dict[str, type[TypeCast]]
     back_cast_class = BackCast
     # ! WARNING: Some FMS *require* the stream=True argument.
     request_kwargs = {
         'stream': True,
         'verify': True,
         'timeout': 25,
     }
-    server_timezone:ZoneInfo = None
+    server_timezone: ZoneInfo
     # see _threaded_paginate function below.
     threaded_paginate = True
-    GET_FILE_REGEX = compile(
+    _GET_FILE_REGEX = compile(
         r'/fmi/xml/cnt/(?P<name>[,%\w\d.-]+)\.(?P<ext>[\w]+)[?]-'
     )
 
     def __init__(
         self,
-        url='http://login:password@localhost/fmi/xml/fmresultset.xml',
-        db='',
-        layout='',
-        debug=False,
+        url: str = 'http://login:password@localhost/fmi/xml/fmresultset.xml',
+        db: str = '',
+        layout: str = '',
+        debug: bool = False,
         **kwargs
     ):
         o = urlparse(url)
         path = o.path
         if path == '/':
             path = None
         self.url = {
@@ -87,61 +90,64 @@
             'path': path or '/fmi/xml/fmresultset.xml',
         }
 
         self.db = db
         self.layout = layout
 
         self.debug = debug
-        self.fm_meta = None
+        self.fm_meta: Optional[FmMeta] = None
 
         self.options = {}
         optkeys = (
             'meta_class',
             'back_cast_class',
             'cast_map',
             'request_kwargs',
             'server_timezone',
             'threaded_paginate',
         )
         for key in optkeys:
             if key in kwargs:
-                base = getattr(self.__class__, key)
+                base = getattr(self.__class__, key, None)
                 # copying default value if the argument is a dict.
                 if hasattr(base, 'update'):
                     self.options[key] = copy.copy(getattr(self.__class__, key))
                     self.options[key].update(kwargs[key])
                 else:
                     self.options[key] = copy.copy(kwargs[key])
             else:
-                self.options[key] = copy.copy(getattr(self.__class__, key))
+                self.options[key] = copy.copy(
+                    getattr(self.__class__, key, None)
+                )
 
-    def get_db_names(self):
+    def get_db_names(self) -> tuple[str]:
         """Returns the list of databases available through xml"""
         query = FmQuery(action='-dbnames', fm_server=self)
         stream = self._do_request(query)
         return tuple(v['DATABASE_NAME'] for v in stream)
 
-    def get_layout_names(self):
+    def get_layout_names(self) -> tuple[str]:
         """Returns a tuple of all the available layouts in a db."""
         query = FmQuery(action='-layoutnames', fm_server=self)
         stream = self._do_request(query)
         return tuple(v['LAYOUT_NAME'] for v in stream)
 
-    def get_script_names(self):
+    def get_script_names(self) -> tuple[str]:
         """Retrurns a tuple of all the scripts"""
         query = FmQuery(action='-scriptnames', fm_server=self)
         stream = self._do_request(query)
         return tuple(v['SCRIPT_NAME'] for v in stream)
 
-    def get_field_names(self):
+    def get_field_names(self) -> tuple[str]:
         """Returns a tuple of all the fields accessible in the layout"""
         self.do_view()
+        assert (self.fm_meta)  # self.do_view sets fm_meta
         return tuple(self.fm_meta.fields.keys())
 
-    def get_file(self, file_xml_uri, canonical_filename=True):
+    def get_file(self, file_xml_uri, canonical_filename=True) -> tuple[str, str, bytes]:
         """Fetches container data from an FM server
 
         e.g. on file mydb.fmp12, a layout 'my_layout' has a field 'join'
         of type container
 
             fm = FmServer(db='mydb', layout=my_layout)
             record = fm.do_find_any()
@@ -153,24 +159,24 @@
         if :canonical_filename: is True, the filename and file extension must
         match the regexp pattern below. Otherwise filename and file_extension
         are empty strings.
         """
         file_name = ""
         file_extension = ""
         if canonical_filename:
-            find = FmServer.GET_FILE_REGEX.match(file_xml_uri)
+            find = FmServer._GET_FILE_REGEX.match(file_xml_uri)
             if not find:
                 raise FmError(code=700)
 
             file_name = find.group('name')
             file_extension = find.group('ext')
         file_binary = self._do_request(is_file=True, query=file_xml_uri)
         return (file_name, file_extension, file_binary)
 
-    def do_script(self, script_name, param=None, return_all=True):
+    def do_script(self, script_name: str, param: str = '', return_all: bool = True) -> FmRecordStream:
         """
         Triggers the excution of script :script_name: on the FM server.
         Note that a script always returns the results from the layout with
         findall.
 
         Returns an iterator.
 
@@ -201,45 +207,61 @@
 
         stream = self._do_request(query)
         return stream
 
     def do_script_after(self, func, func_kwargs={}, script_name='', params=None):
         raise NotImplementedError("not yet implemented")
 
-    def fetched_records_number(self, safe=True):
-        """Returns the number of result in the resultset
+    def fetched_records_number(self, safe: bool = True) -> int:
+        """Return the number of result in the resultset
 
         ATM available only once the first result has been parsed, not before.
         """
         try:
             return self.fm_meta.fetch_count
-        except AttributeError:
+        except Exception:
             if safe:
                 return -1
             raise AttributeError("Resultset has not been evaluated yet.")
 
-    def total_records_number(self, safe=True):
+    def total_records_number(self, safe: bool = True) -> int:
         """
         Returns the number of result that would be returned in a do_find_all
         request.
 
         Available only once the first result has been parsed, not before. E.g.
 
           fm = FmServer(...)
           fm.do_find_any()     # queries and parses the resultset
           fm.total_records_number()
         """
         try:
             return self.fm_meta.total_count
-        except AttributeError:
+        except Exception:
             if safe:
                 return -1
-            raise AttributeError("Resultset has not been evaluated yet.")
+        raise AttributeError("Resultset has not been evaluated yet.")
+
+    def fms_version(self, safe: bool=True) -> str:
+        """Return the version of the server."""
+        try:
+            return self.fm_meta.fms_version
+        except Exception:
+            if safe:
+                return ''
+        raise AttributeError("No query has been done yet, fms_version is unknown.")
 
-    def do_find_query(self, query_dict, skip=None, max=None, sort=[], paginate=None):
+    def do_find_query(
+        self,
+        query_dict,
+        skip: int = 0,
+        max: int = 0,
+        sort: Iterable = [],
+        paginate: int = 0
+    ) -> FmRecordStream:
         """
         Allows to do more complex queries than do_find.
 
         Operators in the Django like syntax like size__gt=22 are not possible
         in this mode but one can still use FM operators using e.g. 'size'='>22'
 
         # search for blue color houses:
@@ -336,15 +358,24 @@
         query.add_args('-query', ";".join(i for i in query_list))
         for k, v in query_values:
             query.add_param(k, v, parse_operator=False)
 
         stream = self._do_request(query, paginate=paginate)
         return stream
 
-    def do_find(self, what={}, sort=[], skip=None, max=None, lop='AND', paginate=None, **kwargs):
+    def do_find(
+        self,
+        what={},
+        sort=[],
+        skip: int = 0,
+        max: int = 0,
+        lop: str = 'AND',
+        paginate: int = 0,
+        **kwargs
+    ) -> FmRecordStream:
         """Performs a find query on the FM server
 
         search criterions can be specified through the :what: parameters or
         through the kwargs arguments. The two forms can be combined. The
         :kwargs: forms as precedence.
 
         # e.g.
@@ -403,31 +434,31 @@
         for key, value in what.items():
             query.add_param(key, value)
         for key, value in kwargs.items():
             query.add_param(key, value)
         stream = self._do_request(query, paginate=paginate)
         return stream
 
-    def do_find_all(self, sort=[], skip=None, max=None, paginate=None):
+    def do_find_all(self, sort=[], skip: int = 0, max: int = 0, paginate: int = 0) -> FmRecordStream:
         """Finds all records in the layout."""
         query = FmQuery(action='-findall', fm_server=self)
         query.pre_find(sort=sort, skip=skip, max=max)
         stream = self._do_request(query, paginate=paginate)
         return stream
 
-    def do_find_any(self, what={}, sort=[], lop='AND', **params):
+    def do_find_any(self, sort=[]):
         """Finds all records in the layout."""
         query = FmQuery(action='-findany', fm_server=self)
-        query.pre_find(sort=sort, lop=lop)
+        query.pre_find(sort=sort)
         stream = tuple(self._do_request(query))
         if stream and len(stream) > 0:
             return stream[0]
         return []
 
-    def do_delete(self, what, error_if_missing=True):
+    def do_delete(self, what: MutableDict, error_if_missing: bool = True):
         """
         Deletes the record identified by the rec-id attribute of the xml
         E.g.
         # if one knows the rec-id attribute:
         fm = FmServer(...)
         fm.do_delete(what=34)
 
@@ -452,19 +483,21 @@
             tuple(self._do_request(query))
         except FmError as e:
             if e.code == 101:
                 if not error_if_missing:
                     return None
             raise FmError from e
 
-    def do_edit(self, what=None, **kwargs):
+    def do_edit(self, what: Optional[Union[MutableDict, dict]] = None, **kwargs) -> None:
         """
-        Edits a record.
-        Trick to editate multi value fields:
+        Edits a record. If what is a classical dict, it must contains the
+        record_id field (an internal value of fms) or the record_id must be
+        passed in the kwargs.
 
+        Trick to editate multi value fields:
         fm.do_edit(what={'record_id':rec.record_id, 'dataC(3)':'bijour'})
 
         """
         query = FmQuery(action='-edit', fm_server=self)
         self._parse_what_and_kwargs(
             what=what,
             kwargs=kwargs,
@@ -537,26 +570,45 @@
             query.add_args(name='-recid', value=kwargs.pop('record_id'))
             if 'mod_id' in kwargs:
                 query.add_args(name='-modid', value=kwargs.pop('mod_id'))
 
         for key, value in kwargs.items():
             query.add_param(name=key, value=value)
 
-    def _build_url(self):
+    def _build_url(self) -> str:
         tmpl = "{scheme}://{hostname}:{port}{path}"
         return tmpl.format(**self.url)
 
-    def _build_file_url(self, xml_req):
+    def _build_file_url(self, xml_req) -> str:
         """Builds url for fetching the files from FM."""
         return '{scheme}://{hostname}:{port}{xml_req}'.format(
             xml_req=xml_req,
             **self.url
         )
 
-    def _do_request(self, query, is_file=False, paginate=None):
+    @overload
+    def _do_request(
+        self,
+        query: 'FmQuery',
+        is_file: Literal[True],
+        paginate: int = 0) -> bytes: ...
+
+    @overload
+    def _do_request(
+        self,
+        query: 'FmQuery',
+        is_file: Literal[False] = False,
+        paginate: int = 0) -> FmRecordStream: ...
+
+    def _do_request(
+        self,
+        query: 'FmQuery',
+        is_file: bool = False,
+        paginate: int = 0,
+    ) -> Union[bytes, FmRecordStream]:
         if is_file:
             url = self._build_file_url(xml_req=query)
         else:
             url = self._build_url()
             url = url + '?' + query.format()
 
         if paginate and not is_file:
@@ -574,18 +626,18 @@
                 return _paginate(
                     fm_server=self,
                     query=query,
                     page_size=paginate
                 )
 
         if self.debug:
-            log.info("FmServer({})".format(url))
+            log.info(f"FmServer({url})")
             if not is_file:
                 for item in query.request:
-                    log.info("  {}".format(item))
+                    log.info(f"  {item}")
 
         resp = requests.get(
             url=url,
             auth=(self.url.get('username', ''), self.url.get('password', '')),
             **self.options['request_kwargs']
         )
         # does this breaks streamed response ?
@@ -605,21 +657,21 @@
         # parse returns a generator, so no try catch can be done here.
         return parse(
             stream=resp.raw,
             fm_meta=self.fm_meta,
         )
 
 
-class FmQuery():
+class FmQuery:
     """This class is internal to FmServer. It is used to define the arguements
     that can or must be passed with a given action and it formats and casts
     theses arguments before building a request url."""
     _scripts = [
-        '-script', '–script.param', '-script.prefind', '-script.prefind.param',
-        '-script.presort', '–script.presort.param'
+        '-script', '-script.param', '-script.prefind', '-script.prefind.param',
+        '-script.presort', '-script.presort.param'
     ]
     _layr = ['-lay.response']
     _finds = ['-recid', '-lop', '-op', '-max',
               '-skip', '-sortorder', '-sortfield']
 
     actions = {
         '-dbnames': {
@@ -699,46 +751,55 @@
         'does_not_contains': 'neq',
         'gt': 'gt',
         'gte': 'gte',
         'lt': 'lt',
         'lte': 'lte',
     }
 
-    def __init__(self, action=None, fm_server=None):
+    def __init__(self, action: str, fm_server: FmServer):
         if action not in self.__class__.actions:
-            raise FmError("Invalid action name ({})".format(action))
+            raise FmError(f"Invalid action name '{action}'.")
         self.fm_server = fm_server
         self.action = action
         self.grammar = self.__class__.actions[self.action]
-        self.args = {
+        self.args: dict[str, Union[str, int]] = {
             '-db': self.fm_server.db,
             '-lay': self.fm_server.layout,
         }
         self._params = []
         self.back_cast = None
 
-    def set_max(self, value):
+    def set_max(self, value: int):
         try:
             _max = int(value)
         except ValueError:
-            raise FmError("Max value must be a number (got {})".format(value))
+            raise FmError(f"Max value must be a number (got {value})")
         if _max < 0:
-            raise FmError("Max value must be positive (got {})".format(_max))
+            raise FmError(f"Max value must be positive (got {_max})")
         self.args['-max'] = _max
 
-    def set_skip(self, value):
+    def set_skip(self, value: int):
         try:
             _skip = int(value)
         except ValueError:
-            raise FmError("Skip value must be a number (got {})".format(value))
+            raise FmError(f"Skip value must be a number (got {value})")
         if _skip < 0:
-            raise FmError("Skip value must be positive (got {})".format(_skip))
+            raise FmError(f"Skip value must be positive (got {_skip})")
         self.args['-skip'] = _skip
 
-    def add_sort_params(self, sort):
+    def add_sort_params(self, sort: Iterable[Union[str, tuple[str, str]]]):
+        """
+        Add a sorting criterion to the query.
+
+        E.g. 
+        sort = ['fieldA', '-fieldB', ...]
+        or sort = [('fieldA','ascend'), ('fieldB', 'descend'), 'fieldC', ...]
+
+        syntaxes -field ('field','ascend'), ('field', '<') are all equivalent.
+        """
         for i, item in enumerate(sort):
             if isinstance(item, str):
                 field = item
                 sort_order = 'ascend'
                 if field[0] == '-':
                     field = field[1:]
                     sort_order = 'descend'
@@ -749,34 +810,37 @@
                 sort_order = 'ascend'
             elif sort_order == '>':
                 sort_order = 'descend'
             self._params.append(('-sortfield.{}'.format(i+1), field))
             if sort_order:
                 self._params.append(('-sortorder.{}'.format(i+1), sort_order))
 
-    def pre_find(self, sort=[], skip=None, max=None, lop='AND'):
-        """This function will process attributtes for all -find* commands."""
+    def pre_find(self, sort=[], skip: int = 0, max: int = 0, lop: str = 'AND'):
+        """Process attributtes for all -find* commands."""
         self.add_sort_params(sort)
         if skip:
             self.set_skip(skip)
         if max:
             self.set_max(max)
         if lop:
             if lop.lower() not in ['and', 'or']:
                 raise FmError(
-                    'Unsupported logical operator '
-                    '(not one of "and" or "or").'
+                    f"Logical operator must be 'and' or 'or'. Got '{lop}'."
                 )
             self.args['-lop'] = lop.lower()
 
-    def add_args(self, name, value):
+    def add_args(self, name: str, value):
+        """Add a keyword for the futur query
+
+        :value: must be encodable for an url. So basically int or str.
+        """
         self.args[name] = value
 
-    def add_param(self, name, value, parse_operator=True):
-        """Adds a database parameter"""
+    def add_param(self, name: str, value, parse_operator: bool = True):
+        """Add a keyword/value for the futur query"""
 
         # finding the table and operator parts if any
         parts = name.split('__')
         op = None
         if (
             parse_operator and
             len(parts) > 1 and
@@ -791,33 +855,27 @@
         if not self.back_cast:
             bc = self.fm_server.options['back_cast_class']
             self.back_cast = bc(fm_server=self.fm_server)
         casted_value = self.back_cast(field=field, value=value)
 
         self._params.append((field, casted_value))
         if op:
-            self._params.append(("{}.op".format(field), op))
-
-    def is_allowed(self, name):
-        self.grammar = self.__class__.actions[self.action]
-        if name in self.grammar.required or name in self.grammar.optional:
-            return True
-        return False
+            self._params.append((f"{field}.op", op))
 
-    def format(self):
+    def format(self) -> str:
+        """Builds the query as url string"""
         if not self.action:
             raise FmError("Empty action name")
         request = []
         args = copy.copy(self.args)
         params = copy.copy(self._params)
         for key in self.grammar['required']:
             if key not in args:
                 raise ValueError(
-                    "A required argument ({}) is not present for action {}"
-                    .format(key, self.action)
+                    f"A required argument ({key}) is not present for action {self.action}"
                 )
 
             value = args.pop(key)
             if not value:
                 raise ValueError(
                     f"A required argument ({key}) is empty ({value})"
                 )
@@ -833,24 +891,24 @@
 
         request.append((self.action, ''))
         self.request = request
 
         return urlencode(request, doseq=False)
 
 
-def _paginate(fm_server, query, page_size, current=0):
+def _paginate(fm_server: FmServer, query: FmQuery, page_size: int, current: int = 0) -> FmRecordStream:
     fm_server_copy = copy.copy(fm_server)
     query = copy.copy(query)
 
     query.set_skip(current)
     query.set_max(page_size)
     for item in fm_server_copy._do_request(
         query,
         is_file=False,
-        paginate=None
+        paginate=0
     ):
         fm_server.fm_meta = fm_server_copy.fm_meta
         yield item
 
     N = fm_server_copy.fetched_records_number()
     if N < page_size:
         return
@@ -862,15 +920,15 @@
         query,
         page_size,
         current=current+page_size
     ):
         yield item
 
 
-def _threaded_paginate(fm_server, query, page_size):
+def _threaded_paginate(fm_server: FmServer, query: FmQuery, page_size: int) -> FmRecordStream:
     """
     Instead of 'classic' pagination, we launch a thread that only fetchs the
     data and fills a queue.Queue objects. The main loop consumes the queue and
     looks like an iterator over the returned item.
 
     The advantage comes when processing the objects retrieved from FMS takes
     some IO time (like storing them in a DB.). In this case, the fetching can
@@ -878,30 +936,30 @@
     worse than the classical one.
 
     Note that the queries fetching the FMS objects are still done one after the
     other as it is launched by the same thread. The FIFO queue ensures the
     processing order is preserved.
     """
 
-    def _data_fetcher(fm_server, query, page_size, current, share_mem):
+    def _data_fetcher(fm_server: FmServer, query: FmQuery, page_size: int, current, share_mem):
         """"
         Procuces a recursive call to do_request for the next :page_size: object
         and always fills the result into share_mem['data'] then notifies the
         waiting threads.
         """
         # simply copy the fm_server objects and query.
         fm_server_copy = copy.copy(fm_server)
         query = copy.copy(query)
         query.set_skip(current)
         query.set_max(page_size)
         try:
             for item in fm_server_copy._do_request(
                 query,
                 is_file=False,
-                paginate=None
+                paginate=0
             ):
                 fm_server.fm_meta = fm_server_copy.fm_meta
                 # push data into queue.Queue object
                 share_mem['data'].put(item)
         except requests.ConnectionError:
             share_mem['end-of-job'] = True
             log.info("Failed to establish a connection.")
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/tests/test_caster.py` & `pyfilemaker2-0.2.6/pyfilemaker2/tests/test_caster.py`

 * *Files identical despite different names*

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/tests/test_data.py` & `pyfilemaker2-0.2.6/pyfilemaker2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/tests/test_metadata.py` & `pyfilemaker2-0.2.6/pyfilemaker2/tests/test_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf8 -*-
 import unittest
 import datetime
-import pytz
+from zoneinfo import ZoneInfo
 
 from pyfilemaker2.metadata import FmMeta
 from pyfilemaker2.parser import parse
 from pyfilemaker2.caster import (
     TextCast,
     NumberCast,
     DateCast,
@@ -45,19 +45,19 @@
             'f_calculation_text': TextCast,
             'f_calculation_number': NumberCast,
             'f_multi_text': TextCast,
             'f_multi_number': NumberCast,
         }
 
         for k, v in map.items():
-            f = b.get_fm_field(raw_name=k, table=None)
+            f = b.get_fm_field(raw_name=k, related_table='')
             self.assertEqual(f.caster.__class__, v)
 
     def test_data1(self):
-        # https://{user}:{pswd}@{host}/fmi/xml/fmresultset.xml?-db=TestJeremie&-lay=test_table1&-findall
+        # https://{user}:{pswd}@{host}/fmi/xml/fmresultset.xml?-db=TestFile&-lay=test_table1&-findall
         f1 = os.path.join(basedir, './fields_types.xml')
         nodeiter = parse(stream=f1)
         data = [p for p in nodeiter]
         out = {
             'f_text': 'pure ascii text',
             'f_number': 0.123,
             'f_time': datetime.time(hour=11, minute=53, second=56),
@@ -73,34 +73,34 @@
         }
 
         for k, v in out.items():
             self.assertEqual(data[0][k], out[k])
 
     def test_data_tz(self):
         f1 = os.path.join(basedir, './fields_types.xml')
-        tz = pytz.timezone('Europe/Zurich')
+        tz = ZoneInfo('Europe/Zurich')
         d = datetime.datetime(
             year=2018,
             month=9,
             day=1,
             hour=11,
             minute=54,
-            second=7
+            second=7,
+            tzinfo=tz,
         )
-        d = tz.normalize(tz.localize(d))
 
         fm = FmMeta(server_timezone=tz)
         nodeiter = parse(stream=f1, fm_meta=fm)
         data = [p for p in nodeiter]
         val = data[0]['f_timestamp']
 
         self.assertEqual(d, val)
 
     def test_non_ascii_chars(self):
-        # https://{user}:{pswd}@{host}/fmi/xml/fmresultset.xml?-db=TestJeremie&-lay=test_awfull_table&-findall
+        # https://{user}:{pswd}@{host}/fmi/xml/fmresultset.xml?-db=TestFile&-lay=test_awfull_table&-findall
         f1 = os.path.join(basedir, './non_ascii_chars.xml')
         nodeiter = parse(stream=f1)
         data = [p for p in nodeiter]
         out = {
             'field1': """éà¢ß
 non-secable dash: –
 non-secable space: ' '
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2/tests/test_server.py` & `pyfilemaker2-0.2.6/pyfilemaker2/tests/test_server.py`

 * *Files 15% similar despite different names*

```diff
@@ -86,14 +86,25 @@
         fm = FmServer(db='test')
         lst = fm.get_script_names()
         self.assertEqual(set(lst), set([
             'generate_dummy_data',
             'étoile mâtinée',
         ]))
 
+    @mock.patch.object(requests, 'get')
+    def test_relatedset(self, mock_get):
+        mock_get.return_value = Dummy('./ressources/related_set.xml')
+        fm = FmServer(db='test', layout='dummy')
+        record = list(fm.do_find(idb=3))[0]
+        self.assertEqual(
+            record,
+            {"idb": "3", "link2C": "2", "tableC": "elem de B", "tableA": [{"tableA": {"link2B": "3", "data": "abc", "tableC": {
+                "dataC": ["Un texte"]}}}, {"tableA": {"link2B": "3", "data": "def", "tableC": {"dataC": [""]}}}]}
+        )
+
 
 class TestServerOnline(unittest.TestCase):
     def test_find_equal(self):
         fm = get_fm_server()
         fm.layout = 'test_table_query'
         resultset = fm.do_find(id=1)
         r = tuple(resultset)
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2.egg-info/PKG-INFO` & `pyfilemaker2-0.2.6/pyfilemaker2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfilemaker2
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python Object Wrapper for FileMaker Server XML Interface
 Home-page: https://github.com/jeremie-borel/pyfilemaker2/
 Author: Klokan Petr Pridal, Pieter Claerhout, Marcin Kawa, Jeremie Borel
 Author-email: klokan@klokan.cz, pieter@yellowduck.be, kawa.macin@gmail.com
 License: http://www.opensource.org/licenses/bsd-license.php
 Download-URL: https://github.com/jeremie-borel/pyfilemaker2/
 Keywords: FileMaker
@@ -107,15 +107,15 @@
 extensive docstring. Starts in particular with the server.py file. Moreover an
 FmServer object is likely the unique thing one will need to import from this
 package.
 
 ### 5. CHANGES
 
 0.2.5:
-- server_timezone parameter now requires a zoneinfo.ZoneInfo object or None.
+- BACKWARD INCOMPATIBLE: server_timezone parameter now requires a zoneinfo.ZoneInfo object or None. Timezones from pytz are not supported anymore. To use another package (e.g. pytz), one can overload the BackCast class from caster and define it as the :back_cast_class: static member of FmInstance.
 
 0.2.4:
 - Fix https://github.com/jeremie-borel/pyfilemaker2/issues/1 that prevented FMS 19 to work.
 
 0.2.3:
 -
```

### Comparing `pyfilemaker2-0.2.5/pyfilemaker2.egg-info/SOURCES.txt` & `pyfilemaker2-0.2.6/pyfilemaker2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfilemaker2-0.2.5/setup.py` & `pyfilemaker2-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name='pyfilemaker2',
-    version="0.2.5",
+    version="0.2.6",
     description='Python Object Wrapper for FileMaker Server XML Interface',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         'Environment :: Console',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
```

