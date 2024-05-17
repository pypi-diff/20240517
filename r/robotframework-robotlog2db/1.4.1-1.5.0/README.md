# Comparing `tmp/robotframework-robotlog2db-1.4.1.tar.gz` & `tmp/robotframework-robotlog2db-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robotlog2db-1.4.1.tar", last modified: Tue Apr  9 15:50:30 2024, max compression
+gzip compressed data, was "robotframework-robotlog2db-1.5.0.tar", last modified: Fri May 17 09:01:10 2024, max compression
```

## Comparing `robotframework-robotlog2db-1.4.1.tar` & `robotframework-robotlog2db-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10865 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/RobotLog2DB/
--rw-r--r--   0 runner    (1001) docker     (127)    41226 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (127)   606978 2024-04-09 15:50:29.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/RobotLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46378 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/robotlog2db.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/RobotLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/RobotLog2DB/xsd/robot.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11444 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-09 15:50:30.000000 robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:50:30.194208 robotframework-robotlog2db-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-04-09 15:48:49.000000 robotframework-robotlog2db-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:01:10.240848 robotframework-robotlog2db-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-05-17 09:01:10.240848 robotframework-robotlog2db-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10941 2024-05-17 08:59:31.000000 robotframework-robotlog2db-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:01:10.236848 robotframework-robotlog2db-1.5.0/RobotLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (127)   586038 2024-05-17 09:01:09.000000 robotframework-robotlog2db-1.5.0/RobotLog2DB/RobotLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 08:59:31.000000 robotframework-robotlog2db-1.5.0/RobotLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-17 08:59:31.000000 robotframework-robotlog2db-1.5.0/RobotLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46549 2024-05-17 08:59:31.000000 robotframework-robotlog2db-1.5.0/RobotLog2DB/robotlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-17 08:59:31.000000 robotframework-robotlog2db-1.5.0/RobotLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:01:10.236848 robotframework-robotlog2db-1.5.0/RobotLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-05-17 08:59:31.000000 robotframework-robotlog2db-1.5.0/RobotLog2DB/xsd/robot.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 09:01:10.240848 robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11522 2024-05-17 09:01:10.000000 robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-17 09:01:10.000000 robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 09:01:10.000000 robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 09:01:10.000000 robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-17 09:01:10.000000 robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 09:01:10.000000 robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 09:01:10.240848 robotframework-robotlog2db-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9364 2024-05-17 08:59:31.000000 robotframework-robotlog2db-1.5.0/setup.py
```

### Comparing `robotframework-robotlog2db-1.4.1/PKG-INFO` & `robotframework-robotlog2db-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.4.1
+Version: 1.5.0
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -156,14 +156,16 @@
     --recursive          if set, then the path is searched recursively for output files to be imported.
     --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
     --append             is used in combination with --UUID <UUID>.If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
     --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided RobotLog2DB will generate an UUID for the whole import.
     --variant VARIANT    variant name to be set for this import.
     --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
     --config CONFIG      configuration json file for component mapping information.
+    --interface {db,rest}
+                         database access interface.
 
 The below command is simple usage with all required arguments to import
 Robot Framework results into TestResultWebApp\'s database:
 
     RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
```

### Comparing `robotframework-robotlog2db-1.4.1/README.rst` & `robotframework-robotlog2db-1.5.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,16 @@
    --recursive          if set, then the path is searched recursively for output files to be imported.
    --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
    --append             is used in combination with --UUID <UUID>.If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
    --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided RobotLog2DB will generate an UUID for the whole import.
    --variant VARIANT    variant name to be set for this import.
    --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
    --config CONFIG      configuration json file for component mapping information.
+   --interface {db,rest}
+                        database access interface.
 
 
 The below command is simple usage with all required arguments to import
 Robot Framework results into TestResultWebApp's database:
 
 ::
```

### Comparing `robotframework-robotlog2db-1.4.1/RobotLog2DB/RobotLog2DB.pdf` & `robotframework-robotlog2db-1.5.0/RobotLog2DB/RobotLog2DB.pdf`

 * *Files 15% similar despite different names*

#### Comparing `robotframework-robotlog2db-1.4.1/RobotLog2DB/RobotLog2DB.pdf` & `robotframework-robotlog2db-1.5.0/RobotLog2DB/RobotLog2DB.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20240409155028Z'
+CreationDate: 'D:20240517090108Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20240409155028Z'
+ModDate: 'D:20240517090108Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 RobotLog2DB
-v. 1.4.1
+v. 1.5.0
 Tran Duy Ngoan
-15.03.2024
+22.04.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -74,260 +74,143 @@
 
 2.2.5
 
 Append to existing execution result . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 8
 
-Display on WebApp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-10
-
-3 CDataBase.py
-3.1
+2.2.6
 
-11
+Switch Database Access Interface . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-Class: CDataBase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+9
 
-11
+Display on WebApp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-3.1.1
+10
 
-Method: connect . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3 robotlog2db.py
 
 11
 
