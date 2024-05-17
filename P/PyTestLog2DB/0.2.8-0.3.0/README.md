# Comparing `tmp/PyTestLog2DB-0.2.8.tar.gz` & `tmp/PyTestLog2DB-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTestLog2DB-0.2.8.tar", last modified: Mon Jan 15 12:25:36 2024, max compression
+gzip compressed data, was "PyTestLog2DB-0.3.0.tar", last modified: Fri May 17 08:56:02 2024, max compression
```

## Comparing `PyTestLog2DB-0.2.8.tar` & `PyTestLog2DB-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:25:36.352511 PyTestLog2DB-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-01-15 12:25:36.352511 PyTestLog2DB-0.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:25:36.352511 PyTestLog2DB-0.2.8/PyTestLog2DB/
--rw-r--r--   0 runner    (1001) docker     (127)    41226 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/PyTestLog2DB/CDataBase.py
--rw-r--r--   0 runner    (1001) docker     (127)   533245 2024-01-15 12:25:36.000000 PyTestLog2DB-0.2.8/PyTestLog2DB/PyTestLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/PyTestLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/PyTestLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43490 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/PyTestLog2DB/pytestlog2db.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/PyTestLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:25:36.352511 PyTestLog2DB-0.2.8/PyTestLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/PyTestLog2DB/xsd/junit.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-15 12:25:36.352511 PyTestLog2DB-0.2.8/PyTestLog2DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10800 2024-01-15 12:25:36.000000 PyTestLog2DB-0.2.8/PyTestLog2DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-01-15 12:25:36.000000 PyTestLog2DB-0.2.8/PyTestLog2DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-15 12:25:36.000000 PyTestLog2DB-0.2.8/PyTestLog2DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-15 12:25:36.000000 PyTestLog2DB-0.2.8/PyTestLog2DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-15 12:25:36.000000 PyTestLog2DB-0.2.8/PyTestLog2DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-15 12:25:36.352511 PyTestLog2DB-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-01-15 12:23:42.000000 PyTestLog2DB-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PyTestLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (127)   520412 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/PyTestLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43689 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/pytestlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PyTestLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/xsd/junit.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/setup.py
```

### Comparing `PyTestLog2DB-0.2.8/LICENSE` & `PyTestLog2DB-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.8/PKG-INFO` & `PyTestLog2DB-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.2.8
+Version: 0.3.0
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -152,14 +152,16 @@
     --recursive          if set, then the path is searched recursively for output files to be imported.
     --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
     --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
     --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided PyTestLog2DB will generate an UUID for the whole import.
     --variant VARIANT    variant name to be set for this import.
     --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
     --config CONFIG      configuration json file for component mapping information.
