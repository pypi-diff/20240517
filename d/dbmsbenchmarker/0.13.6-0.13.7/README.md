# Comparing `tmp/dbmsbenchmarker-0.13.6.tar.gz` & `tmp/dbmsbenchmarker-0.13.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/DBMS-Benchmarker/DBMS-Benchmarker/dist/.tmp-bernedti/dbmsbenchmarker-0.13.6.tar", last modified: Wed Feb 14 06:21:45 2024, max compression
+gzip compressed data, was "/home/runner/work/DBMS-Benchmarker/DBMS-Benchmarker/dist/.tmp-hip66lo2/dbmsbenchmarker-0.13.7.tar", last modified: Fri May 17 11:49:46 2024, max compression
```

## Comparing `dbmsbenchmarker-0.13.6.tar` & `dbmsbenchmarker-0.13.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    97695 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/benchmarker.py
--rw-r--r--   0 runner    (1001) docker     (127)    36381 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    27997 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)    22030 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    28564 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/check_box-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/check_box_outline_blank-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/clear-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/get_app-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/info-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/radio_button_unchecked-24px.svg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/tune-black-24dp.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/styles.css
--rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   137186 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/dashboardcli.py
--rw-r--r--   0 runner    (1001) docker     (127)    77528 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 06:21:45.000000 dbmsbenchmarker-0.13.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-14 06:21:39.000000 dbmsbenchmarker-0.13.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10182 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98237 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/benchmarker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36491 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28813 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22030 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28802 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18245 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/check_box-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/check_box_outline_blank-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/clear-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/get_app-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/info-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/radio_button_unchecked-24px.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/tune-black-24dp.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8214 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8751 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137186 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/dashboardcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78029 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:49:46.000000 dbmsbenchmarker-0.13.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-17 11:49:42.000000 dbmsbenchmarker-0.13.7/setup.py
```

### Comparing `dbmsbenchmarker-0.13.6/LICENSE` & `dbmsbenchmarker-0.13.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/PKG-INFO` & `dbmsbenchmarker-0.13.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmsbenchmarker
-Version: 0.13.6
+Version: 0.13.7
 Summary: DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.
 Home-page: https://github.com/Beuth-Erdelt/DBMS-Benchmarker
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `dbmsbenchmarker-0.13.6/README.md` & `dbmsbenchmarker-0.13.7/README.md`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/benchmarker.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/benchmarker.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,15 +828,19 @@
             params = tools.joinDicts(params, parameter.defaultParameters)
             return queryTemplate.format(**params)
         # if query is given as a list of strings (create view, ..., drop view)
         if isinstance(queryString,list):
             queryPart = []
             for queryTemplate in queryString:
                 if len(self.protocol['query'][str(numQuery)]['parameter']) > 0:
+                    # parametrized
                     queryPart.append(parametrize(queryTemplate, numQuery, numRun))
+                else:
+                    # not parametrized
+                    queryPart.append(queryTemplate)
             #print(queryPart)
             queryString = queryPart
         else:
             if len(self.protocol['query'][str(numQuery)]['parameter']) > 0:
                 queryString = parametrize(queryString, numQuery, numRun)
         # it is a query template
         #if len(self.protocol['query'][str(numQuery)]['parameter']) > 0:
@@ -1106,15 +1110,18 @@
         keepResultsets = False
         # do we want to cancel / abort loop over benchmarks?
         breakLoop = False
         try:
             # start connecting
             self.timerExecution.startTimer(numQuery, query, connectionname)
             self.timerTransfer.startTimer(numQuery, query, connectionname)
-            if not query.withConnect:
+            if singleConnection and len(self.activeConnections):
+                # we have a global connection
+                self.timerConnect.skipTimer(numQuery, query, connectionname)
+            elif not query.withConnect:
                 # we do not benchmark connection time, so we connect directly and once
                 self.timerConnect.skipTimer(numQuery, query, connectionname)
                 self.connectDBMS(c)
             else:
                 self.timerConnect.startTimer(numQuery, query, connectionname)
             #queryString = query.query
             #if c in query.DBMS:
@@ -1314,22 +1321,22 @@
                         #print(l_data[i])
                         if not l_data[i] == self.protocol['query'][str(numQuery)]['dataStorage'][i]:
                             self.protocol['query'][str(numQuery)]['warnings'][c] = 'NumRun '+str(i+1)+': Received differing result set'
                             self.logger.debug('Received differing result set')
                             keepResultsets = True
                             break
                             #raise ValueError('Received differing result set')
