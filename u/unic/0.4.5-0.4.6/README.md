# Comparing `tmp/unic-0.4.5.tar.gz` & `tmp/unic-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unic-0.4.5.tar", max compression
+gzip compressed data, was "unic-0.4.6.tar", max compression
```

## Comparing `unic-0.4.5.tar` & `unic-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.5/LICENSE
--rw-r--r--   0        0        0      888 2024-05-12 14:10:18.293002 unic-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-0.4.5/README.md
--rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.5/unic/__init__.py
--rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.5/unic/configs/metirc_system/settings.toml
--rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.5/unic/configs/timeunit/settings.toml
--rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.5/unic/configs/timezone/settings.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.5/unic/length_unit/metric_system/__init__.py
--rw-r--r--   0        0        0      683 2024-05-10 14:37:46.429999 unic-0.4.5/unic/length_unit/metric_system/metric_system_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.5/unic/length_unit/validators/__init__.py
--rw-r--r--   0        0        0     1279 2024-05-10 14:36:03.640060 unic-0.4.5/unic/length_unit/validators/validators.py
--rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.5/unic/time_unit/datetime/__init__.py
--rw-r--r--   0        0        0     1301 2024-05-10 14:38:56.907969 unic-0.4.5/unic/time_unit/datetime/datetime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.5/unic/time_unit/time/__init__.py
--rw-r--r--   0        0        0      660 2024-05-10 14:34:06.458160 unic-0.4.5/unic/time_unit/time/time_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.5/unic/time_unit/unixtime/__init__.py
--rw-r--r--   0        0        0     1005 2024-05-10 14:34:11.031532 unic-0.4.5/unic/time_unit/unixtime/unixtime_model.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.5/unic/time_unit/validators/__init__.py
--rw-r--r--   0        0        0     2557 2024-05-10 14:33:34.102958 unic-0.4.5/unic/time_unit/validators/validators.py
--rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.5/unic/utils/__init__.py
--rw-r--r--   0        0        0      391 2023-10-29 05:14:04.780174 unic-0.4.5/unic/utils/config_parser.py
--rw-r--r--   0        0        0     3097 1970-01-01 00:00:00.000000 unic-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-08-02 13:34:57.957684 unic-0.4.6/LICENSE
+-rw-r--r--   0        0        0      888 2024-05-17 15:00:39.830539 unic-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2398 2024-05-03 12:41:18.395441 unic-0.4.6/README.md
+-rw-r--r--   0        0        0      897 2023-12-11 12:31:51.919297 unic-0.4.6/unic/__init__.py
+-rw-r--r--   0        0        0      912 2023-12-11 13:01:08.512829 unic-0.4.6/unic/configs/metirc_system/settings.toml
+-rw-r--r--   0        0        0      244 2023-08-02 13:34:57.987478 unic-0.4.6/unic/configs/timeunit/settings.toml
+-rw-r--r--   0        0        0     2232 2023-08-02 13:34:57.987478 unic-0.4.6/unic/configs/timezone/settings.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.6/unic/length_unit/metric_system/__init__.py
+-rw-r--r--   0        0        0      751 2024-05-16 14:57:00.498671 unic-0.4.6/unic/length_unit/metric_system/metric_system_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.6/unic/length_unit/validators/__init__.py
+-rw-r--r--   0        0        0     1279 2024-05-10 14:36:03.640060 unic-0.4.6/unic/length_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-08 15:37:47.030079 unic-0.4.6/unic/time_unit/datetime/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-16 14:49:57.983327 unic-0.4.6/unic/time_unit/datetime/datetime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:57.999736 unic-0.4.6/unic/time_unit/time/__init__.py
+-rw-r--r--   0        0        0      728 2024-05-16 14:56:54.023059 unic-0.4.6/unic/time_unit/time/time_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.002017 unic-0.4.6/unic/time_unit/unixtime/__init__.py
+-rw-r--r--   0        0        0     1094 2024-05-16 14:56:45.186999 unic-0.4.6/unic/time_unit/unixtime/unixtime_model.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.6/unic/time_unit/validators/__init__.py
+-rw-r--r--   0        0        0     2557 2024-05-10 14:33:34.102958 unic-0.4.6/unic/time_unit/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:34:58.004259 unic-0.4.6/unic/utils/__init__.py
+-rw-r--r--   0        0        0      399 2024-05-14 16:00:12.297440 unic-0.4.6/unic/utils/config_parser.py
+-rw-r--r--   0        0        0     3096 1970-01-01 00:00:00.000000 unic-0.4.6/PKG-INFO
```

### Comparing `unic-0.4.5/LICENSE` & `unic-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unic-0.4.5/pyproject.toml` & `unic-0.4.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unic"
-version = "0.4.5"
+version = "0.4.6"
 description = "Python package for converting various units."
 authors = ["Subretu"]
 maintainers = ["Subretu"]
 license = "MIT"
 readme = 'README.md'
 repository = 'https://github.com/subretu/unic'
 keywords = ['unit', 'convert', 'time', 'timestamp', 'length']
