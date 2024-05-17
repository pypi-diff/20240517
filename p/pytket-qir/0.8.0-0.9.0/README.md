# Comparing `tmp/pytket_qir-0.8.0-py3-none-any.whl.zip` & `tmp/pytket_qir-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 19924 bytes, number of entries: 13
--rw-r--r--  2.0 unx      842 b- defN 24-Jan-23 13:50 pytket/qir/__init__.py
--rw-r--r--  2.0 unx       66 b- defN 24-Jan-23 13:50 pytket/qir/_metadata.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-23 13:50 pytket/qir/py.typed
--rw-r--r--  2.0 unx      711 b- defN 24-Jan-23 13:50 pytket/qir/conversion/__init__.py
--rw-r--r--  2.0 unx     4866 b- defN 24-Jan-23 13:50 pytket/qir/conversion/api.py
--rw-r--r--  2.0 unx    41567 b- defN 24-Jan-23 13:50 pytket/qir/conversion/conversion.py
--rw-r--r--  2.0 unx     3960 b- defN 24-Jan-23 13:50 pytket/qir/conversion/gatesets.py
--rw-r--r--  2.0 unx     1465 b- defN 24-Jan-23 13:50 pytket/qir/conversion/module.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Jan-23 13:50 pytket_qir-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     4689 b- defN 24-Jan-23 13:50 pytket_qir-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-23 13:50 pytket_qir-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Jan-23 13:50 pytket_qir-0.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1075 b- defN 24-Jan-23 13:50 pytket_qir-0.8.0.dist-info/RECORD
-13 files, 70697 bytes uncompressed, 18118 bytes compressed:  74.4%
+Zip file size: 19953 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      842 b- defN 24-Mar-19 15:26 pytket/qir/__init__.py
+-rw-r--r--  2.0 unx       66 b- defN 24-Mar-19 15:26 pytket/qir/_metadata.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-19 15:26 pytket/qir/py.typed
+-rw-r--r--  2.0 unx      711 b- defN 24-Mar-19 15:26 pytket/qir/conversion/__init__.py
+-rw-r--r--  2.0 unx     4967 b- defN 24-Mar-19 15:26 pytket/qir/conversion/api.py
+-rw-r--r--  2.0 unx    41567 b- defN 24-Mar-19 15:26 pytket/qir/conversion/conversion.py
+-rw-r--r--  2.0 unx     3960 b- defN 24-Mar-19 15:26 pytket/qir/conversion/gatesets.py
+-rw-r--r--  2.0 unx     1465 b- defN 24-Mar-19 15:26 pytket/qir/conversion/module.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Mar-19 15:26 pytket_qir-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4689 b- defN 24-Mar-19 15:26 pytket_qir-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-19 15:26 pytket_qir-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Mar-19 15:26 pytket_qir-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1075 b- defN 24-Mar-19 15:26 pytket_qir-0.9.0.dist-info/RECORD
+13 files, 70798 bytes uncompressed, 18147 bytes compressed:  74.4%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: pytket/qir/conversion/gatesets.py
 Comment: 
 
 Filename: pytket/qir/conversion/module.py
 Comment: 
 
-Filename: pytket_qir-0.8.0.dist-info/LICENSE
+Filename: pytket_qir-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: pytket_qir-0.8.0.dist-info/METADATA
+Filename: pytket_qir-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: pytket_qir-0.8.0.dist-info/WHEEL
+Filename: pytket_qir-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: pytket_qir-0.8.0.dist-info/top_level.txt
+Filename: pytket_qir-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pytket_qir-0.8.0.dist-info/RECORD
+Filename: pytket_qir-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytket/qir/_metadata.py

```diff
@@ -1,2 +1,2 @@
-__extension_version__ = "0.8.0"
+__extension_version__ = "0.9.0"
 __extension_name__ = "pytket-qir"
```

## pytket/qir/conversion/api.py

