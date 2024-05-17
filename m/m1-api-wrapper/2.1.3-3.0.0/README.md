# Comparing `tmp/m1_api_wrapper-2.1.3.tar.gz` & `tmp/m1_api_wrapper-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m1_api_wrapper-2.1.3.tar", last modified: Mon Mar 25 11:30:57 2024, max compression
+gzip compressed data, was "m1_api_wrapper-3.0.0.tar", last modified: Fri May 17 08:56:42 2024, max compression
```

## Comparing `m1_api_wrapper-2.1.3.tar` & `m1_api_wrapper-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-03-25 11:30:57.855654 m1_api_wrapper-2.1.3/
--rw-rw-r--   0 marek     (1000) marek     (1000)       16 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.3/LICENSE
--rw-rw-r--   0 marek     (1000) marek     (1000)      491 2024-03-25 11:30:57.855654 m1_api_wrapper-2.1.3/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      185 2024-03-25 11:14:13.000000 m1_api_wrapper-2.1.3/README.md
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-03-25 11:30:57.855654 m1_api_wrapper-2.1.3/m1_api_wrapper.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)      491 2024-03-25 11:30:57.000000 m1_api_wrapper-2.1.3/m1_api_wrapper.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      342 2024-03-25 11:30:57.000000 m1_api_wrapper-2.1.3/m1_api_wrapper.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-03-25 11:30:57.000000 m1_api_wrapper-2.1.3/m1_api_wrapper.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       34 2024-03-25 11:30:57.000000 m1_api_wrapper-2.1.3/m1_api_wrapper.egg-info/requires.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)       10 2024-03-25 11:30:57.000000 m1_api_wrapper-2.1.3/m1_api_wrapper.egg-info/top_level.txt
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-03-25 11:30:57.855654 m1_api_wrapper-2.1.3/m1wrapper/
--rw-rw-r--   0 marek     (1000) marek     (1000)      126 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.3/m1wrapper/__init__.py
--rw-rw-r--   0 marek     (1000) marek     (1000)      312 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.3/m1wrapper/config.py
--rw-rw-r--   0 marek     (1000) marek     (1000)      730 2024-03-25 11:14:13.000000 m1_api_wrapper-2.1.3/m1wrapper/errors.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     4074 2023-05-16 17:22:41.000000 m1_api_wrapper-2.1.3/m1wrapper/m1wrapper.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     5625 2023-05-16 17:22:41.000000 m1_api_wrapper-2.1.3/m1wrapper/search.py
--rw-rw-r--   0 marek     (1000) marek     (1000)     1308 2023-03-28 15:06:30.000000 m1_api_wrapper-2.1.3/m1wrapper/traverse.py
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2024-03-25 11:30:57.859654 m1_api_wrapper-2.1.3/setup.cfg
--rwxrwxr-x   0 marek     (1000) marek     (1000)      579 2024-03-25 11:14:13.000000 m1_api_wrapper-2.1.3/setup.py
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-05-17 08:56:42.886651 m1_api_wrapper-3.0.0/
+-rw-rw-r--   0 marek     (1000) marek     (1000)       16 2023-03-28 15:06:30.000000 m1_api_wrapper-3.0.0/LICENSE
+-rw-rw-r--   0 marek     (1000) marek     (1000)      491 2024-05-17 08:56:42.886651 m1_api_wrapper-3.0.0/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      185 2024-03-25 11:14:13.000000 m1_api_wrapper-3.0.0/README.md
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-05-17 08:56:42.886651 m1_api_wrapper-3.0.0/m1_api_wrapper.egg-info/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      491 2024-05-17 08:56:42.000000 m1_api_wrapper-3.0.0/m1_api_wrapper.egg-info/PKG-INFO
+-rw-rw-r--   0 marek     (1000) marek     (1000)      342 2024-05-17 08:56:42.000000 m1_api_wrapper-3.0.0/m1_api_wrapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-05-17 08:56:42.000000 m1_api_wrapper-3.0.0/m1_api_wrapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       34 2024-05-17 08:56:42.000000 m1_api_wrapper-3.0.0/m1_api_wrapper.egg-info/requires.txt
+-rw-rw-r--   0 marek     (1000) marek     (1000)       10 2024-05-17 08:56:42.000000 m1_api_wrapper-3.0.0/m1_api_wrapper.egg-info/top_level.txt
+drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-05-17 08:56:42.886651 m1_api_wrapper-3.0.0/m1wrapper/
+-rw-rw-r--   0 marek     (1000) marek     (1000)      126 2023-03-28 15:06:30.000000 m1_api_wrapper-3.0.0/m1wrapper/__init__.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)      312 2023-03-28 15:06:30.000000 m1_api_wrapper-3.0.0/m1wrapper/config.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)      730 2024-04-26 09:05:05.000000 m1_api_wrapper-3.0.0/m1wrapper/errors.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     3893 2024-05-17 08:54:39.000000 m1_api_wrapper-3.0.0/m1wrapper/m1wrapper.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     5367 2024-05-17 08:54:39.000000 m1_api_wrapper-3.0.0/m1wrapper/search.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)     1308 2023-03-28 15:06:30.000000 m1_api_wrapper-3.0.0/m1wrapper/traverse.py
+-rw-rw-r--   0 marek     (1000) marek     (1000)       38 2024-05-17 08:56:42.886651 m1_api_wrapper-3.0.0/setup.cfg
+-rwxrwxr-x   0 marek     (1000) marek     (1000)      579 2024-05-17 08:54:39.000000 m1_api_wrapper-3.0.0/setup.py
```

### Comparing `m1_api_wrapper-2.1.3/m1wrapper/errors.py` & `m1_api_wrapper-3.0.0/m1wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `m1_api_wrapper-2.1.3/m1wrapper/m1wrapper.py` & `m1_api_wrapper-3.0.0/m1wrapper/m1wrapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     LOW = 3,
     NORMAL = 5,
     HIGH = 8,
     HIGHEST = 10
 
 class DetailLevel(str, Enum):
     SCORE = 'score',
-    SYNTHESIS = 'synthesis'
+    BEST_PATH = 'best_path',
+    ALL_PATHS = 'all_paths'
 
 class InvalidTargetStrategy(str, Enum):
     REJECT = 'reject',
     PASS = 'pass'
 
 class MoleculeOneWrapper:
     """
@@ -63,39 +64,36 @@
     def run_batch_search(
             self,
             targets: List[str],
             parameters: Dict = None,
             detail_level = DetailLevel.SCORE,
             priority = Priority.NORMAL,
             invalid_target_strategy = InvalidTargetStrategy.REJECT ,
-            starting_materials: List[str] = None,
             preset = None,
             name = None
     ) -> BatchSearch:
         return BatchSearch(
                 self.api_base_url,
                 self.request_headers,
                 targets=targets,
                 parameters=parameters,
                 detail_level=detail_level,
                 priority=int(priority),
                 invalid_target_strategy=invalid_target_strategy,
-                starting_materials=starting_materials,
                 preset=preset,
                 name=name
             )
 
     def run_batch_search_with_metadata(
             self,
             targets_with_metadata: List[Dict[str, str]],
             parameters: Dict = None,
             detail_level = DetailLevel.SCORE,
             priority = Priority.NORMAL,
             invalid_target_strategy = InvalidTargetStrategy.REJECT ,
-            starting_materials: List[str] = None,
             preset = None,
             name = None
     ) -> BatchSearch:
         targets = []
         targets_with_metadata_copy = copy.deepcopy(targets_with_metadata)
         targets_metadata = {}
         for index, item in enumerate(targets_with_metadata_copy):
@@ -109,15 +107,14 @@
                 self.api_base_url,
                 self.request_headers,
                 targets=targets,
                 parameters=parameters,
                 detail_level=detail_level,
                 priority=int(priority),
                 invalid_target_strategy=invalid_target_strategy,
-                starting_materials=starting_materials,
                 name=name,
                 preset=preset,
                 targets_metadata=targets_metadata
             )
 
     def get_batch_search(self, search_id: str) -> BatchSearch:
         search = BatchSearch.from_id(
```

