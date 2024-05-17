# Comparing `tmp/openai_priority_loadbalancer-1.0.5.tar.gz` & `tmp/openai_priority_loadbalancer-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_priority_loadbalancer-1.0.5.tar", last modified: Fri May 17 00:01:12 2024, max compression
+gzip compressed data, was "openai_priority_loadbalancer-1.0.6.tar", last modified: Fri May 17 10:52:07 2024, max compression
```

## Comparing `openai_priority_loadbalancer-1.0.5.tar` & `openai_priority_loadbalancer-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 00:01:12.663713 openai_priority_loadbalancer-1.0.5/
--rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.5/LICENSE
--rw-rw-rw-   0        0        0    13018 2024-05-16 22:09:58.000000 openai_priority_loadbalancer-1.0.5/PACKAGE_README.md
--rw-rw-rw-   0        0        0    13869 2024-05-17 00:01:12.662720 openai_priority_loadbalancer-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    12397 2024-05-15 19:08:43.000000 openai_priority_loadbalancer-1.0.5/README.md
--rw-rw-rw-   0        0        0      726 2024-05-17 00:00:28.000000 openai_priority_loadbalancer-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 00:01:12.664922 openai_priority_loadbalancer-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 00:01:12.571797 openai_priority_loadbalancer-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 00:01:12.608340 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer/
--rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer/__init__.py
--rw-rw-rw-   0        0        0    13499 2024-05-16 20:36:45.000000 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
-drwxrwxrwx   0        0        0        0 2024-05-17 00:01:12.659280 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer.egg-info/
--rw-rw-rw-   0        0        0    13869 2024-05-17 00:01:12.000000 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2024-05-17 00:01:12.000000 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 00:01:12.000000 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-17 00:01:12.000000 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2024-05-17 00:01:12.000000 openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 10:52:07.730890 openai_priority_loadbalancer-1.0.6/
+-rw-rw-rw-   0        0        0     1068 2024-05-11 18:48:22.000000 openai_priority_loadbalancer-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0    13852 2024-05-17 10:36:38.000000 openai_priority_loadbalancer-1.0.6/PACKAGE_README.md
+-rw-rw-rw-   0        0        0    14748 2024-05-17 10:52:07.727430 openai_priority_loadbalancer-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12246 2024-05-17 10:37:02.000000 openai_priority_loadbalancer-1.0.6/README.md
+-rw-rw-rw-   0        0        0      724 2024-05-17 10:51:18.000000 openai_priority_loadbalancer-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 10:52:07.731897 openai_priority_loadbalancer-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 10:52:07.623523 openai_priority_loadbalancer-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 10:52:07.660576 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer/
+-rw-rw-rw-   0        0        0       45 2024-05-14 20:10:13.000000 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer/__init__.py
+-rw-rw-rw-   0        0        0    13499 2024-05-16 20:36:45.000000 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py
+drwxrwxrwx   0        0        0        0 2024-05-17 10:52:07.722434 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer.egg-info/
+-rw-rw-rw-   0        0        0    14748 2024-05-17 10:52:07.000000 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      439 2024-05-17 10:52:07.000000 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 10:52:07.000000 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-17 10:52:07.000000 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2024-05-17 10:52:07.000000 openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer.egg-info/top_level.txt
```

### Comparing `openai_priority_loadbalancer-1.0.5/LICENSE` & `openai_priority_loadbalancer-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.5/PACKAGE_README.md` & `openai_priority_loadbalancer-1.0.6/PACKAGE_README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,48 +30,62 @@
 ## Prerequisites
 
 It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
 It's also good to have some knowledge of authentication and identities.
 
 ## Getting Started
 
