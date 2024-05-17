# Comparing `tmp/metabase_query_api-1.1.0-py3-none-any.whl.zip` & `tmp/metabase_query_api-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 15391 bytes, number of entries: 13
--rw-r--r--  2.0 unx       15 b- defN 23-Oct-08 10:19 metabase_query_api/__init__.py
+Zip file size: 15699 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       99 b- defN 24-May-17 04:42 metabase_query_api/__init__.py
 -rw-r--r--  2.0 unx     2519 b- defN 23-Nov-09 05:29 metabase_query_api/async_card.py
 -rw-r--r--  2.0 unx     2395 b- defN 23-Nov-09 05:29 metabase_query_api/async_dataset.py
--rw-r--r--  2.0 unx     6955 b- defN 24-Jan-11 07:30 metabase_query_api/async_query.py
+-rw-r--r--  2.0 unx     7645 b- defN 24-May-17 05:41 metabase_query_api/async_query.py
 -rw-r--r--  2.0 unx     1203 b- defN 23-Nov-27 08:57 metabase_query_api/retry_errors.py
 -rw-r--r--  2.0 unx     7347 b- defN 23-Nov-09 05:29 metabase_query_api/sync_card.py
 -rw-r--r--  2.0 unx     6224 b- defN 23-Nov-09 05:29 metabase_query_api/sync_dataset.py
 -rw-r--r--  2.0 unx     3241 b- defN 23-Nov-09 05:29 metabase_query_api/sync_query.py
--rw-r--r--  2.0 unx     1076 b- defN 24-Jan-11 07:39 metabase_query_api-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     5482 b- defN 24-Jan-11 07:39 metabase_query_api-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-11 07:39 metabase_query_api-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Jan-11 07:39 metabase_query_api-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1156 b- defN 24-Jan-11 07:39 metabase_query_api-1.1.0.dist-info/RECORD
-13 files, 37724 bytes uncompressed, 13431 bytes compressed:  64.4%
+-rw-r--r--  2.0 unx     1076 b- defN 24-May-17 05:59 metabase_query_api-1.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-17 05:59 metabase_query_api-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 05:59 metabase_query_api-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-17 05:59 metabase_query_api-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1156 b- defN 24-May-17 05:59 metabase_query_api-1.1.1.dist-info/RECORD
+13 files, 38525 bytes uncompressed, 13739 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: metabase_query_api/sync_dataset.py
 Comment: 
 
 Filename: metabase_query_api/sync_query.py
 Comment: 
 
-Filename: metabase_query_api-1.1.0.dist-info/LICENSE
+Filename: metabase_query_api-1.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: metabase_query_api-1.1.0.dist-info/METADATA
+Filename: metabase_query_api-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: metabase_query_api-1.1.0.dist-info/WHEEL
+Filename: metabase_query_api-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: metabase_query_api-1.1.0.dist-info/top_level.txt
+Filename: metabase_query_api-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: metabase_query_api-1.1.0.dist-info/RECORD
+Filename: metabase_query_api-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## metabase_query_api/__init__.py

```diff
@@ -1 +1,2 @@
-from . import *
+from .async_query import export_question_bulk_filter_values
+from .sync_query import export_question
```

## metabase_query_api/async_query.py

```diff
@@ -108,14 +108,18 @@
                                            verbose=verbose,
                                            timeout=timeout,
                                            custom_retry_errors=custom_retry_errors)
 
         # Get data
         query_records = await get_query_data()
 
+        # Test error
+        if print_suffix == '(2/2)':
+            raise Exception('Test Error')
+
         # Raise error by user
         if 'error' in query_records:
             raise Exception(query_records['error'])
 
         # Sort columns
         if column_sort_order:
             query_records = [{col: item[col] for col in column_sort_order if col in item} for item in query_records]
@@ -140,11 +144,23 @@
         counter = 0
         for modified_dataset_query in modified_dataset_query_list:
             counter += 1
             tasks.append(asyncio.create_task(query_quest(payload=modified_dataset_query, print_suffix=f'({counter}/{total})', verbose=verbose)))
             await asyncio.sleep(1)
 
     # Combine tasks results
-    res = await asyncio.gather(*tasks)
+    res = await asyncio.gather(*tasks, return_exceptions=True) # return_exceptions to handle error and send user successful data
     await client_session.close()
 
-    return sum(res, [])
+    success_results = []
+    has_error = False
+    for idx, result in enumerate(res):
+        idx += 1
+        if isinstance(result, Exception):
+            print(f"Task ({idx}/{total}) error: {result}")
+            has_error = True
+        else:
+            success_results.append(result)
+    if has_error:
+        print('There were error parts. You will receive the successfully retrieved data. Please filter out the parts that have not been retrieved so that you can run them again.')
+
+    return sum(success_results, [])
```

## Comparing `metabase_query_api-1.1.0.dist-info/LICENSE` & `metabase_query_api-1.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `metabase_query_api-1.1.0.dist-info/METADATA` & `metabase_query_api-1.1.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabase-query-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: Metabase Query API with Retry and Bulk Param Values
 Home-page: https://github.com/tranngocminhhieu/metabase-query-api
 Author: Tran Ngoc Minh Hieu
 Author-email: tnmhieu@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
