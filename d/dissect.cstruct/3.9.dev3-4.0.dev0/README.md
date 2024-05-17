# Comparing `tmp/dissect.cstruct-3.9.dev3.tar.gz` & `tmp/dissect_cstruct-4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.cstruct-3.9.dev3.tar", last modified: Fri Aug  4 12:14:58 2023, max compression
+gzip compressed data, was "dissect_cstruct-4.0.dev0.tar", last modified: Fri May 17 14:33:57 2024, max compression
```

## Comparing `dissect.cstruct-3.9.dev3.tar` & `dissect_cstruct-4.0.dev0.tar`

### file list

```diff
@@ -1,68 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.046307 dissect.cstruct-3.9.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-04 12:14:58.046307 dissect.cstruct-3.9.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.022307 dissect.cstruct-3.9.dev3/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.034307 dissect.cstruct-3.9.dev3/dissect/cstruct/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    19489 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.038307 dissect.cstruct-3.9.dev3/dissect/cstruct/types/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/bytesinteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/chartype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/packedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/voidtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/types/wchartype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/dissect/cstruct/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.030307 dissect.cstruct-3.9.dev3/dissect.cstruct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-04 12:14:57.000000 dissect.cstruct-3.9.dev3/dissect.cstruct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-08-04 12:14:58.000000 dissect.cstruct-3.9.dev3/dissect.cstruct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:14:57.000000 dissect.cstruct-3.9.dev3/dissect.cstruct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 12:14:57.000000 dissect.cstruct-3.9.dev3/dissect.cstruct.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.038307 dissect.cstruct-3.9.dev3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/examples/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/examples/mirai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/examples/pe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/examples/secdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-04 12:14:44.000000 dissect.cstruct-3.9.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:14:58.046307 dissect.cstruct-3.9.dev3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.046307 dissect.cstruct-3.9.dev3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.046307 dissect.cstruct-3.9.dev3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/data/testdef.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:14:58.046307 dissect.cstruct-3.9.dev3/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_bitfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_bytesinteger.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_ctypes_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_packedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-04 12:14:38.000000 dissect.cstruct-3.9.dev3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.717146 dissect_cstruct-4.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.701146 dissect_cstruct-4.0.dev0/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.705146 dissect_cstruct-4.0.dev0/dissect/cstruct/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14851 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.709146 dissect_cstruct-4.0.dev0/dissect/cstruct/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/leb128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23954 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/void.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/types/wchar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10297 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/dissect/cstruct/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8303 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 14:33:57.000000 dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.709146 dissect_cstruct-4.0.dev0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/mirai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/examples/secdesc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:33:57.717146 dissect_cstruct-4.0.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/data/testdef.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:33:57.713146 dissect_cstruct-4.0.dev0/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8508 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13692 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5627 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_bitfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9208 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8853 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12932 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_leb128.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_packed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_void.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_types_wchar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-17 14:33:48.000000 dissect_cstruct-4.0.dev0/tox.ini
```

### Comparing `dissect.cstruct-3.9.dev3/LICENSE` & `dissect_cstruct-4.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev3/PKG-INFO` & `dissect_cstruct-4.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 3.9.dev3
+Version: 4.0.dev0
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
@@ -220,15 +220,15 @@
 assert a.dumps() == d
 ```
 
 ### Enums
 The API to access enum members and their values is similar to that of the native Enum type in Python 3. Functionally, it's best comparable to the IntEnum type.
 
 ### Custom types
-You can implement your own types by subclassing `BaseType` or `RawType`, and adding them to your cstruct instance with `addtype(name, type)`
+You can implement your own types by subclassing `BaseType` or `RawType`, and adding them to your cstruct instance with `add_type(name, type)`
 
 ### Custom definition parsers
 Don't like the C-like definition syntax? Write your own syntax parser!
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
```

### Comparing `dissect.cstruct-3.9.dev3/README.md` & `dissect_cstruct-4.0.dev0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 assert a.dumps() == d
 ```
 
 ### Enums
 The API to access enum members and their values is similar to that of the native Enum type in Python 3. Functionally, it's best comparable to the IntEnum type.
 
 ### Custom types
-You can implement your own types by subclassing `BaseType` or `RawType`, and adding them to your cstruct instance with `addtype(name, type)`
+You can implement your own types by subclassing `BaseType` or `RawType`, and adding them to your cstruct instance with `add_type(name, type)`
 
 ### Custom definition parsers
 Don't like the C-like definition syntax? Write your own syntax parser!
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
```

### Comparing `dissect.cstruct-3.9.dev3/dissect/cstruct/bitbuffer.py` & `dissect_cstruct-4.0.dev0/dissect/cstruct/bitbuffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, BinaryIO, Union
+from typing import TYPE_CHECKING, BinaryIO
 
 if TYPE_CHECKING:
-    from dissect.cstruct.types import RawType
+    from dissect.cstruct.types import BaseType
 
 
 class BitBuffer:
     """Implements a bit buffer that can read and write bit fields."""
 
     def __init__(self, stream: BinaryIO, endian: str):
         self.stream = stream
         self.endian = endian
 
         self._type = None
         self._buffer = 0
         self._remaining = 0
 
-    def read(self, field_type: RawType, bits: Union[int, bytes]) -> int:
+    def read(self, field_type: BaseType, bits: int) -> int:
         if self._remaining == 0 or self._type != field_type:
             self._type = field_type
             self._remaining = field_type.size * 8
             self._buffer = field_type._read(self.stream)
 
         if isinstance(self._buffer, bytes):
             if self.endian == "<":
@@ -39,15 +39,15 @@
         else:
             v = self._buffer & (((1 << (self._remaining - bits)) - 1) ^ ((1 << self._remaining) - 1))
             v >>= self._remaining - bits
             self._remaining -= bits
 
         return v
 
-    def write(self, field_type: RawType, data: int, bits: int) -> None:
+    def write(self, field_type: BaseType, data: int, bits: int) -> None:
         if self._remaining == 0 or self._type != field_type:
             if self._type:
                 self.flush()
             self._remaining = field_type.size * 8
             self._type = field_type
 
         if self.endian == "<":
```

### Comparing `dissect.cstruct-3.9.dev3/dissect/cstruct/parser.py` & `dissect_cstruct-4.0.dev0/dissect/cstruct/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from __future__ import annotations
 
 import ast
 import re
-from typing import TYPE_CHECKING, Dict, List
+from typing import TYPE_CHECKING
 
-from dissect.cstruct.compiler import Compiler
-from dissect.cstruct.exceptions import ParserError
+from dissect.cstruct import compiler
+from dissect.cstruct.exceptions import (
+    ExpressionParserError,
+    ExpressionTokenizerError,
+    ParserError,
+)
 from dissect.cstruct.expression import Expression
-from dissect.cstruct.types import Array, Enum, Field, Flag, Pointer, Structure, Union
+from dissect.cstruct.types import ArrayMetaType, Field, MetaType
 
 if TYPE_CHECKING:
     from dissect.cstruct import cstruct
 
 
 class Parser:
     """Base class for definition parsers.
@@ -38,15 +42,15 @@
         cs: An instance of cstruct.
         compiled: Whether structs should be compiled or not.
     """
 
     def __init__(self, cs: cstruct, compiled: bool = True, align: bool = False):
         super().__init__(cs)
 
-        self.compiler = Compiler(self.cstruct) if compiled else None
+        self.compiled = compiled
         self.align = align
         self.TOK = self._tokencollection()
 
     @staticmethod
     def _tokencollection() -> TokenCollection:
         TOK = TokenCollection()
         TOK.add(r"#\[(?P<values>[^\]]+)\](?=\s*)", "CONFIG_FLAG")
@@ -55,15 +59,15 @@
         TOK.add(r"(?:struct|union)(?=\s|{)", "STRUCT")
         TOK.add(
             r"(?P<enumtype>enum|flag)\s+(?P<name>[^\s:{]+)?\s*(:\s"
             r"*(?P<type>[^{]+?)\s*)?\{(?P<values>[^}]+)\}\s*(?=;)",
             "ENUM",
         )
         TOK.add(r"(?<=})\s*(?P<defs>(?:[a-zA-Z0-9_]+\s*,\s*)+[a-zA-Z0-9_]+)\s*(?=;)", "DEFS")
-        TOK.add(r"(?P<name>\*?[a-zA-Z0-9_]+)(?:\s*:\s*(?P<bits>\d+))?(?:\[(?P<count>[^;\n]*)\])?\s*(?=;)", "NAME")
+        TOK.add(r"(?P<name>\**?\s*[a-zA-Z0-9_]+)(?:\s*:\s*(?P<bits>\d+))?(?:\[(?P<count>[^;\n]*)\])?\s*(?=;)", "NAME")
         TOK.add(r"[a-zA-Z_][a-zA-Z0-9_]*", "IDENTIFIER")
         TOK.add(r"[{}]", "BLOCK")
         TOK.add(r"\$(?P<name>[^\s]+) = (?P<value>{[^}]+})\w*[\r\n]+", "LOOKUP")
         TOK.add(r";", "EOL")
         TOK.add(r"\s+", None)
         TOK.add(r".", None)
 
@@ -82,18 +86,19 @@
 
         value = match["value"]
         try:
             value = ast.literal_eval(value)
         except (ValueError, SyntaxError):
             pass
 
-        try:
-            value = Expression(self.cstruct, value).evaluate()
-        except Exception:
-            pass
+        if isinstance(value, str):
+            try:
+                value = Expression(self.cstruct, value).evaluate()
+            except (ExpressionParserError, ExpressionTokenizerError):
+                pass
 
         self.cstruct.consts[match["name"]] = value
 
     def _enum(self, tokens: TokenConsumer) -> None:
         # We cheat with enums because the entire enum is in the token
         etok = tokens.consume()
 
@@ -105,15 +110,15 @@
         nextval = 0
         if enumtype == "flag":
             nextval = 1
 
         values = {}
         for line in d["values"].splitlines():
             for v in line.split(","):
-                key, sep, val = v.partition("=")
+                key, _, val = v.partition("=")
                 key = key.strip()
                 val = val.strip()
                 if not key:
                     continue
                 if not val:
                     val = nextval
                 else:
@@ -126,25 +131,21 @@
                     nextval = val + 1
 
                 values[key] = val
 
         if not d["type"]:
             d["type"] = "uint32"
 
-        enumcls = Enum
-        if enumtype == "flag":
-            enumcls = Flag
-
-        enum = enumcls(self.cstruct, d["name"], self.cstruct.resolve(d["type"]), values)
+        factory = self.cstruct._make_flag if enumtype == "flag" else self.cstruct._make_enum
 
-        if not enum.name:
-            for name, value in enum.values.items():
-                self.cstruct.consts[name] = enum(value)
+        enum = factory(d["name"] or "", self.cstruct.resolve(d["type"]), values)
+        if not enum.__name__:
+            self.cstruct.consts.update(enum.__members__)
         else:
-            self.cstruct.addtype(enum.name, enum)
+            self.cstruct.add_type(enum.__name__, enum)
 
         tokens.eol()
 
     def _typedef(self, tokens: TokenConsumer) -> None:
         tokens.consume()
         type_ = None
 
@@ -154,25 +155,44 @@
             # The register thing is a bit dirty
             # Basically consumes all NAME tokens and
             # registers the struct
             type_ = self._struct(tokens, register=True)
 
         names = self._names(tokens)
         for name in names:
-            self.cstruct.addtype(name, type_)
+            type_, name, bits = self._parse_field_type(type_, name)
+            if bits is not None:
+                raise ParserError(f"line {self._lineno(tokens.previous)}: typedefs cannot have bitfields")
+            self.cstruct.add_type(name, type_)
 
     def _struct(self, tokens: TokenConsumer, register: bool = False) -> None:
         stype = tokens.consume()
 
+        factory = self.cstruct._make_union if stype.value.startswith("union") else self.cstruct._make_struct
+
+        st = None
         names = []
+        registered = False
+
         if tokens.next == self.TOK.IDENTIFIER:
             ident = tokens.consume()
-            names.append(ident.value)
+            if register:
+                # Pre-register an empty struct for self-referencing
+                # We update this instance later with the fields
+                st = factory(ident.value, [], align=self.align)
+                if self.compiled and "nocompile" not in tokens.flags:
+                    st = compiler.compile(st)
+                self.cstruct.add_type(ident.value, st)
+                registered = True
+            else:
+                names.append(ident.value)
 
         if tokens.next == self.TOK.NAME:
+            # As part of a struct field
+            # struct type_name field_name;
             if not len(names):
                 raise ParserError(f"line {self._lineno(tokens.next)}: unexpected anonymous struct")
             return self.cstruct.resolve(names[0])
 
         if tokens.next != self.TOK.BLOCK:
             raise ParserError(f"line {self._lineno(tokens.next)}: expected start of block '{tokens.next}'")
 
@@ -182,38 +202,40 @@
             if tokens.next == self.TOK.BLOCK and tokens.next.value == "}":
                 tokens.consume()
                 break
 
             field = self._parse_field(tokens)
             fields.append(field)
 
+        # All names from here on are from typedef's
         # Parsing names consumes the EOL token
         names.extend(self._names(tokens))
         name = names[0] if names else None
 
-        if stype.value.startswith("union"):
-            class_ = Union
+        if st is None:
+            is_anonymous = False
+            if not name:
+                is_anonymous = True
+                name = self.cstruct._next_anonymous()
+
+            st = factory(name, fields, align=self.align, anonymous=is_anonymous)
+            if self.compiled and "nocompile" not in tokens.flags:
+                st = compiler.compile(st)
         else:
-            class_ = Structure
-        is_anonymous = False
-        if not name:
-            is_anonymous = True
-            name = self.cstruct._next_anonymous()
-
-        st = class_(self.cstruct, name, fields, align=self.align, anonymous=is_anonymous)
-        if self.compiler and "nocompile" not in tokens.flags:
-            st = self.compiler.compile(st)
+            st.__fields__.extend(fields)
+            st.commit()
 
         # This is pretty dirty
         if register:
-            if not names:
+            if not names and not registered:
                 raise ParserError(f"line {self._lineno(stype)}: struct has no name")
 
             for name in names:
-                self.cstruct.addtype(name, st)
+                self.cstruct.add_type(name, st)
+
         tokens.reset_flags()
         return st
 
     def _lookup(self, tokens: TokenConsumer) -> None:
         # Just like enums, we cheat and have the entire lookup in the token
         ltok = tokens.consume()
 
@@ -226,30 +248,36 @@
     def _parse_field(self, tokens: TokenConsumer) -> Field:
         type_ = None
         if tokens.next == self.TOK.IDENTIFIER:
             type_ = self.cstruct.resolve(self._identifier(tokens))
         elif tokens.next == self.TOK.STRUCT:
             type_ = self._struct(tokens)
             if tokens.next != self.TOK.NAME:
-                return Field(type_.name, type_)
+                return Field(type_.__name__, type_)
 
         if tokens.next != self.TOK.NAME:
             raise ParserError(f"line {self._lineno(tokens.next)}: expected name")
         nametok = tokens.consume()
 
+        type_, name, bits = self._parse_field_type(type_, nametok.value)
+
+        tokens.eol()
+        return Field(name.strip(), type_, bits)
+
+    def _parse_field_type(self, type_: MetaType, name: str) -> tuple[MetaType, str, int | None]:
         pattern = self.TOK.patterns[self.TOK.NAME]
         # Dirty trick because the regex expects a ; but we don't want it to be part of the value
-        d = pattern.match(nametok.value + ";").groupdict()
+        d = pattern.match(name + ";").groupdict()
 
         name = d["name"]
         count_expression = d["count"]
 
-        if name.startswith("*"):
+        while name.startswith("*"):
             name = name[1:]
-            type_ = Pointer(self.cstruct, type_)
+            type_ = self.cstruct._make_pointer(type_)
 
         if count_expression is not None:
             # Poor mans multi-dimensional array by abusing the eager regex match of count
             if "][" in count_expression:
                 counts = count_expression.split("][")
             else:
                 counts = [count_expression]
@@ -260,35 +288,34 @@
                 else:
                     count = Expression(self.cstruct, count)
                     try:
                         count = count.evaluate()
                     except Exception:
                         pass
 
-                if isinstance(type_, Array) and count is None:
+                if isinstance(type_, ArrayMetaType) and count is None:
                     raise ParserError("Depth required for multi-dimensional array")
 
-                type_ = Array(self.cstruct, type_, count)
+                type_ = self.cstruct._make_array(type_, count)
 
-        tokens.eol()
-        return Field(name, type_, int(d["bits"]) if d["bits"] else None)
+        return type_, name.strip(), int(d["bits"]) if d["bits"] else None
 
-    def _names(self, tokens: TokenConsumer) -> List[str]:
+    def _names(self, tokens: TokenConsumer) -> list[str]:
         names = []
         while True:
             if tokens.next == self.TOK.EOL:
                 tokens.eol()
                 break
 
             if tokens.next not in (self.TOK.NAME, self.TOK.DEFS):
                 break
 
             ntoken = tokens.consume()
             if ntoken == self.TOK.NAME:
-                names.append(ntoken.value)
+                names.append(ntoken.value.strip())
             elif ntoken == self.TOK.DEFS:
                 for name in ntoken.value.strip().split(","):
                     names.append(name.strip())
 
         return names
 
     @staticmethod