+The steps below are not comprehensive for every way to set up Azure OpenAI integration with the [OpenAI Python API library](https://github.com/openai/openai-python) (e.g. the token provider). You can see specific implementation examples in [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) in the GitHub repo.
+
 ### Installing the Package
 
+You should already have the `openai` package set up.
+
 1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
 
     ```text
     openai_priority_loadbalancer
     ```
 
 1. Run `pip install -r </path/to/requirements.txt>`.
 
 ### Importing Classes
 
-Either import the **synchronous** load balancer:
+Either import the **synchronous** `AzureOpenAI` and `LoadBalancer`:
 
 ```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AzureOpenAI
+
+# openai-priority-loadbalancer imports
 from typing import List
 import httpx
 from openai_priority_loadbalancer import LoadBalancer, Backend
 ```
 
-Or import the **asynchronous** load balancer:
+Or import the **asynchronous** `AsyncAzureOpenAI` and `AsyncLoadBalancer`:
 
 ```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AsyncAzureOpenAI
+
+# openai-priority-loadbalancer imports
 from typing import List
 import httpx
 from openai_priority_loadbalancer import AsyncLoadBalancer, Backend
 ```
 
 *Importing `httpx` lets us use `httpx.Client` and `httpx.AsyncClient`. This avoids having to update openai to at least
 [1.17.0](https://github.com/openai/openai-python/releases/tag/v1.17.0). The `openai` properties for `DefaultHttpxClient` and `DefaultAsyncHttpxClient` are mere wrappers for `httpx.Client` and `httpx.AsyncClient`.*
 
 ### Configuring the Backends and Load Balancer
 
-1. Define a list of backends according to the *Load Balancer Configuration* section below.
+1. Define a list of backends according to the *Load Balancer Backend Configuration* section below.
 
     ```python
     backends: List[Backend] = [
         Backend("oai-eastus.openai.azure.com", 1),
         Backend("oai-southcentralus.openai.azure.com", 1)
     ]
     ```
@@ -92,70 +106,25 @@
     ```
 
     **Asynchronous**
 
     ```python
     lb = AsyncLoadBalancer(backends)
 
-    client = AzureOpenAI(
+    client = AsyncAzureOpenAI(
         azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
         azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
         api_version = "2024-04-01-preview",
         http_client = httpx.AsyncClient(transport = lb)         # Inject the asynchronous load balancer as the transport in a new default async httpx client.
     )
     ```
 
-### Using the Load Balancer
-
-As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
-
-### Logging
-
-OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+## Load Balancer Backend Configuration
 
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
-
-## Load Balancer Configuration
-
-At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
 
 I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
 The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
 While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
 
 ### One Backend
 
@@ -214,7 +183,52 @@
 # Define the backends and their priority
 backends = [
     Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
     Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
     Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
 ]
 ```
+
+### Using the Load Balancer
+
+As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
+
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
```

### Comparing `openai_priority_loadbalancer-1.0.5/PKG-INFO` & `openai_priority_loadbalancer-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.5
+Version: 1.0.6
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai
+Requires-Dist: httpx
+Requires-Dist: python-dateutil
 
 # OpenAI Priority Load Balancer
 
 Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
 
 - Distribution of requests over multiple consumption instances to mitigate throttling.
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
@@ -45,48 +46,62 @@
 ## Prerequisites
 
 It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
 It's also good to have some knowledge of authentication and identities.
 
 ## Getting Started
 
+The steps below are not comprehensive for every way to set up Azure OpenAI integration with the [OpenAI Python API library](https://github.com/openai/openai-python) (e.g. the token provider). You can see specific implementation examples in [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) in the GitHub repo.
+
 ### Installing the Package
 
+You should already have the `openai` package set up.
+
 1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
 
     ```text
     openai_priority_loadbalancer
     ```
 
 1. Run `pip install -r </path/to/requirements.txt>`.
 
 ### Importing Classes
 
-Either import the **synchronous** load balancer:
+Either import the **synchronous** `AzureOpenAI` and `LoadBalancer`:
 
 ```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AzureOpenAI
+
+# openai-priority-loadbalancer imports
 from typing import List
 import httpx
 from openai_priority_loadbalancer import LoadBalancer, Backend
 ```
 
-Or import the **asynchronous** load balancer:
+Or import the **asynchronous** `AsyncAzureOpenAI` and `AsyncLoadBalancer`:
 
 ```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AsyncAzureOpenAI
+
+# openai-priority-loadbalancer imports
 from typing import List
 import httpx
 from openai_priority_loadbalancer import AsyncLoadBalancer, Backend
 ```
 
 *Importing `httpx` lets us use `httpx.Client` and `httpx.AsyncClient`. This avoids having to update openai to at least
 [1.17.0](https://github.com/openai/openai-python/releases/tag/v1.17.0). The `openai` properties for `DefaultHttpxClient` and `DefaultAsyncHttpxClient` are mere wrappers for `httpx.Client` and `httpx.AsyncClient`.*
 
 ### Configuring the Backends and Load Balancer
 
-1. Define a list of backends according to the *Load Balancer Configuration* section below.
+1. Define a list of backends according to the *Load Balancer Backend Configuration* section below.
 
     ```python
     backends: List[Backend] = [
         Backend("oai-eastus.openai.azure.com", 1),
         Backend("oai-southcentralus.openai.azure.com", 1)
     ]
     ```
@@ -107,70 +122,25 @@
     ```
 
     **Asynchronous**
 
     ```python
     lb = AsyncLoadBalancer(backends)
 
-    client = AzureOpenAI(
+    client = AsyncAzureOpenAI(
         azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
         azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
         api_version = "2024-04-01-preview",
         http_client = httpx.AsyncClient(transport = lb)         # Inject the asynchronous load balancer as the transport in a new default async httpx client.
     )
     ```
 
-### Using the Load Balancer
-
-As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
-
-### Logging
-
-OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+## Load Balancer Backend Configuration
 
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
-
-## Load Balancer Configuration
-
-At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
 
 I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
 The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
 While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
 
 ### One Backend
 
@@ -229,7 +199,52 @@
 # Define the backends and their priority
 backends = [
     Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
     Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
     Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
 ]
 ```
+
+### Using the Load Balancer
+
+As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
+
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
```

### Comparing `openai_priority_loadbalancer-1.0.5/README.md` & `openai_priority_loadbalancer-1.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,183 +1,183 @@
-# Python OpenAI Load Balancer
-
-TL;DR! How do I [start](#getting-started)?
-
----
-
-Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
-
-- Distribution of requests over multiple consumption instances to mitigate throttling.
-- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
-- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
-
-While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
-
-And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
-
-Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
-
-## Disclaimer
-
-**This is a pseudo load-balancer.**
-
-When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
-immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
-
-Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
-
-## Attribution
-
-This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
-
-## Prerequisites
-
-It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
-It's also good to have some knowledge of authentication and identities.
-
-## Authentication
-
-Locally, you can log into Azure via the CLI and the steps below and use the `AzureDefaultCredential` (what I use in my example). When deploying this application in Azure, it's recommended to use a managed identity for authentication. It's best to avoid using the Azure OpenAI instances' keys as that could a) accidentally leave credentials in your source code, and b) the keys are different for each instance, which would probably require expanding upon the `Backends` class. Best to just avoid keys.
-
-## Getting Started
-
-### Cloning the repo & Preparing the python environment
-
-1. Clone the repo.
-1. Open the cloned repo folder in VS Code.
-1. Open a terminal session in VS Code.
-1. Run [setup-python.ps1](./setup-python.ps1) to prepare the python environment.
-
-### Configuration
-
-For the load-balanced approach, please use the same model across all instances.
-
-1. Open [aoai.py](./aoai.py).
-1. Replace `<your-aoai-model>` with the name of your Azure OpenAI model.
-1. Replace `<your-aoai-instance>` with the primary/single Azure OpenAI instance.
-1. Replace `<your-aoai-instance-1>`, `<your-aoai-instance-2>`, `<your-aoai-instance-3>` with all the Azure OpenAI instances you want to load-balance across. Delete entries you don't need. See [Load Balancer Configuration](#load-balancer-configuration) for details.
-1. Replace the value for variable `num_of_requests` with the number of requests you wish to execute.
-
-### Credentials
-
-Locally, your `AzureDefaultCredential` is used. Each Azure OpenAI instance must be configured with the `Cognitive Services OpenAI` User role for your Azure credential (the identity you use after logging in). This ensures that you can use your credential across all Azure OpenAI instances.
-
-When running in Azure, it's advised to use managed identities.
-
-1. Log in with `az login`.
-1. Set your subscription in which your Azure OpenAI assets reside: `az account set -s <name or id>`
-
-    *Missing this step may result in HTTP 400 errors for a tenant mismatch.*
-
-## Execution
-
-1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
-1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-![Parallel Execution](./assets/parallel-execution.png)
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
-
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
-
-## Load Balancer Configuration
-
-At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
-
-I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
-The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
-While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
-
-### One Backend
-
-This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Two Backends with Same Priority
-
-Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Same Priority
-
-Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
-]
-```
-
-### Three Backends with Two Different Priorities
-
-The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
-]
-```
-
-### Three Backends with Three Different Priorities
-
-An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
-
-```python
-# Define the backends and their priority
-backends = [
-    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
-    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
-    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
-]
-```
+# Python OpenAI Load Balancer
+
+TL;DR! How do I [start](#getting-started)?
+
+---
+
+Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
+
+- Distribution of requests over multiple consumption instances to mitigate throttling.
+- Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
+- Tiered prioritization of multiple consumption instances (e.g. use instances first that are geographically closer).
+
+While the [OpenAI Python API library](https://github.com/openai/openai-python) respects HTTP 429 and automatically retries after the requested wait period, the library is not set up to support the aforementioned customer desires. The library does, however, allow for the injection of custom httpx clients. This gave rise to this project.
+
+And while there are other Python OpenAI load balancers freely available, I have not seen one yet that addresses the aforementioned scenarios.
+
+Python OpenAI LoadBalancer is injected cleanly into the OpenAI Python API library. The changes between a conventional and a load-balanced Azure OpenAI implementation are few and almost entirely configuration of the backends to be used. You can see a side-by-side example in the [aoai.py](./aoai.py) file in this repo.
+
+## Disclaimer
+
+**This is a pseudo load-balancer.**
+
+When executing this code in parallel, there is no way to distribute requests uniformly across all Azure OpenAI instances. Doing so would require a centralized service, cache, etc. to keep track of a common backends list, but that would also imply a locking mechanism for updates, which would
+immediately inhibit the performance benefits of the load balancer. Without knowledge of any other python workers, we can only randomize selection of an available backend.
+
+Furthermore, while the load balancer handles retries across available backends, the [OpenAI Python API library](https://github.com/openai/openai-python) is not fully insulated from failing on multiple HTTP 429s when all backends are returning HTTP 429s. It is advised to load-test with multiple concurrent python workers to understand how your specific Azure OpenAI instances, your limits, and your load balancer configuration function.
+
+## Attribution
+
+This project would not have been possible without the incredible work that [@andredewes](https://github.com/andredewes) has done with his [Smart Load Balancing for OpenAI Endpoints and Azure API Management](https://github.com/Azure-Samples/openai-apim-lb). If you use Azure API Management in your infrastructure, I highly recommend you consider his policy.
+
+## Prerequisites
+
+It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in `aoai.py` here will look very familiar to you.
+It's also good to have some knowledge of authentication and identities.
+
+## Authentication
+
+Locally, you can log into Azure via the CLI and the steps below and use the `AzureDefaultCredential` (what I use in my example). When deploying this application in Azure, it's recommended to use a managed identity for authentication. It's best to avoid using the Azure OpenAI instances' keys as that could a) accidentally leave credentials in your source code, and b) the keys are different for each instance, which would probably require expanding upon the `Backends` class. Best to just avoid keys.
+
+## Getting Started
+
+### Cloning the repo & Preparing the python environment
+
+1. Clone the repo.
+1. Open the cloned repo folder in VS Code.
+1. Open a terminal session in VS Code.
+1. Run [setup-python.ps1](./setup-python.ps1) to prepare the python environment.
+
+### Configuration
+
+For the load-balanced approach, please use the same model across all instances.
+
+1. Open [aoai.py](./aoai.py).
+1. Replace `<your-aoai-model>` with the name of your Azure OpenAI model.
+1. Replace `<your-aoai-instance>` with the primary/single Azure OpenAI instance.
+1. Replace `<your-aoai-instance-1>`, `<your-aoai-instance-2>`, `<your-aoai-instance-3>` with all the Azure OpenAI instances you want to load-balance across. Delete entries you don't need. See [Load Balancer Backend Configuration](#load-balancer-backend-configuration) for details.
+1. Replace the value for variable `num_of_requests` with the number of requests you wish to execute.
+
+### Credentials
+
+Locally, your `AzureDefaultCredential` is used. Each Azure OpenAI instance must be configured with the `Cognitive Services OpenAI` User role for your Azure credential (the identity you use after logging in). This ensures that you can use your credential across all Azure OpenAI instances.
+
+When running in Azure, it's advised to use managed identities.
+
+1. Log in with `az login`.
+1. Set your subscription in which your Azure OpenAI assets reside: `az account set -s <name or id>`
+
+    *Missing this step may result in HTTP 400 errors for a tenant mismatch.*
+
+## Execution
+
+1. Initially, [python-aoai.ps1](./python-aoai.ps1) once to ensure it executes correctly.
+1. Run [python-aoai.ps1](./python-aoai.ps1) concurrently in multiple terminals to simulate parallel requests from multiple python workers.
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+![Parallel Execution](./assets/parallel-execution.png)
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
+
+## Load Balancer Backend Configuration
+
+At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+
+I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
+The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
+While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
+
+### One Backend
+
+This is logically equivalent to what the standard approach does. This configuration does not provide value over the standard approach.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Two Backends with Same Priority
+
+Load-balancing evenly between Azure OpenAI instances hedges you against being stalled due to a 429 from a single instance.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Same Priority
+
+Adding a third backend with same priority exacerbates the difference to the standard approach further. Here, we need to use 20 requests to incur more HTTP 429s.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 1)
+]
+```
+
+### Three Backends with Two Different Priorities
+
+The most common reason for this approach may well be the prioritization of Provisioned Throughput Units (PTUs). This is a reserved capacity over a period of time that is billed at that reservation and not flexible as consumption instances. Aside from guaranteed capacity, latency is also much more stable. Naturally, this is an instance that you would want to prioritize over all others but allow yourself to have fallbacks if you burst over what the PTU provides.
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 2)
+]
+```
+
+### Three Backends with Three Different Priorities
+
+An example of this setup may be that most of your assets reside in one region (e.g. East US). It stands to reason that you want to use the Azure OpenAI instance in that region. To hedge yourself against HTTP 429s, you decide to add a second region that's geographically close (e.g. East US 2) as well as a third (e.g. West US).
+
+```python
+# Define the backends and their priority
+backends = [
+    Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
+    Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
+    Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
+]
+```
```

### Comparing `openai_priority_loadbalancer-1.0.5/pyproject.toml` & `openai_priority_loadbalancer-1.0.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-[project]
-name = "openai_priority_loadbalancer"
-version = "1.0.5"
-authors = [
-  { name="Simon Kurtz", email="simonkurtz@gmail.com" },
-]
-description = "A multi-backend, prioritization load balancer for OpenAI"
-readme = "PACKAGE_README.md"
-requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-    "openai",
-]
-[project.urls]
-Homepage = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer"
-Issues = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues"
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+[project]
+name = "openai_priority_loadbalancer"
+version = "1.0.6"
+authors = [
+  { name="Simon Kurtz", email="simonkurtz@gmail.com" },
+]
+description = "A multi-backend, prioritization load balancer for OpenAI"
+readme = "PACKAGE_README.md"
+requires-python = ">=3.8"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+    "httpx",
+    "python-dateutil"
+]
+[project.urls]
+Homepage = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer"
+Issues = "https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
```

### Comparing `openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py` & `openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer/openai_priority_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `openai_priority_loadbalancer-1.0.5/src/openai_priority_loadbalancer.egg-info/PKG-INFO` & `openai_priority_loadbalancer-1.0.6/src/openai_priority_loadbalancer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: openai_priority_loadbalancer
-Version: 1.0.5
+Version: 1.0.6
 Summary: A multi-backend, prioritization load balancer for OpenAI
 Author-email: Simon Kurtz <simonkurtz@gmail.com>
 Project-URL: Homepage, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer
 Project-URL: Issues, https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai
+Requires-Dist: httpx
+Requires-Dist: python-dateutil
 
 # OpenAI Priority Load Balancer
 
 Many AI workloads require using more than one Azure OpenAI instance to prioritize Provisioned Throughput Units (PTUs) and insulate themselves from timeouts. In having worked with customers on Azure OpenAI implementations, there are a few common, desired configurations:
 
 - Distribution of requests over multiple consumption instances to mitigate throttling.
 - Prioritize exhaustion of all tokens in a PTU instance with a fallback onto multiple consumption instances.
@@ -45,48 +46,62 @@
 ## Prerequisites
 
 It helps to have some familiarity with how the [OpenAI Python API library](https://github.com/openai/openai-python) works. If you have used it before, then the code in the [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) test harness for this package will look very familiar to you.
 It's also good to have some knowledge of authentication and identities.
 
 ## Getting Started
 
+The steps below are not comprehensive for every way to set up Azure OpenAI integration with the [OpenAI Python API library](https://github.com/openai/openai-python) (e.g. the token provider). You can see specific implementation examples in [aoai.py](https://github.com/simonkurtz-MSFT/python-openai-loadbalancer/blob/main/aoai.py) in the GitHub repo.
+
 ### Installing the Package
 
+You should already have the `openai` package set up.
+
 1. Add `openai_priority_loadbalancer` to your *requirements.txt* file.
 
     ```text
     openai_priority_loadbalancer
     ```
 
 1. Run `pip install -r </path/to/requirements.txt>`.
 
 ### Importing Classes
 
-Either import the **synchronous** load balancer:
+Either import the **synchronous** `AzureOpenAI` and `LoadBalancer`:
 
 ```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AzureOpenAI
+
+# openai-priority-loadbalancer imports
 from typing import List
 import httpx
 from openai_priority_loadbalancer import LoadBalancer, Backend
 ```
 
-Or import the **asynchronous** load balancer:
+Or import the **asynchronous** `AsyncAzureOpenAI` and `AsyncLoadBalancer`:
 
 ```python
+# openai & other imports
+from azure.identity import DefaultAzureCredential, get_bearer_token_provider
+from openai import AsyncAzureOpenAI
+
+# openai-priority-loadbalancer imports
 from typing import List
 import httpx
 from openai_priority_loadbalancer import AsyncLoadBalancer, Backend
 ```
 
 *Importing `httpx` lets us use `httpx.Client` and `httpx.AsyncClient`. This avoids having to update openai to at least
 [1.17.0](https://github.com/openai/openai-python/releases/tag/v1.17.0). The `openai` properties for `DefaultHttpxClient` and `DefaultAsyncHttpxClient` are mere wrappers for `httpx.Client` and `httpx.AsyncClient`.*
 
 ### Configuring the Backends and Load Balancer
 
-1. Define a list of backends according to the *Load Balancer Configuration* section below.
+1. Define a list of backends according to the *Load Balancer Backend Configuration* section below.
 
     ```python
     backends: List[Backend] = [
         Backend("oai-eastus.openai.azure.com", 1),
         Backend("oai-southcentralus.openai.azure.com", 1)
     ]
     ```
@@ -107,70 +122,25 @@
     ```
 
     **Asynchronous**
 
     ```python
     lb = AsyncLoadBalancer(backends)
 
-    client = AzureOpenAI(
+    client = AsyncAzureOpenAI(
         azure_endpoint = f"https://{backends[0].host}",         # Must be seeded, so we use the first host. It will get overwritten by the load balancer.
         azure_ad_token_provider = token_provider,               # Your authentication may vary. Please adjust accordingly.
         api_version = "2024-04-01-preview",
         http_client = httpx.AsyncClient(transport = lb)         # Inject the asynchronous load balancer as the transport in a new default async httpx client.
     )
     ```
 
-### Using the Load Balancer
-
-As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
-
-### Logging
-
-OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
-
-## Distribution of Requests
-
-### Across Different Priorities
-
-Requests are made to the highest priority backend that is available. For example:
-
-- Priority 1, when available, will always supersede priority 2.
-- Priority 2, when available, will always supersede an unavailable priority 1.
-- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
-
-### Across Multiple Backends of Same Priority
-
-In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
-
-There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
-
-## Backoff & Retries
-
-When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
-You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
-
-In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
-The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+## Load Balancer Backend Configuration
 
-```text
-2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
-2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
-2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
-2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
-2024-05-11 00:56:32.452883:   No backends available. Exiting.
-2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
-2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
-2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
-```
-
-## Load Balancer Configuration
-
-At its core, the Load Balancer configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
+At its core, the Load Balancer Backend configuration requires one or more backend hosts and a numeric priority starting at 1. Please take note that you define a host, not a URL.
 
 I use a total of three Azure OpenAI instances in three regions. These instances are set up with intentionally small tokens-per-minute (tpm) to trigger HTTP 429s.
 The standard approach never changes and uses the same host (first in the backend list), which provides a stable comparison to the load-balanced approach.
 While the number of requests differs per tests below, we issue the same number of requests against standard and load-balanced approaches.
 
 ### One Backend
 
@@ -229,7 +199,52 @@
 # Define the backends and their priority
 backends = [
     Backends("oai-eastus-xxxxxxxx.openai.azure.com", 1),
     Backends("oai-southcentralus-xxxxxxxx.openai.azure.com", 2),
     Backends("oai-westus-xxxxxxxx.openai.azure.com", 3)
 ]
 ```
+
+### Using the Load Balancer
+
+As these are the only changes to the [OpenAI Python API library](https://github.com/openai/openai-python) implementation, simply execute your python code.
+
+### Logging
+
+OpenAI Priority Load Balancer uses Python's [logging](https://docs.python.org/3/library/logging.html) module. The name of the logger is `openai-priority-loadbalancer`.
+
+## Distribution of Requests
+
+### Across Different Priorities
+
+Requests are made to the highest priority backend that is available. For example:
+
+- Priority 1, when available, will always supersede priority 2.
+- Priority 2, when available, will always supersede an unavailable priority 1.
+- Priority 3, when available, will always supersede unavailable priorities 1 & 2.
+
+### Across Multiple Backends of Same Priority
+
+In the single-requestor model, the distribution of attempts over available backends should be fairly uniform for backends of the same priority.
+
+There is no likelihood of a uniform distribution across available endpoints when running multiple python workers in parallel. In the below example, each terminal is executing 20 requests over two Azure OpenAI instances, both set up with the lowest of tokens-per-minute setting. Available backends are selected randomly (see the first request in each terminal). No sharing of data between the two terminals exists. Recovery takes place, when possible; otherwise, an HTTP 429 is returned to the OpenAI Python API library.
+
+## Backoff & Retries
+
+When no backends are available (e.g. all timed out), Python OpenAI Load Balancer returns the soonest retry in seconds determined based on the `retry_after` value on each backend.
+You may notice a delay in the logs between when the load balancer returns and when the next request is made. In addition to the `Retry-After` header value, the OpenAI Python library [uses a short exponential backoff](https://github.com/openai/openai-python?tab=readme-ov-file#retries).
+
+In this log excerpt, we see that all three backends are timing out. As the standard behavior returns an HTTP 429 from a single backend, we do the same here with the load-balanced approach. This allows the OpenAI Python library to handle the HTTP 429 that it believes it received from a singular backend.
+The wait periods are 44 seconds (westus), 4 seconds (eastus), and 7 seconds (southcentralus) in this log. Our logic determines that eastus will become available soonest. Therefore, we return a `Retry-After` header with a value of `4`. The OpenAI Python library then adds its exponential backoff (~2 seconds here).
+
+```text
+2024-05-11 00:56:32.299477:   Request sent to server: https://oai-westus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.299477:   Backend oai-westus-20240509.openai.azure.com is throttling. Retry after 44 second(s).
+2024-05-11 00:56:32.394350:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.395578:   Backend oai-eastus-20240509.openai.azure.com is throttling. Retry after 4 second(s).
+2024-05-11 00:56:32.451891:   Request sent to server: https://oai-southcentralus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status Code: 429 - FAIL
+2024-05-11 00:56:32.452883:   Backend oai-southcentralus-20240509.openai.azure.com is throttling. Retry after 7 second(s).
+2024-05-11 00:56:32.452883:   No backends available. Exiting.
+2024-05-11 00:56:32.453891:   Soonest Retry After: oai-eastus-20240509.openai.azure.com - 4 second(s)
+2024-05-11 00:56:38.551672:   Backend oai-eastus-20240509.openai.azure.com is no longer throttling.
+2024-05-11 00:56:39.851076:   Request sent to server: https://oai-eastus-20240509.openai.azure.com/openai/deployments/gpt-35-turbo-sjk-001/chat/completions?api-version=2024-04-01-preview, Status code: 200
+```
```