@@ -13,14 +13,16 @@
 
 # Metabase Query API
 [![Downloads](https://img.shields.io/pypi/dm/metabase-query-api)](https://pypi.org/project/metabase-query-api)
 [![Pypi](https://img.shields.io/pypi/v/metabase-query-api)](https://pypi.org/project/metabase-query-api)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](https://github.com/tranngocminhhieu/metabase-query-api/issues)
 [![MIT](https://img.shields.io/github/license/tranngocminhhieu/metabase-query-api)](https://github.com/tranngocminhhieu/metabase-query-api/blob/main/LICENSE)
 
+![example-table.png](images%2Fexample-table.png)
+
 This package will help Data workers get data from [Metabase](https://www.metabase.com/) questions more easily and effectively. It only focuses on the [Card Query API](https://www.metabase.com/docs/latest/api/card#post-apicardcard-idqueryexport-format), [Dataset API](https://www.metabase.com/docs/latest/api/dataset#post-apidatasetexport-format) and does not include other Metabase APIs.
 
 ## Features
 1. Get question data in any data format provided by Metabase (JSON, CSV, XLSX).
 2. Input question URL and Metabase Session. No need to provide parameters payload.
 3. JSON results have the same column sort order as the browser.
 4. Automatically check if Metabase session is available.
@@ -33,16 +35,16 @@
 pip install metabase-query-api
 ```
 
 
 ## Instruction
 ### Import package
 ```python
-from metabase_query_api.sync_query import export_question
-from metabase_query_api.async_query import export_question_bulk_filter_values
+from metabase_query_api import export_question
+from metabase_query_api import export_question_bulk_filter_values
 import asyncio
 ```
 
 ### Get question data
 - Copy the question URL in the browser. Note that you must fill in the necessary parameters before copying.
 - Use a different API to get the [Metabase Session](https://www.metabase.com/docs/latest/api/session#post-apisession). Or you can use this [Chrome extension](https://chrome.google.com/webstore/detail/cookie-tab-viewer/fdlghnedhhdgjjfgdpgpaaiddipafhgk) to get it.
```

## Comparing `metabase_query_api-1.1.0.dist-info/RECORD` & `metabase_query_api-1.1.1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-metabase_query_api/__init__.py,sha256=ovguP4wzQEDNguczwiZnhMm4dRRVcvnzmHrfQtlRCNQ,15
+metabase_query_api/__init__.py,sha256=btMlUoInXZnprUgJAmm-xsp_0Y7_MHRnxZMqh-rz2pM,99
 metabase_query_api/async_card.py,sha256=HzJymPYV21L6ba6FWLqqg3TBF6uv1XnRLgyEXdB8MVk,2519
 metabase_query_api/async_dataset.py,sha256=peMzKoa9qrl4-Irieg4CSYrg-P9AFyRR9NBfx4wZECc,2395
-metabase_query_api/async_query.py,sha256=CHiuiWCL0zxVwsh1rTvwq5_xiD2_bNYwH5OBjSr0WwA,6955
+metabase_query_api/async_query.py,sha256=8xTuCAvtcnKaZETS3eokyecAinln7O2tJyxr-NEhXiU,7645
 metabase_query_api/retry_errors.py,sha256=KKra-Gp3O3wrlujSOo1jXtqwxRE6cWMGMytlx2JrXek,1203
 metabase_query_api/sync_card.py,sha256=Ll3Dyt_syKDc_QEz5hepiC9mETs_zNnbUNyCo4y_YpE,7347
 metabase_query_api/sync_dataset.py,sha256=ngrsKlXujFhWcjc-B34UH3kLN5f6J4MVSqNWrrDYS60,6224
 metabase_query_api/sync_query.py,sha256=uqwzzFqsinvpc24asAT4CWvpZlrpcclN1shfvZ5BAmM,3241
-metabase_query_api-1.1.0.dist-info/LICENSE,sha256=do2v2Zr9PKexWB6RWWOZVRJi73GgCDowDBwt6EZLnmg,1076
-metabase_query_api-1.1.0.dist-info/METADATA,sha256=brl9iGe_D2q7jk9-GhL9-DNnOU5eASD87DgqvvQq0Zo,5482
-metabase_query_api-1.1.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-metabase_query_api-1.1.0.dist-info/top_level.txt,sha256=qD1E4cNblF3wEGDsjTes6zA8gO5dMDE10jCoDCMpL2w,19
-metabase_query_api-1.1.0.dist-info/RECORD,,
+metabase_query_api-1.1.1.dist-info/LICENSE,sha256=do2v2Zr9PKexWB6RWWOZVRJi73GgCDowDBwt6EZLnmg,1076
+metabase_query_api-1.1.1.dist-info/METADATA,sha256=a4Aq5GsHDO2sikCWsyl9w425SjFp50HAR9HELqDcvdU,5509
+metabase_query_api-1.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+metabase_query_api-1.1.1.dist-info/top_level.txt,sha256=qD1E4cNblF3wEGDsjTes6zA8gO5dMDE10jCoDCMpL2w,19
+metabase_query_api-1.1.1.dist-info/RECORD,,
```

