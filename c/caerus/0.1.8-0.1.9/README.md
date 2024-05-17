# Comparing `tmp/caerus-0.1.8.tar.gz` & `tmp/caerus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caerus-0.1.8.tar", last modified: Fri May 20 17:58:57 2022, max compression
+gzip compressed data, was "caerus-0.1.9.tar", last modified: Wed Mar 22 09:30:16 2023, max compression
```

## Comparing `caerus-0.1.8.tar` & `caerus-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-05-20 17:58:57.034719 caerus-0.1.8/
--rw-rw-rw-   0        0        0     1119 2021-01-17 22:44:45.000000 caerus-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       52 2021-01-17 22:44:45.000000 caerus-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4037 2022-05-20 17:58:57.030495 caerus-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3497 2022-05-20 17:57:00.000000 caerus-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-05-20 17:58:56.990987 caerus-0.1.8/caerus/
--rw-rw-rw-   0        0        0     1127 2022-05-20 17:58:17.000000 caerus-0.1.8/caerus/__init__.py
--rw-rw-rw-   0        0        0    12719 2022-05-20 17:42:34.000000 caerus-0.1.8/caerus/caerus.py
-drwxrwxrwx   0        0        0        0 2022-05-20 17:58:57.020482 caerus-0.1.8/caerus/data/
--rw-rw-rw-   0        0        0        0 2021-01-17 22:44:45.000000 caerus-0.1.8/caerus/data/__init__.py
--rw-rw-rw-   0        0        0      967 2022-03-13 18:40:05.000000 caerus-0.1.8/caerus/examples.py
-drwxrwxrwx   0        0        0        0 2022-05-20 17:58:57.028541 caerus-0.1.8/caerus/utils/
--rw-rw-rw-   0        0        0        0 2021-04-02 09:10:48.000000 caerus-0.1.8/caerus/utils/__init__.py
--rw-rw-rw-   0        0        0     4647 2022-03-13 15:45:56.000000 caerus-0.1.8/caerus/utils/csplots.py
--rw-rw-rw-   0        0        0     7831 2022-05-20 17:53:02.000000 caerus-0.1.8/caerus/utils/csutils.py
--rw-rw-rw-   0        0        0     2778 2022-03-13 15:46:40.000000 caerus-0.1.8/caerus/utils/ones2idx.py
--rw-rw-rw-   0        0        0     8510 2021-01-17 22:44:45.000000 caerus-0.1.8/caerus/utils/risk_performance_metrics.py
-drwxrwxrwx   0        0        0        0 2022-05-20 17:58:57.019485 caerus-0.1.8/caerus.egg-info/
--rw-rw-rw-   0        0        0     4037 2022-05-20 17:58:56.000000 caerus-0.1.8/caerus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2022-05-20 17:58:56.000000 caerus-0.1.8/caerus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-20 17:58:56.000000 caerus-0.1.8/caerus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2022-05-20 17:58:56.000000 caerus-0.1.8/caerus.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-05-20 17:58:56.000000 caerus-0.1.8/caerus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-20 17:58:57.034719 caerus-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1342 2022-03-13 15:33:39.000000 caerus-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-22 09:30:16.723190 caerus-0.1.9/
+-rw-rw-rw-   0        0        0     1119 2021-01-17 22:44:45.000000 caerus-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-01-17 22:44:45.000000 caerus-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4037 2023-03-22 09:30:16.722192 caerus-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3497 2022-05-20 17:57:00.000000 caerus-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-22 09:30:16.661850 caerus-0.1.9/caerus/
+-rw-rw-rw-   0        0        0     1127 2023-03-22 09:26:42.000000 caerus-0.1.9/caerus/__init__.py
+-rw-rw-rw-   0        0        0    12719 2022-05-20 17:42:34.000000 caerus-0.1.9/caerus/caerus.py
+drwxrwxrwx   0        0        0        0 2023-03-22 09:30:16.701721 caerus-0.1.9/caerus/data/
+-rw-rw-rw-   0        0        0        0 2021-01-17 22:44:45.000000 caerus-0.1.9/caerus/data/__init__.py
+-rw-rw-rw-   0        0        0      967 2022-03-13 18:40:05.000000 caerus-0.1.9/caerus/examples.py
+drwxrwxrwx   0        0        0        0 2023-03-22 09:30:16.720198 caerus-0.1.9/caerus/utils/
+-rw-rw-rw-   0        0        0        0 2021-04-02 09:10:48.000000 caerus-0.1.9/caerus/utils/__init__.py
+-rw-rw-rw-   0        0        0     4790 2023-03-22 09:22:13.000000 caerus-0.1.9/caerus/utils/csplots.py
+-rw-rw-rw-   0        0        0     7831 2022-05-20 17:53:02.000000 caerus-0.1.9/caerus/utils/csutils.py
+-rw-rw-rw-   0        0        0     2778 2022-03-13 15:46:40.000000 caerus-0.1.9/caerus/utils/ones2idx.py
+-rw-rw-rw-   0        0        0     8510 2021-01-17 22:44:45.000000 caerus-0.1.9/caerus/utils/risk_performance_metrics.py
+drwxrwxrwx   0        0        0        0 2023-03-22 09:30:16.684900 caerus-0.1.9/caerus.egg-info/
+-rw-rw-rw-   0        0        0     4037 2023-03-22 09:30:15.000000 caerus-0.1.9/caerus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-03-22 09:30:16.000000 caerus-0.1.9/caerus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-22 09:30:15.000000 caerus-0.1.9/caerus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-03-22 09:30:16.000000 caerus-0.1.9/caerus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-22 09:30:16.000000 caerus-0.1.9/caerus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-22 09:30:16.723190 caerus-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2022-03-13 15:33:39.000000 caerus-0.1.9/setup.py
```

### Comparing `caerus-0.1.8/LICENSE` & `caerus-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `caerus-0.1.8/PKG-INFO` & `caerus-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: caerus
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package caerus
 Home-page: https://erdogant.github.io/caerus
-Download-URL: https://github.com/erdogant/caerus/archive/0.1.8.tar.gz
+Download-URL: https://github.com/erdogant/caerus/archive/0.1.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: caerus Version: 0.1.8 Summary: Python package
+Metadata-Version: 2.1 Name: caerus Version: 0.1.9 Summary: Python package
 caerus Home-page: https://erdogant.github.io/caerus Download-URL: https://
-github.com/erdogant/caerus/archive/0.1.8.tar.gz Author: Erdogan Taskesen
+github.com/erdogant/caerus/archive/0.1.9.tar.gz Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE # caerus [!
 [Python](https://img.shields.io/pypi/pyversions/caerus)](https://
 img.shields.io/pypi/pyversions/caerus) [![PyPI Version](https://img.shields.io/
 pypi/v/caerus)](https://pypi.org/project/caerus/) [![License](https://
```