-            #if len(self.resultfolder_subfolder) > 0:
-            # always store complete resultset for subfolders
-            filename = self.path+"/query_"+str(numQuery)+"_resultset_complete_"+connectionname+".pickle"
-            if BENCHMARKER_VERBOSE_PROCESS:
-                self.logger.info("Store pickle of complete result set to "+filename)
-            f = open(filename, "wb")
-            pickle.dump(data, f)
-            f.close()
+            # TODO: why always store complete resultset for subfolders, even if there is none?
+            if not self.resultfolder_subfolder is None and len(self.resultfolder_subfolder) > 0:
+                filename = self.path+"/query_"+str(numQuery)+"_resultset_complete_"+connectionname+".pickle"
+                if BENCHMARKER_VERBOSE_PROCESS:
+                    self.logger.info("Store pickle of complete result set to "+filename)
+                f = open(filename, "wb")
+                pickle.dump(data, f)
+                f.close()
         except Exception as e:
             self.logger.exception('Caught an error: %s' % str(e))
             self.protocol['query'][str(numQuery)]['errors'][c] = 'ERROR ({}) - {}'.format(type(e).__name__, e)
             # store end time for query / connection
             self.protocol['query'][str(numQuery)]['ends'][c] = str(datetime.datetime.now())
             # benchmark is 0 due to error
             self.timerExecution.abortTimerRun()
@@ -1566,25 +1573,27 @@
         # store connection data again, it may have changed
         self.store_connectiondata()
         if self.bBatch:
             # generate reports at the end only
             self.generateReportsAll()
         # stop logging multiprocessing
         mp.log_to_stderr(logging.ERROR)
-    def readResultfolder(self):
+    def readResultfolder(self, silent=False):
         """
         Reads data of previous benchmark from folder.
 
+        :param silent: No output of status
         :return: returns nothing
         """
-        print("Read results")
+        if not silent:
+            print("Read results")
         self.clearBenchmarks()
         # read from stored results
         self.logger.debug("Read from "+self.path)
-        self.reporterStore.readProtocol()
+        self.reporterStore.readProtocol(silent)
         for numQuery,q in enumerate(self.queries):
             query = tools.query(q)
             loaded = self.reporterStore.load(query, numQuery+1, [self.timerExecution, self.timerTransfer, self.timerConnect])
             if not loaded:
                 break
         # show finished benchmarks
         """
@@ -1900,15 +1909,15 @@
 class inspector(benchmarker):
     """
     Class for inspecting done benchmarks
     """
     def __init__(self, result_path, code, anonymize=False, silent=False):
         benchmarker.__init__(self,result_path=result_path+"/"+str(code), anonymize=anonymize)
         self.getConfig()
-        self.readResultfolder()
+        self.readResultfolder(silent=silent)
         if not silent:
             print("Connections:")
             for c in self.connections:
                 print(c['name'])
             print("Queries:")
             for i,q in enumerate(self.queries):
                 if 'active' in q and q['active']:
```

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/evaluator.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,31 +35,32 @@
 import numpy as np
 
 class evaluator():
     evaluation = {}
     """
     Class for generating evaluation cube.
     """
-    def __init__(self, benchmarker, load=False, force=False):
+    def __init__(self, benchmarker, load=False, force=False, silent=False):
         """
         Construct a new 'evaluator' object.
 
         :param benchmarker: Object of benchmarker containing information about queries, connections and benchmark times
+        :param silent: No output of status
         :return: returns nothing
         """
         self.benchmarker = benchmarker
         if force:
             evaluator.evaluation = {}
         if len(evaluator.evaluation) == 0:
             if load:
-                self.load()
+                self.load(silent)
             else:
                 evaluator.evaluation = self.generate()
                 # force to use stored format
-                self.load()
+                self.load(silent)
     def get_evaluation(self):
         return evaluator.evaluation
     def generate(self):
         """
         Prepares a dict containing evaluation data about experiment, dbms query and timer.
         Anonymizes dbms if activated.
 
@@ -410,16 +411,17 @@
         with open(filename, 'w') as f:
             f.write(str(evaluation))
             #pprint.pprint(evaluation, f)
         filename = self.benchmarker.path+'/evaluation.json'
         with open(filename, 'w') as f:
             json.dump(evaluation, f)
         return evaluation
-    def load(self):
-        print("Load Evaluation")
+    def load(self, silent=False):
+        if not silent:
+            print("Load Evaluation")
         filename = self.benchmarker.path+'/evaluation.json'
         with open(filename,'r') as f:
             evaluator.evaluation = json.load(f)
             #evaluator.evaluation = ast.literal_eval(inp.read())
         #filename = self.benchmarker.path+'/evaluation.dict'
         #with open(filename,'r') as f:
         #    #evaluator.evaluation = ast.literal_eval(inp.read())
