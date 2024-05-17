# Comparing `tmp/oda_api-1.2.8.tar.gz` & `tmp/oda_api-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oda_api-1.2.8.tar", last modified: Mon Jan 29 22:54:11 2024, max compression
+gzip compressed data, was "oda_api-1.2.9.tar", last modified: Wed Feb  7 08:49:28 2024, max compression
```

## Comparing `oda_api-1.2.8.tar` & `oda_api-1.2.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:54:11.006027 oda_api-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-01-29 22:54:02.000000 oda_api-1.2.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-29 22:54:02.000000 oda_api-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-29 22:54:11.006027 oda_api-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-01-29 22:54:02.000000 oda_api-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:54:11.002027 oda_api-1.2.8/oda_api/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52150 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9070 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/custom_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/data_products.py
--rw-r--r--   0 runner    (1001) docker     (127)    44772 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/gallery_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/misc_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    15547 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/ontology_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-29 22:54:05.000000 oda_api-1.2.8/oda_api/pkg_info.json
--rw-r--r--   0 runner    (1001) docker     (127)    47167 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/plot_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-01-29 22:54:02.000000 oda_api-1.2.8/oda_api/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:54:11.006027 oda_api-1.2.8/oda_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-01-29 22:54:10.000000 oda_api-1.2.8/oda_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-01-29 22:54:10.000000 oda_api-1.2.8/oda_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 22:54:10.000000 oda_api-1.2.8/oda_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-29 22:54:10.000000 oda_api-1.2.8/oda_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-01-29 22:54:10.000000 oda_api-1.2.8/oda_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-29 22:54:10.000000 oda_api-1.2.8/oda_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-29 22:54:02.000000 oda_api-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-29 22:54:11.006027 oda_api-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-01-29 22:54:02.000000 oda_api-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 22:54:11.006027 oda_api-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_data_products.py
--rw-r--r--   0 runner    (1001) docker     (127)    42459 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_drupal.py
--rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_live.py
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_plot_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_progress_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-01-29 22:54:02.000000 oda_api-1.2.8/tests/test_sites.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:28.311293 oda_api-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-02-07 08:49:16.000000 oda_api-1.2.9/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-07 08:49:16.000000 oda_api-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-07 08:49:28.311293 oda_api-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-07 08:49:16.000000 oda_api-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:28.307294 oda_api-1.2.9/oda_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52150 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9324 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/custom_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/data_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44772 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/gallery_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/misc_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15547 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/ontology_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-07 08:49:23.000000 oda_api-1.2.9/oda_api/pkg_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47167 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/plot_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-02-07 08:49:16.000000 oda_api-1.2.9/oda_api/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:28.307294 oda_api-1.2.9/oda_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-02-07 08:49:28.000000 oda_api-1.2.9/oda_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-07 08:49:28.000000 oda_api-1.2.9/oda_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 08:49:28.000000 oda_api-1.2.9/oda_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-07 08:49:28.000000 oda_api-1.2.9/oda_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-07 08:49:28.000000 oda_api-1.2.9/oda_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-07 08:49:28.000000 oda_api-1.2.9/oda_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-07 08:49:16.000000 oda_api-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-07 08:49:28.311293 oda_api-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-02-07 08:49:16.000000 oda_api-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 08:49:28.307294 oda_api-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7304 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_data_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42459 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_drupal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_plot_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-07 08:49:16.000000 oda_api-1.2.9/tests/test_sites.py
```

### Comparing `oda_api-1.2.8/LICENSE.rst` & `oda_api-1.2.9/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/PKG-INFO` & `oda_api-1.2.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oda_api
-Version: 1.2.8
+Version: 1.2.9
 Summary: API plugin  for CDCI online data analysis
 Author: Andrea Tramacere, Volodymyr Savchenko
 Author-email: contact@odahub.io
 Requires-Python: >=2.7
 License-File: LICENSE.rst
 Requires-Dist: requests
 Requires-Dist: future
```

### Comparing `oda_api-1.2.8/README.md` & `oda_api-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/__init__.py` & `oda_api-1.2.9/oda_api/__init__.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/api.py` & `oda_api-1.2.9/oda_api/api.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/cli.py` & `oda_api-1.2.9/oda_api/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,18 +183,22 @@
                 sort_keys=True,
             )
 
     # if validate:
     if not group_by_job:
         for record in sorted(state['records'], key=lambda r:r['mtime']):
             logger.info(f"session_id: {record['session_id']}, job_id: {record['job_id']} - {datetime.fromtimestamp(record['mtime'])}")
