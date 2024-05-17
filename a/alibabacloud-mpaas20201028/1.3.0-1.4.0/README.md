# Comparing `tmp/alibabacloud_mpaas20201028-1.3.0.tar.gz` & `tmp/alibabacloud_mpaas20201028-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mpaas20201028-1.3.0.tar", last modified: Tue Feb  6 17:14:13 2024, max compression
+gzip compressed data, was "dist/alibabacloud_mpaas20201028-1.4.0.tar", last modified: Fri May 17 08:24:22 2024, max compression
```

## Comparing `alibabacloud_mpaas20201028-1.3.0.tar` & `alibabacloud_mpaas20201028-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      330 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2421 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1103 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1188 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)   447238 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028/client.py
--rw-r--r--   0 root         (0) root         (0)  1050430 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2421 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      436 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2627 2024-02-06 17:14:13.000000 alibabacloud_mpaas20201028-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      398 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   527128 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028/client.py
+-rw-r--r--   0 root         (0) root         (0)  1072012 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      436 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-05-17 08:24:22.000000 alibabacloud_mpaas20201028-1.4.0/setup.py
```

### Comparing `alibabacloud_mpaas20201028-1.3.0/LICENSE` & `alibabacloud_mpaas20201028-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mpaas20201028-1.3.0/PKG-INFO` & `alibabacloud_mpaas20201028-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mpaas20201028
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Mobile PaaS (20201028) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mpaas20201028-1.3.0/README-CN.md` & `alibabacloud_mpaas20201028-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mpaas20201028-1.3.0/README.md` & `alibabacloud_mpaas20201028-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028/client.py` & `alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -98,14 +98,19 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_mds_mini_config_with_options(
         self,
         request: m_paa_s20201028_models.AddMdsMiniConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.AddMdsMiniConfigResponse:
+        """
+        @param request: AddMdsMiniConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddMdsMiniConfigResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mini_config_add_json_str):
             body['MpaasMappcenterMiniConfigAddJsonStr'] = request.mpaas_mappcenter_mini_config_add_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -132,14 +137,19 @@
         )
 
     async def add_mds_mini_config_with_options_async(
         self,
         request: m_paa_s20201028_models.AddMdsMiniConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.AddMdsMiniConfigResponse:
+        """
+        @param request: AddMdsMiniConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddMdsMiniConfigResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mini_config_add_json_str):
             body['MpaasMappcenterMiniConfigAddJsonStr'] = request.mpaas_mappcenter_mini_config_add_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -165,29 +175,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_mds_mini_config(
         self,
         request: m_paa_s20201028_models.AddMdsMiniConfigRequest,
     ) -> m_paa_s20201028_models.AddMdsMiniConfigResponse:
+        """
+        @param request: AddMdsMiniConfigRequest
+        @return: AddMdsMiniConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_mds_mini_config_with_options(request, runtime)
 
     async def add_mds_mini_config_async(
         self,
         request: m_paa_s20201028_models.AddMdsMiniConfigRequest,
     ) -> m_paa_s20201028_models.AddMdsMiniConfigResponse:
+        """
+        @param request: AddMdsMiniConfigRequest
+        @return: AddMdsMiniConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.add_mds_mini_config_with_options_async(request, runtime)
 
     def cancel_push_scheduler_with_options(
         self,
         request: m_paa_s20201028_models.CancelPushSchedulerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CancelPushSchedulerResponse:
+        """
+        @param request: CancelPushSchedulerRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CancelPushSchedulerResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.type):
             body['Type'] = request.type
         if not UtilClient.is_unset(request.unique_ids):
@@ -214,14 +237,19 @@
         )
 
     async def cancel_push_scheduler_with_options_async(
         self,
         request: m_paa_s20201028_models.CancelPushSchedulerRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CancelPushSchedulerResponse:
+        """
+        @param request: CancelPushSchedulerRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CancelPushSchedulerResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.type):
             body['Type'] = request.type
         if not UtilClient.is_unset(request.unique_ids):
@@ -247,29 +275,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def cancel_push_scheduler(
         self,
         request: m_paa_s20201028_models.CancelPushSchedulerRequest,
     ) -> m_paa_s20201028_models.CancelPushSchedulerResponse:
+        """
+        @param request: CancelPushSchedulerRequest
+        @return: CancelPushSchedulerResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.cancel_push_scheduler_with_options(request, runtime)
 
     async def cancel_push_scheduler_async(
         self,
         request: m_paa_s20201028_models.CancelPushSchedulerRequest,
     ) -> m_paa_s20201028_models.CancelPushSchedulerResponse:
+        """
+        @param request: CancelPushSchedulerRequest
+        @return: CancelPushSchedulerResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.cancel_push_scheduler_with_options_async(request, runtime)
 
     def change_mcube_mini_task_status_with_options(
         self,
         request: m_paa_s20201028_models.ChangeMcubeMiniTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ChangeMcubeMiniTaskStatusResponse:
+        """
+        @param request: ChangeMcubeMiniTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeMcubeMiniTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_type):
             body['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.package_id):
@@ -302,14 +343,19 @@
         )
 
     async def change_mcube_mini_task_status_with_options_async(
         self,
         request: m_paa_s20201028_models.ChangeMcubeMiniTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ChangeMcubeMiniTaskStatusResponse:
+        """
+        @param request: ChangeMcubeMiniTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeMcubeMiniTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_type):
             body['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.package_id):
@@ -341,29 +387,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def change_mcube_mini_task_status(
         self,
         request: m_paa_s20201028_models.ChangeMcubeMiniTaskStatusRequest,
     ) -> m_paa_s20201028_models.ChangeMcubeMiniTaskStatusResponse:
+        """
+        @param request: ChangeMcubeMiniTaskStatusRequest
+        @return: ChangeMcubeMiniTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.change_mcube_mini_task_status_with_options(request, runtime)
 
     async def change_mcube_mini_task_status_async(
         self,
         request: m_paa_s20201028_models.ChangeMcubeMiniTaskStatusRequest,
     ) -> m_paa_s20201028_models.ChangeMcubeMiniTaskStatusResponse:
+        """
+        @param request: ChangeMcubeMiniTaskStatusRequest
+        @return: ChangeMcubeMiniTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.change_mcube_mini_task_status_with_options_async(request, runtime)
 
     def change_mcube_nebula_task_status_with_options(
         self,
         request: m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusResponse:
+        """
+        @param request: ChangeMcubeNebulaTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeMcubeNebulaTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_type):
             body['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.package_id):
@@ -396,14 +455,19 @@
         )
 
     async def change_mcube_nebula_task_status_with_options_async(
         self,
         request: m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusResponse:
+        """
+        @param request: ChangeMcubeNebulaTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeMcubeNebulaTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_type):
             body['BizType'] = request.biz_type
         if not UtilClient.is_unset(request.package_id):
@@ -435,29 +499,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def change_mcube_nebula_task_status(
         self,
         request: m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusRequest,
     ) -> m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusResponse:
+        """
+        @param request: ChangeMcubeNebulaTaskStatusRequest
+        @return: ChangeMcubeNebulaTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.change_mcube_nebula_task_status_with_options(request, runtime)
 
     async def change_mcube_nebula_task_status_async(
         self,
         request: m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusRequest,
     ) -> m_paa_s20201028_models.ChangeMcubeNebulaTaskStatusResponse:
+        """
+        @param request: ChangeMcubeNebulaTaskStatusRequest
+        @return: ChangeMcubeNebulaTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.change_mcube_nebula_task_status_with_options_async(request, runtime)
 
     def change_mcube_public_task_status_with_options(
         self,
         request: m_paa_s20201028_models.ChangeMcubePublicTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ChangeMcubePublicTaskStatusResponse:
+        """
+        @param request: ChangeMcubePublicTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeMcubePublicTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.task_status):
@@ -486,14 +563,19 @@
         )
 
     async def change_mcube_public_task_status_with_options_async(
         self,
         request: m_paa_s20201028_models.ChangeMcubePublicTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ChangeMcubePublicTaskStatusResponse:
+        """
+        @param request: ChangeMcubePublicTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ChangeMcubePublicTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.task_status):
@@ -521,29 +603,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def change_mcube_public_task_status(
         self,
         request: m_paa_s20201028_models.ChangeMcubePublicTaskStatusRequest,
     ) -> m_paa_s20201028_models.ChangeMcubePublicTaskStatusResponse:
+        """
+        @param request: ChangeMcubePublicTaskStatusRequest
+        @return: ChangeMcubePublicTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.change_mcube_public_task_status_with_options(request, runtime)
 
     async def change_mcube_public_task_status_async(
         self,
         request: m_paa_s20201028_models.ChangeMcubePublicTaskStatusRequest,
     ) -> m_paa_s20201028_models.ChangeMcubePublicTaskStatusResponse:
+        """
+        @param request: ChangeMcubePublicTaskStatusRequest
+        @return: ChangeMcubePublicTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.change_mcube_public_task_status_with_options_async(request, runtime)
 
     def copy_mcdp_group_with_options(
         self,
         request: m_paa_s20201028_models.CopyMcdpGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CopyMcdpGroupResponse:
+        """
+        @param request: CopyMcdpGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CopyMcdpGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_group_copy_json_str):
             body['MpaasMappcenterMcdpGroupCopyJsonStr'] = request.mpaas_mappcenter_mcdp_group_copy_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -570,14 +665,19 @@
         )
 
     async def copy_mcdp_group_with_options_async(
         self,
         request: m_paa_s20201028_models.CopyMcdpGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CopyMcdpGroupResponse:
+        """
+        @param request: CopyMcdpGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CopyMcdpGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_group_copy_json_str):
             body['MpaasMappcenterMcdpGroupCopyJsonStr'] = request.mpaas_mappcenter_mcdp_group_copy_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -603,29 +703,158 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def copy_mcdp_group(
         self,
         request: m_paa_s20201028_models.CopyMcdpGroupRequest,
     ) -> m_paa_s20201028_models.CopyMcdpGroupResponse:
+        """
+        @param request: CopyMcdpGroupRequest
+        @return: CopyMcdpGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.copy_mcdp_group_with_options(request, runtime)
 
     async def copy_mcdp_group_async(
         self,
         request: m_paa_s20201028_models.CopyMcdpGroupRequest,
     ) -> m_paa_s20201028_models.CopyMcdpGroupResponse:
+        """
+        @param request: CopyMcdpGroupRequest
+        @return: CopyMcdpGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.copy_mcdp_group_with_options_async(request, runtime)
 
+    def create_link_with_options(
+        self,
+        request: m_paa_s20201028_models.CreateLinkRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> m_paa_s20201028_models.CreateLinkResponse:
+        """
+        @summary 创建短链
+        
+        @param request: CreateLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateLinkResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_id):
+            body['AppId'] = request.app_id
+        if not UtilClient.is_unset(request.cors):
+            body['Cors'] = request.cors
+        if not UtilClient.is_unset(request.domain):
+            body['Domain'] = request.domain
+        if not UtilClient.is_unset(request.dynamicfield):
+            body['Dynamicfield'] = request.dynamicfield
+        if not UtilClient.is_unset(request.target_url):
+            body['TargetUrl'] = request.target_url
+        if not UtilClient.is_unset(request.workspace_id):
+            body['WorkspaceId'] = request.workspace_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateLink',
+            version='2020-10-28',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            m_paa_s20201028_models.CreateLinkResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_link_with_options_async(
+        self,
+        request: m_paa_s20201028_models.CreateLinkRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> m_paa_s20201028_models.CreateLinkResponse:
+        """
+        @summary 创建短链
+        
+        @param request: CreateLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateLinkResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_id):
+            body['AppId'] = request.app_id
+        if not UtilClient.is_unset(request.cors):
+            body['Cors'] = request.cors
+        if not UtilClient.is_unset(request.domain):
+            body['Domain'] = request.domain
+        if not UtilClient.is_unset(request.dynamicfield):
+            body['Dynamicfield'] = request.dynamicfield
+        if not UtilClient.is_unset(request.target_url):
+            body['TargetUrl'] = request.target_url
+        if not UtilClient.is_unset(request.workspace_id):
+            body['WorkspaceId'] = request.workspace_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateLink',
+            version='2020-10-28',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            m_paa_s20201028_models.CreateLinkResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_link(
+        self,
+        request: m_paa_s20201028_models.CreateLinkRequest,
+    ) -> m_paa_s20201028_models.CreateLinkResponse:
+        """
+        @summary 创建短链
+        
+        @param request: CreateLinkRequest
+        @return: CreateLinkResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.create_link_with_options(request, runtime)
+
+    async def create_link_async(
+        self,
+        request: m_paa_s20201028_models.CreateLinkRequest,
+    ) -> m_paa_s20201028_models.CreateLinkResponse:
+        """
+        @summary 创建短链
+        
+        @param request: CreateLinkRequest
+        @return: CreateLinkResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.create_link_with_options_async(request, runtime)
+
     def create_mas_crowd_with_options(
         self,
         request: m_paa_s20201028_models.CreateMasCrowdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMasCrowdResponse:
+        """
+        @param request: CreateMasCrowdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMasCrowdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_mas_crowd_create_json_str):
             body['MpaasMappcenterMcdpMasCrowdCreateJsonStr'] = request.mpaas_mappcenter_mcdp_mas_crowd_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -652,14 +881,19 @@
         )
 
     async def create_mas_crowd_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMasCrowdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMasCrowdResponse:
+        """
+        @param request: CreateMasCrowdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMasCrowdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_mas_crowd_create_json_str):
             body['MpaasMappcenterMcdpMasCrowdCreateJsonStr'] = request.mpaas_mappcenter_mcdp_mas_crowd_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -685,29 +919,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mas_crowd(
         self,
         request: m_paa_s20201028_models.CreateMasCrowdRequest,
     ) -> m_paa_s20201028_models.CreateMasCrowdResponse:
+        """
+        @param request: CreateMasCrowdRequest
+        @return: CreateMasCrowdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mas_crowd_with_options(request, runtime)
 
     async def create_mas_crowd_async(
         self,
         request: m_paa_s20201028_models.CreateMasCrowdRequest,
     ) -> m_paa_s20201028_models.CreateMasCrowdResponse:
+        """
+        @param request: CreateMasCrowdRequest
+        @return: CreateMasCrowdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mas_crowd_with_options_async(request, runtime)
 
     def create_mas_funnel_with_options(
         self,
         request: m_paa_s20201028_models.CreateMasFunnelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMasFunnelResponse:
+        """
+        @param request: CreateMasFunnelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMasFunnelResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_mas_funnel_create_json_str):
             body['MpaasMappcenterMcdpMasFunnelCreateJsonStr'] = request.mpaas_mappcenter_mcdp_mas_funnel_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -734,14 +981,19 @@
         )
 
     async def create_mas_funnel_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMasFunnelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMasFunnelResponse:
+        """
+        @param request: CreateMasFunnelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMasFunnelResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_mas_funnel_create_json_str):
             body['MpaasMappcenterMcdpMasFunnelCreateJsonStr'] = request.mpaas_mappcenter_mcdp_mas_funnel_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -767,29 +1019,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mas_funnel(
         self,
         request: m_paa_s20201028_models.CreateMasFunnelRequest,
     ) -> m_paa_s20201028_models.CreateMasFunnelResponse:
+        """
+        @param request: CreateMasFunnelRequest
+        @return: CreateMasFunnelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mas_funnel_with_options(request, runtime)
 
     async def create_mas_funnel_async(
         self,
         request: m_paa_s20201028_models.CreateMasFunnelRequest,
     ) -> m_paa_s20201028_models.CreateMasFunnelResponse:
+        """
+        @param request: CreateMasFunnelRequest
+        @return: CreateMasFunnelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mas_funnel_with_options_async(request, runtime)
 
     def create_mcdp_event_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpEventResponse:
+        """
+        @param request: CreateMcdpEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpEventResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_create_json_str):
             body['MpaasMappcenterMcdpEventCreateJsonStr'] = request.mpaas_mappcenter_mcdp_event_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -816,14 +1081,19 @@
         )
 
     async def create_mcdp_event_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpEventResponse:
+        """
+        @param request: CreateMcdpEventRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpEventResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_create_json_str):
             body['MpaasMappcenterMcdpEventCreateJsonStr'] = request.mpaas_mappcenter_mcdp_event_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -849,29 +1119,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcdp_event(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventRequest,
     ) -> m_paa_s20201028_models.CreateMcdpEventResponse:
+        """
+        @param request: CreateMcdpEventRequest
+        @return: CreateMcdpEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcdp_event_with_options(request, runtime)
 
     async def create_mcdp_event_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventRequest,
     ) -> m_paa_s20201028_models.CreateMcdpEventResponse:
+        """
+        @param request: CreateMcdpEventRequest
+        @return: CreateMcdpEventResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcdp_event_with_options_async(request, runtime)
 
     def create_mcdp_event_attribute_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpEventAttributeResponse:
+        """
+        @param request: CreateMcdpEventAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpEventAttributeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_attribute_create_json_str):
             body['MpaasMappcenterMcdpEventAttributeCreateJsonStr'] = request.mpaas_mappcenter_mcdp_event_attribute_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -898,14 +1181,19 @@
         )
 
     async def create_mcdp_event_attribute_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpEventAttributeResponse:
+        """
+        @param request: CreateMcdpEventAttributeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpEventAttributeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_attribute_create_json_str):
             body['MpaasMappcenterMcdpEventAttributeCreateJsonStr'] = request.mpaas_mappcenter_mcdp_event_attribute_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -931,29 +1219,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcdp_event_attribute(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventAttributeRequest,
     ) -> m_paa_s20201028_models.CreateMcdpEventAttributeResponse:
+        """
+        @param request: CreateMcdpEventAttributeRequest
+        @return: CreateMcdpEventAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcdp_event_attribute_with_options(request, runtime)
 
     async def create_mcdp_event_attribute_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpEventAttributeRequest,
     ) -> m_paa_s20201028_models.CreateMcdpEventAttributeResponse:
+        """
+        @param request: CreateMcdpEventAttributeRequest
+        @return: CreateMcdpEventAttributeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcdp_event_attribute_with_options_async(request, runtime)
 
     def create_mcdp_group_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcdpGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpGroupResponse:
+        """
+        @param request: CreateMcdpGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_group_create_json_str):
             body['MpaasMappcenterMcdpGroupCreateJsonStr'] = request.mpaas_mappcenter_mcdp_group_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -980,14 +1281,19 @@
         )
 
     async def create_mcdp_group_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpGroupResponse:
+        """
+        @param request: CreateMcdpGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_group_create_json_str):
             body['MpaasMappcenterMcdpGroupCreateJsonStr'] = request.mpaas_mappcenter_mcdp_group_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -1013,29 +1319,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcdp_group(
         self,
         request: m_paa_s20201028_models.CreateMcdpGroupRequest,
     ) -> m_paa_s20201028_models.CreateMcdpGroupResponse:
+        """
+        @param request: CreateMcdpGroupRequest
+        @return: CreateMcdpGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcdp_group_with_options(request, runtime)
 
     async def create_mcdp_group_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpGroupRequest,
     ) -> m_paa_s20201028_models.CreateMcdpGroupResponse:
+        """
+        @param request: CreateMcdpGroupRequest
+        @return: CreateMcdpGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcdp_group_with_options_async(request, runtime)
 
     def create_mcdp_material_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcdpMaterialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpMaterialResponse:
+        """
+        @param request: CreateMcdpMaterialRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpMaterialResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_material_create_json_str):
             body['MpaasMappcenterMcdpMaterialCreateJsonStr'] = request.mpaas_mappcenter_mcdp_material_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -1062,14 +1381,19 @@
         )
 
     async def create_mcdp_material_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpMaterialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpMaterialResponse:
+        """
+        @param request: CreateMcdpMaterialRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpMaterialResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_material_create_json_str):
             body['MpaasMappcenterMcdpMaterialCreateJsonStr'] = request.mpaas_mappcenter_mcdp_material_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -1095,29 +1419,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcdp_material(
         self,
         request: m_paa_s20201028_models.CreateMcdpMaterialRequest,
     ) -> m_paa_s20201028_models.CreateMcdpMaterialResponse:
+        """
+        @param request: CreateMcdpMaterialRequest
+        @return: CreateMcdpMaterialResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcdp_material_with_options(request, runtime)
 
     async def create_mcdp_material_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpMaterialRequest,
     ) -> m_paa_s20201028_models.CreateMcdpMaterialResponse:
+        """
+        @param request: CreateMcdpMaterialRequest
+        @return: CreateMcdpMaterialResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcdp_material_with_options_async(request, runtime)
 
     def create_mcdp_zone_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcdpZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpZoneResponse:
+        """
+        @param request: CreateMcdpZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpZoneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_zone_create_json_str):
             body['MpaasMappcenterMcdpZoneCreateJsonStr'] = request.mpaas_mappcenter_mcdp_zone_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -1144,14 +1481,19 @@
         )
 
     async def create_mcdp_zone_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcdpZoneResponse:
+        """
+        @param request: CreateMcdpZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcdpZoneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_zone_create_json_str):
             body['MpaasMappcenterMcdpZoneCreateJsonStr'] = request.mpaas_mappcenter_mcdp_zone_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -1177,29 +1519,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcdp_zone(
         self,
         request: m_paa_s20201028_models.CreateMcdpZoneRequest,
     ) -> m_paa_s20201028_models.CreateMcdpZoneResponse:
+        """
+        @param request: CreateMcdpZoneRequest
+        @return: CreateMcdpZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcdp_zone_with_options(request, runtime)
 
     async def create_mcdp_zone_async(
         self,
         request: m_paa_s20201028_models.CreateMcdpZoneRequest,
     ) -> m_paa_s20201028_models.CreateMcdpZoneResponse:
+        """
+        @param request: CreateMcdpZoneRequest
+        @return: CreateMcdpZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcdp_zone_with_options_async(request, runtime)
 
     def create_mcube_mini_app_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeMiniAppResponse:
+        """
+        @param request: CreateMcubeMiniAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeMiniAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.h_5name):
@@ -1228,14 +1583,19 @@
         )
 
     async def create_mcube_mini_app_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeMiniAppResponse:
+        """
+        @param request: CreateMcubeMiniAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeMiniAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.h_5name):
@@ -1263,29 +1623,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_mini_app(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniAppRequest,
     ) -> m_paa_s20201028_models.CreateMcubeMiniAppResponse:
