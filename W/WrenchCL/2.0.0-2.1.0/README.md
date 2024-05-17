# Comparing `tmp/WrenchCL-2.0.0.tar.gz` & `tmp/WrenchCL-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-2.0.0.tar", last modified: Fri May 17 06:29:11 2024, max compression
+gzip compressed data, was "WrenchCL-2.1.0.tar", last modified: Fri May 17 19:51:38 2024, max compression
```

## Comparing `WrenchCL-2.0.0.tar` & `WrenchCL-2.1.0.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21640 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.692785 WrenchCL-2.0.0/WrenchCL/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Classes/
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Classes/_ConfigurationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Classes/_SshTunnelManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Connect/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/AWSClientHub.py
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/RdsServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/S3ServiceGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Decorators/
--rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/Retryable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/SingletonClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/TimedMethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/build_return_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/handle_lambda_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/trigger_dataflow_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Models/
--rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/OpenAIFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/OpenAIGateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/_ConversationManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/Coalesce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/DictValidator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/FetchMetaData.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/FileTyper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/Image2B64.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)    26396 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.692785 WrenchCL-2.0.0/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-17 06:29:10.000000 WrenchCL-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.552937 WrenchCL-2.1.0/WrenchCL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/AwsClientHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/RdsServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/S3ServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/DataFlow/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/build_return_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/handle_lambda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/Retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/SingletonClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/TimedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15468 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/_ConversationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/OpenAI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/Coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/DictValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/FetchMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/FileTyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/Image2B64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28041 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/Tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/WrenchCL/_Internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/_Internal/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/_Internal/_SshTunnelManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/_Internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-17 19:51:16.000000 WrenchCL-2.1.0/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:51:38.556938 WrenchCL-2.1.0/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 19:51:38.000000 WrenchCL-2.1.0/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:51:38.560938 WrenchCL-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-17 19:51:36.000000 WrenchCL-2.1.0/setup.py
```

### Comparing `WrenchCL-2.0.0/LICENSE` & `WrenchCL-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/PKG-INFO` & `WrenchCL-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.0.0
+Version: 2.1.0
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Author: willem@wrench.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
-    <img src="resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
+    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
     <a href="https://github.com/Kydoimos97" style="text-decoration: none;">
         <img src="https://img.shields.io/badge/Kydoimos97-cb632b?label=Code%20Maintainer" alt="Maintainer" height="20"/>
     </a>
     <a href="https://github.com/WrenchAI/WrenchCL/actions/workflows/publish-to-pypi.yml" style="text-decoration: none;">
@@ -30,20 +30,20 @@
 
 WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 
 **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/WrenchCL/)
 
 ## Package Structure
 
-- **Classes**: Contains internal classes for configuration and SSH tunnel management.
+- **_Internal**: Contains internal classes for configuration and SSH tunnel management.
 - **Connect**: Provides gateways for AWS RDS and S3 services and the `AWSClientHub`.
 - **Decorators**: Utility decorators for retry logic, singleton pattern, and method timing.
-- **Models**: Classes for interacting with OpenAI models.
+- **Models**: _Internal for interacting with OpenAI models.
 - **Tools**: Miscellaneous utility tools such as coalescing values, file typing, image encoding, and a custom logger.
-- **Helpers**: Response focused tools to aid in returning values and generating logs based on status codes.
+- **DataFlow**: Response focused tools to aid in returning values and generating logs based on status codes.
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
@@ -54,15 +54,15 @@
 
 ### Connecting to AWS Services
 
 To interact with AWS RDS and S3 services, follow these steps:
 
 1. **Setup `AWSClientHub`**:
    ```python
-   from WrenchCL.Connections import AWSClientHub
+   from WrenchCL.Connections import AwsClientHub
 
    # Initialize the AWSClientHub using an env file or keyword arguments
    aws_client_hub = AWSClientHub(env_path="path/to/your/env/file")
    # Alternatively, use keyword arguments or existing env variables
    # aws_client_hub = AWSClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
    ```
 
@@ -124,15 +124,15 @@
 
 ### Interacting with OpenAI Models
 
 To use OpenAI models, follow these steps:
 
 1. **Setup `OpenAIGateway`**:
    ```python
-   from WrenchCL.Models import OpenAIGateway
+   from WrenchCL.Models.OpenAI import OpenAIGateway
 
    # Initialize OpenAIGateway with your OpenAI API key
    openai_gateway = OpenAIGateway(api_key="your_openai_api_key")
 
    # Example: Generating text
    response = openai_gateway.handle_text("Your prompt here")
    print(response)
@@ -156,15 +156,15 @@
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
    - `initiate_conversation(initial_text: str, **kwargs)`
      - Initiates a conversation using the provided initial text.
 
 2. **Using `OpenAIFactory`**:
    ```python
-   from WrenchCL.Models import OpenAIFactory
+   from WrenchCL.Models.OpenAI import OpenAIFactory
 
    # Initialize OpenAIFactory with your OpenAI API key
    openai_factory = OpenAIFactory(api_key="your_openai_api_key")
 
    # Example: Transcribing audio to text and getting embeddings
    audio_path = "path/to/your/audio/file"
    embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
@@ -369,39 +369,40 @@
       time.sleep(2)
       return "Done"
 
   result = slow_function()
   print(result)  # Output: "Done"
   ```
 
-### Helpers
+### DataFlow
 
-WrenchCL includes various helper functions to assist with common tasks. These helpers are located in the `Helpers` module.
+WrenchCL includes various helper functions to assist with common tasks. These helpers are located in the `DataFlow` module.
 
 #### build_return_json
 
 Constructs a JSON response with a given status code and message.
 
 ```python
-from WrenchCL.Helpers import build_return_json
+from WrenchCL.DataFlow import build_return_json
 
 response = build_return_json(code=200, message="Success")
 print(response)  # Output: {'statusCode': 200, 'body': '{"message": "Success"}'}
 ```
 
 #### handle_lambda_response
 
 Handles Lambda function responses, including logging and error handling. It stops the Lambda function execution and returns a specified response when a `GuardedResponseTrigger` exception is raised. This is particularly useful for ensuring that the Lambda function exits immediately and returns the correct response, even if the exception occurs deep within nested function calls.
 
 Here’s a comprehensive example demonstrating how to use `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and propagate responses up the call hierarchy in an AWS Lambda function.
 
 ```python
 import time
 from WrenchCL import wrench_logger
-from WrenchCL.Helpers import build_return_json, handle_lambda_response, GuardedResponseTrigger
+from WrenchCL.DataFlow import build_return_json, handle_lambda_response, GuardedResponseTrigger
+
 
 # Mock implementation of LambdaCore for the example
 class LambdaCore:
     def __init__(self, event, context):
         self.event = event
         self.context = context
 
@@ -411,42 +412,50 @@
 
     def process_request(self):
         try:
             # Perform some processing
             self.get_score({"key": "value"}, {"input_key": "input_value"})
         except Exception as e:
             # Handle other exceptions and wrap them into the GuardedResponseTrigger
-            handle_lambda_response(500, str(e), {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
-    
+            handle_lambda_response(500, str(e),
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
+
     def get_score(self, target_dict, input_dict):
         # Mock scoring process which might throw an error
         try:
             score = self.compute_score(target_dict, input_dict)
             if score is None:
-                handle_lambda_response(732, "Prediction Error: Invalid prediction provided by model.", {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
-            handle_lambda_response(200, f"Score computed successfully: {score}", {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
+                handle_lambda_response(732, "Prediction Error: Invalid prediction provided by model.",
+                                       {"event": self.event, "context": self.context, "start_time": time.time(),
+                                        "lambda_client": "lambda_client_instance"})
+            handle_lambda_response(200, f"Score computed successfully: {score}",
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
         except GuardedResponseTrigger as e:
             raise e  # Propagate the GuardedResponseTrigger upwards
         except Exception as e:
-            handle_lambda_response(757, str(e), {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
+            handle_lambda_response(757, str(e),
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
 
     def compute_score(self, target_dict, input_dict):
         # This is a placeholder for the actual scoring logic
         # Raise an error to simulate a failure
         raise ValueError("Simulated scoring error")
 
 
 def lambda_handler(event, context):
     wrench_logger.initiate_new_run()
 
     if event.get('is_warmer'):
         wrench_logger.run_id = 'R-LAMBDAS-WARM'
         wrench_logger.context("Lambda Warmed")
         return build_return_json(200, 'Warmed Lambda')
-    
+
     start_time = time.time()
     try:
         wrench_logger.info("Invoking Lambda Core")
         lambda_core_instance = LambdaCore(event=event, context=context)
         lambda_core_instance.route()
         wrench_logger.info(f"Finished Run in {round(time.time() - start_time, 2)} seconds")
     except GuardedResponseTrigger as e:
@@ -476,42 +485,27 @@
 By using `GuardedResponseTrigger` and `handle_lambda_response`, you can manage errors effectively and ensure that your Lambda function returns the correct response even when an error occurs deep within nested function calls.
 
 #### trigger_minimum_dataflow_metrics
 
 Triggers minimal data flow metrics for monitoring purposes.
 
 ```python
-from WrenchCL.Helpers import trigger_minimum_dataflow_metrics
+from WrenchCL.DataFlow import trigger_minimum_dataflow_metrics
 
-trigger_minimum_dataflow_metrics(
-    event="event_data",
-    context="context_data",
-    start_time=1625256000,
-    lambda_client="lambda_client_instance",
-    job_name="Model Inference Service",
-    job_type="Lambda",
-    status_code="200",
-    message="Success"
-)
+trigger_minimum_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
+    lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
+    message="Success")
 ```
 
 #### trigger_dataflow_metrics
 
 Triggers detailed data flow metrics for monitoring purposes.
 
 ```python
