# Comparing `tmp/promptflow-1.8.0-py3-none-any.whl.zip` & `tmp/promptflow-1.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 17576 bytes, number of entries: 7
--rw-rw-r--  2.0 unx     2762 b- defN 24-Apr-10 09:42 promptflow/__init__.py
--rw-rw-r--  2.0 unx      199 b- defN 24-Apr-10 09:42 promptflow/_version.py
--rw-rw-r--  2.0 unx    20797 b- defN 24-Apr-10 09:42 promptflow-1.8.0.dist-info/METADATA
--rw-rw-r--  2.0 unx    34988 b- defN 24-Apr-10 09:42 promptflow-1.8.0.dist-info/NOTICE.txt
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-10 09:42 promptflow-1.8.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 24-Apr-10 09:42 promptflow-1.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      563 b- defN 24-Apr-10 09:42 promptflow-1.8.0.dist-info/RECORD
-7 files, 59412 bytes uncompressed, 16580 bytes compressed:  72.1%
+Zip file size: 18172 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     2762 b- defN 24-Apr-17 07:02 promptflow/__init__.py
+-rw-rw-r--  2.0 unx      199 b- defN 24-Apr-17 07:02 promptflow/_version.py
+-rwxrwxr-x  2.0 unx      168 b- defN 24-Apr-17 07:02 promptflow-1.9.0.data/scripts/pf.autocomplete.sh
+-rw-rw-r--  2.0 unx    21599 b- defN 24-Apr-17 07:02 promptflow-1.9.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx    34988 b- defN 24-Apr-17 07:02 promptflow-1.9.0.dist-info/NOTICE.txt
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-17 07:02 promptflow-1.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 24-Apr-17 07:02 promptflow-1.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      667 b- defN 24-Apr-17 07:02 promptflow-1.9.0.dist-info/RECORD
+8 files, 60486 bytes uncompressed, 17004 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: promptflow/__init__.py
 Comment: 
 
 Filename: promptflow/_version.py
 Comment: 
 
-Filename: promptflow-1.8.0.dist-info/METADATA
+Filename: promptflow-1.9.0.data/scripts/pf.autocomplete.sh
 Comment: 
 
-Filename: promptflow-1.8.0.dist-info/NOTICE.txt
+Filename: promptflow-1.9.0.dist-info/METADATA
 Comment: 
 
-Filename: promptflow-1.8.0.dist-info/WHEEL
+Filename: promptflow-1.9.0.dist-info/NOTICE.txt
 Comment: 
 
-Filename: promptflow-1.8.0.dist-info/top_level.txt
+Filename: promptflow-1.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: promptflow-1.8.0.dist-info/RECORD
+Filename: promptflow-1.9.0.dist-info/top_level.txt
+Comment: 
+
+Filename: promptflow-1.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## promptflow/_version.py

```diff
@@ -1,5 +1,5 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
-VERSION = "1.8.0"
+VERSION = "1.9.0"
```

## Comparing `promptflow-1.8.0.dist-info/METADATA` & `promptflow-1.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptflow
-Version: 1.8.0
+Version: 1.9.0
 Summary: Prompt flow Python SDK - build high-quality LLM apps
 Home-page: https://github.com/microsoft/promptflow
 Author: Microsoft Corporation
 Author-email: aml-pt-eng@microsoft.com
 License: MIT License
 Project-URL: Bug Reports, https://github.com/microsoft/promptflow/issues
 Project-URL: Source, https://github.com/microsoft/promptflow
@@ -16,29 +16,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: <4.0,>=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: promptflow-core (==1.8.0)
-Requires-Dist: promptflow-devkit (==1.8.0)
-Requires-Dist: promptflow-tracing (==1.8.0)
+Requires-Dist: promptflow-core (==1.9.0)
+Requires-Dist: promptflow-devkit (==1.9.0)
+Requires-Dist: promptflow-tracing (==1.9.0)
 Provides-Extra: all
