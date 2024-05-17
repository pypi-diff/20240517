# Comparing `tmp/ph-utils-0.0.7.tar.gz` & `tmp/ph_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ph-utils-0.0.7.tar", last modified: Mon Sep 25 10:23:58 2023, max compression
+gzip compressed data, was "ph_utils-0.0.8.tar", last modified: Fri May 17 09:35:39 2024, max compression
```

## Comparing `ph-utils-0.0.7.tar` & `ph_utils-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-09-25 10:23:58.873402 ph-utils-0.0.7/
--rw-rw-rw-   0        0        0     9592 2023-08-15 04:05:27.000000 ph-utils-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     5528 2023-09-25 10:23:58.873402 ph-utils-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     4764 2023-08-21 11:36:53.000000 ph-utils-0.0.7/README.md
--rw-rw-rw-   0        0        0      717 2023-09-25 10:23:44.000000 ph-utils-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-09-25 10:23:58.874402 ph-utils-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-25 10:23:58.858401 ph-utils-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-09-25 10:23:58.861401 ph-utils-0.0.7/src/ph_utils/
--rw-rw-rw-   0        0        0      505 2023-08-15 04:07:11.000000 ph-utils-0.0.7/src/ph_utils/__init__.py
--rw-rw-rw-   0        0        0     5548 2023-09-25 10:23:35.000000 ph-utils-0.0.7/src/ph_utils/common.py
--rw-rw-rw-   0        0        0     3403 2023-08-21 07:05:15.000000 ph-utils-0.0.7/src/ph_utils/config.py
--rw-rw-rw-   0        0        0     2348 2023-08-22 11:16:09.000000 ph-utils-0.0.7/src/ph_utils/crypto.py
--rw-rw-rw-   0        0        0     8067 2023-09-25 10:17:17.000000 ph-utils-0.0.7/src/ph_utils/date.py
--rw-rw-rw-   0        0        0     8851 2023-09-07 11:03:33.000000 ph-utils-0.0.7/src/ph_utils/logger.py
-drwxrwxrwx   0        0        0        0 2023-09-25 10:23:58.872402 ph-utils-0.0.7/src/ph_utils.egg-info/
--rw-rw-rw-   0        0        0     5528 2023-09-25 10:23:58.000000 ph-utils-0.0.7/src/ph_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-09-25 10:23:58.000000 ph-utils-0.0.7/src/ph_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-25 10:23:58.000000 ph-utils-0.0.7/src/ph_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-09-25 10:23:58.000000 ph-utils-0.0.7/src/ph_utils.egg-info/top_level.txt
+-rw-r--r--   0        0        0     9592 2024-05-17 08:54:46.495620 ph_utils-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4764 2024-05-17 08:54:46.495620 ph_utils-0.0.8/README.md
+-rw-r--r--   0        0        0      804 2024-05-17 09:35:39.755991 ph_utils-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      505 2024-05-17 08:54:46.496617 ph_utils-0.0.8/src/ph_utils/__init__.py
+-rw-r--r--   0        0        0     5351 2024-05-17 08:59:28.753822 ph_utils-0.0.8/src/ph_utils/common.py
+-rw-r--r--   0        0        0     3403 2024-05-17 08:54:46.496617 ph_utils-0.0.8/src/ph_utils/config.py
+-rw-r--r--   0        0        0     2348 2024-05-17 08:54:46.496617 ph_utils-0.0.8/src/ph_utils/crypto.py
+-rw-r--r--   0        0        0     8067 2024-05-17 08:54:46.497614 ph_utils-0.0.8/src/ph_utils/date.py
+-rw-r--r--   0        0        0     8851 2024-05-17 08:54:46.497614 ph_utils-0.0.8/src/ph_utils/logger.py
+-rw-r--r--   0        0        0      293 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      713 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/common_utils.py
+-rw-r--r--   0        0        0      193 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/config_utils.py
+-rw-r--r--   0        0        0      201 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/crypto_utils.py
+-rw-r--r--   0        0        0      501 2024-05-17 08:54:46.498612 ph_utils-0.0.8/tests/date_utils.py
+-rw-r--r--   0        0        0      280 2024-05-17 08:54:46.499609 ph_utils-0.0.8/tests/logger_utils.py
+-rw-r--r--   0        0        0     5304 1970-01-01 00:00:00.000000 ph_utils-0.0.8/PKG-INFO
```

### Comparing `ph-utils-0.0.7/LICENSE` & `ph_utils-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ph-utils-0.0.7/PKG-INFO` & `ph_utils-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,202 +1,201 @@
-Metadata-Version: 2.1
-Name: ph-utils
-Version: 0.0.7
-Summary: The python3 tool classes
-Author-email: Tenny <tenny.shu@foxmail.com>
-License: MulanPSL-2.0
-Project-URL: Homepage, https://gitee.com/towardly/ph-utils_py
-Project-URL: Bug Tracker, https://gitee.com/towardly/ph-utils_py/issues
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ph-utils
-
-## Install
-
-```shell
-pip install ph-utils
-```
-
-The python3 tool classes. Includes the following modules:
-
-1. `config_utils`: Configure relevant tool classes, `load_env`
-2. `date_utils`: The date processing tool, `parse`、`format`、`set`、`start_of`、`end_of`、`add`、`sub`、`diff`、`timestamp`
-
-## 1. `config_utils`
-
-Configure relevant tool classes.
-
-### Usage
-
-```python
-from ph_utils.config_utils import load_env
-```
-
-### `1. load_env(file_dir, env_files): dict`:
-
-Load the environment variable file, the content behind the list will replace the content in front. `file_dir` - The environment variable file folder, default: `os.cwd()`; `env_files` - The environment variable file list, if `None` or empty list load `['.env', '.env.local', '.env.development', '.env.production']`
-
-### `2. load_json(file_dir, json_files): dict`:
-
-Load json file. default: `['config.json']`
-
-### `3. load_ini(file_dir, ini_files): dict`:
-
-Load `ini` file. default: `[config.ini]`
-
-## 2. `date-utils`
-
-The date processing tool.
-
-### Usage
-
-```python
-import ph_utils.date_utils as date_utils
-from ph_utils.date_utils import parse, format
-```
-
-### `1. parse(date_data: Any, fmt=None): datetime`
-
-You can parse various data formats into date objects, including time stamps, strings, and date objects themselves. Return `datetime` object.
-
-1. parse timestamp
-
-```python
-date_utils.parse(1691997308) # 2023-08-14 15:15:08
-```
-
-2. parse strings
-
-```python
-date_utils.parse('2023-08-14 15:23:23') # 2023-08-14 15:23:23
-date_utils.parse('20230814 152323') # 2023-08-14 15:23:23
-date_utils.parse('2023/08/14 15:23:23', '%Y/%m/%d %H:%M:%S') # 2023-08-14 15:23:23
-```
-
-3. parse `None` object
-
-```python
-date_utils.parse() # 2023-08-14 15:15:23.830691
-date_utils.parse(None) # 2023-08-14 15:15:23.830691
-```
-
-4. parse `datetime`
-
-```python
-date_utils.parse(date_utils.parse()) # 2023-08-14 15:19:48.382871
-```
-
-### `2. format(ori_date, pattern): str`
-
-Date formatting is the process of converting a date to a specific format.
-
-Parameter description:
-
-1. `ori_date`: **optional** All parameters that can be supported by the `parse` function.
-2. `pattern`: **optional** `default: %Y-%m-%d`, eg: `%Y-%m-%d %H:%M:%S`
-
-```python
-date_utils.format(None, '%Y-%m-%d %H:%M:%S')
-date_utils.format(1691997308, '%Y-%m-%d %H:%M:%S')
-```
-
-### `3. start_of(ori_date, unit, __format): datetime | int`
-
-Set the start of a time at a certain moment.
-
-Paramater description:
-
-1. `unit`: **optional** `default: date`, `date` - start time of a day
-2. `__format`: **optional** `default: None`, set the returned data, `None` - return `datetime`, `s`、`ms` return timestamp
-
-```python
-start_of() # datetime - 2023-08-15 00:00:00
-start_of(__format='s') # int - 1692028800
-```
-
-### `4. end_of(ori_date, unit, __format): datetime | int`
-
-Set the end of a time at a certain moment.
-
-```python
-end_of() # datetime - 2023-08-15 23:59:59
-```
-
-### `5. timestamp(ori_date, unit): int`
-
-Get timestamp of a time
-
-1. `unit`: `s` - _default_ length: 10，accurate to second、 `ms` length: 13, accurate to milliseconds.
-
-```python
-timestamp()
-```
-
-### `6. set(ori_date, values): datetime`
-
-Set date values to a given date.
-
-Sets time values to date from object . A value is not set if it is undefined or null or doesn't exist in values.
-
-`values`: `str | dict`，the given date. If is `dict`, include the follow property. `year`、`month`、`day`、`hour`、`minute`、`second`
-
-```python
-set(None, '2023-08-15 14:49:49')
-set(None, '2023/08/15 14:49:49')
-set(None, '20230815 144949')
-set(None, '20230815')
-set(None, '144949')
-set(None, { 'year': 2023, 'month': 8, 'day': 15, 'hour': 14, 'minute': 49, 'second': 49 })
-set(None, { 'year': 2023, 'month': 8, 'day': 15 })
-set(None, { 'hour': 14, 'minute': 49, 'second': 49 })
-```
-
-### `7. add(ori_date, duration): datetime`
-
-Add the specified years, months, weeks, days, hours, minutes and seconds to the given date.
-
-`duration` the object with years, months, weeks, days, hours, minutes and seconds to be added.
-
-```python
-add(duration={
-  'years': 2,
-  'months': 9,
-  'days': 7,
-  'hours': 5,
-  'minutes': 9,
-  'seconds': 30,
-})
-```
-
-### `8. subtract(ori_date, duration): datetime`
-
-Subtract the specified years, months, weeks, days, hours, minutes and seconds from the given date.
-
-```python
-subtract(duration={
-  'years': 2,
-  'months': 9,
-  'days': 7,
-  'hours': 5,
-  'minutes': 9,
-  'seconds': 30,
-})
-```
-
-### `9. sub(ori_date, duration): datetime`
-
-Alias of `subtract`.
-
-### `10: diff(start, end, result): int | timedelta`
-
-Get the number of full day periods between two dates.
-
-`result`: set the returned data. if `result = days` - return `int`, difference in days; otherwise return `timedelta`. default: `days`
-
-```python
-diff(parse(), parse()) # => 0
-```
+Metadata-Version: 2.1
+Name: ph-utils
+Version: 0.0.8
+Summary: The python3 tool classes
+Author-Email: Tenny <tenny.shu@foxmail.com>
+License: MulanPSL-2.0
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
+Classifier: Operating System :: OS Independent
+Project-URL: Homepage, https://gitee.com/towardly/ph-utils_py
+Project-URL: Bug tracker, https://gitee.com/towardly/ph-utils_py/issues
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+
+# ph-utils
+
+## Install
+
+```shell
+pip install ph-utils
+```
+
+The python3 tool classes. Includes the following modules:
+
+1. `config_utils`: Configure relevant tool classes, `load_env`
+2. `date_utils`: The date processing tool, `parse`、`format`、`set`、`start_of`、`end_of`、`add`、`sub`、`diff`、`timestamp`
+
+## 1. `config_utils`
+
+Configure relevant tool classes.
+
+### Usage
+
+```python
+from ph_utils.config_utils import load_env
+```
+
+### `1. load_env(file_dir, env_files): dict`:
+
+Load the environment variable file, the content behind the list will replace the content in front. `file_dir` - The environment variable file folder, default: `os.cwd()`; `env_files` - The environment variable file list, if `None` or empty list load `['.env', '.env.local', '.env.development', '.env.production']`
+
+### `2. load_json(file_dir, json_files): dict`:
+
+Load json file. default: `['config.json']`
+
+### `3. load_ini(file_dir, ini_files): dict`:
+
+Load `ini` file. default: `[config.ini]`
+
+## 2. `date-utils`
+
+The date processing tool.
+
+### Usage
+
+```python
+import ph_utils.date_utils as date_utils
+from ph_utils.date_utils import parse, format
+```
+
+### `1. parse(date_data: Any, fmt=None): datetime`
+
+You can parse various data formats into date objects, including time stamps, strings, and date objects themselves. Return `datetime` object.
+
+1. parse timestamp
+
+```python
+date_utils.parse(1691997308) # 2023-08-14 15:15:08
+```
+
+2. parse strings
+
+```python
+date_utils.parse('2023-08-14 15:23:23') # 2023-08-14 15:23:23
+date_utils.parse('20230814 152323') # 2023-08-14 15:23:23
+date_utils.parse('2023/08/14 15:23:23', '%Y/%m/%d %H:%M:%S') # 2023-08-14 15:23:23
+```
+
+3. parse `None` object
+
+```python
+date_utils.parse() # 2023-08-14 15:15:23.830691
+date_utils.parse(None) # 2023-08-14 15:15:23.830691
+```
+
+4. parse `datetime`
+
+```python
+date_utils.parse(date_utils.parse()) # 2023-08-14 15:19:48.382871
+```
+
+### `2. format(ori_date, pattern): str`
+
+Date formatting is the process of converting a date to a specific format.
+
+Parameter description:
+
+1. `ori_date`: **optional** All parameters that can be supported by the `parse` function.
+2. `pattern`: **optional** `default: %Y-%m-%d`, eg: `%Y-%m-%d %H:%M:%S`
+
+```python
+date_utils.format(None, '%Y-%m-%d %H:%M:%S')
+date_utils.format(1691997308, '%Y-%m-%d %H:%M:%S')
+```
+
+### `3. start_of(ori_date, unit, __format): datetime | int`
+
+Set the start of a time at a certain moment.
+
+Paramater description:
+
+1. `unit`: **optional** `default: date`, `date` - start time of a day
+2. `__format`: **optional** `default: None`, set the returned data, `None` - return `datetime`, `s`、`ms` return timestamp
+
+```python
+start_of() # datetime - 2023-08-15 00:00:00
+start_of(__format='s') # int - 1692028800
+```
+
+### `4. end_of(ori_date, unit, __format): datetime | int`
+
+Set the end of a time at a certain moment.
+
+```python
+end_of() # datetime - 2023-08-15 23:59:59
+```
+
+### `5. timestamp(ori_date, unit): int`
+
+Get timestamp of a time
+
+1. `unit`: `s` - _default_ length: 10，accurate to second、 `ms` length: 13, accurate to milliseconds.
+
+```python
+timestamp()
+```
+
+### `6. set(ori_date, values): datetime`
+
+Set date values to a given date.
+
+Sets time values to date from object . A value is not set if it is undefined or null or doesn't exist in values.
+
+`values`: `str | dict`，the given date. If is `dict`, include the follow property. `year`、`month`、`day`、`hour`、`minute`、`second`
+
+```python
+set(None, '2023-08-15 14:49:49')
+set(None, '2023/08/15 14:49:49')
+set(None, '20230815 144949')
+set(None, '20230815')
+set(None, '144949')
+set(None, { 'year': 2023, 'month': 8, 'day': 15, 'hour': 14, 'minute': 49, 'second': 49 })
+set(None, { 'year': 2023, 'month': 8, 'day': 15 })
+set(None, { 'hour': 14, 'minute': 49, 'second': 49 })
+```
+
+### `7. add(ori_date, duration): datetime`
+
+Add the specified years, months, weeks, days, hours, minutes and seconds to the given date.
+
+`duration` the object with years, months, weeks, days, hours, minutes and seconds to be added.
+
+```python
+add(duration={
+  'years': 2,
+  'months': 9,
+  'days': 7,
+  'hours': 5,
+  'minutes': 9,
+  'seconds': 30,
+})
+```
+
+### `8. subtract(ori_date, duration): datetime`
+
+Subtract the specified years, months, weeks, days, hours, minutes and seconds from the given date.
+
+```python
+subtract(duration={
+  'years': 2,
+  'months': 9,
+  'days': 7,
+  'hours': 5,
+  'minutes': 9,
+  'seconds': 30,
+})
+```
+
+### `9. sub(ori_date, duration): datetime`
+
+Alias of `subtract`.
+
+### `10: diff(start, end, result): int | timedelta`
+
+Get the number of full day periods between two dates.
+
+`result`: set the returned data. if `result = days` - return `int`, difference in days; otherwise return `timedelta`. default: `days`
+
+```python
+diff(parse(), parse()) # => 0
+```
```

### Comparing `ph-utils-0.0.7/README.md` & `ph_utils-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ph-utils-0.0.7/src/ph_utils/config.py` & `ph_utils-0.0.8/src/ph_utils/config.py`

 * *Files identical despite different names*

### Comparing `ph-utils-0.0.7/src/ph_utils/crypto.py` & `ph_utils-0.0.8/src/ph_utils/crypto.py`

 * *Files identical despite different names*

### Comparing `ph-utils-0.0.7/src/ph_utils/date.py` & `ph_utils-0.0.8/src/ph_utils/date.py`

 * *Files identical despite different names*

### Comparing `ph-utils-0.0.7/src/ph_utils/logger.py` & `ph_utils-0.0.8/src/ph_utils/logger.py`

 * *Files identical despite different names*