+    --interface {db,rest}
+                         database access interface.
 
 The below command is simple usage with all required arguments to import
 [pytest](https://docs.pytest.org) results into TestResultWebApp\'s
 database:
 
     PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
```

### Comparing `PyTestLog2DB-0.2.8/PyTestLog2DB/CDataBase.py` & `PyTestLog2DB-0.3.0/PyTestLog2DB/pytestlog2db.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,1494 +9,1267 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 # *******************************************************************************
 #
-# File: CDataBase.py
+# File: pytestlog2db.py
 #
-# Initialy created by Pollerspoeck Thomas (CM/PJ-CMD) / June 2016
-#
-# This class provides methods to interact with TestResultWebApp's database.
+# Initialy created by Tran Duy Ngoan(RBVH/ECM11) / November 2022
+#lxml
+# This tool is used to parse the pytest JUnit XML report file(s)
+# then import them into TestResultWebApp's database
 #
 # History:
 #
-# June 2016:
+# 2022-11-22:
 #  - initial version
 #
-# February 2022:
-#  - update sourcecode document
-#
 # *******************************************************************************
 
-import MySQLdb as db
+import re
+import uuid
+import base64
+import argparse
+import os
+import sys
+import colorama as col
+import json
+from lxml import etree
+from datetime import datetime, timedelta
+import platform
+from pkg_resources import get_distribution
 
-class CDataBase(object):
-   """
-CDataBase class play a role as mysqlclient and provide methods to interact
-with TestResultWebApp's database.
-   """
-   __single = None
+from TestResultDBAccess import DBAccessFactory
+from PyTestLog2DB.version import VERSION, VERSION_DATE
 
-   __NUM_BUFFERD_ELEMENTS_FOR_EXECUTEMANY=100
+PYTEST_DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%f"
+DB_DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
-   #make the CDataBase to singleton
-   #! __new__ requires inheritance from "object" !
-   def __new__(classtype, *args, **kwargs):
-      """
-Create object method to make singleton class ``CDataBase``.
-      """
-      # Check to see if a __single exists already for this class
-      # Compare class types instead of just looking for None so
-      # that subclasses will create their own __single objects
-      if classtype != type(classtype.__single):
-         classtype.__single = object.__new__(classtype)
-      return classtype.__single
-
-   def __init__(self):
-      """
-Initializer of class ``CDataBase``.
-      """
-      con      = None
-      db       = None
-      self.lTestCases = []
-
-   def __del__(self):
-      pass
-
-   def connect(self,host        = None,
-                    user        = None,
-                    passwd      = None,
-                    database    = None,
-                    charset     = 'utf8',
-                    use_unicode = True):
-      """
-Connect to the database with provided authentication and db info.
+def __current_user():
+   """
+Get current executing user.\
+This information is used as default value for `tester` when importing.
 
 **Arguments:**
 
-*  ``host``
-
-   / *Condition*: required / *Type*: str /
-
-   URL which is hosted the TestResultWebApp's database.
-
-*  ``user``
-
-   / *Condition*: required / *Type*: str /
-
-   User name for database authentication.
-
-*  ``passwd``
-
-   / *Condition*: required / *Type*: str /
-
-   User's password for database authentication.
-
-*  ``database``
-
-   / *Condition*: required / *Type*: str /
-
-   Database name.
-
-*  ``charset``
-
-   / *Condition*: optional / *Type*: str / *Default*: 'utf8' /
-
-   The connection character set.
-
-*  ``use_unicode``
-
-   / *Condition*: optional / *Type*: bool / *Default*: True /
-
-   If True, CHAR and VARCHAR and TEXT columns are returned as Unicode strings,
-   using the configured character set.
+(*no arguments*)
 
 **Returns:**
 
-(*no returns*)
-      """
+*  ``sUserName``
 
-      if (host==None or user==None or passwd==None or database==None):
-         raise Exception("host, user, passwd and database need to be provided!")
+   / *Type*: str /
 
-      self.db = database
+   User name of current user.
+   """
 
-      # default encoding of python is latin-1,
-      # therefore we force mysql to convert to encode to utf8.
-      self.con = db.connect(host,user,passwd,db=database,charset=charset,use_unicode=use_unicode)
-      #for test purpose activate autocommit with (True)
-      self.con.autocommit(False)
-      print("Successfully connected to: %s@%s" % (self.db, host))
+   sUserName=""
+   # allow windows system access only in windows systems
+   if platform.system().lower()!="windows":
+      try:
+         sUserName=os.getenv("USER","")
+      except Exception as reason:
+         pass
+   else:
+      import ctypes
+      try:
+         GetUserNameEx = ctypes.windll.secur32.GetUserNameExW
+         NameDisplay = 3
+
+         size = ctypes.pointer(ctypes.c_ulong(0))
+         GetUserNameEx(NameDisplay, None, size)
+
+         nameBuffer = ctypes.create_unicode_buffer(size.contents.value)
+         GetUserNameEx(NameDisplay, nameBuffer, size)
+
+         sUserName=nameBuffer.value
+      except:
+         pass
 
-   def disconnect(self):
-      """
-Disconnect from TestResultWebApp's database.
+   return sUserName
+
+def __curent_testtool():
+   """
+Get current versions of Python and PyTest.\
+This information is used as default value for `testtool` when importing.
 
 **Arguments:**
 
 (*no arguments*)
 
 **Returns:**
 
-(*no returns*)
-      """
-      self.con.commit()
-      self.con.close()
-
-   def cleanAllTables(self):
-      """
-Delete all table data. Please be careful before calling this method.
+   / *Type*: str /
 
-**Arguments:**
+   Current PyTest and Python verions as testtool.\
+   E.g: PyTest 6.2.5 (Python 3.9.0)
+   """
+   sPytestVersion = "unknown_version"
+   # Try to get pytest version
+   # Incase pytest is not installed, set to 'unknown_version'
+   try:
+      sPytestVersion = get_distribution('pytest').version
+   except:
+      pass
 
-(*no arguments*)
+   return f"PyTest {sPytestVersion} (Python {platform.python_version()})"
 
-**Returns:**
+CONFIG_SCHEMA = {
+   "components" : [str, dict],
+   "variant"   : str,
+   "version_sw": str,
+   "version_hw": str,
+   "version_test": str,
+   "testtool"  :  str,
+   "tester"    :  str
+}
+
+DEFAULT_METADATA = {
+   "components"   :  "unknown",
+   "variant"      :  "PyTest",
+   "version_sw"   :  "",
+   "version_hw"   :  "",
+   "version_test" :  "",
+   "testtool"     :  __curent_testtool(),
+   "tester"       :  __current_user()
+}
+
+iTotalTestcase = 0
+iSuccessTestcase = 0
+dComponentCounter = {}
 
-(*no returns*)
-      """
-      print(">> Deleting all table data!")
-      sql="""delete from """ + self.db + """.evtbl_result_main where test_result_id!="" """
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.evtbl_failed_unknown_per_component where test_result_id!="" """
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_usr_case where test_case_id>0"""
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_usr_case_history where test_case_id>0"""
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_usr_comments where test_case_id>0"""
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_usr_links where test_case_id>0"""
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_usr_result where test_result_id!="" """
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_usr_result_history where test_result_id!="" """
-      self.__arExec(sql)
-
-      sql="""delete from """ + self.db + """.tbl_file_header where file_id>0"""
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_case where test_case_id>0"""
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_file where file_id>0"""
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_result where test_result_id!="" """
-      self.__arExec(sql)
-      sql="""delete from """ + self.db + """.tbl_prj where project<>"a" """
-      self.__arExec(sql)
-      self.con.commit()
+class Logger():
+   """
+Logger class for logging message.
+   """
+   output_logfile = None
+   output_console = True
+   color_normal   = col.Fore.WHITE + col.Style.NORMAL
+   color_error    = col.Fore.RED + col.Style.BRIGHT
+   color_warn     = col.Fore.YELLOW + col.Style.BRIGHT
+   color_reset    = col.Style.RESET_ALL + col.Fore.RESET + col.Back.RESET
+   prefix_warn    = "WARN: "
+   prefix_error   = "ERROR: "
+   prefix_fatalerror = "FATAL ERROR: "
+   prefix_all = ""
+   dryrun = False
 
-   def __arExec(self, command, values=None, bHasResponse=False, bReturnInsertedID=False):
+   @classmethod
+   def config(cls, output_console=True, output_logfile=None, indent=0, dryrun=False):
       """
-Execute a query. By default don't try to fetch a result.
+Configure Logger class.
 
 **Arguments:**
 
-*  ``command``
-
-   / *Condition*: required / *Type*: str /
-
-   Query need to be executed.
-
-*  ``values``
-
-   / *Condition*: optional / *Type*: list / *Default*: None /
-
-   Sequence of parameters to be used with the query.
-
-*  ``bHasResponse``
-
-   / *Condition*: optional / *Type*: bool / *Default*: False /
-
-   If True, respsonse is expected.
+*  ``output_console``
 
-*  ``bReturnInsertedID``
+   / *Condition*: optional / *Type*: bool / *Default*: True /
 
-   / *Condition*: optional / *Type*: bool / *Default*: False /
+   Write message to console output.
 
-   If True, the lastrowid will be returned.
+*  ``output_logfile``
 
-**Returns:**
+   / *Condition*: optional / *Type*: str / *Default*: None /
 
-*  ``arRes``
+   Path to log file output.
 
-   / *Type*: list /
+*  ``indent``
 
-   List of reponse data (or lastrowid if bReturnInsertedID is set).
-      """
-      arRes = None
-      c = self.con.cursor()
-      c.execute(command,values)
-      if bHasResponse:
-         arRes = c.fetchall()
-      elif bReturnInsertedID:
-         arRes = c.lastrowid
-      c.close()
-      return arRes
-
-   def __vExecMany(self, command, values=None):
-      """
-Execute a query for bulk insert of many elements. No response expected.
+   / *Condition*: optional / *Type*: int / *Default*: 0 /
 
-**Arguments:**
+   Offset indent.
 
-*  ``command``
+*  ``dryrun``
 
-   / *Condition*: required / *Type*: str /
-
-   Query need to be executed.
-
-*  ``values``
-
-   / *Condition*: optional / *Type*: list / *Default*: None /
+   / *Condition*: optional / *Type*: bool / *Default*: True /
 
-   Sequence of parameters to be used with the query.
+   If set, a prefix as 'dryrun' is added for all messages.
 
 **Returns:**
 
 (*no returns*)
       """
-      c = self.con.cursor()
-      c.executemany(command,values)
-      c.close()
-
-   def __nGetLastInsertID(self, tbl):
-      """
-Return the last_insert_id of a given table.
-
-**Arguments:**
-
-*  ``tbl``
-
-   / *Condition*: required / *Type*: str /
-
-   Table name to get the last_insert_id.
+      cls.output_console = output_console
+      cls.output_logfile = output_logfile
+      cls.dryrun = dryrun
+      if cls.dryrun:
+         cls.prefix_all = cls.color_warn + "DRYRUN  " + cls.color_reset
 
-**Returns:**
-
-*  ``res``
-
-   / *Type*: str /
-
-   The last_insert_id.
-      """
-      # "select last_insert_id from table" returns as result a one column table
-      # where the number of rows is the length of the full table.
-      # Each row has the same value of the last_insert_id.
-      # This causes dramatic performance problems.
-      # Anyhow we need only one element, therefore we limit here to 1
-      sql = """select last_insert_id() from """ + self.db + "." + tbl + " limit 1"
-      res = self.__arExec(sql,bHasResponse=True)[0][0]
-      return res
-
-   def sCreateNewTestResult(self, _tbl_prj_project,
-                                  _tbl_prj_variant,
-                                  _tbl_prj_branch,
-                                  _tbl_test_result_id,
-                                  _tbl_result_interpretation,
-                                  _tbl_result_time_start,
-                                  _tbl_result_time_end,
-                                  _tbl_result_version_sw_target,
-                                  _tbl_result_version_sw_test,
-                                  _tbl_result_version_target,
-                                  _tbl_result_jenkinsurl,
-                                  _tbl_result_reporting_qualitygate
-                            ):
+   @classmethod
+   def log(cls, msg="", color=None, indent=0):
       """
-Creates a new test result in ``tbl_result``. This is the main table which is
-linked to all other data by means of ``test_result_id``.
+Write log message to console/file output.
 
 **Arguments:**
 
-*  ``_tbl_prj_project``
-
-   / *Condition*: required / *Type*: str /
-
-   Project information.
+*  ``msg``
 
-*  ``_tbl_prj_variant``
+   / *Condition*: optional / *Type*: str / *Default*: "" /
 
-   / *Condition*: required / *Type*: str /
+   Message which is written to output.
 
-   Variant information.
+*  ``color``
 
-*  ``_tbl_prj_branch``
+   / *Condition*: optional / *Type*: str / *Default*: None /
 
-   / *Condition*: required / *Type*: str /
+   Color style for the message.
 
-   Branch information.
+*  ``indent``
 
-*  ``_tbl_test_result_id``
+   / *Condition*: optional / *Type*: int / *Default*: 0 /
 
-   / *Condition*: required / *Type*: str /
-
-   UUID of test result.
-
-*  ``_tbl_result_interpretation``
-
-   / *Condition*: required / *Type*: str /
-
-   Result interpretation.
-
-*  ``_tbl_result_time_start``
-
-   / *Condition*: required / *Type*: str /
-
-   Test result start time as format ``%Y-%m-%d %H:%M:%S``.
-
-*  ``_tbl_result_time_end``
-
-   / *Condition*: required / *Type*: str /
-
-   Test result end time as format ``%Y-%m-%d %H:%M:%S``.
-
-*  ``_tbl_result_version_sw_target``
-
-   / *Condition*: required / *Type*: str /
-
-   Software version information.
-
-*  ``_tbl_result_version_sw_test``
-
-   / *Condition*: required / *Type*: str /
-
-   Test version information.
-
-*  ``_tbl_result_version_target``
-
-   / *Condition*: required / *Type*: str /
-
-   Hardware version information.
-
-*  ``_tbl_result_jenkinsurl``
-
-   / *Condition*: required / *Type*: str /
-
-   Jenkinsurl in case test result is executed by jenkins.
-
-*  ``_tbl_result_reporting_qualitygate``
-
-   / *Condition*: required / *Type*: str /
-
-   Qualitygate information for reporting.
+   Offset indent.
 
 **Returns:**
 
-*  ``_tbl_test_result_id``
-
-   / *Type*: str /
-
-   ``test_result_id`` of new test result.
+(*no returns*)
       """
-      sql,sqlval = """select count(*) from """ + self.db + """.tbl_prj where
-               (project=%s and variant=%s and branch=%s)""", (_tbl_prj_project,
-                                                              _tbl_prj_variant,
-                                                              _tbl_prj_branch)
-      res = self.__arExec(sql,sqlval,True)[0][0]
-      if res == 0:
-         sql,sqlval = """insert into """ + self.db + """.tbl_prj
-         ( variant,project, branch) values (%s, %s, %s)""" , (_tbl_prj_variant,
-                                                              _tbl_prj_project,
-                                                              _tbl_prj_branch)
-         self.__arExec(sql,sqlval)
-
-      sql,sqlval = """insert into """ + self.db + """.tbl_result (test_result_id,
-         variant,project,branch, time_start,time_end, version_sw_target,
-         version_sw_test,version_hardware,jenkinsurl,reporting_qualitygate,result_state)
-         values (%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s)""" , (_tbl_test_result_id,
-                                                            _tbl_prj_variant,
-                                                            _tbl_prj_project,
-                                                            _tbl_prj_branch,
-                                                            _tbl_result_time_start,
-                                                            _tbl_result_time_end,
-                                                            _tbl_result_version_sw_target,
-                                                            _tbl_result_version_sw_test,
-                                                            _tbl_result_version_target,
-                                                            _tbl_result_jenkinsurl,
-                                                            _tbl_result_reporting_qualitygate,
-                                                            "in progress")
-      self.__arExec(sql,sqlval)
-
-      if _tbl_result_interpretation!='':
-         sql,sqlval = """update """ + self.db + """.tbl_result set interpretation=%s
-            where test_result_id='""" + _tbl_test_result_id + "'", (_tbl_result_interpretation,)
-         self.__arExec(sql,sqlval)
-
-      return _tbl_test_result_id
-
-   def nCreateNewFile(self,_tbl_file_name,
-                           _tbl_file_tester_account,
-                           _tbl_file_tester_machine,
-                           _tbl_file_time_start,
-                           _tbl_file_time_end,
-                           _tbl_test_result_id,
-                           _tbl_file_origin="ROBFW"):
+      if color==None:
+         color = cls.color_normal
+      if cls.output_console:
+         print(cls.prefix_all + cls.color_reset + color + " "*indent + msg + cls.color_reset)
+      if cls.output_logfile!=None and os.path.isfile(cls.output_logfile):
+         with open(cls.output_logfile, "a") as f:
+            f.write(" "*indent + msg)
+      return
+
+   @classmethod
+   def log_warning(cls, msg):
       """
-Create new file entry in ``tbl_file`` table.
+Write warning message to console/file output.
 
 **Arguments:**
 
-*  ``_tbl_file_name``
-
-   / *Condition*: required / *Type*: str /
-
-   File name information.
-
-*  ``_tbl_file_tester_account``
-
-   / *Condition*: required / *Type*: str /
-
-   Tester account information.
-
-*  ``_tbl_file_tester_machine``
-
-   / *Condition*: required / *Type*: str /
-
-   Test machine information.
-
-*  ``_tbl_file_time_start``
+*  ``msg``
 
    / *Condition*: required / *Type*: str /
 
-   Test file start time as format ``%Y-%m-%d %H:%M:%S``.
-
-*  ``_tbl_file_time_end``
-
-   / *Condition*: required / *Type*: str /
-
-   Test file end time as format ``%Y-%m-%d %H:%M:%S``.
-
-*  ``_tbl_test_result_id``
-
-   / *Condition*: required / *Type*: str /
-
-   UUID of test result for linking to `tbl_result` table.
-
-*  ``_tbl_file_origin``
-
-   / *Condition*: required / *Type*: str /
-
-   Origin (test framework) of test file. Deafult is "ROBFW"
+   Warning message which is written to output.
 
 **Returns:**
 
-*  ``iInsertedID``
-
-   / *Type*: int /
-
-   ID of new entry.
+(*no returns*)
       """
-      sql,sqlval ="""insert into """ + self.db + """.tbl_file (name,tester_account,
-                     tester_machine,time_start,time_end,test_result_id,origin)
-                     values (%s,%s,%s,%s,%s,%s,%s)""" , ( _tbl_file_name,
-                                                         _tbl_file_tester_account,
-                                                         _tbl_file_tester_machine,
-                                                         _tbl_file_time_start,
-                                                         _tbl_file_time_end,
-                                                         _tbl_test_result_id,
-                                                         _tbl_file_origin)
-      iInsertedID = self.__arExec(sql,sqlval, bReturnInsertedID=True)
-      return iInsertedID
-
-   def vCreateNewHeader(self, _tbl_file_id,
-                              _tbl_header_testtoolconfiguration_testtoolname,
-                              _tbl_header_testtoolconfiguration_testtoolversionstring,
-                              _tbl_header_testtoolconfiguration_projectname,
-                              _tbl_header_testtoolconfiguration_logfileencoding,
-                              _tbl_header_testtoolconfiguration_pythonversion,
-                              _tbl_header_testtoolconfiguration_testfile,
-                              _tbl_header_testtoolconfiguration_logfilepath,
-                              _tbl_header_testtoolconfiguration_logfilemode,
-                              _tbl_header_testtoolconfiguration_ctrlfilepath,
-                              _tbl_header_testtoolconfiguration_configfile,
-                              _tbl_header_testtoolconfiguration_confname,
-
-                              _tbl_header_testfileheader_author,
-                              _tbl_header_testfileheader_project,
-                              _tbl_header_testfileheader_testfiledate,
-                              _tbl_header_testfileheader_version_major,
-                              _tbl_header_testfileheader_version_minor,
-                              _tbl_header_testfileheader_version_patch,
-                              _tbl_header_testfileheader_keyword,
-                              _tbl_header_testfileheader_shortdescription,
-                              _tbl_header_testexecution_useraccount,
-                              _tbl_header_testexecution_computername,
-
-                              _tbl_header_testrequirements_documentmanagement,
-                              _tbl_header_testrequirements_testenvironment,
-
-                              _tbl_header_testbenchconfig_name,
-                              _tbl_header_testbenchconfig_data,
-                              _tbl_header_preprocessor_filter,
-                              _tbl_header_preprocessor_parameters ):
+      cls.log(cls.prefix_warn+str(msg), cls.color_warn)
+
+   @classmethod
+   def log_error(cls, msg, fatal_error=False):
       """
-Create a new header entry in ``tbl_file_header`` table which is linked with the file.
+Write error message to console/file output.
 
 **Arguments:**
 
-*  ``_tbl_file_id``
-
-   / *Condition*: required / *Type*: int /
-
-   File ID information.
-
-*  ``_tbl_header_testtoolconfiguration_testtoolname``
-
-   / *Condition*: required / *Type*: str /
-
-   Test tool name.
-
-*  ``_tbl_header_testtoolconfiguration_testtoolversionstring``
-
-   / *Condition*: required / *Type*: str /
-
-   Test tool version.
-
-*  ``_tbl_header_testtoolconfiguration_projectname``
-
-   / *Condition*: required / *Type*: str /
-
-   Project name.
-
-*  ``_tbl_header_testtoolconfiguration_logfileencoding``
-
-   / *Condition*: required / *Type*: str /
-
-   Encoding of logfile.
-
-*  ``_tbl_header_testtoolconfiguration_pythonversion``
-
-   / *Condition*: required / *Type*: str /
-
-   Python version info.
-
-*  ``_tbl_header_testtoolconfiguration_testfile``
-
-   / *Condition*: required / *Type*: str /
-
-   Test file name.
-
-*  ``_tbl_header_testtoolconfiguration_logfilepath``
-
-   / *Condition*: required / *Type*: str /
-
-   Path to log file.
-
-*  ``_tbl_header_testtoolconfiguration_logfilemode``
-
-   / *Condition*: required / *Type*: str /
-
-   Mode of log file.
-
-*  ``_tbl_header_testtoolconfiguration_ctrlfilepath``
-
-   / *Condition*: required / *Type*: str /
-
-   Path to control file.
-
-*  ``_tbl_header_testtoolconfiguration_configfile``
-
-   / *Condition*: required / *Type*: str /
-
-   Path to configuration file.
-
-*  ``_tbl_header_testtoolconfiguration_confname``
-
-   / *Condition*: required / *Type*: str /
-
-   Configuration name.
-
-*  ``_tbl_header_testfileheader_author``
-
-   / *Condition*: required / *Type*: str /
-
-   File author.
-
-*  ``_tbl_header_testfileheader_project``
-
-   / *Condition*: required / *Type*: str /
-
-   Project information.
-
-*  ``_tbl_header_testfileheader_testfiledate``
-
-   / *Condition*: required / *Type*: str /
-
-   File creation date.
-
-*  ``_tbl_header_testfileheader_version_major``
-
-   / *Condition*: required / *Type*: str /
-
-   File major version.
-
-*  ``_tbl_header_testfileheader_version_minor``
-
-   / *Condition*: required / *Type*: str /
-
-   File minor version.
-
-*  ``_tbl_header_testfileheader_version_patch``
-
-   / *Condition*: required / *Type*: str /
-
-   File patch version.
-
-*  ``_tbl_header_testfileheader_keyword``
-
-   / *Condition*: required / *Type*: str /
-
-   File keyword.
-
-*  ``_tbl_header_testfileheader_shortdescription``
-
-   / *Condition*: required / *Type*: str /
-
-   File short description.
-
-*  ``_tbl_header_testexecution_useraccount``
-
-   / *Condition*: required / *Type*: str /
-
-   Tester account who run the execution.
-
-*  ``_tbl_header_testexecution_computername``
-
-   / *Condition*: required / *Type*: str /
-
-   Machine name which is executed on.
-
-*  ``_tbl_header_testrequirements_documentmanagement``
-
-   / *Condition*: required / *Type*: str /
-
-   Requirement management information.
-
-*  ``_tbl_header_testrequirements_testenvironment``
-
-   / *Condition*: required / *Type*: str /
-
-   Requirement environment information.
-
-*  ``_tbl_header_testbenchconfig_name``
+*  ``msg``
 
    / *Condition*: required / *Type*: str /
 
-   Testbench configuration name.
+   Error message which is written to output.
 
-*  ``_tbl_header_testbenchconfig_data``
+*  ``fatal_error``
 
-   / *Condition*: required / *Type*: str /
-
-   Testbench configuration data.
-
-*  ``_tbl_header_preprocessor_filter``
-
-   / *Condition*: required / *Type*: str /
-
-   Preprocessor filter information.
-
-*  ``_tbl_header_preprocessor_parameters``
-
-   / *Condition*: required / *Type*: str /
+   / *Condition*: optional / *Type*: bool / *Default*: False /
 
-   Preprocessor parameters definition.
+   If set, tool will terminate after logging error message.
 
 **Returns:**
 
 (*no returns*)
       """
-      sql,sqlval ="""insert into """ + self.db + """.tbl_file_header
-                        ( file_id,
-                          testtoolconfiguration_testtoolname,
-                          testtoolconfiguration_testtoolversionstring,
-                          testtoolconfiguration_projectname,
-                          testtoolconfiguration_logfileencoding,
-                          testtoolconfiguration_pythonversion,
-                          testtoolconfiguration_testfile,
-                          testtoolconfiguration_logfilepath,
-                          testtoolconfiguration_logfilemode,
-                          testtoolconfiguration_ctrlfilepath,
-                          testtoolconfiguration_configfile,
-                          testtoolconfiguration_confname,
-
-                          testfileheader_author,
-                          testfileheader_project,
-                          testfileheader_testfiledate,
-                          testfileheader_version_major,
-                          testfileheader_version_minor,
-                          testfileheader_version_patch,
-                          testfileheader_keyword,
-                          testfileheader_shortdescription,
-                          testexecution_useraccount,
-                          testexecution_computername,
-
-                          testrequirements_documentmanagement,
-                          testrequirements_testenvironment,
-
-                          testbenchconfig_name,
-                          testbenchconfig_data,
-                          preprocessor_filter,
-                          preprocessor_parameters)
-                  values ( %s, %s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s, %s,
-                           %s, %s, %s,%s,%s,%s,%s,%s,%s,%s,%s,%s)""" , \
-                        ( _tbl_file_id,
-                          _tbl_header_testtoolconfiguration_testtoolname,
-                          _tbl_header_testtoolconfiguration_testtoolversionstring,
-                          _tbl_header_testtoolconfiguration_projectname,
-                          _tbl_header_testtoolconfiguration_logfileencoding,
-                          _tbl_header_testtoolconfiguration_pythonversion,
-                          _tbl_header_testtoolconfiguration_testfile,
-                          _tbl_header_testtoolconfiguration_logfilepath,
-                          _tbl_header_testtoolconfiguration_logfilemode,
-                          _tbl_header_testtoolconfiguration_ctrlfilepath,
-                          _tbl_header_testtoolconfiguration_configfile,
-                          _tbl_header_testtoolconfiguration_confname,
-
-                          _tbl_header_testfileheader_author,
-                          _tbl_header_testfileheader_project,
-                          _tbl_header_testfileheader_testfiledate,
-                          _tbl_header_testfileheader_version_major,
-                          _tbl_header_testfileheader_version_minor,
-                          _tbl_header_testfileheader_version_patch,
-                          _tbl_header_testfileheader_keyword,
-                          _tbl_header_testfileheader_shortdescription,
-                          _tbl_header_testexecution_useraccount,
-                          _tbl_header_testexecution_computername,
-
-                          _tbl_header_testrequirements_documentmanagement,
-                          _tbl_header_testrequirements_testenvironment,
-
-                          _tbl_header_testbenchconfig_name,
-                          _tbl_header_testbenchconfig_data,
-                          _tbl_header_preprocessor_filter,
-                          _tbl_header_preprocessor_parameters)
-      self.__arExec(sql,sqlval)
-
-   def nCreateNewSingleTestCase(self,
-                                _tbl_case_name,
-                                _tbl_case_issue,
-                                _tbl_case_tcid,
-                                _tbl_case_fid,
-                                _tbl_case_testnumber,
-                                _tbl_case_repeatcount,
-                                _tbl_case_component,
-                                _tbl_case_time_start,
-                                _tbl_case_result_main,
-                                _tbl_case_result_state,
-                                _tbl_case_result_return,
-                                _tbl_case_counter_resets,
-                                _tbl_case_lastlog,
-                                _tbl_test_result_id,
-                                _tbl_file_id
-                               ):
-      """
-Create single testcase entry in ``tbl_case`` table immediately.
-
-**Arguments:**
-
-*  ``_tbl_case_name``
-
-   / *Condition*: required / *Type*: str /
-
-   Test case name.
+      prefix = cls.prefix_error
+      if fatal_error:
+         prefix = cls.prefix_fatalerror
+
+      cls.log(prefix+str(msg), cls.color_error)
+      if fatal_error:
+         cls.log(f"{(sys.argv[0])} has been stopped!", cls.color_error)
+         exit(1)
 
-*  ``_tbl_case_issue``
-
-   / *Condition*: required / *Type*: str /
-
-   Test case issue ID.
-
-*  ``_tbl_case_tcid``
-
-   / *Condition*: required / *Type*: str /
-
-   Test case ID (used for testmanagement tool).
-
-*  ``_tbl_case_fid``
-
-   / *Condition*: required / *Type*: str /
+def __process_commandline():
+   """
+Process provided argument(s) from command line.
 
-   Test case requirement (function) ID.
+Avalable arguments in command line:
 
-*  ``_tbl_case_testnumber``
+   - `-v`, `--version` : tool version information.
+   - `resultxmlfile` : path to the xml pytest result file or directory of result files to be imported.
+   - `server` : server which hosts the database (IP or URL).
+   - `user` : user for database login.
+   - `password` : password for database login.
+   - `database` : database name.
+   - `--recursive` : if True, then the path is searched recursively for *.xml files to be imported.
+   - `--dryrun` : if True, then verify all input arguments (includes DB connection) and show what would be done.
+   - `--append` : if True, then allow to append new result(s) to existing execution result UUID which is provided by --UUID argument.
+   - `--UUID` : UUID used to identify the import and version ID on TestResultWebApp.
+   - `--variant` : variant name to be set for this import.
+   - `--versions` : metadata: Versions (Software;Hardware;Test) to be set for this import.
+   - `--config` : configuration json file for component mapping information.
+   - `--interface` : database access interface.
 
-   / *Condition*: required / *Type*: int /
+**Arguments:**
 
-   Order of test case in file.
+(*no arguments*)
 
-*  ``_tbl_case_repeatcount``
+**Returns:**
 
-   / *Condition*: required / *Type*: int /
+   / *Type*: `ArgumentParser` object /
 
-   Test case repeatition count.
+   ArgumentParser object.
+   """
+   cmdlineparser=argparse.ArgumentParser(prog="PyTestLog2DB (PyTestXMLReport to TestResultWebApp importer)",
+                                         description="PyTestLog2DB imports pytest JUnit XML report file(s)" + \
+                                                     "generated by pytest into a WebApp database."
+                                        )
+
+   cmdlineparser.add_argument('-v', '--version',action='version', version=f'v{VERSION} ({VERSION_DATE})',help='version of the PyTestLog2DB importer.')
+   cmdlineparser.add_argument('resultxmlfile', type=str, help='absolute or relative path to the pytest JUnit XML report file or directory of report files to be imported.')
+   cmdlineparser.add_argument('server', type=str, help='server which hosts the database (IP or URL).')
+   cmdlineparser.add_argument('user', type=str, help='user for database login.')
+   cmdlineparser.add_argument('password', type=str, help='password for database login.')
+   cmdlineparser.add_argument('database', type=str, help='database schema for database login.')
+   cmdlineparser.add_argument('--recursive', action="store_true", help='if set, then the path is searched recursively for output files to be imported.')
+   cmdlineparser.add_argument('--dryrun', action="store_true", help='if set, then verify all input arguments (includes DB connection) and show what would be done.')
+   cmdlineparser.add_argument('--append', action="store_true", help='is used in combination with --UUID <UUID>.' +\
+                              ' If set, allow to append new result(s) to existing execution result UUID in --UUID argument.')
+   cmdlineparser.add_argument('--UUID', type=str, help='UUID used to identify the import and version ID on webapp.' + \
+                              ' If not provided PyTestLog2DB will generate an UUID for the whole import.')
+   cmdlineparser.add_argument('--variant', type=str, help='variant name to be set for this import.')
+   cmdlineparser.add_argument('--versions', type=str, help='metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).')
+   cmdlineparser.add_argument('--config', type=str, help='configuration json file for component mapping information.')
+   cmdlineparser.add_argument('--interface', choices=['db', 'rest'], default='db', help='database access interface.')
 
-*  ``_tbl_case_component``
+   return cmdlineparser.parse_args()
 
-   / *Condition*: required / *Type*: str /
+def collect_xml_result_files(path, search_recursive=False):
+   """
+Collect all valid Robot xml result file in given path.
 
-   Component which test case is belong to.
+**Arguments:**
 
-*  ``_tbl_case_time_start``
+*  ``path``
 
    / *Condition*: required / *Type*: str /
 
-   Test case start time as format ``%Y-%m-%d %H:%M:%S``.
+   Path to Robot result folder or file to be searched.
 
-*  ``_tbl_case_result_main``
+*  ``search_recursive``
 
-   / *Condition*: required / *Type*: str /
-
-   Test case main result.
-
-*  ``_tbl_case_result_state``
+   / *Condition*: optional / *Type*: bool / *Default*: False /
 
-   / *Condition*: required / *Type*: str /
+   If set, the given path is searched recursively for xml result files.
 
-   Test case completion state.
+**Returns:**
 
-*  ``_tbl_case_result_return``
+*  ``lFoundFiles``
 
-   / *Condition*: required / *Type*: int /
+   / *Type*: list /
 
-   Test case result code (as integer).
+   List of valid xml result file(s) in given path.
+   """
+   lFoundFiles = []
+   if os.path.exists(path):
+      if os.path.isfile(path):
+         validate_xml_result(path)
+         lFoundFiles.append(path)
+      else:
+         if search_recursive:
+            Logger.log("Searching *.xml result files recursively...")
+            for root, _, files in os.walk(path):
+               for file in files:
+                  if file.endswith(".xml"):
+                     xml_result_pathfile = os.path.join(root, file)
+                     Logger.log(xml_result_pathfile, indent=2)
+                     validate_xml_result(xml_result_pathfile)
+                     lFoundFiles.append(xml_result_pathfile)
+         else:
+            Logger.log("Searching *.xml result files...")
+            for file in os.listdir(path):
+               if file.endswith(".xml"):
+                  xml_result_pathfile = os.path.join(path, file)
+                  Logger.log(xml_result_pathfile, indent=2)
+                  validate_xml_result(xml_result_pathfile)
+                  lFoundFiles.append(xml_result_pathfile)
+
+         # Terminate tool with error when no logfile under provided folder
+         if len(lFoundFiles) == 0:
+            Logger.log_error(f"No *.xml result file under '{path}' folder.", fatal_error=True)
+   else:
+      Logger.log_error(f"Given resultxmlfile is not existing: '{path}'", fatal_error=True)
 
-*  ``_tbl_case_counter_resets``
+   return lFoundFiles
 
-   / *Condition*: required / *Type*: int /
+def validate_xml_result(xml_result, xsd_schema=os.path.join(os.path.dirname(__file__),'xsd/junit.xsd'), exit_on_failure=True):
+   """
+Verify the given xml result file is valid or not.
 
-   Counter of target reset within test case execution.
+**Arguments:**
 
-*  ``_tbl_case_lastlog``
+*  ``xml_result``
 
    / *Condition*: required / *Type*: str /
 
-   Traceback information when test case is failed.
+   Path to PyTest result file.
 
-*  ``_tbl_test_result_id``
+*  ``xsd_schema``
 
-   / *Condition*: required / *Type*: str /
+   / *Condition*: optional / *Type*: str / *Default*: <installed_folder>\/xsd\/junit.xsd /
 
-   UUID of test result for linking to file in ``tbl_result`` table.
+   Path to Robot schema *.xsd file.
 
-*  ``_tbl_file_id``
+*  ``exit_on_failure``
 
-   / *Condition*: required / *Type*: int /
+   / *Condition*: optional / *Type*: bool / *Default*: True /
 
-   Test file ID for linking to file in ``tbl_file`` table.
+   If set, exit with fatal error if the schema validation of given xml file failed.
 
 **Returns:**
 
-*  ``iInsertedID``
+*  / *Type*: bool /
 
-   / *Type*: int /
+   True if the given xml result is valid with the provided schema *.xsd.
+   """
+   try:
+      xmlschema_doc = etree.parse(xsd_schema)
+      xmlschema = etree.XMLSchema(xmlschema_doc)
+   except Exception as reason:
+      Logger.log_error(f"schema xsd file '{xsd_schema}' is not a valid.\nReason: {reason}", fatal_error=True)
+
+   if exit_on_failure:
+      try:
+         xml_doc = etree.parse(xml_result)
+         xmlschema.assert_(xml_doc)
+      except AssertionError as reason:
+         Logger.log_error(f"xml result file '{xml_result}' is not a valid PyTest result.\nReason: {reason}", fatal_error=True)
+      except Exception as reason:
+         Logger.log_error(f"result file '{xml_result}' is not a valid xml format.\nReason: {reason}", fatal_error=True)
 
-   ID of new entry.
-      """
-      if _tbl_case_lastlog == "":
-         _tbl_case_lastlog = None
-      sql = """insert into """ + self.db + """.tbl_case (name, issue, tcid, fid,
-               testnumber, repeatcount, component, time_start, result_main, result_state,
-               result_return, counter_resets, lastlog, test_result_id, file_id)
-               values (%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s)"""
-      sqlval = (_tbl_case_name,
-                _tbl_case_issue,
-                _tbl_case_tcid,
-                _tbl_case_fid,
-                _tbl_case_testnumber,
-                _tbl_case_repeatcount,
-                _tbl_case_component,
-                _tbl_case_time_start,
-                _tbl_case_result_main,
-                _tbl_case_result_state,
-                _tbl_case_result_return,
-                _tbl_case_counter_resets,
-                _tbl_case_lastlog,
-                _tbl_test_result_id,
-                _tbl_file_id
-               )
-      iInsertedTestID = self.__arExec(sql, sqlval, bReturnInsertedID=True)
-      return iInsertedTestID
-
-   #
-   # create a new test case entry:
-   #
-   #
-   def nCreateNewTestCase(self,
-                          _tbl_case_name,
-                          _tbl_case_issue,
-                          _tbl_case_tcid,
-                          _tbl_case_fid,
-                          _tbl_case_testnumber,
-                          _tbl_case_repeatcount,
-                          _tbl_case_component,
-                          _tbl_case_time_start,
-                          _tbl_case_result_main,
-                          _tbl_case_result_state,
-                          _tbl_case_result_return,
-                          _tbl_case_counter_resets,
-                          _tbl_case_lastlog,
-                          _tbl_test_result_id,
-                          _tbl_file_id
-                           ):
-      """
-Create bulk of test case entries: new test cases are buffered and inserted as bulk.
+   return xmlschema.validate(xml_doc)
 
-Once ``__NUM_BUFFERD_ELEMENTS_FOR_EXECUTEMANY`` is reached, the creation query is executed.
+def is_valid_uuid(uuid_to_test, version=4):
+   """
+Verify the given UUID is valid or not.
 
 **Arguments:**
 
-*  ``_tbl_case_name``
-
-   / *Condition*: required / *Type*: str /
-
-   Test case name.
-
-*  ``_tbl_case_issue``
+*  ``uuid_to_test``
 
    / *Condition*: required / *Type*: str /
 
-   Test case issue ID.
-
-*  ``_tbl_case_tcid``
+   UUID to be verified.
 
-   / *Condition*: required / *Type*: str /
-
-   Test case ID (used for testmanagement tool).
+*  ``version``
 
-*  ``_tbl_case_fid``
+   / *Condition*: optional / *Type*: int / *Default*: 4 /
 
-   / *Condition*: required / *Type*: str /
+   UUID version.
 
-   Test case requirement (function) ID.
+**Returns:**
 
-*  ``_tbl_case_testnumber``
+*  ``bValid``
 
-   / *Condition*: required / *Type*: int /
+   / *Type*: bool /
 
-   Order of test case in file.
+   True if the given UUID is valid.
+   """
+   bValid = False
+   try:
+      uuid_obj = uuid.UUID(uuid_to_test, version=version)
+   except:
+      return bValid
 
-*  ``_tbl_case_repeatcount``
+   if str(uuid_obj) == uuid_to_test:
+      bValid = True
 
-   / *Condition*: required / *Type*: int /
+   return bValid
 
-   Test case repeatition count.
+def is_valid_config(dConfig, dSchema=CONFIG_SCHEMA, bExitOnFail=True):
+   """
+Validate the json configuration base on given schema.
 
-*  ``_tbl_case_component``
+Default schema supports below information:
 
-   / *Condition*: required / *Type*: str /
+.. code:: python
 
-   Component which test case is belong to.
+   CONFIG_SCHEMA = {
+      "components": [str, dict],
+      "variant"   : str,
+      "version_sw": str,
+      "version_hw": str,
+      "version_test": str,
+      "testtool"  :  str,
+      "tester"    :  str
+   }
 
-*  ``_tbl_case_time_start``
+**Arguments:**
 
-   / *Condition*: required / *Type*: str /
+*  ``dConfig``
 
-   Test case start time as format ``%Y-%m-%d %H:%M:%S``.
+   / *Condition*: required / *Type*: dict /
 
-*  ``_tbl_case_result_main``
+   Json configuration object to be verified.
 
-   / *Condition*: required / *Type*: str /
+*  ``dSchema``
 
-   Test case main result.
+   / *Condition*: optional / *Type*: dict / *Default*: CONFIG_SCHEMA /
 
-*  ``_tbl_case_result_state``
+   Schema for the validation.
 
-   / *Condition*: required / *Type*: str /
+*  ``bExitOnFail``
 
-   Test case completion state.
+   / *Condition*: optional / *Type*: bool / *Default*: True /
 
-*  ``_tbl_case_result_return``
+   If True, exit tool in case the validation is fail.
 
-   / *Condition*: required / *Type*: int /
+**Returns:**
 
-   Test case result code (as integer).
+*  ``bValid``
 
-*  ``_tbl_case_counter_resets``
+   / *Type*: bool /
 
-   / *Condition*: required / *Type*: int /
+   True if the given json configuration data is valid.
+   """
+   bValid = True
+   for key in dConfig:
+      if key in dSchema.keys():
+         # List of support types
+         if isinstance(dSchema[key], list):
+            if type(dConfig[key]) not in dSchema[key]:
+               bValid = False
+         # Fixed type
+         else:
+            if type(dConfig[key]) != dSchema[key]:
+               bValid = False
+
+         if not bValid:
+            Logger.log_error(f"Value of '{key}' has wrong type '{type(dConfig[key])}' in configuration json file.", fatal_error=bExitOnFail)
+            break
+
+      else:
+         bValid = False
+         Logger.log_error(f"Invalid key '{key}' in configuration json file.", fatal_error=bExitOnFail)
+         break
 
-   Counter of target reset within test case execution.
+   return bValid
 
-*  ``_tbl_case_lastlog``
 
-   / *Condition*: required / *Type*: str /
+def parse_pytest_xml(*xmlfiles):
+   """
+Parse and merge all given pytest *.xml result files into one result file.\
+Besides, `starttime` and `endtime` are also calculated and added in the merged result.
 
-   Traceback information when test case is failed.
+**Arguments:**
 
-*  ``_tbl_test_result_id``
+*  ``xmlfiles``
 
    / *Condition*: required / *Type*: str /
 
-   UUID of test result for linking to file in `tbl_result` table.
-
-*  ``_tbl_file_id``
-
-   / *Condition*: required / *Type*: int /
-
-   Test file ID for linking to file in ``tbl_file`` table.
+   Path to pytest *.xml result file(s).
 
 **Returns:**
 
-(*no returns*)
-      """
-      if _tbl_case_lastlog == "":
-         _tbl_case_lastlog = None
-      sqlval = (_tbl_case_name,
-                _tbl_case_issue,
-                _tbl_case_tcid,
-                _tbl_case_fid,
-                _tbl_case_testnumber,
-                _tbl_case_repeatcount,
-                _tbl_case_component,
-                _tbl_case_time_start,
-                _tbl_case_result_main,
-                _tbl_case_result_state,
-                _tbl_case_result_return,
-                _tbl_case_counter_resets,
-                _tbl_test_result_id,
-                _tbl_file_id,
-                _tbl_case_lastlog,
-                )
-      self.lTestCases.append(sqlval)
-      if len(self.lTestCases) >= CDataBase.__NUM_BUFFERD_ELEMENTS_FOR_EXECUTEMANY:
-         self.vEnableForeignKeyCheck(False)
-         self.__vUploadTestCaseListToDb(self.lTestCases)
-         self.vEnableForeignKeyCheck(True)
-         # Clear test cases list
-         self.lTestCases = []
-
-   def __vUploadTestCaseListToDb(self, lTestCases):
-      """
-Bulk insert test case results.
+*  ``oMergedTree``
 
-**Arguments:**
-
-*  ``lTestCases``
+   / *Type*: `etree._Element` object /
 
-   / *Condition*: required / *Type*: str /
+   The result object which is parsed from provided pytest *.xml result file(s).
+   """
+   oMergedTree = None
+   dtStartTime = None
+   dtEndTime   = None
+
+   try:
+      for item in xmlfiles:
+         oTree = etree.parse(item).getroot()
+         if oMergedTree == None:
+            oMergedTree = oTree
+            sStartTime  = oMergedTree.getchildren()[0].get("timestamp")
+            dtStartTime = datetime.strptime(sStartTime, PYTEST_DATETIME_FORMAT)
+            dtEndTime   = dtStartTime + timedelta(seconds=float(oMergedTree.getchildren()[0].get("time")))
+         else:
+            oAdditionalTree = etree.parse(item)
+            for oSuite in oAdditionalTree.getroot().iterchildren("testsuite"):
+               oMergedTree.append(oSuite)
+               dtTimestamp = datetime.strptime(oSuite.get("timestamp"), PYTEST_DATETIME_FORMAT)
+
+               # check starttime and endtime for the execution result
+               if dtTimestamp < dtStartTime:
+                  dtStartTime = dtTimestamp
+               elif (dtTimestamp + timedelta(seconds=float(oSuite.get("time"))))> dtEndTime:
+                  dtEndTime = dtTimestamp
+
+   except Exception as reason:
+      Logger.log_error(f"Error when merging pytest xml files. Reason: {reason}", fatal_error=True)
+
+   # Additional attributes for testsuites
+   oMergedTree.attrib["starttime"] = datetime.strftime(dtStartTime, DB_DATETIME_FORMAT)
+   oMergedTree.attrib["endtime"] = datetime.strftime(dtEndTime, DB_DATETIME_FORMAT)
 
-   List of test case for creation.
+   return oMergedTree
 
-**Returns:**
+def get_branch_from_swversion(sw_version):
+   """
+Get branch name from software version information.
 
-(*no returns*)
-      """
-      sql = """insert into """ + self.db + """.tbl_case (name, issue, tcid, fid,
-            testnumber, repeatcount, component, time_start, result_main, result_state,
-            result_return, counter_resets, test_result_id, file_id, lastlog)
-            values (%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s,%s)"""
-      self.__vExecMany(sql, lTestCases)
+Convention of branch information in suffix of software version:
 
-   def vCreateTags(self, _tbl_test_result_id, _tbl_usr_result_tags):
-      """
-Create tag entries.
+*  All software version with .0F is the main/freature branch.
+   The leading number is the current year. E.g. ``17.0F03``
+*  All software version with ``.1S``, ``.2S``, ... is a stabi branch.
+   The leading number is the year of branching out for stabilization.
+   The number before "S" is the order of branching out in the year.
 
 **Arguments:**
 
-*  ``_tbl_test_result_id``
+*  ``sw_version``
 
    / *Condition*: required / *Type*: str /
 
-   UUID of test result.
-
-*  ``_tbl_usr_result_tags``
-
-   / *Condition*: required / *Type*: str /
-
-   User tags information.
+   Software version.
 
 **Returns:**
 
-(*no returns*)
-      """
-      sql,sqlval="""insert into """ + self.db + """.tbl_usr_result (test_result_id, tags)
-                    values (%s,%s)""", (_tbl_test_result_id , _tbl_usr_result_tags)
-      self.__arExec(sql,sqlval)
-
-   def vSetCategory(self, _tbl_test_result_id, tbl_result_category_main):
-      """
-Create category entry.
+*  ``branch_name``
 
-**Arguments:**
+   / *Type*: str /
 
-*  ``_tbl_test_result_id``
+   Branch name.
+   """
+   branch_name = "main"
+   version_number=re.findall(r"(\d+\.)(\d+)([S,F])\d+",sw_version.upper())
+   try:
+      branch_name = "".join(version_number[0])
+   except:
+      pass
+   if branch_name.endswith(".0F"):
+      branch_name="main"
+   return branch_name
 
-   / *Condition*: required / *Type*: str /
+def get_test_result(oTest):
+   """
+Get test result from provided Testcase object.
 
-   UUID of test result.
+**Arguments:**
 
-*  ``tbl_result_category_main``
+*  ``oTest``
 
-   / *Condition*: required / *Type*: str /
+   / *Condition*: required / *Type*: `etree._Element` object /
 
-   Category information.
+   Testcase object.
 
 **Returns:**
 
-(*no returns*)
-      """
-      sql="""update """ + self.db + """.tbl_result set category_main='""" + \
-                  tbl_result_category_main + """' where test_result_id='""" + \
-                  _tbl_test_result_id + "'"
-      self.__arExec(sql)
-
-   def vUpdateStartEndTime(self, _tbl_test_result_id, _tbl_result_time_start, _tbl_result_time_end):
-      """
-Create start-end time entry.
+   / *Type*: typle /
 
-**Arguments:**
+   Testcase result which contains `result_main`, `lastlog` and `result_return`.
+   """
+   main_result = "Passed"
+   traceback_log = ""
+   return_code = 11
+   if failure := list(oTest.iterchildren("failure")):
+      main_result = "Failed"
+      traceback_log = f"{failure[0].get('message')}\n{failure[0].text}"
+      return_code = 12
+   elif error := list(oTest.iterchildren("error")):
+      main_result = "unknown"
+      traceback_log = f"{error[0].get('message')}\n{error[0].text}"
+      return_code = 5
+   elif list(oTest.iterchildren("skipped")):
+      main_result = "unknown"
+      traceback_log = f"This test is skipped."
+      return_code = 20
 
-*  ``_tbl_test_result_id``
+   return (main_result, base64.b64encode(traceback_log.encode()), return_code)
 
-   / *Condition*: required / *Type*: str /
+def process_component_info(dConfig, sTestClassname):
+   """
+Return the component name bases on provided testcase's classname and component
+mapping.
 
-   UUID of test result.
+**Arguments:**
 
-*  ``_tbl_result_time_start``
+*  ``dConfig``
 
-   / *Condition*: required / *Type*: str /
+   / *Condition*: required / *Type*: dict /
 
-   Result start time as format ``%Y-%m-%d %H:%M:%S``.
+   Configuration which contains the mapping between component and testcase's classname.
 
-*  ``_tbl_result_time_end``
+*  ``sTestClassname``
 
    / *Condition*: required / *Type*: str /
 
-   Result end time as format ``%Y-%m-%d %H:%M:%S``.
+   Testcase's classname to get the component info.
 
 **Returns:**
 
-(*no returns*)
-      """
-      sql,sqlval="""update """ + self.db + """.tbl_result set time_start=%s, time_end=%s
-                  where test_result_id='""" + _tbl_test_result_id + "'" , \
-                  (_tbl_result_time_start, _tbl_result_time_end)
-      self.__arExec(sql,sqlval)
-
-   def arGetCategories(self):
-      """
-Get existing categories.
-
-**Arguments:**
-
-(*no arguments*)
-
-**Returns:**
-
-*  ``arCategories``
-
-   / *Type*: list /
-
-   List of exsiting categories.
-      """
-      sql="""select category from """ + self.db + """.tbl_result_categories"""
-      res=self.__arExec(sql, bHasResponse=True)
-      arCategories=[]
-      for cat in res:
-         arCategories.append(cat[0])
-      return arCategories
-
-   #
-   # create abort reason entry
-   #
-   def vCreateAbortReason(self,
-                          _tbl_test_result_id,
-                          _tbl_abort_reason,
-                          _tbl_abort_message
-                           ):
-      """
-Create abort reason entry.
-
-**Arguments:**
+*  ``sComponent``
 
-*  ``_tbl_test_result_id``
-
-   / *Condition*: required / *Type*: str /
+   / *Type*: typle /
 
-   UUID of test result.
-
-*  ``_tbl_abort_reason``
-
-   / *Condition*: required / *Type*: str /
+   Component name maps with given testcase's classname.
+   Otherwise, "unknown" will be return as component name.
+   """
+   sComponent = "unknown"
 
-   Abort reason.
+   if dConfig != None and "components" in dConfig:
+      # component info as object in json file
+      if isinstance(dConfig["components"], dict):
+         for cmpt in dConfig["components"]:
+            # component name maps with an array of classnames
+            if isinstance(dConfig["components"][cmpt], list):
+               bFound = False
+               for clsName in dConfig["components"][cmpt]:
+                  if clsName in sTestClassname:
+                     sComponent = cmpt
+                     bFound = True
+                     break
+               if bFound:
+                  break
+            # component maps with single classname
+            elif isinstance(dConfig["components"][cmpt], str):
+               if dConfig["components"][cmpt] in sTestClassname:
+                  sComponent = cmpt
+                  break
+      # component info as string in json file
+      elif isinstance(dConfig["components"], str) and dConfig["components"].strip() != "":
+         sComponent = dConfig["components"]
 
-*  ``_tbl_abort_message``
+   return sComponent
 
-   / *Condition*: required / *Type*: str /
+def process_config_file(config_file):
+   """
+Parse information from configuration file:
 
-   Detail message of abort.
+*  ``component``:
 
-**Returns:**
+   .. code:: python
 
-(*no returns*)
-      """
-      sql,sqlval = """insert into """ + self.db + """.tbl_abort
-                           (test_result_id, abort_reason, msg_detail)
-                           values (%s,%s,%s)""" , (_tbl_test_result_id,
-                                                   _tbl_abort_reason,
-                                                   _tbl_abort_message,
-                                                   )
-      self.__arExec(sql,sqlval)
+      {
+         "components" : {
+            "componentA" : "componentA/path/to/testcase",
+            "componentB" : "componentB/path/to/testcase",
+            "componentC" : [
+               "componentC1/path/to/testcase",
+               "componentC2/path/to/testcase"
+            ]
+         }
+      }
 
-   def vCreateReanimation(self, _tbl_test_result_id, _tbl_num_of_reanimation):
-      """
-Create reanimation entry.
+   Then all testcases which their paths contain ``componentA/path/to/testcase``
+   will be belong to ``componentA``, ...
 
 **Arguments:**
 
-*  ``_tbl_test_result_id``
+*  ``config_file``
 
    / *Condition*: required / *Type*: str /
 
-   UUID of test result.
-
-*  ``_tbl_num_of_reanimation``
-
-   / *Condition*: required / *Type*: int /
-
-   Counter of target reanimation during execution.
+   Path to configuration file.
 
 **Returns:**
 
-(*no returns*)
-      """
-      sql, sqlval = """update """ + self.db + """.tbl_result set num_of_reanimation=%s where
-                        test_result_id='""" + _tbl_test_result_id + "'", (_tbl_num_of_reanimation)
-      self.__arExec(sql, sqlval)
-
-   def vCreateCCRdata(self, _tbl_test_case_id, lCCRdata):
-      """
-Create CCR data per test case.
+*  ``dConfig``
 
-**Arguments:**
+   / *Type*: dict /
 
-*  ``_tbl_test_case_id``
-
-   / *Condition*: required / *Type*: int /
-
-   test case ID.
-
-*  ``lCCRdata``
+   Configuration object.
+   """
 
-   / *Condition*: required / *Type*: list /
+   with open(config_file, encoding='utf-8') as f:
+      try:
+         dConfig = json.load(f)
+      except Exception as reason:
+         Logger.log_error(f"Cannot parse the json file '{config_file}'. Reason: {reason}", fatal_error=True)
 
-   list of CCR data.
+   if not is_valid_config(dConfig, bExitOnFail=False):
+      Logger.log_error(f"Error in configuration file '{config_file}'.", fatal_error=True)
 
-**Returns:**
+   return dConfig
 
-(*no returns*)
-      """
-      sql = """insert into """ + self.db + """.tbl_ccr (test_case_id, timestamp, MEM, CPU) values(%s,%s,%s,%s)"""
-      sqlVals = []
-      for row in lCCRdata:
-         row.insert(0, _tbl_test_case_id)
-         sqlVals.append(tuple(row))
-      self.__vExecMany(sql, sqlVals)
-
-   def vFinishTestResult(self,_tbl_test_result_id):
-      """
-Finish upload:
-
-* First do bulk insert of rest of test cases if buffer is not empty.
-* Then set state to "new report".
+def process_test(db, test, file_id, test_result_id, component_name, test_number, start_time):
+   """
+Process test case data and create new test case record.
 
 **Arguments:**
 
-*  ``_tbl_test_result_id``
+*  ``db``
 
-   / *Condition*: required / *Type*: str /
+   / *Condition*: required / *Type*: `CDataBase` object /
 
-   UUID of test result.
+   CDataBase object.
 
-**Returns:**
+*  ``test``
 
-(*no returns*)
-      """
-      if len(self.lTestCases) > 0:
-         self.vEnableForeignKeyCheck(False)
-         self.__vUploadTestCaseListToDb(self.lTestCases)
-         self.vEnableForeignKeyCheck(True)
-      sql="""update """ + self.db + """.tbl_result set result_state="new report"
-                  where test_result_id='""" + _tbl_test_result_id + "'"
-      self.__arExec(sql)
+   / *Condition*: required / *Type*: `etree._Element` object /
 
-   def vUpdateEvtbls(self):
-      """
-Call ``update_evtbls`` stored procedure.
+   Robot test object.
 
-**Arguments:**
+*  ``file_id``
 
-(*no arguments*)
+   / *Condition*: required / *Type*: int /
 
-**Returns:**
+   File ID for mapping.
 
-(*no returns*)
-      """
-      sql="""call """ + self.db + """.update_evtbls();"""
-      self.__arExec(sql)
+*  ``test_result_id``
 
-   def vUpdateEvtbl(self, _tbl_test_result_id):
-      """
-Call ``update_evtbl`` stored procedure to update provided ``test_result_id``.
+   / *Condition*: required / *Type*: str /
 
-**Arguments:**
+   Test result ID for mapping.
 
-*  ``_tbl_test_result_id``
+*  ``component_name``
 
    / *Condition*: required / *Type*: str /
 
-   UUID of test result.
+   Component name which this test case is belong to.
 
-**Returns:**
+*  ``test_number``
 
-(*no returns*)
-      """
-      sql="""call """ + self.db + """.update_evtbl('%s');"""%_tbl_test_result_id
-      self.__arExec(sql)
-
-   def vEnableForeignKeyCheck(self, enable=True):
-      """
-Switch ``foreign_key_checks`` flag.
+   / *Condition*: required / *Type*: int /
 
-**Arguments:**
+   Order of test case in file.
 
-*  ``enable``
+*  ``start_time``
 
-   / *Condition*: optional / *Type*: bool / *Default*: True /
+   / *Condition*: required / *Type*: `datetime` object /
 
-   If True, enable foreign key constraint.
+   Start time of testcase.
 
 **Returns:**
 
-(*no returns*)
-      """
-      sql = "SET FOREIGN_KEY_CHECKS=%s;" %str(int(enable))
-      self.__arExec(sql)
-
-   def sGetLatestFileID(self, _tbl_test_result_id):
-      """
-Get latest file ID from ``tbl_file`` table.
+   / *Type*: float /
 
-**Arguments:**
-
-*  ``_tbl_test_result_id``
-
-   / *Condition*: required / *Type*: str /
-
-   UUID of test result.
-
-**Returns:**
-
-*  ``_tbl_file_id``
+   Duration (in second) of test execution.
+   """
+   global iTotalTestcase
+   global iSuccessTestcase
+   global dComponentCounter
+   iTotalTestcase += 1
+   _tbl_case_name  = test.get("name")
+   _tbl_case_issue = ""
+   _tbl_case_tcid  = ""
+   _tbl_case_fid   = ""
+   _tbl_case_testnumber  = test_number
+   _tbl_case_repeatcount = 1
+   _tbl_case_component   = component_name
+   _tbl_case_time_start  = datetime.strftime(start_time, DB_DATETIME_FORMAT)
+   if _tbl_case_component not in dComponentCounter:
+      dComponentCounter[_tbl_case_component] = 0
+
+   try:
+      _tbl_case_result_main, _tbl_case_lastlog, _tbl_case_result_return = get_test_result(test)
+   except Exception as reason:
+      Logger.log_error(f"Error when getting PyTest result of test '{_tbl_case_name}'. Reason: {reason}", fatal_error=True)
+      return
+
+   _tbl_case_result_state   = "complete"
+   _tbl_case_result_return  = 11
+   _tbl_case_counter_resets = 0
+   _tbl_test_result_id = test_result_id
+   _tbl_file_id = file_id
+
+   if not Logger.dryrun:
+      try:
+         tbl_case_id = db.nCreateNewSingleTestCase(_tbl_case_name,
+                                                   _tbl_case_issue,
+                                                   _tbl_case_tcid,
+                                                   _tbl_case_fid,
+                                                   _tbl_case_testnumber,
+                                                   _tbl_case_repeatcount,
+                                                   _tbl_case_component,
+                                                   _tbl_case_time_start,
+                                                   _tbl_case_result_main,
+                                                   _tbl_case_result_state,
+                                                   _tbl_case_result_return,
+                                                   _tbl_case_counter_resets,
+                                                   _tbl_case_lastlog,
+                                                   _tbl_test_result_id,
+                                                   _tbl_file_id
+                                                )
+      except Exception as reason:
+         Logger.log_error(f"Cannot create new test case result for test '{_tbl_case_name}' in database.\nReason: {reason}")
+         return float(test.get("time"))
+   else:
+      tbl_case_id = "testcase id for dryrun"
+   iSuccessTestcase += 1
+   dComponentCounter[_tbl_case_component] += 1
+   component_msg = f" (component: {_tbl_case_component})" if _tbl_case_component != "unknown" else ""
+   Logger.log(f"Created test case result for test '{_tbl_case_name}' successfully: {str(tbl_case_id)}{component_msg}", indent=4)
 
-   / *Type*: int /
+   return float(test.get("time"))
 
-   File ID.
-      """
-      sql = "SELECT MAX(file_id) FROM %s.tbl_file WHERE test_result_id='%s'"%(self.db, _tbl_test_result_id)
-      _tbl_file_id = self.__arExec(sql,bHasResponse=True)[0][0]
-      return _tbl_file_id
+def process_suite(db, suite, _tbl_test_result_id, dConfig=None):
+   """
+Process to the lowest suite level (test file):
 
-   def vUpdateFileEndTime(self, _tbl_file_id, _tbl_file_time_end):
-      """
-Update test file end time.
+* Create new file and its header information
+* Then, process all child test cases
 
 **Arguments:**
 
-*  ``_tbl_file_id``
-
-   / *Condition*: required / *Type*: int /
-
-   File ID to be updated.
+*  ``db``
 
-*  ``_tbl_file_time_end``
+   / *Condition*: required / *Type*: `CDataBase` object /
 
-   / *Condition*: required / *Type*: str /
+   CDataBase object.
 
-   File end time as format ``%Y-%m-%d %H:%M:%S``.
+*  ``suite``
 
-**Returns:**
+   / *Condition*: required / *Type*: `etree._Element` object /
 
-(*no returns*)
-      """
-      sql = "UPDATE %s.tbl_file SET time_end='%s' WHERE file_id=%s"%(self.db, _tbl_file_time_end, _tbl_file_id)
-      self.__arExec(sql)
-
-   def vUpdateResultEndTime(self, _tbl_test_result_id, _tbl_result_time_end):
-      """
-Update test result end time.
-
-**Arguments:**
+   Robot suite object.
 
 *  ``_tbl_test_result_id``
 
    / *Condition*: required / *Type*: str /
 
-   Result UUID to be updated.
+   UUID of test result for importing.
 
-*  ``_tbl_result_time_end``
+*  ``dConfig``
 
-   / *Condition*: required / *Type*: str /
+   / *Condition*: required / *Type*: dict / *Default*: None /
 
-   Result end time as format ``%Y-%m-%d %H:%M:%S``.
+   Configuration data which is parsed from given json configuration file.
 
 **Returns:**
 
 (*no returns*)
-      """
-      sql = "UPDATE %s.tbl_result SET time_end='%s' WHERE test_result_id='%s'"%(self.db, _tbl_result_time_end, _tbl_test_result_id)
-      self.__arExec(sql)
-
-   def bExistingResultID(self, _tbl_test_result_id):
-      """
-Verify the given test result UUID is existing in ``tbl_result`` table or not.
-
-**Arguments:**
-
-*  ``_tbl_test_result_id``
-
-   / *Condition*: required / *Type*: str /
-
-   Result UUID to be verified.
-
-**Returns:**
+   """
 
-*  ``bExisting``
+   # File metadata
+   previous_file_name = ""
+   _tbl_file_id = None
+   _tbl_file_tester_account = dConfig["tester"]
+   _tbl_file_tester_machine = suite.get("hostname")
+   _tbl_file_time_start = suite.get("timestamp")
+   test_start_time      = datetime.strptime(_tbl_file_time_start, PYTEST_DATETIME_FORMAT)
+   _tbl_file_time_end   = datetime.strftime(test_start_time + timedelta(seconds=float(suite.get("time"))), DB_DATETIME_FORMAT)
+
+   test_number = 1
+   for test in suite.iterchildren("testcase"):
+      _tbl_file_name = test.get("classname")
+      component_name = process_component_info(dConfig, _tbl_file_name)
+      # Create new testfile if not existing in this execution (different classname with previous one)
+      if previous_file_name != _tbl_file_name:
+         _tbl_header_testtoolconfiguration_testtoolname      = ""
+         _tbl_header_testtoolconfiguration_testtoolversion   = ""
+         _tbl_header_testtoolconfiguration_pythonversion     = ""
+         if dConfig["testtool"]:
+            sFindstring = r"([a-zA-Z\s\_]+[^\s])\s+([\d\.rcab]+)\s+\(Python\s+(.*)\)"
+            oTesttool = re.search(sFindstring, dConfig["testtool"])
+            if oTesttool:
+               _tbl_header_testtoolconfiguration_testtoolname    = oTesttool.group(1)
+               _tbl_header_testtoolconfiguration_testtoolversion = oTesttool.group(2)
+               _tbl_header_testtoolconfiguration_pythonversion   = oTesttool.group(3)
+
+         _tbl_header_testtoolconfiguration_projectname     = dConfig["variant"]
+         _tbl_header_testtoolconfiguration_logfileencoding = "UTF-8"
+         _tbl_header_testtoolconfiguration_testfile        = _tbl_file_name
+         _tbl_header_testtoolconfiguration_logfilepath     = ""
+         _tbl_header_testtoolconfiguration_logfilemode     = ""
+         _tbl_header_testtoolconfiguration_ctrlfilepath    = ""
+         _tbl_header_testtoolconfiguration_configfile      = ""
+         _tbl_header_testtoolconfiguration_confname        = ""
+
+         _tbl_header_testfileheader_author           = dConfig["tester"]
+         _tbl_header_testfileheader_project          = dConfig["variant"]
+         _tbl_header_testfileheader_testfiledate     = ""
+         _tbl_header_testfileheader_version_major    = ""
+         _tbl_header_testfileheader_version_minor    = ""
+         _tbl_header_testfileheader_version_patch    = ""
+         _tbl_header_testfileheader_keyword          = ""
+         _tbl_header_testfileheader_shortdescription = ""
+         _tbl_header_testexecution_useraccount       = dConfig["tester"]
+         _tbl_header_testexecution_computername      = _tbl_file_tester_machine
+
+         _tbl_header_testrequirements_documentmanagement = ""
+         _tbl_header_testrequirements_testenvironment    = ""
+
+         _tbl_header_testbenchconfig_name    = ""
+         _tbl_header_testbenchconfig_data    = ""
+         _tbl_header_preprocessor_filter     = ""
+         _tbl_header_preprocessor_parameters = ""
+
+         if not Logger.dryrun:
+            try:
+               _tbl_file_id = db.nCreateNewFile(_tbl_file_name,
+                                                _tbl_file_tester_account,
+                                                _tbl_file_tester_machine,
+                                                _tbl_file_time_start,
+                                                _tbl_file_time_end,
+                                                _tbl_test_result_id)
+               db.vCreateNewHeader(_tbl_file_id,
+                                 _tbl_header_testtoolconfiguration_testtoolname,
+                                 _tbl_header_testtoolconfiguration_testtoolversion,
+                                 _tbl_header_testtoolconfiguration_projectname,
+                                 _tbl_header_testtoolconfiguration_logfileencoding,
+                                 _tbl_header_testtoolconfiguration_pythonversion,
+                                 _tbl_header_testtoolconfiguration_testfile,
+                                 _tbl_header_testtoolconfiguration_logfilepath,
+                                 _tbl_header_testtoolconfiguration_logfilemode,
+                                 _tbl_header_testtoolconfiguration_ctrlfilepath,
+                                 _tbl_header_testtoolconfiguration_configfile,
+                                 _tbl_header_testtoolconfiguration_confname,
+
+                                 _tbl_header_testfileheader_author,
+                                 _tbl_header_testfileheader_project,
+                                 _tbl_header_testfileheader_testfiledate,
+                                 _tbl_header_testfileheader_version_major,
+                                 _tbl_header_testfileheader_version_minor,
+                                 _tbl_header_testfileheader_version_patch,
+                                 _tbl_header_testfileheader_keyword,
+                                 _tbl_header_testfileheader_shortdescription,
+                                 _tbl_header_testexecution_useraccount,
+                                 _tbl_header_testexecution_computername,
+
+                                 _tbl_header_testrequirements_documentmanagement,
+                                 _tbl_header_testrequirements_testenvironment,
+
+                                 _tbl_header_testbenchconfig_name,
+                                 _tbl_header_testbenchconfig_data,
+                                 _tbl_header_preprocessor_filter,
+                                 _tbl_header_preprocessor_parameters
+                                 )
+            except Exception as reason:
+               Logger.log_error(f"Cannot create new test file result for file '{_tbl_file_name}' in database.\nReason: {reason}",
+                                  fatal_error=True)
+         else:
+            _tbl_file_id = "file id for dryrun"
+         Logger.log(f"Created test file result for classname '{_tbl_file_name}' successfully: {str(_tbl_file_id)}", indent=2)
+         previous_file_name = _tbl_file_name
+
+      # Process testcase
+      if _tbl_file_id:
+         duration = process_test(db, test, _tbl_file_id, _tbl_test_result_id, component_name, test_number, test_start_time)
+         test_start_time += timedelta(seconds=duration)
+         test_number += 1
+      else:
+         Logger.log_error(f"No found testfile ID for classname {_tbl_file_name}.", fatal_error=True)
 
-   / *Type*: bool /
+def PyTestLog2DB(args=None):
+   """
+Import pytest results from ``*.xml`` file(s) to TestResultWebApp's database.
 
-   True if test result UUID is already existing.
-      """
-      sql = "SELECT test_result_id FROM %s.tbl_result WHERE test_result_id='%s'"%(self.db, _tbl_test_result_id)
-      res = self.__arExec(sql, bHasResponse=True)
-      bExisting = False
-      if res and len(res)>0:
-         bExisting = True
-      return bExisting
+Flow to import PyTest results to database:
 
-   def arGetProjectVersionSWByID(self, _tbl_test_result_id):
-      """
-Get the project and version_sw information of given `test_result_id`
+1. Process provided arguments from command line.
+2. Parse PyTest results.
+3. Connect to database.
+4. Import results into database.
+5. Disconnect from database.
 
 **Arguments:**
 
-*  ``_tbl_test_result_id``
+*  ``args``
 
-   / *Condition*: required / *Type*: str /
+   / *Condition*: required / *Type*: `ArgumentParser` object /
 
-   Result UUID to be get the information.
+   Argument parser object which contains:
 
-**Returns:**
+   * `resultxmlfile` : path to the xml result file or directory of result files to be imported.
+   * `server` : server which hosts the database (IP or URL).
+   * `user` : user for database login.
+   * `password` : password for database login.
+   * `database` : database name.
+   * `recursive` : if True, then the path is searched recursively for log files to be imported.
+   * `dryrun` : if True, then verify all input arguments (includes DB connection) and show what would be done.
+   * `append` : if True, then allow to append new result(s) to existing execution result UUID which is provided by --UUID argument.
+   * `UUID` : UUID used to identify the import and version ID on TestResultWebApp.
+   * `variant` : variant name to be set for this import.
+   * `versions` : metadata: Versions (Software;Hardware;Test) to be set for this import.
+   * `config` : configuration json file for component mapping information.
 
-*  / *Type*: tuple /
+**Returns:**
 
-   None if test result UUID is not existing, else the tuple which contains project and version_sw: (project, variant) is returned.
-      """
-      sql = "SELECT project, version_sw_target FROM %s.tbl_result WHERE test_result_id='%s'"%(self.db, _tbl_test_result_id)
-      res = self.__arExec(sql, bHasResponse=True)
-      if res and len(res)>0:
-         return res[0]
+(*no returns*)
+   """
+   # 1. process provided arguments from command line as default
+   args = __process_commandline()
+   Logger.config(dryrun=args.dryrun)
+
+   # 2. Parse results from PyTest xml result file(s)
+   listEntries = collect_xml_result_files(args.resultxmlfile, args.recursive)
+
+   pytest_result = parse_pytest_xml(*listEntries)
+
+   # Validate provided UUID
+   if args.UUID!=None:
+      if is_valid_uuid(args.UUID):
+         pass
+      else:
+         Logger.log_error(f"The uuid provided is not valid: '{args.UUID}'", fatal_error=True)
+
+   # Validate provided versions info (software;hardware;test)
+   arVersions = []
+   if args.versions!=None and args.versions.strip() != "":
+      arVersions=args.versions.split(";")
+      arVersions=[x.strip() for x in arVersions]
+      if len(arVersions)>3:
+         Logger.log_error(f"The provided versions information is not valid: '{str(args.versions)}'",
+                          fatal_error=True)
+
+   # Validate provided configuration file (component, variant, version_sw)
+   dConfig = {}
+   if args.config != None:
+      if os.path.isfile(args.config):
+         dConfig = process_config_file(args.config)
+      else:
+         Logger.log_error(f"The provided config file is not existing: '{args.config}'", fatal_error=True)
+
+   # Set default value for missing metadata bases on DEFAULT_METADATA
+   for key in DEFAULT_METADATA:
+      if key not in dConfig:
+         dConfig[key] = DEFAULT_METADATA[key]
+
+
+   # 3. Connect to database
+   db = DBAccessFactory().create(args.interface)
+   try:
+      db.connect(args.server,
+                 args.user,
+                 args.password,
+                 args.database,
+                 "utf8mb4")
+   except Exception as reason:
+      Logger.log_error(f"Could not connect to database: '{reason}'", fatal_error=True)
+
+   # 4. Import results into database
+   #    Create new execution result in database
+   #    |
+   #    '---Create new file result(s)
+   #        |
+   #        '---Create new test result(s)
+   try:
+      bUseDefaultPrjVariant = True
+      bUseDefaultVersionSW  = True
+      sMsgVarirantSetBy = sMsgVersionSWSetBy = "default value"
+
+      # Process project/variant
+      sVariant = dConfig["variant"]
+      if args.variant!=None and args.variant.strip() != "":
+         bUseDefaultPrjVariant = False
+         sMsgVarirantSetBy = "from --variant commandline argument"
+         sVariant = args.variant.strip()
+      elif sVariant != DEFAULT_METADATA["variant"]:
+         bUseDefaultPrjVariant = False
+         sMsgVarirantSetBy = f"from configuration '{args.config}' file provided by --config"
+      _tbl_prj_project = _tbl_prj_variant = sVariant
+
+      # Process versions info
+      sVersionSW = dConfig["version_sw"]
+      sVersionHW = dConfig["version_hw"]
+      sVersionTest = dConfig["version_test"]
+      if sVersionSW != DEFAULT_METADATA["version_sw"]:
+         bUseDefaultVersionSW = False
+         sMsgVersionSWSetBy = f"from configuration '{args.config}' file provided by --config"
+      if len(arVersions) > 0:
+         bUseDefaultVersionSW = False
+         sMsgVersionSWSetBy = "from --versions commandline argument"
+         if len(arVersions)==1 or len(arVersions)==2 or len(arVersions)==3:
+            sVersionSW = arVersions[0]
+         if len(arVersions)==2 or len(arVersions)==3:
+            sVersionHW = arVersions[1]
+         if len(arVersions)==3:
+            sVersionTest = arVersions[2]
+      _tbl_result_version_sw_target = sVersionSW
+      _tbl_result_version_hardware  = sVersionHW
+      _tbl_result_version_sw_test   = sVersionTest
+
+      # Set version as start time of the execution if not provided in metadata
+      # Format: %Y%m%d_%H%M%S from %Y-%m-%d %H:%M:%S
+      if _tbl_result_version_sw_target=="":
+         _tbl_result_version_sw_target = datetime.strftime(datetime.strptime(pytest_result.get("starttime"), DB_DATETIME_FORMAT), "%Y%m%d_%H%M%S")
+
+      if not args.append:
+         Logger.log(f"Set project/variant to '{sVariant}' ({sMsgVarirantSetBy})")
+         Logger.log(f"Set version_sw to '{_tbl_result_version_sw_target}' ({sMsgVersionSWSetBy})")
+
+      # Process branch info from software version
+      _tbl_prj_branch = get_branch_from_swversion(_tbl_result_version_sw_target)
+
+      # Process UUID info
+      if args.UUID != None:
+         _tbl_test_result_id = args.UUID
+      else:
+         _tbl_test_result_id = str(uuid.uuid4())
+         if args.append:
+            Logger.log_error("'--append' argument should be used in combination with '--UUID <UUID>` argument.", fatal_error=True)
+
+      # Process start/end time info
+      _tbl_result_time_start = pytest_result.get("starttime")
+      _tbl_result_time_end   = pytest_result.get("endtime")
+
+      # Process other info
+      _tbl_result_interpretation = ""
+      _tbl_result_jenkinsurl     = ""
+      _tbl_result_reporting_qualitygate = ""
+
+      # Check the UUID is existing or not
+      error_indent = len(Logger.prefix_fatalerror)*' '
+      _db_result_info = db.arGetProjectVersionSWByID(_tbl_test_result_id)
+      if _db_result_info:
+         if args.append:
+            # Check given variant/project and version_sw (not default values) with existing values in db
+            _db_prj_variant = _db_result_info[0]
+            _db_version_sw  = _db_result_info[1]
+            if not bUseDefaultPrjVariant and _tbl_prj_variant != _db_prj_variant:
+               Logger.log_error(f"Given project/variant '{_tbl_prj_variant}' ({sMsgVarirantSetBy}) is different with existing value '{_db_prj_variant}' in database.", fatal_error=True)
+            elif not bUseDefaultVersionSW and _tbl_result_version_sw_target != _db_version_sw:
+               Logger.log_error(f"Given version software '{_tbl_result_version_sw_target}' ({sMsgVersionSWSetBy}) is different with existing value '{_db_version_sw}' in database.", fatal_error=True)
+            else:
+               Logger.log(f"Append to existing test execution result for variant '{_db_prj_variant}' - version '{_db_version_sw}' - UUID '{_tbl_test_result_id}'.")
+         else:
+            Logger.log_error(f"Execution result with UUID '{_tbl_test_result_id}' is already existing. \
+               \n{error_indent}Please use other UUID (or remove '--UUID' argument from your command) for new execution result. \
+               \n{error_indent}Or add '--append' argument in your command to append new result(s) to this existing UUID.",
+               fatal_error=True)
+      else:
+         if args.append:
+            Logger.log_error(f"Execution result with UUID '{_tbl_test_result_id}' is not existing for appending.\
+               \n{error_indent}Please use an existing UUID to append new result(s) to that UUID. \
+               \n{error_indent}Or remove '--append' argument in your command to create new execution result with given UUID.",
+               fatal_error=True)
+         else:
+            # Process new test result
+            if not Logger.dryrun:
+               db.sCreateNewTestResult(_tbl_prj_project,
+                                       _tbl_prj_variant,
+                                       _tbl_prj_branch,
+                                       _tbl_test_result_id,
+                                       _tbl_result_interpretation,
+                                       _tbl_result_time_start,
+                                       _tbl_result_time_end,
+                                       _tbl_result_version_sw_target,
+                                       _tbl_result_version_sw_test,
+                                       _tbl_result_version_hardware,
+                                       _tbl_result_jenkinsurl,
+                                       _tbl_result_reporting_qualitygate)
+            Logger.log(f"Created test execution result for variant '{_tbl_prj_variant}' - version '{_tbl_result_version_sw_target}' successfully: {str(_tbl_test_result_id)}")
+   except Exception as reason:
+      Logger.log_error(f"Could not create new execution result in database. Reason: {reason}", fatal_error=True)
+
+   for suite in pytest_result.iterchildren("testsuite"):
+      process_suite(db, suite, _tbl_test_result_id, dConfig)
+
+   if not Logger.dryrun:
+      db.vUpdateEvtbls()
+      db.vFinishTestResult(_tbl_test_result_id)
+      if args.append:
+         db.vUpdateEvtbl(_tbl_test_result_id)
+
+   # 5. Disconnect from database
+   db.disconnect()
+   import_mode_msg = "appended" if args.append else "written"
+   testcnt_msg = f"All {iTotalTestcase}"
+   extended_msg = ""
+   if (iTotalTestcase>iSuccessTestcase):
+      testcnt_msg  = f"{iSuccessTestcase} of {iTotalTestcase}"
+      extended_msg = f" {iTotalTestcase-iSuccessTestcase} test cases are skipped because of errors."
+   Logger.log()
+   Logger.log(f"{testcnt_msg} test cases are {import_mode_msg} to database successfully.{extended_msg}")
+
+   # Components's statistics
+   iMaxlenCmptStr = len(max(dComponentCounter, key=len))
+   for component in dComponentCounter:
+      Logger.log(f"Component {component.ljust(iMaxlenCmptStr, ' ')} : {dComponentCounter[component]} test cases")
 
-      return None
+if __name__=="__main__":
+   PyTestLog2DB()
```

### Comparing `PyTestLog2DB-0.2.8/PyTestLog2DB/PyTestLog2DB.pdf` & `PyTestLog2DB-0.3.0/PyTestLog2DB/PyTestLog2DB.pdf`

 * *Files 16% similar despite different names*

#### Comparing `PyTestLog2DB-0.2.8/PyTestLog2DB/PyTestLog2DB.pdf` & `PyTestLog2DB-0.3.0/PyTestLog2DB/PyTestLog2DB.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20240115122534Z'
+CreationDate: 'D:20240517085601Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20240115122534Z'
+ModDate: 'D:20240517085601Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 PyTestLog2DB
-v. 0.2.8
+v. 0.3.0
 Tran Duy Ngoan
-14.12.2023
+07.05.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -54,246 +54,125 @@
 
 2.2.5
 
 Append to existing execution result . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 5
 
-Display on TestResultWebApp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-7
-
-2.3
-
-3 CDataBase.py
-3.1
-
-8
+2.2.6
 
-Class: CDataBase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Switch Database Access Interface . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-8
-
-3.1.1
+6
 
-Method: connect . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+Display on TestResultWebApp . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
 8
 
-3.1.2
-
-Method: disconnect . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-9
-
-3.1.3
-
-Method: cleanAllTables . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-9
-
-3.1.4
+2.3
 
-Method: sCreateNewTestResult . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3 pytestlog2db.py
 
 9
 
-3.1.5
-
-Method: nCreateNewFile . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-10
-
-3.1.6
-
-Method: vCreateNewHeader . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-11
-
-3.1.7
-
-Method: nCreateNewSingleTestCase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-13
-
-3.1.8
-
-Method: nCreateNewTestCase . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-14
-
-3.1.9
-
-Method: vCreateTags . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-15
-
-3.1.10 Method: vSetCategory . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-15
-
-3.1.11 Method: vUpdateStartEndTime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-16
-
-3.1.12 Method: arGetCategories . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-16
-
-3.1.13 Method: vCreateAbortReason . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-16
-
-3.1.14 Method: vCreateReanimation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-17
-
-3.1.15 Method: vCreateCCRdata . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-17
-
-3.1.16 Method: vFinishTestResult . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-17
-
-3.1.17 Method: vUpdateEvtbls . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-17
-
-3.1.18 Method: vUpdateEvtbl . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-18
-
-3.1.19 Method: vEnableForeignKeyCheck . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-18
-
-3.1.20 Method: sGetLatestFileID . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-18
-
-3.1.21 Method: vUpdateFileEndTime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-18
-
-3.1.22 Method: vUpdateResultEndTime . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-19
-
-3.1.23 Method: bExistingResultID . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-
-19
-
-A
-
-CONTENTS
-
-CONTENTS
-
-3.1.24 Method: arGetProjectVersionSWByID . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
-4 pytestlog2db.py
-
-19
-20
-
-4.1
+3.1
 
 Function: collect xml result files . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-20
+9
 
-4.2
+3.2
 
 Function: validate xml result . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-20
+9
 
-4.3
+3.3
 
 Function: is valid uuid . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-21
+10
 
-4.4
+3.4
 
 Function: is valid config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-21
+10
 
-4.5
+3.5
 
 Function: parse pytest xml . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-22
+11
 
-4.6
+3.6
 
 Function: get branch from swversion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-22
+11
 
-4.7
+3.7
 
 Function: get test result . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-22
+11
 
-4.8
+3.8
 
 Function: process component info . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-23
+12
 
-4.9
+3.9
 
 Function: process config file . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-23
+12
 
-4.10 Function: process test . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.10 Function: process test . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-24
+13
 
-4.11 Function: process suite . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.11 Function: process suite . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-24
+13
 
-4.12 Function: PyTestLog2DB . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.12 Function: PyTestLog2DB . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+14
 
-4.13 Class: Logger . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.13 Class: Logger . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-25
+14
 
-4.13.1 Method: config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.13.1 Method: config . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+15
 
-4.13.2 Method: log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.13.2 Method: log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+15
 
-4.13.3 Method: log warning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.13.3 Method: log warning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-26
+15
 
-4.13.4 Method: log error . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
+3.13.4 Method: log error . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . .
 
-27
+16
 
-5 Appendix
+4 Appendix
 
-28
+17
 
-6 History
+5 History
 
-29
+18
 
-B
+A
 
 CHAPTER 1. INTRODUCTION
 
 Chapter 1
 
 Introduction
 PyTestLog2DB is a command-line tool that enables you to import pytest XML result files into TestResultWebApp’s
@@ -385,21 +264,25 @@
 CHAPTER 2. DESCRIPTION
 
 2.2. TOOL FEATURES
 
 If not provided PyTestLog2DB will generate an UUID for the whole ←,→ import.
 --variant VARIANT
 --versions VERSIONS
---config CONFIG
 
 variant name to be set for this import.
 metadata: Versions (Software;Hardware;Test) to be set for this import
 (semicolon separated)
 configuration json file for component mapping information.
 
+--config CONFIG
+--interface {db,rest}
+
+database access interface.
+
 The below command is simple usage with all required arguments to import pytest results into TestResultWebApp’s
 database:
 PyTestLog2DB resultxmlfile server user password database
 
 Besides the executable file, you can also run tool as a Python module
 python -m PyTestLog2DB resultxmlfile server user password database
 
@@ -618,18 +501,59 @@
 version_sw
 are provided within
 When using append mode and
 --variant VARIANT , --versions VERSIONS or --config CONFIG arguments, they will be validated with the existing values in database.
 An error will be raised in case the given value is not matched with the existing ones. E.g:
 FATAL ERROR: Given version software 'my_version' is different with existing ←,→ value 'SW01' in database.
 
+2.2.6
+
+Switch Database Access Interface
+
+In addition to direct database connections — which can sometimes be restricted or prohibited due to security concerns
+— the PyTestLog2DB tool also provides users with an alternative way (interface) to import test data into the
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
+PyTestLog2DB output.xml db host db user db password db name --interface db
+
+This method provides flexibility, allowing users to choose between interfaces explicitly or rely on the default behavior.
+REST API Backend (interface=”rest”)
+The ’rest’ interface allows users to import data into the database through a REST API. This mode is particularly
+useful in scenarios where direct database connections are restricted or not feasible, such as when the database is
+secured and direct connections are not allowed.
+
 6
 
 CHAPTER 2. DESCRIPTION
 
+2.2. TOOL FEATURES
+
+PyTestLog2DB output.xml api endpoint api user api password db name --interface rest
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
+7
+
+CHAPTER 2. DESCRIPTION
+
 2.3
 
 2.3. DISPLAY ON TESTRESULTWEBAPP
 
 Display on TestResultWebApp
 
 As soon as the *.xml file(s) is imported sucessfully to database, the result for that execution will be available on
@@ -637,780 +561,22 @@
 Dashboard view:
 
 Figure 2.1: Dashboard view
 Datatable view:
 
 Figure 2.2: Datatable view
 
-7
-
-CHAPTER 3. CDATABASE.PY
-
-Chapter 3
-
-CDataBase.py
-3.1
-
-Class: CDataBase
-
-Imported by:
-from PyTestLog2DB.CDataBase import CDataBase
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
 8
 
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
-9
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
-10
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
-11
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
-12
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
-13
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
+CHAPTER 3. PYTESTLOG2DB.PY
 
-/ Condition: required / Type: str /
-Test case start time as format %Y-%m-%d %H:%M:%S.
- tbl case result main
-
-/ Condition: required / Type: str /
-Test case main result.
-
-14
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
-15
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
-16
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
-17
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
-18
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
-19
-
-CHAPTER 4. PYTESTLOG2DB.PY
-
-Chapter 4
+Chapter 3
 
 pytestlog2db.py
-4.1
+3.1
 
 Function: collect xml result files
 
 Collect all valid Robot xml result file in given path.
 Arguments:
  path
 
@@ -1422,15 +588,15 @@
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
 
@@ -1444,21 +610,21 @@
 
 / Condition: optional / Type: bool / Default: True /
 If set, exit with fatal error if the schema validation of given xml file failed.
 Returns:
  / Type: bool /
 
 True if the given xml result is valid with the provided schema *.xsd.
-20
+9
 
-CHAPTER 4. PYTESTLOG2DB.PY
+CHAPTER 3. PYTESTLOG2DB.PY
 
-4.3
+3.3
 
-4.3. FUNCTION: IS VALID UUID
+3.3. FUNCTION: IS VALID UUID
 
 Function: is valid uuid
 
 Verify the given UUID is valid or not.
 Arguments:
  uuid to test
 
@@ -1470,15 +636,15 @@
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
@@ -1506,21 +672,21 @@
 If True, exit tool in case the validation is fail.
 Returns:
  bValid
 
 / Type: bool /
 True if the given json configuration data is valid.
 
-21
+10
 
-CHAPTER 4. PYTESTLOG2DB.PY
+CHAPTER 3. PYTESTLOG2DB.PY
 
-4.5
+3.5
 
-4.5. FUNCTION: PARSE PYTEST XML
+3.5. FUNCTION: PARSE PYTEST XML
 
 Function: parse pytest xml
 
 Parse and merge all given pytest *.xml result files into one result file.Besides, starttime and endtime are also calculated
 and added in the merged result.
 Arguments:
  xmlfiles
@@ -1529,15 +695,15 @@
 Path to pytest *.xml result file(s).
 Returns:
  oMergedTree
 
 / Type: etree. Element object /
 The result object which is parsed from provided pytest *.xml result file(s).
 
-4.6
+3.6
 
 Function: get branch from swversion
 
 Get branch name from software version information.
 Convention of branch information in suffix of software version:
  All software version with .0F is the main/freature branch. The leading number is the current year. E.g.
 17.0F03
@@ -1551,35 +717,35 @@
 Software version.
 Returns:
  branch name
 
 / Type: str /
 Branch name.
 
-4.7
+3.7
 
 Function: get test result
 
 Get test result from provided Testcase object.
 Arguments:
  oTest
 
 / Condition: required / Type: etree. Element object /
 Testcase object.
 Returns:
 / Type: typle /
 Testcase result which contains result main, lastlog and result return.
 
-22
+11
 
-CHAPTER 4. PYTESTLOG2DB.PY
+CHAPTER 3. PYTESTLOG2DB.PY
 
-4.8
+3.8
 
-4.8. FUNCTION: PROCESS COMPONENT INFO
+3.8. FUNCTION: PROCESS COMPONENT INFO
 
 Function: process component info
 
 Return the component name bases on provided testcase’s classname and component mapping.
 Arguments:
  dConfig
 
@@ -1594,15 +760,15 @@
 
 / Type: typle /
 Component name maps with given testcase’s classname. Otherwise, ”unknown” will be return as component
 name.
 
 Function: process config file
 
-4.9
+3.9
 
 Parse information from configuration file:
  component:
 
 {
 "components" : {
 "componentA" : "componentA/path/to/testcase",
@@ -1622,21 +788,21 @@
 Path to configuration file.
 Returns:
  dConfig
 
 / Type: dict /
 Configuration object.
 
-23
+12
 
-CHAPTER 4. PYTESTLOG2DB.PY
+CHAPTER 3. PYTESTLOG2DB.PY
 
-4.10
+3.10
 
-4.10. FUNCTION: PROCESS TEST
+3.10. FUNCTION: PROCESS TEST
 
 Function: process test
 
 Process test case data and create new test case record.
 Arguments:
  db
 
@@ -1666,15 +832,15 @@
 
 / Condition: required / Type: datetime object /
 Start time of testcase.
 Returns:
 / Type: float /
 Duration (in second) of test execution.
 
-4.11
+3.11
 
 Function: process suite
 
 Process to the lowest suite level (test file):
  Create new file and its header information
  Then, process all child test cases
 
@@ -1684,32 +850,32 @@
 / Condition: required / Type: CDataBase object /
 CDataBase object.
  suite
 
 / Condition: required / Type: etree. Element object /
 Robot suite object.
 
-24
+13
 
-CHAPTER 4. PYTESTLOG2DB.PY
+CHAPTER 3. PYTESTLOG2DB.PY
 
-4.12. FUNCTION: PYTESTLOG2DB
+3.12. FUNCTION: PYTESTLOG2DB
 
  tbl test result id
 
 / Condition: required / Type: str /
 UUID of test result for importing.
  dConfig
 
 / Condition: required / Type: dict / Default: None /
 Configuration data which is parsed from given json configuration file.
 Returns:
 (no returns)
 
-4.12
+3.12
 
 Function: PyTestLog2DB
 
 Import pytest results from *.xml file(s) to TestResultWebApp’s database.
 Flow to import PyTest results to database:
 1. Process provided arguments from command line.
 2. Parse PyTest results.
@@ -1733,30 +899,30 @@
 – UUID : UUID used to identify the import and version ID on TestResultWebApp.
 – variant : variant name to be set for this import.
 – versions : metadata: Versions (Software;Hardware;Test) to be set for this import.
 – config : configuration json file for component mapping information.
 Returns:
 (no returns)
 
-4.13
+3.13
 
 Class: Logger
 
 Imported by:
 
-25
+14
 
-CHAPTER 4. PYTESTLOG2DB.PY
+CHAPTER 3. PYTESTLOG2DB.PY
 
-4.13. CLASS: LOGGER
+3.13. CLASS: LOGGER
 
 from PyTestLog2DB.pytestlog2db import Logger
 Logger class for logging message.
 
-4.13.1
+3.13.1
 
 Method: config
 
 Configure Logger class.
 Arguments:
  output console
 
@@ -1773,15 +939,15 @@
  dryrun
 
 / Condition: optional / Type: bool / Default: True /
 If set, a prefix as ’dryrun’ is added for all messages.
 Returns:
 (no returns)
 
-4.13.2
+3.13.2
 
 Method: log
 
 Write log message to console/file output.
 Arguments:
  msg
 
@@ -1794,35 +960,35 @@
  indent
 
 / Condition: optional / Type: int / Default: 0 /
 Offset indent.
 Returns:
 (no returns)
 
-4.13.3
+3.13.3
 
 Method: log warning
 
 Write warning message to console/file output.
 Arguments:
 
-26
+15
 
-CHAPTER 4. PYTESTLOG2DB.PY
+CHAPTER 3. PYTESTLOG2DB.PY
 
-4.13. CLASS: LOGGER
+3.13. CLASS: LOGGER
 
  msg
 
 / Condition: required / Type: str /
 Warning message which is written to output.
 Returns:
 (no returns)
 
-4.13.4
+3.13.4
 
 Method: log error
 
 Write error message to console/file output.
 Arguments:
  msg
 
@@ -1831,38 +997,38 @@
  fatal error
 
 / Condition: optional / Type: bool / Default: False /
 If set, tool will terminate after logging error message.
 Returns:
 (no returns)
 
-27
+16
 
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
 
 PyTestLog2DB
 
 Version
 
-0.2.8
+0.3.0
 
 Date
 
-14.12.2023
+07.05.2024
 
 Description
 
 Imports pytest result(s) to TestResultWebApp database
 
 Package URL
 
@@ -1900,19 +1066,19 @@
 
 Intended Audience :: Developers
 
 Topic
 
 Topic :: Software Development
 
-28
+17
 
-CHAPTER 6. HISTORY
+CHAPTER 5. HISTORY
 
-Chapter 6
+Chapter 5
 
 History
 0.1.0
 
 11/2022
 
 Initial version
@@ -1968,15 +1134,27 @@
 
 Update README for publishing package to PyPI
 0.2.8
 
 14.12.2023
 
 Fix missing return of test duration when failed to import testcase
+0.3.0
+
+07.05.2024
+
+Add optional argument
+and rest interfaces
+
+--interface
+
+which allow to switch between
 
 PyTestLog2DB.pdf
-Created at 15.01.2024 - 12:25:32
+Created at 17.05.2024 - 08:55:59
 by GenPackageDoc v. 0.41.1
 
-29
+18
+
+db
```

### Comparing `PyTestLog2DB-0.2.8/PyTestLog2DB/__init__.py` & `PyTestLog2DB-0.3.0/PyTestLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.8/PyTestLog2DB/__main__.py` & `PyTestLog2DB-0.3.0/PyTestLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.8/PyTestLog2DB/xsd/junit.xsd` & `PyTestLog2DB-0.3.0/PyTestLog2DB/xsd/junit.xsd`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.2.8/PyTestLog2DB.egg-info/PKG-INFO` & `PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.2.8
+Version: 0.3.0
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -152,14 +152,16 @@
     --recursive          if set, then the path is searched recursively for output files to be imported.
     --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
     --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
     --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided PyTestLog2DB will generate an UUID for the whole import.
     --variant VARIANT    variant name to be set for this import.
     --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
     --config CONFIG      configuration json file for component mapping information.
+    --interface {db,rest}
+                         database access interface.
 
 The below command is simple usage with all required arguments to import
 [pytest](https://docs.pytest.org) results into TestResultWebApp\'s
 database:
 
     PyTestLog2DB <resultxmlfile> <server> <user> <password> <database>
```

### Comparing `PyTestLog2DB-0.2.8/README.rst` & `PyTestLog2DB-0.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,16 @@
    --recursive          if set, then the path is searched recursively for output files to be imported.
    --dryrun             if set, then verify all input arguments (includes DB connection) and show what would be done.
    --append             is used in combination with --UUID <UUID>. If set, allow to append new result(s) to existing execution result UUID in --UUID argument.
    --UUID UUID          UUID used to identify the import and version ID on webapp. If not provided PyTestLog2DB will generate an UUID for the whole import.
    --variant VARIANT    variant name to be set for this import.
    --versions VERSIONS  metadata: Versions (Software;Hardware;Test) to be set for this import (semicolon separated).
    --config CONFIG      configuration json file for component mapping information.
+   --interface {db,rest}
+                        database access interface.
 
 
 The below command is simple usage with all required arguments to import
 pytest_ results into TestResultWebApp's database:
 
 ::
```

### Comparing `PyTestLog2DB-0.2.8/setup.py` & `PyTestLog2DB-0.3.0/setup.py`

 * *Files identical despite different names*

