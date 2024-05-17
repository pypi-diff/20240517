# Comparing `tmp/alibabacloud_csas20230120-1.4.0.tar.gz` & `tmp/alibabacloud_csas20230120-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_csas20230120-1.4.0.tar", last modified: Thu Apr 25 05:40:29 2024, max compression
+gzip compressed data, was "dist/alibabacloud_csas20230120-1.4.1.tar", last modified: Fri May 17 17:22:36 2024, max compression
```

## Comparing `alibabacloud_csas20230120-1.4.0.tar` & `alibabacloud_csas20230120-1.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     1074 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/__init__.py
--rw-r--r--   0 root         (0) root         (0)   210038 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/client.py
--rw-r--r--   0 root         (0) root         (0)   458459 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2024-04-25 05:40:29.000000 alibabacloud_csas20230120-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   270444 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120/client.py
+-rw-r--r--   0 root         (0) root         (0)   463708 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-05-17 17:22:36.000000 alibabacloud_csas20230120-1.4.1/setup.py
```

### Comparing `alibabacloud_csas20230120-1.4.0/LICENSE` & `alibabacloud_csas20230120-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.4.0/PKG-INFO` & `alibabacloud_csas20230120-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_csas20230120
-Version: 1.4.0
+Version: 1.4.1
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120-1.4.0/README-CN.md` & `alibabacloud_csas20230120-1.4.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.4.0/README.md` & `alibabacloud_csas20230120-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/client.py` & `alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,14 +42,21 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def attach_application_2connector_with_options(
         self,
         tmp_req: csas_20230120_models.AttachApplication2ConnectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.AttachApplication2ConnectorResponse:
+        """
+        @summary 挂载connector的应用
+        
+        @param tmp_req: AttachApplication2ConnectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachApplication2ConnectorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.AttachApplication2ConnectorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.application_ids):
             request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.application_ids_shrink):
@@ -76,14 +83,21 @@
         )
 
     async def attach_application_2connector_with_options_async(
         self,
         tmp_req: csas_20230120_models.AttachApplication2ConnectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.AttachApplication2ConnectorResponse:
+        """
+        @summary 挂载connector的应用
+        
+        @param tmp_req: AttachApplication2ConnectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AttachApplication2ConnectorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.AttachApplication2ConnectorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.application_ids):
             request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.application_ids_shrink):
@@ -109,29 +123,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def attach_application_2connector(
         self,
         request: csas_20230120_models.AttachApplication2ConnectorRequest,
     ) -> csas_20230120_models.AttachApplication2ConnectorResponse:
+        """
+        @summary 挂载connector的应用
+        
+        @param request: AttachApplication2ConnectorRequest
+        @return: AttachApplication2ConnectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.attach_application_2connector_with_options(request, runtime)
 
     async def attach_application_2connector_async(
         self,
         request: csas_20230120_models.AttachApplication2ConnectorRequest,
     ) -> csas_20230120_models.AttachApplication2ConnectorResponse:
+        """
+        @summary 挂载connector的应用
+        
+        @param request: AttachApplication2ConnectorRequest
+        @return: AttachApplication2ConnectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.attach_application_2connector_with_options_async(request, runtime)
 
     def create_client_user_with_options(
         self,
         request: csas_20230120_models.CreateClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateClientUserResponse:
+        """
+        @summary 创建自定义身份源用户
+        
+        @param request: CreateClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.email):
@@ -164,14 +197,21 @@
         )
 
     async def create_client_user_with_options_async(
         self,
         request: csas_20230120_models.CreateClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateClientUserResponse:
+        """
+        @summary 创建自定义身份源用户
+        
+        @param request: CreateClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.email):
@@ -203,29 +243,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_client_user(
         self,
         request: csas_20230120_models.CreateClientUserRequest,
     ) -> csas_20230120_models.CreateClientUserResponse:
