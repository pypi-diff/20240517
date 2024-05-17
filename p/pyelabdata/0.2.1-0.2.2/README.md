# Comparing `tmp/pyelabdata-0.2.1.tar.gz` & `tmp/pyelabdata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyelabdata-0.2.1.tar", last modified: Thu May 16 10:51:50 2024, max compression
+gzip compressed data, was "pyelabdata-0.2.2.tar", last modified: Thu May 16 17:32:28 2024, max compression
```

## Comparing `pyelabdata-0.2.1.tar` & `pyelabdata-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 10:51:50.060470 pyelabdata-0.2.1/
--rw-rw-rw-   0        0        0     1097 2024-01-25 17:49:20.000000 pyelabdata-0.2.1/LICENSE
--rw-rw-rw-   0        0        0    10883 2024-05-16 10:51:50.058483 pyelabdata-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     9934 2024-05-16 10:06:32.000000 pyelabdata-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 10:51:50.030466 pyelabdata-0.2.1/pyelabdata/
--rw-rw-rw-   0        0        0       27 2024-02-23 10:39:15.000000 pyelabdata-0.2.1/pyelabdata/__init__.py
--rw-rw-rw-   0        0        0    27062 2024-05-16 10:03:05.000000 pyelabdata-0.2.1/pyelabdata/pyelabdata.py
-drwxrwxrwx   0        0        0        0 2024-05-16 10:51:50.057472 pyelabdata-0.2.1/pyelabdata.egg-info/
--rw-rw-rw-   0        0        0    10883 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 10:51:50.000000 pyelabdata-0.2.1/pyelabdata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1154 2024-05-16 10:51:21.000000 pyelabdata-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 10:51:50.060470 pyelabdata-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 17:32:28.133171 pyelabdata-0.2.2/
+-rw-rw-rw-   0        0        0     1097 2024-01-25 17:49:20.000000 pyelabdata-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0    10880 2024-05-16 17:32:28.132179 pyelabdata-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9934 2024-05-16 10:06:32.000000 pyelabdata-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 17:32:28.106170 pyelabdata-0.2.2/pyelabdata/
+-rw-rw-rw-   0        0        0       27 2024-02-23 10:39:15.000000 pyelabdata-0.2.2/pyelabdata/__init__.py
+-rw-rw-rw-   0        0        0    28874 2024-05-16 17:28:38.000000 pyelabdata-0.2.2/pyelabdata/pyelabdata.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:32:28.131170 pyelabdata-0.2.2/pyelabdata.egg-info/
+-rw-rw-rw-   0        0        0    10880 2024-05-16 17:32:28.000000 pyelabdata-0.2.2/pyelabdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-16 17:32:28.000000 pyelabdata-0.2.2/pyelabdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:32:28.000000 pyelabdata-0.2.2/pyelabdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-16 17:32:28.000000 pyelabdata-0.2.2/pyelabdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 17:32:28.000000 pyelabdata-0.2.2/pyelabdata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1151 2024-05-16 17:30:49.000000 pyelabdata-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:32:28.134170 pyelabdata-0.2.2/setup.cfg
```

### Comparing `pyelabdata-0.2.1/LICENSE` & `pyelabdata-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyelabdata-0.2.1/PKG-INFO` & `pyelabdata-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyelabdata
-Version: 0.2.1
+Version: 0.2.2
 Summary: pyelabdata provides functions for simple one-line access to data in eLabFTW
 Author-email: "Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg" <physik-ep@fau.de>, "Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg" <michael.krieger@fau.de>
 Project-URL: Repository, https://github.com/FAU-PHYSIK-EP/pyelabdata
 Project-URL: Issues, https://github.com/FAU-PHYSIK-EP/pyelabdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: elabapi_python
 Requires-Dist: pandas
 Requires-Dist: h5py
-Requires-Dist: ipyparams
 Requires-Dist: matplotlib
 Requires-Dist: pathlib
 Requires-Dist: datetime
-Requires-Dist: IPython
+Requires-Dist: ipylab
+Requires-Dist: asyncio
 
 # pyelabdata
 pyelabdata provides functions for simple one-line access to data stored
 in eLabFTW via Python or Jupyter.
 
 ## Examples
 Examples for the use of pyelabdata can be found in the examples folder.
