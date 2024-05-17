# Comparing `tmp/lotgi-0.0.8.tar.gz` & `tmp/lotgi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lotgi-0.0.8.tar", last modified: Wed May  8 04:23:08 2024, max compression
+gzip compressed data, was "lotgi-0.0.9.tar", last modified: Fri May 17 00:03:34 2024, max compression
```

## Comparing `lotgi-0.0.8.tar` & `lotgi-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 04:23:08.311086 lotgi-0.0.8/
--rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-08 04:23:08.310932 lotgi-0.0.8/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      705 2024-05-08 04:22:56.000000 lotgi-0.0.8/pyproject.toml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 04:23:08.307840 lotgi-0.0.8/python/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 04:23:08.309147 lotgi-0.0.8/python/lotgi/
--rw-r--r--   0 alex       (501) staff       (20)     7950 2024-05-08 04:22:35.000000 lotgi-0.0.8/python/lotgi/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.8/python/lotgi/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.8/python/lotgi/_openai.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 04:23:08.309872 lotgi-0.0.8/python/lotgi/asyncio/
--rw-r--r--   0 alex       (501) staff       (20)     1015 2024-05-07 20:29:22.000000 lotgi-0.0.8/python/lotgi/asyncio/rest_client.py
--rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.8/python/lotgi/logging.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 04:23:08.310198 lotgi-0.0.8/python/lotgi/models/
--rw-r--r--   0 alex       (501) staff       (20)     2203 2024-05-07 04:23:13.000000 lotgi-0.0.8/python/lotgi/models/rest.py
--rw-r--r--   0 alex       (501) staff       (20)     6156 2024-05-08 02:51:15.000000 lotgi-0.0.8/python/lotgi/rest_client.py
--rw-r--r--   0 alex       (501) staff       (20)     1316 2024-05-01 23:14:33.000000 lotgi-0.0.8/python/lotgi/tokens.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 04:23:08.310753 lotgi-0.0.8/python/lotgi.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-08 04:23:08.000000 lotgi-0.0.8/python/lotgi.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      472 2024-05-08 04:23:08.000000 lotgi-0.0.8/python/lotgi.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-08 04:23:08.000000 lotgi-0.0.8/python/lotgi.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       36 2024-05-08 04:23:08.000000 lotgi-0.0.8/python/lotgi.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       95 2024-05-08 04:23:08.000000 lotgi-0.0.8/python/lotgi.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       12 2024-05-08 04:23:08.000000 lotgi-0.0.8/python/lotgi.egg-info/top_level.txt
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-08 04:23:08.310467 lotgi-0.0.8/python/tests/
--rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.8/python/tests/test_basic.py
--rw-r--r--   0 alex       (501) staff       (20)       38 2024-05-08 04:23:08.311118 lotgi-0.0.8/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-17 00:03:34.825160 lotgi-0.0.9/
+-rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-17 00:03:34.825002 lotgi-0.0.9/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      705 2024-05-17 00:03:17.000000 lotgi-0.0.9/pyproject.toml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-17 00:03:34.820986 lotgi-0.0.9/python/
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-17 00:03:34.823038 lotgi-0.0.9/python/lotgi/
+-rw-r--r--   0 alex       (501) staff       (20)     7141 2024-05-16 23:08:59.000000 lotgi-0.0.9/python/lotgi/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)       61 2024-04-27 22:29:31.000000 lotgi-0.0.9/python/lotgi/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)      706 2024-04-11 20:15:07.000000 lotgi-0.0.9/python/lotgi/_openai.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-17 00:03:34.823936 lotgi-0.0.9/python/lotgi/asyncio/
+-rw-r--r--   0 alex       (501) staff       (20)     1015 2024-05-07 20:29:22.000000 lotgi-0.0.9/python/lotgi/asyncio/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)      736 2024-05-16 21:46:16.000000 lotgi-0.0.9/python/lotgi/convert_to_seconds.py
+-rw-r--r--   0 alex       (501) staff       (20)      383 2024-04-11 18:54:15.000000 lotgi-0.0.9/python/lotgi/logging.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-17 00:03:34.824139 lotgi-0.0.9/python/lotgi/models/
+-rw-r--r--   0 alex       (501) staff       (20)     1570 2024-05-16 22:37:34.000000 lotgi-0.0.9/python/lotgi/models/rest.py
+-rw-r--r--   0 alex       (501) staff       (20)     5584 2024-05-16 23:08:03.000000 lotgi-0.0.9/python/lotgi/rest_client.py
+-rw-r--r--   0 alex       (501) staff       (20)     1316 2024-05-01 23:14:33.000000 lotgi-0.0.9/python/lotgi/tokens.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-17 00:03:34.824828 lotgi-0.0.9/python/lotgi.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      525 2024-05-17 00:03:34.000000 lotgi-0.0.9/python/lotgi.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      547 2024-05-17 00:03:34.000000 lotgi-0.0.9/python/lotgi.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2024-05-17 00:03:34.000000 lotgi-0.0.9/python/lotgi.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       36 2024-05-17 00:03:34.000000 lotgi-0.0.9/python/lotgi.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       95 2024-05-17 00:03:34.000000 lotgi-0.0.9/python/lotgi.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       12 2024-05-17 00:03:34.000000 lotgi-0.0.9/python/lotgi.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2024-05-17 00:03:34.824581 lotgi-0.0.9/python/tests/
+-rw-r--r--   0 alex       (501) staff       (20)       49 2024-04-08 18:16:29.000000 lotgi-0.0.9/python/tests/test_basic.py
+-rw-r--r--   0 alex       (501) staff       (20)      982 2024-05-16 21:48:21.000000 lotgi-0.0.9/python/tests/test_convert_to_seconds.py
+-rw-r--r--   0 alex       (501) staff       (20)       38 2024-05-17 00:03:34.825191 lotgi-0.0.9/setup.cfg
```

### Comparing `lotgi-0.0.8/PKG-INFO` & `lotgi-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lotgi
-Version: 0.0.8
+Version: 0.0.9
 Summary: For the love of the game
 Author-email: Alex Wu <alexanderwu@berkeley.edu>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.0
