# Comparing `tmp/cdk-sops-secrets-1.8.1.tar.gz` & `tmp/cdk-sops-secrets-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-sops-secrets-1.8.1.tar", last modified: Thu May 16 14:09:28 2024, max compression
+gzip compressed data, was "cdk-sops-secrets-1.8.2.tar", last modified: Fri May 17 06:44:52 2024, max compression
```

## Comparing `cdk-sops-secrets-1.8.1.tar` & `cdk-sops-secrets-1.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:28.887076 cdk-sops-secrets-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-05-16 14:09:28.887076 cdk-sops-secrets-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:09:28.887076 cdk-sops-secrets-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:28.871075 cdk-sops-secrets-1.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:28.875076 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets/
--rw-r--r--   0 runner    (1001) docker     (127)    84982 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:28.875076 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  8966758 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.8.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:09:17.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:09:28.875076 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12662 2024-05-16 14:09:28.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-16 14:09:28.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:09:28.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 14:09:28.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 14:09:28.000000 cdk-sops-secrets-1.8.1/src/cdk_sops_secrets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:44:52.605512 cdk-sops-secrets-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-17 06:44:52.605512 cdk-sops-secrets-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11721 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:44:52.605512 cdk-sops-secrets-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:44:52.593512 cdk-sops-secrets-1.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:44:52.593512 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)    80660 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:44:52.593512 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  8975365 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets/_jsii/cdk-sops-secrets@1.8.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:44:39.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:44:52.593512 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-05-17 06:44:52.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-17 06:44:52.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:44:52.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 06:44:52.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 06:44:52.000000 cdk-sops-secrets-1.8.2/src/cdk_sops_secrets.egg-info/top_level.txt
```

### Comparing `cdk-sops-secrets-1.8.1/LICENSE` & `cdk-sops-secrets-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.8.1/PKG-INFO` & `cdk-sops-secrets-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.8.1
+Version: 1.8.2
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/dbsystel/cdk-sops-secrets/blob/main/img/banner-dl-small.png?raw=true">
 <p/>