```

### Comparing `pyelabdata-0.2.1/README.md` & `pyelabdata-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyelabdata-0.2.1/pyelabdata/pyelabdata.py` & `pyelabdata-0.2.2/pyelabdata/pyelabdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 import elabapi_python
 import pandas as pd
 import json
 import h5py
 import tempfile
 import os
 import time
-import ipyparams
 from matplotlib.figure import Figure
 from io import StringIO, BytesIO
 from pathlib import Path
-from datetime import datetime, date, time
-from IPython.display import display, Javascript
+from datetime import datetime, date as dt_date, time as dt_time
+from ipylab import JupyterFrontEnd
+import asyncio
+
 
 __APICLIENT__ = None
 __EXPID__ = None
 
+__APP__ = JupyterFrontEnd()
+
 
 ### General functions ###
 
 
 def connect(host: str, apikey: str):
     """Connect to eLabFTW server API.
     
@@ -253,27 +256,35 @@
     if format == 'html':
         return exp.body_html
     else:
         return exp.body
 
 
 def get_table_data(tableidx: int=0, header: bool=True, 
+                   decimal: str='.', thousands: str=None,
                    datatype: str='np', expid: int=None):   
     """Read and return table data from the body text of an experiment 
     stored in eLabFTW.
 
     Parameters
     ----------
     tableidx : int, optional
         The index of the table to be read; first table has index 0. 
         The default is 0.
     header : bool, optional
         If True, the first table row contains the column names, which
         are used as headings for the pandas dataframe. 
         The default is True.
+    decimal: str, optional
+        Character representing the decimal point.
+        The default is '.'.
+    thousands: str, optional
+        Character used to parse thousands.
+        If None, ',' or '.' is used if decimal is '.' or ',', respectively.
+        The default is None.
     datatype : str, optional
         'df': return a pandas dataframe,
         'np': return a dictionary of numpy arrays for each column. 
         The default is 'np'.
     expid : int, optional
         The id of the experiment in eLabFTW to be read.
         If None, the experiment specified by open_experiment() is used.
@@ -298,15 +309,17 @@
     if expid is None:
         raise RuntimeError('No experiment opened or specified')
    
     # fetch experiment
     exp = exp_api.get_experiment(expid)
     
     # extract table
-    tables = pd.read_html(exp.body_html)
+    if thousands is None:
+        thousands = '.' if decimal==',' else ','
+    tables = pd.read_html(StringIO(exp.body_html), decimal=decimal, thousands=thousands)
     
     # extract selected table and assign header if requested
     if header:
         table = tables[tableidx].iloc[1:]
         table.columns = tables[tableidx].iloc[0]
     else:
         table = tables[tableidx]
@@ -364,17 +377,17 @@
     else:
         value = data[fieldname]['value']
         if data[fieldname]['type'] == 'number':
             return float(value)
         if data[fieldname]['type'] == 'datetime-local':
             return datetime.fromisoformat(value)
         if data[fieldname]['type'] == 'date':
-            return date.fromisoformat(value)
+            return dt_date.fromisoformat(value)
         if data[fieldname]['type'] == 'time':
-            return time.fromisoformat(value)
+            return dt_time.fromisoformat(value)
         else:
             return value
 
         
 ### Read files ###    
     
     
@@ -458,14 +471,15 @@
             'experiments', expid, uploadid, format='binary', 
             _preload_content=False).data
 
     
 def get_file_csv_data(filename: str, 
                       filename_is_long_name: bool=False,
                       header: bool=True, sep: str=',', 
+                      decimal: str='.', thousands: str=None,
                       datatype: str='np', expid: int=None):   
     """Read and return data from a csv-like text file attached to 
     an experiment stored in eLabFTW.
 
     Parameters
     ----------
     filename : str
@@ -476,14 +490,21 @@
     header : bool, optional
         If True, the first table row contains the column names, which
         are used as headings for the pandas dataframe. 
         The default is True.
     sep : str, optional
         The column separator used in the file.
         The default is ','.
+    decimal: str, optional
+        Character representing the decimal point.
+        The default is '.'.
+    thousands: str, optional
+        Character used to parse thousands.
+        If None, ',' or '.' is used if decimal is '.' or ',', respectively.
+        The default is None.
     datatype : str, optional
         'df': return a pandas dataframe,
         'np': return a dictionary of numpy arrays for each column. 
         The default is 'np'.
     expid : int, optional
         The id of the experiment in eLabFTW to be read.
         If None, the experiment specified by open_experiment() is used.
@@ -496,16 +517,19 @@
 
     """
 
     # fetch file data
     filedata = get_file_data(filename, filename_is_long_name, expid).decode('utf-8')
 
     # extract data