```

### Comparing `lotgi-0.0.8/pyproject.toml` & `lotgi-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   "tabulate",
   "transformers",
   "openai",
   "tomli",
   "pandas",
   "shortuuid",
 ]
-version="0.0.8"
+version="0.0.9"
 
 
 [tool.setuptools.packages.find]
 where = ["python/"]
 
 [project.scripts]
 lotgi = "lotgi:cli"
```

### Comparing `lotgi-0.0.8/python/lotgi/__init__.py` & `lotgi-0.0.9/python/lotgi/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 ]
 
 
 from lotgi.rest_client import RestClient
 from lotgi.tokens import estimate_token_usage
 from lotgi.logging import init_logging
 from lotgi.models import rest
+from lotgi.convert_to_seconds import convert_to_seconds
 
 import click
 from tabulate import tabulate
 from datetime import timedelta
 from typing import Optional
 import sys
 import requests
 import datetime
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 import os
 import hashlib
 import binascii
 import pkg_resources
+import re
 
 __version__ = pkg_resources.get_distribution(__name__).version
 
 @click.group
 @click.version_option(__version__)
 def cli():
     """
@@ -82,30 +84,24 @@
     to_hash = f.read(2**20)
     while to_hash:
         sha256.update(to_hash)
         to_hash = f.read(2**20)
     return binascii.hexlify(sha256.digest()).decode()
 
 @cli.command
-@click.option("--model", required=True, help="The model to run inference with.")
+@click.option("--name", required=False, help="The model to run inference with.")
 @click.option("--input-file", required=False, help="The name of the file (uploaded with `lotgi upload`)to run inference on.")
 @click.option("--input-path", required=False, help="The url or path to a file to run inference on.")
-@click.option("--field", required=True, help="The field within a row containing the data.")
-@click.option("--tradeoff", required=False, default=None, help=f"The tradeoff ({rest.EXECUTION_TRADEOFFS}).")
-@click.option("--prompt", required=False, help="Prompt to use for inference. Leave empty if prompt is already included in the dataset.")
-@click.option("--max-output-tokens", required=False, help="The maximum number of output tokens. [default=32]. Changing this value may affect the job cost.")
-@click.option("--regex", required=False, help="Force the output to match a given regular expression.")
+@click.option("--target-duration", required=False, help="The url or path to a file to run inference on.")
 def submit(
-        model : str,
+        *,
         input_file : str,
-        input_path : str, field : str,
-        tradeoff : Optional[str],
-        prompt: Optional[str],
-        max_output_tokens : Optional[int],
-        regex : Optional[str],
+        input_path : str,
+        name : Optional[str],
+        target_duration : Optional[str] = None,
 ):
     """
     Submit a new batch inference job.
 
     Your job file is expected to be formatted as a jsonl file. Each line corresponds to a request and should be a json object. Use the `--field` argument to specify which field of the json object contains the text to complete.
 
     For example, if a file stored at `example.com/dataset.jsonl` contains the contents