```

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/inspector.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from os.path import isdir, isfile, join
 import sys
 import ast
 from colour import Color
 from numpy import nan
 from datetime import datetime, timezone
 import copy
+import re
 
 from dbmsbenchmarker import benchmarker, tools, evaluator, monitor
 
 color_ranges = [
     ["#ff0000", "#ffcccc"],
     ["#006600", "#ccffcc"],
     ["#000066", "#ccccff"],
@@ -91,14 +92,19 @@
 
     :param lst1: First list
     :param lst2: Second list
     :return: Intersection
     """
     lst3 = [value for value in lst1 if value in lst2] 
     return lst3 
+def natural_sort(l): 
+    convert = lambda text: int(text) if text.isdigit() else text.lower()
+    alphanum_key = lambda key: [convert(c) for c in re.split('([0-9]+)', key)]
+    return sorted(l, key=alphanum_key)
+
 
 
 class inspector():
     """
     Class for inspecting done benchmarks
     """
     def __init__(self, result_path, anonymize=False):
@@ -140,15 +146,15 @@
         if anonymize is not None:
             self.anonymize = anonymize
         # TODO: force clean dbms aliases
         self.queries_successful = []
         self.benchmarks = benchmarker.inspector(self.result_path, code, anonymize=self.anonymize, silent=silent)
         self.benchmarks.computeTimerRun()
         self.benchmarks.computeTimerSession()
-        self.e = evaluator.evaluator(self.benchmarks, load=load, force=True)
+        self.e = evaluator.evaluator(self.benchmarks, load=load, force=True, silent=silent)
         self.workload = copy.deepcopy(self.e.evaluation['general'])
         # remove metrics
         if 'loadingmetrics' in self.workload:
             del(self.workload['loadingmetrics'])
         if 'streamingmetrics' in self.workload:
             del(self.workload['streamingmetrics'])
         if 'reporting' in self.workload:
@@ -440,14 +446,28 @@
                 filename=initfilename(connection, i)
                 if isfile(filename):
                     script += open(filename).read()
                     i = i + 1
                 else:
                     break
         return script
+    def get_monitoring_metric(self, metric, component="loading"):
+        """
+        Returns list of names of metrics using during monitoring.
+
+        :return: List of monitoring metrics
+        """
+        filename = '/query_{component}_metric_{metric}.csv'.format(component=component, metric=metric)
+        if isfile(self.benchmarks.path+"/"+filename):
+            df = pd.read_csv(self.benchmarks.path+"/"+filename).T
+            #print(df)
+            df = df.reindex(index=natural_sort(df.index))
+            return df.T
+        else:
+            return pd.DataFrame()
     def get_loading_metrics(self, metric):
         return evaluator.dfLoadingMetric(self.e.evaluation, metric)
     def get_streaming_metrics(self, metric):
         return evaluator.dfStreamingMetric(self.e.evaluation, metric)
     def get_loader_metrics(self, metric):
         return evaluator.dfLoaderMetric(self.e.evaluation, metric)
     def get_benchmarker_metrics(self, metric):
```

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/layout.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/layout.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/monitor.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,16 @@
                     metric = connectiondata['monitoring']['metrics'][metric_code].copy()
                 else:
                     metric = metrics.metrics[metric_code].copy()
                 #print(metric)
                 if container is not None:
                     metric['query'] = metric['query'].replace('container_label_io_kubernetes_container_name="dbms"', 'container_label_io_kubernetes_container_name="{}"'.format(container))
                     metric['query'] = metric['query'].replace('container_label_io_kubernetes_container_name!="dbms"', 'container_label_io_kubernetes_container_name!="{}"'.format(container))
+                    metric['query'] = metric['query'].replace('container="dbms"', 'container="{}"'.format(container))
+                    metric['query'] = metric['query'].replace('container!="dbms"', 'container!="{}"'.format(container))
                     # open TODO:
                     # container_label_component="worker"
                     # container_label_component="sut"
                 # this yields seconds
                 # is there a global timeshift
                 if 'grafanashift' in connectiondata['monitoring']:
                     time_shift = connectiondata['monitoring']['grafanashift']
```

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/parameter.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/parameter.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/reporter.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/reporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,18 +175,19 @@
         Saves procol of benchmarker in JSON format.
 
         :return: returns nothing
         """
         filename = self.benchmarker.path+'/protocol.json'
         with open(filename, 'w') as f:
             json.dump(self.benchmarker.protocol, f)
-    def readProtocol(self):
+    def readProtocol(self, silent=False):
         """
         Loads procol of benchmarker in JSON format.
 
+        :param silent: No output of status
         :return: returns nothing
         """
         try:
             filename = self.benchmarker.path+'/protocol.json'
             with open(filename, 'r') as f:
                 self.benchmarker.protocol = json.load(f)
         except Exception as e:
```

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_down.svg`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/icons/chevron_up.svg`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/assets/styles.css` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/assets/styles.css`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/cli.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/scripts/dashboardcli.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/scripts/dashboardcli.py`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker/tools.py` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,15 +376,15 @@
         """
         Creates object and stores data given in dict into object.
 
         :param query: Dict containing query infos - query, numRun, numParallel, withData, warmup, cooldown, title
         :return: returns nothing
         """
         self.maxTime = None