+    if thousands is None:
+        thousands = '.' if decimal==',' else ','
     df = pd.read_csv(StringIO(filedata), sep=sep, 
-                     header=(0 if header else 'infer'))
+                     header=(0 if header else 'infer'),
+                     decimal=decimal, thousands=thousands)
 
     # return result
     if datatype == 'df':
         return df
     elif datatype == 'np':
         return __conv_df_to_np(df)
     else:
@@ -594,45 +618,58 @@
         expid = __EXPID__
 
     if expid is None:
         raise RuntimeError('No experiment opened or specified')
    
     # fetch experiment
     exp = exp_api.get_experiment(expid)
-    metadata = json.loads(exp.metadata)
+    if exp.metadata is None:
+        # no metadata yet, then create it
+        metadata = {'extra_fields': {}}
+    else:
+        metadata = json.loads(exp.metadata)
     
     # check if fieldname already exists
     if fieldname in metadata['extra_fields'].keys():
         raise RuntimeError('Fieldname already exists')
     
     if groupname is not None:
+        # no elabftw or extra_fields_groups entries, then create them
+        if 'elabftw' not in metadata.keys():
+            metadata['elabftw'] = {}
+        if 'extra_fields_groups' not in metadata['elabftw'].keys():
+            metadata['elabftw']['extra_fields_groups'] = []
+        
         # check if group already exists
         groupid = [group['id'] for group in metadata['elabftw']['extra_fields_groups'] 
                    if group['name']==groupname]
         groupid = groupid[0] if len(groupid)>0 else None
 
         # create group if not yet existing
         if groupid is None:
-            groupid = max([group['id'] for group in metadata['elabftw']['extra_fields_groups']]) + 1
+            if len(metadata['elabftw']['extra_fields_groups']) > 0:
+                groupid = max([group['id'] for group in metadata['elabftw']['extra_fields_groups']]) + 1
+            else:
+                groupid = 1
             metadata['elabftw']['extra_fields_groups'].append({'id': groupid, 'name': groupname})
     
     # create field
     if fieldtype == 'datetime':
         fieldtype = 'datetime-local'
     metadata['extra_fields'][fieldname] = {'type': fieldtype}
 
     if type(value) != str:
         if fieldtype == 'number':
             value = str(value)
         if fieldtype == 'datetime-local':
             value = datetime.isoformat(value.replace(second=0, microsecond=0))
         if fieldtype == 'date':
-            value = date.isoformat(value)
+            value = dt_date.isoformat(value)
         if fieldtype == 'time':
-            value = time.isoformat(value.replace(second=0, microsecond=0))
+            value = dt_time.isoformat(value.replace(second=0, microsecond=0))
 
     metadata['extra_fields'][fieldname]['value'] = value
     
     if unit is not None:
         metadata['extra_fields'][fieldname]['unit'] = unit
         if units is None:
             units = [unit]
@@ -690,17 +727,17 @@
         fieldtype = metadata['extra_fields'][fieldname]['type']
 
         if fieldtype == 'number':
             value = str(value)
         if fieldtype == 'datetime-local':
             value = datetime.isoformat(value.replace(second=0, microsecond=0))
         if fieldtype == 'date':
-            value = date.isoformat(value)
+            value = dt_date.isoformat(value)
         if fieldtype == 'time':
