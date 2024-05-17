# Comparing `tmp/cirro-1.1.1.tar.gz` & `tmp/cirro-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirro-1.1.1.tar", max compression
+gzip compressed data, was "cirro-1.1.2.tar", max compression
```

## Comparing `cirro-1.1.1.tar` & `cirro-1.1.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1066 2024-05-09 20:28:42.450644 cirro-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     6113 2024-05-09 20:28:42.450644 cirro-1.1.1/README.md
--rw-r--r--   0        0        0      476 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/__init__.py
--rw-r--r--   0        0        0     1486 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/__init__.py
--rw-r--r--   0        0        0      308 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/base.py
--rw-r--r--   0        0        0     6983 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/device_code.py
--rw-r--r--   0        0        0      432 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/auth/oauth_models.py
--rw-r--r--   0        0        0     4246 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cirro_client.py
--rw-r--r--   0        0        0      190 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/__init__.py
--rw-r--r--   0        0        0     2538 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/cli.py
--rw-r--r--   0        0        0     6694 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/controller.py
--rw-r--r--   0        0        0        0 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/__init__.py
--rw-r--r--   0        0        0     1277 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/auth_args.py
--rw-r--r--   0        0        0      773 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/common_args.py
--rw-r--r--   0        0        0     5229 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/download_args.py
--rw-r--r--   0        0        0      576 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/list_dataset_args.py
--rw-r--r--   0        0        0     5672 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/upload_args.py
--rw-r--r--   0        0        0     2557 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/interactive/utils.py
--rw-r--r--   0        0        0      443 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/cli/models.py
--rw-r--r--   0        0        0       68 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/clients/__init__.py
--rw-r--r--   0        0        0     4456 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/clients/s3.py
--rw-r--r--   0        0        0     4335 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/config.py
--rw-r--r--   0        0        0     4033 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/file_utils.py
--rw-r--r--   0        0        0      164 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/__init__.py
--rw-r--r--   0        0        0     1708 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/constants.py
--rw-r--r--   0        0        0     5202 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/form.py
--rw-r--r--   0        0        0     5922 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/helpers/preprocess_dataset.py
--rw-r--r--   0        0        0        0 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/__init__.py
--rw-r--r--   0        0        0     3567 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/file.py
--rw-r--r--   0        0        0     2607 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/form_specification.py
--rw-r--r--   0        0        0      502 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/s3_path.py
--rw-r--r--   0        0        0      110 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/models/tenant.py
--rw-r--r--   0        0        0        0 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/__init__.py
--rw-r--r--   0        0        0     2993 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/asset.py
--rw-r--r--   0        0        0     7080 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/dataset.py
--rw-r--r--   0        0        0      245 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/exceptions.py
--rw-r--r--   0        0        0     5496 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/file.py
--rw-r--r--   0        0        0     1536 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/helpers.py
--rw-r--r--   0        0        0     4607 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/portal.py
--rw-r--r--   0        0        0     2230 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/process.py
--rw-r--r--   0        0        0     7733 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/project.py
--rw-r--r--   0        0        0     1823 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/reference.py
--rw-r--r--   0        0        0     1188 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/sdk/reference_type.py
--rw-r--r--   0        0        0      544 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/services/__init__.py
--rw-r--r--   0        0        0      981 2024-05-09 20:28:42.450644 cirro-1.1.1/cirro/services/base.py
--rw-r--r--   0        0        0     1417 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/billing.py
--rw-r--r--   0        0        0     7475 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/dataset.py
--rw-r--r--   0        0        0     4680 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/execution.py
--rw-r--r--   0        0        0     6282 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/file.py
--rw-r--r--   0        0        0     2412 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/metadata.py
--rw-r--r--   0        0        0      831 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/metrics.py
--rw-r--r--   0        0        0     3754 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/process.py
--rw-r--r--   0        0        0     5572 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/projects.py
--rw-r--r--   0        0        0      789 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/services/references.py
--rw-r--r--   0        0        0     1514 2024-05-09 20:28:42.454645 cirro-1.1.1/cirro/utils.py
--rw-r--r--   0        0        0      925 2024-05-09 20:28:42.454645 cirro-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 cirro-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 00:35:45.145764 cirro-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     6113 2024-05-17 00:35:45.145764 cirro-1.1.2/README.md
+-rw-r--r--   0        0        0      476 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/__init__.py
+-rw-r--r--   0        0        0     1486 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/__init__.py
+-rw-r--r--   0        0        0      308 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/base.py
+-rw-r--r--   0        0        0     6983 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/device_code.py
+-rw-r--r--   0        0        0      432 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/auth/oauth_models.py
+-rw-r--r--   0        0        0     4470 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cirro_client.py
+-rw-r--r--   0        0        0      190 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/__init__.py
+-rw-r--r--   0        0        0     2538 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/cli.py
+-rw-r--r--   0        0        0     6694 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/controller.py
+-rw-r--r--   0        0        0        0 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/auth_args.py
+-rw-r--r--   0        0        0      773 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/common_args.py
+-rw-r--r--   0        0        0     5229 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/download_args.py
+-rw-r--r--   0        0        0      576 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/list_dataset_args.py
+-rw-r--r--   0        0        0     5672 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/upload_args.py
+-rw-r--r--   0        0        0     2801 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/interactive/utils.py
+-rw-r--r--   0        0        0      443 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/cli/models.py
+-rw-r--r--   0        0        0       68 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/clients/__init__.py
+-rw-r--r--   0        0        0     4456 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/clients/s3.py
+-rw-r--r--   0        0        0     4335 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/config.py
+-rw-r--r--   0        0        0     4033 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/file_utils.py
+-rw-r--r--   0        0        0      164 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/__init__.py
+-rw-r--r--   0        0        0     1708 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/constants.py
+-rw-r--r--   0        0        0     5202 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/form.py
+-rw-r--r--   0        0        0     5922 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/helpers/preprocess_dataset.py
+-rw-r--r--   0        0        0        0 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/__init__.py
+-rw-r--r--   0        0        0     3567 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/file.py
+-rw-r--r--   0        0        0     2607 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/form_specification.py
+-rw-r--r--   0        0        0      502 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/s3_path.py
+-rw-r--r--   0        0        0      110 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/models/tenant.py
+-rw-r--r--   0        0        0        0 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/__init__.py
+-rw-r--r--   0        0        0     2993 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/asset.py
+-rw-r--r--   0        0        0     7080 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/dataset.py
+-rw-r--r--   0        0        0      245 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/exceptions.py
+-rw-r--r--   0        0        0     5496 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/file.py
+-rw-r--r--   0        0        0     1536 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/helpers.py
+-rw-r--r--   0        0        0     4607 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/portal.py
+-rw-r--r--   0        0        0     2230 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/process.py
+-rw-r--r--   0        0        0     7733 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/project.py
+-rw-r--r--   0        0        0     1823 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/reference.py
+-rw-r--r--   0        0        0     1188 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/sdk/reference_type.py
+-rw-r--r--   0        0        0      593 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/__init__.py
+-rw-r--r--   0        0        0      981 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/base.py
+-rw-r--r--   0        0        0     1417 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/billing.py
+-rw-r--r--   0        0        0     7475 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/dataset.py
+-rw-r--r--   0        0        0     4680 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/execution.py
+-rw-r--r--   0        0        0     6282 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/file.py
+-rw-r--r--   0        0        0     2412 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/metadata.py
+-rw-r--r--   0        0        0      831 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/metrics.py
+-rw-r--r--   0        0        0     3754 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/process.py
+-rw-r--r--   0        0        0     5572 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/projects.py
+-rw-r--r--   0        0        0      789 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/references.py
+-rw-r--r--   0        0        0      819 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/services/user.py
+-rw-r--r--   0        0        0     1514 2024-05-17 00:35:45.145764 cirro-1.1.2/cirro/utils.py
+-rw-r--r--   0        0        0      925 2024-05-17 00:35:45.145764 cirro-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7255 1970-01-01 00:00:00.000000 cirro-1.1.2/PKG-INFO
```

### Comparing `cirro-1.1.1/LICENSE.txt` & `cirro-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/README.md` & `cirro-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/auth/__init__.py` & `cirro-1.1.2/cirro/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/auth/device_code.py` & `cirro-1.1.2/cirro/auth/device_code.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cirro_client.py` & `cirro-1.1.2/cirro/cirro_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from cirro_api_client import CirroApiClient
 
 from cirro.auth import get_auth_info_from_config
 from cirro.auth.base import AuthInfo
 from cirro.config import AppConfig
 from cirro.services import FileService, DatasetService, ProjectService, ProcessService, ExecutionService, \
