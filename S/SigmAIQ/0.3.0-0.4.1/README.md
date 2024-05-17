# Comparing `tmp/sigmaiq-0.3.0.tar.gz` & `tmp/sigmaiq-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaiq-0.3.0.tar", max compression
+gzip compressed data, was "sigmaiq-0.4.1.tar", max compression
```

## Comparing `sigmaiq-0.3.0.tar` & `sigmaiq-0.4.1.tar`

### file list

```diff
@@ -1,56 +1,58 @@
--rw-r--r--   0        0        0    26526 2023-11-17 21:32:10.321670 sigmaiq-0.3.0/LICENSE
--rw-r--r--   0        0        0    24187 2023-11-17 21:32:10.321670 sigmaiq-0.3.0/README.md
--rw-r--r--   0        0        0     1683 2023-11-17 21:32:10.321670 sigmaiq-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2964 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/.gitignore
--rw-r--r--   0        0        0      131 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/__init__.py
--rw-r--r--   0        0        0        0 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/__init__.py
--rw-r--r--   0        0        0       51 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/carbonblack/__init__.py
--rw-r--r--   0        0        0      781 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/carbonblack/carbonblack.py
--rw-r--r--   0        0        0       47 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/cortexxdr/__init__.py
--rw-r--r--   0        0        0      732 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/cortexxdr/cortexxdr.py
--rw-r--r--   0        0        0       57 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/crowdstrike/__init__.py
--rw-r--r--   0        0        0      393 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/crowdstrike/crowdstrike.py
--rw-r--r--   0        0        0       55 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/elasticsearch/__init__.py
--rw-r--r--   0        0        0      407 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/elasticsearch/elasticsearch.py
--rw-r--r--   0        0        0       49 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/insightidr/__init__.py
--rw-r--r--   0        0        0      337 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/insightidr/insightidr.py
--rw-r--r--   0        0        0       37 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/loki/__init__.py
--rw-r--r--   0        0        0      380 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/loki/loki.py
--rw-r--r--   0        0        0       69 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/microsoft365defender/__init__.py
--rw-r--r--   0        0        0      396 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/microsoft365defender/microsoft365defender.py
--rw-r--r--   0        0        0       49 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/opensearch/__init__.py
--rw-r--r--   0        0        0      489 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/opensearch/opensearch.py
--rw-r--r--   0        0        0       41 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/qradar/__init__.py
--rw-r--r--   0        0        0      470 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/qradar/qradar.py
--rw-r--r--   0        0        0       51 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/sentinelone/__init__.py
--rw-r--r--   0        0        0      789 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/sentinelone/sentinelone.py
--rw-r--r--   0        0        0       39 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/sigma/__init__.py
--rw-r--r--   0        0        0     3484 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/sigma/sigma.py
--rw-r--r--   0        0        0    10128 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/sigmaiq_abstract_backend.py
--rw-r--r--   0        0        0       41 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/splunk/__init__.py
--rw-r--r--   0        0        0     1557 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/splunk/savedsearches_template.txt
--rw-r--r--   0        0        0     3082 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/splunk/splunk.py
--rw-r--r--   0        0        0       37 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/stix/__init__.py
--rw-r--r--   0        0        0      410 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/backends/stix/stix.py
--rw-r--r--   0        0        0     1327 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/exceptions.py
--rw-r--r--   0        0        0      218 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/globals.py
--rw-r--r--   0        0        0     6341 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/README.md
--rw-r--r--   0        0        0        0 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/__init__.py
--rw-r--r--   0        0        0     8189 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/base.py
--rw-r--r--   0        0        0        0 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/toolkits/__init__.py
--rw-r--r--   0        0        0     5861 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/toolkits/base.py
--rw-r--r--   0        0        0     1125 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/toolkits/prompts.py
--rw-r--r--   0        0        0      881 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/toolkits/sigma_toolkit.py
--rw-r--r--   0        0        0        0 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/tools/__init__.py
--rw-r--r--   0        0        0     4537 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/tools/create_sigma_rule.py
--rw-r--r--   0        0        0     4132 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/llm/tools/translate_sigma_rule.py
--rw-r--r--   0        0        0        0 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/pipelines/__init__.py
--rw-r--r--   0        0        0      134 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/pipelines/splunk_windows_audit/__init__.py
--rw-r--r--   0        0        0      794 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py
--rw-r--r--   0        0        0    11483 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/sigmaiq_backend_factory.py
--rw-r--r--   0        0        0    17599 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/sigmaiq_pipeline_factory.py
--rw-r--r--   0        0        0        0 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/utils/sigma/__init__.py
--rw-r--r--   0        0        0     6386 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/utils/sigma/rule_updater.py
--rw-r--r--   0        0        0        0 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/utils/sigmaiq/__init__.py
--rw-r--r--   0        0        0     1905 2023-11-17 21:32:10.325671 sigmaiq-0.3.0/sigmaiq/utils/sigmaiq/sigmaiq_utils.py
--rw-r--r--   0        0        0    25746 1970-01-01 00:00:00.000000 sigmaiq-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2024-05-17 17:36:40.934271 sigmaiq-0.4.1/LICENSE
+-rw-r--r--   0        0        0    24187 2024-05-17 17:36:40.934271 sigmaiq-0.4.1/README.md
+-rw-r--r--   0        0        0     1904 2024-05-17 17:36:40.934271 sigmaiq-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2964 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/.gitignore
+-rw-r--r--   0        0        0      131 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/carbonblack/__init__.py
+-rw-r--r--   0        0        0      781 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/carbonblack/carbonblack.py
+-rw-r--r--   0        0        0       47 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/cortexxdr/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/cortexxdr/cortexxdr.py
+-rw-r--r--   0        0        0       57 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/crowdstrike/__init__.py
+-rw-r--r--   0        0        0      393 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/crowdstrike/crowdstrike.py
+-rw-r--r--   0        0        0       55 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/elasticsearch/elasticsearch.py
+-rw-r--r--   0        0        0       49 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/insightidr/__init__.py
+-rw-r--r--   0        0        0      337 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/insightidr/insightidr.py
+-rw-r--r--   0        0        0       37 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/loki/__init__.py
+-rw-r--r--   0        0        0      380 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/loki/loki.py
+-rw-r--r--   0        0        0       69 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/microsoft365defender/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/microsoft365defender/microsoft365defender.py
+-rw-r--r--   0        0        0       49 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/opensearch/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/opensearch/opensearch.py
+-rw-r--r--   0        0        0       41 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/qradar/__init__.py
+-rw-r--r--   0        0        0      470 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/qradar/qradar.py
+-rw-r--r--   0        0        0       51 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/sentinelone/__init__.py
+-rw-r--r--   0        0        0      789 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/sentinelone/sentinelone.py
+-rw-r--r--   0        0        0       39 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/sigma/__init__.py
+-rw-r--r--   0        0        0     3484 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/sigma/sigma.py
+-rw-r--r--   0        0        0    10128 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/sigmaiq_abstract_backend.py
+-rw-r--r--   0        0        0       41 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/splunk/__init__.py
+-rw-r--r--   0        0        0     1557 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/splunk/savedsearches_template.txt
+-rw-r--r--   0        0        0     3082 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/splunk/splunk.py
+-rw-r--r--   0        0        0       37 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/stix/__init__.py
+-rw-r--r--   0        0        0      410 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/backends/stix/stix.py
+-rw-r--r--   0        0        0     1327 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/exceptions.py
+-rw-r--r--   0        0        0      218 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/globals.py
+-rw-r--r--   0        0        0     6385 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/__init__.py
+-rw-r--r--   0        0        0     8189 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/base.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/toolkits/__init__.py
+-rw-r--r--   0        0        0     5833 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/toolkits/base.py
+-rw-r--r--   0        0        0     1325 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/toolkits/prompts.py
+-rw-r--r--   0        0        0     1159 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/toolkits/sigma_toolkit.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/tools/__init__.py
+-rw-r--r--   0        0        0     6104 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/tools/create_sigma_rule.py
+-rw-r--r--   0        0        0     3368 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/tools/find_sigma_rule.py
+-rw-r--r--   0        0        0     5132 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/tools/query_to_sigma_rule.py
+-rw-r--r--   0        0        0     4133 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/llm/tools/translate_sigma_rule.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/pipelines/__init__.py
+-rw-r--r--   0        0        0      134 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/pipelines/splunk_windows_audit/__init__.py
+-rw-r--r--   0        0        0      794 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py
+-rw-r--r--   0        0        0    11483 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/sigmaiq_backend_factory.py
+-rw-r--r--   0        0        0    17599 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/sigmaiq_pipeline_factory.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/utils/sigma/__init__.py
+-rw-r--r--   0        0        0     6386 2024-05-17 17:36:40.938271 sigmaiq-0.4.1/sigmaiq/utils/sigma/rule_updater.py
+-rw-r--r--   0        0        0        0 2024-05-17 17:36:40.942271 sigmaiq-0.4.1/sigmaiq/utils/sigmaiq/__init__.py
+-rw-r--r--   0        0        0     1905 2024-05-17 17:36:40.942271 sigmaiq-0.4.1/sigmaiq/utils/sigmaiq/sigmaiq_utils.py
+-rw-r--r--   0        0        0    25767 1970-01-01 00:00:00.000000 sigmaiq-0.4.1/PKG-INFO
```

### Comparing `sigmaiq-0.3.0/LICENSE` & `sigmaiq-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/README.md` & `sigmaiq-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/pyproject.toml` & `sigmaiq-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SigmAIQ"
-version = "0.3.0"
+version = "0.4.1"
 description = "Wrapper and tools for pySigma and Sigma rules"
 authors = ["Stephen Lincoln <stephen.lincoln@attackiq.com>", "AttackIQ <support@attackiq.com>"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)",
