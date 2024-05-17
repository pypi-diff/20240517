# Comparing `tmp/antchain_blockchain-1.28.2.tar.gz` & `tmp/antchain_blockchain-1.28.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_blockchain-1.28.2.tar", last modified: Sun Feb  4 06:17:38 2024, max compression
+gzip compressed data, was "dist/antchain_blockchain-1.28.20.tar", last modified: Fri May 17 08:51:41 2024, max compression
```

## Comparing `antchain_blockchain-1.28.2.tar` & `antchain_blockchain-1.28.20.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 06:17:38.000000 antchain_blockchain-1.28.2/
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2205 2024-02-04 06:17:38.000000 antchain_blockchain-1.28.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      825 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1011 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 06:17:38.000000 antchain_blockchain-1.28.2/antchain_blockchain.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2205 2024-02-04 06:17:37.000000 antchain_blockchain-1.28.2/antchain_blockchain.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      379 2024-02-04 06:17:37.000000 antchain_blockchain-1.28.2/antchain_blockchain.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 06:17:37.000000 antchain_blockchain-1.28.2/antchain_blockchain.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-02-04 06:17:37.000000 antchain_blockchain-1.28.2/antchain_blockchain.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2024-02-04 06:17:37.000000 antchain_blockchain-1.28.2/antchain_blockchain.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 06:17:38.000000 antchain_blockchain-1.28.2/antchain_sdk_blockchain/
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/antchain_sdk_blockchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1473511 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/antchain_sdk_blockchain/client.py
--rw-r--r--   0 root         (0) root         (0)  3030119 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/antchain_sdk_blockchain/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-04 06:17:38.000000 antchain_blockchain-1.28.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2524 2024-02-04 06:17:36.000000 antchain_blockchain-1.28.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      825 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/antchain_blockchain.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2206 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/antchain_blockchain.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/antchain_blockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/antchain_blockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/antchain_blockchain.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/antchain_blockchain.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/antchain_sdk_blockchain/
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/antchain_sdk_blockchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1485891 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/antchain_sdk_blockchain/client.py
+-rw-r--r--   0 root         (0) root         (0)  3052650 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/antchain_sdk_blockchain/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 08:51:41.000000 antchain_blockchain-1.28.20/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-05-17 08:51:40.000000 antchain_blockchain-1.28.20/setup.py
```

### Comparing `antchain_blockchain-1.28.2/LICENSE` & `antchain_blockchain-1.28.20/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_blockchain-1.28.2/PKG-INFO` & `antchain_blockchain-1.28.20/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_blockchain
-Version: 1.28.2
+Version: 1.28.20
 Summary: Ant Chain BLOCKCHAIN SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_blockchain-1.28.2/README-CN.md` & `antchain_blockchain-1.28.20/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_blockchain-1.28.2/README.md` & `antchain_blockchain-1.28.20/README.md`

 * *Files identical despite different names*

### Comparing `antchain_blockchain-1.28.2/antchain_blockchain.egg-info/PKG-INFO` & `antchain_blockchain-1.28.20/antchain_blockchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-blockchain
-Version: 1.28.2
+Version: 1.28.20
 Summary: Ant Chain BLOCKCHAIN SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_blockchain-1.28.2/antchain_sdk_blockchain/client.py` & `antchain_blockchain-1.28.20/antchain_sdk_blockchain/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.28.2',