-Requires-Dist: promptflow-azure (==1.8.0) ; extra == 'all'
-Requires-Dist: promptflow-core[executor-service] (==1.8.0) ; extra == 'all'
-Requires-Dist: promptflow-devkit[all] (==1.8.0) ; extra == 'all'
+Requires-Dist: promptflow-azure (==1.9.0) ; extra == 'all'
+Requires-Dist: promptflow-core[executor-service] (==1.9.0) ; extra == 'all'
+Requires-Dist: promptflow-devkit[all] (==1.9.0) ; extra == 'all'
 Provides-Extra: azure
-Requires-Dist: promptflow-azure (==1.8.0) ; extra == 'azure'
+Requires-Dist: promptflow-azure (==1.9.0) ; extra == 'azure'
 Provides-Extra: azureml-serving
-Requires-Dist: promptflow-core[azureml-serving] (==1.8.0) ; extra == 'azureml-serving'
+Requires-Dist: promptflow-core[azureml-serving] (==1.9.0) ; extra == 'azureml-serving'
 Provides-Extra: executable
-Requires-Dist: promptflow-devkit[executable] (==1.8.0) ; extra == 'executable'
+Requires-Dist: promptflow-devkit[executable] (==1.9.0) ; extra == 'executable'
 Provides-Extra: executor-service
-Requires-Dist: promptflow-core[executor-service] (==1.8.0) ; extra == 'executor-service'
+Requires-Dist: promptflow-core[executor-service] (==1.9.0) ; extra == 'executor-service'
 
 
 # Prompt flow
 
 [![Python package](https://img.shields.io/pypi/v/promptflow)](https://pypi.org/project/promptflow/)
 [![Python](https://img.shields.io/pypi/pyversions/promptflow.svg?maxAge=2592000)](https://pypi.python.org/pypi/promptflow/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/promptflow)](https://pypi.org/project/promptflow/)
@@ -118,15 +118,31 @@
 ```
 
 #### Continue to delve deeper into [prompt flow](https://github.com/microsoft/promptflow).
 
 
 # Release History
 
-## 1.8.0 (2024.04.03)
+## 1.9.0 (2024.04.17)
+
+### Features Added
+- [promptflow-devkit]: Added autocomplete feature for linux, reach [here](https://microsoft.github.io/promptflow/reference/pf-command-reference.html#autocomplete) for more details.
+- [promptflow-devkit]: Support trace experience in flow test and batch run. See [here](https://microsoft.github.io/promptflow/how-to-guides/tracing/index.html) for more details.
+
+### Bugs Fixed
+- [promptflow-devkit] Fix run name missing directory name in some scenario of `pf.run`.
+- [promptflow-devkit] Raise not supported instead of 404 when trying to create Azure AI connection.
+
+### Others
+- [promptflow-core] Connection default api version changed:
+  - AzureOpenAIConnection: 2023-07-01-preview -> 2024-02-01
+  - CognitiveSearchConnection: 2023-07-01-preview -> 2023-11-01
+
+
+## 1.8.0 (2024.04.10)
 
 ### NOTICES
 - `promptflow` package has been split into multiple packages. When installing `promptflow`, you will get the following packages:
   - `promptflow`:
     - `promptflow-tracing`: Tracing capability for promptflow.
     - `promptflow-core`: Core functionality to run flow.
     - `promptflow-devkit`: Development kit for promptflow.
@@ -136,15 +152,14 @@
 - [SDK/CLI] Create a run with `resume_from`, note that only run created with `promptflow>=1.8.0` can be used as the value of `resume_from`:
   - CLI: Support `pf run create --resume-from <original-run-name>` to create a run resume from another run.
   - SDK: Support `pf.run(resume_from=<original-run-name>)` to create a run resume from another run.
 - [SDK/CLI][azure] Create a run with `resume_from`.
   - CLI: Support `pfazure run create --resume-from <original-run-name>` to create a run resume from another run.
   - SDK: Support `p.run(resume_from=<original-run-name>)` to create a run resume from another run.
 
-
 ## 1.7.0 (2024.03.25)
 
 ### NOTICES
 - Import warnings will be printed when importing from `promptflow` namespace, please use imports from new namespaces
   suggested in the warning message.
 
 ### Features Added
```

## Comparing `promptflow-1.8.0.dist-info/NOTICE.txt` & `promptflow-1.9.0.dist-info/NOTICE.txt`

 * *Files identical despite different names*