@@ -17,16 +17,16 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-toml = "^0.10.2"
 pydantic = "^2.1"
+tomli = "^2.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 mypy = "^1.4.1"
 black = "^23.7.0"
 
 [build-system]
```

### Comparing `unic-0.4.5/README.md` & `unic-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `unic-0.4.5/unic/__init__.py` & `unic-0.4.6/unic/__init__.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.5/unic/configs/metirc_system/settings.toml` & `unic-0.4.6/unic/configs/metirc_system/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.5/unic/configs/timezone/settings.toml` & `unic-0.4.6/unic/configs/timezone/settings.toml`

 * *Files identical despite different names*

### Comparing `unic-0.4.5/unic/length_unit/metric_system/metric_system_model.py` & `unic-0.4.6/unic/time_unit/time/time_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from pydantic import ValidationError
 from unic.utils import config_parser
-from unic.length_unit.validators import validators
+from unic.time_unit.validators import validators
 from fractions import Fraction
 
 
-class MetricSystemModel:
+class TimeModel:
     def convert(self, data: int, *, from_unit: str, to_unit: str) -> int:
         try:
-            input_data = validators.MetricSystemModelValidator(
+            input_data = validators.TimeModelValidator(
                 data=data, from_unit=from_unit, to_unit=to_unit
             )
         except ValidationError as e:
-            raise ValueError(e.errors()[0]["msg"])
+            error_messages = "; ".join(err["msg"] for err in e.errors())
+            raise ValueError(error_messages)
 
-        parameter = config_parser.parse_toml("metirc_system")
+        parameter = config_parser.parse_toml("timeunit")
         data = float(input_data.data * Fraction(parameter[from_unit][to_unit]))
 
         return data
```

### Comparing `unic-0.4.5/unic/length_unit/validators/validators.py` & `unic-0.4.6/unic/length_unit/validators/validators.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.5/unic/time_unit/datetime/datetime_model.py` & `unic-0.4.6/unic/time_unit/datetime/datetime_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from pydantic import ValidationError
 from datetime import date, datetime, timezone, timedelta
 from unic.utils import config_parser
 from unic.time_unit.validators import validators
 from typing import Union
-import math
 
 
 class DatetimeModel:
+    def __init__(self):
+        self.timezone_parameters = config_parser.parse_toml("timezone")
+
     def convert(self, data: int, format: str, tz: str = None) -> Union[date, datetime]:
         try:
             input_data = validators.DatetimeModelValidator(
                 data=data, format=format, tz=tz
             )
         except ValidationError as e:
-            raise ValueError(e.errors()[0]["msg"])
+            error_messages = "; ".join(err["msg"] for err in e.errors())
+            raise ValueError(error_messages)
 
-        timezone_hour = 0
-        if tz:
-            parameter = config_parser.parse_toml("timezone")
-            timezone_hour = parameter[tz]["value"]
+        timezone_hour = self.timezone_parameters.get(tz, {}).get("value", 0)
 
         converted_data = self.convert_timestamp_by_digits(
             input_data.data, timezone_hour, format
         )
 
         return converted_data
```

### Comparing `unic-0.4.5/unic/time_unit/validators/validators.py` & `unic-0.4.6/unic/time_unit/validators/validators.py`

 * *Files identical despite different names*

### Comparing `unic-0.4.5/PKG-INFO` & `unic-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unic
-Version: 0.4.5
+Version: 0.4.6
 Summary: Python package for converting various units.
 Home-page: https://github.com/subretu/unic
 License: MIT
 Keywords: unit,convert,time,timestamp,length
 Author: Subretu
 Maintainer: Subretu
 Requires-Python: >=3.8,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=2.1,<3.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/subretu/unic
 Description-Content-Type: text/markdown
 
 ![Python minimum version](https://img.shields.io/badge/Python-3.8%2B-brightgreen)
 [![pytest](https://github.com/subretu/unic/actions/workflows/pytest.yml/badge.svg)](https://github.com/subretu/unic/actions/workflows/pytest.yml)
 [![black](https://github.com/subretu/unic/actions/workflows/format.yml/badge.svg)](https://github.com/subretu/unic/actions/workflows/format.yml)
```