+        """
+        @param request: CreateMcubeMiniAppRequest
+        @return: CreateMcubeMiniAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_mini_app_with_options(request, runtime)
 
     async def create_mcube_mini_app_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniAppRequest,
     ) -> m_paa_s20201028_models.CreateMcubeMiniAppResponse:
+        """
+        @param request: CreateMcubeMiniAppRequest
+        @return: CreateMcubeMiniAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_mini_app_with_options_async(request, runtime)
 
     def create_mcube_mini_task_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeMiniTaskResponse:
+        """
+        @param request: CreateMcubeMiniTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeMiniTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.grey_config_info):
             body['GreyConfigInfo'] = request.grey_config_info
         if not UtilClient.is_unset(request.grey_endtime_data):
@@ -1326,14 +1699,19 @@
         )
 
     async def create_mcube_mini_task_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeMiniTaskResponse:
+        """
+        @param request: CreateMcubeMiniTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeMiniTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.grey_config_info):
             body['GreyConfigInfo'] = request.grey_config_info
         if not UtilClient.is_unset(request.grey_endtime_data):
@@ -1373,29 +1751,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_mini_task(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniTaskRequest,
     ) -> m_paa_s20201028_models.CreateMcubeMiniTaskResponse:
+        """
+        @param request: CreateMcubeMiniTaskRequest
+        @return: CreateMcubeMiniTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_mini_task_with_options(request, runtime)
 
     async def create_mcube_mini_task_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeMiniTaskRequest,
     ) -> m_paa_s20201028_models.CreateMcubeMiniTaskResponse:
+        """
+        @param request: CreateMcubeMiniTaskRequest
+        @return: CreateMcubeMiniTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_mini_task_with_options_async(request, runtime)
 
     def create_mcube_nebula_app_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaAppResponse:
+        """
+        @param request: CreateMcubeNebulaAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeNebulaAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.h_5name):
@@ -1424,14 +1815,19 @@
         )
 
     async def create_mcube_nebula_app_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaAppResponse:
+        """
+        @param request: CreateMcubeNebulaAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeNebulaAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.h_5name):
@@ -1459,29 +1855,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_nebula_app(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaAppRequest,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaAppResponse:
+        """
+        @param request: CreateMcubeNebulaAppRequest
+        @return: CreateMcubeNebulaAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_nebula_app_with_options(request, runtime)
 
     async def create_mcube_nebula_app_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaAppRequest,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaAppResponse:
+        """
+        @param request: CreateMcubeNebulaAppRequest
+        @return: CreateMcubeNebulaAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_nebula_app_with_options_async(request, runtime)
 
     def create_mcube_nebula_resource_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaResourceResponse:
+        """
+        @param request: CreateMcubeNebulaResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeNebulaResourceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.auto_install):
             body['AutoInstall'] = request.auto_install
         if not UtilClient.is_unset(request.client_version_max):
@@ -1540,14 +1949,19 @@
         )
 
     async def create_mcube_nebula_resource_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaResourceResponse:
+        """
+        @param request: CreateMcubeNebulaResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeNebulaResourceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.auto_install):
             body['AutoInstall'] = request.auto_install
         if not UtilClient.is_unset(request.client_version_max):
@@ -1605,29 +2019,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_nebula_resource(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaResourceRequest,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaResourceResponse:
+        """
+        @param request: CreateMcubeNebulaResourceRequest
+        @return: CreateMcubeNebulaResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_nebula_resource_with_options(request, runtime)
 
     async def create_mcube_nebula_resource_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaResourceRequest,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaResourceResponse:
+        """
+        @param request: CreateMcubeNebulaResourceRequest
+        @return: CreateMcubeNebulaResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_nebula_resource_with_options_async(request, runtime)
 
     def create_mcube_nebula_task_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaTaskResponse:
+        """
+        @param request: CreateMcubeNebulaTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeNebulaTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_code):
             body['AppCode'] = request.app_code
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_type):
@@ -1722,14 +2149,19 @@
         )
 
     async def create_mcube_nebula_task_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaTaskResponse:
+        """
+        @param request: CreateMcubeNebulaTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeNebulaTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_code):
             body['AppCode'] = request.app_code
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.biz_type):
@@ -1823,29 +2255,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_nebula_task(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaTaskRequest,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaTaskResponse:
+        """
+        @param request: CreateMcubeNebulaTaskRequest
+        @return: CreateMcubeNebulaTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_nebula_task_with_options(request, runtime)
 
     async def create_mcube_nebula_task_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeNebulaTaskRequest,
     ) -> m_paa_s20201028_models.CreateMcubeNebulaTaskResponse:
+        """
+        @param request: CreateMcubeNebulaTaskRequest
+        @return: CreateMcubeNebulaTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_nebula_task_with_options_async(request, runtime)
 
     def create_mcube_upgrade_package_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradePackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradePackageResponse:
+        """
+        @param request: CreateMcubeUpgradePackageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeUpgradePackageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_version):
             body['AppVersion'] = request.app_version
         if not UtilClient.is_unset(request.appstore_url):
@@ -1900,14 +2345,19 @@
         )
 
     async def create_mcube_upgrade_package_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradePackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradePackageResponse:
+        """
+        @param request: CreateMcubeUpgradePackageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeUpgradePackageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_version):
             body['AppVersion'] = request.app_version
         if not UtilClient.is_unset(request.appstore_url):
@@ -1961,29 +2411,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_upgrade_package(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradePackageRequest,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradePackageResponse:
+        """
+        @param request: CreateMcubeUpgradePackageRequest
+        @return: CreateMcubeUpgradePackageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_upgrade_package_with_options(request, runtime)
 
     async def create_mcube_upgrade_package_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradePackageRequest,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradePackageResponse:
+        """
+        @param request: CreateMcubeUpgradePackageRequest
+        @return: CreateMcubeUpgradePackageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_upgrade_package_with_options_async(request, runtime)
 
     def create_mcube_upgrade_task_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradeTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradeTaskResponse:
+        """
+        @param request: CreateMcubeUpgradeTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeUpgradeTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.grey_config_info):
             body['GreyConfigInfo'] = request.grey_config_info
         if not UtilClient.is_unset(request.grey_endtime_data):
@@ -2030,14 +2493,19 @@
         )
 
     async def create_mcube_upgrade_task_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradeTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradeTaskResponse:
+        """
+        @param request: CreateMcubeUpgradeTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeUpgradeTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.grey_config_info):
             body['GreyConfigInfo'] = request.grey_config_info
         if not UtilClient.is_unset(request.grey_endtime_data):
@@ -2083,29 +2551,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_upgrade_task(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradeTaskRequest,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradeTaskResponse:
+        """
+        @param request: CreateMcubeUpgradeTaskRequest
+        @return: CreateMcubeUpgradeTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_upgrade_task_with_options(request, runtime)
 
     async def create_mcube_upgrade_task_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeUpgradeTaskRequest,
     ) -> m_paa_s20201028_models.CreateMcubeUpgradeTaskResponse:
+        """
+        @param request: CreateMcubeUpgradeTaskRequest
+        @return: CreateMcubeUpgradeTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_upgrade_task_with_options_async(request, runtime)
 
     def create_mcube_vhost_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeVhostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeVhostResponse:
+        """
+        @param request: CreateMcubeVhostRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeVhostResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.vhost):
@@ -2132,14 +2613,19 @@
         )
 
     async def create_mcube_vhost_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeVhostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeVhostResponse:
+        """
+        @param request: CreateMcubeVhostRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeVhostResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.vhost):
@@ -2165,29 +2651,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_vhost(
         self,
         request: m_paa_s20201028_models.CreateMcubeVhostRequest,
     ) -> m_paa_s20201028_models.CreateMcubeVhostResponse:
+        """
+        @param request: CreateMcubeVhostRequest
+        @return: CreateMcubeVhostResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_vhost_with_options(request, runtime)
 
     async def create_mcube_vhost_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeVhostRequest,
     ) -> m_paa_s20201028_models.CreateMcubeVhostResponse:
+        """
+        @param request: CreateMcubeVhostRequest
+        @return: CreateMcubeVhostResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_vhost_with_options_async(request, runtime)
 
     def create_mcube_whitelist_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistResponse:
