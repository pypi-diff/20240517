# Comparing `tmp/alibabacloud_dbs20210101-2.0.0.tar.gz` & `tmp/alibabacloud_dbs20210101-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dbs20210101-2.0.0.tar", last modified: Mon Apr 29 04:42:49 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dbs20210101-2.0.1.tar", last modified: Fri May 17 17:23:03 2024, max compression
```

## Comparing `alibabacloud_dbs20210101-2.0.0.tar` & `alibabacloud_dbs20210101-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      255 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79419 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/client.py
--rw-r--r--   0 root         (0) root         (0)   136353 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-04-29 04:42:49.000000 alibabacloud_dbs20210101-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      449 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91515 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/client.py
+-rw-r--r--   0 root         (0) root         (0)   138060 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-05-17 17:23:03.000000 alibabacloud_dbs20210101-2.0.1/setup.py
```

### Comparing `alibabacloud_dbs20210101-2.0.0/LICENSE` & `alibabacloud_dbs20210101-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-2.0.0/PKG-INFO` & `alibabacloud_dbs20210101-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dbs20210101
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dbs20210101-2.0.0/README-CN.md` & `alibabacloud_dbs20210101-2.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-2.0.0/README.md` & `alibabacloud_dbs20210101-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/client.py` & `alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,14 +67,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def change_resource_group_with_options(
         self,
         request: dbs_20210101_models.ChangeResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.ChangeResourceGroupResponse:
+        """
+        @summary Moves a resource from one resource group to another.
+        
+        @param request: ChangeResourceGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
         if not UtilClient.is_unset(request.region_code):
@@ -103,14 +110,21 @@
         )
 
     async def change_resource_group_with_options_async(
         self,
         request: dbs_20210101_models.ChangeResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.ChangeResourceGroupResponse:
+        """
+        @summary Moves a resource from one resource group to another.
+        
+        @param request: ChangeResourceGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeResourceGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.new_resource_group_id):
             query['NewResourceGroupId'] = request.new_resource_group_id
         if not UtilClient.is_unset(request.region_code):
@@ -138,39 +152,53 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def change_resource_group(
         self,
         request: dbs_20210101_models.ChangeResourceGroupRequest,
     ) -> dbs_20210101_models.ChangeResourceGroupResponse:
+        """
+        @summary Moves a resource from one resource group to another.
+        
+        @param request: ChangeResourceGroupRequest
+        @return: ChangeResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.change_resource_group_with_options(request, runtime)
 
     async def change_resource_group_async(
         self,
         request: dbs_20210101_models.ChangeResourceGroupRequest,
     ) -> dbs_20210101_models.ChangeResourceGroupResponse:
+        """
+        @summary Moves a resource from one resource group to another.
+        
+        @param request: ChangeResourceGroupRequest
+        @return: ChangeResourceGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.change_resource_group_with_options_async(request, runtime)
 
     def create_download_with_options(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Creates an advanced download task for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: CreateDownloadRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDownloadResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -217,23 +245,25 @@
 
     async def create_download_with_options_async(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Creates an advanced download task for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: CreateDownloadRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDownloadResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -279,58 +309,64 @@
         )
 
     def create_download(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Creates an advanced download task for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: CreateDownloadRequest
         @return: CreateDownloadResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_download_with_options(request, runtime)
 
     async def create_download_async(
         self,
         request: dbs_20210101_models.CreateDownloadRequest,
     ) -> dbs_20210101_models.CreateDownloadResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Creates an advanced download task for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         For the instances that meet your business requirements, you can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: CreateDownloadRequest
         @return: CreateDownloadResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_download_with_options_async(request, runtime)
 
     def delete_sandbox_instance_with_options(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Releases a sandbox instance.
+        
+        @description This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -361,15 +397,17 @@
 
     async def delete_sandbox_instance_with_options_async(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Releases a sandbox instance.
+        
+        @description This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSandboxInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -399,40 +437,51 @@
         )
 
     def delete_sandbox_instance(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Releases a sandbox instance.
+        
+        @description This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @return: DeleteSandboxInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_sandbox_instance_with_options(request, runtime)
 
     async def delete_sandbox_instance_async(
         self,
         request: dbs_20210101_models.DeleteSandboxInstanceRequest,
     ) -> dbs_20210101_models.DeleteSandboxInstanceResponse:
         """
-        This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Releases a sandbox instance.
+        
+        @description This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DeleteSandboxInstanceRequest
         @return: DeleteSandboxInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_sandbox_instance_with_options_async(request, runtime)
 
     def describe_backup_data_list_with_options(
         self,
         request: dbs_20210101_models.DescribeBackupDataListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeBackupDataListResponse:
+        """
+        @summary 备份数据列表查询接口
+        
+        @param request: DescribeBackupDataListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupDataListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.backup_method):
             query['BackupMethod'] = request.backup_method
         if not UtilClient.is_unset(request.backup_mode):
@@ -483,14 +532,21 @@
         )
 
     async def describe_backup_data_list_with_options_async(
         self,
         request: dbs_20210101_models.DescribeBackupDataListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeBackupDataListResponse:
+        """
+        @summary 备份数据列表查询接口
+        
+        @param request: DescribeBackupDataListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupDataListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.backup_id):
             query['BackupId'] = request.backup_id
         if not UtilClient.is_unset(request.backup_method):
             query['BackupMethod'] = request.backup_method
         if not UtilClient.is_unset(request.backup_mode):
@@ -540,29 +596,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_backup_data_list(
         self,
         request: dbs_20210101_models.DescribeBackupDataListRequest,
     ) -> dbs_20210101_models.DescribeBackupDataListResponse:
+        """
+        @summary 备份数据列表查询接口
+        
+        @param request: DescribeBackupDataListRequest
+        @return: DescribeBackupDataListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_data_list_with_options(request, runtime)
 
     async def describe_backup_data_list_async(
         self,
         request: dbs_20210101_models.DescribeBackupDataListRequest,
     ) -> dbs_20210101_models.DescribeBackupDataListResponse:
+        """
+        @summary 备份数据列表查询接口
+        
+        @param request: DescribeBackupDataListRequest
+        @return: DescribeBackupDataListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_backup_data_list_with_options_async(request, runtime)
 
     def describe_backup_policy_with_options(
         self,
         request: dbs_20210101_models.DescribeBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        """
+        @summary 获取备份策略接口
+        
+        @param request: DescribeBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -585,14 +660,21 @@
         )
 
     async def describe_backup_policy_with_options_async(
         self,
         request: dbs_20210101_models.DescribeBackupPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        """
+        @summary 获取备份策略接口
+        
+        @param request: DescribeBackupPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeBackupPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_name):
             query['InstanceName'] = request.instance_name
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -614,29 +696,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_backup_policy(
         self,
         request: dbs_20210101_models.DescribeBackupPolicyRequest,
     ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        """
+        @summary 获取备份策略接口
+        
+        @param request: DescribeBackupPolicyRequest
+        @return: DescribeBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_backup_policy_with_options(request, runtime)
 
     async def describe_backup_policy_async(
         self,
         request: dbs_20210101_models.DescribeBackupPolicyRequest,
     ) -> dbs_20210101_models.DescribeBackupPolicyResponse:
+        """
+        @summary 获取备份策略接口
+        
+        @param request: DescribeBackupPolicyRequest
+        @return: DescribeBackupPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_backup_policy_with_options_async(request, runtime)
 
     def describe_dbtables_recovery_backup_set_with_options(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryBackupSetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryBackupSetResponse:
+        """
+        @param request: DescribeDBTablesRecoveryBackupSetRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBTablesRecoveryBackupSetResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -659,14 +758,19 @@
         )
 
     async def describe_dbtables_recovery_backup_set_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryBackupSetRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryBackupSetResponse:
+        """
+        @param request: DescribeDBTablesRecoveryBackupSetRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBTablesRecoveryBackupSetResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -688,29 +792,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbtables_recovery_backup_set(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryBackupSetRequest,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryBackupSetResponse:
+        """
+        @param request: DescribeDBTablesRecoveryBackupSetRequest
+        @return: DescribeDBTablesRecoveryBackupSetResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbtables_recovery_backup_set_with_options(request, runtime)
 
     async def describe_dbtables_recovery_backup_set_async(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryBackupSetRequest,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryBackupSetResponse:
+        """
+        @param request: DescribeDBTablesRecoveryBackupSetRequest
+        @return: DescribeDBTablesRecoveryBackupSetResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbtables_recovery_backup_set_with_options_async(request, runtime)
 
     def describe_dbtables_recovery_state_with_options(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryStateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryStateResponse:
+        """
+        @param request: DescribeDBTablesRecoveryStateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBTablesRecoveryStateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -733,14 +850,19 @@
         )
 
     async def describe_dbtables_recovery_state_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryStateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryStateResponse:
+        """
+        @param request: DescribeDBTablesRecoveryStateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBTablesRecoveryStateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -762,29 +884,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbtables_recovery_state(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryStateRequest,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryStateResponse:
+        """
+        @param request: DescribeDBTablesRecoveryStateRequest
+        @return: DescribeDBTablesRecoveryStateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbtables_recovery_state_with_options(request, runtime)
 
     async def describe_dbtables_recovery_state_async(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryStateRequest,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryStateResponse:
+        """
+        @param request: DescribeDBTablesRecoveryStateRequest
+        @return: DescribeDBTablesRecoveryStateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbtables_recovery_state_with_options_async(request, runtime)
 
     def describe_dbtables_recovery_time_range_with_options(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeResponse:
+        """
+        @param request: DescribeDBTablesRecoveryTimeRangeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBTablesRecoveryTimeRangeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -807,14 +942,19 @@
         )
 
     async def describe_dbtables_recovery_time_range_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeResponse:
+        """
+        @param request: DescribeDBTablesRecoveryTimeRangeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDBTablesRecoveryTimeRangeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -836,38 +976,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dbtables_recovery_time_range(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeRequest,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeResponse:
+        """
+        @param request: DescribeDBTablesRecoveryTimeRangeRequest
+        @return: DescribeDBTablesRecoveryTimeRangeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dbtables_recovery_time_range_with_options(request, runtime)
 
     async def describe_dbtables_recovery_time_range_async(
         self,
         request: dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeRequest,
     ) -> dbs_20210101_models.DescribeDBTablesRecoveryTimeRangeResponse:
+        """
+        @param request: DescribeDBTablesRecoveryTimeRangeRequest
+        @return: DescribeDBTablesRecoveryTimeRangeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dbtables_recovery_time_range_with_options_async(request, runtime)
 
     def describe_download_backup_set_storage_info_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the storage information of a downloaded backup set.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -902,22 +1052,24 @@
 
     async def describe_download_backup_set_storage_info_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the storage information of a downloaded backup set.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -951,64 +1103,70 @@
         )
 
     def describe_download_backup_set_storage_info(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the storage information of a downloaded backup set.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_backup_set_storage_info_with_options(request, runtime)
 
     async def describe_download_backup_set_storage_info_async(
         self,
         request: dbs_20210101_models.DescribeDownloadBackupSetStorageInfoRequest,
     ) -> dbs_20210101_models.DescribeDownloadBackupSetStorageInfoResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the storage information of a downloaded backup set.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadBackupSetStorageInfoRequest
         @return: DescribeDownloadBackupSetStorageInfoResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_backup_set_storage_info_with_options_async(request, runtime)
 
     def describe_download_support_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries whether an instance supports the advanced download feature.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadSupportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadSupportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1037,23 +1195,25 @@
 
     async def describe_download_support_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries whether an instance supports the advanced download feature.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadSupportRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadSupportResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1081,65 +1241,71 @@
         )
 
     def describe_download_support(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries whether an instance supports the advanced download feature.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadSupportRequest
         @return: DescribeDownloadSupportResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_support_with_options(request, runtime)
 
     async def describe_download_support_async(
         self,
         request: dbs_20210101_models.DescribeDownloadSupportRequest,
     ) -> dbs_20210101_models.DescribeDownloadSupportResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries whether an instance supports the advanced download feature.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
         You can create an advanced download task by point in time or backup set. You can set the download destination to a URL or directly upload the downloaded backup set to your Object Storage Service (OSS) bucket to facilitate data analysis and offline archiving.
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadSupportRequest
         @return: DescribeDownloadSupportResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_support_with_options_async(request, runtime)
 
     def describe_download_task_with_options(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the advanced download tasks for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1188,22 +1354,24 @@
 
     async def describe_download_task_with_options_async(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the advanced download tasks for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadTaskRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDownloadTaskResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1251,56 +1419,62 @@
         )
 
     def describe_download_task(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the advanced download tasks for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadTaskRequest
         @return: DescribeDownloadTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_download_task_with_options(request, runtime)
 
     async def describe_download_task_async(
         self,
         request: dbs_20210101_models.DescribeDownloadTaskRequest,
     ) -> dbs_20210101_models.DescribeDownloadTaskResponse:
         """
-        ### [](#)Supported database engines
-        *   ApsaraDB RDS for MySQL
-        *   ApsaraDB RDS for PostgreSQL
-        *   PolarDB for MySQL
+        @summary Queries the advanced download tasks for an ApsaraDB RDS for MySQL instance, an ApsaraDB RDS for PostgreSQL instance, or a PolarDB for MySQL cluster.
+        
+        @description ### [](#)Supported database engines
+        ApsaraDB RDS for MySQL
+        ApsaraDB RDS for PostgreSQL
+        PolarDB for MySQL
         ### [](#)References
-        *   [Download the backup files of an ApsaraDB RDS for MySQL instance](~~98819~~)
-        *   [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](~~96774~~)
-        *   [Download the backup files of a PolarDB for MySQL cluster](~~2627635~~)
+        [Download the backup files of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/98819.html)
+        [Download the backup files of an ApsaraDB RDS for PostgreSQL instance](https://help.aliyun.com/document_detail/96774.html)
+        [Download the backup files of a PolarDB for MySQL cluster](https://help.aliyun.com/document_detail/2627635.html)
         
         @param request: DescribeDownloadTaskRequest
         @return: DescribeDownloadTaskResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_download_task_with_options_async(request, runtime)
 
     def describe_sandbox_backup_sets_with_options(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the snapshots of an instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxBackupSetsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1333,15 +1507,17 @@
 
     async def describe_sandbox_backup_sets_with_options_async(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the snapshots of an instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxBackupSetsResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1373,42 +1549,48 @@
         )
 
     def describe_sandbox_backup_sets(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the snapshots of an instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @return: DescribeSandboxBackupSetsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_sandbox_backup_sets_with_options(request, runtime)
 
     async def describe_sandbox_backup_sets_async(
         self,
         request: dbs_20210101_models.DescribeSandboxBackupSetsRequest,
     ) -> dbs_20210101_models.DescribeSandboxBackupSetsResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the snapshots of an instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only for the Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxBackupSetsRequest
         @return: DescribeSandboxBackupSetsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sandbox_backup_sets_with_options_async(request, runtime)
 
     def describe_sandbox_instances_with_options(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries sandbox instances that are created within an account.
+        
+        @description This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxInstancesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1441,15 +1623,17 @@
 
     async def describe_sandbox_instances_with_options_async(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries sandbox instances that are created within an account.
+        
+        @description This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxInstancesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1481,42 +1665,48 @@
         )
 
     def describe_sandbox_instances(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries sandbox instances that are created within an account.
+        
+        @description This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @return: DescribeSandboxInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_sandbox_instances_with_options(request, runtime)
 
     async def describe_sandbox_instances_async(
         self,
         request: dbs_20210101_models.DescribeSandboxInstancesRequest,
     ) -> dbs_20210101_models.DescribeSandboxInstancesResponse:
         """
-        This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries sandbox instances that are created within an account.
+        
+        @description This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxInstancesRequest
         @return: DescribeSandboxInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sandbox_instances_with_options_async(request, runtime)
 
     def describe_sandbox_recovery_time_with_options(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the recoverable time range of a sandbox instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxRecoveryTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1543,15 +1733,17 @@
 
     async def describe_sandbox_recovery_time_with_options_async(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the recoverable time range of a sandbox instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSandboxRecoveryTimeResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1577,40 +1769,49 @@
         )
 
     def describe_sandbox_recovery_time(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the recoverable time range of a sandbox instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @return: DescribeSandboxRecoveryTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_sandbox_recovery_time_with_options(request, runtime)
 
     async def describe_sandbox_recovery_time_async(
         self,
         request: dbs_20210101_models.DescribeSandboxRecoveryTimeRequest,
     ) -> dbs_20210101_models.DescribeSandboxRecoveryTimeResponse:
         """
-        Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](~~203154~~) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](~~185577~~). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
+        @summary Queries the recoverable time range of a sandbox instance.
+        
+        @description Before you call this operation, you must enable the sandbox feature for the database instance. For more information, see [Use the emergency recovery feature of an ApsaraDB RDS for MySQL instance](https://help.aliyun.com/document_detail/203154.html) or [Create a sandbox instance for emergency disaster recovery of a self-managed MySQL database](https://help.aliyun.com/document_detail/185577.html). This operation is available only in Database Backup (DBS) API of the 2021-01-01 version.
         
         @param request: DescribeSandboxRecoveryTimeRequest
         @return: DescribeSandboxRecoveryTimeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sandbox_recovery_time_with_options_async(request, runtime)
 
     def modify_dbtables_recovery_state_with_options(
         self,
         request: dbs_20210101_models.ModifyDBTablesRecoveryStateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.ModifyDBTablesRecoveryStateResponse:
+        """
+        @param request: ModifyDBTablesRecoveryStateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBTablesRecoveryStateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
@@ -1637,14 +1838,19 @@
         )
 
     async def modify_dbtables_recovery_state_with_options_async(
         self,
         request: dbs_20210101_models.ModifyDBTablesRecoveryStateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.ModifyDBTablesRecoveryStateResponse:
+        """
+        @param request: ModifyDBTablesRecoveryStateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDBTablesRecoveryStateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
@@ -1670,29 +1876,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dbtables_recovery_state(
         self,
         request: dbs_20210101_models.ModifyDBTablesRecoveryStateRequest,
     ) -> dbs_20210101_models.ModifyDBTablesRecoveryStateResponse:
+        """
+        @param request: ModifyDBTablesRecoveryStateRequest
+        @return: ModifyDBTablesRecoveryStateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dbtables_recovery_state_with_options(request, runtime)
 
     async def modify_dbtables_recovery_state_async(
         self,
         request: dbs_20210101_models.ModifyDBTablesRecoveryStateRequest,
     ) -> dbs_20210101_models.ModifyDBTablesRecoveryStateResponse:
+        """
+        @param request: ModifyDBTablesRecoveryStateRequest
+        @return: ModifyDBTablesRecoveryStateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dbtables_recovery_state_with_options_async(request, runtime)
 
     def support_dbtable_recovery_with_options(
         self,
         request: dbs_20210101_models.SupportDBTableRecoveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.SupportDBTableRecoveryResponse:
+        """
+        @param request: SupportDBTableRecoveryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SupportDBTableRecoveryResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -1715,14 +1934,19 @@
         )
 
     async def support_dbtable_recovery_with_options_async(
         self,
         request: dbs_20210101_models.SupportDBTableRecoveryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dbs_20210101_models.SupportDBTableRecoveryResponse:
+        """
+        @param request: SupportDBTableRecoveryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SupportDBTableRecoveryResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.region_code):
             query['RegionCode'] = request.region_code
         req = open_api_models.OpenApiRequest(
@@ -1744,16 +1968,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def support_dbtable_recovery(
         self,
         request: dbs_20210101_models.SupportDBTableRecoveryRequest,
     ) -> dbs_20210101_models.SupportDBTableRecoveryResponse:
+        """
+        @param request: SupportDBTableRecoveryRequest
+        @return: SupportDBTableRecoveryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.support_dbtable_recovery_with_options(request, runtime)
 
     async def support_dbtable_recovery_async(
         self,
         request: dbs_20210101_models.SupportDBTableRecoveryRequest,
     ) -> dbs_20210101_models.SupportDBTableRecoveryResponse:
+        """
+        @param request: SupportDBTableRecoveryRequest
+        @return: SupportDBTableRecoveryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.support_dbtable_recovery_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101/models.py` & `alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,20 +12,26 @@
         region_code: str = None,
         resource_id: str = None,
         resource_type: str = None,
     ):
         # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # The ID of the resource group to which you want to move the resource.
+        # 
+        # This parameter is required.
         self.new_resource_group_id = new_resource_group_id
         # The region ID of the instance.
         self.region_code = region_code
         # The ID of the resource.
+        # 
+        # This parameter is required.
         self.resource_id = resource_id
         # The type of the resource. Set the value to backupplan.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -188,19 +194,19 @@
         instance_name: str = None,
         region_code: str = None,
         target_bucket: str = None,
         target_oss_region: str = None,
         target_path: str = None,
         target_type: str = None,
     ):
-        # The ID of the backup set. You can call the [DescribeBackups](~~26273~~) operation to query the ID of the backup set.
+        # The ID of the backup set. You can call the [DescribeBackups](https://help.aliyun.com/document_detail/26273.html) operation to query the ID of the backup set.
         # 
         # > This parameter is required if the BakSetType parameter is set to full.
         self.bak_set_id = bak_set_id
-        # The size of the full backup set. Unit: bytes. You can call the [DescribeBackups](~~26273~~) operation to query the size of the full backup set.
+        # The size of the full backup set. Unit: bytes. You can call the [DescribeBackups](https://help.aliyun.com/document_detail/26273.html) operation to query the size of the full backup set.
         self.bak_set_size = bak_set_size
         # The type of the download task. Valid values:
         # 
         # *   **full**: downloads a full backup set.
         # *   **pitr**: downloads a backup set at a specific point in time.
         self.bak_set_type = bak_set_type
         # The point in time at which the backup set is downloaded. Specify a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC.
@@ -212,21 +218,25 @@
         # *   **CSV**\
         # *   **SQL**\
         # *   **Parquet**\
         # 
         # > This parameter is required.
         self.format_type = format_type
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_name = instance_name
-        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
+        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](https://help.aliyun.com/document_detail/26231.html) operation to query the region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_code = region_code
         # The name of the OSS bucket that is used to store the backup set.
         # 
         # *   This parameter is required if the TargetType parameter is set to OSS.
-        # *   Make sure that your account is granted the **AliyunDBSDefaultRole** permission. For more information, see [Use RAM for resource authorization](~~26307~~). You can also grant permissions based on the operation instructions in the Resource Access Management (RAM) console.
+        # *   Make sure that your account is granted the **AliyunDBSDefaultRole** permission. For more information, see [Use RAM for resource authorization](https://help.aliyun.com/document_detail/26307.html). You can also grant permissions based on the operation instructions in the Resource Access Management (RAM) console.
         self.target_bucket = target_bucket
         # The region in which the OSS bucket resides.
         # 
         # > This parameter is required if the TargetType parameter is set to OSS.
         self.target_oss_region = target_oss_region
         # The destination path to which the backup set is downloaded.
         # 
@@ -542,19 +552,23 @@
 class DeleteSandboxInstanceRequest(TeaModel):
     def __init__(
         self,
         backup_plan_id: str = None,
         instance_id: str = None,
         zone_id: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to query the ID of the backup schedule.
+        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](https://help.aliyun.com/document_detail/437215.html) operation to query the ID of the backup schedule.
         # 
-        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](https://help.aliyun.com/document_detail/193091.html) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # 
+        # This parameter is required.
         self.backup_plan_id = backup_plan_id
-        # The ID of the sandbox instance. You can call the [DescribeSandboxInstances](~~437257~~) operation to query the ID of the sandbox instance.
+        # The ID of the sandbox instance. You can call the [DescribeSandboxInstances](https://help.aliyun.com/document_detail/437257.html) operation to query the ID of the sandbox instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         self.zone_id = zone_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1233,28 +1247,30 @@
         bak_type: str = None,
         dest_region: str = None,
         dest_type: str = None,
         dump_action: str = None,
         filter_key: str = None,
         filter_type: str = None,
         filter_value: str = None,
+        policy_id: str = None,
         retention_type: str = None,
         retention_value: str = None,
         src_region: str = None,
         src_type: str = None,
         strategy_id: str = None,
     ):
         self.auto_created = auto_created
         self.bak_type = bak_type
         self.dest_region = dest_region
         self.dest_type = dest_type
         self.dump_action = dump_action
         self.filter_key = filter_key
         self.filter_type = filter_type
         self.filter_value = filter_value
+        self.policy_id = policy_id
         self.retention_type = retention_type
         self.retention_value = retention_value
         self.src_region = src_region
         self.src_type = src_type
         self.strategy_id = strategy_id
 
     def validate(self):
@@ -1278,14 +1294,16 @@
             result['DumpAction'] = self.dump_action
         if self.filter_key is not None:
             result['FilterKey'] = self.filter_key
         if self.filter_type is not None:
             result['FilterType'] = self.filter_type
         if self.filter_value is not None:
             result['FilterValue'] = self.filter_value
+        if self.policy_id is not None:
+            result['PolicyId'] = self.policy_id
         if self.retention_type is not None:
             result['RetentionType'] = self.retention_type
         if self.retention_value is not None:
             result['RetentionValue'] = self.retention_value
         if self.src_region is not None:
             result['SrcRegion'] = self.src_region
         if self.src_type is not None:
@@ -1308,14 +1326,16 @@
             self.dump_action = m.get('DumpAction')
         if m.get('FilterKey') is not None:
             self.filter_key = m.get('FilterKey')
         if m.get('FilterType') is not None:
             self.filter_type = m.get('FilterType')
         if m.get('FilterValue') is not None:
             self.filter_value = m.get('FilterValue')
+        if m.get('PolicyId') is not None:
+            self.policy_id = m.get('PolicyId')
         if m.get('RetentionType') is not None:
             self.retention_type = m.get('RetentionType')
         if m.get('RetentionValue') is not None:
             self.retention_value = m.get('RetentionValue')
         if m.get('SrcRegion') is not None:
             self.src_region = m.get('SrcRegion')
         if m.get('SrcType') is not None:
@@ -2075,25 +2095,29 @@
         # The ID of the backup set.
         self.backup_set_id = backup_set_id
         # The validity period of the URL that is used as the download destination. Take note of the following items:
         # 
         # *   Default value: 7200. This means that the URL is valid for 2 hours by default.
         # *   Valid values: 300 to 86400. Unit: seconds. This means that you can specify a validity period in the range of 5 minutes to 1 day.
         # *   Before you specify this parameter, convert the validity period to seconds. For example, if you want to set the validity period of the URL to 5 minutes, enter 300.
+        # 
+        # This parameter is required.
         self.duration = duration
         # The ID of the instance.
         # 
         # > The **BackupSetId** parameter is required if you specify the **InstanceName** parameter.
         self.instance_name = instance_name
-        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
+        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](https://help.aliyun.com/document_detail/26231.html) operation to query the region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_code = region_code
-        # The ID of the download task.
+        # The download task ID.
         # 
         # *   The **BackupSetId** and **InstanceName** parameters are required if you do not specify the **TaskId** parameter.
-        # *   You can go to the instance details page in the Alibaba Cloud Management Console and click **Backup and Restoration** in the left-side navigation pane. On the **Backup Download** tab, view the task ID.
+        # *   To view the download task ID, go to the instance details page in the console and click **Backup and Restoration** in the left-side navigation pane. On the **Backup Download** tab, view the task ID.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2291,16 +2315,20 @@
 class DescribeDownloadSupportRequest(TeaModel):
     def __init__(
         self,
         instance_name: str = None,
         region_code: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_name = instance_name
-        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
+        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](https://help.aliyun.com/document_detail/26231.html) operation to query the region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_code = region_code
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2452,19 +2480,19 @@
         order_direct: str = None,
         page_size: str = None,
         region_code: str = None,
         start_time: str = None,
         state: str = None,
         task_type: str = None,
     ):
-        # The ID of the backup set generated when you create a download task. You can call the [DescribeBackups](~~26273~~) operation to query the ID.
+        # The ID of the backup set generated when you create a download task. You can call the [DescribeBackups](https://help.aliyun.com/document_detail/26273.html) operation to query the ID.
         self.backup_set_id = backup_set_id
         # The page number of the page to return.
         self.current_page = current_page
-        # The ID of the Database Backup (DBS) data source. Specify the parameter in the format of *ds-${Instance ID}\_${regionId}*.
+        # The ID of the Database Backup (DBS) data source. Specify the parameter in the format of *ds-${Instance ID}_${regionId}*.
         self.datasource_id = datasource_id
         # The end of the time range to query. Specify this parameter as a timestamp of the LONG type. Unit: milliseconds.
         self.end_time = end_time
         # The ID of the instance.
         # 
         # > This parameter is required.
         self.instance_name = instance_name
@@ -2473,15 +2501,17 @@
         # The order in which you want to sort the entries. Valid values:
         # 
         # *   **asc**: the ascending order.
         # *   **desc**: the descending order. This is the default value.
         self.order_direct = order_direct
         # The number of entries to return on each page.
         self.page_size = page_size
-        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](~~26231~~) operation to query the region ID of the instance.
+        # The ID of the region in which the instance resides. You can call the [DescribeDBInstanceAttribute](https://help.aliyun.com/document_detail/26231.html) operation to query the region ID of the instance.
+        # 
+        # This parameter is required.
         self.region_code = region_code
         # The beginning of the time range to query. Specify this parameter as a timestamp of the LONG type. Unit: milliseconds.
         self.start_time = start_time
         # The state of the download task. Valid values:
         # 
         # *   **Initializing**: The download task is being initialized.
         # *   **queueing**: The download task is queuing.
@@ -2906,27 +2936,29 @@
     def __init__(
         self,
         backup_plan_id: str = None,
         backup_set_id: str = None,
         page_number: str = None,
         page_size: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to query the ID of the backup schedule.
+        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](https://help.aliyun.com/document_detail/437215.html) operation to query the ID of the backup schedule.
+        # 
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](https://help.aliyun.com/document_detail/193091.html) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         # 
-        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # This parameter is required.
         self.backup_plan_id = backup_plan_id
         # The ID of the backup set. If this parameter is specified, only the snapshot of the specified backup set is returned. If this parameter is not specified, all the snapshots of the backup schedule are returned.
         self.backup_set_id = backup_set_id
         # The number of the page to return. Pages start from page 1. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
         # *   30: This is the default value.
-        # *   50\.
-        # *   100\.
+        # *   50\\.
+        # *   100\\.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3077,25 +3109,27 @@
     def __init__(
         self,
         backup_plan_id: str = None,
         instance_id: str = None,
         page_number: str = None,
         page_size: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule.
+        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](https://help.aliyun.com/document_detail/437215.html) operation to obtain the ID of the backup schedule.
         # 
-        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](https://help.aliyun.com/document_detail/193091.html) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # 
+        # This parameter is required.
         self.backup_plan_id = backup_plan_id
-        # The ID of the sandbox instance. You can call the [CreateSandboxInstance](~~437252~~) operation to obtain the ID of the sandbox instance.
+        # The ID of the sandbox instance. You can call the [CreateSandboxInstance](https://help.aliyun.com/document_detail/437252.html) operation to obtain the ID of the sandbox instance.
         self.instance_id = instance_id
         # The number of the page to return. The value must be an integer that is greater than 0. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values:
         # 
-        # *   30\. This is the default value.
+        # *   30\\. This is the default value.
         # *   50
         # *   100
         self.page_size = page_size
 
     def validate(self):
         pass
 
@@ -3252,17 +3286,19 @@
 
 
 class DescribeSandboxRecoveryTimeRequest(TeaModel):
     def __init__(
         self,
         backup_plan_id: str = None,
     ):
-        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](~~437215~~) operation to obtain the ID of the backup schedule. If you set this parameter to the backup schedule ID obtained by calling the DescribeBackupPlanList operation, the dbs prefix must be removed. Otherwise, the call fails.
+        # The ID of the backup schedule. You can call the [DescribeBackupPlanList](https://help.aliyun.com/document_detail/437215.html) operation to obtain the ID of the backup schedule. If you set this parameter to the backup schedule ID obtained by calling the DescribeBackupPlanList operation, the dbs prefix must be removed. Otherwise, the call fails.
+        # 
+        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](https://help.aliyun.com/document_detail/193091.html) to automatically add the instance to DBS and obtain the ID of the backup schedule.
         # 
-        # > If your instance is an ApsaraDB RDS for MySQL instance, you can [configure automatic access to a data source](~~193091~~) to automatically add the instance to DBS and obtain the ID of the backup schedule.
+        # This parameter is required.
         self.backup_plan_id = backup_plan_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_dbs20210101-2.0.0/alibabacloud_dbs20210101.egg-info/PKG-INFO` & `alibabacloud_dbs20210101-2.0.1/alibabacloud_dbs20210101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dbs20210101
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud Dbs (20210101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dbs20210101-2.0.0/setup.py` & `alibabacloud_dbs20210101-2.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dbs20210101.
 
-Created on 29/04/2024
+Created on 17/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dbs20210101"
 NAME = "alibabacloud_dbs20210101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dbs (20210101) SDK Library for Python"
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