```diff
@@ -73,15 +73,18 @@
 
     if cut_pytket_register:
         cpass = _scratch_reg_resize_pass(int_type)
         cpass.apply(circ)  # type: ignore
 
     for creg in circ.c_registers:
         if creg.size > 64:
-            raise ValueError("classical registers must not have more than 64 bits")
+            raise ValueError(
+                """classical registers must not have more than 64 bits, \
+you could try to set cut_pytket_register=True in the conversion"""
+            )
 
     m = tketqirModule(
         name=name,
         num_qubits=circ.n_qubits,
         num_results=circ.n_qubits,
     )
```

## Comparing `pytket_qir-0.8.0.dist-info/LICENSE` & `pytket_qir-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pytket_qir-0.8.0.dist-info/METADATA` & `pytket_qir-0.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytket-qir
-Version: 0.8.0
+Version: 0.9.0
 Summary: Extension for pytket, providing functions for conversion into to qir
 Author: TKET development team
 Author-email: tket-support@cambridgequantum.com
 License: Apache 2
 Project-URL: Documentation, https://tket.quantinuum.com/extensions/pytket-qir/index.html
 Project-URL: Source, https://github.com/CQCL/pytket-qir
 Project-URL: Tracker, https://github.com/CQCL/pytket-qir/issues
@@ -18,15 +18,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket ~=1.24
+Requires-Dist: pytket ~=1.26
 Requires-Dist: pyqir ==0.10.0
 
 # pytket-qir -- Pytket QIR Extension
 
 ## This is currently work in progress
 
 This repository contains the pytket-qir extension, using Quantinuum's
```

## Comparing `pytket_qir-0.8.0.dist-info/RECORD` & `pytket_qir-0.9.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 pytket/qir/__init__.py,sha256=s81GuzX7ftBqwVn3V6uW-f_8gnhadESlYjH9XGrvBH8,842
-pytket/qir/_metadata.py,sha256=CWHRJJCi4EDgOyetrwfKp5-NlcIWf9QOXQ8vkxboXvA,66
+pytket/qir/_metadata.py,sha256=FfW6yW2UXVwmqjb_eq7e5G8iauzbDEg7wa-VDxVZzek,66
 pytket/qir/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytket/qir/conversion/__init__.py,sha256=FKBWIdacKdT7Z-hy6dh_MeoOWNNkVVMiw1NqHM0NZts,711
-pytket/qir/conversion/api.py,sha256=rUL-d9a-qeIyPCkoc05nX7342st_4YrhzzhHcik9qM0,4866
+pytket/qir/conversion/api.py,sha256=DvxsPcSlrDNR86KUZNZJpLF5pqqCqDAMo-ktOErwK9o,4967
 pytket/qir/conversion/conversion.py,sha256=ZF6tqjVeMrnvW7g5ojAnHgaRlmXPY8JjkxNAJwkbf9g,41567
 pytket/qir/conversion/gatesets.py,sha256=o6_pw_8A7BaTrl9ickx3J_aFmHuQeNeZpreTpaPmKIU,3960
 pytket/qir/conversion/module.py,sha256=TOMygxQv3yhyTX35RidNnWGZXH7Rxz4ERTK5YtggzEk,1465
-pytket_qir-0.8.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pytket_qir-0.8.0.dist-info/METADATA,sha256=YRkDifDOvSBij-YsbRUVuywNED0Fa1xvwK74_X-FpPg,4689
-pytket_qir-0.8.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-pytket_qir-0.8.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
-pytket_qir-0.8.0.dist-info/RECORD,,
+pytket_qir-0.9.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pytket_qir-0.9.0.dist-info/METADATA,sha256=hsd6eM2uDVkAwTjuo7hyBGJJi0xSGRrhUVgOpU5S6K4,4689
+pytket_qir-0.9.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+pytket_qir-0.9.0.dist-info/top_level.txt,sha256=GsvCQQpJ7P8Vrx4ydtbjs36yufXiD59vSbbQFtFgcQ0,7
+pytket_qir-0.9.0.dist-info/RECORD,,
```