### Comparing `caerus-0.1.8/README.md` & `caerus-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `caerus-0.1.8/caerus/__init__.py` & `caerus-0.1.9/caerus/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from caerus.caerus import caerus
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 # module level doc-string
 __doc__ = """
 caerus
 =====================================================================
 
 Description
```

### Comparing `caerus-0.1.8/caerus/caerus.py` & `caerus-0.1.9/caerus/caerus.py`

 * *Files identical despite different names*

### Comparing `caerus-0.1.8/caerus/examples.py` & `caerus-0.1.9/caerus/examples.py`

 * *Files identical despite different names*

### Comparing `caerus-0.1.8/caerus/utils/csplots.py` & `caerus-0.1.9/caerus/utils/csplots.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,114 +7,115 @@
 #--------------------------------------------------------------------------
 import warnings
 import caerus.utils.csutils as csutils
 import matplotlib.pyplot as plt
 import numpy as np
 warnings.filterwarnings('ignore')
 
+
 # %%
-def _plot_graph(out, figsize=(15,8)):
+def _plot_graph(out, xlabel='Time', ylabel='Input value', figsize=(15,8)):
     df = out['df']
     fig, ax = plt.subplots(figsize=figsize)
     ax.plot(df['X'].loc[df['peak']], 'or', linewidth=1)
     ax.plot(df['X'].loc[df['valley']], 'og', linewidth=1)
     ax.plot(df['X'], 'k', linewidth=0.5)
     ax.vlines(np.where(df['peak'])[0], df['X'].min(), df['X'].max(), linestyles='--', colors='r')
     ax.vlines(np.where(df['valley'])[0], df['X'].min(), df['X'].max(), linestyles='--', colors='g')
-    
+
     uilabx = np.unique(df['labx'])
     for labx in uilabx:
         if labx>0:
             Iloc = df['labx']==labx
             plt.plot(np.where(Iloc)[0], df['X'].loc[Iloc].values, marker='.', linewidth=0.1)
 
-    ax.set_ylabel('Input value')
-    ax.set_xlabel('Time')
+    ax.set_ylabel(ylabel)
+    ax.set_xlabel(xlabel)
     ax.grid(True)
 
     return ax
 
 # %%
-def _plot_gridsearch(out, figsize=(15,8)):
+def _plot_gridsearch(out, xlabel1='Percentage', ylabel1='winning_balance', xlabel2='Percentage', ylabel2='Nr Trades', figsize=(15,8)):
     # Make figure
-    [fig,(ax1,ax2)]=plt.subplots(2,1, figsize=figsize)
+    fig, (ax1, ax2) = plt.subplots(2,1, figsize=figsize)
 
     # Make plots across the gridsearch
     for k in range(0,len(out['window'])):
         for i in range(0,len(out['minperc'])):
             # label = list(map(( lambda x: 'window_' + x), windows.astype(str)))
             ax1.plot(out['minperc'], out['balances'][:,k], label='window_' + str(out['window'][k]))
             ax2.plot(out['minperc'], out['trades'][:,k], label='window_' + str(out['window'][k]))
 
     # ax1.legend()
     ax1.grid(True)
-    ax1.set_xlabel('Percentage')
-    ax1.set_ylabel('winning_balance')
+    ax1.set_xlabel(xlabel1)
+    ax1.set_ylabel(ylabel1)
     ax2.grid(True)
-    ax2.set_xlabel('Percentage')
-    ax2.set_ylabel('Nr Trades')
+    ax2.set_xlabel(xlabel2)
+    ax2.set_ylabel(ylabel2)
     plt.show()
 
 # Make plot
-def _plot(out, threshold=0.25, figsize=(25,15)):
+def _plot(out, threshold=0.25, xlabel='Time', ylabel='Input value', figsize=(25,15)):
     df = out['X']
     loc_start = out['loc_start']
     loc_stop = out['loc_stop']
     loc_start_best = out['loc_start_best']
     loc_stop_best = out['loc_stop_best']
     simmat = out['simmat']
 
     # Top plot
     # agg = out['agg']
-    fig, (ax1,ax2,ax3) = plt.subplots(3,1, figsize=figsize)
+    fig, (ax1, ax2, ax3) = plt.subplots(3, 1, figsize=figsize)
     # Make heatmap
     ax1.matshow(np.flipud(simmat.T))
     ax1.set_aspect('auto')
     # ax1.gca().set_aspect('auto')
     ax1.grid(False)
     ax1.set_ylabel('Perc.difference in window\n(higher=better)')
-    ax1.set_xlim(0,simmat.shape[0])
+    ax1.set_xlim(0, simmat.shape[0])
 
     xlabels = simmat.columns.values.astype(str)
-    Iloc=np.mod(simmat.columns.values,10)==0
+    Iloc=np.mod(simmat.columns.values, 10)==0
     xlabels[Iloc==False]=''
     xlabels[-1]=simmat.columns.values[-1].astype(str)
     xlabels[0]=simmat.columns.values[0].astype(str)
-    ax1.set_yticks(range(0,len(xlabels)))
+    ax1.set_yticks(range(0, len(xlabels)))
     ax1.set_yticklabels(np.flipud(xlabels))
     ax1.grid(True, axis='x')
 
     # make aggregated figure
     # Normalized successes across the n windows for percentages above minperc.
     # 1 depicts that for location i, all of the 1000 windows of different length was succesfull in computing a percentage above minperc
     [outagg, I] = csutils._agg_scores(simmat, threshold)
     ax2.plot(outagg)
     ax2.grid(True)
     ax2.set_ylabel('Cummulative\n#success windows')
-    ax2.set_xlim(0,simmat.shape[0])
-    ax2.hlines(threshold,0,simmat.shape[0], linestyles='--', colors='r')
+    ax2.set_xlim(0, simmat.shape[0])
+    ax2.hlines(threshold, 0, simmat.shape[0], linestyles='--', colors='r')
 
     # Plot local maxima
     if loc_stop_best is not None:
-        ax2.vlines(loc_stop_best,0,1, linestyles='--', colors='r')
-        ax3.plot(df.iloc[loc_stop_best],'or', linewidth=1)
+        ax2.vlines(loc_stop_best, 0, 1, linestyles='--', colors='r')
+        ax3.plot(df.iloc[loc_stop_best], 'or', linewidth=1)
     # Plot local minima
     if loc_start_best is not None:
-        ax2.vlines(loc_start_best,0,1, linestyles='--', colors='g')
-        ax3.plot(df.iloc[loc_start_best],'og', linewidth=1)
+        ax2.vlines(loc_start_best, 0, 1, linestyles='--', colors='g')
+        ax3.plot(df.iloc[loc_start_best], 'og', linewidth=1)
 
         for i in range(0,len(loc_start)):
             ax3.plot(df.iloc[np.arange(loc_start[i][0],loc_start[i][1])],'g', linewidth=2)
             for k in range(0,len(loc_stop[i])):
                 ax3.plot(df.iloc[np.arange(loc_stop[i][k][0],loc_stop[i][k][1])],'r', linewidth=2)
     # Plot region-minima-maxima
     ax3.plot(df,'k', linewidth=1)
 
-    ax3.set_ylabel('Input value')
-    ax3.set_xlabel('Time')
+    ax3.set_xlabel(xlabel)
+    ax3.set_ylabel(ylabel)
     ax3.grid(True)
     ax3.set_xlim(0,simmat.shape[0])
     if loc_start_best is not None:
         ax3.vlines(loc_start_best,df.min(),df.max(), linestyles='--', colors='g')
     if loc_stop_best is not None:
         ax3.vlines(loc_stop_best,df.min(),df.max(), linestyles='--', colors='r')
     plt.show()
```

### Comparing `caerus-0.1.8/caerus/utils/csutils.py` & `caerus-0.1.9/caerus/utils/csutils.py`

 * *Files identical despite different names*

### Comparing `caerus-0.1.8/caerus/utils/ones2idx.py` & `caerus-0.1.9/caerus/utils/ones2idx.py`

 * *Files identical despite different names*

### Comparing `caerus-0.1.8/caerus/utils/risk_performance_metrics.py` & `caerus-0.1.9/caerus/utils/risk_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `caerus-0.1.8/caerus.egg-info/PKG-INFO` & `caerus-0.1.9/caerus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: caerus
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package caerus
 Home-page: https://erdogant.github.io/caerus
-Download-URL: https://github.com/erdogant/caerus/archive/0.1.8.tar.gz
+Download-URL: https://github.com/erdogant/caerus/archive/0.1.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: caerus Version: 0.1.8 Summary: Python package
+Metadata-Version: 2.1 Name: caerus Version: 0.1.9 Summary: Python package
 caerus Home-page: https://erdogant.github.io/caerus Download-URL: https://
-github.com/erdogant/caerus/archive/0.1.8.tar.gz Author: Erdogan Taskesen
+github.com/erdogant/caerus/archive/0.1.9.tar.gz Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3
 Description-Content-Type: text/markdown License-File: LICENSE # caerus [!
 [Python](https://img.shields.io/pypi/pyversions/caerus)](https://
 img.shields.io/pypi/pyversions/caerus) [![PyPI Version](https://img.shields.io/
 pypi/v/caerus)](https://pypi.org/project/caerus/) [![License](https://
```

### Comparing `caerus-0.1.8/setup.py` & `caerus-0.1.9/setup.py`

 * *Files identical despite different names*