-from WrenchCL.Helpers import trigger_dataflow_metrics
+from WrenchCL.DataFlow import trigger_dataflow_metrics
 
-trigger_dataflow_metrics(
-    event="event_data",
-    context="context_data",
-    start_time=1625256000,
-    lambda_client="lambda_client_instance",
-    job_name="Model Inference Service",
-    job_type="Lambda",
-    status_code="200",
-    message="Success",
-    additional_data={"key": "value"}
-)
+trigger_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
+    lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
+    message="Success", additional_data={"key": "value"})
 ```
 
 With these detailed instructions and examples, you should be well-equipped to utilize the WrenchCL library for your projects. If you have any further questions or need additional support, please refer to the documentation or contact the maintainers.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.0.0 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.0 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Author: willem@wrench.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
@@ -10,30 +10,30 @@
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
     [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
-WrenchCL/) ## Package Structure - **Classes**: Contains internal classes for
+WrenchCL/) ## Package Structure - **_Internal**: Contains internal classes for
 configuration and SSH tunnel management. - **Connect**: Provides gateways for
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
-Classes for interacting with OpenAI models. - **Tools**: Miscellaneous utility
-tools such as coalescing values, file typing, image encoding, and a custom
-logger. - **Helpers**: Response focused tools to aid in returning values and
-generating logs based on status codes. ## Installation To install the package,
-simply run the following command: ```bash pip install WrenchCL ``` # User
-Guides Sure! Here's an updated and more detailed README that provides extensive
-instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
+_Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
+utility tools such as coalescing values, file typing, image encoding, and a
+custom logger. - **DataFlow**: Response focused tools to aid in returning
+values and generating logs based on status codes. ## Installation To install
+the package, simply run the following command: ```bash pip install WrenchCL ```
+# User Guides Sure! Here's an updated and more detailed README that provides
+extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
 `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and
 `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and
 other utility tools. ### Connecting to AWS Services To interact with AWS RDS
 and S3 services, follow these steps: 1. **Setup `AWSClientHub`**: ```python
