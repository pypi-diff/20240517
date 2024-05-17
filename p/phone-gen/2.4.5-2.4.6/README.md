# Comparing `tmp/phone_gen-2.4.5.tar.gz` & `tmp/phone_gen-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phone_gen-2.4.5.tar", last modified: Thu May  9 14:12:13 2024, max compression
+gzip compressed data, was "phone_gen-2.4.6.tar", last modified: Fri May 17 14:46:36 2024, max compression
```

## Comparing `phone_gen-2.4.5.tar` & `phone_gen-2.4.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:13.778395 phone_gen-2.4.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:13.774395 phone_gen-2.4.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:13.774395 phone_gen-2.4.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-09 14:12:08.000000 phone_gen-2.4.5/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-09 14:12:08.000000 phone_gen-2.4.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-09 14:12:08.000000 phone_gen-2.4.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-09 14:12:08.000000 phone_gen-2.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-09 14:12:13.778395 phone_gen-2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-09 14:12:08.000000 phone_gen-2.4.5/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-09 14:12:08.000000 phone_gen-2.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:13.774395 phone_gen-2.4.5/dev_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-09 14:12:08.000000 phone_gen-2.4.5/dev_tools/patterns_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-09 14:12:08.000000 phone_gen-2.4.5/dev_tools/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:13.778395 phone_gen-2.4.5/phone_gen/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-09 14:12:08.000000 phone_gen-2.4.5/phone_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 14:12:13.000000 phone_gen-2.4.5/phone_gen/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-09 14:12:08.000000 phone_gen-2.4.5/phone_gen/_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-09 14:12:08.000000 phone_gen-2.4.5/phone_gen/alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-09 14:12:08.000000 phone_gen-2.4.5/phone_gen/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-05-09 14:12:08.000000 phone_gen-2.4.5/phone_gen/country_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-09 14:12:08.000000 phone_gen-2.4.5/phone_gen/iso3.py
--rw-r--r--   0 runner    (1001) docker     (127)    89041 2024-05-09 14:12:08.000000 phone_gen-2.4.5/phone_gen/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:13.778395 phone_gen-2.4.5/phone_gen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-09 14:12:13.000000 phone_gen-2.4.5/phone_gen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-09 14:12:13.000000 phone_gen-2.4.5/phone_gen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:12:13.000000 phone_gen-2.4.5/phone_gen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-09 14:12:13.000000 phone_gen-2.4.5/phone_gen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 14:12:13.000000 phone_gen-2.4.5/phone_gen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-09 14:12:13.778395 phone_gen-2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-09 14:12:08.000000 phone_gen-2.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:12:13.778395 phone_gen-2.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 14:12:08.000000 phone_gen-2.4.5/tests/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-09 14:12:08.000000 phone_gen-2.4.5/tests/test_alt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-09 14:12:08.000000 phone_gen-2.4.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-09 14:12:08.000000 phone_gen-2.4.5/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-09 14:12:08.000000 phone_gen-2.4.5/tests/test_load_alt_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-09 14:12:08.000000 phone_gen-2.4.5/tests/test_phone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:36.144308 phone_gen-2.4.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:36.140308 phone_gen-2.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:36.140308 phone_gen-2.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 14:46:31.000000 phone_gen-2.4.6/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-17 14:46:31.000000 phone_gen-2.4.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-17 14:46:31.000000 phone_gen-2.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 14:46:31.000000 phone_gen-2.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-17 14:46:36.144308 phone_gen-2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-17 14:46:31.000000 phone_gen-2.4.6/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-17 14:46:31.000000 phone_gen-2.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:36.140308 phone_gen-2.4.6/dev_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-17 14:46:31.000000 phone_gen-2.4.6/dev_tools/patterns_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-05-17 14:46:31.000000 phone_gen-2.4.6/dev_tools/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:36.144308 phone_gen-2.4.6/phone_gen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-17 14:46:31.000000 phone_gen-2.4.6/phone_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-17 14:46:36.000000 phone_gen-2.4.6/phone_gen/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-17 14:46:31.000000 phone_gen-2.4.6/phone_gen/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-17 14:46:31.000000 phone_gen-2.4.6/phone_gen/alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-17 14:46:31.000000 phone_gen-2.4.6/phone_gen/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-05-17 14:46:31.000000 phone_gen-2.4.6/phone_gen/country_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-17 14:46:31.000000 phone_gen-2.4.6/phone_gen/iso3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89027 2024-05-17 14:46:31.000000 phone_gen-2.4.6/phone_gen/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:36.144308 phone_gen-2.4.6/phone_gen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-17 14:46:36.000000 phone_gen-2.4.6/phone_gen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-17 14:46:36.000000 phone_gen-2.4.6/phone_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:46:36.000000 phone_gen-2.4.6/phone_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 14:46:36.000000 phone_gen-2.4.6/phone_gen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-17 14:46:36.000000 phone_gen-2.4.6/phone_gen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-17 14:46:36.144308 phone_gen-2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-17 14:46:31.000000 phone_gen-2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:46:36.144308 phone_gen-2.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-17 14:46:31.000000 phone_gen-2.4.6/tests/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-17 14:46:31.000000 phone_gen-2.4.6/tests/test_alt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-17 14:46:31.000000 phone_gen-2.4.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-17 14:46:31.000000 phone_gen-2.4.6/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-17 14:46:31.000000 phone_gen-2.4.6/tests/test_load_alt_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-17 14:46:31.000000 phone_gen-2.4.6/tests/test_phone.py
```

### Comparing `phone_gen-2.4.5/.github/workflows/python-package.yml` & `phone_gen-2.4.6/.github/workflows/python-package.yml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.36
+          python -m pip install flake8 pep8-naming pytest black pytest-cov phonenumbers==8.13.37
           python -m pip install -e .
       - name: Flake8
         run: |
           flake8 phone_gen
       - name: Black
         run: |
           black --check phone_gen
