# Comparing `tmp/great_expectations_cloud-20240516.1.dev0.tar.gz` & `tmp/great_expectations_cloud-20240517.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_expectations_cloud-20240516.1.dev0.tar", max compression
+gzip compressed data, was "great_expectations_cloud-20240517.0.dev0.tar", max compression
```

## Comparing `great_expectations_cloud-20240516.1.dev0.tar` & `great_expectations_cloud-20240517.0.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     2084 2024-05-16 18:17:47.430803 great_expectations_cloud-20240516.1.dev0/LICENSE
--rw-r--r--   0        0        0     9760 2024-05-16 18:17:47.430803 great_expectations_cloud-20240516.1.dev0/README.md
--rw-r--r--   0        0        0      150 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/__init__.py
--rw-r--r--   0        0        0      244 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/__init__.py
--rw-r--r--   0        0        0      733 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/__init__.py
--rw-r--r--   0        0        0      763 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/agent_action.py
--rw-r--r--   0        0        0      316 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
--rw-r--r--   0        0        0     1511 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
--rw-r--r--   0        0        0     1503 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
--rw-r--r--   0        0        0     4279 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
--rw-r--r--   0        0        0     4171 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
--rw-r--r--   0        0        0     2881 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/list_table_names.py
--rw-r--r--   0        0        0     2041 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
--rw-r--r--   0        0        0     2993 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
--rw-r--r--   0        0        0      739 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/unknown.py
--rw-r--r--   0        0        0    17221 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/agent.py
--rw-r--r--   0        0        0      362 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/agent_warnings.py
--rw-r--r--   0        0        0     2851 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/cli.py
--rw-r--r--   0        0        0      858 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/config.py
--rw-r--r--   0        0        0      246 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/constants.py
--rw-r--r--   0        0        0     4632 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/event_handler.py
--rw-r--r--   0        0        0     1360 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/message_service/__init__.py
--rw-r--r--   0        0        0     9260 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
--rw-r--r--   0        0        0     5836 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/message_service/subscriber.py
--rw-r--r--   0        0        0     3562 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/models.py
--rw-r--r--   0        0        0      639 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/run.py
--rw-r--r--   0        0        0     1762 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/logging/README.md
--rw-r--r--   0        0        0     5918 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/logging/logging_cfg.py
--rw-r--r--   0        0        0     9543 2024-05-16 18:17:47.462803 great_expectations_cloud-20240516.1.dev0/pyproject.toml
--rw-r--r--   0        0        0    11114 1970-01-01 00:00:00.000000 great_expectations_cloud-20240516.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     2084 2024-05-17 14:29:51.794510 great_expectations_cloud-20240517.0.dev0/LICENSE
+-rw-r--r--   0        0        0     9758 2024-05-17 14:29:51.794510 great_expectations_cloud-20240517.0.dev0/README.md
+-rw-r--r--   0        0        0      150 2024-05-17 14:29:51.822510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-17 14:29:51.822510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-17 14:29:51.822510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/__init__.py
+-rw-r--r--   0        0        0      763 2024-05-17 14:29:51.822510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/agent_action.py
+-rw-r--r--   0        0        0      316 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/data_assistants/__init__.py
+-rw-r--r--   0        0        0     1511 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py
+-rw-r--r--   0        0        0     1503 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py
+-rw-r--r--   0        0        0     4279 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py
+-rw-r--r--   0        0        0     4171 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py
+-rw-r--r--   0        0        0     2881 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py
+-rw-r--r--   0        0        0     2041 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py
+-rw-r--r--   0        0        0     2993 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py
+-rw-r--r--   0        0        0      739 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/unknown.py
+-rw-r--r--   0        0        0    17221 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/agent.py
+-rw-r--r--   0        0        0      362 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/agent_warnings.py
+-rw-r--r--   0        0        0     2851 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/cli.py
+-rw-r--r--   0        0        0      858 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/config.py
+-rw-r--r--   0        0        0      246 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/constants.py
+-rw-r--r--   0        0        0     4632 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/event_handler.py
+-rw-r--r--   0        0        0     1360 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/message_service/__init__.py
+-rw-r--r--   0        0        0     9260 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py
+-rw-r--r--   0        0        0     5836 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py
+-rw-r--r--   0        0        0     3562 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/models.py
+-rw-r--r--   0        0        0      639 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/run.py
+-rw-r--r--   0        0        0     1762 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/logging/README.md
+-rw-r--r--   0        0        0     5918 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/logging/logging_cfg.py
+-rw-r--r--   0        0        0    10065 2024-05-17 14:29:51.826510 great_expectations_cloud-20240517.0.dev0/pyproject.toml
+-rw-r--r--   0        0        0    11112 1970-01-01 00:00:00.000000 great_expectations_cloud-20240517.0.dev0/PKG-INFO
```

### Comparing `great_expectations_cloud-20240516.1.dev0/LICENSE` & `great_expectations_cloud-20240517.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/README.md` & `great_expectations_cloud-20240517.0.dev0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 ## Dev Setup
 
 See also [CONTRIBUTING.md](https://github.com/great-expectations/cloud/blob/main/CONTRIBUTING.md)
 
 1. [Install `poetry`](https://python-poetry.org/docs/#installation)
    - [`pipx install poetry`](https://python-poetry.org/docs/#installing-with-pipx)
-2. Set up virtual environment and install dependencies.
+2. Set up virtual environment and install dependencies
    - `poetry install --sync`
-3. Activate your virtual environment.
+3. Activate your virtual environment
    - `poetry shell`
 4. Set up precommit hooks
    - `pre-commit install`
 
 ### Developer Tasks
 
 Common developer tasks are available via `invoke` (defined in `tasks.py`)
```

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/__init__.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/agent_action.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/agent_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_missingness_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/data_assistants/run_onboarding_data_assistant.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/data_assistants/utils.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/draft_datasource_config_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/list_table_names.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/list_table_names.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/run_checkpoint.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/run_metric_list_action.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/actions/unknown.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/actions/unknown.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/agent.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/agent.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/cli.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/cli.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/config.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/config.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/event_handler.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/event_handler.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/exceptions.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/message_service/asyncio_rabbit_mq_client.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/message_service/subscriber.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/message_service/subscriber.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/models.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/models.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/agent/run.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/agent/run.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/logging/README.md` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/logging/README.md`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/great_expectations_cloud/logging/logging_cfg.py` & `great_expectations_cloud-20240517.0.dev0/great_expectations_cloud/logging/logging_cfg.py`

 * *Files identical despite different names*

### Comparing `great_expectations_cloud-20240516.1.dev0/pyproject.toml` & `great_expectations_cloud-20240517.0.dev0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "great_expectations_cloud"
-version = "20240516.1.dev0"
+version = "20240517.0.dev0"
 description = "Great Expectations Cloud"
 authors = ["The Great Expectations Team <team@greatexpectations.io>"]
 repository = "https://github.com/great-expectations/cloud"
 homepage = "https://greatexpectations.io"
 readme = "README.md"
 license = "Proprietary"
 classifiers = [
@@ -40,21 +40,22 @@
 snowflake-sqlalchemy = ">=1.5.0"
 snowflake-connector-python = ">=3.3.1"
 # TODO: Remove the python constraint once this PR is merged - https://github.com/sqlalchemy-redshift/sqlalchemy-redshift/pull/288
 sqlalchemy-redshift = { version = "^0.8.8", python = "<3.11" }
 psycopg2-binary = "^2.9.9"
 
 [tool.poetry.group.dev.dependencies]
+coverage = {extras = ["toml"], version = "^7.5.1"}
 freezegun = "^1.4.0"
 invoke = "^2.2.0"
 mypy = "1.10.0"
 pre-commit = "^3.3.3"
 pyfakefs = "^5.4.1"
 pytest = ">=7.4,<9.0"
-pytest-cov = ">=4.1,<6.0"
+pytest-cov = ">=5"
 pytest-icdiff = "*"
 pytest-mock = "*"
 responses = "^0.23.1"
 ruff = "0.4.4"
 tenacity = "^8.2.3"
 tomlkit = "^0.12.1"
 types-requests = "^2.31"
@@ -191,15 +192,15 @@
     "UP007", # non-pep604-annotation - pydantic models use annotations at runtime
 ]
 "tasks.py" = [
     "S101", # https://docs.astral.sh/ruff/rules/assert/
 ]
 
 [tool.pytest.ini_options]
-addopts = "--cov=great_expectations_cloud --cov-config=.coveragerc"
+addopts = "--cov=great_expectations_cloud"
 markers = [
     "agentjobs",
     "unit: mark a test as a unit test i.e. no external dependencies.",
     "integration: test that relies on a running GX Cloud and mercury instance.",
 ]
 log_level = "info"
 filterwarnings = [
@@ -228,7 +229,21 @@
     # IAM_ROLE_NAME_RE = re.compile('[A-Za-z0-9+=,.@\-_]{1,64}')"
     # DeprecationWarning: invalid escape sequence \-
     "ignore:invalid escape sequence",
     # Full warning:
     # PoetryVersionOutdated: The latest version of poetry is latest_poetry_version: 1.8.0 but the poetry.lock file was generated using 1.7.1.
     "once:.*:tests.test_project.PoetryVersionOutdated",
 ]
+
+[tool.coverage.report]
+# https://coverage.readthedocs.io/en/7.5.1/config.html
+# Regexes for lines to exclude from consideration
+exclude_also = [
+    # type-checking imports don't exist at runtime
+    "if TYPE_CHECKING:",
+    # Don't complain if tests don't hit NotImplementedError:
+    "raise NotImplementedError",
+    # Don't complain if non-runnable code isn't run:
+    "if __name__ == .__main__.:",
+    # Don't complain about abstract methods, they aren't run:
+    "@(abc\\.)?abstractmethod",
+    ]
```

### Comparing `great_expectations_cloud-20240516.1.dev0/PKG-INFO` & `great_expectations_cloud-20240517.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great_expectations_cloud
-Version: 20240516.1.dev0
+Version: 20240517.0.dev0
 Summary: Great Expectations Cloud
 Home-page: https://greatexpectations.io
 License: Proprietary
 Author: The Great Expectations Team
 Author-email: team@greatexpectations.io
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -90,17 +90,17 @@
 
 ## Dev Setup
 
 See also [CONTRIBUTING.md](https://github.com/great-expectations/cloud/blob/main/CONTRIBUTING.md)
 
 1. [Install `poetry`](https://python-poetry.org/docs/#installation)
    - [`pipx install poetry`](https://python-poetry.org/docs/#installing-with-pipx)
-2. Set up virtual environment and install dependencies.
+2. Set up virtual environment and install dependencies
    - `poetry install --sync`
-3. Activate your virtual environment.
+3. Activate your virtual environment
    - `poetry shell`
 4. Set up precommit hooks
    - `pre-commit install`
 
 ### Developer Tasks
 
 Common developer tasks are available via `invoke` (defined in `tasks.py`)
```

