# Comparing `tmp/swarkn-0.1.9.tar.gz` & `tmp/swarkn-0.1.9rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarkn-0.1.9.tar", max compression
+gzip compressed data, was "swarkn-0.1.9rc0.tar", max compression
```

## Comparing `swarkn-0.1.9.tar` & `swarkn-0.1.9rc0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      324 2023-11-14 08:46:24.502508 swarkn-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        7 2023-07-15 13:17:10.917432 swarkn-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-07-15 13:17:53.493071 swarkn-0.1.9/swarkn/__init__.py
--rw-r--r--   0        0        0        0 2023-08-31 00:35:10.883707 swarkn-0.1.9/swarkn/aws/__init__.py
--rw-r--r--   0        0        0      888 2023-10-03 08:30:37.551876 swarkn-0.1.9/swarkn/aws/s3.py
--rw-r--r--   0        0        0      398 2023-10-03 08:20:03.443679 swarkn-0.1.9/swarkn/caching.py
--rw-r--r--   0        0        0        0 2023-08-25 12:31:28.285903 swarkn-0.1.9/swarkn/charting/__init__.py
--rw-r--r--   0        0        0      292 2023-08-25 12:39:25.100665 swarkn-0.1.9/swarkn/charting/colors.py
--rw-r--r--   0        0        0     3959 2023-09-10 21:44:31.896276 swarkn-0.1.9/swarkn/charting/plotly_utils.py
--rw-r--r--   0        0        0     1365 2023-10-03 08:09:20.901933 swarkn-0.1.9/swarkn/collections.py
--rw-r--r--   0        0        0        0 2023-07-15 13:21:57.310233 swarkn-0.1.9/swarkn/db/__init__.py
--rw-r--r--   0        0        0     8855 2023-08-08 19:10:51.976901 swarkn-0.1.9/swarkn/db/postgres.py
--rw-r--r--   0        0        0      838 2023-07-15 13:27:35.425095 swarkn-0.1.9/swarkn/db/sql.py
--rw-r--r--   0        0        0     2020 2023-11-14 08:46:24.533475 swarkn-0.1.9/swarkn/helpers.py
--rw-r--r--   0        0        0      527 2023-09-20 08:23:42.871686 swarkn-0.1.9/swarkn/imports.py
--rw-r--r--   0        0        0      143 2023-07-15 13:27:35.417093 swarkn-0.1.9/swarkn/strings.py
--rw-r--r--   0        0        0        0 2023-09-20 08:19:25.230734 swarkn-0.1.9/swarkn/test/__init__.py
--rw-r--r--   0        0        0      543 2023-10-03 08:21:05.962782 swarkn-0.1.9/swarkn/test/caching.py
--rw-r--r--   0        0        0      326 2023-10-03 08:03:28.999823 swarkn-0.1.9/swarkn/test/collections.py
--rw-r--r--   0        0        0      253 2023-11-14 08:46:59.856245 swarkn-0.1.9/swarkn/test/helpers.py
--rw-r--r--   0        0        0      345 2023-09-20 08:30:47.864812 swarkn-0.1.9/swarkn/test/imports.py
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 swarkn-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      326 2023-11-13 09:03:51.607997 swarkn-0.1.9rc0/pyproject.toml
+-rw-r--r--   0        0        0        7 2023-07-15 13:17:10.917432 swarkn-0.1.9rc0/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 13:17:53.493071 swarkn-0.1.9rc0/swarkn/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-31 00:35:10.883707 swarkn-0.1.9rc0/swarkn/aws/__init__.py
+-rw-r--r--   0        0        0      888 2023-10-03 08:30:37.551876 swarkn-0.1.9rc0/swarkn/aws/s3.py
+-rw-r--r--   0        0        0      398 2023-10-03 08:20:03.443679 swarkn-0.1.9rc0/swarkn/caching.py
+-rw-r--r--   0        0        0        0 2023-08-25 12:31:28.285903 swarkn-0.1.9rc0/swarkn/charting/__init__.py
+-rw-r--r--   0        0        0      292 2023-08-25 12:39:25.100665 swarkn-0.1.9rc0/swarkn/charting/colors.py
+-rw-r--r--   0        0        0     3959 2023-09-10 21:44:31.896276 swarkn-0.1.9rc0/swarkn/charting/plotly_utils.py
+-rw-r--r--   0        0        0     1365 2023-10-03 08:09:20.901933 swarkn-0.1.9rc0/swarkn/collections.py
+-rw-r--r--   0        0        0        0 2023-07-15 13:21:57.310233 swarkn-0.1.9rc0/swarkn/db/__init__.py
+-rw-r--r--   0        0        0     8855 2023-08-08 19:10:51.976901 swarkn-0.1.9rc0/swarkn/db/postgres.py
+-rw-r--r--   0        0        0      838 2023-07-15 13:27:35.425095 swarkn-0.1.9rc0/swarkn/db/sql.py
+-rw-r--r--   0        0        0     1904 2023-11-13 08:25:24.924213 swarkn-0.1.9rc0/swarkn/helpers.py
+-rw-r--r--   0        0        0      527 2023-09-20 08:23:42.871686 swarkn-0.1.9rc0/swarkn/imports.py
+-rw-r--r--   0        0        0      143 2023-07-15 13:27:35.417093 swarkn-0.1.9rc0/swarkn/strings.py
+-rw-r--r--   0        0        0        0 2023-09-20 08:19:25.230734 swarkn-0.1.9rc0/swarkn/test/__init__.py
+-rw-r--r--   0        0        0      543 2023-10-03 08:21:05.962782 swarkn-0.1.9rc0/swarkn/test/caching.py
+-rw-r--r--   0        0        0      326 2023-10-03 08:03:28.999823 swarkn-0.1.9rc0/swarkn/test/collections.py
+-rw-r--r--   0        0        0      154 2023-11-13 08:25:24.861445 swarkn-0.1.9rc0/swarkn/test/helpers.py
+-rw-r--r--   0        0        0      345 2023-09-20 08:30:47.864812 swarkn-0.1.9rc0/swarkn/test/imports.py
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 swarkn-0.1.9rc0/PKG-INFO
```

### Comparing `swarkn-0.1.9/swarkn/aws/s3.py` & `swarkn-0.1.9rc0/swarkn/aws/s3.py`

 * *Files identical despite different names*

### Comparing `swarkn-0.1.9/swarkn/charting/plotly_utils.py` & `swarkn-0.1.9rc0/swarkn/charting/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `swarkn-0.1.9/swarkn/collections.py` & `swarkn-0.1.9rc0/swarkn/collections.py`

 * *Files identical despite different names*

