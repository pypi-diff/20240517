# Comparing `tmp/antchain_tax-1.8.6.tar.gz` & `tmp/antchain_tax-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_tax-1.8.6.tar", last modified: Thu Dec 21 07:48:30 2023, max compression
+gzip compressed data, was "dist/antchain_tax-1.8.8.tar", last modified: Thu Jan 18 08:59:52 2024, max compression
```

## Comparing `antchain_tax-1.8.6.tar` & `antchain_tax-1.8.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/
--rw-r--r--   0 root         (0) root         (0)      600 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2162 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/antchain_sdk_tax/
--rw-r--r--   0 root         (0) root         (0)       21 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/antchain_sdk_tax/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90084 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/antchain_sdk_tax/client.py
--rw-r--r--   0 root         (0) root         (0)   245665 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/antchain_sdk_tax/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/antchain_tax.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2162 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/antchain_tax.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/antchain_tax.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/antchain_tax.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/antchain_tax.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/antchain_tax.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-12-21 07:48:30.000000 antchain_tax-1.8.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2489 2023-12-21 07:48:29.000000 antchain_tax-1.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/antchain_sdk_tax/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/antchain_sdk_tax/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90084 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/antchain_sdk_tax/client.py
+-rw-r--r--   0 root         (0) root         (0)   245665 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/antchain_sdk_tax/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/antchain_tax.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2162 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/antchain_tax.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/antchain_tax.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/antchain_tax.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/antchain_tax.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/antchain_tax.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-01-18 08:59:52.000000 antchain_tax-1.8.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2489 2024-01-18 08:59:51.000000 antchain_tax-1.8.8/setup.py
```

### Comparing `antchain_tax-1.8.6/LICENSE` & `antchain_tax-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_tax-1.8.6/PKG-INFO` & `antchain_tax-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_tax
-Version: 1.8.6
+Version: 1.8.8
 Summary: Ant Chain TAX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_tax-1.8.6/README-CN.md` & `antchain_tax-1.8.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_tax-1.8.6/README.md` & `antchain_tax-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `antchain_tax-1.8.6/antchain_sdk_tax/client.py` & `antchain_tax-1.8.8/antchain_sdk_tax/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.6',
+                    'sdk_version': '1.8.8',
                     '_prod_code': 'TAX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.6',
+                    'sdk_version': '1.8.8',
                     '_prod_code': 'TAX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_tax-1.8.6/antchain_sdk_tax/models.py` & `antchain_tax-1.8.8/antchain_sdk_tax/models.py`

 * *Files identical despite different names*

### Comparing `antchain_tax-1.8.6/antchain_tax.egg-info/PKG-INFO` & `antchain_tax-1.8.8/antchain_tax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-tax
-Version: 1.8.6
+Version: 1.8.8
 Summary: Ant Chain TAX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_tax-1.8.6/setup.py` & `antchain_tax-1.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_tax.
 
-Created on 21/12/2023
+Created on 18/01/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_tax"
 NAME = "antchain_tax" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain TAX SDK Library for Python"
```