@@ -123,40 +119,33 @@
             --tradeoff Cheapest 
             --prompt "Summarize the following text"`. 
     
     This will run the mistral-7b model against the inputs "hello" and "lorem" with the provided prompt, optimizing for cost.
     """
     client = RestClient()
 
-    # if tradeoff is None:
-    #     print(f"Scanning job to estimate costs...")
-    #     job_execution_options_input = estimate_token_usage(input_file=input_file, prompt="", model=model, field=field)
-    #     options = client.job_exection_options(job_execution_options_input=job_execution_options_input)
-
-    #     print(format_execution_options(options))
-    #     tradeoff = get_tradeoff()
+    if target_duration is None:
+        target_duration_s = -1
+    else:
+        target_duration_s = convert_to_seconds(target_duration)
+        assert target_duration_s >= 5 * 60, f"Target duration should be at least 5m. {target_duration=}"
 
     if (not (input_file or input_path)) or (input_file and input_path):
         print("Must specify exactly one of --input-file or --input-path", file=sys.stderr)
         sys.exit(1)
 
     if input_path:
         with open(input_path, "rb") as f:
             input_file = "sha256:" + sha256_file(f)
         upload_file(client, input_file, input_path)
 
     result = client.submit_job(
-        model=model,
+        name=name or "<anonymous>",
         input_file=input_file,
-        field=field,
-        target_cost=-1,
-        target_deadline=-1,
-        execution_tradeoff=tradeoff,
-        max_output_tokens=max_output_tokens,
-        regex=regex,
+        target_duration=target_duration_s,
     )
     print("Success!")
     print(result)
 
 
 @cli.command
 def list():
@@ -164,19 +153,18 @@
     List your batch inferences jobs.
     """
     client = RestClient()
     jobs = sorted(client.list_jobs(), key=lambda job: job.submission_time, reverse=True)
 
     to_display = {
         "Job ID": [job.job_id for job in jobs],
-        "Model": [job.model for job in jobs],
+        "Name": [job.name for job in jobs],
         "Status": [job.state for job in jobs],
         "Submission time": [datetime.datetime.fromtimestamp(job.submission_time).strftime('%Y-%m-%d %H:%M:%S') for job in jobs],
-        "Tradeoff": [job.execution_tradeoff for job in jobs],
-        "Field": [job.field for job in jobs],
+        "Target Duration": [format_duration(job.target_duration) for job in jobs],
         "Input": [job.input_file for job in jobs],
     }
 
     print(tabulate(to_display, headers="keys"))
 
 
 @cli.command
```

### Comparing `lotgi-0.0.8/python/lotgi/_openai.py` & `lotgi-0.0.9/python/lotgi/_openai.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.8/python/lotgi/asyncio/rest_client.py` & `lotgi-0.0.9/python/lotgi/asyncio/rest_client.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.8/python/lotgi/models/rest.py` & `lotgi-0.0.9/python/lotgi/models/rest.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,57 +17,34 @@
 
     @model_validator(mode="after")
     def atleast_one_credential(self):
         if not (self.modal_credentials or self.runpod_credentials):
             raise ValueError("At least one set of credentials should be specified.")
         return self
 