@@ -389,17 +416,17 @@
 
             nextval = 0
             if enumtype == "flag":
                 nextval = 1
 
             values = {}
             for line in d["values"].split("\n"):
-                line, sep, comment = line.partition("//")
+                line, _, _ = line.partition("//")
                 for v in line.split(","):
-                    key, sep, val = v.partition("=")
+                    key, _, val = v.partition("=")
                     key = key.strip()
                     val = val.strip()
                     if not key:
                         continue
                     if not val:
                         val = nextval
                     else:
@@ -412,23 +439,22 @@
                         nextval = val + 1
 
                     values[key] = val
 
             if not d["type"]:
                 d["type"] = "uint32"
 
-            enumcls = Enum
+            factory = self.cstruct._make_enum
             if enumtype == "flag":
-                enumcls = Flag
+                factory = self.cstruct._make_flag
 
-            enum = enumcls(self.cstruct, d["name"], self.cstruct.resolve(d["type"]), values)
-            self.cstruct.addtype(enum.name, enum)
+            enum = factory(d["name"], self.cstruct.resolve(d["type"]), values)
+            self.cstruct.add_type(enum.__name__, enum)
 
     def _structs(self, data: str) -> None:
-        compiler = Compiler(self.cstruct)
         r = re.finditer(
             r"(#(?P<flags>(?:compile))\s+)?"
             r"((?P<typedef>typedef)\s+)?"
             r"(?P<type>[^\s]+)\s+"
             r"(?P<name>[^\s]+)?"
             r"(?P<fields>"
             r"\s*{[^}]+\}(?P<defs>\s+[^;\n]+)?"
@@ -443,29 +469,29 @@
             elif d["defs"]:
                 name = d["defs"].strip().split(",")[0].strip()
             else:
                 raise ParserError("No name for struct")
 
             if d["type"] == "struct":
                 data = self._parse_fields(d["fields"][1:-1].strip())
-                st = Structure(self.cstruct, name, data)
+                st = self.cstruct._make_struct(name, data)
                 if d["flags"] == "compile" or self.compiled:
                     st = compiler.compile(st)
             elif d["typedef"] == "typedef":
                 st = d["type"]
             else:
                 continue
 
             if d["name"]:
-                self.cstruct.addtype(d["name"], st)
+                self.cstruct.add_type(d["name"], st)
 
             if d["defs"]:
                 for td in d["defs"].strip().split(","):
                     td = td.strip()
-                    self.cstruct.addtype(td, st)
+                    self.cstruct.add_type(td, st)
 
     def _parse_fields(self, data: str) -> None:
         fields = re.finditer(
             r"(?P<type>[^\s]+)\s+(?P<name>[^\s\[:]+)(:(?P<bits>\d+))?(\[(?P<count>[^;\n]*)\])?;",
             data,
         )
 
@@ -487,26 +513,26 @@
                 else:
                     count = Expression(self.cstruct, d["count"])
                     try:
                         count = count.evaluate()
                     except Exception:
                         pass
 
-                type_ = Array(self.cstruct, type_, count)
+                type_ = self.cstruct._make_array(type_, count)
 
             if d["name"].startswith("*"):
                 d["name"] = d["name"][1:]
-                type_ = Pointer(self.cstruct, type_)
+                type_ = self.cstruct._make_pointer(type_)
 
             field = Field(d["name"], type_, int(d["bits"]) if d["bits"] else None)
             result.append(field)
 
         return result
 
-    def _lookups(self, data: str, consts: Dict[str, int]) -> None:
+    def _lookups(self, data: str, consts: dict[str, int]) -> None:
         r = re.finditer(r"\$(?P<name>[^\s]+) = ({[^}]+})\w*\n", data)
 
         for t in r:
             d = ast.literal_eval(t.group(2))
             self.cstruct.lookups[t.group(1)] = dict([(self.cstruct.consts[k], v) for k, v in d.items()])
 
     def parse(self, data: str) -> None:
@@ -535,17 +561,17 @@
 
     def __repr__(self):
         return f"<Token.{self.token} value={self.value!r}>"
 
 
 class TokenCollection:
     def __init__(self):
-        self.tokens: List[Token] = []
-        self.lookup: Dict[str, str] = {}
-        self.patterns: Dict[str, re.Pattern] = {}
+        self.tokens: list[Token] = []
+        self.lookup: dict[str, str] = {}
+        self.patterns: dict[str, re.Pattern] = {}
 
     def __getattr__(self, attr: str):
         try:
             return self.lookup[attr]
         except AttributeError:
             pass
 
@@ -557,19 +583,20 @@
         else:
             self.lookup[name] = name
             self.patterns[name] = re.compile(regex)
             self.tokens.append((regex, lambda s, t: Token(name, t, s.match)))
 
 
 class TokenConsumer:
-    def __init__(self, tokens: List[Token]):
+    def __init__(self, tokens: list[Token]):
         self.tokens = tokens
         self.flags = []
+        self.previous = None
 
-    def __contains__(self, token) -> bool:
+    def __contains__(self, token: Token) -> bool:
         return token in self.tokens
 
     def __len__(self) -> int:
         return len(self.tokens)
 
     def __repr__(self) -> str:
         return f"<TokenConsumer next={self.next!r}>"
@@ -578,15 +605,16 @@
     def next(self) -> Token:
         try:
             return self.tokens[0]
         except IndexError:
             return None
 
     def consume(self) -> Token:
-        return self.tokens.pop(0)
+        self.previous = self.tokens.pop(0)
+        return self.previous
 
     def reset_flags(self) -> None:
         self.flags = []
 
     def eol(self) -> None:
         token = self.consume()
         if token.token != "EOL":
```

### Comparing `dissect.cstruct-3.9.dev3/dissect/cstruct/types/chartype.py` & `dissect_cstruct-4.0.dev0/dissect/cstruct/types/char.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,79 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Any, BinaryIO
+from typing import Any, BinaryIO
 
-from dissect.cstruct.types import RawType
+from dissect.cstruct.types.base import EOF, ArrayMetaType, BaseType
 
-if TYPE_CHECKING:
-    from dissect.cstruct import cstruct
 
+class CharArray(bytes, BaseType, metaclass=ArrayMetaType):
+    """Character array type for reading and writing byte strings."""
 
-class CharType(RawType):
-    """Implements a character type that can properly handle strings."""
+    @classmethod
+    def _read(cls, stream: BinaryIO, context: dict[str, Any] = None) -> CharArray:
+        return type.__call__(cls, ArrayMetaType._read(cls, stream, context))
 
-    def __init__(self, cstruct: cstruct):
-        super().__init__(cstruct, "char", size=1, alignment=1)
+    @classmethod
+    def _write(cls, stream: BinaryIO, data: bytes) -> int:
+        if isinstance(data, list) and data and isinstance(data[0], int):
+            data = bytes(data)
 
-    def _read(self, stream: BinaryIO, context: dict[str, Any] = None) -> bytes:
-        return stream.read(1)
+        elif isinstance(data, str):
+            data = data.encode("latin-1")
+
+        if cls.null_terminated:
+            return stream.write(data + b"\x00")
+        return stream.write(data)
+
+    @classmethod
+    def default(cls) -> CharArray:
+        return type.__call__(cls, b"\x00" * (0 if cls.dynamic or cls.null_terminated else cls.num_entries))
+
+
+class Char(bytes, BaseType):
+    """Character type for reading and writing bytes."""
 
-    def _read_array(self, stream: BinaryIO, count: int, context: dict[str, Any] = None) -> bytes:
+    ArrayType = CharArray
+
+    @classmethod
+    def _read(cls, stream: BinaryIO, context: dict[str, Any] = None) -> Char:
+        return cls._read_array(stream, 1, context)
+
+    @classmethod
+    def _read_array(cls, stream: BinaryIO, count: int, context: dict[str, Any] = None) -> Char:
         if count == 0:
-            return b""
+            return type.__call__(cls, b"")
+
+        data = stream.read(-1 if count == EOF else count)
+        if count != EOF and len(data) != count:
+            raise EOFError(f"Read {len(data)} bytes, but expected {count}")
 
-        return stream.read(count)
+        return type.__call__(cls, data)
 
-    def _read_0(self, stream: BinaryIO, context: dict[str, Any] = None) -> bytes:
-        byte_array = []
+    @classmethod
+    def _read_0(cls, stream: BinaryIO, context: dict[str, Any] = None) -> Char:
+        buf = []
         while True:
-            bytes_stream = stream.read(1)
-            if bytes_stream == b"":
-                raise EOFError()
+            byte = stream.read(1)
+            if byte == b"":
+                raise EOFError("Read 0 bytes, but expected 1")
 
-            if bytes_stream == b"\x00":
+            if byte == b"\x00":
                 break
 
-            byte_array.append(bytes_stream)
+            buf.append(byte)
 
-        return b"".join(byte_array)
+        return type.__call__(cls, b"".join(buf))
 
-    def _write(self, stream: BinaryIO, data: bytes) -> int:
+    @classmethod
+    def _write(cls, stream: BinaryIO, data: bytes | int | str) -> int:
         if isinstance(data, int):
             data = chr(data)
 
         if isinstance(data, str):
             data = data.encode("latin-1")
 
         return stream.write(data)
 
-    def _write_array(self, stream: BinaryIO, data: bytes) -> int:
-        return self._write(stream, data)
-
-    def _write_0(self, stream: BinaryIO, data: bytes) -> int:
-        return self._write(stream, data + b"\x00")
-
-    def default(self) -> bytes:
-        return b"\x00"
-
-    def default_array(self, count: int) -> bytes:
-        return b"\x00" * count
+    @classmethod
+    def default(cls) -> Char:
+        return type.__call__(cls, b"\x00")
```

### Comparing `dissect.cstruct-3.9.dev3/dissect/cstruct/types/structure.py` & `dissect_cstruct-4.0.dev0/dissect/cstruct/compiler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,370 +1,418 @@
+# Made in Japan
+
 from __future__ import annotations
 
 import io
-from collections import OrderedDict
-from typing import TYPE_CHECKING, Any, BinaryIO, List
+import logging
+from enum import Enum
+from textwrap import dedent, indent
+from types import MethodType
+from typing import TYPE_CHECKING, Iterator
 
 from dissect.cstruct.bitbuffer import BitBuffer
-from dissect.cstruct.types import BaseType, Enum, Instance
+from dissect.cstruct.types import (
+    Array,
+    ArrayMetaType,
+    Char,
+    CharArray,
+    Flag,
+    Int,
+    MetaType,
+    Packed,
+    Pointer,
+    Structure,
+    Union,
+    Void,
+    Wchar,
+    WcharArray,
+)
+from dissect.cstruct.types.packed import _struct
 
 if TYPE_CHECKING:
-    from dissect.cstruct import cstruct
-
+    from dissect.cstruct.cstruct import cstruct
+    from dissect.cstruct.types.structure import Field
 
-class Field:
-    """Holds a structure field."""
+SUPPORTED_TYPES = (
+    Array,
+    Char,
+    CharArray,
+    Enum,
+    Flag,
+    Int,
+    Packed,
+    Pointer,
+    Structure,
+    Void,
+    Wchar,
+    WcharArray,
+)
 
-    def __init__(self, name: str, type_: BaseType, bits: int = None, offset: int = None):
-        self.name = name
-        self.type = type_
-        self.bits = bits
-        self.offset = offset
-        self.alignment = type_.alignment
-
-    def __repr__(self):
-        bits_str = " : {self.bits}" if self.bits else ""
-        return f"<Field {self.name} {self.type}{bits_str}>"
-
-
-class Structure(BaseType):
-    """Type class for structures."""
-
-    def __init__(
-        self, cstruct: cstruct, name: str, fields: List[Field] = None, align: bool = False, anonymous: bool = False
-    ):
-        super().__init__(cstruct)
-        self.name = name
-        self.size = None
-        self.alignment = None
+log = logging.getLogger(__name__)
 
-        self.lookup = OrderedDict()
-        self.fields = fields
-
-        self.align = align
-        self.anonymous = anonymous
-        self.dynamic = False
+python_compile = compile
 
-        for field in self.fields:
-            self.lookup[field.name] = field
-            if isinstance(field.type, Structure) and field.type.anonymous:
-                self.lookup.update(field.type.lookup)
 
-        self._calc_size_and_offsets()
+def compile(structure: type[Structure]) -> type[Structure]:
+    return Compiler(structure.cs).compile(structure)
 
-    def __len__(self) -> int:
-        if self.dynamic:
-            raise TypeError("Dynamic size")
 
-        if self.size is None:
-            self._calc_size_and_offsets()
+class Compiler:
+    def __init__(self, cs: cstruct):
+        self.cs = cs
 
-        return self.size
+    def compile(self, structure: type[Structure]) -> type[Structure]:
+        if issubclass(structure, Union):
+            return structure
 
-    def __repr__(self) -> str:
-        return f"<Structure {self.name}>"
+        try:
+            structure._read = self.compile_read(structure.__fields__, structure.__name__, structure.__align__)
+            structure.__compiled__ = True
+        except Exception as e:
+            # Silently ignore, we didn't compile unfortunately
+            log.debug("Failed to compile %s", structure, exc_info=e)
 
-    def _calc_size_and_offsets(self) -> None:
-        """Iterate all fields in this structure to calculate the field offsets and total structure size.
+        return structure
 
-        If a structure has a dynamic field, further field offsets will be set to None and self.dynamic
-        will be set to True.
-        """
-        # The current offset, set to None if we become dynamic
-        offset = 0
-        # The current alignment for this structure
-        alignment = 0
-
-        # The current bit field type
-        bits_type = None
-        # The offset of the current bit field, set to None if we become dynamic
-        bits_field_offset = 0
-        # How many bits we have left in the current bit field
-        bits_remaining = 0
+    def compile_read(self, fields: list[Field], name: str | None = None, align: bool = False) -> MethodType:
+        return _ReadSourceGenerator(self.cs, fields, name, align).generate()
 
-        for field in self.fields:
-            if field.offset is not None:
-                # If a field already has an offset, it's leading
-                offset = field.offset
-
-            if self.align and offset is not None:
-                # Round to next alignment
-                offset += -offset & (field.alignment - 1)
-
-            # The alignment of this struct is equal to its largest members' alignment
-            alignment = max(alignment, field.type.alignment)
-
-            if field.bits:
-                field_type = field.type
-
-                if isinstance(field_type, Enum):
-                    field_type = field_type.type
-
-                # Bit fields have special logic
-                if (
-                    # Exhausted a bit field
-                    bits_remaining == 0
-                    # Moved to a bit field of another type, e.g. uint16 f1 : 8, uint32 f2 : 8;
-                    or field_type != bits_type
-                    # Still processing a bit field, but it's at a different offset due to alignment or a manual offset
-                    or (bits_type is not None and offset > bits_field_offset + bits_type.size)
-                ):
-                    # ... if any of this is true, we have to move to the next field
-                    bits_type = field_type
-                    bits_count = bits_type.size * 8
-                    bits_remaining = bits_count
-                    bits_field_offset = offset
-
-                    if offset is not None:
-                        # We're not dynamic, update the structure size and current offset
-                        offset += bits_type.size
 
-                    field.offset = bits_field_offset
+class _ReadSourceGenerator:
+    def __init__(self, cs: cstruct, fields: list[Field], name: str | None = None, align: bool = False):
+        self.cs = cs
+        self.fields = fields
+        self.name = name
+        self.align = align
 
-                bits_remaining -= field.bits
+        self.field_map: dict[str, Field] = {}
+        self._token_id = 0
 
-                if bits_remaining < 0:
-                    raise ValueError("Straddled bit fields are unsupported")
-            else:
-                # Reset bits stuff
-                bits_type = None
-                bits_field_offset = bits_remaining = 0
-
-                field.offset = offset
-
-                if offset is not None:
-                    # We're not dynamic, update the structure size and current offset
-                    try:
-                        field_len = len(field.type)
-                    except TypeError:
-                        # This field is dynamic
-                        offset = None
-                        self.dynamic = True
-                        continue
-
-                    offset += field_len
-
-        if self.align and offset is not None:
-            # Add "tail padding" if we need to align
-            # This bit magic rounds up to the next alignment boundary
-            # E.g. offset = 3; alignment = 8; -offset & (alignment - 1) = 5
-            offset += -offset & (alignment - 1)
-
-        # The structure size is whatever the currently calculated offset is
-        self.size = offset
-        self.alignment = alignment
-
-    def _read(self, stream: BinaryIO, context: dict[str, Any] = None) -> Instance:
-        bit_buffer = BitBuffer(stream, self.cstruct.endian)
-        struct_start = stream.tell()
+    def _map_field(self, field: Field) -> str:
+        token = f"_{self._token_id}"
+        self.field_map[token] = field
+        self._token_id += 1
+        return token
+
+    def generate(self) -> MethodType:
+        source = self.generate_source()
+        symbols = {token: field.type for token, field in self.field_map.items()}
+
+        code = python_compile(source, f"<compiled {self.name or 'anonymous'}._read>", "exec")
+        exec(code, {"BitBuffer": BitBuffer, "_struct": _struct, **symbols}, d := {})
+        obj = d.popitem()[1]
+        obj.__source__ = source
+
+        return classmethod(obj)
+
+    def generate_source(self) -> str:
+        preamble = """
+        r = {}
+        s = {}
+        """
 
-        result = OrderedDict()
-        sizes = {}
-        for field in self.fields:
-            offset = stream.tell()
-            field_type = self.cstruct.resolve(field.type)
+        if any(field.bits for field in self.fields):
+            preamble += "bit_reader = BitBuffer(stream, cls.cs.endian)\n"
 
-            if field.offset and offset != struct_start + field.offset:
-                # Field is at a specific offset, either alligned or added that way
-                offset = struct_start + field.offset
-                stream.seek(offset)
+        read_code = "\n".join(self._generate_fields())
 
-            if self.align and field.offset is None:
-                # Previous field was dynamically sized and we need to align
-                offset += -offset & (field.alignment - 1)
-                stream.seek(offset)
-
-            if field.bits:
-                if isinstance(field_type, Enum):
-                    value = field_type(bit_buffer.read(field_type.type, field.bits))
-                else:
-                    value = bit_buffer.read(field_type, field.bits)
+        outro = """
+        obj = type.__call__(cls, **r)
+        obj._sizes = s
+        obj._values = r
 
-                if field.name:
-                    result[field.name] = value
-                continue
-            else:
-                bit_buffer.reset()
+        return obj
+        """
 
-            value = field_type._read(stream, result)
+        code = indent(dedent(preamble).lstrip() + read_code + dedent(outro), "    ")
 
-            if isinstance(field_type, Structure) and field_type.anonymous:
-                sizes.update(value._sizes)
-                result.update(value._values)
-            else:
-                if field.name:
-                    sizes[field.name] = stream.tell() - offset
-                    result[field.name] = value
+        template = f"def _read(cls, stream, context=None):\n{code}"
+        return template
 
-        if self.align:
-            # Align the stream
-            stream.seek(-stream.tell() & (self.alignment - 1), io.SEEK_CUR)
+    def _generate_fields(self) -> Iterator[str]:
+        current_offset = 0
+        current_block: list[Field] = []
+        prev_was_bits = False
+        prev_bits_type = None
+        bits_remaining = 0
+        bits_rollover = False
 
-        return Instance(self, result, sizes)
+        def flush() -> Iterator[str]:
+            if current_block:
+                if self.align and current_block[0].offset is None:
+                    yield f"stream.seek(-stream.tell() & ({current_block[0].alignment} - 1), {io.SEEK_CUR})"
+
+                yield from self._generate_packed(current_block)
+                current_block[:] = []
+
+        def align_to_field(field: Field) -> Iterator[str]:
+            nonlocal current_offset
+
+            if field.offset is not None and field.offset != current_offset:
+                # If a field has a set offset and it's not the same as the current tracked offset, seek to it
+                yield f"stream.seek({field.offset})"
+                current_offset = field.offset
 
-    def _write(self, stream: BinaryIO, data: Instance) -> int:
-        bit_buffer = BitBuffer(stream, self.cstruct.endian)
-        struct_start = stream.tell()
-        num = 0
+            if self.align and field.offset is None:
+                yield f"stream.seek(-stream.tell() & ({field.alignment} - 1), {io.SEEK_CUR})"
 
         for field in self.fields:
-            bit_field_type = (field.type.type if isinstance(field.type, Enum) else field.type) if field.bits else None
-            # Current field is not a bit field, but previous was
-            # Or, moved to a bit field of another type, e.g. uint16 f1 : 8, uint32 f2 : 8;
-            if (not field.bits and bit_buffer._type is not None) or (
-                bit_buffer._type and bit_buffer._type != bit_field_type
-            ):
-                # Flush the current bit buffer so we can process alignment properly
-                bit_buffer.flush()
+            field_type = self.cs.resolve(field.type)
 
-            offset = stream.tell()
+            if not issubclass(field_type, SUPPORTED_TYPES):
+                raise TypeError(f"Unsupported type for compiler: {field_type}")
 
-            if field.offset and offset < struct_start + field.offset:
-                # Field is at a specific offset, either alligned or added that way
-                stream.write(b"\x00" * (struct_start + field.offset - offset))
-                offset = struct_start + field.offset
+            if prev_was_bits and not field.bits:
+                yield "bit_reader.reset()"
+                prev_was_bits = False
+                bits_remaining = 0
+
+            try:
+                size = len(field_type)
+                is_dynamic = False
+            except TypeError:
+                size = None
+                is_dynamic = True
+
+            # Sub structure
+            if issubclass(field_type, Structure):
+                yield from flush()
+                yield from align_to_field(field)
+                yield from self._generate_structure(field)
+
+            # Array of structures and multi-dimensional arrays
+            elif issubclass(field_type, (Array, CharArray, WcharArray)) and (
+                issubclass(field_type.type, Structure) or isinstance(field_type.type, ArrayMetaType) or is_dynamic
+            ):
+                yield from flush()
+                yield from align_to_field(field)
+                yield from self._generate_array(field)
+
+            # Bit fields
+            elif field.bits:
+                if not prev_was_bits:
+                    prev_bits_type = field.type
+                    prev_was_bits = True
+
+                if bits_remaining == 0 or prev_bits_type != field.type:
+                    bits_remaining = (size * 8) - field.bits
+                    bits_rollover = True
+
+                yield from flush()
+                yield from align_to_field(field)
+                yield from self._generate_bits(field)
 
-            if self.align and field.offset is None:
-                is_bitbuffer_boundary = bit_buffer._type and (
-                    bit_buffer._remaining == 0 or bit_buffer._type != field.type
-                )
-                if not bit_buffer._type or is_bitbuffer_boundary:
-                    # Previous field was dynamically sized and we need to align
-                    align_pad = -offset & (field.alignment - 1)
-                    stream.write(b"\x00" * align_pad)
-                    offset += align_pad
-
-            value = getattr(data, field.name, None)
-            if value is None:
-                value = field.type.default()
-
-            if field.bits:
-                if isinstance(field.type, Enum):
-                    bit_buffer.write(field.type.type, value.value, field.bits)
-                else:
-                    bit_buffer.write(field.type, value, field.bits)
+            # Everything else - basic and composite types (and arrays of them)
             else:
-                if isinstance(field.type, Structure) and field.type.anonymous:
-                    field.type._write(stream, data)
-                else:
-                    field.type._write(stream, value)
-                num += stream.tell() - offset
+                current_block.append(field)
 
-        if bit_buffer._type is not None:
-            bit_buffer.flush()
+            if current_offset is not None and size is not None:
+                if not field.bits or (field.bits and bits_rollover):
+                    current_offset += size
+                    bits_rollover = False
+
+        yield from flush()
 
         if self.align:
-            # Align the stream
-            stream.write(b"\x00" * (-stream.tell() & (self.alignment - 1)))
+            yield f"stream.seek(-stream.tell() & (cls.alignment - 1), {io.SEEK_CUR})"
 
-        return num
+    def _generate_structure(self, field: Field) -> Iterator[str]:
+        template = f"""
+        _s = stream.tell()
+        r["{field.name}"] = {self._map_field(field)}._read(stream, context=r)
+        s["{field.name}"] = stream.tell() - _s
+        """
 
-    def add_field(self, name: str, type_: BaseType, bits: int = None, offset: int = None) -> None:
-        """Add a field to this structure.
+        yield dedent(template)
 
-        Args:
-            name: The field name.
-            type_: The field type.
-            bits: The bit of the field.
-            offset: The field offset.
+    def _generate_array(self, field: Field) -> Iterator[str]:
+        template = f"""
+        _s = stream.tell()
+        r["{field.name}"] = {self._map_field(field)}._read(stream, context=r)
+        s["{field.name}"] = stream.tell() - _s
         """
-        field = Field(name, type_, bits=bits, offset=offset)
-        self.fields.append(field)
-        self.lookup[name] = field
-        if isinstance(field.type, Structure) and field.type.anonymous:
-            self.lookup.update(field.type.lookup)
-        self.size = None
 
-    def default(self) -> Instance:
-        """Create and return an empty Instance from this structure.
+        yield dedent(template)
 
-        Returns:
-            An empty Instance from this structure.
+    def _generate_bits(self, field: Field) -> Iterator[str]:
+        lookup = self._map_field(field)
+        read_type = "_t"
+        field_type = field.type
+        if issubclass(field_type, (Enum, Flag)):
+            read_type += ".type"
+            field_type = field_type.type
+
+        if issubclass(field_type, Char):
+            field_type = field_type.cs.uint8
+            lookup = "cls.cs.uint8"
+
+        template = f"""
+        _t = {lookup}
+        r["{field.name}"] = type.__call__(_t, bit_reader.read({read_type}, {field.bits}))
         """
-        result = OrderedDict()
-        for field in self.fields:
-            if isinstance(field.type, Structure) and field.type.anonymous:
-                result.update(field.type.default()._values)
+
+        yield dedent(template)
+
+    def _generate_packed(self, fields: list[Field]) -> Iterator[str]:
+        info = list(_generate_struct_info(self.cs, fields, self.align))
+        reads = []
+
+        size = 0
+        slice_index = 0
+        for field, count, _ in info:
+            if field is None:
+                # Padding
+                size += count
+                continue
+
+            field_type = self.cs.resolve(field.type)
+            read_type = _get_read_type(self.cs, field_type)
+
+            if issubclass(field_type, (Array, CharArray, WcharArray)):
+                count = field_type.num_entries
+                read_type = _get_read_type(self.cs, field_type.type)
+
+                if issubclass(read_type, (Char, Wchar, Int)):
+                    count *= read_type.size
+                    getter = f"buf[{size}:{size + count}]"
+                else:
+                    getter = f"data[{slice_index}:{slice_index + count}]"
+                    slice_index += count
+            elif issubclass(read_type, (Char, Wchar, Int)):
+                getter = f"buf[{size}:{size + read_type.size}]"
             else:
-                result[field.name] = field.type.default()
+                getter = f"data[{slice_index}]"
+                slice_index += 1
 
-        return Instance(self, result)
+            if issubclass(read_type, (Wchar, Int)):
+                # Types that parse bytes further down to their own type
+                parser_template = "{type}({getter})"
+            else:
+                # All other types can be simply intialized
+                parser_template = "type.__call__({type}, {getter})"
 
-    def show(self, indent: int = 0) -> None:
-        """Pretty print this structure."""
-        if indent == 0:
-            print(f"struct {self.name}")
+            # Create the final reading code
+            if issubclass(field_type, Array):
+                reads.append(f"_t = {self._map_field(field)}")
+                reads.append("_et = _t.type")
+
+                if issubclass(field_type.type, Int):
+                    reads.append(f"_b = {getter}")
+                    item_parser = parser_template.format(type="_et", getter=f"_b[i:i + {field_type.type.size}]")
+                    list_comp = f"[{item_parser} for i in range(0, {count}, {field_type.type.size})]"
+                elif issubclass(field_type.type, Pointer):
+                    item_parser = "_et.__new__(_et, e, stream, r)"
+                    list_comp = f"[{item_parser} for e in {getter}]"
+                else:
+                    item_parser = parser_template.format(type="_et", getter="e")
+                    list_comp = f"[{item_parser} for e in {getter}]"
 
-        for field in self.fields:
-            if field.offset is None:
-                offset = "0x??"
+                parser = f"type.__call__(_t, {list_comp})"
+            elif issubclass(field_type, CharArray):
+                parser = f"type.__call__({self._map_field(field)}, {getter})"
+            elif issubclass(field_type, Pointer):
+                reads.append(f"_pt = {self._map_field(field)}")
+                parser = f"_pt.__new__(_pt, {getter}, stream, r)"
             else:
-                offset = f"0x{field.offset:02x}"
+                parser = parser_template.format(type=self._map_field(field), getter=getter)
 
-            print(f"{' ' * indent}+{offset} {field.name} {field.type}")
+            reads.append(f'r["{field.name}"] = {parser}')
+            reads.append(f's["{field.name}"] = {field_type.size}')
+            reads.append("")  # Generates a newline in the resulting code
 
-            if isinstance(field.type, Structure):
-                field.type.show(indent + 1)
+            size += field_type.size
 
+        fmt = _optimize_struct_fmt(info)
+        if fmt == "x" or (len(fmt) == 2 and fmt[1] == "x"):
+            unpack = ""
+        else:
+            unpack = f'data = _struct(cls.cs.endian, "{fmt}").unpack(buf)\n'
 
-class Union(Structure):
-    """Type class for unions"""
+        template = f"""
+        buf = stream.read({size})
+        if len(buf) != {size}: raise EOFError()
+        {unpack}
+        """
 
-    def __repr__(self) -> str:
-        return f"<Union {self.name}>"
+        yield dedent(template) + "\n".join(reads)
 
-    def _calc_size_and_offsets(self) -> None:
-        size = 0
-        alignment = 0
 
-        for field in self.fields:
-            if field.alignment is None:
-                # If a field already has an alignment, it's leading
-                field.alignment = field.type.alignment
-
-            size = max(len(field.type), size)
-            alignment = max(field.alignment, alignment)
-
-        self.size = size
-        self.alignment = alignment
-
-    def _read(self, stream: BinaryIO, context: dict[str, Any] = None) -> Instance:
-        buf = io.BytesIO(memoryview(stream.read(len(self))))
-        result = OrderedDict()
-        sizes = {}
+def _generate_struct_info(cs: cstruct, fields: list[Field], align: bool = False) -> Iterator[tuple[Field, int, str]]:
+    if not fields:
+        return
+
+    current_offset = fields[0].offset
+    imaginary_offset = 0
+    for field in fields:
+        # We moved -- probably due to alignment
+        if field.offset is not None and (drift := field.offset - current_offset) > 0:
+            yield None, drift, "x"
+            current_offset += drift
+
+        if align and field.offset is None and (drift := -imaginary_offset & (field.alignment - 1)) > 0:
+            # Assume we started at a correctly aligned boundary
+            yield None, drift, "x"
+            imaginary_offset += drift
+
+        count = 1
+        read_type = _get_read_type(cs, field.type)
+
+        # Drop voids
+        if issubclass(read_type, Void):
+            continue
+
+        # Array of more complex types are handled elsewhere
+        if issubclass(read_type, (Array, CharArray, WcharArray)):
+            count = read_type.num_entries
+            read_type = _get_read_type(cs, read_type.type)
+
+        # Take the pack char for Packed
+        if issubclass(read_type, Packed):
+            yield field, count, read_type.packchar
+
+        # Other types are byte based
+        # We don't actually unpack anything here but slice directly out of the buffer
+        elif issubclass(read_type, (Char, Wchar, Int)):
+            yield field, count * read_type.size, "x"
+
+        size = count * read_type.size
+        imaginary_offset += size
+        if current_offset is not None:
+            current_offset += size
+
+
+def _optimize_struct_fmt(info: Iterator[tuple[Field, int, str]]) -> str:
+    chars = []
+
+    current_count = 0
+    current_char = None
+
+    for _, count, char in info:
+        if current_char is None:
+            current_count = count
+            current_char = char
+            continue
+
+        if char != current_char:
+            if current_count:
+                chars.append((current_count, current_char))
+            current_count = count
+            current_char = char
+        else:
+            current_count += count
 
-        for field in self.fields:
-            start = 0
-            buf.seek(0)
-            field_type = self.cstruct.resolve(field.type)
-
-            if field.offset:
-                buf.seek(field.offset)
-                start = field.offset
-
-            v = field_type._read(buf, result)
-
-            if isinstance(field_type, Structure) and field_type.anonymous:
-                sizes.update(v._sizes)
-                result.update(v._values)
-            else:
-                sizes[field.name] = buf.tell() - start
-                result[field.name] = v
+    if current_char is not None and current_count:
+        chars.append((current_count, current_char))
 
-        return Instance(self, result, sizes)
+    return "".join(f"{count if count > 1 else ''}{char}" for count, char in chars)
 
-    def _write(self, stream: BinaryIO, data: Instance) -> Instance:
-        offset = stream.tell()
 
-        # Find the largest field
-        field = max(self.fields, key=lambda e: len(e.type))
+def _get_read_type(cs: cstruct, type_: MetaType | str) -> MetaType:
+    type_ = cs.resolve(type_)
 
-        # Write the value to the stream using the largest field type
-        if isinstance(field.type, Structure) and field.type.anonymous:
-            field.type._write(stream, data)
-        else:
-            field.type._write(stream, getattr(data, field.name))
+    if issubclass(type_, (Enum, Flag)):
+        type_ = type_.type
 
-        return stream.tell() - offset
+    if issubclass(type_, Pointer):
+        type_ = cs.pointer
 
-    def show(self, indent: int = 0) -> None:
-        raise NotImplementedError()
+    return cs.resolve(type_)
```

### Comparing `dissect.cstruct-3.9.dev3/dissect/cstruct/utils.py` & `dissect_cstruct-4.0.dev0/dissect/cstruct/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from __future__ import annotations
+
 import pprint
 import string
-from typing import List, Tuple
+import sys
+from typing import Iterator
 
-from dissect.cstruct.types import Instance, Structure
+from dissect.cstruct.types.structure import Structure
 
 COLOR_RED = "\033[1;31m"
 COLOR_GREEN = "\033[1;32m"
 COLOR_YELLOW = "\033[1;33m"
 COLOR_BLUE = "\033[1;34m"
 COLOR_PURPLE = "\033[1;35m"
 COLOR_CYAN = "\033[1;36m"
@@ -20,24 +23,26 @@
 COLOR_BG_PURPLE = "\033[1;45m\033[1;37m"
 COLOR_BG_CYAN = "\033[1;46m\033[1;37m"
 COLOR_BG_WHITE = "\033[1;47m\033[1;30m"
 
 PRINTABLE = string.digits + string.ascii_letters + string.punctuation + " "
 
 ENDIANNESS_MAP = {
-    "network": "big",
+    "@": sys.byteorder,
+    "=": sys.byteorder,
     "<": "little",
     ">": "big",
     "!": "big",
+    "network": "big",
 }
 
-Palette = List[Tuple[str, str]]
+Palette = list[tuple[str, str]]
 
 
-def _hexdump(data: bytes, palette: Palette = None, offset: int = 0, prefix: str = ""):
+def _hexdump(data: bytes, palette: Palette | None = None, offset: int = 0, prefix: str = "") -> Iterator[str]:
     """Hexdump some data.
 
     Args:
         data: Bytes to hexdump.
         offset: Byte offset of the hexdump.
         prefix: Optional prefix.
         palette: Colorize the hexdump using this color pattern.
@@ -51,14 +56,21 @@
     for i in range(0, len(data), 16):
         values = ""
         chars = []
 
         for j in range(16):
             if not active and palette:
                 remaining, active = palette.pop()
+                while remaining == 0:
+                    if len(palette) == 0:
+                        # Last palette tuple is empty: print remaining whitespaces
+                        active = ""
+                        break
+                    else:
+                        remaining, active = palette.pop()
                 values += active
             elif active and j == 0:
                 values += active
 
             if i + j >= len(data):
                 values += "  "
             else:
@@ -89,15 +101,17 @@
             if j == 7:
                 values += " "
 
         chars = "".join(chars)
         yield f"{prefix}{offset + i:08x}  {values:48s}  {chars}"
 
 
-def hexdump(data: bytes, palette=None, offset: int = 0, prefix: str = "", output: str = "print"):
+def hexdump(
+    data: bytes, palette: Palette | None = None, offset: int = 0, prefix: str = "", output: str = "print"
+) -> Iterator[str] | str | None:
     """Hexdump some data.
 
     Args:
         data: Bytes to hexdump.
         palette: Colorize the hexdump using this color pattern.
         offset: Byte offset of the hexdump.
         prefix: Optional prefix.
@@ -112,40 +126,42 @@
         return "\n".join(list(generator))
     else:
         raise ValueError(f"Invalid output argument: {output!r} (should be 'print', 'generator' or 'string').")
 
 
 def _dumpstruct(
     structure: Structure,
-    instance: Instance,
     data: bytes,
     offset: int,
     color: bool,
     output: str,
-):
+) -> str | None:
     palette = []
     colors = [
         (COLOR_RED, COLOR_BG_RED),
         (COLOR_GREEN, COLOR_BG_GREEN),
         (COLOR_YELLOW, COLOR_BG_YELLOW),
         (COLOR_BLUE, COLOR_BG_BLUE),
         (COLOR_PURPLE, COLOR_BG_PURPLE),
         (COLOR_CYAN, COLOR_BG_CYAN),
         (COLOR_WHITE, COLOR_BG_WHITE),
     ]
     ci = 0