+        """
+        @param request: CreateMcubeWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeWhitelistResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.white_list_name):
@@ -2216,14 +2715,19 @@
         )
 
     async def create_mcube_whitelist_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistResponse:
+        """
+        @param request: CreateMcubeWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeWhitelistResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.white_list_name):
@@ -2251,29 +2755,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_whitelist(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistRequest,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistResponse:
+        """
+        @param request: CreateMcubeWhitelistRequest
+        @return: CreateMcubeWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_whitelist_with_options(request, runtime)
 
     async def create_mcube_whitelist_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistRequest,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistResponse:
+        """
+        @param request: CreateMcubeWhitelistRequest
+        @return: CreateMcubeWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_whitelist_with_options_async(request, runtime)
 
     def create_mcube_whitelist_for_ide_with_options(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistForIdeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistForIdeResponse:
+        """
+        @param request: CreateMcubeWhitelistForIdeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeWhitelistForIdeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.user_id):
@@ -2302,14 +2819,19 @@
         )
 
     async def create_mcube_whitelist_for_ide_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistForIdeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistForIdeResponse:
+        """
+        @param request: CreateMcubeWhitelistForIdeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMcubeWhitelistForIdeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.user_id):
@@ -2337,29 +2859,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mcube_whitelist_for_ide(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistForIdeRequest,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistForIdeResponse:
+        """
+        @param request: CreateMcubeWhitelistForIdeRequest
+        @return: CreateMcubeWhitelistForIdeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mcube_whitelist_for_ide_with_options(request, runtime)
 
     async def create_mcube_whitelist_for_ide_async(
         self,
         request: m_paa_s20201028_models.CreateMcubeWhitelistForIdeRequest,
     ) -> m_paa_s20201028_models.CreateMcubeWhitelistForIdeResponse:
+        """
+        @param request: CreateMcubeWhitelistForIdeRequest
+        @return: CreateMcubeWhitelistForIdeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mcube_whitelist_for_ide_with_options_async(request, runtime)
 
     def create_mds_miniprogram_task_with_options(
         self,
         request: m_paa_s20201028_models.CreateMdsMiniprogramTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMdsMiniprogramTaskResponse:
+        """
+        @param request: CreateMdsMiniprogramTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMdsMiniprogramTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.grey_config_info):
             body['GreyConfigInfo'] = request.grey_config_info
         if not UtilClient.is_unset(request.grey_endtime_data):
@@ -2404,14 +2939,19 @@
         )
 
     async def create_mds_miniprogram_task_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMdsMiniprogramTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMdsMiniprogramTaskResponse:
+        """
+        @param request: CreateMdsMiniprogramTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMdsMiniprogramTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.grey_config_info):
             body['GreyConfigInfo'] = request.grey_config_info
         if not UtilClient.is_unset(request.grey_endtime_data):
@@ -2455,29 +2995,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mds_miniprogram_task(
         self,
         request: m_paa_s20201028_models.CreateMdsMiniprogramTaskRequest,
     ) -> m_paa_s20201028_models.CreateMdsMiniprogramTaskResponse:
+        """
+        @param request: CreateMdsMiniprogramTaskRequest
+        @return: CreateMdsMiniprogramTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mds_miniprogram_task_with_options(request, runtime)
 
     async def create_mds_miniprogram_task_async(
         self,
         request: m_paa_s20201028_models.CreateMdsMiniprogramTaskRequest,
     ) -> m_paa_s20201028_models.CreateMdsMiniprogramTaskResponse:
+        """
+        @param request: CreateMdsMiniprogramTaskRequest
+        @return: CreateMdsMiniprogramTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mds_miniprogram_task_with_options_async(request, runtime)
 
     def create_msa_enhance_with_options(
         self,
         request: m_paa_s20201028_models.CreateMsaEnhanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMsaEnhanceResponse:
+        """
+        @param request: CreateMsaEnhanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMsaEnhanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_msa_enhance_create_json_str):
             body['MpaasMappcenterMsaEnhanceCreateJsonStr'] = request.mpaas_mappcenter_msa_enhance_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -2504,14 +3057,19 @@
         )
 
     async def create_msa_enhance_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateMsaEnhanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateMsaEnhanceResponse:
+        """
+        @param request: CreateMsaEnhanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMsaEnhanceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_msa_enhance_create_json_str):
             body['MpaasMappcenterMsaEnhanceCreateJsonStr'] = request.mpaas_mappcenter_msa_enhance_create_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -2537,29 +3095,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_msa_enhance(
         self,
         request: m_paa_s20201028_models.CreateMsaEnhanceRequest,
     ) -> m_paa_s20201028_models.CreateMsaEnhanceResponse:
+        """
+        @param request: CreateMsaEnhanceRequest
+        @return: CreateMsaEnhanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_msa_enhance_with_options(request, runtime)
 
     async def create_msa_enhance_async(
         self,
         request: m_paa_s20201028_models.CreateMsaEnhanceRequest,
     ) -> m_paa_s20201028_models.CreateMsaEnhanceResponse:
+        """
+        @param request: CreateMsaEnhanceRequest
+        @return: CreateMsaEnhanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_msa_enhance_with_options_async(request, runtime)
 
     def create_open_global_data_with_options(
         self,
         request: m_paa_s20201028_models.CreateOpenGlobalDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateOpenGlobalDataResponse:
+        """
+        @param request: CreateOpenGlobalDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateOpenGlobalDataResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_max_version):
             body['AppMaxVersion'] = request.app_max_version
         if not UtilClient.is_unset(request.app_min_version):
@@ -2606,14 +3177,19 @@
         )
 
     async def create_open_global_data_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateOpenGlobalDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateOpenGlobalDataResponse:
+        """
+        @param request: CreateOpenGlobalDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateOpenGlobalDataResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_max_version):
             body['AppMaxVersion'] = request.app_max_version
         if not UtilClient.is_unset(request.app_min_version):
@@ -2659,29 +3235,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_open_global_data(
         self,
         request: m_paa_s20201028_models.CreateOpenGlobalDataRequest,
     ) -> m_paa_s20201028_models.CreateOpenGlobalDataResponse:
+        """
+        @param request: CreateOpenGlobalDataRequest
+        @return: CreateOpenGlobalDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_open_global_data_with_options(request, runtime)
 
     async def create_open_global_data_async(
         self,
         request: m_paa_s20201028_models.CreateOpenGlobalDataRequest,
     ) -> m_paa_s20201028_models.CreateOpenGlobalDataResponse:
+        """
+        @param request: CreateOpenGlobalDataRequest
+        @return: CreateOpenGlobalDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_open_global_data_with_options_async(request, runtime)
 
     def create_open_single_data_with_options(
         self,
         request: m_paa_s20201028_models.CreateOpenSingleDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateOpenSingleDataResponse:
+        """
+        @param request: CreateOpenSingleDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateOpenSingleDataResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_max_version):
             body['AppMaxVersion'] = request.app_max_version
         if not UtilClient.is_unset(request.app_min_version):
@@ -2726,14 +3315,19 @@
         )
 
     async def create_open_single_data_with_options_async(
         self,
         request: m_paa_s20201028_models.CreateOpenSingleDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.CreateOpenSingleDataResponse:
+        """
+        @param request: CreateOpenSingleDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateOpenSingleDataResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_max_version):
             body['AppMaxVersion'] = request.app_max_version
         if not UtilClient.is_unset(request.app_min_version):
@@ -2777,29 +3371,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_open_single_data(
         self,
         request: m_paa_s20201028_models.CreateOpenSingleDataRequest,
     ) -> m_paa_s20201028_models.CreateOpenSingleDataResponse:
+        """
+        @param request: CreateOpenSingleDataRequest
+        @return: CreateOpenSingleDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_open_single_data_with_options(request, runtime)
 
     async def create_open_single_data_async(
         self,
         request: m_paa_s20201028_models.CreateOpenSingleDataRequest,
     ) -> m_paa_s20201028_models.CreateOpenSingleDataResponse:
+        """
+        @param request: CreateOpenSingleDataRequest
+        @return: CreateOpenSingleDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_open_single_data_with_options_async(request, runtime)
 
     def delete_cubecard_whitelist_content_with_options(
         self,
         request: m_paa_s20201028_models.DeleteCubecardWhitelistContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteCubecardWhitelistContentResponse:
+        """
+        @param request: DeleteCubecardWhitelistContentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteCubecardWhitelistContentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.whitelist_id):
@@ -2828,14 +3435,19 @@
         )
 
     async def delete_cubecard_whitelist_content_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteCubecardWhitelistContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteCubecardWhitelistContentResponse:
+        """
+        @param request: DeleteCubecardWhitelistContentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteCubecardWhitelistContentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.whitelist_id):
@@ -2863,29 +3475,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_cubecard_whitelist_content(
         self,
         request: m_paa_s20201028_models.DeleteCubecardWhitelistContentRequest,
     ) -> m_paa_s20201028_models.DeleteCubecardWhitelistContentResponse:
+        """
+        @param request: DeleteCubecardWhitelistContentRequest
+        @return: DeleteCubecardWhitelistContentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_cubecard_whitelist_content_with_options(request, runtime)
 
     async def delete_cubecard_whitelist_content_async(
         self,
         request: m_paa_s20201028_models.DeleteCubecardWhitelistContentRequest,
     ) -> m_paa_s20201028_models.DeleteCubecardWhitelistContentResponse:
+        """
+        @param request: DeleteCubecardWhitelistContentRequest
+        @return: DeleteCubecardWhitelistContentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_cubecard_whitelist_content_with_options_async(request, runtime)
 
     def delete_mcdp_aim_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcdpAimRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpAimResponse:
+        """
+        @param request: DeleteMcdpAimRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpAimResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_aim_delete_json_str):
             body['MpaasMappcenterMcdpAimDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_aim_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -2912,14 +3537,19 @@
         )
 
     async def delete_mcdp_aim_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpAimRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpAimResponse:
+        """
+        @param request: DeleteMcdpAimRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpAimResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_aim_delete_json_str):
             body['MpaasMappcenterMcdpAimDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_aim_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -2945,29 +3575,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcdp_aim(
         self,
         request: m_paa_s20201028_models.DeleteMcdpAimRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpAimResponse:
+        """
+        @param request: DeleteMcdpAimRequest
+        @return: DeleteMcdpAimResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcdp_aim_with_options(request, runtime)
 
     async def delete_mcdp_aim_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpAimRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpAimResponse:
+        """
+        @param request: DeleteMcdpAimRequest
+        @return: DeleteMcdpAimResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcdp_aim_with_options_async(request, runtime)
 
     def delete_mcdp_crowd_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcdpCrowdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpCrowdResponse:
+        """
+        @param request: DeleteMcdpCrowdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpCrowdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_crowd_delete_json_str):
             body['MpaasMappcenterMcdpCrowdDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_crowd_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -2994,14 +3637,19 @@
         )
 
     async def delete_mcdp_crowd_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpCrowdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpCrowdResponse:
+        """
+        @param request: DeleteMcdpCrowdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpCrowdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_crowd_delete_json_str):
             body['MpaasMappcenterMcdpCrowdDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_crowd_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3027,29 +3675,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcdp_crowd(
         self,
         request: m_paa_s20201028_models.DeleteMcdpCrowdRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpCrowdResponse:
+        """
+        @param request: DeleteMcdpCrowdRequest
+        @return: DeleteMcdpCrowdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcdp_crowd_with_options(request, runtime)
 
     async def delete_mcdp_crowd_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpCrowdRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpCrowdResponse:
+        """
+        @param request: DeleteMcdpCrowdRequest
+        @return: DeleteMcdpCrowdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcdp_crowd_with_options_async(request, runtime)
 
     def delete_mcdp_event_attribute_by_id_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventAttributeByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpEventAttributeByIdResponse:
+        """
+        @param request: DeleteMcdpEventAttributeByIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpEventAttributeByIdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_attribute_delete_json_str):
             body['MpaasMappcenterMcdpEventAttributeDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_event_attribute_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3076,14 +3737,19 @@
         )
 
     async def delete_mcdp_event_attribute_by_id_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventAttributeByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpEventAttributeByIdResponse:
+        """
+        @param request: DeleteMcdpEventAttributeByIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpEventAttributeByIdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_attribute_delete_json_str):
             body['MpaasMappcenterMcdpEventAttributeDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_event_attribute_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3109,29 +3775,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcdp_event_attribute_by_id(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventAttributeByIdRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpEventAttributeByIdResponse:
+        """
+        @param request: DeleteMcdpEventAttributeByIdRequest
+        @return: DeleteMcdpEventAttributeByIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcdp_event_attribute_by_id_with_options(request, runtime)
 
     async def delete_mcdp_event_attribute_by_id_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventAttributeByIdRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpEventAttributeByIdResponse:
+        """
+        @param request: DeleteMcdpEventAttributeByIdRequest
+        @return: DeleteMcdpEventAttributeByIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcdp_event_attribute_by_id_with_options_async(request, runtime)
 
     def delete_mcdp_event_by_id_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpEventByIdResponse:
+        """
+        @param request: DeleteMcdpEventByIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpEventByIdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_delete_json_str):
             body['MpaasMappcenterMcdpEventDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_event_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3158,14 +3837,19 @@
         )
 
     async def delete_mcdp_event_by_id_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventByIdRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpEventByIdResponse:
+        """
+        @param request: DeleteMcdpEventByIdRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpEventByIdResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_event_delete_json_str):
             body['MpaasMappcenterMcdpEventDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_event_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3191,29 +3875,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcdp_event_by_id(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventByIdRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpEventByIdResponse:
+        """
+        @param request: DeleteMcdpEventByIdRequest
+        @return: DeleteMcdpEventByIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcdp_event_by_id_with_options(request, runtime)
 
     async def delete_mcdp_event_by_id_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpEventByIdRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpEventByIdResponse:
+        """
+        @param request: DeleteMcdpEventByIdRequest
+        @return: DeleteMcdpEventByIdResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcdp_event_by_id_with_options_async(request, runtime)
 
     def delete_mcdp_material_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcdpMaterialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpMaterialResponse:
+        """
+        @param request: DeleteMcdpMaterialRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpMaterialResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_material_delete_json_str):
             body['MpaasMappcenterMcdpMaterialDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_material_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3240,14 +3937,19 @@
         )
 
     async def delete_mcdp_material_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpMaterialRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpMaterialResponse:
+        """
+        @param request: DeleteMcdpMaterialRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpMaterialResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_material_delete_json_str):
             body['MpaasMappcenterMcdpMaterialDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_material_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3273,29 +3975,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcdp_material(
         self,
         request: m_paa_s20201028_models.DeleteMcdpMaterialRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpMaterialResponse:
+        """
+        @param request: DeleteMcdpMaterialRequest
+        @return: DeleteMcdpMaterialResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcdp_material_with_options(request, runtime)
 
     async def delete_mcdp_material_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpMaterialRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpMaterialResponse:
+        """
+        @param request: DeleteMcdpMaterialRequest
+        @return: DeleteMcdpMaterialResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcdp_material_with_options_async(request, runtime)
 
     def delete_mcdp_zone_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcdpZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpZoneResponse:
+        """
+        @param request: DeleteMcdpZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpZoneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_zone_delete_json_str):
             body['MpaasMappcenterMcdpZoneDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_zone_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3322,14 +4037,19 @@
         )
 
     async def delete_mcdp_zone_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcdpZoneResponse:
+        """
+        @param request: DeleteMcdpZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcdpZoneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mcdp_zone_delete_json_str):
             body['MpaasMappcenterMcdpZoneDeleteJsonStr'] = request.mpaas_mappcenter_mcdp_zone_delete_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -3355,29 +4075,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcdp_zone(
         self,
         request: m_paa_s20201028_models.DeleteMcdpZoneRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpZoneResponse:
+        """
+        @param request: DeleteMcdpZoneRequest
+        @return: DeleteMcdpZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcdp_zone_with_options(request, runtime)
 
     async def delete_mcdp_zone_async(
         self,
         request: m_paa_s20201028_models.DeleteMcdpZoneRequest,
     ) -> m_paa_s20201028_models.DeleteMcdpZoneResponse:
+        """
+        @param request: DeleteMcdpZoneRequest
+        @return: DeleteMcdpZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcdp_zone_with_options_async(request, runtime)
 
     def delete_mcube_mini_app_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcubeMiniAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeMiniAppResponse:
+        """
+        @param request: DeleteMcubeMiniAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeMiniAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.tenant_id):
@@ -3404,14 +4137,19 @@
         )
 
     async def delete_mcube_mini_app_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeMiniAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeMiniAppResponse:
+        """
+        @param request: DeleteMcubeMiniAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeMiniAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.tenant_id):
@@ -3437,29 +4175,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcube_mini_app(
         self,
         request: m_paa_s20201028_models.DeleteMcubeMiniAppRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeMiniAppResponse:
+        """
+        @param request: DeleteMcubeMiniAppRequest
+        @return: DeleteMcubeMiniAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcube_mini_app_with_options(request, runtime)
 
     async def delete_mcube_mini_app_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeMiniAppRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeMiniAppResponse:
+        """
+        @param request: DeleteMcubeMiniAppRequest
+        @return: DeleteMcubeMiniAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcube_mini_app_with_options_async(request, runtime)
 
     def delete_mcube_nebula_app_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcubeNebulaAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeNebulaAppResponse:
+        """
+        @param request: DeleteMcubeNebulaAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeNebulaAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.tenant_id):
@@ -3486,14 +4237,19 @@
         )
 
     async def delete_mcube_nebula_app_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeNebulaAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeNebulaAppResponse:
+        """
+        @param request: DeleteMcubeNebulaAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeNebulaAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.tenant_id):
@@ -3519,29 +4275,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcube_nebula_app(
         self,
         request: m_paa_s20201028_models.DeleteMcubeNebulaAppRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeNebulaAppResponse:
+        """
+        @param request: DeleteMcubeNebulaAppRequest
+        @return: DeleteMcubeNebulaAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcube_nebula_app_with_options(request, runtime)
 
     async def delete_mcube_nebula_app_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeNebulaAppRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeNebulaAppResponse:
+        """
+        @param request: DeleteMcubeNebulaAppRequest
+        @return: DeleteMcubeNebulaAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcube_nebula_app_with_options_async(request, runtime)
 
     def delete_mcube_upgrade_resource_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcubeUpgradeResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeUpgradeResourceResponse:
+        """
+        @param request: DeleteMcubeUpgradeResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeUpgradeResourceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.platform):
@@ -3570,14 +4339,19 @@
         )
 
     async def delete_mcube_upgrade_resource_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeUpgradeResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeUpgradeResourceResponse:
+        """
+        @param request: DeleteMcubeUpgradeResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeUpgradeResourceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.platform):
@@ -3605,29 +4379,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcube_upgrade_resource(
         self,
         request: m_paa_s20201028_models.DeleteMcubeUpgradeResourceRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeUpgradeResourceResponse:
+        """
+        @param request: DeleteMcubeUpgradeResourceRequest
+        @return: DeleteMcubeUpgradeResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcube_upgrade_resource_with_options(request, runtime)
 
     async def delete_mcube_upgrade_resource_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeUpgradeResourceRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeUpgradeResourceResponse:
+        """
+        @param request: DeleteMcubeUpgradeResourceRequest
+        @return: DeleteMcubeUpgradeResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcube_upgrade_resource_with_options_async(request, runtime)
 
     def delete_mcube_whitelist_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMcubeWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeWhitelistResponse:
+        """
+        @param request: DeleteMcubeWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeWhitelistResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -3654,14 +4441,19 @@
         )
 
     async def delete_mcube_whitelist_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMcubeWhitelistResponse:
+        """
+        @param request: DeleteMcubeWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMcubeWhitelistResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -3687,29 +4479,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mcube_whitelist(
         self,
         request: m_paa_s20201028_models.DeleteMcubeWhitelistRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeWhitelistResponse:
+        """
+        @param request: DeleteMcubeWhitelistRequest
+        @return: DeleteMcubeWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mcube_whitelist_with_options(request, runtime)
 
     async def delete_mcube_whitelist_async(
         self,
         request: m_paa_s20201028_models.DeleteMcubeWhitelistRequest,
     ) -> m_paa_s20201028_models.DeleteMcubeWhitelistResponse:
+        """
+        @param request: DeleteMcubeWhitelistRequest
+        @return: DeleteMcubeWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mcube_whitelist_with_options_async(request, runtime)
 
     def delete_mds_whitelist_content_with_options(
         self,
         request: m_paa_s20201028_models.DeleteMdsWhitelistContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMdsWhitelistContentResponse:
+        """
+        @param request: DeleteMdsWhitelistContentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMdsWhitelistContentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.whitelist_id):
@@ -3738,14 +4543,19 @@
         )
 
     async def delete_mds_whitelist_content_with_options_async(
         self,
         request: m_paa_s20201028_models.DeleteMdsWhitelistContentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.DeleteMdsWhitelistContentResponse:
+        """
+        @param request: DeleteMdsWhitelistContentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMdsWhitelistContentResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.whitelist_id):
@@ -3773,29 +4583,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mds_whitelist_content(
         self,
         request: m_paa_s20201028_models.DeleteMdsWhitelistContentRequest,
     ) -> m_paa_s20201028_models.DeleteMdsWhitelistContentResponse:
+        """
+        @param request: DeleteMdsWhitelistContentRequest
+        @return: DeleteMdsWhitelistContentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mds_whitelist_content_with_options(request, runtime)
 
     async def delete_mds_whitelist_content_async(
         self,
         request: m_paa_s20201028_models.DeleteMdsWhitelistContentRequest,
     ) -> m_paa_s20201028_models.DeleteMdsWhitelistContentResponse:
+        """
+        @param request: DeleteMdsWhitelistContentRequest
+        @return: DeleteMdsWhitelistContentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mds_whitelist_content_with_options_async(request, runtime)
 
     def exist_mcube_rsa_key_with_options(
         self,
         request: m_paa_s20201028_models.ExistMcubeRsaKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ExistMcubeRsaKeyResponse:
+        """
+        @param request: ExistMcubeRsaKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExistMcubeRsaKeyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -3820,14 +4643,19 @@
         )
 
     async def exist_mcube_rsa_key_with_options_async(
         self,
         request: m_paa_s20201028_models.ExistMcubeRsaKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ExistMcubeRsaKeyResponse:
+        """
+        @param request: ExistMcubeRsaKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExistMcubeRsaKeyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -3851,29 +4679,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def exist_mcube_rsa_key(
         self,
         request: m_paa_s20201028_models.ExistMcubeRsaKeyRequest,
     ) -> m_paa_s20201028_models.ExistMcubeRsaKeyResponse:
+        """
+        @param request: ExistMcubeRsaKeyRequest
+        @return: ExistMcubeRsaKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.exist_mcube_rsa_key_with_options(request, runtime)
 
     async def exist_mcube_rsa_key_async(
         self,
         request: m_paa_s20201028_models.ExistMcubeRsaKeyRequest,
     ) -> m_paa_s20201028_models.ExistMcubeRsaKeyResponse:
+        """
+        @param request: ExistMcubeRsaKeyRequest
+        @return: ExistMcubeRsaKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.exist_mcube_rsa_key_with_options_async(request, runtime)
 
     def export_mapp_center_app_config_with_options(
         self,
         request: m_paa_s20201028_models.ExportMappCenterAppConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ExportMappCenterAppConfigResponse:
+        """
+        @param request: ExportMappCenterAppConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExportMappCenterAppConfigResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.apk_file_url):
             body['ApkFileUrl'] = request.apk_file_url
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cert_rsa_base_64):
@@ -3906,14 +4747,19 @@
         )
 
     async def export_mapp_center_app_config_with_options_async(
         self,
         request: m_paa_s20201028_models.ExportMappCenterAppConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ExportMappCenterAppConfigResponse:
+        """
+        @param request: ExportMappCenterAppConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ExportMappCenterAppConfigResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.apk_file_url):
             body['ApkFileUrl'] = request.apk_file_url
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.cert_rsa_base_64):
@@ -3945,29 +4791,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def export_mapp_center_app_config(
         self,
         request: m_paa_s20201028_models.ExportMappCenterAppConfigRequest,
     ) -> m_paa_s20201028_models.ExportMappCenterAppConfigResponse:
+        """
+        @param request: ExportMappCenterAppConfigRequest
+        @return: ExportMappCenterAppConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.export_mapp_center_app_config_with_options(request, runtime)
 
     async def export_mapp_center_app_config_async(
         self,
         request: m_paa_s20201028_models.ExportMappCenterAppConfigRequest,
     ) -> m_paa_s20201028_models.ExportMappCenterAppConfigResponse:
+        """
+        @param request: ExportMappCenterAppConfigRequest
+        @return: ExportMappCenterAppConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.export_mapp_center_app_config_with_options_async(request, runtime)
 
     def get_file_token_for_upload_to_msa_with_options(
         self,
         request: m_paa_s20201028_models.GetFileTokenForUploadToMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetFileTokenForUploadToMsaResponse:
+        """
+        @param request: GetFileTokenForUploadToMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetFileTokenForUploadToMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.onex_flag):
             body['OnexFlag'] = request.onex_flag
         if not UtilClient.is_unset(request.tenant_id):
@@ -3994,14 +4853,19 @@
         )
 
     async def get_file_token_for_upload_to_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.GetFileTokenForUploadToMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetFileTokenForUploadToMsaResponse:
+        """
+        @param request: GetFileTokenForUploadToMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetFileTokenForUploadToMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.onex_flag):
             body['OnexFlag'] = request.onex_flag
         if not UtilClient.is_unset(request.tenant_id):
@@ -4027,29 +4891,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_file_token_for_upload_to_msa(
         self,
         request: m_paa_s20201028_models.GetFileTokenForUploadToMsaRequest,
     ) -> m_paa_s20201028_models.GetFileTokenForUploadToMsaResponse:
+        """
+        @param request: GetFileTokenForUploadToMsaRequest
+        @return: GetFileTokenForUploadToMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_file_token_for_upload_to_msa_with_options(request, runtime)
 
     async def get_file_token_for_upload_to_msa_async(
         self,
         request: m_paa_s20201028_models.GetFileTokenForUploadToMsaRequest,
     ) -> m_paa_s20201028_models.GetFileTokenForUploadToMsaResponse:
+        """
+        @param request: GetFileTokenForUploadToMsaRequest
+        @return: GetFileTokenForUploadToMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_file_token_for_upload_to_msa_with_options_async(request, runtime)
 
     def get_log_url_in_msa_with_options(
         self,
         request: m_paa_s20201028_models.GetLogUrlInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetLogUrlInMsaResponse:
+        """
+        @param request: GetLogUrlInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetLogUrlInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4076,14 +4953,19 @@
         )
 
     async def get_log_url_in_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.GetLogUrlInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetLogUrlInMsaResponse:
+        """
+        @param request: GetLogUrlInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetLogUrlInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4109,29 +4991,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_log_url_in_msa(
         self,
         request: m_paa_s20201028_models.GetLogUrlInMsaRequest,
     ) -> m_paa_s20201028_models.GetLogUrlInMsaResponse:
+        """
+        @param request: GetLogUrlInMsaRequest
+        @return: GetLogUrlInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_log_url_in_msa_with_options(request, runtime)
 
     async def get_log_url_in_msa_async(
         self,
         request: m_paa_s20201028_models.GetLogUrlInMsaRequest,
     ) -> m_paa_s20201028_models.GetLogUrlInMsaResponse:
+        """
+        @param request: GetLogUrlInMsaRequest
+        @return: GetLogUrlInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_log_url_in_msa_with_options_async(request, runtime)
 
     def get_mcube_file_token_with_options(
         self,
         request: m_paa_s20201028_models.GetMcubeFileTokenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeFileTokenResponse:
+        """
+        @param request: GetMcubeFileTokenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeFileTokenResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.onex_flag):
             body['OnexFlag'] = request.onex_flag
         if not UtilClient.is_unset(request.tenant_id):
@@ -4158,14 +5053,19 @@
         )
 
     async def get_mcube_file_token_with_options_async(
         self,
         request: m_paa_s20201028_models.GetMcubeFileTokenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeFileTokenResponse:
+        """
+        @param request: GetMcubeFileTokenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeFileTokenResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.onex_flag):
             body['OnexFlag'] = request.onex_flag
         if not UtilClient.is_unset(request.tenant_id):
@@ -4191,29 +5091,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_mcube_file_token(
         self,
         request: m_paa_s20201028_models.GetMcubeFileTokenRequest,
     ) -> m_paa_s20201028_models.GetMcubeFileTokenResponse:
+        """
+        @param request: GetMcubeFileTokenRequest
+        @return: GetMcubeFileTokenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_mcube_file_token_with_options(request, runtime)
 
     async def get_mcube_file_token_async(
         self,
         request: m_paa_s20201028_models.GetMcubeFileTokenRequest,
     ) -> m_paa_s20201028_models.GetMcubeFileTokenResponse:
+        """
+        @param request: GetMcubeFileTokenRequest
+        @return: GetMcubeFileTokenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_mcube_file_token_with_options_async(request, runtime)
 
     def get_mcube_nebula_resource_with_options(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeNebulaResourceResponse:
+        """
+        @param request: GetMcubeNebulaResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeNebulaResourceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4240,14 +5153,19 @@
         )
 
     async def get_mcube_nebula_resource_with_options_async(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaResourceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeNebulaResourceResponse:
+        """
+        @param request: GetMcubeNebulaResourceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeNebulaResourceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4273,29 +5191,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_mcube_nebula_resource(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaResourceRequest,
     ) -> m_paa_s20201028_models.GetMcubeNebulaResourceResponse:
+        """
+        @param request: GetMcubeNebulaResourceRequest
+        @return: GetMcubeNebulaResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_mcube_nebula_resource_with_options(request, runtime)
 
     async def get_mcube_nebula_resource_async(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaResourceRequest,
     ) -> m_paa_s20201028_models.GetMcubeNebulaResourceResponse:
+        """
+        @param request: GetMcubeNebulaResourceRequest
+        @return: GetMcubeNebulaResourceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_mcube_nebula_resource_with_options_async(request, runtime)
 
     def get_mcube_nebula_task_detail_with_options(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaTaskDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeNebulaTaskDetailResponse:
+        """
+        @param request: GetMcubeNebulaTaskDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeNebulaTaskDetailResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4322,14 +5253,19 @@
         )
 
     async def get_mcube_nebula_task_detail_with_options_async(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaTaskDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeNebulaTaskDetailResponse:
+        """
+        @param request: GetMcubeNebulaTaskDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeNebulaTaskDetailResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4355,29 +5291,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_mcube_nebula_task_detail(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaTaskDetailRequest,
     ) -> m_paa_s20201028_models.GetMcubeNebulaTaskDetailResponse:
+        """
+        @param request: GetMcubeNebulaTaskDetailRequest
+        @return: GetMcubeNebulaTaskDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_mcube_nebula_task_detail_with_options(request, runtime)
 
     async def get_mcube_nebula_task_detail_async(
         self,
         request: m_paa_s20201028_models.GetMcubeNebulaTaskDetailRequest,
     ) -> m_paa_s20201028_models.GetMcubeNebulaTaskDetailResponse:
+        """
+        @param request: GetMcubeNebulaTaskDetailRequest
+        @return: GetMcubeNebulaTaskDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_mcube_nebula_task_detail_with_options_async(request, runtime)
 
     def get_mcube_upgrade_package_info_with_options(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradePackageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeUpgradePackageInfoResponse:
+        """
+        @param request: GetMcubeUpgradePackageInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeUpgradePackageInfoResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.package_id):
             body['PackageId'] = request.package_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4404,14 +5353,19 @@
         )
 
     async def get_mcube_upgrade_package_info_with_options_async(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradePackageInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeUpgradePackageInfoResponse:
+        """
+        @param request: GetMcubeUpgradePackageInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeUpgradePackageInfoResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.package_id):
             body['PackageId'] = request.package_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4437,29 +5391,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_mcube_upgrade_package_info(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradePackageInfoRequest,
     ) -> m_paa_s20201028_models.GetMcubeUpgradePackageInfoResponse:
+        """
+        @param request: GetMcubeUpgradePackageInfoRequest
+        @return: GetMcubeUpgradePackageInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_mcube_upgrade_package_info_with_options(request, runtime)
 
     async def get_mcube_upgrade_package_info_async(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradePackageInfoRequest,
     ) -> m_paa_s20201028_models.GetMcubeUpgradePackageInfoResponse:
+        """
+        @param request: GetMcubeUpgradePackageInfoRequest
+        @return: GetMcubeUpgradePackageInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_mcube_upgrade_package_info_with_options_async(request, runtime)
 
     def get_mcube_upgrade_task_info_with_options(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradeTaskInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeUpgradeTaskInfoResponse:
+        """
+        @param request: GetMcubeUpgradeTaskInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeUpgradeTaskInfoResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4486,14 +5453,19 @@
         )
 
     async def get_mcube_upgrade_task_info_with_options_async(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradeTaskInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMcubeUpgradeTaskInfoResponse:
+        """
+        @param request: GetMcubeUpgradeTaskInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMcubeUpgradeTaskInfoResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4519,29 +5491,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_mcube_upgrade_task_info(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradeTaskInfoRequest,
     ) -> m_paa_s20201028_models.GetMcubeUpgradeTaskInfoResponse:
+        """
+        @param request: GetMcubeUpgradeTaskInfoRequest
+        @return: GetMcubeUpgradeTaskInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_mcube_upgrade_task_info_with_options(request, runtime)
 
     async def get_mcube_upgrade_task_info_async(
         self,
         request: m_paa_s20201028_models.GetMcubeUpgradeTaskInfoRequest,
     ) -> m_paa_s20201028_models.GetMcubeUpgradeTaskInfoResponse:
+        """
+        @param request: GetMcubeUpgradeTaskInfoRequest
+        @return: GetMcubeUpgradeTaskInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_mcube_upgrade_task_info_with_options_async(request, runtime)
 
     def get_mds_mini_config_with_options(
         self,
         request: m_paa_s20201028_models.GetMdsMiniConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMdsMiniConfigResponse:
+        """
+        @param request: GetMdsMiniConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMdsMiniConfigResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4568,14 +5553,19 @@
         )
 
     async def get_mds_mini_config_with_options_async(
         self,
         request: m_paa_s20201028_models.GetMdsMiniConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetMdsMiniConfigResponse:
+        """
+        @param request: GetMdsMiniConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMdsMiniConfigResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4601,29 +5591,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_mds_mini_config(
         self,
         request: m_paa_s20201028_models.GetMdsMiniConfigRequest,
     ) -> m_paa_s20201028_models.GetMdsMiniConfigResponse:
+        """
+        @param request: GetMdsMiniConfigRequest
+        @return: GetMdsMiniConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_mds_mini_config_with_options(request, runtime)
 
     async def get_mds_mini_config_async(
         self,
         request: m_paa_s20201028_models.GetMdsMiniConfigRequest,
     ) -> m_paa_s20201028_models.GetMdsMiniConfigResponse:
+        """
+        @param request: GetMdsMiniConfigRequest
+        @return: GetMdsMiniConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_mds_mini_config_with_options_async(request, runtime)
 
     def get_user_app_donwload_url_in_msa_with_options(
         self,
         request: m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaResponse:
+        """
+        @param request: GetUserAppDonwloadUrlInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserAppDonwloadUrlInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4650,14 +5653,19 @@
         )
 
     async def get_user_app_donwload_url_in_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaResponse:
+        """
+        @param request: GetUserAppDonwloadUrlInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserAppDonwloadUrlInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4683,29 +5691,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_app_donwload_url_in_msa(
         self,
         request: m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaRequest,
     ) -> m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaResponse:
+        """
+        @param request: GetUserAppDonwloadUrlInMsaRequest
+        @return: GetUserAppDonwloadUrlInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_app_donwload_url_in_msa_with_options(request, runtime)
 
     async def get_user_app_donwload_url_in_msa_async(
         self,
         request: m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaRequest,
     ) -> m_paa_s20201028_models.GetUserAppDonwloadUrlInMsaResponse:
+        """
+        @param request: GetUserAppDonwloadUrlInMsaRequest
+        @return: GetUserAppDonwloadUrlInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_app_donwload_url_in_msa_with_options_async(request, runtime)
 
     def get_user_app_enhance_process_in_msa_with_options(
         self,
         request: m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaResponse:
+        """
+        @param request: GetUserAppEnhanceProcessInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserAppEnhanceProcessInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4732,14 +5753,19 @@
         )
 
     async def get_user_app_enhance_process_in_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaResponse:
+        """
+        @param request: GetUserAppEnhanceProcessInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserAppEnhanceProcessInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4765,29 +5791,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_app_enhance_process_in_msa(
         self,
         request: m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaRequest,
     ) -> m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaResponse:
+        """
+        @param request: GetUserAppEnhanceProcessInMsaRequest
+        @return: GetUserAppEnhanceProcessInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_app_enhance_process_in_msa_with_options(request, runtime)
 
     async def get_user_app_enhance_process_in_msa_async(
         self,
         request: m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaRequest,
     ) -> m_paa_s20201028_models.GetUserAppEnhanceProcessInMsaResponse:
+        """
+        @param request: GetUserAppEnhanceProcessInMsaRequest
+        @return: GetUserAppEnhanceProcessInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_app_enhance_process_in_msa_with_options_async(request, runtime)
 
     def get_user_app_upload_process_in_msa_with_options(
         self,
         request: m_paa_s20201028_models.GetUserAppUploadProcessInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetUserAppUploadProcessInMsaResponse:
+        """
+        @param request: GetUserAppUploadProcessInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserAppUploadProcessInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4814,14 +5853,19 @@
         )
 
     async def get_user_app_upload_process_in_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.GetUserAppUploadProcessInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.GetUserAppUploadProcessInMsaResponse:
+        """
+        @param request: GetUserAppUploadProcessInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserAppUploadProcessInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -4847,28 +5891,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_app_upload_process_in_msa(
         self,
         request: m_paa_s20201028_models.GetUserAppUploadProcessInMsaRequest,
     ) -> m_paa_s20201028_models.GetUserAppUploadProcessInMsaResponse:
+        """
+        @param request: GetUserAppUploadProcessInMsaRequest
+        @return: GetUserAppUploadProcessInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_app_upload_process_in_msa_with_options(request, runtime)
 
     async def get_user_app_upload_process_in_msa_async(
         self,
         request: m_paa_s20201028_models.GetUserAppUploadProcessInMsaRequest,
     ) -> m_paa_s20201028_models.GetUserAppUploadProcessInMsaResponse:
+        """
+        @param request: GetUserAppUploadProcessInMsaRequest
+        @return: GetUserAppUploadProcessInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_app_upload_process_in_msa_with_options_async(request, runtime)
 
     def list_mapp_center_apps_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMappCenterAppsResponse:
+        """
+        @param request: ListMappCenterAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMappCenterAppsResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='ListMappCenterApps',
             version='2020-10-28',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4882,14 +5939,19 @@
             self.call_api(params, req, runtime)
         )
 
     async def list_mapp_center_apps_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMappCenterAppsResponse:
+        """
+        @param request: ListMappCenterAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMappCenterAppsResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='ListMappCenterApps',
             version='2020-10-28',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4900,25 +5962,36 @@
         )
         return TeaCore.from_map(
             m_paa_s20201028_models.ListMappCenterAppsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mapp_center_apps(self) -> m_paa_s20201028_models.ListMappCenterAppsResponse:
+        """
+        @return: ListMappCenterAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mapp_center_apps_with_options(runtime)
 
     async def list_mapp_center_apps_async(self) -> m_paa_s20201028_models.ListMappCenterAppsResponse:
+        """
+        @return: ListMappCenterAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mapp_center_apps_with_options_async(runtime)
 
     def list_mapp_center_workspaces_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMappCenterWorkspacesResponse:
+        """
+        @param request: ListMappCenterWorkspacesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMappCenterWorkspacesResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='ListMappCenterWorkspaces',
             version='2020-10-28',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4932,14 +6005,19 @@
             self.call_api(params, req, runtime)
         )
 
     async def list_mapp_center_workspaces_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMappCenterWorkspacesResponse:
+        """
+        @param request: ListMappCenterWorkspacesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMappCenterWorkspacesResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='ListMappCenterWorkspaces',
             version='2020-10-28',
             protocol='HTTPS',
             pathname='/',
             method='POST',
@@ -4950,26 +6028,37 @@
         )
         return TeaCore.from_map(
             m_paa_s20201028_models.ListMappCenterWorkspacesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mapp_center_workspaces(self) -> m_paa_s20201028_models.ListMappCenterWorkspacesResponse:
+        """
+        @return: ListMappCenterWorkspacesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mapp_center_workspaces_with_options(runtime)
 
     async def list_mapp_center_workspaces_async(self) -> m_paa_s20201028_models.ListMappCenterWorkspacesResponse:
+        """
+        @return: ListMappCenterWorkspacesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mapp_center_workspaces_with_options_async(runtime)
 
     def list_mcdp_aim_with_options(
         self,
         request: m_paa_s20201028_models.ListMcdpAimRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcdpAimResponse:
+        """
+        @param request: ListMcdpAimRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcdpAimResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.empty_tag):
             body['EmptyTag'] = request.empty_tag
         if not UtilClient.is_unset(request.keyword):
@@ -5010,14 +6099,19 @@
         )
 
     async def list_mcdp_aim_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcdpAimRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcdpAimResponse:
+        """
+        @param request: ListMcdpAimRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcdpAimResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.empty_tag):
             body['EmptyTag'] = request.empty_tag
         if not UtilClient.is_unset(request.keyword):
@@ -5057,29 +6151,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcdp_aim(
         self,
         request: m_paa_s20201028_models.ListMcdpAimRequest,
     ) -> m_paa_s20201028_models.ListMcdpAimResponse:
+        """
+        @param request: ListMcdpAimRequest
+        @return: ListMcdpAimResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcdp_aim_with_options(request, runtime)
 
     async def list_mcdp_aim_async(
         self,
         request: m_paa_s20201028_models.ListMcdpAimRequest,
     ) -> m_paa_s20201028_models.ListMcdpAimResponse:
+        """
+        @param request: ListMcdpAimRequest
+        @return: ListMcdpAimResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcdp_aim_with_options_async(request, runtime)
 
     def list_mcube_mini_apps_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeMiniAppsResponse:
+        """
+        @param request: ListMcubeMiniAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeMiniAppsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.keyword):
             body['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_num):
@@ -5110,14 +6217,19 @@
         )
 
     async def list_mcube_mini_apps_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeMiniAppsResponse:
+        """
+        @param request: ListMcubeMiniAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeMiniAppsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.keyword):
             body['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_num):
@@ -5147,29 +6259,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_mini_apps(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniAppsRequest,
     ) -> m_paa_s20201028_models.ListMcubeMiniAppsResponse:
+        """
+        @param request: ListMcubeMiniAppsRequest
+        @return: ListMcubeMiniAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_mini_apps_with_options(request, runtime)
 
     async def list_mcube_mini_apps_async(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniAppsRequest,
     ) -> m_paa_s20201028_models.ListMcubeMiniAppsResponse:
+        """
+        @param request: ListMcubeMiniAppsRequest
+        @return: ListMcubeMiniAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_mini_apps_with_options_async(request, runtime)
 
     def list_mcube_mini_packages_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniPackagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeMiniPackagesResponse:
+        """
+        @param request: ListMcubeMiniPackagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeMiniPackagesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.package_types):
@@ -5202,14 +6327,19 @@
         )
 
     async def list_mcube_mini_packages_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniPackagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeMiniPackagesResponse:
+        """
+        @param request: ListMcubeMiniPackagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeMiniPackagesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.package_types):
@@ -5241,29 +6371,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_mini_packages(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniPackagesRequest,
     ) -> m_paa_s20201028_models.ListMcubeMiniPackagesResponse:
+        """
+        @param request: ListMcubeMiniPackagesRequest
+        @return: ListMcubeMiniPackagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_mini_packages_with_options(request, runtime)
 
     async def list_mcube_mini_packages_async(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniPackagesRequest,
     ) -> m_paa_s20201028_models.ListMcubeMiniPackagesResponse:
+        """
+        @param request: ListMcubeMiniPackagesRequest
+        @return: ListMcubeMiniPackagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_mini_packages_with_options_async(request, runtime)
 
     def list_mcube_mini_tasks_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeMiniTasksResponse:
+        """
+        @param request: ListMcubeMiniTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeMiniTasksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -5290,14 +6433,19 @@
         )
 
     async def list_mcube_mini_tasks_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeMiniTasksResponse:
+        """
+        @param request: ListMcubeMiniTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeMiniTasksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -5323,29 +6471,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_mini_tasks(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniTasksRequest,
     ) -> m_paa_s20201028_models.ListMcubeMiniTasksResponse:
+        """
+        @param request: ListMcubeMiniTasksRequest
+        @return: ListMcubeMiniTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_mini_tasks_with_options(request, runtime)
 
     async def list_mcube_mini_tasks_async(
         self,
         request: m_paa_s20201028_models.ListMcubeMiniTasksRequest,
     ) -> m_paa_s20201028_models.ListMcubeMiniTasksResponse:
+        """
+        @param request: ListMcubeMiniTasksRequest
+        @return: ListMcubeMiniTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_mini_tasks_with_options_async(request, runtime)
 
     def list_mcube_nebula_apps_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeNebulaAppsResponse:
+        """
+        @param request: ListMcubeNebulaAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeNebulaAppsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.keyword):
             body['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_num):
@@ -5376,14 +6537,19 @@
         )
 
     async def list_mcube_nebula_apps_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeNebulaAppsResponse:
+        """
+        @param request: ListMcubeNebulaAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeNebulaAppsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.keyword):
             body['Keyword'] = request.keyword
         if not UtilClient.is_unset(request.page_num):
@@ -5413,29 +6579,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_nebula_apps(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaAppsRequest,
     ) -> m_paa_s20201028_models.ListMcubeNebulaAppsResponse:
+        """
+        @param request: ListMcubeNebulaAppsRequest
+        @return: ListMcubeNebulaAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_nebula_apps_with_options(request, runtime)
 
     async def list_mcube_nebula_apps_async(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaAppsRequest,
     ) -> m_paa_s20201028_models.ListMcubeNebulaAppsResponse:
+        """
+        @param request: ListMcubeNebulaAppsRequest
+        @return: ListMcubeNebulaAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_nebula_apps_with_options_async(request, runtime)
 
     def list_mcube_nebula_resources_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeNebulaResourcesResponse:
+        """
+        @param request: ListMcubeNebulaResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeNebulaResourcesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.page_num):
@@ -5466,14 +6645,19 @@
         )
 
     async def list_mcube_nebula_resources_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeNebulaResourcesResponse:
+        """
+        @param request: ListMcubeNebulaResourcesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeNebulaResourcesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.page_num):
@@ -5503,29 +6687,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_nebula_resources(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaResourcesRequest,
     ) -> m_paa_s20201028_models.ListMcubeNebulaResourcesResponse:
+        """
+        @param request: ListMcubeNebulaResourcesRequest
+        @return: ListMcubeNebulaResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_nebula_resources_with_options(request, runtime)
 
     async def list_mcube_nebula_resources_async(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaResourcesRequest,
     ) -> m_paa_s20201028_models.ListMcubeNebulaResourcesResponse:
+        """
+        @param request: ListMcubeNebulaResourcesRequest
+        @return: ListMcubeNebulaResourcesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_nebula_resources_with_options_async(request, runtime)
 
     def list_mcube_nebula_tasks_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeNebulaTasksResponse:
+        """
+        @param request: ListMcubeNebulaTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeNebulaTasksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -5552,14 +6749,19 @@
         )
 
     async def list_mcube_nebula_tasks_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeNebulaTasksResponse:
+        """
+        @param request: ListMcubeNebulaTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeNebulaTasksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -5585,29 +6787,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_nebula_tasks(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaTasksRequest,
     ) -> m_paa_s20201028_models.ListMcubeNebulaTasksResponse:
+        """
+        @param request: ListMcubeNebulaTasksRequest
+        @return: ListMcubeNebulaTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_nebula_tasks_with_options(request, runtime)
 
     async def list_mcube_nebula_tasks_async(
         self,
         request: m_paa_s20201028_models.ListMcubeNebulaTasksRequest,
     ) -> m_paa_s20201028_models.ListMcubeNebulaTasksResponse:
+        """
+        @param request: ListMcubeNebulaTasksRequest
+        @return: ListMcubeNebulaTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_nebula_tasks_with_options_async(request, runtime)
 
     def list_mcube_upgrade_packages_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradePackagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeUpgradePackagesResponse:
+        """
+        @param request: ListMcubeUpgradePackagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeUpgradePackagesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_num):
             body['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
@@ -5636,14 +6851,19 @@
         )
 
     async def list_mcube_upgrade_packages_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradePackagesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeUpgradePackagesResponse:
+        """
+        @param request: ListMcubeUpgradePackagesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeUpgradePackagesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_num):
             body['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
@@ -5671,29 +6891,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_upgrade_packages(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradePackagesRequest,
     ) -> m_paa_s20201028_models.ListMcubeUpgradePackagesResponse:
+        """
+        @param request: ListMcubeUpgradePackagesRequest
+        @return: ListMcubeUpgradePackagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_upgrade_packages_with_options(request, runtime)
 
     async def list_mcube_upgrade_packages_async(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradePackagesRequest,
     ) -> m_paa_s20201028_models.ListMcubeUpgradePackagesResponse:
+        """
+        @param request: ListMcubeUpgradePackagesRequest
+        @return: ListMcubeUpgradePackagesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_upgrade_packages_with_options_async(request, runtime)
 
     def list_mcube_upgrade_tasks_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradeTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeUpgradeTasksResponse:
+        """
+        @param request: ListMcubeUpgradeTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeUpgradeTasksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.package_id):
             body['PackageId'] = request.package_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -5720,14 +6953,19 @@
         )
 
     async def list_mcube_upgrade_tasks_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradeTasksRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeUpgradeTasksResponse:
+        """
+        @param request: ListMcubeUpgradeTasksRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeUpgradeTasksResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.package_id):
             body['PackageId'] = request.package_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -5753,29 +6991,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_upgrade_tasks(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradeTasksRequest,
     ) -> m_paa_s20201028_models.ListMcubeUpgradeTasksResponse:
+        """
+        @param request: ListMcubeUpgradeTasksRequest
+        @return: ListMcubeUpgradeTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_upgrade_tasks_with_options(request, runtime)
 
     async def list_mcube_upgrade_tasks_async(
         self,
         request: m_paa_s20201028_models.ListMcubeUpgradeTasksRequest,
     ) -> m_paa_s20201028_models.ListMcubeUpgradeTasksResponse:
+        """
+        @param request: ListMcubeUpgradeTasksRequest
+        @return: ListMcubeUpgradeTasksResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_upgrade_tasks_with_options_async(request, runtime)
 
     def list_mcube_whitelists_with_options(
         self,
         request: m_paa_s20201028_models.ListMcubeWhitelistsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeWhitelistsResponse:
+        """
+        @param request: ListMcubeWhitelistsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeWhitelistsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_num):
             body['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
@@ -5806,14 +7057,19 @@
         )
 
     async def list_mcube_whitelists_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMcubeWhitelistsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMcubeWhitelistsResponse:
+        """
+        @param request: ListMcubeWhitelistsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMcubeWhitelistsResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_num):
             body['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
@@ -5843,29 +7099,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mcube_whitelists(
         self,
         request: m_paa_s20201028_models.ListMcubeWhitelistsRequest,
     ) -> m_paa_s20201028_models.ListMcubeWhitelistsResponse:
+        """
+        @param request: ListMcubeWhitelistsRequest
+        @return: ListMcubeWhitelistsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mcube_whitelists_with_options(request, runtime)
 
     async def list_mcube_whitelists_async(
         self,
         request: m_paa_s20201028_models.ListMcubeWhitelistsRequest,
     ) -> m_paa_s20201028_models.ListMcubeWhitelistsResponse:
+        """
+        @param request: ListMcubeWhitelistsRequest
+        @return: ListMcubeWhitelistsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mcube_whitelists_with_options_async(request, runtime)
 
     def list_mgs_api_with_options(
         self,
         request: m_paa_s20201028_models.ListMgsApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMgsApiResponse:
+        """
+        @param request: ListMgsApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMgsApiResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_status):
             body['ApiStatus'] = request.api_status
         if not UtilClient.is_unset(request.api_type):
             body['ApiType'] = request.api_type
         if not UtilClient.is_unset(request.app_id):
@@ -5916,14 +7185,19 @@
         )
 
     async def list_mgs_api_with_options_async(
         self,
         request: m_paa_s20201028_models.ListMgsApiRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.ListMgsApiResponse:
+        """
+        @param request: ListMgsApiRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListMgsApiResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_status):
             body['ApiStatus'] = request.api_status
         if not UtilClient.is_unset(request.api_type):
             body['ApiType'] = request.api_type
         if not UtilClient.is_unset(request.app_id):
@@ -5973,29 +7247,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_mgs_api(
         self,
         request: m_paa_s20201028_models.ListMgsApiRequest,
     ) -> m_paa_s20201028_models.ListMgsApiResponse:
+        """
+        @param request: ListMgsApiRequest
+        @return: ListMgsApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_mgs_api_with_options(request, runtime)
 
     async def list_mgs_api_async(
         self,
         request: m_paa_s20201028_models.ListMgsApiRequest,
     ) -> m_paa_s20201028_models.ListMgsApiResponse:
+        """
+        @param request: ListMgsApiRequest
+        @return: ListMgsApiResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_mgs_api_with_options_async(request, runtime)
 
     def log_msa_query_with_options(
         self,
         request: m_paa_s20201028_models.LogMsaQueryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.LogMsaQueryResponse:
+        """
+        @param request: LogMsaQueryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: LogMsaQueryResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.onex_flag):
@@ -6024,14 +7311,19 @@
         )
 
     async def log_msa_query_with_options_async(
         self,
         request: m_paa_s20201028_models.LogMsaQueryRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.LogMsaQueryResponse:
+        """
+        @param request: LogMsaQueryRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: LogMsaQueryResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.onex_flag):
@@ -6059,29 +7351,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def log_msa_query(
         self,
         request: m_paa_s20201028_models.LogMsaQueryRequest,
     ) -> m_paa_s20201028_models.LogMsaQueryResponse:
+        """
+        @param request: LogMsaQueryRequest
+        @return: LogMsaQueryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.log_msa_query_with_options(request, runtime)
 
     async def log_msa_query_async(
         self,
         request: m_paa_s20201028_models.LogMsaQueryRequest,
     ) -> m_paa_s20201028_models.LogMsaQueryResponse:
+        """
+        @param request: LogMsaQueryRequest
+        @return: LogMsaQueryResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.log_msa_query_with_options_async(request, runtime)
 
     def m_trsocrservice_with_options(
         self,
         request: m_paa_s20201028_models.MTRSOCRServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.MTRSOCRServiceResponse:
+        """
+        @summary OCR通用接口
+        
+        @param request: MTRSOCRServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MTRSOCRServiceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.image_raw):
             body['ImageRaw'] = request.image_raw
         if not UtilClient.is_unset(request.mask):
@@ -6112,14 +7419,21 @@
         )
 
     async def m_trsocrservice_with_options_async(
         self,
         request: m_paa_s20201028_models.MTRSOCRServiceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.MTRSOCRServiceResponse:
+        """
+        @summary OCR通用接口
+        
+        @param request: MTRSOCRServiceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: MTRSOCRServiceResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.image_raw):
             body['ImageRaw'] = request.image_raw
         if not UtilClient.is_unset(request.mask):
@@ -6149,29 +7463,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def m_trsocrservice(
         self,
         request: m_paa_s20201028_models.MTRSOCRServiceRequest,
     ) -> m_paa_s20201028_models.MTRSOCRServiceResponse:
+        """
+        @summary OCR通用接口
+        
+        @param request: MTRSOCRServiceRequest
+        @return: MTRSOCRServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.m_trsocrservice_with_options(request, runtime)
 
     async def m_trsocrservice_async(
         self,
         request: m_paa_s20201028_models.MTRSOCRServiceRequest,
     ) -> m_paa_s20201028_models.MTRSOCRServiceResponse:
+        """
+        @summary OCR通用接口
+        
+        @param request: MTRSOCRServiceRequest
+        @return: MTRSOCRServiceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.m_trsocrservice_with_options_async(request, runtime)
 
     def open_api_add_active_code_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiAddActiveCodeResponse:
+        """
+        @summary 新增主扫码
+        
+        @param request: OpenApiAddActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiAddActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_add_active_code_req_json_str):
             body['MpaasMqcpOpenApiAddActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_add_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6198,14 +7531,21 @@
         )
 
     async def open_api_add_active_code_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiAddActiveCodeResponse:
+        """
+        @summary 新增主扫码
+        
+        @param request: OpenApiAddActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiAddActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_add_active_code_req_json_str):
             body['MpaasMqcpOpenApiAddActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_add_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6231,29 +7571,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_add_active_code(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiAddActiveCodeResponse:
+        """
+        @summary 新增主扫码
+        
+        @param request: OpenApiAddActiveCodeRequest
+        @return: OpenApiAddActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_add_active_code_with_options(request, runtime)
 
     async def open_api_add_active_code_async(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiAddActiveCodeResponse:
+        """
+        @summary 新增主扫码
+        
+        @param request: OpenApiAddActiveCodeRequest
+        @return: OpenApiAddActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_add_active_code_with_options_async(request, runtime)
 
     def open_api_add_active_scene_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiAddActiveSceneResponse:
+        """
+        @summary 新增场景
+        
+        @param request: OpenApiAddActiveSceneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiAddActiveSceneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_add_active_scene_req_json_str):
             body['MpaasMqcpOpenApiAddActiveSceneReqJsonStr'] = request.mpaas_mqcp_open_api_add_active_scene_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6280,14 +7639,21 @@
         )
 
     async def open_api_add_active_scene_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiAddActiveSceneResponse:
+        """
+        @summary 新增场景
+        
+        @param request: OpenApiAddActiveSceneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiAddActiveSceneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_add_active_scene_req_json_str):
             body['MpaasMqcpOpenApiAddActiveSceneReqJsonStr'] = request.mpaas_mqcp_open_api_add_active_scene_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6313,29 +7679,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_add_active_scene(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveSceneRequest,
     ) -> m_paa_s20201028_models.OpenApiAddActiveSceneResponse:
+        """
+        @summary 新增场景
+        
+        @param request: OpenApiAddActiveSceneRequest
+        @return: OpenApiAddActiveSceneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_add_active_scene_with_options(request, runtime)
 
     async def open_api_add_active_scene_async(
         self,
         request: m_paa_s20201028_models.OpenApiAddActiveSceneRequest,
     ) -> m_paa_s20201028_models.OpenApiAddActiveSceneResponse:
+        """
+        @summary 新增场景
+        
+        @param request: OpenApiAddActiveSceneRequest
+        @return: OpenApiAddActiveSceneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_add_active_scene_with_options_async(request, runtime)
 
     def open_api_callback_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiCallbackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiCallbackResponse:
+        """
+        @summary 用户注册
+        
+        @param request: OpenApiCallbackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiCallbackResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_callback_request_json_str):
             body['MpaasMqcpOpenApiCallbackRequestJsonStr'] = request.mpaas_mqcp_open_api_callback_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6362,14 +7747,21 @@
         )
 
     async def open_api_callback_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiCallbackRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiCallbackResponse:
+        """
+        @summary 用户注册
+        
+        @param request: OpenApiCallbackRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiCallbackResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_callback_request_json_str):
             body['MpaasMqcpOpenApiCallbackRequestJsonStr'] = request.mpaas_mqcp_open_api_callback_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6395,29 +7787,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_callback(
         self,
         request: m_paa_s20201028_models.OpenApiCallbackRequest,
     ) -> m_paa_s20201028_models.OpenApiCallbackResponse:
+        """
+        @summary 用户注册
+        
+        @param request: OpenApiCallbackRequest
+        @return: OpenApiCallbackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_callback_with_options(request, runtime)
 
     async def open_api_callback_async(
         self,
         request: m_paa_s20201028_models.OpenApiCallbackRequest,
     ) -> m_paa_s20201028_models.OpenApiCallbackResponse:
+        """
+        @summary 用户注册
+        
+        @param request: OpenApiCallbackRequest
+        @return: OpenApiCallbackResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_callback_with_options_async(request, runtime)
 
     def open_api_decode_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiDecodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiDecodeResponse:
+        """
+        @summary 解码
+        
+        @param request: OpenApiDecodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiDecodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_decode_request_json_str):
             body['MpaasMqcpOpenApiDecodeRequestJsonStr'] = request.mpaas_mqcp_open_api_decode_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6444,14 +7855,21 @@
         )
 
     async def open_api_decode_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiDecodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiDecodeResponse:
+        """
+        @summary 解码
+        
+        @param request: OpenApiDecodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiDecodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_decode_request_json_str):
             body['MpaasMqcpOpenApiDecodeRequestJsonStr'] = request.mpaas_mqcp_open_api_decode_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6477,29 +7895,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_decode(
         self,
         request: m_paa_s20201028_models.OpenApiDecodeRequest,
     ) -> m_paa_s20201028_models.OpenApiDecodeResponse:
+        """
+        @summary 解码
+        
+        @param request: OpenApiDecodeRequest
+        @return: OpenApiDecodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_decode_with_options(request, runtime)
 
     async def open_api_decode_async(
         self,
         request: m_paa_s20201028_models.OpenApiDecodeRequest,
     ) -> m_paa_s20201028_models.OpenApiDecodeResponse:
+        """
+        @summary 解码
+        
+        @param request: OpenApiDecodeRequest
+        @return: OpenApiDecodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_decode_with_options_async(request, runtime)
 
     def open_api_delete_active_code_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiDeleteActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiDeleteActiveCodeResponse:
+        """
+        @summary 删除主扫码
+        
+        @param request: OpenApiDeleteActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiDeleteActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_delete_active_code_req_json_str):
             body['MpaasMqcpOpenApiDeleteActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_delete_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6526,14 +7963,21 @@
         )
 
     async def open_api_delete_active_code_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiDeleteActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiDeleteActiveCodeResponse:
+        """
+        @summary 删除主扫码
+        
+        @param request: OpenApiDeleteActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiDeleteActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_delete_active_code_req_json_str):
             body['MpaasMqcpOpenApiDeleteActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_delete_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6559,29 +8003,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_delete_active_code(
         self,
         request: m_paa_s20201028_models.OpenApiDeleteActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiDeleteActiveCodeResponse:
+        """
+        @summary 删除主扫码
+        
+        @param request: OpenApiDeleteActiveCodeRequest
+        @return: OpenApiDeleteActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_delete_active_code_with_options(request, runtime)
 
     async def open_api_delete_active_code_async(
         self,
         request: m_paa_s20201028_models.OpenApiDeleteActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiDeleteActiveCodeResponse:
+        """
+        @summary 删除主扫码
+        
+        @param request: OpenApiDeleteActiveCodeRequest
+        @return: OpenApiDeleteActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_delete_active_code_with_options_async(request, runtime)
 
     def open_api_encode_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiEncodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiEncodeResponse:
+        """
+        @summary 编码
+        
+        @param request: OpenApiEncodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiEncodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_encode_request_json_str):
             body['MpaasMqcpOpenApiEncodeRequestJsonStr'] = request.mpaas_mqcp_open_api_encode_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6608,14 +8071,21 @@
         )
 
     async def open_api_encode_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiEncodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiEncodeResponse:
+        """
+        @summary 编码
+        
+        @param request: OpenApiEncodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiEncodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_encode_request_json_str):
             body['MpaasMqcpOpenApiEncodeRequestJsonStr'] = request.mpaas_mqcp_open_api_encode_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6641,29 +8111,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_encode(
         self,
         request: m_paa_s20201028_models.OpenApiEncodeRequest,
     ) -> m_paa_s20201028_models.OpenApiEncodeResponse:
+        """
+        @summary 编码
+        
+        @param request: OpenApiEncodeRequest
+        @return: OpenApiEncodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_encode_with_options(request, runtime)
 
     async def open_api_encode_async(
         self,
         request: m_paa_s20201028_models.OpenApiEncodeRequest,
     ) -> m_paa_s20201028_models.OpenApiEncodeResponse:
+        """
+        @summary 编码
+        
+        @param request: OpenApiEncodeRequest
+        @return: OpenApiEncodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_encode_with_options_async(request, runtime)
 
     def open_api_query_active_code_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveCodeResponse:
+        """
+        @summary 主扫码查询
+        
+        @param request: OpenApiQueryActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiQueryActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_query_active_code_req_json_str):
             body['MpaasMqcpOpenApiQueryActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_query_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6690,14 +8179,21 @@
         )
 
     async def open_api_query_active_code_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveCodeResponse:
+        """
+        @summary 主扫码查询
+        
+        @param request: OpenApiQueryActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiQueryActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_query_active_code_req_json_str):
             body['MpaasMqcpOpenApiQueryActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_query_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6723,29 +8219,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_query_active_code(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveCodeResponse:
+        """
+        @summary 主扫码查询
+        
+        @param request: OpenApiQueryActiveCodeRequest
+        @return: OpenApiQueryActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_query_active_code_with_options(request, runtime)
 
     async def open_api_query_active_code_async(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveCodeResponse:
+        """
+        @summary 主扫码查询
+        
+        @param request: OpenApiQueryActiveCodeRequest
+        @return: OpenApiQueryActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_query_active_code_with_options_async(request, runtime)
 
     def open_api_query_active_scene_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveSceneResponse:
+        """
+        @summary 查询场景
+        
+        @param request: OpenApiQueryActiveSceneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiQueryActiveSceneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_query_active_scene_req_json_str):
             body['MpaasMqcpOpenApiQueryActiveSceneReqJsonStr'] = request.mpaas_mqcp_open_api_query_active_scene_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6772,14 +8287,21 @@
         )
 
     async def open_api_query_active_scene_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveSceneResponse:
+        """
+        @summary 查询场景
+        
+        @param request: OpenApiQueryActiveSceneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiQueryActiveSceneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_query_active_scene_req_json_str):
             body['MpaasMqcpOpenApiQueryActiveSceneReqJsonStr'] = request.mpaas_mqcp_open_api_query_active_scene_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6805,29 +8327,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_query_active_scene(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveSceneRequest,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveSceneResponse:
+        """
+        @summary 查询场景
+        
+        @param request: OpenApiQueryActiveSceneRequest
+        @return: OpenApiQueryActiveSceneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_query_active_scene_with_options(request, runtime)
 
     async def open_api_query_active_scene_async(
         self,
         request: m_paa_s20201028_models.OpenApiQueryActiveSceneRequest,
     ) -> m_paa_s20201028_models.OpenApiQueryActiveSceneResponse:
+        """
+        @summary 查询场景
+        
+        @param request: OpenApiQueryActiveSceneRequest
+        @return: OpenApiQueryActiveSceneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_query_active_scene_with_options_async(request, runtime)
 
     def open_api_unique_encode_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiUniqueEncodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiUniqueEncodeResponse:
+        """
+        @summary 生成唯一被扫码
+        
+        @param request: OpenApiUniqueEncodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiUniqueEncodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_unique_encode_request_json_str):
             body['MpaasMqcpOpenApiUniqueEncodeRequestJsonStr'] = request.mpaas_mqcp_open_api_unique_encode_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6854,14 +8395,21 @@
         )
 
     async def open_api_unique_encode_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiUniqueEncodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiUniqueEncodeResponse:
+        """
+        @summary 生成唯一被扫码
+        
+        @param request: OpenApiUniqueEncodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiUniqueEncodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_unique_encode_request_json_str):
             body['MpaasMqcpOpenApiUniqueEncodeRequestJsonStr'] = request.mpaas_mqcp_open_api_unique_encode_request_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6887,29 +8435,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_unique_encode(
         self,
         request: m_paa_s20201028_models.OpenApiUniqueEncodeRequest,
     ) -> m_paa_s20201028_models.OpenApiUniqueEncodeResponse:
+        """
+        @summary 生成唯一被扫码
+        
+        @param request: OpenApiUniqueEncodeRequest
+        @return: OpenApiUniqueEncodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_unique_encode_with_options(request, runtime)
 
     async def open_api_unique_encode_async(
         self,
         request: m_paa_s20201028_models.OpenApiUniqueEncodeRequest,
     ) -> m_paa_s20201028_models.OpenApiUniqueEncodeResponse:
+        """
+        @summary 生成唯一被扫码
+        
+        @param request: OpenApiUniqueEncodeRequest
+        @return: OpenApiUniqueEncodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_unique_encode_with_options_async(request, runtime)
 
     def open_api_update_active_code_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveCodeResponse:
+        """
+        @summary 更新主扫码
+        
+        @param request: OpenApiUpdateActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiUpdateActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_update_active_code_req_json_str):
             body['MpaasMqcpOpenApiUpdateActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_update_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6936,14 +8503,21 @@
         )
 
     async def open_api_update_active_code_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveCodeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveCodeResponse:
+        """
+        @summary 更新主扫码
+        
+        @param request: OpenApiUpdateActiveCodeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiUpdateActiveCodeResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_update_active_code_req_json_str):
             body['MpaasMqcpOpenApiUpdateActiveCodeReqJsonStr'] = request.mpaas_mqcp_open_api_update_active_code_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -6969,29 +8543,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_update_active_code(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveCodeResponse:
+        """
+        @summary 更新主扫码
+        
+        @param request: OpenApiUpdateActiveCodeRequest
+        @return: OpenApiUpdateActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_update_active_code_with_options(request, runtime)
 
     async def open_api_update_active_code_async(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveCodeRequest,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveCodeResponse:
+        """
+        @summary 更新主扫码
+        
+        @param request: OpenApiUpdateActiveCodeRequest
+        @return: OpenApiUpdateActiveCodeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_update_active_code_with_options_async(request, runtime)
 
     def open_api_update_active_scene_with_options(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveSceneResponse:
+        """
+        @summary 更新场景
+        
+        @param request: OpenApiUpdateActiveSceneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiUpdateActiveSceneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_update_active_scene_req_json_str):
             body['MpaasMqcpOpenApiUpdateActiveSceneReqJsonStr'] = request.mpaas_mqcp_open_api_update_active_scene_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -7018,14 +8611,21 @@
         )
 
     async def open_api_update_active_scene_with_options_async(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveSceneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveSceneResponse:
+        """
+        @summary 更新场景
+        
+        @param request: OpenApiUpdateActiveSceneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: OpenApiUpdateActiveSceneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mqcp_open_api_update_active_scene_req_json_str):
             body['MpaasMqcpOpenApiUpdateActiveSceneReqJsonStr'] = request.mpaas_mqcp_open_api_update_active_scene_req_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -7051,29 +8651,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def open_api_update_active_scene(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveSceneRequest,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveSceneResponse:
+        """
+        @summary 更新场景
+        
+        @param request: OpenApiUpdateActiveSceneRequest
+        @return: OpenApiUpdateActiveSceneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.open_api_update_active_scene_with_options(request, runtime)
 
     async def open_api_update_active_scene_async(
         self,
         request: m_paa_s20201028_models.OpenApiUpdateActiveSceneRequest,
     ) -> m_paa_s20201028_models.OpenApiUpdateActiveSceneResponse:
+        """
+        @summary 更新场景
+        
+        @param request: OpenApiUpdateActiveSceneRequest
+        @return: OpenApiUpdateActiveSceneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.open_api_update_active_scene_with_options_async(request, runtime)
 
     def push_bind_with_options(
         self,
         request: m_paa_s20201028_models.PushBindRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushBindResponse:
+        """
+        @param request: PushBindRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushBindResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.delivery_token):
             body['DeliveryToken'] = request.delivery_token
         if not UtilClient.is_unset(request.os_type):
@@ -7104,14 +8721,19 @@
         )
 
     async def push_bind_with_options_async(
         self,
         request: m_paa_s20201028_models.PushBindRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushBindResponse:
+        """
+        @param request: PushBindRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushBindResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.delivery_token):
             body['DeliveryToken'] = request.delivery_token
         if not UtilClient.is_unset(request.os_type):
@@ -7141,29 +8763,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_bind(
         self,
         request: m_paa_s20201028_models.PushBindRequest,
     ) -> m_paa_s20201028_models.PushBindResponse:
+        """
+        @param request: PushBindRequest
+        @return: PushBindResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_bind_with_options(request, runtime)
 
     async def push_bind_async(
         self,
         request: m_paa_s20201028_models.PushBindRequest,
     ) -> m_paa_s20201028_models.PushBindResponse:
+        """
+        @param request: PushBindRequest
+        @return: PushBindResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_bind_with_options_async(request, runtime)
 
     def push_broadcast_with_options(
         self,
         tmp_req: m_paa_s20201028_models.PushBroadcastRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushBroadcastResponse:
+        """
+        @param tmp_req: PushBroadcastRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushBroadcastResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushBroadcastShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.android_channel):
@@ -7230,14 +8865,19 @@
         )
 
     async def push_broadcast_with_options_async(
         self,
         tmp_req: m_paa_s20201028_models.PushBroadcastRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushBroadcastResponse:
+        """
+        @param tmp_req: PushBroadcastRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushBroadcastResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushBroadcastShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.android_channel):
@@ -7303,29 +8943,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_broadcast(
         self,
         request: m_paa_s20201028_models.PushBroadcastRequest,
     ) -> m_paa_s20201028_models.PushBroadcastResponse:
+        """
+        @param request: PushBroadcastRequest
+        @return: PushBroadcastResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_broadcast_with_options(request, runtime)
 
     async def push_broadcast_async(
         self,
         request: m_paa_s20201028_models.PushBroadcastRequest,
     ) -> m_paa_s20201028_models.PushBroadcastResponse:
+        """
+        @param request: PushBroadcastRequest
+        @return: PushBroadcastResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_broadcast_with_options_async(request, runtime)
 
     def push_multiple_with_options(
         self,
         tmp_req: m_paa_s20201028_models.PushMultipleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushMultipleResponse:
+        """
+        @param tmp_req: PushMultipleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushMultipleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushMultipleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.activity_content_state):
@@ -7388,14 +9041,19 @@
         )
 
     async def push_multiple_with_options_async(
         self,
         tmp_req: m_paa_s20201028_models.PushMultipleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushMultipleResponse:
+        """
+        @param tmp_req: PushMultipleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushMultipleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushMultipleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.activity_content_state):
@@ -7457,29 +9115,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_multiple(
         self,
         request: m_paa_s20201028_models.PushMultipleRequest,
     ) -> m_paa_s20201028_models.PushMultipleResponse:
+        """
+        @param request: PushMultipleRequest
+        @return: PushMultipleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_multiple_with_options(request, runtime)
 
     async def push_multiple_async(
         self,
         request: m_paa_s20201028_models.PushMultipleRequest,
     ) -> m_paa_s20201028_models.PushMultipleResponse:
+        """
+        @param request: PushMultipleRequest
+        @return: PushMultipleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_multiple_with_options_async(request, runtime)
 
     def push_report_with_options(
         self,
         request: m_paa_s20201028_models.PushReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushReportResponse:
+        """
+        @param request: PushReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_version):
             body['AppVersion'] = request.app_version
         if not UtilClient.is_unset(request.channel):
@@ -7524,14 +9195,19 @@
         )
 
     async def push_report_with_options_async(
         self,
         request: m_paa_s20201028_models.PushReportRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushReportResponse:
+        """
+        @param request: PushReportRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushReportResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_version):
             body['AppVersion'] = request.app_version
         if not UtilClient.is_unset(request.channel):
@@ -7575,29 +9251,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_report(
         self,
         request: m_paa_s20201028_models.PushReportRequest,
     ) -> m_paa_s20201028_models.PushReportResponse:
+        """
+        @param request: PushReportRequest
+        @return: PushReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_report_with_options(request, runtime)
 
     async def push_report_async(
         self,
         request: m_paa_s20201028_models.PushReportRequest,
     ) -> m_paa_s20201028_models.PushReportResponse:
+        """
+        @param request: PushReportRequest
+        @return: PushReportResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_report_with_options_async(request, runtime)
 
     def push_simple_with_options(
         self,
         tmp_req: m_paa_s20201028_models.PushSimpleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushSimpleResponse:
+        """
+        @param tmp_req: PushSimpleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushSimpleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushSimpleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.activity_content_state):
@@ -7678,14 +9367,19 @@
         )
 
     async def push_simple_with_options_async(
         self,
         tmp_req: m_paa_s20201028_models.PushSimpleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushSimpleResponse:
+        """
+        @param tmp_req: PushSimpleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushSimpleResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushSimpleShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.activity_content_state):
@@ -7765,29 +9459,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_simple(
         self,
         request: m_paa_s20201028_models.PushSimpleRequest,
     ) -> m_paa_s20201028_models.PushSimpleResponse:
+        """
+        @param request: PushSimpleRequest
+        @return: PushSimpleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_simple_with_options(request, runtime)
 
     async def push_simple_async(
         self,
         request: m_paa_s20201028_models.PushSimpleRequest,
     ) -> m_paa_s20201028_models.PushSimpleResponse:
+        """
+        @param request: PushSimpleRequest
+        @return: PushSimpleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_simple_with_options_async(request, runtime)
 
     def push_template_with_options(
         self,
         tmp_req: m_paa_s20201028_models.PushTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushTemplateResponse:
+        """
+        @param tmp_req: PushTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.activity_content_state):
@@ -7860,14 +9567,19 @@
         )
 
     async def push_template_with_options_async(
         self,
         tmp_req: m_paa_s20201028_models.PushTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushTemplateResponse:
+        """
+        @param tmp_req: PushTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = m_paa_s20201028_models.PushTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.third_channel_category):
             request.third_channel_category_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.third_channel_category, 'ThirdChannelCategory', 'json')
         body = {}
         if not UtilClient.is_unset(request.activity_content_state):
@@ -7939,29 +9651,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_template(
         self,
         request: m_paa_s20201028_models.PushTemplateRequest,
     ) -> m_paa_s20201028_models.PushTemplateResponse:
+        """
+        @param request: PushTemplateRequest
+        @return: PushTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_template_with_options(request, runtime)
 
     async def push_template_async(
         self,
         request: m_paa_s20201028_models.PushTemplateRequest,
     ) -> m_paa_s20201028_models.PushTemplateResponse:
+        """
+        @param request: PushTemplateRequest
+        @return: PushTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_template_with_options_async(request, runtime)
 
     def push_un_bind_with_options(
         self,
         request: m_paa_s20201028_models.PushUnBindRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushUnBindResponse:
+        """
+        @param request: PushUnBindRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushUnBindResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.delivery_token):
             body['DeliveryToken'] = request.delivery_token
         if not UtilClient.is_unset(request.user_id):
@@ -7988,14 +9713,19 @@
         )
 
     async def push_un_bind_with_options_async(
         self,
         request: m_paa_s20201028_models.PushUnBindRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.PushUnBindResponse:
+        """
+        @param request: PushUnBindRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: PushUnBindResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.delivery_token):
             body['DeliveryToken'] = request.delivery_token
         if not UtilClient.is_unset(request.user_id):
@@ -8021,29 +9751,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def push_un_bind(
         self,
         request: m_paa_s20201028_models.PushUnBindRequest,
     ) -> m_paa_s20201028_models.PushUnBindResponse:
+        """
+        @param request: PushUnBindRequest
+        @return: PushUnBindResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.push_un_bind_with_options(request, runtime)
 
     async def push_un_bind_async(
         self,
         request: m_paa_s20201028_models.PushUnBindRequest,
     ) -> m_paa_s20201028_models.PushUnBindResponse:
+        """
+        @param request: PushUnBindRequest
+        @return: PushUnBindResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.push_un_bind_with_options_async(request, runtime)
 
     def query_info_from_mdp_with_options(
         self,
         request: m_paa_s20201028_models.QueryInfoFromMdpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryInfoFromMdpResponse:
+        """
+        @summary 查询Device+服务的
+        
+        @param request: QueryInfoFromMdpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInfoFromMdpResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mobile):
             body['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.mobile_md_5):
@@ -8076,14 +9821,21 @@
         )
 
     async def query_info_from_mdp_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryInfoFromMdpRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryInfoFromMdpResponse:
+        """
+        @summary 查询Device+服务的
+        
+        @param request: QueryInfoFromMdpRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryInfoFromMdpResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mobile):
             body['Mobile'] = request.mobile
         if not UtilClient.is_unset(request.mobile_md_5):
@@ -8115,29 +9867,150 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_info_from_mdp(
         self,
         request: m_paa_s20201028_models.QueryInfoFromMdpRequest,
     ) -> m_paa_s20201028_models.QueryInfoFromMdpResponse:
+        """
+        @summary 查询Device+服务的
+        
+        @param request: QueryInfoFromMdpRequest
+        @return: QueryInfoFromMdpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_info_from_mdp_with_options(request, runtime)
 
     async def query_info_from_mdp_async(
         self,
         request: m_paa_s20201028_models.QueryInfoFromMdpRequest,
     ) -> m_paa_s20201028_models.QueryInfoFromMdpResponse:
+        """
+        @summary 查询Device+服务的
+        
+        @param request: QueryInfoFromMdpRequest
+        @return: QueryInfoFromMdpResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_info_from_mdp_with_options_async(request, runtime)
 
+    def query_link_with_options(
+        self,
+        request: m_paa_s20201028_models.QueryLinkRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> m_paa_s20201028_models.QueryLinkResponse:
+        """
+        @summary 查询短链
+        
+        @param request: QueryLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryLinkResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_id):
+            body['AppId'] = request.app_id
+        if not UtilClient.is_unset(request.url):
+            body['Url'] = request.url
+        if not UtilClient.is_unset(request.workspace_id):
+            body['WorkspaceId'] = request.workspace_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryLink',
+            version='2020-10-28',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            m_paa_s20201028_models.QueryLinkResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def query_link_with_options_async(
+        self,
+        request: m_paa_s20201028_models.QueryLinkRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> m_paa_s20201028_models.QueryLinkResponse:
+        """
+        @summary 查询短链
+        
+        @param request: QueryLinkRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryLinkResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.app_id):
+            body['AppId'] = request.app_id
+        if not UtilClient.is_unset(request.url):
+            body['Url'] = request.url
+        if not UtilClient.is_unset(request.workspace_id):
+            body['WorkspaceId'] = request.workspace_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='QueryLink',
+            version='2020-10-28',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            m_paa_s20201028_models.QueryLinkResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def query_link(
+        self,
+        request: m_paa_s20201028_models.QueryLinkRequest,
+    ) -> m_paa_s20201028_models.QueryLinkResponse:
+        """
+        @summary 查询短链
+        
+        @param request: QueryLinkRequest
+        @return: QueryLinkResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.query_link_with_options(request, runtime)
+
+    async def query_link_async(
+        self,
+        request: m_paa_s20201028_models.QueryLinkRequest,
+    ) -> m_paa_s20201028_models.QueryLinkResponse:
+        """
+        @summary 查询短链
+        
+        @param request: QueryLinkRequest
+        @return: QueryLinkResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.query_link_with_options_async(request, runtime)
+
     def query_mapp_center_app_with_options(
         self,
         request: m_paa_s20201028_models.QueryMappCenterAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMappCenterAppResponse:
+        """
+        @param request: QueryMappCenterAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMappCenterAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.workspace_id):
             body['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
@@ -8160,14 +10033,19 @@
         )
 
     async def query_mapp_center_app_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMappCenterAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMappCenterAppResponse:
+        """
+        @param request: QueryMappCenterAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMappCenterAppResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.workspace_id):
             body['WorkspaceId'] = request.workspace_id
         req = open_api_models.OpenApiRequest(
@@ -8189,29 +10067,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mapp_center_app(
         self,
         request: m_paa_s20201028_models.QueryMappCenterAppRequest,
     ) -> m_paa_s20201028_models.QueryMappCenterAppResponse:
+        """
+        @param request: QueryMappCenterAppRequest
+        @return: QueryMappCenterAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mapp_center_app_with_options(request, runtime)
 
     async def query_mapp_center_app_async(
         self,
         request: m_paa_s20201028_models.QueryMappCenterAppRequest,
     ) -> m_paa_s20201028_models.QueryMappCenterAppResponse:
+        """
+        @param request: QueryMappCenterAppRequest
+        @return: QueryMappCenterAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mapp_center_app_with_options_async(request, runtime)
 
     def query_mcdp_aim_with_options(
         self,
         request: m_paa_s20201028_models.QueryMcdpAimRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcdpAimResponse:
+        """
+        @param request: QueryMcdpAimRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcdpAimResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8238,14 +10129,19 @@
         )
 
     async def query_mcdp_aim_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMcdpAimRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcdpAimResponse:
+        """
+        @param request: QueryMcdpAimRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcdpAimResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8271,29 +10167,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mcdp_aim(
         self,
         request: m_paa_s20201028_models.QueryMcdpAimRequest,
     ) -> m_paa_s20201028_models.QueryMcdpAimResponse:
+        """
+        @param request: QueryMcdpAimRequest
+        @return: QueryMcdpAimResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mcdp_aim_with_options(request, runtime)
 
     async def query_mcdp_aim_async(
         self,
         request: m_paa_s20201028_models.QueryMcdpAimRequest,
     ) -> m_paa_s20201028_models.QueryMcdpAimResponse:
+        """
+        @param request: QueryMcdpAimRequest
+        @return: QueryMcdpAimResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mcdp_aim_with_options_async(request, runtime)
 
     def query_mcdp_zone_with_options(
         self,
         request: m_paa_s20201028_models.QueryMcdpZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcdpZoneResponse:
+        """
+        @param request: QueryMcdpZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcdpZoneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8320,14 +10229,19 @@
         )
 
     async def query_mcdp_zone_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMcdpZoneRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcdpZoneResponse:
+        """
+        @param request: QueryMcdpZoneRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcdpZoneResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8353,29 +10267,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mcdp_zone(
         self,
         request: m_paa_s20201028_models.QueryMcdpZoneRequest,
     ) -> m_paa_s20201028_models.QueryMcdpZoneResponse:
+        """
+        @param request: QueryMcdpZoneRequest
+        @return: QueryMcdpZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mcdp_zone_with_options(request, runtime)
 
     async def query_mcdp_zone_async(
         self,
         request: m_paa_s20201028_models.QueryMcdpZoneRequest,
     ) -> m_paa_s20201028_models.QueryMcdpZoneResponse:
+        """
+        @param request: QueryMcdpZoneRequest
+        @return: QueryMcdpZoneResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mcdp_zone_with_options_async(request, runtime)
 
     def query_mcube_mini_package_with_options(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniPackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcubeMiniPackageResponse:
+        """
+        @param request: QueryMcubeMiniPackageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcubeMiniPackageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.id):
@@ -8404,14 +10331,19 @@
         )
 
     async def query_mcube_mini_package_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniPackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcubeMiniPackageResponse:
+        """
+        @param request: QueryMcubeMiniPackageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcubeMiniPackageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.h_5id):
             body['H5Id'] = request.h_5id
         if not UtilClient.is_unset(request.id):
@@ -8439,29 +10371,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mcube_mini_package(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniPackageRequest,
     ) -> m_paa_s20201028_models.QueryMcubeMiniPackageResponse:
+        """
+        @param request: QueryMcubeMiniPackageRequest
+        @return: QueryMcubeMiniPackageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mcube_mini_package_with_options(request, runtime)
 
     async def query_mcube_mini_package_async(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniPackageRequest,
     ) -> m_paa_s20201028_models.QueryMcubeMiniPackageResponse:
+        """
+        @param request: QueryMcubeMiniPackageRequest
+        @return: QueryMcubeMiniPackageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mcube_mini_package_with_options_async(request, runtime)
 
     def query_mcube_mini_task_with_options(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcubeMiniTaskResponse:
+        """
+        @param request: QueryMcubeMiniTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcubeMiniTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8488,14 +10433,19 @@
         )
 
     async def query_mcube_mini_task_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcubeMiniTaskResponse:
+        """
+        @param request: QueryMcubeMiniTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcubeMiniTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8521,29 +10471,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mcube_mini_task(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniTaskRequest,
     ) -> m_paa_s20201028_models.QueryMcubeMiniTaskResponse:
+        """
+        @param request: QueryMcubeMiniTaskRequest
+        @return: QueryMcubeMiniTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mcube_mini_task_with_options(request, runtime)
 
     async def query_mcube_mini_task_async(
         self,
         request: m_paa_s20201028_models.QueryMcubeMiniTaskRequest,
     ) -> m_paa_s20201028_models.QueryMcubeMiniTaskResponse:
+        """
+        @param request: QueryMcubeMiniTaskRequest
+        @return: QueryMcubeMiniTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mcube_mini_task_with_options_async(request, runtime)
 
     def query_mcube_vhost_with_options(
         self,
         request: m_paa_s20201028_models.QueryMcubeVhostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcubeVhostResponse:
+        """
+        @param request: QueryMcubeVhostRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcubeVhostResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -8568,14 +10531,19 @@
         )
 
     async def query_mcube_vhost_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMcubeVhostRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMcubeVhostResponse:
+        """
+        @param request: QueryMcubeVhostRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMcubeVhostResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -8599,29 +10567,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mcube_vhost(
         self,
         request: m_paa_s20201028_models.QueryMcubeVhostRequest,
     ) -> m_paa_s20201028_models.QueryMcubeVhostResponse:
+        """
+        @param request: QueryMcubeVhostRequest
+        @return: QueryMcubeVhostResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mcube_vhost_with_options(request, runtime)
 
     async def query_mcube_vhost_async(
         self,
         request: m_paa_s20201028_models.QueryMcubeVhostRequest,
     ) -> m_paa_s20201028_models.QueryMcubeVhostResponse:
+        """
+        @param request: QueryMcubeVhostRequest
+        @return: QueryMcubeVhostResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mcube_vhost_with_options_async(request, runtime)
 
     def query_mds_upgrade_task_detail_with_options(
         self,
         request: m_paa_s20201028_models.QueryMdsUpgradeTaskDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMdsUpgradeTaskDetailResponse:
+        """
+        @param request: QueryMdsUpgradeTaskDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMdsUpgradeTaskDetailResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8648,14 +10629,19 @@
         )
 
     async def query_mds_upgrade_task_detail_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMdsUpgradeTaskDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMdsUpgradeTaskDetailResponse:
+        """
+        @param request: QueryMdsUpgradeTaskDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMdsUpgradeTaskDetailResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.tenant_id):
@@ -8681,29 +10667,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mds_upgrade_task_detail(
         self,
         request: m_paa_s20201028_models.QueryMdsUpgradeTaskDetailRequest,
     ) -> m_paa_s20201028_models.QueryMdsUpgradeTaskDetailResponse:
+        """
+        @param request: QueryMdsUpgradeTaskDetailRequest
+        @return: QueryMdsUpgradeTaskDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mds_upgrade_task_detail_with_options(request, runtime)
 
     async def query_mds_upgrade_task_detail_async(
         self,
         request: m_paa_s20201028_models.QueryMdsUpgradeTaskDetailRequest,
     ) -> m_paa_s20201028_models.QueryMdsUpgradeTaskDetailResponse:
+        """
+        @param request: QueryMdsUpgradeTaskDetailRequest
+        @return: QueryMdsUpgradeTaskDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mds_upgrade_task_detail_with_options_async(request, runtime)
 
     def query_mgs_apipage_with_options(
         self,
         request: m_paa_s20201028_models.QueryMgsApipageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMgsApipageResponse:
+        """
+        @param request: QueryMgsApipageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMgsApipageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_status):
             body['ApiStatus'] = request.api_status
         if not UtilClient.is_unset(request.api_type):
             body['ApiType'] = request.api_type
         if not UtilClient.is_unset(request.app_id):
@@ -8754,14 +10753,19 @@
         )
 
     async def query_mgs_apipage_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMgsApipageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMgsApipageResponse:
+        """
+        @param request: QueryMgsApipageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMgsApipageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.api_status):
             body['ApiStatus'] = request.api_status
         if not UtilClient.is_unset(request.api_type):
             body['ApiType'] = request.api_type
         if not UtilClient.is_unset(request.app_id):
@@ -8811,29 +10815,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mgs_apipage(
         self,
         request: m_paa_s20201028_models.QueryMgsApipageRequest,
     ) -> m_paa_s20201028_models.QueryMgsApipageResponse:
+        """
+        @param request: QueryMgsApipageRequest
+        @return: QueryMgsApipageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mgs_apipage_with_options(request, runtime)
 
     async def query_mgs_apipage_async(
         self,
         request: m_paa_s20201028_models.QueryMgsApipageRequest,
     ) -> m_paa_s20201028_models.QueryMgsApipageResponse:
+        """
+        @param request: QueryMgsApipageRequest
+        @return: QueryMgsApipageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mgs_apipage_with_options_async(request, runtime)
 
     def query_mgs_apirest_with_options(
         self,
         request: m_paa_s20201028_models.QueryMgsApirestRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMgsApirestResponse:
+        """
+        @param request: QueryMgsApirestRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMgsApirestResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.format):
             body['Format'] = request.format
         if not UtilClient.is_unset(request.id):
@@ -8864,14 +10881,19 @@
         )
 
     async def query_mgs_apirest_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMgsApirestRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMgsApirestResponse:
+        """
+        @param request: QueryMgsApirestRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMgsApirestResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.format):
             body['Format'] = request.format
         if not UtilClient.is_unset(request.id):
@@ -8901,29 +10923,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mgs_apirest(
         self,
         request: m_paa_s20201028_models.QueryMgsApirestRequest,
     ) -> m_paa_s20201028_models.QueryMgsApirestResponse:
+        """
+        @param request: QueryMgsApirestRequest
+        @return: QueryMgsApirestResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mgs_apirest_with_options(request, runtime)
 
     async def query_mgs_apirest_async(
         self,
         request: m_paa_s20201028_models.QueryMgsApirestRequest,
     ) -> m_paa_s20201028_models.QueryMgsApirestResponse:
+        """
+        @param request: QueryMgsApirestRequest
+        @return: QueryMgsApirestResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mgs_apirest_with_options_async(request, runtime)
 
     def query_mgs_testreqbodyautogen_with_options(
         self,
         request: m_paa_s20201028_models.QueryMgsTestreqbodyautogenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMgsTestreqbodyautogenResponse:
+        """
+        @param request: QueryMgsTestreqbodyautogenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMgsTestreqbodyautogenResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.format):
             body['Format'] = request.format
         if not UtilClient.is_unset(request.mpaas_mappcenter_mgs_testreqbodyautogen_query_json_str):
@@ -8952,14 +10987,19 @@
         )
 
     async def query_mgs_testreqbodyautogen_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMgsTestreqbodyautogenRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMgsTestreqbodyautogenResponse:
+        """
+        @param request: QueryMgsTestreqbodyautogenRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMgsTestreqbodyautogenResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.format):
             body['Format'] = request.format
         if not UtilClient.is_unset(request.mpaas_mappcenter_mgs_testreqbodyautogen_query_json_str):
@@ -8987,29 +11027,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mgs_testreqbodyautogen(
         self,
         request: m_paa_s20201028_models.QueryMgsTestreqbodyautogenRequest,
     ) -> m_paa_s20201028_models.QueryMgsTestreqbodyautogenResponse:
+        """
+        @param request: QueryMgsTestreqbodyautogenRequest
+        @return: QueryMgsTestreqbodyautogenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mgs_testreqbodyautogen_with_options(request, runtime)
 
     async def query_mgs_testreqbodyautogen_async(
         self,
         request: m_paa_s20201028_models.QueryMgsTestreqbodyautogenRequest,
     ) -> m_paa_s20201028_models.QueryMgsTestreqbodyautogenResponse:
+        """
+        @param request: QueryMgsTestreqbodyautogenRequest
+        @return: QueryMgsTestreqbodyautogenResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mgs_testreqbodyautogen_with_options_async(request, runtime)
 
     def query_mps_scheduler_list_with_options(
         self,
         request: m_paa_s20201028_models.QueryMpsSchedulerListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMpsSchedulerListResponse:
+        """
+        @param request: QueryMpsSchedulerListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMpsSchedulerListResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.page_number):
@@ -9044,14 +11097,19 @@
         )
 
     async def query_mps_scheduler_list_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryMpsSchedulerListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryMpsSchedulerListResponse:
+        """
+        @param request: QueryMpsSchedulerListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryMpsSchedulerListResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.page_number):
@@ -9085,29 +11143,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_mps_scheduler_list(
         self,
         request: m_paa_s20201028_models.QueryMpsSchedulerListRequest,
     ) -> m_paa_s20201028_models.QueryMpsSchedulerListResponse:
+        """
+        @param request: QueryMpsSchedulerListRequest
+        @return: QueryMpsSchedulerListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_mps_scheduler_list_with_options(request, runtime)
 
     async def query_mps_scheduler_list_async(
         self,
         request: m_paa_s20201028_models.QueryMpsSchedulerListRequest,
     ) -> m_paa_s20201028_models.QueryMpsSchedulerListResponse:
+        """
+        @param request: QueryMpsSchedulerListRequest
+        @return: QueryMpsSchedulerListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_mps_scheduler_list_with_options_async(request, runtime)
 
     def query_push_analysis_core_index_with_options(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisCoreIndexRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushAnalysisCoreIndexResponse:
+        """
+        @param request: QueryPushAnalysisCoreIndexRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushAnalysisCoreIndexResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel):
             body['Channel'] = request.channel
         if not UtilClient.is_unset(request.end_time):
@@ -9142,14 +11213,19 @@
         )
 
     async def query_push_analysis_core_index_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisCoreIndexRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushAnalysisCoreIndexResponse:
+        """
+        @param request: QueryPushAnalysisCoreIndexRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushAnalysisCoreIndexResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel):
             body['Channel'] = request.channel
         if not UtilClient.is_unset(request.end_time):
@@ -9183,29 +11259,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_push_analysis_core_index(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisCoreIndexRequest,
     ) -> m_paa_s20201028_models.QueryPushAnalysisCoreIndexResponse:
+        """
+        @param request: QueryPushAnalysisCoreIndexRequest
+        @return: QueryPushAnalysisCoreIndexResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_push_analysis_core_index_with_options(request, runtime)
 
     async def query_push_analysis_core_index_async(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisCoreIndexRequest,
     ) -> m_paa_s20201028_models.QueryPushAnalysisCoreIndexResponse:
+        """
+        @param request: QueryPushAnalysisCoreIndexRequest
+        @return: QueryPushAnalysisCoreIndexResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_push_analysis_core_index_with_options_async(request, runtime)
 
     def query_push_analysis_task_detail_with_options(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskDetailResponse:
+        """
+        @param request: QueryPushAnalysisTaskDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushAnalysisTaskDetailResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -9230,14 +11319,19 @@
         )
 
     async def query_push_analysis_task_detail_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskDetailResponse:
+        """
+        @param request: QueryPushAnalysisTaskDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushAnalysisTaskDetailResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -9261,29 +11355,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_push_analysis_task_detail(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskDetailRequest,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskDetailResponse:
+        """
+        @param request: QueryPushAnalysisTaskDetailRequest
+        @return: QueryPushAnalysisTaskDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_push_analysis_task_detail_with_options(request, runtime)
 
     async def query_push_analysis_task_detail_async(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskDetailRequest,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskDetailResponse:
+        """
+        @param request: QueryPushAnalysisTaskDetailRequest
+        @return: QueryPushAnalysisTaskDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_push_analysis_task_detail_with_options_async(request, runtime)
 
     def query_push_analysis_task_list_with_options(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskListResponse:
+        """
+        @param request: QueryPushAnalysisTaskListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushAnalysisTaskListResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_number):
             body['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -9316,14 +11423,19 @@
         )
 
     async def query_push_analysis_task_list_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskListResponse:
+        """
+        @param request: QueryPushAnalysisTaskListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushAnalysisTaskListResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.page_number):
             body['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -9355,29 +11467,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_push_analysis_task_list(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskListRequest,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskListResponse:
+        """
+        @param request: QueryPushAnalysisTaskListRequest
+        @return: QueryPushAnalysisTaskListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_push_analysis_task_list_with_options(request, runtime)
 
     async def query_push_analysis_task_list_async(
         self,
         request: m_paa_s20201028_models.QueryPushAnalysisTaskListRequest,
     ) -> m_paa_s20201028_models.QueryPushAnalysisTaskListResponse:
+        """
+        @param request: QueryPushAnalysisTaskListRequest
+        @return: QueryPushAnalysisTaskListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_push_analysis_task_list_with_options_async(request, runtime)
 
     def query_push_scheduler_list_with_options(
         self,
         request: m_paa_s20201028_models.QueryPushSchedulerListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushSchedulerListResponse:
+        """
+        @param request: QueryPushSchedulerListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushSchedulerListResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.page_number):
@@ -9412,14 +11537,19 @@
         )
 
     async def query_push_scheduler_list_with_options_async(
         self,
         request: m_paa_s20201028_models.QueryPushSchedulerListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.QueryPushSchedulerListResponse:
+        """
+        @param request: QueryPushSchedulerListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: QueryPushSchedulerListResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             body['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.page_number):
@@ -9453,29 +11583,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def query_push_scheduler_list(
         self,
         request: m_paa_s20201028_models.QueryPushSchedulerListRequest,
     ) -> m_paa_s20201028_models.QueryPushSchedulerListResponse:
+        """
+        @param request: QueryPushSchedulerListRequest
+        @return: QueryPushSchedulerListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.query_push_scheduler_list_with_options(request, runtime)
 
     async def query_push_scheduler_list_async(
         self,
         request: m_paa_s20201028_models.QueryPushSchedulerListRequest,
     ) -> m_paa_s20201028_models.QueryPushSchedulerListResponse:
+        """
+        @param request: QueryPushSchedulerListRequest
+        @return: QueryPushSchedulerListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.query_push_scheduler_list_with_options_async(request, runtime)
 
     def revoke_push_message_with_options(
         self,
         request: m_paa_s20201028_models.RevokePushMessageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.RevokePushMessageResponse:
+        """
+        @param request: RevokePushMessageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokePushMessageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.message_id):
             body['MessageId'] = request.message_id
         if not UtilClient.is_unset(request.target_id):
@@ -9502,14 +11645,19 @@
         )
 
     async def revoke_push_message_with_options_async(
         self,
         request: m_paa_s20201028_models.RevokePushMessageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.RevokePushMessageResponse:
+        """
+        @param request: RevokePushMessageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokePushMessageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.message_id):
             body['MessageId'] = request.message_id
         if not UtilClient.is_unset(request.target_id):
@@ -9535,29 +11683,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def revoke_push_message(
         self,
         request: m_paa_s20201028_models.RevokePushMessageRequest,
     ) -> m_paa_s20201028_models.RevokePushMessageResponse:
+        """
+        @param request: RevokePushMessageRequest
+        @return: RevokePushMessageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.revoke_push_message_with_options(request, runtime)
 
     async def revoke_push_message_async(
         self,
         request: m_paa_s20201028_models.RevokePushMessageRequest,
     ) -> m_paa_s20201028_models.RevokePushMessageResponse:
+        """
+        @param request: RevokePushMessageRequest
+        @return: RevokePushMessageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.revoke_push_message_with_options_async(request, runtime)
 
     def revoke_push_task_with_options(
         self,
         request: m_paa_s20201028_models.RevokePushTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.RevokePushTaskResponse:
+        """
+        @param request: RevokePushTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokePushTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -9582,14 +11743,19 @@
         )
 
     async def revoke_push_task_with_options_async(
         self,
         request: m_paa_s20201028_models.RevokePushTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.RevokePushTaskResponse:
+        """
+        @param request: RevokePushTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RevokePushTaskResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.task_id):
             body['TaskId'] = request.task_id
         if not UtilClient.is_unset(request.workspace_id):
@@ -9613,29 +11779,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def revoke_push_task(
         self,
         request: m_paa_s20201028_models.RevokePushTaskRequest,
     ) -> m_paa_s20201028_models.RevokePushTaskResponse:
+        """
+        @param request: RevokePushTaskRequest
+        @return: RevokePushTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.revoke_push_task_with_options(request, runtime)
 
     async def revoke_push_task_async(
         self,
         request: m_paa_s20201028_models.RevokePushTaskRequest,
     ) -> m_paa_s20201028_models.RevokePushTaskResponse:
+        """
+        @param request: RevokePushTaskRequest
+        @return: RevokePushTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.revoke_push_task_with_options_async(request, runtime)
 
     def run_msa_diff_with_options(
         self,
         request: m_paa_s20201028_models.RunMsaDiffRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.RunMsaDiffResponse:
+        """
+        @param request: RunMsaDiffRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RunMsaDiffResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_msa_diff_run_json_str):
             body['MpaasMappcenterMsaDiffRunJsonStr'] = request.mpaas_mappcenter_msa_diff_run_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -9662,14 +11841,19 @@
         )
 
     async def run_msa_diff_with_options_async(
         self,
         request: m_paa_s20201028_models.RunMsaDiffRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.RunMsaDiffResponse:
+        """
+        @param request: RunMsaDiffRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RunMsaDiffResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_msa_diff_run_json_str):
             body['MpaasMappcenterMsaDiffRunJsonStr'] = request.mpaas_mappcenter_msa_diff_run_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -9695,29 +11879,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def run_msa_diff(
         self,
         request: m_paa_s20201028_models.RunMsaDiffRequest,
     ) -> m_paa_s20201028_models.RunMsaDiffResponse:
+        """
+        @param request: RunMsaDiffRequest
+        @return: RunMsaDiffResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.run_msa_diff_with_options(request, runtime)
 
     async def run_msa_diff_async(
         self,
         request: m_paa_s20201028_models.RunMsaDiffRequest,
     ) -> m_paa_s20201028_models.RunMsaDiffResponse:
+        """
+        @param request: RunMsaDiffRequest
+        @return: RunMsaDiffResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.run_msa_diff_with_options_async(request, runtime)
 
     def save_mgs_apirest_with_options(
         self,
         request: m_paa_s20201028_models.SaveMgsApirestRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.SaveMgsApirestResponse:
+        """
+        @param request: SaveMgsApirestRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SaveMgsApirestResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mgs_apirest_save_json_str):
             body['MpaasMappcenterMgsApirestSaveJsonStr'] = request.mpaas_mappcenter_mgs_apirest_save_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -9744,14 +11941,19 @@
         )
 
     async def save_mgs_apirest_with_options_async(
         self,
         request: m_paa_s20201028_models.SaveMgsApirestRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.SaveMgsApirestResponse:
+        """
+        @param request: SaveMgsApirestRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SaveMgsApirestResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.mpaas_mappcenter_mgs_apirest_save_json_str):
             body['MpaasMappcenterMgsApirestSaveJsonStr'] = request.mpaas_mappcenter_mgs_apirest_save_json_str
         if not UtilClient.is_unset(request.tenant_id):
@@ -9777,29 +11979,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def save_mgs_apirest(
         self,
         request: m_paa_s20201028_models.SaveMgsApirestRequest,
     ) -> m_paa_s20201028_models.SaveMgsApirestResponse:
+        """
+        @param request: SaveMgsApirestRequest
+        @return: SaveMgsApirestResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.save_mgs_apirest_with_options(request, runtime)
 
     async def save_mgs_apirest_async(
         self,
         request: m_paa_s20201028_models.SaveMgsApirestRequest,
     ) -> m_paa_s20201028_models.SaveMgsApirestResponse:
+        """
+        @param request: SaveMgsApirestRequest
+        @return: SaveMgsApirestResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.save_mgs_apirest_with_options_async(request, runtime)
 
     def start_user_app_async_enhance_in_msa_with_options(
         self,
         request: m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaResponse:
+        """
+        @param request: StartUserAppAsyncEnhanceInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartUserAppAsyncEnhanceInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.apk_protector):
             body['ApkProtector'] = request.apk_protector
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.assets_file_list):
@@ -9858,14 +12073,19 @@
         )
 
     async def start_user_app_async_enhance_in_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaResponse:
+        """
+        @param request: StartUserAppAsyncEnhanceInMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartUserAppAsyncEnhanceInMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.apk_protector):
             body['ApkProtector'] = request.apk_protector
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.assets_file_list):
@@ -9923,29 +12143,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_user_app_async_enhance_in_msa(
         self,
         request: m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaRequest,
     ) -> m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaResponse:
+        """
+        @param request: StartUserAppAsyncEnhanceInMsaRequest
+        @return: StartUserAppAsyncEnhanceInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_user_app_async_enhance_in_msa_with_options(request, runtime)
 
     async def start_user_app_async_enhance_in_msa_async(
         self,
         request: m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaRequest,
     ) -> m_paa_s20201028_models.StartUserAppAsyncEnhanceInMsaResponse:
+        """
+        @param request: StartUserAppAsyncEnhanceInMsaRequest
+        @return: StartUserAppAsyncEnhanceInMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_user_app_async_enhance_in_msa_with_options_async(request, runtime)
 
     def update_mcube_whitelist_with_options(
         self,
         request: m_paa_s20201028_models.UpdateMcubeWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UpdateMcubeWhitelistResponse:
+        """
+        @param request: UpdateMcubeWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMcubeWhitelistResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.key_ids):
@@ -9978,14 +12211,19 @@
         )
 
     async def update_mcube_whitelist_with_options_async(
         self,
         request: m_paa_s20201028_models.UpdateMcubeWhitelistRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UpdateMcubeWhitelistResponse:
+        """
+        @param request: UpdateMcubeWhitelistRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMcubeWhitelistResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.id):
             body['Id'] = request.id
         if not UtilClient.is_unset(request.key_ids):
@@ -10017,29 +12255,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_mcube_whitelist(
         self,
         request: m_paa_s20201028_models.UpdateMcubeWhitelistRequest,
     ) -> m_paa_s20201028_models.UpdateMcubeWhitelistResponse:
+        """
+        @param request: UpdateMcubeWhitelistRequest
+        @return: UpdateMcubeWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_mcube_whitelist_with_options(request, runtime)
 
     async def update_mcube_whitelist_async(
         self,
         request: m_paa_s20201028_models.UpdateMcubeWhitelistRequest,
     ) -> m_paa_s20201028_models.UpdateMcubeWhitelistResponse:
+        """
+        @param request: UpdateMcubeWhitelistRequest
+        @return: UpdateMcubeWhitelistResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_mcube_whitelist_with_options_async(request, runtime)
 
     def update_mpaas_app_info_with_options(
         self,
         request: m_paa_s20201028_models.UpdateMpaasAppInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UpdateMpaasAppInfoResponse:
+        """
+        @param request: UpdateMpaasAppInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMpaasAppInfoResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_name):
             body['AppName'] = request.app_name
         if not UtilClient.is_unset(request.icon_file_url):
@@ -10072,14 +12323,19 @@
         )
 
     async def update_mpaas_app_info_with_options_async(
         self,
         request: m_paa_s20201028_models.UpdateMpaasAppInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UpdateMpaasAppInfoResponse:
+        """
+        @param request: UpdateMpaasAppInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMpaasAppInfoResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_name):
             body['AppName'] = request.app_name
         if not UtilClient.is_unset(request.icon_file_url):
@@ -10111,29 +12367,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_mpaas_app_info(
         self,
         request: m_paa_s20201028_models.UpdateMpaasAppInfoRequest,
     ) -> m_paa_s20201028_models.UpdateMpaasAppInfoResponse:
+        """
+        @param request: UpdateMpaasAppInfoRequest
+        @return: UpdateMpaasAppInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_mpaas_app_info_with_options(request, runtime)
 
     async def update_mpaas_app_info_async(
         self,
         request: m_paa_s20201028_models.UpdateMpaasAppInfoRequest,
     ) -> m_paa_s20201028_models.UpdateMpaasAppInfoResponse:
+        """
+        @param request: UpdateMpaasAppInfoRequest
+        @return: UpdateMpaasAppInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_mpaas_app_info_with_options_async(request, runtime)
 
     def upload_bitcode_to_msa_with_options(
         self,
         request: m_paa_s20201028_models.UploadBitcodeToMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadBitcodeToMsaResponse:
+        """
+        @summary 上传字节码到msa进行加固
+        
+        @param request: UploadBitcodeToMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadBitcodeToMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.bitcode):
             body['Bitcode'] = request.bitcode
         if not UtilClient.is_unset(request.code_version):
@@ -10166,14 +12437,21 @@
         )
 
     async def upload_bitcode_to_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.UploadBitcodeToMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadBitcodeToMsaResponse:
+        """
+        @summary 上传字节码到msa进行加固
+        
+        @param request: UploadBitcodeToMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadBitcodeToMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.bitcode):
             body['Bitcode'] = request.bitcode
         if not UtilClient.is_unset(request.code_version):
@@ -10205,29 +12483,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def upload_bitcode_to_msa(
         self,
         request: m_paa_s20201028_models.UploadBitcodeToMsaRequest,
     ) -> m_paa_s20201028_models.UploadBitcodeToMsaResponse:
+        """
+        @summary 上传字节码到msa进行加固
+        
+        @param request: UploadBitcodeToMsaRequest
+        @return: UploadBitcodeToMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.upload_bitcode_to_msa_with_options(request, runtime)
 
     async def upload_bitcode_to_msa_async(
         self,
         request: m_paa_s20201028_models.UploadBitcodeToMsaRequest,
     ) -> m_paa_s20201028_models.UploadBitcodeToMsaResponse:
+        """
+        @summary 上传字节码到msa进行加固
+        
+        @param request: UploadBitcodeToMsaRequest
+        @return: UploadBitcodeToMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.upload_bitcode_to_msa_with_options_async(request, runtime)
 
     def upload_mcube_mini_package_with_options(
         self,
         request: m_paa_s20201028_models.UploadMcubeMiniPackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadMcubeMiniPackageResponse:
+        """
+        @param request: UploadMcubeMiniPackageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadMcubeMiniPackageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.auto_install):
             body['AutoInstall'] = request.auto_install
         if not UtilClient.is_unset(request.client_version_max):
@@ -10296,14 +12591,19 @@
         )
 
     async def upload_mcube_mini_package_with_options_async(
         self,
         request: m_paa_s20201028_models.UploadMcubeMiniPackageRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadMcubeMiniPackageResponse:
+        """
+        @param request: UploadMcubeMiniPackageRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadMcubeMiniPackageResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.auto_install):
             body['AutoInstall'] = request.auto_install
         if not UtilClient.is_unset(request.client_version_max):
@@ -10371,29 +12671,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def upload_mcube_mini_package(
         self,
         request: m_paa_s20201028_models.UploadMcubeMiniPackageRequest,
     ) -> m_paa_s20201028_models.UploadMcubeMiniPackageResponse:
+        """
+        @param request: UploadMcubeMiniPackageRequest
+        @return: UploadMcubeMiniPackageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.upload_mcube_mini_package_with_options(request, runtime)
 
     async def upload_mcube_mini_package_async(
         self,
         request: m_paa_s20201028_models.UploadMcubeMiniPackageRequest,
     ) -> m_paa_s20201028_models.UploadMcubeMiniPackageResponse:
+        """
+        @param request: UploadMcubeMiniPackageRequest
+        @return: UploadMcubeMiniPackageResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.upload_mcube_mini_package_with_options_async(request, runtime)
 
     def upload_mcube_rsa_key_with_options(
         self,
         request: m_paa_s20201028_models.UploadMcubeRsaKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadMcubeRsaKeyResponse:
+        """
+        @param request: UploadMcubeRsaKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadMcubeRsaKeyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.file_url):
             body['FileUrl'] = request.file_url
         if not UtilClient.is_unset(request.onex_flag):
@@ -10422,14 +12735,19 @@
         )
 
     async def upload_mcube_rsa_key_with_options_async(
         self,
         request: m_paa_s20201028_models.UploadMcubeRsaKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadMcubeRsaKeyResponse:
+        """
+        @param request: UploadMcubeRsaKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadMcubeRsaKeyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.file_url):
             body['FileUrl'] = request.file_url
         if not UtilClient.is_unset(request.onex_flag):
@@ -10457,29 +12775,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def upload_mcube_rsa_key(
         self,
         request: m_paa_s20201028_models.UploadMcubeRsaKeyRequest,
     ) -> m_paa_s20201028_models.UploadMcubeRsaKeyResponse:
+        """
+        @param request: UploadMcubeRsaKeyRequest
+        @return: UploadMcubeRsaKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.upload_mcube_rsa_key_with_options(request, runtime)
 
     async def upload_mcube_rsa_key_async(
         self,
         request: m_paa_s20201028_models.UploadMcubeRsaKeyRequest,
     ) -> m_paa_s20201028_models.UploadMcubeRsaKeyResponse:
+        """
+        @param request: UploadMcubeRsaKeyRequest
+        @return: UploadMcubeRsaKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.upload_mcube_rsa_key_with_options_async(request, runtime)
 
     def upload_user_app_to_msa_with_options(
         self,
         request: m_paa_s20201028_models.UploadUserAppToMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadUserAppToMsaResponse:
+        """
+        @param request: UploadUserAppToMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadUserAppToMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.file_url):
             body['FileUrl'] = request.file_url
         if not UtilClient.is_unset(request.tenant_id):
@@ -10506,14 +12837,19 @@
         )
 
     async def upload_user_app_to_msa_with_options_async(
         self,
         request: m_paa_s20201028_models.UploadUserAppToMsaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> m_paa_s20201028_models.UploadUserAppToMsaResponse:
+        """
+        @param request: UploadUserAppToMsaRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadUserAppToMsaResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.app_id):
             body['AppId'] = request.app_id
         if not UtilClient.is_unset(request.file_url):
             body['FileUrl'] = request.file_url
         if not UtilClient.is_unset(request.tenant_id):
@@ -10539,16 +12875,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def upload_user_app_to_msa(
         self,
         request: m_paa_s20201028_models.UploadUserAppToMsaRequest,
     ) -> m_paa_s20201028_models.UploadUserAppToMsaResponse:
+        """
+        @param request: UploadUserAppToMsaRequest
+        @return: UploadUserAppToMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.upload_user_app_to_msa_with_options(request, runtime)
 
     async def upload_user_app_to_msa_async(
         self,
         request: m_paa_s20201028_models.UploadUserAppToMsaRequest,
     ) -> m_paa_s20201028_models.UploadUserAppToMsaResponse:
+        """
+        @param request: UploadUserAppToMsaRequest
+        @return: UploadUserAppToMsaResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.upload_user_app_to_msa_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028/models.py` & `alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,21 @@
     def __init__(
         self,
         app_id: str = None,
         mpaas_mappcenter_mini_config_add_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mini_config_add_json_str = mpaas_mappcenter_mini_config_add_json_str
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -227,17 +231,20 @@
     def __init__(
         self,
         app_id: str = None,
         type: int = None,
         unique_ids: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.type = type
+        # This parameter is required.
         self.unique_ids = unique_ids
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -361,20 +368,27 @@
         biz_type: str = None,
         package_id: int = None,
         task_id: int = None,
         task_status: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.biz_type = biz_type
+        # This parameter is required.
         self.package_id = package_id
+        # This parameter is required.
         self.task_id = task_id
+        # This parameter is required.
         self.task_status = task_status
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -935,14 +949,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_group_copy_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_group_copy_json_str = mpaas_mappcenter_mcdp_group_copy_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -1104,23 +1119,212 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CopyMcdpGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateLinkRequest(TeaModel):
+    def __init__(
+        self,
+        app_id: str = None,
+        cors: str = None,
+        domain: str = None,
+        dynamicfield: str = None,
+        target_url: str = None,
+        workspace_id: str = None,
+    ):
+        # This parameter is required.
+        self.app_id = app_id
+        self.cors = cors
+        self.domain = domain
+        self.dynamicfield = dynamicfield
+        # This parameter is required.
+        self.target_url = target_url
+        # This parameter is required.
+        self.workspace_id = workspace_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_id is not None:
+            result['AppId'] = self.app_id
+        if self.cors is not None:
+            result['Cors'] = self.cors
+        if self.domain is not None:
+            result['Domain'] = self.domain
+        if self.dynamicfield is not None:
+            result['Dynamicfield'] = self.dynamicfield
+        if self.target_url is not None:
+            result['TargetUrl'] = self.target_url
+        if self.workspace_id is not None:
+            result['WorkspaceId'] = self.workspace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppId') is not None:
+            self.app_id = m.get('AppId')
+        if m.get('Cors') is not None:
+            self.cors = m.get('Cors')
+        if m.get('Domain') is not None:
+            self.domain = m.get('Domain')
+        if m.get('Dynamicfield') is not None:
+            self.dynamicfield = m.get('Dynamicfield')
+        if m.get('TargetUrl') is not None:
+            self.target_url = m.get('TargetUrl')
+        if m.get('WorkspaceId') is not None:
+            self.workspace_id = m.get('WorkspaceId')
+        return self
+
+
+class CreateLinkResponseBodyResultContent(TeaModel):
+    def __init__(
+        self,
+        data: str = None,
+        target: str = None,
+        version: str = None,
+    ):
+        self.data = data
+        self.target = target
+        self.version = version
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.target is not None:
+            result['Target'] = self.target
+        if self.version is not None:
+            result['Version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Target') is not None:
+            self.target = m.get('Target')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        return self
+
+
+class CreateLinkResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        result_code: str = None,
+        result_content: CreateLinkResponseBodyResultContent = None,
+        result_message: str = None,
+    ):
+        # Id of the request
+        self.request_id = request_id
+        self.result_code = result_code
+        self.result_content = result_content
+        self.result_message = result_message
+
+    def validate(self):
+        if self.result_content:
+            self.result_content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result_code is not None:
+            result['ResultCode'] = self.result_code
+        if self.result_content is not None:
+            result['ResultContent'] = self.result_content.to_map()
+        if self.result_message is not None:
+            result['ResultMessage'] = self.result_message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResultCode') is not None:
+            self.result_code = m.get('ResultCode')
+        if m.get('ResultContent') is not None:
+            temp_model = CreateLinkResponseBodyResultContent()
+            self.result_content = temp_model.from_map(m['ResultContent'])
+        if m.get('ResultMessage') is not None:
+            self.result_message = m.get('ResultMessage')
+        return self
+
+
+class CreateLinkResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateLinkResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateLinkResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateMasCrowdRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_mas_crowd_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_mas_crowd_create_json_str = mpaas_mappcenter_mcdp_mas_crowd_create_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -1291,14 +1495,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_mas_funnel_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_mas_funnel_create_json_str = mpaas_mappcenter_mcdp_mas_funnel_create_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -1469,14 +1674,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_event_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_event_create_json_str = mpaas_mappcenter_mcdp_event_create_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -1647,14 +1853,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_event_attribute_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_event_attribute_create_json_str = mpaas_mappcenter_mcdp_event_attribute_create_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -1825,14 +2032,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_group_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_group_create_json_str = mpaas_mappcenter_mcdp_group_create_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -2003,14 +2211,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_material_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_material_create_json_str = mpaas_mappcenter_mcdp_material_create_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -2181,14 +2390,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_zone_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_zone_create_json_str = mpaas_mappcenter_mcdp_zone_create_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -2359,18 +2569,23 @@
         self,
         app_id: str = None,
         h_5id: str = None,
         h_5name: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.h_5id = h_5id
+        # This parameter is required.
         self.h_5name = h_5name
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2543,24 +2758,31 @@
         package_id: int = None,
         publish_mode: int = None,
         publish_type: int = None,
         tenant_id: str = None,
         whitelist_ids: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.grey_config_info = grey_config_info
         self.grey_endtime_data = grey_endtime_data
         self.grey_num = grey_num
+        # This parameter is required.
         self.memo = memo
+        # This parameter is required.
         self.package_id = package_id
+        # This parameter is required.
         self.publish_mode = publish_mode
+        # This parameter is required.
         self.publish_type = publish_type
+        # This parameter is required.
         self.tenant_id = tenant_id
         self.whitelist_ids = whitelist_ids
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4114,17 +4336,21 @@
     def __init__(
         self,
         app_id: str = None,
         tenant_id: str = None,
         vhost: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.vhost = vhost
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4287,18 +4513,23 @@
         self,
         app_id: str = None,
         tenant_id: str = None,
         white_list_name: str = None,
         whitelist_type: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.white_list_name = white_list_name
+        # This parameter is required.
         self.whitelist_type = whitelist_type
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4465,18 +4696,23 @@
         self,
         app_id: str = None,
         tenant_id: str = None,
         user_id: str = None,
         whitelist_value: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.user_id = user_id
+        # This parameter is required.
         self.whitelist_value = whitelist_value
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4655,18 +4891,21 @@
         whitelist_ids: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
         self.grey_config_info = grey_config_info
         self.grey_endtime_data = grey_endtime_data
         self.grey_num = grey_num
+        # This parameter is required.
         self.id = id
         self.memo = memo
+        # This parameter is required.
         self.package_id = package_id
         self.publish_mode = publish_mode
+        # This parameter is required.
         self.publish_type = publish_type
         self.sync_mode = sync_mode
         self.tenant_id = tenant_id
         self.whitelist_ids = whitelist_ids
         self.workspace_id = workspace_id
 
     def validate(self):
@@ -4915,17 +5154,21 @@
     def __init__(
         self,
         app_id: str = None,
         mpaas_mappcenter_msa_enhance_create_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_msa_enhance_create_json_str = mpaas_mappcenter_msa_enhance_create_json_str
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5103,27 +5346,32 @@
         payload: str = None,
         third_msg_id: str = None,
         uids: str = None,
         valid_time_end: int = None,
         valid_time_start: int = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.app_max_version = app_max_version
         self.app_min_version = app_min_version
+        # This parameter is required.
         self.biz_type = biz_type
         self.ext_attr_str = ext_attr_str
         self.max_uid = max_uid
         self.min_uid = min_uid
         self.os_type = os_type
+        # This parameter is required.
         self.payload = payload
+        # This parameter is required.
         self.third_msg_id = third_msg_id
         self.uids = uids
         self.valid_time_end = valid_time_end
         self.valid_time_start = valid_time_start
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5293,26 +5541,32 @@
         os_type: str = None,
         payload: str = None,
         third_msg_id: str = None,
         valid_time_end: int = None,
         valid_time_start: int = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.app_max_version = app_max_version
         self.app_min_version = app_min_version
+        # This parameter is required.
         self.biz_type = biz_type
         self.check_online = check_online
         self.ext_attr_str = ext_attr_str
+        # This parameter is required.
         self.link_token = link_token
         self.os_type = os_type
+        # This parameter is required.
         self.payload = payload
+        # This parameter is required.
         self.third_msg_id = third_msg_id
         self.valid_time_end = valid_time_end
         self.valid_time_start = valid_time_start
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5689,14 +5943,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_aim_delete_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_aim_delete_json_str = mpaas_mappcenter_mcdp_aim_delete_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -5867,14 +6122,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_crowd_delete_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_crowd_delete_json_str = mpaas_mappcenter_mcdp_crowd_delete_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -6045,14 +6301,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_event_attribute_delete_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_event_attribute_delete_json_str = mpaas_mappcenter_mcdp_event_attribute_delete_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -6223,14 +6480,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_event_delete_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_event_delete_json_str = mpaas_mappcenter_mcdp_event_delete_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -6401,14 +6659,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_material_delete_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_material_delete_json_str = mpaas_mappcenter_mcdp_material_delete_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -6579,14 +6838,15 @@
         self,
         app_id: str = None,
         mpaas_mappcenter_mcdp_zone_delete_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_mcdp_zone_delete_json_str = mpaas_mappcenter_mcdp_zone_delete_json_str
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -6756,17 +7016,21 @@
     def __init__(
         self,
         app_id: str = None,
         h_5id: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.h_5id = h_5id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7290,17 +7554,21 @@
     def __init__(
         self,
         app_id: str = None,
         id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.id = id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7680,16 +7948,19 @@
 class ExistMcubeRsaKeyRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7853,16 +8124,19 @@
         onex_flag: bool = None,
         system_type: str = None,
         workspace_id: str = None,
     ):
         self.apk_file_url = apk_file_url
         self.app_id = app_id
         self.cert_rsa_base_64 = cert_rsa_base_64
+        # This parameter is required.
         self.identifier = identifier
+        # This parameter is required.
         self.onex_flag = onex_flag
+        # This parameter is required.
         self.system_type = system_type
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -8037,17 +8311,20 @@
     def __init__(
         self,
         app_id: str = None,
         onex_flag: bool = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.onex_flag = onex_flag
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8280,17 +8557,20 @@
     def __init__(
         self,
         app_id: str = None,
         id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.id = id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8458,17 +8738,21 @@
     def __init__(
         self,
         app_id: str = None,
         onex_flag: bool = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.onex_flag = onex_flag
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10720,17 +11004,21 @@
     def __init__(
         self,
         app_id: str = None,
         h_5id: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.h_5id = h_5id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11357,17 +11645,21 @@
     def __init__(
         self,
         app_id: str = None,
         id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.id = id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11570,17 +11862,21 @@
     def __init__(
         self,
         app_id: str = None,
         id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.id = id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11944,17 +12240,21 @@
     def __init__(
         self,
         app_id: str = None,
         id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.id = id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13144,19 +13444,22 @@
         app_id: str = None,
         keyword: str = None,
         page_num: int = None,
         page_size: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.keyword = keyword
         self.page_num = page_num
         self.page_size = page_size
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13412,20 +13715,25 @@
         h_5id: str = None,
         package_types: str = None,
         page_num: int = None,
         page_size: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.h_5id = h_5id
+        # This parameter is required.
         self.package_types = package_types
         self.page_num = page_num
         self.page_size = page_size
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13784,17 +14092,21 @@
     def __init__(
         self,
         app_id: str = None,
         id: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.id = id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16162,19 +16474,22 @@
         app_id: str = None,
         page_num: int = None,
         page_size: int = None,
         tenant_id: str = None,
         whitelist_name: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.page_num = page_num
         self.page_size = page_size
+        # This parameter is required.
         self.tenant_id = tenant_id
         self.whitelist_name = whitelist_name
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17509,18 +17824,21 @@
         self,
         app_id: str = None,
         id: str = None,
         onex_flag: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.id = id
         self.onex_flag = onex_flag
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17695,17 +18013,19 @@
         image_raw: str = None,
         mask: bool = None,
         tenant_id: str = None,
         type: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.image_raw = image_raw
         self.mask = mask
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.type = type
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -19230,19 +19550,24 @@
         app_id: str = None,
         delivery_token: str = None,
         os_type: int = None,
         phone_number: str = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.delivery_token = delivery_token
+        # This parameter is required.
         self.os_type = os_type
         self.phone_number = phone_number
+        # This parameter is required.
         self.user_id = user_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19431,34 +19756,40 @@
         template_key_value: str = None,
         template_name: str = None,
         third_channel_category: Dict[str, Any] = None,
         un_bind_period: int = None,
         workspace_id: str = None,
     ):
         self.android_channel = android_channel
+        # This parameter is required.
         self.app_id = app_id
         self.bind_period = bind_period
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.delivery_type = delivery_type
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.mi_channel_id = mi_channel_id
+        # This parameter is required.
         self.msgkey = msgkey
         self.notify_type = notify_type
         self.push_action = push_action
         self.push_status = push_status
         self.silent = silent
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
         self.task_name = task_name
         self.template_key_value = template_key_value
+        # This parameter is required.
         self.template_name = template_name
         self.third_channel_category = third_channel_category
         self.un_bind_period = un_bind_period
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19584,34 +19915,40 @@
         template_key_value: str = None,
         template_name: str = None,
         third_channel_category_shrink: str = None,
         un_bind_period: int = None,
         workspace_id: str = None,
     ):
         self.android_channel = android_channel
+        # This parameter is required.
         self.app_id = app_id
         self.bind_period = bind_period
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.delivery_type = delivery_type
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.mi_channel_id = mi_channel_id
+        # This parameter is required.
         self.msgkey = msgkey
         self.notify_type = notify_type
         self.push_action = push_action
         self.push_status = push_status
         self.silent = silent
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
         self.task_name = task_name
         self.template_key_value = template_key_value
+        # This parameter is required.
         self.template_name = template_name
         self.third_channel_category_shrink = third_channel_category_shrink
         self.un_bind_period = un_bind_period
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -19846,15 +20183,17 @@
         self,
         extended_params: str = None,
         msg_key: str = None,
         target: str = None,
         template_key_value: str = None,
     ):
         self.extended_params = extended_params
+        # This parameter is required.
         self.msg_key = msg_key
+        # This parameter is required.
         self.target = target
         self.template_key_value = template_key_value
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -19908,31 +20247,37 @@
         task_name: str = None,
         template_name: str = None,
         third_channel_category: Dict[str, Any] = None,
         workspace_id: str = None,
     ):
         self.activity_content_state = activity_content_state
         self.activity_event = activity_event
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.delivery_type = delivery_type
         self.dismissal_date = dismissal_date
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.mi_channel_id = mi_channel_id
         self.notify_type = notify_type
         self.push_action = push_action
         self.silent = silent
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
+        # This parameter is required.
         self.target_msg = target_msg
         self.task_name = task_name
+        # This parameter is required.
         self.template_name = template_name
         self.third_channel_category = third_channel_category
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.target_msg:
             for k in self.target_msg:
                 if k:
                     k.validate()
@@ -20040,15 +20385,17 @@
         self,
         extended_params: str = None,
         msg_key: str = None,
         target: str = None,
         template_key_value: str = None,
     ):
         self.extended_params = extended_params
+        # This parameter is required.
         self.msg_key = msg_key
+        # This parameter is required.
         self.target = target
         self.template_key_value = template_key_value
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -20102,31 +20449,37 @@
         task_name: str = None,
         template_name: str = None,
         third_channel_category_shrink: str = None,
         workspace_id: str = None,
     ):
         self.activity_content_state = activity_content_state
         self.activity_event = activity_event
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.delivery_type = delivery_type
         self.dismissal_date = dismissal_date
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.mi_channel_id = mi_channel_id
         self.notify_type = notify_type
         self.push_action = push_action
         self.silent = silent
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
+        # This parameter is required.
         self.target_msg = target_msg
         self.task_name = task_name
+        # This parameter is required.
         self.template_name = template_name
         self.third_channel_category_shrink = third_channel_category_shrink
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         if self.target_msg:
             for k in self.target_msg:
                 if k:
                     k.validate()
@@ -20369,26 +20722,30 @@
         model: str = None,
         os_type: int = None,
         push_version: str = None,
         third_channel: int = None,
         third_channel_device_token: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.app_version = app_version
         self.channel = channel
         self.connect_type = connect_type
+        # This parameter is required.
         self.delivery_token = delivery_token
         self.imei = imei
         self.imsi = imsi
         self.model = model
+        # This parameter is required.
         self.os_type = os_type
         self.push_version = push_version
         self.third_channel = third_channel
         self.third_channel_device_token = third_channel_device_token
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20613,20 +20970,24 @@
         third_channel_category: Dict[str, Any] = None,
         title: str = None,
         uri: str = None,
         workspace_id: str = None,
     ):
         self.activity_content_state = activity_content_state
         self.activity_event = activity_event
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.content = content
+        # This parameter is required.
         self.delivery_type = delivery_type
         self.dismissal_date = dismissal_date
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.icon_urls = icon_urls
         self.image_urls = image_urls
         self.mi_channel_id = mi_channel_id
         self.notify_type = notify_type
         self.push_action = push_action
@@ -20634,19 +20995,22 @@
         self.silent = silent
         self.sms_sign_name = sms_sign_name
         self.sms_strategy = sms_strategy
         self.sms_template_code = sms_template_code
         self.sms_template_param = sms_template_param
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
+        # This parameter is required.
         self.target_msgkey = target_msgkey
         self.task_name = task_name
         self.third_channel_category = third_channel_category
+        # This parameter is required.
         self.title = title
         self.uri = uri
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -20808,20 +21172,24 @@
         third_channel_category_shrink: str = None,
         title: str = None,
         uri: str = None,
         workspace_id: str = None,
     ):
         self.activity_content_state = activity_content_state
         self.activity_event = activity_event
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.content = content
+        # This parameter is required.
         self.delivery_type = delivery_type
         self.dismissal_date = dismissal_date
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.icon_urls = icon_urls
         self.image_urls = image_urls
         self.mi_channel_id = mi_channel_id
         self.notify_type = notify_type
         self.push_action = push_action
@@ -20829,19 +21197,22 @@
         self.silent = silent
         self.sms_sign_name = sms_sign_name
         self.sms_strategy = sms_strategy
         self.sms_template_code = sms_template_code
         self.sms_template_param = sms_template_param
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
+        # This parameter is required.
         self.target_msgkey = target_msgkey
         self.task_name = task_name
         self.third_channel_category_shrink = third_channel_category_shrink
+        # This parameter is required.
         self.title = title
         self.uri = uri
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21126,36 +21497,42 @@
         template_key_value: str = None,
         template_name: str = None,
         third_channel_category: Dict[str, Any] = None,
         workspace_id: str = None,
     ):
         self.activity_content_state = activity_content_state
         self.activity_event = activity_event
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.delivery_type = delivery_type
         self.dismissal_date = dismissal_date
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.mi_channel_id = mi_channel_id
         self.notify_type = notify_type
         self.push_action = push_action
         self.silent = silent
         self.sms_sign_name = sms_sign_name
         self.sms_strategy = sms_strategy
         self.sms_template_code = sms_template_code
         self.sms_template_param = sms_template_param
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
+        # This parameter is required.
         self.target_msgkey = target_msgkey
         self.task_name = task_name
         self.template_key_value = template_key_value
+        # This parameter is required.
         self.template_name = template_name
         self.third_channel_category = third_channel_category
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21297,36 +21674,42 @@
         template_key_value: str = None,
         template_name: str = None,
         third_channel_category_shrink: str = None,
         workspace_id: str = None,
     ):
         self.activity_content_state = activity_content_state
         self.activity_event = activity_event
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
         self.classification = classification
+        # This parameter is required.
         self.delivery_type = delivery_type
         self.dismissal_date = dismissal_date
+        # This parameter is required.
         self.expired_seconds = expired_seconds
         self.extended_params = extended_params
         self.mi_channel_id = mi_channel_id
         self.notify_type = notify_type
         self.push_action = push_action
         self.silent = silent
         self.sms_sign_name = sms_sign_name
         self.sms_strategy = sms_strategy
         self.sms_template_code = sms_template_code
         self.sms_template_param = sms_template_param
         self.strategy_content = strategy_content
         self.strategy_type = strategy_type
+        # This parameter is required.
         self.target_msgkey = target_msgkey
         self.task_name = task_name
         self.template_key_value = template_key_value
+        # This parameter is required.
         self.template_name = template_name
         self.third_channel_category_shrink = third_channel_category_shrink
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21572,17 +21955,21 @@
     def __init__(
         self,
         app_id: str = None,
         delivery_token: str = None,
         user_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.delivery_token = delivery_token
+        # This parameter is required.
         self.user_id = user_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21747,20 +22134,23 @@
         mobile: str = None,
         mobile_md_5: str = None,
         mobile_sha_256: str = None,
         risk_scene: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.mobile = mobile
         self.mobile_md_5 = mobile_md_5
         self.mobile_sha_256 = mobile_sha_256
+        # This parameter is required.
         self.risk_scene = risk_scene
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -21891,21 +22281,193 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = QueryInfoFromMdpResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class QueryLinkRequest(TeaModel):
+    def __init__(
+        self,
+        app_id: str = None,
+        url: str = None,
+        workspace_id: str = None,
+    ):
+        # This parameter is required.
+        self.app_id = app_id
+        # This parameter is required.
+        self.url = url
+        # This parameter is required.
+        self.workspace_id = workspace_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.app_id is not None:
+            result['AppId'] = self.app_id
+        if self.url is not None:
+            result['Url'] = self.url
+        if self.workspace_id is not None:
+            result['WorkspaceId'] = self.workspace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AppId') is not None:
+            self.app_id = m.get('AppId')
+        if m.get('Url') is not None:
+            self.url = m.get('Url')
+        if m.get('WorkspaceId') is not None:
+            self.workspace_id = m.get('WorkspaceId')
+        return self
+
+
+class QueryLinkResponseBodyResultContent(TeaModel):
+    def __init__(
+        self,
+        data: Any = None,
+        target: str = None,
+        version: str = None,
+    ):
+        self.data = data
+        self.target = target
+        self.version = version
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data
+        if self.target is not None:
+            result['Target'] = self.target
+        if self.version is not None:
+            result['Version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            self.data = m.get('Data')
+        if m.get('Target') is not None:
+            self.target = m.get('Target')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        return self
+
+
+class QueryLinkResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        result_code: str = None,
+        result_content: QueryLinkResponseBodyResultContent = None,
+        result_message: str = None,
+    ):
+        # Id of the request
+        self.request_id = request_id
+        self.result_code = result_code
+        self.result_content = result_content
+        self.result_message = result_message
+
+    def validate(self):
+        if self.result_content:
+            self.result_content.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.result_code is not None:
+            result['ResultCode'] = self.result_code
+        if self.result_content is not None:
+            result['ResultContent'] = self.result_content.to_map()
+        if self.result_message is not None:
+            result['ResultMessage'] = self.result_message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ResultCode') is not None:
+            self.result_code = m.get('ResultCode')
+        if m.get('ResultContent') is not None:
+            temp_model = QueryLinkResponseBodyResultContent()
+            self.result_content = temp_model.from_map(m['ResultContent'])
+        if m.get('ResultMessage') is not None:
+            self.result_message = m.get('ResultMessage')
+        return self
+
+
+class QueryLinkResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: QueryLinkResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = QueryLinkResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class QueryMappCenterAppRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22244,14 +22806,15 @@
         self,
         app_id: str = None,
         id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.id = id
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -22600,18 +23163,23 @@
         self,
         app_id: str = None,
         h_5id: str = None,
         id: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.h_5id = h_5id
+        # This parameter is required.
         self.id = id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22932,17 +23500,21 @@
     def __init__(
         self,
         app_id: str = None,
         task_id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.task_id = task_id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23228,16 +23800,19 @@
 class QueryMcubeVhostRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -23396,14 +23971,15 @@
         self,
         app_id: str = None,
         task_id: int = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
         self.app_id = app_id
+        # This parameter is required.
         self.task_id = task_id
         self.tenant_id = tenant_id
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
@@ -26341,21 +26917,23 @@
         page_number: int = None,
         page_size: int = None,
         start_time: int = None,
         type: int = None,
         unique_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.end_time = end_time
         self.page_number = page_number
         self.page_size = page_size
         self.start_time = start_time
         self.type = type
         self.unique_id = unique_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26655,21 +27233,25 @@
         end_time: int = None,
         platform: str = None,
         start_time: int = None,
         task_id: str = None,
         type: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.channel = channel
+        # This parameter is required.
         self.end_time = end_time
         self.platform = platform
+        # This parameter is required.
         self.start_time = start_time
         self.task_id = task_id
         self.type = type
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -26905,16 +27487,19 @@
 class QueryPushAnalysisTaskDetailRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         task_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.task_id = task_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27128,20 +27713,23 @@
         page_number: int = None,
         page_size: int = None,
         start_time: int = None,
         task_id: str = None,
         task_name: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.page_number = page_number
         self.page_size = page_size
+        # This parameter is required.
         self.start_time = start_time
         self.task_id = task_id
         self.task_name = task_name
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27443,21 +28031,25 @@
         page_number: int = None,
         page_size: int = None,
         start_time: int = None,
         type: int = None,
         unique_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_time = end_time
         self.page_number = page_number
         self.page_size = page_size
+        # This parameter is required.
         self.start_time = start_time
         self.type = type
         self.unique_id = unique_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27753,17 +28345,21 @@
     def __init__(
         self,
         app_id: str = None,
         message_id: str = None,
         target_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.message_id = message_id
+        # This parameter is required.
         self.target_id = target_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27924,16 +28520,19 @@
 class RevokePushTaskRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         task_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.task_id = task_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28091,17 +28690,21 @@
     def __init__(
         self,
         app_id: str = None,
         mpaas_mappcenter_msa_diff_run_json_str: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.mpaas_mappcenter_msa_diff_run_json_str = mpaas_mappcenter_msa_diff_run_json_str
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28458,32 +29061,36 @@
         task_type: str = None,
         tenant_id: str = None,
         total_switch: bool = None,
         use_ashield: bool = None,
         workspace_id: str = None,
     ):
         self.apk_protector = apk_protector
+        # This parameter is required.
         self.app_id = app_id
         self.assets_file_list = assets_file_list
         self.classes = classes
         self.dalvik_debugger = dalvik_debugger
         self.emulator_environment = emulator_environment
+        # This parameter is required.
         self.id = id
         self.java_hook = java_hook
         self.memory_dump = memory_dump
         self.native_debugger = native_debugger
         self.native_hook = native_hook
         self.package_tampered = package_tampered
         self.root = root
         self.run_mode = run_mode
         self.so_file_list = so_file_list
         self.task_type = task_type
+        # This parameter is required.
         self.tenant_id = tenant_id
         self.total_switch = total_switch
         self.use_ashield = use_ashield
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28914,20 +29521,25 @@
         id: str = None,
         key_ids: str = None,
         onex_flag: bool = None,
         oss_url: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.id = id
         self.key_ids = key_ids
+        # This parameter is required.
         self.onex_flag = onex_flag
         self.oss_url = oss_url
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29382,20 +29994,23 @@
         bitcode: str = None,
         code_version: str = None,
         license: str = None,
         tenant_id: str = None,
         type: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.bitcode = bitcode
         self.code_version = code_version
         self.license = license
+        # This parameter is required.
         self.tenant_id = tenant_id
         self.type = type
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29596,38 +30211,58 @@
         resource_type: int = None,
         tenant_id: str = None,
         user_id: str = None,
         uuid: str = None,
         vhost: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.auto_install = auto_install
         self.client_version_max = client_version_max
+        # This parameter is required.
         self.client_version_min = client_version_min
+        # This parameter is required.
         self.enable_keep_alive = enable_keep_alive
+        # This parameter is required.
         self.enable_option_menu = enable_option_menu
+        # This parameter is required.
         self.enable_tab_bar = enable_tab_bar
         self.extend_info = extend_info
+        # This parameter is required.
         self.h_5id = h_5id
+        # This parameter is required.
         self.h_5name = h_5name
+        # This parameter is required.
         self.h_5version = h_5version
         self.icon_file_url = icon_file_url
         self.icon_url = icon_url
+        # This parameter is required.
         self.install_type = install_type
+        # This parameter is required.
         self.main_url = main_url
+        # This parameter is required.
         self.onex_flag = onex_flag
+        # This parameter is required.
         self.package_type = package_type
+        # This parameter is required.
         self.platform = platform
+        # This parameter is required.
         self.resource_file_url = resource_file_url
+        # This parameter is required.
         self.resource_type = resource_type
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.user_id = user_id
         self.uuid = uuid
+        # This parameter is required.
         self.vhost = vhost
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -29915,18 +30550,23 @@
         self,
         app_id: str = None,
         file_url: str = None,
         onex_flag: bool = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.file_url = file_url
+        # This parameter is required.
         self.onex_flag = onex_flag
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30092,17 +30732,20 @@
     def __init__(
         self,
         app_id: str = None,
         file_url: str = None,
         tenant_id: str = None,
         workspace_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.file_url = file_url
+        # This parameter is required.
         self.tenant_id = tenant_id
+        # This parameter is required.
         self.workspace_id = workspace_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_mpaas20201028-1.3.0/alibabacloud_mpaas20201028.egg-info/PKG-INFO` & `alibabacloud_mpaas20201028-1.4.0/alibabacloud_mpaas20201028.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mpaas20201028
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud Mobile PaaS (20201028) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mpaas20201028-1.3.0/setup.py` & `alibabacloud_mpaas20201028-1.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mpaas20201028.
 
-Created on 06/02/2024
+Created on 17/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mpaas20201028"
 NAME = "alibabacloud_mpaas20201028" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Mobile PaaS (20201028) SDK Library for Python"
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