-            value = time.isoformat(value.replace(second=0, microsecond=0))
+            value = dt_time.isoformat(value.replace(second=0, microsecond=0))
         
     exp_api.patch_experiment(expid, body={'action': 'updatemetadatafield', fieldname: value})
 
     
 def delete_extrafield(fieldname: str, expid: int=None):
     """Delete an extra field in an experiment.
 
@@ -882,14 +919,34 @@
     # create a temporary directory for the file, create it and upload
     with tempfile.TemporaryDirectory() as tmpdir:
         tmpfile = os.path.join(tmpdir, filename)
         df.to_csv(tmpfile, index=index)
         upload_file(tmpfile, comment, replacefile, expid=expid)
     
     
+async def _callback_savenotebook():
+    await __APP__.ready()
+
+    # save current notebook
+    print('Saving file ...')
+    __APP__.commands.execute('docmanager:save')
+
+
+async def _callback_upload(comment: str, replacefile: bool, expid: int):
+    await __APP__.ready()
+
+    # get filename of the current notebook
+    file = os.path.join(os.getcwd(), __APP__.sessions.current_session['name'])
+    print(file)
+    # upload to elabftw
+    print('Uploading to eLabFTW ...')
+    upload_file(file, comment, replacefile, expid=expid)
+    print('Done.')
+
+
 def upload_this_jupyternotebook(comment: str, replacefile: bool=True,
                                 expid: int=None):
     """Saves and uploads the current jupyter notebook
     to an experiment on eLabFTW
     
     Parameters
     ----------
@@ -905,20 +962,12 @@
         The default is None.
         
     Returns
     -------
     None.
 
     """
-   
-    # get Jupyter notebook filename
-    filename = ipyparams.notebook_name
-    file = os.path.join(os.getcwd(), filename)
-    
-    # save notebook and wait for completion
-    start = os.path.getmtime(file)
-    display(Javascript('IPython.notebook.save_checkpoint()'))
-    while os.path.getmtime(file) == start:
-        time.sleep(0.1)
-        
-    # upload to elabftw
-    upload_file(file, comment, replacefile, expid=expid)
+
+    # start async tasks to save and upload notebook
+    asyncio.gather(_callback_savenotebook(), 
+                   _callback_upload(comment, replacefile, expid))
+
```

### Comparing `pyelabdata-0.2.1/pyelabdata.egg-info/PKG-INFO` & `pyelabdata-0.2.2/pyelabdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pyelabdata
-Version: 0.2.1
+Version: 0.2.2
 Summary: pyelabdata provides functions for simple one-line access to data in eLabFTW
 Author-email: "Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg" <physik-ep@fau.de>, "Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg" <michael.krieger@fau.de>
 Project-URL: Repository, https://github.com/FAU-PHYSIK-EP/pyelabdata
 Project-URL: Issues, https://github.com/FAU-PHYSIK-EP/pyelabdata/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: elabapi_python
 Requires-Dist: pandas
 Requires-Dist: h5py
-Requires-Dist: ipyparams
 Requires-Dist: matplotlib
 Requires-Dist: pathlib
 Requires-Dist: datetime
-Requires-Dist: IPython
+Requires-Dist: ipylab
+Requires-Dist: asyncio
 
 # pyelabdata
 pyelabdata provides functions for simple one-line access to data stored
 in eLabFTW via Python or Jupyter.
 
 ## Examples
 Examples for the use of pyelabdata can be found in the examples folder.
```

### Comparing `pyelabdata-0.2.1/pyproject.toml` & `pyelabdata-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyelabdata"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
     { name="Elektronikpraktikum, Department Physik, FAU Erlangen-Nürnberg", email="physik-ep@fau.de" },
     { name="Michael Krieger, Lehrstuhl für Angewandte Physik, FAU Erlangen-Nürnberg", email="michael.krieger@fau.de"}
 ]
 description = "pyelabdata provides functions for simple one-line access to data in eLabFTW"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -24,17 +24,17 @@
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "numpy",
     "elabapi_python",
     "pandas",
     "h5py",
-    "ipyparams",
     "matplotlib",
     "pathlib",
     "datetime",
-    "IPython"
+    "ipylab",
+    "asyncio"
 ]
 
 [project.urls]
 "Repository" = "https://github.com/FAU-PHYSIK-EP/pyelabdata"
 "Issues" = "https://github.com/FAU-PHYSIK-EP/pyelabdata/issues"
```