```

### Comparing `cdk-sops-secrets-1.8.1/README.md` & `cdk-sops-secrets-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk-sops-secrets-1.8.1/setup.py` & `cdk-sops-secrets-1.8.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-sops-secrets",
-    "version": "1.8.1",
+    "version": "1.8.2",
     "description": "CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.",
     "license": "Apache-2.0",
     "url": "https://constructs.dev/packages/cdk-sops-secrets",
     "long_description_content_type": "text/markdown",
     "author": "Markus Siebert<markus.siebert@deutschebahn.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_sops_secrets",
         "cdk_sops_secrets._jsii"
     ],
     "package_data": {
         "cdk_sops_secrets._jsii": [
-            "cdk-sops-secrets@1.8.1.jsii.tgz"
+            "cdk-sops-secrets@1.8.2.jsii.tgz"
         ],
         "cdk_sops_secrets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
@@ -46,15 +46,15 @@
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `cdk-sops-secrets-1.8.1/src/cdk_sops_secrets/__init__.py` & `cdk-sops-secrets-1.8.2/src/cdk_sops_secrets/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -257,18 +257,15 @@
 
 @jsii.implements(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret)
 class SopsSecret(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-sops-secrets.SopsSecret",
 ):
-    '''(experimental) A drop in replacement for the normal Secret, that is populated with the encrypted content of the given sops file.
-
-    :stability: experimental
-    '''
+    '''A drop in replacement for the normal Secret, that is populated with the encrypted content of the given sops file.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         description: typing.Optional[builtins.str] = None,
@@ -294,27 +291,25 @@
         :param id: -
         :param description: An optional, human-friendly description of the secret. Default: - No description.
         :param encryption_key: The customer-managed encryption key to use for encrypting the secret value. Default: - A default KMS key for the account and region is used.
         :param generate_secret_string: Configuration for how to generate a secret value. Default: - 32 characters with upper-case letters, lower-case letters, punctuation and numbers (at least one from each category), per the default values of ``SecretStringGenerator``.
         :param removal_policy: Policy to apply when the secret is removed from this stack. Default: - Not set.
         :param replica_regions: A list of regions where to replicate this secret. Default: - Secret is not replicated
         :param secret_name: A name for the secret. Note that deleting secrets from SecretsManager does not happen immediately, but after a 7 to 30 days blackout period. During that period, it is not possible to create another secret that shares the same name. Default: - A name is generated by CloudFormation.
-        :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
-        :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
-        :param sops_age_key: (experimental) The age key that should be used for encryption.
-        :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
-        :param sops_file_path: (experimental) The filepath to the sops file.
-        :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
-        :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
-        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
-        :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
-
-        :stability: experimental
+        :param convert_to_json: Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
+        :param flatten: Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
+        :param sops_age_key: The age key that should be used for encryption.
+        :param sops_file_format: The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: The filepath to the sops file.
+        :param sops_kms_key: The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
+        :param sops_provider: The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param stringify_values: Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
+        :param upload_type: How should the secret be passed to the CustomResource? Default: INLINE
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__641b47276285e7c457eb639fea01f8b2e2f54dd58d3bc6f9e184404914516a11)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = SopsSecretProps(
             description=description,
@@ -343,22 +338,20 @@
         self,
         id: builtins.str,
         *,
         automatically_after: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         hosted_rotation: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.HostedRotation] = None,
         rotation_lambda: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IFunction] = None,
     ) -> _aws_cdk_aws_secretsmanager_ceddda9d.RotationSchedule:
-        '''(experimental) Adds a rotation schedule to the secret.
+        '''Adds a rotation schedule to the secret.
 
         :param id: -
         :param automatically_after: Specifies the number of days after the previous rotation before Secrets Manager triggers the next automatic rotation. Default: Duration.days(30)
         :param hosted_rotation: Hosted rotation. Default: - either ``rotationLambda`` or ``hostedRotation`` must be specified
         :param rotation_lambda: A Lambda function that can rotate the secret. Default: - either ``rotationLambda`` or ``hostedRotation`` must be specified
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__bd08508625195135b318d9657d717ca369ecceb1cc51cd6b3fa8c66c489c3dad)
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         options = _aws_cdk_aws_secretsmanager_ceddda9d.RotationScheduleOptions(
             automatically_after=automatically_after,
             hosted_rotation=hosted_rotation,
@@ -368,232 +361,192 @@
         return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.RotationSchedule, jsii.invoke(self, "addRotationSchedule", [id, options]))
 
     @jsii.member(jsii_name="addToResourcePolicy")
     def add_to_resource_policy(
         self,
         statement: _aws_cdk_aws_iam_ceddda9d.PolicyStatement,
     ) -> _aws_cdk_aws_iam_ceddda9d.AddToResourcePolicyResult:
-        '''(experimental) Adds a statement to the IAM resource policy associated with this secret.
+        '''Adds a statement to the IAM resource policy associated with this secret.
 
         If this secret was created in this stack, a resource policy will be
         automatically created upon the first call to ``addToResourcePolicy``. If
         the secret is imported, then this is a no-op.
 
         :param statement: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__54076b0a3bb41bb64b3bbd471f51ee813e6ce6437b4b2ee14f76246051614126)
             check_type(argname="argument statement", value=statement, expected_type=type_hints["statement"])
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.AddToResourcePolicyResult, jsii.invoke(self, "addToResourcePolicy", [statement]))
 
     @jsii.member(jsii_name="applyRemovalPolicy")
     def apply_removal_policy(self, policy: _aws_cdk_ceddda9d.RemovalPolicy) -> None:
-        '''(experimental) Apply the given removal policy to this resource.
+        '''Apply the given removal policy to this resource.
 
         The Removal Policy controls what happens to this resource when it stops
         being managed by CloudFormation, either because you've removed it from the
         CDK application or because you've made a change that requires the resource
         to be replaced.
 
         The resource can be deleted (``RemovalPolicy.DESTROY``), or left in your AWS
         account for data recovery and cleanup later (``RemovalPolicy.RETAIN``).
 
         :param policy: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__85d3b1469d7d365dc715e5fc30a5ca749e3a126bab5731a9cb3e3bd09de54905)
             check_type(argname="argument policy", value=policy, expected_type=type_hints["policy"])
         return typing.cast(None, jsii.invoke(self, "applyRemovalPolicy", [policy]))
 
     @jsii.member(jsii_name="attach")
     def attach(
         self,
         target: _aws_cdk_aws_secretsmanager_ceddda9d.ISecretAttachmentTarget,
     ) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
-        '''(experimental) Attach a target to this secret.
+        '''Attach a target to this secret.
 
         :param target: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7169bcc05cc9fef09daa2e6732c5c382897a8dace487c441a5df1ea46b3123fc)
             check_type(argname="argument target", value=target, expected_type=type_hints["target"])
         return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, jsii.invoke(self, "attach", [target]))
 
     @jsii.member(jsii_name="currentVersionId")
     def current_version_id(self) -> builtins.str:
-        '''(experimental) Returns the current versionId that was created via the SopsSync.
-
-        :stability: experimental
-        '''
+        '''Returns the current versionId that was created via the SopsSync.'''
         return typing.cast(builtins.str, jsii.invoke(self, "currentVersionId", []))
 
     @jsii.member(jsii_name="denyAccountRootDelete")
     def deny_account_root_delete(self) -> None:
-        '''(experimental) Denies the ``DeleteSecret`` action to all principals within the current account.
-
-        :stability: experimental
-        '''
+        '''Denies the ``DeleteSecret`` action to all principals within the current account.'''
         return typing.cast(None, jsii.invoke(self, "denyAccountRootDelete", []))
 
     @jsii.member(jsii_name="grantRead")
     def grant_read(
         self,
         grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
         version_stages: typing.Optional[typing.Sequence[builtins.str]] = None,
     ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
-        '''(experimental) Grants reading the secret value to some role.
+        '''Grants reading the secret value to some role.
 
         :param grantee: -
         :param version_stages: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b84d1e6becdb6cf951b358b8a8bc63f668e555a12d11b0028528af866931a1c8)
             check_type(argname="argument grantee", value=grantee, expected_type=type_hints["grantee"])
             check_type(argname="argument version_stages", value=version_stages, expected_type=type_hints["version_stages"])
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantRead", [grantee, version_stages]))
 
     @jsii.member(jsii_name="grantWrite")
     def grant_write(
         self,
         _grantee: _aws_cdk_aws_iam_ceddda9d.IGrantable,
     ) -> _aws_cdk_aws_iam_ceddda9d.Grant:
-        '''(experimental) Grants writing and updating the secret value to some role.
+        '''Grants writing and updating the secret value to some role.
 
         :param _grantee: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4fd3a17eb68d15973a8af9441eb6cd97ed5338dead66b7679f005db68637eb5f)
             check_type(argname="argument _grantee", value=_grantee, expected_type=type_hints["_grantee"])
         return typing.cast(_aws_cdk_aws_iam_ceddda9d.Grant, jsii.invoke(self, "grantWrite", [_grantee]))
 
     @jsii.member(jsii_name="secretValueFromJson")
     def secret_value_from_json(
         self,
         json_field: builtins.str,
     ) -> _aws_cdk_ceddda9d.SecretValue:
-        '''(experimental) Interpret the secret as a JSON object and return a field's value from it as a ``SecretValue``.
+        '''Interpret the secret as a JSON object and return a field's value from it as a ``SecretValue``.
 
         :param json_field: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d65919d041d660423e596dfdaa79882405d878d5eda9d3e1171335aa874544f9)
             check_type(argname="argument json_field", value=json_field, expected_type=type_hints["json_field"])
         return typing.cast(_aws_cdk_ceddda9d.SecretValue, jsii.invoke(self, "secretValueFromJson", [json_field]))
 
     @builtins.property
     @jsii.member(jsii_name="env")
     def env(self) -> _aws_cdk_ceddda9d.ResourceEnvironment:
-        '''(experimental) The environment this resource belongs to.
+        '''The environment this resource belongs to.
 
         For resources that are created and managed by the CDK
         (generally, those created by creating new class instances like Role, Bucket, etc.),
         this is always the same as the environment of the stack they belong to;
         however, for imported resources
         (those obtained from static methods like fromRoleArn, fromBucketName, etc.),
         that might be different than the stack they were imported into.
-
-        :stability: experimental
         '''
         return typing.cast(_aws_cdk_ceddda9d.ResourceEnvironment, jsii.get(self, "env"))
 
     @builtins.property
     @jsii.member(jsii_name="secretArn")
     def secret_arn(self) -> builtins.str:
-        '''(experimental) The ARN of the secret in AWS Secrets Manager.
+        '''The ARN of the secret in AWS Secrets Manager.
 
         Will return the full ARN if available, otherwise a partial arn.
         For secrets imported by the deprecated ``fromSecretName``, it will return the ``secretName``.
-
-        :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "secretArn"))
 
     @builtins.property
     @jsii.member(jsii_name="secretName")
     def secret_name(self) -> builtins.str:
-        '''(experimental) The name of the secret.
+        '''The name of the secret.
 
         For "owned" secrets, this will be the full resource name (secret name + suffix), unless the
         '@aws-cdk/aws-secretsmanager:parseOwnedSecretName' feature flag is set.
-
-        :stability: experimental
         '''
         return typing.cast(builtins.str, jsii.get(self, "secretName"))
 
     @builtins.property
     @jsii.member(jsii_name="secretValue")
     def secret_value(self) -> _aws_cdk_ceddda9d.SecretValue:
-        '''(experimental) Retrieve the value of the stored secret as a ``SecretValue``.
-
-        :stability: experimental
-        '''
+        '''Retrieve the value of the stored secret as a ``SecretValue``.'''
         return typing.cast(_aws_cdk_ceddda9d.SecretValue, jsii.get(self, "secretValue"))
 
     @builtins.property
     @jsii.member(jsii_name="stack")
     def stack(self) -> _aws_cdk_ceddda9d.Stack:
-        '''(experimental) The stack in which this resource is defined.
-
-        :stability: experimental
-        '''
+        '''The stack in which this resource is defined.'''
         return typing.cast(_aws_cdk_ceddda9d.Stack, jsii.get(self, "stack"))
 
     @builtins.property
     @jsii.member(jsii_name="sync")
     def sync(self) -> "SopsSync":
-        '''
-        :stability: experimental
-        '''
         return typing.cast("SopsSync", jsii.get(self, "sync"))
 
     @builtins.property
     @jsii.member(jsii_name="encryptionKey")
     def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
-        '''(experimental) The customer-managed encryption key that is used to encrypt this secret, if any.
+        '''The customer-managed encryption key that is used to encrypt this secret, if any.
 
         When not specified, the default
         KMS key for the account and region is being used.
-
-        :stability: experimental
         '''
         return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], jsii.get(self, "encryptionKey"))
 
     @builtins.property
     @jsii.member(jsii_name="secretFullArn")
     def secret_full_arn(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The full ARN of the secret in AWS Secrets Manager, which is the ARN including the Secrets Manager-supplied 6-character suffix.
+        '''The full ARN of the secret in AWS Secrets Manager, which is the ARN including the Secrets Manager-supplied 6-character suffix.
 
         This is equal to ``secretArn`` in most cases, but is undefined when a full ARN is not available (e.g., secrets imported by name).
-
-        :stability: experimental
         '''
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "secretFullArn"))
 
 
 class SopsSync(
     _constructs_77d1e7e8.Construct,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-sops-secrets.SopsSync",
 ):
-    '''(experimental) The custom resource, that is syncing the content from a sops file to a secret.
-
-    :stability: experimental
-    '''
+    '''The custom resource, that is syncing the content from a sops file to a secret.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
@@ -608,28 +561,26 @@
         sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional["UploadType"] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
-        :param secret: (experimental) The secret that will be populated with the encrypted sops file content.
-        :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
-        :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
-        :param sops_age_key: (experimental) The age key that should be used for encryption.
-        :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
-        :param sops_file_path: (experimental) The filepath to the sops file.
-        :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
-        :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
-        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
-        :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
-
-        :stability: experimental
+        :param secret: The secret that will be populated with the encrypted sops file content.
+        :param convert_to_json: Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
+        :param flatten: Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
+        :param sops_age_key: The age key that should be used for encryption.
+        :param sops_file_format: The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: The filepath to the sops file.
+        :param sops_kms_key: The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
+        :param sops_provider: The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param stringify_values: Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
+        :param upload_type: How should the secret be passed to the CustomResource? Default: INLINE
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6b3134de7215a676a4feb3291975d227477d2dc9d5914405b8ab165ac30d7bad)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = SopsSyncProps(
             secret=secret,
@@ -647,45 +598,33 @@
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @builtins.property
     @jsii.member(jsii_name="converToJSON")
     def conver_to_json(self) -> builtins.bool:
-        '''(experimental) Was the format converted to json?
-
-        :stability: experimental
-        '''
+        '''Was the format converted to json?'''
         return typing.cast(builtins.bool, jsii.get(self, "converToJSON"))
 
     @builtins.property
     @jsii.member(jsii_name="flatten")
     def flatten(self) -> builtins.bool:
-        '''(experimental) Was the structure flattened?
-
-        :stability: experimental
-        '''
+        '''Was the structure flattened?'''
         return typing.cast(builtins.bool, jsii.get(self, "flatten"))
 
     @builtins.property
     @jsii.member(jsii_name="stringifiedValues")
     def stringified_values(self) -> builtins.bool:
-        '''(experimental) Were the values stringified?
-
-        :stability: experimental
-        '''
+        '''Were the values stringified?'''
         return typing.cast(builtins.bool, jsii.get(self, "stringifiedValues"))
 
     @builtins.property
     @jsii.member(jsii_name="versionId")
     def version_id(self) -> builtins.str:
-        '''(experimental) The current versionId of the secret populated via this resource.
-
-        :stability: experimental
-        '''
+        '''The current versionId of the secret populated via this resource.'''
         return typing.cast(builtins.str, jsii.get(self, "versionId"))
 
 
 @jsii.data_type(
     jsii_type="cdk-sops-secrets.SopsSyncOptions",
     jsii_struct_bases=[],
     name_mapping={
@@ -714,29 +653,27 @@
         sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
         sops_provider: typing.Optional["SopsSyncProvider"] = None,
         sops_s3_bucket: typing.Optional[builtins.str] = None,
         sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional["UploadType"] = None,
     ) -> None:
-        '''(experimental) Configuration options for the SopsSync.
+        '''Configuration options for the SopsSync.
 
-        :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
-        :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
-        :param sops_age_key: (experimental) The age key that should be used for encryption.
-        :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
-        :param sops_file_path: (experimental) The filepath to the sops file.
-        :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
-        :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
-        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
-        :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
-
-        :stability: experimental
+        :param convert_to_json: Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
+        :param flatten: Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
+        :param sops_age_key: The age key that should be used for encryption.
+        :param sops_file_format: The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: The filepath to the sops file.
+        :param sops_kms_key: The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
+        :param sops_provider: The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param stringify_values: Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
+        :param upload_type: How should the secret be passed to the CustomResource? Default: INLINE
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c2e7f5d5a68ee1675b645864f7bab39e30d7c7922956c69686578f4d6fb05723)
             check_type(argname="argument convert_to_json", value=convert_to_json, expected_type=type_hints["convert_to_json"])
             check_type(argname="argument flatten", value=flatten, expected_type=type_hints["flatten"])
             check_type(argname="argument sops_age_key", value=sops_age_key, expected_type=type_hints["sops_age_key"])
             check_type(argname="argument sops_file_format", value=sops_file_format, expected_type=type_hints["sops_file_format"])
@@ -769,136 +706,110 @@
         if stringify_values is not None:
             self._values["stringify_values"] = stringify_values
         if upload_type is not None:
             self._values["upload_type"] = upload_type
 
     @builtins.property
     def convert_to_json(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the encrypted sops value should be converted to JSON?
+        '''Should the encrypted sops value should be converted to JSON?
 
         Only JSON can be handled by cloud formations dynamic references.
 
         :default: true
-
-        :stability: experimental
         '''
         result = self._values.get("convert_to_json")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def flatten(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the structure be flattened?
+        '''Should the structure be flattened?
 
         The result will be a flat structure and all
         object keys will be replaced with the full jsonpath as key.
         This is usefull for dynamic references, as those don't support nested objects.
 
         :default: true
-
-        :stability: experimental
         '''
         result = self._values.get("flatten")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def sops_age_key(self) -> typing.Optional[_aws_cdk_ceddda9d.SecretValue]:
-        '''(experimental) The age key that should be used for encryption.
-
-        :stability: experimental
-        '''
+        '''The age key that should be used for encryption.'''
         result = self._values.get("sops_age_key")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.SecretValue], result)
 
     @builtins.property
     def sops_file_format(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The format of the sops file.
+        '''The format of the sops file.
 
         :default: - The fileformat will be derived from the file ending
-
-        :stability: experimental
         '''
         result = self._values.get("sops_file_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_file_path(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The filepath to the sops file.
-
-        :stability: experimental
-        '''
+        '''The filepath to the sops file.'''
         result = self._values.get("sops_file_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_kms_key(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]]:
-        '''(experimental) The kmsKey used to encrypt the sops file.
+        '''The kmsKey used to encrypt the sops file.
 
         Encrypt permissions
         will be granted to the custom resource provider.
 
         :default: - The key will be derived from the sops file
-
-        :stability: experimental
         '''
         result = self._values.get("sops_kms_key")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]], result)
 
     @builtins.property
     def sops_provider(self) -> typing.Optional["SopsSyncProvider"]:
-        '''(experimental) The custom resource provider to use.
+        '''The custom resource provider to use.
 
         If you don't specify any, a new
         provider will be created - or if already exists within this stack - reused.
 
         :default: - A new singleton provider will be created
-
-        :stability: experimental
         '''
         result = self._values.get("sops_provider")
         return typing.cast(typing.Optional["SopsSyncProvider"], result)
 
     @builtins.property
     def sops_s3_bucket(self) -> typing.Optional[builtins.str]:
-        '''(experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-
-        :stability: experimental
-        '''
+        '''If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.'''
         result = self._values.get("sops_s3_bucket")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_s3_key(self) -> typing.Optional[builtins.str]:
-        '''(experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-
-        :stability: experimental
-        '''
+        '''If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.'''
         result = self._values.get("sops_s3_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def stringify_values(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Shall all values be flattened?
+        '''Shall all values be flattened?
 
         This is usefull for dynamic references, as there
         are lookup errors for certain float types
-
-        :stability: experimental
         '''
         result = self._values.get("stringify_values")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def upload_type(self) -> typing.Optional["UploadType"]:
-        '''(experimental) How should the secret be passed to the CustomResource?
+        '''How should the secret be passed to the CustomResource?
 
         :default: INLINE
-
-        :stability: experimental
         '''
         result = self._values.get("upload_type")
         return typing.cast(typing.Optional["UploadType"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -942,30 +853,28 @@
         sops_provider: typing.Optional["SopsSyncProvider"] = None,
         sops_s3_bucket: typing.Optional[builtins.str] = None,
         sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional["UploadType"] = None,
         secret: _aws_cdk_aws_secretsmanager_ceddda9d.ISecret,
     ) -> None:
-        '''(experimental) The configuration options extended by the target Secret.
-
-        :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
-        :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
-        :param sops_age_key: (experimental) The age key that should be used for encryption.
-        :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
-        :param sops_file_path: (experimental) The filepath to the sops file.
-        :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
-        :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
-        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
-        :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
-        :param secret: (experimental) The secret that will be populated with the encrypted sops file content.
+        '''The configuration options extended by the target Secret.
 
-        :stability: experimental
+        :param convert_to_json: Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
+        :param flatten: Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
+        :param sops_age_key: The age key that should be used for encryption.
+        :param sops_file_format: The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: The filepath to the sops file.
+        :param sops_kms_key: The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
+        :param sops_provider: The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param stringify_values: Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
+        :param upload_type: How should the secret be passed to the CustomResource? Default: INLINE
+        :param secret: The secret that will be populated with the encrypted sops file content.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3baaf21b8ae44e7f4d83d5677857cc4141222b3d41237073b75dca6d425c2c34)
             check_type(argname="argument convert_to_json", value=convert_to_json, expected_type=type_hints["convert_to_json"])
             check_type(argname="argument flatten", value=flatten, expected_type=type_hints["flatten"])
             check_type(argname="argument sops_age_key", value=sops_age_key, expected_type=type_hints["sops_age_key"])
             check_type(argname="argument sops_file_format", value=sops_file_format, expected_type=type_hints["sops_file_format"])
@@ -1001,146 +910,117 @@
         if stringify_values is not None:
             self._values["stringify_values"] = stringify_values
         if upload_type is not None:
             self._values["upload_type"] = upload_type
 
     @builtins.property
     def convert_to_json(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the encrypted sops value should be converted to JSON?
+        '''Should the encrypted sops value should be converted to JSON?
 
         Only JSON can be handled by cloud formations dynamic references.
 
         :default: true
-
-        :stability: experimental
         '''
         result = self._values.get("convert_to_json")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def flatten(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the structure be flattened?
+        '''Should the structure be flattened?
 
         The result will be a flat structure and all
         object keys will be replaced with the full jsonpath as key.
         This is usefull for dynamic references, as those don't support nested objects.
 
         :default: true
-
-        :stability: experimental
         '''
         result = self._values.get("flatten")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def sops_age_key(self) -> typing.Optional[_aws_cdk_ceddda9d.SecretValue]:
-        '''(experimental) The age key that should be used for encryption.
-
-        :stability: experimental
-        '''
+        '''The age key that should be used for encryption.'''
         result = self._values.get("sops_age_key")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.SecretValue], result)
 
     @builtins.property
     def sops_file_format(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The format of the sops file.
+        '''The format of the sops file.
 
         :default: - The fileformat will be derived from the file ending
-
-        :stability: experimental
         '''
         result = self._values.get("sops_file_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_file_path(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The filepath to the sops file.
-
-        :stability: experimental
-        '''
+        '''The filepath to the sops file.'''
         result = self._values.get("sops_file_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_kms_key(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]]:
-        '''(experimental) The kmsKey used to encrypt the sops file.
+        '''The kmsKey used to encrypt the sops file.
 
         Encrypt permissions
         will be granted to the custom resource provider.
 
         :default: - The key will be derived from the sops file
-
-        :stability: experimental
         '''
         result = self._values.get("sops_kms_key")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]], result)
 
     @builtins.property
     def sops_provider(self) -> typing.Optional["SopsSyncProvider"]:
-        '''(experimental) The custom resource provider to use.
+        '''The custom resource provider to use.
 
         If you don't specify any, a new
         provider will be created - or if already exists within this stack - reused.
 
         :default: - A new singleton provider will be created
-
-        :stability: experimental
         '''
         result = self._values.get("sops_provider")
         return typing.cast(typing.Optional["SopsSyncProvider"], result)
 
     @builtins.property
     def sops_s3_bucket(self) -> typing.Optional[builtins.str]:
-        '''(experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-
-        :stability: experimental
-        '''
+        '''If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.'''
         result = self._values.get("sops_s3_bucket")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_s3_key(self) -> typing.Optional[builtins.str]:
-        '''(experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-
-        :stability: experimental
-        '''
+        '''If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.'''
         result = self._values.get("sops_s3_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def stringify_values(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Shall all values be flattened?
+        '''Shall all values be flattened?
 
         This is usefull for dynamic references, as there
         are lookup errors for certain float types
-
-        :stability: experimental
         '''
         result = self._values.get("stringify_values")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def upload_type(self) -> typing.Optional["UploadType"]:
-        '''(experimental) How should the secret be passed to the CustomResource?
+        '''How should the secret be passed to the CustomResource?
 
         :default: INLINE
-
-        :stability: experimental
         '''
         result = self._values.get("upload_type")
         return typing.cast(typing.Optional["UploadType"], result)
 
     @builtins.property
     def secret(self) -> _aws_cdk_aws_secretsmanager_ceddda9d.ISecret:
-        '''(experimental) The secret that will be populated with the encrypted sops file content.
-
-        :stability: experimental
-        '''
+        '''The secret that will be populated with the encrypted sops file content.'''
         result = self._values.get("secret")
         assert result is not None, "Required property 'secret' is missing"
         return typing.cast(_aws_cdk_aws_secretsmanager_ceddda9d.ISecret, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1155,64 +1035,46 @@
 
 @jsii.implements(_aws_cdk_aws_iam_ceddda9d.IGrantable)
 class SopsSyncProvider(
     _aws_cdk_aws_lambda_ceddda9d.SingletonFunction,
     metaclass=jsii.JSIIMeta,
     jsii_type="cdk-sops-secrets.SopsSyncProvider",
 ):
-    '''
-    :stability: experimental
-    '''
-
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6d2ccd4bddb65030756f5b6473575c1a4cc9c9ef0202c6dbe31603b006c05734)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         jsii.create(self.__class__, self, [scope, id])
 
     @jsii.member(jsii_name="addAgeKey")
     def add_age_key(self, key: _aws_cdk_ceddda9d.SecretValue) -> None:
         '''
         :param key: -
-
-        :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8f2a1da09ecfa1b4ae9738b2c30c913950581a07762445e7b2bb6fc32606a17d)
             check_type(argname="argument key", value=key, expected_type=type_hints["key"])
         return typing.cast(None, jsii.invoke(self, "addAgeKey", [key]))
 
 
 @jsii.enum(jsii_type="cdk-sops-secrets.UploadType")
 class UploadType(enum.Enum):
-    '''
-    :stability: experimental
-    '''
-
     INLINE = "INLINE"
-    '''(experimental) Pass the secret data inline (base64 encoded and compressed).
-
-    :stability: experimental
-    '''
+    '''Pass the secret data inline (base64 encoded and compressed).'''
     ASSET = "ASSET"
-    '''(experimental) Uplaod the secert data as asset.
-
-    :stability: experimental
-    '''
+    '''Uplaod the secert data as asset.'''
 
 
 @jsii.data_type(
     jsii_type="cdk-sops-secrets.SopsSecretProps",
     jsii_struct_bases=[
         _aws_cdk_aws_secretsmanager_ceddda9d.SecretProps, SopsSyncOptions
     ],
@@ -1257,35 +1119,33 @@
         sops_kms_key: typing.Optional[typing.Sequence[_aws_cdk_aws_kms_ceddda9d.IKey]] = None,
         sops_provider: typing.Optional[SopsSyncProvider] = None,
         sops_s3_bucket: typing.Optional[builtins.str] = None,
         sops_s3_key: typing.Optional[builtins.str] = None,
         stringify_values: typing.Optional[builtins.bool] = None,
         upload_type: typing.Optional[UploadType] = None,
     ) -> None:
-        '''(experimental) The configuration options of the SopsSecret.
+        '''The configuration options of the SopsSecret.
 
         :param description: An optional, human-friendly description of the secret. Default: - No description.
         :param encryption_key: The customer-managed encryption key to use for encrypting the secret value. Default: - A default KMS key for the account and region is used.
         :param generate_secret_string: Configuration for how to generate a secret value. Default: - 32 characters with upper-case letters, lower-case letters, punctuation and numbers (at least one from each category), per the default values of ``SecretStringGenerator``.
         :param removal_policy: Policy to apply when the secret is removed from this stack. Default: - Not set.
         :param replica_regions: A list of regions where to replicate this secret. Default: - Secret is not replicated
         :param secret_name: A name for the secret. Note that deleting secrets from SecretsManager does not happen immediately, but after a 7 to 30 days blackout period. During that period, it is not possible to create another secret that shares the same name. Default: - A name is generated by CloudFormation.
-        :param convert_to_json: (experimental) Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
-        :param flatten: (experimental) Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
-        :param sops_age_key: (experimental) The age key that should be used for encryption.
-        :param sops_file_format: (experimental) The format of the sops file. Default: - The fileformat will be derived from the file ending
-        :param sops_file_path: (experimental) The filepath to the sops file.
-        :param sops_kms_key: (experimental) The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
-        :param sops_provider: (experimental) The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
-        :param sops_s3_bucket: (experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param sops_s3_key: (experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-        :param stringify_values: (experimental) Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
-        :param upload_type: (experimental) How should the secret be passed to the CustomResource? Default: INLINE
-
-        :stability: experimental
+        :param convert_to_json: Should the encrypted sops value should be converted to JSON? Only JSON can be handled by cloud formations dynamic references. Default: true
+        :param flatten: Should the structure be flattened? The result will be a flat structure and all object keys will be replaced with the full jsonpath as key. This is usefull for dynamic references, as those don't support nested objects. Default: true
+        :param sops_age_key: The age key that should be used for encryption.
+        :param sops_file_format: The format of the sops file. Default: - The fileformat will be derived from the file ending
+        :param sops_file_path: The filepath to the sops file.
+        :param sops_kms_key: The kmsKey used to encrypt the sops file. Encrypt permissions will be granted to the custom resource provider. Default: - The key will be derived from the sops file
+        :param sops_provider: The custom resource provider to use. If you don't specify any, a new provider will be created - or if already exists within this stack - reused. Default: - A new singleton provider will be created
+        :param sops_s3_bucket: If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param sops_s3_key: If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
+        :param stringify_values: Shall all values be flattened? This is usefull for dynamic references, as there are lookup errors for certain float types
+        :param upload_type: How should the secret be passed to the CustomResource? Default: INLINE
         '''
         if isinstance(generate_secret_string, dict):
             generate_secret_string = _aws_cdk_aws_secretsmanager_ceddda9d.SecretStringGenerator(**generate_secret_string)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__6b5ff836a3767bbc726a1167e9f5e789f0fad2dcaf72b41a245494f0a121a8a3)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
@@ -1402,136 +1262,110 @@
         :default: - A name is generated by CloudFormation.
         '''
         result = self._values.get("secret_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def convert_to_json(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the encrypted sops value should be converted to JSON?
+        '''Should the encrypted sops value should be converted to JSON?
 
         Only JSON can be handled by cloud formations dynamic references.
 
         :default: true
-
-        :stability: experimental
         '''
         result = self._values.get("convert_to_json")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def flatten(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Should the structure be flattened?
+        '''Should the structure be flattened?
 
         The result will be a flat structure and all
         object keys will be replaced with the full jsonpath as key.
         This is usefull for dynamic references, as those don't support nested objects.
 
         :default: true
-
-        :stability: experimental
         '''
         result = self._values.get("flatten")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def sops_age_key(self) -> typing.Optional[_aws_cdk_ceddda9d.SecretValue]:
-        '''(experimental) The age key that should be used for encryption.
-
-        :stability: experimental
-        '''
+        '''The age key that should be used for encryption.'''
         result = self._values.get("sops_age_key")
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.SecretValue], result)
 
     @builtins.property
     def sops_file_format(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The format of the sops file.
+        '''The format of the sops file.
 
         :default: - The fileformat will be derived from the file ending
-
-        :stability: experimental
         '''
         result = self._values.get("sops_file_format")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_file_path(self) -> typing.Optional[builtins.str]:
-        '''(experimental) The filepath to the sops file.
-
-        :stability: experimental
-        '''
+        '''The filepath to the sops file.'''
         result = self._values.get("sops_file_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_kms_key(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]]:
-        '''(experimental) The kmsKey used to encrypt the sops file.
+        '''The kmsKey used to encrypt the sops file.
 
         Encrypt permissions
         will be granted to the custom resource provider.
 
         :default: - The key will be derived from the sops file
-
-        :stability: experimental
         '''
         result = self._values.get("sops_kms_key")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_kms_ceddda9d.IKey]], result)
 
     @builtins.property
     def sops_provider(self) -> typing.Optional[SopsSyncProvider]:
-        '''(experimental) The custom resource provider to use.
+        '''The custom resource provider to use.
 
         If you don't specify any, a new
         provider will be created - or if already exists within this stack - reused.
 
         :default: - A new singleton provider will be created
-
-        :stability: experimental
         '''
         result = self._values.get("sops_provider")
         return typing.cast(typing.Optional[SopsSyncProvider], result)
 
     @builtins.property
     def sops_s3_bucket(self) -> typing.Optional[builtins.str]:
-        '''(experimental) If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-
-        :stability: experimental
-        '''
+        '''If you want to pass the sops file via s3, you can specify the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.'''
         result = self._values.get("sops_s3_bucket")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sops_s3_key(self) -> typing.Optional[builtins.str]:
-        '''(experimental) If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.
-
-        :stability: experimental
-        '''
+        '''If you want to pass the sops file via s3, you can specify the key inside the bucket you can use cfn parameter here Both, sopsS3Bucket and sopsS3Key have to be specified.'''
         result = self._values.get("sops_s3_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def stringify_values(self) -> typing.Optional[builtins.bool]:
-        '''(experimental) Shall all values be flattened?
+        '''Shall all values be flattened?
 
         This is usefull for dynamic references, as there
         are lookup errors for certain float types
-
-        :stability: experimental
         '''
         result = self._values.get("stringify_values")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def upload_type(self) -> typing.Optional[UploadType]:
-        '''(experimental) How should the secret be passed to the CustomResource?
+        '''How should the secret be passed to the CustomResource?
 
         :default: INLINE
-
-        :stability: experimental
         '''
         result = self._values.get("upload_type")
         return typing.cast(typing.Optional[UploadType], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdk-sops-secrets-1.8.1/src/cdk_sops_secrets.egg-info/PKG-INFO` & `cdk-sops-secrets-1.8.2/src/cdk_sops_secrets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cdk-sops-secrets
-Version: 1.8.1
+Version: 1.8.2
 Summary: CDK Constructs that syncs your sops secrets into AWS SecretsManager secrets.
 Home-page: https://constructs.dev/packages/cdk-sops-secrets
 Author: Markus Siebert<markus.siebert@deutschebahn.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/dbsystel/cdk-sops-secrets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="https://github.com/dbsystel/cdk-sops-secrets/blob/main/img/banner-dl-small.png?raw=true">
 <p/>
```

