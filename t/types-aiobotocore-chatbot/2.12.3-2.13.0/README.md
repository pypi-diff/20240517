# Comparing `tmp/types-aiobotocore-chatbot-2.12.3.tar.gz` & `tmp/types_aiobotocore_chatbot-2.13.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chatbot-2.12.3.tar", last modified: Fri Apr 12 01:17:01 2024, max compression
+gzip compressed data, was "types_aiobotocore_chatbot-2.13.0.tar", last modified: Fri May 17 01:21:58 2024, max compression
```

## Comparing `types-aiobotocore-chatbot-2.12.3.tar` & `types_aiobotocore_chatbot-2.13.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 01:01:19.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 01:17:01.409308 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 01:17:01.000000 types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:58.827110 types_aiobotocore_chatbot-2.13.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-17 01:21:58.827110 types_aiobotocore_chatbot-2.13.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 01:21:58.827110 types_aiobotocore_chatbot-2.13.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:58.823110 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23979 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-05-17 01:04:52.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16177 2024-05-17 01:04:52.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 01:04:51.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 01:21:58.827110 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12260 2024-05-17 01:21:58.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-17 01:21:58.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:21:58.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 01:21:58.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 01:21:58.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 01:21:58.000000 types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chatbot-2.12.3/LICENSE` & `types_aiobotocore_chatbot-2.13.0/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chatbot-2.12.3/PKG-INFO` & `types_aiobotocore_chatbot-2.13.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chatbot
-Version: 2.12.3
-Summary: Type annotations for aiobotocore.Chatbot 2.12.3 service generated with mypy-boto3-builder 7.23.2
+Version: 2.13.0
+Summary: Type annotations for aiobotocore.Chatbot 2.13.0 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chatbot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chatbot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chatbot)](https://pepy.tech/project/types-aiobotocore-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chatbot 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
+[aiobotocore.Chatbot 2.13.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-chatbot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chatbot-2.12.3/README.md` & `types_aiobotocore_chatbot-2.13.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chatbot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chatbot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chatbot)](https://pepy.tech/project/types-aiobotocore-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chatbot 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
+[aiobotocore.Chatbot 2.13.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-chatbot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chatbot-2.12.3/setup.py` & `types_aiobotocore_chatbot-2.13.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chatbot",
-    version="2.12.3",
+    version="2.13.0",
     packages=["types_aiobotocore_chatbot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore.Chatbot 2.12.3 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for aiobotocore.Chatbot 2.13.0 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.py` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/client.pyi` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.py` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -109,24 +110,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -323,14 +326,15 @@
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

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/literals.pyi` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -109,24 +110,26 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -323,14 +326,15 @@
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

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.py` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,32 +368,32 @@
         "WebhookConfiguration": ChimeWebhookConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeChimeWebhookConfigurationsResultTypeDef = TypedDict(
     "DescribeChimeWebhookConfigurationsResultTypeDef",
     {
-        "NextToken": str,
         "WebhookConfigurations": List[ChimeWebhookConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetAccountPreferencesResultTypeDef = TypedDict(
     "GetAccountPreferencesResultTypeDef",
     {
         "AccountPreferences": AccountPreferencesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListMicrosoftTeamsConfiguredTeamsResultTypeDef = TypedDict(
     "ListMicrosoftTeamsConfiguredTeamsResultTypeDef",
     {
         "ConfiguredTeams": List[ConfiguredTeamTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateAccountPreferencesResultTypeDef = TypedDict(
     "UpdateAccountPreferencesResultTypeDef",
     {
         "AccountPreferences": AccountPreferencesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -412,17 +412,17 @@
         "ChannelConfiguration": SlackChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSlackChannelConfigurationsResultTypeDef = TypedDict(
     "DescribeSlackChannelConfigurationsResultTypeDef",
     {
-        "NextToken": str,
         "SlackChannelConfigurations": List[SlackChannelConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateSlackChannelConfigurationResultTypeDef = TypedDict(
     "UpdateSlackChannelConfigurationResultTypeDef",
     {
         "ChannelConfiguration": SlackChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -441,43 +441,43 @@
         "ChannelConfiguration": TeamsChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTeamsChannelConfigurationsResultTypeDef = TypedDict(
     "ListTeamsChannelConfigurationsResultTypeDef",
     {
-        "NextToken": str,
         "TeamChannelConfigurations": List[TeamsChannelConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateTeamsChannelConfigurationResultTypeDef = TypedDict(
     "UpdateTeamsChannelConfigurationResultTypeDef",
     {
         "ChannelConfiguration": TeamsChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSlackUserIdentitiesResultTypeDef = TypedDict(
     "DescribeSlackUserIdentitiesResultTypeDef",
     {
         "SlackUserIdentities": List[SlackUserIdentityTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSlackWorkspacesResultTypeDef = TypedDict(
     "DescribeSlackWorkspacesResultTypeDef",
     {
         "SlackWorkspaces": List[SlackWorkspaceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMicrosoftTeamsUserIdentitiesResultTypeDef = TypedDict(
     "ListMicrosoftTeamsUserIdentitiesResultTypeDef",
     {
         "TeamsUserIdentities": List[TeamsUserIdentityTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot/type_defs.pyi` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -368,32 +368,32 @@
         "WebhookConfiguration": ChimeWebhookConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeChimeWebhookConfigurationsResultTypeDef = TypedDict(
     "DescribeChimeWebhookConfigurationsResultTypeDef",
     {
-        "NextToken": str,
         "WebhookConfigurations": List[ChimeWebhookConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 GetAccountPreferencesResultTypeDef = TypedDict(
     "GetAccountPreferencesResultTypeDef",
     {
         "AccountPreferences": AccountPreferencesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListMicrosoftTeamsConfiguredTeamsResultTypeDef = TypedDict(
     "ListMicrosoftTeamsConfiguredTeamsResultTypeDef",
     {
         "ConfiguredTeams": List[ConfiguredTeamTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateAccountPreferencesResultTypeDef = TypedDict(
     "UpdateAccountPreferencesResultTypeDef",
     {
         "AccountPreferences": AccountPreferencesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -412,17 +412,17 @@
         "ChannelConfiguration": SlackChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSlackChannelConfigurationsResultTypeDef = TypedDict(
     "DescribeSlackChannelConfigurationsResultTypeDef",
     {
-        "NextToken": str,
         "SlackChannelConfigurations": List[SlackChannelConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateSlackChannelConfigurationResultTypeDef = TypedDict(
     "UpdateSlackChannelConfigurationResultTypeDef",
     {
         "ChannelConfiguration": SlackChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -441,43 +441,43 @@
         "ChannelConfiguration": TeamsChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTeamsChannelConfigurationsResultTypeDef = TypedDict(
     "ListTeamsChannelConfigurationsResultTypeDef",
     {
-        "NextToken": str,
         "TeamChannelConfigurations": List[TeamsChannelConfigurationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateTeamsChannelConfigurationResultTypeDef = TypedDict(
     "UpdateTeamsChannelConfigurationResultTypeDef",
     {
         "ChannelConfiguration": TeamsChannelConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeSlackUserIdentitiesResultTypeDef = TypedDict(
     "DescribeSlackUserIdentitiesResultTypeDef",
     {
         "SlackUserIdentities": List[SlackUserIdentityTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeSlackWorkspacesResultTypeDef = TypedDict(
     "DescribeSlackWorkspacesResultTypeDef",
     {
         "SlackWorkspaces": List[SlackWorkspaceTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListMicrosoftTeamsUserIdentitiesResultTypeDef = TypedDict(
     "ListMicrosoftTeamsUserIdentitiesResultTypeDef",
     {
         "TeamsUserIdentities": List[TeamsUserIdentityTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/PKG-INFO` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-chatbot
-Version: 2.12.3
-Summary: Type annotations for aiobotocore.Chatbot 2.12.3 service generated with mypy-boto3-builder 7.23.2
+Version: 2.13.0
+Summary: Type annotations for aiobotocore.Chatbot 2.13.0 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chatbot.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chatbot)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-chatbot)](https://pepy.tech/project/types-aiobotocore-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Chatbot 2.12.3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
+[aiobotocore.Chatbot 2.13.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-chatbot docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chatbot/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-chatbot-2.12.3/types_aiobotocore_chatbot.egg-info/SOURCES.txt` & `types_aiobotocore_chatbot-2.13.0/types_aiobotocore_chatbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