+                    'sdk_version': '1.28.20',
                     '_prod_code': 'BLOCKCHAIN',
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
-                    'sdk_version': '1.28.2',
+                    'sdk_version': '1.28.20',
                     '_prod_code': 'BLOCKCHAIN',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -23283,14 +23283,294 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             blockchain_models.RepayAuthEquityResponse(),
             await self.do_request_async('1.0', 'baas.auth.equity.repay', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def verify_auth_token_validity(
+        self,
+        request: blockchain_models.VerifyAuthTokenValidityRequest,
+    ) -> blockchain_models.VerifyAuthTokenValidityResponse:
+        """
+        Description: 授权token校验
+        Summary: 授权token校验
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.verify_auth_token_validity_ex(request, headers, runtime)
+
+    async def verify_auth_token_validity_async(
+        self,
+        request: blockchain_models.VerifyAuthTokenValidityRequest,
+    ) -> blockchain_models.VerifyAuthTokenValidityResponse:
+        """
+        Description: 授权token校验
+        Summary: 授权token校验
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.verify_auth_token_validity_ex_async(request, headers, runtime)
+
+    def verify_auth_token_validity_ex(
+        self,
+        request: blockchain_models.VerifyAuthTokenValidityRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.VerifyAuthTokenValidityResponse:
+        """
+        Description: 授权token校验
+        Summary: 授权token校验
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.VerifyAuthTokenValidityResponse(),
+            self.do_request('1.0', 'baas.auth.token.validity.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def verify_auth_token_validity_ex_async(
+        self,
+        request: blockchain_models.VerifyAuthTokenValidityRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.VerifyAuthTokenValidityResponse:
+        """
+        Description: 授权token校验
+        Summary: 授权token校验
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.VerifyAuthTokenValidityResponse(),
+            await self.do_request_async('1.0', 'baas.auth.token.validity.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def verify_auth_business_user(
+        self,
+        request: blockchain_models.VerifyAuthBusinessUserRequest,
+    ) -> blockchain_models.VerifyAuthBusinessUserResponse:
+        """
+        Description: 核验当前用户是否权益新用户
+        Summary: 权益核验是否新用户
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.verify_auth_business_user_ex(request, headers, runtime)
+
+    async def verify_auth_business_user_async(
+        self,
+        request: blockchain_models.VerifyAuthBusinessUserRequest,
+    ) -> blockchain_models.VerifyAuthBusinessUserResponse:
+        """
+        Description: 核验当前用户是否权益新用户
+        Summary: 权益核验是否新用户
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.verify_auth_business_user_ex_async(request, headers, runtime)
+
+    def verify_auth_business_user_ex(
+        self,
+        request: blockchain_models.VerifyAuthBusinessUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.VerifyAuthBusinessUserResponse:
+        """
+        Description: 核验当前用户是否权益新用户
+        Summary: 权益核验是否新用户
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.VerifyAuthBusinessUserResponse(),
+            self.do_request('1.0', 'baas.auth.business.user.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def verify_auth_business_user_ex_async(
+        self,
+        request: blockchain_models.VerifyAuthBusinessUserRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.VerifyAuthBusinessUserResponse:
+        """
+        Description: 核验当前用户是否权益新用户
+        Summary: 权益核验是否新用户
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.VerifyAuthBusinessUserResponse(),
+            await self.do_request_async('1.0', 'baas.auth.business.user.verify', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def submit_auth_business_data(
+        self,
+        request: blockchain_models.SubmitAuthBusinessDataRequest,
+    ) -> blockchain_models.SubmitAuthBusinessDataResponse:
+        """
+        Description: 代运营场景下第三方应用调用该接口推送相关信息，例如车辆信息
+        Summary: 代运营-推送用户授权的相关信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_auth_business_data_ex(request, headers, runtime)
+
+    async def submit_auth_business_data_async(
+        self,
+        request: blockchain_models.SubmitAuthBusinessDataRequest,
+    ) -> blockchain_models.SubmitAuthBusinessDataResponse:
+        """
+        Description: 代运营场景下第三方应用调用该接口推送相关信息，例如车辆信息
+        Summary: 代运营-推送用户授权的相关信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_auth_business_data_ex_async(request, headers, runtime)
+
+    def submit_auth_business_data_ex(
+        self,
+        request: blockchain_models.SubmitAuthBusinessDataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.SubmitAuthBusinessDataResponse:
+        """
+        Description: 代运营场景下第三方应用调用该接口推送相关信息，例如车辆信息
+        Summary: 代运营-推送用户授权的相关信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.SubmitAuthBusinessDataResponse(),
+            self.do_request('1.0', 'baas.auth.business.data.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_auth_business_data_ex_async(
+        self,
+        request: blockchain_models.SubmitAuthBusinessDataRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.SubmitAuthBusinessDataResponse:
+        """
+        Description: 代运营场景下第三方应用调用该接口推送相关信息，例如车辆信息
+        Summary: 代运营-推送用户授权的相关信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.SubmitAuthBusinessDataResponse(),
+            await self.do_request_async('1.0', 'baas.auth.business.data.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def upload_auth_business_card(
+        self,
+        request: blockchain_models.UploadAuthBusinessCardRequest,
+    ) -> blockchain_models.UploadAuthBusinessCardResponse:
+        """
+        Description: 支持调用该接口上传行驶证照片，返回上传链接
+        Summary: 行驶证上传接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.upload_auth_business_card_ex(request, headers, runtime)
+
+    async def upload_auth_business_card_async(
+        self,
+        request: blockchain_models.UploadAuthBusinessCardRequest,
+    ) -> blockchain_models.UploadAuthBusinessCardResponse:
+        """
+        Description: 支持调用该接口上传行驶证照片，返回上传链接
+        Summary: 行驶证上传接口
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.upload_auth_business_card_ex_async(request, headers, runtime)
+
+    def upload_auth_business_card_ex(
+        self,
+        request: blockchain_models.UploadAuthBusinessCardRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.UploadAuthBusinessCardResponse:
+        """
+        Description: 支持调用该接口上传行驶证照片，返回上传链接
+        Summary: 行驶证上传接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.UploadAuthBusinessCardResponse(),
+            self.do_request('1.0', 'baas.auth.business.card.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def upload_auth_business_card_ex_async(
+        self,
+        request: blockchain_models.UploadAuthBusinessCardRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.UploadAuthBusinessCardResponse:
+        """
+        Description: 支持调用该接口上传行驶证照片，返回上传链接
+        Summary: 行驶证上传接口
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.UploadAuthBusinessCardResponse(),
+            await self.do_request_async('1.0', 'baas.auth.business.card.upload', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def query_auth_vc_transaction(
+        self,
+        request: blockchain_models.QueryAuthVcTransactionRequest,
+    ) -> blockchain_models.QueryAuthVcTransactionResponse:
+        """
+        Description: 通过指定可验证声明id，获取目标可验证声明链上交易信息，需要可验证声明的拥有者分享声明才可查询，如果没有权限则获取失败。
+        Summary: 获取目标可验证声明链上交易信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_auth_vc_transaction_ex(request, headers, runtime)
+
+    async def query_auth_vc_transaction_async(
+        self,
+        request: blockchain_models.QueryAuthVcTransactionRequest,
+    ) -> blockchain_models.QueryAuthVcTransactionResponse:
+        """
+        Description: 通过指定可验证声明id，获取目标可验证声明链上交易信息，需要可验证声明的拥有者分享声明才可查询，如果没有权限则获取失败。
+        Summary: 获取目标可验证声明链上交易信息
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_auth_vc_transaction_ex_async(request, headers, runtime)
+
+    def query_auth_vc_transaction_ex(
+        self,
+        request: blockchain_models.QueryAuthVcTransactionRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.QueryAuthVcTransactionResponse:
+        """
+        Description: 通过指定可验证声明id，获取目标可验证声明链上交易信息，需要可验证声明的拥有者分享声明才可查询，如果没有权限则获取失败。
+        Summary: 获取目标可验证声明链上交易信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.QueryAuthVcTransactionResponse(),
+            self.do_request('1.0', 'baas.auth.vc.transaction.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_auth_vc_transaction_ex_async(
+        self,
+        request: blockchain_models.QueryAuthVcTransactionRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> blockchain_models.QueryAuthVcTransactionResponse:
+        """
+        Description: 通过指定可验证声明id，获取目标可验证声明链上交易信息，需要可验证声明的拥有者分享声明才可查询，如果没有权限则获取失败。
+        Summary: 获取目标可验证声明链上交易信息
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            blockchain_models.QueryAuthVcTransactionResponse(),
+            await self.do_request_async('1.0', 'baas.auth.vc.transaction.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def start_did_corporate_agentcreate(
         self,
         request: blockchain_models.StartDidCorporateAgentcreateRequest,
     ) -> blockchain_models.StartDidCorporateAgentcreateResponse:
         """
         Description: 通过代理模式为企业创建did
         Summary: 通过代理模式为企业创建did
```

### Comparing `antchain_blockchain-1.28.2/antchain_sdk_blockchain/models.py` & `antchain_blockchain-1.28.20/antchain_sdk_blockchain/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6026,14 +6026,114 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_type') is not None:
             self.auth_type = m.get('auth_type')
         return self
 
 
+class TxInfo(TeaModel):
+    def __init__(
+        self,
+        tx_receipt_result: str = None,
+        biz_id: str = None,
+        tx_hash: str = None,
+        tx_type: str = None,
+        timestamp: int = None,
+        block_number: str = None,
+        nonce: str = None,
+        from_: str = None,
+        to: str = None,
+        signature: str = None,
+    ):
+        # 上链结果
+        self.tx_receipt_result = tx_receipt_result
+        # 区块链id
+        self.biz_id = biz_id
+        # 交易hash
+        self.tx_hash = tx_hash
+        # 交易类型
+        self.tx_type = tx_type
+        # 时间戳
+        self.timestamp = timestamp
+        # 区块高度
+        self.block_number = block_number
+        # 交易随机数Nonce
+        self.nonce = nonce
+        # 发起地址
+        self.from_ = from_
+        # 目标地址
+        self.to = to
+        # 签名
+        self.signature = signature
+
+    def validate(self):
+        self.validate_required(self.tx_receipt_result, 'tx_receipt_result')
+        self.validate_required(self.biz_id, 'biz_id')
+        self.validate_required(self.tx_hash, 'tx_hash')
+        self.validate_required(self.tx_type, 'tx_type')
+        self.validate_required(self.timestamp, 'timestamp')
+        self.validate_required(self.block_number, 'block_number')
+        self.validate_required(self.nonce, 'nonce')
+        self.validate_required(self.from_, 'from_')
+        self.validate_required(self.to, 'to')
+        self.validate_required(self.signature, 'signature')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.tx_receipt_result is not None:
+            result['tx_receipt_result'] = self.tx_receipt_result
+        if self.biz_id is not None:
+            result['biz_id'] = self.biz_id
+        if self.tx_hash is not None:
+            result['tx_hash'] = self.tx_hash
+        if self.tx_type is not None:
+            result['tx_type'] = self.tx_type
+        if self.timestamp is not None:
+            result['timestamp'] = self.timestamp
+        if self.block_number is not None:
+            result['block_number'] = self.block_number
+        if self.nonce is not None:
+            result['nonce'] = self.nonce
+        if self.from_ is not None:
+            result['from'] = self.from_
+        if self.to is not None:
+            result['to'] = self.to
+        if self.signature is not None:
+            result['signature'] = self.signature
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('tx_receipt_result') is not None:
+            self.tx_receipt_result = m.get('tx_receipt_result')
+        if m.get('biz_id') is not None:
+            self.biz_id = m.get('biz_id')
+        if m.get('tx_hash') is not None:
+            self.tx_hash = m.get('tx_hash')
+        if m.get('tx_type') is not None:
+            self.tx_type = m.get('tx_type')
+        if m.get('timestamp') is not None:
+            self.timestamp = m.get('timestamp')
+        if m.get('block_number') is not None:
+            self.block_number = m.get('block_number')
+        if m.get('nonce') is not None:
+            self.nonce = m.get('nonce')
+        if m.get('from') is not None:
+            self.from_ = m.get('from')
+        if m.get('to') is not None:
+            self.to = m.get('to')
+        if m.get('signature') is not None:
+            self.signature = m.get('signature')
+        return self
+
+
 class ServiceDiscoveryResult(TeaModel):
     def __init__(
         self,
         did: str = None,
         services: List[DidDocServicesInfo] = None,
     ):
         # 提供该服务能力的did
@@ -62887,14 +62987,562 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class VerifyAuthTokenValidityRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        user_id: str = None,
+        authorized_token: str = None,
+        data_type: str = None,
+        scene_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 用户ID
+        self.user_id = user_id
+        # 授权凭证
+        self.authorized_token = authorized_token
+        # 数据产品类型
+        self.data_type = data_type
+        # 授权场景码
+        self.scene_code = scene_code
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.authorized_token, 'authorized_token')
+        self.validate_required(self.data_type, 'data_type')
+        self.validate_required(self.scene_code, 'scene_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.authorized_token is not None:
+            result['authorized_token'] = self.authorized_token
+        if self.data_type is not None:
+            result['data_type'] = self.data_type
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('authorized_token') is not None:
+            self.authorized_token = m.get('authorized_token')
+        if m.get('data_type') is not None:
+            self.data_type = m.get('data_type')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        return self
+
+
+class VerifyAuthTokenValidityResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        verify_result: bool = None,
+        err_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 验证结果（ture表示通过，false表示不通过）
+        self.verify_result = verify_result
+        # 错误信息
+        self.err_msg = err_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.verify_result is not None:
+            result['verify_result'] = self.verify_result
+        if self.err_msg is not None:
+            result['err_msg'] = self.err_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('verify_result') is not None:
+            self.verify_result = m.get('verify_result')
+        if m.get('err_msg') is not None:
+            self.err_msg = m.get('err_msg')
+        return self
+
+
+class VerifyAuthBusinessUserRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        user_id: str = None,
+        scene_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 用户id
+        self.user_id = user_id
+        # 场景码
+        self.scene_code = scene_code
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.scene_code, 'scene_code')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        return self
+
+
+class VerifyAuthBusinessUserResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        record_type: str = None,
+        encrypt_biz_id: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 用户当前记录状态
+        self.record_type = record_type
+        # 加密后的用户授权记录id
+        self.encrypt_biz_id = encrypt_biz_id
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.record_type is not None:
+            result['record_type'] = self.record_type
+        if self.encrypt_biz_id is not None:
+            result['encrypt_biz_id'] = self.encrypt_biz_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('record_type') is not None:
+            self.record_type = m.get('record_type')
+        if m.get('encrypt_biz_id') is not None:
+            self.encrypt_biz_id = m.get('encrypt_biz_id')
+        return self
+
+
+class SubmitAuthBusinessDataRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        user_id: str = None,
+        scene_code: str = None,
+        push_data_content: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 用户id
+        self.user_id = user_id
+        # 场景码
+        self.scene_code = scene_code
+        # 推送的数据内容，json字符串形式
+        self.push_data_content = push_data_content
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.scene_code, 'scene_code')
+        self.validate_required(self.push_data_content, 'push_data_content')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        if self.push_data_content is not None:
+            result['push_data_content'] = self.push_data_content
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        if m.get('push_data_content') is not None:
+            self.push_data_content = m.get('push_data_content')
+        return self
+
+
+class SubmitAuthBusinessDataResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        push_success: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 推送是否成功
+        self.push_success = push_success
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.push_success is not None:
+            result['push_success'] = self.push_success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('push_success') is not None:
+            self.push_success = m.get('push_success')
+        return self
+
+
+class UploadAuthBusinessCardRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        user_id: str = None,
+        scene_code: str = None,
+        file_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 用户id
+        self.user_id = user_id
+        # 运营场景码
+        self.scene_code = scene_code
+        # 上传证件类型
+        self.file_type = file_type
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.scene_code, 'scene_code')
+        self.validate_required(self.file_type, 'file_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.scene_code is not None:
+            result['scene_code'] = self.scene_code
+        if self.file_type is not None:
+            result['file_type'] = self.file_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('scene_code') is not None:
+            self.scene_code = m.get('scene_code')
+        if m.get('file_type') is not None:
+            self.file_type = m.get('file_type')
+        return self
+
+
+class UploadAuthBusinessCardResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        presigned_url_policy: PresignedUrlPolicy = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # oss文件上传策略
+        self.presigned_url_policy = presigned_url_policy
+
+    def validate(self):
+        if self.presigned_url_policy:
+            self.presigned_url_policy.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.presigned_url_policy is not None:
+            result['presigned_url_policy'] = self.presigned_url_policy.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('presigned_url_policy') is not None:
+            temp_model = PresignedUrlPolicy()
+            self.presigned_url_policy = temp_model.from_map(m['presigned_url_policy'])
+        return self
+
+
+class QueryAuthVcTransactionRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        vc_id: str = None,
+        biz_type: str = None,
+        owner_did: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 查询目标可验证声明的ID
+        self.vc_id = vc_id
+        # 业务类型，通常需要与授权宝服务沟通确定，业务类型可能影响此接口内部实现逻辑，长度不超过32字符。
+        self.biz_type = biz_type
+        # 如果此字段为空，则默认使用当前请求租户在授权宝配置的did来进行查询(此did需授权有权限)，此外情况都需要指定目标vc_id的owner_did
+        # 
+        self.owner_did = owner_did
+
+    def validate(self):
+        self.validate_required(self.vc_id, 'vc_id')
+        self.validate_required(self.biz_type, 'biz_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.vc_id is not None:
+            result['vc_id'] = self.vc_id
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
+        if self.owner_did is not None:
+            result['owner_did'] = self.owner_did
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('vc_id') is not None:
+            self.vc_id = m.get('vc_id')
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        if m.get('owner_did') is not None:
+            self.owner_did = m.get('owner_did')
+        return self
+
+
+class QueryAuthVcTransactionResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        tx_info: TxInfo = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 链上交易信息
+        self.tx_info = tx_info
+
+    def validate(self):
+        if self.tx_info:
+            self.tx_info.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.tx_info is not None:
+            result['tx_info'] = self.tx_info.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('tx_info') is not None:
+            temp_model = TxInfo()
+            self.tx_info = temp_model.from_map(m['tx_info'])
+        return self
+
+
 class StartDidCorporateAgentcreateRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         biz_code: str = None,
         extension_info: str = None,
```

### Comparing `antchain_blockchain-1.28.2/setup.py` & `antchain_blockchain-1.28.20/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_blockchain.
 
-Created on 04/02/2024
+Created on 17/05/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_blockchain"
 NAME = "antchain_blockchain" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BLOCKCHAIN SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

