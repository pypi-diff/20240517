# Comparing `tmp/PyQBDI-0.8.0-cp39-cp39-win_amd64.whl.zip` & `tmp/PyQBDI-0.9.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1259920 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat  5731328 b- defN 21-Feb-11 15:24 pyqbdi.pyd
--rw-rw-rw-  2.0 fat     2937 b- defN 21-Feb-11 15:24 pyqbdipreload.py
--rw-rw-rw-  2.0 fat    11340 b- defN 21-Feb-11 15:24 PyQBDI-0.8.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4662 b- defN 21-Feb-11 15:24 PyQBDI-0.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 21-Feb-11 15:24 PyQBDI-0.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 21-Feb-11 15:24 PyQBDI-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      529 b- defN 21-Feb-11 15:24 PyQBDI-0.8.0.dist-info/RECORD
-7 files, 5750903 bytes uncompressed, 1258998 bytes compressed:  78.1%
+Zip file size: 1398936 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat  5827584 b- defN 22-Mar-31 10:39 pyqbdi.pyd
+-rw-rw-rw-  2.0 fat     3097 b- defN 22-Mar-31 10:39 pyqbdipreload.py
+-rw-rw-rw-  2.0 fat    12462 b- defN 22-Mar-31 10:39 PyQBDI-0.9.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4791 b- defN 22-Mar-31 10:39 PyQBDI-0.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 22-Mar-31 10:39 PyQBDI-0.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 22-Mar-31 10:39 PyQBDI-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      529 b- defN 22-Mar-31 10:39 PyQBDI-0.9.0.dist-info/RECORD
+7 files, 5848570 bytes uncompressed, 1398014 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pyqbdi.pyd
 Comment: 
 
 Filename: pyqbdipreload.py
 Comment: 
 
-Filename: PyQBDI-0.8.0.dist-info/LICENSE.txt
+Filename: PyQBDI-0.9.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PyQBDI-0.8.0.dist-info/METADATA
+Filename: PyQBDI-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: PyQBDI-0.8.0.dist-info/WHEEL
+Filename: PyQBDI-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: PyQBDI-0.8.0.dist-info/top_level.txt
+Filename: PyQBDI-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: PyQBDI-0.8.0.dist-info/RECORD
+Filename: PyQBDI-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyqbdipreload.py

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 
 # This file is part of pyQBDI (python binding for QBDI).
 #
-# Copyright 2017 Quarkslab
+# Copyright 2017 - 2022 Quarkslab
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,25 +18,29 @@
 
 
 import platform
 import pyqbdi
 from ctypes import util as ctypesutil
 import sys
 import os
-
+import argparse
 
 def run():
 
-    if len(sys.argv) <= 2 or sys.argv[1] in ['-h', '--help']:
-        print("Usage: python -m {} <script> <target> [<args> ...]".format(sys.argv[0]))
-        exit(1)
-
-    script = sys.argv[1]
-    binary = sys.argv[2]
-    args = sys.argv[2:]
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument("script", type=str, help="PyQBDI script")
+    parser.add_argument("target", type=str, help="command to instrument")
+    parser.add_argument("args", type=str, help="command arguments", nargs='*')
+
+    args = parser.parse_args()
+
+    script = args.script
+    binary = args.target
+    args = [args.target] + args.args
     environ = os.environ.copy()
 
     # add LD_PRELOAD or DYLD_INSERT_LIBRARIES
     if platform.system() == 'Darwin':
         environ["DYLD_INSERT_LIBRARIES"] = pyqbdi.__file__
     elif platform.system() == 'Linux':
         libpythonname = "python{}.{}".format(sys.version_info.major, sys.version_info.minor)