-3.1.2
-
-Method: disconnect . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-12
-
-3.1.3
-
-Method: cleanAllTables . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-12
-
-3.1.4
-
-Method: sCreateNewTestResult . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-12
-
-3.1.5
-
-Method: nCreateNewFile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-13
-
-3.1.6
-
-Method: vCreateNewHeader . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-14
-
-3.1.7
-
-Method: nCreateNewSingleTestCase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-16
-
-3.1.8
-
-Method: nCreateNewTestCase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-17
-
-3.1.9
-
-Method: vCreateTags . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-18
-
-3.1.10 Method: vSetCategory . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-18
-
-3.1.11 Method: vUpdateStartEndTime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-19
-
-3.1.12 Method: arGetCategories . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-19
-
-3.1.13 Method: vCreateAbortReason . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-19
-
-3.1.14 Method: vCreateReanimation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-20
-
-3.1.15 Method: vCreateCCRdata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-20
-
-3.1.16 Method: vFinishTestResult . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-20
-
-3.1.17 Method: vUpdateEvtbls . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-20
-
-3.1.18 Method: vUpdateEvtbl . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-21
-
-3.1.19 Method: vEnableForeignKeyCheck . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-21
-
-3.1.20 Method: sGetLatestFileID . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-21
-
-A
-
-CONTENTS
-
-CONTENTS
-
-3.1.21 Method: vUpdateFileEndTime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-21
-
-3.1.22 Method: vUpdateResultEndTime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-22
-
-3.1.23 Method: bExistingResultID . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-22
-
-3.1.24 Method: arGetProjectVersionSWByID . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-22
-
-4 robotlog2db.py
-
-23
-
-4.1
+3.1
 
 Function: collect xml result files . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-23
+11
 
-4.2
+3.2
 
 Function: validate xml result . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-23
+11
 
-4.3
+3.3
 
 Function: is valid uuid . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-24
+12
 
-4.4
+3.4
 
 Function: is valid config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-24
+12
 
-4.5
+3.5
 
 Function: get from tags . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+13
 
-4.6
+3.6
 
 Function: get branch from swversion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+13
 
-4.7
+3.7
 
 Function: format time . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+13
 
-4.8
+3.8
 
 Function: retrieve result starttime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+14
 
-4.9
+3.9
 
 Function: retrieve result endtime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+14
 
-4.10 Function: process suite metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.10 Function: process suite metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+14
 
-4.11 Function: process metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.11 Function: process metadata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-27
+15
 
-4.12 Function: process suite . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.12 Function: process suite . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-27
+15
 
-4.13 Function: process test . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.13 Function: process test . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-28
+16
 
-4.14 Function: process config file . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.14 Function: process config file . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-28
+16
 
-4.15 Function: normalize path . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.15 Function: normalize path . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-29
+17
 
-4.16 Function: RobotLog2DB . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.16 Function: RobotLog2DB . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-29
+17
 
-4.17 Class: Logger . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.17 Class: Logger . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-30
+18
 
-4.17.1 Method: config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.17.1 Method: config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-30
+18
 
-4.17.2 Method: log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.17.2 Method: log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-30
+18
 
-4.17.3 Method: log warning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.17.3 Method: log warning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-31
+19
+
+A
+
+CONTENTS
 
-4.17.4 Method: log error . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+CONTENTS
 
-31
+3.17.4 Method: log error . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-5 Appendix
+19
 
-32
+4 Appendix
 
-6 History
+20
 
-33
+5 History
+
+21
 
 B
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
@@ -602,21 +485,14 @@
 database
 database schema for database login.
 optional arguments:
 -h, --help
 -v, --version
 --recursive
 --dryrun
---append
-
---UUID UUID
-
---variant VARIANT
---versions VERSIONS
---config CONFIG
 
 show this help message and exit
 version of the RobotLog2DB importer.
 if set, then the path is searched recursively for output
 files to be imported.
 if set, then verify all input arguments (includes DB
 connection) and show what would be done.
@@ -627,14 +503,25 @@
 If not provided RobotLog2DB will generate an UUID for the
 whole import.
 variant name to be set for this import.
 metadata: Versions (Software;Hardware;Test) to be set for
 this import (semicolon separated).
 configuration json file for component mapping information.
 
+--append
+
+--UUID UUID
+
+--variant VARIANT
+--versions VERSIONS
+--config CONFIG
+--interface {db,rest}
+
+database access interface.
+
 As above instruction, RobotLog2DB tool requires 5 positional arguments which contains all required information
 for inporting.
 The below command is simple usage with all required arguments to import robot results into TestResultWebApp’s
 database:
 RobotLog2DB output.xml localhost db user db pw db name
 
 Besides the executable file RobotLog2DB you can also run tool as a Python module
@@ -854,14 +741,48 @@
 project / variant ,
 version_sw
 are provided within
 --variant VARIANT , --versions VERSIONS or --config CONFIG arguments, they will be validated with the existing values in database.
 An error will be raised in case the given value is not matched with the existing ones. E.g:
 FATAL ERROR: Given version software 'my_version' is different with existing ←,→ value 'SW01' in database.
 
