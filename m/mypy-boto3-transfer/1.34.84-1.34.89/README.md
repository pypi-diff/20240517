# Comparing `tmp/mypy_boto3_transfer-1.34.84.tar.gz` & `tmp/mypy_boto3_transfer-1.34.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_transfer-1.34.84.tar", last modified: Fri Apr 12 19:32:38 2024, max compression
+gzip compressed data, was "mypy_boto3_transfer-1.34.89.tar", last modified: Mon Apr 22 19:19:14 2024, max compression
```

## Comparing `mypy_boto3_transfer-1.34.84.tar` & `mypy_boto3_transfer-1.34.89.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47413 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    47410 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-04-12 19:32:23.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13303 2024-04-12 19:32:23.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-12 19:32:24.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51669 2024-04-12 19:32:23.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-12 19:32:22.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 19:32:38.000000 mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:38.645303 mypy_boto3_transfer-1.34.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-12 19:32:21.000000 mypy_boto3_transfer-1.34.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:14.139680 mypy_boto3_transfer-1.34.89/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-22 19:19:14.139680 mypy_boto3_transfer-1.34.89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:14.135680 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48094 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48091 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13326 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13326 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12188 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12176 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52241 2024-04-22 19:19:01.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52241 2024-04-22 19:19:01.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-22 19:19:00.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 19:19:14.139680 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-04-22 19:19:14.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-22 19:19:14.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:14.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 19:19:14.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-22 19:19:14.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-22 19:19:14.000000 mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 19:19:14.139680 mypy_boto3_transfer-1.34.89/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-22 19:18:59.000000 mypy_boto3_transfer-1.34.89/setup.py
```

### Comparing `mypy_boto3_transfer-1.34.84/LICENSE` & `mypy_boto3_transfer-1.34.89/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/PKG-INFO` & `mypy_boto3_transfer-1.34.89/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.34.84
-Summary: Type annotations for boto3.Transfer 1.34.84 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.89
+Summary: Type annotations for boto3.Transfer 1.34.89 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_transfer-1.34.84/README.md` & `mypy_boto3_transfer-1.34.89/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.py` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__init__.pyi` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/__main__.py` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Transfer 1.34.84\n"
-        "Version:         1.34.84\n"
+        "Type annotations for boto3.Transfer 1.34.89\n"
+        "Version:         1.34.89\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.84")
+    print("1.34.89")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.py` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     PosixProfileTypeDef,
     ProtocolDetailsTypeDef,
     S3StorageOptionsTypeDef,
     SftpConnectorConfigTypeDef,
+    StartDirectoryListingResponseTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
@@ -702,14 +703,29 @@
         """
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#send_workflow_step_state)
         """
 
+    def start_directory_listing(
+        self,
+        *,
+        ConnectorId: str,
+        RemoteDirectoryPath: str,
+        OutputDirectoryPath: str,
+        MaxItems: int = ...,
+    ) -> StartDirectoryListingResponseTypeDef:
+        """
+        Retrieves a list of the contents of a directory from a remote SFTP server.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_directory_listing)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_directory_listing)
+        """
+
     def start_file_transfer(
         self,
         *,
         ConnectorId: str,
         SendFilePaths: Sequence[str] = ...,
         RetrieveFilePaths: Sequence[str] = ...,
         LocalDirectoryPath: str = ...,
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/client.pyi` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     PosixProfileTypeDef,
     ProtocolDetailsTypeDef,
     S3StorageOptionsTypeDef,
     SftpConnectorConfigTypeDef,
+    StartDirectoryListingResponseTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
     TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
@@ -699,14 +700,29 @@
         """
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#send_workflow_step_state)
         """
 
+    def start_directory_listing(
+        self,
+        *,
+        ConnectorId: str,
+        RemoteDirectoryPath: str,
+        OutputDirectoryPath: str,
+        MaxItems: int = ...,
+    ) -> StartDirectoryListingResponseTypeDef:
+        """
+        Retrieves a list of the contents of a directory from a remote SFTP server.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_directory_listing)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/client/#start_directory_listing)
+        """
+
     def start_file_transfer(
         self,
         *,
         ConnectorId: str,
         SendFilePaths: Sequence[str] = ...,
         RetrieveFilePaths: Sequence[str] = ...,
         LocalDirectoryPath: str = ...,
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.py` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,14 +432,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/literals.pyi` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -432,14 +432,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.py` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/paginator.pyi` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.py` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
+    "StartDirectoryListingRequestRequestTypeDef",
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
@@ -151,14 +152,15 @@
     "CreateUserResponseTypeDef",
     "CreateWorkflowResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ImportCertificateResponseTypeDef",
     "ImportHostKeyResponseTypeDef",
     "ImportSshPublicKeyResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
+    "StartDirectoryListingResponseTypeDef",
     "StartFileTransferResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "TestIdentityProviderResponseTypeDef",
     "UpdateAccessResponseTypeDef",
     "UpdateAgreementResponseTypeDef",
     "UpdateCertificateResponseTypeDef",
     "UpdateConnectorResponseTypeDef",
@@ -765,14 +767,23 @@
     "UserDetailsTypeDef",
     {
         "UserName": str,
         "ServerId": str,
         "SessionId": NotRequired[str],
     },
 )