```

## Comparing `PyQBDI-0.8.0.dist-info/LICENSE.txt` & `PyQBDI-0.9.0.dist-info/LICENSE.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+################################################################################
+QBDI package license
+################################################################################
+
+QBDI binaries and packages can be statically linked with the followed source:
+
+- QBDI under the Apache License v2.0
+- LLVM under the Apache License v2.0 with LLVM Exceptions
+    https://releases.llvm.org/10.0.0/LICENSE.TXT
+- spdlog under the MIT License
+    https://github.com/gabime/spdlog/blob/v1.x/LICENSE
+- fmtlib under the MIT License
+    https://github.com/fmtlib/fmt/blob/master/LICENSE.rst
+- Catch2 under the Boost Software License 1.0
+    https://github.com/catchorg/Catch2/blob/devel/LICENSE.txt
+- Pybind11 under a BSD-style license
+    https://github.com/pybind/pybind11/blob/master/LICENSE
+- A sha256 implementation under GPLv3 / Apache License v2.0
+    https://github.com/aguinet/sha256_literal#licensing
+
+################################################################################
+QBDI source code is under the Apache License v2.0
+################################################################################
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
@@ -183,15 +206,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2017 Quarkslab
+   Copyright 2017 - 2022 Quarkslab
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `PyQBDI-0.8.0.dist-info/METADATA` & `PyQBDI-0.9.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQBDI
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python binding for QBDI
 Home-page: UNKNOWN
 Author: Nicolas Surbayrole
 Author-email: qbdi@quarkslab.com
 License: apache2
 Project-URL: Documentation, https://qbdi.readthedocs.io/
 Project-URL: Source, https://github.com/QBDI/QBDI
@@ -12,41 +12,47 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Debuggers
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/qbdi/badge/?version=stable
     :target: https://qbdi.readthedocs.io/en/stable/?badge=stable
     :alt: Documentation Status
 
-.. image:: https://travis-ci.com/QBDI/QBDI.svg?branch=master
-    :target: https://travis-ci.com/QBDI/QBDI
-
 .. image:: https://ci.appveyor.com/api/projects/status/s2qvpu8k8yiau647/branch/master?svg=true
     :target: https://ci.appveyor.com/project/QBDI/qbdi/branch/master
 
+.. image:: https://img.shields.io/github/v/release/QBDI/QBDI
+    :target: https://github.com/QBDI/QBDI/releases
+
+.. image:: https://img.shields.io/pypi/pyversions/PyQBDI
+    :target: https://pypi.org/project/PyQBDI/
+
+.. image:: https://img.shields.io/pypi/v/PyQBDI
+    :target: https://pypi.org/project/PyQBDI/
+
 QuarkslaB Dynamic binary Instrumentation (QBDI) is a modular, cross-platform and cross-architecture
 DBI framework. It aims to support Linux, macOS, Android, iOS and Windows operating systems running on
 x86, x86-64, ARM and AArch64 architectures. In addition of C/C++ API, Python and JS/frida bindings are
 available to script QBDI. Information about what is a DBI framework and how QBDI
-works can be found in the user documentation introduction (`User Documentation <https://qbdi.readthedocs.io/en/stable/user.html>`_).
+works can be found in the `documentation introduction <https://qbdi.readthedocs.io/en/stable/intro.html>`_.
 
 QBDI modularity means it doesn't contain a preferred injection method and it is designed to be
 used in conjunction with an external injection tool. QBDI includes a tiny (``LD_PRELOAD`` based)
 Linux and macOS injector for dynamic executables (QBDIPreload).
 QBDI is also fully integrated with `Frida <https://frida.re>`_, a reference dynamic instrumentation toolkit,
 allowing anybody to use their combined powers.
 
@@ -59,26 +65,24 @@
 ++++++
 
 .. role:: green
 .. role:: yellow
 .. role:: orange
 .. role:: red
 
-=======   ==============================   ======================   =================================
-CPU       Operating Systems                Execution                Memory Access Information
-=======   ==============================   ======================   =================================
-x86-64    Android, Linux, macOS, Windows   :green:`Supported`       :green:`Supported`
-x86       Android, Linux, macOS, Windows   :green:`Supported`       :green:`Supported`
-ARM       Linux, Android, iOS              :orange:`Planned (*)`    :orange:`Planned (*)`
-AArch64   Android                          :orange:`Planned (*)`    :orange:`Planned (*)`
-=======   ==============================   ======================   =================================
-
-.. warning::
+=======   ==============================   ========================   =================================
+CPU       Operating Systems                Execution                  Memory Access Information
+=======   ==============================   ========================   =================================
+x86-64    Android, Linux, macOS, Windows   :green:`Supported`         :green:`Supported`
+x86       Android, Linux, macOS, Windows   :green:`Supported`         :green:`Supported`
+ARM       Linux, Android, iOS              :orange:`Planned (*)`      :orange:`Planned (*)`
+AArch64   Android, Linux, macOS            :orange:`Supported (*)`    :orange:`Supported (*)`
+=======   ==============================   ========================   =================================
 
-   The ARM and AArch64 instruction sets are supported but they still need to be integrated along with x86 and x86-64.
+\* The ARM and AArch64 instruction sets are supported for internal use at the moment.
 
 Installation
 ============
 
 Python API (PyQBDI)
 +++++++++++++++++++
```

