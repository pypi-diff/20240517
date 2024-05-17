# Comparing `tmp/pywindmill-1.0.0.1-py3-none-any.whl.zip` & `tmp/pywindmill-1.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2892 bytes, number of entries: 7
--rw-r--r--  2.0 unx      213 b- defN 24-Mar-28 13:47 windmillclient/__init__.py
--rw-r--r--  2.0 unx      213 b- defN 24-Mar-28 13:47 windmillclient/client/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-Mar-28 13:47 windmillclient/client/windmill_client.py
--rw-r--r--  2.0 unx      909 b- defN 24-Mar-28 13:47 pywindmill-1.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-28 13:47 pywindmill-1.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Mar-28 13:47 pywindmill-1.0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      585 b- defN 24-Mar-28 13:47 pywindmill-1.0.0.1.dist-info/RECORD
-7 files, 4098 bytes uncompressed, 1844 bytes compressed:  55.0%
+Zip file size: 2677 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-26 03:08 windmillclient/__init__.py
+-rw-r--r--  2.0 unx      213 b- defN 24-Apr-26 03:08 windmillclient/client/__init__.py
+-rw-r--r--  2.0 unx     1437 b- defN 24-Apr-26 03:08 windmillclient/client/windmill_client.py
+-rw-r--r--  2.0 unx      895 b- defN 24-Apr-26 03:08 pywindmill-1.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-26 03:08 pywindmill-1.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-26 03:08 pywindmill-1.0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      585 b- defN 24-Apr-26 03:08 pywindmill-1.0.0.2.dist-info/RECORD
+7 files, 3450 bytes uncompressed, 1629 bytes compressed:  52.8%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: windmillclient/client/__init__.py
 Comment: 
 
 Filename: windmillclient/client/windmill_client.py
 Comment: 
 
-Filename: pywindmill-1.0.0.1.dist-info/METADATA
+Filename: pywindmill-1.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pywindmill-1.0.0.1.dist-info/WHEEL
+Filename: pywindmill-1.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pywindmill-1.0.0.1.dist-info/top_level.txt
+Filename: pywindmill-1.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pywindmill-1.0.0.1.dist-info/RECORD
+Filename: pywindmill-1.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## windmillclient/client/windmill_client.py

```diff
@@ -5,45 +5,32 @@
 
 # @Time : 2024/2/27 16:16
 # @Author : yangtingyu01
 # @Email: yangtingyu01@baidu.com
 # @File : windmill_client.py
 # @Software: PyCharm
 """
-from typing import Optional
-from baidubce.bce_client_configuration import BceClientConfiguration
 from windmillartifactv1.client.artifact_client import ArtifactClient
 from windmillcomputev1.client.compute_client import ComputeClient
 from windmillendpointv1.client.endpoint_monitor_client import EndpointMonitorClient
 from windmillendpointv1.client.endpoint_client import EndpointClient
 from windmillmodelv1.client.model_client import ModelClient
 from windmilltrainingv1.client.training_client import TrainingClient
 from windmillcategoryv1.client.category_client import CategoryClient
+from windmillworkspacev1.client.workspace_client import WorkspaceClient
 from windmillusersettingv1.client.internal_usersetting_client import InternalUsersettingClient
 
 
-class WindmillClient(ArtifactClient,
+class WindmillClient(WorkspaceClient,
+                     ArtifactClient,
                      ModelClient,
                      TrainingClient,
                      ComputeClient,
                      EndpointClient,
                      EndpointMonitorClient,
                      CategoryClient,
                      InternalUsersettingClient):
     """
     A client class for interacting with the windmill service. Initializes with default configuration.
 
     This client provides an interface to send requests to the BceService.
-
-    Args:
-            config (Optional[BceClientConfiguration]): The client configuration to use.
-            ak (Optional[str]): Access key for authentication.
-            sk (Optional[str]): Secret key for authentication.
-            endpoint (Optional[str]): The service endpoint URL.
-    """
-
-    def __init__(self, config: Optional[BceClientConfiguration] = None, ak: Optional[str] = "", sk: Optional[str] = "",
-                 endpoint: Optional[str] = ""):
-        """
-        Initialize the WindmillClient with the provided configuration.
-        """
-        super(WindmillClient, self).__init__(config=config, ak=ak, sk=sk, endpoint=endpoint)
+    """
```