+2.2.6
+
+Switch Database Access Interface
+
+In addition to direct database connections — which can sometimes be restricted or prohibited due to security concerns
+— the RobotLog2DB tool also provides users with an alternative way (interface) to import test data into the
+database, namely the REST API.
+--interface INTERFACE : An optional argument to specify the database backend interface. The default value is
+db (direct connection to MySQL database). It can also be set to rest to import data into the database via a
+
+REST API.
+Direct Connection Backend (interface=”db”)
+The default mode of operation for the import tool is the direct connection to the MySQL database. This means
+that when you run the tool without specifying the --interface option, it automatically uses the db interface,
+establishing a direct connection to the MySQL database.
+You can also explicitly specify the db interface by using the --interface option with the value db .
+RobotLog2DB output.xml db host db user db password db name --interface db
+
+This method provides flexibility, allowing users to choose between interfaces explicitly or rely on the default behavior.
+REST API Backend (interface=”rest”)
+The ’rest’ interface allows users to import data into the database through a REST API. This mode is particularly
+useful in scenarios where direct database connections are restricted or not feasible, such as when the database is
+secured and direct connections are not allowed.
+RobotLog2DB output.xml api endpoint api user api password db name --interface rest
+
+Additional Notes
+
+!
+
+This feature offers easy switching between database backends, making it transparent and convenient for
+end-users.
+When using the REST API interface, ensure that you have the necessary credentials and permissions to
+access the REST API endpoints.
+
 9
 
 CHAPTER 2. DESCRIPTION
 
 2.3
 
 2.3. DISPLAY ON WEBAPP
@@ -877,778 +798,20 @@
 Figure 2.1: Dashboard view
 Suite/File metadata and test case information:
 
 Figure 2.2: Datatable view
 
 10
 
-CHAPTER 3. CDATABASE.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
 Chapter 3
 