-    out = [f"struct {structure.name}:"]
+    out = [f"struct {structure.__class__.__name__}:"]
     foreground, background = None, None
-    for field in instance._type.fields:
+    for field in structure.__class__.__fields__:
+        if getattr(field.type, "anonymous", False):
+            continue
+
         if color:
             foreground, background = colors[ci % len(colors)]
-            palette.append((instance._size(field.name), background))
+            palette.append((structure._sizes[field.name], background))
         ci += 1
 
-        value = getattr(instance, field.name)
+        value = getattr(structure, field.name)
         if isinstance(value, str):
             value = repr(value)
         elif isinstance(value, int):
             value = hex(value)
         elif isinstance(value, list):
             value = pprint.pformat(value)
             if "\n" in value:
@@ -163,32 +179,38 @@
         hexdump(data, palette, offset=offset)
         print()
         print(out)
     elif output == "string":
         return "\n".join(["", hexdump(data, palette, offset=offset, output="string"), "", out])
 
 
-def dumpstruct(obj, data: bytes = None, offset: int = 0, color: bool = True, output: str = "print"):
+def dumpstruct(
+    obj: Structure | type[Structure],
+    data: bytes | None = None,
+    offset: int = 0,
+    color: bool = True,
+    output: str = "print",
+) -> str | None:
     """Dump a structure or parsed structure instance.
 
     Prints a colorized hexdump and parsed structure output.
 
     Args:
-        obj: Structure or Instance to dump.
-        data: Bytes to parse the Structure on, if obj is not a parsed Instance.
+        obj: Structure to dump.
+        data: Bytes to parse the Structure on, if obj is not a parsed Structure already.
         offset: Byte offset of the hexdump.
         output: Output format, can be 'print' or 'string'.
     """
     if output not in ("print", "string"):
         raise ValueError(f"Invalid output argument: {output!r} (should be 'print' or 'string').")
 
