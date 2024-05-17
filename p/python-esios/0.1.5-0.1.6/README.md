# Comparing `tmp/python_esios-0.1.5.tar.gz` & `tmp/python_esios-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_esios-0.1.5.tar", last modified: Wed May 15 10:48:34 2024, max compression
+gzip compressed data, was "python_esios-0.1.6.tar", last modified: Fri May 17 06:57:16 2024, max compression
```

## Comparing `python_esios-0.1.5.tar` & `python_esios-0.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:34.807633 python_esios-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-15 10:48:27.000000 python_esios-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 10:48:34.807633 python_esios-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 10:48:27.000000 python_esios-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:34.803633 python_esios-0.1.5/esios/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:27.000000 python_esios-0.1.5/esios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-15 10:48:27.000000 python_esios-0.1.5/esios/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:34.803633 python_esios-0.1.5/esios/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-15 10:48:27.000000 python_esios-0.1.5/esios/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:34.803633 python_esios-0.1.5/esios/endpoints/archives/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-15 10:48:27.000000 python_esios-0.1.5/esios/endpoints/archives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:34.803633 python_esios-0.1.5/esios/endpoints/archives/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-15 10:48:27.000000 python_esios-0.1.5/esios/endpoints/archives/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-05-15 10:48:27.000000 python_esios-0.1.5/esios/endpoints/archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:34.803633 python_esios-0.1.5/esios/endpoints/indicators/
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-15 10:48:27.000000 python_esios-0.1.5/esios/endpoints/indicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 10:48:34.807633 python_esios-0.1.5/python_esios.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-15 10:48:34.000000 python_esios-0.1.5/python_esios.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-15 10:48:34.000000 python_esios-0.1.5/python_esios.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 10:48:34.000000 python_esios-0.1.5/python_esios.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 10:48:34.000000 python_esios-0.1.5/python_esios.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 10:48:34.000000 python_esios-0.1.5/python_esios.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 10:48:34.807633 python_esios-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 10:48:27.000000 python_esios-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.327729 python_esios-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 06:57:08.000000 python_esios-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 06:57:16.327729 python_esios-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 06:57:08.000000 python_esios-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/archives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/archives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/archives/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/archives/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.323729 python_esios-0.1.6/esios/endpoints/indicators/
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-05-17 06:57:08.000000 python_esios-0.1.6/esios/endpoints/indicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:57:16.327729 python_esios-0.1.6/python_esios.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 06:57:16.000000 python_esios-0.1.6/python_esios.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:57:16.327729 python_esios-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-17 06:57:08.000000 python_esios-0.1.6/setup.py
```

### Comparing `python_esios-0.1.5/LICENSE` & `python_esios-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.5/PKG-INFO` & `python_esios-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.5/esios/api_client.py` & `python_esios-0.1.6/esios/api_client.py`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.5/esios/endpoints/archives/__init__.py` & `python_esios-0.1.6/esios/endpoints/archives/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,21 +13,30 @@
         data = response.json()
         
         if as_dataframe:
             return pd.DataFrame(data['archives'])
         else:
             return data
 
-    def get(self, archive_id, start_date, end_date, output_dir='.'):
+    def get(self, archive_id, start_date=None, end_date=None, date_type='datos'):
+        """
+        start_date : str, optional
+            The start date of the data to retrieve (format: 'YYYY-MM-DD').
+        end_date : str, optional
+            The end date of the data to retrieve (format: 'YYYY-MM-DD').
+        date_type : str {'datos', 'publicacion'}, default 'datos'
+            The type of date to filter by. Options are 'datos' (data date) or 'publicacion' (publication date).
+        """
+        
+        params = {'date_type': date_type}
         
-        params = {
-            'start_date': start_date,
-            'end_date': end_date,
-            'date_type': 'datos'
-        }
+        if start_date:
+            params['start_date'] = start_date
+        if end_date:
+            params['end_date'] = end_date
         
         endpoint = f"/archives/{archive_id}"
         response = self._api_call('GET', endpoint, params=params)
     
         return ArchiveData(response.json(), self.base_url)
 
 
@@ -46,15 +55,15 @@
             The directory where the archive contents will be extracted.
         """
         data = self.data['archive']['download']
         name = data['name']
         url = self.base_url + data['url']
         
         path = os.path.join(output_dir, name)
-        utils.download_zip(url, path)
+        utils.download_file(url, path)
         
         
     def get_metadata(self):
         """
         Returns the metadata of the archive.
         
         Returns
```

### Comparing `python_esios-0.1.5/esios/endpoints/archives/utils.py` & `python_esios-0.1.6/esios/endpoints/archives/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                 nested_dir = os.path.splitext(member_path)[0]
                 os.makedirs(nested_dir, exist_ok=True)
                 with open(member_path, 'rb') as nested_file:
                     extract_zip(nested_file, nested_dir)
                 os.remove(member_path)  # Remove the nested ZIP file after extraction
                 
                 
-def download_zip(url, output_dir):
+def download_file(url, output_dir):
     """
     Downloads a ZIP file from the given URL and extracts its contents to the specified output directory.
     Handles nested ZIP files by extracting them recursively.
     """
     response = requests.get(url)
     response.raise_for_status()
```

### Comparing `python_esios-0.1.5/esios/endpoints/indicators/__init__.py` & `python_esios-0.1.6/esios/endpoints/indicators/__init__.py`

 * *Files identical despite different names*

### Comparing `python_esios-0.1.5/python_esios.egg-info/PKG-INFO` & `python_esios-0.1.6/python_esios.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esios
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python wrapper for the ESIOS API
 Home-page: https://github.com/datons/python-esios
 Author: Jesús López
 Author-email: jesus.lopez@datons.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python_esios-0.1.5/setup.py` & `python_esios-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 setup(
     name='python-esios',
-    version='0.1.5',
+    version='0.1.6',
     packages=find_packages(),
     install_requires=[
         'requests',
         'pandas',
     ],
     author="Jesús López",
     author_email="jesus.lopez@datons.ai",
```