-CDataBase.py
-3.1
-
-Class: CDataBase
-
-Imported by:
-from RobotLog2DB.CDataBase import CDataBase
-CDataBase class play a role as mysqlclient and provide methods to interact with TestResultWebApp’s database.
-
-3.1.1
-
-Method: connect
-
-Connect to the database with provided authentication and db info.
-Arguments:
- host
-
-/ Condition: required / Type: str /
-URL which is hosted the TestResultWebApp’s database.
- user
-
-/ Condition: required / Type: str /
-User name for database authentication.
- passwd
-
-/ Condition: required / Type: str /
-User’s password for database authentication.
- database
-
-/ Condition: required / Type: str /
-Database name.
- charset
-
-/ Condition: optional / Type: str / Default: ’utf8’ /
-The connection character set.
- use unicode
-
-/ Condition: optional / Type: bool / Default: True /
-If True, CHAR and VARCHAR and TEXT columns are returned as Unicode strings, using the configured
-character set.
-Returns:
-(no returns)
-
-11
-
-CHAPTER 3. CDATABASE.PY
-
-3.1.2
-
-3.1. CLASS: CDATABASE
-
-Method: disconnect
-
-Disconnect from TestResultWebApp’s database.
-Arguments:
-(no arguments)
-Returns:
-(no returns)
-
-3.1.3
-
-Method: cleanAllTables
-
-Delete all table data. Please be careful before calling this method.
-Arguments:
-(no arguments)
-Returns:
-(no returns)
-
-3.1.4
-
-Method: sCreateNewTestResult
-
-Creates a new test result in tbl result. This is the main table which is linked to all other data by means of
-test result id.
-Arguments:
- tbl prj project
-
-/ Condition: required / Type: str /
-Project information.
- tbl prj variant
-
-/ Condition: required / Type: str /
-Variant information.
- tbl prj branch
-
-/ Condition: required / Type: str /
-Branch information.
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
- tbl result interpretation
-
-/ Condition: required / Type: str /
-Result interpretation.
- tbl result time start
-
-/ Condition: required / Type: str /
-Test result start time as format %Y-%m-%d %H:%M:%S.
- tbl result time end
-
-/ Condition: required / Type: str /
-Test result end time as format %Y-%m-%d %H:%M:%S.
- tbl result version sw target
-
-/ Condition: required / Type: str /
-Software version information.
-
-12
-
-CHAPTER 3. CDATABASE.PY
-
-3.1. CLASS: CDATABASE
-
- tbl result version sw test
-
-/ Condition: required / Type: str /
-Test version information.
- tbl result version target
-
-/ Condition: required / Type: str /
-Hardware version information.
- tbl result jenkinsurl
-
-/ Condition: required / Type: str /
-Jenkinsurl in case test result is executed by jenkins.
- tbl result reporting qualitygate
-
-/ Condition: required / Type: str /
-Qualitygate information for reporting.
-Returns:
- tbl test result id
-
-/ Type: str /
-test result id of new test result.
-
-3.1.5
-
-Method: nCreateNewFile
-
-Create new file entry in tbl file table.
-Arguments:
- tbl file name
-
-/ Condition: required / Type: str /
-File name information.
- tbl file tester account
-
-/ Condition: required / Type: str /
-Tester account information.
- tbl file tester machine
-
-/ Condition: required / Type: str /
-Test machine information.
- tbl file time start
-
-/ Condition: required / Type: str /
-Test file start time as format %Y-%m-%d %H:%M:%S.
- tbl file time end
-
-/ Condition: required / Type: str /
-Test file end time as format %Y-%m-%d %H:%M:%S.
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result for linking to tbl result table.
- tbl file origin
-
-/ Condition: required / Type: str /
-Origin (test framework) of test file. Deafult is ”ROBFW”
-Returns:
- iInsertedID
-
-/ Type: int /
-ID of new entry.
-13
-
-CHAPTER 3. CDATABASE.PY
-
-3.1.6
-
-3.1. CLASS: CDATABASE
-
-Method: vCreateNewHeader
-
-Create a new header entry in tbl file header table which is linked with the file.
-Arguments:
- tbl file id
-
-/ Condition: required / Type: int /
-File ID information.
- tbl header testtoolconfiguration testtoolname
-
-/ Condition: required / Type: str /
-Test tool name.
- tbl header testtoolconfiguration testtoolversionstring
-
-/ Condition: required / Type: str /
-Test tool version.
- tbl header testtoolconfiguration projectname
-
-/ Condition: required / Type: str /
-Project name.
- tbl header testtoolconfiguration logfileencoding
-
-/ Condition: required / Type: str /
-Encoding of logfile.
- tbl header testtoolconfiguration pythonversion
-
-/ Condition: required / Type: str /
-Python version info.
- tbl header testtoolconfiguration testfile
-
-/ Condition: required / Type: str /
-Test file name.
- tbl header testtoolconfiguration logfilepath
-
-/ Condition: required / Type: str /
-Path to log file.
- tbl header testtoolconfiguration logfilemode
-
-/ Condition: required / Type: str /
-Mode of log file.
- tbl header testtoolconfiguration ctrlfilepath
-
-/ Condition: required / Type: str /
-Path to control file.
- tbl header testtoolconfiguration configfile
-
-/ Condition: required / Type: str /
-Path to configuration file.
- tbl header testtoolconfiguration confname
-
-/ Condition: required / Type: str /
-Configuration name.
- tbl header testfileheader author
-
-/ Condition: required / Type: str /
-File author.
-
-14
-
-CHAPTER 3. CDATABASE.PY
-
-3.1. CLASS: CDATABASE
-
- tbl header testfileheader project
-
-/ Condition: required / Type: str /
-Project information.
- tbl header testfileheader testfiledate
-
-/ Condition: required / Type: str /
-File creation date.
- tbl header testfileheader version major
-
-/ Condition: required / Type: str /
-File major version.
- tbl header testfileheader version minor
-
-/ Condition: required / Type: str /
-File minor version.
- tbl header testfileheader version patch
-
-/ Condition: required / Type: str /
-File patch version.
- tbl header testfileheader keyword
-
-/ Condition: required / Type: str /
-File keyword.
- tbl header testfileheader shortdescription
-
-/ Condition: required / Type: str /
-File short description.
- tbl header testexecution useraccount
-
-/ Condition: required / Type: str /
-Tester account who run the execution.
- tbl header testexecution computername
-
-/ Condition: required / Type: str /
-Machine name which is executed on.
- tbl header testrequirements documentmanagement
-
-/ Condition: required / Type: str /
-Requirement management information.
- tbl header testrequirements testenvironment
-
-/ Condition: required / Type: str /
-Requirement environment information.
- tbl header testbenchconfig name
-
-/ Condition: required / Type: str /
-Testbench configuration name.
- tbl header testbenchconfig data
-
-/ Condition: required / Type: str /
-Testbench configuration data.
- tbl header preprocessor filter
-
-/ Condition: required / Type: str /
-Preprocessor filter information.
- tbl header preprocessor parameters
-
-/ Condition: required / Type: str /
-Preprocessor parameters definition.
-Returns:
-(no returns)
-15
-
-CHAPTER 3. CDATABASE.PY
-
-3.1.7
-
-3.1. CLASS: CDATABASE
-
-Method: nCreateNewSingleTestCase
-
-Create single testcase entry in tbl case table immediately.
-Arguments:
- tbl case name
-
-/ Condition: required / Type: str /
-Test case name.
- tbl case issue
-
-/ Condition: required / Type: str /
-Test case issue ID.
- tbl case tcid
-
-/ Condition: required / Type: str /
-Test case ID (used for testmanagement tool).
- tbl case fid
-
-/ Condition: required / Type: str /
-Test case requirement (function) ID.
- tbl case testnumber
-
-/ Condition: required / Type: int /
-Order of test case in file.
- tbl case repeatcount
-
-/ Condition: required / Type: int /
-Test case repeatition count.
- tbl case component
-
-/ Condition: required / Type: str /
-Component which test case is belong to.
- tbl case time start
-
-/ Condition: required / Type: str /
-Test case start time as format %Y-%m-%d %H:%M:%S.
- tbl case result main
-
-/ Condition: required / Type: str /
-Test case main result.
- tbl case result state
-
-/ Condition: required / Type: str /
-Test case completion state.
- tbl case result return
-
-/ Condition: required / Type: int /
-Test case result code (as integer).
- tbl case counter resets
-
-/ Condition: required / Type: int /
-Counter of target reset within test case execution.
- tbl case lastlog
-
-/ Condition: required / Type: str /
-Traceback information when test case is failed.
-
-16
-
-CHAPTER 3. CDATABASE.PY
-
-3.1. CLASS: CDATABASE
-
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result for linking to file in tbl result table.
- tbl file id
-
-/ Condition: required / Type: int /
-Test file ID for linking to file in tbl file table.
-Returns:
- iInsertedID
-
-/ Type: int /
-ID of new entry.
-
-3.1.8
-
-Method: nCreateNewTestCase
-
-Create bulk of test case entries: new test cases are buffered and inserted as bulk.
-Once
-
-NUM BUFFERD ELEMENTS FOR EXECUTEMANY is reached, the creation query is executed.
-
-Arguments:
- tbl case name
-
-/ Condition: required / Type: str /
-Test case name.
- tbl case issue
-
-/ Condition: required / Type: str /
-Test case issue ID.
- tbl case tcid
-
-/ Condition: required / Type: str /
-Test case ID (used for testmanagement tool).
- tbl case fid
-
-/ Condition: required / Type: str /
-Test case requirement (function) ID.
- tbl case testnumber
-
-/ Condition: required / Type: int /
-Order of test case in file.
- tbl case repeatcount
-
-/ Condition: required / Type: int /
-Test case repeatition count.
- tbl case component
-
-/ Condition: required / Type: str /
-Component which test case is belong to.
- tbl case time start
-
-/ Condition: required / Type: str /
-Test case start time as format %Y-%m-%d %H:%M:%S.
- tbl case result main
-
-/ Condition: required / Type: str /
-Test case main result.
-
-17
-
-CHAPTER 3. CDATABASE.PY
-
-3.1. CLASS: CDATABASE
-
- tbl case result state
-
-/ Condition: required / Type: str /
-Test case completion state.
- tbl case result return
-
-/ Condition: required / Type: int /
-Test case result code (as integer).
- tbl case counter resets
-
-/ Condition: required / Type: int /
-Counter of target reset within test case execution.
- tbl case lastlog
-
-/ Condition: required / Type: str /
-Traceback information when test case is failed.
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result for linking to file in tbl result table.
- tbl file id
-
-/ Condition: required / Type: int /
-Test file ID for linking to file in tbl file table.
-Returns:
-(no returns)
-
-3.1.9
-
-Method: vCreateTags
-
-Create tag entries.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
- tbl usr result tags
-
-/ Condition: required / Type: str /
-User tags information.
-Returns:
-(no returns)
-
-3.1.10
-
-Method: vSetCategory
-
-Create category entry.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
- tbl result category main
-
-/ Condition: required / Type: str /
-Category information.
-Returns:
-(no returns)
-18
-
-CHAPTER 3. CDATABASE.PY
-
-3.1.11
-
-3.1. CLASS: CDATABASE
-
-Method: vUpdateStartEndTime
-
-Create start-end time entry.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
- tbl result time start
-
-/ Condition: required / Type: str /
-Result start time as format %Y-%m-%d %H:%M:%S.
- tbl result time end
-
-/ Condition: required / Type: str /
-Result end time as format %Y-%m-%d %H:%M:%S.
-Returns:
-(no returns)
-
-3.1.12
-
-Method: arGetCategories
-
-Get existing categories.
-Arguments:
-(no arguments)
-Returns:
- arCategories
-
-/ Type: list /
-List of exsiting categories.
-
-3.1.13
-
-Method: vCreateAbortReason
-
-Create abort reason entry.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
- tbl abort reason
-
-/ Condition: required / Type: str /
-Abort reason.
- tbl abort message
-
-/ Condition: required / Type: str /
-Detail message of abort.
-Returns:
-(no returns)
-
-19
-
-CHAPTER 3. CDATABASE.PY
-
-3.1.14
-
-3.1. CLASS: CDATABASE
-
-Method: vCreateReanimation
-
-Create reanimation entry.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
- tbl num of reanimation
-
-/ Condition: required / Type: int /
-Counter of target reanimation during execution.
-Returns:
-(no returns)
-
-3.1.15
-
-Method: vCreateCCRdata
-
-Create CCR data per test case.
-Arguments:
- tbl test case id
-
-/ Condition: required / Type: int /
-test case ID.
- lCCRdata
-
-/ Condition: required / Type: list /
-list of CCR data.
-Returns:
-(no returns)
-
-3.1.16
-
-Method: vFinishTestResult
-
-Finish upload:
- First do bulk insert of rest of test cases if buffer is not empty.
- Then set state to ”new report”.
-
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
-Returns:
-(no returns)
-
-3.1.17
-
-Method: vUpdateEvtbls
-
-Call update evtbls stored procedure.
-Arguments:
-(no arguments)
-Returns:
-(no returns)
-20
-
-CHAPTER 3. CDATABASE.PY
-
-3.1.18
-
-3.1. CLASS: CDATABASE
-
-Method: vUpdateEvtbl
-
-Call update evtbl stored procedure to update provided test result id.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
-Returns:
-(no returns)
-
-3.1.19
-
-Method: vEnableForeignKeyCheck
-
-Switch foreign key checks flag.
-Arguments:
- enable
-
-/ Condition: optional / Type: bool / Default: True /
-If True, enable foreign key constraint.
-Returns:
-(no returns)
-
-3.1.20
-
-Method: sGetLatestFileID
-
-Get latest file ID from tbl file table.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-UUID of test result.
-Returns:
- tbl file id
-
-/ Type: int /
-File ID.
-
-3.1.21
-
-Method: vUpdateFileEndTime
-
-Update test file end time.
-Arguments:
- tbl file id
-
-/ Condition: required / Type: int /
-File ID to be updated.
- tbl file time end
-
-/ Condition: required / Type: str /
-File end time as format %Y-%m-%d %H:%M:%S.
-Returns:
-(no returns)
-21
-
-CHAPTER 3. CDATABASE.PY
-
-3.1.22
-
-3.1. CLASS: CDATABASE
-
-Method: vUpdateResultEndTime
-
-Update test result end time.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-Result UUID to be updated.
- tbl result time end
-
-/ Condition: required / Type: str /
-Result end time as format %Y-%m-%d %H:%M:%S.
-Returns:
-(no returns)
-
-3.1.23
-
-Method: bExistingResultID
-
-Verify the given test result UUID is existing in tbl result table or not.
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-Result UUID to be verified.
-Returns:
- bExisting
-
-/ Type: bool /
-True if test result UUID is already existing.
-
-3.1.24
-
-Method: arGetProjectVersionSWByID
-
-Get the project and version sw information of given test result id
-Arguments:
- tbl test result id
-
-/ Condition: required / Type: str /
-Result UUID to be get the information.
-Returns:
- / Type: tuple /
-
-None if test result UUID is not existing, else the tuple which contains project and version sw: (project, variant)
-is returned.
-
-22
-
-CHAPTER 4. ROBOTLOG2DB.PY
-
-Chapter 4
-
 robotlog2db.py