-from WrenchCL.Connections import AWSClientHub # Initialize the AWSClientHub
+from WrenchCL.Connections import AwsClientHub # Initialize the AWSClientHub
 using an env file or keyword arguments aws_client_hub = AWSClientHub
 (env_path="path/to/your/env/file") # Alternatively, use keyword arguments or
 existing env variables # aws_client_hub = AWSClientHub
 (aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
@@ -66,42 +66,43 @@
 another. - `rename_object(bucket_name: str, src_object_key: str,
 dst_object_key: str) -> None` - Renames an object in S3. -
 `check_object_existence(bucket_name: str, object_key: str) -> bool` - Checks if
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
-**Setup `OpenAIGateway`**: ```python from WrenchCL.Models import OpenAIGateway
-# Initialize OpenAIGateway with your OpenAI API key openai_gateway =
-OpenAIGateway(api_key="your_openai_api_key") # Example: Generating text
-response = openai_gateway.handle_text("Your prompt here") print(response) ```
-**Methods in `OpenAIGateway`**: - `handle_text(text: str, model: str = "gpt-
-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] =
-None, json_mode: bool = False, **kwargs) -> Union[str, dict]` - Processes text
-input using the specified model and returns the response. - `get_embeddings
-(text: str, model: str = "text-embedding-3-small") -> list` - Retrieves
-embeddings for the given text using the specified model. - `generate_image
-(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -
-> str` - Generates an image based on the provided prompt. - `process_audio
-(audio_path: str, model: str = "whisper-1") -> str` - Processes an audio file
-and returns its transcription. - `create_image_variation(image_path: str, n:
-int = 1, size: str = "1024x1024") -> str` - Creates variations of an image
-based on the provided image path. - `edit_image(image_path: str, prompt: str,
-mask_path: str, n: int = 1, size: str = "1024x1024") -> str` - Edits an image
-based on the provided prompt and mask. - `vision_query(question: str,
-image_path: str, **kwargs) -> dict` - Processes a vision query based on the
-provided question and image. - `convert_image_to_url_or_base64(image_path: str)
--> str` - Converts an image to a URL or base64 encoded string. -
-`initiate_conversation(initial_text: str, **kwargs)` - Initiates a conversation
-using the provided initial text. 2. **Using `OpenAIFactory`**: ```python from
-WrenchCL.Models import OpenAIFactory # Initialize OpenAIFactory with your
-OpenAI API key openai_factory = OpenAIFactory(api_key="your_openai_api_key") #
-Example: Transcribing audio to text and getting embeddings audio_path = "path/
-to/your/audio/file" embeddings = openai_factory.audio_to_text_to_embeddings
-(audio_path) print(embeddings) ``` **Methods in `OpenAIFactory`**: -
+**Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
+OpenAIGateway # Initialize OpenAIGateway with your OpenAI API key
+openai_gateway = OpenAIGateway(api_key="your_openai_api_key") # Example:
+Generating text response = openai_gateway.handle_text("Your prompt here") print
+(response) ``` **Methods in `OpenAIGateway`**: - `handle_text(text: str, model:
+str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional
+[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]` -
+Processes text input using the specified model and returns the response. -
+`get_embeddings(text: str, model: str = "text-embedding-3-small") -> list` -
+Retrieves embeddings for the given text using the specified model. -
+`generate_image(prompt: str, size: str = "1024x1024", quality: str =
+"standard", n: int = 1) -> str` - Generates an image based on the provided
+prompt. - `process_audio(audio_path: str, model: str = "whisper-1") -> str` -
+Processes an audio file and returns its transcription. -
+`create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -
+> str` - Creates variations of an image based on the provided image path. -
+`edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str
+= "1024x1024") -> str` - Edits an image based on the provided prompt and mask.
+- `vision_query(question: str, image_path: str, **kwargs) -> dict` - Processes
+a vision query based on the provided question and image. -
+`convert_image_to_url_or_base64(image_path: str) -> str` - Converts an image to
+a URL or base64 encoded string. - `initiate_conversation(initial_text: str,
+**kwargs)` - Initiates a conversation using the provided initial text. 2.
+**Using `OpenAIFactory`**: ```python from WrenchCL.Models.OpenAI import
+OpenAIFactory # Initialize OpenAIFactory with your OpenAI API key
+openai_factory = OpenAIFactory(api_key="your_openai_api_key") # Example:
+Transcribing audio to text and getting embeddings audio_path = "path/to/your/
+audio/file" embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
+print(embeddings) ``` **Methods in `OpenAIFactory`**: -
 `audio_to_text_to_embeddings(audio_path: str, embedding_model: str = "text-
 embedding-3-small") -> list` - Transcribes audio to text and then generates
 embeddings for the text. - `image_to_text_to_embeddings(image_path: str,
 question: str, embedding_model: str = "text-embedding-3-small") -> list` -
 Performs a vision query to understand an image and then generates embeddings
 for the response. - `validate_response_with_gpt(initial_response: str,
 validation_prompt: str) -> str` - Uses an initial response and validates or
@@ -183,30 +184,30 @@
 return "Success" result = might_fail() print(result) ``` - **SingletonClass**:
 Ensures a class only has one instance. ```python from WrenchCL.Decorators
 import SingletonClass @SingletonClass class MySingleton: def __init__(self):
 self.value = 42 instance1 = MySingleton() instance2 = MySingleton() print
 (instance1 is instance2) # Output: True ``` - **TimedMethod**: Logs the time
 taken to execute a method. ```python from WrenchCL.Decorators import
 TimedMethod @TimedMethod def slow_function(): time.sleep(2) return "Done"
-result = slow_function() print(result) # Output: "Done" ``` ### Helpers
+result = slow_function() print(result) # Output: "Done" ``` ### DataFlow
 WrenchCL includes various helper functions to assist with common tasks. These
-helpers are located in the `Helpers` module. #### build_return_json Constructs
+helpers are located in the `DataFlow` module. #### build_return_json Constructs
 a JSON response with a given status code and message. ```python from
-WrenchCL.Helpers import build_return_json response = build_return_json
+WrenchCL.DataFlow import build_return_json response = build_return_json
 (code=200, message="Success") print(response) # Output: {'statusCode': 200,
 'body': '{"message": "Success"}'} ``` #### handle_lambda_response Handles
 Lambda function responses, including logging and error handling. It stops the
 Lambda function execution and returns a specified response when a
 `GuardedResponseTrigger` exception is raised. This is particularly useful for
 ensuring that the Lambda function exits immediately and returns the correct
 response, even if the exception occurs deep within nested function calls.
 Hereâs a comprehensive example demonstrating how to use
 `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and
 propagate responses up the call hierarchy in an AWS Lambda function. ```python
-import time from WrenchCL import wrench_logger from WrenchCL.Helpers import
+import time from WrenchCL import wrench_logger from WrenchCL.DataFlow import
 build_return_json, handle_lambda_response, GuardedResponseTrigger # Mock
 implementation of LambdaCore for the example class LambdaCore: def __init__
 (self, event, context): self.event = event self.context = context def route
 (self): # Example of nested function call where an error might occur
 self.process_request() def process_request(self): try: # Perform some
 processing self.get_score({"key": "value"}, {"input_key": "input_value"})
 except Exception as e: # Handle other exceptions and wrap them into the
@@ -251,21 +252,21 @@
 that when an error is encountered deep in the call hierarchy, the Lambda
 function stops execution and returns a response immediately. This response is
 propagated back up through the nested calls to the top-level Lambda handler. By
 using `GuardedResponseTrigger` and `handle_lambda_response`, you can manage
 errors effectively and ensure that your Lambda function returns the correct
 response even when an error occurs deep within nested function calls. ####
 trigger_minimum_dataflow_metrics Triggers minimal data flow metrics for
-monitoring purposes. ```python from WrenchCL.Helpers import
+monitoring purposes. ```python from WrenchCL.DataFlow import
 trigger_minimum_dataflow_metrics trigger_minimum_dataflow_metrics
-( event="event_data", context="context_data", start_time=1625256000,
+(event="event_data", context="context_data", start_time=1625256000,
 lambda_client="lambda_client_instance", job_name="Model Inference Service",
-job_type="Lambda", status_code="200", message="Success" ) ``` ####
+job_type="Lambda", status_code="200", message="Success") ``` ####
 trigger_dataflow_metrics Triggers detailed data flow metrics for monitoring
-purposes. ```python from WrenchCL.Helpers import trigger_dataflow_metrics
-trigger_dataflow_metrics( event="event_data", context="context_data",
+purposes. ```python from WrenchCL.DataFlow import trigger_dataflow_metrics
+trigger_dataflow_metrics(event="event_data", context="context_data",
 start_time=1625256000, lambda_client="lambda_client_instance", job_name="Model
 Inference Service", job_type="Lambda", status_code="200", message="Success",
-additional_data={"key": "value"} ) ``` With these detailed instructions and
+additional_data={"key": "value"}) ``` With these detailed instructions and
 examples, you should be well-equipped to utilize the WrenchCL library for your
 projects. If you have any further questions or need additional support, please
 refer to the documentation or contact the maintainers.
```

### Comparing `WrenchCL-2.0.0/README.md` & `WrenchCL-2.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
-    <img src="resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
+    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
     <a href="https://github.com/Kydoimos97" style="text-decoration: none;">
         <img src="https://img.shields.io/badge/Kydoimos97-cb632b?label=Code%20Maintainer" alt="Maintainer" height="20"/>
     </a>
     <a href="https://github.com/WrenchAI/WrenchCL/actions/workflows/publish-to-pypi.yml" style="text-decoration: none;">
@@ -17,20 +17,20 @@
 
 WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 
 **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/WrenchCL/)
 
 ## Package Structure
 
-- **Classes**: Contains internal classes for configuration and SSH tunnel management.
+- **_Internal**: Contains internal classes for configuration and SSH tunnel management.
 - **Connect**: Provides gateways for AWS RDS and S3 services and the `AWSClientHub`.
 - **Decorators**: Utility decorators for retry logic, singleton pattern, and method timing.
-- **Models**: Classes for interacting with OpenAI models.
+- **Models**: _Internal for interacting with OpenAI models.
 - **Tools**: Miscellaneous utility tools such as coalescing values, file typing, image encoding, and a custom logger.
-- **Helpers**: Response focused tools to aid in returning values and generating logs based on status codes.
+- **DataFlow**: Response focused tools to aid in returning values and generating logs based on status codes.
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
@@ -41,15 +41,15 @@
 
 ### Connecting to AWS Services
 
 To interact with AWS RDS and S3 services, follow these steps:
 
 1. **Setup `AWSClientHub`**:
    ```python
-   from WrenchCL.Connections import AWSClientHub
+   from WrenchCL.Connections import AwsClientHub
 
    # Initialize the AWSClientHub using an env file or keyword arguments
    aws_client_hub = AWSClientHub(env_path="path/to/your/env/file")
    # Alternatively, use keyword arguments or existing env variables
    # aws_client_hub = AWSClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
    ```
 
@@ -111,15 +111,15 @@
 
 ### Interacting with OpenAI Models
 
 To use OpenAI models, follow these steps:
 
 1. **Setup `OpenAIGateway`**:
    ```python
-   from WrenchCL.Models import OpenAIGateway
+   from WrenchCL.Models.OpenAI import OpenAIGateway
 
    # Initialize OpenAIGateway with your OpenAI API key
    openai_gateway = OpenAIGateway(api_key="your_openai_api_key")
 
    # Example: Generating text
    response = openai_gateway.handle_text("Your prompt here")
    print(response)
@@ -143,15 +143,15 @@
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
    - `initiate_conversation(initial_text: str, **kwargs)`
      - Initiates a conversation using the provided initial text.
 
 2. **Using `OpenAIFactory`**:
    ```python
-   from WrenchCL.Models import OpenAIFactory
+   from WrenchCL.Models.OpenAI import OpenAIFactory
 
    # Initialize OpenAIFactory with your OpenAI API key
    openai_factory = OpenAIFactory(api_key="your_openai_api_key")
 
    # Example: Transcribing audio to text and getting embeddings
    audio_path = "path/to/your/audio/file"
    embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
@@ -356,39 +356,40 @@
       time.sleep(2)
       return "Done"
 
   result = slow_function()
   print(result)  # Output: "Done"
   ```
 
-### Helpers
+### DataFlow
 
-WrenchCL includes various helper functions to assist with common tasks. These helpers are located in the `Helpers` module.
+WrenchCL includes various helper functions to assist with common tasks. These helpers are located in the `DataFlow` module.
 
 #### build_return_json
 
 Constructs a JSON response with a given status code and message.
 
 ```python
-from WrenchCL.Helpers import build_return_json
+from WrenchCL.DataFlow import build_return_json
 
 response = build_return_json(code=200, message="Success")
 print(response)  # Output: {'statusCode': 200, 'body': '{"message": "Success"}'}
 ```
 
 #### handle_lambda_response
 
 Handles Lambda function responses, including logging and error handling. It stops the Lambda function execution and returns a specified response when a `GuardedResponseTrigger` exception is raised. This is particularly useful for ensuring that the Lambda function exits immediately and returns the correct response, even if the exception occurs deep within nested function calls.
 
 Here’s a comprehensive example demonstrating how to use `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and propagate responses up the call hierarchy in an AWS Lambda function.
 
 ```python
 import time
 from WrenchCL import wrench_logger
-from WrenchCL.Helpers import build_return_json, handle_lambda_response, GuardedResponseTrigger
+from WrenchCL.DataFlow import build_return_json, handle_lambda_response, GuardedResponseTrigger
+
 
 # Mock implementation of LambdaCore for the example
 class LambdaCore:
     def __init__(self, event, context):
         self.event = event
         self.context = context
 
@@ -398,42 +399,50 @@
 
     def process_request(self):
         try:
             # Perform some processing
             self.get_score({"key": "value"}, {"input_key": "input_value"})
         except Exception as e:
             # Handle other exceptions and wrap them into the GuardedResponseTrigger
-            handle_lambda_response(500, str(e), {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
-    
+            handle_lambda_response(500, str(e),
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
+
     def get_score(self, target_dict, input_dict):
         # Mock scoring process which might throw an error
         try:
             score = self.compute_score(target_dict, input_dict)
             if score is None:
-                handle_lambda_response(732, "Prediction Error: Invalid prediction provided by model.", {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
-            handle_lambda_response(200, f"Score computed successfully: {score}", {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
+                handle_lambda_response(732, "Prediction Error: Invalid prediction provided by model.",
+                                       {"event": self.event, "context": self.context, "start_time": time.time(),
+                                        "lambda_client": "lambda_client_instance"})
+            handle_lambda_response(200, f"Score computed successfully: {score}",
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
         except GuardedResponseTrigger as e:
             raise e  # Propagate the GuardedResponseTrigger upwards
         except Exception as e:
-            handle_lambda_response(757, str(e), {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
+            handle_lambda_response(757, str(e),
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
 
     def compute_score(self, target_dict, input_dict):
         # This is a placeholder for the actual scoring logic
         # Raise an error to simulate a failure
         raise ValueError("Simulated scoring error")
 
 
 def lambda_handler(event, context):
     wrench_logger.initiate_new_run()
 
     if event.get('is_warmer'):
         wrench_logger.run_id = 'R-LAMBDAS-WARM'
         wrench_logger.context("Lambda Warmed")
         return build_return_json(200, 'Warmed Lambda')
-    
+
     start_time = time.time()
     try:
         wrench_logger.info("Invoking Lambda Core")
         lambda_core_instance = LambdaCore(event=event, context=context)
         lambda_core_instance.route()
         wrench_logger.info(f"Finished Run in {round(time.time() - start_time, 2)} seconds")
     except GuardedResponseTrigger as e:
@@ -463,42 +472,27 @@
 By using `GuardedResponseTrigger` and `handle_lambda_response`, you can manage errors effectively and ensure that your Lambda function returns the correct response even when an error occurs deep within nested function calls.
 
 #### trigger_minimum_dataflow_metrics
 
 Triggers minimal data flow metrics for monitoring purposes.
 
 ```python
-from WrenchCL.Helpers import trigger_minimum_dataflow_metrics
+from WrenchCL.DataFlow import trigger_minimum_dataflow_metrics
 
-trigger_minimum_dataflow_metrics(
-    event="event_data",
-    context="context_data",
-    start_time=1625256000,
-    lambda_client="lambda_client_instance",
-    job_name="Model Inference Service",
-    job_type="Lambda",
-    status_code="200",
-    message="Success"
-)
+trigger_minimum_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
+    lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
+    message="Success")
 ```
 
 #### trigger_dataflow_metrics
 
 Triggers detailed data flow metrics for monitoring purposes.
 
 ```python
-from WrenchCL.Helpers import trigger_dataflow_metrics
+from WrenchCL.DataFlow import trigger_dataflow_metrics
 
-trigger_dataflow_metrics(
-    event="event_data",
-    context="context_data",
-    start_time=1625256000,
-    lambda_client="lambda_client_instance",
-    job_name="Model Inference Service",
-    job_type="Lambda",
-    status_code="200",
-    message="Success",
-    additional_data={"key": "value"}
-)
+trigger_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
+    lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
+    message="Success", additional_data={"key": "value"})
 ```
 
 With these detailed instructions and examples, you should be well-equipped to utilize the WrenchCL library for your projects. If you have any further questions or need additional support, please refer to the documentation or contact the maintainers.
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
     [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
-WrenchCL/) ## Package Structure - **Classes**: Contains internal classes for
+WrenchCL/) ## Package Structure - **_Internal**: Contains internal classes for
 configuration and SSH tunnel management. - **Connect**: Provides gateways for
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
-Classes for interacting with OpenAI models. - **Tools**: Miscellaneous utility
-tools such as coalescing values, file typing, image encoding, and a custom
-logger. - **Helpers**: Response focused tools to aid in returning values and
-generating logs based on status codes. ## Installation To install the package,
-simply run the following command: ```bash pip install WrenchCL ``` # User
-Guides Sure! Here's an updated and more detailed README that provides extensive
-instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
+_Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
+utility tools such as coalescing values, file typing, image encoding, and a
+custom logger. - **DataFlow**: Response focused tools to aid in returning
+values and generating logs based on status codes. ## Installation To install
+the package, simply run the following command: ```bash pip install WrenchCL ```
+# User Guides Sure! Here's an updated and more detailed README that provides
+extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
 `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and
 `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and
 other utility tools. ### Connecting to AWS Services To interact with AWS RDS
 and S3 services, follow these steps: 1. **Setup `AWSClientHub`**: ```python
