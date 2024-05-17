# Comparing `tmp/ftmq-0.6.3.tar.gz` & `tmp/ftmq-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftmq-0.6.3.tar", max compression
+gzip compressed data, was "ftmq-0.6.4.tar", max compression
```

## Comparing `ftmq-0.6.3.tar` & `ftmq-0.6.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.6.3/LICENSE
--rw-r--r--   0        0        0     4741 2024-01-31 02:14:30.592540 ftmq-0.6.3/README.md
--rw-r--r--   0        0        0       72 2024-05-17 10:35:24.709751 ftmq-0.6.3/ftmq/__init__.py
--rw-r--r--   0        0        0     2011 2024-01-03 16:54:37.194210 ftmq-0.6.3/ftmq/aggregate.py
--rw-r--r--   0        0        0     4790 2024-03-14 08:37:57.172570 ftmq-0.6.3/ftmq/aggregations.py
--rw-r--r--   0        0        0     4059 2024-03-14 17:13:11.419765 ftmq-0.6.3/ftmq/aleph.py
--rw-r--r--   0        0        0    10790 2024-04-04 12:20:24.054303 ftmq-0.6.3/ftmq/cli.py
--rw-r--r--   0        0        0      580 2024-02-23 20:01:04.717383 ftmq-0.6.3/ftmq/dedupe.py
--rw-r--r--   0        0        0     2517 2024-02-24 16:21:44.983220 ftmq-0.6.3/ftmq/enums.py
--rw-r--r--   0        0        0       93 2023-10-14 09:45:57.814196 ftmq-0.6.3/ftmq/exceptions.py
--rw-r--r--   0        0        0     7069 2023-10-14 09:45:57.814196 ftmq-0.6.3/ftmq/filters.py
--rw-r--r--   0        0        0     2807 2024-02-24 16:21:02.863390 ftmq-0.6.3/ftmq/io.py
--rw-r--r--   0        0        0      292 2024-03-13 18:50:42.659003 ftmq-0.6.3/ftmq/model/__init__.py
--rw-r--r--   0        0        0     4090 2024-03-13 19:40:59.788009 ftmq-0.6.3/ftmq/model/coverage.py
--rw-r--r--   0        0        0     5051 2024-05-17 10:17:43.525455 ftmq-0.6.3/ftmq/model/dataset.py
--rw-r--r--   0        0        0      482 2024-02-26 10:46:34.773368 ftmq-0.6.3/ftmq/model/mixins.py
--rw-r--r--   0        0        0     1866 2024-04-04 13:32:02.291870 ftmq-0.6.3/ftmq/model/proxy.py
--rw-r--r--   0        0        0    10276 2024-03-14 08:34:41.217377 ftmq-0.6.3/ftmq/query.py
--rw-r--r--   0        0        0    12223 2024-03-14 07:39:24.177208 ftmq-0.6.3/ftmq/sql.py
--rw-r--r--   0        0        0     2054 2024-03-14 05:58:47.124786 ftmq-0.6.3/ftmq/store/__init__.py
--rw-r--r--   0        0        0     1310 2024-02-24 16:21:45.719217 ftmq-0.6.3/ftmq/store/aleph.py
--rw-r--r--   0        0        0     3362 2024-03-14 08:35:41.593130 ftmq-0.6.3/ftmq/store/base.py
--rw-r--r--   0        0        0      768 2024-02-24 16:21:45.719217 ftmq-0.6.3/ftmq/store/level.py
--rw-r--r--   0        0        0      550 2024-03-13 18:57:03.036638 ftmq-0.6.3/ftmq/store/memory.py
--rw-r--r--   0        0        0      441 2024-02-23 20:01:36.309188 ftmq-0.6.3/ftmq/store/redis.py
--rw-r--r--   0        0        0     4878 2024-03-13 18:57:03.036638 ftmq-0.6.3/ftmq/store/sql.py
--rw-r--r--   0        0        0     1118 2024-04-04 12:11:45.481029 ftmq-0.6.3/ftmq/types.py
--rw-r--r--   0        0        0     5963 2024-04-04 12:14:29.656166 ftmq-0.6.3/ftmq/util.py
--rw-r--r--   0        0        0     1734 2024-05-17 10:35:24.709751 ftmq-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     6155 1970-01-01 00:00:00.000000 ftmq-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-04 14:31:45.930293 ftmq-0.6.4/LICENSE
+-rw-r--r--   0        0        0     4741 2024-01-31 02:14:30.592540 ftmq-0.6.4/README.md
+-rw-r--r--   0        0        0       72 2024-05-17 10:45:05.608660 ftmq-0.6.4/ftmq/__init__.py
+-rw-r--r--   0        0        0     2011 2024-01-03 16:54:37.194210 ftmq-0.6.4/ftmq/aggregate.py
+-rw-r--r--   0        0        0     4790 2024-03-14 08:37:57.172570 ftmq-0.6.4/ftmq/aggregations.py
+-rw-r--r--   0        0        0     4059 2024-03-14 17:13:11.419765 ftmq-0.6.4/ftmq/aleph.py
+-rw-r--r--   0        0        0    10790 2024-04-04 12:20:24.054303 ftmq-0.6.4/ftmq/cli.py
+-rw-r--r--   0        0        0      580 2024-02-23 20:01:04.717383 ftmq-0.6.4/ftmq/dedupe.py
+-rw-r--r--   0        0        0     2517 2024-02-24 16:21:44.983220 ftmq-0.6.4/ftmq/enums.py
+-rw-r--r--   0        0        0       93 2023-10-14 09:45:57.814196 ftmq-0.6.4/ftmq/exceptions.py
+-rw-r--r--   0        0        0     7069 2023-10-14 09:45:57.814196 ftmq-0.6.4/ftmq/filters.py
+-rw-r--r--   0        0        0     2807 2024-02-24 16:21:02.863390 ftmq-0.6.4/ftmq/io.py
+-rw-r--r--   0        0        0      292 2024-03-13 18:50:42.659003 ftmq-0.6.4/ftmq/model/__init__.py
+-rw-r--r--   0        0        0     4090 2024-03-13 19:40:59.788009 ftmq-0.6.4/ftmq/model/coverage.py
+-rw-r--r--   0        0        0     5051 2024-05-17 10:17:43.525455 ftmq-0.6.4/ftmq/model/dataset.py
+-rw-r--r--   0        0        0      482 2024-02-26 10:46:34.773368 ftmq-0.6.4/ftmq/model/mixins.py
+-rw-r--r--   0        0        0     1866 2024-04-04 13:32:02.291870 ftmq-0.6.4/ftmq/model/proxy.py
+-rw-r--r--   0        0        0    10276 2024-03-14 08:34:41.217377 ftmq-0.6.4/ftmq/query.py
+-rw-r--r--   0        0        0    12223 2024-03-14 07:39:24.177208 ftmq-0.6.4/ftmq/sql.py
+-rw-r--r--   0        0        0     2054 2024-03-14 05:58:47.124786 ftmq-0.6.4/ftmq/store/__init__.py
+-rw-r--r--   0        0        0     1310 2024-02-24 16:21:45.719217 ftmq-0.6.4/ftmq/store/aleph.py
+-rw-r--r--   0        0        0     3362 2024-03-14 08:35:41.593130 ftmq-0.6.4/ftmq/store/base.py
+-rw-r--r--   0        0        0      768 2024-02-24 16:21:45.719217 ftmq-0.6.4/ftmq/store/level.py
+-rw-r--r--   0        0        0      550 2024-03-13 18:57:03.036638 ftmq-0.6.4/ftmq/store/memory.py
+-rw-r--r--   0        0        0      441 2024-02-23 20:01:36.309188 ftmq-0.6.4/ftmq/store/redis.py
+-rw-r--r--   0        0        0     4878 2024-03-13 18:57:03.036638 ftmq-0.6.4/ftmq/store/sql.py
+-rw-r--r--   0        0        0     1118 2024-04-04 12:11:45.481029 ftmq-0.6.4/ftmq/types.py
+-rw-r--r--   0        0        0     5963 2024-04-04 12:14:29.656166 ftmq-0.6.4/ftmq/util.py
+-rw-r--r--   0        0        0     1755 2024-05-17 10:45:05.608660 ftmq-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     6197 1970-01-01 00:00:00.000000 ftmq-0.6.4/PKG-INFO
```

### Comparing `ftmq-0.6.3/LICENSE` & `ftmq-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/README.md` & `ftmq-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/aggregate.py` & `ftmq-0.6.4/ftmq/aggregate.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/aggregations.py` & `ftmq-0.6.4/ftmq/aggregations.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/aleph.py` & `ftmq-0.6.4/ftmq/aleph.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/cli.py` & `ftmq-0.6.4/ftmq/cli.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/dedupe.py` & `ftmq-0.6.4/ftmq/dedupe.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/enums.py` & `ftmq-0.6.4/ftmq/enums.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/filters.py` & `ftmq-0.6.4/ftmq/filters.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/io.py` & `ftmq-0.6.4/ftmq/io.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/model/coverage.py` & `ftmq-0.6.4/ftmq/model/coverage.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/model/dataset.py` & `ftmq-0.6.4/ftmq/model/dataset.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/model/proxy.py` & `ftmq-0.6.4/ftmq/model/proxy.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/query.py` & `ftmq-0.6.4/ftmq/query.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/sql.py` & `ftmq-0.6.4/ftmq/sql.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/store/__init__.py` & `ftmq-0.6.4/ftmq/store/__init__.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/store/aleph.py` & `ftmq-0.6.4/ftmq/store/aleph.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/store/base.py` & `ftmq-0.6.4/ftmq/store/base.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/store/level.py` & `ftmq-0.6.4/ftmq/store/level.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/store/memory.py` & `ftmq-0.6.4/ftmq/store/memory.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/store/sql.py` & `ftmq-0.6.4/ftmq/store/sql.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/types.py` & `ftmq-0.6.4/ftmq/types.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/ftmq/util.py` & `ftmq-0.6.4/ftmq/util.py`

 * *Files identical despite different names*

### Comparing `ftmq-0.6.3/pyproject.toml` & `ftmq-0.6.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ftmq"
-version = "0.6.3"
+version = "0.6.4"
 description = "followthemoney query dsl and io helpers"
 authors = ["Simon Wörpel <simon.woerpel@pm.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/investigativedata/ftmq"
 repository = "https://github.com/investigativedata/ftmq"
 documentation = "https://github.com/investigativedata/ftmq"
@@ -36,14 +36,15 @@
 pydantic = "^2.7.1"
 sqlalchemy = "^2.0.30"
 alephclient = "^2.4.1"
 pycountry = "^23.12.11"
 urllib3 = "<3"
 nomenklatura = "^3.10.6"
 anystore = "^0.1.3"
+pantomime = "^0.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3,<9.0.0"
 pytest-cov = ">=4.1,<6.0"
 black = ">=23.11,<25.0"
 isort = "^5.12.0"
 mypy = "^1.7.0"
```

### Comparing `ftmq-0.6.3/PKG-INFO` & `ftmq-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftmq
-Version: 0.6.3
+Version: 0.6.4
 Summary: followthemoney query dsl and io helpers
 Home-page: https://github.com/investigativedata/ftmq
 License: MIT
 Author: Simon Wörpel
 Author-email: simon.woerpel@pm.me
 Requires-Python: >=3.11,<3.12
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Requires-Dist: certifi (>=2024.2.2)
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: click-default-group (>=1.2.4,<2.0.0)
 Requires-Dist: cryptography (>=42.0.7,<43.0.0)
 Requires-Dist: followthemoney (>=3.6.0,<4.0.0)
 Requires-Dist: nomenklatura (>=3.10.6,<4.0.0)
 Requires-Dist: orjson (>=3.10.3,<4.0.0)
+Requires-Dist: pantomime (>=0.6.1,<0.7.0)
 Requires-Dist: pycountry (>=23.12.11,<24.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
 Requires-Dist: urllib3 (<3)
 Project-URL: Bug Tracker, https://github.com/investigativedata/ftmq/issues
 Project-URL: Documentation, https://github.com/investigativedata/ftmq
 Project-URL: Repository, https://github.com/investigativedata/ftmq
```