-4.1
+3.1
 
 Function: collect xml result files
 
 Collect all valid Robot xml result file in given path.
 Arguments:
  path
 
@@ -1660,15 +823,15 @@
 If set, the given path is searched recursively for xml result files.
 Returns:
  lFoundFiles
 
 / Type: list /
 List of valid xml result file(s) in given path.
 
-4.2
+3.2
 
 Function: validate xml result
 
 Verify the given xml result file is valid or not.
 Arguments:
  xml result
 
@@ -1682,21 +845,21 @@
 
 / Condition: optional / Type: bool / Default: True /
 If set, exit with fatal error if the schema validation of given xml file failed.
 Returns:
  / Type: bool /
 
 True if the given xml result is valid with the provided schema *.xsd.
-23
+11
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.3
+3.3
 
-4.3. FUNCTION: IS VALID UUID
+3.3. FUNCTION: IS VALID UUID
 
 Function: is valid uuid
 
 Verify the given UUID is valid or not.
 Arguments:
  uuid to test
 
@@ -1708,15 +871,15 @@
 UUID version.
 Returns:
  bValid
 
 / Type: bool /
 True if the given UUID is valid.
 
-4.4
+3.4
 
 Function: is valid config
 
 Validate the json configuration base on given schema.
 Default schema supports below information:
 CONFIG SCHEMA = {
 "components": [str, dict],
@@ -1744,21 +907,21 @@
 If True, exit tool in case the validation is fail.
 Returns:
  bValid
 
 / Type: bool /
 True if the given json configuration data is valid.
 
-24
+12
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.5
+3.5
 
-4.5. FUNCTION: GET FROM TAGS
+3.5. FUNCTION: GET FROM TAGS
 
 Function: get from tags
 
 Extract testcase information from tags.
 Example: TCID-xxxx, FID-xxxx, ...
 Arguments:
  lTags
@@ -1771,15 +934,15 @@
 Regex to get the expectated info (ID) from tag info.
 Returns:
  lInfo
 
 / Type: list /
 List of expected information (ID)
 
-4.6
+3.6
 
 Function: get branch from swversion
 
 Get branch name from software version information.
 Convention of branch information in suffix of software version:
  All software version with .0F is the main/freature branch. The leading number is the current year. E.g.
 17.0F03
@@ -1793,36 +956,36 @@
 Software version.
 Returns:
  branch name
 
 / Type: str /
 Branch name.
 
-4.7
+3.7
 
 Function: format time
 
 Format the given time string to TestResultWebApp’s format for importing to db.
 Arguments:
  stime
 
 / Condition: required / Type: str /
 String of time.
 Returns:
  sFormatedTime
 
 / Type: str /
 TestResultWebApp’s time as format %Y-%m-%d %H:%M:%S.
-25
+13
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.8
+3.8
 
-4.8. FUNCTION: RETRIEVE RESULT STARTTIME
+3.8. FUNCTION: RETRIEVE RESULT STARTTIME
 
 Function: retrieve result starttime
 
 Retrieve starttime infomration from given result object (TestSuite or TestCase). In case the starttime in given suite
 is ’N/A’, it will try to get this information from its children suite/test.
 Arguments:
  stime
@@ -1832,29 +995,29 @@
 Returns:
  / Type: str /
 
 Start time of given result.
 
 Function: retrieve result endtime
 
-4.9
+3.9
 
 Retrieve endtime infomration from given result object (TestSuite or TestCase). In case the endtime in given suite is
 ’N/A’, it will try to get this information from its children suite/test.
 Arguments:
  stime
 
 / Condition: required / Type: TestSuite or TestCase object /
 Result object to retrieve endtime.
 Returns:
  / Type: str /
 
 End time of given result.
 
-4.10
+3.10
 
 Function: process suite metadata
 
 Try to find metadata information from all suite levels.
 Metadata at top suite level has a highest priority.
 Arguments:
  suite
@@ -1867,21 +1030,21 @@
 Initial Metadata information for updating.
 Returns:
  dMetadata
 
 / Type: dict /
 Dictionary of Metadata information.
 
-26
+14
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.11
+3.11
 
-4.11. FUNCTION: PROCESS METADATA
+3.11. FUNCTION: PROCESS METADATA
 
 Function: process metadata
 
 Extract metadata from suite result bases on DEFAULT METADATA.
 Arguments:
  metadata
 
@@ -1893,15 +1056,15 @@
 Initial Metadata information for updating.
 Returns:
  dMetadata
 
 / Type: dict /
 Dictionary of Metadata information.
 
-4.12
+3.12
 
 Function: process suite
 
 Process to the lowest suite level (test file):
  Create new file and its header information
  Then, process all child test cases
 
@@ -1925,21 +1088,21 @@
  dConfig
 
 / Condition: required / Type: dict / Default: None /
 Configuration data which is parsed from given json configuration file.
 Returns:
 (no returns)
 
-27
+15
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.13
+3.13
 
-4.13. FUNCTION: PROCESS TEST
+3.13. FUNCTION: PROCESS TEST
 
 Function: process test
 
 Process test case data and create new test case record.
 Arguments:
  db
 
@@ -1964,15 +1127,15 @@
  test number
 
 / Condition: required / Type: int /
 Order of test case in file.
 Returns:
 (no returns)
 
-4.14
+3.14
 
 Function: process config file
 
 Parse information from configuration file:
  component:
 
 {
@@ -1987,46 +1150,46 @@
 }
 Then all testcases which their paths contain componentA/path/to/testcase will be belong to
 componentA, ...
  variant, version sw: configuration file has low priority than command line.
 
 Arguments:
 
-28
+16
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.15. FUNCTION: NORMALIZE PATH
+3.15. FUNCTION: NORMALIZE PATH
 
  config file
 
 / Condition: required / Type: str /
 Path to configuration file.
 Returns:
  dConfig
 
 / Type: dict /
 Configuration object.
 
-4.15
+3.15
 
 Function: normalize path
 
 Normalize path file.
 Arguments:
  sPath
 
 / Condition: required / Type: str /
 Path file to be normalized.
  sNPath
 
 / Type: str /
 Normalized path file.
 
-4.16
+3.16
 
 Function: RobotLog2DB
 
 Import robot results from output.xml to TestResultWebApp’s database.
 Flow to import Robot results to database:
 1. Process provided arguments from command line.
 2. Parse Robot results.
@@ -2044,35 +1207,35 @@
 – password : password for database login.
 – database : database name.
 – recursive : if True, then the path is searched recursively for log files to be imported.
 – dryrun : if True, then verify all input arguments (includes DB connection) and show what would be done.
 – append : if True, then allow to append new result(s) to existing execution result UUID which is provided
 by --UUID argument.
 – UUID : UUID used to identify the import and version ID on TestResultWebApp.
-29
+17
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.17. CLASS: LOGGER
+3.17. CLASS: LOGGER
 
 – variant : variant name to be set for this import.
 – versions : metadata: Versions (Software;Hardware;Test) to be set for this import.
 – config : configuration json file for component mapping information.
 Returns:
 (no returns)
 
-4.17
+3.17
 
 Class: Logger
 
 Imported by:
 from RobotLog2DB.robotlog2db import Logger
 Logger class for logging message.
 
-4.17.1
+3.17.1
 
 Method: config
 
 Configure Logger class.
 Arguments:
  output console
 
@@ -2085,15 +1248,15 @@
  dryrun
 
 / Condition: optional / Type: bool / Default: True /
 If set, a prefix as ’dryrun’ is added for all messages.
 Returns:
 (no returns)
 
-4.17.2
+3.17.2
 
 Method: log
 
 Write log message to console/file output.
 Arguments:
  msg
 
@@ -2105,34 +1268,34 @@
 Color style for the message.
  indent
 
 / Condition: optional / Type: int / Default: 0 /
 Offset indent.
 Returns:
 (no returns)
-30
+18
 
-CHAPTER 4. ROBOTLOG2DB.PY
+CHAPTER 3. ROBOTLOG2DB.PY
 
-4.17.3
+3.17.3
 
-4.17. CLASS: LOGGER
+3.17. CLASS: LOGGER
 
 Method: log warning
 
 Write warning message to console/file output.
 Arguments:
  msg
 
 / Condition: required / Type: str /
 Warning message which is written to output.
 Returns:
 (no returns)
 
-4.17.4
+3.17.4
 
 Method: log error
 
 Write error message to console/file output.
 Arguments:
  msg
 
@@ -2141,38 +1304,38 @@
  fatal error
 
 / Condition: optional / Type: bool / Default: False /
 If set, tool will terminate after logging error message.
 Returns:
 (no returns)
 
-31
+19
 
-CHAPTER 5. APPENDIX
+CHAPTER 4. APPENDIX
 
-Chapter 5
+Chapter 4
 
 Appendix
 About this package:
-Table 5.1: Package setup
+Table 4.1: Package setup
 Setup parameter
 
 Value
 
 Name
 
 RobotLog2DB
 
 Version
 
-1.4.1
+1.5.0
 
 Date
 
-15.03.2024
+22.04.2024
 
 Description
 
 Imports robot result(s) to TestResultWebApp database
 
 Package URL
 
@@ -2210,19 +1373,19 @@
 
 Intended Audience :: Developers
 
 Topic
 
 Topic :: Software Development
 
-32
+20
 
-CHAPTER 6. HISTORY
+CHAPTER 5. HISTORY
 
-Chapter 6
+Chapter 5
 
 History
 0.1.0
 
 07/2022
 
 Initial version
@@ -2292,17 +1455,17 @@
 - Add try/except for database access
 1.3.7
 
 14.06.2023
 
 Update README with new instruction for installation and image’s links
 
-33
+21
 
-CHAPTER 6. HISTORY
+CHAPTER 5. HISTORY
 
 1.3.8
 
 21.06.2023
 
 Fix issue with suite.starttime at root suite is N/A
 1.3.9
@@ -2318,23 +1481,35 @@
 Adaption for Robotframework 6.1 with change of
 datatype
 
 TestSuite.source
 
 15.03.2024
 1.4.1
-update robot.xsd
+Update robot.xsd
 framework
+1.5.0
 
 schema to support the new log level
 
+USER
+
+of Robot-
+
+22.04.2024
+
+Add optional argument
+and rest interfaces
+
+--interface
+
+which allow to switch between
+
 RobotLog2DB.pdf
-Created at 09.04.2024 - 15:50:26
+Created at 17.05.2024 - 09:01:06
 by GenPackageDoc v. 0.41.1
 
-34
-
-USER
+22
 
-of Robot-
+db
```

### Comparing `robotframework-robotlog2db-1.4.1/RobotLog2DB/__init__.py` & `robotframework-robotlog2db-1.5.0/RobotLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.1/RobotLog2DB/__main__.py` & `robotframework-robotlog2db-1.5.0/RobotLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.1/RobotLog2DB/robotlog2db.py` & `robotframework-robotlog2db-1.5.0/RobotLog2DB/robotlog2db.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 import os
 import sys
 import colorama as col
 import json
 
 from lxml import etree
 from robot.api import ExecutionResult
-from RobotLog2DB.CDataBase import CDataBase
+from TestResultDBAccess import DBAccessFactory
 from RobotLog2DB.version import VERSION, VERSION_DATE
 
 DRESULT_MAPPING = {
    "PASS":  "Passed",
    "FAIL":  "Failed",
    "UNKNOWN": "Unknown"
 }
@@ -684,14 +684,15 @@
                                 'If not provided RobotLog2DB will generate an UUID for the whole import.')
    cmdParser.add_argument('--variant', type=str,
                            help='variant name to be set for this import.')
    cmdParser.add_argument('--versions', type=str,
                            help='metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).')
    cmdParser.add_argument('--config', type=str,
                            help='configuration json file for component mapping information.')