-        self.numRunStd = 5
+        self.numRunStd = 1
         self.numRun = 0
         self.numParallel = 1
         self.warmup = 0
         self.cooldown = 0
         self.active = True
         self.title = ''
         self.DBMS = {}
@@ -458,28 +458,39 @@
             if self.timer['datatransfer']['active']:
                 self.withData = True
             #if 'store' in self.timer['datatransfer'] and self.timer['datatransfer']['store'] == True:
             #    self.storeData = True
             if 'compare' in self.timer['datatransfer'] and self.timer['datatransfer']['compare']:
                 self.result = self.timer['datatransfer']['compare']
                 self.storeData = True
+                self.storeResultSet = True
+                self.storeResultSetFormat = 'dataframe'
             if 'precision' in self.timer['datatransfer']:
                 self.restrict_precision = self.timer['datatransfer']['precision']
                 self.storeData = True
+                self.storeResultSet = True
+                self.storeResultSetFormat = 'dataframe'
             if 'sorted' in self.timer['datatransfer']:
                 self.sorted = self.timer['datatransfer']['sorted']
                 self.storeData = True
-            if 'store' in self.timer['datatransfer'] and not self.timer['datatransfer']['store'] == False:
                 self.storeResultSet = True
-                self.storeData = True
-                if not self.timer['datatransfer']['store'] == True:
-                    if isinstance(self.timer['datatransfer']['store'], str):
-                        self.storeResultSetFormat = [self.timer['datatransfer']['store']]
-                    else:
-                        self.storeResultSetFormat = self.timer['datatransfer']['store']
+                self.storeResultSetFormat = 'dataframe'
+            if 'store' in self.timer['datatransfer']:
+                if self.timer['datatransfer']['store'] == False:
+                    self.storeResultSet = False
+                    self.storeData = False
+                    self.storeResultSetFormat = ''
+                else:
+                    self.storeResultSet = True
+                    self.storeData = True
+                    if not self.timer['datatransfer']['store'] == True:
+                        if isinstance(self.timer['datatransfer']['store'], str):
+                            self.storeResultSetFormat = [self.timer['datatransfer']['store']]
+                        else:
+                            self.storeResultSetFormat = self.timer['datatransfer']['store']
         # timerConnect
         if 'connection' in self.timer:
             if self.timer['connection']['active']:
                 self.withConnect = True
             if 'delay' in self.timer['connection']:
                 self.delay_connect = float(self.timer['connection']['delay'])
         # we do not have a query string, but a list of (other) queries
```

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/PKG-INFO` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbmsbenchmarker
-Version: 0.13.6
+Version: 0.13.7
 Summary: DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.
 Home-page: https://github.com/Beuth-Erdelt/DBMS-Benchmarker
 Author: Patrick Erdelt
 Author-email: perdelt@beuth-hochschule.de
 License: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/SOURCES.txt` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbmsbenchmarker-0.13.6/dbmsbenchmarker.egg-info/requires.txt` & `dbmsbenchmarker-0.13.7/dbmsbenchmarker.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 JayDeBeApi>=1.1.1
 matplotlib>=3.1.1
 numpy>=1.22.2
 pandas>=0.25.1
 tabulate>=0.8.2
 tqdm>=4.28.1
-requests>=2.22.0
+requests>=2.31.0
 JPype1>=1.2.0
 scipy>=1.4.1
 colour>=0.1.5
 Brotli>=1.0.7
-certifi>=2020.4.5.2
+certifi>=2023.7.22
 chardet>=3.0.4
 click>=6.7
 colour>=0.1.5
 cycler>=0.10.0
 dash>=2.15.0
 dash-auth
 dash-core-components
@@ -37,7 +37,8 @@
 urllib3==1.26.18
 uuid>=1.30
 Werkzeug>=3.0.1
 mistune>=2.0.3
 pillow>=10.0.1
 setuptools>=65.5.1
 fonttools>=4.43.0
+jinja2>=3.1.3
```

### Comparing `dbmsbenchmarker-0.13.6/setup.py` & `dbmsbenchmarker-0.13.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="dbmsbenchmarker",
-    version="0.13.6",
+    version="0.13.7",
     author="Patrick Erdelt",
     author_email="perdelt@beuth-hochschule.de",
     description="DBMS-Benchmarker is a Python-based application-level blackbox benchmark tool for Database Management Systems (DBMS). It connects to a given list of DBMS (via JDBC) and runs a given list of parametrized and randomized (SQL) benchmark queries. Evaluations are available via Python interface, in reports and at an interactive multi-dimensional dashboard.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Beuth-Erdelt/DBMS-Benchmarker",
     packages=setuptools.find_packages(),
```