-    if isinstance(obj, Instance):
-        return _dumpstruct(obj._type, obj, obj.dumps(), offset, color, output)
-    elif isinstance(obj, Structure) and data:
-        return _dumpstruct(obj, obj(data), data, offset, color, output)
+    if isinstance(obj, Structure):
+        return _dumpstruct(obj, obj.dumps(), offset, color, output)
+    elif issubclass(obj, Structure) and data:
+        return _dumpstruct(obj(data), data, offset, color, output)
     else:
         raise ValueError("Invalid arguments")
 
 
 def pack(value: int, size: int = None, endian: str = "little") -> bytes:
     """Pack an integer value to a given bit size, endianness.
```

### Comparing `dissect.cstruct-3.9.dev3/dissect.cstruct.egg-info/PKG-INFO` & `dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 3.9.dev3
+Version: 4.0.dev0
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
@@ -220,15 +220,15 @@
 assert a.dumps() == d
 ```
 
 ### Enums
 The API to access enum members and their values is similar to that of the native Enum type in Python 3. Functionally, it's best comparable to the IntEnum type.
 
 ### Custom types
-You can implement your own types by subclassing `BaseType` or `RawType`, and adding them to your cstruct instance with `addtype(name, type)`
+You can implement your own types by subclassing `BaseType` or `RawType`, and adding them to your cstruct instance with `add_type(name, type)`
 
 ### Custom definition parsers
 Don't like the C-like definition syntax? Write your own syntax parser!
 
 ## Copyright and license
 
 Dissect is released as open source by Fox-IT (<https://www.fox-it.com>) part of NCC Group Plc
```

### Comparing `dissect.cstruct-3.9.dev3/dissect.cstruct.egg-info/SOURCES.txt` & `dissect_cstruct-4.0.dev0/dissect.cstruct.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -14,44 +14,51 @@
 dissect/cstruct/cstruct.py
 dissect/cstruct/exceptions.py
 dissect/cstruct/expression.py
 dissect/cstruct/parser.py
 dissect/cstruct/utils.py
 dissect/cstruct/types/__init__.py
 dissect/cstruct/types/base.py
-dissect/cstruct/types/bytesinteger.py
-dissect/cstruct/types/chartype.py
+dissect/cstruct/types/char.py
 dissect/cstruct/types/enum.py
 dissect/cstruct/types/flag.py
-dissect/cstruct/types/instance.py
-dissect/cstruct/types/packedtype.py
+dissect/cstruct/types/int.py
+dissect/cstruct/types/leb128.py
+dissect/cstruct/types/packed.py
 dissect/cstruct/types/pointer.py
 dissect/cstruct/types/structure.py
-dissect/cstruct/types/voidtype.py
-dissect/cstruct/types/wchartype.py
+dissect/cstruct/types/void.py
+dissect/cstruct/types/wchar.py
 examples/disk.py
 examples/mirai.py
 examples/pe.py
+examples/protobuf.py
 examples/secdesc.py
 tests/__init__.py
 tests/conftest.py
 tests/test_align.py
 tests/test_basic.py
 tests/test_bitbuffer.py
 tests/test_bitfield.py
-tests/test_bytesinteger.py
-tests/test_ctypes_type.py
-tests/test_enum.py
+tests/test_compiler.py
+tests/test_ctypes.py
 tests/test_expression.py
-tests/test_flag.py
-tests/test_packedtype.py
 tests/test_parser.py
-tests/test_pointer.py
-tests/test_struct.py
-tests/test_union.py
-tests/test_util.py
+tests/test_types_base.py
+tests/test_types_char.py
+tests/test_types_custom.py
+tests/test_types_enum.py
+tests/test_types_flag.py
+tests/test_types_int.py
+tests/test_types_leb128.py
+tests/test_types_packed.py
+tests/test_types_pointer.py
+tests/test_types_structure.py
+tests/test_types_union.py
+tests/test_types_void.py
+tests/test_types_wchar.py
 tests/test_utils.py
 tests/utils.py
 tests/data/testdef.txt
 tests/docs/Makefile
 tests/docs/conf.py
 tests/docs/index.rst
```

### Comparing `dissect.cstruct-3.9.dev3/examples/disk.py` & `dissect_cstruct-4.0.dev0/examples/disk.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev3/examples/mirai.py` & `dissect_cstruct-4.0.dev0/examples/mirai.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev3/examples/pe.py` & `dissect_cstruct-4.0.dev0/examples/pe.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev3/examples/secdesc.py` & `dissect_cstruct-4.0.dev0/examples/secdesc.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,16 +48,16 @@
     uint16  Mask;
     LDAP_SID Sid;
 };
 
 struct ACCESS_ALLOWED_OBJECT_ACE {
     uint32  Mask;
     uint32  Flags;
-    char    ObjectType[Flags & 1 * 16];
-    char    InheritedObjectType[Flags & 2 * 8];
+    char    ObjectType[(Flags & 1) * 16];
+    char    InheritedObjectType[(Flags & 2) * 8];
     LDAP_SID Sid;
 };
 """
 c_secd = cstruct()
 c_secd.load(cdef, compiled=True)
 
 
@@ -93,20 +93,17 @@
         if fh:
             self.fh = fh
             self.ldap_sid = c_secd.LDAP_SID(fh)
         else:
             self.ldap_sid = in_obj
 
     def __repr__(self):
-        return "S-{}-{}-{}".format(
-            self.ldap_sid.Revision,
-            bytearray(self.ldap_sid.IdentifierAuthority.Value)[5],
-            "-".join(["{}".format(v) for v in self.ldap_sid.SubAuthority]),
-        )
-
+        authority = bytearray(self.ldap_sid.IdentifierAuthority.Value)[5]
+        sub_authority = "-".join(f"{v}" for v in self.ldap_sid.SubAuthority)
+        return f"S-{self.ldap_sid.Revision}-{authority}-{sub_authority}"
 
 class ACL:
     def __init__(self, fh):
         self.fh = fh
         self.acl = c_secd.ACL(fh)
         self.aces = []
```

### Comparing `dissect.cstruct-3.9.dev3/pyproject.toml` & `dissect_cstruct-4.0.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -42,8 +42,7 @@
 [tool.setuptools]
 license-files = ["LICENSE", "COPYRIGHT"]
 
 [tool.setuptools.packages.find]
 include = ["dissect.*"]
 
 [tool.setuptools_scm]
-local_scheme = "no-local-version"
```

### Comparing `dissect.cstruct-3.9.dev3/tests/docs/Makefile` & `dissect_cstruct-4.0.dev0/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev3/tests/docs/conf.py` & `dissect_cstruct-4.0.dev0/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev3/tests/test_align.py` & `dissect_cstruct-4.0.dev0/tests/test_align.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,182 +1,201 @@
 from io import BytesIO
 