+   cmdParser.add_argument('--interface', choices=['db', 'rest'], default='db', help='database access interface.')
 
    return cmdParser.parse_args()
 
 def process_suite_metadata(suite, default_metadata=DEFAULT_METADATA):
    """
 Try to find metadata information from all suite levels.
 
@@ -1025,15 +1026,15 @@
    except Exception:
       Logger.log_error(f"Invalid Robotframework result state '{test.status}' of test '{_tbl_case_name}'.")
       return
    _tbl_case_result_state   = "complete"
    _tbl_case_result_return  = 11
    _tbl_case_counter_resets = 0
    try:
-      _tbl_case_lastlog = base64.b64encode(test.message.encode())
+      _tbl_case_lastlog = str(base64.b64encode(test.message.encode()), encoding="utf-8")
    except:
       _tbl_case_lastlog = None
    _tbl_test_result_id = test_result_id
    _tbl_file_id = file_id
 
    if not Logger.dryrun:
       try:
@@ -1225,15 +1226,15 @@
       if os.path.isfile(args.config):
          dConfig = process_config_file(args.config)
       else:
          Logger.log_error(f"The provided config file is not existing: '{args.config}'" ,
                           fatal_error=True)
 
    # 3. Connect to database
-   db=CDataBase()
+   db = DBAccessFactory().create(args.interface)
    try:
       db.connect(args.server,
                  args.user,
                  args.password,
                  args.database,
                  "utf8mb4")
    except Exception as reason:
```

### Comparing `robotframework-robotlog2db-1.4.1/RobotLog2DB/version.py` & `robotframework-robotlog2db-1.5.0/RobotLog2DB/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of RobotLog2DB
 #
-VERSION      = "1.4.1"
-VERSION_DATE = "15.03.2024"
+VERSION      = "1.5.0"
+VERSION_DATE = "22.04.2024"
```

### Comparing `robotframework-robotlog2db-1.4.1/RobotLog2DB/xsd/robot.xsd` & `robotframework-robotlog2db-1.5.0/RobotLog2DB/xsd/robot.xsd`

 * *Files identical despite different names*

### Comparing `robotframework-robotlog2db-1.4.1/robotframework_robotlog2db.egg-info/PKG-INFO` & `robotframework-robotlog2db-1.5.0/robotframework_robotlog2db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robotlog2db
-Version: 1.4.1
+Version: 1.5.0
 Summary: Imports robot result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/robotframework-robotlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -156,14 +156,16 @@
     --recursive          if set, then the path is searched recursively for output files to be imported.
     --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
     --append             is used in combination with --UUID <UUID>.If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
     --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided RobotLog2DB will generate an UUID for the whole import.
     --variant VARIANT    variant name to be set for this import.
     --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
     --config CONFIG      configuration json file for component mapping information.
+    --interface {db,rest}
+                         database access interface.
 
 The below command is simple usage with all required arguments to import
 Robot Framework results into TestResultWebApp\'s database:
 
     RobotLog2DB <resultxmlfile> <server> <user> <password> <database>
 
 Besides the executable file, you can also run tool as a Python module
```

### Comparing `robotframework-robotlog2db-1.4.1/setup.py` & `robotframework-robotlog2db-1.5.0/setup.py`

 * *Files identical despite different names*