### Comparing `swarkn-0.1.9/swarkn/db/postgres.py` & `swarkn-0.1.9rc0/swarkn/db/postgres.py`

 * *Files identical despite different names*

### Comparing `swarkn-0.1.9/swarkn/db/sql.py` & `swarkn-0.1.9rc0/swarkn/db/sql.py`

 * *Files identical despite different names*

### Comparing `swarkn-0.1.9/swarkn/helpers.py` & `swarkn-0.1.9rc0/swarkn/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 from collections.abc import Mapping
 from functools import lru_cache
 from time import perf_counter
 from contextlib import contextmanager
 logger = logging.getLogger(__name__)
 
 @contextmanager
-def timer(msg=None, logger_=logger, level='info') -> float:
+def timer(msg=None) -> float:
     start = perf_counter()
     yield perf_counter() - start
     cost = perf_counter() - start
     msg = msg or "Time taken: {cost}s"
-    fn = getattr(logger_, level)
-    fn(msg.format(cost=cost))
+    logger.info(msg.format(cost=cost))
 
 @lru_cache()
 def is_local():
     return 'win' in sys.platform
 
 def init_logger(level=logging.INFO, format='%(asctime)s|%(name)s|%(levelname)s|%(message)s'):
     logging.basicConfig(level=level, format=format)
@@ -33,20 +32,19 @@
             fn(f'failed func: {func} args: {args}, kwargs: {kwargs}, exception: {e}', **logger_kwags)
             if return_exception:
                 return e
 
     return innerfunc
 
 @contextmanager
-def swallow_exception(level='error', logger_=logger, **kwargs):
+def swallow_exception(**kwags):
     try:
         yield
     except Exception as ex:
-        fn = getattr(logger_, level)
-        fn(ex, **kwargs)
+        logger.error(ex, **kwags)
 
 
 def freeze(x):
     from frozendict import frozendict
     return frozendict(x) if isinstance(x, dict) else x
 
 def unfreeze(x):
```

### Comparing `swarkn-0.1.9/swarkn/imports.py` & `swarkn-0.1.9rc0/swarkn/imports.py`

 * *Files identical despite different names*

### Comparing `swarkn-0.1.9/swarkn/test/caching.py` & `swarkn-0.1.9rc0/swarkn/test/caching.py`

 * *Files identical despite different names*

