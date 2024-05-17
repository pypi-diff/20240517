# Comparing `tmp/arize_phoenix_evals-0.8.2.tar.gz` & `tmp/arize_phoenix_evals-0.9.0.tar.gz`

## Comparing `arize_phoenix_evals-0.8.2.tar` & `arize_phoenix_evals-0.9.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/__init__.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/classify.py
--rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/default_templates.py
--rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/evaluators.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/exceptions.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/executors.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/py.typed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/retrievals.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/templates.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/utils.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/anthropic.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/base.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/bedrock.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/litellm.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/mistralai.py
--rw-r--r--   0        0        0    15069 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/openai.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/rate_limiters.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertex.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertexai.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/.gitignore
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/IP_NOTICE
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/LICENSE
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/README.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/__init__.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/classify.py
+-rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/default_templates.py
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/evaluators.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/exceptions.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/executors.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/generate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/py.typed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/retrievals.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/templates.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/utils.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/anthropic.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/base.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/bedrock.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/litellm.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/mistralai.py
+-rw-r--r--   0        0        0    15311 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/openai.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/rate_limiters.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertex.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertexai.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/IP_NOTICE
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/README.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.0/PKG-INFO
```

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/__init__.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/classify.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/classify.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/default_templates.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/default_templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/evaluators.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/evaluators.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/executors.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/executors.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/generate.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/generate.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/retrievals.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/retrievals.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/templates.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/utils.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/anthropic.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/base.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/base.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/bedrock.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/litellm.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/litellm.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/mistralai.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/mistralai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/openai.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import warnings
 from dataclasses import dataclass, field, fields
 from typing import (
     Any,
     Callable,
     Dict,
     List,
+    Mapping,
     Optional,
     Tuple,
     Union,
     get_args,
     get_origin,
 )
 
@@ -94,14 +95,16 @@
     """
     The endpoint to use for azure openai. Available in the azure portal.
     https://learn.microsoft.com/en-us/azure/cognitive-services/openai/how-to/create-resource?pivots=web-portal#create-a-resource
     """
     azure_deployment: Optional[str] = field(default=None)
     azure_ad_token: Optional[str] = field(default=None)
     azure_ad_token_provider: Optional[Callable[[], str]] = field(default=None)
+    default_headers: Optional[Mapping[str, str]] = field(default=None)
+    """Default headers required by AzureOpenAI"""
 
     # Deprecated fields
     model_name: Optional[str] = field(default=None)
     """
     .. deprecated:: 3.0.0
        use `model` instead. This will be removed
     """
@@ -174,23 +177,25 @@
                 azure_endpoint=azure_options.azure_endpoint,
                 azure_deployment=azure_options.azure_deployment,
                 api_version=azure_options.api_version,
                 azure_ad_token=azure_options.azure_ad_token,
                 azure_ad_token_provider=azure_options.azure_ad_token_provider,
                 api_key=self.api_key,
                 organization=self.organization,
+                default_headers=self.default_headers,
             )
             self._async_client = self._openai.AsyncAzureOpenAI(
                 azure_endpoint=azure_options.azure_endpoint,
                 azure_deployment=azure_options.azure_deployment,
                 api_version=azure_options.api_version,
                 azure_ad_token=azure_options.azure_ad_token,
                 azure_ad_token_provider=azure_options.azure_ad_token_provider,
                 api_key=self.api_key,
                 organization=self.organization,
+                default_headers=self.default_headers,
             )
             # return early since we don't need to check the model
             return
 
         # The client is not azure, so it must be openai
         self._client = self._openai.OpenAI(
             api_key=self.api_key,
```

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/rate_limiters.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertex.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertex.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/src/phoenix/evals/models/vertexai.py` & `arize_phoenix_evals-0.9.0/src/phoenix/evals/models/vertexai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/LICENSE` & `arize_phoenix_evals-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/README.md` & `arize_phoenix_evals-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.8.2/pyproject.toml` & `arize_phoenix_evals-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-version = "0.8.2"
+version = "0.9.0"
 dependencies = [
   "pandas",
   "tqdm",
   "typing-extensions>=4.5, <5",
 ]
 
 [project.optional-dependencies]
```

### Comparing `arize_phoenix_evals-0.8.2/PKG-INFO` & `arize_phoenix_evals-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arize-phoenix-evals
-Version: 0.8.2
+Version: 0.9.0
 Summary: LLM Evaluations
 Project-URL: Documentation, https://docs.arize.com/phoenix/
 Project-URL: Issues, https://github.com/Arize-ai/phoenix/issues
 Project-URL: Source, https://github.com/Arize-ai/phoenix
 Author-email: Arize AI <phoenix-devs@arize.com>
 License: Elastic-2.0
 License-File: IP_NOTICE
```