-    MetricsService, MetadataService, BillingService, ReferenceService
+    MetricsService, MetadataService, BillingService, ReferenceService, UserService
 
 
 class CirroApi:
     """
     Client for interacting directly with the Cirro API
     """
     def __init__(self, auth_info: AuthInfo = None, base_url: str = None):
@@ -51,14 +51,15 @@
         self._project_service = ProjectService(self._api_client)
         self._process_service = ProcessService(self._api_client)
         self._execution_service = ExecutionService(self._api_client)
         self._metrics_service = MetricsService(self._api_client)
         self._metadata_service = MetadataService(self._api_client)
         self._billing_service = BillingService(self._api_client)
         self._references_service = ReferenceService(self._api_client)
+        self._users_service = UserService(self._api_client)
 
     @property
     def datasets(self) -> DatasetService:
         """
         Create, list, delete, and modify Datasets
         """
         return self._dataset_service
@@ -109,14 +110,21 @@
     def references(self) -> ReferenceService:
         """
         List References and Reference types
         """
         return self._references_service
 
     @property
+    def users(self) -> UserService:
+        """
+        List and update user information
+        """
+        return self._users_service
+
+    @property
     def file(self) -> FileService:
         """
         Read, download, and create file objects
         """
         return self._file_service
 
     @property
