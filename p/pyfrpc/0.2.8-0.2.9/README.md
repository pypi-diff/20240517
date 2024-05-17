# Comparing `tmp/pyfrpc-0.2.8.tar.gz` & `tmp/pyfrpc-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfrpc-0.2.8.tar", last modified: Mon Jul 24 08:06:59 2023, max compression
+gzip compressed data, was "pyfrpc-0.2.9.tar", last modified: Wed Aug 30 14:54:56 2023, max compression
```

## Comparing `pyfrpc-0.2.8.tar` & `pyfrpc-0.2.9.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.645895 pyfrpc-0.2.8/
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4423 2023-07-24 08:06:59.645895 pyfrpc-0.2.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3752 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 08:06:59.645895 pyfrpc-0.2.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2180 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.638895 pyfrpc-0.2.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.641895 pyfrpc-0.2.8/src/pyfrpc/
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    15603 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/_coding_base_c.pyx
--rw-rw-rw-   0 root         (0) root         (0)    10197 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/_coding_base_py.py
--rw-rw-rw-   0 root         (0) root         (0)     3218 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/asyncclient.py
--rw-rw-rw-   0 root         (0) root         (0)     3939 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3278 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/coding.py
--rw-rw-rw-   0 root         (0) root         (0)      718 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/models.py
--rw-rw-rw-   0 root         (0) root         (0)      820 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/src/pyfrpc/netcat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.643895 pyfrpc-0.2.8/src/pyfrpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4423 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      599 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-24 08:06:59.000000 pyfrpc-0.2.8/src/pyfrpc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 08:06:59.644895 pyfrpc-0.2.8/test/
--rw-rw-rw-   0 root         (0) root         (0)     2854 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_fastrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     2401 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol_v1.py
--rw-rw-rw-   0 root         (0) root         (0)     5658 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2023-07-24 08:06:43.000000 pyfrpc-0.2.8/test/test_protocol_v3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-30 14:54:56.015337 pyfrpc-0.2.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4423 2023-08-30 14:54:56.015337 pyfrpc-0.2.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3752 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-30 14:54:56.015337 pyfrpc-0.2.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2180 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-30 14:54:56.008004 pyfrpc-0.2.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-30 14:54:56.011670 pyfrpc-0.2.9/src/pyfrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14845 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/_coding_base_c.pyx
+-rw-rw-rw-   0 root         (0) root         (0)    10341 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/_coding_base_py.py
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/asyncclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3278 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/coding.py
+-rw-rw-rw-   0 root         (0) root         (0)      718 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      820 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/src/pyfrpc/netcat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-30 14:54:56.013503 pyfrpc-0.2.9/src/pyfrpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4423 2023-08-30 14:54:55.000000 pyfrpc-0.2.9/src/pyfrpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      623 2023-08-30 14:54:56.000000 pyfrpc-0.2.9/src/pyfrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-30 14:54:55.000000 pyfrpc-0.2.9/src/pyfrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-30 14:54:55.000000 pyfrpc-0.2.9/src/pyfrpc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-08-30 14:54:55.000000 pyfrpc-0.2.9/src/pyfrpc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-30 14:54:55.000000 pyfrpc-0.2.9/src/pyfrpc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-30 14:54:56.014420 pyfrpc-0.2.9/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2854 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/test/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/test/test_fastrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/test/test_protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     2401 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/test/test_protocol_v1.py
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/test/test_protocol_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/test/test_protocol_v3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-08-30 14:54:35.000000 pyfrpc-0.2.9/test/test_subclasses.py
```

### Comparing `pyfrpc-0.2.8/LICENSE.txt` & `pyfrpc-0.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/PKG-INFO` & `pyfrpc-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrpc
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python implementation of fastrpc protocol
 Home-page: https://gitlab.com/vladaburian/pyfrpc
 Author: Vladimir Burian
 License: MIT
 Keywords: frpc fastrpc
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrpc-0.2.8/README.md` & `pyfrpc-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/setup.py` & `pyfrpc-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 PYFRPC_NOEXT = bool(int(os.environ.get('PYFRPC_NOEXT', '0')))
 
 
 setup_args = dict(
     name='pyfrpc',
-    version='0.2.8',
+    version='0.2.9',
     description='Python implementation of fastrpc protocol',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Vladimir Burian',
     license='MIT',
     url='https://gitlab.com/vladaburian/pyfrpc',
     classifiers=[
```

### Comparing `pyfrpc-0.2.8/src/pyfrpc/_coding_base_c.pyx` & `pyfrpc-0.2.9/src/pyfrpc/_coding_base_c.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,21 @@
 # -*- coding: utf-8 -*-
 
 import cython
 
+from collections.abc import ByteString, Mapping, Sequence
 from datetime import datetime, timezone, timedelta
+from numbers import Integral, Real
 
 from libc.stdint cimport *
 from libc.string cimport memcpy
 
+from cpython.bytearray cimport PyByteArray_Size, PyByteArray_AsString, PyByteArray_Resize
 from cpython.bytes cimport PyBytes_Size, PyBytes_AsString
-from cpython.version cimport PY_MAJOR_VERSION
-
-
-cdef extern from "Python.h":
-    char* PyUnicode_AsUTF8AndSize(object unicode, Py_ssize_t *size)
-    # Return a pointer to the UTF-8 encoding of the Unicode object, and store
-    # the size of the encoded representation (in bytes) in size. The size
-    # argument can be NULL; in this case no size will be stored. The returned
-    # buffer always has an extra null byte appended (not included in size),
-    # regardless of whether there are any other null code points.
-    #
-    # In the case of an error, NULL is returned with an exception set and no
-    # size is stored.
-    #
-    # This caches the UTF-8 representation of the string in the Unicode object,
-    # and subsequent calls will return a pointer to the same buffer. The caller
-    # is not responsible for deallocating the buffer.
-    #
-    # New in version 3.3.
-
-    Py_ssize_t PyByteArray_Size(object bytearray)
-    # Return the size of bytearray after checking for a NULL pointer.
-
-    char* PyByteArray_AsString(object bytearray)
-    # Return the contents of bytearray as a char array after checking for a NULL
-    # pointer. The returned array always has an extra null byte appended.
-
-    int PyByteArray_Resize(object bytearray, Py_ssize_t len)
-    # Resize the internal buffer of bytearray to len.
-
+from cpython.unicode cimport PyUnicode_AsUTF8AndSize
 
 
 @cython.final
 cdef class FrpcDecoder:
     cdef BinaryReader io
     cdef int32_t version
 
@@ -208,21 +182,21 @@
 
     cdef _encode_data(self, value):
         value_type = type(value)
 
         if value_type is bool:
             self.io.write_int(0x10 | (0x01 if value else 0x00), 1)
 
-        elif (value_type is int) or (value_type is long):
+        elif value_type is int:
             self._encode_int(value)
 
         elif value_type is float:
             self._encode_double(value)
 
-        elif (value_type is str):
+        elif value_type is str:
             self._encode_str(value)
 
         elif (value_type is bytearray) or (value_type is bytes):
             self._encode_bin(value)
 
         elif value is None:
             self._encode_null()
@@ -232,14 +206,26 @@
 
         elif (value_type is list) or (value_type is tuple):
             self._encode_array(value)
 
         elif value_type is datetime:
             self._encode_datetime(value)
 
+        elif issubclass(value_type, ByteString):
+            self._encode_bin(bytes(value))
+
+        elif issubclass(value_type, Mapping):
+            self._encode_struct(value)
+
+        elif issubclass(value_type, Sequence):
+            self._encode_array(value)
+
+        elif issubclass(value_type, datetime):
+            self._encode_datetime(value)
+
         else:
             raise Exception("unknown type to encode ({})".format(value_type))
 
     cdef _etwi(self, int32_t type_id, uint64_t value):
         """
         Encode type with integer.
         """
@@ -301,18 +287,18 @@
     cdef _encode_null(self):
         if self.version < 0x0201:
             # Null was introduced in v2.1
             raise Exception("null can't be encoded")
 
         self.io.write_int(0x0C << 3, 1)
 
-    cdef _encode_struct(self, dict value):
+    cdef _encode_struct(self, value):
         self._etwi(0x0A, len(value))
 
-        for k, v in value.iteritems():
+        for k, v in value.items():
             self._encode_struct_key(k)
             self._encode_data(v)
 
     cdef _encode_struct_key(self, key):
         utf8 = string_to_utf8(key)
 
         if utf8.size > 0xff:
@@ -384,15 +370,15 @@
         if isinstance(value, bytes):
             self.io.write_raw(PyBytes_AsString(value), size)
 
         elif isinstance(value, bytearray):
             self.io.write_raw(PyByteArray_AsString(value), size)
 
         else:
-            Exception("this should never happen")
+            raise Exception("this should never happen")
 
 
 ################################################################################
 # Low level binary IO
 ################################################################################
 
 @cython.final
```

### Comparing `pyfrpc-0.2.8/src/pyfrpc/_coding_base_py.py` & `pyfrpc-0.2.9/src/pyfrpc/_coding_base_py.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import struct
 
+from collections.abc import ByteString, Mapping, Sequence
 from datetime import datetime, timezone, timedelta
 
 
 class FrpcDecoder:
     def __init__(self, buf, offset, version):
         self.buf = buf
         self.idx = offset
@@ -214,21 +215,24 @@
 
         elif isinstance(value, datetime):
             self._encode_datetime(value)
 
         elif isinstance(value, (bytearray, bytes)):
             self._encode_bin(value)
 
+        elif isinstance(value, ByteString):
+            self._encode_bin(bytes(value))
+
         elif value is None:
             self._encode_null()
 
-        elif isinstance(value, dict):
+        elif isinstance(value, Mapping):
             self._encode_struct(value)
 
-        elif isinstance(value, (list, tuple)):
+        elif isinstance(value, Sequence):
             self._encode_array(value)
 
         else:
             raise Exception("unknown type to encode ({})".format(value_type))
 
     def _etwi(self, type_id, value):
         """
```

### Comparing `pyfrpc-0.2.8/src/pyfrpc/asyncclient.py` & `pyfrpc-0.2.9/src/pyfrpc/asyncclient.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/src/pyfrpc/client.py` & `pyfrpc-0.2.9/src/pyfrpc/client.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/src/pyfrpc/coding.py` & `pyfrpc-0.2.9/src/pyfrpc/coding.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/src/pyfrpc/models.py` & `pyfrpc-0.2.9/src/pyfrpc/models.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/src/pyfrpc/netcat.py` & `pyfrpc-0.2.9/src/pyfrpc/netcat.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/src/pyfrpc.egg-info/PKG-INFO` & `pyfrpc-0.2.9/src/pyfrpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfrpc
-Version: 0.2.8
+Version: 0.2.9
 Summary: Python implementation of fastrpc protocol
 Home-page: https://gitlab.com/vladaburian/pyfrpc
 Author: Vladimir Burian
 License: MIT
 Keywords: frpc fastrpc
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pyfrpc-0.2.8/test/conftest.py` & `pyfrpc-0.2.9/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/test/test_fastrpc.py` & `pyfrpc-0.2.9/test/test_fastrpc.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/test/test_protocol.py` & `pyfrpc-0.2.9/test/test_protocol.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/test/test_protocol_v1.py` & `pyfrpc-0.2.9/test/test_protocol_v1.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/test/test_protocol_v2.py` & `pyfrpc-0.2.9/test/test_protocol_v2.py`

 * *Files identical despite different names*

### Comparing `pyfrpc-0.2.8/test/test_protocol_v3.py` & `pyfrpc-0.2.9/test/test_protocol_v3.py`

 * *Files identical despite different names*