```

### Comparing `phone_gen-2.4.5/.github/workflows/python-publish.yml` & `phone_gen-2.4.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/.gitignore` & `phone_gen-2.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/LICENSE` & `phone_gen-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/PKG-INFO` & `phone_gen-2.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_gen
-Version: 2.4.5
+Version: 2.4.6
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.4.5/README.md` & `phone_gen-2.4.6/README.md`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/dev_tools/patterns_generator.py` & `phone_gen-2.4.6/dev_tools/patterns_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/dev_tools/update.py` & `phone_gen-2.4.6/dev_tools/update.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/phone_gen/__init__.py` & `phone_gen-2.4.6/phone_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/phone_gen/_generator.py` & `phone_gen-2.4.6/phone_gen/_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/phone_gen/alt_patterns.py` & `phone_gen-2.4.6/phone_gen/alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/phone_gen/cli.py` & `phone_gen-2.4.6/phone_gen/cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/phone_gen/country_name.py` & `phone_gen-2.4.6/phone_gen/country_name.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/phone_gen/iso3.py` & `phone_gen-2.4.6/phone_gen/iso3.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/phone_gen/patterns.py` & `phone_gen-2.4.6/phone_gen/patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 """
-Auto-generated file 2024-05-09 14:06:39 UTC
-Resource: https://github.com/google/libphonenumber v8.13.36
+Auto-generated file 2024-05-17 14:37:40 UTC
+Resource: https://github.com/google/libphonenumber v8.13.37
 """
 
 
 PATTERNS = {
-    "info": "libphonenumber v8.13.36",
+    "info": "libphonenumber v8.13.37",
     "data": {
         "AC": {
             "code": "247",
             "pattern": "((6[2-467][\\d]{3}))",
             "mobile": "((4[\\d]{4}))",
         },
         "AD": {
@@ -67,15 +67,15 @@
             "code": "43",
             "pattern": "((1(11[\\d])|([2-9][\\d]{3:11}))|((316)|(463)|((51)|(66)|(73)2)[\\d]{3:10})|((2(1[467])|(2[13-8])|(5[2357])|(6[1-46-8])|(7[1-8])|(8[124-7])|(9[1458]))|(3(1[1-578])|(3[23568])|(4[5-7])|(5[1378])|(6[1-38])|(8[3-68]))|(4(2[1-8])|(35)|(7[1368])|(8[2457]))|(5(2[1-8])|(3[357])|(4[147])|(5[12578])|(6[37]))|(6(13)|(2[1-47])|(4[135-8])|(5[468]))|(7(2[1-8])|(35)|(4[13478])|(5[68])|(6[16-8])|(7[1-6])|(9[45]))[\\d]{4:10}))",
             "mobile": "((6(5[0-3579])|(6[013-9])|([7-9][\\d])[\\d]{4:10}))",
         },
         "AU": {
             "code": "61",
             "pattern": "(((((2([0-26-9][\\d])|(3[0-8])|(4[02-9])|(5[0135-9]))|(7([013-57-9][\\d])|(2[0-8]))[\\d])|(3(([0-3589][\\d])|(6[1-9])|(7[0-35-9])[\\d])|(4([0-578][\\d])|(90)))[\\d][\\d])|(8(51(0(0[03-9])|([12479][\\d])|(3[2-9])|(5[0-8])|(6[1-9])|(8[0-7]))|(1([0235689][\\d])|(1[0-69])|(4[0-589])|(7[0-47-9]))|(2(0[0-79])|([18][13579])|(2[14-9])|(3[0-46-9])|([4-6][\\d])|(7[89])|(9[0-4]))|(3[\\d][\\d]))|((6[0-8])|([78][\\d])[\\d]{3})|(9([02-9][\\d]{3})|(1(([0-58][\\d])|(6[0135-9])[\\d])|(7(0[0-24-9])|([1-9][\\d]))|(9([0-46-9][\\d])|(5[0-79])))))[\\d]{3}))",
-            "mobile": "((4((79)|(94)[01])|(83[0-389])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[0-36-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
+            "mobile": "((4(79[01])|(83[0-389])|(94[0-4])[\\d]{5})|(4([0-36][\\d])|(4[047-9])|(5[0-25-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
         },
         "AW": {
             "code": "297",
             "pattern": "((5(2[\\d])|(8[1-9])[\\d]{4}))",
             "mobile": "(((290)|(5[69][\\d])|(6([03]0)|(22)|(4[0-2])|([69][\\d]))|(7([34][\\d])|(7[07]))|(9(6[45])|(9[4-8]))[\\d]{4}))",
         },
         "AX": {
@@ -96,15 +96,15 @@
         "BB": {
             "code": "1",
             "pattern": "((246521[0369][\\d]{3})|(246(2(2[78])|(7[0-4]))|(4(1[024-6])|(2[\\d])|(3[2-9]))|(5(20)|([34][\\d])|(54)|(7[1-3]))|(6(2[\\d])|(38))|(7[35]7)|(9(1[89])|(63))[\\d]{4}))",
             "mobile": "((246((2([3568][\\d])|(4[0-57-9]))|(3(5[2-9])|(6[0-6]))|(4(46)|(5[\\d]))|(69[5-7])|(8([2-5][\\d])|(83))[\\d])|(52(1[147])|(20))[\\d]{3}))",
         },
         "BD": {
             "code": "880",
-            "pattern": "(((4(31[\\d][\\d])|(423))|(5222)[\\d]{3}([\\d]{2})?)|(8332[6-9][\\d][\\d])|((3(03[56])|(224))|(4(22[25])|(653))[\\d]{3:4})|((3(42[47])|(529)|(823))|(4(027)|(525)|(65(28)|(8)))|(562)|(6257)|(7(1(5[3-5])|(6[12])|(7[156])|(89))|(22[589]56)|(32)|(42675)|(52([25689](56)|(8))|([347]8))|(71(6[1267])|(75)|(89))|(92374))|(82(2[59])|(32)56)|(9(03[23]56)|(23(256)|(373))|(31)|(5(1)|(2[4589]56)))[\\d]{3})|((3(02[348])|(22[35])|(324)|(422))|(4(22[67])|(32[236-9])|(6(2[46])|(5[57]))|(953))|(5526)|(6(024)|(6655))|(81)[\\d]{4:5})|((2(7(1[0-267])|(2[0-289])|(3[0-29])|(4[01])|(5[1-3])|(6[013])|(7[0178])|(91))|(8(0[125])|(1[1-6])|(2[0157-9])|(3[1-69])|(41)|(6[1-35])|(7[1-5])|(8[1-8])|(9[0-6]))|(9(0[0-2])|(1[0-4])|(2[568])|(3[3-6])|(5[5-7])|(6[0136-9])|(7[0-7])|(8[014-9])))|(3(0(2[025-79])|(3[2-4]))|(181)|(22[12])|(32[2356])|(824))|(4(02[09])|(22[348])|(32[045])|(523)|(6(27)|(54)))|(666(22)|(53))|(7(22[57-9])|(42[56])|(82[35])8)|(8(0[124-9])|(2(181)|(2[02-4679]8))|(4[12])|([5-7]2))|(9([04]2)|(2(2)|(328))|(81))[\\d]{4})|((2(222)|([45][\\d])[\\d])|(3(1(2[5-7])|([5-7]))|(425)|(822))|(4(033)|(1[\\d])|([257]1)|(332)|(4(2[246])|(5[25]))|(6(2[35])|(56)|(62))|(8(23)|(54))|(92[2-5]))|(5(02[03489])|(22[457])|(32[35-79])|(42[46])|(6([18])|(53))|(724)|(826))|(6(023)|(2(2[2-5])|(5[3-5])|(8))|(32[3478])|(42[34])|(52[47])|(6([18])|(6(2[34])|(5[24])))|([78]2[2-5])|(92[2-6]))|(7(02)|(21[\\d])|([3-589]1)|(6[12])|(72[24]))|(8(217)|(3[12])|([5-7]1))|(9[24]1)[\\d]{5})|(((3[2-8])|(5[2-57-9])|(6[03-589])1)|(4[4689][18])[\\d]{5})|([59]1[\\d]{5}))",
+            "pattern": "(((4(31[\\d][\\d])|(423))|(5222)[\\d]{3}([\\d]{2})?)|(8332[6-9][\\d][\\d])|((3(03[56])|(224))|(4(22[25])|(653))[\\d]{3:4})|((3(42[47])|(529)|(823))|(4(027)|(525)|(65(28)|(8)))|(562)|(6257)|(7(1(5[3-5])|(6[12])|(7[156])|(89))|(22[589]56)|(32)|(42675)|(52([25689](56)|(8))|([347]8))|(71(6[1267])|(75)|(89))|(92374))|(82(2[59])|(32)56)|(9(03[23]56)|(23(256)|(373))|(31)|(5(1)|(2[4589]56)))[\\d]{3})|((3(02[348])|(22[35])|(324)|(422))|(4(22[67])|(32[236-9])|(6(2[46])|(5[57]))|(953))|(5526)|(6(024)|(6655))|(81)[\\d]{4:5})|((2(7(1[0-267])|(2[0-289])|(3[0-29])|(4[01])|(5[1-3])|(6[013])|(7[0178])|(91))|(8(0[125])|(1[1-6])|(2[0157-9])|(3[1-69])|(41)|(6[1-35])|(7[1-5])|(8[1-8])|(9[0-6]))|(9(0[0-2])|(1[0-4])|(2[568])|(3[3-6])|(5[5-7])|(6[0136-9])|(7[0-7])|(8[014-9])))|(3(0(2[025-79])|(3[2-4]))|(181)|(22[12])|(32[2356])|(824))|(4(02[09])|(22[348])|(32[045])|(523)|(6(27)|(54)))|(666(22)|(53))|(7(22[57-9])|(42[56])|(82[35])8)|(8(0[124-9])|(2(181)|(2[02-4679]8))|(4[12])|([5-7]2))|(9([04]2)|(2(2)|(328))|(81))[\\d]{4})|((2(2[\\d])|([45])[\\d][\\d])|(3(1(2[5-7])|([5-7]))|(425)|(822))|(4(033)|(1[\\d])|([257]1)|(332)|(4(2[246])|(5[25]))|(6(2[35])|(56)|(62))|(8(23)|(54))|(92[2-5]))|(5(02[03489])|(22[457])|(32[35-79])|(42[46])|(6([18])|(53))|(724)|(826))|(6(023)|(2(2[2-5])|(5[3-5])|(8))|(32[3478])|(42[34])|(52[47])|(6([18])|(6(2[34])|(5[24])))|([78]2[2-5])|(92[2-6]))|(7(02)|(21[\\d])|([3-589]1)|(6[12])|(72[24]))|(8(217)|(3[12])|([5-7]1))|(9[24]1)[\\d]{5})|(((3[2-8])|(5[2-57-9])|(6[03-589])1)|(4[4689][18])[\\d]{5})|([59]1[\\d]{5}))",
             "mobile": "(((1[13-9][\\d])|(644)[\\d]{7})|((3[78])|(44)|(66)[02-9][\\d]{7}))",
         },
         "BE": {
             "code": "32",
             "pattern": "((80[2-8][\\d]{5})|((1[0-69])|([23][2-8])|(4[23])|(5[\\d])|(6[013-57-9])|(71)|(8[1-79])|(9[2-4])[\\d]{6}))",
             "mobile": "((4[5-9][\\d]{7}))",
         },
@@ -192,15 +192,15 @@
             "code": "1",
             "pattern": "(((2(04)|([23]6)|([48]9)|(50)|(63))|(3(06)|(43)|(54)|(6[578])|(82))|(4(03)|(1[68])|([26]8)|(3[178])|(50)|(74))|(5(06)|(1[49])|(48)|(79)|(8[147]))|(6(04)|([18]3)|(39)|(47)|(72))|(7(0[59])|(42)|(53)|(78)|(8[02]))|(8([06]7)|(19)|(25)|(7[39]))|(90[25])[2-9][\\d]{6}))",
             "mobile": "(((2(04)|([23]6)|([48]9)|(50)|(63))|(3(06)|(43)|(54)|(6[578])|(82))|(4(03)|(1[68])|([26]8)|(3[178])|(50)|(74))|(5(06)|(1[49])|(48)|(79)|(8[147]))|(6(04)|([18]3)|(39)|(47)|(72))|(7(0[59])|(42)|(53)|(78)|(8[02]))|(8([06]7)|(19)|(25)|(7[39]))|(90[25])[2-9][\\d]{6}))",
         },
         "CC": {
             "code": "61",
             "pattern": "((8(51(0(02)|(31)|(60)|(89))|(1(18)|(76))|(223))|(91(0(1[0-2])|(29))|(1([28]2)|(50)|(79))|(2(10)|(64))|(3([06]8)|(22))|(4[29]8)|(62[\\d])|(70[23])|(959))[\\d]{3}))",
-            "mobile": "((4((79)|(94)[01])|(83[0-389])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[0-36-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
+            "mobile": "((4(79[01])|(83[0-389])|(94[0-4])[\\d]{5})|(4([0-36][\\d])|(4[047-9])|(5[0-25-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
         },
         "CD": {
             "code": "243",
             "pattern": "((12[\\d]{7})|([1-6][\\d]{6}))",
             "mobile": "((88[\\d]{5})|((8[0-69])|(9[017-9])[\\d]{7}))",
         },
         "CF": {
@@ -267,15 +267,15 @@
             "code": "599",
             "pattern": "((9(4(3[0-5])|(4[14])|(6[\\d]))|(50[\\d])|(7(2[014])|(3[02-9])|(4[4-9])|(6[357])|(77)|(8[7-9]))|(8(3[39])|([46][\\d])|(7[01])|(8[57-9]))[\\d]{4}))",
             "mobile": "((953[01][\\d]{4})|(9(5[12467])|(6[5-9])[\\d]{5}))",
         },
         "CX": {
             "code": "61",
             "pattern": "((8(51(0(01)|(30)|(59)|(88))|(1(17)|(46)|(75))|(2(22)|(35)))|(91(00[6-9])|(1([28]1)|(49)|(78))|(2(09)|(63))|(3(12)|(26)|(75))|(4(56)|(97))|(64[\\d])|(7(0[01])|(1[0-2]))|(958))[\\d]{3}))",
-            "mobile": "((4((79)|(94)[01])|(83[0-389])[\\d]{5})|(4([0-3][\\d])|(4[047-9])|(5[0-25-9])|(6[0-36-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
+            "mobile": "((4(79[01])|(83[0-389])|(94[0-4])[\\d]{5})|(4([0-36][\\d])|(4[047-9])|(5[0-25-9])|(7[02-8])|(8[0-24-9])|(9[0-37-9])[\\d]{6}))",
         },
         "CY": {
             "code": "357",
             "pattern": "((2[2-6][\\d]{6}))",
             "mobile": "((9(10)|([4-79][\\d])[\\d]{5}))",
         },
         "CZ": {
@@ -462,15 +462,15 @@
             "code": "245",
             "pattern": "((443[\\d]{6}))",
             "mobile": "((9(5[\\d])|(6[569])|(77)[\\d]{6}))",
         },
         "GY": {
             "code": "592",
             "pattern": "(((2(1[6-9])|(2[0-35-9])|(3[1-4])|(5[3-9])|(6[\\d])|(7[0-79]))|(3(2[25-9])|(3[\\d]))|(4(4[0-24])|(5[56]))|(50[0-6])|(77[1-57])[\\d]{4}))",
-            "mobile": "(((510)|(6[\\d][\\d])|(7([01][\\d])|(2[0-256])|(3[0-2])|(49))[\\d]{4}))",
+            "mobile": "(((510)|(6[\\d][\\d])|(7([013][\\d])|(2[0-25-8])|(4[0-29]))[\\d]{4}))",
         },
         "HK": {
             "code": "852",
             "pattern": "(((2([13-9][\\d])|(2[013-9])[\\d])|(3(([1569][0-24-9])|(4[0-246-9])|(7[0-24-69])[\\d])|(8(4[0-8])|([59][\\d])|(6[01])))|(58(0[1-9])|(1[2-9]))[\\d]{4}))",
             "mobile": "(((4(44[0-25-9])|(6(1[0-7])|(4[0-57-9])|(6[0-4])))|(5(73[0-6])|(95[0-8]))|(6(26[013-8])|(66[0-3]))|(70(7[1-8])|(8[0-4]))|(848[0-35-9])|(9(29[013-9])|(39[01])|(59[0-4])|(899))[\\d]{4})|((4(4[0-35-8])|(6[02357-9]))|(5([1-59][0-46-9])|(6[0-4689])|(7[0-246-9]))|(6(0[1-9])|([13-59][\\d])|([268][0-57-9])|(7[0-79]))|(70[129])|(84[0-29])|(9(0[1-9])|(1[02-9])|([2358][0-8])|([467][\\d]))[\\d]{5}))",
         },
         "HN": {
@@ -789,15 +789,15 @@
             "code": "687",
             "pattern": "(((2[03-9])|(3[0-5])|(4[1-7])|(88)[\\d]{4}))",
             "mobile": "(((5[0-4])|([79][\\d])|(8[0-79])[\\d]{4}))",
         },
         "NE": {
             "code": "227",
             "pattern": "((2(0(20)|(3[1-8])|(4[13-5])|(5[14])|(6[14578])|(7[1-578]))|(1(4[145])|(5[14])|(6[14-68])|(7[169])|(88))[\\d]{4}))",
-            "mobile": "(((23)|(7[047])|([89][\\d])[\\d]{6}))",
+            "mobile": "(((23)|(7[0467])|([89][\\d])[\\d]{6}))",
         },
         "NF": {
             "code": "672",
             "pattern": "(((1(06)|(17)|(28)|(39))|(3[0-2][\\d])[\\d]{3}))",
             "mobile": "(((14)|(3[58])[\\d]{4}))",
         },
         "NG": {
@@ -919,15 +919,15 @@
             "code": "262",
             "pattern": "((26(2[\\d][\\d])|(3(0[\\d])|(1[0-6]))[\\d]{4}))",
             "mobile": "((69(2[\\d][\\d])|(3([06][0-6])|(1[013])|(2[0-2])|(3[0-39])|(4[\\d])|(5[0-5])|(7[0-37])|(8[0-8])|(9[0-479]))[\\d]{4}))",
         },
         "RO": {
             "code": "40",
             "pattern": "(([23][13-6][\\d]{7})|((2(19[\\d])|([3-6][\\d]9))|(31[\\d][\\d])[\\d][\\d]))",
-            "mobile": "((7020[\\d]{5})|((6([04]0)|(2[\\d]))|(7(0[013-9])|(1[0-3])|([2-7][\\d])|(8[03-8])|(9[0-39]))[\\d]{6}))",
+            "mobile": "(((630)|(702)0[\\d]{5})|((6([04]0)|(2[\\d]))|(7(0[013-9])|(1[0-3])|([2-7][\\d])|(8[03-8])|(9[0-39]))[\\d]{6}))",
         },
         "RS": {
             "code": "381",
             "pattern": "(((11[1-9][\\d])|((2[389])|(39)(0[2-9])|([2-9][\\d]))[\\d]{3:8})|((1[02-9])|(2[0-24-7])|(3[0-8])[2-9][\\d]{4:9}))",
             "mobile": "((6([0-689])|(7[\\d])[\\d]{6:7}))",
         },
         "RU": {
```

### Comparing `phone_gen-2.4.5/phone_gen.egg-info/PKG-INFO` & `phone_gen-2.4.6/phone_gen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phone_gen
-Version: 2.4.5
+Version: 2.4.6
 Summary: International phone number generation
 Home-page: https://github.com/tolstislon/phone-gen
 Author: tolstislon
 Author-email: tolstislon@gmail.com
 License: MIT License
 Keywords: testing,test-data,phone-number,phone,test-data-generator
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `phone_gen-2.4.5/phone_gen.egg-info/SOURCES.txt` & `phone_gen-2.4.6/phone_gen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/setup.py` & `phone_gen-2.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/tests/test_alt_pattern.py` & `phone_gen-2.4.6/tests/test_alt_pattern.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/tests/test_cli.py` & `phone_gen-2.4.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/tests/test_generator.py` & `phone_gen-2.4.6/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/tests/test_load_alt_patterns.py` & `phone_gen-2.4.6/tests/test_load_alt_patterns.py`

 * *Files identical despite different names*

### Comparing `phone_gen-2.4.5/tests/test_phone.py` & `phone_gen-2.4.6/tests/test_phone.py`

 * *Files identical despite different names*