```

### Comparing `cirro-1.1.1/cirro/cli/cli.py` & `cirro-1.1.2/cirro/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cli/controller.py` & `cirro-1.1.2/cirro/cli/controller.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cli/interactive/auth_args.py` & `cirro-1.1.2/cirro/cli/interactive/auth_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cli/interactive/common_args.py` & `cirro-1.1.2/cirro/cli/interactive/common_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cli/interactive/download_args.py` & `cirro-1.1.2/cirro/cli/interactive/download_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cli/interactive/list_dataset_args.py` & `cirro-1.1.2/cirro/cli/interactive/list_dataset_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cli/interactive/upload_args.py` & `cirro-1.1.2/cirro/cli/interactive/upload_args.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/cli/interactive/utils.py` & `cirro-1.1.2/cirro/cli/interactive/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, Callable
+from typing import List, Union, Callable, TypeVar, Optional
 
 import questionary
 from questionary import prompt
 
 
 class InputError(Exception):
     """Errors detected from user input"""
@@ -76,16 +76,23 @@
     return resp
 
 
 def ask_yes_no(msg):
     return ask("select", msg, choices=["Yes", "No"]) == "Yes"
 
 
-def get_id_from_name(items, name_or_id: str) -> str:
-    return get_item_from_name_or_id(items, name_or_id).id
+T = TypeVar('T')
 
 
-def get_item_from_name_or_id(items, name_or_id: str):
+def get_id_from_name(items: List[T], name_or_id: str) -> Optional[str]:
+    matched = get_item_from_name_or_id(items, name_or_id)
+    if not matched:
+        item_type = type(items[0]).__name__
+        raise InputError(f"Could not find {item_type} {name_or_id}")
+    return matched.id
+
+
+def get_item_from_name_or_id(items: List[T], name_or_id: str) -> Optional[T]:
     matched = next((p for p in items if p.id == name_or_id), None)
     if matched:
         return matched
