# Comparing `tmp/tfrecord_slow-0.5.1.tar.gz` & `tmp/tfrecord_slow-0.6.0.tar.gz`

## Comparing `tfrecord_slow-0.5.1.tar` & `tfrecord_slow-0.6.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/requirements-dev.lock
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/requirements.lock
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/__init__.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/bench_fbs_reader.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/bench_fbs_writer.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/bench_flex_reader.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/bench_flex_writer.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/bench_reader.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/bench_writer.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/common.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/message.fbs
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/Data/Message.py
--rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/Data/NdArray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/examples/Data/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/__init__.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/__main__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/reader.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/writer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/loaders/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/loaders/msgpack_loader.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/loaders/raw_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/utils/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/utils/masked_crc.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/utils/msgpack.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/src/tfrecord_slow/utils/numpy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/tests/test_crc32c.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/tests/test_ndarray.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/tests/test_pickle.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/.gitignore
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/README.md
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 tfrecord_slow-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/requirements-dev.lock
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/requirements.lock
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/__init__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/bench_fbs_reader.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/bench_fbs_writer.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/bench_flex_reader.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/bench_flex_writer.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/bench_reader.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/bench_writer.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/common.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/message.fbs
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/Data/Message.py
+-rw-r--r--   0        0        0     4293 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/Data/NdArray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/examples/Data/__init__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/__init__.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/__main__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/reader.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/writer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/loaders/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/loaders/msgpack_loader.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/loaders/raw_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/utils/__init__.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/utils/masked_crc.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/utils/msgpack.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/src/tfrecord_slow/utils/numpy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/tests/test_crc32c.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/tests/test_ndarray.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/tests/test_pickle.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/.gitignore
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/LICENSE
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/README.md
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 tfrecord_slow-0.6.0/PKG-INFO
```

### Comparing `tfrecord_slow-0.5.1/requirements-dev.lock` & `tfrecord_slow-0.6.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/.github/workflows/python-package.yml` & `tfrecord_slow-0.6.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/.github/workflows/python-publish.yml` & `tfrecord_slow-0.6.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/examples/bench_fbs_reader.py` & `tfrecord_slow-0.6.0/examples/bench_fbs_reader.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/examples/bench_fbs_writer.py` & `tfrecord_slow-0.6.0/examples/bench_fbs_writer.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/examples/bench_flex_reader.py` & `tfrecord_slow-0.6.0/examples/bench_flex_reader.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/examples/bench_flex_writer.py` & `tfrecord_slow-0.6.0/examples/bench_flex_writer.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/examples/Data/Message.py` & `tfrecord_slow-0.6.0/examples/Data/Message.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/examples/Data/NdArray.py` & `tfrecord_slow-0.6.0/examples/Data/NdArray.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/src/tfrecord_slow/__main__.py` & `tfrecord_slow-0.6.0/src/tfrecord_slow/__main__.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/src/tfrecord_slow/reader.py` & `tfrecord_slow-0.6.0/src/tfrecord_slow/reader.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/src/tfrecord_slow/writer.py` & `tfrecord_slow-0.6.0/src/tfrecord_slow/writer.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/src/tfrecord_slow/loaders/msgpack_loader.py` & `tfrecord_slow-0.6.0/src/tfrecord_slow/loaders/msgpack_loader.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/src/tfrecord_slow/loaders/raw_loader.py` & `tfrecord_slow-0.6.0/src/tfrecord_slow/loaders/raw_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import BufferedIOBase
 from tfrecord_slow.reader import TfrecordReader
 
 T = TypeVar("T")
 
 
 def _default_func(buf: memoryview):
-    return buf.tobytes()
+    return buf
 
 
 class RawTfrecordLoader(Generic[T]):
     def __init__(
         self,
         datapipe: Iterable[BufferedIOBase],
         func: Callable[[memoryview], T] = _default_func,
```

### Comparing `tfrecord_slow-0.5.1/src/tfrecord_slow/utils/msgpack.py` & `tfrecord_slow-0.6.0/src/tfrecord_slow/utils/msgpack.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/tests/test_ndarray.py` & `tfrecord_slow-0.6.0/tests/test_ndarray.py`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/.gitignore` & `tfrecord_slow-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/README.md` & `tfrecord_slow-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `tfrecord_slow-0.5.1/pyproject.toml` & `tfrecord_slow-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tfrecord-slow"
-version = "0.5.1"
+version = "0.6.0"
 description = "TFRecord reader and writer without protobuf."
 authors = [
     { name = "SunDoge", email = "triplez0@outlook.com" }
 ]
 dependencies = [
 ]
 readme = "README.md"
```

### Comparing `tfrecord_slow-0.5.1/PKG-INFO` & `tfrecord_slow-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: tfrecord-slow
-Version: 0.5.1
+Version: 0.6.0
 Summary: TFRecord reader and writer without protobuf.
 Author-email: SunDoge <triplez0@outlook.com>
+License-File: LICENSE
 Requires-Python: >=3.9
 Provides-Extra: cli
 Requires-Dist: loguru>=0.7.2; extra == 'cli'
 Requires-Dist: tqdm>=4.66.2; extra == 'cli'
 Provides-Extra: crc32c
 Requires-Dist: crc32c>=2.4; extra == 'crc32c'
 Requires-Dist: numpy>=1; extra == 'crc32c'
```

