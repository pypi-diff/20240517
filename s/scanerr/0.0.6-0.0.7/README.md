# Comparing `tmp/scanerr-0.0.6.tar.gz` & `tmp/scanerr-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanerr-0.0.6.tar", last modified: Wed Mar 20 22:40:30 2024, max compression
+gzip compressed data, was "scanerr-0.0.7.tar", last modified: Fri May 17 17:59:10 2024, max compression
```

## Comparing `scanerr-0.0.6.tar` & `scanerr-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-03-20 22:40:30.332649 scanerr-0.0.6/
--rw-r--r--   0 landon     (501) staff       (20)     1073 2024-02-27 21:49:18.000000 scanerr-0.0.6/LICENSE.md
--rw-r--r--   0 landon     (501) staff       (20)     1200 2024-03-20 22:40:30.332450 scanerr-0.0.6/PKG-INFO
--rw-r--r--   0 landon     (501) staff       (20)      520 2024-03-06 16:39:37.000000 scanerr-0.0.6/README.md
--rw-r--r--   0 landon     (501) staff       (20)      732 2024-03-20 22:40:23.000000 scanerr-0.0.6/pyproject.toml
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-03-20 22:40:30.332256 scanerr-0.0.6/scanerr.egg-info/
--rw-r--r--   0 landon     (501) staff       (20)     1200 2024-03-20 22:40:30.000000 scanerr-0.0.6/scanerr.egg-info/PKG-INFO
--rw-r--r--   0 landon     (501) staff       (20)      311 2024-03-20 22:40:30.000000 scanerr-0.0.6/scanerr.egg-info/SOURCES.txt
--rw-r--r--   0 landon     (501) staff       (20)        1 2024-03-20 22:40:30.000000 scanerr-0.0.6/scanerr.egg-info/dependency_links.txt
--rw-r--r--   0 landon     (501) staff       (20)       50 2024-03-20 22:40:30.000000 scanerr-0.0.6/scanerr.egg-info/entry_points.txt
--rw-r--r--   0 landon     (501) staff       (20)       34 2024-03-20 22:40:30.000000 scanerr-0.0.6/scanerr.egg-info/requires.txt
--rw-r--r--   0 landon     (501) staff       (20)        4 2024-03-20 22:40:30.000000 scanerr-0.0.6/scanerr.egg-info/top_level.txt
--rw-r--r--   0 landon     (501) staff       (20)       38 2024-03-20 22:40:30.332686 scanerr-0.0.6/setup.cfg
--rw-r--r--   0 landon     (501) staff       (20)      342 2024-03-20 22:40:23.000000 scanerr-0.0.6/setup.py
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-03-20 22:40:30.331551 scanerr-0.0.6/src/
--rw-r--r--   0 landon     (501) staff       (20)        0 2024-02-27 23:04:31.000000 scanerr-0.0.6/src/__init__.py
-drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-03-20 22:40:30.331854 scanerr-0.0.6/src/scanerr/
--rw-r--r--   0 landon     (501) staff       (20)        0 2024-02-27 21:48:01.000000 scanerr-0.0.6/src/scanerr/__init__.py
--rw-r--r--   0 landon     (501) staff       (20)    15565 2024-03-20 22:39:04.000000 scanerr-0.0.6/src/scanerr/api.py
--rw-r--r--   0 landon     (501) staff       (20)     8753 2024-03-19 19:38:03.000000 scanerr-0.0.6/src/scanerr/root.py
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-05-17 17:59:10.963991 scanerr-0.0.7/
+-rw-r--r--   0 landon     (501) staff       (20)     1073 2024-02-27 21:49:18.000000 scanerr-0.0.7/LICENSE.md
+-rw-r--r--   0 landon     (501) staff       (20)     1200 2024-05-17 17:59:10.963508 scanerr-0.0.7/PKG-INFO
+-rw-r--r--   0 landon     (501) staff       (20)      520 2024-03-06 16:39:37.000000 scanerr-0.0.7/README.md
+-rw-r--r--   0 landon     (501) staff       (20)      732 2024-05-17 15:19:55.000000 scanerr-0.0.7/pyproject.toml
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-05-17 17:59:10.962969 scanerr-0.0.7/scanerr.egg-info/
+-rw-r--r--   0 landon     (501) staff       (20)     1200 2024-05-17 17:59:10.000000 scanerr-0.0.7/scanerr.egg-info/PKG-INFO
+-rw-r--r--   0 landon     (501) staff       (20)      311 2024-05-17 17:59:10.000000 scanerr-0.0.7/scanerr.egg-info/SOURCES.txt
+-rw-r--r--   0 landon     (501) staff       (20)        1 2024-05-17 17:59:10.000000 scanerr-0.0.7/scanerr.egg-info/dependency_links.txt
+-rw-r--r--   0 landon     (501) staff       (20)       50 2024-05-17 17:59:10.000000 scanerr-0.0.7/scanerr.egg-info/entry_points.txt
+-rw-r--r--   0 landon     (501) staff       (20)       34 2024-05-17 17:59:10.000000 scanerr-0.0.7/scanerr.egg-info/requires.txt
+-rw-r--r--   0 landon     (501) staff       (20)        4 2024-05-17 17:59:10.000000 scanerr-0.0.7/scanerr.egg-info/top_level.txt
+-rw-r--r--   0 landon     (501) staff       (20)       38 2024-05-17 17:59:10.964121 scanerr-0.0.7/setup.cfg
+-rw-r--r--   0 landon     (501) staff       (20)      342 2024-05-17 15:20:39.000000 scanerr-0.0.7/setup.py
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-05-17 17:59:10.962078 scanerr-0.0.7/src/
+-rw-r--r--   0 landon     (501) staff       (20)        0 2024-02-27 23:04:31.000000 scanerr-0.0.7/src/__init__.py
+drwxr-xr-x   0 landon     (501) staff       (20)        0 2024-05-17 17:59:10.962444 scanerr-0.0.7/src/scanerr/
+-rw-r--r--   0 landon     (501) staff       (20)        0 2024-02-27 21:48:01.000000 scanerr-0.0.7/src/scanerr/__init__.py
+-rw-r--r--   0 landon     (501) staff       (20)    21518 2024-05-17 17:56:10.000000 scanerr-0.0.7/src/scanerr/api.py
+-rw-r--r--   0 landon     (501) staff       (20)     9395 2024-05-17 17:36:57.000000 scanerr-0.0.7/src/scanerr/root.py
```

### Comparing `scanerr-0.0.6/LICENSE.md` & `scanerr-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scanerr-0.0.6/PKG-INFO` & `scanerr-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanerr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Official Scanerr CLI
 Author-email: Scanerr <hello@scanerr.io>
 Project-URL: Homepage, https://github.com/scanerr-io/cli
 Project-URL: Issues, https://github.com/scanerr-io/cli/issues
 Project-URL: Documentaion, https://docs.scanerr.io
 Keywords: regression testing,vrt,visual regression testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scanerr-0.0.6/README.md` & `scanerr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `scanerr-0.0.6/pyproject.toml` & `scanerr-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scanerr"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Scanerr", email="hello@scanerr.io" },
 ]
 description = "Official Scanerr CLI"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["regression testing", "vrt", "visual regression testing"]
```