-            for email in record.get('analysis_parameters', {}).get('email_history', []):
-                logger.info(f"    - {email}")
-            for matrix_message in record.get('analysis_parameters', {}).get('matrix_message_history', []):
-                logger.info(f"    - {matrix_message}")
+            record_analysis_parameters = record.get('analysis_parameters', None)
+            if record_analysis_parameters is not None and isinstance(record_analysis_parameters, dict):
+                for email in record_analysis_parameters.get('email_history', []):
+                    logger.info(f"    - {email}")
+                for matrix_message in record_analysis_parameters.get('matrix_message_history', []):
+                    logger.info(f"    - {matrix_message}")
+            else:
+                logger.debug(record_analysis_parameters)
             request_completed = record['request_completed']
             token_expired = record.get('token_expired', None)
             if not request_completed:
                 msg = '\tRequest did not complete'
                 if token_expired:
                     msg += ' because the token was expired'
             else:
```

### Comparing `oda_api-1.2.8/oda_api/custom_formatters.py` & `oda_api-1.2.9/oda_api/custom_formatters.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/data_products.py` & `oda_api-1.2.9/oda_api/data_products.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/gallery_api.py` & `oda_api-1.2.9/oda_api/gallery_api.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/json.py` & `oda_api-1.2.9/oda_api/json.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/misc_helpers.py` & `oda_api-1.2.9/oda_api/misc_helpers.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/ontology_helper.py` & `oda_api-1.2.9/oda_api/ontology_helper.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/plot_tools.py` & `oda_api-1.2.9/oda_api/plot_tools.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api/token.py` & `oda_api-1.2.9/oda_api/token.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/oda_api.egg-info/PKG-INFO` & `oda_api-1.2.9/oda_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oda_api
-Version: 1.2.8
+Version: 1.2.9
 Summary: API plugin  for CDCI online data analysis
 Author: Andrea Tramacere, Volodymyr Savchenko
 Author-email: contact@odahub.io
 Requires-Python: >=2.7
 License-File: LICENSE.rst
 Requires-Dist: requests
 Requires-Dist: future
```

### Comparing `oda_api-1.2.8/oda_api.egg-info/SOURCES.txt` & `oda_api-1.2.9/oda_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/setup.cfg` & `oda_api-1.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.8
+current_version = 1.2.9
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `oda_api-1.2.8/setup.py` & `oda_api-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_basic.py` & `oda_api-1.2.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_cli.py` & `oda_api-1.2.9/tests/test_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import re
 from typing import ChainMap
 from click.testing import CliRunner
 import pytest
 import os
 import jwt
 import time
+import glob
 
 from oda_api import cli
 from cdci_data_analysis.pytest_fixtures import DispatcherJobState
-# from tests.test_basic import default_token_payload, secret_key
+from conftest import remove_scratch_folders
 
 secret_key = 'secretkey_test'
 default_exp_time = int(time.time()) + 5000
 default_token_payload = dict(
     sub="mtm@mtmco.net",
     name="mmeharga",
     roles="general",
@@ -39,14 +40,22 @@
     runner = CliRunner()
     args = ['-u', dispatcher_live_fixture, 'inspect']
     if group_by_job:
         args.append('--group-by-job')
     result = runner.invoke(cli.cli, args=args, obj={})
     assert result.exit_code == 0
 
+    # check there is no crash in case the analysis_parameters.json fil e was not found
+    list_scratch_dir = glob.glob(f'scratch_sid_*_jid_*')
+    os.remove(os.path.join(list_scratch_dir[0], "analysis_parameters.json"))
+
+    runner = CliRunner()
+    args = ['-u', dispatcher_live_fixture, 'inspect']
+    result = runner.invoke(cli.cli, args=args, obj={})
+    assert result.exit_code == 0
 
 @pytest.mark.parametrize('token_placement', ['no', 'env', 'homedotfile', 'cwddotfile'])
 def test_token_inspect(token_placement, default_token, monkeypatch, caplog, tmpdir):
     # this to make sure the level is sufficient to capture the DEBUG logs
     logging.getLogger('oda_api').setLevel("DEBUG")
     # reset any existing token locations    
     os.makedirs(tmpdir, exist_ok=True)
```

### Comparing `oda_api-1.2.8/tests/test_data_products.py` & `oda_api-1.2.9/tests/test_data_products.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_drupal.py` & `oda_api-1.2.9/tests/test_drupal.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_live.py` & `oda_api-1.2.9/tests/test_live.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_ontology.py` & `oda_api-1.2.9/tests/test_ontology.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_plot_tools.py` & `oda_api-1.2.9/tests/test_plot_tools.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_progress_report.py` & `oda_api-1.2.9/tests/test_progress_report.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_remote.py` & `oda_api-1.2.9/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `oda_api-1.2.8/tests/test_sites.py` & `oda_api-1.2.9/tests/test_sites.py`

 * *Files identical despite different names*