-    return next(p for p in items if p.name == name_or_id)
+    return next((p for p in items if p.name == name_or_id), None)
```

### Comparing `cirro-1.1.1/cirro/clients/s3.py` & `cirro-1.1.2/cirro/clients/s3.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/config.py` & `cirro-1.1.2/cirro/config.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/file_utils.py` & `cirro-1.1.2/cirro/file_utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/helpers/constants.py` & `cirro-1.1.2/cirro/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/helpers/form.py` & `cirro-1.1.2/cirro/helpers/form.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/helpers/preprocess_dataset.py` & `cirro-1.1.2/cirro/helpers/preprocess_dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/models/file.py` & `cirro-1.1.2/cirro/models/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/models/form_specification.py` & `cirro-1.1.2/cirro/models/form_specification.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/asset.py` & `cirro-1.1.2/cirro/sdk/asset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/dataset.py` & `cirro-1.1.2/cirro/sdk/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/file.py` & `cirro-1.1.2/cirro/sdk/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/helpers.py` & `cirro-1.1.2/cirro/sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/portal.py` & `cirro-1.1.2/cirro/sdk/portal.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/process.py` & `cirro-1.1.2/cirro/sdk/process.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/project.py` & `cirro-1.1.2/cirro/sdk/project.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/reference.py` & `cirro-1.1.2/cirro/sdk/reference.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/sdk/reference_type.py` & `cirro-1.1.2/cirro/sdk/reference_type.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/__init__.py` & `cirro-1.1.2/cirro/services/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from .execution import ExecutionService
 from .file import FileService
 from .metadata import MetadataService
 from .metrics import MetricsService
 from .process import ProcessService
 from .projects import ProjectService
 from .references import ReferenceService
+from .user import UserService
 
 __all__ = [
     'BillingService',
     'DatasetService',
     'ExecutionService',
     'FileService',
     'MetadataService',
     'MetricsService',
     'ProcessService',
     'ProjectService',
-    'ReferenceService'
+    'ReferenceService',
+    'UserService'
 ]
```

### Comparing `cirro-1.1.1/cirro/services/base.py` & `cirro-1.1.2/cirro/services/base.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/billing.py` & `cirro-1.1.2/cirro/services/billing.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/dataset.py` & `cirro-1.1.2/cirro/services/dataset.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/execution.py` & `cirro-1.1.2/cirro/services/execution.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/file.py` & `cirro-1.1.2/cirro/services/file.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/metadata.py` & `cirro-1.1.2/cirro/services/metadata.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/metrics.py` & `cirro-1.1.2/cirro/services/metrics.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/process.py` & `cirro-1.1.2/cirro/services/process.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/projects.py` & `cirro-1.1.2/cirro/services/projects.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/services/references.py` & `cirro-1.1.2/cirro/services/references.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/cirro/utils.py` & `cirro-1.1.2/cirro/utils.py`

 * *Files identical despite different names*

### Comparing `cirro-1.1.1/pyproject.toml` & `cirro-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cirro"
-version = "1.1.1"
+version = "1.1.2"
 description = "CLI tool and SDK for interacting with the Cirro platform"
 authors = ["Cirro Bio <support@cirro.bio>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CirroBio/Cirro-client"
 packages = [{include = "cirro"}]
```

### Comparing `cirro-1.1.1/PKG-INFO` & `cirro-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirro
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI tool and SDK for interacting with the Cirro platform
 Home-page: https://github.com/CirroBio/Cirro-client
 License: MIT
 Author: Cirro Bio
 Author-email: support@cirro.bio
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