### Comparing `m1_api_wrapper-2.1.3/m1wrapper/search.py` & `m1_api_wrapper-3.0.0/m1wrapper/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         headers,
         search_id=None,
         targets=None,
         parameters=None,
         detail_level=None,
         priority=None,
         invalid_target_strategy=None,
-        starting_materials=None,
         preset=None,
         name=None,
         targets_metadata=None,
     ):
         self.search_id = search_id
         self.base_url = base_url
         self.headers = headers
@@ -47,31 +46,28 @@
         if self.search_id is None:
             new_search = self.__run(
                     targets=targets,
                     parameters=parameters,
                     detail_level=detail_level,
                     priority=priority,
                     invalid_target_strategy=invalid_target_strategy,
-                    starting_materials=starting_materials,
                     preset=preset,
                     name=name,
                     targets_metadata=targets_metadata
             )
             self.search_id = new_search['id']
 
-    def __prepare_payload(self, targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, preset, name, targets_metadata) -> dict:
+    def __prepare_payload(self, targets, parameters, detail_level, priority, invalid_target_strategy, preset, name, targets_metadata) -> dict:
         payload = {
             'targets': targets,
             'parameters': parameters or {},
             'detail_level': detail_level,
             'priority': priority,
             'invalid_target_strategy': invalid_target_strategy
         }
-        if starting_materials is not None:
-            payload["starting_materials"] = starting_materials
         if preset is not None:
             payload["preset"] = preset 
         if name is not None:
             payload["name"] = name
         if targets_metadata is not None:
             payload['targets_metadata'] = targets_metadata
 
@@ -87,16 +83,16 @@
         )
         adapter = HTTPAdapter(max_retries=retry_strategy)
         http = requests.Session()
         http.mount("https://", adapter)
         http.mount("http://", adapter)
         return http
 
-    def __run(self, targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, preset, name, targets_metadata):
-        payload = self.__prepare_payload(targets, parameters, detail_level, priority, invalid_target_strategy, starting_materials, preset, name, targets_metadata)
+    def __run(self, targets, parameters, detail_level, priority, invalid_target_strategy, preset, name, targets_metadata):
+        payload = self.__prepare_payload(targets, parameters, detail_level, priority, invalid_target_strategy, preset, name, targets_metadata)
         response = self.http.post(
             urljoin(self.base_url, api_search_endpoint),
             data=json.dumps(payload),
             headers=self.headers,
         )
         maybe_handle_error(response)
         return response.json()
```

### Comparing `m1_api_wrapper-2.1.3/m1wrapper/traverse.py` & `m1_api_wrapper-3.0.0/m1wrapper/traverse.py`

 * *Files identical despite different names*

### Comparing `m1_api_wrapper-2.1.3/setup.py` & `m1_api_wrapper-3.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='m1_api_wrapper',
-    version='2.1.3',
+    version='3.0.0',
     description='M1 RetroScore API Wrapper',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Molecule.one',
     author_email='support@molecule.one',
     url='https://github.com/molecule-one/m1wrapper-python',
     license=license,
```