+StartDirectoryListingRequestRequestTypeDef = TypedDict(
+    "StartDirectoryListingRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+        "RemoteDirectoryPath": str,
+        "OutputDirectoryPath": str,
+        "MaxItems": NotRequired[int],
+    },
+)
 StartFileTransferRequestRequestTypeDef = TypedDict(
     "StartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
         "SendFilePaths": NotRequired[Sequence[str]],
         "RetrieveFilePaths": NotRequired[Sequence[str]],
         "LocalDirectoryPath": NotRequired[str],
@@ -985,14 +996,22 @@
     "ListSecurityPoliciesResponseTypeDef",
     {
         "NextToken": str,
         "SecurityPolicyNames": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartDirectoryListingResponseTypeDef = TypedDict(
+    "StartDirectoryListingResponseTypeDef",
+    {
+        "ListingId": str,
+        "OutputFileName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StartFileTransferResponseTypeDef = TypedDict(
     "StartFileTransferResponseTypeDef",
     {
         "TransferId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/type_defs.pyi` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     "ListUsersRequestRequestTypeDef",
     "ListedUserTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ListedWorkflowTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
+    "StartDirectoryListingRequestRequestTypeDef",
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
     "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
@@ -151,14 +152,15 @@
     "CreateUserResponseTypeDef",
     "CreateWorkflowResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ImportCertificateResponseTypeDef",
     "ImportHostKeyResponseTypeDef",
     "ImportSshPublicKeyResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
+    "StartDirectoryListingResponseTypeDef",
     "StartFileTransferResponseTypeDef",
     "TestConnectionResponseTypeDef",
     "TestIdentityProviderResponseTypeDef",
     "UpdateAccessResponseTypeDef",
     "UpdateAgreementResponseTypeDef",
     "UpdateCertificateResponseTypeDef",
     "UpdateConnectorResponseTypeDef",
@@ -765,14 +767,23 @@
     "UserDetailsTypeDef",
     {
         "UserName": str,
         "ServerId": str,
         "SessionId": NotRequired[str],
     },
 )
+StartDirectoryListingRequestRequestTypeDef = TypedDict(
+    "StartDirectoryListingRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+        "RemoteDirectoryPath": str,
+        "OutputDirectoryPath": str,
+        "MaxItems": NotRequired[int],
+    },
+)
 StartFileTransferRequestRequestTypeDef = TypedDict(
     "StartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
         "SendFilePaths": NotRequired[Sequence[str]],
         "RetrieveFilePaths": NotRequired[Sequence[str]],
         "LocalDirectoryPath": NotRequired[str],
@@ -985,14 +996,22 @@
     "ListSecurityPoliciesResponseTypeDef",
     {
         "NextToken": str,
         "SecurityPolicyNames": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+StartDirectoryListingResponseTypeDef = TypedDict(
+    "StartDirectoryListingResponseTypeDef",
+    {
+        "ListingId": str,
+        "OutputFileName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 StartFileTransferResponseTypeDef = TypedDict(
     "StartFileTransferResponseTypeDef",
     {
         "TransferId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.py` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer/waiter.pyi` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/PKG-INFO` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-transfer
-Version: 1.34.84
-Summary: Type annotations for boto3.Transfer 1.34.84 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.89
+Summary: Type annotations for boto3.Transfer 1.34.89 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-transfer.svg?color=blue)](https://pypi.org/project/mypy-boto3-transfer)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_transfer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-transfer)](https://pepy.tech/project/mypy-boto3-transfer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Transfer 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
+[boto3.Transfer 1.34.89](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy_boto3_transfer-1.34.84/mypy_boto3_transfer.egg-info/SOURCES.txt` & `mypy_boto3_transfer-1.34.89/mypy_boto3_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_transfer-1.34.84/setup.py` & `mypy_boto3_transfer-1.34.89/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-transfer",
-    version="1.34.84",
+    version="1.34.89",
     packages=["mypy_boto3_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Transfer 1.34.84 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Transfer 1.34.89 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