-from dissect import cstruct
+from dissect.cstruct import cstruct
+from tests.utils import verify_compiled
 
 
-def test_align_struct():
-    d = """
+def test_align_struct(cs: cstruct, compiled: bool) -> None:
+    cdef = """
     struct test {
         uint32  a;  // 0x00
         uint64  b;  // 0x08
         uint16  c;  // 0x10
         uint32  d;  // 0x14
         uint8   e;  // 0x18
         uint16  f;  // 0x1a
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.load(cdef, compiled=compiled, align=True)
 
-    fields = c.test.fields
-    assert c.test.align
-    assert c.test.alignment == 8
-    assert c.test.size == 32
+    assert verify_compiled(cs.test, compiled)
+
+    fields = cs.test.__fields__
+    assert cs.test.__align__
+    assert cs.test.alignment == 8
+    assert cs.test.size == 32
     assert fields[0].offset == 0x00
     assert fields[1].offset == 0x08
     assert fields[2].offset == 0x10
     assert fields[3].offset == 0x14
     assert fields[4].offset == 0x18
     assert fields[5].offset == 0x1A
 
     buf = """
         00 00 00 00 00 00 00 00  08 00 00 00 00 00 00 00
         10 00 00 00 14 00 00 00  18 00 1a 00 00 00 00 00
     """
     buf = bytes.fromhex(buf)
     fh = BytesIO(buf)
 
-    obj = c.test(fh)
+    obj = cs.test(fh)
     assert fh.tell() == 32
 
     for name, value in obj._values.items():
-        assert c.test.lookup[name].offset == value
+        assert cs.test.fields[name].offset == value
 
     assert obj.dumps() == buf
 
 
-def test_align_union():
-    d = """
+def test_align_union(cs: cstruct) -> None:
+    cdef = """
     union test {
         uint32  a;
         uint64  b;
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.load(cdef, align=True)
 
-    assert c.test.align
-    assert c.test.alignment == 8
-    assert c.test.size == 8
+    assert cs.test.__align__
+    assert cs.test.alignment == 8
+    assert cs.test.size == 8
 
     buf = """
         00 00 00 01 00 00 00 02
     """
     buf = bytes.fromhex(buf)
     fh = BytesIO(buf)
 
-    obj = c.test(fh)
+    obj = cs.test(fh)
     assert fh.tell() == 8
     assert obj.a == 0x01000000
     assert obj.b == 0x0200000001000000
 
     assert obj.dumps() == buf
 
 
-def test_align_array():
-    d = """
+def test_align_union_tail(cs: cstruct) -> None:
+    cdef = """
+    union test {
+        uint64 a;
+        uint32 b[3];
+    };
+    """
+    cs.load(cdef, align=True)
+
+    assert cs.test.__align__
+    assert cs.test.alignment == 8
+    assert cs.test.size == 16
+
+
+def test_align_array(cs: cstruct, compiled: bool) -> None:
+    cdef = """
     struct test {
         uint32  a;      // 0x00
         uint64  b[4];   // 0x08
         uint16  c;      // 0x28
         uint32  d[2];   // 0x2c
         uint64  e;      // 0x38
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.load(cdef, compiled=compiled, align=True)
 
-    fields = c.test.fields
-    assert c.test.align
-    assert c.test.alignment == 8
-    assert c.test.size == 64
+    assert verify_compiled(cs.test, compiled)
+
+    fields = cs.test.__fields__
+    assert cs.test.__align__
+    assert cs.test.alignment == 8
+    assert cs.test.size == 64
     assert fields[0].offset == 0x00
     assert fields[1].offset == 0x08
     assert fields[2].offset == 0x28
     assert fields[3].offset == 0x2C
     assert fields[4].offset == 0x38
 
     buf = """
         00 00 00 00 00 00 00 00  08 00 00 00 00 00 00 00
         10 00 00 00 00 00 00 00  18 00 00 00 00 00 00 00
         20 00 00 00 00 00 00 00  28 00 00 00 2c 00 00 00
         30 00 00 00 00 00 00 00  38 00 00 00 00 00 00 00
     """
     buf = bytes.fromhex(buf)
 
-    obj = c.test(buf)
+    obj = cs.test(buf)
 
     assert obj.a == 0x00
     assert obj.b == [0x08, 0x10, 0x18, 0x20]
     assert obj.c == 0x28
     assert obj.d == [0x2C, 0x30]
     assert obj.e == 0x38
 
     assert obj.dumps() == buf
 
 
-def test_align_struct_array():
-    d = """
+def test_align_struct_array(cs: cstruct, compiled: bool) -> None:
+    cdef = """
     struct test {
         uint32  a;      // 0x00
         uint64  b;      // 0x08
     };
 
     struct array {
         test    a[4];
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.load(cdef, compiled=compiled, align=True)
+
+    assert verify_compiled(cs.test, compiled)
+    assert verify_compiled(cs.array, compiled)
 
-    fields = c.test.fields
-    assert c.test.align
-    assert c.test.alignment == 8
-    assert c.test.size == 16
+    fields = cs.test.__fields__
+    assert cs.test.__align__
+    assert cs.test.alignment == 8
+    assert cs.test.size == 16
     assert fields[0].offset == 0x00
     assert fields[1].offset == 0x08
 
     buf = """
         00 00 00 00 00 00 00 00  08 00 00 00 00 00 00 00
         10 00 00 00 00 00 00 00  18 00 00 00 00 00 00 00
         20 00 00 00 00 00 00 00  28 00 00 00 00 00 00 00
         30 00 00 00 00 00 00 00  38 00 00 00 00 00 00 00
     """
     buf = bytes.fromhex(buf)
 
-    obj = c.array(buf)
+    obj = cs.array(buf)
 
     assert obj.a[0].a == 0x00
     assert obj.a[0].b == 0x08
     assert obj.a[1].a == 0x10
     assert obj.a[1].b == 0x18
     assert obj.a[2].a == 0x20
     assert obj.a[2].b == 0x28
     assert obj.a[3].a == 0x30
     assert obj.a[3].b == 0x38
 
     assert obj.dumps() == buf
 
 
-def test_align_dynamic():
-    d = """
+def test_align_dynamic(cs: cstruct, compiled: bool) -> None:
+    cdef = """
     struct test {
         uint8   a;      // 0x00 (value is 6 in test case)
         uint16  b[a];   // 0x02
         uint32  c;      // 0x?? (0x10 in test case)
         uint64  d;      // 0x?? (0x18 in test case)
         uint8   e;      // 0x?? (0x20, value is 2 in test case)
         uint32  f[e];   // 0x?? (0x24 in test case)
         uint64  g;      // 0x?? (0x30 in test case)
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.load(cdef, compiled=compiled, align=True)
+
+    assert verify_compiled(cs.test, compiled)
 
-    fields = c.test.fields
+    fields = cs.test.__fields__
     assert fields[0].offset == 0
     assert fields[1].offset == 2
     assert fields[2].offset is None
     assert fields[3].offset is None
     assert fields[4].offset is None
     assert fields[5].offset is None
     assert fields[6].offset is None
@@ -184,130 +203,134 @@
     buf = """
         06 00 02 00 04 00 06 00  08 00 0a 00 0c 00 00 00
         10 00 00 00 00 00 00 00  18 00 00 00 00 00 00 00
         02 00 00 00 24 00 00 00  28 00 00 00 00 00 00 00
         30 00 00 00 00 00 00 00
     """
     buf = bytes.fromhex(buf)
-    obj = c.test(buf)
+    obj = cs.test(buf)
 
     assert obj.a == 0x06
     assert obj.b == [0x02, 0x04, 0x06, 0x08, 0x0A, 0x0C]
     assert obj.c == 0x10
     assert obj.d == 0x18
     assert obj.e == 0x02
     assert obj.f == [0x24, 0x28]
     assert obj.g == 0x30
 
     assert obj.dumps() == buf
 
 
-def test_align_nested_struct():
-    d = """
+def test_align_nested_struct(cs: cstruct, compiled: bool) -> None:
+    cdef = """
     struct test {
         uint32  a;      // 0x00
         struct {
             uint64  b;  // 0x08
             uint32  c;  // 0x10
         } nested;
         uint64  d;      // 0x18
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.load(cdef, compiled=compiled, align=True)
 
-    fields = c.test.fields
+    assert verify_compiled(cs.test, compiled)
+
+    fields = cs.test.__fields__
     assert fields[0].offset == 0x00
     assert fields[1].offset == 0x08
     assert fields[2].offset == 0x18
 
     buf = """
         00 00 00 00 00 00 00 00  08 00 00 00 00 00 00 00
         10 00 00 00 00 00 00 00  18 00 00 00 00 00 00 00
     """
     buf = bytes.fromhex(buf)
-    obj = c.test(buf)
+    obj = cs.test(buf)
 
     assert obj.a == 0x00
     assert obj.nested.b == 0x08
     assert obj.nested.c == 0x10
     assert obj.d == 0x18
 
     assert obj.dumps() == buf
 
 
-def test_align_bitfield():
-    d = """
+def test_align_bitfield(cs: cstruct, compiled: bool) -> None:
+    cdef = """
     struct test {
         uint16  a:4;    // 0x00
         uint16  b:4;
         uint64  c:4;    // 0x08
         uint64  d:4;
         uint16  e;      // 0x10
         uint32  f:4;    // 0x14
         uint64  g;      // 0x18
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.load(cdef, compiled=compiled, align=True)
+
+    assert verify_compiled(cs.test, compiled)
 
-    fields = c.test.fields
+    fields = cs.test.__fields__
     assert fields[0].offset == 0x00
     assert fields[1].offset is None
     assert fields[2].offset == 0x08
     assert fields[3].offset is None
     assert fields[4].offset == 0x10
     assert fields[5].offset == 0x14
     assert fields[6].offset == 0x18
 
     buf = """
         12 00 00 00 00 00 00 00  12 00 00 00 00 00 00 00
         10 00 00 00 02 00 00 00  18 00 00 00 00 00 00 00
     """
     buf = bytes.fromhex(buf)
-    obj = c.test(buf)
+    obj = cs.test(buf)
 
     assert obj.a == 0b10
     assert obj.b == 0b01
     assert obj.c == 0b10
     assert obj.d == 0b01
     assert obj.e == 0x10
     assert obj.f == 0b10
     assert obj.g == 0x18
 
     assert obj.dumps() == buf
 
 
-def test_align_pointer():
-    d = """
+def test_align_pointer(cs: cstruct, compiled: bool) -> None:
+    cdef = """
     struct test {
         uint32  a;
         uint32  *b;
         uint16  c;
         uint16  d;
     };
     """
-    c = cstruct.cstruct()
-    c.load(d, align=True)
+    cs.pointer = cs.uint64
+    cs.load(cdef, compiled=compiled, align=True)
+
+    assert verify_compiled(cs.test, compiled)
 
-    fields = c.test.fields
-    assert c.test.align
-    assert c.test.alignment == 8
-    assert c.test.size == 24
+    fields = cs.test.__fields__
+    assert cs.test.__align__
+    assert cs.test.alignment == 8
+    assert cs.test.size == 24
     assert fields[0].offset == 0x00
     assert fields[1].offset == 0x08
     assert fields[2].offset == 0x10
     assert fields[3].offset == 0x12
 
     buf = """
         00 00 00 00 00 00 00 00  18 00 00 00 00 00 00 00
         10 00 12 00 00 00 00 00  18 00 00 00
     """
     buf = bytes.fromhex(buf)
-    obj = c.test(buf)
+    obj = cs.test(buf)
 
     assert obj.a == 0x00
     assert obj.b.dereference() == 0x18
     assert obj.c == 0x10
     assert obj.d == 0x12
 
     assert obj.dumps() == buf[:-4]  # Without pointer value
```

### Comparing `dissect.cstruct-3.9.dev3/tests/test_basic.py` & `dissect_cstruct-4.0.dev0/tests/test_basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,122 +1,77 @@
+from __future__ import annotations
+
 import os
+from io import BytesIO
+from typing import BinaryIO
 
 import pytest
-from dissect import cstruct
 
+from dissect.cstruct.cstruct import cstruct
 from dissect.cstruct.exceptions import ArraySizeError, ParserError, ResolveError
+from dissect.cstruct.types import BaseType
 
 from .utils import verify_compiled
 
 
-def test_simple_types():
-    cs = cstruct.cstruct()
-    assert cs.uint32(b"\x01\x00\x00\x00") == 1
-    assert cs.uint32[10](b"A" * 20 + b"B" * 20) == [0x41414141] * 5 + [0x42424242] * 5
-    assert cs.uint32[None](b"A" * 20 + b"\x00" * 4) == [0x41414141] * 5
-
-    with pytest.raises(EOFError):
-        cs.char[None](b"aaa")
-
-    with pytest.raises(EOFError):
-        cs.wchar[None](b"a\x00a\x00a")
-
-
-def test_write():
-    cs = cstruct.cstruct()
-
-    assert cs.uint32.dumps(1) == b"\x01\x00\x00\x00"
-    assert cs.uint16.dumps(255) == b"\xff\x00"
-    assert cs.int8.dumps(-10) == b"\xf6"
-    assert cs.uint8[4].dumps([1, 2, 3, 4]) == b"\x01\x02\x03\x04"
-    assert cs.uint24.dumps(300) == b"\x2c\x01\x00"
-    assert cs.int24.dumps(-1337) == b"\xc7\xfa\xff"
-    assert cs.uint24[4].dumps([1, 2, 3, 4]) == b"\x01\x00\x00\x02\x00\x00\x03\x00\x00\x04\x00\x00"
-    assert cs.uint24[None].dumps([1, 2]) == b"\x01\x00\x00\x02\x00\x00\x00\x00\x00"
-    assert cs.char.dumps(0x61) == b"a"
-    assert cs.wchar.dumps("lala") == b"l\x00a\x00l\x00a\x00"
-    assert cs.uint32[None].dumps([1]) == b"\x01\x00\x00\x00\x00\x00\x00\x00"
-
-
-def test_write_be():
-    cs = cstruct.cstruct(endian=">")
-
-    assert cs.uint32.dumps(1) == b"\x00\x00\x00\x01"
-    assert cs.uint16.dumps(255) == b"\x00\xff"
-    assert cs.int8.dumps(-10) == b"\xf6"
-    assert cs.uint8[4].dumps([1, 2, 3, 4]) == b"\x01\x02\x03\x04"
-    assert cs.uint24.dumps(300) == b"\x00\x01\x2c"
-    assert cs.int24.dumps(-1337) == b"\xff\xfa\xc7"
-    assert cs.uint24[4].dumps([1, 2, 3, 4]) == b"\x00\x00\x01\x00\x00\x02\x00\x00\x03\x00\x00\x04"
-    assert cs.char.dumps(0x61) == b"a"
-    assert cs.wchar.dumps("lala") == b"\x00l\x00a\x00l\x00a"
-
-
-def test_duplicate_type(compiled):
+def test_duplicate_type(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint32  a;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     with pytest.raises(ValueError):
         cs.load(cdef)
 
 
-def test_load_file(compiled):
+def test_load_file(cs: cstruct, compiled: bool) -> None:
     path = os.path.join(os.path.dirname(__file__), "data/testdef.txt")
 
-    cs = cstruct.cstruct()
     cs.loadfile(path, compiled=compiled)
     assert "test" in cs.typedefs
 
 
-def test_read_type_name():
-    cs = cstruct.cstruct()
+def test_read_type_name(cs: cstruct) -> None:
     cs.read("uint32", b"\x01\x00\x00\x00") == 1
 
 
-def test_type_resolve():
-    cs = cstruct.cstruct()
-
+def test_type_resolve(cs: cstruct) -> None:
     assert cs.resolve("BYTE") == cs.uint8
 
-    with pytest.raises(cstruct.ResolveError) as excinfo:
+    with pytest.raises(ResolveError) as excinfo:
         cs.resolve("fake")
     assert "Unknown type" in str(excinfo.value)
 
-    cs.addtype("ref0", "uint32")
+    cs.add_type("ref0", "uint32")
     for i in range(1, 15):  # Recursion limit is currently 10
-        cs.addtype(f"ref{i}", f"ref{i - 1}")
+        cs.add_type(f"ref{i}", f"ref{i - 1}")
 
-    with pytest.raises(cstruct.ResolveError) as excinfo:
+    with pytest.raises(ResolveError) as excinfo:
         cs.resolve("ref14")
     assert "Recursion limit exceeded" in str(excinfo.value)
 
 
-def test_constants():
+def test_constants(cs: cstruct) -> None:
     cdef = """
     #define a 1
     #define b 0x2
     #define c "test"
     #define d 1 << 1
     """
-    cs = cstruct.cstruct()
     cs.load(cdef)
 
     assert cs.a == 1
     assert cs.b == 2
     assert cs.c == "test"
     assert cs.d == 2
 
 
-def test_duplicate_types():
-    cs = cstruct.cstruct()
+def test_duplicate_types(cs: cstruct) -> None:
     cdef = """
     struct A {
         uint32 a;
     };
     """
     cs.load(cdef)
     assert cs.A
@@ -132,37 +87,35 @@
     assert cs.Test is cs.uint32
 
     with pytest.raises(ValueError) as excinfo:
         cs.load("""typedef uint64 Test;""")
     assert "Duplicate type" in str(excinfo.value)
 
 
-def test_typedef():
+def test_typedef(cs: cstruct) -> None:
     cdef = """
     typedef uint32 test;
     """
-    cs = cstruct.cstruct()
     cs.load(cdef)
 
     assert cs.test == cs.uint32
     assert cs.resolve("test") == cs.uint32
 
 
-def test_lookups(compiled):
+def test_lookups(cs: cstruct, compiled: bool) -> None:
     cdef = """
     #define test_1 1
     #define test_2 2
     $a = {'test_1': 3, 'test_2': 4}
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
     assert cs.lookups["a"] == {1: 3, 2: 4}
 
 
-def test_default_constructors(compiled):
+def test_default_constructors(cs: cstruct, compiled: bool) -> None:
     cdef = """
     enum Enum {
         a = 0,
         b = 1
     };
 
     flag Flag {
@@ -181,15 +134,14 @@
         wchar   t_wchar_array[2];
         Enum    t_enum;
         Enum    t_enum_array[2];
         Flag    t_flag;
         Flag    t_flag_array[2];
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
     obj = cs.test()
     assert obj.t_int == 0
     assert obj.t_int_array == [0, 0]
@@ -202,16 +154,19 @@
     assert obj.t_enum == cs.Enum(0)
     assert obj.t_enum_array == [cs.Enum(0), cs.Enum(0)]
     assert obj.t_flag == cs.Flag(0)
     assert obj.t_flag_array == [cs.Flag(0), cs.Flag(0)]
 
     assert obj.dumps() == b"\x00" * 54
 
+    for name in obj.fields.keys():
+        assert isinstance(getattr(obj, name), BaseType)
 
-def test_default_constructors_dynamic(compiled):
+
+def test_default_constructors_dynamic(cs: cstruct, compiled: bool) -> None:
     cdef = """
     enum Enum {
         a = 0,
         b = 1
     };
     flag Flag {
         a = 0,
@@ -229,102 +184,100 @@
         wchar   t_wchar_array_d[x];
         Enum    t_enum_array_n[];
         Enum    t_enum_array_d[x];
         Flag    t_flag_array_n[];
         Flag    t_flag_array_d[x];
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
+
     assert verify_compiled(cs.test, compiled)
+
     obj = cs.test()
+
     assert obj.t_int_array_n == obj.t_int_array_d == []
     assert obj.t_bytesint_array_n == obj.t_bytesint_array_d == []
     assert obj.t_char_array_n == obj.t_char_array_d == b""
     assert obj.t_wchar_array_n == obj.t_wchar_array_d == ""
     assert obj.t_enum_array_n == obj.t_enum_array_d == []
     assert obj.t_flag_array_n == obj.t_flag_array_d == []
     assert obj.dumps() == b"\x00" * 19
 
+    for name in obj.fields.keys():
+        assert isinstance(getattr(obj, name), BaseType)
 
-def test_config_flag_nocompile(compiled):
+
+def test_config_flag_nocompile(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct compiled_global
     {
         uint32  a;
     };
 
     #[nocompile]
     struct never_compiled
     {
         uint32  a;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.compiled_global, compiled)
     assert verify_compiled(cs.never_compiled, False)
 
 
-def test_compiler_slicing_multiple(compiled):
+def test_compiler_slicing_multiple(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct compile_slicing {
         char single;
         char multiple[2];
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.compile_slicing, compiled)
 
     obj = cs.compile_slicing(b"\x01\x02\x03")
     assert obj.single == b"\x01"
     assert obj.multiple == b"\x02\x03"
 
 
-def test_underscores_attribute(compiled):
+def test_underscores_attribute(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct __test {
         uint32 test_val;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.__test, compiled)
 
     data = b"\x39\x05\x00\x00"
     obj = cs.__test(data)
     assert obj.test_val == 1337
 
 
-def test_half_compiled_struct():
-    from dissect.cstruct import RawType
-
-    class OffByOne(RawType):
-        def __init__(self, cstruct_obj):
-            self._t = cstruct_obj.uint64
-            super().__init__(cstruct_obj, "OffByOne", 8)
-
-        def _read(self, stream, context=None):
-            return self._t._read(stream, context) + 1
-
-        def _write(self, stream, data):
-            return self._t._write(stream, data - 1)
+def test_half_compiled_struct(cs: cstruct) -> None:
+    class OffByOne(int, BaseType):
+        type: BaseType
+
+        @classmethod
+        def _read(cls, stream: BinaryIO, context: dict | None = None) -> OffByOne:
+            return cls(cls.type._read(stream, context) + 1)
+
+        @classmethod
+        def _write(cls, stream: BinaryIO, data: int) -> OffByOne:
+            return cls(cls.type._write(stream, data - 1))
 
-        def default(self):
-            return 0
-
-    cs = cstruct.cstruct()
     # Add an unsupported type for the cstruct compiler
     # so that it returns the original struct,
     # only partially compiling the struct.
-    cs.addtype("offbyone", OffByOne(cs))
+    offbyone = cs._make_type("offbyone", (OffByOne,), 8, attrs={"type": cs.uint64})
+    cs.add_type("offbyone", offbyone)
+
     cdef = """
     struct uncompiled {
         uint32      a;
         offbyone    b;
         uint16      c;
     };
 
@@ -346,147 +299,137 @@
     assert obj.b.b == 3
     assert obj.b.c == 3
     assert obj.c == 4
 
     assert obj.dumps() == buf
 
 
-def test_cstruct_bytearray():
+def test_cstruct_bytearray(cs: cstruct) -> None:
     cdef = """
     struct test {
         uint8 a;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef)
 
     obj = cs.test(bytearray([10]))
     assert obj.a == 10
 
 
-def test_multipart_type_name():
+def test_multipart_type_name(cs: cstruct) -> None:
     cdef = """
     enum TestEnum : unsigned int {
         A = 0,
         B = 1
     };
 
     struct test {
         unsigned int    a;
         unsigned long long  b;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef)
 
     assert cs.TestEnum.type == cs.resolve("unsigned int")
-    assert cs.test.fields[0].type == cs.resolve("unsigned int")
-    assert cs.test.fields[1].type == cs.resolve("unsigned long long")
+    assert cs.test.__fields__[0].type == cs.resolve("unsigned int")
+    assert cs.test.__fields__[1].type == cs.resolve("unsigned long long")
 
     with pytest.raises(ResolveError) as exc:
         cdef = """
-        struct test {
+        struct test1 {
             unsigned long long unsigned a;
         };
         """
-        cs = cstruct.cstruct()
         cs.load(cdef)
 
     with pytest.raises(ResolveError) as exc:
         cdef = """
         enum TestEnum : unsigned int and more {
             A = 0,
             B = 1
         };
         """
-        cs = cstruct.cstruct()
         cs.load(cdef)
 
     assert str(exc.value) == "Unknown type unsigned int and more"
 
 
-def test_dunder_bytes():
+def test_dunder_bytes(cs: cstruct) -> None:
     cdef = """
     struct test {
         DWORD   a;
         QWORD   b;
     };
     """
-    cs = cstruct.cstruct(endian=">")
+    cs.endian = ">"
     cs.load(cdef)
 
     a = cs.test(a=0xBADC0DE, b=0xACCE55ED)
     assert len(bytes(a)) == 12
     assert bytes(a) == a.dumps()
     assert bytes(a) == b"\x0b\xad\xc0\xde\x00\x00\x00\x00\xac\xce\x55\xed"
 
 
-@pytest.mark.parametrize("compiled", [True, False])
-def test_array_of_null_terminated_strings(compiled):
+def test_array_of_null_terminated_strings(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct args {
         uint32 argc;
         char   argv[argc][];
     }
     """
-    cs = cstruct.cstruct(endian="<")
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.args, compiled)
 
     buf = b"\x02\x00\x00\x00hello\0world\0"
     obj = cs.args(buf)
 
     assert obj.argc == 2
     assert obj.argv[0] == b"hello"
     assert obj.argv[1] == b"world"
 
     with pytest.raises(ParserError) as exc:
         cdef = """
-        struct args {
+        struct args2 {
             uint32 argc;
             char   argv[][argc];
         }
         """
         cs.load(cdef)
 
     assert str(exc.value) == "Depth required for multi-dimensional array"
 
 
-@pytest.mark.parametrize("compiled", [True, False])
-def test_array_of_size_limited_strings(compiled):
+def test_array_of_size_limited_strings(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct args {
         uint32 argc;
         char   argv[argc][8];
     }
     """
-    cs = cstruct.cstruct(endian="<")
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.args, compiled)
 
     buf = b"\x04\x00\x00\x00lorem\0\0\0ipsum\0\0\0dolor\0\0\0sit amet"
     obj = cs.args(buf)
 
     assert obj.argc == 4
     assert obj.argv[0] == b"lorem\0\0\0"
     assert obj.argv[1] == b"ipsum\0\0\0"
     assert obj.argv[2] == b"dolor\0\0\0"
     assert obj.argv[3] == b"sit amet"
 
 
-@pytest.mark.parametrize("compiled", [True, False])
-def test_array_three_dimensional(compiled):
+def test_array_three_dimensional(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint8   a[2][2][2];
     }
     """
-    cs = cstruct.cstruct(endian="<")
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
     buf = b"\x01\x02\x03\x04\x05\x06\x07\x08"
     obj = cs.test(buf)
 
@@ -498,25 +441,23 @@
     assert obj.a[1][0][1] == 6
     assert obj.a[1][1][0] == 7
     assert obj.a[1][1][1] == 8
 
     assert obj.dumps() == buf
 
 
-@pytest.mark.parametrize("compiled", [True, False])
-def test_nested_array_of_variable_size(compiled: bool):
+def test_nested_array_of_variable_size(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint8   outer;
         uint8   medior;
         uint8   inner;
         uint8   a[outer][medior][inner];
     }
     """
-    cs = cstruct.cstruct(endian="<")
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
     buf = b"\x02\x01\x03\x01\x02\x03\x04\x05\x06"
     obj = cs.test(buf)
 
@@ -529,20 +470,115 @@
     assert obj.a[1][0][0] == 4
     assert obj.a[1][0][1] == 5
     assert obj.a[1][0][2] == 6
 
     assert obj.dumps() == buf
 
 
-def test_report_array_size_mismatch():
+def test_report_array_size_mismatch(cs: cstruct) -> None:
     cdef = """
     struct test {
         uint8   a[2];
     };
     """
-    cs = cstruct.cstruct(endian=">")
     cs.load(cdef)
 
     a = cs.test(a=[1, 2, 3])
 
     with pytest.raises(ArraySizeError):
         a.dumps()
+
+
+def test_reserved_keyword(cs: cstruct, compiled: bool) -> None:
+    cdef = """
+    struct in {
+        uint8 a;
+    };
+
+    struct class {
+        uint8 a;
+    };
+
+    struct for {
+        uint8 a;
+    };
+    """
+    cs.load(cdef, compiled=compiled)
+
+    for name in ["in", "class", "for"]:
+        assert name in cs.typedefs
+        assert verify_compiled(cs.resolve(name), compiled)
+
+        assert cs.resolve(name)(b"\x01").a == 1
+
+
+def test_array_class_name(cs: cstruct) -> None:
+    cdef = """
+    struct test {
+        uint8   a[2];
+    };
+
+    struct test2 {
+        uint8   a;
+        uint8   b[a + 1];
+    };
+    """
+    cs.load(cdef)
+
+    assert cs.test.__fields__[0].type.__name__ == "uint8[2]"
+    assert cs.test2.__fields__[1].type.__name__ == "uint8[a + 1]"
+
+
+def test_size_and_aligment(cs: cstruct) -> None:
+    test = cs._make_int_type("test", 1, False, alignment=8)
+    assert test.size == 1
+    assert test.alignment == 8
+
+    test = cs._make_packed_type("test", "B", int, alignment=8)
+    assert test.size == 1
+    assert test.alignment == 8
+
+
+def test_dynamic_substruct_size(cs: cstruct) -> None:
+    cdef = """
+    struct {
+        int32 len;
+        char str[len];
+    } sub;
+
+    struct {
+        sub data[1];
+    } test;
+    """
+    cs.load(cdef)
+
+    assert cs.sub.dynamic
+    assert cs.test.dynamic
+
+
+def test_dumps_write_overload(cs: cstruct) -> None:
+    assert cs.uint8.dumps(1) == cs.uint8(1).dumps() == b"\x01"
+
+    fh = BytesIO()
+    cs.uint8.write(fh, 1)
+    assert fh.getvalue() == b"\x01"
+    cs.uint8(2).write(fh)
+    assert fh.getvalue() == b"\x01\x02"
+
+
+def test_linked_list(cs: cstruct) -> None:
+    cdef = """
+    struct node {
+        uint16 data;
+        node* next;
+    };
+    """
+    cs.pointer = cs.uint16
+    cs.load(cdef)
+
+    assert cs.node.__fields__[1].type.type == cs.node
+
+    obj = cs.node(b"\x01\x00\x04\x00\x02\x00\x00\x00")
+    assert repr(obj) == "<node data=0x1 next=<node* @ 0x4>>"
+
+    assert obj.data == 1
+    assert obj.next.data == 2
```

### Comparing `dissect.cstruct-3.9.dev3/tests/test_bitbuffer.py` & `dissect_cstruct-4.0.dev0/tests/test_bitbuffer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 from io import BytesIO
 
 import pytest
-from dissect import cstruct
 
 from dissect.cstruct.bitbuffer import BitBuffer
+from dissect.cstruct.cstruct import cstruct
 
 
-def test_bitbuffer_read():
-    cs = cstruct.cstruct()
-
+def test_bitbuffer_read(cs: cstruct) -> None:
     bb = BitBuffer(BytesIO(b"\xff"), "<")
     assert bb.read(cs.uint8, 8) == 0b11111111
 
     bb = BitBuffer(BytesIO(b"\xf0"), "<")
     assert bb.read(cs.uint8, 4) == 0b0000
     assert bb.read(cs.uint8, 4) == 0b1111
```

### Comparing `dissect.cstruct-3.9.dev3/tests/test_bitfield.py` & `dissect_cstruct-4.0.dev0/tests/test_bitfield.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import pytest
-from dissect import cstruct
+
+from dissect.cstruct.cstruct import cstruct
 
 from .utils import verify_compiled
 
 
-def test_bitfield(compiled):
+def test_bitfield(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a:4;
         uint16  b:4;
         uint16  c:4;
         uint16  d:4;
         uint32  e;
         uint16  f:2;
         uint16  g:3;
         uint32  h;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
     assert len(cs.test) == 12
 
     buf = b"\x12\x34\xff\x00\x00\x00\x1f\x00\x01\x00\x00\x00"
     obj = cs.test(buf)
@@ -33,30 +33,29 @@
     assert obj.e == 0xFF
     assert obj.f == 0b11
     assert obj.g == 0b111
     assert obj.h == 1
     assert obj.dumps() == buf
 
 
-def test_bitfield_consecutive(compiled):
+def test_bitfield_consecutive(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a:4;
         uint16  b:4;
         uint16  c:4;
         uint16  d:4;
         uint16  e:16;
         uint16  _pad1;
         uint16  f:2;
         uint16  g:3;
         uint16  h:11;
         uint16  _pad2;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
     assert len(cs.test) == 10
 
     buf = b"\x12\x34\xff\x00\x00\x00\x1f\x01\x00\x00"
     obj = cs.test(buf)
@@ -68,15 +67,15 @@
     assert obj.e == 0xFF
     assert obj.f == 0b11
     assert obj.g == 0b111
     assert obj.h == 0b1000
     assert obj.dumps() == buf
 
 
-def test_struct_after_bitfield(compiled):
+def test_struct_after_bitfield(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a:4;
         uint16  b:4;
         uint32  c;
         struct {
             uint32 d;
@@ -85,15 +84,14 @@
         uint16  f:4;
         struct {
             uint32 g;
         } nested2;
         uint32  h;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
     assert len(cs.test) == 20
 
     buf = b"\x12\x00\xff\x00\x00\x00\x01\x00\x00\x00\x12\x00\x02\x00\x00\x00\xfe\x00\x00\x00"
     obj = cs.test(buf)
@@ -105,29 +103,29 @@
     assert obj.e == 0b10
     assert obj.f == 0b01
     assert obj.nested2.g == 0x02
     assert obj.h == 0xFE
     assert obj.dumps() == buf
 
 
-def test_bitfield_be(compiled):
+def test_bitfield_be(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a:4;
         uint16  b:4;
         uint16  c:4;
         uint16  d:4;
         uint32  e;
         uint16  f:2;
         uint16  g:3;
         uint16  h:4;
         uint32  i;
     };
     """
-    cs = cstruct.cstruct(endian=">")
+    cs.endian = ">"
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
     assert len(cs.test) == 12
 
     buf = b"\x12\x34\x00\x00\x00\xff\x1f\x00\x00\x00\x00\x01"
     obj = cs.test(buf)
@@ -140,83 +138,81 @@
     assert obj.f == 0
     assert obj.g == 0b11
     assert obj.h == 0b1110
     assert obj.i == 1
     assert obj.dumps() == buf
 
 
-def test_bitfield_straddle(compiled):
+def test_bitfield_straddle(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a:12;
         uint16  b:12;
         uint16  c:8;
         uint32  d;
         uint16  e:2;
         uint16  f:3;
         uint32  g;
     };
     """
-    cs = cstruct.cstruct()
 
     with pytest.raises(ValueError) as exc:
         cs.load(cdef, compiled=compiled)
 
     assert str(exc.value) == "Straddled bit fields are unsupported"
 
 
-def test_bitfield_write(compiled):
+def test_bitfield_write(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a:1;
         uint16  b:1;
         uint32  c;
         uint16  d:2;
         uint16  e:3;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     obj = cs.test()
     obj.a = 0b1
     obj.b = 0b1
     obj.c = 0xFF
     obj.d = 0b11
     obj.e = 0b111
 
     assert obj.dumps() == b"\x03\x00\xff\x00\x00\x00\x1f\x00"
 
 
-def test_bitfield_write_be(compiled):
+def test_bitfield_write_be(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a:1;
         uint16  b:1;
         uint32  c;
         uint16  d:2;
         uint16  e:3;
     };
     """
-    cs = cstruct.cstruct(endian=">")
+    cs.endian = ">"
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
     obj = cs.test()
     obj.a = 0b1
     obj.b = 0b1
     obj.c = 0xFF
     obj.d = 0b11
     obj.e = 0b111
 
     assert obj.dumps() == b"\xc0\x00\x00\x00\x00\xff\xf8\x00"
 
 
-def test_bitfield_with_enum_or_flag(compiled):
+def test_bitfield_with_enum_or_flag(cs: cstruct, compiled: bool) -> None:
     cdef = """
     flag Flag8 : uint8 {
         A = 1,
         B = 2
     };
 
     flag Flag16 : uint16 {
@@ -227,15 +223,15 @@
     struct test {
         uint16  a:1;
         uint16  b:1;
         Flag16  c:2;
         Flag8   d:4;
     };
     """
-    cs = cstruct.cstruct(endian=">")
+    cs.endian = ">"
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
     buf = b"\xf0\x00\x30"
     obj = cs.test(buf)
 
@@ -243,25 +239,23 @@
     assert obj.b == 0b1
     assert obj.c == cs.Flag16.A | cs.Flag16.B
     assert obj.d == cs.Flag8.A | cs.Flag8.B
 
     assert obj.dumps() == buf
 
 
-def test_bitfield_char(compiled):
+def test_bitfield_char(cs: cstruct, compiled: bool) -> None:
     cdef = """
     struct test {
         uint16  a : 4;
         uint16  b : 4;
         char    c : 8;
         char    d[4];
     };
     """
-
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
     buf = b"\x12\x00\xff\x69420"
     obj = cs.test(buf)
```

### Comparing `dissect.cstruct-3.9.dev3/tests/test_ctypes_type.py` & `dissect_cstruct-4.0.dev0/tests/test_ctypes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import ctypes as _ctypes
+from typing import Any
 
 import pytest
-from dissect import cstruct
 
-DUMMY_CSTRUCT = cstruct.cstruct()
-PACKED_TYPE_INT8 = cstruct.PackedType(DUMMY_CSTRUCT, "int8", 1, "b")
+from dissect.cstruct import MetaType, cstruct, ctypes_type
+
+DUMMY_CSTRUCT = cstruct()
+
+
+# TODO: test structure/union
 
 
 @pytest.mark.parametrize(
-    "cstruct_type, ctypes_type",
+    "input, expected",
     [
-        (PACKED_TYPE_INT8, _ctypes.c_int8),
-        (cstruct.CharType(DUMMY_CSTRUCT), _ctypes.c_char),
-        (cstruct.Array(DUMMY_CSTRUCT, PACKED_TYPE_INT8, 3), _ctypes.c_int8 * 3),
-        (cstruct.Pointer(DUMMY_CSTRUCT, PACKED_TYPE_INT8), _ctypes.POINTER(_ctypes.c_int8)),
+        (DUMMY_CSTRUCT.int8, _ctypes.c_int8),
+        (DUMMY_CSTRUCT.char, _ctypes.c_char),
+        (DUMMY_CSTRUCT.char[3], _ctypes.c_char * 3),
+        (DUMMY_CSTRUCT.int8[3], _ctypes.c_int8 * 3),
+        (DUMMY_CSTRUCT._make_pointer(DUMMY_CSTRUCT.int8), _ctypes.POINTER(_ctypes.c_int8)),
     ],
 )
-def test_ctypes_type(cstruct_type, ctypes_type):
-    assert ctypes_type == cstruct.ctypes_type(cstruct_type)
+def test_ctypes_type(input: MetaType, expected: Any) -> None:
+    assert expected == ctypes_type(input)
 
 
-def test_ctypes_type_exception():
+def test_ctypes_type_exception() -> None:
     with pytest.raises(NotImplementedError):
-        cstruct.ctypes_type("FAIL")
+        ctypes_type(DUMMY_CSTRUCT.float16)
```

### Comparing `dissect.cstruct-3.9.dev3/tests/test_enum.py` & `dissect_cstruct-4.0.dev0/tests/test_types_flag.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,278 +1,235 @@
+from enum import Flag as StdFlag
+
 import pytest
-from dissect import cstruct
+
+from dissect.cstruct.cstruct import cstruct
+from dissect.cstruct.types.enum import PY_311
+from dissect.cstruct.types.flag import Flag
 
 from .utils import verify_compiled
 
 
-def test_enum(compiled):
-    cdef = """
-    enum Test16 : uint16 {
-        A = 0x1,
-        B = 0x2
-    };
+@pytest.fixture
+def TestFlag(cs: cstruct) -> type[Flag]:
+    return cs._make_flag("Test", cs.uint8, {"A": 1, "B": 2})
 
-    enum Test24 : uint24 {
-        A = 0x1,    // comment, best one
-        B = 0x2
-    };
 
-    enum Test32 : uint32 {
-        A = 0x1,
-        B = 0x2     // comment
-    };
+def test_flag(cs: cstruct, TestFlag: type[Flag]) -> None:
+    assert issubclass(TestFlag, StdFlag)
+    assert TestFlag.cs is cs
+    assert TestFlag.type is cs.uint8
+    assert TestFlag.size == 1
+    assert TestFlag.alignment == 1
 
-    struct test {
-        Test16  a16;
-        Test16  b16;
-        Test24  a24;
-        Test24  b24;
-        Test32  a32;
-        Test32  b32;        // this is a comment, awesome
-        Test16  l[2];
-    };
+    assert TestFlag.A == 1
+    assert TestFlag.B == 2
+    assert TestFlag(1) == TestFlag.A
+    assert TestFlag(2) == TestFlag.B
 
-    struct test_term {
-        Test16  null[];
-    };
+    assert TestFlag(0) == 0
+    assert TestFlag(0).name is None
+    assert TestFlag(0).value == 0
 
-    struct test_expr {
-        uint16  size;
-        Test16  expr[size * 2];
-    };
-    """
-    cs = cstruct.cstruct()
-    cs.load(cdef, compiled=compiled)
 
-    assert verify_compiled(cs.test, compiled)
-    assert verify_compiled(cs.test_term, compiled)
-    assert verify_compiled(cs.test_expr, compiled)
+def test_flag_read(TestFlag: type[Flag]) -> None:
+    assert TestFlag(b"\x02") == TestFlag.B
 
-    buf = b"\x01\x00\x02\x00\x01\x00\x00\x02\x00\x00\x01\x00\x00\x00\x02\x00\x00\x00\x01\x00\x02\x00"
-    obj = cs.test(buf)
 
-    assert obj.a16.enum == cs.Test16 and obj.a16 == cs.Test16.A
-    assert obj.b16.enum == cs.Test16 and obj.b16 == cs.Test16.B
-    assert obj.a24.enum == cs.Test24 and obj.a24 == cs.Test24.A
-    assert obj.b24.enum == cs.Test24 and obj.b24 == cs.Test24.B
-    assert obj.a32.enum == cs.Test32 and obj.a32 == cs.Test32.A
-    assert obj.b32.enum == cs.Test32 and obj.b32 == cs.Test32.B
+def test_flag_write(TestFlag: type[Flag]) -> None:
+    assert TestFlag.A.dumps() == b"\x01"
+    assert TestFlag(b"\x02").dumps() == b"\x02"
 
-    assert len(obj.l) == 2
-    assert obj.l[0].enum == cs.Test16 and obj.l[0] == cs.Test16.A
-    assert obj.l[1].enum == cs.Test16 and obj.l[1] == cs.Test16.B
 
-    assert "A" in cs.Test16
-    assert "Foo" not in cs.Test16
-    assert cs.Test16(1) == cs.Test16["A"]
-    assert cs.Test24(2) == cs.Test24.B
-    assert cs.Test16.A != cs.Test24.A
+def test_flag_array_read(TestFlag: type[Flag]) -> None:
+    assert TestFlag[2](b"\x02\x01") == [TestFlag.B, TestFlag.A]
+    assert TestFlag[None](b"\x02\x01\x00") == [TestFlag.B, TestFlag.A]
 
-    with pytest.raises(KeyError):
-        cs.Test16["C"]
 
-    with pytest.raises(AttributeError):
-        cs.Test16.C
+def test_flag_array_write(TestFlag: type[Flag]) -> None:
+    assert TestFlag[2]([TestFlag.B, TestFlag.A]).dumps() == b"\x02\x01"
+    assert TestFlag[None]([TestFlag.B, TestFlag.A]).dumps() == b"\x02\x01\x00"
 
-    assert obj.dumps() == buf
 
-    buf = b"\x01\x00\x02\x00\x00\x00"
-    assert cs.test_term(buf).null == [cs.Test16.A, cs.Test16.B]
-    assert cs.test_term(null=[cs.Test16.A, cs.Test16.B]).dumps() == buf
-
-    buf = b"\x01\x00\x01\x00\x02\x00"
-    assert cs.test_expr(buf).expr == [cs.Test16.A, cs.Test16.B]
-    assert cs.test_expr(size=1, expr=[cs.Test16.A, cs.Test16.B]).dumps() == buf
-
-    obj = {
-        cs.Test16.A: "Test16.A",
-        cs.Test16.B: "Test16.B",
-        cs.Test24.A: "Test24.A",
-        cs.Test24.B: "Test24.B",
-    }
-
-    assert obj[cs.Test16.A] == "Test16.A"
-    assert obj[cs.Test16(2)] == "Test16.B"
-    assert obj[cs.Test24(1)] == "Test24.A"
-    assert obj[cs.Test24.B] == "Test24.B"
+def test_flag_operator(TestFlag: type[Flag]) -> None:
+    assert TestFlag.A | TestFlag.B == 3
+    assert TestFlag(3) == TestFlag.A | TestFlag.B
+    assert isinstance(TestFlag.A | TestFlag.B, TestFlag)
 
-    with pytest.raises(KeyError):
-        obj[cs.Test32.A]
+    assert TestFlag(b"\x03") == TestFlag.A | TestFlag.B
+    assert TestFlag[2](b"\x02\x03") == [TestFlag.B, (TestFlag.A | TestFlag.B)]
 
+    assert (TestFlag.A | TestFlag.B).dumps() == b"\x03"
+    assert TestFlag[2]([TestFlag.B, (TestFlag.A | TestFlag.B)]).dumps() == b"\x02\x03"
 
-def test_enum_comments():
-    cdef = """
-    enum Inline { hello=7, world, foo, bar }; // inline enum
 
-    enum Test {
-        a = 2,  // comment, 2
-        b,      // comment, 3
-        c       // comment, 4
+def test_flag_struct(cs: cstruct) -> None:
+    cdef = """
+    flag Test {
+        a,
+        b,
+        c,
+        d
     };
 
-    enum Odd {
-        a = 0,          // hello, world
-        b,              // next
-        c,              // next
-        d = 5, e, f     // inline, from 5
-        g               // next
+    flag Odd {
+        a = 2,
+        b,
+        c,
+        d = 32, e, f,
+        g
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef)
 
-    assert cs.Inline.hello == 7
-    assert cs.Inline.world == 8
-    assert cs.Inline.foo == 9
-    assert cs.Inline.bar == 10
-
-    assert cs.Test.a == 2
-    assert cs.Test.b == 3
+    assert cs.Test.a == 1
+    assert cs.Test.b == 2
     assert cs.Test.c == 4
+    assert cs.Test.d == 8
 
-    assert cs.Odd.a == 0
-    assert cs.Odd.b == 1
-    assert cs.Odd.c == 2
-
-    assert cs.Odd.d == 5
-    assert cs.Odd.e == 6
-    assert cs.Odd.f == 7
-    assert cs.Odd.g == 8
+    assert cs.Odd.a == 2
+    assert cs.Odd.b == 4
+    assert cs.Odd.c == 8
+    assert cs.Odd.d == 32
+    assert cs.Odd.e == 64
+    assert cs.Odd.f == 128
+    assert cs.Odd.g == 256
 
     assert cs.Test.a == cs.Test.a
     assert cs.Test.a != cs.Test.b
+    assert cs.Test.b != cs.Odd.a
+    assert bool(cs.Test(0)) is False
+    assert bool(cs.Test(1)) is True
+
+    assert cs.Test.a | cs.Test.b == 3
+    if PY_311:
+        assert repr(cs.Test.c | cs.Test.d) == "<Test.c|d: 12>"
+        assert str(cs.Test.c | cs.Test.d) == "Test.c|d"
+        assert repr(cs.Test.a | cs.Test.b) == "<Test.a|b: 3>"
+        assert str(cs.Test.a | cs.Test.b) == "Test.a|b"
+        assert repr(cs.Test(69)) == "<Test.a|c|64: 69>"
+        assert str(cs.Test(69)) == "Test.a|c|64"
+    else:
+        assert repr(cs.Test.c | cs.Test.d) == "<Test.d|c: 12>"
+        assert str(cs.Test.c | cs.Test.d) == "Test.d|c"
+        assert repr(cs.Test.a | cs.Test.b) == "<Test.b|a: 3>"
+        assert str(cs.Test.a | cs.Test.b) == "Test.b|a"
+        assert repr(cs.Test(69)) == "<Test.64|c|a: 69>"
+        assert str(cs.Test(69)) == "Test.64|c|a"
+    assert cs.Test(2) == cs.Test.b
+    assert cs.Test(3) == cs.Test.a | cs.Test.b
+    assert cs.Test.c & 12 == cs.Test.c
+    assert cs.Test.b & 12 == 0
+    assert cs.Test.b ^ cs.Test.a == cs.Test.a | cs.Test.b
+
+    # TODO: determine if we want to stay true to Python stdlib or a consistent behaviour
+    if PY_311:
+        assert ~cs.Test.a == 14
+        assert repr(~cs.Test.a) == "<Test.b|c|d: 14>"
+    else:
+        assert ~cs.Test.a == -2
+        assert repr(~cs.Test.a) == "<Test.d|c|b: -2>"
 
 
-def test_enum_name(compiled):
-    cdef = """
-    enum Color: uint16 {
-          RED = 1,
-          GREEN = 2,
-          BLUE = 3,
-    };
-
-    struct Pixel {
-        uint8 x;
-        uint8 y;
-        Color color;
-        uint32 hue;
-    };
-    """
-    cs = cstruct.cstruct()
-    cs.load(cdef, compiled=compiled)
-
-    assert verify_compiled(cs.Pixel, compiled)
-
-    Color = cs.Color
-    Pixel = cs.Pixel
-
-    pixel = Pixel(b"\xFF\x0A\x01\x00\xAA\xBB\xCC\xDD")
-    assert pixel.x == 255
-    assert pixel.y == 10
-    assert pixel.color.name == "RED"
-    assert pixel.color.value == Color.RED
-    assert pixel.color.value == 1
-    assert pixel.hue == 0xDDCCBBAA
-
-    # unknown enum values default to <enum name>_<value>
-    pixel = Pixel(b"\x00\x00\xFF\x00\xAA\xBB\xCC\xDD")
-    assert pixel.color.name == "Color_255"
-    assert pixel.color.value == 0xFF
-
-
-def test_enum_write(compiled):
+def test_flag_struct_read(cs: cstruct, compiled: bool) -> None:
     cdef = """
-    enum Test16 : uint16 {
+    flag Test16 : uint16 {
         A = 0x1,
         B = 0x2
     };
 
-    enum Test24 : uint24 {
+    flag Test24 : uint24 {
         A = 0x1,
         B = 0x2
     };
 
-    enum Test32 : uint32 {
+    flag Test32 : uint32 {
         A = 0x1,
         B = 0x2
     };
 
     struct test {
         Test16  a16;
         Test16  b16;
         Test24  a24;
         Test24  b24;
         Test32  a32;
         Test32  b32;
-        Test16  list[2];
+        Test16  l[2];
+        Test16  c16;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
-    obj = cs.test()
-    obj.a16 = cs.Test16.A
-    obj.b16 = cs.Test16.B
-    obj.a24 = cs.Test24.A
-    obj.b24 = cs.Test24.B
-    obj.a32 = cs.Test32.A
-    obj.b32 = cs.Test32.B
-    obj.list = [cs.Test16.A, cs.Test16.B]
+    buf = b"\x01\x00\x02\x00\x01\x00\x00\x02\x00\x00\x01\x00\x00\x00\x02\x00\x00\x00\x01\x00\x02\x00\x03\x00"
+    obj = cs.test(buf)
 
-    assert obj.dumps() == b"\x01\x00\x02\x00\x01\x00\x00\x02\x00\x00\x01\x00\x00\x00\x02\x00\x00\x00\x01\x00\x02\x00"
+    assert isinstance(obj.a16, cs.Test16) and obj.a16.value == cs.Test16.A
+    assert isinstance(obj.b16, cs.Test16) and obj.b16.value == cs.Test16.B
+    assert isinstance(obj.a24, cs.Test24) and obj.a24.value == cs.Test24.A
+    assert isinstance(obj.b24, cs.Test24) and obj.b24.value == cs.Test24.B
+    assert isinstance(obj.a32, cs.Test32) and obj.a32.value == cs.Test32.A
+    assert isinstance(obj.b32, cs.Test32) and obj.b32.value == cs.Test32.B
 
+    assert len(obj.l) == 2
+    assert isinstance(obj.l[0], cs.Test16) and obj.l[0].value == cs.Test16.A
+    assert isinstance(obj.l[1], cs.Test16) and obj.l[1].value == cs.Test16.B
+
+    assert obj.c16 == cs.Test16.A | cs.Test16.B
+    assert obj.c16 & cs.Test16.A
+    if PY_311:
+        assert repr(obj.c16) == "<Test16.A|B: 3>"
+    else:
+        assert repr(obj.c16) == "<Test16.B|A: 3>"
+
+    assert obj.dumps() == buf
 
-def test_enum_anonymous(compiled):
+
+def test_flag_anonymous(cs: cstruct, compiled: bool) -> None:
     cdef = """
-    enum : uint16 {
-          RED = 1,
-          GREEN = 2,
-          BLUE = 3,
+    flag : uint16 {
+          A,
+          B,
+          C,
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
-    assert cs.RED == 1
-    assert cs.GREEN == 2
-    assert cs.BLUE == 3
+    assert cs.A == 1
+    assert cs.B == 2
+    assert cs.C == 4
+
+    assert cs.A.name == "A"
+    assert cs.A.value == 1
+    assert repr(cs.A) == "<A: 1>"
+    assert str(cs.A) == "A"
 
-    assert cs.RED.name == "RED"
-    assert cs.RED.value == 1
-    assert repr(cs.RED) == "<RED: 1>"
+    if PY_311:
+        assert repr(cs.A | cs.B) == "<A|B: 3>"
+        assert str(cs.A | cs.B) == "A|B"
+        assert repr(cs.A.__class__(69)) == "<A|C|64: 69>"
+        assert str(cs.A.__class__(69)) == "A|C|64"
+    else:
+        assert repr(cs.A | cs.B) == "<B|A: 3>"
+        assert str(cs.A | cs.B) == "B|A"
+        assert repr(cs.A.__class__(69)) == "<64|C|A: 69>"
+        assert str(cs.A.__class__(69)) == "64|C|A"
 
 
-def test_enum_anonymous_struct(compiled):
+def test_flag_anonymous_struct(cs: cstruct, compiled: bool) -> None:
     cdef = """
-    enum : uint32 {
+    flag : uint32 {
           nElements = 4
     };
 
     struct test {
         uint32  arr[nElements];
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     test = cs.test
 
     t = test(b"\xff\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x0A\x00\x00\x00")
     assert t.arr == [255, 0, 0, 10]
-
-
-def test_enum_reference_own_member(compiled):
-    cdef = """
-    enum test {
-        A,
-        B = A + 3,
-        C
-    };
-    """
-    cs = cstruct.cstruct()
-    cs.load(cdef, compiled=compiled)
-
-    assert cs.test.A == 0
-    assert cs.test.B == 3
-    assert cs.test.C == 4
```

### Comparing `dissect.cstruct-3.9.dev3/tests/test_struct.py` & `dissect_cstruct-4.0.dev0/tests/test_types_union.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,320 +1,338 @@
-from io import BytesIO
+import inspect
 
 import pytest
-from dissect import cstruct
+
+from dissect.cstruct.cstruct import cstruct
+from dissect.cstruct.types.base import Array
+from dissect.cstruct.types.structure import Field, Union
 
 from .utils import verify_compiled
 
 
-def test_struct_simple(compiled):
-    cdef = """
-    struct test {
-        char    magic[4];
-        wchar   wmagic[4];
-        uint8   a;
-        uint16  b;
-        uint32  c;
-        char    string[];
-        wchar   wstring[];
-    };
-    """
-    cs = cstruct.cstruct()
-    cs.load(cdef, compiled=compiled)
-
-    assert verify_compiled(cs.test, compiled)
+@pytest.fixture
+def TestUnion(cs: cstruct) -> type[Union]:
+    return cs._make_union(
+        "TestUnion",
+        [Field("a", cs.uint32), Field("b", cs.uint16)],
+    )
 
-    buf = b"testt\x00e\x00s\x00t\x00\x01\x02\x03\x04\x05\x06\x07lalala\x00t\x00e\x00s\x00t\x00\x00\x00"
-    obj = cs.test(buf)
 
-    assert "magic" in obj
-    assert obj.magic == b"test"
-    assert obj["magic"] == obj.magic
-    assert obj.wmagic == "test"
-    assert obj.a == 0x01
-    assert obj.b == 0x0302
-    assert obj.c == 0x07060504
-    assert obj.string == b"lalala"
-    assert obj.wstring == "test"
+def test_union(TestUnion: type[Union]) -> None:
+    assert issubclass(TestUnion, Union)
+    assert len(TestUnion.fields) == 2
+    assert TestUnion.fields["a"].name == "a"
+    assert TestUnion.fields["b"].name == "b"
+
+    assert TestUnion.size == 4
+    assert TestUnion.alignment == 4
+
+    spec = inspect.getfullargspec(TestUnion.__init__)
+    assert spec.args == ["self", "a", "b"]
+    assert spec.defaults == (None, None)
+
+    obj = TestUnion(1, 2)
+    assert isinstance(obj, TestUnion)
+    assert obj.a == 1
+    assert obj.b == 2
+    assert len(obj) == 4
+
+    obj = TestUnion(a=1)
+    assert obj.a == 1
+    assert obj.b is None
+    assert len(obj) == 4
+
+
+def test_union_read(TestUnion: type[Union]) -> None:
+    obj = TestUnion(b"\x01\x00\x00\x00")
+
+    assert isinstance(obj, TestUnion)
+    assert obj.a == 1
+    assert obj.b == 1
+
+
+def test_union_write(TestUnion: type[Union]) -> None:
+    buf = b"\x01\x00\x00\x00"
+    obj = TestUnion(buf)
 
-    with pytest.raises(AttributeError):
-        obj.nope
+    assert obj.dumps() == buf
 
-    assert obj._size("magic") == 4
-    assert len(obj) == len(buf)
+    obj = TestUnion(a=1, b=2)
     assert obj.dumps() == buf
+    assert bytes(obj) == buf
 
-    assert repr(obj)
+    obj = TestUnion(b=1)
+    assert obj.dumps() == b"\x01\x00\x00\x00"
 
-    fh = BytesIO()
-    obj.write(fh)
-    assert fh.getvalue() == buf
+    obj = TestUnion()
+    assert obj.dumps() == b"\x00\x00\x00\x00"
 
 
-def test_struct_simple_be(compiled):
-    cdef = """
-    struct test {
-        char    magic[4];
-        wchar   wmagic[4];
-        uint8   a;
-        uint16  b;
-        uint32  c;
-        char    string[];
-        wchar   wstring[];
-    };
-    """
-    cs = cstruct.cstruct(endian=">")
-    cs.load(cdef, compiled=compiled)
+def test_union_array_read(TestUnion: type[Union]) -> None:
+    TestUnionArray = TestUnion[2]
 
-    assert verify_compiled(cs.test, compiled)
+    assert issubclass(TestUnionArray, Array)
+    assert TestUnionArray.num_entries == 2
+    assert TestUnionArray.type == TestUnion
 
-    buf = b"test\x00t\x00e\x00s\x00t\x01\x02\x03\x04\x05\x06\x07lalala\x00\x00t\x00e\x00s\x00t\x00\x00"
-    obj = cs.test(buf)
+    buf = b"\x01\x00\x00\x00\x02\x00\x00\x00"
+    obj = TestUnionArray(buf)
+
+    assert isinstance(obj, TestUnionArray)
+    assert len(obj) == 2
+    assert obj[0].a == 1
+    assert obj[0].b == 1
+    assert obj[1].a == 2
+    assert obj[1].b == 2
 
-    assert obj.magic == b"test"
-    assert obj.wmagic == "test"
-    assert obj.a == 0x01
-    assert obj.b == 0x0203
-    assert obj.c == 0x04050607
-    assert obj.string == b"lalala"
-    assert obj.wstring == "test"
     assert obj.dumps() == buf
+    assert obj == [TestUnion(1), TestUnion(2)]
 
+    obj = TestUnion[None](b"\x01\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00")
+    assert obj == [TestUnion(1), TestUnion(2)]
 
-def test_struct_definitions(compiled):
-    cdef = """
-    struct _test {
-        uint32  a;
-        // uint32 comment
-        uint32  b;
-    } test, test1;
-    """
-    cs = cstruct.cstruct()
-    cs.load(cdef, compiled=compiled)
 
-    assert verify_compiled(cs.test, compiled)
+def test_union_array_write(TestUnion: type[Union]) -> None:
+    TestUnionArray = TestUnion[2]
 
-    assert cs._test == cs.test == cs.test1
-    assert cs.test.name == "_test"
-    assert cs._test.name == "_test"
-
-    assert "a" in cs.test.lookup
-    assert "b" in cs.test.lookup
-
-    with pytest.raises(cstruct.ParserError):
-        cdef = """
-        struct {
-            uint32  a;
-        };
-        """
-        cs.load(cdef)
+    obj = TestUnionArray([TestUnion(1), TestUnion(2)])
 
+    assert len(obj) == 2
+    assert obj.dumps() == b"\x01\x00\x00\x00\x02\x00\x00\x00"
 
-def test_struct_expressions(compiled):
-    cdef = """
-    #define const 1
-    struct test {
-        uint8   flag;
-        uint8   data_1[flag & 1 * 4];
-        uint8   data_2[flag & (1 << 2)];
-        uint8   data_3[const];
-    };
-    """
-    cs = cstruct.cstruct()
-    cs.load(cdef, compiled=compiled)
+    obj = TestUnion[None]([TestUnion(1)])
+    assert obj.dumps() == b"\x01\x00\x00\x00\x00\x00\x00\x00"
 
-    assert verify_compiled(cs.test, compiled)
 
-    obj = cs.test(b"\x01\x00\x01\x02\x03\xff")
-    assert obj.flag == 1
-    assert obj.data_1 == [0, 1, 2, 3]
-    assert obj.data_2 == []
-    assert obj.data_3 == [255]
-
-    obj = cs.test(b"\x04\x04\x05\x06\x07\xff")
-    assert obj.flag == 4
-    assert obj.data_1 == []
-    assert obj.data_2 == [4, 5, 6, 7]
-    assert obj.data_3 == [255]
+def test_union_modify(cs: cstruct) -> None:
+    TestUnion = cs._make_union("Test", [Field("a", cs.char)])
 
+    assert len(TestUnion.fields) == len(TestUnion.lookup) == 1
+    assert len(TestUnion) == 1
+    spec = inspect.getfullargspec(TestUnion.__init__)
+    assert spec.args == ["self", "a"]
+    assert spec.defaults == (None,)
 
-def test_struct_sizes(compiled):
-    cdef = """
-    struct static {
-        uint32  test;
-    };
+    TestUnion.add_field("b", cs.uint32)
 
-    struct dynamic {
-        uint32  test[];
-    };
-    """
-    cs = cstruct.cstruct()
-    cs.load(cdef, compiled=compiled)
+    assert len(TestUnion.fields) == len(TestUnion.lookup) == 2
+    assert len(TestUnion) == 4
+    spec = inspect.getfullargspec(TestUnion.__init__)
+    assert spec.args == ["self", "a", "b"]
+    assert spec.defaults == (None, None)
+
+    with TestUnion.start_update():
+        TestUnion.add_field("c", cs.uint16)
+        TestUnion.add_field("d", cs.uint8)
+
+    assert len(TestUnion.fields) == len(TestUnion.lookup) == 4
+    assert len(TestUnion) == 4
+    spec = inspect.getfullargspec(TestUnion.__init__)
+    assert spec.args == ["self", "a", "b", "c", "d"]
+    assert spec.defaults == (None, None, None, None)
+
+    obj = TestUnion(b"\x01\x02\x03\x04")
+    assert obj.a == b"\x01"
+    assert obj.b == 0x04030201
+    assert obj.c == 0x0201
+    assert obj.d == 0x01
+
+
+def test_union_bool(TestUnion: type[Union]) -> None:
+    assert bool(TestUnion(1, 2)) is True
+    assert bool(TestUnion(1, 1)) is True
+    assert bool(TestUnion()) is False
+    assert bool(TestUnion(0, 0)) is False
 
-    assert verify_compiled(cs.static, compiled)
-    assert verify_compiled(cs.dynamic, compiled)
 
-    assert len(cs.static) == 4
+def test_union_cmp(TestUnion: type[Union]) -> None:
+    assert TestUnion(1) == TestUnion(1)
+    assert TestUnion(1, 2) == TestUnion(1, 2)
+    assert TestUnion(1, 2) != TestUnion(2, 3)
+    assert TestUnion(b=2) == TestUnion(a=2)
 
-    if not compiled:
-        cs.static.add_field("another", cs.uint32)
-        assert len(cs.static) == 8
-        cs.static.add_field("atoffset", cs.uint32, offset=12)
-        assert len(cs.static) == 16
-
-        obj = cs.static(b"\x01\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x03\x00\x00\x00")
-        assert obj.test == 1
-        assert obj.another == 2
-        assert obj.atoffset == 3
-
-        with pytest.raises(TypeError) as excinfo:
-            len(cs.dynamic)
-        assert str(excinfo.value) == "Dynamic size"
-    else:
-        with pytest.raises(NotImplementedError) as excinfo:
-            cs.static.add_field("another", cs.uint32)
-        assert str(excinfo.value) == "Can't add fields to a compiled structure"
 
+def test_union_repr(TestUnion: type[Union]) -> None:
+    obj = TestUnion(1, 2)
+    assert repr(obj) == f"<{TestUnion.__name__} a=0x1 b=0x2>"
 
-def test_struct_nested(compiled):
+
+def test_union_eof(TestUnion: type[Union]) -> None:
+    with pytest.raises(EOFError):
+        TestUnion(b"")
+
+    with pytest.raises(EOFError):
+        TestUnion[2](b"\x01\x00\x00\x00")
+
+    with pytest.raises(EOFError):
+        TestUnion[None](b"\x01\x00\x00\x00\x02\x00\x00\x00")
+
+
+def test_union_definition(cs: cstruct) -> None:
     cdef = """
-    struct test_named {
-        char magic[4];
-        struct {
-            uint32 a;
-            uint32 b;
-        } a;
-        struct {
-            char   c[8];
-        } b;
+    union test {
+        uint32 a;
+        char   b[8];
     };
+    """
+    cs.load(cdef, compiled=False)
 
-    struct test_anonymous {
+    assert len(cs.test) == 8
+
+    buf = b"zomgbeef"
+    obj = cs.test(buf)
+
+    assert obj.a == 0x676D6F7A
+    assert obj.b == b"zomgbeef"
+
+    assert obj.dumps() == buf
+    assert cs.test().dumps() == b"\x00\x00\x00\x00\x00\x00\x00\x00"
+
+
+def test_union_definition_nested(cs: cstruct, compiled: bool) -> None:
+    cdef = """
+    struct test {
         char magic[4];
-        struct {
-            uint32 a;
-            uint32 b;
-        };
-        struct {
-            char   c[8];
-        };
+        union {
+            struct {
+                uint32 a;
+                uint32 b;
+            } a;
+            struct {
+                char   b[8];
+            } b;
+        } c;
     };
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
-    assert verify_compiled(cs.test_named, compiled)
-    assert verify_compiled(cs.test_anonymous, compiled)
+    assert verify_compiled(cs.test, compiled)
 
-    assert len(cs.test_named) == len(cs.test_anonymous) == 20
+    assert len(cs.test) == 12
 
-    data = b"zomg\x39\x05\x00\x00\x28\x23\x00\x00deadbeef"
-    obj = cs.test_named(data)
-    assert obj.magic == b"zomg"
-    assert obj.a.a == 1337
-    assert obj.a.b == 9000
-    assert obj.b.c == b"deadbeef"
-    assert obj.dumps() == data
+    buf = b"zomgholybeef"
+    obj = cs.test(buf)
 
-    obj = cs.test_anonymous(data)
     assert obj.magic == b"zomg"
-    assert obj.a == 1337
-    assert obj.b == 9000
-    assert obj.c == b"deadbeef"
-    assert obj.dumps() == data
+    assert obj.c.a.a == 0x796C6F68
+    assert obj.c.a.b == 0x66656562
+    assert obj.c.b.b == b"holybeef"
+
+    assert obj.dumps() == buf
 
 
-def test_struct_write(compiled):
+def test_union_definition_anonymous(cs: cstruct, compiled: bool) -> None:
     cdef = """
-    struct test {
-        char    magic[4];
-        wchar   wmagic[4];
-        uint8   a;
-        uint16  b;
-        uint32  c;
-        char    string[];
-        wchar   wstring[];
-    };
+    typedef struct test
+    {
+        union
+        {
+            uint32 a;
+            struct
+            {
+                char b[3];
+                char c;
+            };
+        };
+        uint32 d;
+    }
     """
-    cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     assert verify_compiled(cs.test, compiled)
 
-    buf = b"testt\x00e\x00s\x00t\x00\x01\x02\x03\x04\x05\x06\x07lalala\x00t\x00e\x00s\x00t\x00\x00\x00"
+    buf = b"\x01\x01\x02\x02\x03\x03\x04\x04"
+    obj = cs.test(buf)
 
-    obj = cs.test()
-    obj.magic = "test"
-    obj.wmagic = "test"
-    obj.a = 0x01
-    obj.b = 0x0302
-    obj.c = 0x07060504
-    obj.string = b"lalala"
-    obj.wstring = "test"
+    assert obj.a == 0x02020101
+    assert obj.b == b"\x01\x01\x02"
+    assert obj.c == b"\x02"
+    assert obj.d == 0x04040303
+    assert obj.dumps() == buf
 
-    with pytest.raises(AttributeError):
-        obj.nope = 1
 
-    assert obj.dumps() == buf
+def test_union_definition_dynamic(cs: cstruct) -> None:
+    cdef = """
+    struct dynamic {
+        uint8   size;
+        char    data[size];
+    };
 
-    inst = cs.test(
-        magic=b"test",
-        wmagic="test",
-        a=0x01,
-        b=0x0302,
-        c=0x07060504,
-        string=b"lalala",
-        wstring="test",
-    )
-    assert inst.dumps() == buf
+    union test {
+        dynamic a;
+        uint64  b;
+    };
+    """
+    cs.load(cdef, compiled=False)
+
+    buf = b"\x09aaaaaaaaa"
+    obj = cs.test(buf)
+
+    assert obj.a.size == 9
+    assert obj.a.data == b"aaaaaaaaa"
+    assert obj.b == 0x6161616161616109
 
 
-def test_struct_write_be(compiled):
+def test_union_update(cs: cstruct) -> None:
     cdef = """
-    struct test {
-        char    magic[4];
-        wchar   wmagic[4];
+    union test {
         uint8   a;
         uint16  b;
-        uint32  c;
-        char    string[];
-        wchar   wstring[];
     };
     """
-    cs = cstruct.cstruct(endian=">")
-    cs.load(cdef, compiled=compiled)
-
-    assert verify_compiled(cs.test, compiled)
-
-    buf = b"test\x00t\x00e\x00s\x00t\x01\x02\x03\x04\x05\x06\x07lalala\x00\x00t\x00e\x00s\x00t\x00\x00"
+    cs.load(cdef)
 
     obj = cs.test()
-    obj.magic = "test"
-    obj.wmagic = "test"
-    obj.a = 0x01
-    obj.b = 0x0203
-    obj.c = 0x04050607
-    obj.string = b"lalala"
-    obj.wstring = "test"
-
-    assert obj.dumps() == buf
+    obj.a = 1
+    assert obj.b == 1
+    obj.b = 2
+    assert obj.a == 2
+    obj.b = 0xFFFF
+    assert obj.a == 0xFF
+    assert obj.dumps() == b"\xFF\xFF"
 
 
-def test_struct_write_anonymous():
+def test_union_nested_update(cs: cstruct) -> None:
     cdef = """
     struct test {
-        uint32 a;
+        char magic[4];
         union {
             struct {
-                uint16 b1;
-                uint16 b2;
+                uint32 a;
+                uint32 b;
+            } a;
+            struct {
+                char   b[8];
+            } b;
+        } c;
+    };
+    """
+    cs.load(cdef)
+
+    obj = cs.test()
+    obj.magic = b"1337"
+    obj.c.b.b = b"ABCDEFGH"
+    assert obj.c.a.a == 0x44434241
+    assert obj.c.a.b == 0x48474645
+    assert obj.dumps() == b"1337ABCDEFGH"
+
+
+def test_union_anonymous_update(cs: cstruct) -> None:
+    cdef = """
+    typedef struct test
+    {
+        union {
+            uint32 a;
+            struct
+            {
+                char b[3];
+                char c;
             };
-            uint32 b;
         };
-        uint32 c;
-    };
+        uint32 d;
+    }
     """
-    cs = cstruct.cstruct()
     cs.load(cdef)
 
-    obj = cs.test(a=1, c=3)
-    assert obj.dumps() == b"\x01\x00\x00\x00\x00\x00\x00\x00\x03\x00\x00\x00"
+    obj = cs.test()
+    obj.a = 0x41414141
+    assert obj.b == b"AAA"
```

### Comparing `dissect.cstruct-3.9.dev3/tox.ini` & `dissect_cstruct-4.0.dev0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tox]
 envlist = lint, py3, pypy3
 # This version of tox will autoprovision itself and the requirements defined in
 # requires if they are not available on the host system. This requires the
 # locally installed tox to have a minimum version 3.3.0. This means the names
 # of the configuration options are still according to the tox 3.x syntax.
-minversion = 4.2.4
+minversion = 4.4.3
 # This version of virtualenv will install setuptools version 65.5.0 and pip
 # 22.3. These versions fully support python projects defined only through a
 # pyproject.toml file (PEP-517/PEP-518/PEP-621)
 requires = virtualenv>=20.16.6
 
 [testenv]
 deps =
```

