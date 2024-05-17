# Comparing `tmp/cpg-utils-5.0.8.tar.gz` & `tmp/cpg-utils-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpg-utils-5.0.8.tar", last modified: Thu May  2 01:13:42 2024, max compression
+gzip compressed data, was "cpg-utils-5.0.9.tar", last modified: Mon May 13 00:39:31 2024, max compression
```

## Comparing `cpg-utils-5.0.8.tar` & `cpg-utils-5.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/cpg_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cloudpath_hail_az.py
--rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    27898 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/cromwell_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14008 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/dataproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/hail_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/membership.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/cpg_utils/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/cpg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 01:13:42.000000 cpg-utils-5.0.8/cpg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:42.618062 cpg-utils-5.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/test_cromwell.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-02 01:13:39.000000 cpg-utils-5.0.8/test/test_doctests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:39:31.052421 cpg-utils-5.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-13 00:39:31.052421 cpg-utils-5.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:39:31.048421 cpg-utils-5.0.9/cpg_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14297 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/cloudpath_hail_az.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27959 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13229 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/cromwell_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14031 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/dataproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/hail_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/cpg_utils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:39:31.052421 cpg-utils-5.0.9/cpg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-13 00:39:31.000000 cpg-utils-5.0.9/cpg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-13 00:39:31.000000 cpg-utils-5.0.9/cpg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:39:31.000000 cpg-utils-5.0.9/cpg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-13 00:39:31.000000 cpg-utils-5.0.9/cpg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 00:39:31.000000 cpg-utils-5.0.9/cpg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 00:39:31.052421 cpg-utils-5.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1348 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:39:31.052421 cpg-utils-5.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/test/test_cromwell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 00:39:30.000000 cpg-utils-5.0.9/test/test_doctests.py
```

### Comparing `cpg-utils-5.0.8/LICENSE` & `cpg-utils-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/PKG-INFO` & `cpg-utils-5.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.8
+Version: 5.0.9
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.8/README.md` & `cpg-utils-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/__init__.py` & `cpg-utils-5.0.9/cpg_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/cloud.py` & `cpg-utils-5.0.9/cpg_utils/cloud.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/cloudpath_hail_az.py` & `cpg-utils-5.0.9/cpg_utils/cloudpath_hail_az.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/config.py` & `cpg-utils-5.0.9/cpg_utils/config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/constants.py` & `cpg-utils-5.0.9/cpg_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/cromwell.py` & `cpg-utils-5.0.9/cpg_utils/cromwell.py`

 * *Files 0% similar despite different names*

```diff
@@ -569,14 +569,15 @@
     otherwise write the value into a file which will be a batch resource.
 
     :param driver_image: If specified, must contain python3 (w/ requests), gcloud, jq
     :param b: Batch object
     :param job_prefix: Prefix for the job name
     :param workflow_id_file: File containing the workflow ID
     :param outputs_to_collect: dict of output name -> CromwellOutputType
+    :param min_poll_interval: Min time to wait between polls
     :param max_poll_interval: Maximum time to wait between polls
     :param exponential_decrease_seconds: Exponential decrease in wait time
     :param max_sequential_exception_count: Maximum number of exceptions before giving up
     :param time_limit_seconds: a maximum runtime before abort is triggered
     """
 
     driver_image = driver_image or get_driver_image()
```

### Comparing `cpg-utils-5.0.8/cpg_utils/cromwell_model.py` & `cpg-utils-5.0.9/cpg_utils/cromwell_model.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/dataproc.py` & `cpg-utils-5.0.9/cpg_utils/dataproc.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
 
 
 def _add_submit_job(
     batch: hb.Batch,
     cluster_id: str,
     script: str,
     region: str,
-    hail_version: str,
+    hail_version: str = DEFAULT_HAIL_VERSION,
     pyfiles: list[str] | None = None,
     job_name: str | None = None,
     cluster_name: str | None = None,
     attributes: dict | None = None,
 ) -> hb.batch.job.Job:
     """
     Returns a job that submits a script to the Dataproc cluster
```

### Comparing `cpg-utils-5.0.8/cpg_utils/git.py` & `cpg-utils-5.0.9/cpg_utils/git.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/hail_batch.py` & `cpg-utils-5.0.9/cpg_utils/hail_batch.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/membership.py` & `cpg-utils-5.0.9/cpg_utils/membership.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils/slack.py` & `cpg-utils-5.0.9/cpg_utils/slack.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/cpg_utils.egg-info/PKG-INFO` & `cpg-utils-5.0.9/cpg_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpg-utils
-Version: 5.0.8
+Version: 5.0.9
 Summary: Library of convenience functions specific to the CPG
 Home-page: https://github.com/populationgenomics/cpg-utils
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cpg-utils-5.0.8/cpg_utils.egg-info/SOURCES.txt` & `cpg-utils-5.0.9/cpg_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/pyproject.toml` & `cpg-utils-5.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/setup.py` & `cpg-utils-5.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='cpg-utils',
     # This tag is automatically updated by bumpversion
-    version='5.0.8',
+    version='5.0.9',
     description='Library of convenience functions specific to the CPG',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/populationgenomics/cpg-utils',
     license='MIT',
     packages=find_packages(),
     package_data={
```

### Comparing `cpg-utils-5.0.8/test/test_config.py` & `cpg-utils-5.0.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cpg-utils-5.0.8/test/test_cromwell.py` & `cpg-utils-5.0.9/test/test_cromwell.py`

 * *Files identical despite different names*