### Comparing `scanerr-0.0.6/scanerr.egg-info/PKG-INFO` & `scanerr-0.0.7/scanerr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanerr
-Version: 0.0.6
+Version: 0.0.7
 Summary: Official Scanerr CLI
 Author-email: Scanerr <hello@scanerr.io>
 Project-URL: Homepage, https://github.com/scanerr-io/cli
 Project-URL: Issues, https://github.com/scanerr-io/cli/issues
 Project-URL: Documentaion, https://docs.scanerr.io
 Keywords: regression testing,vrt,visual regression testing
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scanerr-0.0.6/src/scanerr/api.py` & `scanerr-0.0.7/src/scanerr/api.py`

 * *Files 24% similar despite different names*

```diff
@@ -202,14 +202,15 @@
     resp = format_response(res)
 
     # return object as dict
     return resp
 
 
 
+
 def api_add_page(*args, **kwargs):
 
     """
     This endpoint will create a new `Page` 
     object associated with the passed "site_id". 
     Also creates an initial `Scan` object for each new `Page`
     """
@@ -471,14 +472,15 @@
     resp = format_response(res)
 
     # return object as dict
     return resp
 
 
 
+
 def api_get_tests(*args, **kwargs):
 
     """
     This Endpoint will retrieve one or more `Tests` for 
     only the passed "page_id" - recommend using "lean=true"
     """
 
