# Comparing `tmp/iam_actions-1.2.20240515.tar.gz` & `tmp/iam_actions-1.2.20240516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240515.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240516.tar", max compression
```

## Comparing `iam_actions-1.2.20240515.tar` & `iam_actions-1.2.20240516.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/README.md
--rw-r--r--   0        0        0      228 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/__init__.py
--rw-r--r--   0        0        0  4832046 2024-05-15 02:27:09.338042 iam_actions-1.2.20240515/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-15 02:25:17.741721 iam_actions-1.2.20240515/iam_actions/generate/services.py
--rw-r--r--   0        0        0   628534 2024-05-15 02:27:09.338042 iam_actions-1.2.20240515/iam_actions/policies.json
--rw-r--r--   0        0        0   209565 2024-05-15 02:27:09.338042 iam_actions-1.2.20240515/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   609873 2024-05-15 02:27:09.338042 iam_actions-1.2.20240515/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-15 02:27:09.990044 iam_actions-1.2.20240515/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240515/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240515/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/README.md
+-rw-r--r--   0        0        0      228 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4834343 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-16 02:21:43.383255 iam_actions-1.2.20240516/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   628769 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/policies.json
+-rw-r--r--   0        0        0   209690 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   610102 2024-05-16 02:23:31.118457 iam_actions-1.2.20240516/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-16 02:23:31.766452 iam_actions-1.2.20240516/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240516/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240516/PKG-INFO
```

### Comparing `iam_actions-1.2.20240515/LICENSE` & `iam_actions-1.2.20240516/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/README.md` & `iam_actions-1.2.20240516/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/iam_actions/actions.json` & `iam_actions-1.2.20240516/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996868552963564%*

 * *Differences: {"'connect'": "{'DeleteAttachedFile': {'access_level': 'Write', 'condition_keys': "*

 * *              "['aws:RequestTag/${TagKey}', 'aws:TagKeys', 'connect:InstanceId'], 'description': "*

 * *              "'Grants permission to delete an attached file from an Amazon Connect instance', "*

 * *              "'resources': ['attached-file']}, 'CompleteAttachedFileUpload': {'access_level': "*

 * *              "'Write', 'condition_keys': ['aws:RequestTag/${TagKey}', 'aws:TagKeys', "*

 * *              "'connect:InstanceId'], 'descript […]*

```diff
@@ -34495,20 +34495,26 @@
             "description": "Grants permission to revoke access and to disassociate the datasets with the specified AWS account",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
         "BatchGetAttachedFileMetadata": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "BatchGetAttachedFileMetadata",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to get metadata for multiple attached files from an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "attached-file"
+            ]
         },
         "BatchGetFlowAssociation": {
             "access_level": "List",
             "action": "BatchGetFlowAssociation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
@@ -34545,20 +34551,26 @@
             "resources": [
                 "instance",
                 "traffic-distribution-group",
                 "wildcard-phone-number"
             ]
         },
         "CompleteAttachedFileUpload": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CompleteAttachedFileUpload",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to complete an attached file upload in an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "attached-file"
+            ]
         },
         "CreateAgentStatus": {
             "access_level": "Write",
             "action": "CreateAgentStatus",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
@@ -34900,20 +34912,26 @@
             "description": "Grants permission to deactivate an evaluation form in the specified Amazon Connect instance. After a form is deactivated, it is no longer available for users to start new evaluations based on the form",
             "orphan": false,
             "resources": [
                 "evaluation-form"
             ]
         },
         "DeleteAttachedFile": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteAttachedFile",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to delete an attached file from an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "attached-file"
+            ]
         },
         "DeleteContactEvaluation": {
             "access_level": "Write",
             "action": "DeleteContactEvaluation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
@@ -35689,20 +35707,26 @@
             "description": "Grants permission to dismiss terminated Contact from Agent CCP",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
         "GetAttachedFile": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetAttachedFile",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to get an attached file from an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "attached-file"
+            ]
         },
         "GetContactAttributes": {
             "access_level": "Read",
             "action": "GetContactAttributes",
             "condition_keys": [
                 "connect:InstanceId"
             ],
@@ -36628,20 +36652,27 @@
             "action": "SendChatIntegrationEvent",
             "condition_keys": [],
             "description": "Grants permission to send chat integration events using the Amazon Connect API",
             "orphan": false,
             "resources": []
         },
         "StartAttachedFileUpload": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartAttachedFileUpload",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys",
+                "connect:InstanceId",
+                "connect:UserArn"
+            ],
+            "description": "Grants permission to start an attached file upload in an Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "attached-file"
+            ]
         },
         "StartChatContact": {
             "access_level": "Write",
             "action": "StartChatContact",
             "condition_keys": [
                 "connect:InstanceId"
             ],
@@ -68914,20 +68945,25 @@
             "description": "Grants permission to update an endpoint",
             "orphan": false,
             "resources": [
                 "endpoint"
             ]
         },
         "UpdateEventBus": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateEventBus",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to update event buses",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "event-bus"
+            ]
         }
     },
     "evidently": {
         "BatchEvaluateFeature": {
             "access_level": "Write",
             "action": "BatchEvaluateFeature",
             "condition_keys": [],
@@ -78282,14 +78318,30 @@
             "condition_keys": [],
             "description": "Grants permission to create API keys for a workspace",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         },
+        "CreateWorkspaceServiceAccount": {
+            "access_level": "Undocumented",
+            "action": "CreateWorkspaceServiceAccount",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateWorkspaceServiceAccountToken": {
+            "access_level": "Undocumented",
+            "action": "CreateWorkspaceServiceAccountToken",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteWorkspace": {
             "access_level": "Write",
             "action": "DeleteWorkspace",
             "condition_keys": [],
             "description": "Grants permission to delete a workspace",
             "orphan": false,
             "resources": [
@@ -78302,14 +78354,30 @@
             "condition_keys": [],
             "description": "Grants permission to delete API keys from a workspace",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         },
+        "DeleteWorkspaceServiceAccount": {
+            "access_level": "Undocumented",
+            "action": "DeleteWorkspaceServiceAccount",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteWorkspaceServiceAccountToken": {
+            "access_level": "Undocumented",
+            "action": "DeleteWorkspaceServiceAccountToken",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeWorkspace": {
             "access_level": "Read",
             "action": "DescribeWorkspace",
             "condition_keys": [],
             "description": "Grants permission to describe a workspace",
             "orphan": false,
             "resources": [
@@ -78372,14 +78440,30 @@
             "condition_keys": [],
             "description": "Grants permission to list all available supported Grafana versions. Optionally, include a workspace to list the versions to which it can be upgraded",
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         },
+        "ListWorkspaceServiceAccountTokens": {
+            "access_level": "Undocumented",
+            "action": "ListWorkspaceServiceAccountTokens",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListWorkspaceServiceAccounts": {
+            "access_level": "Undocumented",
+            "action": "ListWorkspaceServiceAccounts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListWorkspaces": {
             "access_level": "Read",
             "action": "ListWorkspaces",
             "condition_keys": [],
             "description": "Grants permission to list workspaces",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20240515/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240516/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240516/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/iam_actions/generate/generate.py` & `iam_actions-1.2.20240516/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240516/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240516/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/iam_actions/generate/services.py` & `iam_actions-1.2.20240516/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240515/iam_actions/policies.json` & `iam_actions-1.2.20240516/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999975669099757%*

 * *Differences: {"'serviceMap'": "{'Amazon Managed Grafana': {'Actions': {insert: [(3, "*

 * *                 "'CreateWorkspaceServiceAccount'), (4, 'CreateWorkspaceServiceAccountToken'), (7, "*

 * *                 "'DeleteWorkspaceServiceAccount'), (8, 'DeleteWorkspaceServiceAccountToken'), "*

 * *                 "(16, 'ListWorkspaceServiceAccountTokens'), (17, "*

 * *                 "'ListWorkspaceServiceAccounts')]}}}"}*

```diff
@@ -17685,23 +17685,29 @@
         "Amazon Managed Grafana": {
             "ARNFormat": "arn:aws:grafana:${Region}:${Account}:/${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:grafana:.+:.+:.+",
             "Actions": [
                 "AssociateLicense",
                 "CreateWorkspace",
                 "CreateWorkspaceApiKey",
+                "CreateWorkspaceServiceAccount",
+                "CreateWorkspaceServiceAccountToken",
                 "DeleteWorkspace",
                 "DeleteWorkspaceApiKey",
+                "DeleteWorkspaceServiceAccount",
+                "DeleteWorkspaceServiceAccountToken",
                 "DescribeWorkspace",
                 "DescribeWorkspaceAuthentication",
                 "DescribeWorkspaceConfiguration",
                 "DisassociateLicense",
                 "ListPermissions",
                 "ListTagsForResource",
                 "ListVersions",
+                "ListWorkspaceServiceAccountTokens",
+                "ListWorkspaceServiceAccounts",
                 "ListWorkspaces",
                 "TagResource",
                 "UntagResource",
                 "UpdatePermissions",
                 "UpdateWorkspace",
                 "UpdateWorkspaceAuthentication",
                 "UpdateWorkspaceConfiguration"
```

### Comparing `iam_actions-1.2.20240515/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240516/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998046165030897%*

 * *Differences: {"'connect'": "{'attached-file': OrderedDict([('arn_pattern', "*

 * *              "'arn:*:connect:*:*:instance/*/file/*'), ('condition_keys', "*

 * *              "'aws:ResourceTag/${TagKey}')])}",*

 * * "'neptune-db'": "{'database': {'arn_pattern': 'arn:*:neptune-db:*:*:*/*'}}"}*

```diff
@@ -1468,14 +1468,18 @@
         }
     },
     "connect": {
         "agent-status": {
             "arn_pattern": "arn:*:connect:*:*:instance/*/agent-state/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "attached-file": {
+            "arn_pattern": "arn:*:connect:*:*:instance/*/file/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "aws-managed-view": {
             "arn_pattern": "arn:*:connect:*:aws:view/*",
             "condition_keys": null
         },
         "contact": {
             "arn_pattern": "arn:*:connect:*:*:instance/*/contact/*",
             "condition_keys": null
@@ -4733,15 +4737,15 @@
         "configurations": {
             "arn_pattern": "arn:*:mq:*:*:configuration:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "neptune-db": {
         "database": {
-            "arn_pattern": "arn:*:neptune-db:*:*:*/database",
+            "arn_pattern": "arn:*:neptune-db:*:*:*/*",
             "condition_keys": null
         }
     },
     "neptune-graph": {},
     "network-firewall": {
         "Firewall": {
             "arn_pattern": "arn:*:network-firewall:*:*:firewall/*",
```

### Comparing `iam_actions-1.2.20240515/iam_actions/services.json` & `iam_actions-1.2.20240516/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999745547073792%*

 * *Differences: {"'grafana'": "{'Actions': {insert: [(3, 'CreateWorkspaceServiceAccount'), (4, "*

 * *              "'CreateWorkspaceServiceAccountToken'), (7, 'DeleteWorkspaceServiceAccount'), (8, "*

 * *              "'DeleteWorkspaceServiceAccountToken'), (16, 'ListWorkspaceServiceAccountTokens'), "*

 * *              "(17, 'ListWorkspaceServiceAccounts')]}}"}*

```diff
@@ -10651,23 +10651,29 @@
         "ARNRegexes": [
             "^arn:aws:grafana:.+:.+:.+"
         ],
         "Actions": [
             "AssociateLicense",
             "CreateWorkspace",
             "CreateWorkspaceApiKey",
+            "CreateWorkspaceServiceAccount",
+            "CreateWorkspaceServiceAccountToken",
             "DeleteWorkspace",
             "DeleteWorkspaceApiKey",
+            "DeleteWorkspaceServiceAccount",
+            "DeleteWorkspaceServiceAccountToken",
             "DescribeWorkspace",
             "DescribeWorkspaceAuthentication",
             "DescribeWorkspaceConfiguration",
             "DisassociateLicense",
             "ListPermissions",
             "ListTagsForResource",
             "ListVersions",
+            "ListWorkspaceServiceAccountTokens",
+            "ListWorkspaceServiceAccounts",
             "ListWorkspaces",
             "TagResource",
             "UntagResource",
             "UpdatePermissions",
             "UpdateWorkspace",
             "UpdateWorkspaceAuthentication",
             "UpdateWorkspaceConfiguration"
```

### Comparing `iam_actions-1.2.20240515/pyproject.toml` & `iam_actions-1.2.20240516/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240515"
+version = "1.2.20240516"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240515/setup.py` & `iam_actions-1.2.20240516/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240515',
+    'version': '1.2.20240516',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240515/PKG-INFO` & `iam_actions-1.2.20240516/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240515
+Version: 1.2.20240516
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