+        """
+        @summary 创建自定义身份源用户
+        
+        @param request: CreateClientUserRequest
+        @return: CreateClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_client_user_with_options(request, runtime)
 
     async def create_client_user_async(
         self,
         request: csas_20230120_models.CreateClientUserRequest,
     ) -> csas_20230120_models.CreateClientUserResponse:
+        """
+        @summary 创建自定义身份源用户
+        
+        @param request: CreateClientUserRequest
+        @return: CreateClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_client_user_with_options_async(request, runtime)
 
     def create_dynamic_route_with_options(
         self,
         request: csas_20230120_models.CreateDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateDynamicRouteResponse:
+        """
+        @summary 创建动态路由
+        
+        @param request: CreateDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -267,14 +326,21 @@
         )
 
     async def create_dynamic_route_with_options_async(
         self,
         request: csas_20230120_models.CreateDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateDynamicRouteResponse:
+        """
+        @summary 创建动态路由
+        
+        @param request: CreateDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -315,29 +381,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_dynamic_route(
         self,
         request: csas_20230120_models.CreateDynamicRouteRequest,
     ) -> csas_20230120_models.CreateDynamicRouteResponse:
+        """
+        @summary 创建动态路由
+        
+        @param request: CreateDynamicRouteRequest
+        @return: CreateDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_dynamic_route_with_options(request, runtime)
 
     async def create_dynamic_route_async(
         self,
         request: csas_20230120_models.CreateDynamicRouteRequest,
     ) -> csas_20230120_models.CreateDynamicRouteResponse:
+        """
+        @summary 创建动态路由
+        
+        @param request: CreateDynamicRouteRequest
+        @return: CreateDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_dynamic_route_with_options_async(request, runtime)
 
     def create_idp_department_with_options(
         self,
         request: csas_20230120_models.CreateIdpDepartmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateIdpDepartmentResponse:
+        """
+        @summary 创建自定义身份源部门
+        
+        @param request: CreateIdpDepartmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateIdpDepartmentResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_name):
             query['DepartmentName'] = request.department_name
         if not UtilClient.is_unset(request.idp_config_id):
             query['IdpConfigId'] = request.idp_config_id
         req = open_api_models.OpenApiRequest(
@@ -360,14 +445,21 @@
         )
 
     async def create_idp_department_with_options_async(
         self,
         request: csas_20230120_models.CreateIdpDepartmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateIdpDepartmentResponse:
+        """
+        @summary 创建自定义身份源部门
+        
+        @param request: CreateIdpDepartmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateIdpDepartmentResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_name):
             query['DepartmentName'] = request.department_name
         if not UtilClient.is_unset(request.idp_config_id):
             query['IdpConfigId'] = request.idp_config_id
         req = open_api_models.OpenApiRequest(
@@ -389,29 +481,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_idp_department(
         self,
         request: csas_20230120_models.CreateIdpDepartmentRequest,
     ) -> csas_20230120_models.CreateIdpDepartmentResponse:
+        """
+        @summary 创建自定义身份源部门
+        
+        @param request: CreateIdpDepartmentRequest
+        @return: CreateIdpDepartmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_idp_department_with_options(request, runtime)
 
     async def create_idp_department_async(
         self,
         request: csas_20230120_models.CreateIdpDepartmentRequest,
     ) -> csas_20230120_models.CreateIdpDepartmentResponse:
+        """
+        @summary 创建自定义身份源部门
+        
+        @param request: CreateIdpDepartmentRequest
+        @return: CreateIdpDepartmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_idp_department_with_options_async(request, runtime)
 
     def create_private_access_application_with_options(
         self,
         request: csas_20230120_models.CreatePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreatePrivateAccessApplicationResponse:
+        """
+        @summary 创建内网访问应用
+        
+        @param request: CreatePrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.addresses):
             body_flat['Addresses'] = request.addresses
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
@@ -447,14 +558,21 @@
         )
 
     async def create_private_access_application_with_options_async(
         self,
         request: csas_20230120_models.CreatePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreatePrivateAccessApplicationResponse:
+        """
+        @summary 创建内网访问应用
+        
+        @param request: CreatePrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.addresses):
             body_flat['Addresses'] = request.addresses
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
@@ -489,29 +607,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_private_access_application(
         self,
         request: csas_20230120_models.CreatePrivateAccessApplicationRequest,
     ) -> csas_20230120_models.CreatePrivateAccessApplicationResponse:
+        """
+        @summary 创建内网访问应用
+        
+        @param request: CreatePrivateAccessApplicationRequest
+        @return: CreatePrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_private_access_application_with_options(request, runtime)
 
     async def create_private_access_application_async(
         self,
         request: csas_20230120_models.CreatePrivateAccessApplicationRequest,
     ) -> csas_20230120_models.CreatePrivateAccessApplicationResponse:
+        """
+        @summary 创建内网访问应用
+        
+        @param request: CreatePrivateAccessApplicationRequest
+        @return: CreatePrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_private_access_application_with_options_async(request, runtime)
 
     def create_private_access_policy_with_options(
         self,
         request: csas_20230120_models.CreatePrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreatePrivateAccessPolicyResponse:
+        """
+        @summary 创建内网访问策略
+        
+        @param request: CreatePrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -557,14 +694,21 @@
         )
 
     async def create_private_access_policy_with_options_async(
         self,
         request: csas_20230120_models.CreatePrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreatePrivateAccessPolicyResponse:
+        """
+        @summary 创建内网访问策略
+        
+        @param request: CreatePrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -609,29 +753,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_private_access_policy(
         self,
         request: csas_20230120_models.CreatePrivateAccessPolicyRequest,
     ) -> csas_20230120_models.CreatePrivateAccessPolicyResponse:
+        """
+        @summary 创建内网访问策略
+        
+        @param request: CreatePrivateAccessPolicyRequest
+        @return: CreatePrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_private_access_policy_with_options(request, runtime)
 
     async def create_private_access_policy_async(
         self,
         request: csas_20230120_models.CreatePrivateAccessPolicyRequest,
     ) -> csas_20230120_models.CreatePrivateAccessPolicyResponse:
+        """
+        @summary 创建内网访问策略
+        
+        @param request: CreatePrivateAccessPolicyRequest
+        @return: CreatePrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_private_access_policy_with_options_async(request, runtime)
 
     def create_private_access_tag_with_options(
         self,
         request: csas_20230120_models.CreatePrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreatePrivateAccessTagResponse:
+        """
+        @summary 创建内网访问标签
+        
+        @param request: CreatePrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         req = open_api_models.OpenApiRequest(
@@ -654,14 +817,21 @@
         )
 
     async def create_private_access_tag_with_options_async(
         self,
         request: csas_20230120_models.CreatePrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreatePrivateAccessTagResponse:
+        """
+        @summary 创建内网访问标签
+        
+        @param request: CreatePrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreatePrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.name):
             body['Name'] = request.name
         req = open_api_models.OpenApiRequest(
@@ -683,29 +853,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_private_access_tag(
         self,
         request: csas_20230120_models.CreatePrivateAccessTagRequest,
     ) -> csas_20230120_models.CreatePrivateAccessTagResponse:
+        """
+        @summary 创建内网访问标签
+        
+        @param request: CreatePrivateAccessTagRequest
+        @return: CreatePrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_private_access_tag_with_options(request, runtime)
 
     async def create_private_access_tag_async(
         self,
         request: csas_20230120_models.CreatePrivateAccessTagRequest,
     ) -> csas_20230120_models.CreatePrivateAccessTagResponse:
+        """
+        @summary 创建内网访问标签
+        
+        @param request: CreatePrivateAccessTagRequest
+        @return: CreatePrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_private_access_tag_with_options_async(request, runtime)
 
     def create_registration_policy_with_options(
         self,
         tmp_req: csas_20230120_models.CreateRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateRegistrationPolicyResponse:
+        """
+        @summary 创建设备注册策略
+        
+        @param tmp_req: CreateRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateRegistrationPolicyResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.CreateRegistrationPolicyShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.company_limit_count):
             request.company_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.company_limit_count, 'CompanyLimitCount', 'json')
         if not UtilClient.is_unset(tmp_req.personal_limit_count):
             request.personal_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.personal_limit_count, 'PersonalLimitCount', 'json')
@@ -755,14 +944,21 @@
         )
 
     async def create_registration_policy_with_options_async(
         self,
         tmp_req: csas_20230120_models.CreateRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateRegistrationPolicyResponse:
+        """
+        @summary 创建设备注册策略
+        
+        @param tmp_req: CreateRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateRegistrationPolicyResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.CreateRegistrationPolicyShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.company_limit_count):
             request.company_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.company_limit_count, 'CompanyLimitCount', 'json')
         if not UtilClient.is_unset(tmp_req.personal_limit_count):
             request.personal_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.personal_limit_count, 'PersonalLimitCount', 'json')
@@ -811,29 +1007,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_registration_policy(
         self,
         request: csas_20230120_models.CreateRegistrationPolicyRequest,
     ) -> csas_20230120_models.CreateRegistrationPolicyResponse:
+        """
+        @summary 创建设备注册策略
+        
+        @param request: CreateRegistrationPolicyRequest
+        @return: CreateRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_registration_policy_with_options(request, runtime)
 
     async def create_registration_policy_async(
         self,
         request: csas_20230120_models.CreateRegistrationPolicyRequest,
     ) -> csas_20230120_models.CreateRegistrationPolicyResponse:
+        """
+        @summary 创建设备注册策略
+        
+        @param request: CreateRegistrationPolicyRequest
+        @return: CreateRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_registration_policy_with_options_async(request, runtime)
 
     def create_user_group_with_options(
         self,
         request: csas_20230120_models.CreateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateUserGroupResponse:
+        """
+        @summary 创建用户组
+        
+        @param request: CreateUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.attributes):
             body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
@@ -861,14 +1076,21 @@
         )
 
     async def create_user_group_with_options_async(
         self,
         request: csas_20230120_models.CreateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.CreateUserGroupResponse:
+        """
+        @summary 创建用户组
+        
+        @param request: CreateUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateUserGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.attributes):
             body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
@@ -895,29 +1117,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_user_group(
         self,
         request: csas_20230120_models.CreateUserGroupRequest,
     ) -> csas_20230120_models.CreateUserGroupResponse:
+        """
+        @summary 创建用户组
+        
+        @param request: CreateUserGroupRequest
+        @return: CreateUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_user_group_with_options(request, runtime)
 
     async def create_user_group_async(
         self,
         request: csas_20230120_models.CreateUserGroupRequest,
     ) -> csas_20230120_models.CreateUserGroupResponse:
+        """
+        @summary 创建用户组
+        
+        @param request: CreateUserGroupRequest
+        @return: CreateUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_user_group_with_options_async(request, runtime)
 
     def delete_client_user_with_options(
         self,
         request: csas_20230120_models.DeleteClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteClientUserResponse:
+        """
+        @summary 删除自定义身份源指定用户
+        
+        @param request: DeleteClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -938,14 +1179,21 @@
         )
 
     async def delete_client_user_with_options_async(
         self,
         request: csas_20230120_models.DeleteClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteClientUserResponse:
+        """
+        @summary 删除自定义身份源指定用户
+        
+        @param request: DeleteClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -965,29 +1213,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_client_user(
         self,
         request: csas_20230120_models.DeleteClientUserRequest,
     ) -> csas_20230120_models.DeleteClientUserResponse:
+        """
+        @summary 删除自定义身份源指定用户
+        
+        @param request: DeleteClientUserRequest
+        @return: DeleteClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_client_user_with_options(request, runtime)
 
     async def delete_client_user_async(
         self,
         request: csas_20230120_models.DeleteClientUserRequest,
     ) -> csas_20230120_models.DeleteClientUserResponse:
+        """
+        @summary 删除自定义身份源指定用户
+        
+        @param request: DeleteClientUserRequest
+        @return: DeleteClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_client_user_with_options_async(request, runtime)
 
     def delete_dynamic_route_with_options(
         self,
         request: csas_20230120_models.DeleteDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteDynamicRouteResponse:
+        """
+        @summary 删除动态路由
+        
+        @param request: DeleteDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dynamic_route_id):
             query['DynamicRouteId'] = request.dynamic_route_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1008,14 +1275,21 @@
         )
 
     async def delete_dynamic_route_with_options_async(
         self,
         request: csas_20230120_models.DeleteDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteDynamicRouteResponse:
+        """
+        @summary 删除动态路由
+        
+        @param request: DeleteDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dynamic_route_id):
             query['DynamicRouteId'] = request.dynamic_route_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
@@ -1035,29 +1309,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dynamic_route(
         self,
         request: csas_20230120_models.DeleteDynamicRouteRequest,
     ) -> csas_20230120_models.DeleteDynamicRouteResponse:
+        """
+        @summary 删除动态路由
+        
+        @param request: DeleteDynamicRouteRequest
+        @return: DeleteDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dynamic_route_with_options(request, runtime)
 
     async def delete_dynamic_route_async(
         self,
         request: csas_20230120_models.DeleteDynamicRouteRequest,
     ) -> csas_20230120_models.DeleteDynamicRouteResponse:
+        """
+        @summary 删除动态路由
+        
+        @param request: DeleteDynamicRouteRequest
+        @return: DeleteDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dynamic_route_with_options_async(request, runtime)
 
     def delete_idp_department_with_options(
         self,
         request: csas_20230120_models.DeleteIdpDepartmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
+        """
+        @summary 删除指定自定义身份源部门
+        
+        @param request: DeleteIdpDepartmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteIdpDepartmentResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.idp_config_id):
             query['IdpConfigId'] = request.idp_config_id
         req = open_api_models.OpenApiRequest(
@@ -1080,14 +1373,21 @@
         )
 
     async def delete_idp_department_with_options_async(
         self,
         request: csas_20230120_models.DeleteIdpDepartmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
+        """
+        @summary 删除指定自定义身份源部门
+        
+        @param request: DeleteIdpDepartmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteIdpDepartmentResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.idp_config_id):
             query['IdpConfigId'] = request.idp_config_id
         req = open_api_models.OpenApiRequest(
@@ -1109,29 +1409,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_idp_department(
         self,
         request: csas_20230120_models.DeleteIdpDepartmentRequest,
     ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
+        """
+        @summary 删除指定自定义身份源部门
+        
+        @param request: DeleteIdpDepartmentRequest
+        @return: DeleteIdpDepartmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_idp_department_with_options(request, runtime)
 
     async def delete_idp_department_async(
         self,
         request: csas_20230120_models.DeleteIdpDepartmentRequest,
     ) -> csas_20230120_models.DeleteIdpDepartmentResponse:
+        """
+        @summary 删除指定自定义身份源部门
+        
+        @param request: DeleteIdpDepartmentRequest
+        @return: DeleteIdpDepartmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_idp_department_with_options_async(request, runtime)
 
     def delete_private_access_application_with_options(
         self,
         request: csas_20230120_models.DeletePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeletePrivateAccessApplicationResponse:
+        """
+        @summary 删除内网访问应用
+        
+        @param request: DeletePrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1152,14 +1471,21 @@
         )
 
     async def delete_private_access_application_with_options_async(
         self,
         request: csas_20230120_models.DeletePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeletePrivateAccessApplicationResponse:
+        """
+        @summary 删除内网访问应用
+        
+        @param request: DeletePrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1179,29 +1505,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_private_access_application(
         self,
         request: csas_20230120_models.DeletePrivateAccessApplicationRequest,
     ) -> csas_20230120_models.DeletePrivateAccessApplicationResponse:
+        """
+        @summary 删除内网访问应用
+        
+        @param request: DeletePrivateAccessApplicationRequest
+        @return: DeletePrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_private_access_application_with_options(request, runtime)
 
     async def delete_private_access_application_async(
         self,
         request: csas_20230120_models.DeletePrivateAccessApplicationRequest,
     ) -> csas_20230120_models.DeletePrivateAccessApplicationResponse:
+        """
+        @summary 删除内网访问应用
+        
+        @param request: DeletePrivateAccessApplicationRequest
+        @return: DeletePrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_private_access_application_with_options_async(request, runtime)
 
     def delete_private_access_policy_with_options(
         self,
         request: csas_20230120_models.DeletePrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeletePrivateAccessPolicyResponse:
+        """
+        @summary 删除内网访问策略
+        
+        @param request: DeletePrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.policy_id):
             body['PolicyId'] = request.policy_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1222,14 +1567,21 @@
         )
 
     async def delete_private_access_policy_with_options_async(
         self,
         request: csas_20230120_models.DeletePrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeletePrivateAccessPolicyResponse:
+        """
+        @summary 删除内网访问策略
+        
+        @param request: DeletePrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.policy_id):
             body['PolicyId'] = request.policy_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1249,29 +1601,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_private_access_policy(
         self,
         request: csas_20230120_models.DeletePrivateAccessPolicyRequest,
     ) -> csas_20230120_models.DeletePrivateAccessPolicyResponse:
+        """
+        @summary 删除内网访问策略
+        
+        @param request: DeletePrivateAccessPolicyRequest
+        @return: DeletePrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_private_access_policy_with_options(request, runtime)
 
     async def delete_private_access_policy_async(
         self,
         request: csas_20230120_models.DeletePrivateAccessPolicyRequest,
     ) -> csas_20230120_models.DeletePrivateAccessPolicyResponse:
+        """
+        @summary 删除内网访问策略
+        
+        @param request: DeletePrivateAccessPolicyRequest
+        @return: DeletePrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_private_access_policy_with_options_async(request, runtime)
 
     def delete_private_access_tag_with_options(
         self,
         request: csas_20230120_models.DeletePrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeletePrivateAccessTagResponse:
+        """
+        @summary 删除内网访问标签
+        
+        @param request: DeletePrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.tag_id):
             body['TagId'] = request.tag_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1292,14 +1663,21 @@
         )
 
     async def delete_private_access_tag_with_options_async(
         self,
         request: csas_20230120_models.DeletePrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeletePrivateAccessTagResponse:
+        """
+        @summary 删除内网访问标签
+        
+        @param request: DeletePrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeletePrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.tag_id):
             body['TagId'] = request.tag_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1319,29 +1697,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_private_access_tag(
         self,
         request: csas_20230120_models.DeletePrivateAccessTagRequest,
     ) -> csas_20230120_models.DeletePrivateAccessTagResponse:
+        """
+        @summary 删除内网访问标签
+        
+        @param request: DeletePrivateAccessTagRequest
+        @return: DeletePrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_private_access_tag_with_options(request, runtime)
 
     async def delete_private_access_tag_async(
         self,
         request: csas_20230120_models.DeletePrivateAccessTagRequest,
     ) -> csas_20230120_models.DeletePrivateAccessTagResponse:
+        """
+        @summary 删除内网访问标签
+        
+        @param request: DeletePrivateAccessTagRequest
+        @return: DeletePrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_private_access_tag_with_options_async(request, runtime)
 
     def delete_registration_policies_with_options(
         self,
         request: csas_20230120_models.DeleteRegistrationPoliciesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteRegistrationPoliciesResponse:
+        """
+        @summary 删除设备注册策略
+        
+        @param request: DeleteRegistrationPoliciesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteRegistrationPoliciesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.policy_ids):
             body_flat['PolicyIds'] = request.policy_ids
         body = TeaCore.merge(body,
             OpenApiUtilClient.query(body_flat))
@@ -1365,14 +1762,21 @@
         )
 
     async def delete_registration_policies_with_options_async(
         self,
         request: csas_20230120_models.DeleteRegistrationPoliciesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteRegistrationPoliciesResponse:
+        """
+        @summary 删除设备注册策略
+        
+        @param request: DeleteRegistrationPoliciesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteRegistrationPoliciesResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.policy_ids):
             body_flat['PolicyIds'] = request.policy_ids
         body = TeaCore.merge(body,
             OpenApiUtilClient.query(body_flat))
@@ -1395,29 +1799,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_registration_policies(
         self,
         request: csas_20230120_models.DeleteRegistrationPoliciesRequest,
     ) -> csas_20230120_models.DeleteRegistrationPoliciesResponse:
+        """
+        @summary 删除设备注册策略
+        
+        @param request: DeleteRegistrationPoliciesRequest
+        @return: DeleteRegistrationPoliciesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_registration_policies_with_options(request, runtime)
 
     async def delete_registration_policies_async(
         self,
         request: csas_20230120_models.DeleteRegistrationPoliciesRequest,
     ) -> csas_20230120_models.DeleteRegistrationPoliciesResponse:
+        """
+        @summary 删除设备注册策略
+        
+        @param request: DeleteRegistrationPoliciesRequest
+        @return: DeleteRegistrationPoliciesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_registration_policies_with_options_async(request, runtime)
 
     def delete_user_group_with_options(
         self,
         request: csas_20230120_models.DeleteUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteUserGroupResponse:
+        """
+        @summary 删除用户组
+        
+        @param request: DeleteUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_group_id):
             body['UserGroupId'] = request.user_group_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1438,14 +1861,21 @@
         )
 
     async def delete_user_group_with_options_async(
         self,
         request: csas_20230120_models.DeleteUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DeleteUserGroupResponse:
+        """
+        @summary 删除用户组
+        
+        @param request: DeleteUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteUserGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.user_group_id):
             body['UserGroupId'] = request.user_group_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
         )
@@ -1465,29 +1895,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_user_group(
         self,
         request: csas_20230120_models.DeleteUserGroupRequest,
     ) -> csas_20230120_models.DeleteUserGroupResponse:
+        """
+        @summary 删除用户组
+        
+        @param request: DeleteUserGroupRequest
+        @return: DeleteUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_user_group_with_options(request, runtime)
 
     async def delete_user_group_async(
         self,
         request: csas_20230120_models.DeleteUserGroupRequest,
     ) -> csas_20230120_models.DeleteUserGroupResponse:
+        """
+        @summary 删除用户组
+        
+        @param request: DeleteUserGroupRequest
+        @return: DeleteUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_user_group_with_options_async(request, runtime)
 
     def detach_application_2connector_with_options(
         self,
         tmp_req: csas_20230120_models.DetachApplication2ConnectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DetachApplication2ConnectorResponse:
+        """
+        @summary 卸载connector的应用
+        
+        @param tmp_req: DetachApplication2ConnectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachApplication2ConnectorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.DetachApplication2ConnectorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.application_ids):
             request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.application_ids_shrink):
@@ -1514,14 +1963,21 @@
         )
 
     async def detach_application_2connector_with_options_async(
         self,
         tmp_req: csas_20230120_models.DetachApplication2ConnectorRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.DetachApplication2ConnectorResponse:
+        """
+        @summary 卸载connector的应用
+        
+        @param tmp_req: DetachApplication2ConnectorRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DetachApplication2ConnectorResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.DetachApplication2ConnectorShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.application_ids):
             request.application_ids_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.application_ids, 'ApplicationIds', 'json')
         body = {}
         if not UtilClient.is_unset(request.application_ids_shrink):
@@ -1547,28 +2003,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def detach_application_2connector(
         self,
         request: csas_20230120_models.DetachApplication2ConnectorRequest,
     ) -> csas_20230120_models.DetachApplication2ConnectorResponse:
+        """
+        @summary 卸载connector的应用
+        
+        @param request: DetachApplication2ConnectorRequest
+        @return: DetachApplication2ConnectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.detach_application_2connector_with_options(request, runtime)
 
     async def detach_application_2connector_async(
         self,
         request: csas_20230120_models.DetachApplication2ConnectorRequest,
     ) -> csas_20230120_models.DetachApplication2ConnectorResponse:
+        """
+        @summary 卸载connector的应用
+        
+        @param request: DetachApplication2ConnectorRequest
+        @return: DetachApplication2ConnectorResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.detach_application_2connector_with_options_async(request, runtime)
 
     def get_active_idp_config_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetActiveIdpConfigResponse:
+        """
+        @summary 查询已启用的身份源配置
+        
+        @param request: GetActiveIdpConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetActiveIdpConfigResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetActiveIdpConfig',
             version='2023-01-20',
             protocol='HTTPS',
             pathname='/',
             method='GET',
@@ -1582,14 +2057,21 @@
             self.call_api(params, req, runtime)
         )
 
     async def get_active_idp_config_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetActiveIdpConfigResponse:
+        """
+        @summary 查询已启用的身份源配置
+        
+        @param request: GetActiveIdpConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetActiveIdpConfigResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='GetActiveIdpConfig',
             version='2023-01-20',
             protocol='HTTPS',
             pathname='/',
             method='GET',
@@ -1600,26 +2082,43 @@
         )
         return TeaCore.from_map(
             csas_20230120_models.GetActiveIdpConfigResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def get_active_idp_config(self) -> csas_20230120_models.GetActiveIdpConfigResponse:
+        """
+        @summary 查询已启用的身份源配置
+        
+        @return: GetActiveIdpConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_active_idp_config_with_options(runtime)
 
     async def get_active_idp_config_async(self) -> csas_20230120_models.GetActiveIdpConfigResponse:
+        """
+        @summary 查询已启用的身份源配置
+        
+        @return: GetActiveIdpConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_active_idp_config_with_options_async(runtime)
 
     def get_client_user_with_options(
         self,
         request: csas_20230120_models.GetClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetClientUserResponse:
+        """
+        @summary 查询自定义身份源指定用户
+        
+        @param request: GetClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetClientUser',
@@ -1638,14 +2137,21 @@
         )
 
     async def get_client_user_with_options_async(
         self,
         request: csas_20230120_models.GetClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetClientUserResponse:
+        """
+        @summary 查询自定义身份源指定用户
+        
+        @param request: GetClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetClientUser',
@@ -1663,29 +2169,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_client_user(
         self,
         request: csas_20230120_models.GetClientUserRequest,
     ) -> csas_20230120_models.GetClientUserResponse:
+        """
+        @summary 查询自定义身份源指定用户
+        
+        @param request: GetClientUserRequest
+        @return: GetClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_client_user_with_options(request, runtime)
 
     async def get_client_user_async(
         self,
         request: csas_20230120_models.GetClientUserRequest,
     ) -> csas_20230120_models.GetClientUserResponse:
+        """
+        @summary 查询自定义身份源指定用户
+        
+        @param request: GetClientUserRequest
+        @return: GetClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_client_user_with_options_async(request, runtime)
 
     def get_dynamic_route_with_options(
         self,
         request: csas_20230120_models.GetDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetDynamicRouteResponse:
+        """
+        @summary 查询动态路由详情
+        
+        @param request: GetDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetDynamicRoute',
@@ -1704,14 +2229,21 @@
         )
 
     async def get_dynamic_route_with_options_async(
         self,
         request: csas_20230120_models.GetDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetDynamicRouteResponse:
+        """
+        @summary 查询动态路由详情
+        
+        @param request: GetDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetDynamicRoute',
@@ -1729,29 +2261,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_dynamic_route(
         self,
         request: csas_20230120_models.GetDynamicRouteRequest,
     ) -> csas_20230120_models.GetDynamicRouteResponse:
+        """
+        @summary 查询动态路由详情
+        
+        @param request: GetDynamicRouteRequest
+        @return: GetDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_dynamic_route_with_options(request, runtime)
 
     async def get_dynamic_route_async(
         self,
         request: csas_20230120_models.GetDynamicRouteRequest,
     ) -> csas_20230120_models.GetDynamicRouteResponse:
+        """
+        @summary 查询动态路由详情
+        
+        @param request: GetDynamicRouteRequest
+        @return: GetDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_dynamic_route_with_options_async(request, runtime)
 
     def get_idp_config_with_options(
         self,
         request: csas_20230120_models.GetIdpConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetIdpConfigResponse:
+        """
+        @summary 查询身份源配置详情
+        
+        @param request: GetIdpConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetIdpConfigResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetIdpConfig',
@@ -1770,14 +2321,21 @@
         )
 
     async def get_idp_config_with_options_async(
         self,
         request: csas_20230120_models.GetIdpConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetIdpConfigResponse:
+        """
+        @summary 查询身份源配置详情
+        
+        @param request: GetIdpConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetIdpConfigResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetIdpConfig',
@@ -1795,29 +2353,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_idp_config(
         self,
         request: csas_20230120_models.GetIdpConfigRequest,
     ) -> csas_20230120_models.GetIdpConfigResponse:
+        """
+        @summary 查询身份源配置详情
+        
+        @param request: GetIdpConfigRequest
+        @return: GetIdpConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_idp_config_with_options(request, runtime)
 
     async def get_idp_config_async(
         self,
         request: csas_20230120_models.GetIdpConfigRequest,
     ) -> csas_20230120_models.GetIdpConfigResponse:
+        """
+        @summary 查询身份源配置详情
+        
+        @param request: GetIdpConfigRequest
+        @return: GetIdpConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_idp_config_with_options_async(request, runtime)
 
     def get_private_access_application_with_options(
         self,
         request: csas_20230120_models.GetPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetPrivateAccessApplicationResponse:
+        """
+        @summary 查询内网访问应用详情
+        
+        @param request: GetPrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPrivateAccessApplication',
@@ -1836,14 +2413,21 @@
         )
 
     async def get_private_access_application_with_options_async(
         self,
         request: csas_20230120_models.GetPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetPrivateAccessApplicationResponse:
+        """
+        @summary 查询内网访问应用详情
+        
+        @param request: GetPrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPrivateAccessApplication',
@@ -1861,29 +2445,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_private_access_application(
         self,
         request: csas_20230120_models.GetPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.GetPrivateAccessApplicationResponse:
+        """
+        @summary 查询内网访问应用详情
+        
+        @param request: GetPrivateAccessApplicationRequest
+        @return: GetPrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_private_access_application_with_options(request, runtime)
 
     async def get_private_access_application_async(
         self,
         request: csas_20230120_models.GetPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.GetPrivateAccessApplicationResponse:
+        """
+        @summary 查询内网访问应用详情
+        
+        @param request: GetPrivateAccessApplicationRequest
+        @return: GetPrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_private_access_application_with_options_async(request, runtime)
 
     def get_private_access_policy_with_options(
         self,
         request: csas_20230120_models.GetPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetPrivateAccessPolicyResponse:
+        """
+        @summary 查询内网访问策略详情
+        
+        @param request: GetPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPrivateAccessPolicy',
@@ -1902,14 +2505,21 @@
         )
 
     async def get_private_access_policy_with_options_async(
         self,
         request: csas_20230120_models.GetPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetPrivateAccessPolicyResponse:
+        """
+        @summary 查询内网访问策略详情
+        
+        @param request: GetPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetPrivateAccessPolicy',
@@ -1927,29 +2537,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_private_access_policy(
         self,
         request: csas_20230120_models.GetPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.GetPrivateAccessPolicyResponse:
+        """
+        @summary 查询内网访问策略详情
+        
+        @param request: GetPrivateAccessPolicyRequest
+        @return: GetPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_private_access_policy_with_options(request, runtime)
 
     async def get_private_access_policy_async(
         self,
         request: csas_20230120_models.GetPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.GetPrivateAccessPolicyResponse:
+        """
+        @summary 查询内网访问策略详情
+        
+        @param request: GetPrivateAccessPolicyRequest
+        @return: GetPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_private_access_policy_with_options_async(request, runtime)
 
     def get_registration_policy_with_options(
         self,
         request: csas_20230120_models.GetRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略详情
+        
+        @param request: GetRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetRegistrationPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetRegistrationPolicy',
@@ -1968,14 +2597,21 @@
         )
 
     async def get_registration_policy_with_options_async(
         self,
         request: csas_20230120_models.GetRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略详情
+        
+        @param request: GetRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetRegistrationPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetRegistrationPolicy',
@@ -1993,29 +2629,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_registration_policy(
         self,
         request: csas_20230120_models.GetRegistrationPolicyRequest,
     ) -> csas_20230120_models.GetRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略详情
+        
+        @param request: GetRegistrationPolicyRequest
+        @return: GetRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_registration_policy_with_options(request, runtime)
 
     async def get_registration_policy_async(
         self,
         request: csas_20230120_models.GetRegistrationPolicyRequest,
     ) -> csas_20230120_models.GetRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略详情
+        
+        @param request: GetRegistrationPolicyRequest
+        @return: GetRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_registration_policy_with_options_async(request, runtime)
 
     def get_user_device_with_options(
         self,
         request: csas_20230120_models.GetUserDeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetUserDeviceResponse:
+        """
+        @summary 查询用户设备详情
+        
+        @param request: GetUserDeviceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserDeviceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetUserDevice',
@@ -2034,14 +2689,21 @@
         )
 
     async def get_user_device_with_options_async(
         self,
         request: csas_20230120_models.GetUserDeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetUserDeviceResponse:
+        """
+        @summary 查询用户设备详情
+        
+        @param request: GetUserDeviceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserDeviceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetUserDevice',
@@ -2059,29 +2721,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_device(
         self,
         request: csas_20230120_models.GetUserDeviceRequest,
     ) -> csas_20230120_models.GetUserDeviceResponse:
+        """
+        @summary 查询用户设备详情
+        
+        @param request: GetUserDeviceRequest
+        @return: GetUserDeviceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_device_with_options(request, runtime)
 
     async def get_user_device_async(
         self,
         request: csas_20230120_models.GetUserDeviceRequest,
     ) -> csas_20230120_models.GetUserDeviceResponse:
+        """
+        @summary 查询用户设备详情
+        
+        @param request: GetUserDeviceRequest
+        @return: GetUserDeviceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_device_with_options_async(request, runtime)
 
     def get_user_group_with_options(
         self,
         request: csas_20230120_models.GetUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetUserGroupResponse:
+        """
+        @summary 查询用户组详情
+        
+        @param request: GetUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserGroupResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetUserGroup',
@@ -2100,14 +2781,21 @@
         )
 
     async def get_user_group_with_options_async(
         self,
         request: csas_20230120_models.GetUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.GetUserGroupResponse:
+        """
+        @summary 查询用户组详情
+        
+        @param request: GetUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetUserGroupResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='GetUserGroup',
@@ -2125,29 +2813,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_user_group(
         self,
         request: csas_20230120_models.GetUserGroupRequest,
     ) -> csas_20230120_models.GetUserGroupResponse:
+        """
+        @summary 查询用户组详情
+        
+        @param request: GetUserGroupRequest
+        @return: GetUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_user_group_with_options(request, runtime)
 
     async def get_user_group_async(
         self,
         request: csas_20230120_models.GetUserGroupRequest,
     ) -> csas_20230120_models.GetUserGroupResponse:
+        """
+        @summary 查询用户组详情
+        
+        @param request: GetUserGroupRequest
+        @return: GetUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_user_group_with_options_async(request, runtime)
 
     def list_applications_for_private_access_policy_with_options(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的应用
+        
+        @param request: ListApplicationsForPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListApplicationsForPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessPolicy',
@@ -2166,14 +2873,21 @@
         )
 
     async def list_applications_for_private_access_policy_with_options_async(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的应用
+        
+        @param request: ListApplicationsForPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListApplicationsForPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessPolicy',
@@ -2191,29 +2905,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_applications_for_private_access_policy(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的应用
+        
+        @param request: ListApplicationsForPrivateAccessPolicyRequest
+        @return: ListApplicationsForPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_applications_for_private_access_policy_with_options(request, runtime)
 
     async def list_applications_for_private_access_policy_async(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的应用
+        
+        @param request: ListApplicationsForPrivateAccessPolicyRequest
+        @return: ListApplicationsForPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_applications_for_private_access_policy_with_options_async(request, runtime)
 
     def list_applications_for_private_access_tag_with_options(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的应用
+        
+        @param request: ListApplicationsForPrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListApplicationsForPrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessTag',
@@ -2232,14 +2965,21 @@
         )
 
     async def list_applications_for_private_access_tag_with_options_async(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的应用
+        
+        @param request: ListApplicationsForPrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListApplicationsForPrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListApplicationsForPrivateAccessTag',
@@ -2257,29 +2997,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_applications_for_private_access_tag(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的应用
+        
+        @param request: ListApplicationsForPrivateAccessTagRequest
+        @return: ListApplicationsForPrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_applications_for_private_access_tag_with_options(request, runtime)
 
     async def list_applications_for_private_access_tag_async(
         self,
         request: csas_20230120_models.ListApplicationsForPrivateAccessTagRequest,
     ) -> csas_20230120_models.ListApplicationsForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的应用
+        
+        @param request: ListApplicationsForPrivateAccessTagRequest
+        @return: ListApplicationsForPrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_applications_for_private_access_tag_with_options_async(request, runtime)
 
     def list_client_users_with_options(
         self,
         request: csas_20230120_models.ListClientUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListClientUsersResponse:
+        """
+        @summary 查询自定义身份源用户
+        
+        @param request: ListClientUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListClientUsersResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListClientUsers',
@@ -2298,14 +3057,21 @@
         )
 
     async def list_client_users_with_options_async(
         self,
         request: csas_20230120_models.ListClientUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListClientUsersResponse:
+        """
+        @summary 查询自定义身份源用户
+        
+        @param request: ListClientUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListClientUsersResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListClientUsers',
@@ -2323,29 +3089,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_client_users(
         self,
         request: csas_20230120_models.ListClientUsersRequest,
     ) -> csas_20230120_models.ListClientUsersResponse:
+        """
+        @summary 查询自定义身份源用户
+        
+        @param request: ListClientUsersRequest
+        @return: ListClientUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_client_users_with_options(request, runtime)
 
     async def list_client_users_async(
         self,
         request: csas_20230120_models.ListClientUsersRequest,
     ) -> csas_20230120_models.ListClientUsersResponse:
+        """
+        @summary 查询自定义身份源用户
+        
+        @param request: ListClientUsersRequest
+        @return: ListClientUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_client_users_with_options_async(request, runtime)
 
     def list_connectors_with_options(
         self,
         request: csas_20230120_models.ListConnectorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListConnectorsResponse:
+        """
+        @summary 批量查询connector
+        
+        @param request: ListConnectorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConnectorsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListConnectors',
@@ -2364,14 +3149,21 @@
         )
 
     async def list_connectors_with_options_async(
         self,
         request: csas_20230120_models.ListConnectorsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListConnectorsResponse:
+        """
+        @summary 批量查询connector
+        
+        @param request: ListConnectorsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListConnectorsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListConnectors',
@@ -2389,28 +3181,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_connectors(
         self,
         request: csas_20230120_models.ListConnectorsRequest,
     ) -> csas_20230120_models.ListConnectorsResponse:
+        """
+        @summary 批量查询connector
+        
+        @param request: ListConnectorsRequest
+        @return: ListConnectorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_connectors_with_options(request, runtime)
 
     async def list_connectors_async(
         self,
         request: csas_20230120_models.ListConnectorsRequest,
     ) -> csas_20230120_models.ListConnectorsResponse:
+        """
+        @summary 批量查询connector
+        
+        @param request: ListConnectorsRequest
+        @return: ListConnectorsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_connectors_with_options_async(request, runtime)
 
     def list_dynamic_route_regions_with_options(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListDynamicRouteRegionsResponse:
+        """
+        @summary 批量查询动态路由的地域
+        
+        @param request: ListDynamicRouteRegionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDynamicRouteRegionsResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='ListDynamicRouteRegions',
             version='2023-01-20',
             protocol='HTTPS',
             pathname='/',
             method='GET',
@@ -2424,14 +3235,21 @@
             self.call_api(params, req, runtime)
         )
 
     async def list_dynamic_route_regions_with_options_async(
         self,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListDynamicRouteRegionsResponse:
+        """
+        @summary 批量查询动态路由的地域
+        
+        @param request: ListDynamicRouteRegionsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDynamicRouteRegionsResponse
+        """
         req = open_api_models.OpenApiRequest()
         params = open_api_models.Params(
             action='ListDynamicRouteRegions',
             version='2023-01-20',
             protocol='HTTPS',
             pathname='/',
             method='GET',
@@ -2442,26 +3260,43 @@
         )
         return TeaCore.from_map(
             csas_20230120_models.ListDynamicRouteRegionsResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
     def list_dynamic_route_regions(self) -> csas_20230120_models.ListDynamicRouteRegionsResponse:
+        """
+        @summary 批量查询动态路由的地域
+        
+        @return: ListDynamicRouteRegionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_dynamic_route_regions_with_options(runtime)
 
     async def list_dynamic_route_regions_async(self) -> csas_20230120_models.ListDynamicRouteRegionsResponse:
+        """
+        @summary 批量查询动态路由的地域
+        
+        @return: ListDynamicRouteRegionsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_dynamic_route_regions_with_options_async(runtime)
 
     def list_dynamic_routes_with_options(
         self,
         request: csas_20230120_models.ListDynamicRoutesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListDynamicRoutesResponse:
+        """
+        @summary 批量查询动态路由
+        
+        @param request: ListDynamicRoutesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDynamicRoutesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListDynamicRoutes',
@@ -2480,14 +3315,21 @@
         )
 
     async def list_dynamic_routes_with_options_async(
         self,
         request: csas_20230120_models.ListDynamicRoutesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListDynamicRoutesResponse:
+        """
+        @summary 批量查询动态路由
+        
+        @param request: ListDynamicRoutesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDynamicRoutesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListDynamicRoutes',
@@ -2505,29 +3347,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_dynamic_routes(
         self,
         request: csas_20230120_models.ListDynamicRoutesRequest,
     ) -> csas_20230120_models.ListDynamicRoutesResponse:
+        """
+        @summary 批量查询动态路由
+        
+        @param request: ListDynamicRoutesRequest
+        @return: ListDynamicRoutesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_dynamic_routes_with_options(request, runtime)
 
     async def list_dynamic_routes_async(
         self,
         request: csas_20230120_models.ListDynamicRoutesRequest,
     ) -> csas_20230120_models.ListDynamicRoutesResponse:
+        """
+        @summary 批量查询动态路由
+        
+        @param request: ListDynamicRoutesRequest
+        @return: ListDynamicRoutesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_dynamic_routes_with_options_async(request, runtime)
 
     def list_excessive_device_registration_applications_with_options(
         self,
         request: csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsResponse:
+        """
+        @summary 批量查询超额注册申请列表
+        
+        @param request: ListExcessiveDeviceRegistrationApplicationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListExcessiveDeviceRegistrationApplicationsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListExcessiveDeviceRegistrationApplications',
@@ -2546,14 +3407,21 @@
         )
 
     async def list_excessive_device_registration_applications_with_options_async(
         self,
         request: csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsResponse:
+        """
+        @summary 批量查询超额注册申请列表
+        
+        @param request: ListExcessiveDeviceRegistrationApplicationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListExcessiveDeviceRegistrationApplicationsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListExcessiveDeviceRegistrationApplications',
@@ -2571,29 +3439,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_excessive_device_registration_applications(
         self,
         request: csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsRequest,
     ) -> csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsResponse:
+        """
+        @summary 批量查询超额注册申请列表
+        
+        @param request: ListExcessiveDeviceRegistrationApplicationsRequest
+        @return: ListExcessiveDeviceRegistrationApplicationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_excessive_device_registration_applications_with_options(request, runtime)
 
     async def list_excessive_device_registration_applications_async(
         self,
         request: csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsRequest,
     ) -> csas_20230120_models.ListExcessiveDeviceRegistrationApplicationsResponse:
+        """
+        @summary 批量查询超额注册申请列表
+        
+        @param request: ListExcessiveDeviceRegistrationApplicationsRequest
+        @return: ListExcessiveDeviceRegistrationApplicationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_excessive_device_registration_applications_with_options_async(request, runtime)
 
     def list_idp_configs_with_options(
         self,
         request: csas_20230120_models.ListIdpConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListIdpConfigsResponse:
+        """
+        @summary 查询IDP配置
+        
+        @param request: ListIdpConfigsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListIdpConfigsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListIdpConfigs',
@@ -2612,14 +3499,21 @@
         )
 
     async def list_idp_configs_with_options_async(
         self,
         request: csas_20230120_models.ListIdpConfigsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListIdpConfigsResponse:
+        """
+        @summary 查询IDP配置
+        
+        @param request: ListIdpConfigsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListIdpConfigsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListIdpConfigs',
@@ -2637,29 +3531,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_idp_configs(
         self,
         request: csas_20230120_models.ListIdpConfigsRequest,
     ) -> csas_20230120_models.ListIdpConfigsResponse:
+        """
+        @summary 查询IDP配置
+        
+        @param request: ListIdpConfigsRequest
+        @return: ListIdpConfigsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_idp_configs_with_options(request, runtime)
 
     async def list_idp_configs_async(
         self,
         request: csas_20230120_models.ListIdpConfigsRequest,
     ) -> csas_20230120_models.ListIdpConfigsResponse:
+        """
+        @summary 查询IDP配置
+        
+        @param request: ListIdpConfigsRequest
+        @return: ListIdpConfigsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_idp_configs_with_options_async(request, runtime)
 
     def list_idp_departments_with_options(
         self,
         request: csas_20230120_models.ListIdpDepartmentsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListIdpDepartmentsResponse:
+        """
+        @summary 查询自定义身份源部门
+        
+        @param request: ListIdpDepartmentsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListIdpDepartmentsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListIdpDepartments',
@@ -2678,14 +3591,21 @@
         )
 
     async def list_idp_departments_with_options_async(
         self,
         request: csas_20230120_models.ListIdpDepartmentsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListIdpDepartmentsResponse:
+        """
+        @summary 查询自定义身份源部门
+        
+        @param request: ListIdpDepartmentsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListIdpDepartmentsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListIdpDepartments',
@@ -2703,29 +3623,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_idp_departments(
         self,
         request: csas_20230120_models.ListIdpDepartmentsRequest,
     ) -> csas_20230120_models.ListIdpDepartmentsResponse:
+        """
+        @summary 查询自定义身份源部门
+        
+        @param request: ListIdpDepartmentsRequest
+        @return: ListIdpDepartmentsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_idp_departments_with_options(request, runtime)
 
     async def list_idp_departments_async(
         self,
         request: csas_20230120_models.ListIdpDepartmentsRequest,
     ) -> csas_20230120_models.ListIdpDepartmentsResponse:
+        """
+        @summary 查询自定义身份源部门
+        
+        @param request: ListIdpDepartmentsRequest
+        @return: ListIdpDepartmentsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_idp_departments_with_options_async(request, runtime)
 
     def list_polices_for_private_access_application_with_options(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的策略
+        
+        @param request: ListPolicesForPrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPolicesForPrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessApplication',
@@ -2744,14 +3683,21 @@
         )
 
     async def list_polices_for_private_access_application_with_options_async(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的策略
+        
+        @param request: ListPolicesForPrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPolicesForPrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessApplication',
@@ -2769,29 +3715,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_polices_for_private_access_application(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的策略
+        
+        @param request: ListPolicesForPrivateAccessApplicationRequest
+        @return: ListPolicesForPrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_polices_for_private_access_application_with_options(request, runtime)
 
     async def list_polices_for_private_access_application_async(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的策略
+        
+        @param request: ListPolicesForPrivateAccessApplicationRequest
+        @return: ListPolicesForPrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_polices_for_private_access_application_with_options_async(request, runtime)
 
     def list_polices_for_private_access_tag_with_options(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的策略
+        
+        @param request: ListPolicesForPrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPolicesForPrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessTag',
@@ -2810,14 +3775,21 @@
         )
 
     async def list_polices_for_private_access_tag_with_options_async(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的策略
+        
+        @param request: ListPolicesForPrivateAccessTagRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPolicesForPrivateAccessTagResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForPrivateAccessTag',
@@ -2835,29 +3807,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_polices_for_private_access_tag(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的策略
+        
+        @param request: ListPolicesForPrivateAccessTagRequest
+        @return: ListPolicesForPrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_polices_for_private_access_tag_with_options(request, runtime)
 
     async def list_polices_for_private_access_tag_async(
         self,
         request: csas_20230120_models.ListPolicesForPrivateAccessTagRequest,
     ) -> csas_20230120_models.ListPolicesForPrivateAccessTagResponse:
+        """
+        @summary 批量查询内网访问标签的策略
+        
+        @param request: ListPolicesForPrivateAccessTagRequest
+        @return: ListPolicesForPrivateAccessTagResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_polices_for_private_access_tag_with_options_async(request, runtime)
 
     def list_polices_for_user_group_with_options(
         self,
         request: csas_20230120_models.ListPolicesForUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
+        """
+        @summary 批量查询用户组的策略
+        
+        @param request: ListPolicesForUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPolicesForUserGroupResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForUserGroup',
@@ -2876,14 +3867,21 @@
         )
 
     async def list_polices_for_user_group_with_options_async(
         self,
         request: csas_20230120_models.ListPolicesForUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
+        """
+        @summary 批量查询用户组的策略
+        
+        @param request: ListPolicesForUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPolicesForUserGroupResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPolicesForUserGroup',
@@ -2901,29 +3899,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_polices_for_user_group(
         self,
         request: csas_20230120_models.ListPolicesForUserGroupRequest,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
+        """
+        @summary 批量查询用户组的策略
+        
+        @param request: ListPolicesForUserGroupRequest
+        @return: ListPolicesForUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_polices_for_user_group_with_options(request, runtime)
 
     async def list_polices_for_user_group_async(
         self,
         request: csas_20230120_models.ListPolicesForUserGroupRequest,
     ) -> csas_20230120_models.ListPolicesForUserGroupResponse:
+        """
+        @summary 批量查询用户组的策略
+        
+        @param request: ListPolicesForUserGroupRequest
+        @return: ListPolicesForUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_polices_for_user_group_with_options_async(request, runtime)
 
     def list_pop_traffic_statistics_with_options(
         self,
         request: csas_20230120_models.ListPopTrafficStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        """
+        @summary pop节点流量统计
+        
+        @param request: ListPopTrafficStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPopTrafficStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPopTrafficStatistics',
@@ -2942,14 +3959,21 @@
         )
 
     async def list_pop_traffic_statistics_with_options_async(
         self,
         request: csas_20230120_models.ListPopTrafficStatisticsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        """
+        @summary pop节点流量统计
+        
+        @param request: ListPopTrafficStatisticsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPopTrafficStatisticsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPopTrafficStatistics',
@@ -2967,29 +3991,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_pop_traffic_statistics(
         self,
         request: csas_20230120_models.ListPopTrafficStatisticsRequest,
     ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        """
+        @summary pop节点流量统计
+        
+        @param request: ListPopTrafficStatisticsRequest
+        @return: ListPopTrafficStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_pop_traffic_statistics_with_options(request, runtime)
 
     async def list_pop_traffic_statistics_async(
         self,
         request: csas_20230120_models.ListPopTrafficStatisticsRequest,
     ) -> csas_20230120_models.ListPopTrafficStatisticsResponse:
+        """
+        @summary pop节点流量统计
+        
+        @param request: ListPopTrafficStatisticsRequest
+        @return: ListPopTrafficStatisticsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_pop_traffic_statistics_with_options_async(request, runtime)
 
     def list_private_access_applications_with_options(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
+        """
+        @summary 批量查询内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessApplicationsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessApplications',
@@ -3008,14 +4051,21 @@
         )
 
     async def list_private_access_applications_with_options_async(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
+        """
+        @summary 批量查询内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessApplicationsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessApplications',
@@ -3033,29 +4083,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_private_access_applications(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
+        """
+        @summary 批量查询内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsRequest
+        @return: ListPrivateAccessApplicationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_applications_with_options(request, runtime)
 
     async def list_private_access_applications_async(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsRequest,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsResponse:
+        """
+        @summary 批量查询内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsRequest
+        @return: ListPrivateAccessApplicationsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_applications_with_options_async(request, runtime)
 
     def list_private_access_applications_for_dynamic_route_with_options(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsForDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessApplicationsForDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessApplicationsForDynamicRoute',
@@ -3074,14 +4143,21 @@
         )
 
     async def list_private_access_applications_for_dynamic_route_with_options_async(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsForDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessApplicationsForDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessApplicationsForDynamicRoute',
@@ -3099,29 +4175,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_private_access_applications_for_dynamic_route(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteRequest,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsForDynamicRouteRequest
+        @return: ListPrivateAccessApplicationsForDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_applications_for_dynamic_route_with_options(request, runtime)
 
     async def list_private_access_applications_for_dynamic_route_async(
         self,
         request: csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteRequest,
     ) -> csas_20230120_models.ListPrivateAccessApplicationsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问应用
+        
+        @param request: ListPrivateAccessApplicationsForDynamicRouteRequest
+        @return: ListPrivateAccessApplicationsForDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_applications_for_dynamic_route_with_options_async(request, runtime)
 
     def list_private_access_polices_with_options(
         self,
         request: csas_20230120_models.ListPrivateAccessPolicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessPolicesResponse:
+        """
+        @summary 批量查询内网访问策略
+        
+        @param request: ListPrivateAccessPolicesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessPolicesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessPolices',
@@ -3140,14 +4235,21 @@
         )
 
     async def list_private_access_polices_with_options_async(
         self,
         request: csas_20230120_models.ListPrivateAccessPolicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessPolicesResponse:
+        """
+        @summary 批量查询内网访问策略
+        
+        @param request: ListPrivateAccessPolicesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessPolicesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessPolices',
@@ -3165,29 +4267,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_private_access_polices(
         self,
         request: csas_20230120_models.ListPrivateAccessPolicesRequest,
     ) -> csas_20230120_models.ListPrivateAccessPolicesResponse:
+        """
+        @summary 批量查询内网访问策略
+        
+        @param request: ListPrivateAccessPolicesRequest
+        @return: ListPrivateAccessPolicesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_polices_with_options(request, runtime)
 
     async def list_private_access_polices_async(
         self,
         request: csas_20230120_models.ListPrivateAccessPolicesRequest,
     ) -> csas_20230120_models.ListPrivateAccessPolicesResponse:
+        """
+        @summary 批量查询内网访问策略
+        
+        @param request: ListPrivateAccessPolicesRequest
+        @return: ListPrivateAccessPolicesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_polices_with_options_async(request, runtime)
 
     def list_private_access_tags_with_options(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessTagsResponse:
+        """
+        @summary Queries the information about all internal access tags within the current Alibaba Cloud account.
+        
+        @param request: ListPrivateAccessTagsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessTagsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessTags',
@@ -3206,14 +4327,21 @@
         )
 
     async def list_private_access_tags_with_options_async(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessTagsResponse:
+        """
+        @summary Queries the information about all internal access tags within the current Alibaba Cloud account.
+        
+        @param request: ListPrivateAccessTagsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessTagsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessTags',
@@ -3231,29 +4359,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_private_access_tags(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsRequest,
     ) -> csas_20230120_models.ListPrivateAccessTagsResponse:
+        """
+        @summary Queries the information about all internal access tags within the current Alibaba Cloud account.
+        
+        @param request: ListPrivateAccessTagsRequest
+        @return: ListPrivateAccessTagsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_tags_with_options(request, runtime)
 
     async def list_private_access_tags_async(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsRequest,
     ) -> csas_20230120_models.ListPrivateAccessTagsResponse:
+        """
+        @summary Queries the information about all internal access tags within the current Alibaba Cloud account.
+        
+        @param request: ListPrivateAccessTagsRequest
+        @return: ListPrivateAccessTagsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_tags_with_options_async(request, runtime)
 
     def list_private_access_tags_for_dynamic_route_with_options(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsForDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessTagsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问标签
+        
+        @param request: ListPrivateAccessTagsForDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessTagsForDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessTagsForDynamicRoute',
@@ -3272,14 +4419,21 @@
         )
 
     async def list_private_access_tags_for_dynamic_route_with_options_async(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsForDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListPrivateAccessTagsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问标签
+        
+        @param request: ListPrivateAccessTagsForDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListPrivateAccessTagsForDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListPrivateAccessTagsForDynamicRoute',
@@ -3297,29 +4451,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_private_access_tags_for_dynamic_route(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsForDynamicRouteRequest,
     ) -> csas_20230120_models.ListPrivateAccessTagsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问标签
+        
+        @param request: ListPrivateAccessTagsForDynamicRouteRequest
+        @return: ListPrivateAccessTagsForDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_private_access_tags_for_dynamic_route_with_options(request, runtime)
 
     async def list_private_access_tags_for_dynamic_route_async(
         self,
         request: csas_20230120_models.ListPrivateAccessTagsForDynamicRouteRequest,
     ) -> csas_20230120_models.ListPrivateAccessTagsForDynamicRouteResponse:
+        """
+        @summary 批量查询动态路由的内网访问标签
+        
+        @param request: ListPrivateAccessTagsForDynamicRouteRequest
+        @return: ListPrivateAccessTagsForDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_private_access_tags_for_dynamic_route_with_options_async(request, runtime)
 
     def list_registration_policies_with_options(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListRegistrationPoliciesResponse:
+        """
+        @summary 查询用户设备注册策略列表
+        
+        @param request: ListRegistrationPoliciesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRegistrationPoliciesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRegistrationPolicies',
@@ -3338,14 +4511,21 @@
         )
 
     async def list_registration_policies_with_options_async(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListRegistrationPoliciesResponse:
+        """
+        @summary 查询用户设备注册策略列表
+        
+        @param request: ListRegistrationPoliciesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRegistrationPoliciesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRegistrationPolicies',
@@ -3363,29 +4543,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_registration_policies(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesRequest,
     ) -> csas_20230120_models.ListRegistrationPoliciesResponse:
+        """
+        @summary 查询用户设备注册策略列表
+        
+        @param request: ListRegistrationPoliciesRequest
+        @return: ListRegistrationPoliciesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_registration_policies_with_options(request, runtime)
 
     async def list_registration_policies_async(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesRequest,
     ) -> csas_20230120_models.ListRegistrationPoliciesResponse:
+        """
+        @summary 查询用户设备注册策略列表
+        
+        @param request: ListRegistrationPoliciesRequest
+        @return: ListRegistrationPoliciesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_registration_policies_with_options_async(request, runtime)
 
     def list_registration_policies_for_user_group_with_options(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesForUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListRegistrationPoliciesForUserGroupResponse:
+        """
+        @summary 查询用户组相关的设备注册策略
+        
+        @param request: ListRegistrationPoliciesForUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRegistrationPoliciesForUserGroupResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRegistrationPoliciesForUserGroup',
@@ -3404,14 +4603,21 @@
         )
 
     async def list_registration_policies_for_user_group_with_options_async(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesForUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListRegistrationPoliciesForUserGroupResponse:
+        """
+        @summary 查询用户组相关的设备注册策略
+        
+        @param request: ListRegistrationPoliciesForUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListRegistrationPoliciesForUserGroupResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListRegistrationPoliciesForUserGroup',
@@ -3429,29 +4635,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_registration_policies_for_user_group(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesForUserGroupRequest,
     ) -> csas_20230120_models.ListRegistrationPoliciesForUserGroupResponse:
+        """
+        @summary 查询用户组相关的设备注册策略
+        
+        @param request: ListRegistrationPoliciesForUserGroupRequest
+        @return: ListRegistrationPoliciesForUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_registration_policies_for_user_group_with_options(request, runtime)
 
     async def list_registration_policies_for_user_group_async(
         self,
         request: csas_20230120_models.ListRegistrationPoliciesForUserGroupRequest,
     ) -> csas_20230120_models.ListRegistrationPoliciesForUserGroupResponse:
+        """
+        @summary 查询用户组相关的设备注册策略
+        
+        @param request: ListRegistrationPoliciesForUserGroupRequest
+        @return: ListRegistrationPoliciesForUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_registration_policies_for_user_group_with_options_async(request, runtime)
 
     def list_software_for_user_device_with_options(
         self,
         request: csas_20230120_models.ListSoftwareForUserDeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListSoftwareForUserDeviceResponse:
+        """
+        @summary 批量查询终端安装软件列表
+        
+        @param request: ListSoftwareForUserDeviceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSoftwareForUserDeviceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListSoftwareForUserDevice',
@@ -3470,14 +4695,21 @@
         )
 
     async def list_software_for_user_device_with_options_async(
         self,
         request: csas_20230120_models.ListSoftwareForUserDeviceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListSoftwareForUserDeviceResponse:
+        """
+        @summary 批量查询终端安装软件列表
+        
+        @param request: ListSoftwareForUserDeviceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSoftwareForUserDeviceResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListSoftwareForUserDevice',
@@ -3495,29 +4727,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_software_for_user_device(
         self,
         request: csas_20230120_models.ListSoftwareForUserDeviceRequest,
     ) -> csas_20230120_models.ListSoftwareForUserDeviceResponse:
+        """
+        @summary 批量查询终端安装软件列表
+        
+        @param request: ListSoftwareForUserDeviceRequest
+        @return: ListSoftwareForUserDeviceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_software_for_user_device_with_options(request, runtime)
 
     async def list_software_for_user_device_async(
         self,
         request: csas_20230120_models.ListSoftwareForUserDeviceRequest,
     ) -> csas_20230120_models.ListSoftwareForUserDeviceResponse:
+        """
+        @summary 批量查询终端安装软件列表
+        
+        @param request: ListSoftwareForUserDeviceRequest
+        @return: ListSoftwareForUserDeviceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_software_for_user_device_with_options_async(request, runtime)
 
     def list_tags_for_private_access_application_with_options(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的标签
+        
+        @param request: ListTagsForPrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagsForPrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessApplication',
@@ -3536,14 +4787,21 @@
         )
 
     async def list_tags_for_private_access_application_with_options_async(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的标签
+        
+        @param request: ListTagsForPrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagsForPrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessApplication',
@@ -3561,29 +4819,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tags_for_private_access_application(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.ListTagsForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的标签
+        
+        @param request: ListTagsForPrivateAccessApplicationRequest
+        @return: ListTagsForPrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_tags_for_private_access_application_with_options(request, runtime)
 
     async def list_tags_for_private_access_application_async(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessApplicationRequest,
     ) -> csas_20230120_models.ListTagsForPrivateAccessApplicationResponse:
+        """
+        @summary 批量查询内网访问应用的标签
+        
+        @param request: ListTagsForPrivateAccessApplicationRequest
+        @return: ListTagsForPrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_tags_for_private_access_application_with_options_async(request, runtime)
 
     def list_tags_for_private_access_policy_with_options(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的标签
+        
+        @param request: ListTagsForPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagsForPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessPolicy',
@@ -3602,14 +4879,21 @@
         )
 
     async def list_tags_for_private_access_policy_with_options_async(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListTagsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的标签
+        
+        @param request: ListTagsForPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTagsForPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTagsForPrivateAccessPolicy',
@@ -3627,29 +4911,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_tags_for_private_access_policy(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListTagsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的标签
+        
+        @param request: ListTagsForPrivateAccessPolicyRequest
+        @return: ListTagsForPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_tags_for_private_access_policy_with_options(request, runtime)
 
     async def list_tags_for_private_access_policy_async(
         self,
         request: csas_20230120_models.ListTagsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListTagsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的标签
+        
+        @param request: ListTagsForPrivateAccessPolicyRequest
+        @return: ListTagsForPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_tags_for_private_access_policy_with_options_async(request, runtime)
 
     def list_user_devices_with_options(
         self,
         request: csas_20230120_models.ListUserDevicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserDevicesResponse:
+        """
+        @summary 批量查询用户设备列表
+        
+        @param request: ListUserDevicesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserDevicesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserDevices',
@@ -3668,14 +4971,21 @@
         )
 
     async def list_user_devices_with_options_async(
         self,
         request: csas_20230120_models.ListUserDevicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserDevicesResponse:
+        """
+        @summary 批量查询用户设备列表
+        
+        @param request: ListUserDevicesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserDevicesResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserDevices',
@@ -3693,29 +5003,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_user_devices(
         self,
         request: csas_20230120_models.ListUserDevicesRequest,
     ) -> csas_20230120_models.ListUserDevicesResponse:
+        """
+        @summary 批量查询用户设备列表
+        
+        @param request: ListUserDevicesRequest
+        @return: ListUserDevicesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_user_devices_with_options(request, runtime)
 
     async def list_user_devices_async(
         self,
         request: csas_20230120_models.ListUserDevicesRequest,
     ) -> csas_20230120_models.ListUserDevicesResponse:
+        """
+        @summary 批量查询用户设备列表
+        
+        @param request: ListUserDevicesRequest
+        @return: ListUserDevicesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_devices_with_options_async(request, runtime)
 
     def list_user_groups_with_options(
         self,
         request: csas_20230120_models.ListUserGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsResponse:
+        """
+        @summary 批量查询用户组
+        
+        @param request: ListUserGroupsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserGroupsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroups',
@@ -3734,14 +5063,21 @@
         )
 
     async def list_user_groups_with_options_async(
         self,
         request: csas_20230120_models.ListUserGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsResponse:
+        """
+        @summary 批量查询用户组
+        
+        @param request: ListUserGroupsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserGroupsResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroups',
@@ -3759,29 +5095,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_user_groups(
         self,
         request: csas_20230120_models.ListUserGroupsRequest,
     ) -> csas_20230120_models.ListUserGroupsResponse:
+        """
+        @summary 批量查询用户组
+        
+        @param request: ListUserGroupsRequest
+        @return: ListUserGroupsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_user_groups_with_options(request, runtime)
 
     async def list_user_groups_async(
         self,
         request: csas_20230120_models.ListUserGroupsRequest,
     ) -> csas_20230120_models.ListUserGroupsResponse:
+        """
+        @summary 批量查询用户组
+        
+        @param request: ListUserGroupsRequest
+        @return: ListUserGroupsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_groups_with_options_async(request, runtime)
 
     def list_user_groups_for_private_access_policy_with_options(
         self,
         request: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的用户组
+        
+        @param request: ListUserGroupsForPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserGroupsForPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroupsForPrivateAccessPolicy',
@@ -3800,14 +5155,21 @@
         )
 
     async def list_user_groups_for_private_access_policy_with_options_async(
         self,
         request: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的用户组
+        
+        @param request: ListUserGroupsForPrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserGroupsForPrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroupsForPrivateAccessPolicy',
@@ -3825,29 +5187,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_user_groups_for_private_access_policy(
         self,
         request: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListUserGroupsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的用户组
+        
+        @param request: ListUserGroupsForPrivateAccessPolicyRequest
+        @return: ListUserGroupsForPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_user_groups_for_private_access_policy_with_options(request, runtime)
 
     async def list_user_groups_for_private_access_policy_async(
         self,
         request: csas_20230120_models.ListUserGroupsForPrivateAccessPolicyRequest,
     ) -> csas_20230120_models.ListUserGroupsForPrivateAccessPolicyResponse:
+        """
+        @summary 批量查询内网访问策略的用户组
+        
+        @param request: ListUserGroupsForPrivateAccessPolicyRequest
+        @return: ListUserGroupsForPrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_groups_for_private_access_policy_with_options_async(request, runtime)
 
     def list_user_groups_for_registration_policy_with_options(
         self,
         request: csas_20230120_models.ListUserGroupsForRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsForRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略相关用户组
+        
+        @param request: ListUserGroupsForRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserGroupsForRegistrationPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroupsForRegistrationPolicy',
@@ -3866,14 +5247,21 @@
         )
 
     async def list_user_groups_for_registration_policy_with_options_async(
         self,
         request: csas_20230120_models.ListUserGroupsForRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUserGroupsForRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略相关用户组
+        
+        @param request: ListUserGroupsForRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUserGroupsForRegistrationPolicyResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUserGroupsForRegistrationPolicy',
@@ -3891,29 +5279,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_user_groups_for_registration_policy(
         self,
         request: csas_20230120_models.ListUserGroupsForRegistrationPolicyRequest,
     ) -> csas_20230120_models.ListUserGroupsForRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略相关用户组
+        
+        @param request: ListUserGroupsForRegistrationPolicyRequest
+        @return: ListUserGroupsForRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_user_groups_for_registration_policy_with_options(request, runtime)
 
     async def list_user_groups_for_registration_policy_async(
         self,
         request: csas_20230120_models.ListUserGroupsForRegistrationPolicyRequest,
     ) -> csas_20230120_models.ListUserGroupsForRegistrationPolicyResponse:
+        """
+        @summary 查询设备注册策略相关用户组
+        
+        @param request: ListUserGroupsForRegistrationPolicyRequest
+        @return: ListUserGroupsForRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_user_groups_for_registration_policy_with_options_async(request, runtime)
 
     def list_users_with_options(
         self,
         request: csas_20230120_models.ListUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUsersResponse:
+        """
+        @summary 列表查询登陆用户
+        
+        @param request: ListUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUsersResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUsers',
@@ -3932,14 +5339,21 @@
         )
 
     async def list_users_with_options_async(
         self,
         request: csas_20230120_models.ListUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.ListUsersResponse:
+        """
+        @summary 列表查询登陆用户
+        
+        @param request: ListUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListUsersResponse
+        """
         UtilClient.validate_model(request)
         query = OpenApiUtilClient.query(UtilClient.to_map(request))
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListUsers',
@@ -3957,29 +5371,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_users(
         self,
         request: csas_20230120_models.ListUsersRequest,
     ) -> csas_20230120_models.ListUsersResponse:
+        """
+        @summary 列表查询登陆用户
+        
+        @param request: ListUsersRequest
+        @return: ListUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_users_with_options(request, runtime)
 
     async def list_users_async(
         self,
         request: csas_20230120_models.ListUsersRequest,
     ) -> csas_20230120_models.ListUsersResponse:
+        """
+        @summary 列表查询登陆用户
+        
+        @param request: ListUsersRequest
+        @return: ListUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_users_with_options_async(request, runtime)
 
     def update_client_user_with_options(
         self,
         request: csas_20230120_models.UpdateClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateClientUserResponse:
+        """
+        @summary 修改自定义身份源指定用户
+        
+        @param request: UpdateClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.email):
@@ -4008,14 +5441,21 @@
         )
 
     async def update_client_user_with_options_async(
         self,
         request: csas_20230120_models.UpdateClientUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateClientUserResponse:
+        """
+        @summary 修改自定义身份源指定用户
+        
+        @param request: UpdateClientUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateClientUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.description):
             query['Description'] = request.description
         if not UtilClient.is_unset(request.email):
@@ -4043,29 +5483,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_client_user(
         self,
         request: csas_20230120_models.UpdateClientUserRequest,
     ) -> csas_20230120_models.UpdateClientUserResponse:
+        """
+        @summary 修改自定义身份源指定用户
+        
+        @param request: UpdateClientUserRequest
+        @return: UpdateClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_client_user_with_options(request, runtime)
 
     async def update_client_user_async(
         self,
         request: csas_20230120_models.UpdateClientUserRequest,
     ) -> csas_20230120_models.UpdateClientUserResponse:
+        """
+        @summary 修改自定义身份源指定用户
+        
+        @param request: UpdateClientUserRequest
+        @return: UpdateClientUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_client_user_with_options_async(request, runtime)
 
     def update_client_user_password_with_options(
         self,
         request: csas_20230120_models.UpdateClientUserPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
+        """
+        @summary 修改自定义身份源指定用户密码
+        
+        @param request: UpdateClientUserPasswordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateClientUserPasswordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
         if not UtilClient.is_unset(request.username):
@@ -4090,14 +5549,21 @@
         )
 
     async def update_client_user_password_with_options_async(
         self,
         request: csas_20230120_models.UpdateClientUserPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
+        """
+        @summary 修改自定义身份源指定用户密码
+        
+        @param request: UpdateClientUserPasswordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateClientUserPasswordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.password):
             query['Password'] = request.password
         if not UtilClient.is_unset(request.username):
@@ -4121,29 +5587,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_client_user_password(
         self,
         request: csas_20230120_models.UpdateClientUserPasswordRequest,
     ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
+        """
+        @summary 修改自定义身份源指定用户密码
+        
+        @param request: UpdateClientUserPasswordRequest
+        @return: UpdateClientUserPasswordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_client_user_password_with_options(request, runtime)
 
     async def update_client_user_password_async(
         self,
         request: csas_20230120_models.UpdateClientUserPasswordRequest,
     ) -> csas_20230120_models.UpdateClientUserPasswordResponse:
+        """
+        @summary 修改自定义身份源指定用户密码
+        
+        @param request: UpdateClientUserPasswordRequest
+        @return: UpdateClientUserPasswordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_client_user_password_with_options_async(request, runtime)
 
     def update_client_user_status_with_options(
         self,
         request: csas_20230120_models.UpdateClientUserStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateClientUserStatusResponse:
+        """
+        @summary 修改自定义身份源指定用户启用状态
+        
+        @param request: UpdateClientUserStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateClientUserStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
@@ -4166,14 +5651,21 @@
         )
 
     async def update_client_user_status_with_options_async(
         self,
         request: csas_20230120_models.UpdateClientUserStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateClientUserStatusResponse:
+        """
+        @summary 修改自定义身份源指定用户启用状态
+        
+        @param request: UpdateClientUserStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateClientUserStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.id):
             query['Id'] = request.id
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
@@ -4195,29 +5687,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_client_user_status(
         self,
         request: csas_20230120_models.UpdateClientUserStatusRequest,
     ) -> csas_20230120_models.UpdateClientUserStatusResponse:
+        """
+        @summary 修改自定义身份源指定用户启用状态
+        
+        @param request: UpdateClientUserStatusRequest
+        @return: UpdateClientUserStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_client_user_status_with_options(request, runtime)
 
     async def update_client_user_status_async(
         self,
         request: csas_20230120_models.UpdateClientUserStatusRequest,
     ) -> csas_20230120_models.UpdateClientUserStatusResponse:
+        """
+        @summary 修改自定义身份源指定用户启用状态
+        
+        @param request: UpdateClientUserStatusRequest
+        @return: UpdateClientUserStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_client_user_status_with_options_async(request, runtime)
 
     def update_dynamic_route_with_options(
         self,
         request: csas_20230120_models.UpdateDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateDynamicRouteResponse:
+        """
+        @summary 修改动态路由
+        
+        @param request: UpdateDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -4263,14 +5774,21 @@
         )
 
     async def update_dynamic_route_with_options_async(
         self,
         request: csas_20230120_models.UpdateDynamicRouteRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateDynamicRouteResponse:
+        """
+        @summary 修改动态路由
+        
+        @param request: UpdateDynamicRouteRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateDynamicRouteResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -4315,29 +5833,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_dynamic_route(
         self,
         request: csas_20230120_models.UpdateDynamicRouteRequest,
     ) -> csas_20230120_models.UpdateDynamicRouteResponse:
+        """
+        @summary 修改动态路由
+        
+        @param request: UpdateDynamicRouteRequest
+        @return: UpdateDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_dynamic_route_with_options(request, runtime)
 
     async def update_dynamic_route_async(
         self,
         request: csas_20230120_models.UpdateDynamicRouteRequest,
     ) -> csas_20230120_models.UpdateDynamicRouteResponse:
+        """
+        @summary 修改动态路由
+        
+        @param request: UpdateDynamicRouteRequest
+        @return: UpdateDynamicRouteResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_dynamic_route_with_options_async(request, runtime)
 
     def update_excessive_device_registration_applications_status_with_options(
         self,
         request: csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusResponse:
+        """
+        @summary 批量更新超额注册申请状态
+        
+        @param request: UpdateExcessiveDeviceRegistrationApplicationsStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateExcessiveDeviceRegistrationApplicationsStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
@@ -4363,14 +5900,21 @@
         )
 
     async def update_excessive_device_registration_applications_status_with_options_async(
         self,
         request: csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusResponse:
+        """
+        @summary 批量更新超额注册申请状态
+        
+        @param request: UpdateExcessiveDeviceRegistrationApplicationsStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateExcessiveDeviceRegistrationApplicationsStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.status):
             body['Status'] = request.status
@@ -4395,29 +5939,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_excessive_device_registration_applications_status(
         self,
         request: csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusRequest,
     ) -> csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusResponse:
+        """
+        @summary 批量更新超额注册申请状态
+        
+        @param request: UpdateExcessiveDeviceRegistrationApplicationsStatusRequest
+        @return: UpdateExcessiveDeviceRegistrationApplicationsStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_excessive_device_registration_applications_status_with_options(request, runtime)
 
     async def update_excessive_device_registration_applications_status_async(
         self,
         request: csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusRequest,
     ) -> csas_20230120_models.UpdateExcessiveDeviceRegistrationApplicationsStatusResponse:
+        """
+        @summary 批量更新超额注册申请状态
+        
+        @param request: UpdateExcessiveDeviceRegistrationApplicationsStatusRequest
+        @return: UpdateExcessiveDeviceRegistrationApplicationsStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_excessive_device_registration_applications_status_with_options_async(request, runtime)
 
     def update_idp_department_with_options(
         self,
         request: csas_20230120_models.UpdateIdpDepartmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
+        """
+        @summary 修改指定自定义身份源部门
+        
+        @param request: UpdateIdpDepartmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateIdpDepartmentResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.department_name):
             query['DepartmentName'] = request.department_name
         if not UtilClient.is_unset(request.idp_config_id):
@@ -4442,14 +6005,21 @@
         )
 
     async def update_idp_department_with_options_async(
         self,
         request: csas_20230120_models.UpdateIdpDepartmentRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
+        """
+        @summary 修改指定自定义身份源部门
+        
+        @param request: UpdateIdpDepartmentRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateIdpDepartmentResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.department_id):
             query['DepartmentId'] = request.department_id
         if not UtilClient.is_unset(request.department_name):
             query['DepartmentName'] = request.department_name
         if not UtilClient.is_unset(request.idp_config_id):
@@ -4473,29 +6043,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_idp_department(
         self,
         request: csas_20230120_models.UpdateIdpDepartmentRequest,
     ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
+        """
+        @summary 修改指定自定义身份源部门
+        
+        @param request: UpdateIdpDepartmentRequest
+        @return: UpdateIdpDepartmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_idp_department_with_options(request, runtime)
 
     async def update_idp_department_async(
         self,
         request: csas_20230120_models.UpdateIdpDepartmentRequest,
     ) -> csas_20230120_models.UpdateIdpDepartmentResponse:
+        """
+        @summary 修改指定自定义身份源部门
+        
+        @param request: UpdateIdpDepartmentRequest
+        @return: UpdateIdpDepartmentResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_idp_department_with_options_async(request, runtime)
 
     def update_private_access_application_with_options(
         self,
         request: csas_20230120_models.UpdatePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdatePrivateAccessApplicationResponse:
+        """
+        @summary 修改内网访问应用
+        
+        @param request: UpdatePrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdatePrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.addresses):
             body_flat['Addresses'] = request.addresses
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
@@ -4533,14 +6122,21 @@
         )
 
     async def update_private_access_application_with_options_async(
         self,
         request: csas_20230120_models.UpdatePrivateAccessApplicationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdatePrivateAccessApplicationResponse:
+        """
+        @summary 修改内网访问应用
+        
+        @param request: UpdatePrivateAccessApplicationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdatePrivateAccessApplicationResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.addresses):
             body_flat['Addresses'] = request.addresses
         if not UtilClient.is_unset(request.application_id):
             body['ApplicationId'] = request.application_id
@@ -4577,29 +6173,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_private_access_application(
         self,
         request: csas_20230120_models.UpdatePrivateAccessApplicationRequest,
     ) -> csas_20230120_models.UpdatePrivateAccessApplicationResponse:
+        """
+        @summary 修改内网访问应用
+        
+        @param request: UpdatePrivateAccessApplicationRequest
+        @return: UpdatePrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_private_access_application_with_options(request, runtime)
 
     async def update_private_access_application_async(
         self,
         request: csas_20230120_models.UpdatePrivateAccessApplicationRequest,
     ) -> csas_20230120_models.UpdatePrivateAccessApplicationResponse:
+        """
+        @summary 修改内网访问应用
+        
+        @param request: UpdatePrivateAccessApplicationRequest
+        @return: UpdatePrivateAccessApplicationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_private_access_application_with_options_async(request, runtime)
 
     def update_private_access_policy_with_options(
         self,
         request: csas_20230120_models.UpdatePrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdatePrivateAccessPolicyResponse:
+        """
+        @summary 修改内网访问策略
+        
+        @param request: UpdatePrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdatePrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -4647,14 +6262,21 @@
         )
 
     async def update_private_access_policy_with_options_async(
         self,
         request: csas_20230120_models.UpdatePrivateAccessPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdatePrivateAccessPolicyResponse:
+        """
+        @summary 修改内网访问策略
+        
+        @param request: UpdatePrivateAccessPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdatePrivateAccessPolicyResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.application_ids):
             body_flat['ApplicationIds'] = request.application_ids
         if not UtilClient.is_unset(request.application_type):
             body['ApplicationType'] = request.application_type
@@ -4701,29 +6323,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_private_access_policy(
         self,
         request: csas_20230120_models.UpdatePrivateAccessPolicyRequest,
     ) -> csas_20230120_models.UpdatePrivateAccessPolicyResponse:
+        """
+        @summary 修改内网访问策略
+        
+        @param request: UpdatePrivateAccessPolicyRequest
+        @return: UpdatePrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_private_access_policy_with_options(request, runtime)
 
     async def update_private_access_policy_async(
         self,
         request: csas_20230120_models.UpdatePrivateAccessPolicyRequest,
     ) -> csas_20230120_models.UpdatePrivateAccessPolicyResponse:
+        """
+        @summary 修改内网访问策略
+        
+        @param request: UpdatePrivateAccessPolicyRequest
+        @return: UpdatePrivateAccessPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_private_access_policy_with_options_async(request, runtime)
 
     def update_registration_policy_with_options(
         self,
         tmp_req: csas_20230120_models.UpdateRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateRegistrationPolicyResponse:
+        """
+        @summary 修改设备注册策略
+        
+        @param tmp_req: UpdateRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRegistrationPolicyResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.UpdateRegistrationPolicyShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.company_limit_count):
             request.company_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.company_limit_count, 'CompanyLimitCount', 'json')
         if not UtilClient.is_unset(tmp_req.personal_limit_count):
             request.personal_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.personal_limit_count, 'PersonalLimitCount', 'json')
@@ -4775,14 +6416,21 @@
         )
 
     async def update_registration_policy_with_options_async(
         self,
         tmp_req: csas_20230120_models.UpdateRegistrationPolicyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateRegistrationPolicyResponse:
+        """
+        @summary 修改设备注册策略
+        
+        @param tmp_req: UpdateRegistrationPolicyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRegistrationPolicyResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = csas_20230120_models.UpdateRegistrationPolicyShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.company_limit_count):
             request.company_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.company_limit_count, 'CompanyLimitCount', 'json')
         if not UtilClient.is_unset(tmp_req.personal_limit_count):
             request.personal_limit_count_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.personal_limit_count, 'PersonalLimitCount', 'json')
@@ -4833,29 +6481,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_registration_policy(
         self,
         request: csas_20230120_models.UpdateRegistrationPolicyRequest,
     ) -> csas_20230120_models.UpdateRegistrationPolicyResponse:
+        """
+        @summary 修改设备注册策略
+        
+        @param request: UpdateRegistrationPolicyRequest
+        @return: UpdateRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_registration_policy_with_options(request, runtime)
 
     async def update_registration_policy_async(
         self,
         request: csas_20230120_models.UpdateRegistrationPolicyRequest,
     ) -> csas_20230120_models.UpdateRegistrationPolicyResponse:
+        """
+        @summary 修改设备注册策略
+        
+        @param request: UpdateRegistrationPolicyRequest
+        @return: UpdateRegistrationPolicyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_registration_policy_with_options_async(request, runtime)
 
     def update_user_devices_sharing_status_with_options(
         self,
         request: csas_20230120_models.UpdateUserDevicesSharingStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserDevicesSharingStatusResponse:
+        """
+        @summary 批量更新用户设备共享状态
+        
+        @param request: UpdateUserDevicesSharingStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserDevicesSharingStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.device_tags):
             body_flat['DeviceTags'] = request.device_tags
         if not UtilClient.is_unset(request.sharing_status):
             body['SharingStatus'] = request.sharing_status
@@ -4881,14 +6548,21 @@
         )
 
     async def update_user_devices_sharing_status_with_options_async(
         self,
         request: csas_20230120_models.UpdateUserDevicesSharingStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserDevicesSharingStatusResponse:
+        """
+        @summary 批量更新用户设备共享状态
+        
+        @param request: UpdateUserDevicesSharingStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserDevicesSharingStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.device_tags):
             body_flat['DeviceTags'] = request.device_tags
         if not UtilClient.is_unset(request.sharing_status):
             body['SharingStatus'] = request.sharing_status
@@ -4913,29 +6587,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_user_devices_sharing_status(
         self,
         request: csas_20230120_models.UpdateUserDevicesSharingStatusRequest,
     ) -> csas_20230120_models.UpdateUserDevicesSharingStatusResponse:
+        """
+        @summary 批量更新用户设备共享状态
+        
+        @param request: UpdateUserDevicesSharingStatusRequest
+        @return: UpdateUserDevicesSharingStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_user_devices_sharing_status_with_options(request, runtime)
 
     async def update_user_devices_sharing_status_async(
         self,
         request: csas_20230120_models.UpdateUserDevicesSharingStatusRequest,
     ) -> csas_20230120_models.UpdateUserDevicesSharingStatusResponse:
+        """
+        @summary 批量更新用户设备共享状态
+        
+        @param request: UpdateUserDevicesSharingStatusRequest
+        @return: UpdateUserDevicesSharingStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_devices_sharing_status_with_options_async(request, runtime)
 
     def update_user_devices_status_with_options(
         self,
         request: csas_20230120_models.UpdateUserDevicesStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserDevicesStatusResponse:
+        """
+        @summary 批量更新用户设备状态
+        
+        @param request: UpdateUserDevicesStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserDevicesStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.device_action):
             body['DeviceAction'] = request.device_action
         body_flat = {}
         if not UtilClient.is_unset(request.device_tags):
             body_flat['DeviceTags'] = request.device_tags
@@ -4961,14 +6654,21 @@
         )
 
     async def update_user_devices_status_with_options_async(
         self,
         request: csas_20230120_models.UpdateUserDevicesStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserDevicesStatusResponse:
+        """
+        @summary 批量更新用户设备状态
+        
+        @param request: UpdateUserDevicesStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserDevicesStatusResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.device_action):
             body['DeviceAction'] = request.device_action
         body_flat = {}
         if not UtilClient.is_unset(request.device_tags):
             body_flat['DeviceTags'] = request.device_tags
@@ -4993,29 +6693,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_user_devices_status(
         self,
         request: csas_20230120_models.UpdateUserDevicesStatusRequest,
     ) -> csas_20230120_models.UpdateUserDevicesStatusResponse:
+        """
+        @summary 批量更新用户设备状态
+        
+        @param request: UpdateUserDevicesStatusRequest
+        @return: UpdateUserDevicesStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_user_devices_status_with_options(request, runtime)
 
     async def update_user_devices_status_async(
         self,
         request: csas_20230120_models.UpdateUserDevicesStatusRequest,
     ) -> csas_20230120_models.UpdateUserDevicesStatusResponse:
+        """
+        @summary 批量更新用户设备状态
+        
+        @param request: UpdateUserDevicesStatusRequest
+        @return: UpdateUserDevicesStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_devices_status_with_options_async(request, runtime)
 
     def update_user_group_with_options(
         self,
         request: csas_20230120_models.UpdateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserGroupResponse:
+        """
+        @summary 修改用户组
+        
+        @param request: UpdateUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.attributes):
             body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
@@ -5045,14 +6764,21 @@
         )
 
     async def update_user_group_with_options_async(
         self,
         request: csas_20230120_models.UpdateUserGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUserGroupResponse:
+        """
+        @summary 修改用户组
+        
+        @param request: UpdateUserGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUserGroupResponse
+        """
         UtilClient.validate_model(request)
         body = {}
         body_flat = {}
         if not UtilClient.is_unset(request.attributes):
             body_flat['Attributes'] = request.attributes
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
@@ -5081,29 +6807,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_user_group(
         self,
         request: csas_20230120_models.UpdateUserGroupRequest,
     ) -> csas_20230120_models.UpdateUserGroupResponse:
+        """
+        @summary 修改用户组
+        
+        @param request: UpdateUserGroupRequest
+        @return: UpdateUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_user_group_with_options(request, runtime)
 
     async def update_user_group_async(
         self,
         request: csas_20230120_models.UpdateUserGroupRequest,
     ) -> csas_20230120_models.UpdateUserGroupResponse:
+        """
+        @summary 修改用户组
+        
+        @param request: UpdateUserGroupRequest
+        @return: UpdateUserGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_user_group_with_options_async(request, runtime)
 
     def update_users_status_with_options(
         self,
         request: csas_20230120_models.UpdateUsersStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        """
+        @summary 批量修改登陆用户状态
+        
+        @param request: UpdateUsersStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUsersStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.sase_user_ids):
             query['SaseUserIds'] = request.sase_user_ids
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
@@ -5126,14 +6871,21 @@
         )
 
     async def update_users_status_with_options_async(
         self,
         request: csas_20230120_models.UpdateUsersStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        """
+        @summary 批量修改登陆用户状态
+        
+        @param request: UpdateUsersStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateUsersStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.sase_user_ids):
             query['SaseUserIds'] = request.sase_user_ids
         if not UtilClient.is_unset(request.status):
             query['Status'] = request.status
         req = open_api_models.OpenApiRequest(
@@ -5155,16 +6907,28 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_users_status(
         self,
         request: csas_20230120_models.UpdateUsersStatusRequest,
     ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        """
+        @summary 批量修改登陆用户状态
+        
+        @param request: UpdateUsersStatusRequest
+        @return: UpdateUsersStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_users_status_with_options(request, runtime)
 
     async def update_users_status_async(
         self,
         request: csas_20230120_models.UpdateUsersStatusRequest,
     ) -> csas_20230120_models.UpdateUsersStatusResponse:
+        """
+        @summary 批量修改登陆用户状态
+        
+        @param request: UpdateUsersStatusRequest
+        @return: UpdateUsersStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_users_status_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120/models.py` & `alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 
 class AttachApplication2ConnectorRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
         connector_id: str = None,
     ):
+        # This parameter is required.
         self.application_ids = application_ids
         # ConnectorID。
+        # 
+        # This parameter is required.
         self.connector_id = connector_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40,16 +43,19 @@
 
 class AttachApplication2ConnectorShrinkRequest(TeaModel):
     def __init__(
         self,
         application_ids_shrink: str = None,
         connector_id: str = None,
     ):
+        # This parameter is required.
         self.application_ids_shrink = application_ids_shrink
         # ConnectorID。
+        # 
+        # This parameter is required.
         self.connector_id = connector_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -149,18 +155,21 @@
         idp_config_id: str = None,
         mobile_number: str = None,
         password: str = None,
         username: str = None,
     ):
         self.department_id = department_id
         self.description = description
+        # This parameter is required.
         self.email = email
+        # This parameter is required.
         self.idp_config_id = idp_config_id
         self.mobile_number = mobile_number
         self.password = password
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -288,21 +297,28 @@
         next_hop: str = None,
         priority: int = None,
         region_ids: List[str] = None,
         status: str = None,
         tag_ids: List[str] = None,
     ):
         self.application_ids = application_ids
+        # This parameter is required.
         self.application_type = application_type
         self.description = description
+        # This parameter is required.
         self.dynamic_route_type = dynamic_route_type
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.next_hop = next_hop
+        # This parameter is required.
         self.priority = priority
+        # This parameter is required.
         self.region_ids = region_ids
+        # This parameter is required.
         self.status = status
         self.tag_ids = tag_ids
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -434,15 +450,17 @@
 
 class CreateIdpDepartmentRequest(TeaModel):
     def __init__(
         self,
         department_name: str = None,
         idp_config_id: str = None,
     ):
+        # This parameter is required.
         self.department_name = department_name
+        # This parameter is required.
         self.idp_config_id = idp_config_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -541,15 +559,17 @@
 
 class CreatePrivateAccessApplicationRequestPortRanges(TeaModel):
     def __init__(
         self,
         begin: int = None,
         end: int = None,
     ):
+        # This parameter is required.
         self.begin = begin
+        # This parameter is required.
         self.end = end
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -579,19 +599,24 @@
         description: str = None,
         name: str = None,
         port_ranges: List[CreatePrivateAccessApplicationRequestPortRanges] = None,
         protocol: str = None,
         status: str = None,
         tag_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.addresses = addresses
         self.description = description
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.port_ranges = port_ranges
+        # This parameter is required.
         self.protocol = protocol
+        # This parameter is required.
         self.status = status
         self.tag_ids = tag_ids
 
     def validate(self):
         if self.port_ranges:
             for k in self.port_ranges:
                 if k:
@@ -775,28 +800,35 @@
         priority: int = None,
         status: str = None,
         tag_ids: List[str] = None,
         user_group_ids: List[str] = None,
         user_group_mode: str = None,
     ):
         self.application_ids = application_ids
+        # This parameter is required.
         self.application_type = application_type
         self.custom_user_attributes = custom_user_attributes
         self.description = description
         self.device_attribute_id = device_attribute_id
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.policy_action = policy_action
+        # This parameter is required.
         self.priority = priority
+        # This parameter is required.
         self.status = status
         # 内网访问标签ID集合。最多可输入100个内网访问标签ID。当**ApplicationType**为**Tag时**，必填。和**ApplicationIds**互斥。
         self.tag_ids = tag_ids
         self.user_group_ids = user_group_ids
         # 内网访问策略的用户组类型。取值：
         # - **Normal**：普通用户组。
         # - **Custom**：自定义用户组。
+        # 
+        # This parameter is required.
         self.user_group_mode = user_group_mode
 
     def validate(self):
         if self.custom_user_attributes:
             for k in self.custom_user_attributes:
                 if k:
                     k.validate()
@@ -944,14 +976,15 @@
 class CreatePrivateAccessTagRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         name: str = None,
     ):
         self.description = description
+        # This parameter is required.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1138,21 +1171,26 @@
         personal_limit_type: str = None,
         priority: int = None,
         status: str = None,
         user_group_ids: List[str] = None,
         whitelist: List[str] = None,
     ):
         self.company_limit_count = company_limit_count
+        # This parameter is required.
         self.company_limit_type = company_limit_type
         self.description = description
+        # This parameter is required.
         self.match_mode = match_mode
+        # This parameter is required.
         self.name = name
         self.personal_limit_count = personal_limit_count
+        # This parameter is required.
         self.personal_limit_type = personal_limit_type
         self.priority = priority
+        # This parameter is required.
         self.status = status
         self.user_group_ids = user_group_ids
         self.whitelist = whitelist
 
     def validate(self):
         if self.company_limit_count:
             self.company_limit_count.validate()
@@ -1230,21 +1268,26 @@
         personal_limit_type: str = None,
         priority: int = None,
         status: str = None,
         user_group_ids: List[str] = None,
         whitelist: List[str] = None,
     ):
         self.company_limit_count_shrink = company_limit_count_shrink
+        # This parameter is required.
         self.company_limit_type = company_limit_type
         self.description = description
+        # This parameter is required.
         self.match_mode = match_mode
+        # This parameter is required.
         self.name = name
         self.personal_limit_count_shrink = personal_limit_count_shrink
+        # This parameter is required.
         self.personal_limit_type = personal_limit_type
         self.priority = priority
+        # This parameter is required.
         self.status = status
         self.user_group_ids = user_group_ids
         self.whitelist = whitelist
 
     def validate(self):
         pass
 
@@ -1555,16 +1598,19 @@
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
     ):
         self.idp_id = idp_id
+        # This parameter is required.
         self.relation = relation
+        # This parameter is required.
         self.user_group_type = user_group_type
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1598,16 +1644,18 @@
 class CreateUserGroupRequest(TeaModel):
     def __init__(
         self,
         attributes: List[CreateUserGroupRequestAttributes] = None,
         description: str = None,
         name: str = None,
     ):
+        # This parameter is required.
         self.attributes = attributes
         self.description = description
+        # This parameter is required.
         self.name = name
 
     def validate(self):
         if self.attributes:
             for k in self.attributes:
                 if k:
                     k.validate()
@@ -1717,14 +1765,15 @@
 
 
 class DeleteClientUserRequest(TeaModel):
     def __init__(
         self,
         id: str = None,
     ):
+        # This parameter is required.
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1812,14 +1861,15 @@
 
 
 class DeleteDynamicRouteRequest(TeaModel):
     def __init__(
         self,
         dynamic_route_id: str = None,
     ):
+        # This parameter is required.
         self.dynamic_route_id = dynamic_route_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1908,15 +1958,17 @@
 
 class DeleteIdpDepartmentRequest(TeaModel):
     def __init__(
         self,
         department_id: str = None,
         idp_config_id: str = None,
     ):
+        # This parameter is required.
         self.department_id = department_id
+        # This parameter is required.
         self.idp_config_id = idp_config_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2008,14 +2060,15 @@
 
 
 class DeletePrivateAccessApplicationRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
     ):
+        # This parameter is required.
         self.application_id = application_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2103,14 +2156,15 @@
 
 
 class DeletePrivateAccessPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
     ):
+        # This parameter is required.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2198,14 +2252,15 @@
 
 
 class DeletePrivateAccessTagRequest(TeaModel):
     def __init__(
         self,
         tag_id: str = None,
     ):
+        # This parameter is required.
         self.tag_id = tag_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2293,14 +2348,15 @@
 
 
 class DeleteRegistrationPoliciesRequest(TeaModel):
     def __init__(
         self,
         policy_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.policy_ids = policy_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2388,14 +2444,15 @@
 
 
 class DeleteUserGroupRequest(TeaModel):
     def __init__(
         self,
         user_group_id: str = None,
     ):
+        # This parameter is required.
         self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2484,16 +2541,19 @@
 
 class DetachApplication2ConnectorRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
         connector_id: str = None,
     ):
+        # This parameter is required.
         self.application_ids = application_ids
         # ConnectorID。
+        # 
+        # This parameter is required.
         self.connector_id = connector_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2518,16 +2578,19 @@
 
 class DetachApplication2ConnectorShrinkRequest(TeaModel):
     def __init__(
         self,
         application_ids_shrink: str = None,
         connector_id: str = None,
     ):
+        # This parameter is required.
         self.application_ids_shrink = application_ids_shrink
         # ConnectorID。
+        # 
+        # This parameter is required.
         self.connector_id = connector_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2741,15 +2804,17 @@
 
 class GetClientUserRequest(TeaModel):
     def __init__(
         self,
         idp_config_id: str = None,
         username: str = None,
     ):
+        # This parameter is required.
         self.idp_config_id = idp_config_id
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2965,14 +3030,15 @@
 
 
 class GetDynamicRouteRequest(TeaModel):
     def __init__(
         self,
         dynamic_route_id: str = None,
     ):
+        # This parameter is required.
         self.dynamic_route_id = dynamic_route_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3161,14 +3227,15 @@
 
 
 class GetIdpConfigRequest(TeaModel):
     def __init__(
         self,
         id: str = None,
     ):
+        # This parameter is required.
         self.id = id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3395,14 +3462,15 @@
 
 
 class GetPrivateAccessApplicationRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
     ):
+        # This parameter is required.
         self.application_id = application_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3626,14 +3694,15 @@
 
 
 class GetPrivateAccessPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
     ):
+        # This parameter is required.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3887,14 +3956,15 @@
 
 
 class GetRegistrationPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_id: str = None,
     ):
+        # This parameter is required.
         self.policy_id = policy_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4130,14 +4200,15 @@
 
 
 class GetUserDeviceRequest(TeaModel):
     def __init__(
         self,
         device_tag: str = None,
     ):
+        # This parameter is required.
         self.device_tag = device_tag
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4451,14 +4522,15 @@
 
 
 class GetUserGroupRequest(TeaModel):
     def __init__(
         self,
         user_group_id: str = None,
     ):
+        # This parameter is required.
         self.user_group_id = user_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4658,14 +4730,15 @@
 
 
 class ListApplicationsForPrivateAccessPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.policy_ids = policy_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4918,14 +4991,15 @@
 
 
 class ListApplicationsForPrivateAccessTagRequest(TeaModel):
     def __init__(
         self,
         tag_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.tag_ids = tag_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5189,14 +5263,15 @@
         page_size: int = None,
         status: str = None,
         username: str = None,
     ):
         self.current_page = current_page
         self.department_id = department_id
         self.email = email
+        # This parameter is required.
         self.idp_config_id = idp_config_id
         self.mobile_number = mobile_number
         self.page_size = page_size
         self.status = status
         self.username = username
 
     def validate(self):
@@ -5487,16 +5562,18 @@
         current_page: int = None,
         name: str = None,
         page_size: int = None,
         status: str = None,
         switch_status: str = None,
     ):
         self.connector_ids = connector_ids
+        # This parameter is required.
         self.current_page = current_page
         self.name = name
+        # This parameter is required.
         self.page_size = page_size
         self.status = status
         self.switch_status = switch_status
 
     def validate(self):
         pass
 
@@ -5922,18 +5999,20 @@
         next_hop: str = None,
         page_size: int = None,
         region_ids: List[str] = None,
         status: str = None,
         tag_id: str = None,
     ):
         self.application_id = application_id
+        # This parameter is required.
         self.current_page = current_page
         self.dynamic_route_ids = dynamic_route_ids
         self.name = name
         self.next_hop = next_hop
+        # This parameter is required.
         self.page_size = page_size
         self.region_ids = region_ids
         self.status = status
         self.tag_id = tag_id
 
     def validate(self):
         pass
@@ -6179,19 +6258,21 @@
         mac: str = None,
         page_size: int = None,
         sase_user_id: str = None,
         statuses: List[str] = None,
         username: str = None,
     ):
         self.application_ids = application_ids
+        # This parameter is required.
         self.current_page = current_page
         self.department = department
         self.device_tag = device_tag
         self.hostname = hostname
         self.mac = mac
+        # This parameter is required.
         self.page_size = page_size
         self.sase_user_id = sase_user_id
         self.statuses = statuses
         self.username = username
 
     def validate(self):
         pass
@@ -6677,14 +6758,15 @@
     def __init__(
         self,
         current_page: int = None,
         idp_config_id: str = None,
         page_size: int = None,
     ):
         self.current_page = current_page
+        # This parameter is required.
         self.idp_config_id = idp_config_id
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6869,14 +6951,15 @@
 
 
 class ListPolicesForPrivateAccessApplicationRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.application_ids = application_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7153,14 +7236,15 @@
 
 
 class ListPolicesForPrivateAccessTagRequest(TeaModel):
     def __init__(
         self,
         tag_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.tag_ids = tag_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7453,14 +7537,15 @@
 
 
 class ListPolicesForUserGroupRequest(TeaModel):
     def __init__(
         self,
         user_group_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.user_group_ids = user_group_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7849,16 +7934,18 @@
         policy_id: str = None,
         status: str = None,
         tag_id: str = None,
     ):
         self.address = address
         self.application_ids = application_ids
         self.connector_id = connector_id
+        # This parameter is required.
         self.current_page = current_page
         self.name = name
+        # This parameter is required.
         self.page_size = page_size
         self.policy_id = policy_id
         self.status = status
         self.tag_id = tag_id
 
     def validate(self):
         pass
@@ -8129,14 +8216,15 @@
 
 
 class ListPrivateAccessApplicationsForDynamicRouteRequest(TeaModel):
     def __init__(
         self,
         dynamic_route_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.dynamic_route_ids = dynamic_route_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8401,16 +8489,18 @@
         status: str = None,
         tag_id: str = None,
         tag_name: str = None,
         user_group_id: str = None,
     ):
         self.application_id = application_id
         self.application_name = application_name
+        # This parameter is required.
         self.current_page = current_page
         self.name = name
+        # This parameter is required.
         self.page_size = page_size
         self.policy_action = policy_action
         self.policy_ids = policy_ids
         self.status = status
         self.tag_id = tag_id
         self.tag_name = tag_name
         # 用户组ID。取值来源：
@@ -8737,18 +8827,22 @@
     ):
         # The ID of the internal access application. You can obtain the application ID by calling the following operations:
         # 
         # *   [ListPrivateAccessApplications](~~ListPrivateAccessApplications~~): queries all internal access applications.
         # *   [CreatePrivateAccessApplication](~~CreatePrivateAccessApplication~~): creates an internal access application.
         self.application_id = application_id
         # The page number. Valid values: 1 to 10000.
+        # 
+        # This parameter is required.
         self.current_page = current_page
-        # The name of the internal access tag. The name must be 1 to 128 characters in length and can contain letters, digits, periods (.), underscores (\_), and hyphens (-).
+        # The name of the internal access tag. The name must be 1 to 128 characters in length and can contain letters, digits, periods (.), underscores (_), and hyphens (-).
         self.name = name
         # The number of entries per page. Valid values: 1 to 1000.
+        # 
+        # This parameter is required.
         self.page_size = page_size
         # The ID of the internal access policy. You can obtain the policy ID by calling the following operations:
         # 
         # *   [ListPrivateAccessPolices](~~ListPrivateAccessPolices~~): queries all internal access policies.
         # *   [CreatePrivateAccessPolicy](~~CreatePrivateAccessPolicy~~): creates an internal access policy.
         self.policy_id = policy_id
         # Specifies whether to enable the simple query mode. A value of true specifies that policy IDs are not queried.
@@ -8965,14 +9059,15 @@
 
 
 class ListPrivateAccessTagsForDynamicRouteRequest(TeaModel):
     def __init__(
         self,
         dynamic_route_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.dynamic_route_ids = dynamic_route_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9175,17 +9270,19 @@
         page_size: int = None,
         personal_limit_type: str = None,
         policy_ids: List[str] = None,
         status: str = None,
         user_group_id: str = None,
     ):
         self.company_limit_type = company_limit_type
+        # This parameter is required.
         self.current_page = current_page
         self.match_mode = match_mode
         self.name = name
+        # This parameter is required.
         self.page_size = page_size
         self.personal_limit_type = personal_limit_type
         self.policy_ids = policy_ids
         self.status = status
         self.user_group_id = user_group_id
 
     def validate(self):
@@ -9498,14 +9595,15 @@
 
 
 class ListRegistrationPoliciesForUserGroupRequest(TeaModel):
     def __init__(
         self,
         user_group_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.user_group_ids = user_group_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9813,16 +9911,19 @@
 class ListSoftwareForUserDeviceRequest(TeaModel):
     def __init__(
         self,
         current_page: int = None,
         device_tag: str = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.current_page = current_page
+        # This parameter is required.
         self.device_tag = device_tag
+        # This parameter is required.
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9983,14 +10084,15 @@
 
 
 class ListTagsForPrivateAccessApplicationRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.application_ids = application_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10184,14 +10286,15 @@
 
 
 class ListTagsForPrivateAccessPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.policy_ids = policy_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10394,36 +10497,40 @@
         device_belong: str = None,
         device_statuses: List[str] = None,
         device_tags: List[str] = None,
         device_types: List[str] = None,
         dlp_statuses: List[str] = None,
         hostname: str = None,
         ia_statuses: List[str] = None,
+        inner_ip: str = None,
         mac: str = None,
         nac_statuses: List[str] = None,
         pa_statuses: List[str] = None,
         page_size: int = None,
         sase_user_id: str = None,
         sharing_status: bool = None,
         sort_by: str = None,
         username: str = None,
     ):
         self.app_statuses = app_statuses
+        # This parameter is required.
         self.current_page = current_page
         self.department = department
         self.device_belong = device_belong
         self.device_statuses = device_statuses
         self.device_tags = device_tags
         self.device_types = device_types
         self.dlp_statuses = dlp_statuses
         self.hostname = hostname
         self.ia_statuses = ia_statuses
+        self.inner_ip = inner_ip
         self.mac = mac
         self.nac_statuses = nac_statuses
         self.pa_statuses = pa_statuses
+        # This parameter is required.
         self.page_size = page_size
         self.sase_user_id = sase_user_id
         self.sharing_status = sharing_status
         self.sort_by = sort_by
         self.username = username
 
     def validate(self):
@@ -10451,14 +10558,16 @@
             result['DeviceTypes'] = self.device_types
         if self.dlp_statuses is not None:
             result['DlpStatuses'] = self.dlp_statuses
         if self.hostname is not None:
             result['Hostname'] = self.hostname
         if self.ia_statuses is not None:
             result['IaStatuses'] = self.ia_statuses
+        if self.inner_ip is not None:
+            result['InnerIp'] = self.inner_ip
         if self.mac is not None:
             result['Mac'] = self.mac
         if self.nac_statuses is not None:
             result['NacStatuses'] = self.nac_statuses
         if self.pa_statuses is not None:
             result['PaStatuses'] = self.pa_statuses
         if self.page_size is not None:
@@ -10491,14 +10600,16 @@
             self.device_types = m.get('DeviceTypes')
         if m.get('DlpStatuses') is not None:
             self.dlp_statuses = m.get('DlpStatuses')
         if m.get('Hostname') is not None:
             self.hostname = m.get('Hostname')
         if m.get('IaStatuses') is not None:
             self.ia_statuses = m.get('IaStatuses')
+        if m.get('InnerIp') is not None:
+            self.inner_ip = m.get('InnerIp')
         if m.get('Mac') is not None:
             self.mac = m.get('Mac')
         if m.get('NacStatuses') is not None:
             self.nac_statuses = m.get('NacStatuses')
         if m.get('PaStatuses') is not None:
             self.pa_statuses = m.get('PaStatuses')
         if m.get('PageSize') is not None:
@@ -10780,18 +10891,20 @@
         current_page: int = None,
         name: str = None,
         papolicy_id: str = None,
         page_size: int = None,
         user_group_ids: List[str] = None,
     ):
         self.attribute_value = attribute_value
+        # This parameter is required.
         self.current_page = current_page
         # 用户组名称。长度为1~128个字符，支持中文和大小写英文字母，可包含数字、半角句号（.）、下划线（_）和短划线（-）。
         self.name = name
         self.papolicy_id = papolicy_id
+        # This parameter is required.
         self.page_size = page_size
         self.user_group_ids = user_group_ids
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -11024,14 +11137,15 @@
 
 
 class ListUserGroupsForPrivateAccessPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.policy_ids = policy_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11279,14 +11393,15 @@
 
 
 class ListUserGroupsForRegistrationPolicyRequest(TeaModel):
     def __init__(
         self,
         policy_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.policy_ids = policy_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11539,17 +11654,19 @@
         department: str = None,
         fuzzy_username: str = None,
         page_size: int = None,
         precise_username: str = None,
         sase_user_ids: List[str] = None,
         status: str = None,
     ):
+        # This parameter is required.
         self.current_page = current_page
         self.department = department
         self.fuzzy_username = fuzzy_username
+        # This parameter is required.
         self.page_size = page_size
         self.precise_username = precise_username
         self.sase_user_ids = sase_user_ids
         self.status = status
 
     def validate(self):
         pass
@@ -11754,14 +11871,15 @@
         email: str = None,
         id: str = None,
         mobile_number: str = None,
     ):
         self.department_id = department_id
         self.description = description
         self.email = email
+        # This parameter is required.
         self.id = id
         self.mobile_number = mobile_number
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -11974,15 +12092,17 @@
 
 class UpdateClientUserStatusRequest(TeaModel):
     def __init__(
         self,
         id: str = None,
         status: str = None,
     ):
+        # This parameter is required.
         self.id = id
+        # This parameter is required.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12088,14 +12208,15 @@
         region_ids: List[str] = None,
         status: str = None,
         tag_ids: List[str] = None,
     ):
         self.application_ids = application_ids
         self.application_type = application_type
         self.description = description
+        # This parameter is required.
         self.dynamic_route_id = dynamic_route_id
         self.dynamic_route_type = dynamic_route_type
         self.modify_type = modify_type
         self.name = name
         self.next_hop = next_hop
         self.priority = priority
         self.region_ids = region_ids
@@ -12236,15 +12357,17 @@
 
 class UpdateExcessiveDeviceRegistrationApplicationsStatusRequest(TeaModel):
     def __init__(
         self,
         application_ids: List[str] = None,
         status: str = None,
     ):
+        # This parameter is required.
         self.application_ids = application_ids
+        # This parameter is required.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12445,16 +12568,19 @@
 class UpdateIdpDepartmentRequest(TeaModel):
     def __init__(
         self,
         department_id: str = None,
         department_name: str = None,
         idp_config_id: str = None,
     ):
+        # This parameter is required.
         self.department_id = department_id
+        # This parameter is required.
         self.department_name = department_name
+        # This parameter is required.
         self.idp_config_id = idp_config_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12591,14 +12717,15 @@
         modify_type: str = None,
         port_ranges: List[UpdatePrivateAccessApplicationRequestPortRanges] = None,
         protocol: str = None,
         status: str = None,
         tag_ids: List[str] = None,
     ):
         self.addresses = addresses
+        # This parameter is required.
         self.application_id = application_id
         self.description = description
         self.modify_type = modify_type
         self.port_ranges = port_ranges
         self.protocol = protocol
         self.status = status
         self.tag_ids = tag_ids
@@ -12732,16 +12859,19 @@
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
     ):
         self.idp_id = idp_id
+        # This parameter is required.
         self.relation = relation
+        # This parameter is required.
         self.user_group_type = user_group_type
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12792,14 +12922,15 @@
         self.application_ids = application_ids
         self.application_type = application_type
         self.custom_user_attributes = custom_user_attributes
         self.description = description
         self.device_attribute_id = device_attribute_id
         self.modify_type = modify_type
         self.policy_action = policy_action
+        # This parameter is required.
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
         # 内网访问标签ID集合。一条策略最多支持100个内网访问标签ID。
         self.tag_ids = tag_ids
         self.user_group_ids = user_group_ids
         # 内网访问策略的用户组类型。取值：
@@ -13048,14 +13179,15 @@
         self.company_limit_count = company_limit_count
         self.company_limit_type = company_limit_type
         self.description = description
         self.match_mode = match_mode
         self.name = name
         self.personal_limit_count = personal_limit_count
         self.personal_limit_type = personal_limit_type
+        # This parameter is required.
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
         self.user_group_ids = user_group_ids
         self.whitelist = whitelist
 
     def validate(self):
@@ -13146,14 +13278,15 @@
         self.company_limit_count_shrink = company_limit_count_shrink
         self.company_limit_type = company_limit_type
         self.description = description
         self.match_mode = match_mode
         self.name = name
         self.personal_limit_count_shrink = personal_limit_count_shrink
         self.personal_limit_type = personal_limit_type
+        # This parameter is required.
         self.policy_id = policy_id
         self.priority = priority
         self.status = status
         self.user_group_ids = user_group_ids
         self.whitelist = whitelist
 
     def validate(self):
@@ -13467,15 +13600,17 @@
 
 class UpdateUserDevicesSharingStatusRequest(TeaModel):
     def __init__(
         self,
         device_tags: List[str] = None,
         sharing_status: bool = None,
     ):
+        # This parameter is required.
         self.device_tags = device_tags
+        # This parameter is required.
         self.sharing_status = sharing_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13753,15 +13888,17 @@
 
 class UpdateUserDevicesStatusRequest(TeaModel):
     def __init__(
         self,
         device_action: str = None,
         device_tags: List[str] = None,
     ):
+        # This parameter is required.
         self.device_action = device_action
+        # This parameter is required.
         self.device_tags = device_tags
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14042,16 +14179,19 @@
         self,
         idp_id: int = None,
         relation: str = None,
         user_group_type: str = None,
         value: str = None,
     ):
         self.idp_id = idp_id
+        # This parameter is required.
         self.relation = relation
+        # This parameter is required.
         self.user_group_type = user_group_type
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14089,14 +14229,15 @@
         description: str = None,
         modify_type: str = None,
         user_group_id: str = None,
     ):
         self.attributes = attributes
         self.description = description
         self.modify_type = modify_type
+        # This parameter is required.
         self.user_group_id = user_group_id
 
     def validate(self):
         if self.attributes:
             for k in self.attributes:
                 if k:
                     k.validate()
@@ -14205,15 +14346,17 @@
 
 class UpdateUsersStatusRequest(TeaModel):
     def __init__(
         self,
         sase_user_ids: List[str] = None,
         status: str = None,
     ):
+        # This parameter is required.
         self.sase_user_ids = sase_user_ids
+        # This parameter is required.
         self.status = status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_csas20230120-1.4.0/alibabacloud_csas20230120.egg-info/PKG-INFO` & `alibabacloud_csas20230120-1.4.1/alibabacloud_csas20230120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-csas20230120
-Version: 1.4.0
+Version: 1.4.1
 Summary: Alibaba Cloud csas (20230120) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_csas20230120-1.4.0/setup.py` & `alibabacloud_csas20230120-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_csas20230120.
 
-Created on 25/04/2024
+Created on 17/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_csas20230120"
 NAME = "alibabacloud_csas20230120" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud csas (20230120) SDK Library for Python"
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

