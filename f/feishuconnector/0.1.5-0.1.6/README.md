# Comparing `tmp/feishuconnector-0.1.5.tar.gz` & `tmp/feishuconnector-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/feishuconnector-0.1.5.tar", last modified: Mon May 13 08:05:50 2024, max compression
+gzip compressed data, was "dist/feishuconnector-0.1.6.tar", last modified: Fri May 17 00:11:40 2024, max compression
```

## Comparing `feishuconnector-0.1.5.tar` & `feishuconnector-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/
--rw-r--r--   0 root         (0) root         (0)      268 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1089 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1760 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.954038 feishuconnector-0.1.5/feishuconnector/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/feishuconnector/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-13 08:05:21.000000 feishuconnector-0.1.5/feishuconnector/_version.py
--rw-r--r--   0 root         (0) root         (0)      442 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/feishuconnector/encoder.py
--rw-r--r--   0 root         (0) root         (0)    16808 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/feishuconnector/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/feishuconnector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1760 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      381 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-13 08:05:50.000000 feishuconnector-0.1.5/feishuconnector.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      107 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1193 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:05:50.955038 feishuconnector-0.1.5/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/test/run.py
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 08:04:31.000000 feishuconnector-0.1.5/upload.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/
+-rw-r--r--   0 root         (0) root         (0)      268 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1089 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.914301 feishuconnector-0.1.6/feishuconnector/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/feishuconnector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-17 00:10:52.000000 feishuconnector-0.1.6/feishuconnector/_version.py
+-rw-r--r--   0 root         (0) root         (0)      442 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/feishuconnector/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    16970 2024-05-17 00:10:00.000000 feishuconnector-0.1.6/feishuconnector/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/feishuconnector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1760 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      381 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-17 00:11:40.000000 feishuconnector-0.1.6/feishuconnector.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1193 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 00:11:40.915301 feishuconnector-0.1.6/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/test/run.py
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 08:04:31.000000 feishuconnector-0.1.6/upload.sh
```

### Comparing `feishuconnector-0.1.5/LICENSE` & `feishuconnector-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feishuconnector-0.1.5/PKG-INFO` & `feishuconnector-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feishuconnector
-Version: 0.1.5
+Version: 0.1.6
 Summary: connect feishu content franchise
 Home-page: http://www.puyuan.tech
 Author: Changhao Jiang
 Author-email: jch@puyuan.tech
 License: MIT License
 Platform: all
 Classifier: Development Status :: 4 - Beta
```

### Comparing `feishuconnector-0.1.5/README.rst` & `feishuconnector-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `feishuconnector-0.1.5/feishuconnector/manager.py` & `feishuconnector-0.1.6/feishuconnector/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,20 +57,22 @@
             assert False, f'fail to get a correct node detail {d}'
         has_more = True
         total_num = None
         page_token = None
         records = []
         try_num = 0
         while has_more:
+            if (page_token is None) and (try_num > 0):
+                raise Exception('page_token is None while has more records to fetch.')
             d = self._get_bitable_records(app_token, table_id, page_token=page_token)
             try_num += 1
             has_more = d['has_more']
             records.extend(d['items'])
             total_num = d['total']
-            page_token = d['page_token']
+            page_token = d.get('page_token', None)
         item_num = len(records)
         self.log(f'records from {node_token} table {table_id} with {try_num} requests. ApiTotal={total_num}, RecordNum={item_num}')
         return records
 
     def insert_bitable_records(self, node_token, table_id, records):
         # to depreciated...
         self.log('insert_bitable_records will be replaced by append_bitable_records')
@@ -244,15 +246,15 @@
         }
         r = requests.get(f'https://open.feishu.cn/open-apis/bitable/v1/apps/{app_token}/tables/{table_id}/records', params=params, headers=headers)
         d = json.loads(r.text)
         assert d.get('code') == 0, f'fail to get_bitable_records={r.text}'
         data = d['data']
         sz = len(data['items'])
         total_num = data['total']
-        page_token = data['page_token']
+        page_token = data.get('page_token', None)
         self.log(f'bitable records fetched. (table_id){table_id} (num){sz} (page_t){page_token} (total){total_num}')
         return data
 
     def _append_bitable_record(self, app_token, table_id, records):
         headers = {
             'Authorization': f'Bearer {self.token}',
             'Content-Type': 'application/json; charset=utf-8'
```

### Comparing `feishuconnector-0.1.5/feishuconnector.egg-info/PKG-INFO` & `feishuconnector-0.1.6/feishuconnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feishuconnector
-Version: 0.1.5
+Version: 0.1.6
 Summary: connect feishu content franchise
 Home-page: http://www.puyuan.tech
 Author: Changhao Jiang
 Author-email: jch@puyuan.tech
 License: MIT License
 Platform: all
 Classifier: Development Status :: 4 - Beta
```

### Comparing `feishuconnector-0.1.5/setup.py` & `feishuconnector-0.1.6/setup.py`

 * *Files identical despite different names*