@@ -511,14 +513,141 @@
 
     # return object as dict
     return resp
 
 
 
 
+def api_get_cases(*args, **kwargs):
+
+    """
+    This Endpoint will retrieve one or more `Cases` for 
+    only the passed "site_id"
+    """
+
+    # get kwargs
+    site_id = kwargs.get('site_id')
+    case_id = kwargs.get('case_id')
+    api_key = kwargs.get('api_key')
+
+    # setup configs
+    url = f'{SCANERR_API_BASE_URL}/case'
+
+    params = {
+        'case_id': case_id, 
+        'site_id': site_id,
+    }
+
+    # check headers for API KEY
+    headers = check_headers(api_key=api_key)
+
+    # send the request
+    res = requests.get(
+        url=url, 
+        headers=headers, 
+        params=params
+    )
+
+    # format response
+    resp = format_response(res)
+
+    # get steps data from resp
+    if resp['success']:
+        steps_data = requests.get(
+            url=resp['data']['steps']['url'],
+            headers=headers
+        ).json()
+
+        # update resp with new data
+        resp['data']['steps']['steps'] = steps_data
+
+    # return object as dict
+    return resp
+
+
+
+
+def api_get_testcases(*args, **kwargs):
+
+    """
+    This Endpoint will retrieve one or more `Testcases` for 
+    only the passed "site_id"
+    """
+
+    # get kwargs
+    site_id = kwargs.get('site_id')
+    testcase_id = kwargs.get('testcase_id')
+    api_key = kwargs.get('api_key')
+
+    # setup configs
+    url = f'{SCANERR_API_BASE_URL}/testcase'
+
+    params = {
+        'testcase_id': testcase_id,
+        'site_id': site_id,
+    }
+
+    # check headers for API KEY
+    headers = check_headers(api_key=api_key)
+
+    # send the request
+    res = requests.get(
+        url=url, 
+        headers=headers, 
+        params=params
+    )
+
+    # format response
+    resp = format_response(res)
+
+    # return object as dict
+    return resp
+
+
+
+
+def api_add_testcases(*args, **kwargs):
+
+    """
+    This Endpoint will create and run a new `Testcases` 
+    for the passed "site_id" & "case_id"
+    """
+
+    # get kwargs
+    site_id = kwargs.get('site_id')
+    case_id = kwargs.get('case_id')
+    updates = kwargs.get('updates')
+    api_key = kwargs.get('api_key')
+
+    # setup configs
+    url = f'{SCANERR_API_BASE_URL}/testcase/delay'
+
+    data = {
+        'case_id': case_id,
+        'site_id': site_id,
+        'updates': updates
+    }
+
+    # check headers for API KEY
+    headers = check_headers(api_key=api_key)
+
+    # send the request
+    res = requests.post(
+        url=url, 
+        headers=headers,
+        data=json.dumps(data)
+    )
+
+    # format response
+    resp = format_response(res)
+
+    # return object as dict
+    return resp
+
+
 
 def wait_for_completion(ids: list, obj: str) -> None:
 
     """ 
     This method waits for either a set of `Scan` or `Test` objects
     finish running - or timesout at max_wait_time (900s)
     """
@@ -532,14 +661,16 @@
         wait_time += 15
         # checking status of obj
         for id in ids:
             if obj == 'scan':
                 time_complete = api_get_scans(scan_id=id, page_id=None)['data']['time_completed']
             if obj == 'test':
                 time_complete = api_get_tests(test_id=id, page_id=None)['data']['time_completed']
+            if obj == 'testcase':
+                time_complete = api_get_testcases(testcase_id=id)['data']['time_completed']
             
             # alerting completion
             if time_complete is not None and id not in completions:
                 rprint('[green bold]' + u'\u2714' + '[/green bold]' + f' {obj} completed -> {id}')
                 completions.append(id)
 
     return None
@@ -665,13 +796,131 @@
 
     # returning results
     return success
 
 
 
 