-from WrenchCL.Connections import AWSClientHub # Initialize the AWSClientHub
+from WrenchCL.Connections import AwsClientHub # Initialize the AWSClientHub
 using an env file or keyword arguments aws_client_hub = AWSClientHub
 (env_path="path/to/your/env/file") # Alternatively, use keyword arguments or
 existing env variables # aws_client_hub = AWSClientHub
 (aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
@@ -57,42 +57,43 @@
 another. - `rename_object(bucket_name: str, src_object_key: str,
 dst_object_key: str) -> None` - Renames an object in S3. -
 `check_object_existence(bucket_name: str, object_key: str) -> bool` - Checks if
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
-**Setup `OpenAIGateway`**: ```python from WrenchCL.Models import OpenAIGateway
-# Initialize OpenAIGateway with your OpenAI API key openai_gateway =
-OpenAIGateway(api_key="your_openai_api_key") # Example: Generating text
-response = openai_gateway.handle_text("Your prompt here") print(response) ```
-**Methods in `OpenAIGateway`**: - `handle_text(text: str, model: str = "gpt-
-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] =
-None, json_mode: bool = False, **kwargs) -> Union[str, dict]` - Processes text
-input using the specified model and returns the response. - `get_embeddings
-(text: str, model: str = "text-embedding-3-small") -> list` - Retrieves
-embeddings for the given text using the specified model. - `generate_image
-(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -
-> str` - Generates an image based on the provided prompt. - `process_audio
-(audio_path: str, model: str = "whisper-1") -> str` - Processes an audio file
-and returns its transcription. - `create_image_variation(image_path: str, n:
-int = 1, size: str = "1024x1024") -> str` - Creates variations of an image
-based on the provided image path. - `edit_image(image_path: str, prompt: str,
-mask_path: str, n: int = 1, size: str = "1024x1024") -> str` - Edits an image
-based on the provided prompt and mask. - `vision_query(question: str,
-image_path: str, **kwargs) -> dict` - Processes a vision query based on the
-provided question and image. - `convert_image_to_url_or_base64(image_path: str)
--> str` - Converts an image to a URL or base64 encoded string. -
-`initiate_conversation(initial_text: str, **kwargs)` - Initiates a conversation
-using the provided initial text. 2. **Using `OpenAIFactory`**: ```python from
-WrenchCL.Models import OpenAIFactory # Initialize OpenAIFactory with your
-OpenAI API key openai_factory = OpenAIFactory(api_key="your_openai_api_key") #
-Example: Transcribing audio to text and getting embeddings audio_path = "path/
-to/your/audio/file" embeddings = openai_factory.audio_to_text_to_embeddings
-(audio_path) print(embeddings) ``` **Methods in `OpenAIFactory`**: -
+**Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
+OpenAIGateway # Initialize OpenAIGateway with your OpenAI API key
+openai_gateway = OpenAIGateway(api_key="your_openai_api_key") # Example:
+Generating text response = openai_gateway.handle_text("Your prompt here") print
+(response) ``` **Methods in `OpenAIGateway`**: - `handle_text(text: str, model:
+str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional
+[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]` -
+Processes text input using the specified model and returns the response. -
+`get_embeddings(text: str, model: str = "text-embedding-3-small") -> list` -
+Retrieves embeddings for the given text using the specified model. -
+`generate_image(prompt: str, size: str = "1024x1024", quality: str =
+"standard", n: int = 1) -> str` - Generates an image based on the provided
+prompt. - `process_audio(audio_path: str, model: str = "whisper-1") -> str` -
+Processes an audio file and returns its transcription. -
+`create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -
+> str` - Creates variations of an image based on the provided image path. -
+`edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str
+= "1024x1024") -> str` - Edits an image based on the provided prompt and mask.
+- `vision_query(question: str, image_path: str, **kwargs) -> dict` - Processes
+a vision query based on the provided question and image. -
+`convert_image_to_url_or_base64(image_path: str) -> str` - Converts an image to
+a URL or base64 encoded string. - `initiate_conversation(initial_text: str,
+**kwargs)` - Initiates a conversation using the provided initial text. 2.
+**Using `OpenAIFactory`**: ```python from WrenchCL.Models.OpenAI import
+OpenAIFactory # Initialize OpenAIFactory with your OpenAI API key
+openai_factory = OpenAIFactory(api_key="your_openai_api_key") # Example:
+Transcribing audio to text and getting embeddings audio_path = "path/to/your/
+audio/file" embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
+print(embeddings) ``` **Methods in `OpenAIFactory`**: -
 `audio_to_text_to_embeddings(audio_path: str, embedding_model: str = "text-
 embedding-3-small") -> list` - Transcribes audio to text and then generates
 embeddings for the text. - `image_to_text_to_embeddings(image_path: str,
 question: str, embedding_model: str = "text-embedding-3-small") -> list` -
 Performs a vision query to understand an image and then generates embeddings
 for the response. - `validate_response_with_gpt(initial_response: str,
 validation_prompt: str) -> str` - Uses an initial response and validates or
@@ -174,30 +175,30 @@
 return "Success" result = might_fail() print(result) ``` - **SingletonClass**:
 Ensures a class only has one instance. ```python from WrenchCL.Decorators
 import SingletonClass @SingletonClass class MySingleton: def __init__(self):
 self.value = 42 instance1 = MySingleton() instance2 = MySingleton() print
 (instance1 is instance2) # Output: True ``` - **TimedMethod**: Logs the time
 taken to execute a method. ```python from WrenchCL.Decorators import
 TimedMethod @TimedMethod def slow_function(): time.sleep(2) return "Done"
-result = slow_function() print(result) # Output: "Done" ``` ### Helpers
+result = slow_function() print(result) # Output: "Done" ``` ### DataFlow
 WrenchCL includes various helper functions to assist with common tasks. These
-helpers are located in the `Helpers` module. #### build_return_json Constructs
+helpers are located in the `DataFlow` module. #### build_return_json Constructs
 a JSON response with a given status code and message. ```python from
-WrenchCL.Helpers import build_return_json response = build_return_json
+WrenchCL.DataFlow import build_return_json response = build_return_json
 (code=200, message="Success") print(response) # Output: {'statusCode': 200,
 'body': '{"message": "Success"}'} ``` #### handle_lambda_response Handles
 Lambda function responses, including logging and error handling. It stops the
 Lambda function execution and returns a specified response when a
 `GuardedResponseTrigger` exception is raised. This is particularly useful for
 ensuring that the Lambda function exits immediately and returns the correct
 response, even if the exception occurs deep within nested function calls.
 Hereâs a comprehensive example demonstrating how to use
 `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and
 propagate responses up the call hierarchy in an AWS Lambda function. ```python
-import time from WrenchCL import wrench_logger from WrenchCL.Helpers import
+import time from WrenchCL import wrench_logger from WrenchCL.DataFlow import
 build_return_json, handle_lambda_response, GuardedResponseTrigger # Mock
 implementation of LambdaCore for the example class LambdaCore: def __init__
 (self, event, context): self.event = event self.context = context def route
 (self): # Example of nested function call where an error might occur
 self.process_request() def process_request(self): try: # Perform some
 processing self.get_score({"key": "value"}, {"input_key": "input_value"})
 except Exception as e: # Handle other exceptions and wrap them into the
@@ -242,21 +243,21 @@
 that when an error is encountered deep in the call hierarchy, the Lambda
 function stops execution and returns a response immediately. This response is
 propagated back up through the nested calls to the top-level Lambda handler. By
 using `GuardedResponseTrigger` and `handle_lambda_response`, you can manage
 errors effectively and ensure that your Lambda function returns the correct
 response even when an error occurs deep within nested function calls. ####
 trigger_minimum_dataflow_metrics Triggers minimal data flow metrics for
-monitoring purposes. ```python from WrenchCL.Helpers import
+monitoring purposes. ```python from WrenchCL.DataFlow import
 trigger_minimum_dataflow_metrics trigger_minimum_dataflow_metrics
-( event="event_data", context="context_data", start_time=1625256000,
+(event="event_data", context="context_data", start_time=1625256000,
 lambda_client="lambda_client_instance", job_name="Model Inference Service",
-job_type="Lambda", status_code="200", message="Success" ) ``` ####
+job_type="Lambda", status_code="200", message="Success") ``` ####
 trigger_dataflow_metrics Triggers detailed data flow metrics for monitoring
-purposes. ```python from WrenchCL.Helpers import trigger_dataflow_metrics
-trigger_dataflow_metrics( event="event_data", context="context_data",
+purposes. ```python from WrenchCL.DataFlow import trigger_dataflow_metrics
+trigger_dataflow_metrics(event="event_data", context="context_data",
 start_time=1625256000, lambda_client="lambda_client_instance", job_name="Model
 Inference Service", job_type="Lambda", status_code="200", message="Success",
-additional_data={"key": "value"} ) ``` With these detailed instructions and
+additional_data={"key": "value"}) ``` With these detailed instructions and
 examples, you should be well-equipped to utilize the WrenchCL library for your
 projects. If you have any further questions or need additional support, please
 refer to the documentation or contact the maintainers.
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Classes/_ConfigurationManager.py` & `WrenchCL-2.1.0/WrenchCL/_Internal/_ConfigurationManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 
 
 import os
 from pathlib import Path
 from dotenv import load_dotenv
 
-from Tools.WrenchLogger import logger
+from ..Tools.WrenchLogger import logger
 
 
 class _ConfigurationManager:
     """
     Manages the configuration settings for the application, including AWS and OpenAI credentials, SSH details,
     and database batch size. Configurations can be initialized from environment files, environment variables,
     or keyword arguments.
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Classes/_SshTunnelManager.py` & `WrenchCL-2.1.0/WrenchCL/_Internal/_SshTunnelManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
-from Tools.WrenchLogger import logger
+from ..Tools.WrenchLogger import logger
 from sshtunnel import SSHTunnelForwarder
 
 class _SshTunnelManager:
     """
     Manages the SSH tunnel for securely connecting to a remote database server. This class uses the SSHTunnelForwarder
     to establish and manage the SSH tunnel.
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Connect/AWSClientHub.py` & `WrenchCL-2.1.0/WrenchCL/Connect/AwsClientHub.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 
 import json
 import psycopg2
 import boto3
-from Classes._ConfigurationManager import _ConfigurationManager
-from Classes._SshTunnelManager import _SshTunnelManager
-from Decorators.SingletonClass import SingletonClass
-from Tools.WrenchLogger import logger
-from Tools.Coalesce import coalesce
+from .._Internal._ConfigurationManager import _ConfigurationManager
+from .._Internal._SshTunnelManager import _SshTunnelManager
+from ..Decorators.SingletonClass import SingletonClass
+from ..Tools.WrenchLogger import logger
+from ..Tools.Coalesce import coalesce
 from mypy_boto3_s3.client import S3Client
 from mypy_boto3_rds.client import RDSClient
 
 
 @SingletonClass
 class AwsClientHub:
     """
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Connect/RdsServiceGateway.py` & `WrenchCL-2.1.0/WrenchCL/Connect/RdsServiceGateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,25 @@
 import collections
 import math
 from typing import Optional, Type, Any, Union, List, Tuple
 
 import psycopg2
 import psycopg2.extras
 
-from Connect import AwsClientHub
-from Decorators.SingletonClass import SingletonClass
-from Tools.Coalesce import coalesce
-from Tools.WrenchLogger import logger
+from .AwsClientHub import AwsClientHub
+from ..Decorators.SingletonClass import SingletonClass
+from ..Tools.Coalesce import coalesce
+from ..Tools.WrenchLogger import logger
 
 try:
     import pandas as pd
     PANDAS_AVAILABLE = True
 except ImportError:
     PANDAS_AVAILABLE = False
 
-
 @SingletonClass
 class RdsServiceGateway:
     """
     Provides methods to interact with an RDS database, including querying data and updating the database. Ensures
     that a single instance is used throughout the application via the Singleton pattern.
 
     Attributes:
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Connect/S3ServiceGateway.py` & `WrenchCL-2.1.0/WrenchCL/Connect/S3ServiceGateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 # 
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 # 
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 import io
-
 from botocore.exceptions import ClientError
 
-from Decorators.Retryable import Retryable
-from Decorators.SingletonClass import SingletonClass
-from Tools.WrenchLogger import logger
-from Connect.AWSClientHub import AwsClientHub
+from ..Decorators.Retryable import Retryable
+from ..Decorators.SingletonClass import SingletonClass
+from ..Tools.WrenchLogger import logger
+from .AwsClientHub import AwsClientHub
+
 
 @SingletonClass
 class S3ServiceGateway:
     """
     Provides methods to interact with AWS S3, including uploading, downloading, moving, and deleting objects. Ensures
     that a single instance is used throughout the application via the Singleton pattern.
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Decorators/Retryable.py` & `WrenchCL-2.1.0/WrenchCL/Decorators/Retryable.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 from botocore.exceptions import ClientError, BotoCoreError
 
-from Tools.WrenchLogger import logger
+from ..Tools.WrenchLogger import logger
 
 def Retryable(retry_on_exceptions=(ClientError, BotoCoreError), max_retries=3, delay=2):
     """
     Decorator to retry function calls based on specified exceptions. If the function raises any of the specified
     exceptions, it will be retried up to `max_retries` times with a delay between retries.
 
     :param retry_on_exceptions: A tuple of exceptions that should trigger a retry.
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Decorators/SingletonClass.py` & `WrenchCL-2.1.0/WrenchCL/Decorators/SingletonClass.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/WrenchCL/Decorators/TimedMethod.py` & `WrenchCL-2.1.0/WrenchCL/Decorators/TimedMethod.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 import time
 
-from Tools.WrenchLogger import logger
+from ..Tools.WrenchLogger import logger
 
 def TimedMethod(func):
     """
     Decorator that logs the execution time of the decorated function. This can be useful for monitoring performance
     and identifying bottlenecks in the code.
 
     :param func: The function to be decorated.
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Helpers/build_return_json.py` & `WrenchCL-2.1.0/WrenchCL/DataFlow/build_return_json.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/WrenchCL/Helpers/handle_lambda_response.py` & `WrenchCL-2.1.0/WrenchCL/DataFlow/handle_lambda_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 from boto3 import client as boto3client
 
-from Tools.DictValidator import validate_input_dict
-from Tools.WrenchLogger import logger
+from ..Tools.DictValidator import validate_input_dict
+from ..Tools.WrenchLogger import logger
 from .build_return_json import build_return_json
 from .trigger_dataflow_metrics import trigger_minimum_dataflow_metrics
 
 lambda_response = None
 
 class GuardedResponseTrigger(Exception):
     """Custom exception to signal early exit from the Lambda function."""
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Helpers/trigger_dataflow_metrics.py` & `WrenchCL-2.1.0/WrenchCL/DataFlow/trigger_dataflow_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #
 
 
 import time
 import json
 import uuid
 from typing import Any, Dict
-from Tools.WrenchLogger import logger
+from ..Tools.WrenchLogger import logger
 
 # Created by Jeong Kim
 # Github: https://github.com/dalmad2
 # Annotated by Willem van der Schans
 # Github: https://github.com/Kydoimos97
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Models/OpenAIFactory.py` & `WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIFactory.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,28 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
-from Decorators.TimedMethod import TimedMethod
-from Models.OpenAIGateway import OpenAIGateway
+#
+#  MIT License
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+#
+#
+#
+#  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
+#
+#  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
+#
+
+from ...Decorators.TimedMethod import TimedMethod
+from .OpenAIGateway import OpenAIGateway
 
 
 class OpenAIFactory(OpenAIGateway):
     """
     A factory class that extends OpenAIGateway to provide additional methods for processing audio, images, and text,
     and generating embeddings using OpenAI's models.
     """
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Models/OpenAIGateway.py` & `WrenchCL-2.1.0/WrenchCL/Models/OpenAI/OpenAIGateway.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,22 +9,34 @@
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
+#
+#  MIT License
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+#
+#
+#
+#  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
+#
+#  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
+#
+
 import json
 import base64
 import os
 from openai import OpenAI
 
-from Decorators.TimedMethod import TimedMethod
-from Models._ConversationManager import ConversationManager
-from Tools.WrenchLogger import logger
+from ...Decorators.TimedMethod import TimedMethod
+from ._ConversationManager import ConversationManager
+from ...Tools.WrenchLogger import logger
 
 
 class OpenAIGateway:
     """
     A gateway class to interact with OpenAI's API, providing methods to handle text, image, and audio processing.
     """
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Models/_ConversationManager.py` & `WrenchCL-2.1.0/WrenchCL/Models/OpenAI/_ConversationManager.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,22 +8,34 @@
 #
 #  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
+
+#
+#  MIT License
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+#
+#
+#
+#  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
+#
+#  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
+#
 try:
     from colorama import Fore, Style
     COLORAMA_AVAILABLE = True
 except ImportError:
     COLORAMA_AVAILABLE = False
 
 from openai import AssistantEventHandler, OpenAI
-from Tools.WrenchLogger import logger
+from ...Tools.WrenchLogger import logger
 
 
 class EventHandler(AssistantEventHandler):
     """
     Custom event handler for OpenAI Assistant that handles text and tool call events, printing them with colored output.
     """
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Tools/Coalesce.py` & `WrenchCL-2.1.0/WrenchCL/Tools/Coalesce.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/WrenchCL/Tools/DictValidator.py` & `WrenchCL-2.1.0/WrenchCL/Tools/DictValidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 #
 #  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
 #
 #  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
 #
 
 from typing import Any, Dict, Type, Literal
-from Tools.WrenchLogger import logger
+from .WrenchLogger import logger
 
 
 def validate_input_dict(
     params: Dict[str, Any],
     expected_types: Dict[str, Type],
     errors: Literal['raise', 'coerce'] = 'raise'
 ) -> None:
```

### Comparing `WrenchCL-2.0.0/WrenchCL/Tools/FetchMetaData.py` & `WrenchCL-2.1.0/WrenchCL/Tools/FetchMetaData.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/WrenchCL/Tools/FileTyper.py` & `WrenchCL-2.1.0/WrenchCL/Tools/FileTyper.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/WrenchCL/Tools/Image2B64.py` & `WrenchCL-2.1.0/WrenchCL/Tools/Image2B64.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/WrenchCL/Tools/MaybeMonad.py` & `WrenchCL-2.1.0/WrenchCL/Tools/MaybeMonad.py`

 * *Files identical despite different names*

### Comparing `WrenchCL-2.0.0/WrenchCL/Tools/WrenchLogger.py` & `WrenchCL-2.1.0/WrenchCL/Tools/WrenchLogger.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,25 +21,68 @@
 import sys
 import time
 import traceback
 from datetime import datetime, timedelta
 from textwrap import fill
 from typing import Any, Optional
 
-from Decorators.SingletonClass import SingletonClass
-
 try:
     from colorama import init, Fore as ColoramaFore, Style as ColoramaStyle
 
     colorama_imported = True
 except ImportError:
     colorama_imported = False
     logging.warning("colorama package not found. Colored logging is disabled.")
 
-@SingletonClass
+
+def LoggerSingleton(cls):
+    """
+    Decorator for a class to implement the Singleton pattern. This decorator ensures that only one instance of the
+    decorated class can exist at any time. If an instance of the class already exists, it returns that instance;
+    otherwise, it creates and returns a new instance.
+
+    The Singleton pattern is particularly useful when exactly one object is needed to coordinate actions across the
+    system, such as in the case of managing database connections.
+
+    :param cls: The class to be decorated as a Singleton.
+    :type cls: type
+    :returns: A wrapper function that manages the instantiation of the singleton class, ensuring that only one
+              instance exists.
+    :rtype: function
+
+    **Example**::
+
+        >>> @SingletonClass
+        ... class DatabaseManager:
+        ...     def __init__(self, connection_string):
+        ...         self.connection_string = connection_string
+        ...
+        >>> db_manager1 = DatabaseManager('db_connection_string')
+        >>> db_manager2 = DatabaseManager('db_connection_string')
+        >>> assert db_manager1 is db_manager2  # Both variables point to the same instance
+    """
+    instances = {}
+
+    def get_instance(*args, **kwargs):
+        """
+        Returns the singleton instance of the class, creating it if it does not already exist.
+
+        :param args: Positional arguments for the class constructor.
+        :param kwargs: Keyword arguments for the class constructor.
+        :returns: The singleton instance of the class.
+        """
+        if cls not in instances:
+            instances[cls] = cls(*args, **kwargs)
+        return instances[cls]
+
+    return get_instance
+
+
+
+@LoggerSingleton
 class _wrench_logger:
 
     def __init__(self, level: str = 'INFO', file_logging=False, file_name_append_mode: Optional[str] = None) -> None:
         self._start_time = None
         self.run_id = self._generate_run_id()
         self.running_on_lambda = 'AWS_LAMBDA_FUNCTION_NAME' in os.environ
         self.previous_level = None
```

### Comparing `WrenchCL-2.0.0/WrenchCL.egg-info/PKG-INFO` & `WrenchCL-2.1.0/WrenchCL.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: WrenchCL
-Version: 2.0.0
+Version: 2.1.0
 Summary: WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 Home-page: https://github.com/WrenchAI/WrenchCL
 Author: willem@wrench.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <h1 align="center">Wrench Code Library</h1>
 
 <p align="center">
-    <img src="resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
+    <img src="https://raw.githubusercontent.com/WrenchAI/WrenchCL/release/resources/img/logo.svg" alt="Logo" style="display: inline-block; vertical-align: middle; margin-bottom: -50px; width: 90%; max-width: 800px;">
     <a href="https://pypi.org/project/WrenchCL/" style="text-decoration: none;">
         <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/WrenchCL?logo=pypi&logoColor=green&color=green">
     </a>
     <a href="https://github.com/Kydoimos97" style="text-decoration: none;">
         <img src="https://img.shields.io/badge/Kydoimos97-cb632b?label=Code%20Maintainer" alt="Maintainer" height="20"/>
     </a>
     <a href="https://github.com/WrenchAI/WrenchCL/actions/workflows/publish-to-pypi.yml" style="text-decoration: none;">
@@ -30,20 +30,20 @@
 
 WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.
 
 **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/WrenchCL/)
 
 ## Package Structure
 
-- **Classes**: Contains internal classes for configuration and SSH tunnel management.
+- **_Internal**: Contains internal classes for configuration and SSH tunnel management.
 - **Connect**: Provides gateways for AWS RDS and S3 services and the `AWSClientHub`.
 - **Decorators**: Utility decorators for retry logic, singleton pattern, and method timing.
-- **Models**: Classes for interacting with OpenAI models.
+- **Models**: _Internal for interacting with OpenAI models.
 - **Tools**: Miscellaneous utility tools such as coalescing values, file typing, image encoding, and a custom logger.
-- **Helpers**: Response focused tools to aid in returning values and generating logs based on status codes.
+- **DataFlow**: Response focused tools to aid in returning values and generating logs based on status codes.
 ## Installation
 
 To install the package, simply run the following command:
 
 ```bash
 pip install WrenchCL
 ```
@@ -54,15 +54,15 @@
 
 ### Connecting to AWS Services
 
 To interact with AWS RDS and S3 services, follow these steps:
 
 1. **Setup `AWSClientHub`**:
    ```python
-   from WrenchCL.Connections import AWSClientHub
+   from WrenchCL.Connections import AwsClientHub
 
    # Initialize the AWSClientHub using an env file or keyword arguments
    aws_client_hub = AWSClientHub(env_path="path/to/your/env/file")
    # Alternatively, use keyword arguments or existing env variables
    # aws_client_hub = AWSClientHub(aws_profile='your_profile', region_name='your_region', secret_arn='your_secret_arn', ...)
    ```
 
@@ -124,15 +124,15 @@
 
 ### Interacting with OpenAI Models
 
 To use OpenAI models, follow these steps:
 
 1. **Setup `OpenAIGateway`**:
    ```python
-   from WrenchCL.Models import OpenAIGateway
+   from WrenchCL.Models.OpenAI import OpenAIGateway
 
    # Initialize OpenAIGateway with your OpenAI API key
    openai_gateway = OpenAIGateway(api_key="your_openai_api_key")
 
    # Example: Generating text
    response = openai_gateway.handle_text("Your prompt here")
    print(response)
@@ -156,15 +156,15 @@
    - `convert_image_to_url_or_base64(image_path: str) -> str`
      - Converts an image to a URL or base64 encoded string.
    - `initiate_conversation(initial_text: str, **kwargs)`
      - Initiates a conversation using the provided initial text.
 
 2. **Using `OpenAIFactory`**:
    ```python
-   from WrenchCL.Models import OpenAIFactory
+   from WrenchCL.Models.OpenAI import OpenAIFactory
 
    # Initialize OpenAIFactory with your OpenAI API key
    openai_factory = OpenAIFactory(api_key="your_openai_api_key")
 
    # Example: Transcribing audio to text and getting embeddings
    audio_path = "path/to/your/audio/file"
    embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
@@ -369,39 +369,40 @@
       time.sleep(2)
       return "Done"
 
   result = slow_function()
   print(result)  # Output: "Done"
   ```
 
-### Helpers
+### DataFlow
 
-WrenchCL includes various helper functions to assist with common tasks. These helpers are located in the `Helpers` module.
+WrenchCL includes various helper functions to assist with common tasks. These helpers are located in the `DataFlow` module.
 
 #### build_return_json
 
 Constructs a JSON response with a given status code and message.
 
 ```python
-from WrenchCL.Helpers import build_return_json
+from WrenchCL.DataFlow import build_return_json
 
 response = build_return_json(code=200, message="Success")
 print(response)  # Output: {'statusCode': 200, 'body': '{"message": "Success"}'}
 ```
 
 #### handle_lambda_response
 
 Handles Lambda function responses, including logging and error handling. It stops the Lambda function execution and returns a specified response when a `GuardedResponseTrigger` exception is raised. This is particularly useful for ensuring that the Lambda function exits immediately and returns the correct response, even if the exception occurs deep within nested function calls.
 
 Here’s a comprehensive example demonstrating how to use `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and propagate responses up the call hierarchy in an AWS Lambda function.
 
 ```python
 import time
 from WrenchCL import wrench_logger
-from WrenchCL.Helpers import build_return_json, handle_lambda_response, GuardedResponseTrigger
+from WrenchCL.DataFlow import build_return_json, handle_lambda_response, GuardedResponseTrigger
+
 
 # Mock implementation of LambdaCore for the example
 class LambdaCore:
     def __init__(self, event, context):
         self.event = event
         self.context = context
 
@@ -411,42 +412,50 @@
 
     def process_request(self):
         try:
             # Perform some processing
             self.get_score({"key": "value"}, {"input_key": "input_value"})
         except Exception as e:
             # Handle other exceptions and wrap them into the GuardedResponseTrigger
-            handle_lambda_response(500, str(e), {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
-    
+            handle_lambda_response(500, str(e),
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
+
     def get_score(self, target_dict, input_dict):
         # Mock scoring process which might throw an error
         try:
             score = self.compute_score(target_dict, input_dict)
             if score is None:
-                handle_lambda_response(732, "Prediction Error: Invalid prediction provided by model.", {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
-            handle_lambda_response(200, f"Score computed successfully: {score}", {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
+                handle_lambda_response(732, "Prediction Error: Invalid prediction provided by model.",
+                                       {"event": self.event, "context": self.context, "start_time": time.time(),
+                                        "lambda_client": "lambda_client_instance"})
+            handle_lambda_response(200, f"Score computed successfully: {score}",
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
         except GuardedResponseTrigger as e:
             raise e  # Propagate the GuardedResponseTrigger upwards
         except Exception as e:
-            handle_lambda_response(757, str(e), {"event": self.event, "context": self.context, "start_time": time.time(), "lambda_client": "lambda_client_instance"})
+            handle_lambda_response(757, str(e),
+                                   {"event": self.event, "context": self.context, "start_time": time.time(),
+                                    "lambda_client": "lambda_client_instance"})
 
     def compute_score(self, target_dict, input_dict):
         # This is a placeholder for the actual scoring logic
         # Raise an error to simulate a failure
         raise ValueError("Simulated scoring error")
 
 
 def lambda_handler(event, context):
     wrench_logger.initiate_new_run()
 
     if event.get('is_warmer'):
         wrench_logger.run_id = 'R-LAMBDAS-WARM'
         wrench_logger.context("Lambda Warmed")
         return build_return_json(200, 'Warmed Lambda')
-    
+
     start_time = time.time()
     try:
         wrench_logger.info("Invoking Lambda Core")
         lambda_core_instance = LambdaCore(event=event, context=context)
         lambda_core_instance.route()
         wrench_logger.info(f"Finished Run in {round(time.time() - start_time, 2)} seconds")
     except GuardedResponseTrigger as e:
@@ -476,42 +485,27 @@
 By using `GuardedResponseTrigger` and `handle_lambda_response`, you can manage errors effectively and ensure that your Lambda function returns the correct response even when an error occurs deep within nested function calls.
 
 #### trigger_minimum_dataflow_metrics
 
 Triggers minimal data flow metrics for monitoring purposes.
 
 ```python
-from WrenchCL.Helpers import trigger_minimum_dataflow_metrics
+from WrenchCL.DataFlow import trigger_minimum_dataflow_metrics
 
-trigger_minimum_dataflow_metrics(
-    event="event_data",
-    context="context_data",
-    start_time=1625256000,
-    lambda_client="lambda_client_instance",
-    job_name="Model Inference Service",
-    job_type="Lambda",
-    status_code="200",
-    message="Success"
-)
+trigger_minimum_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
+    lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
+    message="Success")
 ```
 
 #### trigger_dataflow_metrics
 
 Triggers detailed data flow metrics for monitoring purposes.
 
 ```python
-from WrenchCL.Helpers import trigger_dataflow_metrics
+from WrenchCL.DataFlow import trigger_dataflow_metrics
 
-trigger_dataflow_metrics(
-    event="event_data",
-    context="context_data",
-    start_time=1625256000,
-    lambda_client="lambda_client_instance",
-    job_name="Model Inference Service",
-    job_type="Lambda",
-    status_code="200",
-    message="Success",
-    additional_data={"key": "value"}
-)
+trigger_dataflow_metrics(event="event_data", context="context_data", start_time=1625256000,
+    lambda_client="lambda_client_instance", job_name="Model Inference Service", job_type="Lambda", status_code="200",
+    message="Success", additional_data={"key": "value"})
 ```
 
 With these detailed instructions and examples, you should be well-equipped to utilize the WrenchCL library for your projects. If you have any further questions or need additional support, please refer to the documentation or contact the maintainers.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: WrenchCL Version: 2.0.0 Summary: WrenchCL is a
+Metadata-Version: 2.1 Name: WrenchCL Version: 2.1.0 Summary: WrenchCL is a
 comprehensive library designed to facilitate seamless interactions with AWS
 services, OpenAI models, and various utility tools. This package aims to
 streamline the development process by providing robust components for database
 interactions, cloud storage, and AI-powered functionalities. Home-page: https:/
 /github.com/WrenchAI/WrenchCL Author: willem@wrench.ai Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
@@ -10,30 +10,30 @@
                        ************ WWrreenncchh CCooddee LLiibbrraarryy ************
     [Logo]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_M_a_i_n_t_a_i_n_e_r_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_ _(_w_i_t_h_ _e_v_e_n_t_)_]
 ## Description WrenchCL is a comprehensive library designed to facilitate
 seamless interactions with AWS services, OpenAI models, and various utility
 tools. This package aims to streamline the development process by providing
 robust components for database interactions, cloud storage, and AI-powered
 functionalities. **PyPI Link:** [WrenchCL on PyPI](https://pypi.org/project/
-WrenchCL/) ## Package Structure - **Classes**: Contains internal classes for
+WrenchCL/) ## Package Structure - **_Internal**: Contains internal classes for
 configuration and SSH tunnel management. - **Connect**: Provides gateways for
 AWS RDS and S3 services and the `AWSClientHub`. - **Decorators**: Utility
 decorators for retry logic, singleton pattern, and method timing. - **Models**:
-Classes for interacting with OpenAI models. - **Tools**: Miscellaneous utility
-tools such as coalescing values, file typing, image encoding, and a custom
-logger. - **Helpers**: Response focused tools to aid in returning values and
-generating logs based on status codes. ## Installation To install the package,
-simply run the following command: ```bash pip install WrenchCL ``` # User
-Guides Sure! Here's an updated and more detailed README that provides extensive
-instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
+_Internal for interacting with OpenAI models. - **Tools**: Miscellaneous
+utility tools such as coalescing values, file typing, image encoding, and a
+custom logger. - **DataFlow**: Response focused tools to aid in returning
+values and generating logs based on status codes. ## Installation To install
+the package, simply run the following command: ```bash pip install WrenchCL ```
+# User Guides Sure! Here's an updated and more detailed README that provides
+extensive instructions on how to use `AWSClientHub`, `RdsServiceGateway`,
 `S3ServiceGateway`, `ConversationManager`, `OpenAIFactory`, and
 `OpenAIGateway`. It also includes practical examples for the `Maybe` monad and
 other utility tools. ### Connecting to AWS Services To interact with AWS RDS
 and S3 services, follow these steps: 1. **Setup `AWSClientHub`**: ```python
-from WrenchCL.Connections import AWSClientHub # Initialize the AWSClientHub
+from WrenchCL.Connections import AwsClientHub # Initialize the AWSClientHub
 using an env file or keyword arguments aws_client_hub = AWSClientHub
 (env_path="path/to/your/env/file") # Alternatively, use keyword arguments or
 existing env variables # aws_client_hub = AWSClientHub
 (aws_profile='your_profile', region_name='your_region',
 secret_arn='your_secret_arn', ...) ``` 2. **Using `RdsServiceGateway`**:
 ```python from WrenchCL.Connections import RdsServiceGateway # Initialize
 RdsServiceGateway with the AWSClientHub instance rds_service =
@@ -66,42 +66,43 @@
 another. - `rename_object(bucket_name: str, src_object_key: str,
 dst_object_key: str) -> None` - Renames an object in S3. -
 `check_object_existence(bucket_name: str, object_key: str) -> bool` - Checks if
 an object exists in S3. - `list_objects(bucket_name: str, prefix: Optional[str]
 = None) -> list` - Lists objects in an S3 bucket. - `check_bucket_permissions
 (bucket_name: str) -> dict` - Checks the permissions of an S3 bucket. ###
 Interacting with OpenAI Models To use OpenAI models, follow these steps: 1.
-**Setup `OpenAIGateway`**: ```python from WrenchCL.Models import OpenAIGateway
-# Initialize OpenAIGateway with your OpenAI API key openai_gateway =
-OpenAIGateway(api_key="your_openai_api_key") # Example: Generating text
-response = openai_gateway.handle_text("Your prompt here") print(response) ```
-**Methods in `OpenAIGateway`**: - `handle_text(text: str, model: str = "gpt-
-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional[str] =
-None, json_mode: bool = False, **kwargs) -> Union[str, dict]` - Processes text
-input using the specified model and returns the response. - `get_embeddings
-(text: str, model: str = "text-embedding-3-small") -> list` - Retrieves
-embeddings for the given text using the specified model. - `generate_image
-(prompt: str, size: str = "1024x1024", quality: str = "standard", n: int = 1) -
-> str` - Generates an image based on the provided prompt. - `process_audio
-(audio_path: str, model: str = "whisper-1") -> str` - Processes an audio file
-and returns its transcription. - `create_image_variation(image_path: str, n:
-int = 1, size: str = "1024x1024") -> str` - Creates variations of an image
-based on the provided image path. - `edit_image(image_path: str, prompt: str,
-mask_path: str, n: int = 1, size: str = "1024x1024") -> str` - Edits an image
-based on the provided prompt and mask. - `vision_query(question: str,
-image_path: str, **kwargs) -> dict` - Processes a vision query based on the
-provided question and image. - `convert_image_to_url_or_base64(image_path: str)
--> str` - Converts an image to a URL or base64 encoded string. -
-`initiate_conversation(initial_text: str, **kwargs)` - Initiates a conversation
-using the provided initial text. 2. **Using `OpenAIFactory`**: ```python from
-WrenchCL.Models import OpenAIFactory # Initialize OpenAIFactory with your
-OpenAI API key openai_factory = OpenAIFactory(api_key="your_openai_api_key") #
-Example: Transcribing audio to text and getting embeddings audio_path = "path/
-to/your/audio/file" embeddings = openai_factory.audio_to_text_to_embeddings
-(audio_path) print(embeddings) ``` **Methods in `OpenAIFactory`**: -
+**Setup `OpenAIGateway`**: ```python from WrenchCL.Models.OpenAI import
+OpenAIGateway # Initialize OpenAIGateway with your OpenAI API key
+openai_gateway = OpenAIGateway(api_key="your_openai_api_key") # Example:
+Generating text response = openai_gateway.handle_text("Your prompt here") print
+(response) ``` **Methods in `OpenAIGateway`**: - `handle_text(text: str, model:
+str = "gpt-3.5-turbo", system_prompt: Optional[str] = None, image_url: Optional
+[str] = None, json_mode: bool = False, **kwargs) -> Union[str, dict]` -
+Processes text input using the specified model and returns the response. -
+`get_embeddings(text: str, model: str = "text-embedding-3-small") -> list` -
+Retrieves embeddings for the given text using the specified model. -
+`generate_image(prompt: str, size: str = "1024x1024", quality: str =
+"standard", n: int = 1) -> str` - Generates an image based on the provided
+prompt. - `process_audio(audio_path: str, model: str = "whisper-1") -> str` -
+Processes an audio file and returns its transcription. -
+`create_image_variation(image_path: str, n: int = 1, size: str = "1024x1024") -
+> str` - Creates variations of an image based on the provided image path. -
+`edit_image(image_path: str, prompt: str, mask_path: str, n: int = 1, size: str
+= "1024x1024") -> str` - Edits an image based on the provided prompt and mask.
+- `vision_query(question: str, image_path: str, **kwargs) -> dict` - Processes
+a vision query based on the provided question and image. -
+`convert_image_to_url_or_base64(image_path: str) -> str` - Converts an image to
+a URL or base64 encoded string. - `initiate_conversation(initial_text: str,
+**kwargs)` - Initiates a conversation using the provided initial text. 2.
+**Using `OpenAIFactory`**: ```python from WrenchCL.Models.OpenAI import
+OpenAIFactory # Initialize OpenAIFactory with your OpenAI API key
+openai_factory = OpenAIFactory(api_key="your_openai_api_key") # Example:
+Transcribing audio to text and getting embeddings audio_path = "path/to/your/
+audio/file" embeddings = openai_factory.audio_to_text_to_embeddings(audio_path)
+print(embeddings) ``` **Methods in `OpenAIFactory`**: -
 `audio_to_text_to_embeddings(audio_path: str, embedding_model: str = "text-
 embedding-3-small") -> list` - Transcribes audio to text and then generates
 embeddings for the text. - `image_to_text_to_embeddings(image_path: str,
 question: str, embedding_model: str = "text-embedding-3-small") -> list` -
 Performs a vision query to understand an image and then generates embeddings
 for the response. - `validate_response_with_gpt(initial_response: str,
 validation_prompt: str) -> str` - Uses an initial response and validates or
@@ -183,30 +184,30 @@
 return "Success" result = might_fail() print(result) ``` - **SingletonClass**:
 Ensures a class only has one instance. ```python from WrenchCL.Decorators
 import SingletonClass @SingletonClass class MySingleton: def __init__(self):
 self.value = 42 instance1 = MySingleton() instance2 = MySingleton() print
 (instance1 is instance2) # Output: True ``` - **TimedMethod**: Logs the time
 taken to execute a method. ```python from WrenchCL.Decorators import
 TimedMethod @TimedMethod def slow_function(): time.sleep(2) return "Done"
-result = slow_function() print(result) # Output: "Done" ``` ### Helpers
+result = slow_function() print(result) # Output: "Done" ``` ### DataFlow
 WrenchCL includes various helper functions to assist with common tasks. These
-helpers are located in the `Helpers` module. #### build_return_json Constructs
+helpers are located in the `DataFlow` module. #### build_return_json Constructs
 a JSON response with a given status code and message. ```python from
-WrenchCL.Helpers import build_return_json response = build_return_json
+WrenchCL.DataFlow import build_return_json response = build_return_json
 (code=200, message="Success") print(response) # Output: {'statusCode': 200,
 'body': '{"message": "Success"}'} ``` #### handle_lambda_response Handles
 Lambda function responses, including logging and error handling. It stops the
 Lambda function execution and returns a specified response when a
 `GuardedResponseTrigger` exception is raised. This is particularly useful for
 ensuring that the Lambda function exits immediately and returns the correct
 response, even if the exception occurs deep within nested function calls.
 Hereâs a comprehensive example demonstrating how to use
 `handle_lambda_response` and `GuardedResponseTrigger` to handle errors and
 propagate responses up the call hierarchy in an AWS Lambda function. ```python
-import time from WrenchCL import wrench_logger from WrenchCL.Helpers import
+import time from WrenchCL import wrench_logger from WrenchCL.DataFlow import
 build_return_json, handle_lambda_response, GuardedResponseTrigger # Mock
 implementation of LambdaCore for the example class LambdaCore: def __init__
 (self, event, context): self.event = event self.context = context def route
 (self): # Example of nested function call where an error might occur
 self.process_request() def process_request(self): try: # Perform some
 processing self.get_score({"key": "value"}, {"input_key": "input_value"})
 except Exception as e: # Handle other exceptions and wrap them into the
@@ -251,21 +252,21 @@
 that when an error is encountered deep in the call hierarchy, the Lambda
 function stops execution and returns a response immediately. This response is
 propagated back up through the nested calls to the top-level Lambda handler. By
 using `GuardedResponseTrigger` and `handle_lambda_response`, you can manage
 errors effectively and ensure that your Lambda function returns the correct
 response even when an error occurs deep within nested function calls. ####
 trigger_minimum_dataflow_metrics Triggers minimal data flow metrics for
-monitoring purposes. ```python from WrenchCL.Helpers import
+monitoring purposes. ```python from WrenchCL.DataFlow import
 trigger_minimum_dataflow_metrics trigger_minimum_dataflow_metrics
-( event="event_data", context="context_data", start_time=1625256000,
+(event="event_data", context="context_data", start_time=1625256000,
 lambda_client="lambda_client_instance", job_name="Model Inference Service",
-job_type="Lambda", status_code="200", message="Success" ) ``` ####
+job_type="Lambda", status_code="200", message="Success") ``` ####
 trigger_dataflow_metrics Triggers detailed data flow metrics for monitoring
-purposes. ```python from WrenchCL.Helpers import trigger_dataflow_metrics
-trigger_dataflow_metrics( event="event_data", context="context_data",
+purposes. ```python from WrenchCL.DataFlow import trigger_dataflow_metrics
+trigger_dataflow_metrics(event="event_data", context="context_data",
 start_time=1625256000, lambda_client="lambda_client_instance", job_name="Model
 Inference Service", job_type="Lambda", status_code="200", message="Success",
-additional_data={"key": "value"} ) ``` With these detailed instructions and
+additional_data={"key": "value"}) ``` With these detailed instructions and
 examples, you should be well-equipped to utilize the WrenchCL library for your
 projects. If you have any further questions or need additional support, please
 refer to the documentation or contact the maintainers.
```

### Comparing `WrenchCL-2.0.0/WrenchCL.egg-info/SOURCES.txt` & `WrenchCL-2.1.0/WrenchCL.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 setup.py
 WrenchCL/__init__.py
 WrenchCL.egg-info/PKG-INFO
 WrenchCL.egg-info/SOURCES.txt
 WrenchCL.egg-info/dependency_links.txt
 WrenchCL.egg-info/requires.txt
 WrenchCL.egg-info/top_level.txt
-WrenchCL/Classes/_ConfigurationManager.py
-WrenchCL/Classes/_SshTunnelManager.py
-WrenchCL/Classes/__init__.py
-WrenchCL/Connect/AWSClientHub.py
+WrenchCL/Connect/AwsClientHub.py
 WrenchCL/Connect/RdsServiceGateway.py
 WrenchCL/Connect/S3ServiceGateway.py
 WrenchCL/Connect/__init__.py
+WrenchCL/DataFlow/__init__.py
+WrenchCL/DataFlow/build_return_json.py
+WrenchCL/DataFlow/handle_lambda_response.py
+WrenchCL/DataFlow/trigger_dataflow_metrics.py
 WrenchCL/Decorators/Retryable.py
 WrenchCL/Decorators/SingletonClass.py
 WrenchCL/Decorators/TimedMethod.py
 WrenchCL/Decorators/__init__.py
-WrenchCL/Helpers/__init__.py
-WrenchCL/Helpers/build_return_json.py
-WrenchCL/Helpers/handle_lambda_response.py
-WrenchCL/Helpers/trigger_dataflow_metrics.py
-WrenchCL/Models/OpenAIFactory.py
-WrenchCL/Models/OpenAIGateway.py
-WrenchCL/Models/_ConversationManager.py
 WrenchCL/Models/__init__.py
+WrenchCL/Models/OpenAI/OpenAIFactory.py
+WrenchCL/Models/OpenAI/OpenAIGateway.py
+WrenchCL/Models/OpenAI/_ConversationManager.py
+WrenchCL/Models/OpenAI/__init__.py
 WrenchCL/Tools/Coalesce.py
 WrenchCL/Tools/DictValidator.py
 WrenchCL/Tools/FetchMetaData.py
 WrenchCL/Tools/FileTyper.py
 WrenchCL/Tools/Image2B64.py
 WrenchCL/Tools/MaybeMonad.py
 WrenchCL/Tools/WrenchLogger.py
-WrenchCL/Tools/__init__.py
+WrenchCL/Tools/__init__.py
+WrenchCL/_Internal/_ConfigurationManager.py
+WrenchCL/_Internal/_SshTunnelManager.py
+WrenchCL/_Internal/__init__.py
```