-EXECUTION_TRADEOFFS = {
-    "Cheapest",
-    "Hour",
-}
-
-DEFAULT_MAX_OUTPUT_TOKENS = 32
-DEFAULT_REGEX = r".*"
-
 class JobSpec(BaseModel):
     job_id : str = Field(default_factory=lambda : f"job-{uuid_generator.uuid()}")
+    name : str
     cloud_credentials : Optional[CloudCredentials] = None
     input_file : str
-    target_cost : float
-    target_deadline : int # Specified as a unix timestamp
-    model : str
-    field : str
-    execution_tradeoff : str
-    max_output_tokens : int = DEFAULT_MAX_OUTPUT_TOKENS
-    regex : str = DEFAULT_REGEX
+    target_duration : Optional[int] # Duration in s -1 for Cheapest
     huggingface_token : Optional[str] = None
 
-    # @model_validator(mode="after")
-    # def valid_execution_tradeoff(self):
-    #     if self.execution_tradeoff not in EXECUTION_TRADEOFFS:
-    #         raise ValueError(f"execution_tradeoff must be one off {EXECUTION_TRADEOFFS}")
-    #     return self
-
 class JobStatus(BaseModel, extra=Extra.allow):
     job_id : str
+    name : str
     state : str
-    model : str
     submission_time : int
-    execution_tradeoff : str
     input_file : str
-    target_cost : float
-    target_deadline : int # Specified as a unix timestamp
-    field : str
+    target_duration : int # -1 for Cheapest
 
 class JobExecutionOptionsInput(BaseModel):
     input_token_count : int
     num_requests : int
     model : str
-    max_output_tokens : int = 32
 
 class JobExecutionTradeoffOption(BaseModel):
     option_name : str
     expected_cost : float
     expected_duration : int # In seconds
 
 class MetricInput(BaseModel):
```

### Comparing `lotgi-0.0.8/python/lotgi/rest_client.py` & `lotgi-0.0.9/python/lotgi/rest_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,56 +55,40 @@
 
         self.headers = {
             "lotgi-token": self._token,
             "Content-type": "application/json",
         }
 
     def submit_job(self, *,
-                   model : str,
+                   name : str,
                    input_file : str,
-                   field : str,
-                   target_cost : float,
-                   target_deadline : int,
-                   execution_tradeoff : str,
-                   max_output_tokens : Optional[int],
-                   regex : Optional[str],
+                   target_duration : int,
                    _autodetect_cloud_credentials : bool = False
                    ) -> rest.JobStatus:
         url = f"{self.endpoint}/create_job"
 
         if _autodetect_cloud_credentials:
             cloud_credentials = get_cloud_credentials()
         else:
             cloud_credentials = None
 
 
-        if max_output_tokens is None:
-            max_output_tokens = rest.DEFAULT_MAX_OUTPUT_TOKENS
-        if regex  is None:
-            regex = rest.DEFAULT_REGEX
-
         if _autodetect_cloud_credentials:
             huggingface_token = get_huggingface_credentials()
         else:
             huggingface_token = ""
 
         job_spec = rest.JobSpec(
             cloud_credentials=cloud_credentials,
             input_file=input_file,
-            model=model,
-            field=field,
-            target_cost=target_cost,
-            target_deadline=target_deadline,
-            execution_tradeoff=execution_tradeoff,
+            name=name,
+            target_duration=target_duration,
             huggingface_token=huggingface_token,
-            max_output_tokens=max_output_tokens,
-            regex=regex,
         )
 
-
         body = job_spec.dict()
 
         result = requests.post(url, headers=self.headers, json=body)
 
         if result.status_code == 401:
             raise PermissionError(f"Request authentication failed. Is your `LOTGI_TOKEN` environment variable set correctly? {result.status_code} : {result.json()['detail']}")
```

### Comparing `lotgi-0.0.8/python/lotgi/tokens.py` & `lotgi-0.0.9/python/lotgi/tokens.py`

 * *Files identical despite different names*

### Comparing `lotgi-0.0.8/python/lotgi.egg-info/PKG-INFO` & `lotgi-0.0.9/python/lotgi.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lotgi
-Version: 0.0.8
+Version: 0.0.9
 Summary: For the love of the game
 Author-email: Alex Wu <alexanderwu@berkeley.edu>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: click>=7.0
```