@@ -16,47 +16,59 @@
 ]
 
 packages = [
     { include = "sigmaiq" }
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1, <=3.11.6"
-pysigma = "0.9.11"
-certifi = "^2023.07.22"
-pysigma-backend-carbonblack = "0.1.4"
-pysigma-backend-cortexxdr = "0.1.1"
-pysigma-backend-elasticsearch = "1.0.5"
-pysigma-backend-insightidr = "0.2.1"
-pysigma-backend-loki = "0.9.1"
-pysigma-backend-microsoft365defender = "0.2.1"
-pysigma-backend-opensearch = "1.0.0"
-pysigma-backend-qradar-aql = "0.2.3"
-pysigma-backend-sentinelone = "0.1.2"
-pysigma-backend-splunk = "1.0.2"
-pysigma-backend-stix = "0.1.8"
-pysigma-pipeline-crowdstrike = "1.0.0"
-pysigma-pipeline-sysmon = "1.0.2"
-pysigma-pipeline-windows = "1.1.0"
+python = ">=3.8.1, <=3.11.9"
+pysigma = "0.10.10"
+certifi = ">=2023.7.22"
+pysigma-backend-carbonblack = "^0.1.6"
+pysigma-backend-cortexxdr = "0.1.2"
+pysigma-backend-elasticsearch = "1.0.10"
+pysigma-backend-insightidr = "0.2.2"
+pysigma-backend-loki = "0.10.3"
+pysigma-backend-microsoft365defender = "0.2.6"
+pysigma-backend-opensearch = "1.0.1"
+pysigma-backend-qradar-aql = "^0.3.2"
+pysigma-backend-sentinelone = "^0.1.3"
+pysigma-backend-splunk = "1.0.3"
+pysigma-backend-stix2 = "^0.2.0"
+pysigma-pipeline-crowdstrike = "1.0.1"
+pysigma-pipeline-sysmon = "1.0.3"
+pysigma-pipeline-windows = "1.1.1"
 importlib-resources = "^5.13.0"
 
-[tool.poetry.dev-dependencies]
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
-black = "^23.7.0"
-ruff = "^0.0.286"
-
 [tool.poetry.group.llm]
 optional = true
 
 [tool.poetry.group.llm.dependencies]
+aiohttp = "^3.9.4"
 langchain = "^0.0.335"
 openai = "^1.2.4"
 tiktoken = "^0.5.1"
 faiss-cpu = "^1.7.4"
 
+
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+black = "^24.4.2"
+ruff = "^0.0.286"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 120
+line-length = 120
+
+[tool.coverage.run]
+omit = [
+    # omit anything in a tests directory
+    "tests/*",
+    # omit everything in LLM
+    "sigmaiq/llm/*",
+    # omit globals
+    "sigmaiq/globals.py",
+    ]
```

### Comparing `sigmaiq-0.3.0/sigmaiq/.gitignore` & `sigmaiq-0.4.1/sigmaiq/.gitignore`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/backends/carbonblack/carbonblack.py` & `sigmaiq-0.4.1/sigmaiq/backends/carbonblack/carbonblack.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/backends/cortexxdr/cortexxdr.py` & `sigmaiq-0.4.1/sigmaiq/backends/cortexxdr/cortexxdr.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/backends/sentinelone/sentinelone.py` & `sigmaiq-0.4.1/sigmaiq/backends/sentinelone/sentinelone.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/backends/sigma/sigma.py` & `sigmaiq-0.4.1/sigmaiq/backends/sigma/sigma.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/backends/sigmaiq_abstract_backend.py` & `sigmaiq-0.4.1/sigmaiq/backends/sigmaiq_abstract_backend.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/backends/splunk/savedsearches_template.txt` & `sigmaiq-0.4.1/sigmaiq/backends/splunk/savedsearches_template.txt`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/backends/splunk/splunk.py` & `sigmaiq-0.4.1/sigmaiq/backends/splunk/splunk.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/exceptions.py` & `sigmaiq-0.4.1/sigmaiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/llm/README.md` & `sigmaiq-0.4.1/sigmaiq/llm/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 The goal of this SigmAIQ feature is to utilize the power of LLMs and Vector Databases with Sigma Rules.  
 This feature uses [langchain](https://github.com/langchain-ai/langchain) and [pySigma](https://github.com/SigmaHQ/pySigma)
 to utilize LLMs and Agents for Sigma Rule translation and creation.
 Currently, the use cases of this feature include:
 - Embedding creation and storage of Sigma Rules
 - Sigma Rule similarity searching
 - Agent/Bot for Sigma Rule translation and creation
+- Converting backend queries to Sigma Rules
 
 Please see the `examples` folder for use case examples.
 
 ### Embedding Creation and Storage
 The `sigmaiq.llm.base.SigmaLLM` class is used to automatically download the latest Sigma Rules from the [SigmaHQ](https://github.com/SigmaHQ/sigma/releases/latest) repo. 
 By default, this downloads the `sigma_core` ruleset into this projects `data` directory.  Embeddings are then created for each rule and stored in a Vector Database.
 By default, `OpenAIEmbeddings` and `FAISS` are used, respectively.  The `sigmaiq.llm.base.SigmaLLM` class can be extended to use different embedding and vector database implementations.
```

#### html2text {}

```diff
@@ -5,23 +5,24 @@
 models (gpt-3.5-turbo) are used, which require an OpenAI API key set in the
 environmental variable `OPENAI_API_KEY`. ## Overview The goal of this SigmAIQ
 feature is to utilize the power of LLMs and Vector Databases with Sigma Rules.
 This feature uses [langchain](https://github.com/langchain-ai/langchain) and
 [pySigma](https://github.com/SigmaHQ/pySigma) to utilize LLMs and Agents for
 Sigma Rule translation and creation. Currently, the use cases of this feature
 include: - Embedding creation and storage of Sigma Rules - Sigma Rule
-similarity searching - Agent/Bot for Sigma Rule translation and creation Please
-see the `examples` folder for use case examples. ### Embedding Creation and
-Storage The `sigmaiq.llm.base.SigmaLLM` class is used to automatically download
-the latest Sigma Rules from the [SigmaHQ](https://github.com/SigmaHQ/sigma/
-releases/latest) repo. By default, this downloads the `sigma_core` ruleset into
-this projects `data` directory. Embeddings are then created for each rule and
-stored in a Vector Database. By default, `OpenAIEmbeddings` and `FAISS` are
-used, respectively. The `sigmaiq.llm.base.SigmaLLM` class can be extended to
-use different embedding and vector database implementations. ### Sigma Rule
+similarity searching - Agent/Bot for Sigma Rule translation and creation -
+Converting backend queries to Sigma Rules Please see the `examples` folder for
+use case examples. ### Embedding Creation and Storage The
+`sigmaiq.llm.base.SigmaLLM` class is used to automatically download the latest
+Sigma Rules from the [SigmaHQ](https://github.com/SigmaHQ/sigma/releases/
+latest) repo. By default, this downloads the `sigma_core` ruleset into this
+projects `data` directory. Embeddings are then created for each rule and stored
+in a Vector Database. By default, `OpenAIEmbeddings` and `FAISS` are used,
+respectively. The `sigmaiq.llm.base.SigmaLLM` class can be extended to use
+different embedding and vector database implementations. ### Sigma Rule
 Similarity Searching The `sigmaiq.llm.base.SigmaLLM` class is also used to
 search for similar Sigma Rules using a similarity search. This does not require
 LLM models to be trained, as the embeddings are already created and stored in
 the Vector Database. This can be a cheaper, yet less accurate option, for
 searching through Sigma Rules. By default, the top 3 matching rules are
 returned based on the query sent to the similarity search. Other `langchain`
 `VectorStore` searching functionality can be used on the VectorStore as well.
```

### Comparing `sigmaiq-0.3.0/sigmaiq/llm/base.py` & `sigmaiq-0.4.1/sigmaiq/llm/base.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/llm/toolkits/base.py` & `sigmaiq-0.4.1/sigmaiq/llm/toolkits/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 
 # sigmaiq
 from sigmaiq.llm.toolkits.sigma_toolkit import SigmaToolkit
 from sigmaiq.llm.toolkits.prompts import SIGMA_AGENT_PROMPT
 
 
 def create_sigma_agent(
-    agent_llm: BaseLanguageModel = ChatOpenAI(model="gpt-3.5-turbo"),
-    rule_creation_llm: BaseLanguageModel = ChatOpenAI(model="gpt-3.5-turbo"),
+    agent_llm: BaseLanguageModel = ChatOpenAI(model="gpt-4o"),
+    rule_creation_llm: BaseLanguageModel = ChatOpenAI(model="gpt-4o"),
     sigma_vectorstore: VectorStore = None,
     toolkit: Type[SigmaToolkit] = SigmaToolkit,
     prompt: Optional[ChatPromptTemplate] = SIGMA_AGENT_PROMPT,
     verbose: bool = False,
     return_intermediate_steps: bool = False,
     agent_executor_kwargs: Optional[Dict[str, Any]] = None,
 ) -> AgentExecutor:
     """Construct a Sigma agent from an LLM and tools.
 
     Args:
-        agent_llm (BaseLanguageModel, optional): The LLM to use for the agent. Defaults to ChatOpenAI(model="gpt-3.5-turbo").
-        rule_creation_llm (BaseLanguageModel, optional): The LLM to use for the rule creation tool. Defaults to ChatOpenAI(model="gpt-3.5-turbo").
+        agent_llm (BaseLanguageModel, optional): The LLM to use for the agent. Defaults to ChatOpenAI(model="gpt-4o").
+        rule_creation_llm (BaseLanguageModel, optional): The LLM to use for the rule creation tool. Defaults to ChatOpenAI(model="gpt-4o").
         sigma_vectorstore (VectorStore, optional): The vectorstore containing Sigma rules to use for the agent. Defaults to None.
         toolkit (Type[SigmaToolkit], optional): The toolkit to use for the agent. Defaults to SigmaToolkit.
         prompt (Optional[ChatPromptTemplate], optional): The prompt to use for the agent. Defaults to SIGMA_AGENT_PROMPT.
         verbose (bool, optional): Whether to print verbose output. Defaults to False.
         return_intermediate_steps (bool, optional): Whether to return intermediate steps. Defaults to False.
         agent_executor_kwargs (Optional[Dict[str, Any]], optional): Additional kwargs to pass to the AgentExecutor. Defaults to None.
```

### Comparing `sigmaiq-0.3.0/sigmaiq/llm/toolkits/prompts.py` & `sigmaiq-0.4.1/sigmaiq/llm/toolkits/prompts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from langchain.prompts import ChatPromptTemplate, MessagesPlaceholder
 
 # Default prompts for Sigma agents
 SIGMA_AGENT_PROMPT = prompt = ChatPromptTemplate.from_messages(
     [
         (
             "system",
-            "You are a threat detection engineering assistant bot specializing in Sigma rules."
-            "You have two tools at your disposal: translate_sigma_rule and create_sigma_rule_vectorstore."
-            "translate_sigma_rule will convert or translate a Sigma Rule into a query for a specific backend."
-            "create_sigma_rule_vectorstore will take the users input, find similar Sigma Rules from the vectorstore,"
-            "then create a brand new Sigma Rule based on the users input and the similar Sigma Rules returned from the vectorstore"
-            "to use as context. The output is a Sigma Rule in YAML format. Do not use 'translate_sigma_rule' unless "
-            "the user explicitly asks for a Sigma Rule to be converted or translated into a query for a specific backend.",
+            "You are a threat detection engineering assistant bot specializing in Sigma Rules."
+            "You have four tools at your disposal: "
+            "1. translate_sigma_rule: converts or translates a Sigma Rule into a query for a specific backend/product."
+            "2. find_sigma_rule: Searches for a Sigma Rule in the vector database based on the users question."
+            "3. create_sigma_rule_vectorstore: Creates new Sigma Rule from the users input, as well as rules in a sigma rule vectorstore to use as context based on the users question. If the user's question already contains a query, use 'query_to_sigma_rule' instead."
+            "4. query_to_sigma_rule: Converts/translates a product/SIEM/backend query or search from the query language into a YAML Sigma Rule."
+            "Do not use 'translate_sigma_rule' unless the user explicitly asks for a Sigma Rule to be converted or translated "
+            "into a query for a specific backend, pipeline, and/or output format."
         ),
         ("user", "{input}"),
         MessagesPlaceholder(variable_name="agent_scratchpad"),
     ]
 )
```

### Comparing `sigmaiq-0.3.0/sigmaiq/llm/toolkits/sigma_toolkit.py` & `sigmaiq-0.4.1/sigmaiq/llm/toolkits/sigma_toolkit.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,24 +8,28 @@
 # langchain typing
 from langchain.schema.language_model import BaseLanguageModel
 from langchain.schema.vectorstore import VectorStore
 
 # sigmaiq tools
 from sigmaiq.llm.tools.create_sigma_rule import CreateSigmaRuleVectorStoreTool
 from sigmaiq.llm.tools.translate_sigma_rule import TranslateSigmaRuleTool
+from sigmaiq.llm.tools.find_sigma_rule import FindSigmaRuleTool
+from sigmaiq.llm.tools.query_to_sigma_rule import QueryToSigmaRuleTool
 
 
 class SigmaToolkit(BaseToolkit):
     """Sigma Toolkit."""
 
     sigmadb: VectorStore
     rule_creation_llm: BaseLanguageModel
 
     class Config:
         arbitrary_types_allowed = True
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return [
+            FindSigmaRuleTool(sigmadb=self.sigmadb, llm=self.rule_creation_llm),
             TranslateSigmaRuleTool(),
             CreateSigmaRuleVectorStoreTool(sigmadb=self.sigmadb, llm=self.rule_creation_llm),
+            QueryToSigmaRuleTool(llm=self.rule_creation_llm),
         ]
```

### Comparing `sigmaiq-0.3.0/sigmaiq/llm/tools/create_sigma_rule.py` & `sigmaiq-0.4.1/sigmaiq/llm/tools/query_to_sigma_rule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,119 @@
-# stdlib
-from typing import Type, Optional
+import json
+from typing import Union, Type, Optional
 
-# langchain
 from langchain.callbacks.manager import CallbackManagerForToolRun
 from langchain.prompts import ChatPromptTemplate
-from langchain.tools import BaseTool
-from langchain.pydantic_v1 import BaseModel, Field
-
-# langchain typing
 from langchain.schema.language_model import BaseLanguageModel
-from langchain.schema.runnable import RunnablePassthrough
 from langchain.schema.output_parser import StrOutputParser
-from langchain.schema.vectorstore import VectorStore
+from langchain.schema.runnable import RunnablePassthrough
+from langchain.tools import BaseTool
+from pydantic import BaseModel, Field, Extra
 
+from sigmaiq.sigmaiq_backend_factory import AVAILABLE_BACKENDS, SigmAIQBackend
 
-class CreateSigmaRuleInput(BaseModel):
-    """Input for TranslateSigmaRule tool, which uses SigmAIQ backend factory to convert a Sigma Rule into
-    a query for a specific backend."""
 
-    query: str = Field(
-        description="The users question, used to search through the Sigma VectorStore and create a Sigma Rule."
-    )
+class QueryToSigmaRuleInput(BaseModel):
+    """Input for QueryToSigmaRule tool, which converts a backend query to a Sigma Rule, and
+    uses SigmAIQ backend factory for validation.
+    """
 
-    class Config(BaseTool.Config):
-        pass
+    query: Union[str, dict] = Field(
+        default=None,
+        description="""A query string for a backend, which should be converted to a Sigma Rule YAML string."""
+    )
+    backend: str = Field(
+        default=None,
+        description="""The backend that the query is for, and what should be used for validation. Backend options their descriptions are as 
+        follows:\n"""
+        + f"{json.dumps(AVAILABLE_BACKENDS, indent=2)}",
+    )
 
 
-class CreateSigmaRuleVectorStoreTool(BaseTool):
-    """Class for translating Sigma rules via SigmAIQ Backend Factory"""
+class QueryToSigmaRuleTool(BaseTool):
+    """Class for converting a backend query to a Sigma Rule"""
 
-    name: str = "create_sigma_rule_vectorstore"
-    args_schema: Type[BaseModel] = CreateSigmaRuleInput
-    description: str = """Use this tool to take the users input, find similar Sigma Rules from the vectorstore,
-    then create a brand new Sigma Rule based on the users input and the similar Sigma Rules returned from the vectorstore
-    to use as context. The output is a Sigma Rule in YAML format.
-    """
-    sigmadb: VectorStore
+    name: str = "query_to_sigma_rule"
+    args_schema: Type[BaseModel] = QueryToSigmaRuleInput
+    description: str = """
+        Use this tool to take an already existing query for a backend and convert it to a Sigma Rule.
+        Use the translate_sigma_rule tool to take the created Sigma Rule and convert it back to a query to 
+        determine if the queries are the same and the conversion is successful. Fix any errors if necessary.
+        The input must be a query string for a backend, and the backend must be specified.
+        The output is a Sigma Rule YAML string, or an error message if the conversion fails.
+        """
+    # return_direct = True  # We don't need an agent LLM to think about the output, it is what it is.
     llm: BaseLanguageModel
-    k: int = 3
-    verbose = True
+    verbose = False
+
+    class Config:
+        """Configuration for this pydantic object."""
+
+        extra = Extra.forbid
 
     def _run(
         self,
-        query: str,
+        query: str = None,
+        backend: str = None,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
-        """Run the tool"""
-
         template = """You are a cybersecurity detection engineering assistant bot specializing in Sigma Rule creation.
-                You are assisting a user in creating a new Sigma Rule based on the users question.  
-                The users question is first used to find similar Sigma Rules from the a vectorstore containing official 
-                Sigma Rules. The official Sigma Rules should be used as context as needed in conjunction with the detection specified
-                in the users question to create a new Sigma Rule. Set the 'author' to 'SigmAIQ (AttackIQ)', 
-                the date to today's date, and the reference to 'https://github.com/AttackIQ/SigmAIQ'.  
-                The created Sigma Rule should be in YAML format and use the official Sigma schema.  The detection field
-                can contain multiple 'selection' identifiers and multiple 'filter' identifiers as needed, 
-                which can be used in the condition field to select criteria and filter out criteria respectively.
-
-                Sigma Rule Schema:
-                
-                title
-                id [optional]
-                related [optional]
-                   - id {{rule-id}}
-                     type {{type-identifier}}
-                status [optional]
-                description [optional]
-                references [optional]
-                author [optional]
-                date [optional]
-                modified [optional]
-                tags [optional]
-                logsource
-                   category [optional]
-                   product [optional]
-                   service [optional]
-                   definition [optional]
-                   ...
-                detection
-                   {{search-identifier}} [optional]
-                      {{string-list}} [optional]
-                      {{map-list}} [optional]
-                      {{field: valu}}> [optional]
-                   ... # Multiple search identifiers can be specified as needed and used in the condition
-                   condition
-                fields [optional]
-                falsepositives [optional]
-                level [optional]:
-                -------
-                Vectorstore Search Results:
-
-                {context}
-                ------
-                User's Question: 
-                {question}
-                """
+                    You are assisting a user in taking a query for a security/SIEM product, and converting it to a Sigma Rule.
+                    The backend is used to validate the query and ensure it is compatible with the backend.
+                    The created Sigma Rule should be in YAML format and use the official Sigma schema.  The detection field
+                    can contain multiple 'selection' identifiers and multiple 'filter' identifiers as needed, 
+                    which can be used in the condition field to select criteria and filter out criteria respectively.  
+                    The fields should be Sysmon field names if possible, or Windows Event Log field names if possible.  
+    
+                    -----------
+                    
+                    Sigma Rule Schema:
+    
+                    title
+                    id [optional]
+                    related [optional]
+                       - id {{rule-id}}
+                         type {{type-identifier}}
+                    status [optional]
+                    description [optional]
+                    references [optional]
+                    author [optional]
+                    date [optional]
+                    modified [optional]
+                    tags [optional]
+                    logsource
+                       category [optional]
+                       product [optional]
+                       service [optional]
+                       definition [optional]
+                       ...
+                    detection
+                       {{search-identifier}} [optional]
+                          {{string-list}} [optional]
+                          {{map-list}} [optional]
+                          {{field: valu}}> [optional]
+                       ... # Multiple search identifiers can be specified as needed and used in the condition
+                       condition
+                    fields [optional]
+                    falsepositives [optional]
+                    level [optional]:
+                    
+                    -----------
+                    
+                    User's Question: 
+                    {question}
+                    """
 
         prompt = ChatPromptTemplate.from_template(template)
-        retriever = self.sigmadb.as_retriever(search_kwargs={"k": self.k})
-        chain = {"context": retriever, "question": RunnablePassthrough()} | prompt | self.llm | StrOutputParser()
+        chain = {"question": RunnablePassthrough()} | prompt | self.llm | StrOutputParser()
         return chain.invoke(query)
 
     async def _arun(
         self,
-        query: str,
-        k: int,
+        sigma_rule: Union[str, dict] = None,
+        backend: str = None,
+        processing_pipeline: str = None,
+        output_format: str = "default",
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         """Async run the tool"""
         raise NotImplementedError
```

### Comparing `sigmaiq-0.3.0/sigmaiq/llm/tools/translate_sigma_rule.py` & `sigmaiq-0.4.1/sigmaiq/llm/tools/translate_sigma_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         The input must be a Sigma Rule, which can be provided as a YAML string or dict object.
         Additionally, the backend (product) must be specified, and the processing pipeline and output format can be 
         optionally specified.
         The output is json of the translated rule to a query for the backend, or an error message if the 
         translation fails.
         """
     # return_direct = True  # We don't need an agent LLM to think about the output, it is what it is.
-    verbose = True
+    verbose = False
 
     class Config:
         """Configuration for this pydantic object."""
 
         extra = Extra.forbid
 
     def _run(
```

### Comparing `sigmaiq-0.3.0/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py` & `sigmaiq-0.4.1/sigmaiq/pipelines/splunk_windows_audit/splunk_wineventlog.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/sigmaiq_backend_factory.py` & `sigmaiq-0.4.1/sigmaiq/sigmaiq_backend_factory.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/sigmaiq_pipeline_factory.py` & `sigmaiq-0.4.1/sigmaiq/sigmaiq_pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/utils/sigma/rule_updater.py` & `sigmaiq-0.4.1/sigmaiq/utils/sigma/rule_updater.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/sigmaiq/utils/sigmaiq/sigmaiq_utils.py` & `sigmaiq-0.4.1/sigmaiq/utils/sigmaiq/sigmaiq_utils.py`

 * *Files identical despite different names*

### Comparing `sigmaiq-0.3.0/PKG-INFO` & `sigmaiq-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: SigmAIQ
-Version: 0.3.0
+Version: 0.4.1
 Summary: Wrapper and tools for pySigma and Sigma rules
 Author: Stephen Lincoln
 Author-email: stephen.lincoln@attackiq.com
-Requires-Python: >=3.8.1,<=3.11.6
+Requires-Python: >=3.8.1,<=3.11.9
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Security
-Requires-Dist: certifi (>=2023.07.22,<2024.0.0)
+Requires-Dist: certifi (>=2023.7.22)
 Requires-Dist: importlib-resources (>=5.13.0,<6.0.0)
-Requires-Dist: pysigma (==0.9.11)
-Requires-Dist: pysigma-backend-carbonblack (==0.1.4)
-Requires-Dist: pysigma-backend-cortexxdr (==0.1.1)
-Requires-Dist: pysigma-backend-elasticsearch (==1.0.5)
-Requires-Dist: pysigma-backend-insightidr (==0.2.1)
-Requires-Dist: pysigma-backend-loki (==0.9.1)
-Requires-Dist: pysigma-backend-microsoft365defender (==0.2.1)
-Requires-Dist: pysigma-backend-opensearch (==1.0.0)
-Requires-Dist: pysigma-backend-qradar-aql (==0.2.3)
-Requires-Dist: pysigma-backend-sentinelone (==0.1.2)
-Requires-Dist: pysigma-backend-splunk (==1.0.2)
-Requires-Dist: pysigma-backend-stix (==0.1.8)
-Requires-Dist: pysigma-pipeline-crowdstrike (==1.0.0)
-Requires-Dist: pysigma-pipeline-sysmon (==1.0.2)
-Requires-Dist: pysigma-pipeline-windows (==1.1.0)
+Requires-Dist: pysigma (==0.10.10)
+Requires-Dist: pysigma-backend-carbonblack (>=0.1.6,<0.2.0)
+Requires-Dist: pysigma-backend-cortexxdr (==0.1.2)
+Requires-Dist: pysigma-backend-elasticsearch (==1.0.10)
+Requires-Dist: pysigma-backend-insightidr (==0.2.2)
+Requires-Dist: pysigma-backend-loki (==0.10.3)
+Requires-Dist: pysigma-backend-microsoft365defender (==0.2.6)
+Requires-Dist: pysigma-backend-opensearch (==1.0.1)
+Requires-Dist: pysigma-backend-qradar-aql (>=0.3.2,<0.4.0)
+Requires-Dist: pysigma-backend-sentinelone (>=0.1.3,<0.2.0)
+Requires-Dist: pysigma-backend-splunk (==1.0.3)
+Requires-Dist: pysigma-backend-stix2 (>=0.2.0,<0.3.0)
+Requires-Dist: pysigma-pipeline-crowdstrike (==1.0.1)
+Requires-Dist: pysigma-pipeline-sysmon (==1.0.3)
+Requires-Dist: pysigma-pipeline-windows (==1.1.1)
 Description-Content-Type: text/markdown
 
 <div align="center">
     <a href="https://www.attackiq.com" target="_blank">
         <img src="https://www.attackiq.com/wp-content/uploads/2021/10/col-dflt.png" height="300" alt="AttackIQ">
     </a>
 </div>
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: SigmAIQ Version: 0.3.0 Summary: Wrapper and tools
+Metadata-Version: 2.1 Name: SigmAIQ Version: 0.4.1 Summary: Wrapper and tools
 for pySigma and Sigma rules Author: Stephen Lincoln Author-email:
-stephen.lincoln@attackiq.com Requires-Python: >=3.8.1,<=3.11.6 Classifier:
+stephen.lincoln@attackiq.com Requires-Python: >=3.8.1,<=3.11.9 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2
 (LGPLv2) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Topic :: Security Requires-
-Dist: certifi (>=2023.07.22,<2024.0.0) Requires-Dist: importlib-resources
-(>=5.13.0,<6.0.0) Requires-Dist: pysigma (==0.9.11) Requires-Dist: pysigma-
-backend-carbonblack (==0.1.4) Requires-Dist: pysigma-backend-cortexxdr
-(==0.1.1) Requires-Dist: pysigma-backend-elasticsearch (==1.0.5) Requires-Dist:
-pysigma-backend-insightidr (==0.2.1) Requires-Dist: pysigma-backend-loki
-(==0.9.1) Requires-Dist: pysigma-backend-microsoft365defender (==0.2.1)
-Requires-Dist: pysigma-backend-opensearch (==1.0.0) Requires-Dist: pysigma-
-backend-qradar-aql (==0.2.3) Requires-Dist: pysigma-backend-sentinelone
-(==0.1.2) Requires-Dist: pysigma-backend-splunk (==1.0.2) Requires-Dist:
-pysigma-backend-stix (==0.1.8) Requires-Dist: pysigma-pipeline-crowdstrike
-(==1.0.0) Requires-Dist: pysigma-pipeline-sysmon (==1.0.2) Requires-Dist:
-pysigma-pipeline-windows (==1.1.0) Description-Content-Type: text/markdown
+Dist: certifi (>=2023.7.22) Requires-Dist: importlib-resources
+(>=5.13.0,<6.0.0) Requires-Dist: pysigma (==0.10.10) Requires-Dist: pysigma-
+backend-carbonblack (>=0.1.6,<0.2.0) Requires-Dist: pysigma-backend-cortexxdr
+(==0.1.2) Requires-Dist: pysigma-backend-elasticsearch (==1.0.10) Requires-
+Dist: pysigma-backend-insightidr (==0.2.2) Requires-Dist: pysigma-backend-loki
+(==0.10.3) Requires-Dist: pysigma-backend-microsoft365defender (==0.2.6)
+Requires-Dist: pysigma-backend-opensearch (==1.0.1) Requires-Dist: pysigma-
+backend-qradar-aql (>=0.3.2,<0.4.0) Requires-Dist: pysigma-backend-sentinelone
+(>=0.1.3,<0.2.0) Requires-Dist: pysigma-backend-splunk (==1.0.3) Requires-Dist:
+pysigma-backend-stix2 (>=0.2.0,<0.3.0) Requires-Dist: pysigma-pipeline-
+crowdstrike (==1.0.1) Requires-Dist: pysigma-pipeline-sysmon (==1.0.3)
+Requires-Dist: pysigma-pipeline-windows (==1.1.1) Description-Content-Type:
+text/markdown
                                   _[_A_t_t_a_c_k_I_Q_]
                 ************ SSiiggmmAAIIQQ:: ppyySSiiggmmaa WWrraappppeerr && UUttiillss ************
 ![Tests](https://github.com/AttackIQ/SigmAIQ/actions/workflows/test.yml/
 badge.svg) ![Coverage Badge](https://img.shields.io/endpoint?url=https://
 gist.githubusercontent.com/slincoln-aiq/f6d72f7ec2b300546a114fd80d371f7e/raw/
 slincoln-aiq-SigmAIQ.json) ![Status](https://img.shields.io/badge/Status-pre--
 release-orange) SigmAIQ is a wrapper for [pySigma](https://github.com/SigmaHQ/
```

