# Comparing `tmp/alibabacloud_polardb20170801-5.1.0.tar.gz` & `tmp/alibabacloud_polardb20170801-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_polardb20170801-5.1.0.tar", last modified: Wed Apr 24 01:48:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_polardb20170801-5.1.1.tar", last modified: Fri May 17 17:19:14 2024, max compression
```

## Comparing `alibabacloud_polardb20170801-5.1.0.tar` & `alibabacloud_polardb20170801-5.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/
--rw-r--r--   0 root         (0) root         (0)     4003 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2442 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1111 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1196 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   730040 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801/client.py
--rw-r--r--   0 root         (0) root         (0)  1217802 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2442 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-24 01:48:03.000000 alibabacloud_polardb20170801-5.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2644 2024-04-24 01:48:02.000000 alibabacloud_polardb20170801-5.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/
+-rw-r--r--   0 root         (0) root         (0)     4060 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   858320 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/client.py
+-rw-r--r--   0 root         (0) root         (0)  1239934 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2442 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 17:19:14.000000 alibabacloud_polardb20170801-5.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2644 2024-05-17 17:19:13.000000 alibabacloud_polardb20170801-5.1.1/setup.py
```

### Comparing `alibabacloud_polardb20170801-5.1.0/ChangeLog.md` & `alibabacloud_polardb20170801-5.1.1/ChangeLog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-24 Version: 5.1.0
+- Support API RestartDBLink.
+
+
 2024-04-18 Version: 5.0.8
 - Update API DescribeDBClusterAttribute: update response param.
 - Update API DescribeDBClusters: update response param.
 
 
 2024-04-09 Version: 5.0.7
 - Update API DescribeDBClusters: update response param.
```

### Comparing `alibabacloud_polardb20170801-5.1.0/LICENSE` & `alibabacloud_polardb20170801-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801-5.1.0/PKG-INFO` & `alibabacloud_polardb20170801-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_polardb20170801
-Version: 5.1.0
+Version: 5.1.1
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801-5.1.0/README-CN.md` & `alibabacloud_polardb20170801-5.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801-5.1.0/README.md` & `alibabacloud_polardb20170801-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801/client.py` & `alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,14 +90,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def cancel_schedule_tasks_with_options(
         self,
         request: polardb_20170801_models.CancelScheduleTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CancelScheduleTasksResponse:
+        """
+        @summary Cancels scheduled tasks that are not yet started.
+        
+        @param request: CancelScheduleTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CancelScheduleTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -130,14 +137,21 @@
         )
 
     async def cancel_schedule_tasks_with_options_async(
         self,
         request: polardb_20170801_models.CancelScheduleTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CancelScheduleTasksResponse:
+        """
+        @summary Cancels scheduled tasks that are not yet started.
+        
+        @param request: CancelScheduleTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CancelScheduleTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -169,29 +183,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def cancel_schedule_tasks(
         self,
         request: polardb_20170801_models.CancelScheduleTasksRequest,
     ) -> polardb_20170801_models.CancelScheduleTasksResponse:
+        """
+        @summary Cancels scheduled tasks that are not yet started.
+        
+        @param request: CancelScheduleTasksRequest
+        @return: CancelScheduleTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.cancel_schedule_tasks_with_options(request, runtime)
 
     async def cancel_schedule_tasks_async(
         self,
         request: polardb_20170801_models.CancelScheduleTasksRequest,
     ) -> polardb_20170801_models.CancelScheduleTasksResponse:
+        """
+        @summary Cancels scheduled tasks that are not yet started.
+        
+        @param request: CancelScheduleTasksRequest
+        @return: CancelScheduleTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.cancel_schedule_tasks_with_options_async(request, runtime)
 
     def check_account_name_with_options(
         self,
         request: polardb_20170801_models.CheckAccountNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckAccountNameResponse:
+        """
+        @summary Checks whether an account name is valid or unique in a cluster.
+        
+        @param request: CheckAccountNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckAccountNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -222,14 +255,21 @@
         )
 
     async def check_account_name_with_options_async(
         self,
         request: polardb_20170801_models.CheckAccountNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckAccountNameResponse:
+        """
+        @summary Checks whether an account name is valid or unique in a cluster.
+        
+        @param request: CheckAccountNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckAccountNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -259,29 +299,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def check_account_name(
         self,
         request: polardb_20170801_models.CheckAccountNameRequest,
     ) -> polardb_20170801_models.CheckAccountNameResponse:
+        """
+        @summary Checks whether an account name is valid or unique in a cluster.
+        
+        @param request: CheckAccountNameRequest
+        @return: CheckAccountNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.check_account_name_with_options(request, runtime)
 
     async def check_account_name_async(
         self,
         request: polardb_20170801_models.CheckAccountNameRequest,
     ) -> polardb_20170801_models.CheckAccountNameResponse:
+        """
+        @summary Checks whether an account name is valid or unique in a cluster.
+        
+        @param request: CheckAccountNameRequest
+        @return: CheckAccountNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.check_account_name_with_options_async(request, runtime)
 
     def check_dbname_with_options(
         self,
         request: polardb_20170801_models.CheckDBNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckDBNameResponse:
+        """
+        @summary Checks whether a database name is valid or whether the name is already used by another database in the current cluster.
+        
+        @param request: CheckDBNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckDBNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbname):
             query['DBName'] = request.dbname
         if not UtilClient.is_unset(request.owner_account):
@@ -312,14 +371,21 @@
         )
 
     async def check_dbname_with_options_async(
         self,
         request: polardb_20170801_models.CheckDBNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckDBNameResponse:
+        """
+        @summary Checks whether a database name is valid or whether the name is already used by another database in the current cluster.
+        
+        @param request: CheckDBNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckDBNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbname):
             query['DBName'] = request.dbname
         if not UtilClient.is_unset(request.owner_account):
@@ -349,29 +415,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def check_dbname(
         self,
         request: polardb_20170801_models.CheckDBNameRequest,
     ) -> polardb_20170801_models.CheckDBNameResponse:
+        """
+        @summary Checks whether a database name is valid or whether the name is already used by another database in the current cluster.
+        
+        @param request: CheckDBNameRequest
+        @return: CheckDBNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.check_dbname_with_options(request, runtime)
 
     async def check_dbname_async(
         self,
         request: polardb_20170801_models.CheckDBNameRequest,
     ) -> polardb_20170801_models.CheckDBNameResponse:
+        """
+        @summary Checks whether a database name is valid or whether the name is already used by another database in the current cluster.
+        
+        @param request: CheckDBNameRequest
+        @return: CheckDBNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.check_dbname_with_options_async(request, runtime)
 
     def check_kmsauthorized_with_options(
         self,
         request: polardb_20170801_models.CheckKMSAuthorizedRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckKMSAuthorizedResponse:
+        """
+        @summary Queries whether the cluster is authorized to use Key Management Service (KMS).
+        
+        @param request: CheckKMSAuthorizedRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckKMSAuthorizedResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -404,14 +489,21 @@
         )
 
     async def check_kmsauthorized_with_options_async(
         self,
         request: polardb_20170801_models.CheckKMSAuthorizedRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckKMSAuthorizedResponse:
+        """
+        @summary Queries whether the cluster is authorized to use Key Management Service (KMS).
+        
+        @param request: CheckKMSAuthorizedRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckKMSAuthorizedResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -443,29 +535,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def check_kmsauthorized(
         self,
         request: polardb_20170801_models.CheckKMSAuthorizedRequest,
     ) -> polardb_20170801_models.CheckKMSAuthorizedResponse:
+        """
+        @summary Queries whether the cluster is authorized to use Key Management Service (KMS).
+        
+        @param request: CheckKMSAuthorizedRequest
+        @return: CheckKMSAuthorizedResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.check_kmsauthorized_with_options(request, runtime)
 
     async def check_kmsauthorized_async(
         self,
         request: polardb_20170801_models.CheckKMSAuthorizedRequest,
     ) -> polardb_20170801_models.CheckKMSAuthorizedResponse:
+        """
+        @summary Queries whether the cluster is authorized to use Key Management Service (KMS).
+        
+        @param request: CheckKMSAuthorizedRequest
+        @return: CheckKMSAuthorizedResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.check_kmsauthorized_with_options_async(request, runtime)
 
     def check_service_linked_role_with_options(
         self,
         request: polardb_20170801_models.CheckServiceLinkedRoleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckServiceLinkedRoleResponse:
+        """
+        @summary Checks whether a service-linked role (SLR) is created.
+        
+        @param request: CheckServiceLinkedRoleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckServiceLinkedRoleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -492,14 +603,21 @@
         )
 
     async def check_service_linked_role_with_options_async(
         self,
         request: polardb_20170801_models.CheckServiceLinkedRoleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CheckServiceLinkedRoleResponse:
+        """
+        @summary Checks whether a service-linked role (SLR) is created.
+        
+        @param request: CheckServiceLinkedRoleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CheckServiceLinkedRoleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -525,29 +643,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def check_service_linked_role(
         self,
         request: polardb_20170801_models.CheckServiceLinkedRoleRequest,
     ) -> polardb_20170801_models.CheckServiceLinkedRoleResponse:
+        """
+        @summary Checks whether a service-linked role (SLR) is created.
+        
+        @param request: CheckServiceLinkedRoleRequest
+        @return: CheckServiceLinkedRoleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.check_service_linked_role_with_options(request, runtime)
 
     async def check_service_linked_role_async(
         self,
         request: polardb_20170801_models.CheckServiceLinkedRoleRequest,
     ) -> polardb_20170801_models.CheckServiceLinkedRoleResponse:
+        """
+        @summary Checks whether a service-linked role (SLR) is created.
+        
+        @param request: CheckServiceLinkedRoleRequest
+        @return: CheckServiceLinkedRoleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.check_service_linked_role_with_options_async(request, runtime)
 
     def close_aitask_with_options(
         self,
         request: polardb_20170801_models.CloseAITaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CloseAITaskResponse:
+        """
+        @summary 关闭DB4AI
+        
+        @param request: CloseAITaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CloseAITaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -578,14 +715,21 @@
         )
 
     async def close_aitask_with_options_async(
         self,
         request: polardb_20170801_models.CloseAITaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CloseAITaskResponse:
+        """
+        @summary 关闭DB4AI
+        
+        @param request: CloseAITaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CloseAITaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -615,33 +759,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def close_aitask(
         self,
         request: polardb_20170801_models.CloseAITaskRequest,
     ) -> polardb_20170801_models.CloseAITaskResponse:
+        """
+        @summary 关闭DB4AI
+        
+        @param request: CloseAITaskRequest
+        @return: CloseAITaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.close_aitask_with_options(request, runtime)
 
     async def close_aitask_async(
         self,
         request: polardb_20170801_models.CloseAITaskRequest,
     ) -> polardb_20170801_models.CloseAITaskResponse:
+        """
+        @summary 关闭DB4AI
+        
+        @param request: CloseAITaskRequest
+        @return: CloseAITaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.close_aitask_with_options_async(request, runtime)
 
     def close_dbcluster_migration_with_options(
         self,
         request: polardb_20170801_models.CloseDBClusterMigrationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CloseDBClusterMigrationResponse:
         """
-        You can call this operation to cancel the migration task before data migration.
-        *   You can call this operation to perform the migration task after data migration.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Cancels or completes the migration task that upgrades an RDS cluster to a PolarDB cluster.
+        
+        @description    You can call this operation to cancel the migration task before data migration.
+        You can call this operation to perform the migration task after data migration.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: CloseDBClusterMigrationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CloseDBClusterMigrationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -678,17 +836,19 @@
 
     async def close_dbcluster_migration_with_options_async(
         self,
         request: polardb_20170801_models.CloseDBClusterMigrationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CloseDBClusterMigrationResponse:
         """
-        You can call this operation to cancel the migration task before data migration.
-        *   You can call this operation to perform the migration task after data migration.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Cancels or completes the migration task that upgrades an RDS cluster to a PolarDB cluster.
+        
+        @description    You can call this operation to cancel the migration task before data migration.
+        You can call this operation to perform the migration task after data migration.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: CloseDBClusterMigrationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CloseDBClusterMigrationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -724,44 +884,55 @@
         )
 
     def close_dbcluster_migration(
         self,
         request: polardb_20170801_models.CloseDBClusterMigrationRequest,
     ) -> polardb_20170801_models.CloseDBClusterMigrationResponse:
         """
-        You can call this operation to cancel the migration task before data migration.
-        *   You can call this operation to perform the migration task after data migration.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Cancels or completes the migration task that upgrades an RDS cluster to a PolarDB cluster.
+        
+        @description    You can call this operation to cancel the migration task before data migration.
+        You can call this operation to perform the migration task after data migration.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: CloseDBClusterMigrationRequest
         @return: CloseDBClusterMigrationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.close_dbcluster_migration_with_options(request, runtime)
 
     async def close_dbcluster_migration_async(
         self,
         request: polardb_20170801_models.CloseDBClusterMigrationRequest,
     ) -> polardb_20170801_models.CloseDBClusterMigrationResponse:
         """
-        You can call this operation to cancel the migration task before data migration.
-        *   You can call this operation to perform the migration task after data migration.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Cancels or completes the migration task that upgrades an RDS cluster to a PolarDB cluster.
+        
+        @description    You can call this operation to cancel the migration task before data migration.
+        You can call this operation to perform the migration task after data migration.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: CloseDBClusterMigrationRequest
         @return: CloseDBClusterMigrationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.close_dbcluster_migration_with_options_async(request, runtime)
 
     def create_account_with_options(
         self,
         request: polardb_20170801_models.CreateAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateAccountResponse:
+        """
+        @summary Creates a database account for a PolarDB cluster.
+        
+        @param request: CreateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAccountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_description):
             query['AccountDescription'] = request.account_description
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.account_password):
@@ -806,14 +977,21 @@
         )
 
     async def create_account_with_options_async(
         self,
         request: polardb_20170801_models.CreateAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateAccountResponse:
+        """
+        @summary Creates a database account for a PolarDB cluster.
+        
+        @param request: CreateAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAccountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_description):
             query['AccountDescription'] = request.account_description
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.account_password):
@@ -857,34 +1035,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_account(
         self,
         request: polardb_20170801_models.CreateAccountRequest,
     ) -> polardb_20170801_models.CreateAccountResponse:
+        """
+        @summary Creates a database account for a PolarDB cluster.
+        
+        @param request: CreateAccountRequest
+        @return: CreateAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_account_with_options(request, runtime)
 
     async def create_account_async(
         self,
         request: polardb_20170801_models.CreateAccountRequest,
     ) -> polardb_20170801_models.CreateAccountResponse:
+        """
+        @summary Creates a database account for a PolarDB cluster.
+        
+        @param request: CreateAccountRequest
+        @return: CreateAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_account_with_options_async(request, runtime)
 
     def create_backup_with_options(
         self,
         request: polardb_20170801_models.CreateBackupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateBackupResponse:
         """
-        >
-        *   You can manually create up to three backups for each cluster.
-        *   The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](~~98101~~).
-        *   After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
+        @summary Creates a full snapshot backup for a PolarDB cluster.
+        
+        @description >
+        You can manually create up to three backups for each cluster.
+        The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](https://help.aliyun.com/document_detail/98101.html).
+        After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
         
         @param request: CreateBackupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateBackupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -921,18 +1113,20 @@
 
     async def create_backup_with_options_async(
         self,
         request: polardb_20170801_models.CreateBackupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateBackupResponse:
         """
-        >
-        *   You can manually create up to three backups for each cluster.
-        *   The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](~~98101~~).
-        *   After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
+        @summary Creates a full snapshot backup for a PolarDB cluster.
+        
+        @description >
+        You can manually create up to three backups for each cluster.
+        The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](https://help.aliyun.com/document_detail/98101.html).
+        After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
         
         @param request: CreateBackupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateBackupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -968,46 +1162,57 @@
         )
 
     def create_backup(
         self,
         request: polardb_20170801_models.CreateBackupRequest,
     ) -> polardb_20170801_models.CreateBackupResponse:
         """
-        >
-        *   You can manually create up to three backups for each cluster.
-        *   The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](~~98101~~).
-        *   After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
+        @summary Creates a full snapshot backup for a PolarDB cluster.
+        
+        @description >
+        You can manually create up to three backups for each cluster.
+        The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](https://help.aliyun.com/document_detail/98101.html).
+        After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
         
         @param request: CreateBackupRequest
         @return: CreateBackupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_backup_with_options(request, runtime)
 
     async def create_backup_async(
         self,
         request: polardb_20170801_models.CreateBackupRequest,
     ) -> polardb_20170801_models.CreateBackupResponse:
         """
-        >
-        *   You can manually create up to three backups for each cluster.
-        *   The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](~~98101~~).
-        *   After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
+        @summary Creates a full snapshot backup for a PolarDB cluster.
+        
+        @description >
+        You can manually create up to three backups for each cluster.
+        The `Exceeding the daily backup times of this DB cluster` error message indicates that three manual backups already exist in your cluster. You must delete existing backups before you call this operation to manually create backups. For more information about how to delete backups, see [Delete backups](https://help.aliyun.com/document_detail/98101.html).
+        After you call this operation, a backup task is created in the backend. The task may be time-consuming if you want to back up large amounts of data.
         
         @param request: CreateBackupRequest
         @return: CreateBackupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_backup_with_options_async(request, runtime)
 
     def create_cold_storage_instance_with_options(
         self,
         request: polardb_20170801_models.CreateColdStorageInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateColdStorageInstanceResponse:
+        """
+        @summary 创建冷存储实例
+        
+        @param request: CreateColdStorageInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateColdStorageInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.cold_storage_instance_description):
             query['ColdStorageInstanceDescription'] = request.cold_storage_instance_description
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -1042,14 +1247,21 @@
         )
 
     async def create_cold_storage_instance_with_options_async(
         self,
         request: polardb_20170801_models.CreateColdStorageInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateColdStorageInstanceResponse:
+        """
+        @summary 创建冷存储实例
+        
+        @param request: CreateColdStorageInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateColdStorageInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.cold_storage_instance_description):
             query['ColdStorageInstanceDescription'] = request.cold_storage_instance_description
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -1083,29 +1295,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_cold_storage_instance(
         self,
         request: polardb_20170801_models.CreateColdStorageInstanceRequest,
     ) -> polardb_20170801_models.CreateColdStorageInstanceResponse:
+        """
+        @summary 创建冷存储实例
+        
+        @param request: CreateColdStorageInstanceRequest
+        @return: CreateColdStorageInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_cold_storage_instance_with_options(request, runtime)
 
     async def create_cold_storage_instance_async(
         self,
         request: polardb_20170801_models.CreateColdStorageInstanceRequest,
     ) -> polardb_20170801_models.CreateColdStorageInstanceResponse:
+        """
+        @summary 创建冷存储实例
+        
+        @param request: CreateColdStorageInstanceRequest
+        @return: CreateColdStorageInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_cold_storage_instance_with_options_async(request, runtime)
 
     def create_dbcluster_with_options(
         self,
         request: polardb_20170801_models.CreateDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBClusterResponse:
+        """
+        @summary Creates a PolarDB cluster.
+        
+        @param request: CreateDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_shut_down):
             query['AllowShutDown'] = request.allow_shut_down
         if not UtilClient.is_unset(request.architecture):
             query['Architecture'] = request.architecture
         if not UtilClient.is_unset(request.auto_renew):
@@ -1232,14 +1463,21 @@
         )
 
     async def create_dbcluster_with_options_async(
         self,
         request: polardb_20170801_models.CreateDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBClusterResponse:
+        """
+        @summary Creates a PolarDB cluster.
+        
+        @param request: CreateDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_shut_down):
             query['AllowShutDown'] = request.allow_shut_down
         if not UtilClient.is_unset(request.architecture):
             query['Architecture'] = request.architecture
         if not UtilClient.is_unset(request.auto_renew):
@@ -1365,29 +1603,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_dbcluster(
         self,
         request: polardb_20170801_models.CreateDBClusterRequest,
     ) -> polardb_20170801_models.CreateDBClusterResponse:
+        """
+        @summary Creates a PolarDB cluster.
+        
+        @param request: CreateDBClusterRequest
+        @return: CreateDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_dbcluster_with_options(request, runtime)
 
     async def create_dbcluster_async(
         self,
         request: polardb_20170801_models.CreateDBClusterRequest,
     ) -> polardb_20170801_models.CreateDBClusterResponse:
+        """
+        @summary Creates a PolarDB cluster.
+        
+        @param request: CreateDBClusterRequest
+        @return: CreateDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_dbcluster_with_options_async(request, runtime)
 
     def create_dbcluster_endpoint_with_options(
         self,
         request: polardb_20170801_models.CreateDBClusterEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBClusterEndpointResponse:
+        """
+        @summary Creates a custom cluster endpoint for a PolarDB cluster.
+        
+        @param request: CreateDBClusterEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDBClusterEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_add_new_nodes):
             query['AutoAddNewNodes'] = request.auto_add_new_nodes
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -1430,14 +1687,21 @@
         )
 
     async def create_dbcluster_endpoint_with_options_async(
         self,
         request: polardb_20170801_models.CreateDBClusterEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBClusterEndpointResponse:
+        """
+        @summary Creates a custom cluster endpoint for a PolarDB cluster.
+        
+        @param request: CreateDBClusterEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDBClusterEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_add_new_nodes):
             query['AutoAddNewNodes'] = request.auto_add_new_nodes
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -1479,31 +1743,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_dbcluster_endpoint(
         self,
         request: polardb_20170801_models.CreateDBClusterEndpointRequest,
     ) -> polardb_20170801_models.CreateDBClusterEndpointResponse:
+        """
+        @summary Creates a custom cluster endpoint for a PolarDB cluster.
+        
+        @param request: CreateDBClusterEndpointRequest
+        @return: CreateDBClusterEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_dbcluster_endpoint_with_options(request, runtime)
 
     async def create_dbcluster_endpoint_async(
         self,
         request: polardb_20170801_models.CreateDBClusterEndpointRequest,
     ) -> polardb_20170801_models.CreateDBClusterEndpointResponse:
+        """
+        @summary Creates a custom cluster endpoint for a PolarDB cluster.
+        
+        @param request: CreateDBClusterEndpointRequest
+        @return: CreateDBClusterEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_dbcluster_endpoint_with_options_async(request, runtime)
 
     def create_dbendpoint_address_with_options(
         self,
         request: polardb_20170801_models.CreateDBEndpointAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBEndpointAddressResponse:
         """
-        > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        @summary Creates a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        
+        @description > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
         
         @param request: CreateDBEndpointAddressRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDBEndpointAddressResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1550,15 +1828,17 @@
 
     async def create_dbendpoint_address_with_options_async(
         self,
         request: polardb_20170801_models.CreateDBEndpointAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBEndpointAddressResponse:
         """
-        > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        @summary Creates a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        
+        @description > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
         
         @param request: CreateDBEndpointAddressRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDBEndpointAddressResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1604,45 +1884,51 @@
         )
 
     def create_dbendpoint_address(
         self,
         request: polardb_20170801_models.CreateDBEndpointAddressRequest,
     ) -> polardb_20170801_models.CreateDBEndpointAddressResponse:
         """
-        > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        @summary Creates a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        
+        @description > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
         
         @param request: CreateDBEndpointAddressRequest
         @return: CreateDBEndpointAddressResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dbendpoint_address_with_options(request, runtime)
 
     async def create_dbendpoint_address_async(
         self,
         request: polardb_20170801_models.CreateDBEndpointAddressRequest,
     ) -> polardb_20170801_models.CreateDBEndpointAddressResponse:
         """
-        > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        @summary Creates a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        
+        @description > You can create a public endpoint for the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
         
         @param request: CreateDBEndpointAddressRequest
         @return: CreateDBEndpointAddressResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_dbendpoint_address_with_options_async(request, runtime)
 
     def create_dblink_with_options(
         self,
         request: polardb_20170801_models.CreateDBLinkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBLinkResponse:
         """
-        A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
-        > *   You can create up to 10 database links for a cluster.
-        > *   Each database link connects a source cluster and a destination cluster.
-        > *   The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
+        @summary Creates a database link.
+        
+        @description A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
+        >    You can create up to 10 database links for a cluster.
+        >    Each database link connects a source cluster and a destination cluster.
+        >    The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
         
         @param request: CreateDBLinkRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDBLinkResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1701,18 +1987,20 @@
 
     async def create_dblink_with_options_async(
         self,
         request: polardb_20170801_models.CreateDBLinkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBLinkResponse:
         """
-        A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
-        > *   You can create up to 10 database links for a cluster.
-        > *   Each database link connects a source cluster and a destination cluster.
-        > *   The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
+        @summary Creates a database link.
+        
+        @description A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
+        >    You can create up to 10 database links for a cluster.
+        >    Each database link connects a source cluster and a destination cluster.
+        >    The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
         
         @param request: CreateDBLinkRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDBLinkResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1770,46 +2058,57 @@
         )
 
     def create_dblink(
         self,
         request: polardb_20170801_models.CreateDBLinkRequest,
     ) -> polardb_20170801_models.CreateDBLinkResponse:
         """
-        A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
-        > *   You can create up to 10 database links for a cluster.
-        > *   Each database link connects a source cluster and a destination cluster.
-        > *   The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
+        @summary Creates a database link.
+        
+        @description A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
+        >    You can create up to 10 database links for a cluster.
+        >    Each database link connects a source cluster and a destination cluster.
+        >    The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
         
         @param request: CreateDBLinkRequest
         @return: CreateDBLinkResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dblink_with_options(request, runtime)
 
     async def create_dblink_async(
         self,
         request: polardb_20170801_models.CreateDBLinkRequest,
     ) -> polardb_20170801_models.CreateDBLinkResponse:
         """
-        A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
-        > *   You can create up to 10 database links for a cluster.
-        > *   Each database link connects a source cluster and a destination cluster.
-        > *   The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
+        @summary Creates a database link.
+        
+        @description A database link can be used to connect two PolarDB for PostgreSQL(Compatible with Oracle) clusters, or connect a PolarDB for PostgreSQL(Compatible with Oracle) cluster to a user-created PostgreSQL database that is hosted on an Elastic Compute Service (ECS) instance. You can use database links to query data across clusters.
+        >    You can create up to 10 database links for a cluster.
+        >    Each database link connects a source cluster and a destination cluster.
+        >    The source cluster and the destination cluster or the destination ECS instance must be located in the same region.
         
         @param request: CreateDBLinkRequest
         @return: CreateDBLinkResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_dblink_with_options_async(request, runtime)
 
     def create_dbnodes_with_options(
         self,
         request: polardb_20170801_models.CreateDBNodesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBNodesResponse:
+        """
+        @summary Adds a read-only node to a PolarDB cluster.
+        
+        @param request: CreateDBNodesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDBNodesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode):
@@ -1854,14 +2153,21 @@
         )
 
     async def create_dbnodes_with_options_async(
         self,
         request: polardb_20170801_models.CreateDBNodesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDBNodesResponse:
+        """
+        @summary Adds a read-only node to a PolarDB cluster.
+        
+        @param request: CreateDBNodesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDBNodesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode):
@@ -1905,33 +2211,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_dbnodes(
         self,
         request: polardb_20170801_models.CreateDBNodesRequest,
     ) -> polardb_20170801_models.CreateDBNodesResponse:
+        """
+        @summary Adds a read-only node to a PolarDB cluster.
+        
+        @param request: CreateDBNodesRequest
+        @return: CreateDBNodesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_dbnodes_with_options(request, runtime)
 
     async def create_dbnodes_async(
         self,
         request: polardb_20170801_models.CreateDBNodesRequest,
     ) -> polardb_20170801_models.CreateDBNodesResponse:
+        """
+        @summary Adds a read-only node to a PolarDB cluster.
+        
+        @param request: CreateDBNodesRequest
+        @return: CreateDBNodesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_dbnodes_with_options_async(request, runtime)
 
     def create_database_with_options(
         self,
         request: polardb_20170801_models.CreateDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDatabaseResponse:
         """
-        Before you call this operation, make sure that the following requirements are met:
-        *   The cluster is in the Running state.
-        *   The cluster is unlocked.
+        @summary Creates a database for a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the following requirements are met:
+        The cluster is in the Running state.
+        The cluster is unlocked.
         
         @param request: CreateDatabaseRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDatabaseResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1980,17 +2300,19 @@
 
     async def create_database_with_options_async(
         self,
         request: polardb_20170801_models.CreateDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateDatabaseResponse:
         """
-        Before you call this operation, make sure that the following requirements are met:
-        *   The cluster is in the Running state.
-        *   The cluster is unlocked.
+        @summary Creates a database for a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the following requirements are met:
+        The cluster is in the Running state.
+        The cluster is unlocked.
         
         @param request: CreateDatabaseRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDatabaseResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2038,46 +2360,52 @@
         )
 
     def create_database(
         self,
         request: polardb_20170801_models.CreateDatabaseRequest,
     ) -> polardb_20170801_models.CreateDatabaseResponse:
         """
-        Before you call this operation, make sure that the following requirements are met:
-        *   The cluster is in the Running state.
-        *   The cluster is unlocked.
+        @summary Creates a database for a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the following requirements are met:
+        The cluster is in the Running state.
+        The cluster is unlocked.
         
         @param request: CreateDatabaseRequest
         @return: CreateDatabaseResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_database_with_options(request, runtime)
 
     async def create_database_async(
         self,
         request: polardb_20170801_models.CreateDatabaseRequest,
     ) -> polardb_20170801_models.CreateDatabaseResponse:
         """
-        Before you call this operation, make sure that the following requirements are met:
-        *   The cluster is in the Running state.
-        *   The cluster is unlocked.
+        @summary Creates a database for a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the following requirements are met:
+        The cluster is in the Running state.
+        The cluster is unlocked.
         
         @param request: CreateDatabaseRequest
         @return: CreateDatabaseResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_database_with_options_async(request, runtime)
 
     def create_global_database_network_with_options(
         self,
         request: polardb_20170801_models.CreateGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateGlobalDatabaseNetworkResponse:
         """
-        >  A cluster belongs to only one GDN.
+        @summary Creates a global database network (GDN).
+        
+        @description >  A cluster belongs to only one GDN.
         
         @param request: CreateGlobalDatabaseNetworkRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateGlobalDatabaseNetworkResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2118,15 +2446,17 @@
 
     async def create_global_database_network_with_options_async(
         self,
         request: polardb_20170801_models.CreateGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateGlobalDatabaseNetworkResponse:
         """
-        >  A cluster belongs to only one GDN.
+        @summary Creates a global database network (GDN).
+        
+        @description >  A cluster belongs to only one GDN.
         
         @param request: CreateGlobalDatabaseNetworkRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateGlobalDatabaseNetworkResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2166,40 +2496,51 @@
         )
 
     def create_global_database_network(
         self,
         request: polardb_20170801_models.CreateGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.CreateGlobalDatabaseNetworkResponse:
         """
-        >  A cluster belongs to only one GDN.
+        @summary Creates a global database network (GDN).
+        
+        @description >  A cluster belongs to only one GDN.
         
         @param request: CreateGlobalDatabaseNetworkRequest
         @return: CreateGlobalDatabaseNetworkResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_global_database_network_with_options(request, runtime)
 
     async def create_global_database_network_async(
         self,
         request: polardb_20170801_models.CreateGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.CreateGlobalDatabaseNetworkResponse:
         """
-        >  A cluster belongs to only one GDN.
+        @summary Creates a global database network (GDN).
+        
+        @description >  A cluster belongs to only one GDN.
         
         @param request: CreateGlobalDatabaseNetworkRequest
         @return: CreateGlobalDatabaseNetworkResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_global_database_network_with_options_async(request, runtime)
 
     def create_global_security_ipgroup_with_options(
         self,
         request: polardb_20170801_models.CreateGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateGlobalSecurityIPGroupResponse:
+        """
+        @summary Creates a global IP whitelist template.
+        
+        @param request: CreateGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gip_list):
             query['GIpList'] = request.gip_list
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.owner_account):
@@ -2236,14 +2577,21 @@
         )
 
     async def create_global_security_ipgroup_with_options_async(
         self,
         request: polardb_20170801_models.CreateGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateGlobalSecurityIPGroupResponse:
+        """
+        @summary Creates a global IP whitelist template.
+        
+        @param request: CreateGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gip_list):
             query['GIpList'] = request.gip_list
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.owner_account):
@@ -2279,31 +2627,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_global_security_ipgroup(
         self,
         request: polardb_20170801_models.CreateGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.CreateGlobalSecurityIPGroupResponse:
+        """
+        @summary Creates a global IP whitelist template.
+        
+        @param request: CreateGlobalSecurityIPGroupRequest
+        @return: CreateGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_global_security_ipgroup_with_options(request, runtime)
 
     async def create_global_security_ipgroup_async(
         self,
         request: polardb_20170801_models.CreateGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.CreateGlobalSecurityIPGroupResponse:
+        """
+        @summary Creates a global IP whitelist template.
+        
+        @param request: CreateGlobalSecurityIPGroupRequest
+        @return: CreateGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_global_security_ipgroup_with_options_async(request, runtime)
 
     def create_parameter_group_with_options(
         self,
         request: polardb_20170801_models.CreateParameterGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Creates a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > You can call this operation only on a PolarDB for MySQL cluster.
         
         @param request: CreateParameterGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateParameterGroupResponse
         """
         UtilClient.validate_model(request)
@@ -2351,15 +2713,17 @@
 
     async def create_parameter_group_with_options_async(
         self,
         request: polardb_20170801_models.CreateParameterGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Creates a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > You can call this operation only on a PolarDB for MySQL cluster.
         
         @param request: CreateParameterGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateParameterGroupResponse
         """
         UtilClient.validate_model(request)
@@ -2406,42 +2770,53 @@
         )
 
     def create_parameter_group(
         self,
         request: polardb_20170801_models.CreateParameterGroupRequest,
     ) -> polardb_20170801_models.CreateParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Creates a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > You can call this operation only on a PolarDB for MySQL cluster.
         
         @param request: CreateParameterGroupRequest
         @return: CreateParameterGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_parameter_group_with_options(request, runtime)
 
     async def create_parameter_group_async(
         self,
         request: polardb_20170801_models.CreateParameterGroupRequest,
     ) -> polardb_20170801_models.CreateParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Creates a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > You can call this operation only on a PolarDB for MySQL cluster.
         
         @param request: CreateParameterGroupRequest
         @return: CreateParameterGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_parameter_group_with_options_async(request, runtime)
 
     def create_service_linked_role_with_options(
         self,
         request: polardb_20170801_models.CreateServiceLinkedRoleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateServiceLinkedRoleResponse:
+        """
+        @summary Creates a service-linked role (SLR).
+        
+        @param request: CreateServiceLinkedRoleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateServiceLinkedRoleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -2468,14 +2843,21 @@
         )
 
     async def create_service_linked_role_with_options_async(
         self,
         request: polardb_20170801_models.CreateServiceLinkedRoleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateServiceLinkedRoleResponse:
+        """
+        @summary Creates a service-linked role (SLR).
+        
+        @param request: CreateServiceLinkedRoleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateServiceLinkedRoleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -2501,29 +2883,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_service_linked_role(
         self,
         request: polardb_20170801_models.CreateServiceLinkedRoleRequest,
     ) -> polardb_20170801_models.CreateServiceLinkedRoleResponse:
+        """
+        @summary Creates a service-linked role (SLR).
+        
+        @param request: CreateServiceLinkedRoleRequest
+        @return: CreateServiceLinkedRoleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_service_linked_role_with_options(request, runtime)
 
     async def create_service_linked_role_async(
         self,
         request: polardb_20170801_models.CreateServiceLinkedRoleRequest,
     ) -> polardb_20170801_models.CreateServiceLinkedRoleResponse:
+        """
+        @summary Creates a service-linked role (SLR).
+        
+        @param request: CreateServiceLinkedRoleRequest
+        @return: CreateServiceLinkedRoleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_service_linked_role_with_options_async(request, runtime)
 
     def create_storage_plan_with_options(
         self,
         request: polardb_20170801_models.CreateStoragePlanRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateStoragePlanResponse:
+        """
+        @summary Purchases a storage plan.
+        
+        @param request: CreateStoragePlanRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateStoragePlanResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2560,14 +2961,21 @@
         )
 
     async def create_storage_plan_with_options_async(
         self,
         request: polardb_20170801_models.CreateStoragePlanRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.CreateStoragePlanResponse:
+        """
+        @summary Purchases a storage plan.
+        
+        @param request: CreateStoragePlanRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateStoragePlanResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -2603,31 +3011,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_storage_plan(
         self,
         request: polardb_20170801_models.CreateStoragePlanRequest,
     ) -> polardb_20170801_models.CreateStoragePlanResponse:
+        """
+        @summary Purchases a storage plan.
+        
+        @param request: CreateStoragePlanRequest
+        @return: CreateStoragePlanResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_storage_plan_with_options(request, runtime)
 
     async def create_storage_plan_async(
         self,
         request: polardb_20170801_models.CreateStoragePlanRequest,
     ) -> polardb_20170801_models.CreateStoragePlanResponse:
+        """
+        @summary Purchases a storage plan.
+        
+        @param request: CreateStoragePlanRequest
+        @return: CreateStoragePlanResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_storage_plan_with_options_async(request, runtime)
 
     def delete_account_with_options(
         self,
         request: polardb_20170801_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteAccountResponse:
         """
-        > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        @summary Deletes a database account for a PolarDB cluster.
+        
+        @description > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
         
         @param request: DeleteAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2664,15 +3086,17 @@
 
     async def delete_account_with_options_async(
         self,
         request: polardb_20170801_models.DeleteAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteAccountResponse:
         """
-        > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        @summary Deletes a database account for a PolarDB cluster.
+        
+        @description > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
         
         @param request: DeleteAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteAccountResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2708,46 +3132,52 @@
         )
 
     def delete_account(
         self,
         request: polardb_20170801_models.DeleteAccountRequest,
     ) -> polardb_20170801_models.DeleteAccountResponse:
         """
-        > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        @summary Deletes a database account for a PolarDB cluster.
+        
+        @description > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
         
         @param request: DeleteAccountRequest
         @return: DeleteAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_account_with_options(request, runtime)
 
     async def delete_account_async(
         self,
         request: polardb_20170801_models.DeleteAccountRequest,
     ) -> polardb_20170801_models.DeleteAccountResponse:
         """
-        > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        @summary Deletes a database account for a PolarDB cluster.
+        
+        @description > Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
         
         @param request: DeleteAccountRequest
         @return: DeleteAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_account_with_options_async(request, runtime)
 
     def delete_backup_with_options(
         self,
         request: polardb_20170801_models.DeleteBackupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteBackupResponse:
         """
-        Before you call this operation, make sure that the cluster meets the following requirements:
-        *   The cluster is in the Running state.
-        *   The backup sets are in the Success state.
-        > *   You can call the [DescribeBackups](~~98102~~) operation to query the status of backup sets.
-        >*   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
+        @summary Deletes the backup sets of a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the cluster meets the following requirements:
+        The cluster is in the Running state.
+        The backup sets are in the Success state.
+        >    You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the status of backup sets.
+        >   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
         
         @param request: DeleteBackupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteBackupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2784,19 +3214,21 @@
 
     async def delete_backup_with_options_async(
         self,
         request: polardb_20170801_models.DeleteBackupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteBackupResponse:
         """
-        Before you call this operation, make sure that the cluster meets the following requirements:
-        *   The cluster is in the Running state.
-        *   The backup sets are in the Success state.
-        > *   You can call the [DescribeBackups](~~98102~~) operation to query the status of backup sets.
-        >*   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
+        @summary Deletes the backup sets of a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the cluster meets the following requirements:
+        The cluster is in the Running state.
+        The backup sets are in the Success state.
+        >    You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the status of backup sets.
+        >   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
         
         @param request: DeleteBackupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteBackupResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2832,48 +3264,59 @@
         )
 
     def delete_backup(
         self,
         request: polardb_20170801_models.DeleteBackupRequest,
     ) -> polardb_20170801_models.DeleteBackupResponse:
         """
-        Before you call this operation, make sure that the cluster meets the following requirements:
-        *   The cluster is in the Running state.
-        *   The backup sets are in the Success state.
-        > *   You can call the [DescribeBackups](~~98102~~) operation to query the status of backup sets.
-        >*   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
+        @summary Deletes the backup sets of a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the cluster meets the following requirements:
+        The cluster is in the Running state.
+        The backup sets are in the Success state.
+        >    You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the status of backup sets.
+        >   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
         
         @param request: DeleteBackupRequest
         @return: DeleteBackupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_backup_with_options(request, runtime)
 
     async def delete_backup_async(
         self,
         request: polardb_20170801_models.DeleteBackupRequest,
     ) -> polardb_20170801_models.DeleteBackupResponse:
         """
-        Before you call this operation, make sure that the cluster meets the following requirements:
-        *   The cluster is in the Running state.
-        *   The backup sets are in the Success state.
-        > *   You can call the [DescribeBackups](~~98102~~) operation to query the status of backup sets.
-        >*   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
+        @summary Deletes the backup sets of a PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the cluster meets the following requirements:
+        The cluster is in the Running state.
+        The backup sets are in the Success state.
+        >    You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the status of backup sets.
+        >   After you delete the backup set file, the storage space that is occupied by the file is released. The released storage space is smaller than the size of the file because your snapshots share some data blocks
         
         @param request: DeleteBackupRequest
         @return: DeleteBackupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_backup_with_options_async(request, runtime)
 
     def delete_dbcluster_with_options(
         self,
         request: polardb_20170801_models.DeleteDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBClusterResponse:
+        """
+        @summary Releases a pay-as-you-go PolarDB cluster.
+        
+        @param request: DeleteDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_retention_policy_on_cluster_deletion):
             query['BackupRetentionPolicyOnClusterDeletion'] = request.backup_retention_policy_on_cluster_deletion
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -2904,14 +3347,21 @@
         )
 
     async def delete_dbcluster_with_options_async(
         self,
         request: polardb_20170801_models.DeleteDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBClusterResponse:
+        """
+        @summary Releases a pay-as-you-go PolarDB cluster.
+        
+        @param request: DeleteDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_retention_policy_on_cluster_deletion):
             query['BackupRetentionPolicyOnClusterDeletion'] = request.backup_retention_policy_on_cluster_deletion
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -2941,29 +3391,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dbcluster(
         self,
         request: polardb_20170801_models.DeleteDBClusterRequest,
     ) -> polardb_20170801_models.DeleteDBClusterResponse:
+        """
+        @summary Releases a pay-as-you-go PolarDB cluster.
+        
+        @param request: DeleteDBClusterRequest
+        @return: DeleteDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dbcluster_with_options(request, runtime)
 
     async def delete_dbcluster_async(
         self,
         request: polardb_20170801_models.DeleteDBClusterRequest,
     ) -> polardb_20170801_models.DeleteDBClusterResponse:
+        """
+        @summary Releases a pay-as-you-go PolarDB cluster.
+        
+        @param request: DeleteDBClusterRequest
+        @return: DeleteDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dbcluster_with_options_async(request, runtime)
 
     def delete_dbcluster_endpoint_with_options(
         self,
         request: polardb_20170801_models.DeleteDBClusterEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBClusterEndpointResponse:
+        """
+        @summary Releases a custom cluster endpoint of a PolarDB cluster.
+        
+        @param request: DeleteDBClusterEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBClusterEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
             query['DBEndpointId'] = request.dbendpoint_id
         if not UtilClient.is_unset(request.owner_account):
@@ -2994,14 +3463,21 @@
         )
 
     async def delete_dbcluster_endpoint_with_options_async(
         self,
         request: polardb_20170801_models.DeleteDBClusterEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBClusterEndpointResponse:
+        """
+        @summary Releases a custom cluster endpoint of a PolarDB cluster.
+        
+        @param request: DeleteDBClusterEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBClusterEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
             query['DBEndpointId'] = request.dbendpoint_id
         if not UtilClient.is_unset(request.owner_account):
@@ -3031,32 +3507,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dbcluster_endpoint(
         self,
         request: polardb_20170801_models.DeleteDBClusterEndpointRequest,
     ) -> polardb_20170801_models.DeleteDBClusterEndpointResponse:
+        """
+        @summary Releases a custom cluster endpoint of a PolarDB cluster.
+        
+        @param request: DeleteDBClusterEndpointRequest
+        @return: DeleteDBClusterEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dbcluster_endpoint_with_options(request, runtime)
 
     async def delete_dbcluster_endpoint_async(
         self,
         request: polardb_20170801_models.DeleteDBClusterEndpointRequest,
     ) -> polardb_20170801_models.DeleteDBClusterEndpointResponse:
+        """
+        @summary Releases a custom cluster endpoint of a PolarDB cluster.
+        
+        @param request: DeleteDBClusterEndpointRequest
+        @return: DeleteDBClusterEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dbcluster_endpoint_with_options_async(request, runtime)
 
     def delete_dbendpoint_address_with_options(
         self,
         request: polardb_20170801_models.DeleteDBEndpointAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBEndpointAddressResponse:
         """
-        >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
-        > *   Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
+        @summary Releases the public endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, and custom cluster endpoint.
+        
+        @description >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        >    Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
         
         @param request: DeleteDBEndpointAddressRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDBEndpointAddressResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3095,16 +3585,18 @@
 
     async def delete_dbendpoint_address_with_options_async(
         self,
         request: polardb_20170801_models.DeleteDBEndpointAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBEndpointAddressResponse:
         """
-        >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
-        > *   Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
+        @summary Releases the public endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, and custom cluster endpoint.
+        
+        @description >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        >    Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
         
         @param request: DeleteDBEndpointAddressRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDBEndpointAddressResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3142,42 +3634,53 @@
         )
 
     def delete_dbendpoint_address(
         self,
         request: polardb_20170801_models.DeleteDBEndpointAddressRequest,
     ) -> polardb_20170801_models.DeleteDBEndpointAddressResponse:
         """
-        >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
-        > *   Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
+        @summary Releases the public endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, and custom cluster endpoint.
+        
+        @description >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        >    Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
         
         @param request: DeleteDBEndpointAddressRequest
         @return: DeleteDBEndpointAddressResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_dbendpoint_address_with_options(request, runtime)
 
     async def delete_dbendpoint_address_async(
         self,
         request: polardb_20170801_models.DeleteDBEndpointAddressRequest,
     ) -> polardb_20170801_models.DeleteDBEndpointAddressResponse:
         """
-        >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
-        > *   Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
+        @summary Releases the public endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, and custom cluster endpoint.
+        
+        @description >    You can delete a public-facing or classic network endpoint of the primary endpoint, the default cluster endpoint, or a custom cluster endpoint.
+        >    Classic network endpoints are supported only on the China site (aliyun.com). Therefore, you do not need to delete classic network endpoints on the International site (alibabacloud.com).
         
         @param request: DeleteDBEndpointAddressRequest
         @return: DeleteDBEndpointAddressResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dbendpoint_address_with_options_async(request, runtime)
 
     def delete_dblink_with_options(
         self,
         request: polardb_20170801_models.DeleteDBLinkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBLinkResponse:
+        """
+        @summary Deletes a database link from a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @param request: DeleteDBLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBLinkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dblink_name):
             query['DBLinkName'] = request.dblink_name
         if not UtilClient.is_unset(request.owner_account):
@@ -3208,14 +3711,21 @@
         )
 
     async def delete_dblink_with_options_async(
         self,
         request: polardb_20170801_models.DeleteDBLinkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBLinkResponse:
+        """
+        @summary Deletes a database link from a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @param request: DeleteDBLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBLinkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dblink_name):
             query['DBLinkName'] = request.dblink_name
         if not UtilClient.is_unset(request.owner_account):
@@ -3245,29 +3755,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dblink(
         self,
         request: polardb_20170801_models.DeleteDBLinkRequest,
     ) -> polardb_20170801_models.DeleteDBLinkResponse:
+        """
+        @summary Deletes a database link from a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @param request: DeleteDBLinkRequest
+        @return: DeleteDBLinkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dblink_with_options(request, runtime)
 
     async def delete_dblink_async(
         self,
         request: polardb_20170801_models.DeleteDBLinkRequest,
     ) -> polardb_20170801_models.DeleteDBLinkResponse:
+        """
+        @summary Deletes a database link from a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @param request: DeleteDBLinkRequest
+        @return: DeleteDBLinkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dblink_with_options_async(request, runtime)
 
     def delete_dbnodes_with_options(
         self,
         request: polardb_20170801_models.DeleteDBNodesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBNodesResponse:
+        """
+        @summary Deletes a read-only node from a PolarDB cluster.
+        
+        @param request: DeleteDBNodesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBNodesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_id):
@@ -3302,14 +3831,21 @@
         )
 
     async def delete_dbnodes_with_options_async(
         self,
         request: polardb_20170801_models.DeleteDBNodesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDBNodesResponse:
+        """
+        @summary Deletes a read-only node from a PolarDB cluster.
+        
+        @param request: DeleteDBNodesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDBNodesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_id):
@@ -3343,31 +3879,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dbnodes(
         self,
         request: polardb_20170801_models.DeleteDBNodesRequest,
     ) -> polardb_20170801_models.DeleteDBNodesResponse:
+        """
+        @summary Deletes a read-only node from a PolarDB cluster.
+        
+        @param request: DeleteDBNodesRequest
+        @return: DeleteDBNodesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dbnodes_with_options(request, runtime)
 
     async def delete_dbnodes_async(
         self,
         request: polardb_20170801_models.DeleteDBNodesRequest,
     ) -> polardb_20170801_models.DeleteDBNodesResponse:
+        """
+        @summary Deletes a read-only node from a PolarDB cluster.
+        
+        @param request: DeleteDBNodesRequest
+        @return: DeleteDBNodesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dbnodes_with_options_async(request, runtime)
 
     def delete_database_with_options(
         self,
         request: polardb_20170801_models.DeleteDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDatabaseResponse:
         """
-        >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
+        @summary Deletes a database from a PolarDB cluster.
+        
+        @description >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
         >- The delete operation is performed in an asynchronous manner. A long period of time may be required to delete a large database. A success response for this operation only indicates that the request to delete the database is sent. You must query the database to check whether the database is deleted.
         
         @param request: DeleteDatabaseRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDatabaseResponse
         """
         UtilClient.validate_model(request)
@@ -3405,15 +3955,17 @@
 
     async def delete_database_with_options_async(
         self,
         request: polardb_20170801_models.DeleteDatabaseRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteDatabaseResponse:
         """
-        >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
+        @summary Deletes a database from a PolarDB cluster.
+        
+        @description >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
         >- The delete operation is performed in an asynchronous manner. A long period of time may be required to delete a large database. A success response for this operation only indicates that the request to delete the database is sent. You must query the database to check whether the database is deleted.
         
         @param request: DeleteDatabaseRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteDatabaseResponse
         """
         UtilClient.validate_model(request)
@@ -3450,44 +4002,50 @@
         )
 
     def delete_database(
         self,
         request: polardb_20170801_models.DeleteDatabaseRequest,
     ) -> polardb_20170801_models.DeleteDatabaseResponse:
         """
-        >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
+        @summary Deletes a database from a PolarDB cluster.
+        
+        @description >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
         >- The delete operation is performed in an asynchronous manner. A long period of time may be required to delete a large database. A success response for this operation only indicates that the request to delete the database is sent. You must query the database to check whether the database is deleted.
         
         @param request: DeleteDatabaseRequest
         @return: DeleteDatabaseResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_database_with_options(request, runtime)
 
     async def delete_database_async(
         self,
         request: polardb_20170801_models.DeleteDatabaseRequest,
     ) -> polardb_20170801_models.DeleteDatabaseResponse:
         """
-        >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
+        @summary Deletes a database from a PolarDB cluster.
+        
+        @description >- The cluster must be in the Running state and unlocked. Otherwise, the specified database cannot be deleted.
         >- The delete operation is performed in an asynchronous manner. A long period of time may be required to delete a large database. A success response for this operation only indicates that the request to delete the database is sent. You must query the database to check whether the database is deleted.
         
         @param request: DeleteDatabaseRequest
         @return: DeleteDatabaseResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_database_with_options_async(request, runtime)
 
     def delete_global_database_network_with_options(
         self,
         request: polardb_20170801_models.DeleteGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteGlobalDatabaseNetworkResponse:
         """
-        >  You can delete a GDN only when the GDN includes only a primary cluster.
+        @summary Deletes a global database network (GDN).
+        
+        @description >  You can delete a GDN only when the GDN includes only a primary cluster.
         
         @param request: DeleteGlobalDatabaseNetworkRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteGlobalDatabaseNetworkResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3526,15 +4084,17 @@
 
     async def delete_global_database_network_with_options_async(
         self,
         request: polardb_20170801_models.DeleteGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteGlobalDatabaseNetworkResponse:
         """
-        >  You can delete a GDN only when the GDN includes only a primary cluster.
+        @summary Deletes a global database network (GDN).
+        
+        @description >  You can delete a GDN only when the GDN includes only a primary cluster.
         
         @param request: DeleteGlobalDatabaseNetworkRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteGlobalDatabaseNetworkResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3572,40 +4132,51 @@
         )
 
     def delete_global_database_network(
         self,
         request: polardb_20170801_models.DeleteGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.DeleteGlobalDatabaseNetworkResponse:
         """
-        >  You can delete a GDN only when the GDN includes only a primary cluster.
+        @summary Deletes a global database network (GDN).
+        
+        @description >  You can delete a GDN only when the GDN includes only a primary cluster.
         
         @param request: DeleteGlobalDatabaseNetworkRequest
         @return: DeleteGlobalDatabaseNetworkResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_global_database_network_with_options(request, runtime)
 
     async def delete_global_database_network_async(
         self,
         request: polardb_20170801_models.DeleteGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.DeleteGlobalDatabaseNetworkResponse:
         """
-        >  You can delete a GDN only when the GDN includes only a primary cluster.
+        @summary Deletes a global database network (GDN).
+        
+        @description >  You can delete a GDN only when the GDN includes only a primary cluster.
         
         @param request: DeleteGlobalDatabaseNetworkRequest
         @return: DeleteGlobalDatabaseNetworkResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_global_database_network_with_options_async(request, runtime)
 
     def delete_global_security_ipgroup_with_options(
         self,
         request: polardb_20170801_models.DeleteGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteGlobalSecurityIPGroupResponse:
+        """
+        @summary Deletes a global IP whitelist template.
+        
+        @param request: DeleteGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -3642,14 +4213,21 @@
         )
 
     async def delete_global_security_ipgroup_with_options_async(
         self,
         request: polardb_20170801_models.DeleteGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteGlobalSecurityIPGroupResponse:
+        """
+        @summary Deletes a global IP whitelist template.
+        
+        @param request: DeleteGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -3685,29 +4263,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_global_security_ipgroup(
         self,
         request: polardb_20170801_models.DeleteGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.DeleteGlobalSecurityIPGroupResponse:
+        """
+        @summary Deletes a global IP whitelist template.
+        
+        @param request: DeleteGlobalSecurityIPGroupRequest
+        @return: DeleteGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_global_security_ipgroup_with_options(request, runtime)
 
     async def delete_global_security_ipgroup_async(
         self,
         request: polardb_20170801_models.DeleteGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.DeleteGlobalSecurityIPGroupResponse:
+        """
+        @summary Deletes a global IP whitelist template.
+        
+        @param request: DeleteGlobalSecurityIPGroupRequest
+        @return: DeleteGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_global_security_ipgroup_with_options_async(request, runtime)
 
     def delete_masking_rules_with_options(
         self,
         request: polardb_20170801_models.DeleteMaskingRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteMaskingRulesResponse:
+        """
+        @summary Deletes a data masking rule.
+        
+        @param request: DeleteMaskingRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMaskingRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.rule_name_list):
             query['RuleNameList'] = request.rule_name_list
         req = open_api_models.OpenApiRequest(
@@ -3730,14 +4327,21 @@
         )
 
     async def delete_masking_rules_with_options_async(
         self,
         request: polardb_20170801_models.DeleteMaskingRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteMaskingRulesResponse:
+        """
+        @summary Deletes a data masking rule.
+        
+        @param request: DeleteMaskingRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMaskingRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.rule_name_list):
             query['RuleNameList'] = request.rule_name_list
         req = open_api_models.OpenApiRequest(
@@ -3759,31 +4363,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_masking_rules(
         self,
         request: polardb_20170801_models.DeleteMaskingRulesRequest,
     ) -> polardb_20170801_models.DeleteMaskingRulesResponse:
+        """
+        @summary Deletes a data masking rule.
+        
+        @param request: DeleteMaskingRulesRequest
+        @return: DeleteMaskingRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_masking_rules_with_options(request, runtime)
 
     async def delete_masking_rules_async(
         self,
         request: polardb_20170801_models.DeleteMaskingRulesRequest,
     ) -> polardb_20170801_models.DeleteMaskingRulesResponse:
+        """
+        @summary Deletes a data masking rule.
+        
+        @param request: DeleteMaskingRulesRequest
+        @return: DeleteMaskingRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_masking_rules_with_options_async(request, runtime)
 
     def delete_parameter_group_with_options(
         self,
         request: polardb_20170801_models.DeleteParameterGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Deletes a parameter template of a PolarDB cluster.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         >  When you delete a parameter template, the parameter settings that are applied to PolarDB clusters are not affected.
         
         @param request: DeleteParameterGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteParameterGroupResponse
         """
         UtilClient.validate_model(request)
@@ -3823,15 +4441,17 @@
 
     async def delete_parameter_group_with_options_async(
         self,
         request: polardb_20170801_models.DeleteParameterGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DeleteParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Deletes a parameter template of a PolarDB cluster.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         >  When you delete a parameter template, the parameter settings that are applied to PolarDB clusters are not affected.
         
         @param request: DeleteParameterGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteParameterGroupResponse
         """
         UtilClient.validate_model(request)
@@ -3870,42 +4490,53 @@
         )
 
     def delete_parameter_group(
         self,
         request: polardb_20170801_models.DeleteParameterGroupRequest,
     ) -> polardb_20170801_models.DeleteParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Deletes a parameter template of a PolarDB cluster.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         >  When you delete a parameter template, the parameter settings that are applied to PolarDB clusters are not affected.
         
         @param request: DeleteParameterGroupRequest
         @return: DeleteParameterGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_parameter_group_with_options(request, runtime)
 
     async def delete_parameter_group_async(
         self,
         request: polardb_20170801_models.DeleteParameterGroupRequest,
     ) -> polardb_20170801_models.DeleteParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Deletes a parameter template of a PolarDB cluster.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and quickly apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         >  When you delete a parameter template, the parameter settings that are applied to PolarDB clusters are not affected.
         
         @param request: DeleteParameterGroupRequest
         @return: DeleteParameterGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_parameter_group_with_options_async(request, runtime)
 
     def describe_aitask_status_with_options(
         self,
         request: polardb_20170801_models.DescribeAITaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeAITaskStatusResponse:
+        """
+        @summary Queries the state of the PolarDB for AI feature for a cluster.
+        
+        @param request: DescribeAITaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAITaskStatusResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeAITaskStatus',
@@ -3924,14 +4555,21 @@
         )
 
     async def describe_aitask_status_with_options_async(
         self,
         request: polardb_20170801_models.DescribeAITaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeAITaskStatusResponse:
+        """
+        @summary Queries the state of the PolarDB for AI feature for a cluster.
+        
+        @param request: DescribeAITaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAITaskStatusResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeAITaskStatus',
@@ -3949,29 +4587,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_aitask_status(
         self,
         request: polardb_20170801_models.DescribeAITaskStatusRequest,
     ) -> polardb_20170801_models.DescribeAITaskStatusResponse:
+        """
+        @summary Queries the state of the PolarDB for AI feature for a cluster.
+        
+        @param request: DescribeAITaskStatusRequest
+        @return: DescribeAITaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_aitask_status_with_options(request, runtime)
 
     async def describe_aitask_status_async(
         self,
         request: polardb_20170801_models.DescribeAITaskStatusRequest,
     ) -> polardb_20170801_models.DescribeAITaskStatusResponse:
+        """
+        @summary Queries the state of the PolarDB for AI feature for a cluster.
+        
+        @param request: DescribeAITaskStatusRequest
+        @return: DescribeAITaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_aitask_status_with_options_async(request, runtime)
 
     def describe_accounts_with_options(
         self,
         request: polardb_20170801_models.DescribeAccountsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeAccountsResponse:
+        """
+        @summary Queries information about a database account of a PolarDB cluster.
+        
+        @param request: DescribeAccountsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAccountsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -4006,14 +4663,21 @@
         )
 
     async def describe_accounts_with_options_async(
         self,
         request: polardb_20170801_models.DescribeAccountsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeAccountsResponse:
+        """
+        @summary Queries information about a database account of a PolarDB cluster.
+        
+        @param request: DescribeAccountsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAccountsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -4047,29 +4711,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_accounts(
         self,
         request: polardb_20170801_models.DescribeAccountsRequest,
     ) -> polardb_20170801_models.DescribeAccountsResponse:
+        """
+        @summary Queries information about a database account of a PolarDB cluster.
+        
+        @param request: DescribeAccountsRequest
+        @return: DescribeAccountsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_accounts_with_options(request, runtime)
 
     async def describe_accounts_async(
         self,
         request: polardb_20170801_models.DescribeAccountsRequest,
     ) -> polardb_20170801_models.DescribeAccountsResponse:
+        """
+        @summary Queries information about a database account of a PolarDB cluster.
+        
+        @param request: DescribeAccountsRequest
+        @return: DescribeAccountsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_accounts_with_options_async(request, runtime)
 
     def describe_auto_renew_attribute_with_options(
         self,
         request: polardb_20170801_models.DescribeAutoRenewAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeAutoRenewAttributeResponse:
+        """
+        @summary Queries the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: DescribeAutoRenewAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAutoRenewAttributeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_ids):
             query['DBClusterIds'] = request.dbcluster_ids
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4106,14 +4789,21 @@
         )
 
     async def describe_auto_renew_attribute_with_options_async(
         self,
         request: polardb_20170801_models.DescribeAutoRenewAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeAutoRenewAttributeResponse:
+        """
+        @summary Queries the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: DescribeAutoRenewAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAutoRenewAttributeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_ids):
             query['DBClusterIds'] = request.dbcluster_ids
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4149,29 +4839,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_auto_renew_attribute(
         self,
         request: polardb_20170801_models.DescribeAutoRenewAttributeRequest,
     ) -> polardb_20170801_models.DescribeAutoRenewAttributeResponse:
+        """
+        @summary Queries the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: DescribeAutoRenewAttributeRequest
+        @return: DescribeAutoRenewAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_auto_renew_attribute_with_options(request, runtime)
 
     async def describe_auto_renew_attribute_async(
         self,
         request: polardb_20170801_models.DescribeAutoRenewAttributeRequest,
     ) -> polardb_20170801_models.DescribeAutoRenewAttributeResponse:
+        """
+        @summary Queries the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: DescribeAutoRenewAttributeRequest
+        @return: DescribeAutoRenewAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_auto_renew_attribute_with_options_async(request, runtime)
 
     def describe_backup_logs_with_options(
         self,
         request: polardb_20170801_models.DescribeBackupLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupLogsResponse:
+        """
+        @summary Queries backup logs and the URLs to download the backup logs.
+        
+        @param request: DescribeBackupLogsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupLogsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_region):
             query['BackupRegion'] = request.backup_region
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.end_time):
@@ -4210,14 +4919,21 @@
         )
 
     async def describe_backup_logs_with_options_async(
         self,
         request: polardb_20170801_models.DescribeBackupLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupLogsResponse:
+        """
+        @summary Queries backup logs and the URLs to download the backup logs.
+        
+        @param request: DescribeBackupLogsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupLogsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_region):
             query['BackupRegion'] = request.backup_region
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.end_time):
@@ -4255,29 +4971,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_backup_logs(
         self,
         request: polardb_20170801_models.DescribeBackupLogsRequest,
     ) -> polardb_20170801_models.DescribeBackupLogsResponse:
+        """
+        @summary Queries backup logs and the URLs to download the backup logs.
+        
+        @param request: DescribeBackupLogsRequest
+        @return: DescribeBackupLogsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_logs_with_options(request, runtime)
 
     async def describe_backup_logs_async(
         self,
         request: polardb_20170801_models.DescribeBackupLogsRequest,
     ) -> polardb_20170801_models.DescribeBackupLogsResponse:
+        """
+        @summary Queries backup logs and the URLs to download the backup logs.
+        
+        @param request: DescribeBackupLogsRequest
+        @return: DescribeBackupLogsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_backup_logs_with_options_async(request, runtime)
 
     def describe_backup_policy_with_options(
         self,
         request: polardb_20170801_models.DescribeBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupPolicyResponse:
+        """
+        @summary Queries the automatic backup policy of a PolarDB cluster.
+        
+        @param request: DescribeBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4306,14 +5041,21 @@
         )
 
     async def describe_backup_policy_with_options_async(
         self,
         request: polardb_20170801_models.DescribeBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupPolicyResponse:
+        """
+        @summary Queries the automatic backup policy of a PolarDB cluster.
+        
+        @param request: DescribeBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4341,29 +5083,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_backup_policy(
         self,
         request: polardb_20170801_models.DescribeBackupPolicyRequest,
     ) -> polardb_20170801_models.DescribeBackupPolicyResponse:
+        """
+        @summary Queries the automatic backup policy of a PolarDB cluster.
+        
+        @param request: DescribeBackupPolicyRequest
+        @return: DescribeBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_policy_with_options(request, runtime)
 
     async def describe_backup_policy_async(
         self,
         request: polardb_20170801_models.DescribeBackupPolicyRequest,
     ) -> polardb_20170801_models.DescribeBackupPolicyResponse:
+        """
+        @summary Queries the automatic backup policy of a PolarDB cluster.
+        
+        @param request: DescribeBackupPolicyRequest
+        @return: DescribeBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_backup_policy_with_options_async(request, runtime)
 
     def describe_backup_tasks_with_options(
         self,
         request: polardb_20170801_models.DescribeBackupTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupTasksResponse:
+        """
+        @summary Queries the backup tasks of a PolarDB cluster.
+        
+        @param request: DescribeBackupTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_job_id):
             query['BackupJobId'] = request.backup_job_id
         if not UtilClient.is_unset(request.backup_mode):
             query['BackupMode'] = request.backup_mode
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -4396,14 +5157,21 @@
         )
 
     async def describe_backup_tasks_with_options_async(
         self,
         request: polardb_20170801_models.DescribeBackupTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupTasksResponse:
+        """
+        @summary Queries the backup tasks of a PolarDB cluster.
+        
+        @param request: DescribeBackupTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_job_id):
             query['BackupJobId'] = request.backup_job_id
         if not UtilClient.is_unset(request.backup_mode):
             query['BackupMode'] = request.backup_mode
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -4435,29 +5203,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_backup_tasks(
         self,
         request: polardb_20170801_models.DescribeBackupTasksRequest,
     ) -> polardb_20170801_models.DescribeBackupTasksResponse:
+        """
+        @summary Queries the backup tasks of a PolarDB cluster.
+        
+        @param request: DescribeBackupTasksRequest
+        @return: DescribeBackupTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_tasks_with_options(request, runtime)
 
     async def describe_backup_tasks_async(
         self,
         request: polardb_20170801_models.DescribeBackupTasksRequest,
     ) -> polardb_20170801_models.DescribeBackupTasksResponse:
+        """
+        @summary Queries the backup tasks of a PolarDB cluster.
+        
+        @param request: DescribeBackupTasksRequest
+        @return: DescribeBackupTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_backup_tasks_with_options_async(request, runtime)
 
     def describe_backups_with_options(
         self,
         request: polardb_20170801_models.DescribeBackupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupsResponse:
+        """
+        @summary Queries the backup details of a PolarDB cluster.
+        
+        @param request: DescribeBackupsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.backup_mode):
             query['BackupMode'] = request.backup_mode
         if not UtilClient.is_unset(request.backup_region):
@@ -4502,14 +5289,21 @@
         )
 
     async def describe_backups_with_options_async(
         self,
         request: polardb_20170801_models.DescribeBackupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeBackupsResponse:
+        """
+        @summary Queries the backup details of a PolarDB cluster.
+        
+        @param request: DescribeBackupsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.backup_mode):
             query['BackupMode'] = request.backup_mode
         if not UtilClient.is_unset(request.backup_region):
@@ -4553,29 +5347,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_backups(
         self,
         request: polardb_20170801_models.DescribeBackupsRequest,
     ) -> polardb_20170801_models.DescribeBackupsResponse:
+        """
+        @summary Queries the backup details of a PolarDB cluster.
+        
+        @param request: DescribeBackupsRequest
+        @return: DescribeBackupsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_backups_with_options(request, runtime)
 
     async def describe_backups_async(
         self,
         request: polardb_20170801_models.DescribeBackupsRequest,
     ) -> polardb_20170801_models.DescribeBackupsResponse:
+        """
+        @summary Queries the backup details of a PolarDB cluster.
+        
+        @param request: DescribeBackupsRequest
+        @return: DescribeBackupsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_backups_with_options_async(request, runtime)
 
     def describe_character_set_name_with_options(
         self,
         request: polardb_20170801_models.DescribeCharacterSetNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeCharacterSetNameResponse:
+        """
+        @summary Queries character sets that are supported by a PolarDB for MySQL cluster.
+        
+        @param request: DescribeCharacterSetNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCharacterSetNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4606,14 +5419,21 @@
         )
 
     async def describe_character_set_name_with_options_async(
         self,
         request: polardb_20170801_models.DescribeCharacterSetNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeCharacterSetNameResponse:
+        """
+        @summary Queries character sets that are supported by a PolarDB for MySQL cluster.
+        
+        @param request: DescribeCharacterSetNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCharacterSetNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4643,29 +5463,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_character_set_name(
         self,
         request: polardb_20170801_models.DescribeCharacterSetNameRequest,
     ) -> polardb_20170801_models.DescribeCharacterSetNameResponse:
+        """
+        @summary Queries character sets that are supported by a PolarDB for MySQL cluster.
+        
+        @param request: DescribeCharacterSetNameRequest
+        @return: DescribeCharacterSetNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_character_set_name_with_options(request, runtime)
 
     async def describe_character_set_name_async(
         self,
         request: polardb_20170801_models.DescribeCharacterSetNameRequest,
     ) -> polardb_20170801_models.DescribeCharacterSetNameResponse:
+        """
+        @summary Queries character sets that are supported by a PolarDB for MySQL cluster.
+        
+        @param request: DescribeCharacterSetNameRequest
+        @return: DescribeCharacterSetNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_character_set_name_with_options_async(request, runtime)
 
     def describe_class_list_with_options(
         self,
         request: polardb_20170801_models.DescribeClassListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeClassListResponse:
+        """
+        @summary Queries the specifications of a cluster.
+        
+        @param request: DescribeClassListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeClassListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.commodity_code):
             query['CommodityCode'] = request.commodity_code
         if not UtilClient.is_unset(request.master_ha):
             query['MasterHa'] = request.master_ha
         if not UtilClient.is_unset(request.order_type):
@@ -4702,14 +5541,21 @@
         )
 
     async def describe_class_list_with_options_async(
         self,
         request: polardb_20170801_models.DescribeClassListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeClassListResponse:
+        """
+        @summary Queries the specifications of a cluster.
+        
+        @param request: DescribeClassListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeClassListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.commodity_code):
             query['CommodityCode'] = request.commodity_code
         if not UtilClient.is_unset(request.master_ha):
             query['MasterHa'] = request.master_ha
         if not UtilClient.is_unset(request.order_type):
@@ -4745,29 +5591,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_class_list(
         self,
         request: polardb_20170801_models.DescribeClassListRequest,
     ) -> polardb_20170801_models.DescribeClassListResponse:
+        """
+        @summary Queries the specifications of a cluster.
+        
+        @param request: DescribeClassListRequest
+        @return: DescribeClassListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_class_list_with_options(request, runtime)
 
     async def describe_class_list_async(
         self,
         request: polardb_20170801_models.DescribeClassListRequest,
     ) -> polardb_20170801_models.DescribeClassListResponse:
+        """
+        @summary Queries the specifications of a cluster.
+        
+        @param request: DescribeClassListRequest
+        @return: DescribeClassListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_class_list_with_options_async(request, runtime)
 
     def describe_dbcluster_access_whitelist_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterAccessWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAccessWhitelistResponse:
+        """
+        @summary Queries the IP address whitelists and security groups of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAccessWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAccessWhitelistResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4796,14 +5661,21 @@
         )
 
     async def describe_dbcluster_access_whitelist_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAccessWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAccessWhitelistResponse:
+        """
+        @summary Queries the IP address whitelists and security groups of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAccessWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAccessWhitelistResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4831,29 +5703,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_access_whitelist(
         self,
         request: polardb_20170801_models.DescribeDBClusterAccessWhitelistRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAccessWhitelistResponse:
+        """
+        @summary Queries the IP address whitelists and security groups of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAccessWhitelistRequest
+        @return: DescribeDBClusterAccessWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_access_whitelist_with_options(request, runtime)
 
     async def describe_dbcluster_access_whitelist_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAccessWhitelistRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAccessWhitelistResponse:
+        """
+        @summary Queries the IP address whitelists and security groups of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAccessWhitelistRequest
+        @return: DescribeDBClusterAccessWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_access_whitelist_with_options_async(request, runtime)
 
     def describe_dbcluster_attribute_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAttributeResponse:
+        """
+        @summary Queries information about a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAttributeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.describe_type):
             query['DescribeType'] = request.describe_type
         if not UtilClient.is_unset(request.owner_account):
@@ -4884,14 +5775,21 @@
         )
 
     async def describe_dbcluster_attribute_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAttributeResponse:
+        """
+        @summary Queries information about a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAttributeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.describe_type):
             query['DescribeType'] = request.describe_type
         if not UtilClient.is_unset(request.owner_account):
@@ -4921,29 +5819,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_attribute(
         self,
         request: polardb_20170801_models.DescribeDBClusterAttributeRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAttributeResponse:
+        """
+        @summary Queries information about a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAttributeRequest
+        @return: DescribeDBClusterAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_attribute_with_options(request, runtime)
 
     async def describe_dbcluster_attribute_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAttributeRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAttributeResponse:
+        """
+        @summary Queries information about a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAttributeRequest
+        @return: DescribeDBClusterAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_attribute_with_options_async(request, runtime)
 
     def describe_dbcluster_audit_log_collector_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterAuditLogCollectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAuditLogCollectorResponse:
+        """
+        @summary Describe SQL collector for a PolarDB cluster. Features related to SQL collector include audit log and SQL Explorer.
+        
+        @param request: DescribeDBClusterAuditLogCollectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAuditLogCollectorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -4972,14 +5889,21 @@
         )
 
     async def describe_dbcluster_audit_log_collector_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAuditLogCollectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAuditLogCollectorResponse:
+        """
+        @summary Describe SQL collector for a PolarDB cluster. Features related to SQL collector include audit log and SQL Explorer.
+        
+        @param request: DescribeDBClusterAuditLogCollectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAuditLogCollectorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5007,29 +5931,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_audit_log_collector(
         self,
         request: polardb_20170801_models.DescribeDBClusterAuditLogCollectorRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAuditLogCollectorResponse:
+        """
+        @summary Describe SQL collector for a PolarDB cluster. Features related to SQL collector include audit log and SQL Explorer.
+        
+        @param request: DescribeDBClusterAuditLogCollectorRequest
+        @return: DescribeDBClusterAuditLogCollectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_audit_log_collector_with_options(request, runtime)
 
     async def describe_dbcluster_audit_log_collector_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAuditLogCollectorRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAuditLogCollectorResponse:
+        """
+        @summary Describe SQL collector for a PolarDB cluster. Features related to SQL collector include audit log and SQL Explorer.
+        
+        @param request: DescribeDBClusterAuditLogCollectorRequest
+        @return: DescribeDBClusterAuditLogCollectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_audit_log_collector_with_options_async(request, runtime)
 
     def describe_dbcluster_available_resources_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterAvailableResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAvailableResourcesResponse:
+        """
+        @summary Queries available resources in a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAvailableResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAvailableResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbnode_class):
             query['DBNodeClass'] = request.dbnode_class
         if not UtilClient.is_unset(request.dbtype):
             query['DBType'] = request.dbtype
         if not UtilClient.is_unset(request.dbversion):
@@ -5068,14 +6011,21 @@
         )
 
     async def describe_dbcluster_available_resources_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAvailableResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterAvailableResourcesResponse:
+        """
+        @summary Queries available resources in a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAvailableResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterAvailableResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbnode_class):
             query['DBNodeClass'] = request.dbnode_class
         if not UtilClient.is_unset(request.dbtype):
             query['DBType'] = request.dbtype
         if not UtilClient.is_unset(request.dbversion):
@@ -5113,29 +6063,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_available_resources(
         self,
         request: polardb_20170801_models.DescribeDBClusterAvailableResourcesRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAvailableResourcesResponse:
+        """
+        @summary Queries available resources in a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAvailableResourcesRequest
+        @return: DescribeDBClusterAvailableResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_available_resources_with_options(request, runtime)
 
     async def describe_dbcluster_available_resources_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterAvailableResourcesRequest,
     ) -> polardb_20170801_models.DescribeDBClusterAvailableResourcesResponse:
+        """
+        @summary Queries available resources in a PolarDB cluster.
+        
+        @param request: DescribeDBClusterAvailableResourcesRequest
+        @return: DescribeDBClusterAvailableResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_available_resources_with_options_async(request, runtime)
 
     def describe_dbcluster_connectivity_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterConnectivityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterConnectivityResponse:
+        """
+        @summary Queries whether the source IP address can access a cluster.
+        
+        @param request: DescribeDBClusterConnectivityRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterConnectivityResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5170,14 +6139,21 @@
         )
 
     async def describe_dbcluster_connectivity_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterConnectivityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterConnectivityResponse:
+        """
+        @summary Queries whether the source IP address can access a cluster.
+        
+        @param request: DescribeDBClusterConnectivityRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterConnectivityResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5211,29 +6187,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_connectivity(
         self,
         request: polardb_20170801_models.DescribeDBClusterConnectivityRequest,
     ) -> polardb_20170801_models.DescribeDBClusterConnectivityResponse:
+        """
+        @summary Queries whether the source IP address can access a cluster.
+        
+        @param request: DescribeDBClusterConnectivityRequest
+        @return: DescribeDBClusterConnectivityResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_connectivity_with_options(request, runtime)
 
     async def describe_dbcluster_connectivity_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterConnectivityRequest,
     ) -> polardb_20170801_models.DescribeDBClusterConnectivityResponse:
+        """
+        @summary Queries whether the source IP address can access a cluster.
+        
+        @param request: DescribeDBClusterConnectivityRequest
+        @return: DescribeDBClusterConnectivityResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_connectivity_with_options_async(request, runtime)
 
     def describe_dbcluster_endpoints_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterEndpointsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterEndpointsResponse:
+        """
+        @summary Queries the endpoints of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterEndpointsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterEndpointsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
             query['DBEndpointId'] = request.dbendpoint_id
         if not UtilClient.is_unset(request.describe_type):
@@ -5266,14 +6261,21 @@
         )
 
     async def describe_dbcluster_endpoints_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterEndpointsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterEndpointsResponse:
+        """
+        @summary Queries the endpoints of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterEndpointsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterEndpointsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
             query['DBEndpointId'] = request.dbendpoint_id
         if not UtilClient.is_unset(request.describe_type):
@@ -5305,32 +6307,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_endpoints(
         self,
         request: polardb_20170801_models.DescribeDBClusterEndpointsRequest,
     ) -> polardb_20170801_models.DescribeDBClusterEndpointsResponse:
+        """
+        @summary Queries the endpoints of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterEndpointsRequest
+        @return: DescribeDBClusterEndpointsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_endpoints_with_options(request, runtime)
 
     async def describe_dbcluster_endpoints_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterEndpointsRequest,
     ) -> polardb_20170801_models.DescribeDBClusterEndpointsResponse:
+        """
+        @summary Queries the endpoints of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterEndpointsRequest
+        @return: DescribeDBClusterEndpointsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_endpoints_with_options_async(request, runtime)
 
     def describe_dbcluster_migration_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterMigrationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterMigrationResponse:
         """
-        You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](~~121582~~).
-        *   Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
+        @summary Queries the migration status of PolarDB clusters.
+        
+        @description    You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](https://help.aliyun.com/document_detail/121582.html).
+        Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
         
         @param request: DescribeDBClusterMigrationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBClusterMigrationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5365,16 +6381,18 @@
 
     async def describe_dbcluster_migration_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterMigrationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterMigrationResponse:
         """
-        You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](~~121582~~).
-        *   Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
+        @summary Queries the migration status of PolarDB clusters.
+        
+        @description    You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](https://help.aliyun.com/document_detail/121582.html).
+        Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
         
         @param request: DescribeDBClusterMigrationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBClusterMigrationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5408,42 +6426,53 @@
         )
 
     def describe_dbcluster_migration(
         self,
         request: polardb_20170801_models.DescribeDBClusterMigrationRequest,
     ) -> polardb_20170801_models.DescribeDBClusterMigrationResponse:
         """
-        You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](~~121582~~).
-        *   Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
+        @summary Queries the migration status of PolarDB clusters.
+        
+        @description    You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](https://help.aliyun.com/document_detail/121582.html).
+        Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
         
         @param request: DescribeDBClusterMigrationRequest
         @return: DescribeDBClusterMigrationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_migration_with_options(request, runtime)
 
     async def describe_dbcluster_migration_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterMigrationRequest,
     ) -> polardb_20170801_models.DescribeDBClusterMigrationResponse:
         """
-        You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](~~121582~~).
-        *   Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
+        @summary Queries the migration status of PolarDB clusters.
+        
+        @description    You can call this operation to query the status of data migration from an ApsaraDB RDS instance to a PolarDB cluster. For more information, see [Upgrade ApsaraDB RDS for MySQL to PolarDB for MySQL with one click](https://help.aliyun.com/document_detail/121582.html).
+        Before you call this operation, make sure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**.
         
         @param request: DescribeDBClusterMigrationRequest
         @return: DescribeDBClusterMigrationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_migration_with_options_async(request, runtime)
 
     def describe_dbcluster_monitor_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterMonitorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterMonitorResponse:
+        """
+        @summary Queries the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @param request: DescribeDBClusterMonitorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterMonitorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5472,14 +6501,21 @@
         )
 
     async def describe_dbcluster_monitor_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterMonitorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterMonitorResponse:
+        """
+        @summary Queries the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @param request: DescribeDBClusterMonitorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterMonitorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5507,29 +6543,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_monitor(
         self,
         request: polardb_20170801_models.DescribeDBClusterMonitorRequest,
     ) -> polardb_20170801_models.DescribeDBClusterMonitorResponse:
+        """
+        @summary Queries the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @param request: DescribeDBClusterMonitorRequest
+        @return: DescribeDBClusterMonitorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_monitor_with_options(request, runtime)
 
     async def describe_dbcluster_monitor_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterMonitorRequest,
     ) -> polardb_20170801_models.DescribeDBClusterMonitorResponse:
+        """
+        @summary Queries the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @param request: DescribeDBClusterMonitorRequest
+        @return: DescribeDBClusterMonitorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_monitor_with_options_async(request, runtime)
 
     def describe_dbcluster_parameters_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterParametersResponse:
+        """
+        @summary Queries the parameters of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.describe_type):
             query['DescribeType'] = request.describe_type
         if not UtilClient.is_unset(request.owner_account):
@@ -5560,14 +6615,21 @@
         )
 
     async def describe_dbcluster_parameters_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterParametersResponse:
+        """
+        @summary Queries the parameters of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.describe_type):
             query['DescribeType'] = request.describe_type
         if not UtilClient.is_unset(request.owner_account):
@@ -5597,42 +6659,56 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_parameters(
         self,
         request: polardb_20170801_models.DescribeDBClusterParametersRequest,
     ) -> polardb_20170801_models.DescribeDBClusterParametersResponse:
+        """
+        @summary Queries the parameters of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterParametersRequest
+        @return: DescribeDBClusterParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_parameters_with_options(request, runtime)
 
     async def describe_dbcluster_parameters_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterParametersRequest,
     ) -> polardb_20170801_models.DescribeDBClusterParametersResponse:
+        """
+        @summary Queries the parameters of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterParametersRequest
+        @return: DescribeDBClusterParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_parameters_with_options_async(request, runtime)
 
     def describe_dbcluster_performance_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterPerformanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterPerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBClusterPerformanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBClusterPerformanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5667,26 +6743,28 @@
 
     async def describe_dbcluster_performance_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterPerformanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterPerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBClusterPerformanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBClusterPerformanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5720,62 +6798,73 @@
         )
 
     def describe_dbcluster_performance(
         self,
         request: polardb_20170801_models.DescribeDBClusterPerformanceRequest,
     ) -> polardb_20170801_models.DescribeDBClusterPerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBClusterPerformanceRequest
         @return: DescribeDBClusterPerformanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_performance_with_options(request, runtime)
 
     async def describe_dbcluster_performance_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterPerformanceRequest,
     ) -> polardb_20170801_models.DescribeDBClusterPerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBClusterPerformanceRequest
         @return: DescribeDBClusterPerformanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_performance_with_options_async(request, runtime)
 
     def describe_dbcluster_sslwith_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterSSLRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterSSLResponse:
+        """
+        @summary Queries the Secure Sockets Layer (SSL) settings of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterSSLRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterSSLResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5804,14 +6893,21 @@
         )
 
     async def describe_dbcluster_sslwith_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterSSLRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterSSLResponse:
+        """
+        @summary Queries the Secure Sockets Layer (SSL) settings of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterSSLRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterSSLResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5839,29 +6935,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_ssl(
         self,
         request: polardb_20170801_models.DescribeDBClusterSSLRequest,
     ) -> polardb_20170801_models.DescribeDBClusterSSLResponse:
+        """
+        @summary Queries the Secure Sockets Layer (SSL) settings of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterSSLRequest
+        @return: DescribeDBClusterSSLResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_sslwith_options(request, runtime)
 
     async def describe_dbcluster_ssl_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterSSLRequest,
     ) -> polardb_20170801_models.DescribeDBClusterSSLResponse:
+        """
+        @summary Queries the Secure Sockets Layer (SSL) settings of a PolarDB cluster.
+        
+        @param request: DescribeDBClusterSSLRequest
+        @return: DescribeDBClusterSSLResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_sslwith_options_async(request, runtime)
 
     def describe_dbcluster_serverless_conf_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterServerlessConfRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterServerlessConfResponse:
+        """
+        @summary Queries the configurations of a serverless cluster.
+        
+        @param request: DescribeDBClusterServerlessConfRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterServerlessConfResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5890,14 +7005,21 @@
         )
 
     async def describe_dbcluster_serverless_conf_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterServerlessConfRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterServerlessConfResponse:
+        """
+        @summary Queries the configurations of a serverless cluster.
+        
+        @param request: DescribeDBClusterServerlessConfRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterServerlessConfResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5925,29 +7047,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_serverless_conf(
         self,
         request: polardb_20170801_models.DescribeDBClusterServerlessConfRequest,
     ) -> polardb_20170801_models.DescribeDBClusterServerlessConfResponse:
+        """
+        @summary Queries the configurations of a serverless cluster.
+        
+        @param request: DescribeDBClusterServerlessConfRequest
+        @return: DescribeDBClusterServerlessConfResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_serverless_conf_with_options(request, runtime)
 
     async def describe_dbcluster_serverless_conf_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterServerlessConfRequest,
     ) -> polardb_20170801_models.DescribeDBClusterServerlessConfResponse:
+        """
+        @summary Queries the configurations of a serverless cluster.
+        
+        @param request: DescribeDBClusterServerlessConfRequest
+        @return: DescribeDBClusterServerlessConfResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_serverless_conf_with_options_async(request, runtime)
 
     def describe_dbcluster_tdewith_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterTDERequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterTDEResponse:
+        """
+        @summary Queries the Transparent Data Encryption (TDE) settings of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterTDERequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterTDEResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -5976,14 +7117,21 @@
         )
 
     async def describe_dbcluster_tdewith_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterTDERequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterTDEResponse:
+        """
+        @summary Queries the Transparent Data Encryption (TDE) settings of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterTDERequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterTDEResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -6011,29 +7159,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_tde(
         self,
         request: polardb_20170801_models.DescribeDBClusterTDERequest,
     ) -> polardb_20170801_models.DescribeDBClusterTDEResponse:
+        """
+        @summary Queries the Transparent Data Encryption (TDE) settings of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterTDERequest
+        @return: DescribeDBClusterTDEResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_tdewith_options(request, runtime)
 
     async def describe_dbcluster_tde_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterTDERequest,
     ) -> polardb_20170801_models.DescribeDBClusterTDEResponse:
+        """
+        @summary Queries the Transparent Data Encryption (TDE) settings of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterTDERequest
+        @return: DescribeDBClusterTDEResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_tdewith_options_async(request, runtime)
 
     def describe_dbcluster_version_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClusterVersionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterVersionResponse:
+        """
+        @summary Queries the information about the database engine version of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterVersionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterVersionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.describe_type):
             query['DescribeType'] = request.describe_type
         if not UtilClient.is_unset(request.owner_account):
@@ -6064,14 +7231,21 @@
         )
 
     async def describe_dbcluster_version_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterVersionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClusterVersionResponse:
+        """
+        @summary Queries the information about the database engine version of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterVersionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClusterVersionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.describe_type):
             query['DescribeType'] = request.describe_type
         if not UtilClient.is_unset(request.owner_account):
@@ -6101,29 +7275,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbcluster_version(
         self,
         request: polardb_20170801_models.DescribeDBClusterVersionRequest,
     ) -> polardb_20170801_models.DescribeDBClusterVersionResponse:
+        """
+        @summary Queries the information about the database engine version of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterVersionRequest
+        @return: DescribeDBClusterVersionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbcluster_version_with_options(request, runtime)
 
     async def describe_dbcluster_version_async(
         self,
         request: polardb_20170801_models.DescribeDBClusterVersionRequest,
     ) -> polardb_20170801_models.DescribeDBClusterVersionResponse:
+        """
+        @summary Queries the information about the database engine version of a PolarDB for MySQL cluster.
+        
+        @param request: DescribeDBClusterVersionRequest
+        @return: DescribeDBClusterVersionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbcluster_version_with_options_async(request, runtime)
 
     def describe_dbclusters_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClustersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClustersResponse:
+        """
+        @summary Queries PolarDB clusters or the clusters that can be accessed by an authorized RAM user.
+        
+        @param request: DescribeDBClustersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClustersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.connection_string):
             query['ConnectionString'] = request.connection_string
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_ids):
@@ -6184,14 +7377,21 @@
         )
 
     async def describe_dbclusters_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClustersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClustersResponse:
+        """
+        @summary Queries PolarDB clusters or the clusters that can be accessed by an authorized RAM user.
+        
+        @param request: DescribeDBClustersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClustersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.connection_string):
             query['ConnectionString'] = request.connection_string
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_ids):
@@ -6251,29 +7451,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbclusters(
         self,
         request: polardb_20170801_models.DescribeDBClustersRequest,
     ) -> polardb_20170801_models.DescribeDBClustersResponse:
+        """
+        @summary Queries PolarDB clusters or the clusters that can be accessed by an authorized RAM user.
+        
+        @param request: DescribeDBClustersRequest
+        @return: DescribeDBClustersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbclusters_with_options(request, runtime)
 
     async def describe_dbclusters_async(
         self,
         request: polardb_20170801_models.DescribeDBClustersRequest,
     ) -> polardb_20170801_models.DescribeDBClustersResponse:
+        """
+        @summary Queries PolarDB clusters or the clusters that can be accessed by an authorized RAM user.
+        
+        @param request: DescribeDBClustersRequest
+        @return: DescribeDBClustersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbclusters_with_options_async(request, runtime)
 
     def describe_dbclusters_with_backups_with_options(
         self,
         request: polardb_20170801_models.DescribeDBClustersWithBackupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClustersWithBackupsResponse:
+        """
+        @summary Queries the information about PolarDB clusters that contain backup sets in a region.
+        
+        @param request: DescribeDBClustersWithBackupsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClustersWithBackupsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_ids):
             query['DBClusterIds'] = request.dbcluster_ids
         if not UtilClient.is_unset(request.dbtype):
@@ -6318,14 +7537,21 @@
         )
 
     async def describe_dbclusters_with_backups_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBClustersWithBackupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBClustersWithBackupsResponse:
+        """
+        @summary Queries the information about PolarDB clusters that contain backup sets in a region.
+        
+        @param request: DescribeDBClustersWithBackupsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBClustersWithBackupsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_ids):
             query['DBClusterIds'] = request.dbcluster_ids
         if not UtilClient.is_unset(request.dbtype):
@@ -6369,29 +7595,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbclusters_with_backups(
         self,
         request: polardb_20170801_models.DescribeDBClustersWithBackupsRequest,
     ) -> polardb_20170801_models.DescribeDBClustersWithBackupsResponse:
+        """
+        @summary Queries the information about PolarDB clusters that contain backup sets in a region.
+        
+        @param request: DescribeDBClustersWithBackupsRequest
+        @return: DescribeDBClustersWithBackupsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbclusters_with_backups_with_options(request, runtime)
 
     async def describe_dbclusters_with_backups_async(
         self,
         request: polardb_20170801_models.DescribeDBClustersWithBackupsRequest,
     ) -> polardb_20170801_models.DescribeDBClustersWithBackupsResponse:
+        """
+        @summary Queries the information about PolarDB clusters that contain backup sets in a region.
+        
+        @param request: DescribeDBClustersWithBackupsRequest
+        @return: DescribeDBClustersWithBackupsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbclusters_with_backups_with_options_async(request, runtime)
 
     def describe_dbinitialize_variable_with_options(
         self,
         request: polardb_20170801_models.DescribeDBInitializeVariableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBInitializeVariableResponse:
+        """
+        @summary Queries the attributes that are supported by a PolarDB for PostgreSQL (Compatible with Oracle) cluster or a PolarDB for PostgreSQL cluster, such as the character sets and collations.
+        
+        @param request: DescribeDBInitializeVariableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBInitializeVariableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -6420,14 +7665,21 @@
         )
 
     async def describe_dbinitialize_variable_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBInitializeVariableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBInitializeVariableResponse:
+        """
+        @summary Queries the attributes that are supported by a PolarDB for PostgreSQL (Compatible with Oracle) cluster or a PolarDB for PostgreSQL cluster, such as the character sets and collations.
+        
+        @param request: DescribeDBInitializeVariableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBInitializeVariableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -6455,31 +7707,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbinitialize_variable(
         self,
         request: polardb_20170801_models.DescribeDBInitializeVariableRequest,
     ) -> polardb_20170801_models.DescribeDBInitializeVariableResponse:
+        """
+        @summary Queries the attributes that are supported by a PolarDB for PostgreSQL (Compatible with Oracle) cluster or a PolarDB for PostgreSQL cluster, such as the character sets and collations.
+        
+        @param request: DescribeDBInitializeVariableRequest
+        @return: DescribeDBInitializeVariableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbinitialize_variable_with_options(request, runtime)
 
     async def describe_dbinitialize_variable_async(
         self,
         request: polardb_20170801_models.DescribeDBInitializeVariableRequest,
     ) -> polardb_20170801_models.DescribeDBInitializeVariableResponse:
+        """
+        @summary Queries the attributes that are supported by a PolarDB for PostgreSQL (Compatible with Oracle) cluster or a PolarDB for PostgreSQL cluster, such as the character sets and collations.
+        
+        @param request: DescribeDBInitializeVariableRequest
+        @return: DescribeDBInitializeVariableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbinitialize_variable_with_options_async(request, runtime)
 
     def describe_dblinks_with_options(
         self,
         request: polardb_20170801_models.DescribeDBLinksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBLinksResponse:
         """
-        > You can query only the database links that use a PolarDB for Oracle cluster as the source.
+        @summary Queries the database links of a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @description > You can query only the database links that use a PolarDB for Oracle cluster as the source.
         
         @param request: DescribeDBLinksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBLinksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6516,15 +7782,17 @@
 
     async def describe_dblinks_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBLinksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBLinksResponse:
         """
-        > You can query only the database links that use a PolarDB for Oracle cluster as the source.
+        @summary Queries the database links of a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @description > You can query only the database links that use a PolarDB for Oracle cluster as the source.
         
         @param request: DescribeDBLinksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBLinksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6560,53 +7828,59 @@
         )
 
     def describe_dblinks(
         self,
         request: polardb_20170801_models.DescribeDBLinksRequest,
     ) -> polardb_20170801_models.DescribeDBLinksResponse:
         """
-        > You can query only the database links that use a PolarDB for Oracle cluster as the source.
+        @summary Queries the database links of a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @description > You can query only the database links that use a PolarDB for Oracle cluster as the source.
         
         @param request: DescribeDBLinksRequest
         @return: DescribeDBLinksResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dblinks_with_options(request, runtime)
 
     async def describe_dblinks_async(
         self,
         request: polardb_20170801_models.DescribeDBLinksRequest,
     ) -> polardb_20170801_models.DescribeDBLinksResponse:
         """
-        > You can query only the database links that use a PolarDB for Oracle cluster as the source.
+        @summary Queries the database links of a PolarDB for PostgreSQL (Compatible with Oracle) cluster.
+        
+        @description > You can query only the database links that use a PolarDB for Oracle cluster as the source.
         
         @param request: DescribeDBLinksRequest
         @return: DescribeDBLinksResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dblinks_with_options_async(request, runtime)
 
     def describe_dbnode_performance_with_options(
         self,
         request: polardb_20170801_models.DescribeDBNodePerformanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBNodePerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a node in a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBNodePerformanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBNodePerformanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6645,26 +7919,28 @@
 
     async def describe_dbnode_performance_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBNodePerformanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBNodePerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a node in a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBNodePerformanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBNodePerformanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6702,62 +7978,73 @@
         )
 
     def describe_dbnode_performance(
         self,
         request: polardb_20170801_models.DescribeDBNodePerformanceRequest,
     ) -> polardb_20170801_models.DescribeDBNodePerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a node in a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBNodePerformanceRequest
         @return: DescribeDBNodePerformanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbnode_performance_with_options(request, runtime)
 
     async def describe_dbnode_performance_async(
         self,
         request: polardb_20170801_models.DescribeDBNodePerformanceRequest,
     ) -> polardb_20170801_models.DescribeDBNodePerformanceResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](~~159557~~) operation to set the data collection interval to every 5 seconds.
+        @summary Queries the performance data of a node in a PolarDB cluster.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        >  By default, the monitoring data is collected once every 60 seconds. You can call the [ModifyDBClusterMonitor](https://help.aliyun.com/document_detail/159557.html) operation to set the data collection interval to every 5 seconds.
         
         @param request: DescribeDBNodePerformanceRequest
         @return: DescribeDBNodePerformanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbnode_performance_with_options_async(request, runtime)
 
     def describe_dbnodes_parameters_with_options(
         self,
         request: polardb_20170801_models.DescribeDBNodesParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBNodesParametersResponse:
+        """
+        @summary Queries the parameters of a specified node in a cluster.
+        
+        @param request: DescribeDBNodesParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBNodesParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_ids):
             query['DBNodeIds'] = request.dbnode_ids
         if not UtilClient.is_unset(request.owner_account):
@@ -6788,14 +8075,21 @@
         )
 
     async def describe_dbnodes_parameters_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBNodesParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBNodesParametersResponse:
+        """
+        @summary Queries the parameters of a specified node in a cluster.
+        
+        @param request: DescribeDBNodesParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBNodesParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_ids):
             query['DBNodeIds'] = request.dbnode_ids
         if not UtilClient.is_unset(request.owner_account):
@@ -6825,31 +8119,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbnodes_parameters(
         self,
         request: polardb_20170801_models.DescribeDBNodesParametersRequest,
     ) -> polardb_20170801_models.DescribeDBNodesParametersResponse:
+        """
+        @summary Queries the parameters of a specified node in a cluster.
+        
+        @param request: DescribeDBNodesParametersRequest
+        @return: DescribeDBNodesParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbnodes_parameters_with_options(request, runtime)
 
     async def describe_dbnodes_parameters_async(
         self,
         request: polardb_20170801_models.DescribeDBNodesParametersRequest,
     ) -> polardb_20170801_models.DescribeDBNodesParametersResponse:
+        """
+        @summary Queries the parameters of a specified node in a cluster.
+        
+        @param request: DescribeDBNodesParametersRequest
+        @return: DescribeDBNodesParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbnodes_parameters_with_options_async(request, runtime)
 
     def describe_dbproxy_performance_with_options(
         self,
         request: polardb_20170801_models.DescribeDBProxyPerformanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBProxyPerformanceResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the performance data of PolarProxy.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeDBProxyPerformanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBProxyPerformanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6888,15 +8196,17 @@
 
     async def describe_dbproxy_performance_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDBProxyPerformanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDBProxyPerformanceResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the performance data of PolarProxy.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeDBProxyPerformanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDBProxyPerformanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6934,40 +8244,51 @@
         )
 
     def describe_dbproxy_performance(
         self,
         request: polardb_20170801_models.DescribeDBProxyPerformanceRequest,
     ) -> polardb_20170801_models.DescribeDBProxyPerformanceResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the performance data of PolarProxy.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeDBProxyPerformanceRequest
         @return: DescribeDBProxyPerformanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbproxy_performance_with_options(request, runtime)
 
     async def describe_dbproxy_performance_async(
         self,
         request: polardb_20170801_models.DescribeDBProxyPerformanceRequest,
     ) -> polardb_20170801_models.DescribeDBProxyPerformanceResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the performance data of PolarProxy.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeDBProxyPerformanceRequest
         @return: DescribeDBProxyPerformanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbproxy_performance_with_options_async(request, runtime)
 
     def describe_das_config_with_options(
         self,
         request: polardb_20170801_models.DescribeDasConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDasConfigResponse:
+        """
+        @summary 查看实例的 DAS 配置
+        
+        @param request: DescribeDasConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDasConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -6996,14 +8317,21 @@
         )
 
     async def describe_das_config_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDasConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDasConfigResponse:
+        """
+        @summary 查看实例的 DAS 配置
+        
+        @param request: DescribeDasConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDasConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7031,29 +8359,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_das_config(
         self,
         request: polardb_20170801_models.DescribeDasConfigRequest,
     ) -> polardb_20170801_models.DescribeDasConfigResponse:
+        """
+        @summary 查看实例的 DAS 配置
+        
+        @param request: DescribeDasConfigRequest
+        @return: DescribeDasConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_das_config_with_options(request, runtime)
 
     async def describe_das_config_async(
         self,
         request: polardb_20170801_models.DescribeDasConfigRequest,
     ) -> polardb_20170801_models.DescribeDasConfigResponse:
+        """
+        @summary 查看实例的 DAS 配置
+        
+        @param request: DescribeDasConfigRequest
+        @return: DescribeDasConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_das_config_with_options_async(request, runtime)
 
     def describe_databases_with_options(
         self,
         request: polardb_20170801_models.DescribeDatabasesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDatabasesResponse:
+        """
+        @summary Queries the information about databases in a PolarDB cluster.
+        
+        @param request: DescribeDatabasesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDatabasesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbname):
             query['DBName'] = request.dbname
         if not UtilClient.is_unset(request.owner_account):
@@ -7088,14 +8435,21 @@
         )
 
     async def describe_databases_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDatabasesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDatabasesResponse:
+        """
+        @summary Queries the information about databases in a PolarDB cluster.
+        
+        @param request: DescribeDatabasesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDatabasesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbname):
             query['DBName'] = request.dbname
         if not UtilClient.is_unset(request.owner_account):
@@ -7129,32 +8483,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_databases(
         self,
         request: polardb_20170801_models.DescribeDatabasesRequest,
     ) -> polardb_20170801_models.DescribeDatabasesResponse:
+        """
+        @summary Queries the information about databases in a PolarDB cluster.
+        
+        @param request: DescribeDatabasesRequest
+        @return: DescribeDatabasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_databases_with_options(request, runtime)
 
     async def describe_databases_async(
         self,
         request: polardb_20170801_models.DescribeDatabasesRequest,
     ) -> polardb_20170801_models.DescribeDatabasesResponse:
+        """
+        @summary Queries the information about databases in a PolarDB cluster.
+        
+        @param request: DescribeDatabasesRequest
+        @return: DescribeDatabasesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_databases_with_options_async(request, runtime)
 
     def describe_detached_backups_with_options(
         self,
         request: polardb_20170801_models.DescribeDetachedBackupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDetachedBackupsResponse:
         """
-        Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
-        > You can call the [DescribeDBClusterAttribute](~~98181~~) operation to query the cluster status.
+        @summary Queries the information about the backup sets in a released PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
+        > You can call the [DescribeDBClusterAttribute](https://help.aliyun.com/document_detail/98181.html) operation to query the cluster status.
         
         @param request: DescribeDetachedBackupsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDetachedBackupsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7205,16 +8573,18 @@
 
     async def describe_detached_backups_with_options_async(
         self,
         request: polardb_20170801_models.DescribeDetachedBackupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeDetachedBackupsResponse:
         """
-        Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
-        > You can call the [DescribeDBClusterAttribute](~~98181~~) operation to query the cluster status.
+        @summary Queries the information about the backup sets in a released PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
+        > You can call the [DescribeDBClusterAttribute](https://help.aliyun.com/document_detail/98181.html) operation to query the cluster status.
         
         @param request: DescribeDetachedBackupsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDetachedBackupsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7264,42 +8634,53 @@
         )
 
     def describe_detached_backups(
         self,
         request: polardb_20170801_models.DescribeDetachedBackupsRequest,
     ) -> polardb_20170801_models.DescribeDetachedBackupsResponse:
         """
-        Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
-        > You can call the [DescribeDBClusterAttribute](~~98181~~) operation to query the cluster status.
+        @summary Queries the information about the backup sets in a released PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
+        > You can call the [DescribeDBClusterAttribute](https://help.aliyun.com/document_detail/98181.html) operation to query the cluster status.
         
         @param request: DescribeDetachedBackupsRequest
         @return: DescribeDetachedBackupsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_detached_backups_with_options(request, runtime)
 
     async def describe_detached_backups_async(
         self,
         request: polardb_20170801_models.DescribeDetachedBackupsRequest,
     ) -> polardb_20170801_models.DescribeDetachedBackupsResponse:
         """
-        Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
-        > You can call the [DescribeDBClusterAttribute](~~98181~~) operation to query the cluster status.
+        @summary Queries the information about the backup sets in a released PolarDB cluster.
+        
+        @description Before you call this operation, make sure that the PolarDB cluster is in the *Released** state. You must also confirm that the **Retain All Backups Permanently** or **Retain Last Automatic Backup Permanently** backup retention policy takes effect after you release the cluster. If you delete all backup sets after the cluster is released, you cannot use this API operation to query the cluster.
+        > You can call the [DescribeDBClusterAttribute](https://help.aliyun.com/document_detail/98181.html) operation to query the cluster status.
         
         @param request: DescribeDetachedBackupsRequest
         @return: DescribeDetachedBackupsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_detached_backups_with_options_async(request, runtime)
 
     def describe_global_database_network_with_options(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworkResponse:
+        """
+        @summary Queries the information about a Global Database Network (GDN).
+        
+        @param request: DescribeGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gdnid):
             query['GDNId'] = request.gdnid
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7332,14 +8713,21 @@
         )
 
     async def describe_global_database_network_with_options_async(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworkResponse:
+        """
+        @summary Queries the information about a Global Database Network (GDN).
+        
+        @param request: DescribeGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gdnid):
             query['GDNId'] = request.gdnid
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7371,29 +8759,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_global_database_network(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworkResponse:
+        """
+        @summary Queries the information about a Global Database Network (GDN).
+        
+        @param request: DescribeGlobalDatabaseNetworkRequest
+        @return: DescribeGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_global_database_network_with_options(request, runtime)
 
     async def describe_global_database_network_async(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworkResponse:
+        """
+        @summary Queries the information about a Global Database Network (GDN).
+        
+        @param request: DescribeGlobalDatabaseNetworkRequest
+        @return: DescribeGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_global_database_network_with_options_async(request, runtime)
 
     def describe_global_database_networks_with_options(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworksResponse:
+        """
+        @summary Queries the information about all Global Database Networks (GDNs) that belong to an account.
+        
+        @param request: DescribeGlobalDatabaseNetworksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalDatabaseNetworksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.filter_region):
             query['FilterRegion'] = request.filter_region
         if not UtilClient.is_unset(request.gdndescription):
@@ -7436,14 +8843,21 @@
         )
 
     async def describe_global_database_networks_with_options_async(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworksResponse:
+        """
+        @summary Queries the information about all Global Database Networks (GDNs) that belong to an account.
+        
+        @param request: DescribeGlobalDatabaseNetworksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalDatabaseNetworksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.filter_region):
             query['FilterRegion'] = request.filter_region
         if not UtilClient.is_unset(request.gdndescription):
@@ -7485,29 +8899,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_global_database_networks(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworksRequest,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworksResponse:
+        """
+        @summary Queries the information about all Global Database Networks (GDNs) that belong to an account.
+        
+        @param request: DescribeGlobalDatabaseNetworksRequest
+        @return: DescribeGlobalDatabaseNetworksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_global_database_networks_with_options(request, runtime)
 
     async def describe_global_database_networks_async(
         self,
         request: polardb_20170801_models.DescribeGlobalDatabaseNetworksRequest,
     ) -> polardb_20170801_models.DescribeGlobalDatabaseNetworksResponse:
+        """
+        @summary Queries the information about all Global Database Networks (GDNs) that belong to an account.
+        
+        @param request: DescribeGlobalDatabaseNetworksRequest
+        @return: DescribeGlobalDatabaseNetworksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_global_database_networks_with_options_async(request, runtime)
 
     def describe_global_security_ipgroup_with_options(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupResponse:
+        """
+        @summary Queries global IP whitelist templates.
+        
+        @param request: DescribeGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7542,14 +8975,21 @@
         )
 
     async def describe_global_security_ipgroup_with_options_async(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupResponse:
+        """
+        @summary Queries global IP whitelist templates.
+        
+        @param request: DescribeGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7583,29 +9023,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_global_security_ipgroup(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupResponse:
+        """
+        @summary Queries global IP whitelist templates.
+        
+        @param request: DescribeGlobalSecurityIPGroupRequest
+        @return: DescribeGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_global_security_ipgroup_with_options(request, runtime)
 
     async def describe_global_security_ipgroup_async(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupResponse:
+        """
+        @summary Queries global IP whitelist templates.
+        
+        @param request: DescribeGlobalSecurityIPGroupRequest
+        @return: DescribeGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_global_security_ipgroup_with_options_async(request, runtime)
 
     def describe_global_security_ipgroup_relation_with_options(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Queries the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: DescribeGlobalSecurityIPGroupRelationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalSecurityIPGroupRelationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7640,14 +9099,21 @@
         )
 
     async def describe_global_security_ipgroup_relation_with_options_async(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Queries the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: DescribeGlobalSecurityIPGroupRelationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeGlobalSecurityIPGroupRelationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7681,29 +9147,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_global_security_ipgroup_relation(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationRequest,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Queries the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: DescribeGlobalSecurityIPGroupRelationRequest
+        @return: DescribeGlobalSecurityIPGroupRelationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_global_security_ipgroup_relation_with_options(request, runtime)
 
     async def describe_global_security_ipgroup_relation_async(
         self,
         request: polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationRequest,
     ) -> polardb_20170801_models.DescribeGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Queries the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: DescribeGlobalSecurityIPGroupRelationRequest
+        @return: DescribeGlobalSecurityIPGroupRelationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_global_security_ipgroup_relation_with_options_async(request, runtime)
 
     def describe_log_backup_policy_with_options(
         self,
         request: polardb_20170801_models.DescribeLogBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeLogBackupPolicyResponse:
+        """
+        @summary Queries the retention policy of log backups in a PolarDB cluster.
+        
+        @param request: DescribeLogBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeLogBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7732,14 +9217,21 @@
         )
 
     async def describe_log_backup_policy_with_options_async(
         self,
         request: polardb_20170801_models.DescribeLogBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeLogBackupPolicyResponse:
+        """
+        @summary Queries the retention policy of log backups in a PolarDB cluster.
+        
+        @param request: DescribeLogBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeLogBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -7767,29 +9259,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_log_backup_policy(
         self,
         request: polardb_20170801_models.DescribeLogBackupPolicyRequest,
     ) -> polardb_20170801_models.DescribeLogBackupPolicyResponse:
+        """
+        @summary Queries the retention policy of log backups in a PolarDB cluster.
+        
+        @param request: DescribeLogBackupPolicyRequest
+        @return: DescribeLogBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_log_backup_policy_with_options(request, runtime)
 
     async def describe_log_backup_policy_async(
         self,
         request: polardb_20170801_models.DescribeLogBackupPolicyRequest,
     ) -> polardb_20170801_models.DescribeLogBackupPolicyResponse:
+        """
+        @summary Queries the retention policy of log backups in a PolarDB cluster.
+        
+        @param request: DescribeLogBackupPolicyRequest
+        @return: DescribeLogBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_log_backup_policy_with_options_async(request, runtime)
 
     def describe_masking_rules_with_options(
         self,
         request: polardb_20170801_models.DescribeMaskingRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeMaskingRulesResponse:
+        """
+        @summary Queries the data masking rules of a PolarDB cluster or the information about a specified masking rule.
+        
+        @param request: DescribeMaskingRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMaskingRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.rule_name_list):
             query['RuleNameList'] = request.rule_name_list
         req = open_api_models.OpenApiRequest(
@@ -7812,14 +9323,21 @@
         )
 
     async def describe_masking_rules_with_options_async(
         self,
         request: polardb_20170801_models.DescribeMaskingRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeMaskingRulesResponse:
+        """
+        @summary Queries the data masking rules of a PolarDB cluster or the information about a specified masking rule.
+        
+        @param request: DescribeMaskingRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMaskingRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.rule_name_list):
             query['RuleNameList'] = request.rule_name_list
         req = open_api_models.OpenApiRequest(
@@ -7841,29 +9359,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_masking_rules(
         self,
         request: polardb_20170801_models.DescribeMaskingRulesRequest,
     ) -> polardb_20170801_models.DescribeMaskingRulesResponse:
+        """
+        @summary Queries the data masking rules of a PolarDB cluster or the information about a specified masking rule.
+        
+        @param request: DescribeMaskingRulesRequest
+        @return: DescribeMaskingRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_masking_rules_with_options(request, runtime)
 
     async def describe_masking_rules_async(
         self,
         request: polardb_20170801_models.DescribeMaskingRulesRequest,
     ) -> polardb_20170801_models.DescribeMaskingRulesResponse:
+        """
+        @summary Queries the data masking rules of a PolarDB cluster or the information about a specified masking rule.
+        
+        @param request: DescribeMaskingRulesRequest
+        @return: DescribeMaskingRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_masking_rules_with_options_async(request, runtime)
 
     def describe_meta_list_with_options(
         self,
         request: polardb_20170801_models.DescribeMetaListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeMetaListResponse:
+        """
+        @summary Queries the details of the databases or tables that can be restored.
+        
+        @param request: DescribeMetaListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMetaListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.get_db_name):
@@ -7906,14 +9443,21 @@
         )
 
     async def describe_meta_list_with_options_async(
         self,
         request: polardb_20170801_models.DescribeMetaListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeMetaListResponse:
+        """
+        @summary Queries the details of the databases or tables that can be restored.
+        
+        @param request: DescribeMetaListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMetaListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.get_db_name):
@@ -7955,31 +9499,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_meta_list(
         self,
         request: polardb_20170801_models.DescribeMetaListRequest,
     ) -> polardb_20170801_models.DescribeMetaListResponse:
+        """
+        @summary Queries the details of the databases or tables that can be restored.
+        
+        @param request: DescribeMetaListRequest
+        @return: DescribeMetaListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_meta_list_with_options(request, runtime)
 
     async def describe_meta_list_async(
         self,
         request: polardb_20170801_models.DescribeMetaListRequest,
     ) -> polardb_20170801_models.DescribeMetaListResponse:
+        """
+        @summary Queries the details of the databases or tables that can be restored.
+        
+        @param request: DescribeMetaListRequest
+        @return: DescribeMetaListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_meta_list_with_options_async(request, runtime)
 
     def describe_parameter_group_with_options(
         self,
         request: polardb_20170801_models.DescribeParameterGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries the information about a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This parameter is valid only for a PolarDB for MySQL cluster.
         
         @param request: DescribeParameterGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeParameterGroupResponse
         """
         UtilClient.validate_model(request)
@@ -8019,15 +9577,17 @@
 
     async def describe_parameter_group_with_options_async(
         self,
         request: polardb_20170801_models.DescribeParameterGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries the information about a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This parameter is valid only for a PolarDB for MySQL cluster.
         
         @param request: DescribeParameterGroupRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeParameterGroupResponse
         """
         UtilClient.validate_model(request)
@@ -8066,44 +9626,50 @@
         )
 
     def describe_parameter_group(
         self,
         request: polardb_20170801_models.DescribeParameterGroupRequest,
     ) -> polardb_20170801_models.DescribeParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries the information about a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This parameter is valid only for a PolarDB for MySQL cluster.
         
         @param request: DescribeParameterGroupRequest
         @return: DescribeParameterGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_parameter_group_with_options(request, runtime)
 
     async def describe_parameter_group_async(
         self,
         request: polardb_20170801_models.DescribeParameterGroupRequest,
     ) -> polardb_20170801_models.DescribeParameterGroupResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries the information about a parameter template.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This parameter is valid only for a PolarDB for MySQL cluster.
         
         @param request: DescribeParameterGroupRequest
         @return: DescribeParameterGroupResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_parameter_group_with_options_async(request, runtime)
 
     def describe_parameter_groups_with_options(
         self,
         request: polardb_20170801_models.DescribeParameterGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeParameterGroupsResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries parameter templates that are available in a specified region.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeParameterGroupsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeParameterGroupsResponse
         """
         UtilClient.validate_model(request)
@@ -8145,15 +9711,17 @@
 
     async def describe_parameter_groups_with_options_async(
         self,
         request: polardb_20170801_models.DescribeParameterGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeParameterGroupsResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries parameter templates that are available in a specified region.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeParameterGroupsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeParameterGroupsResponse
         """
         UtilClient.validate_model(request)
@@ -8194,42 +9762,53 @@
         )
 
     def describe_parameter_groups(
         self,
         request: polardb_20170801_models.DescribeParameterGroupsRequest,
     ) -> polardb_20170801_models.DescribeParameterGroupsResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries parameter templates that are available in a specified region.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeParameterGroupsRequest
         @return: DescribeParameterGroupsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_parameter_groups_with_options(request, runtime)
 
     async def describe_parameter_groups_async(
         self,
         request: polardb_20170801_models.DescribeParameterGroupsRequest,
     ) -> polardb_20170801_models.DescribeParameterGroupsResponse:
         """
-        You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
+        @summary Queries parameter templates that are available in a specified region.
+        
+        @description You can use parameter templates to manage multiple parameters at a time and apply existing parameters to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
         > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeParameterGroupsRequest
         @return: DescribeParameterGroupsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_parameter_groups_with_options_async(request, runtime)
 
     def describe_parameter_templates_with_options(
         self,
         request: polardb_20170801_models.DescribeParameterTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeParameterTemplatesResponse:
+        """
+        @summary Queries the default parameters in a cluster.
+        
+        @param request: DescribeParameterTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeParameterTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbtype):
             query['DBType'] = request.dbtype
         if not UtilClient.is_unset(request.dbversion):
             query['DBVersion'] = request.dbversion
         if not UtilClient.is_unset(request.owner_account):
@@ -8264,14 +9843,21 @@
         )
 
     async def describe_parameter_templates_with_options_async(
         self,
         request: polardb_20170801_models.DescribeParameterTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeParameterTemplatesResponse:
+        """
+        @summary Queries the default parameters in a cluster.
+        
+        @param request: DescribeParameterTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeParameterTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbtype):
             query['DBType'] = request.dbtype
         if not UtilClient.is_unset(request.dbversion):
             query['DBVersion'] = request.dbversion
         if not UtilClient.is_unset(request.owner_account):
@@ -8305,29 +9891,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_parameter_templates(
         self,
         request: polardb_20170801_models.DescribeParameterTemplatesRequest,
     ) -> polardb_20170801_models.DescribeParameterTemplatesResponse:
+        """
+        @summary Queries the default parameters in a cluster.
+        
+        @param request: DescribeParameterTemplatesRequest
+        @return: DescribeParameterTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_parameter_templates_with_options(request, runtime)
 
     async def describe_parameter_templates_async(
         self,
         request: polardb_20170801_models.DescribeParameterTemplatesRequest,
     ) -> polardb_20170801_models.DescribeParameterTemplatesResponse:
+        """
+        @summary Queries the default parameters in a cluster.
+        
+        @param request: DescribeParameterTemplatesRequest
+        @return: DescribeParameterTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_parameter_templates_with_options_async(request, runtime)
 
     def describe_pending_maintenance_action_with_options(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionResponse:
+        """
+        @summary Queries the information about a pending event.
+        
+        @param request: DescribePendingMaintenanceActionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePendingMaintenanceActionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.is_history):
             query['IsHistory'] = request.is_history
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8368,14 +9973,21 @@
         )
 
     async def describe_pending_maintenance_action_with_options_async(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionResponse:
+        """
+        @summary Queries the information about a pending event.
+        
+        @param request: DescribePendingMaintenanceActionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePendingMaintenanceActionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.is_history):
             query['IsHistory'] = request.is_history
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8415,29 +10027,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_pending_maintenance_action(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionRequest,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionResponse:
+        """
+        @summary Queries the information about a pending event.
+        
+        @param request: DescribePendingMaintenanceActionRequest
+        @return: DescribePendingMaintenanceActionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_pending_maintenance_action_with_options(request, runtime)
 
     async def describe_pending_maintenance_action_async(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionRequest,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionResponse:
+        """
+        @summary Queries the information about a pending event.
+        
+        @param request: DescribePendingMaintenanceActionRequest
+        @return: DescribePendingMaintenanceActionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_pending_maintenance_action_with_options_async(request, runtime)
 
     def describe_pending_maintenance_actions_with_options(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionsResponse:
+        """
+        @summary Queries the numbers of pending events of different task types.
+        
+        @param request: DescribePendingMaintenanceActionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePendingMaintenanceActionsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.is_history):
             query['IsHistory'] = request.is_history
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8472,14 +10103,21 @@
         )
 
     async def describe_pending_maintenance_actions_with_options_async(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionsResponse:
+        """
+        @summary Queries the numbers of pending events of different task types.
+        
+        @param request: DescribePendingMaintenanceActionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePendingMaintenanceActionsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.is_history):
             query['IsHistory'] = request.is_history
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -8513,29 +10151,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_pending_maintenance_actions(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionsRequest,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionsResponse:
+        """
+        @summary Queries the numbers of pending events of different task types.
+        
+        @param request: DescribePendingMaintenanceActionsRequest
+        @return: DescribePendingMaintenanceActionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_pending_maintenance_actions_with_options(request, runtime)
 
     async def describe_pending_maintenance_actions_async(
         self,
         request: polardb_20170801_models.DescribePendingMaintenanceActionsRequest,
     ) -> polardb_20170801_models.DescribePendingMaintenanceActionsResponse:
+        """
+        @summary Queries the numbers of pending events of different task types.
+        
+        @param request: DescribePendingMaintenanceActionsRequest
+        @return: DescribePendingMaintenanceActionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_pending_maintenance_actions_with_options_async(request, runtime)
 
     def describe_polar_sqlcollector_policy_with_options(
         self,
         request: polardb_20170801_models.DescribePolarSQLCollectorPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribePolarSQLCollectorPolicyResponse:
+        """
+        @summary Queries whether the SQL Explorer feature is enabled for the cluster.
+        
+        @param request: DescribePolarSQLCollectorPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePolarSQLCollectorPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePolarSQLCollectorPolicy',
@@ -8554,14 +10211,21 @@
         )
 
     async def describe_polar_sqlcollector_policy_with_options_async(
         self,
         request: polardb_20170801_models.DescribePolarSQLCollectorPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribePolarSQLCollectorPolicyResponse:
+        """
+        @summary Queries whether the SQL Explorer feature is enabled for the cluster.
+        
+        @param request: DescribePolarSQLCollectorPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePolarSQLCollectorPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePolarSQLCollectorPolicy',
@@ -8579,29 +10243,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_polar_sqlcollector_policy(
         self,
         request: polardb_20170801_models.DescribePolarSQLCollectorPolicyRequest,
     ) -> polardb_20170801_models.DescribePolarSQLCollectorPolicyResponse:
+        """
+        @summary Queries whether the SQL Explorer feature is enabled for the cluster.
+        
+        @param request: DescribePolarSQLCollectorPolicyRequest
+        @return: DescribePolarSQLCollectorPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_polar_sqlcollector_policy_with_options(request, runtime)
 
     async def describe_polar_sqlcollector_policy_async(
         self,
         request: polardb_20170801_models.DescribePolarSQLCollectorPolicyRequest,
     ) -> polardb_20170801_models.DescribePolarSQLCollectorPolicyResponse:
+        """
+        @summary Queries whether the SQL Explorer feature is enabled for the cluster.
+        
+        @param request: DescribePolarSQLCollectorPolicyRequest
+        @return: DescribePolarSQLCollectorPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_polar_sqlcollector_policy_with_options_async(request, runtime)
 
     def describe_regions_with_options(
         self,
         request: polardb_20170801_models.DescribeRegionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeRegionsResponse:
+        """
+        @summary Queries the regions and zones available for PolarDB.
+        
+        @param request: DescribeRegionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRegionsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -8628,14 +10311,21 @@
         )
 
     async def describe_regions_with_options_async(
         self,
         request: polardb_20170801_models.DescribeRegionsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeRegionsResponse:
+        """
+        @summary Queries the regions and zones available for PolarDB.
+        
+        @param request: DescribeRegionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRegionsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -8661,29 +10351,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_regions(
         self,
         request: polardb_20170801_models.DescribeRegionsRequest,
     ) -> polardb_20170801_models.DescribeRegionsResponse:
+        """
+        @summary Queries the regions and zones available for PolarDB.
+        
+        @param request: DescribeRegionsRequest
+        @return: DescribeRegionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_regions_with_options(request, runtime)
 
     async def describe_regions_async(
         self,
         request: polardb_20170801_models.DescribeRegionsRequest,
     ) -> polardb_20170801_models.DescribeRegionsResponse:
+        """
+        @summary Queries the regions and zones available for PolarDB.
+        
+        @param request: DescribeRegionsRequest
+        @return: DescribeRegionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_regions_with_options_async(request, runtime)
 
     def describe_schedule_tasks_with_options(
         self,
         request: polardb_20170801_models.DescribeScheduleTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeScheduleTasksResponse:
+        """
+        @summary Queries the details of all scheduled tasks.
+        
+        @param request: DescribeScheduleTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeScheduleTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.order_id):
@@ -8732,14 +10441,21 @@
         )
 
     async def describe_schedule_tasks_with_options_async(
         self,
         request: polardb_20170801_models.DescribeScheduleTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeScheduleTasksResponse:
+        """
+        @summary Queries the details of all scheduled tasks.
+        
+        @param request: DescribeScheduleTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeScheduleTasksResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.order_id):
@@ -8787,31 +10503,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_schedule_tasks(
         self,
         request: polardb_20170801_models.DescribeScheduleTasksRequest,
     ) -> polardb_20170801_models.DescribeScheduleTasksResponse:
+        """
+        @summary Queries the details of all scheduled tasks.
+        
+        @param request: DescribeScheduleTasksRequest
+        @return: DescribeScheduleTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_schedule_tasks_with_options(request, runtime)
 
     async def describe_schedule_tasks_async(
         self,
         request: polardb_20170801_models.DescribeScheduleTasksRequest,
     ) -> polardb_20170801_models.DescribeScheduleTasksResponse:
+        """
+        @summary Queries the details of all scheduled tasks.
+        
+        @param request: DescribeScheduleTasksRequest
+        @return: DescribeScheduleTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_schedule_tasks_with_options_async(request, runtime)
 
     def describe_slow_log_records_with_options(
         self,
         request: polardb_20170801_models.DescribeSlowLogRecordsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeSlowLogRecordsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the details of the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogRecordsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSlowLogRecordsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8860,15 +10590,17 @@
 
     async def describe_slow_log_records_with_options_async(
         self,
         request: polardb_20170801_models.DescribeSlowLogRecordsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeSlowLogRecordsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the details of the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogRecordsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSlowLogRecordsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8916,42 +10648,48 @@
         )
 
     def describe_slow_log_records(
         self,
         request: polardb_20170801_models.DescribeSlowLogRecordsRequest,
     ) -> polardb_20170801_models.DescribeSlowLogRecordsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the details of the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogRecordsRequest
         @return: DescribeSlowLogRecordsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_slow_log_records_with_options(request, runtime)
 
     async def describe_slow_log_records_async(
         self,
         request: polardb_20170801_models.DescribeSlowLogRecordsRequest,
     ) -> polardb_20170801_models.DescribeSlowLogRecordsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the details of the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogRecordsRequest
         @return: DescribeSlowLogRecordsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_slow_log_records_with_options_async(request, runtime)
 
     def describe_slow_logs_with_options(
         self,
         request: polardb_20170801_models.DescribeSlowLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeSlowLogsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the statistics about the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSlowLogsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8998,15 +10736,17 @@
 
     async def describe_slow_logs_with_options_async(
         self,
         request: polardb_20170801_models.DescribeSlowLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeSlowLogsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the statistics about the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSlowLogsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9052,43 +10792,49 @@
         )
 
     def describe_slow_logs(
         self,
         request: polardb_20170801_models.DescribeSlowLogsRequest,
     ) -> polardb_20170801_models.DescribeSlowLogsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the statistics about the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogsRequest
         @return: DescribeSlowLogsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_slow_logs_with_options(request, runtime)
 
     async def describe_slow_logs_async(
         self,
         request: polardb_20170801_models.DescribeSlowLogsRequest,
     ) -> polardb_20170801_models.DescribeSlowLogsResponse:
         """
-        > This operation is applicable only to PolarDB for MySQL clusters.
+        @summary Queries the statistics about the slow query logs of a PolarDB cluster.
+        
+        @description > This operation is applicable only to PolarDB for MySQL clusters.
         
         @param request: DescribeSlowLogsRequest
         @return: DescribeSlowLogsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_slow_logs_with_options_async(request, runtime)
 
     def describe_tasks_with_options(
         self,
         request: polardb_20170801_models.DescribeTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeTasksResponse:
         """
-        You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](~~98169~~) operation or [create a cluster](~~58769~~) in the console.
-        *   You can view the details of tasks that are generated only when you call the [CreateDBCluster](~~98169~~) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
+        @summary Queries the details of the tasks that are generated by calling API operations. For example, you can call this operation to view the details of the task when you create a cluster.
+        
+        @description    You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation or [create a cluster](https://help.aliyun.com/document_detail/58769.html) in the console.
+        You can view the details of tasks that are generated only when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
         
         @param request: DescribeTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9135,16 +10881,18 @@
 
     async def describe_tasks_with_options_async(
         self,
         request: polardb_20170801_models.DescribeTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeTasksResponse:
         """
-        You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](~~98169~~) operation or [create a cluster](~~58769~~) in the console.
-        *   You can view the details of tasks that are generated only when you call the [CreateDBCluster](~~98169~~) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
+        @summary Queries the details of the tasks that are generated by calling API operations. For example, you can call this operation to view the details of the task when you create a cluster.
+        
+        @description    You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation or [create a cluster](https://help.aliyun.com/document_detail/58769.html) in the console.
+        You can view the details of tasks that are generated only when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
         
         @param request: DescribeTasksRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeTasksResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9190,42 +10938,53 @@
         )
 
     def describe_tasks(
         self,
         request: polardb_20170801_models.DescribeTasksRequest,
     ) -> polardb_20170801_models.DescribeTasksResponse:
         """
-        You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](~~98169~~) operation or [create a cluster](~~58769~~) in the console.
-        *   You can view the details of tasks that are generated only when you call the [CreateDBCluster](~~98169~~) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
+        @summary Queries the details of the tasks that are generated by calling API operations. For example, you can call this operation to view the details of the task when you create a cluster.
+        
+        @description    You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation or [create a cluster](https://help.aliyun.com/document_detail/58769.html) in the console.
+        You can view the details of tasks that are generated only when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
         
         @param request: DescribeTasksRequest
         @return: DescribeTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_tasks_with_options(request, runtime)
 
     async def describe_tasks_async(
         self,
         request: polardb_20170801_models.DescribeTasksRequest,
     ) -> polardb_20170801_models.DescribeTasksResponse:
         """
-        You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](~~98169~~) operation or [create a cluster](~~58769~~) in the console.
-        *   You can view the details of tasks that are generated only when you call the [CreateDBCluster](~~98169~~) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
+        @summary Queries the details of the tasks that are generated by calling API operations. For example, you can call this operation to view the details of the task when you create a cluster.
+        
+        @description    You can call this operation to view the details of a task that is generated by a specific API operation or in the console. The system calls the specific API operation when you perform an operation in the console. For example, you can view the details of the task when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation or [create a cluster](https://help.aliyun.com/document_detail/58769.html) in the console.
+        You can view the details of tasks that are generated only when you call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create a cluster and `CreationOption` is not set to `CreateGdnStandby`.
         
         @param request: DescribeTasksRequest
         @return: DescribeTasksResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_tasks_with_options_async(request, runtime)
 
     def describe_user_encryption_key_list_with_options(
         self,
         request: polardb_20170801_models.DescribeUserEncryptionKeyListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeUserEncryptionKeyListResponse:
+        """
+        @summary Queries the Key Management Service (KMS)-managed customer master keys (CMKs) that are used to encrypt data in a PolarDB cluster.
+        
+        @param request: DescribeUserEncryptionKeyListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUserEncryptionKeyListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9258,14 +11017,21 @@
         )
 
     async def describe_user_encryption_key_list_with_options_async(
         self,
         request: polardb_20170801_models.DescribeUserEncryptionKeyListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeUserEncryptionKeyListResponse:
+        """
+        @summary Queries the Key Management Service (KMS)-managed customer master keys (CMKs) that are used to encrypt data in a PolarDB cluster.
+        
+        @param request: DescribeUserEncryptionKeyListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUserEncryptionKeyListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9297,29 +11063,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_user_encryption_key_list(
         self,
         request: polardb_20170801_models.DescribeUserEncryptionKeyListRequest,
     ) -> polardb_20170801_models.DescribeUserEncryptionKeyListResponse:
+        """
+        @summary Queries the Key Management Service (KMS)-managed customer master keys (CMKs) that are used to encrypt data in a PolarDB cluster.
+        
+        @param request: DescribeUserEncryptionKeyListRequest
+        @return: DescribeUserEncryptionKeyListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_encryption_key_list_with_options(request, runtime)
 
     async def describe_user_encryption_key_list_async(
         self,
         request: polardb_20170801_models.DescribeUserEncryptionKeyListRequest,
     ) -> polardb_20170801_models.DescribeUserEncryptionKeyListResponse:
+        """
+        @summary Queries the Key Management Service (KMS)-managed customer master keys (CMKs) that are used to encrypt data in a PolarDB cluster.
+        
+        @param request: DescribeUserEncryptionKeyListRequest
+        @return: DescribeUserEncryptionKeyListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_encryption_key_list_with_options_async(request, runtime)
 
     def describe_vswitches_with_options(
         self,
         request: polardb_20170801_models.DescribeVSwitchesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeVSwitchesResponse:
+        """
+        @summary Queries a vSwitch.
+        
+        @param request: DescribeVSwitchesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVSwitchesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_host_group_id):
             query['DedicatedHostGroupId'] = request.dedicated_host_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9362,14 +11147,21 @@
         )
 
     async def describe_vswitches_with_options_async(
         self,
         request: polardb_20170801_models.DescribeVSwitchesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DescribeVSwitchesResponse:
+        """
+        @summary Queries a vSwitch.
+        
+        @param request: DescribeVSwitchesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeVSwitchesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_host_group_id):
             query['DedicatedHostGroupId'] = request.dedicated_host_group_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9411,29 +11203,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_vswitches(
         self,
         request: polardb_20170801_models.DescribeVSwitchesRequest,
     ) -> polardb_20170801_models.DescribeVSwitchesResponse:
+        """
+        @summary Queries a vSwitch.
+        
+        @param request: DescribeVSwitchesRequest
+        @return: DescribeVSwitchesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_vswitches_with_options(request, runtime)
 
     async def describe_vswitches_async(
         self,
         request: polardb_20170801_models.DescribeVSwitchesRequest,
     ) -> polardb_20170801_models.DescribeVSwitchesResponse:
+        """
+        @summary Queries a vSwitch.
+        
+        @param request: DescribeVSwitchesRequest
+        @return: DescribeVSwitchesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_vswitches_with_options_async(request, runtime)
 
     def disable_dbcluster_serverless_with_options(
         self,
         request: polardb_20170801_models.DisableDBClusterServerlessRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DisableDBClusterServerlessResponse:
+        """
+        @summary Disables a stable serverless cluster.
+        
+        @param request: DisableDBClusterServerlessRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableDBClusterServerlessResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9462,14 +11273,21 @@
         )
 
     async def disable_dbcluster_serverless_with_options_async(
         self,
         request: polardb_20170801_models.DisableDBClusterServerlessRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.DisableDBClusterServerlessResponse:
+        """
+        @summary Disables a stable serverless cluster.
+        
+        @param request: DisableDBClusterServerlessRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableDBClusterServerlessResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9497,29 +11315,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def disable_dbcluster_serverless(
         self,
         request: polardb_20170801_models.DisableDBClusterServerlessRequest,
     ) -> polardb_20170801_models.DisableDBClusterServerlessResponse:
+        """
+        @summary Disables a stable serverless cluster.
+        
+        @param request: DisableDBClusterServerlessRequest
+        @return: DisableDBClusterServerlessResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.disable_dbcluster_serverless_with_options(request, runtime)
 
     async def disable_dbcluster_serverless_async(
         self,
         request: polardb_20170801_models.DisableDBClusterServerlessRequest,
     ) -> polardb_20170801_models.DisableDBClusterServerlessResponse:
+        """
+        @summary Disables a stable serverless cluster.
+        
+        @param request: DisableDBClusterServerlessRequest
+        @return: DisableDBClusterServerlessResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.disable_dbcluster_serverless_with_options_async(request, runtime)
 
     def enable_dbcluster_serverless_with_options(
         self,
         request: polardb_20170801_models.EnableDBClusterServerlessRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.EnableDBClusterServerlessResponse:
+        """
+        @summary Enables a stable serverless cluster.
+        
+        @param request: EnableDBClusterServerlessRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableDBClusterServerlessResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9560,14 +11397,21 @@
         )
 
     async def enable_dbcluster_serverless_with_options_async(
         self,
         request: polardb_20170801_models.EnableDBClusterServerlessRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.EnableDBClusterServerlessResponse:
+        """
+        @summary Enables a stable serverless cluster.
+        
+        @param request: EnableDBClusterServerlessRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableDBClusterServerlessResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -9607,29 +11451,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_dbcluster_serverless(
         self,
         request: polardb_20170801_models.EnableDBClusterServerlessRequest,
     ) -> polardb_20170801_models.EnableDBClusterServerlessResponse:
+        """
+        @summary Enables a stable serverless cluster.
+        
+        @param request: EnableDBClusterServerlessRequest
+        @return: EnableDBClusterServerlessResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_dbcluster_serverless_with_options(request, runtime)
 
     async def enable_dbcluster_serverless_async(
         self,
         request: polardb_20170801_models.EnableDBClusterServerlessRequest,
     ) -> polardb_20170801_models.EnableDBClusterServerlessResponse:
+        """
+        @summary Enables a stable serverless cluster.
+        
+        @param request: EnableDBClusterServerlessRequest
+        @return: EnableDBClusterServerlessResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.enable_dbcluster_serverless_with_options_async(request, runtime)
 
     def enable_firewall_rules_with_options(
         self,
         request: polardb_20170801_models.EnableFirewallRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.EnableFirewallRulesResponse:
+        """
+        @summary 修改sql防火墙状态
+        
+        @param request: EnableFirewallRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableFirewallRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.owner_account):
@@ -9662,14 +11525,21 @@
         )
 
     async def enable_firewall_rules_with_options_async(
         self,
         request: polardb_20170801_models.EnableFirewallRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.EnableFirewallRulesResponse:
+        """
+        @summary 修改sql防火墙状态
+        
+        @param request: EnableFirewallRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableFirewallRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.owner_account):
@@ -9701,29 +11571,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_firewall_rules(
         self,
         request: polardb_20170801_models.EnableFirewallRulesRequest,
     ) -> polardb_20170801_models.EnableFirewallRulesResponse:
+        """
+        @summary 修改sql防火墙状态
+        
+        @param request: EnableFirewallRulesRequest
+        @return: EnableFirewallRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_firewall_rules_with_options(request, runtime)
 
     async def enable_firewall_rules_async(
         self,
         request: polardb_20170801_models.EnableFirewallRulesRequest,
     ) -> polardb_20170801_models.EnableFirewallRulesResponse:
+        """
+        @summary 修改sql防火墙状态
+        
+        @param request: EnableFirewallRulesRequest
+        @return: EnableFirewallRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.enable_firewall_rules_with_options_async(request, runtime)
 
     def evaluate_region_resource_with_options(
         self,
         request: polardb_20170801_models.EvaluateRegionResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.EvaluateRegionResourceResponse:
+        """
+        @summary Evaluates available resources.
+        
+        @param request: EvaluateRegionResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EvaluateRegionResourceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbinstance_conn_type):
             query['DBInstanceConnType'] = request.dbinstance_conn_type
         if not UtilClient.is_unset(request.dbnode_class):
             query['DBNodeClass'] = request.dbnode_class
         if not UtilClient.is_unset(request.dbtype):
@@ -9770,14 +11659,21 @@
         )
 
     async def evaluate_region_resource_with_options_async(
         self,
         request: polardb_20170801_models.EvaluateRegionResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.EvaluateRegionResourceResponse:
+        """
+        @summary Evaluates available resources.
+        
+        @param request: EvaluateRegionResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EvaluateRegionResourceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbinstance_conn_type):
             query['DBInstanceConnType'] = request.dbinstance_conn_type
         if not UtilClient.is_unset(request.dbnode_class):
             query['DBNodeClass'] = request.dbnode_class
         if not UtilClient.is_unset(request.dbtype):
@@ -9823,29 +11719,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def evaluate_region_resource(
         self,
         request: polardb_20170801_models.EvaluateRegionResourceRequest,
     ) -> polardb_20170801_models.EvaluateRegionResourceResponse:
+        """
+        @summary Evaluates available resources.
+        
+        @param request: EvaluateRegionResourceRequest
+        @return: EvaluateRegionResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.evaluate_region_resource_with_options(request, runtime)
 
     async def evaluate_region_resource_async(
         self,
         request: polardb_20170801_models.EvaluateRegionResourceRequest,
     ) -> polardb_20170801_models.EvaluateRegionResourceResponse:
+        """
+        @summary Evaluates available resources.
+        
+        @param request: EvaluateRegionResourceRequest
+        @return: EvaluateRegionResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.evaluate_region_resource_with_options_async(request, runtime)
 
     def failover_dbcluster_with_options(
         self,
         request: polardb_20170801_models.FailoverDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.FailoverDBClusterResponse:
+        """
+        @summary Performs a manual failover to promote a read-only node to the primary node in a PolarDB cluster.
+        
+        @param request: FailoverDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: FailoverDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -9880,14 +11795,21 @@
         )
 
     async def failover_dbcluster_with_options_async(
         self,
         request: polardb_20170801_models.FailoverDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.FailoverDBClusterResponse:
+        """
+        @summary Performs a manual failover to promote a read-only node to the primary node in a PolarDB cluster.
+        
+        @param request: FailoverDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: FailoverDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -9921,35 +11843,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def failover_dbcluster(
         self,
         request: polardb_20170801_models.FailoverDBClusterRequest,
     ) -> polardb_20170801_models.FailoverDBClusterResponse:
+        """
+        @summary Performs a manual failover to promote a read-only node to the primary node in a PolarDB cluster.
+        
+        @param request: FailoverDBClusterRequest
+        @return: FailoverDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.failover_dbcluster_with_options(request, runtime)
 
     async def failover_dbcluster_async(
         self,
         request: polardb_20170801_models.FailoverDBClusterRequest,
     ) -> polardb_20170801_models.FailoverDBClusterResponse:
+        """
+        @summary Performs a manual failover to promote a read-only node to the primary node in a PolarDB cluster.
+        
+        @param request: FailoverDBClusterRequest
+        @return: FailoverDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.failover_dbcluster_with_options_async(request, runtime)
 
     def grant_account_privilege_with_options(
         self,
         request: polardb_20170801_models.GrantAccountPrivilegeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.GrantAccountPrivilegeResponse:
         """
-        >    An account can be authorized to access one or more databases.
-        > *   If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
-        > *   Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
-        > *   You can call this operation only on a PolarDB for MySQL cluster.
-        > *   By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
+        @summary Grants a standard account the permissions to access one or more databases in a specified PolarDB cluster.
+        
+        @description >    An account can be authorized to access one or more databases.
+        >    If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
+        >    Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        >    You can call this operation only on a PolarDB for MySQL cluster.
+        >    By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
         
         @param request: GrantAccountPrivilegeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GrantAccountPrivilegeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9990,19 +11926,21 @@
 
     async def grant_account_privilege_with_options_async(
         self,
         request: polardb_20170801_models.GrantAccountPrivilegeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.GrantAccountPrivilegeResponse:
         """
-        >    An account can be authorized to access one or more databases.
-        > *   If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
-        > *   Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
-        > *   You can call this operation only on a PolarDB for MySQL cluster.
-        > *   By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
+        @summary Grants a standard account the permissions to access one or more databases in a specified PolarDB cluster.
+        
+        @description >    An account can be authorized to access one or more databases.
+        >    If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
+        >    Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        >    You can call this operation only on a PolarDB for MySQL cluster.
+        >    By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
         
         @param request: GrantAccountPrivilegeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: GrantAccountPrivilegeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10042,48 +11980,59 @@
         )
 
     def grant_account_privilege(
         self,
         request: polardb_20170801_models.GrantAccountPrivilegeRequest,
     ) -> polardb_20170801_models.GrantAccountPrivilegeResponse:
         """
-        >    An account can be authorized to access one or more databases.
-        > *   If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
-        > *   Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
-        > *   You can call this operation only on a PolarDB for MySQL cluster.
-        > *   By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
+        @summary Grants a standard account the permissions to access one or more databases in a specified PolarDB cluster.
+        
+        @description >    An account can be authorized to access one or more databases.
+        >    If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
+        >    Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        >    You can call this operation only on a PolarDB for MySQL cluster.
+        >    By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
         
         @param request: GrantAccountPrivilegeRequest
         @return: GrantAccountPrivilegeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.grant_account_privilege_with_options(request, runtime)
 
     async def grant_account_privilege_async(
         self,
         request: polardb_20170801_models.GrantAccountPrivilegeRequest,
     ) -> polardb_20170801_models.GrantAccountPrivilegeResponse:
         """
-        >    An account can be authorized to access one or more databases.
-        > *   If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
-        > *   Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
-        > *   You can call this operation only on a PolarDB for MySQL cluster.
-        > *   By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
+        @summary Grants a standard account the permissions to access one or more databases in a specified PolarDB cluster.
+        
+        @description >    An account can be authorized to access one or more databases.
+        >    If the specified account already has the access permissions on the specified databases, the operation returns a successful response.
+        >    Before you call this operation, make sure that the cluster is in the Running state. Otherwise, the operation fails.
+        >    You can call this operation only on a PolarDB for MySQL cluster.
+        >    By default, a privileged account for a cluster has all the permissions on the databases in the cluster.
         
         @param request: GrantAccountPrivilegeRequest
         @return: GrantAccountPrivilegeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.grant_account_privilege_with_options_async(request, runtime)
 
     def list_tag_resources_with_options(
         self,
         request: polardb_20170801_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are bound to one or more PolarDB clusters, or queries the PolarDB clusters to which one or more tags are bound.
+        
+        @param request: ListTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -10120,14 +12069,21 @@
         )
 
     async def list_tag_resources_with_options_async(
         self,
         request: polardb_20170801_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are bound to one or more PolarDB clusters, or queries the PolarDB clusters to which one or more tags are bound.
+        
+        @param request: ListTagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -10163,29 +12119,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tag_resources(
         self,
         request: polardb_20170801_models.ListTagResourcesRequest,
     ) -> polardb_20170801_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are bound to one or more PolarDB clusters, or queries the PolarDB clusters to which one or more tags are bound.
+        
+        @param request: ListTagResourcesRequest
+        @return: ListTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_tag_resources_with_options(request, runtime)
 
     async def list_tag_resources_async(
         self,
         request: polardb_20170801_models.ListTagResourcesRequest,
     ) -> polardb_20170801_models.ListTagResourcesResponse:
+        """
+        @summary Queries the tags that are bound to one or more PolarDB clusters, or queries the PolarDB clusters to which one or more tags are bound.
+        
+        @param request: ListTagResourcesRequest
+        @return: ListTagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_tag_resources_with_options_async(request, runtime)
 
     def manually_start_dbcluster_with_options(
         self,
         request: polardb_20170801_models.ManuallyStartDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ManuallyStartDBClusterResponse:
+        """
+        @summary Manually starts a cluster.
+        
+        @param request: ManuallyStartDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ManuallyStartDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -10216,14 +12191,21 @@
         )
 
     async def manually_start_dbcluster_with_options_async(
         self,
         request: polardb_20170801_models.ManuallyStartDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ManuallyStartDBClusterResponse:
+        """
+        @summary Manually starts a cluster.
+        
+        @param request: ManuallyStartDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ManuallyStartDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -10253,29 +12235,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def manually_start_dbcluster(
         self,
         request: polardb_20170801_models.ManuallyStartDBClusterRequest,
     ) -> polardb_20170801_models.ManuallyStartDBClusterResponse:
+        """
+        @summary Manually starts a cluster.
+        
+        @param request: ManuallyStartDBClusterRequest
+        @return: ManuallyStartDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.manually_start_dbcluster_with_options(request, runtime)
 
     async def manually_start_dbcluster_async(
         self,
         request: polardb_20170801_models.ManuallyStartDBClusterRequest,
     ) -> polardb_20170801_models.ManuallyStartDBClusterResponse:
+        """
+        @summary Manually starts a cluster.
+        
+        @param request: ManuallyStartDBClusterRequest
+        @return: ManuallyStartDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.manually_start_dbcluster_with_options_async(request, runtime)
 
     def modify_account_description_with_options(
         self,
         request: polardb_20170801_models.ModifyAccountDescriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyAccountDescriptionResponse:
+        """
+        @summary Modifies the description of a database account of a PolarDB cluster.
+        
+        @param request: ModifyAccountDescriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAccountDescriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_description):
             query['AccountDescription'] = request.account_description
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -10308,14 +12309,21 @@
         )
 
     async def modify_account_description_with_options_async(
         self,
         request: polardb_20170801_models.ModifyAccountDescriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyAccountDescriptionResponse:
+        """
+        @summary Modifies the description of a database account of a PolarDB cluster.
+        
+        @param request: ModifyAccountDescriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAccountDescriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_description):
             query['AccountDescription'] = request.account_description
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -10347,29 +12355,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_account_description(
         self,
         request: polardb_20170801_models.ModifyAccountDescriptionRequest,
     ) -> polardb_20170801_models.ModifyAccountDescriptionResponse:
+        """
+        @summary Modifies the description of a database account of a PolarDB cluster.
+        
+        @param request: ModifyAccountDescriptionRequest
+        @return: ModifyAccountDescriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_account_description_with_options(request, runtime)
 
     async def modify_account_description_async(
         self,
         request: polardb_20170801_models.ModifyAccountDescriptionRequest,
     ) -> polardb_20170801_models.ModifyAccountDescriptionResponse:
+        """
+        @summary Modifies the description of a database account of a PolarDB cluster.
+        
+        @param request: ModifyAccountDescriptionRequest
+        @return: ModifyAccountDescriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_account_description_with_options_async(request, runtime)
 
     def modify_account_password_with_options(
         self,
         request: polardb_20170801_models.ModifyAccountPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyAccountPasswordResponse:
+        """
+        @summary Changes the password of a database account for a specified PolarDB cluster.
+        
+        @param request: ModifyAccountPasswordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAccountPasswordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.new_account_password):
@@ -10404,14 +12431,21 @@
         )
 
     async def modify_account_password_with_options_async(
         self,
         request: polardb_20170801_models.ModifyAccountPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyAccountPasswordResponse:
+        """
+        @summary Changes the password of a database account for a specified PolarDB cluster.
+        
+        @param request: ModifyAccountPasswordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAccountPasswordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.new_account_password):
@@ -10445,29 +12479,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_account_password(
         self,
         request: polardb_20170801_models.ModifyAccountPasswordRequest,
     ) -> polardb_20170801_models.ModifyAccountPasswordResponse:
+        """
+        @summary Changes the password of a database account for a specified PolarDB cluster.
+        
+        @param request: ModifyAccountPasswordRequest
+        @return: ModifyAccountPasswordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_account_password_with_options(request, runtime)
 
     async def modify_account_password_async(
         self,
         request: polardb_20170801_models.ModifyAccountPasswordRequest,
     ) -> polardb_20170801_models.ModifyAccountPasswordResponse:
+        """
+        @summary Changes the password of a database account for a specified PolarDB cluster.
+        
+        @param request: ModifyAccountPasswordRequest
+        @return: ModifyAccountPasswordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_account_password_with_options_async(request, runtime)
 
     def modify_auto_renew_attribute_with_options(
         self,
         request: polardb_20170801_models.ModifyAutoRenewAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyAutoRenewAttributeResponse:
+        """
+        @summary Modifies the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: ModifyAutoRenewAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAutoRenewAttributeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_ids):
             query['DBClusterIds'] = request.dbcluster_ids
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.owner_account):
@@ -10506,14 +12559,21 @@
         )
 
     async def modify_auto_renew_attribute_with_options_async(
         self,
         request: polardb_20170801_models.ModifyAutoRenewAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyAutoRenewAttributeResponse:
+        """
+        @summary Modifies the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: ModifyAutoRenewAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAutoRenewAttributeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_ids):
             query['DBClusterIds'] = request.dbcluster_ids
         if not UtilClient.is_unset(request.duration):
             query['Duration'] = request.duration
         if not UtilClient.is_unset(request.owner_account):
@@ -10551,31 +12611,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_auto_renew_attribute(
         self,
         request: polardb_20170801_models.ModifyAutoRenewAttributeRequest,
     ) -> polardb_20170801_models.ModifyAutoRenewAttributeResponse:
+        """
+        @summary Modifies the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: ModifyAutoRenewAttributeRequest
+        @return: ModifyAutoRenewAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_auto_renew_attribute_with_options(request, runtime)
 
     async def modify_auto_renew_attribute_async(
         self,
         request: polardb_20170801_models.ModifyAutoRenewAttributeRequest,
     ) -> polardb_20170801_models.ModifyAutoRenewAttributeResponse:
+        """
+        @summary Modifies the auto-renewal attributes of a subscription PolarDB cluster.
+        
+        @param request: ModifyAutoRenewAttributeRequest
+        @return: ModifyAutoRenewAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_auto_renew_attribute_with_options_async(request, runtime)
 
     def modify_backup_policy_with_options(
         self,
         request: polardb_20170801_models.ModifyBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyBackupPolicyResponse:
         """
-        > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](~~280422~~).
+        @summary Modifies the automatic backup policy of a PolarDB cluster.
+        
+        @description > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](https://help.aliyun.com/document_detail/280422.html).
         
         @param request: ModifyBackupPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyBackupPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10634,15 +12708,17 @@
 
     async def modify_backup_policy_with_options_async(
         self,
         request: polardb_20170801_models.ModifyBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyBackupPolicyResponse:
         """
-        > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](~~280422~~).
+        @summary Modifies the automatic backup policy of a PolarDB cluster.
+        
+        @description > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](https://help.aliyun.com/document_detail/280422.html).
         
         @param request: ModifyBackupPolicyRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyBackupPolicyResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10700,40 +12776,51 @@
         )
 
     def modify_backup_policy(
         self,
         request: polardb_20170801_models.ModifyBackupPolicyRequest,
     ) -> polardb_20170801_models.ModifyBackupPolicyResponse:
         """
-        > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](~~280422~~).
+        @summary Modifies the automatic backup policy of a PolarDB cluster.
+        
+        @description > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](https://help.aliyun.com/document_detail/280422.html).
         
         @param request: ModifyBackupPolicyRequest
         @return: ModifyBackupPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_backup_policy_with_options(request, runtime)
 
     async def modify_backup_policy_async(
         self,
         request: polardb_20170801_models.ModifyBackupPolicyRequest,
     ) -> polardb_20170801_models.ModifyBackupPolicyResponse:
         """
-        > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](~~280422~~).
+        @summary Modifies the automatic backup policy of a PolarDB cluster.
+        
+        @description > You can also modify the automatic backup policy of a PolarDB cluster in the console. For more information, see [Backup settings](https://help.aliyun.com/document_detail/280422.html).
         
         @param request: ModifyBackupPolicyRequest
         @return: ModifyBackupPolicyResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_backup_policy_with_options_async(request, runtime)
 
     def modify_dbcluster_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterResponse:
+        """
+        @summary Modifies the configurations of a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compress_storage):
             query['CompressStorage'] = request.compress_storage
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.data_sync_mode):
@@ -10774,14 +12861,21 @@
         )
 
     async def modify_dbcluster_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterResponse:
+        """
+        @summary Modifies the configurations of a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.compress_storage):
             query['CompressStorage'] = request.compress_storage
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.data_sync_mode):
@@ -10821,29 +12915,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster(
         self,
         request: polardb_20170801_models.ModifyDBClusterRequest,
     ) -> polardb_20170801_models.ModifyDBClusterResponse:
+        """
+        @summary Modifies the configurations of a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBClusterRequest
+        @return: ModifyDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_with_options(request, runtime)
 
     async def modify_dbcluster_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterRequest,
     ) -> polardb_20170801_models.ModifyDBClusterResponse:
+        """
+        @summary Modifies the configurations of a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBClusterRequest
+        @return: ModifyDBClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_with_options_async(request, runtime)
 
     def modify_dbcluster_access_whitelist_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterAccessWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterAccessWhitelistResponse:
+        """
+        @summary Creates or modifies the whitelists (IP whitelists and security groups) of a specified cluster.
+        
+        @param request: ModifyDBClusterAccessWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterAccessWhitelistResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_iparray_attribute):
             query['DBClusterIPArrayAttribute'] = request.dbcluster_iparray_attribute
         if not UtilClient.is_unset(request.dbcluster_iparray_name):
             query['DBClusterIPArrayName'] = request.dbcluster_iparray_name
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -10884,14 +12997,21 @@
         )
 
     async def modify_dbcluster_access_whitelist_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterAccessWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterAccessWhitelistResponse:
+        """
+        @summary Creates or modifies the whitelists (IP whitelists and security groups) of a specified cluster.
+        
+        @param request: ModifyDBClusterAccessWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterAccessWhitelistResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_iparray_attribute):
             query['DBClusterIPArrayAttribute'] = request.dbcluster_iparray_attribute
         if not UtilClient.is_unset(request.dbcluster_iparray_name):
             query['DBClusterIPArrayName'] = request.dbcluster_iparray_name
         if not UtilClient.is_unset(request.dbcluster_id):
@@ -10931,29 +13051,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_access_whitelist(
         self,
         request: polardb_20170801_models.ModifyDBClusterAccessWhitelistRequest,
     ) -> polardb_20170801_models.ModifyDBClusterAccessWhitelistResponse:
+        """
+        @summary Creates or modifies the whitelists (IP whitelists and security groups) of a specified cluster.
+        
+        @param request: ModifyDBClusterAccessWhitelistRequest
+        @return: ModifyDBClusterAccessWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_access_whitelist_with_options(request, runtime)
 
     async def modify_dbcluster_access_whitelist_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterAccessWhitelistRequest,
     ) -> polardb_20170801_models.ModifyDBClusterAccessWhitelistResponse:
+        """
+        @summary Creates or modifies the whitelists (IP whitelists and security groups) of a specified cluster.
+        
+        @param request: ModifyDBClusterAccessWhitelistRequest
+        @return: ModifyDBClusterAccessWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_access_whitelist_with_options_async(request, runtime)
 
     def modify_dbcluster_and_nodes_parameters_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterAndNodesParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterAndNodesParametersResponse:
+        """
+        @summary Modifies cluster parameters and applies them to specified nodes.
+        
+        @param request: ModifyDBClusterAndNodesParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterAndNodesParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_ids):
             query['DBNodeIds'] = request.dbnode_ids
         if not UtilClient.is_unset(request.from_time_service):
@@ -10994,14 +13133,21 @@
         )
 
     async def modify_dbcluster_and_nodes_parameters_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterAndNodesParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterAndNodesParametersResponse:
+        """
+        @summary Modifies cluster parameters and applies them to specified nodes.
+        
+        @param request: ModifyDBClusterAndNodesParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterAndNodesParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_ids):
             query['DBNodeIds'] = request.dbnode_ids
         if not UtilClient.is_unset(request.from_time_service):
@@ -11041,29 +13187,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_and_nodes_parameters(
         self,
         request: polardb_20170801_models.ModifyDBClusterAndNodesParametersRequest,
     ) -> polardb_20170801_models.ModifyDBClusterAndNodesParametersResponse:
+        """
+        @summary Modifies cluster parameters and applies them to specified nodes.
+        
+        @param request: ModifyDBClusterAndNodesParametersRequest
+        @return: ModifyDBClusterAndNodesParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_and_nodes_parameters_with_options(request, runtime)
 
     async def modify_dbcluster_and_nodes_parameters_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterAndNodesParametersRequest,
     ) -> polardb_20170801_models.ModifyDBClusterAndNodesParametersResponse:
+        """
+        @summary Modifies cluster parameters and applies them to specified nodes.
+        
+        @param request: ModifyDBClusterAndNodesParametersRequest
+        @return: ModifyDBClusterAndNodesParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_and_nodes_parameters_with_options_async(request, runtime)
 
     def modify_dbcluster_audit_log_collector_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterAuditLogCollectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterAuditLogCollectorResponse:
+        """
+        @summary Enables or disables SQL collector for a PolarDB cluster. The features related to SQL collector include Audit Logs and SQL Explorer.
+        
+        @param request: ModifyDBClusterAuditLogCollectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterAuditLogCollectorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.collector_status):
             query['CollectorStatus'] = request.collector_status
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -11094,14 +13259,21 @@
         )
 
     async def modify_dbcluster_audit_log_collector_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterAuditLogCollectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterAuditLogCollectorResponse:
+        """
+        @summary Enables or disables SQL collector for a PolarDB cluster. The features related to SQL collector include Audit Logs and SQL Explorer.
+        
+        @param request: ModifyDBClusterAuditLogCollectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterAuditLogCollectorResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.collector_status):
             query['CollectorStatus'] = request.collector_status
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -11131,29 +13303,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_audit_log_collector(
         self,
         request: polardb_20170801_models.ModifyDBClusterAuditLogCollectorRequest,
     ) -> polardb_20170801_models.ModifyDBClusterAuditLogCollectorResponse:
+        """
+        @summary Enables or disables SQL collector for a PolarDB cluster. The features related to SQL collector include Audit Logs and SQL Explorer.
+        
+        @param request: ModifyDBClusterAuditLogCollectorRequest
+        @return: ModifyDBClusterAuditLogCollectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_audit_log_collector_with_options(request, runtime)
 
     async def modify_dbcluster_audit_log_collector_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterAuditLogCollectorRequest,
     ) -> polardb_20170801_models.ModifyDBClusterAuditLogCollectorResponse:
+        """
+        @summary Enables or disables SQL collector for a PolarDB cluster. The features related to SQL collector include Audit Logs and SQL Explorer.
+        
+        @param request: ModifyDBClusterAuditLogCollectorRequest
+        @return: ModifyDBClusterAuditLogCollectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_audit_log_collector_with_options_async(request, runtime)
 
     def modify_dbcluster_deletion_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterDeletionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterDeletionResponse:
+        """
+        @summary Enables or disables the cluster lock feature for a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDeletionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterDeletionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -11184,14 +13375,21 @@
         )
 
     async def modify_dbcluster_deletion_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterDeletionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterDeletionResponse:
+        """
+        @summary Enables or disables the cluster lock feature for a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDeletionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterDeletionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -11221,29 +13419,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_deletion(
         self,
         request: polardb_20170801_models.ModifyDBClusterDeletionRequest,
     ) -> polardb_20170801_models.ModifyDBClusterDeletionResponse:
+        """
+        @summary Enables or disables the cluster lock feature for a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDeletionRequest
+        @return: ModifyDBClusterDeletionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_deletion_with_options(request, runtime)
 
     async def modify_dbcluster_deletion_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterDeletionRequest,
     ) -> polardb_20170801_models.ModifyDBClusterDeletionResponse:
+        """
+        @summary Enables or disables the cluster lock feature for a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDeletionRequest
+        @return: ModifyDBClusterDeletionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_deletion_with_options_async(request, runtime)
 
     def modify_dbcluster_description_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterDescriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterDescriptionResponse:
+        """
+        @summary Modifies the name of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDescriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterDescriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -11274,14 +13491,21 @@
         )
 
     async def modify_dbcluster_description_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterDescriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterDescriptionResponse:
+        """
+        @summary Modifies the name of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDescriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterDescriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_description):
             query['DBClusterDescription'] = request.dbcluster_description
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -11311,29 +13535,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_description(
         self,
         request: polardb_20170801_models.ModifyDBClusterDescriptionRequest,
     ) -> polardb_20170801_models.ModifyDBClusterDescriptionResponse:
+        """
+        @summary Modifies the name of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDescriptionRequest
+        @return: ModifyDBClusterDescriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_description_with_options(request, runtime)
 
     async def modify_dbcluster_description_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterDescriptionRequest,
     ) -> polardb_20170801_models.ModifyDBClusterDescriptionResponse:
+        """
+        @summary Modifies the name of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterDescriptionRequest
+        @return: ModifyDBClusterDescriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_description_with_options_async(request, runtime)
 
     def modify_dbcluster_endpoint_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterEndpointResponse:
+        """
+        @summary Modifies the attributes of a specified PolarDB cluster endpoint. For example, you can modify the following attributes for the specified cluster endpoint: read/write mode, consistency level, transaction splitting, primary node accepts read requests, and connection pool. You can also call the operation to specify whether newly added nodes are automatically associated with the specified cluster endpoint.
+        
+        @param request: ModifyDBClusterEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_add_new_nodes):
             query['AutoAddNewNodes'] = request.auto_add_new_nodes
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_description):
@@ -11374,14 +13617,21 @@
         )
 
     async def modify_dbcluster_endpoint_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterEndpointResponse:
+        """
+        @summary Modifies the attributes of a specified PolarDB cluster endpoint. For example, you can modify the following attributes for the specified cluster endpoint: read/write mode, consistency level, transaction splitting, primary node accepts read requests, and connection pool. You can also call the operation to specify whether newly added nodes are automatically associated with the specified cluster endpoint.
+        
+        @param request: ModifyDBClusterEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.auto_add_new_nodes):
             query['AutoAddNewNodes'] = request.auto_add_new_nodes
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_description):
@@ -11421,31 +13671,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_endpoint(
         self,
         request: polardb_20170801_models.ModifyDBClusterEndpointRequest,
     ) -> polardb_20170801_models.ModifyDBClusterEndpointResponse:
+        """
+        @summary Modifies the attributes of a specified PolarDB cluster endpoint. For example, you can modify the following attributes for the specified cluster endpoint: read/write mode, consistency level, transaction splitting, primary node accepts read requests, and connection pool. You can also call the operation to specify whether newly added nodes are automatically associated with the specified cluster endpoint.
+        
+        @param request: ModifyDBClusterEndpointRequest
+        @return: ModifyDBClusterEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_endpoint_with_options(request, runtime)
 
     async def modify_dbcluster_endpoint_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterEndpointRequest,
     ) -> polardb_20170801_models.ModifyDBClusterEndpointResponse:
+        """
+        @summary Modifies the attributes of a specified PolarDB cluster endpoint. For example, you can modify the following attributes for the specified cluster endpoint: read/write mode, consistency level, transaction splitting, primary node accepts read requests, and connection pool. You can also call the operation to specify whether newly added nodes are automatically associated with the specified cluster endpoint.
+        
+        @param request: ModifyDBClusterEndpointRequest
+        @return: ModifyDBClusterEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_endpoint_with_options_async(request, runtime)
 
     def modify_dbcluster_maintain_time_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterMaintainTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterMaintainTimeResponse:
         """
-        >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
+        @summary Modifies the maintenance window of a PolarDB cluster.
+        
+        @description >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
         
         @param request: ModifyDBClusterMaintainTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterMaintainTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11482,15 +13746,17 @@
 
     async def modify_dbcluster_maintain_time_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterMaintainTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterMaintainTimeResponse:
         """
-        >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
+        @summary Modifies the maintenance window of a PolarDB cluster.
+        
+        @description >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
         
         @param request: ModifyDBClusterMaintainTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterMaintainTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11526,44 +13792,50 @@
         )
 
     def modify_dbcluster_maintain_time(
         self,
         request: polardb_20170801_models.ModifyDBClusterMaintainTimeRequest,
     ) -> polardb_20170801_models.ModifyDBClusterMaintainTimeResponse:
         """
-        >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
+        @summary Modifies the maintenance window of a PolarDB cluster.
+        
+        @description >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
         
         @param request: ModifyDBClusterMaintainTimeRequest
         @return: ModifyDBClusterMaintainTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_maintain_time_with_options(request, runtime)
 
     async def modify_dbcluster_maintain_time_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterMaintainTimeRequest,
     ) -> polardb_20170801_models.ModifyDBClusterMaintainTimeResponse:
         """
-        >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
+        @summary Modifies the maintenance window of a PolarDB cluster.
+        
+        @description >  We recommend that you set the routine maintenance window to off-peak hours. Alibaba Cloud maintains your cluster within the specified maintenance window to minimize the negative impacts on your business.
         
         @param request: ModifyDBClusterMaintainTimeRequest
         @return: ModifyDBClusterMaintainTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_maintain_time_with_options_async(request, runtime)
 
     def modify_dbcluster_migration_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterMigrationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterMigrationResponse:
         """
-        You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
-        *   You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Switches or rolls back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        
+        @description    You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
+        You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: ModifyDBClusterMigrationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterMigrationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11608,17 +13880,19 @@
 
     async def modify_dbcluster_migration_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterMigrationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterMigrationResponse:
         """
-        You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
-        *   You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Switches or rolls back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        
+        @description    You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
+        You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: ModifyDBClusterMigrationRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterMigrationResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11662,56 +13936,62 @@
         )
 
     def modify_dbcluster_migration(
         self,
         request: polardb_20170801_models.ModifyDBClusterMigrationRequest,
     ) -> polardb_20170801_models.ModifyDBClusterMigrationResponse:
         """
-        You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
-        *   You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Switches or rolls back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        
+        @description    You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
+        You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: ModifyDBClusterMigrationRequest
         @return: ModifyDBClusterMigrationResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_migration_with_options(request, runtime)
 
     async def modify_dbcluster_migration_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterMigrationRequest,
     ) -> polardb_20170801_models.ModifyDBClusterMigrationResponse:
         """
-        You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
-        *   You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
-        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](~~98169~~) operation to create an upgrade task. Set the **CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](~~121582~~).
+        @summary Switches or rolls back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        
+        @description    You can call this operation to switch the task that migrates data from ApsaraDB for RDS to PolarDB.
+        You can call this operation to roll back the task that migrates data from ApsaraDB for RDS to PolarDB.
+        > Before you call this operation, ensure that a one-click upgrade task has been created for the cluster. You can call the [CreateDBCluster](https://help.aliyun.com/document_detail/98169.html) operation to create an upgrade task. Set the *CreationOption** parameter to **MigrationFromRDS**. For more information, see [Create a PolarDB for MySQL cluster by using the Migration from RDS method](https://help.aliyun.com/document_detail/121582.html).
         
         @param request: ModifyDBClusterMigrationRequest
         @return: ModifyDBClusterMigrationResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_migration_with_options_async(request, runtime)
 
     def modify_dbcluster_monitor_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterMonitorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterMonitorResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        @summary Modifies the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
         
         @param request: ModifyDBClusterMonitorRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterMonitorResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11748,25 +14028,27 @@
 
     async def modify_dbcluster_monitor_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterMonitorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterMonitorResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        @summary Modifies the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
         
         @param request: ModifyDBClusterMonitorRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterMonitorResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11802,64 +14084,70 @@
         )
 
     def modify_dbcluster_monitor(
         self,
         request: polardb_20170801_models.ModifyDBClusterMonitorRequest,
     ) -> polardb_20170801_models.ModifyDBClusterMonitorResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        @summary Modifies the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
         
         @param request: ModifyDBClusterMonitorRequest
         @return: ModifyDBClusterMonitorResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_monitor_with_options(request, runtime)
 
     async def modify_dbcluster_monitor_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterMonitorRequest,
     ) -> polardb_20170801_models.ModifyDBClusterMonitorResponse:
         """
-        When the monitoring data is collected every 5 seconds:
-        *   If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
-        *   When the monitoring data is collected every 60 seconds:
-        *   If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
-        *   If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
-        *   If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
-        *   When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        @summary Modifies the interval at which the monitoring data of a PolarDB cluster is collected.
+        
+        @description    When the monitoring data is collected every 5 seconds:
+        If the query time range is less than or equal to 1 hour, the data is displayed at intervals of 5 seconds.
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
+        When the monitoring data is collected every 60 seconds:
+        If the query time range is less than or equal to one day, the data is displayed at intervals of 1 minute.
+        If the query time range is less than or equal to seven days, the data is displayed at intervals of 10 minutes.
+        If the query time range is less than or equal to 30 days, the data is displayed at intervals of 1 hour.
+        When the query time range is greater than 30 days, the data is displayed at intervals of 1 day.
         
         @param request: ModifyDBClusterMonitorRequest
         @return: ModifyDBClusterMonitorResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_monitor_with_options_async(request, runtime)
 
     def modify_dbcluster_parameters_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterParametersResponse:
         """
-        PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
-        **\
-        **Only PolarDB for MySQL clusters support parameter templates.
+        @summary Modifies the parameters of a specified PolarDB cluster or applies existing parameter templates to a specified cluster.
+        
+        @description PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
+        *\
+        *Only PolarDB for MySQL clusters support parameter templates.
         
         @param request: ModifyDBClusterParametersRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterParametersResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11904,17 +14192,19 @@
 
     async def modify_dbcluster_parameters_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterParametersResponse:
         """
-        PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
-        **\
-        **Only PolarDB for MySQL clusters support parameter templates.
+        @summary Modifies the parameters of a specified PolarDB cluster or applies existing parameter templates to a specified cluster.
+        
+        @description PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
+        *\
+        *Only PolarDB for MySQL clusters support parameter templates.
         
         @param request: ModifyDBClusterParametersRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterParametersResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11958,44 +14248,55 @@
         )
 
     def modify_dbcluster_parameters(
         self,
         request: polardb_20170801_models.ModifyDBClusterParametersRequest,
     ) -> polardb_20170801_models.ModifyDBClusterParametersResponse:
         """
-        PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
-        **\
-        **Only PolarDB for MySQL clusters support parameter templates.
+        @summary Modifies the parameters of a specified PolarDB cluster or applies existing parameter templates to a specified cluster.
+        
+        @description PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
+        *\
+        *Only PolarDB for MySQL clusters support parameter templates.
         
         @param request: ModifyDBClusterParametersRequest
         @return: ModifyDBClusterParametersResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_parameters_with_options(request, runtime)
 
     async def modify_dbcluster_parameters_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterParametersRequest,
     ) -> polardb_20170801_models.ModifyDBClusterParametersResponse:
         """
-        PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](~~207009~~).
-        **\
-        **Only PolarDB for MySQL clusters support parameter templates.
+        @summary Modifies the parameters of a specified PolarDB cluster or applies existing parameter templates to a specified cluster.
+        
+        @description PolarDB supports the parameter template feature to centrally manage clusters. You can configure a number of parameters at a time by using a parameter template and apply the template to a PolarDB cluster. For more information, see [Use a parameter template](https://help.aliyun.com/document_detail/207009.html).
+        *\
+        *Only PolarDB for MySQL clusters support parameter templates.
         
         @param request: ModifyDBClusterParametersRequest
         @return: ModifyDBClusterParametersResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_parameters_with_options_async(request, runtime)
 
     def modify_dbcluster_primary_zone_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterPrimaryZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterPrimaryZoneResponse:
+        """
+        @summary Modifies the primary zone of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterPrimaryZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterPrimaryZoneResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.from_time_service):
             query['FromTimeService'] = request.from_time_service
         if not UtilClient.is_unset(request.is_switch_over_for_disaster):
@@ -12040,14 +14341,21 @@
         )
 
     async def modify_dbcluster_primary_zone_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterPrimaryZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterPrimaryZoneResponse:
+        """
+        @summary Modifies the primary zone of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterPrimaryZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterPrimaryZoneResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.from_time_service):
             query['FromTimeService'] = request.from_time_service
         if not UtilClient.is_unset(request.is_switch_over_for_disaster):
@@ -12091,29 +14399,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_primary_zone(
         self,
         request: polardb_20170801_models.ModifyDBClusterPrimaryZoneRequest,
     ) -> polardb_20170801_models.ModifyDBClusterPrimaryZoneResponse:
+        """
+        @summary Modifies the primary zone of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterPrimaryZoneRequest
+        @return: ModifyDBClusterPrimaryZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_primary_zone_with_options(request, runtime)
 
     async def modify_dbcluster_primary_zone_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterPrimaryZoneRequest,
     ) -> polardb_20170801_models.ModifyDBClusterPrimaryZoneResponse:
+        """
+        @summary Modifies the primary zone of a PolarDB cluster.
+        
+        @param request: ModifyDBClusterPrimaryZoneRequest
+        @return: ModifyDBClusterPrimaryZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_primary_zone_with_options_async(request, runtime)
 
     def modify_dbcluster_resource_group_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterResourceGroupResponse:
+        """
+        @param request: ModifyDBClusterResourceGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -12146,14 +14471,19 @@
         )
 
     async def modify_dbcluster_resource_group_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterResourceGroupResponse:
+        """
+        @param request: ModifyDBClusterResourceGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -12185,29 +14515,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_resource_group(
         self,
         request: polardb_20170801_models.ModifyDBClusterResourceGroupRequest,
     ) -> polardb_20170801_models.ModifyDBClusterResourceGroupResponse:
+        """
+        @param request: ModifyDBClusterResourceGroupRequest
+        @return: ModifyDBClusterResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_resource_group_with_options(request, runtime)
 
     async def modify_dbcluster_resource_group_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterResourceGroupRequest,
     ) -> polardb_20170801_models.ModifyDBClusterResourceGroupResponse:
+        """
+        @param request: ModifyDBClusterResourceGroupRequest
+        @return: ModifyDBClusterResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_resource_group_with_options_async(request, runtime)
 
     def modify_dbcluster_sslwith_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterSSLRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterSSLResponse:
+        """
+        @summary Enables or disables Secure Sockets Layer (SSL) encryption or updates the Certificate Authorities (CA) certificate for a specified PolarDB cluster.
+        
+        @param request: ModifyDBClusterSSLRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterSSLResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
             query['DBEndpointId'] = request.dbendpoint_id
         if not UtilClient.is_unset(request.net_type):
@@ -12244,14 +14589,21 @@
         )
 
     async def modify_dbcluster_sslwith_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterSSLRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterSSLResponse:
+        """
+        @summary Enables or disables Secure Sockets Layer (SSL) encryption or updates the Certificate Authorities (CA) certificate for a specified PolarDB cluster.
+        
+        @param request: ModifyDBClusterSSLRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterSSLResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
             query['DBEndpointId'] = request.dbendpoint_id
         if not UtilClient.is_unset(request.net_type):
@@ -12287,29 +14639,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_ssl(
         self,
         request: polardb_20170801_models.ModifyDBClusterSSLRequest,
     ) -> polardb_20170801_models.ModifyDBClusterSSLResponse:
+        """
+        @summary Enables or disables Secure Sockets Layer (SSL) encryption or updates the Certificate Authorities (CA) certificate for a specified PolarDB cluster.
+        
+        @param request: ModifyDBClusterSSLRequest
+        @return: ModifyDBClusterSSLResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_sslwith_options(request, runtime)
 
     async def modify_dbcluster_ssl_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterSSLRequest,
     ) -> polardb_20170801_models.ModifyDBClusterSSLResponse:
+        """
+        @summary Enables or disables Secure Sockets Layer (SSL) encryption or updates the Certificate Authorities (CA) certificate for a specified PolarDB cluster.
+        
+        @param request: ModifyDBClusterSSLRequest
+        @return: ModifyDBClusterSSLResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_sslwith_options_async(request, runtime)
 
     def modify_dbcluster_serverless_conf_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterServerlessConfRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterServerlessConfResponse:
+        """
+        @summary Modifies the configurations of a serverless cluster.
+        
+        @param request: ModifyDBClusterServerlessConfRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterServerlessConfResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_shut_down):
             query['AllowShutDown'] = request.allow_shut_down
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.from_time_service):
@@ -12336,14 +14707,20 @@
             query['ScaleMin'] = request.scale_min
         if not UtilClient.is_unset(request.scale_ro_num_max):
             query['ScaleRoNumMax'] = request.scale_ro_num_max
         if not UtilClient.is_unset(request.scale_ro_num_min):
             query['ScaleRoNumMin'] = request.scale_ro_num_min
         if not UtilClient.is_unset(request.seconds_until_auto_pause):
             query['SecondsUntilAutoPause'] = request.seconds_until_auto_pause
+        if not UtilClient.is_unset(request.serverless_rule_cpu_enlarge_threshold):
+            query['ServerlessRuleCpuEnlargeThreshold'] = request.serverless_rule_cpu_enlarge_threshold
+        if not UtilClient.is_unset(request.serverless_rule_cpu_shrink_threshold):
+            query['ServerlessRuleCpuShrinkThreshold'] = request.serverless_rule_cpu_shrink_threshold
+        if not UtilClient.is_unset(request.serverless_rule_mode):
+            query['ServerlessRuleMode'] = request.serverless_rule_mode
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDBClusterServerlessConf',
             version='2017-08-01',
             protocol='HTTPS',
@@ -12360,14 +14737,21 @@
         )
 
     async def modify_dbcluster_serverless_conf_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterServerlessConfRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterServerlessConfResponse:
+        """
+        @summary Modifies the configurations of a serverless cluster.
+        
+        @param request: ModifyDBClusterServerlessConfRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterServerlessConfResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.allow_shut_down):
             query['AllowShutDown'] = request.allow_shut_down
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.from_time_service):
@@ -12394,14 +14778,20 @@
             query['ScaleMin'] = request.scale_min
         if not UtilClient.is_unset(request.scale_ro_num_max):
             query['ScaleRoNumMax'] = request.scale_ro_num_max
         if not UtilClient.is_unset(request.scale_ro_num_min):
             query['ScaleRoNumMin'] = request.scale_ro_num_min
         if not UtilClient.is_unset(request.seconds_until_auto_pause):
             query['SecondsUntilAutoPause'] = request.seconds_until_auto_pause
+        if not UtilClient.is_unset(request.serverless_rule_cpu_enlarge_threshold):
+            query['ServerlessRuleCpuEnlargeThreshold'] = request.serverless_rule_cpu_enlarge_threshold
+        if not UtilClient.is_unset(request.serverless_rule_cpu_shrink_threshold):
+            query['ServerlessRuleCpuShrinkThreshold'] = request.serverless_rule_cpu_shrink_threshold
+        if not UtilClient.is_unset(request.serverless_rule_mode):
+            query['ServerlessRuleMode'] = request.serverless_rule_mode
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ModifyDBClusterServerlessConf',
             version='2017-08-01',
             protocol='HTTPS',
@@ -12417,29 +14807,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_serverless_conf(
         self,
         request: polardb_20170801_models.ModifyDBClusterServerlessConfRequest,
     ) -> polardb_20170801_models.ModifyDBClusterServerlessConfResponse:
+        """
+        @summary Modifies the configurations of a serverless cluster.
+        
+        @param request: ModifyDBClusterServerlessConfRequest
+        @return: ModifyDBClusterServerlessConfResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_serverless_conf_with_options(request, runtime)
 
     async def modify_dbcluster_serverless_conf_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterServerlessConfRequest,
     ) -> polardb_20170801_models.ModifyDBClusterServerlessConfResponse:
+        """
+        @summary Modifies the configurations of a serverless cluster.
+        
+        @param request: ModifyDBClusterServerlessConfRequest
+        @return: ModifyDBClusterServerlessConfResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_serverless_conf_with_options_async(request, runtime)
 
     def modify_dbcluster_storage_space_with_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterStorageSpaceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterStorageSpaceResponse:
+        """
+        @summary Changes the storage capacity of a pay-as-you-go cluster of Enterprise Edition or a cluster of Standard Edition.
+        
+        @param request: ModifyDBClusterStorageSpaceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterStorageSpaceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -12478,14 +14887,21 @@
         )
 
     async def modify_dbcluster_storage_space_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterStorageSpaceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterStorageSpaceResponse:
+        """
+        @summary Changes the storage capacity of a pay-as-you-go cluster of Enterprise Edition or a cluster of Standard Edition.
+        
+        @param request: ModifyDBClusterStorageSpaceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBClusterStorageSpaceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -12523,32 +14939,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbcluster_storage_space(
         self,
         request: polardb_20170801_models.ModifyDBClusterStorageSpaceRequest,
     ) -> polardb_20170801_models.ModifyDBClusterStorageSpaceResponse:
+        """
+        @summary Changes the storage capacity of a pay-as-you-go cluster of Enterprise Edition or a cluster of Standard Edition.
+        
+        @param request: ModifyDBClusterStorageSpaceRequest
+        @return: ModifyDBClusterStorageSpaceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_storage_space_with_options(request, runtime)
 
     async def modify_dbcluster_storage_space_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterStorageSpaceRequest,
     ) -> polardb_20170801_models.ModifyDBClusterStorageSpaceResponse:
+        """
+        @summary Changes the storage capacity of a pay-as-you-go cluster of Enterprise Edition or a cluster of Standard Edition.
+        
+        @param request: ModifyDBClusterStorageSpaceRequest
+        @return: ModifyDBClusterStorageSpaceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_storage_space_with_options_async(request, runtime)
 
     def modify_dbcluster_tdewith_options(
         self,
         request: polardb_20170801_models.ModifyDBClusterTDERequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterTDEResponse:
         """
-        >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](~~153781~~).
-        > *   After TDE is enabled, you cannot disable TDE.
+        @summary Enables the TDE feature or changes the encryption method for a specified PolarDB for MySQL cluster.
+        
+        @description >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](https://help.aliyun.com/document_detail/153781.html).
+        >    After TDE is enabled, you cannot disable TDE.
         
         @param request: ModifyDBClusterTDERequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterTDEResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12591,16 +15021,18 @@
 
     async def modify_dbcluster_tdewith_options_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterTDERequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBClusterTDEResponse:
         """
-        >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](~~153781~~).
-        > *   After TDE is enabled, you cannot disable TDE.
+        @summary Enables the TDE feature or changes the encryption method for a specified PolarDB for MySQL cluster.
+        
+        @description >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](https://help.aliyun.com/document_detail/153781.html).
+        >    After TDE is enabled, you cannot disable TDE.
         
         @param request: ModifyDBClusterTDERequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDBClusterTDEResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12642,42 +15074,53 @@
         )
 
     def modify_dbcluster_tde(
         self,
         request: polardb_20170801_models.ModifyDBClusterTDERequest,
     ) -> polardb_20170801_models.ModifyDBClusterTDEResponse:
         """
-        >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](~~153781~~).
-        > *   After TDE is enabled, you cannot disable TDE.
+        @summary Enables the TDE feature or changes the encryption method for a specified PolarDB for MySQL cluster.
+        
+        @description >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](https://help.aliyun.com/document_detail/153781.html).
+        >    After TDE is enabled, you cannot disable TDE.
         
         @param request: ModifyDBClusterTDERequest
         @return: ModifyDBClusterTDEResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbcluster_tdewith_options(request, runtime)
 
     async def modify_dbcluster_tde_async(
         self,
         request: polardb_20170801_models.ModifyDBClusterTDERequest,
     ) -> polardb_20170801_models.ModifyDBClusterTDEResponse:
         """
-        >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](~~153781~~).
-        > *   After TDE is enabled, you cannot disable TDE.
+        @summary Enables the TDE feature or changes the encryption method for a specified PolarDB for MySQL cluster.
+        
+        @description >    To perform this operation, you must activate KMS first. For more information, see [Purchase a dedicated KMS instance](https://help.aliyun.com/document_detail/153781.html).
+        >    After TDE is enabled, you cannot disable TDE.
         
         @param request: ModifyDBClusterTDERequest
         @return: ModifyDBClusterTDEResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbcluster_tdewith_options_async(request, runtime)
 
     def modify_dbdescription_with_options(
         self,
         request: polardb_20170801_models.ModifyDBDescriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBDescriptionResponse:
+        """
+        @summary Modifies the description of a database in a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBDescriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBDescriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbdescription):
             query['DBDescription'] = request.dbdescription
         if not UtilClient.is_unset(request.dbname):
@@ -12710,14 +15153,21 @@
         )
 
     async def modify_dbdescription_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBDescriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBDescriptionResponse:
+        """
+        @summary Modifies the description of a database in a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBDescriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBDescriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbdescription):
             query['DBDescription'] = request.dbdescription
         if not UtilClient.is_unset(request.dbname):
@@ -12749,29 +15199,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbdescription(
         self,
         request: polardb_20170801_models.ModifyDBDescriptionRequest,
     ) -> polardb_20170801_models.ModifyDBDescriptionResponse:
+        """
+        @summary Modifies the description of a database in a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBDescriptionRequest
+        @return: ModifyDBDescriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbdescription_with_options(request, runtime)
 
     async def modify_dbdescription_async(
         self,
         request: polardb_20170801_models.ModifyDBDescriptionRequest,
     ) -> polardb_20170801_models.ModifyDBDescriptionResponse:
+        """
+        @summary Modifies the description of a database in a PolarDB for MySQL cluster.
+        
+        @param request: ModifyDBDescriptionRequest
+        @return: ModifyDBDescriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbdescription_with_options_async(request, runtime)
 
     def modify_dbendpoint_address_with_options(
         self,
         request: polardb_20170801_models.ModifyDBEndpointAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBEndpointAddressResponse:
+        """
+        @summary Modifies the endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, custom cluster endpoint, and private domain name.
+        
+        @param request: ModifyDBEndpointAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBEndpointAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.connection_string_prefix):
             query['ConnectionStringPrefix'] = request.connection_string_prefix
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
@@ -12812,14 +15281,21 @@
         )
 
     async def modify_dbendpoint_address_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBEndpointAddressRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBEndpointAddressResponse:
+        """
+        @summary Modifies the endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, custom cluster endpoint, and private domain name.
+        
+        @param request: ModifyDBEndpointAddressRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBEndpointAddressResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.connection_string_prefix):
             query['ConnectionStringPrefix'] = request.connection_string_prefix
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbendpoint_id):
@@ -12859,29 +15335,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbendpoint_address(
         self,
         request: polardb_20170801_models.ModifyDBEndpointAddressRequest,
     ) -> polardb_20170801_models.ModifyDBEndpointAddressResponse:
+        """
+        @summary Modifies the endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, custom cluster endpoint, and private domain name.
+        
+        @param request: ModifyDBEndpointAddressRequest
+        @return: ModifyDBEndpointAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbendpoint_address_with_options(request, runtime)
 
     async def modify_dbendpoint_address_async(
         self,
         request: polardb_20170801_models.ModifyDBEndpointAddressRequest,
     ) -> polardb_20170801_models.ModifyDBEndpointAddressResponse:
+        """
+        @summary Modifies the endpoints of a PolarDB cluster, including the primary endpoint, default cluster endpoint, custom cluster endpoint, and private domain name.
+        
+        @param request: ModifyDBEndpointAddressRequest
+        @return: ModifyDBEndpointAddressResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbendpoint_address_with_options_async(request, runtime)
 
     def modify_dbnode_class_with_options(
         self,
         request: polardb_20170801_models.ModifyDBNodeClassRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodeClassResponse:
+        """
+        @summary Changes the node specifications of a PolarDB cluster.
+        
+        @param request: ModifyDBNodeClassRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodeClassResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_target_class):
@@ -12924,14 +15419,21 @@
         )
 
     async def modify_dbnode_class_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBNodeClassRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodeClassResponse:
+        """
+        @summary Changes the node specifications of a PolarDB cluster.
+        
+        @param request: ModifyDBNodeClassRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodeClassResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_target_class):
@@ -12973,29 +15475,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbnode_class(
         self,
         request: polardb_20170801_models.ModifyDBNodeClassRequest,
     ) -> polardb_20170801_models.ModifyDBNodeClassResponse:
+        """
+        @summary Changes the node specifications of a PolarDB cluster.
+        
+        @param request: ModifyDBNodeClassRequest
+        @return: ModifyDBNodeClassResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbnode_class_with_options(request, runtime)
 
     async def modify_dbnode_class_async(
         self,
         request: polardb_20170801_models.ModifyDBNodeClassRequest,
     ) -> polardb_20170801_models.ModifyDBNodeClassResponse:
+        """
+        @summary Changes the node specifications of a PolarDB cluster.
+        
+        @param request: ModifyDBNodeClassRequest
+        @return: ModifyDBNodeClassResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbnode_class_with_options_async(request, runtime)
 
     def modify_dbnode_hot_replica_mode_with_options(
         self,
         request: polardb_20170801_models.ModifyDBNodeHotReplicaModeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodeHotReplicaModeResponse:
+        """
+        @summary Enables or disables a cluster node.
+        
+        @param request: ModifyDBNodeHotReplicaModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodeHotReplicaModeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_id):
             query['DBNodeId'] = request.dbnode_id
         if not UtilClient.is_unset(request.hot_replica_mode):
@@ -13028,14 +15549,21 @@
         )
 
     async def modify_dbnode_hot_replica_mode_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBNodeHotReplicaModeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodeHotReplicaModeResponse:
+        """
+        @summary Enables or disables a cluster node.
+        
+        @param request: ModifyDBNodeHotReplicaModeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodeHotReplicaModeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_id):
             query['DBNodeId'] = request.dbnode_id
         if not UtilClient.is_unset(request.hot_replica_mode):
@@ -13067,29 +15595,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbnode_hot_replica_mode(
         self,
         request: polardb_20170801_models.ModifyDBNodeHotReplicaModeRequest,
     ) -> polardb_20170801_models.ModifyDBNodeHotReplicaModeResponse:
+        """
+        @summary Enables or disables a cluster node.
+        
+        @param request: ModifyDBNodeHotReplicaModeRequest
+        @return: ModifyDBNodeHotReplicaModeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbnode_hot_replica_mode_with_options(request, runtime)
 
     async def modify_dbnode_hot_replica_mode_async(
         self,
         request: polardb_20170801_models.ModifyDBNodeHotReplicaModeRequest,
     ) -> polardb_20170801_models.ModifyDBNodeHotReplicaModeResponse:
+        """
+        @summary Enables or disables a cluster node.
+        
+        @param request: ModifyDBNodeHotReplicaModeRequest
+        @return: ModifyDBNodeHotReplicaModeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbnode_hot_replica_mode_with_options_async(request, runtime)
 
     def modify_dbnodes_class_with_options(
         self,
         request: polardb_20170801_models.ModifyDBNodesClassRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodesClassResponse:
+        """
+        @summary Changes the specifications of a node in a PolarDB cluster.
+        
+        @param request: ModifyDBNodesClassRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodesClassResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode):
@@ -13130,14 +15677,21 @@
         )
 
     async def modify_dbnodes_class_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBNodesClassRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodesClassResponse:
+        """
+        @summary Changes the specifications of a node in a PolarDB cluster.
+        
+        @param request: ModifyDBNodesClassRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodesClassResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode):
@@ -13177,29 +15731,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbnodes_class(
         self,
         request: polardb_20170801_models.ModifyDBNodesClassRequest,
     ) -> polardb_20170801_models.ModifyDBNodesClassResponse:
+        """
+        @summary Changes the specifications of a node in a PolarDB cluster.
+        
+        @param request: ModifyDBNodesClassRequest
+        @return: ModifyDBNodesClassResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbnodes_class_with_options(request, runtime)
 
     async def modify_dbnodes_class_async(
         self,
         request: polardb_20170801_models.ModifyDBNodesClassRequest,
     ) -> polardb_20170801_models.ModifyDBNodesClassResponse:
+        """
+        @summary Changes the specifications of a node in a PolarDB cluster.
+        
+        @param request: ModifyDBNodesClassRequest
+        @return: ModifyDBNodesClassResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbnodes_class_with_options_async(request, runtime)
 
     def modify_dbnodes_parameters_with_options(
         self,
         request: polardb_20170801_models.ModifyDBNodesParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodesParametersResponse:
+        """
+        @summary Modifies the parameters of a node and applies them to specified nodes.
+        
+        @param request: ModifyDBNodesParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodesParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_ids):
             query['DBNodeIds'] = request.dbnode_ids
         if not UtilClient.is_unset(request.from_time_service):
@@ -13240,14 +15813,21 @@
         )
 
     async def modify_dbnodes_parameters_with_options_async(
         self,
         request: polardb_20170801_models.ModifyDBNodesParametersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyDBNodesParametersResponse:
+        """
+        @summary Modifies the parameters of a node and applies them to specified nodes.
+        
+        @param request: ModifyDBNodesParametersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBNodesParametersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode_ids):
             query['DBNodeIds'] = request.dbnode_ids
         if not UtilClient.is_unset(request.from_time_service):
@@ -13287,29 +15867,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbnodes_parameters(
         self,
         request: polardb_20170801_models.ModifyDBNodesParametersRequest,
     ) -> polardb_20170801_models.ModifyDBNodesParametersResponse:
+        """
+        @summary Modifies the parameters of a node and applies them to specified nodes.
+        
+        @param request: ModifyDBNodesParametersRequest
+        @return: ModifyDBNodesParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbnodes_parameters_with_options(request, runtime)
 
     async def modify_dbnodes_parameters_async(
         self,
         request: polardb_20170801_models.ModifyDBNodesParametersRequest,
     ) -> polardb_20170801_models.ModifyDBNodesParametersResponse:
+        """
+        @summary Modifies the parameters of a node and applies them to specified nodes.
+        
+        @param request: ModifyDBNodesParametersRequest
+        @return: ModifyDBNodesParametersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbnodes_parameters_with_options_async(request, runtime)
 
     def modify_global_database_network_with_options(
         self,
         request: polardb_20170801_models.ModifyGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalDatabaseNetworkResponse:
+        """
+        @summary Modifies a Global Database Network (GDN).
+        
+        @param request: ModifyGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gdndescription):
             query['GDNDescription'] = request.gdndescription
         if not UtilClient.is_unset(request.gdnid):
             query['GDNId'] = request.gdnid
         if not UtilClient.is_unset(request.owner_account):
@@ -13344,14 +15943,21 @@
         )
 
     async def modify_global_database_network_with_options_async(
         self,
         request: polardb_20170801_models.ModifyGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalDatabaseNetworkResponse:
+        """
+        @summary Modifies a Global Database Network (GDN).
+        
+        @param request: ModifyGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gdndescription):
             query['GDNDescription'] = request.gdndescription
         if not UtilClient.is_unset(request.gdnid):
             query['GDNId'] = request.gdnid
         if not UtilClient.is_unset(request.owner_account):
@@ -13385,29 +15991,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_global_database_network(
         self,
         request: polardb_20170801_models.ModifyGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.ModifyGlobalDatabaseNetworkResponse:
+        """
+        @summary Modifies a Global Database Network (GDN).
+        
+        @param request: ModifyGlobalDatabaseNetworkRequest
+        @return: ModifyGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_global_database_network_with_options(request, runtime)
 
     async def modify_global_database_network_async(
         self,
         request: polardb_20170801_models.ModifyGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.ModifyGlobalDatabaseNetworkResponse:
+        """
+        @summary Modifies a Global Database Network (GDN).
+        
+        @param request: ModifyGlobalDatabaseNetworkRequest
+        @return: ModifyGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_global_database_network_with_options_async(request, runtime)
 
     def modify_global_security_ipgroup_with_options(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupResponse:
+        """
+        @summary Modifies an IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gip_list):
             query['GIpList'] = request.gip_list
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.global_security_group_id):
@@ -13446,14 +16071,21 @@
         )
 
     async def modify_global_security_ipgroup_with_options_async(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupResponse:
+        """
+        @summary Modifies an IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalSecurityIPGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.gip_list):
             query['GIpList'] = request.gip_list
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.global_security_group_id):
@@ -13491,29 +16123,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_global_security_ipgroup(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupResponse:
+        """
+        @summary Modifies an IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRequest
+        @return: ModifyGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_global_security_ipgroup_with_options(request, runtime)
 
     async def modify_global_security_ipgroup_async(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRequest,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupResponse:
+        """
+        @summary Modifies an IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRequest
+        @return: ModifyGlobalSecurityIPGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_global_security_ipgroup_with_options_async(request, runtime)
 
     def modify_global_security_ipgroup_name_with_options(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupNameResponse:
+        """
+        @summary Modifies the name of a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalSecurityIPGroupNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -13550,14 +16201,21 @@
         )
 
     async def modify_global_security_ipgroup_name_with_options_async(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupNameResponse:
+        """
+        @summary Modifies the name of a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalSecurityIPGroupNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.global_ig_name):
             query['GlobalIgName'] = request.global_ig_name
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -13593,29 +16251,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_global_security_ipgroup_name(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupNameRequest,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupNameResponse:
+        """
+        @summary Modifies the name of a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupNameRequest
+        @return: ModifyGlobalSecurityIPGroupNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_global_security_ipgroup_name_with_options(request, runtime)
 
     async def modify_global_security_ipgroup_name_async(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupNameRequest,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupNameResponse:
+        """
+        @summary Modifies the name of a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupNameRequest
+        @return: ModifyGlobalSecurityIPGroupNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_global_security_ipgroup_name_with_options_async(request, runtime)
 
     def modify_global_security_ipgroup_relation_with_options(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Modifies the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRelationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalSecurityIPGroupRelationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -13652,14 +16329,21 @@
         )
 
     async def modify_global_security_ipgroup_relation_with_options_async(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Modifies the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRelationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyGlobalSecurityIPGroupRelationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.global_security_group_id):
             query['GlobalSecurityGroupId'] = request.global_security_group_id
         if not UtilClient.is_unset(request.owner_account):
@@ -13695,29 +16379,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_global_security_ipgroup_relation(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationRequest,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Modifies the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRelationRequest
+        @return: ModifyGlobalSecurityIPGroupRelationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_global_security_ipgroup_relation_with_options(request, runtime)
 
     async def modify_global_security_ipgroup_relation_async(
         self,
         request: polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationRequest,
     ) -> polardb_20170801_models.ModifyGlobalSecurityIPGroupRelationResponse:
+        """
+        @summary Modifies the relationship between a cluster and a global IP whitelist template.
+        
+        @param request: ModifyGlobalSecurityIPGroupRelationRequest
+        @return: ModifyGlobalSecurityIPGroupRelationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_global_security_ipgroup_relation_with_options_async(request, runtime)
 
     def modify_log_backup_policy_with_options(
         self,
         request: polardb_20170801_models.ModifyLogBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyLogBackupPolicyResponse:
+        """
+        @summary Modifies the retention policy of the log backups in a PolarDB cluster.
+        
+        @param request: ModifyLogBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyLogBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.log_backup_another_region_region):
             query['LogBackupAnotherRegionRegion'] = request.log_backup_another_region_region
         if not UtilClient.is_unset(request.log_backup_another_region_retention_period):
@@ -13752,14 +16455,21 @@
         )
 
     async def modify_log_backup_policy_with_options_async(
         self,
         request: polardb_20170801_models.ModifyLogBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyLogBackupPolicyResponse:
+        """
+        @summary Modifies the retention policy of the log backups in a PolarDB cluster.
+        
+        @param request: ModifyLogBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyLogBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.log_backup_another_region_region):
             query['LogBackupAnotherRegionRegion'] = request.log_backup_another_region_region
         if not UtilClient.is_unset(request.log_backup_another_region_retention_period):
@@ -13793,29 +16503,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_log_backup_policy(
         self,
         request: polardb_20170801_models.ModifyLogBackupPolicyRequest,
     ) -> polardb_20170801_models.ModifyLogBackupPolicyResponse:
+        """
+        @summary Modifies the retention policy of the log backups in a PolarDB cluster.
+        
+        @param request: ModifyLogBackupPolicyRequest
+        @return: ModifyLogBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_log_backup_policy_with_options(request, runtime)
 
     async def modify_log_backup_policy_async(
         self,
         request: polardb_20170801_models.ModifyLogBackupPolicyRequest,
     ) -> polardb_20170801_models.ModifyLogBackupPolicyResponse:
+        """
+        @summary Modifies the retention policy of the log backups in a PolarDB cluster.
+        
+        @param request: ModifyLogBackupPolicyRequest
+        @return: ModifyLogBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_log_backup_policy_with_options_async(request, runtime)
 
     def modify_masking_rules_with_options(
         self,
         request: polardb_20170801_models.ModifyMaskingRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyMaskingRulesResponse:
+        """
+        @summary Modifies or adds a data masking rule.
+        
+        @param request: ModifyMaskingRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyMaskingRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.rule_config):
@@ -13846,14 +16575,21 @@
         )
 
     async def modify_masking_rules_with_options_async(
         self,
         request: polardb_20170801_models.ModifyMaskingRulesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyMaskingRulesResponse:
+        """
+        @summary Modifies or adds a data masking rule.
+        
+        @param request: ModifyMaskingRulesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyMaskingRulesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.enable):
             query['Enable'] = request.enable
         if not UtilClient.is_unset(request.rule_config):
@@ -13883,29 +16619,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_masking_rules(
         self,
         request: polardb_20170801_models.ModifyMaskingRulesRequest,
     ) -> polardb_20170801_models.ModifyMaskingRulesResponse:
+        """
+        @summary Modifies or adds a data masking rule.
+        
+        @param request: ModifyMaskingRulesRequest
+        @return: ModifyMaskingRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_masking_rules_with_options(request, runtime)
 
     async def modify_masking_rules_async(
         self,
         request: polardb_20170801_models.ModifyMaskingRulesRequest,
     ) -> polardb_20170801_models.ModifyMaskingRulesResponse:
+        """
+        @summary Modifies or adds a data masking rule.
+        
+        @param request: ModifyMaskingRulesRequest
+        @return: ModifyMaskingRulesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_masking_rules_with_options_async(request, runtime)
 
     def modify_pending_maintenance_action_with_options(
         self,
         request: polardb_20170801_models.ModifyPendingMaintenanceActionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyPendingMaintenanceActionResponse:
+        """
+        @summary Modifies the switching time of a pending event.
+        
+        @param request: ModifyPendingMaintenanceActionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPendingMaintenanceActionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ids):
             query['Ids'] = request.ids
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -13942,14 +16697,21 @@
         )
 
     async def modify_pending_maintenance_action_with_options_async(
         self,
         request: polardb_20170801_models.ModifyPendingMaintenanceActionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ModifyPendingMaintenanceActionResponse:
+        """
+        @summary Modifies the switching time of a pending event.
+        
+        @param request: ModifyPendingMaintenanceActionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyPendingMaintenanceActionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.ids):
             query['Ids'] = request.ids
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -13985,29 +16747,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_pending_maintenance_action(
         self,
         request: polardb_20170801_models.ModifyPendingMaintenanceActionRequest,
     ) -> polardb_20170801_models.ModifyPendingMaintenanceActionResponse:
+        """
+        @summary Modifies the switching time of a pending event.
+        
+        @param request: ModifyPendingMaintenanceActionRequest
+        @return: ModifyPendingMaintenanceActionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_pending_maintenance_action_with_options(request, runtime)
 
     async def modify_pending_maintenance_action_async(
         self,
         request: polardb_20170801_models.ModifyPendingMaintenanceActionRequest,
     ) -> polardb_20170801_models.ModifyPendingMaintenanceActionResponse:
+        """
+        @summary Modifies the switching time of a pending event.
+        
+        @param request: ModifyPendingMaintenanceActionRequest
+        @return: ModifyPendingMaintenanceActionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_pending_maintenance_action_with_options_async(request, runtime)
 
     def open_aitask_with_options(
         self,
         request: polardb_20170801_models.OpenAITaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.OpenAITaskResponse:
+        """
+        @summary Enables the PolarDB for AI feature for a cluster.
+        
+        @param request: OpenAITaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenAITaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.node_type):
             query['NodeType'] = request.node_type
         if not UtilClient.is_unset(request.owner_account):
@@ -14046,14 +16827,21 @@
         )
 
     async def open_aitask_with_options_async(
         self,
         request: polardb_20170801_models.OpenAITaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.OpenAITaskResponse:
+        """
+        @summary Enables the PolarDB for AI feature for a cluster.
+        
+        @param request: OpenAITaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenAITaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.node_type):
             query['NodeType'] = request.node_type
         if not UtilClient.is_unset(request.owner_account):
@@ -14091,29 +16879,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_aitask(
         self,
         request: polardb_20170801_models.OpenAITaskRequest,
     ) -> polardb_20170801_models.OpenAITaskResponse:
+        """
+        @summary Enables the PolarDB for AI feature for a cluster.
+        
+        @param request: OpenAITaskRequest
+        @return: OpenAITaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_aitask_with_options(request, runtime)
 
     async def open_aitask_async(
         self,
         request: polardb_20170801_models.OpenAITaskRequest,
     ) -> polardb_20170801_models.OpenAITaskResponse:
+        """
+        @summary Enables the PolarDB for AI feature for a cluster.
+        
+        @param request: OpenAITaskRequest
+        @return: OpenAITaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_aitask_with_options_async(request, runtime)
 
     def refresh_dbcluster_storage_usage_with_options(
         self,
         request: polardb_20170801_models.RefreshDBClusterStorageUsageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RefreshDBClusterStorageUsageResponse:
+        """
+        @summary Updates the storage usage of a cluster.
+        
+        @param request: RefreshDBClusterStorageUsageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RefreshDBClusterStorageUsageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -14142,14 +16949,21 @@
         )
 
     async def refresh_dbcluster_storage_usage_with_options_async(
         self,
         request: polardb_20170801_models.RefreshDBClusterStorageUsageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RefreshDBClusterStorageUsageResponse:
+        """
+        @summary Updates the storage usage of a cluster.
+        
+        @param request: RefreshDBClusterStorageUsageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RefreshDBClusterStorageUsageResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.resource_owner_account):
@@ -14177,31 +16991,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def refresh_dbcluster_storage_usage(
         self,
         request: polardb_20170801_models.RefreshDBClusterStorageUsageRequest,
     ) -> polardb_20170801_models.RefreshDBClusterStorageUsageResponse:
+        """
+        @summary Updates the storage usage of a cluster.
+        
+        @param request: RefreshDBClusterStorageUsageRequest
+        @return: RefreshDBClusterStorageUsageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.refresh_dbcluster_storage_usage_with_options(request, runtime)
 
     async def refresh_dbcluster_storage_usage_async(
         self,
         request: polardb_20170801_models.RefreshDBClusterStorageUsageRequest,
     ) -> polardb_20170801_models.RefreshDBClusterStorageUsageResponse:
+        """
+        @summary Updates the storage usage of a cluster.
+        
+        @param request: RefreshDBClusterStorageUsageRequest
+        @return: RefreshDBClusterStorageUsageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.refresh_dbcluster_storage_usage_with_options_async(request, runtime)
 
     def remove_dbcluster_from_gdnwith_options(
         self,
         request: polardb_20170801_models.RemoveDBClusterFromGDNRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RemoveDBClusterFromGDNResponse:
         """
-        >  You cannot remove the primary cluster from a GDN.
+        @summary Removes a secondary cluster from a GDN.
+        
+        @description >  You cannot remove the primary cluster from a GDN.
         
         @param request: RemoveDBClusterFromGDNRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemoveDBClusterFromGDNResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14240,15 +17068,17 @@
 
     async def remove_dbcluster_from_gdnwith_options_async(
         self,
         request: polardb_20170801_models.RemoveDBClusterFromGDNRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RemoveDBClusterFromGDNResponse:
         """
-        >  You cannot remove the primary cluster from a GDN.
+        @summary Removes a secondary cluster from a GDN.
+        
+        @description >  You cannot remove the primary cluster from a GDN.
         
         @param request: RemoveDBClusterFromGDNRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: RemoveDBClusterFromGDNResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -14286,42 +17116,48 @@
         )
 
     def remove_dbcluster_from_gdn(
         self,
         request: polardb_20170801_models.RemoveDBClusterFromGDNRequest,
     ) -> polardb_20170801_models.RemoveDBClusterFromGDNResponse:
         """
-        >  You cannot remove the primary cluster from a GDN.
+        @summary Removes a secondary cluster from a GDN.
+        
+        @description >  You cannot remove the primary cluster from a GDN.
         
         @param request: RemoveDBClusterFromGDNRequest
         @return: RemoveDBClusterFromGDNResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.remove_dbcluster_from_gdnwith_options(request, runtime)
 
     async def remove_dbcluster_from_gdn_async(
         self,
         request: polardb_20170801_models.RemoveDBClusterFromGDNRequest,
     ) -> polardb_20170801_models.RemoveDBClusterFromGDNResponse:
         """
-        >  You cannot remove the primary cluster from a GDN.
+        @summary Removes a secondary cluster from a GDN.
+        
+        @description >  You cannot remove the primary cluster from a GDN.
         
         @param request: RemoveDBClusterFromGDNRequest
         @return: RemoveDBClusterFromGDNResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.remove_dbcluster_from_gdnwith_options_async(request, runtime)
 
     def reset_account_with_options(
         self,
         request: polardb_20170801_models.ResetAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ResetAccountResponse:
         """
-        >- Only PolarDB for MySQL clusters support this operation.
+        @summary Resets the permissions of a privileged account for a PolarDB cluster.
+        
+        @description >- Only PolarDB for MySQL clusters support this operation.
         >- If the privileged account of your cluster encounters exceptions, you can call this operation to reset the permissions. For example, the permissions are accidentally revoked.
         
         @param request: ResetAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetAccountResponse
         """
         UtilClient.validate_model(request)
@@ -14361,15 +17197,17 @@
 
     async def reset_account_with_options_async(
         self,
         request: polardb_20170801_models.ResetAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ResetAccountResponse:
         """
-        >- Only PolarDB for MySQL clusters support this operation.
+        @summary Resets the permissions of a privileged account for a PolarDB cluster.
+        
+        @description >- Only PolarDB for MySQL clusters support this operation.
         >- If the privileged account of your cluster encounters exceptions, you can call this operation to reset the permissions. For example, the permissions are accidentally revoked.
         
         @param request: ResetAccountRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetAccountResponse
         """
         UtilClient.validate_model(request)
@@ -14408,42 +17246,53 @@
         )
 
     def reset_account(
         self,
         request: polardb_20170801_models.ResetAccountRequest,
     ) -> polardb_20170801_models.ResetAccountResponse:
         """
-        >- Only PolarDB for MySQL clusters support this operation.
+        @summary Resets the permissions of a privileged account for a PolarDB cluster.
+        
+        @description >- Only PolarDB for MySQL clusters support this operation.
         >- If the privileged account of your cluster encounters exceptions, you can call this operation to reset the permissions. For example, the permissions are accidentally revoked.
         
         @param request: ResetAccountRequest
         @return: ResetAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.reset_account_with_options(request, runtime)
 
     async def reset_account_async(
         self,
         request: polardb_20170801_models.ResetAccountRequest,
     ) -> polardb_20170801_models.ResetAccountResponse:
         """
-        >- Only PolarDB for MySQL clusters support this operation.
+        @summary Resets the permissions of a privileged account for a PolarDB cluster.
+        
+        @description >- Only PolarDB for MySQL clusters support this operation.
         >- If the privileged account of your cluster encounters exceptions, you can call this operation to reset the permissions. For example, the permissions are accidentally revoked.
         
         @param request: ResetAccountRequest
         @return: ResetAccountResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.reset_account_with_options_async(request, runtime)
 
     def reset_global_database_network_with_options(
         self,
         request: polardb_20170801_models.ResetGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ResetGlobalDatabaseNetworkResponse:
+        """
+        @summary Rebuilds a secondary cluster in a Global Database Network (GDN).
+        
+        @param request: ResetGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.gdnid):
             query['GDNId'] = request.gdnid
         if not UtilClient.is_unset(request.owner_account):
@@ -14478,14 +17327,21 @@
         )
 
     async def reset_global_database_network_with_options_async(
         self,
         request: polardb_20170801_models.ResetGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.ResetGlobalDatabaseNetworkResponse:
+        """
+        @summary Rebuilds a secondary cluster in a Global Database Network (GDN).
+        
+        @param request: ResetGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ResetGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.gdnid):
             query['GDNId'] = request.gdnid
         if not UtilClient.is_unset(request.owner_account):
@@ -14519,29 +17375,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reset_global_database_network(
         self,
         request: polardb_20170801_models.ResetGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.ResetGlobalDatabaseNetworkResponse:
+        """
+        @summary Rebuilds a secondary cluster in a Global Database Network (GDN).
+        
+        @param request: ResetGlobalDatabaseNetworkRequest
+        @return: ResetGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reset_global_database_network_with_options(request, runtime)
 
     async def reset_global_database_network_async(
         self,
         request: polardb_20170801_models.ResetGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.ResetGlobalDatabaseNetworkResponse:
+        """
+        @summary Rebuilds a secondary cluster in a Global Database Network (GDN).
+        
+        @param request: ResetGlobalDatabaseNetworkRequest
+        @return: ResetGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.reset_global_database_network_with_options_async(request, runtime)
 
     def restart_dblink_with_options(
         self,
         request: polardb_20170801_models.RestartDBLinkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RestartDBLinkResponse:
+        """
+        @summary 重启代理
+        
+        @param request: RestartDBLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RestartDBLinkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -14572,14 +17447,21 @@
         )
 
     async def restart_dblink_with_options_async(
         self,
         request: polardb_20170801_models.RestartDBLinkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RestartDBLinkResponse:
+        """
+        @summary 重启代理
+        
+        @param request: RestartDBLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RestartDBLinkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -14609,29 +17491,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def restart_dblink(
         self,
         request: polardb_20170801_models.RestartDBLinkRequest,
     ) -> polardb_20170801_models.RestartDBLinkResponse:
+        """
+        @summary 重启代理
+        
+        @param request: RestartDBLinkRequest
+        @return: RestartDBLinkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.restart_dblink_with_options(request, runtime)
 
     async def restart_dblink_async(
         self,
         request: polardb_20170801_models.RestartDBLinkRequest,
     ) -> polardb_20170801_models.RestartDBLinkResponse:
+        """
+        @summary 重启代理
+        
+        @param request: RestartDBLinkRequest
+        @return: RestartDBLinkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.restart_dblink_with_options_async(request, runtime)
 
     def restart_dbnode_with_options(
         self,
         request: polardb_20170801_models.RestartDBNodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RestartDBNodeResponse:
+        """
+        @summary Restarts a node in a PolarDB cluster.
+        
+        @param request: RestartDBNodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RestartDBNodeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbnode_id):
             query['DBNodeId'] = request.dbnode_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -14660,14 +17561,21 @@
         )
 
     async def restart_dbnode_with_options_async(
         self,
         request: polardb_20170801_models.RestartDBNodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RestartDBNodeResponse:
+        """
+        @summary Restarts a node in a PolarDB cluster.
+        
+        @param request: RestartDBNodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RestartDBNodeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbnode_id):
             query['DBNodeId'] = request.dbnode_id
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -14695,29 +17603,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def restart_dbnode(
         self,
         request: polardb_20170801_models.RestartDBNodeRequest,
     ) -> polardb_20170801_models.RestartDBNodeResponse:
+        """
+        @summary Restarts a node in a PolarDB cluster.
+        
+        @param request: RestartDBNodeRequest
+        @return: RestartDBNodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.restart_dbnode_with_options(request, runtime)
 
     async def restart_dbnode_async(
         self,
         request: polardb_20170801_models.RestartDBNodeRequest,
     ) -> polardb_20170801_models.RestartDBNodeResponse:
+        """
+        @summary Restarts a node in a PolarDB cluster.
+        
+        @param request: RestartDBNodeRequest
+        @return: RestartDBNodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.restart_dbnode_with_options_async(request, runtime)
 
     def restore_table_with_options(
         self,
         request: polardb_20170801_models.RestoreTableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RestoreTableResponse:
+        """
+        @summary Restores PolarDB databases and tables.
+        
+        @param request: RestoreTableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RestoreTableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -14754,14 +17681,21 @@
         )
 
     async def restore_table_with_options_async(
         self,
         request: polardb_20170801_models.RestoreTableRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RestoreTableResponse:
+        """
+        @summary Restores PolarDB databases and tables.
+        
+        @param request: RestoreTableRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RestoreTableResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.owner_account):
@@ -14797,29 +17731,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def restore_table(
         self,
         request: polardb_20170801_models.RestoreTableRequest,
     ) -> polardb_20170801_models.RestoreTableResponse:
+        """
+        @summary Restores PolarDB databases and tables.
+        
+        @param request: RestoreTableRequest
+        @return: RestoreTableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.restore_table_with_options(request, runtime)
 
     async def restore_table_async(
         self,
         request: polardb_20170801_models.RestoreTableRequest,
     ) -> polardb_20170801_models.RestoreTableResponse:
+        """
+        @summary Restores PolarDB databases and tables.
+        
+        @param request: RestoreTableRequest
+        @return: RestoreTableResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.restore_table_with_options_async(request, runtime)
 
     def revoke_account_privilege_with_options(
         self,
         request: polardb_20170801_models.RevokeAccountPrivilegeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RevokeAccountPrivilegeResponse:
+        """
+        @summary Revokes the access permissions on one or more databases from a specified PolarDB standard account.
+        
+        @param request: RevokeAccountPrivilegeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokeAccountPrivilegeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbname):
@@ -14852,14 +17805,21 @@
         )
 
     async def revoke_account_privilege_with_options_async(
         self,
         request: polardb_20170801_models.RevokeAccountPrivilegeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.RevokeAccountPrivilegeResponse:
+        """
+        @summary Revokes the access permissions on one or more databases from a specified PolarDB standard account.
+        
+        @param request: RevokeAccountPrivilegeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokeAccountPrivilegeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_name):
             query['AccountName'] = request.account_name
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbname):
@@ -14891,29 +17851,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def revoke_account_privilege(
         self,
         request: polardb_20170801_models.RevokeAccountPrivilegeRequest,
     ) -> polardb_20170801_models.RevokeAccountPrivilegeResponse:
+        """
+        @summary Revokes the access permissions on one or more databases from a specified PolarDB standard account.
+        
+        @param request: RevokeAccountPrivilegeRequest
+        @return: RevokeAccountPrivilegeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.revoke_account_privilege_with_options(request, runtime)
 
     async def revoke_account_privilege_async(
         self,
         request: polardb_20170801_models.RevokeAccountPrivilegeRequest,
     ) -> polardb_20170801_models.RevokeAccountPrivilegeResponse:
+        """
+        @summary Revokes the access permissions on one or more databases from a specified PolarDB standard account.
+        
+        @param request: RevokeAccountPrivilegeRequest
+        @return: RevokeAccountPrivilegeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.revoke_account_privilege_with_options_async(request, runtime)
 
     def switch_over_global_database_network_with_options(
         self,
         request: polardb_20170801_models.SwitchOverGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.SwitchOverGlobalDatabaseNetworkResponse:
+        """
+        @param request: SwitchOverGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchOverGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.forced):
             query['Forced'] = request.forced
         if not UtilClient.is_unset(request.gdnid):
@@ -14952,14 +17929,19 @@
         )
 
     async def switch_over_global_database_network_with_options_async(
         self,
         request: polardb_20170801_models.SwitchOverGlobalDatabaseNetworkRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.SwitchOverGlobalDatabaseNetworkResponse:
+        """
+        @param request: SwitchOverGlobalDatabaseNetworkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchOverGlobalDatabaseNetworkResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.forced):
             query['Forced'] = request.forced
         if not UtilClient.is_unset(request.gdnid):
@@ -14997,29 +17979,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def switch_over_global_database_network(
         self,
         request: polardb_20170801_models.SwitchOverGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.SwitchOverGlobalDatabaseNetworkResponse:
+        """
+        @param request: SwitchOverGlobalDatabaseNetworkRequest
+        @return: SwitchOverGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.switch_over_global_database_network_with_options(request, runtime)
 
     async def switch_over_global_database_network_async(
         self,
         request: polardb_20170801_models.SwitchOverGlobalDatabaseNetworkRequest,
     ) -> polardb_20170801_models.SwitchOverGlobalDatabaseNetworkResponse:
+        """
+        @param request: SwitchOverGlobalDatabaseNetworkRequest
+        @return: SwitchOverGlobalDatabaseNetworkResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.switch_over_global_database_network_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: polardb_20170801_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.TagResourcesResponse:
+        """
+        @param request: TagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -15054,14 +18049,19 @@
         )
 
     async def tag_resources_with_options_async(
         self,
         request: polardb_20170801_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.TagResourcesResponse:
+        """
+        @param request: TagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -15095,29 +18095,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def tag_resources(
         self,
         request: polardb_20170801_models.TagResourcesRequest,
     ) -> polardb_20170801_models.TagResourcesResponse:
+        """
+        @param request: TagResourcesRequest
+        @return: TagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     async def tag_resources_async(
         self,
         request: polardb_20170801_models.TagResourcesRequest,
     ) -> polardb_20170801_models.TagResourcesResponse:
+        """
+        @param request: TagResourcesRequest
+        @return: TagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.tag_resources_with_options_async(request, runtime)
 
     def temp_modify_dbnode_with_options(
         self,
         request: polardb_20170801_models.TempModifyDBNodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.TempModifyDBNodeResponse:
+        """
+        @summary Temporarily upgrades the configuration of a PolarDB cluster or adds one or more nodes to a cluster.
+        
+        @param request: TempModifyDBNodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TempModifyDBNodeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode):
@@ -15156,14 +18171,21 @@
         )
 
     async def temp_modify_dbnode_with_options_async(
         self,
         request: polardb_20170801_models.TempModifyDBNodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.TempModifyDBNodeResponse:
+        """
+        @summary Temporarily upgrades the configuration of a PolarDB cluster or adds one or more nodes to a cluster.
+        
+        @param request: TempModifyDBNodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TempModifyDBNodeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.dbcluster_id):
             query['DBClusterId'] = request.dbcluster_id
         if not UtilClient.is_unset(request.dbnode):
@@ -15201,33 +18223,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def temp_modify_dbnode(
         self,
         request: polardb_20170801_models.TempModifyDBNodeRequest,
     ) -> polardb_20170801_models.TempModifyDBNodeResponse:
+        """
+        @summary Temporarily upgrades the configuration of a PolarDB cluster or adds one or more nodes to a cluster.
+        
+        @param request: TempModifyDBNodeRequest
+        @return: TempModifyDBNodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.temp_modify_dbnode_with_options(request, runtime)
 
     async def temp_modify_dbnode_async(
         self,
         request: polardb_20170801_models.TempModifyDBNodeRequest,
     ) -> polardb_20170801_models.TempModifyDBNodeResponse:
+        """
+        @summary Temporarily upgrades the configuration of a PolarDB cluster or adds one or more nodes to a cluster.
+        
+        @param request: TempModifyDBNodeRequest
+        @return: TempModifyDBNodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.temp_modify_dbnode_with_options_async(request, runtime)
 
     def transform_dbcluster_pay_type_with_options(
         self,
         request: polardb_20170801_models.TransformDBClusterPayTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.TransformDBClusterPayTypeResponse:
         """
-        >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](~~172886~~) and [Change the billing method from pay-as-you-go to subscription](~~84076~~).
-        >*   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
-        >*   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
+        @summary Changes the billing method of a PolarDB cluster.
+        
+        @description >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](https://help.aliyun.com/document_detail/172886.html) and [Change the billing method from pay-as-you-go to subscription](https://help.aliyun.com/document_detail/84076.html).
+        >   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
+        >   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
         
         @param request: TransformDBClusterPayTypeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TransformDBClusterPayTypeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15274,17 +18310,19 @@
 
     async def transform_dbcluster_pay_type_with_options_async(
         self,
         request: polardb_20170801_models.TransformDBClusterPayTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.TransformDBClusterPayTypeResponse:
         """
-        >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](~~172886~~) and [Change the billing method from pay-as-you-go to subscription](~~84076~~).
-        >*   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
-        >*   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
+        @summary Changes the billing method of a PolarDB cluster.
+        
+        @description >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](https://help.aliyun.com/document_detail/172886.html) and [Change the billing method from pay-as-you-go to subscription](https://help.aliyun.com/document_detail/84076.html).
+        >   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
+        >   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
         
         @param request: TransformDBClusterPayTypeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TransformDBClusterPayTypeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15330,44 +18368,55 @@
         )
 
     def transform_dbcluster_pay_type(
         self,
         request: polardb_20170801_models.TransformDBClusterPayTypeRequest,
     ) -> polardb_20170801_models.TransformDBClusterPayTypeResponse:
         """
-        >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](~~172886~~) and [Change the billing method from pay-as-you-go to subscription](~~84076~~).
-        >*   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
-        >*   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
+        @summary Changes the billing method of a PolarDB cluster.
+        
+        @description >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](https://help.aliyun.com/document_detail/172886.html) and [Change the billing method from pay-as-you-go to subscription](https://help.aliyun.com/document_detail/84076.html).
+        >   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
+        >   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
         
         @param request: TransformDBClusterPayTypeRequest
         @return: TransformDBClusterPayTypeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.transform_dbcluster_pay_type_with_options(request, runtime)
 
     async def transform_dbcluster_pay_type_async(
         self,
         request: polardb_20170801_models.TransformDBClusterPayTypeRequest,
     ) -> polardb_20170801_models.TransformDBClusterPayTypeResponse:
         """
-        >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](~~172886~~) and [Change the billing method from pay-as-you-go to subscription](~~84076~~).
-        >*   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
-        >*   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
+        @summary Changes the billing method of a PolarDB cluster.
+        
+        @description >    PolarDB clusters support the subscription and pay-as-you-go billing methods. You can change the billing method from subscription to pay-as-you-go or from pay-as-you-go to subscription based on your business requirements. For more information, see [Change the billing method from subscription to pay-as-you-go](https://help.aliyun.com/document_detail/172886.html) and [Change the billing method from pay-as-you-go to subscription](https://help.aliyun.com/document_detail/84076.html).
+        >   You cannot change the billing method from pay-as-you-go to subscription if your account balance is insufficient.
+        >   If you change the billing method from subscription to pay-as-you-go, the system automatically refunds the balance of the prepaid subscription fees.
         
         @param request: TransformDBClusterPayTypeRequest
         @return: TransformDBClusterPayTypeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.transform_dbcluster_pay_type_with_options_async(request, runtime)
 
     def untag_resources_with_options(
         self,
         request: polardb_20170801_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.UntagResourcesResponse:
+        """
+        @summary Unbinds tags from PolarDB clusters.
+        
+        @param request: UntagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UntagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -15404,14 +18453,21 @@
         )
 
     async def untag_resources_with_options_async(
         self,
         request: polardb_20170801_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.UntagResourcesResponse:
+        """
+        @summary Unbinds tags from PolarDB clusters.
+        
+        @param request: UntagResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UntagResourcesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.all):
             query['All'] = request.all
         if not UtilClient.is_unset(request.owner_account):
             query['OwnerAccount'] = request.owner_account
         if not UtilClient.is_unset(request.owner_id):
@@ -15447,32 +18503,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def untag_resources(
         self,
         request: polardb_20170801_models.UntagResourcesRequest,
     ) -> polardb_20170801_models.UntagResourcesResponse:
+        """
+        @summary Unbinds tags from PolarDB clusters.
+        
+        @param request: UntagResourcesRequest
+        @return: UntagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     async def untag_resources_async(
         self,
         request: polardb_20170801_models.UntagResourcesRequest,
     ) -> polardb_20170801_models.UntagResourcesResponse:
+        """
+        @summary Unbinds tags from PolarDB clusters.
+        
+        @param request: UntagResourcesRequest
+        @return: UntagResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
 
     def upgrade_dbcluster_version_with_options(
         self,
         request: polardb_20170801_models.UpgradeDBClusterVersionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.UpgradeDBClusterVersionResponse:
         """
-        >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
-        >*   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
+        @summary Upgrades the kernel version of a PolarDB for MySQL cluster.
+        
+        @description >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
+        >   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
         
         @param request: UpgradeDBClusterVersionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradeDBClusterVersionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15521,16 +18591,18 @@
 
     async def upgrade_dbcluster_version_with_options_async(
         self,
         request: polardb_20170801_models.UpgradeDBClusterVersionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> polardb_20170801_models.UpgradeDBClusterVersionResponse:
         """
-        >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
-        >*   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
+        @summary Upgrades the kernel version of a PolarDB for MySQL cluster.
+        
+        @description >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
+        >   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
         
         @param request: UpgradeDBClusterVersionRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradeDBClusterVersionResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -15578,29 +18650,33 @@
         )
 
     def upgrade_dbcluster_version(
         self,
         request: polardb_20170801_models.UpgradeDBClusterVersionRequest,
     ) -> polardb_20170801_models.UpgradeDBClusterVersionResponse:
         """
-        >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
-        >*   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
+        @summary Upgrades the kernel version of a PolarDB for MySQL cluster.
+        
+        @description >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
+        >   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
         
         @param request: UpgradeDBClusterVersionRequest
         @return: UpgradeDBClusterVersionResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.upgrade_dbcluster_version_with_options(request, runtime)
 
     async def upgrade_dbcluster_version_async(
         self,
         request: polardb_20170801_models.UpgradeDBClusterVersionRequest,
     ) -> polardb_20170801_models.UpgradeDBClusterVersionResponse:
         """
-        >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
-        >*   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
+        @summary Upgrades the kernel version of a PolarDB for MySQL cluster.
+        
+        @description >   You can update only the revision version of a PolarDB for MySQL cluster, for example, from 8.0.1.1.3 to 8.0.1.1.4.
+        >   You can use only your Alibaba Cloud account to create scheduled tasks that update the kernel version of a PolarDB for MySQL cluster. RAM users are not authorized to update the kernel version of a PolarDB for MySQL cluster.
         
         @param request: UpgradeDBClusterVersionRequest
         @return: UpgradeDBClusterVersionResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.upgrade_dbcluster_version_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801/models.py` & `alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,30 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         task_id: str = None,
     ):
         # The cluster ID.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to query the information of all clusters that are deployed in a specified region, such as the cluster IDs.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the information of all clusters that are deployed in a specified region, such as the cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The ID of the scheduled task that you want to cancel.
         # 
-        # > *   You can call the [DescribeScheduleTasks](~~199648~~) operation to query the details of all scheduled tasks that belong to the current account, such as the task IDs.
+        # > *   You can call the [DescribeScheduleTasks](https://help.aliyun.com/document_detail/199648.html) operation to query the details of all scheduled tasks that belong to the current account, such as the task IDs.
         # >*   You can cancel only the tasks whose status is `pending`.``
+        # 
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -158,18 +162,22 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The name of the account.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -289,17 +297,21 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a region, such as the cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a region, such as the cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database.
+        # 
+        # This parameter is required.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -427,21 +439,23 @@
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         tderegion: str = None,
     ):
         # The cluster ID.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to query the information of all clusters that are deployed in a specific region, such as the cluster IDs.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the information of all clusters that are deployed in a specific region, such as the cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the region.
         # 
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query all regions that are available for your account, such as the region IDs.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query all regions that are available for your account, such as the region IDs.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The region in which the TDE key resides.
         self.tderegion = tderegion
 
     def validate(self):
@@ -501,15 +515,15 @@
         # *   **0**: no.
         # *   **1**: yes.
         self.authorization_state = authorization_state
         # The cluster ID.
         self.dbcluster_id = dbcluster_id
         # The request ID.
         self.request_id = request_id
-        # The Alibaba Cloud Resource Name (ARN) of the RAM role. A RAM role is a virtual identity that you can create within your Alibaba Cloud account. For more information, see [RAM role overview](~~93689~~).
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role. A RAM role is a virtual identity that you can create within your Alibaba Cloud account. For more information, see [RAM role overview](https://help.aliyun.com/document_detail/93689.html).
         self.role_arn = role_arn
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -709,18 +723,22 @@
         owner_account: str = None,
         owner_id: int = None,
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -853,14 +871,16 @@
         # *   **false**: disables binary logging.
         # 
         # Default value: **true**.
         # 
         # > If binary logging is disabled, your PolarDB cluster is restarted.
         self.continue_enable_binlog = continue_enable_binlog
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -993,23 +1013,27 @@
         # 
         # *   It cannot start with `http://` or `https://`.
         # *   It must be 2 to 256 characters in length.
         self.account_description = account_description
         # The name of the account. The name must meet the following requirements:
         # 
         # *   It must start with a lowercase letter and end with a letter or a digit.
-        # *   It can contain lowercase letters, digits, and underscores (\_).
+        # *   It can contain lowercase letters, digits, and underscores (_).
         # *   It must be 2 to 16 characters in length.
         # *   It cannot be root, admin, or another username that is reserved by the system.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The password of the account. The password must meet the following requirements:
         # 
         # *   It must contain at least three of the following character types: uppercase letters, lowercase letters, digits, and special characters.
         # *   It must be 8 to 32 characters in length.
         # *   Special characters include `! @ # $ % ^ & * ( ) _ + - =`
+        # 
+        # This parameter is required.
         self.account_password = account_password
         # The permissions that are granted to the account. Valid values:
         # 
         # *   **ReadWrite**: read and write permissions
         # *   **ReadOnly**: read-only permissions
         # *   **DMLOnly**: the permissions to execute only DML statements
         # *   **DDLOnly**: the permissions to execute only DDL statements
@@ -1027,20 +1051,22 @@
         # *   **Normal**: standard account
         # *   **Super**: privileged account
         # 
         # > 
         # 
         # *   If you leave this parameter empty, the default value **Super** is used.
         # 
-        # *   You can create multiple privileged accounts for a PolarDB for Oracle or PolarDB for PostgreSQL cluster. A privileged account is granted more permissions than a standard account. For more information about how to create a database account, see [Create a database account](~~68508~~).
-        # *   You can create only one privileged account for a PolarDB for MySQL cluster. A privileged account is granted more permissions than a standard account. For more information about how to create a database account, see [Create a database account](~~68508~~).
+        # *   You can create multiple privileged accounts for a PolarDB for Oracle or PolarDB for PostgreSQL cluster. A privileged account is granted more permissions than a standard account. For more information about how to create a database account, see [Create a database account](https://help.aliyun.com/document_detail/68508.html).
+        # *   You can create only one privileged account for a PolarDB for MySQL cluster. A privileged account is granted more permissions than a standard account. For more information about how to create a database account, see [Create a database account](https://help.aliyun.com/document_detail/68508.html).
         self.account_type = account_type
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database that can be accessed by the account. To enter multiple database names, separate the names with commas (,).
         # 
         # > This parameter is valid only for standard accounts of PolarDB for MySQL clusters.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
@@ -1194,14 +1220,16 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -1330,14 +1358,15 @@
         owner_id: int = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.client_token = client_token
         self.cold_storage_instance_description = cold_storage_instance_description
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
@@ -1614,35 +1643,35 @@
         # 
         # > 
         # 
         # *   Only when the **DBType** parameter is set to **MySQL** and **the DBVersion** parameter is set to **5.6**, **5.7**, or **8.0**, you can set this parameter to **Basic**.
         # 
         # *   Only when the **DBType** parameter is set to **MySQL** and the **DBVersion** parameter is set to **8.0**, you can set this parameter to **ArchiveNormal** or **NormalMultimaster**.
         # 
-        # For more information, see [Product editions](~~183258~~).
+        # For more information, see [Product editions](https://help.aliyun.com/document_detail/183258.html).
         self.creation_category = creation_category
         # The method that is used to create a cluster. Valid values:
         # 
         # *   **Normal**: creates a PolarDB cluster. For more information about how to perform this operation in the console, see the following topics:
         # 
-        #     *   [Create a PolarDB for MySQL cluster](~~58769~~)
-        #     *   [Create a PolarDB for PostgreSQL cluster](~~118063~~)
-        #     *   [Create a PolarDB for Oracle cluster](~~118182~~)
+        #     *   [Create a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/58769.html)
+        #     *   [Create a PolarDB for PostgreSQL cluster](https://help.aliyun.com/document_detail/118063.html)
+        #     *   [Create a PolarDB for Oracle cluster](https://help.aliyun.com/document_detail/118182.html)
         # 
         # *   **CloneFromPolarDB**: clones data from an existing PolarDB cluster to a new PolarDB cluster. For more information about how to perform this operation in the console, see the following topics:
         # 
-        #     *   [Clone a PolarDB for MySQL cluster](~~87966~~)
-        #     *   [Clone a PolarDB for PostgreSQL cluster](~~118108~~)
-        #     *   [Clone a PolarDB for Oracle cluster](~~118221~~)
+        #     *   [Clone a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/87966.html)
+        #     *   [Clone a PolarDB for PostgreSQL cluster](https://help.aliyun.com/document_detail/118108.html)
+        #     *   [Clone a PolarDB for Oracle cluster](https://help.aliyun.com/document_detail/118221.html)
         # 
-        # *   **CloneFromRDS**: clones data from an existing ApsaraDB RDS for MySQL instance to a new PolarDB for MySQL cluster. For more information about how to perform this operation in the console, see [Create a PolarDB for MySQL cluster by cloning an ApsaraDB RDS for MySQL instance](~~121812~~).
+        # *   **CloneFromRDS**: clones data from an existing ApsaraDB RDS for MySQL instance to a new PolarDB for MySQL cluster. For more information about how to perform this operation in the console, see [Create a PolarDB for MySQL cluster by cloning an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/121812.html).
         # 
-        # *   **MigrationFromRDS**: migrates data from an existing ApsaraDB RDS for MySQL instance to a new PolarDB for MySQL cluster. By default, the created PolarDB cluster is in read-only mode, and the binary logging feature is enabled. For more information about how to perform this operation in the console, see [Create a PolarDB for MySQL cluster from an ApsaraDB RDS for MySQL instance](~~121582~~).
+        # *   **MigrationFromRDS**: migrates data from an existing ApsaraDB RDS for MySQL instance to a new PolarDB for MySQL cluster. By default, the created PolarDB cluster is in read-only mode, and the binary logging feature is enabled. For more information about how to perform this operation in the console, see [Create a PolarDB for MySQL cluster from an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/121582.html).
         # 
-        # *   **CreateGdnStandby**: creates a secondary cluster. For more information about how to perform this operation in the console, see [Add a secondary cluster](~~160381~~).
+        # *   **CreateGdnStandby**: creates a secondary cluster. For more information about how to perform this operation in the console, see [Add a secondary cluster](https://help.aliyun.com/document_detail/160381.html).
         # 
         # Default value: **Normal**.
         # 
         # > 
         # 
         # *   If the **DBType** parameter is set to **MySQL** and the **DBVersion** parameter is set to **5.6** or **5.7**, this parameter can be set to **CloneFromRDS** or **MigrationFromRDS**.
         # 
@@ -1658,25 +1687,29 @@
         # *   **8.0.2**\
         # *   **8.0.1**\
         # 
         # > This parameter is valid only when the **DBType** parameter is set to **MySQL** and the **DBVersion** parameter is set to **8.0**.
         self.dbminor_version = dbminor_version
         # The specifications of the node.
         # 
-        # *   For more information about specifications supported by PolarDB for MySQL, see [Specifications of compute nodes](~~102542~~).
-        # *   For information about node specifications supported by the Oracle database engine, see [Specifications of compute nodes](~~207921~~).
-        # *   For information about node specifications supported by the PostgreSQL database engine, see [Specifications of compute nodes](~~209380~~).
+        # *   For more information about specifications supported by PolarDB for MySQL, see [Specifications of compute nodes](https://help.aliyun.com/document_detail/102542.html).
+        # *   For information about node specifications supported by the Oracle database engine, see [Specifications of compute nodes](https://help.aliyun.com/document_detail/207921.html).
+        # *   For information about node specifications supported by the PostgreSQL database engine, see [Specifications of compute nodes](https://help.aliyun.com/document_detail/209380.html).
+        # 
+        # This parameter is required.
         self.dbnode_class = dbnode_class
         # 标准版节点个数。
         self.dbnode_num = dbnode_num
         # The type of the database engine. Valid values:
         # 
         # *   **MySQL**\
         # *   **PostgreSQL**\
         # *   **Oracle**\
+        # 
+        # This parameter is required.
         self.dbtype = dbtype
         # The version of the database engine.
         # 
         # *   Valid values for the MySQL database engine:
         # 
         #     *   **5.6**\
         #     *   **5.7**\
@@ -1684,14 +1717,16 @@
         # 
         # *   Valid values for the PostgreSQL database engine:
         # 
         #     *   **11**\
         #     *   **14**\
         # 
         # *   Valid value for the Oracle database engine: **11**\
+        # 
+        # This parameter is required.
         self.dbversion = dbversion
         # The time zone of the cluster. The time must be in UTC. You can set the parameter to a value that is on the hour from **-12:00 to +13:00**. Example: 00:00. Default value: **SYSTEM**, which means that the value is the same as the time zone of the region.
         # 
         # > This parameter is valid only when the **DBType** parameter is set to **MySQL**.
         self.default_time_zone = default_time_zone
         # The ID of the Global Database Network (GDN).
         # 
@@ -1722,20 +1757,22 @@
         # 
         # > This parameter is valid only when the **DBType** parameter is set to **MySQL**.
         self.lower_case_table_names = lower_case_table_names
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the parameter template.
         # 
-        # > You can call the [DescribeParameterGroups](~~207178~~) operation to query the details of all parameter templates of a specified region, such as the ID of a parameter template.
+        # > You can call the [DescribeParameterGroups](https://help.aliyun.com/document_detail/207178.html) operation to query the details of all parameter templates of a specified region, such as the ID of a parameter template.
         self.parameter_group_id = parameter_group_id
         # The billing method. Valid values:
         # 
         # *   **Postpaid**: pay-as-you-go
         # *   **Prepaid**: subscription
+        # 
+        # This parameter is required.
         self.pay_type = pay_type
         # The subscription type of the subscription cluster. This parameter is required only when the PayType parameter is set to **Prepaid**. Valid values:
         # 
         # *   **Year**: annual subscription. Unit: years.
         # *   **Month**: monthly subscription. Unit: months.
         self.period = period
         self.provisioned_iops = provisioned_iops
@@ -1744,15 +1781,17 @@
         # 数据库代理类型，取值范围如下：
         # 
         # - **Exclusive**：企业独享版
         # - **General**：企业通用版
         self.proxy_type = proxy_type
         # The region ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The maximum number of PCUs per node for scaling. Valid values: 1 PCU to 32 PCUs.
         # 
@@ -1816,15 +1855,15 @@
         # *   **true**\
         # *   **false**\
         # 
         # > 
         # 
         # *   This parameter is valid only when the **DBType** parameter is set to **PostgreSQL** or **Oracle**.
         # 
-        # *   You can call the [ModifyDBClusterTDE](~~167982~~) operation to enable TDE for a PolarDB for MySQL cluster.
+        # *   You can call the [ModifyDBClusterTDE](https://help.aliyun.com/document_detail/167982.html) operation to enable TDE for a PolarDB for MySQL cluster.
         # *   TDE cannot be disabled after it is enabled.
         self.tdestatus = tdestatus
         # 1
         self.tag = tag
         # *   If the **Period** parameter is set to **Month**, the **UsedTime** parameter can be set to `1, 2, 3, 4, 5, 6, 7, 8, or 9`.
         # *   If the **Period** parameter is set to **Year**, the **UsedTime** parameter can be set to `1, 2, or 3`.
         self.used_time = used_time
@@ -1832,15 +1871,15 @@
         self.vpcid = vpcid
         # The vSwitch ID of the cluster.
         # 
         # > If the VPCId parameter is specified, the VSwitchId parameter is required.
         self.v_switch_id = v_switch_id
         # The zone ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available zones.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available zones.
         self.zone_id = zone_id
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -2191,14 +2230,16 @@
         # *   **Disable**: Newly added nodes are not automatically associated with the cluster endpoint.
         # 
         # Default value: **Disable**.
         self.auto_add_new_nodes = auto_add_new_nodes
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the custom cluster endpoint.
         self.dbendpoint_description = dbendpoint_description
         # The advanced configurations of the cluster endpoint. You must specify the configurations in the JSON format. You can specify the configurations of the following attributes: consistency level, transaction splitting, connection pool, and offload reads from the primary node.
         # 
         # *   Specify the consistency level in the format of `{"ConsistLevel":"Consistency level"}`. Default value: 1. Valid values:
         # 
@@ -2225,14 +2266,16 @@
         # >- You can specify the transaction splitting, connection pool, and offload reads from the primary node features for a PolarDB for MySQL cluster only if ReadWriteMode is set to ReadWrite for the cluster endpoint.
         # >- Only PolarDB for MySQL supports global consistency.
         # >- If the **ReadWriteMode** parameter is set to **ReadOnly**, the consistency level must be **0**.
         # >- You can use one record to specify the consistency level, transaction splitting, connection pool, and offload reads from the primary node features, such as `{"ConsistLevel":"1","DistributedTransaction":"on","ConnectionPersist":"Session","MasterAcceptReads":"on"}`.
         # >- The transaction splitting settings are restricted by the consistency level settings. For example, if you set the consistency level to **0**, transaction splitting cannot be enabled. If you set the consistency level to **1** or **2**, transaction splitting can be enabled.
         self.endpoint_config = endpoint_config
         # The type of the cluster endpoint. Set the value to **Custom**.
+        # 
+        # This parameter is required.
         self.endpoint_type = endpoint_type
         # The reader nodes that you want to associate with the endpoint. If you want to specify multiple reader nodes, separate the reader nodes with commas (,). If you do not specify this parameter, all nodes are used.
         # 
         # >- You need to specify the node IDs for a PolarDB for MySQL cluster.
         # >- You need to specify the role name of each node for a PolarDB for PostgreSQL cluster or a PolarDB for PostgreSQL (Compatible with Oracle) cluster. Example: `Writer, Reader1, Reader2`.
         # >- If you set **ReadWriteMode** to **ReadOnly**, you can associate only one node with the endpoint. If the only node becomes faulty, the cluster endpoint may be unavailable for up to 1 hour. We recommend that you associate more than one node with the cluster endpoint in production environments. We recommend that you associate at least two nodes with the cluster endpoint to improve service availability.
         # >- If you set **ReadWriteMode** to **ReadWrite**, you need to associate at least two nodes with the cluster endpoint.
@@ -2437,20 +2480,26 @@
         # The prefix of the new endpoint. The prefix of the endpoint must meet the following requirements:
         # 
         # *   The prefix can contain lowercase letters, digits, and hyphens (-).
         # *   The prefix must start with a letter and end with a digit or a letter.
         # *   The prefix must be 6 to 40 characters in length.
         self.connection_string_prefix = connection_string_prefix
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the endpoint.
         # 
-        # >  You can call the [DescribeDBClusterEndpoints](~~98205~~) operation to query endpoint details.
+        # >  You can call the [DescribeDBClusterEndpoints](https://help.aliyun.com/document_detail/98205.html) operation to query endpoint details.
+        # 
+        # This parameter is required.
         self.dbendpoint_id = dbendpoint_id
         # The network type of the endpoint. Set the value to **Public**.
+        # 
+        # This parameter is required.
         self.net_type = net_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The ID of the ECS security group.
         self.security_group_id = security_group_id
@@ -2617,58 +2666,70 @@
         target_port: str = None,
         vpc_id: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can only contain ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The ID of the source cluster that the database link connects.
         # 
-        # >  You can call the [DescribeDBClusters](~~173433~~) operation to query PolarDB clusters.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/173433.html) operation to query PolarDB clusters.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database link.
         # 
-        # *   The name must contain lowercase letters and can also contain digits and underscores (\_).
+        # *   The name must contain lowercase letters and can also contain digits and underscores (_).
         # *   The name must start with a letter and end with a letter or digit.
         # *   The name must be 1 to 64 characters in length.
+        # 
+        # This parameter is required.
         self.dblink_name = dblink_name
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the region.
         # 
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query information about regions.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query information about regions.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The name of the source database.
         # 
-        # >  You can call the [DescribeDatabases](~~173558~~) operation to query information about databases in a PolarDB cluster.
+        # >  You can call the [DescribeDatabases](https://help.aliyun.com/document_detail/173558.html) operation to query information about databases in a PolarDB cluster.
+        # 
+        # This parameter is required.
         self.source_dbname = source_dbname
         # The account of the destination database.
         # 
-        # >  You can call the [DescribeAccounts](~~173549~~) operation to query the account of a PolarDB cluster.
+        # >  You can call the [DescribeAccounts](https://help.aliyun.com/document_detail/173549.html) operation to query the account of a PolarDB cluster.
+        # 
+        # This parameter is required.
         self.target_dbaccount = target_dbaccount
         # The ID of the destination cluster that the database link connects.
         # 
         # > *   If the destination cluster is a user-created Oracle database on an ECS instance, set the value to `null`.
-        # > *   You can call the [DescribeDBClusters](~~173433~~) operation to query PolarDB clusters.
+        # > *   You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/173433.html) operation to query PolarDB clusters.
         self.target_dbinstance_name = target_dbinstance_name
         # The name of the destination database.
         # 
-        # >  You can call the [DescribeDatabases](~~173558~~) operation to query information about databases in a PolarDB cluster.
+        # >  You can call the [DescribeDatabases](https://help.aliyun.com/document_detail/173558.html) operation to query information about databases in a PolarDB cluster.
+        # 
+        # This parameter is required.
         self.target_dbname = target_dbname
         # The account password of the destination database.
+        # 
+        # This parameter is required.
         self.target_dbpasswd = target_dbpasswd
         # The IP address of the user-created Oracle database on an ECS instance.
         self.target_ip = target_ip
         # The port number of the user-created Oracle database on an ECS instance.
         self.target_port = target_port
         # The ID of the virtual private cloud (VPC).
         # 
-        # >  You can call the [DescribeVpcs](~~35739~~) operation to query information about VPCs.
+        # >  You can call the [DescribeVpcs](https://help.aliyun.com/document_detail/35739.html) operation to query information about VPCs.
         self.vpc_id = vpc_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2824,23 +2885,23 @@
     def __init__(
         self,
         target_class: str = None,
         zone_id: str = None,
     ):
         # The specifications of the read-only node that you want to add, which must be the same as the specifications of the existing nodes. For more information, see the following topics:
         # 
-        # *   PolarDB for MySQL: [Specifications of compute nodes](~~102542~~)
-        # *   PolarDB for PostgreSQL (Compatible with Oracle): [Specifications of compute nodes](~~207921~~)
-        # *   PolarDB for PostgreSQL: [Specifications of compute nodes](~~209380~~)
+        # *   PolarDB for MySQL: [Specifications of compute nodes](https://help.aliyun.com/document_detail/102542.html)
+        # *   PolarDB for PostgreSQL (Compatible with Oracle): [Specifications of compute nodes](https://help.aliyun.com/document_detail/207921.html)
+        # *   PolarDB for PostgreSQL: [Specifications of compute nodes](https://help.aliyun.com/document_detail/209380.html)
         # 
         # >- You need to specify either DBNode.N.ZoneId or DBNode.N.TargetClass. N is an integer that starts from 1. The maximum value of N is equal to 16 minus the number of existing nodes.
         # >- You can add multiple read-only nodes at the same time only to PolarDB for MySQL clusters, which can contain up to of 15 read-only nodes.
         # >- This parameter is required for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters. This parameter is optional for PolarDB for MySQL clusters.
         self.target_class = target_class
-        # The zone ID of the node that you want to add, which must be the same as the zone ID of existing nodes. You can call the [DescribeRegions](~~98041~~) operation to query the IDs of zones.
+        # The zone ID of the node that you want to add, which must be the same as the zone ID of existing nodes. You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the IDs of zones.
         # 
         # >- You need to specify either DBNode.N.ZoneId or DBNode.N.TargetClass. N is an integer that starts from 1. The maximum value of N is equal to 16 minus the number of existing nodes.
         # >- You can add multiple read-only nodes at the same time only to PolarDB for MySQL clusters, which can contain up to of 15 read-only nodes.
         # >- This parameter is required for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters. This parameter is optional for PolarDB for MySQL clusters.
         self.zone_id = zone_id
 
     def validate(self):
@@ -2883,25 +2944,29 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The details of the read-only node.
+        # 
+        # This parameter is required.
         self.dbnode = dbnode
         # The type of the node. Valid values:
         # 
         # *   RO
         # *   STANDBY
         # *   DLNode
         self.dbnode_type = dbnode_type
         # The ID of the cluster endpoint to which the read-only node is added. If you want to add the read-only node to multiple endpoints at the same time, separate the endpoint IDs with commas (,).
-        # > - You can call the [DescribeDBClusterEndpoints](~~98205~~) operation to query the details of cluster endpoints, including endpoint IDs.
+        # > - You can call the [DescribeDBClusterEndpoints](https://help.aliyun.com/document_detail/98205.html) operation to query the details of cluster endpoints, including endpoint IDs.
         # >- You can enter the ID of the default cluster endpoint or a custom cluster endpoint.
         # >- If you leave this parameter empty, the read-only node is added to all cluster endpoints for which the **Automatically Associate New Nodes** feature is enabled. If you set `AutoAddNewNodes` to `Enable`, the Automatically Associate New Nodes feature is enabled.
         self.endpoint_bind_list = endpoint_bind_list
         # Specifies whether to enable the In-Memory Column Index (IMCI) feature. Default value: OFF. Valid values:
         # 
         # *   **ON**\
         # *   **OFF**\
@@ -3132,15 +3197,15 @@
         dbdescription: str = None,
         dbname: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
-        # The name of the account that is authorized to access the database. You can call the [DescribeAccounts](~~98107~~) operation to query account information.
+        # The name of the account that is authorized to access the database. You can call the [DescribeAccounts](https://help.aliyun.com/document_detail/98107.html) operation to query account information.
         # >- You can specify only a standard account. By default, privileged accounts have all permissions on all databases. You do not need to grant privileged accounts the permissions to access the database.
         # >- This parameter is required for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters. This parameter is optional for PolarDB for MySQL clusters.
         self.account_name = account_name
         # The permissions that are granted to the account. Valid values:
         # 
         # *   **ReadWrite**: read and write permissions.
         # *   **ReadOnly**: read-only permissions.
@@ -3150,15 +3215,17 @@
         # 
         # If you leave this parameter empty, the default value **ReadWrite** is used.
         # 
         # >- This parameter is valid only if you specify **AccountName**.
         # >- This parameter is required for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters.
         # >- This parameter is optional for PolarDB for MySQL clusters.
         self.account_privilege = account_privilege
-        # The character set that is used by the cluster. For more information, see [Character set tables](~~99716~~).
+        # The character set that is used by the cluster. For more information, see [Character set tables](https://help.aliyun.com/document_detail/99716.html).
+        # 
+        # This parameter is required.
         self.character_set_name = character_set_name
         # The language that indicates the collation of the databases that are created.
         # 
         # > *   The language must be compatible with the character set that is specified by **CharacterSetName**.
         # >*   This parameter is required for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters. This parameter is not supported by PolarDB for MySQL clusters.
         # 
         # To view the valid values for this parameter, perform the following steps: Log on to the PolarDB console and click the ID of a cluster. In the left-side navigation pane, choose **Settings and Management** > **Databases**. Then, click **Create Database**.
@@ -3168,28 +3235,32 @@
         # >- The language must be compatible with the character set that is specified by **CharacterSetName**.
         # >- The value that you specify must be the same as the value of **Collate**.
         # >- This parameter is required for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters. This parameter is optional for PolarDB for MySQL clusters.
         # 
         # To view the valid values for this parameter, perform the following steps: Log on to the PolarDB console and click the ID of a cluster. In the left-side navigation pane, choose **Settings and Management** > **Databases**. Then, click **Create Database**.
         self.ctype = ctype
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The description of the database. The description must meet the following requirements:
         # 
         # *   It cannot start with `http://` or `https://`.
         # *   It must be 2 to 256 characters in length.
         # 
         # > This parameter is required for a PolarDB for Oracle or PolarDB for PostgreSQL cluster. This parameter is optional for a PolarDB for MySQL cluster.
         self.dbdescription = dbdescription
         # The name of the database. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, hyphens (-), and underscores (\_).
+        # *   The name can contain lowercase letters, digits, hyphens (-), and underscores (_).
         # *   The name must start with a lowercase letter and end with a lowercase letter or a digit. The name must be 1 to 64 characters in length.
         # 
         # > Do not use reserved words as database names, such as `test` or `mysql`.
+        # 
+        # This parameter is required.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -3334,20 +3405,22 @@
         owner_id: int = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the primary cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The description of the GDN. The description must meet the following requirements:
         # 
         # *   It cannot start with [http:// or https://.](http://https://。)
         # *   It must start with a letter.
-        # *   It can contain letters, digits, underscores (\_), and hyphens (-).
+        # *   It can contain letters, digits, underscores (_), and hyphens (-).
         # *   It must be 2 to 126 characters in length.
         self.gdndescription = gdndescription
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
@@ -3490,24 +3563,30 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The IP address in the whitelist template.
         # 
         # >  Multiple IP addresses are separated by commas (,). You can create up to 1,000 IP addresses or CIDR blocks for all IP whitelists.
+        # 
+        # This parameter is required.
         self.gip_list = gip_list
         # The name of the IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or digit.
         # *   The name must be 2 to 120 characters in length.
+        # 
+        # This parameter is required.
         self.global_ig_name = global_ig_name
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -3573,15 +3652,15 @@
     ):
         # The IP address in the whitelist template.
         # 
         # >  Separate multiple IP addresses with commas (,). You can add up to 1,000 IP addresses or CIDR blocks to all IP whitelists.
         self.gip_list = gip_list
         # The name of the IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or a digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the IP whitelist template.
         self.global_security_group_id = global_security_group_id
         # The ID of the region.
         self.region_id = region_id
@@ -3714,37 +3793,47 @@
         parameters: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The type of the database engine. Only **MySQL** is supported.
+        # 
+        # This parameter is required.
         self.dbtype = dbtype
         # The version of the database engine. Valid values:
         # 
         # *   **5.6**\
         # *   **5.7**\
         # *   **8.0**\
+        # 
+        # This parameter is required.
         self.dbversion = dbversion
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The description of the parameter template. It must be 0 to 199 characters in length.
         self.parameter_group_desc = parameter_group_desc
         # The name of the parameter template. The name must meet the following requirements:
         # 
-        # *   It can contain letters, digits, and underscores (\_). It must start with a letter and cannot end with an underscore.**\
+        # *   It can contain letters, digits, and underscores (_). It must start with a letter and cannot end with an underscore.**\
         # *   It must be 8 to 64 characters in length.
+        # 
+        # This parameter is required.
         self.parameter_group_name = parameter_group_name
         # The JSON string that consists of parameters and values. The parameter values are strings. Example: `{"wait_timeout":"86400","innodb_old_blocks_time":"1000"}`.
         # 
-        # > You can call the [DescribeParameterTemplates](~~207428~~) operation to query the details of all parameters in the cluster of a specified engine version, such as the parameter name and valid values.
+        # > You can call the [DescribeParameterTemplates](https://help.aliyun.com/document_detail/207428.html) operation to query the details of all parameters in the cluster of a specified engine version, such as the parameter name and valid values.
+        # 
+        # This parameter is required.
         self.parameters = parameters
         # The region ID.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -3811,15 +3900,15 @@
     def __init__(
         self,
         parameter_group_id: str = None,
         request_id: str = None,
     ):
         # The ID of the parameter template.
         # 
-        # > You can call the [DescribeParameterGroups](~~207178~~) operation to query the details of all parameter templates of a specified region, such as the ID of a parameter template.
+        # > You can call the [DescribeParameterGroups](https://help.aliyun.com/document_detail/207178.html) operation to query the details of all parameter templates of a specified region, such as the ID of a parameter template.
         self.parameter_group_id = parameter_group_id
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -4016,28 +4105,36 @@
         self.client_token = client_token
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The unit of the subscription duration for the storage plan. Valid values:
         # 
         # *   **Month**\
         # *   **Year**\
+        # 
+        # This parameter is required.
         self.period = period
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The capacity of the storage plan. Unit: GB. Valid values: 50, 100, 200, 300, 500, 1000, 2000, 3000, 5000, 10000, 15000, 20000, 25000, 30000, 50000, 100000, and 200000
+        # 
+        # This parameter is required.
         self.storage_class = storage_class
         # The type of the storage plan. Valid values:
         # 
         # *   **Mainland**: The storage plan is used inside the Chinese mainland.
         # *   **Overseas**: The storage plan is used outside the Chinese mainland.
+        # 
+        # This parameter is required.
         self.storage_type = storage_type
         # The subscription duration of the storage plan.
         # 
         # *   If **Period** is set to **Month**, the value ranges from 1 to 9.
         # *   If **Period** is set to **Year**, the value can be 1, 2, 3, or 5.
+        # 
+        # This parameter is required.
         self.used_time = used_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4178,16 +4275,20 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The username of the account.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -4307,17 +4408,21 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The backup ID. If you need to specify multiple backup IDs, separate the backup IDs with commas (,).
         # 
-        # >  You can call the [DescribeBackups](~~98102~~) operation to query the backup IDs.
+        # >  You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the backup IDs.
+        # 
+        # This parameter is required.
         self.backup_id = backup_id
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -4442,14 +4547,16 @@
         # The retention policy for the backup sets when you delete the cluster. Valid values:
         # 
         # *   **ALL**: permanently retains all backups.
         # *   **LATEST**: permanently retains the most recent backup. A backup is automatically created before you delete the cluster.
         # *   **NONE**: No backup sets are retained after you delete the cluster.
         self.backup_retention_policy_on_cluster_deletion = backup_retention_policy_on_cluster_deletion
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -4568,16 +4675,20 @@
         dbendpoint_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the custom cluster endpoint.
+        # 
+        # This parameter is required.
         self.dbendpoint_id = dbendpoint_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -4698,21 +4809,27 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to query the details of all clusters that belong to your account, such as the cluster ID.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of all clusters that belong to your account, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the endpoint.
         # 
-        # >  You can call the [DescribeDBClusterEndpoints](~~98205~~) operation to query the endpoints of a specified PolarDB cluster.
+        # >  You can call the [DescribeDBClusterEndpoints](https://help.aliyun.com/document_detail/98205.html) operation to query the endpoints of a specified PolarDB cluster.
+        # 
+        # This parameter is required.
         self.dbendpoint_id = dbendpoint_id
         # The network type of the endpoint. Set the value to **Public** (public network).
+        # 
+        # This parameter is required.
         self.net_type = net_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -4836,17 +4953,21 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the source cluster where a database link is to be deleted.
         # 
-        # >  You can call the [DescribeDBClusters](~~173433~~) operation to query PolarDB clusters.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/173433.html) operation to query PolarDB clusters.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database link to be deleted.
+        # 
+        # This parameter is required.
         self.dblink_name = dblink_name
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -4969,18 +5090,22 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The IDs of the nodes.
         # 
-        # > You can call the [DescribeDBClusters](~~185342~~) operation to query the details of all clusters that belong to your Alibaba Cloud account, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/185342.html) operation to query the details of all clusters that belong to your Alibaba Cloud account, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbnode_id = dbnode_id
         # The type of the node. Valid values:
         # 
         # *   RO
         # *   STANDBY
         self.dbnode_type = dbnode_type
         self.owner_account = owner_account
@@ -5126,16 +5251,20 @@
         dbname: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database.
+        # 
+        # This parameter is required.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -5255,14 +5384,16 @@
         owner_id: int = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the GDN.
+        # 
+        # This parameter is required.
         self.gdnid = gdnid
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -5392,23 +5523,27 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The name of the IP whitelist template. The name of the IP whitelist template must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the IP whitelist template.
+        # 
+        # This parameter is required.
         self.global_security_group_id = global_security_group_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -5477,15 +5612,15 @@
         self.dbinstances = dbinstances
         # The IP address in the whitelist template.
         # 
         # >  Multiple IP addresses are separated by commas (,). You can create up to 1,000 IP addresses or CIDR blocks for all IP whitelists.
         self.gip_list = gip_list
         # The name of the global IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or a digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the global IP whitelist template.
         self.global_security_group_id = global_security_group_id
         # The ID of the region.
         self.region_id = region_id
@@ -5614,19 +5749,23 @@
     def __init__(
         self,
         dbcluster_id: str = None,
         rule_name_list: str = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the masking rule. You can specify multiple masking rules at a time. Separate the masking rules with commas (,).
         # 
-        # > You can call the [DescribeMaskingRules](~~212573~~) operation to query details of all the masking rules for a specified cluster, such as the names of the masking rules.
+        # > You can call the [DescribeMaskingRules](https://help.aliyun.com/document_detail/212573.html) operation to query details of all the masking rules for a specified cluster, such as the names of the masking rules.
+        # 
+        # This parameter is required.
         self.rule_name_list = rule_name_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5749,19 +5888,23 @@
         resource_owner_id: int = None,
     ):
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The parameter template ID.
         # 
         #  
-        # >  You can call the [DescribeParameterGroups](~~207178~~) operation to query the parameter template ID.
+        # >  You can call the [DescribeParameterGroups](https://help.aliyun.com/document_detail/207178.html) operation to query the parameter template ID.
+        # 
+        # This parameter is required.
         self.parameter_group_id = parameter_group_id
         # The region ID.
         #  
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query available regions.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -5884,14 +6027,16 @@
         owner_account: str = None,
         owner_id: int = None,
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the region.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -6040,14 +6185,16 @@
         page_size: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The name of the account.
         self.account_name = account_name
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The page number of the page to return. Set this parameter to an integer that is larger than 0. Default value: **1**.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
@@ -6348,15 +6495,17 @@
         self.owner_id = owner_id
         # The page number. The value must be an integer that is larger than 0 and does not exceed the maximum value of the INTEGER data type. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values: 30, 50, and 100. Default value: 30.
         self.page_size = page_size
         # The ID of the region.
         # 
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query the region ID details.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the region ID details.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -6631,16 +6780,20 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         start_time: str = None,
     ):
         # The region for the backup data.
         self.backup_region = backup_region
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The end of the time range to query. The end time must be later than the start time. Specify the time in the ISO 8601 standard in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The page number of the page to return. The value must be an integer that is larger than 0. Default value: **1**.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
@@ -6649,14 +6802,16 @@
         # *   **100**\
         # 
         # Default value: **30**.
         self.page_size = page_size
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6719,23 +6874,23 @@
         backup_log_name: str = None,
         backup_log_size: str = None,
         backup_log_start_time: str = None,
         download_link: str = None,
         intranet_download_link: str = None,
         link_expired_time: str = None,
     ):
-        # The time when the backup task ended. The time follows the ISO 8601 standard in the `YYYY-MM-DD\"T\"HH:mm:ssZ` format. The time is displayed in UTC.
+        # The time when the backup task ended. The time follows the ISO 8601 standard in the `YYYY-MM-DD\\"T\\"HH:mm:ssZ` format. The time is displayed in UTC.
         self.backup_log_end_time = backup_log_end_time
         # The ID of the backup log.
         self.backup_log_id = backup_log_id
         # The name of the backup log.
         self.backup_log_name = backup_log_name
         # The size of the backup log. Unit: bytes.
         self.backup_log_size = backup_log_size
-        # The time when the backup task started. The time follows the ISO 8601 standard in the `YYYY-MM-DD\"T\"HH:mm:ssZ` format. The time is displayed in UTC.
+        # The time when the backup task started. The time follows the ISO 8601 standard in the `YYYY-MM-DD\\"T\\"HH:mm:ssZ` format. The time is displayed in UTC.
         self.backup_log_start_time = backup_log_start_time
         # The public URL used to download the backup log.
         self.download_link = download_link
         # The internal URL used to download the backup log.
         self.intranet_download_link = intranet_download_link
         # The time when the download URL expires.
         self.link_expired_time = link_expired_time
@@ -6929,15 +7084,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -7014,38 +7171,38 @@
         # 
         # *   **Normal**: standard backup. The system backs up data once a day.
         # *   **2/24H**: frequent backup. The system backs up data every 2 hours.
         # *   **3/24H**: frequent backup. The system backs up data every 3 hours.
         # *   **4/24H**: frequent backup. The system backs up data every 4 hours.
         # 
         # >- This parameter is not supported for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_1backup_frequency = data_level_1backup_frequency
         # The backup cycle of level-1 backups. Valid values:
         # 
         # *   **Monday**\
         # *   **Tuesday**\
         # *   **Wednesday**\
         # *   **Thursday**\
         # *   **Friday**\
         # *   **Saturday**\
         # *   **Sunday**\
         # 
         # >- You need to specify at least two values. Separate multiple values with commas (,).
         # >- This parameter is not supported for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_1backup_period = data_level_1backup_period
         # The retention period of level-1 backups. Valid values: 3 to 14. Unit: day.
         self.data_level_1backup_retention_period = data_level_1backup_retention_period
         # The period of time during which automatic backup is performed. The value must be in the `hh:mmZ-hh:mmZ` format. The time must be in UTC. The start time and the end time must be on the hour and must have an interval of 1 hour. Example: `14:00Z-15:00Z`.
         # 
         # >- This parameter is not supported for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_1backup_time = data_level_1backup_time
-        # The region where the cross-region level-2 backup is stored. For information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # The region where the cross-region level-2 backup is stored. For information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_2backup_another_region_region = data_level_2backup_another_region_region
         # The retention period of cross-region level-2 backups. Valid values:
         # 
         # *   **0**: The cross-region level-2 backup feature is disabled.
         # *   **30 to 7300**: Cross-region level-2 backups are retained for 30 to 7,300 days.
         # *   **1**: Cross-region level-2 backups are permanently retained.
         # 
@@ -7059,21 +7216,21 @@
         # *   **Thursday**\
         # *   **Friday**\
         # *   **Saturday**\
         # *   **Sunday**\
         # 
         # >- You need to specify at least two values. Separate multiple values with commas (,).
         # >- This parameter is not supported for PolarDB for PostgreSQL (Compatible with Oracle) clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is unavailable if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_2backup_period = data_level_2backup_period
         # The retention period of level-2 backups. Valid values:
         # 
         # *   0: The level-2 backup feature is disabled.
         # *   30 to 7300: Level-2 backups are retained for 30 to 7,300 days.
-        # *   \-1: Level-2 backups are permanently retained.
+        # *   \\-1: Level-2 backups are permanently retained.
         # 
         # > The default value is **0**. By default, the level-2 backup feature is disabled when you create a cluster.
         self.data_level_2backup_retention_period = data_level_2backup_retention_period
         # The backup cycle. Valid values:
         # 
         # *   Monday
         # *   Tuesday
@@ -7218,14 +7375,16 @@
         self.backup_job_id = backup_job_id
         # The backup mode. Valid values:
         # 
         # *   **Automated**\
         # *   **Manual**\
         self.backup_mode = backup_mode
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -7491,16 +7650,20 @@
         self.backup_region = backup_region
         # The status of the backup set. Valid values:
         # 
         # *   **Success**\
         # *   **Failed**\
         self.backup_status = backup_status
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The end of the time range to query. Specify the time in the `YYYY-MM-DDThh:mmZ` format. The time must be in UTC. The end time must be later than the start time.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The page number. The value must be a positive integer that does not exceed the maximum value of the INTEGER data type. Default value: **1**.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
@@ -7509,14 +7672,16 @@
         # *   **100**\
         # 
         # Default value: **30**.
         self.page_size = page_size
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The beginning of the time range to query. Specify the time in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7610,15 +7775,15 @@
         # The backup mode. Valid values:
         # 
         # *   **Automated**\
         # *   **Manual**\
         self.backup_mode = backup_mode
         # The size of the backup set. Unit: bytes.
         # 
-        # > After you delete the target snapshot backups, the storage space that is consumed by the backups is released. The released storage space is smaller than the size of the backup file, because the snapshots share specific data blocks. For more information, see [FAQ about backup](~~164881~~).
+        # > After you delete the target snapshot backups, the storage space that is consumed by the backups is released. The released storage space is smaller than the size of the backup file, because the snapshots share specific data blocks. For more information, see [FAQ about backup](https://help.aliyun.com/document_detail/164881.html).
         self.backup_set_size = backup_set_size
         # The start time of the backup task. The time is displayed in UTC. Unit: seconds.
         self.backup_start_time = backup_start_time
         # The status of the backup set. Valid values:
         # 
         # *   **Success**\
         # *   **Failed**\
@@ -7891,15 +8056,17 @@
         # 
         # > You can only query character sets that PolarDB for MySQL clusters support. If you enter the ID of a PolarDB for PostgreSQL or PolarDB for Oracle cluster, the returned value of the `CharacterSetNameItems` parameter is an empty string.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -8064,26 +8231,28 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The code of the commodity. Valid values:
         # 
         # *   polardb_sub: the subscription cluster in regions in the Chinese mainland
-        # *   polardb_sub \_intl: the subscription cluster in regions outside the Chinese mainland
+        # *   polardb_sub _intl: the subscription cluster in regions outside the Chinese mainland
         # *   polardb_payg: the pay-as-you-go cluster in regions in the Chinese mainland
         # *   polardb_payg_intl: the pay-as-you-go cluster in regions outside the Chinese mainland
         # *   polardb_sub_jushita: the subscription cluster for CloudTmall
         # *   polardb_payg_jushita: the pay-as-you-go cluster for CloudTmall
         # *   polardb_sub_cainiao: the subscription cluster for Cainiao
         # *   polardb_payg_cainiao: the pay-as-you-go cluster for Cainiao
         # 
         # > *   If you use an Alibaba Cloud account on the China site, you can view only the codes of the commodities that are available in the Chinese mainland.
         # >*   If you are using an Alibaba Cloud international account, you can view only the codes of the commodities that are available outside the Chinese mainland.
         # >*   If you use a CloudTmall account, you can view only the codes of the commodities that are available in CloudTmall.
         # >*   If you use a Cainiao account, you can view only the codes of the commodities that are available in Cainiao.
+        # 
+        # This parameter is required.
         self.commodity_code = commodity_code
         # The number of nodes. Valid values:
         # 
         # *   single: Standalone Edition.
         # *   cluster: Cluster Edition.
         # *   all: both Standalone Edition and Cluster Edition.
         self.master_ha = master_ha
@@ -8393,14 +8562,16 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the PolarDB cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -8697,15 +8868,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specifies whether to query information about AI-related nodes.
         self.describe_type = describe_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -8824,14 +8997,16 @@
         self.max_iops = max_iops
         self.memory_size = memory_size
         self.remote_memory_size = remote_memory_size
         # Indicates whether the global consistency (high-performance mode) feature is enabled for the node. Valid values:
         # 
         # *   **ON**\
         # *   **OFF**\
+        # 
+        # This parameter is required.
         self.scc_mode = scc_mode
         # The routing weight of the node. Valid values: 1 to 100 Default value: 1.
         self.server_weight = server_weight
         # The type of the serverless node. Only **AgileServerless** can be returned.
         # 
         # > This parameter is supported only for serverless clusters.
         self.serverless_type = serverless_type
@@ -9037,15 +9212,15 @@
         # *   DLNode: AI node
         self.ai_type = ai_type
         self.architecture = architecture
         # Maximum blktags in file system.
         self.blktag_total = blktag_total
         # The current blktag usage.
         self.blktag_used = blktag_used
-        # [The edition of PolarDB](~~183258~~). Valid values:
+        # [The edition of PolarDB](https://help.aliyun.com/document_detail/183258.html). Valid values:
         # 
         # *   **Normal**: Cluster Edition.
         # *   **Basic**: Single Node Edition.
         # *   **Archive**: X-Engine Edition.
         # *   **NormalMultimaster**: Multi-master Cluster Edition.
         # *   **SENormal**: Standard Edition.
         # 
@@ -9059,29 +9234,29 @@
         self.creation_time = creation_time
         # The description of the cluster.
         self.dbcluster_description = dbcluster_description
         # The ID of cluster.
         self.dbcluster_id = dbcluster_id
         # The network type of the cluster.
         self.dbcluster_network_type = dbcluster_network_type
-        # The status of the cluster. For information about the valid values, see [Cluster states](~~99286~~).
+        # The status of the cluster. For information about the valid values, see [Cluster states](https://help.aliyun.com/document_detail/99286.html).
         self.dbcluster_status = dbcluster_status
         # The details of the nodes.
         self.dbnodes = dbnodes
         # The type of the database engine.
         self.dbtype = dbtype
         # The version of the database engine.
         self.dbversion = dbversion
         # The status of the minor version. Valid values:
         # 
         # *   **Stable**: The minor version is stable.
         # *   **Old**: The minor version is outdated. We recommend that you upgrade the cluster to the latest version.
         # *   **HighRisk**: The minor version has critical defects. We recommend that you immediately upgrade the cluster to the latest version.
         # 
-        # > For more information about how to upgrade the minor version, see [Upgrade versions](~~158572~~).
+        # > For more information about how to upgrade the minor version, see [Upgrade versions](https://help.aliyun.com/document_detail/158572.html).
         self.dbversion_status = dbversion_status
         # The total physical storage of level-1 backups (snapshots). Unit: bytes.
         self.data_level_1backup_chain_size = data_level_1backup_chain_size
         # Indicates the rule of data replication. Valid values: AsyncSync: asynchronous. SemiSync: semi-synchronous.
         self.data_sync_mode = data_sync_mode
         # Indicates whether the cluster is locked and can be deleted. Valid values:
         # 
@@ -9505,14 +9680,16 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -9640,15 +9817,15 @@
         owner_id: int = None,
         pay_type: str = None,
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         zone_id: str = None,
     ):
-        # The specifications of the node. For more information, see [Specifications of compute nodes](~~102542~~).
+        # The specifications of the node. For more information, see [Specifications of compute nodes](https://help.aliyun.com/document_detail/102542.html).
         self.dbnode_class = dbnode_class
         # The type of the database engine. Valid values:
         # 
         # *   **MySQL**\
         # *   **PostgreSQL**\
         # *   **Oracle**\
         self.dbtype = dbtype
@@ -9669,24 +9846,26 @@
         self.dbversion = dbversion
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The billing method of the cluster. Valid values:
         # 
         # *   **Postpaid**: pay-as-you-go
         # *   **Prepaid**: subscription
+        # 
+        # This parameter is required.
         self.pay_type = pay_type
         # The region ID of the cluster. Default value: **cn-hangzhou**.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query the available regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the available regions.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The zone ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query the available zones.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the available zones.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9971,23 +10150,27 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
         source_ip_address: str = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
         # The source IP address.
+        # 
+        # This parameter is required.
         self.source_ip_address = source_ip_address
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10146,15 +10329,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the endpoint.
         self.dbendpoint_id = dbendpoint_id
         self.describe_type = describe_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
@@ -10505,14 +10690,16 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -11027,14 +11214,16 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -11156,14 +11345,16 @@
         describe_type: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The kernel parameter. Valid values:
         # 
         # *   **Normal**: the kernel parameters.
         # *   **MigrationFromRDS**: compares the current parameters with the parameters of the source RDS instance.
         self.describe_type = describe_type
         self.owner_account = owner_account
@@ -11650,23 +11841,31 @@
         dbcluster_id: str = None,
         end_time: str = None,
         interval: str = None,
         key: str = None,
         start_time: str = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.interval = interval
-        # The performance metrics that you want to query. Separate multiple metrics with commas (,). For more information, see [Performance parameters](~~141787~~).
+        # The performance metrics that you want to query. Separate multiple metrics with commas (,). For more information, see [Performance parameters](https://help.aliyun.com/document_detail/141787.html).
         # 
         # >  You can specify a maximum of five performance metrics.
+        # 
+        # This parameter is required.
         self.key = key
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11979,15 +12178,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -12180,14 +12381,16 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the serverless cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -12235,14 +12438,17 @@
         scale_ap_ro_num_max: str = None,
         scale_ap_ro_num_min: str = None,
         scale_max: str = None,
         scale_min: str = None,
         scale_ro_num_max: str = None,
         scale_ro_num_min: str = None,
         seconds_until_auto_pause: str = None,
+        serverless_rule_cpu_enlarge_threshold: str = None,
+        serverless_rule_cpu_shrink_threshold: str = None,
+        serverless_rule_mode: str = None,
         switchs: str = None,
     ):
         # Indicates whether the no-activity suspension feature is enabled. Default value: false. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.allow_shut_down = allow_shut_down
@@ -12258,14 +12464,17 @@
         self.scale_min = scale_min
         # The maximum number of read-only nodes for scaling. Valid values: 0 to 15.
         self.scale_ro_num_max = scale_ro_num_max
         # The minimum number of read-only nodes for scaling. Valid values: 0 to 15.
         self.scale_ro_num_min = scale_ro_num_min
         # The detection period for no-activity suspension. Valid values: 300 to 86400. Unit: seconds. The value must be a multiple of 300.
         self.seconds_until_auto_pause = seconds_until_auto_pause
+        self.serverless_rule_cpu_enlarge_threshold = serverless_rule_cpu_enlarge_threshold
+        self.serverless_rule_cpu_shrink_threshold = serverless_rule_cpu_shrink_threshold
+        self.serverless_rule_mode = serverless_rule_mode
         self.switchs = switchs
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12289,14 +12498,20 @@
             result['ScaleMin'] = self.scale_min
         if self.scale_ro_num_max is not None:
             result['ScaleRoNumMax'] = self.scale_ro_num_max
         if self.scale_ro_num_min is not None:
             result['ScaleRoNumMin'] = self.scale_ro_num_min
         if self.seconds_until_auto_pause is not None:
             result['SecondsUntilAutoPause'] = self.seconds_until_auto_pause
+        if self.serverless_rule_cpu_enlarge_threshold is not None:
+            result['ServerlessRuleCpuEnlargeThreshold'] = self.serverless_rule_cpu_enlarge_threshold
+        if self.serverless_rule_cpu_shrink_threshold is not None:
+            result['ServerlessRuleCpuShrinkThreshold'] = self.serverless_rule_cpu_shrink_threshold
+        if self.serverless_rule_mode is not None:
+            result['ServerlessRuleMode'] = self.serverless_rule_mode
         if self.switchs is not None:
             result['Switchs'] = self.switchs
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AllowShutDown') is not None:
@@ -12315,14 +12530,20 @@
             self.scale_min = m.get('ScaleMin')
         if m.get('ScaleRoNumMax') is not None:
             self.scale_ro_num_max = m.get('ScaleRoNumMax')
         if m.get('ScaleRoNumMin') is not None:
             self.scale_ro_num_min = m.get('ScaleRoNumMin')
         if m.get('SecondsUntilAutoPause') is not None:
             self.seconds_until_auto_pause = m.get('SecondsUntilAutoPause')
+        if m.get('ServerlessRuleCpuEnlargeThreshold') is not None:
+            self.serverless_rule_cpu_enlarge_threshold = m.get('ServerlessRuleCpuEnlargeThreshold')
+        if m.get('ServerlessRuleCpuShrinkThreshold') is not None:
+            self.serverless_rule_cpu_shrink_threshold = m.get('ServerlessRuleCpuShrinkThreshold')
+        if m.get('ServerlessRuleMode') is not None:
+            self.serverless_rule_mode = m.get('ServerlessRuleMode')
         if m.get('Switchs') is not None:
             self.switchs = m.get('Switchs')
         return self
 
 
 class DescribeDBClusterServerlessConfResponse(TeaModel):
     def __init__(
@@ -12371,14 +12592,16 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -12534,14 +12757,16 @@
         describe_type: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specify to return the latest version information or a list of upgradeable versions.Valid values:
         # 
         # - AVAILABLE_VERSION
         # - LATEST_VERSION
         self.describe_type = describe_type
         self.owner_account = owner_account
@@ -12683,15 +12908,15 @@
         self.dbversion = dbversion
         # The status of the minor version. Valid values:
         # 
         # *   **Stable**: The minor version is stable.
         # *   **Old**: The minor version is outdated. We recommend that you upgrade the cluster to the latest version.
         # *   **HighRisk**: The minor version has critical defects. We recommend that you immediately update the cluster to the latest minor version.
         # 
-        # >  For more information about how to update the minor version, see [Minor version update](~~158572~~).
+        # >  For more information about how to update the minor version, see [Minor version update](https://help.aliyun.com/document_detail/158572.html).
         self.dbversion_status = dbversion_status
         # Indicates whether the kernel is of the latest version. Valid values:
         # 
         # - true
         # - false
         self.is_latest_version = is_latest_version
         # Indicates whether PolarProxy uses the latest version. Valid values:
@@ -12896,15 +13121,15 @@
     ):
         # The endpoint of the cluster.
         self.connection_string = connection_string
         # The description of the cluster. Fuzzy match is supported.
         self.dbcluster_description = dbcluster_description
         # The ID of the cluster. Separate multiple cluster IDs with commas (,).
         self.dbcluster_ids = dbcluster_ids
-        # The state of the cluster that you want to query. For information about valid values, see [Cluster states](~~99286~~).
+        # The state of the cluster that you want to query. For information about valid values, see [Cluster states](https://help.aliyun.com/document_detail/99286.html).
         self.dbcluster_status = dbcluster_status
         # The ID of the node. You can specify multiple node IDs. Separate multiple node IDs with commas (,).
         self.dbnode_ids = dbnode_ids
         # The database engine that the cluster runs. Valid values:
         # 
         # *   **MySQL**\
         # *   **PostgreSQL**\
@@ -12936,15 +13161,17 @@
         self.pay_type = pay_type
         # Filters clusters created in the last N days. Valid values: 0 to 15.
         self.recent_creation_interval = recent_creation_interval
         # Filters clusters that expire after N days. Valid values: 0 to 15.
         self.recent_expiration_interval = recent_expiration_interval
         # The region ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query the available regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The tags of the cluster.
         self.tag = tag
@@ -13731,15 +13958,17 @@
         # *   **50**\
         # *   **100**\
         # 
         # Default value: 30.
         self.page_size = page_size
         # The region ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query information about regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query information about regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -14134,15 +14363,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -14374,15 +14605,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster for which you want to query the database links.
         # 
-        # > You can call the [DescribeDBClusters](~~173433~~) operation to query PolarDB clusters.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/173433.html) operation to query PolarDB clusters.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database link. If you leave this parameter empty, the system returns all the database links.
         self.dblink_name = dblink_name
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -14593,23 +14826,31 @@
         key: str = None,
         start_time: str = None,
         type: str = None,
     ):
         # The cluster ID.
         self.dbcluster_id = dbcluster_id
         # The ID of the cluster node.
+        # 
+        # This parameter is required.
         self.dbnode_id = dbnode_id
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.interval = interval
-        # The performance metrics that you want to query. Separate multiple metrics with commas (,). For more information, see [Performance parameters](~~141787~~).
+        # The performance metrics that you want to query. Separate multiple metrics with commas (,). For more information, see [Performance parameters](https://help.aliyun.com/document_detail/141787.html).
         # 
         # >  You can specify a maximum of five performance metrics.
+        # 
+        # This parameter is required.
         self.key = key
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -14922,16 +15163,20 @@
         dbnode_ids: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The node ID. You can specify multiple node IDs. Separate multiple node IDs with commas (,).
+        # 
+        # This parameter is required.
         self.dbnode_ids = dbnode_ids
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -15255,23 +15500,31 @@
         end_time: str = None,
         interval: str = None,
         key: str = None,
         start_time: str = None,
         type: str = None,
     ):
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the endpoint.
         self.dbendpoint_id = dbendpoint_id
         # The end of the time range to query. Specify the time in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.interval = interval
-        # The performance metrics that you want to query. Separate multiple indicators with commas (,). For more information, see [Performance parameters](~~141787~~).
+        # The performance metrics that you want to query. Separate multiple indicators with commas (,). For more information, see [Performance parameters](https://help.aliyun.com/document_detail/141787.html).
+        # 
+        # This parameter is required.
         self.key = key
         # The beginning of the time range to query. Specify the time in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -15589,14 +15842,15 @@
         self,
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -15725,14 +15979,16 @@
         owner_id: int = None,
         page_number: int = None,
         page_size: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database.
         # 
         # > You cannot specify multiple database names.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
@@ -15908,15 +16164,15 @@
         engine: str = None,
         master_id: str = None,
     ):
         # Details about the accounts.
         # 
         # > A PolarDB for MySQL cluster does not support privileged accounts.
         self.accounts = accounts
-        # The character set that the database uses. For more information, see [Character set tables](~~99716~~).
+        # The character set that the database uses. For more information, see [Character set tables](https://help.aliyun.com/document_detail/99716.html).
         self.character_set_name = character_set_name
         # The description of the database.
         self.dbdescription = dbdescription
         # The name of the database.
         self.dbname = dbname
         # The state of the database. Valid values:
         # 
@@ -16136,16 +16392,20 @@
         self.backup_region = backup_region
         # The status of the backup set. Valid values:
         # 
         # *   **Success**\
         # *   **Failed**\
         self.backup_status = backup_status
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The end of the time range to query. Specify the time in the `YYYY-MM-DDThh:mmZ` format. The time must be in UTC. The end time must be later than the start time.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The page number. The value must be a positive integer that does not exceed the maximum value of the INTEGER data type. Default value: **1**.
         self.page_number = page_number
         # The number of entries per page. Valid values:
         # 
@@ -16154,14 +16414,16 @@
         # *   **100**\
         # 
         # Default value: **30**.
         self.page_size = page_size
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The beginning of the time range to query. Specify the time in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16499,14 +16761,16 @@
         owner_id: int = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the GDN.
+        # 
+        # This parameter is required.
         self.gdnid = gdnid
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -16718,15 +16982,15 @@
         serverless_type: str = None,
         storage_used: str = None,
     ):
         # The description of the cluster.
         self.dbcluster_description = dbcluster_description
         # The ID of the cluster in the GDN.
         self.dbcluster_id = dbcluster_id
-        # The status of the cluster in the GDN. For more information, see [Cluster status table](~~99286~~).
+        # The status of the cluster in the GDN. For more information, see [Cluster status table](https://help.aliyun.com/document_detail/99286.html).
         self.dbcluster_status = dbcluster_status
         # The specifications of the node in the cluster.
         self.dbnode_class = dbnode_class
         # The details of the node.
         self.dbnodes = dbnodes
         # The type of the database engine. Only MySQL is supported.
         self.dbtype = dbtype
@@ -16874,15 +17138,15 @@
         self.dbtype = dbtype
         # The version of the database engine. Only version 8.0 is supported.
         self.dbversion = dbversion
         # The description of the GDN. The description must meet the following requirements:
         # 
         # *   It cannot start with `http://` or `https://`.
         # *   It must start with a letter.
-        # *   It can contain letters, digits, underscores (\_), and hyphens (-).
+        # *   It can contain letters, digits, underscores (_), and hyphens (-).
         # *   It must be 2 to 126 characters in length.
         self.gdndescription = gdndescription
         # The ID of the GDN.
         self.gdnid = gdnid
         # The status of the GDN. Valid values:
         # 
         # *   **Creating**: The GDN is being created.
@@ -17028,23 +17292,23 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
         self.dbcluster_id = dbcluster_id
         # Specify the region in which you want to query GDNs. You can create secondary clusters for the GDNs.
         self.filter_region = filter_region
         # The description of the GDN. The description must meet the following requirements:
         # 
         # *   It cannot start with `http://` or `https://`.
         # *   It must start with a letter.
-        # *   It can contain letters, digits, underscores (\_), and hyphens (-).
+        # *   It can contain letters, digits, underscores (_), and hyphens (-).
         # *   It must be 2 to 126 characters in length.
         self.gdndescription = gdndescription
         # The ID of the GDN.
         self.gdnid = gdnid
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The page number. Default value: 1. The value must be an integer that is greater than 0.
@@ -17137,15 +17401,15 @@
         # The region ID of the cluster.
         self.region_id = region_id
         # The role of the cluster. Valid values:
         # 
         # *   **Primary**: the primary cluster
         # *   **standby**: the secondary cluster
         # 
-        # > A GDN consists of one primary cluster and up to four secondary clusters. For more information, see [GDN](~~160381~~).
+        # > A GDN consists of one primary cluster and up to four secondary clusters. For more information, see [GDN](https://help.aliyun.com/document_detail/160381.html).
         self.role = role
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17191,15 +17455,15 @@
         self.dbtype = dbtype
         # The version of the database engine. Only the **8.0** version is supported.
         self.dbversion = dbversion
         # The description of the GDN. The description must meet the following requirements:
         # 
         # *   It cannot start with `http://` or `https://`.
         # *   It must start with a letter.
-        # *   It can contain letters, digits, underscores (\_), and hyphens (-).
+        # *   It can contain letters, digits, underscores (_), and hyphens (-).
         # *   It must be 2 to 126 characters in length.
         self.gdndescription = gdndescription
         # The ID of the GDN.
         self.gdnid = gdnid
         # The status of the GDN. Valid values:
         # 
         # *   **Creating**: The GDN is being created.
@@ -17379,14 +17643,16 @@
         security_token: str = None,
     ):
         # The ID of the IP whitelist template.
         self.global_security_group_id = global_security_group_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the IP whitelist template.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -17451,15 +17717,15 @@
         self.dbinstances = dbinstances
         # The IP address in the global IP whitelist template.
         # 
         # >  Separate multiple IP addresses with commas (,). You can add up to 1,000 IP addresses or CIDR blocks to all IP whitelists.
         self.gip_list = gip_list
         # The name of the global IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or a digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the global IP whitelist template.
         self.global_security_group_id = global_security_group_id
         # The ID of the region.
         self.region_id = region_id
@@ -17593,18 +17859,22 @@
         region_id: str = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the IP whitelist template.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -17666,15 +17936,15 @@
     ):
         # The IP address in the global IP whitelist template.
         # 
         # >  Separate multiple IP addresses with commas (,). You can add up to 1,000 IP addresses or CIDR blocks to all IP whitelists.
         self.gip_list = gip_list
         # The name of the global IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or a digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the global IP whitelist template.
         self.global_security_group_id = global_security_group_id
         # The ID of the region.
         self.region_id = region_id
@@ -17809,15 +18079,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to query all the information about the available clusters in the target region, including the cluster ID.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query all the information about the available clusters in the target region, including the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -17866,28 +18138,28 @@
         request_id: str = None,
     ):
         # Indicates whether the log backup feature is enabled. Valid values:
         # 
         # *   0: The log backup feature is disabled.
         # *   1: The log backup feature is enabled. By default, the log backup feature is enabled and cannot be disabled.
         self.enable_backup_log = enable_backup_log
-        # The region in which you want to store cross-region log backups. For more information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # The region in which you want to store cross-region log backups. For more information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.log_backup_another_region_region = log_backup_another_region_region
         # The retention period of cross-region log backups. Valid values:
         # 
         # *   **0**: The cross-region backup feature is disabled.
         # *   **30 to 7300**: Cross-region log backups are retained for 30 to 7,300 days.
         # *   **-1**: The log backups are permanently retained.
         # 
         # >  When you create a cluster, the default value of this parameter is **0**.
         self.log_backup_another_region_retention_period = log_backup_another_region_retention_period
         # The retention period of the log backups. Valid values:
         # 
         # *   3 to 7300: The log backups are retained for 3 to 7,300 days.
-        # *   \-1: The log backups are permanently retained.
+        # *   \\-1: The log backups are permanently retained.
         self.log_backup_retention_period = log_backup_retention_period
         # The request ID.
         self.request_id = request_id
 
     def validate(self):
         pass
 
@@ -17969,15 +18241,17 @@
     def __init__(
         self,
         dbcluster_id: str = None,
         rule_name_list: str = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the masking rule.
         self.rule_name_list = rule_name_list
 
     def validate(self):
         pass
 
@@ -18155,19 +18429,21 @@
         resource_owner_id: int = None,
         restore_time: str = None,
         security_token: str = None,
     ):
         # The ID of the data backup file.
         # 
         # >*   When you run a query, you must specify the `BackId` or `RestoreTime` parameter.
-        # >*   You can call the [DescribeBackups](~~98102~~) operation to query the ID of the backup set.
+        # >*   You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the ID of the backup set.
         self.backup_id = backup_id
         # The ID of the cluster.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to query the details of all clusters under your account.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of all clusters under your account.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specify the specific database name (such as `test_db`) to query the names of all data tables that can be restored in the desired database.
         # 
         # >*   You can specify only one database name each time.
         # >*   If you do not specify this parameter, you can query the names of all databases that can be restored in the current backup set. However, you cannot query the names of data tables in each database.
         self.get_db_name = get_db_name
         self.owner_account = owner_account
@@ -18180,21 +18456,21 @@
         # 
         # *   **50**\
         # 
         # *   **100**\
         # 
         #     Default value: **30**.
         self.page_size = page_size
-        # The ID of the region in which the instance resides. You can call the [DescribeDBClusterAttribute](~~2319132~~) operation to query the region ID of the instance.
+        # The ID of the region in which the instance resides. You can call the [DescribeDBClusterAttribute](https://help.aliyun.com/document_detail/2319132.html) operation to query the region ID of the instance.
         self.region_code = region_code
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The point in time for the restoration. Specify the time in the YYYY-MM-DDThh:mmZ format. The time must be in UTC.
         # 
-        # >  When you run a query, you must specify the `BackId` or `RestoreTime` parameter. You can call the [DescribeBackups](~~98102~~) operation to query the point in time for the restoration.
+        # >  When you run a query, you must specify the `BackId` or `RestoreTime` parameter. You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the point in time for the restoration.
         self.restore_time = restore_time
         self.security_token = security_token
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -18423,19 +18699,23 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the parameter template.
         # 
-        # > You can call the [DescribeParameterGroups](~~207178~~) operation to query the details of all parameter templates of a specified region, such as the ID of a parameter template.
+        # > You can call the [DescribeParameterGroups](https://help.aliyun.com/document_detail/207178.html) operation to query the details of all parameter templates of a specified region, such as the ID of a parameter template.
+        # 
+        # This parameter is required.
         self.parameter_group_id = parameter_group_id
         # The region ID.
         # 
-        # >You can call the [DescribeRegions](~~98041~~) operation to query all regions that are available within your account, such as the region ID.
+        # >You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query all regions that are available within your account, such as the region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -18727,15 +19007,17 @@
         # *   **5.7**\
         # *   **8.0**\
         self.dbversion = dbversion
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query all regions that are available for your account, such as the region ID.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query all regions that are available for your account, such as the region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group to which the virtual node belongs.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -18970,26 +19252,32 @@
         owner_id: int = None,
         region_id: str = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The type of the database engine. Only **MySQL** is supported.
+        # 
+        # This parameter is required.
         self.dbtype = dbtype
         # The version of the database. Valid values:
         # 
         # *   **5.6**\
         # *   **5.7**\
         # *   **8.0**\
+        # 
+        # This parameter is required.
         self.dbversion = dbversion
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID.
         # 
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query all regions that are available within your account, such as the region IDs.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query all regions that are available within your account, such as the region IDs.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -19293,17 +19581,19 @@
         self.owner_id = owner_id
         # The page number. The value of this parameter must be an integer that is greater than 0. Default value: **1**.
         self.page_number = page_number
         # The number of entries per page. Valid values: **30**, **50**, or **100**.
         # 
         # Default value: **30**.
         self.page_size = page_size
-        # The region ID of the pending event. You can call the [DescribeRegions](~~98041~~) operation to query the regions and zones that are supported by PolarDB.
+        # The region ID of the pending event. You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the regions and zones that are supported by PolarDB.
         # >- You can set this parameter to **all** to view all pending events within your account.
         # >- If you set `Region` to **all**, you must set `TaskType` to **all**.
+        # 
+        # This parameter is required.
         self.region = region
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
         # The task type of pending events. Valid values:
@@ -19311,14 +19601,16 @@
         # *   **DatabaseSoftwareUpgrading**: database software upgrades
         # *   **DatabaseHardwareMaintenance**: hardware maintenance and upgrades
         # *   **DatabaseStorageUpgrading**: database storage upgrades
         # *   **DatabaseProxyUpgrading**: minor version upgrades of the proxy
         # *   **all**: queries the details of the pending events of all preceding types.
         # 
         # > If the `Region` parameter is set to **all**, the `TaskType` parameter must be set to **all**.
+        # 
+        # This parameter is required.
         self.task_type = task_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19653,14 +19945,16 @@
         # *   **1**: returns the historical tasks.
         # 
         # Default value: **0**.
         self.is_history = is_history
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the region.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -19843,15 +20137,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of all the clusters for your account, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of all the clusters for your account, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -20262,15 +20558,15 @@
     ):
         # The description of the cluster.
         self.dbcluster_description = dbcluster_description
         # The cluster ID.
         # 
         # > 
         # 
-        # *   You can call the [DescribeDBClusters](~~98094~~) operation to query the information of all PolarDB clusters that are deployed in a specific region, such as the cluster IDs.
+        # *   You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the information of all PolarDB clusters that are deployed in a specific region, such as the cluster IDs.
         # 
         # *   If you do not specify this parameter, all scheduled tasks on your clusters are queried.
         self.dbcluster_id = dbcluster_id
         # The ID of the order.
         # 
         # >  The order ID can contain only digits.
         self.order_id = order_id
@@ -20284,15 +20580,15 @@
         self.planned_end_time = planned_end_time
         # The earliest start time of the task that you specified when you created the scheduled task. The time is displayed in UTC.
         self.planned_start_time = planned_start_time
         # The ID of the region.
         # 
         # > 
         # 
-        # *   You can call the [DescribeRegions](~~98041~~) operation to query the region information of all clusters in a specific account.
+        # *   You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the region information of all clusters in a specific account.
         # 
         # *   If you do not specify this parameter, scheduled tasks on your clusters that are deployed in all regions are queried.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -20673,21 +20969,25 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         sqlhash: str = None,
         start_time: str = None,
     ):
         # The ID of cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database.
         self.dbname = dbname
         # The end of the time range to query. The end time must be later than the start time. The interval between the start time and end time must be within 24 hours. Specify the time in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
         # 
         # > This parameter must be set to a time value in UTC (UTC+0 time zone). If your service resides in another time zone, convert the time value. For example, if the local time in the time zone where your service resides is 12:00 (UTC +8) and you want to query slow query logs at 08:00 (UTC +8) to 12:00, set this parameter to a time value that ranges from 00:00, set this parameter to 04:00.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The number of the page to return. The value must be an integer that is larger than 0.
         # 
         # Default value: **1**.
         self.page_number = page_number
@@ -20697,27 +20997,31 @@
         # *   **50**\
         # *   **100**\
         # 
         # Default value: **30**.
         self.page_size = page_size
         # The region ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query all regions that are available for your account, such as the region ID.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query all regions that are available for your account, such as the region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The unique ID of the SQL statement. The ID is used to obtain the slow query logs of the SQL statement.
         self.sqlhash = sqlhash
         # The beginning of the time range to query. Specify the time in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
         # 
         # > 
         # 
         # *   You can specify a time range of up to 30 days.
         # 
         # *   This parameter must be set to a time value in UTC (UTC+0 time zone). If your service resides in another time zone, convert the time value. For example, if the local time in the time zone where your service resides is 12:00 (UTC +8) and you want to query slow query logs at 08:00 (UTC +8) to 12:00, set this parameter to a time value that ranges from 00:00, set this parameter to 04:00.
+        # 
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21031,32 +21335,40 @@
         page_size: int = None,
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         start_time: str = None,
     ):
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the database.
         self.dbname = dbname
         # The end of the time range to query. The end time must be later than the start time. The time span between the start time and the end time cannot exceed 31 days. Specify the time in the yyyy-MM-ddZ format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The number of the page to return. Valid values: any non-zero positive integer.
         # 
         # Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values: 30 to 100. Default value: 30.
         self.page_size = page_size
         # The region ID of the cluster.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The beginning of the time range to query. Specify the time in the yyyy-MM-ddZ format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21409,35 +21721,39 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         start_time: str = None,
         status: str = None,
     ):
         # The cluster ID.
         # 
-        # >  You must specify `DBNodeId` or `DBClusterId`. You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # >  You must specify `DBNodeId` or `DBClusterId`. You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
         self.dbcluster_id = dbcluster_id
         # The node ID.
         # 
-        # >  You must specify `DBNodeId` or `DBClusterId`. You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as node IDs.
+        # >  You must specify `DBNodeId` or `DBClusterId`. You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as node IDs.
         self.dbnode_id = dbnode_id
         # The end of the time range to query. Specify the time in the ISO 8601 standard in the `YYYY-MM-DDThh:mmZ` format. The time must be in UTC. The end time must be later than the start time.
+        # 
+        # This parameter is required.
         self.end_time = end_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The page number of the page to return. The value is an integer that is greater than 0.
         # 
         # Default value: **1**.
         self.page_number = page_number
         # The number of entries to return per page. Valid values: **30**, **50**, and **100**.
         # 
         # Default value: **30**.
         self.page_size = page_size
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The beginning of the time range to query. Specify the time in the ISO 8601 standard in the `yyyy-MM-ddTHH:mmZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.start_time = start_time
         # The state of the tasks that you want to query. Valid values:
         # 
         # *   **Waiting**: The task is pending.
         # *   **Running**: The task is running.
         # *   **Finished**: The task is completed.
         # *   **Closed**: The task is closed.
@@ -21800,21 +22116,23 @@
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         tderegion: str = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the region.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query all regions that are available for your account, such as the region ID.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query all regions that are available for your account, such as the region ID.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The region where the TDE key resides.
         self.tderegion = tderegion
 
     def validate(self):
@@ -22242,14 +22560,16 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -22376,14 +22696,16 @@
         scale_ap_ro_num_min: str = None,
         scale_max: str = None,
         scale_min: str = None,
         scale_ro_num_max: str = None,
         scale_ro_num_min: str = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The maximum number of stable AP read-only nodes. Valid values: 0 to 7.
         self.scale_ap_ro_num_max = scale_ap_ro_num_max
@@ -22541,20 +22863,22 @@
         enable: bool = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         rule_name_list: str = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.enable = enable
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
+        # This parameter is required.
         self.rule_name_list = rule_name_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22700,23 +23024,27 @@
         # 
         # *   **lvs** :Linux virtual server
         # *   **proxy**: proxy server
         # *   **dns**: domain name system
         self.dbinstance_conn_type = dbinstance_conn_type
         # The specifications of the node. For information about node specifications, see the following topics:
         # 
-        # *   PolarDB for MySQL: [Specifications of compute nodes](~~102542~~)
-        # *   PolarDB for Oracle: [Specifications of compute nodes](~~207921~~)
-        # *   PolarDB for PostgreSQL: [Specifications of compute nodes](~~209380~~)
+        # *   PolarDB for MySQL: [Specifications of compute nodes](https://help.aliyun.com/document_detail/102542.html)
+        # *   PolarDB for Oracle: [Specifications of compute nodes](https://help.aliyun.com/document_detail/207921.html)
+        # *   PolarDB for PostgreSQL: [Specifications of compute nodes](https://help.aliyun.com/document_detail/209380.html)
+        # 
+        # This parameter is required.
         self.dbnode_class = dbnode_class
         # The type of the database engine. Valid values:
         # 
         # *   **MySQL**\
         # *   **PostgreSQL**\
         # *   **Oracle**\
+        # 
+        # This parameter is required.
         self.dbtype = dbtype
         # The version of the database engine
         # 
         # *   Valid values for the MySQL database engine:
         # 
         #     *   **5.6**\
         #     *   **5.7**\
@@ -22724,40 +23052,48 @@
         # 
         # *   Valid values for the PostgreSQL database engine:
         # 
         #     *   **11**\
         #     *   **14**\
         # 
         # *   Valid value for the Oracle database engine: **11**\
+        # 
+        # This parameter is required.
         self.dbversion = dbversion
         # Specifies whether to return the zones in which the single-zone deployment method is supported. Default value: 0. Valid values:
         # 
         # *   **0**: no value returned
         # *   **1**: returns the zones.
         self.dispense_mode = dispense_mode
         # Specifies whether Maxscale is created. Default value: true. Valid values:
         # 
         # *   **true**\
         # *   **false**\
+        # 
+        # This parameter is required.
         self.need_max_scale_link = need_max_scale_link
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The subdomain. It is the child domain of the top-level domain name or parent domain. For example, if the parent domain name is cn-beijing, its child domain can be cn-beijing-i-aliyun.
         self.sub_domain = sub_domain
         # The zone ID.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available zones.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available zones.
+        # 
+        # This parameter is required.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22949,21 +23285,23 @@
         resource_owner_id: int = None,
         roll_back_for_disaster: bool = None,
         target_dbnode_id: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.roll_back_for_disaster = roll_back_for_disaster
-        # The ID of the read-only node that you want to promote to the primary node. You can call the [DescribeDBClusters](~~98094~~) operation to query node information, such as node IDs.
+        # The ID of the read-only node that you want to promote to the primary node. You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query node information, such as node IDs.
         # 
         # > *   If you leave this parameter empty, the system selects one or more available read-only nodes that have the highest failover priority as candidate primary nodes. If the failover to the first read-only node fails due to network issues, abnormal replication status, or other reasons, the system attempts to fail over your applications to the next read-only node until the failover is successful.
         # >*  This parameter is required for PolarDB for Oracle and PolarDB for PostgreSQL clusters. This parameter is optional for PolarDB for MySQL clusters.
         self.target_dbnode_id = target_dbnode_id
 
     def validate(self):
         pass
@@ -23091,28 +23429,36 @@
         dbname: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The username of the account.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The permissions that are granted to the account. Valid values:
         # 
         # *   **ReadWrite**: read and write permissions
         # *   **ReadOnly**: read-only permissions
         # *   **DMLOnly**: The account is granted the permissions to execute only DML statements on the database.
         # *   **DDLOnly**: The account is granted the permissions to execute only DDL statements on the database.
         # *   **ReadIndex**: The account has the read and index permissions on the database.
         # 
-        # > The number of **AccountPrivilege** values must be the consistent with the number of **DBName** values. Each account permission must correspond to a database name in sequence. For example, you can set **DBName** to `testdb_1,testdb_2` and set **AccountPrivilege** to `ReadWrite,ReadOnly`. In this case, the specified standard account is granted the **read and write** permissions on the **testdb\_1** database and the **read** permission on the **testdb\_2** database.
+        # > The number of **AccountPrivilege** values must be the consistent with the number of **DBName** values. Each account permission must correspond to a database name in sequence. For example, you can set **DBName** to `testdb_1,testdb_2` and set **AccountPrivilege** to `ReadWrite,ReadOnly`. In this case, the specified standard account is granted the **read and write** permissions on the **testdb_1** database and the **read** permission on the **testdb_2** database.
+        # 
+        # This parameter is required.
         self.account_privilege = account_privilege
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The names of the databases that the account can access. You can grant the access permissions on one or more databases to the specified standard account. If you need to specify multiple database names, separate the database names with commas (,).
+        # 
+        # This parameter is required.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -23286,27 +23632,31 @@
         resource_type: str = None,
         tag: List[ListTagResourcesRequestTag] = None,
     ):
         # The token required to obtain more results. This parameter is not required in the first query. If the first query does not return all results, you can use the token that is returned from the first query in the next query to obtain more results.
         self.next_token = next_token
         self.owner_account = owner_account
         self.owner_id = owner_id
-        # The ID of the region. You can call the [DescribeRegions](~~98041~~) operation to query available region IDs.
+        # The ID of the region. You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available region IDs.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The cluster ID. To query the tags of multiple clusters, click **Add** to add cluster IDs.
         # 
         # > 
         # 
         # *   You must specify at least one of the `ResourceId.N` and `Tag.N.Key` parameters.
         # 
         # *   If you specify the `ResourceId.N` parameter, you can add a maximum of 50 cluster IDs at a time.
         self.resource_id = resource_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The type of the resource. Set the value to **cluster**.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
         # The tags.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
@@ -23543,20 +23893,22 @@
         owner_account: str = None,
         owner_id: int = None,
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available regions.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available regions.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -23677,18 +24029,24 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The description of the account. The description must meet the following requirements:
         # 
         # *   The description cannot start with `http://` or `https://`.
         # *   The description must be 2 to 256 characters in length.
+        # 
+        # This parameter is required.
         self.account_description = account_description
         # The name of the account.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -23813,22 +24171,28 @@
         owner_account: str = None,
         owner_id: int = None,
         password_type: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The username of the account.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The new password of the account. The new password must meet the following requirements:
         # 
         # *   It must contain at least three of the following character types: uppercase letters, lowercase letters, digits, and special characters.
         # *   It must be 8 to 32 characters in length.
         # *   Special characters include `! @ # $ % ^ & * ( ) _ + - =`
+        # 
+        # This parameter is required.
         self.new_account_password = new_account_password
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.password_type = password_type
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
@@ -23960,14 +24324,16 @@
         region_id: str = None,
         renewal_status: str = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID. If you need to specify multiple cluster IDs, separate the cluster IDs with commas (,).
+        # 
+        # This parameter is required.
         self.dbcluster_ids = dbcluster_ids
         # The automatic renewal period.
         # 
         #  
         # *   Valid values when **PeriodUnit** is set to **Month**: `1, 2, 3, 6, and 12`.
         # *   Valid values when **PeriodUnit** is set to **Year**: `1, 2, and 3`.
         #  
@@ -23981,15 +24347,17 @@
         # *   **Month**\
         #  
         # Default value: **Month**.
         self.period_unit = period_unit
         # The ID of the region. The region ID can be up to 50 characters in length.
         # cn-hangzhou
         #  
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query the available regions.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The auto-renewal state of the cluster. Valid values:
         #  
         # *   **AutoRenewal:** The cluster are automatically renewed.
         # *   **Normal**: The cluster is manually renewed.
         # *   **NotRenewal:** The cluster is not renewed after expiration.
         #  
@@ -24153,59 +24521,61 @@
         # *   **Normal**: standard backup. The system backs up data once a day.
         # *   **2/24H**: enhanced backup. The system backs up data every 2 hours.
         # *   **3/24H**: enhanced backup. The system backs up data every 3 hours.
         # *   **4/24H**: enhanced backup. The system backs up data every 4 hours.
         # 
         # >- If you enable enhanced backup, all backups are retained for 24 hours. For backup files that are created earlier than the previous 24 hours, the system permanently retains only the first backup that is created after 00:00 every day and deletes the rest.
         # >- If you enable enhanced backup, **PreferredBackupPeriod** is automatically set to all days in a week (from Monday to Sunday).
-        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed supports the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed supports the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.backup_frequency = backup_frequency
         # Specifies whether to retain backups when you delete a cluster. Valid values:
         # 
         # *   **ALL**: permanently retains all backups.
         # *   **LATEST**: permanently retains only the last backup.
         # *   **NONE**: does not retain backups.
         # 
         # > The default value is NONE.
         self.backup_retention_policy_on_cluster_deletion = backup_retention_policy_on_cluster_deletion
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The frequency of level-1 backups. Default value: Normal. Valid values:
         # 
         # *   **Normal**: standard backup. The system backs up data once a day.
         # *   **2/24H**: enhanced backup. The system backs up data every 2 hours.
         # *   **3/24H**: enhanced backup. The system backs up data every 3 hours.
         # *   **4/24H**: enhanced backup. The system backs up data every 4 hours.
         # 
         # >- This parameter is invalid for PolarDB for Oracle clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_1backup_frequency = data_level_1backup_frequency
         # The backup cycle of level-1 backups. Valid values:
         # 
         # *   **Monday**\
         # *   **Tuesday**\
         # *   **Wednesday**\
         # *   **Thursday**\
         # *   **Friday**\
         # *   **Saturday**\
         # *   **Sunday**\
         # 
         # >- You need to specify at least two values. Separate multiple values with commas (,).
         # >- This parameter is invalid for PolarDB for Oracle clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_1backup_period = data_level_1backup_period
         # The retention period of level-1 backups. Valid values: 3 to 14. Unit: days.
         self.data_level_1backup_retention_period = data_level_1backup_retention_period
         # The time period during which automatic backup for level-1 backup is performed. The time period is in the `hh:mmZ-hh:mmZ` format and is displayed in UTC. The start time and end time are on the hour and have an interval of 1 hour. Example: `14:00Z-15:00Z`.
         # >- This parameter is invalid for PolarDB for Oracle clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_1backup_time = data_level_1backup_time
-        # The region where the cross-region level-2 backup is stored. For information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # The region where the cross-region level-2 backup is stored. For information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_2backup_another_region_region = data_level_2backup_another_region_region
         # The retention period of cross-region level-2 backups. Valid values:
         # 
         # *   **0**: The cross-region level-2 backup feature is disabled.
         # *   **30 to 7300**: Cross-region level-2 backups are retained for 30 to 7,300 days.
         # *   **1**: Cross-region level-2 backups are permanently retained.
         # 
@@ -24219,15 +24589,15 @@
         # *   **Thursday**\
         # *   **Friday**\
         # *   **Saturday**\
         # *   **Sunday**\
         # 
         # >- You need to specify at least two values. Separate multiple values with commas (,).
         # >- This parameter is invalid for PolarDB for Oracle clusters or PolarDB for PostgreSQL clusters.
-        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed does not support the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.data_level_2backup_period = data_level_2backup_period
         # The retention period of level-2 backups. Valid values:
         # 
         # *   **0**: The level-2 backup feature is disabled.
         # *   **30 to 7300**: Cross-region level-2 backups are retained for 30 to 7,300 days.
         # *   **1**: Cross-region level-2 backups are permanently retained.
         # 
@@ -24242,15 +24612,15 @@
         # *   **Wednesday**\
         # *   **Thursday**\
         # *   **Friday**\
         # *   **Saturday**\
         # *   **Sunday**\
         # 
         # >- You need to specify at least two values. Separate multiple values with commas (,).
-        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed supports the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # >- This parameter is invalid if the region where your PolarDB for MySQL cluster is deployed supports the cross-region backup feature. For information about the regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.preferred_backup_period = preferred_backup_period
         # The time period during which automatic backup for level-1 backup is performed. The format is `hh:mmZ-hh:mmZ` format. The time is displayed in UTC. The start time and end time are on the hour and with an interval of one hour. Example: `14:00Z-15:00Z`.
         self.preferred_backup_time = preferred_backup_time
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -24422,14 +24792,16 @@
         storage_upper_bound: int = None,
     ):
         # Enable storage compression function. The value of this parameter is ON.
         self.compress_storage = compress_storage
         # The cluster ID.
         # 
         # >  You can call the DescribeDBClusters operation to query information about all PolarDB clusters that are deployed in a specified region, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The method used to replicate data across zones. Valid values:
         # 
         # *   **AsyncSync**: the asynchronous mode.
         # *   **SemiSync**: the semi-synchronous mode.
         self.data_sync_mode = data_sync_mode
         # The fault scenario that you want to simulate for the cluster.
@@ -24632,14 +25004,16 @@
         # > 
         # 
         # *   You can create a maximum of 50 IP whitelist groups for a cluster.
         # 
         # *   This parameter can be specified only when the **WhiteListType** parameter is set to **IP**.
         self.dbcluster_iparray_name = dbcluster_iparray_name
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The method used to modify the IP whitelist. Valid values:
         # 
         # *   **Cover** (default): overwrites the original IP whitelist.
         # *   **Append**: appends IP addresses to the original whitelist.
         # *   **Delete**: deletes IP addresses.
         # 
@@ -24810,14 +25184,16 @@
         parameters: str = None,
         planned_end_time: str = None,
         planned_start_time: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The node ID. You can set this parameter to modify the parameters of a specified node or of the cluster. Separate multiple node IDs with commas (,).
         # 
         # > If you do not specify this parameter, only the cluster parameters are modified.
         self.dbnode_ids = dbnode_ids
         # Specifies an immediate or scheduled task to modify parameters and restart the cluster. Default value: false. Valid values:
         # 
@@ -24988,16 +25364,20 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # Specifies whether to enable or disable SQL collector. Valid values:
         # 
         # *   Enable
         # *   Disable
+        # 
+        # This parameter is required.
         self.collector_status = collector_status
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -25117,15 +25497,17 @@
         owner_id: int = None,
         protection: bool = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to.obtain the cluster ID.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to.obtain the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # Specifies whether to enable the cluster lock feature. Default value: false. Valid values:
         # 
         # *   **true**: enables the cluster lock feature. If you enable the cluster lock feature, you cannot directly release the cluster. You must disable the cluster lock feature before you can release the cluster.
         # *   **false**: disables the cluster lock feature.
@@ -25252,16 +25634,20 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The name of the cluster. The name must meet the following requirements:
         # 
         # *   The name cannot start with `http://` or `https://`.
         # *   The name must be 2 to 256 characters in length.
+        # 
+        # This parameter is required.
         self.dbcluster_description = dbcluster_description
         # The ID of the PolarDB cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -25390,72 +25776,76 @@
     ):
         # Specifies whether to automatically associate newly added nodes with the cluster endpoint. Default value: Disable. Valid values:
         # 
         # *   **Enable**\
         # *   **Disable**\
         self.auto_add_new_nodes = auto_add_new_nodes
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The name of the custom cluster endpoint.
         self.dbendpoint_description = dbendpoint_description
         # The ID of the endpoint.
+        # 
+        # This parameter is required.
         self.dbendpoint_id = dbendpoint_id
         # The advanced configurations of the cluster endpoint, which are in the JSON format. You can specify the configurations of the following attributes: consistency level, transaction splitting, connection pool, and primary node accepts read requests.
         # 
-        # *   Specifies the load balancing policy in the format of `{\"LoadBalancePolicy\":\"Selected value\"}`. Default value: 0. Valid values:
+        # *   Specifies the load balancing policy in the format of `{\\"LoadBalancePolicy\\":\\"Selected value\\"}`. Default value: 0. Valid values:
         # 
         #     *   **0**: connections-based load balancing
         #     *   **1**: active requests-based load balancing
         # 
-        # *   Specifies whether to enable the primary node accepts read requests feature in the format of `{\"MasterAcceptReads\":\"Selected value\"}`. Default value: on. Valid values:
+        # *   Specifies whether to enable the primary node accepts read requests feature in the format of `{\\"MasterAcceptReads\\":\\"Selected value\\"}`. Default value: on. Valid values:
         # 
         #     *   **on**\
         #     *   **off**\
         # 
-        # *   Specifies whether to enable the transaction splitting feature in the format of `{\"DistributedTransaction\":\"Selected value\"}`. Default value: on. Valid values:
+        # *   Specifies whether to enable the transaction splitting feature in the format of `{\\"DistributedTransaction\\":\\"Selected value\\"}`. Default value: on. Valid values:
         # 
         #     *   **on**\
         #     *   **off**\
         # 
-        # *   Specifies the consistency level in the format of `{\"ConsistLevel\":\"Selected value\"}`. Default value: 1. Valid values:
+        # *   Specifies the consistency level in the format of `{\\"ConsistLevel\\":\\"Selected value\\"}`. Default value: 1. Valid values:
         # 
         #     *   **0**: eventual consistency (weak)
         #     *   **1**: session consistency (medium)
         #     *   **2**: global consistency (strong)
         # 
-        # *   Specifies the connection pool in the format of `{\"ConnectionPersist\":\"Selected value\"}`. Default value: off. Valid values:
+        # *   Specifies the connection pool in the format of `{\\"ConnectionPersist\\":\\"Selected value\\"}`. Default value: off. Valid values:
         # 
         #     *   **off**: disables the connection pool.
         #     *   **Session**: enables the session-level connection pool.
         #     *   **Transaction**: enables the transaction-level connection pool.
         # 
-        # *   Specifies whether to enable the parallel query feature in the format of `{\"MaxParallelDegree\":\"Selected value\"}`. Default value: off. Valid values:
+        # *   Specifies whether to enable the parallel query feature in the format of `{\\"MaxParallelDegree\\":\\"Selected value\\"}`. Default value: off. Valid values:
         # 
         #     *   **on**\
         #     *   **off**\
         # 
-        # *   Specifies whether to enable the automatic request distribution between row store and column store nodes feature in the format of `{\"EnableHtapImci\":\"Selected value\"}`. Default value: off. Valid values:
+        # *   Specifies whether to enable the automatic request distribution between row store and column store nodes feature in the format of `{\\"EnableHtapImci\\":\\"Selected value\\"}`. Default value: off. Valid values:
         # 
         #     *   **on**\
         #     *   **off**\
         # 
-        # *   Specifies whether to enable the overload protection feature in the format of `{\"EnableOverloadThrottle\":\"Selected value\"}`. Default value: off. Valid values:
+        # *   Specifies whether to enable the overload protection feature in the format of `{\\"EnableOverloadThrottle\\":\\"Selected value\\"}`. Default value: off. Valid values:
         # 
         #     *   **on**\
         #     *   **off**\
         # 
         # > 
         # 
         # *   You can specify the transaction splitting, primary node accepts read requests, connection pool, and overload protection features for a PolarDB for MySQL cluster only if ReadWriteMode is set to ReadWrite for the cluster endpoint.
         # 
         # *   If the read /write mode of a PolarDB for MySQL cluster is set to **Read-only**, the **Connection-based SLB** and **Active Request-based SLB** SLB policies are supported. The **Read-write (Automatic read /write splitting) **mode of the cluster supports** Active Request-based SLB** policy.
         # *   If ReadWriteMode is set to **ReadWrite** for the cluster endpoint of a PolarDB for MySQL cluster or if ReadWriteMode is set to **ReadOnly** and the load balancing policy is set to **active requests-based load balancing**, the automatic request distribution between row store and column store nodes feature is supported.
         # *   Only PolarDB for MySQL supports global consistency.
         # *   If the **ReadWriteMode** parameter is set to **ReadOnly**, the consistency level must be **0**.
-        # *   You can specify the consistency level, transaction splitting, connection pool, and primary node accepts read requests features at a time, such as `{\"ConsistLevel\":\"1\",\"DistributedTransaction\":\"on\",\"ConnectionPersist\":\"Session\",\"MasterAcceptReads\":\"on\"}`.
+        # *   You can specify the consistency level, transaction splitting, connection pool, and primary node accepts read requests features at a time, such as `{\\"ConsistLevel\\":\\"1\\",\\"DistributedTransaction\\":\\"on\\",\\"ConnectionPersist\\":\\"Session\\",\\"MasterAcceptReads\\":\\"on\\"}`.
         # *   The transaction splitting settings are restricted by the consistency level settings. For example, if you set the consistency level to **0**, transaction splitting cannot be enabled. If you set the consistency level to **1** or **2**, transaction splitting can be enabled.
         self.endpoint_config = endpoint_config
         # The reader nodes to be associated with the endpoint. If you need to specify multiple reader nodes, separate the reader nodes with commas (,). If you do not specify this parameter, the predefined nodes are used by default.
         # 
         # > 
         # 
         # *   You must specify the node ID for each PolarDB for MySQL cluster.
@@ -25615,18 +26005,22 @@
         maintain_time: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The maintenance window of the cluster. Specify the maintenance window in the `HH:mmZ-HH:mmZ` format. For example, the value `16:00Z-17:00Z` indicates that the cluster can be maintained from 00:00 to 01:00 (UTC+8).
         #  
         # >  The maintenance window must start on the hour and last for an hour.
+        # 
+        # This parameter is required.
         self.maintain_time = maintain_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -25753,26 +26147,32 @@
         swap_connection_string: str = None,
     ):
         # The endpoints to be switched. The endpoints are in the JSON format.
         # 
         # > This parameter is valid when the SwapConnectionString parameter is set to true.
         self.connection_strings = connection_strings
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the new instance or new cluster. Valid values:
         # 
         # *   To perform a data migration, enter the ID of the PolarDB cluster.
         # *   To perform a migration rollback, enter the ID of the ApsaraDB for RDS instance.
+        # 
+        # This parameter is required.
         self.new_master_instance_id = new_master_instance_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
         # The ID of the source ApsaraDB RDS instance.
+        # 
+        # This parameter is required.
         self.source_rdsdbinstance_id = source_rdsdbinstance_id
         # Specifies whether to switch the endpoints. Valid values:
         # 
         # *   **true**: switches the endpoints. If you select this option, you do not need the change the endpoint in your applications.
         # *   **false**: does not switch the endpoints. If you select this option, you must specify the endpoint of the PolarDB cluster in your applications.
         # 
         # Default value: **false**.
@@ -25910,18 +26310,22 @@
         owner_account: str = None,
         owner_id: int = None,
         period: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The interval at which monitoring data is collected. Valid values: **5** and **60**. Unit: seconds.
+        # 
+        # This parameter is required.
         self.period = period
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
         pass
 
@@ -26043,37 +26447,39 @@
         planned_end_time: str = None,
         planned_start_time: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specifies an immediate or scheduled task to modify parameters and restart the cluster. Valid values:
         # 
         # *   false: scheduled task
         # *   true: immediate task
         self.from_time_service = from_time_service
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the parameter template.
         # 
         # > 
         # 
-        # *   You can call the [DescribeParameterGroups](~~207178~~) operation to query the parameter template ID.
+        # *   You can call the [DescribeParameterGroups](https://help.aliyun.com/document_detail/207178.html) operation to query the parameter template ID.
         # 
         # *   You must specify this parameter or the `Parameters` parameter.
         # *   This parameter is valid only for a PolarDB for MySQL cluster.
         self.parameter_group_id = parameter_group_id
         # The JSON string that consists of parameters and values. The parameter values are strings, for example, `{"wait_timeout":"86","innodb_old_blocks_time":"10"}`.
         # 
         # > 
         # 
-        # *   You can call the [DescribeDBClusterParameters](~~98122~~) operation to query the parameters of the PolarDB cluster.
+        # *   You can call the [DescribeDBClusterParameters](https://help.aliyun.com/document_detail/98122.html) operation to query the parameters of the PolarDB cluster.
         # 
         # *   This parameter is required for a PolarDB for Oracle or PolarDB for PostgreSQL cluster.
         # *   For PolarDB for MySQL clusters, you must specify this parameter or the `ParameterGroupId` parameter.
         self.parameters = parameters
         # The latest start time to run the task. Specify the time in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
         # > 
@@ -26233,15 +26639,17 @@
         vpcid: str = None,
         v_switch_id: str = None,
         zone_id: str = None,
         zone_type: str = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~173433~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/173433.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specifies an immediate or scheduled task to switch the primary zone. Valid values:
         # 
         # *   false: scheduled task
         # *   true: immediate task
         self.from_time_service = from_time_service
         # Specifies whether to switch back over to the original primary zone. Valid values: true: Switch over back to the original primary zone. false: Do not switch back over to the original primary zone. If this parameter is set to false, the primary zone of the cluster is changed to the specified destination zone.
@@ -26274,15 +26682,17 @@
         # 
         # *   For a PolarDB for Oracle or PolarDB for PostgreSQL cluster, this parameter is required.
         # 
         # *   For a PolarDB for MySQL cluster: - This parameter is optional if no vSwitches have been created in the destination zone. The default vSwitch is used. - This parameter is required if a vSwitch has been created in the destination zone.
         self.v_switch_id = v_switch_id
         # The ID of the destination primary zone.
         # 
-        # > You can call the [DescribeRegions](~~98041~~) operation to query available zones.
+        # > You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query available zones.
+        # 
+        # This parameter is required.
         self.zone_id = zone_id
         self.zone_type = zone_type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -26426,15 +26836,17 @@
         new_resource_group_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
+        # This parameter is required.
         self.new_resource_group_id = new_resource_group_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
@@ -26560,23 +26972,25 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         sslauto_rotate: str = None,
         sslenabled: str = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the endpoint.
         # 
         # > 
         # 
         # *   This parameter is required for a PolarDB for MySQL cluster.
         # 
         # *   This parameter is not required for a PolarDB for Oracle or PolarDB for PostgreSQL cluster. By default, SSL encryption is enabled for all endpoints.
-        # *   You can call the [DescribeDBClusterSSL](~~153414~~) operation to view the details of the endpoint.
+        # *   You can call the [DescribeDBClusterSSL](https://help.aliyun.com/document_detail/153414.html) operation to view the details of the endpoint.
         self.dbendpoint_id = dbendpoint_id
         # The network type supported by the endpoint that is specified by **DBEndpointId**. Valid values:
         # 
         # *   **Public**\
         # *   **Private**\
         # *   **Inner**\
         # 
@@ -26597,15 +27011,15 @@
         self.sslauto_rotate = sslauto_rotate
         # The SSL encryption status. Valid values:
         # 
         # *   **Disable**: SSL encryption is disabled.
         # *   **Enable**: SSL encryption is enabled.
         # *   **Update**: The SSL certificate is updated.
         # 
-        # > After you enable SSL encryption or update the SSL certificate, you must download and configure the certificate. For more information, see [Configure SSL encryption](~~153182~~).
+        # > After you enable SSL encryption or update the SSL certificate, you must download and configure the certificate. For more information, see [Configure SSL encryption](https://help.aliyun.com/document_detail/153182.html).
         self.sslenabled = sslenabled
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26740,21 +27154,26 @@
         scale_ap_ro_num_max: str = None,
         scale_ap_ro_num_min: str = None,
         scale_max: str = None,
         scale_min: str = None,
         scale_ro_num_max: str = None,
         scale_ro_num_min: str = None,
         seconds_until_auto_pause: str = None,
+        serverless_rule_cpu_enlarge_threshold: str = None,
+        serverless_rule_cpu_shrink_threshold: str = None,
+        serverless_rule_mode: str = None,
     ):
         # Specifies whether to enable No-activity Suspension. Default value: false. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.allow_shut_down = allow_shut_down
         # The ID of the serverless cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specifies an immediate or scheduled task to modify parameters and restart the cluster. Valid values:
         # 
         # *   false: scheduled task
         # *   true: immediate task
         self.from_time_service = from_time_service
         self.owner_account = owner_account
@@ -26780,14 +27199,17 @@
         self.scale_min = scale_min
         # The maximum number of read-only nodes for scaling. Valid values: 0 to 15.
         self.scale_ro_num_max = scale_ro_num_max
         # The minimum number of read-only nodes for scaling. Valid values: 0 to 15.
         self.scale_ro_num_min = scale_ro_num_min
         # The detection period for No-activity Suspension. Valid values: 5 to 1440. Unit: minutes. The detection duration must be a multiple of 5 minutes.
         self.seconds_until_auto_pause = seconds_until_auto_pause
+        self.serverless_rule_cpu_enlarge_threshold = serverless_rule_cpu_enlarge_threshold
+        self.serverless_rule_cpu_shrink_threshold = serverless_rule_cpu_shrink_threshold
+        self.serverless_rule_mode = serverless_rule_mode
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -26822,14 +27244,20 @@
             result['ScaleMin'] = self.scale_min
         if self.scale_ro_num_max is not None:
             result['ScaleRoNumMax'] = self.scale_ro_num_max
         if self.scale_ro_num_min is not None:
             result['ScaleRoNumMin'] = self.scale_ro_num_min
         if self.seconds_until_auto_pause is not None:
             result['SecondsUntilAutoPause'] = self.seconds_until_auto_pause
+        if self.serverless_rule_cpu_enlarge_threshold is not None:
+            result['ServerlessRuleCpuEnlargeThreshold'] = self.serverless_rule_cpu_enlarge_threshold
+        if self.serverless_rule_cpu_shrink_threshold is not None:
+            result['ServerlessRuleCpuShrinkThreshold'] = self.serverless_rule_cpu_shrink_threshold
+        if self.serverless_rule_mode is not None:
+            result['ServerlessRuleMode'] = self.serverless_rule_mode
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AllowShutDown') is not None:
             self.allow_shut_down = m.get('AllowShutDown')
         if m.get('DBClusterId') is not None:
@@ -26858,14 +27286,20 @@
             self.scale_min = m.get('ScaleMin')
         if m.get('ScaleRoNumMax') is not None:
             self.scale_ro_num_max = m.get('ScaleRoNumMax')
         if m.get('ScaleRoNumMin') is not None:
             self.scale_ro_num_min = m.get('ScaleRoNumMin')
         if m.get('SecondsUntilAutoPause') is not None:
             self.seconds_until_auto_pause = m.get('SecondsUntilAutoPause')
+        if m.get('ServerlessRuleCpuEnlargeThreshold') is not None:
+            self.serverless_rule_cpu_enlarge_threshold = m.get('ServerlessRuleCpuEnlargeThreshold')
+        if m.get('ServerlessRuleCpuShrinkThreshold') is not None:
+            self.serverless_rule_cpu_shrink_threshold = m.get('ServerlessRuleCpuShrinkThreshold')
+        if m.get('ServerlessRuleMode') is not None:
+            self.serverless_rule_mode = m.get('ServerlessRuleMode')
         return self
 
 
 class ModifyDBClusterServerlessConfResponseBody(TeaModel):
     def __init__(
         self,
         dbcluster_id: str = None,
@@ -26954,14 +27388,16 @@
         resource_owner_id: int = None,
         storage_space: int = None,
         sub_category: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The token can only contain ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The latest time to upgrade the specifications within the scheduled time period. Specify the time in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # >- The value of this parameter must be at least 30 minutes later than PlannedStartTime.
         # >- By default, if you specify `PlannedStartTime` but do not specify PlannedEndTime, the latest start time of the task is set to `PlannedEndTime + 30 minutes`. For example, if you set `PlannedStartTime` to `2021-01-14T09:00:00Z` and you do not specify PlannedEndTime, the latest start time of the task is `2021-01-14T09:30:00Z`.
         self.planned_end_time = planned_end_time
@@ -26971,14 +27407,16 @@
         # >- If this parameter is left empty, the upgrade task is immediately performed.
         self.planned_start_time = planned_start_time
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The storage capacity that you can select when you change the cluster. Unit: GB.
         # 
         # >  You can set this parameter for PolarDB for MySQL clusters of Standard Edition to a value that ranges from 20 to 32000.
+        # 
+        # This parameter is required.
         self.storage_space = storage_space
         # The category of the cluster. Default value: ON. Valid values:
         # 
         # *   **normal_exclusive**: dedicated
         # *   **normal_general**: general-purpose
         self.sub_category = sub_category
 
@@ -27131,29 +27569,33 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         role_arn: str = None,
         tdestatus: str = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specifies whether to enable automatic encryption for new tables. Valid values:
         # 
         # *   **ON**\
         # *   **OFF**\
         self.encrypt_new_tables = encrypt_new_tables
         # The ID of the custom key.
         self.encryption_key = encryption_key
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
-        # The Alibaba Cloud Resource Name (ARN) of the RAM role. A RAM role is a virtual identity that you can create within your Alibaba Cloud account. For more information, see [RAM role overview](~~93689~~).
+        # The Alibaba Cloud Resource Name (ARN) of the RAM role. A RAM role is a virtual identity that you can create within your Alibaba Cloud account. For more information, see [RAM role overview](https://help.aliyun.com/document_detail/93689.html).
         self.role_arn = role_arn
         # Modifies the TDE status. Set the value to **Enable**.
+        # 
+        # This parameter is required.
         self.tdestatus = tdestatus
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27281,21 +27723,27 @@
         dbname: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The description of the database. The description must meet the following requirements:
         # 
         # *   It cannot start with `http://` or `https://`.
         # *   It must be 2 to 256 characters in length.
+        # 
+        # This parameter is required.
         self.dbdescription = dbdescription
         # The name of the database.
+        # 
+        # This parameter is required.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -27430,38 +27878,44 @@
         # 
         # *   It can contain lowercase letters, digits, and hyphens (-).
         # *   It must start with a letter and end with a digit or a letter.
         # *   It must be 6 to 30 characters in length.
         self.connection_string_prefix = connection_string_prefix
         # The ID of cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the endpoint.
         # 
-        # > You can call the [DescribeDBClusterEndpoints](~~98205~~) operation to query endpoint IDs.
+        # > You can call the [DescribeDBClusterEndpoints](https://help.aliyun.com/document_detail/98205.html) operation to query endpoint IDs.
+        # 
+        # This parameter is required.
         self.dbendpoint_id = dbendpoint_id
         # The network type of the endpoint. Valid values:
         # 
         # *   **Public**\
         # *   **Private**\
+        # 
+        # This parameter is required.
         self.net_type = net_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The port number. Valid values: 3000 to 5999.
         # 
         # > This parameter is valid only for PolarDB for MySQL clusters. If you leave this parameter empty, the default port 3306 is used.
         self.port = port
         # The prefix of the private domain name. The prefix must meet the following requirements:
         # 
         # *   The prefix can contain lowercase letters, digits, and hyphens (-).
         # *   The prefix must start with a letter and end with a digit or a letter.
         # *   The prefix must be 6 to 30 characters in length.
         # 
-        # >- You can bind each internal endpoint of PolarDB to a private domain name. The private domain name takes effect only in the specified virtual private clouds (VPCs) in the current region. Private domain names are managed by using PrivateZone. You can use the CNAME record of PrivateZone to map domain names to PolarDB. You are charged a small fee for this feature. For more information, see [Pricing](~~71338~~).
+        # >- You can bind each internal endpoint of PolarDB to a private domain name. The private domain name takes effect only in the specified virtual private clouds (VPCs) in the current region. Private domain names are managed by using PrivateZone. You can use the CNAME record of PrivateZone to map domain names to PolarDB. You are charged a small fee for this feature. For more information, see [Pricing](https://help.aliyun.com/document_detail/71338.html).
         # >- This parameter takes effect only if you set **NetType** to Private.
         self.private_zone_address_prefix = private_zone_address_prefix
         # The name of the private zone.
         # 
         # > This parameter takes effect only when **NetType** is set to Private.
         self.private_zone_name = private_zone_name
         self.resource_owner_account = resource_owner_account
@@ -27611,27 +28065,33 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         sub_category: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The token can only contain ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
-        # The specifications of all nodes. For more information, see [Specifications of computing nodes](~~102542~~).
+        # The specifications of all nodes. For more information, see [Specifications of computing nodes](https://help.aliyun.com/document_detail/102542.html).
+        # 
+        # This parameter is required.
         self.dbnode_target_class = dbnode_target_class
         # The type of the node. Valid values:
         # 
         # *   RO
         # *   STANDBY
         # *   DLNode
         self.dbnode_type = dbnode_type
         # The type of the configuration change. Valid values:
         # 
         # *   **Upgrade**\
         # *   **Downgrade**\
+        # 
+        # This parameter is required.
         self.modify_type = modify_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The latest start time to upgrade the specifications within the scheduled time period. Specify the time in the ISO 8601 standard in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
         # > *   The value of this parameter must be at least 30 minutes later than the value of PlannedStartTime.
         # >*   By default, if you specify `PlannedStartTime` but do not specify PlannedEndTime, the latest start time of the task is set to `Value of PlannedEndTime + 30 minutes`. For example, if you set `PlannedStartTime` to `2021-01-14T09:00:00Z` and you do not specify PlannedEndTime, the latest start time of the task is `2021-01-14T09:30:00Z`.
@@ -27806,22 +28266,28 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the node in the cluster.
+        # 
+        # This parameter is required.
         self.dbnode_id = dbnode_id
         # Specifies whether to enable the hot standby feature. Valid values:
         # 
         # *   **ON**\
         # *   **OFF**\
+        # 
+        # This parameter is required.
         self.hot_replica_mode = hot_replica_mode
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -27873,15 +28339,15 @@
         self,
         dbcluster_id: str = None,
         order_id: str = None,
         request_id: str = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query information about all clusters that are deployed in a specified region, such as the cluster ID.
         self.dbcluster_id = dbcluster_id
         # The ID of the order.
         self.order_id = order_id
         # The ID of the request.
         self.request_id = request_id
 
     def validate(self):
@@ -27959,15 +28425,15 @@
         dbnode_id: str = None,
         target_class: str = None,
     ):
         # The ID of the node.
         # 
         # >  If you specify this parameter, DBNode.N.TargetClass is required. N is an integer that starts from 1. The maximum value of N is calculated by using the following formula:16 - The number of current nodes.
         self.dbnode_id = dbnode_id
-        # The specifications of the node that you want to change. For more information, see [Specifications of compute nodes](~~102542~~).
+        # The specifications of the node that you want to change. For more information, see [Specifications of compute nodes](https://help.aliyun.com/document_detail/102542.html).
         # 
         # >  If you specify this parameter, DBNode.N.DBNodeId is required. N is an integer that starts from 1. The maximum value of N is calculated by using the following formula:16 - The number of current nodes.
         self.target_class = target_class
 
     def validate(self):
         pass
 
@@ -28006,21 +28472,27 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         sub_category: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length. The token is case-sensitive.
         self.client_token = client_token
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The details of the nodes.
+        # 
+        # This parameter is required.
         self.dbnode = dbnode
         # The type of the configuration change. Valid values:
         # 
         # *   **Upgrade**\
         # *   **Downgrade**\
+        # 
+        # This parameter is required.
         self.modify_type = modify_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The latest start time to upgrade the specifications within the scheduled time period. Specify the time in the ISO 8601 standard in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
         # >*   The value of this parameter must be at least 30 minutes later than the value of PlannedStartTime.
         # >*   By default, if you specify `PlannedStartTime` but do not specify PlannedEndTime, the latest start time of the task is set to `Value of PlannedEndTime + 30 minutes`. For example, if you set `PlannedStartTime` to `2021-01-14T09:00:00Z` and you do not specify PlannedEndTime, the latest start time of the task is `2021-01-14T09:30:00Z`.
@@ -28202,16 +28674,20 @@
         parameters: str = None,
         planned_end_time: str = None,
         planned_start_time: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the node. You can specify multiple node IDs. Separate multiple node IDs with commas (,).
+        # 
+        # This parameter is required.
         self.dbnode_ids = dbnode_ids
         # Specifies whether to immediately run the task to modify parameters and restart the cluster. Valid values: false: runs the task on schedule. true: runs the task immediately. Default value: false.
         self.from_time_service = from_time_service
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the parameter template that is used for the cluster.
         self.parameter_group_id = parameter_group_id
@@ -28365,18 +28841,22 @@
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The description of the GDN. The description must meet the following requirements:
         # 
         # *   It cannot start with `http://` or `https://`.
         # *   It must start with a letter.
-        # *   It can contain letters, digits, underscores (\_), and hyphens (-).
+        # *   It can contain letters, digits, underscores (_), and hyphens (-).
         # *   It must be 2 to 126 characters in length.
+        # 
+        # This parameter is required.
         self.gdndescription = gdndescription
         # The ID of the GDN.
+        # 
+        # This parameter is required.
         self.gdnid = gdnid
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -28512,26 +28992,34 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The IP address in the whitelist template.
         # 
         # >  Multiple IP addresses are separated by commas (,). You can create up to 1,000 IP addresses or CIDR blocks for all IP whitelists.
+        # 
+        # This parameter is required.
         self.gip_list = gip_list
         # The name of the IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or digit.
         # *   The name must be 2 to 120 characters in length.
+        # 
+        # This parameter is required.
         self.global_ig_name = global_ig_name
         # The ID of the IP whitelist template.
+        # 
+        # This parameter is required.
         self.global_security_group_id = global_security_group_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -28604,15 +29092,15 @@
         self.dbinstances = dbinstances
         # The IP address in the whitelist template.
         # 
         # >  Separate multiple IP addresses with commas (,). You can add up to 1,000 IP addresses or CIDR blocks to all IP whitelists.
         self.gip_list = gip_list
         # The name of the IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or a digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the IP whitelist template.
         self.global_security_group_id = global_security_group_id
         # The ID of the region.
         self.region_id = region_id
@@ -28748,23 +29236,29 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The name of the IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or digit.
         # *   The name must be 2 to 120 characters in length.
+        # 
+        # This parameter is required.
         self.global_ig_name = global_ig_name
         # The ID of the IP whitelist template.
+        # 
+        # This parameter is required.
         self.global_security_group_id = global_security_group_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -28830,15 +29324,15 @@
     ):
         # The IP address in the whitelist template.
         # 
         # >  Separate multiple IP addresses with commas (,). You can add up to 1,000 IP addresses or CIDR blocks to all IP whitelists.
         self.gip_list = gip_list
         # The name of the IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or a digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the IP whitelist template.
         self.global_security_group_id = global_security_group_id
         # The ID of the region.
         self.region_id = region_id
@@ -28969,20 +29463,26 @@
         region_id: str = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the IP whitelist template.
+        # 
+        # This parameter is required.
         self.global_security_group_id = global_security_group_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -29048,15 +29548,15 @@
     ):
         # The IP address in the whitelist template.
         # 
         # >  Separate multiple IP addresses with commas (,). You can add up to 1,000 IP addresses or CIDR blocks to all IP whitelists.
         self.gip_list = gip_list
         # The name of the IP whitelist template. The name must meet the following requirements:
         # 
-        # *   The name can contain lowercase letters, digits, and underscores (\_).
+        # *   The name can contain lowercase letters, digits, and underscores (_).
         # *   The name must start with a letter and end with a letter or a digit.
         # *   The name must be 2 to 120 characters in length.
         self.global_ig_name = global_ig_name
         # The ID of the IP whitelist template.
         self.global_security_group_id = global_security_group_id
         # The ID of the region.
         self.region_id = region_id
@@ -29194,30 +29694,32 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The cluster ID.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to query the information of all clusters that are deployed in a specific region, such as the cluster IDs.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the information of all clusters that are deployed in a specific region, such as the cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
-        # The region in which you want to store cross-region log backups. For information about regions that support the cross-region backup feature, see [Overview](~~72672~~).
+        # The region in which you want to store cross-region log backups. For information about regions that support the cross-region backup feature, see [Overview](https://help.aliyun.com/document_detail/72672.html).
         self.log_backup_another_region_region = log_backup_another_region_region
         # The retention period of cross-region log backups. Valid values:
         # 
         # *   **0**: The cross-region backup feature is disabled.
         # *   **30 to 7300**: Cross-region log backups are retained for 30 to 7,300 days.
         # *   **-1**: The log backups are permanently retained.
         # 
         # >  When you create a cluster, the default value of this parameter is **0**.
         self.log_backup_another_region_retention_period = log_backup_another_region_retention_period
         # The retention period of the log backups. Valid values:
         # 
         # *   3 to 7300: The log backups are retained for 3 to 7,300 days.
-        # *   \-1: The log backups are permanently retained.
+        # *   \\-1: The log backups are permanently retained.
         self.log_backup_retention_period = log_backup_retention_period
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -29345,15 +29847,17 @@
         rule_config: str = None,
         rule_name: str = None,
         rule_name_list: str = None,
         rule_version: str = None,
     ):
         # The ID of the cluster.
         # 
-        # > You can call the [DescribeDBClusters](~~98094~~) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # > You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of the clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specifies whether to enable the specified masking rule. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         # 
         # > This parameter is valid only when the `RuleNameList` parameter is specfied.
@@ -29370,15 +29874,15 @@
         # *   `"exempted"`: The names of database accounts to which the masking rule is not applied. Separate the names with commas (,).
         # 
         # >- If you specify `RuleName`, `RuleConfig` parameter is required. 
         # >- You need to select either `"applies_to"` or `"exempted"`.
         self.rule_config = rule_config
         # The name of the data masking rule. You can specify only one rule name at a time.
         # 
-        # >- You can call the [DescribeMaskingRules](~~212573~~) operation to query the details of all masking rules for a specified cluster, such as the names of the masking rules.
+        # >- You can call the [DescribeMaskingRules](https://help.aliyun.com/document_detail/212573.html) operation to query the details of all masking rules for a specified cluster, such as the names of the masking rules.
         # >- If the rule name does not exist in the cluster, the system automatically creates a masking rule based on the name and the value of `RuleConfig`.
         self.rule_name = rule_name
         # The list of masking rule names. You can specify one or more masking rules at a time. Separate the masking rule names with commas (,).
         # 
         # > You must specify either the `RuleName` or `RuleNameList` parameter.
         self.rule_name_list = rule_name_list
         self.rule_version = rule_version
@@ -29521,27 +30025,33 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
         switch_time: str = None,
     ):
         # The ID of the task. You can specify multiple task IDs at a time to modify the switching time of the tasks in a unified manner. The task IDs must be separated with commas (,).
+        # 
+        # This parameter is required.
         self.ids = ids
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
         # 
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query the region ID details.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the region ID details.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
         # The time that you specify for the background to perform the action that corresponds to the pending event. Specify the time in the `yyyy-MM-ddTHH:mm:ssZ` format. The time must be in UTC.
+        # 
+        # This parameter is required.
         self.switch_time = switch_time
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29679,21 +30189,25 @@
         region_id: str = None,
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         username: str = None,
     ):
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.node_type = node_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The password used to access the database for which you want to enable the PolarDB for AI feature.
         self.password = password
         # The ID of the region.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The username used to access the database for which you want to enable the PolarDB for AI feature.
         self.username = username
@@ -29963,17 +30477,21 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the cluster in the GDN.
         # 
-        # >  You can call the [DescribeGlobalDatabaseNetwork](~~264580~~) operation to view the ID of the cluster in the GDN.
+        # >  You can call the [DescribeGlobalDatabaseNetwork](https://help.aliyun.com/document_detail/264580.html) operation to view the ID of the cluster in the GDN.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the GDN.
+        # 
+        # This parameter is required.
         self.gdnid = gdnid
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -30100,22 +30618,26 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The username of the account.
         # 
         # > You can reset only the permissions of a privileged account.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The password of the account. The password must meet the following requirements:
         # 
         # *   It must contain at least three of the following character types: uppercase letters, lowercase letters, digits, and special characters.
         # *   The password must be 8 to 32 characters in length.
         # *   Special characters include `! @ # $ % ^ & * ( ) _ + - =`
         self.account_password = account_password
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -30241,17 +30763,21 @@
         region_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the cluster in the GDN.
         # 
-        # >  You can call the [DescribeGlobalDatabaseNetwork](~~264580~~) operation to view the ID of the cluster in the GDN.
+        # >  You can call the [DescribeGlobalDatabaseNetwork](https://help.aliyun.com/document_detail/264580.html) operation to view the ID of the cluster in the GDN.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The ID of the GDN.
+        # 
+        # This parameter is required.
         self.gdnid = gdnid
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the region.
         self.region_id = region_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -30380,14 +30906,15 @@
         dbcluster_id: str = None,
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         self.security_token = security_token
 
@@ -30518,15 +31045,17 @@
         owner_account: str = None,
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The ID of the node.
         # 
-        # >  You can call the [DescribeDBClusters](~~185342~~) operation to query the details of all clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/185342.html) operation to query the details of all clusters that belong to your Alibaba Cloud account, such as cluster IDs.
+        # 
+        # This parameter is required.
         self.dbnode_id = dbnode_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -30645,19 +31174,21 @@
         resource_owner_id: int = None,
         restore_time: str = None,
         security_token: str = None,
         table_meta: str = None,
     ):
         # The ID of the backup set.
         # 
-        # >  You must specify this parameter if you need to restore a database or a table by using a backup set. You can call the [DescribeBackups](~~98102~~) operation to query the ID of the backup set.
+        # >  You must specify this parameter if you need to restore a database or a table by using a backup set. You can call the [DescribeBackups](https://help.aliyun.com/document_detail/98102.html) operation to query the ID of the backup set.
         self.backup_id = backup_id
         # The cluster ID.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to query the details of all clusters within your account.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to query the details of all clusters within your account.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The point in time for the restoration. Specify the time in the ISO 8601 standard in the YYYY-MM-DDThh:mmZ format. The time must be in UTC.
         # 
@@ -30666,15 +31197,17 @@
         # *   You must specify this parameter if you need to restore the database or the table to a point in time.
         # 
         # *   You can restore your cluster to a particular time only over the past seven days.
         self.restore_time = restore_time
         self.security_token = security_token
         # The JSON string that contains the information of the database and the table that you want to restore. All values of the database and table information are of the string type. Example: `[ { "tables":[ { "name":"testtb", "type":"table", "newname":"testtb_restore" } ], "name":"testdb", "type":"db", "newname":"testdb_restore" } ]`.
         # 
-        # >  You can call the [DescribeMetaList](~~194770~~) operation to query the names and details of databases and tables that can be restored and enter their information into the corresponding locations in the preceding example.
+        # >  You can call the [DescribeMetaList](https://help.aliyun.com/document_detail/194770.html) operation to query the names and details of databases and tables that can be restored and enter their information into the corresponding locations in the preceding example.
+        # 
+        # This parameter is required.
         self.table_meta = table_meta
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30804,18 +31337,24 @@
         owner_id: int = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
     ):
         # The name of the account.
         # 
         # >  You can specify only a standard account.
+        # 
+        # This parameter is required.
         self.account_name = account_name
         # The ID of the PolarDB cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The names of the databases. If you need to specify multiple database names, separate the names with commas (,).
+        # 
+        # This parameter is required.
         self.dbname = dbname
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
 
     def validate(self):
@@ -30943,22 +31482,24 @@
         resource_group_id: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         security_token: str = None,
     ):
         # The ID of the cluster that will become the primary cluster in the GDN.
         # 
-        # You can call the [DescribeGlobalDatabaseNetwork](~~264580~~) operation to query the ID of the cluster in the GDN.
+        # You can call the [DescribeGlobalDatabaseNetwork](https://help.aliyun.com/document_detail/264580.html) operation to query the ID of the cluster in the GDN.
         self.dbcluster_id = dbcluster_id
         # Specifies whether to forcibly switch over the primary and secondary clusters in the GDN. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.forced = forced
         # The ID of the GDN.
+        # 
+        # This parameter is required.
         self.gdnid = gdnid
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
@@ -31141,20 +31682,26 @@
         resource_owner_id: int = None,
         resource_type: str = None,
         tag: List[TagResourcesRequestTag] = None,
     ):
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The region ID of the cluster.
+        # 
+        # This parameter is required.
         self.region_id = region_id
+        # This parameter is required.
         self.resource_id = resource_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The type of the resource. Set the value to **cluster**.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
+        # This parameter is required.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -31282,15 +31829,15 @@
     def __init__(
         self,
         target_class: str = None,
         zone_id: str = None,
     ):
         # The instance type of the added node. The instance type of the added node must be the same as the instance type of the original node.
         # 
-        # >  You can call the [DescribeDBClusters](~~98094~~) operation to view the instance types of original nodes.
+        # >  You can call the [DescribeDBClusters](https://help.aliyun.com/document_detail/98094.html) operation to view the instance types of original nodes.
         self.target_class = target_class
         # The ID of the zone in which the added node is deployed. The instance type of the added node must be the same as the instance type of the original node.
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
@@ -31328,30 +31875,40 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         restore_time: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value. Make sure that the value is unique among different requests. The token can only contain ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # The information of the added node.
+        # 
+        # This parameter is required.
         self.dbnode = dbnode
         # The type of configuration change. Set the value to **TempUpgrade**.
+        # 
+        # This parameter is required.
         self.modify_type = modify_type
         # The type of operation performed on the cluster. Valid values:
         # 
         # *   **Modify**: temporarily upgrade the configuration of the cluster.
+        # 
+        # This parameter is required.
         self.operation_type = operation_type
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The rollback time of the configuration for the temporary upgrade. Specify the time in the ISO 8601 standard in the YYYY-MM-DD hh:mm:ss format.
         # 
         # >  The rollback time cannot be 1 hour earlier than the current time and cannot be later than one day before the time when the cluster expires.
+        # 
+        # This parameter is required.
         self.restore_time = restore_time
 
     def validate(self):
         if self.dbnode:
             for k in self.dbnode:
                 if k:
                     k.validate()
@@ -31518,30 +32075,36 @@
         resource_owner_account: str = None,
         resource_owner_id: int = None,
         used_time: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value. Make sure that the value is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The cluster ID.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The billing method of the cluster. Valid values:
         # 
         # *   **Postpaid**: pay-as-you-go.
         # *   **Prepaid**: subscription.
+        # 
+        # This parameter is required.
         self.pay_type = pay_type
         # The renewal cycle of the cluster. Valid values:
         # 
         # *   **Year**\
         # *   **Month**\
         # 
         # >  This parameter is required if you set the **PayType** parameter to **Prepaid**.
         self.period = period
         # The ID of the region.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The subscription duration of the cluster. Valid values:
         # 
@@ -31730,21 +32293,27 @@
         # 
         # >  This parameter takes effect only when the value of the `TagKey.n` parameter is empty.
         self.all = all
         self.owner_account = owner_account
         self.owner_id = owner_id
         # The ID of the region.
         # 
-        # >  You can call the [DescribeRegions](~~98041~~) operation to query the available regions.
+        # >  You can call the [DescribeRegions](https://help.aliyun.com/document_detail/98041.html) operation to query the available regions.
+        # 
+        # This parameter is required.
         self.region_id = region_id
         # The IDs of the clusters.
+        # 
+        # This parameter is required.
         self.resource_id = resource_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
         # The type of the resource. Set the value to **cluster**.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
         # The keys of the tags.
         self.tag_key = tag_key
 
     def validate(self):
         pass
 
@@ -31879,14 +32448,16 @@
         resource_owner_id: int = None,
         target_dbrevision_version_code: str = None,
         upgrade_label: str = None,
         upgrade_policy: str = None,
         upgrade_type: str = None,
     ):
         # The ID of cluster.
+        # 
+        # This parameter is required.
         self.dbcluster_id = dbcluster_id
         # Specifies whether to immediately run the kernel upgrade task. Valid values:
         # 
         # *   **false** (default)
         # *   **true**\
         # 
         # >  This parameter is not required when you call the operation.
@@ -31901,15 +32472,15 @@
         # The earliest start time to run the task that updates the kernel version of the cluster. Specify the time in the `YYYY-MM-DDThh:mm:ssZ` format. The time must be in UTC.
         # 
         # > *   The earliest start time of the task can be a point in time within the next 24 hours. For example, if the current time is `2021-01-14T09:00:00Z`, you can specify a point in time between `2021-01-14T09:00:00Z` and `2021-01-15T09:00:00Z`.
         # >*   If you do not specify this parameter, the kernel update task runs immediately after you submit the request.
         self.planned_start_time = planned_start_time
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
-        # The code of the version to which you want to upgrade the cluster. You can call the [DescribeDBClusterVersion](~~2319145~~) operation to query the version code.
+        # The code of the version to which you want to upgrade the cluster. You can call the [DescribeDBClusterVersion](https://help.aliyun.com/document_detail/2319145.html) operation to query the version code.
         self.target_dbrevision_version_code = target_dbrevision_version_code
         # The upgrade tag. The value is fixed as **INNOVATE**.
         # 
         # > *   This parameter is applicable only when you upgrade PolarDB for MySQL 8.0.1 to PolarDB for MySQL 8.0.2.
         # >*   If you specify this parameter, you must set `UpgradePolicy` to **COLD**.
         self.upgrade_label = upgrade_label
         # The upgrade policy. Valid values:
```

### Comparing `alibabacloud_polardb20170801-5.1.0/alibabacloud_polardb20170801.egg-info/PKG-INFO` & `alibabacloud_polardb20170801-5.1.1/alibabacloud_polardb20170801.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-polardb20170801
-Version: 5.1.0
+Version: 5.1.1
 Summary: Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_polardb20170801-5.1.0/setup.py` & `alibabacloud_polardb20170801-5.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_polardb20170801.
 
-Created on 24/04/2024
+Created on 17/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_polardb20170801"
 NAME = "alibabacloud_polardb20170801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ApsaraDB for POLARDB (20170801) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