+def api_testcase(
+        site_id: str,
+        case_id: str,
+        max_wait_time: int=120,
+        api_key: str=None,
+        updates: dict=None,
+    ):
+    
+    """ 
+    This method will run a full `Testcase` for the `Site`
+    asocaited with the passed id's. 
+    Full flow:
+        1. Determine if testing full site or page
+        2. Wait for `Site` to be available
+        3. Adjust steps data (from **kwargs)
+        4. Initiate the `Testcase`
+        5. Check for `Testcase` completion
+    """
+
+    # 1. get the site
+    site = api_get_sites(site_id=site_id, api_key=api_key)['data']
+
+    # 2. Wait for `Site` to be available
+    wait_time = 0
+    site_status = 500
+    print(f'checking site availablity...')
+    while str(site_status).startswith('5') and wait_time < max_wait_time:
+        # sleeping for 5 seconds
+        time.sleep(5)
+        wait_time += 5
+        # check site status
+        site_status = requests.get(url=site['site_url']).status_code
+    
+    # determine if timeout 
+    if wait_time >= max_wait_time:
+        rprint(
+            '[red bold]' + u'\u2718' + '[/red bold]' + 
+            ' max wait time reached - proceeding with caution...'
+        )
+    else:
+        rprint(
+            '[green bold]' + u'\u2714' + '[/green bold]' 
+            + ' site is available'
+        )
+
+    # 3. Adjust steps data (from **kwargs)
+    print(f'\nadjusting step data...')
+    _updates = []
+    for i in updates:
+        if '-' not in i or ':' not in i:
+            rprint(
+                '[red bold]' + u'\u2718' + '[/red bold]' + 
+                ' step data formatted incorrectly (step-0:value)'
+            )
+            return
+
+        # parsing data from step
+        _str = str(i).split(':')
+        value = _str[1]
+        index = int(_str[0].split('-')[1])-1
+
+        # adding data to updates
+        _updates.append({
+            'index': index,
+            'value': value
+        })
+
+    # done parsing and updating
+    rprint('[green bold]' + u'\u2714' + '[/green bold]' + f' step data updated')
+
+    # 4. Create new `Testcase`
+    testcase_data = api_add_testcases(
+        case_id=case_id,
+        site_id=site_id,
+        updates=_updates
+    )
+
+    if not testcase_data['success']:
+        rprint(testcase_data)
+        return False
+    
+    # saving testcase_id
+    testcase_id = testcase_data['data']['id']
+
+    # 5. Check for `Testcase` completion
+    print(f'\nwaiting for Testcase completion...')
+    wait_for_completion(ids=[testcase_id], obj='testcase')
+    testcase = api_get_testcases(testcase_id=testcase_id, api_key=api_key)['data']
+    passed = testcase['passed']
+
+    failed = []
+    i = 1
+    # getting failed steps;
+    for step in testcase['steps']:
+        if not step['action']['passed']:
+            failed.append(f'Step #{i}')
+        i += 1
+
+    # displaying results
+    print('\nTestcase results:')
+    if passed:
+        rprint(
+            '[green bold]' + u'\u2714' + '[/green bold]' + 
+            f' Passed : https://app.scanerr.io/testcase/{testcase_id}' 
+        )
+    else:
+        rprint(
+            f'{"\n[red bold]" + u"\u2718" + "[/red bold]"}' + 
+            f' Failed : https://app.scanerr.io/testcase/{testcase_id}' + 
+            f'\n failed steps : {[n for n in failed]}'
+        )
+
+    # returning results
+    return passed
+
+
+
+
```

### Comparing `scanerr-0.0.6/src/scanerr/root.py` & `scanerr-0.0.7/src/scanerr/root.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import typer, os, json, time, shutil
 from pathlib import Path
+from typing import List
 from dotenv import load_dotenv
 from pprint import pprint
 from rich import print as rprint
 from .api import *
 
 
 # High Level Configs
@@ -460,10 +461,42 @@
 
     if not resp:
         raise Exception('- Scanerr Tests Failed -')
 
 
 
 
+@app.command(
+    context_settings={
+        "allow_extra_args": True, 
+        "ignore_unknown_options": True
+    }
+)
+def testcase(
+        site_id: str,
+        case_id: str, 
+        max_wait_time :int=120,
+        api_key: str=None,
+        updates: typer.Context=None
+    ):
+
+    """ 
+    Run a full `Testcase` of a specific `Site`
+    """
+
+    # sending request
+    resp = api_testcase(
+        site_id=site_id, 
+        case_id=case_id, 
+        max_wait_time=max_wait_time,
+        api_key=api_key,
+        updates=updates.args
+    )
+
+    if not resp:
+        raise Exception('- Scanerr Testcase Failed -')
+
+
+
 ## --- CLI entry point --- ##
 def root():
     app()
```

