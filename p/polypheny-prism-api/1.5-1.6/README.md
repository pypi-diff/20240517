# Comparing `tmp/polypheny-prism-api-1.5.tar.gz` & `tmp/polypheny-prism-api-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polypheny-prism-api-1.5.tar", last modified: Fri May 17 11:05:32 2024, max compression
+gzip compressed data, was "polypheny-prism-api-1.6.tar", last modified: Fri May 17 12:00:34 2024, max compression
```

## Comparing `polypheny-prism-api-1.5.tar` & `polypheny-prism-api-1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:05:32.791707 polypheny-prism-api-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 11:05:30.000000 polypheny-prism-api-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-17 11:05:32.791707 polypheny-prism-api-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-17 11:05:30.000000 polypheny-prism-api-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:05:32.787707 polypheny-prism-api-1.5/org/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:05:32.787707 polypheny-prism-api-1.5/org/polypheny/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:05:32.791707 polypheny-prism-api-1.5/org/polypheny/prism/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/connection_requests_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/connection_responses_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/document_frame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/graph_frame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/meta_requests_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/meta_responses_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/namespace_meta_requests_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/namespace_meta_responses_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/protointerface_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/relational_frame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/statement_requests_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/statement_responses_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/transaction_requests_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/transaction_responses_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-05-17 11:05:31.000000 polypheny-prism-api-1.5/org/polypheny/prism/value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 11:05:32.000000 polypheny-prism-api-1.5/org/polypheny/prism/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:05:32.791707 polypheny-prism-api-1.5/polypheny_prism_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-17 11:05:32.000000 polypheny-prism-api-1.5/polypheny_prism_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 11:05:32.000000 polypheny-prism-api-1.5/polypheny_prism_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:05:32.000000 polypheny-prism-api-1.5/polypheny_prism_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 11:05:32.000000 polypheny-prism-api-1.5/polypheny_prism_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 11:05:32.000000 polypheny-prism-api-1.5/polypheny_prism_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:05:32.791707 polypheny-prism-api-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-17 11:05:30.000000 polypheny-prism-api-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:00:34.770534 polypheny-prism-api-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 12:00:32.000000 polypheny-prism-api-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-17 12:00:34.770534 polypheny-prism-api-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-17 12:00:32.000000 polypheny-prism-api-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:00:34.766534 polypheny-prism-api-1.6/org/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:00:34.766534 polypheny-prism-api-1.6/org/polypheny/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:00:34.770534 polypheny-prism-api-1.6/org/polypheny/prism/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/connection_requests_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/connection_responses_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/document_frame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/graph_frame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/meta_requests_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/meta_responses_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/namespace_meta_requests_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/namespace_meta_responses_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/protointerface_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/relational_frame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5056 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/statement_requests_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/statement_responses_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/transaction_requests_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/transaction_responses_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-05-17 12:00:33.000000 polypheny-prism-api-1.6/org/polypheny/prism/value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 12:00:34.000000 polypheny-prism-api-1.6/org/polypheny/prism/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 12:00:34.770534 polypheny-prism-api-1.6/polypheny_prism_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-17 12:00:34.000000 polypheny-prism-api-1.6/polypheny_prism_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-17 12:00:34.000000 polypheny-prism-api-1.6/polypheny_prism_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 12:00:34.000000 polypheny-prism-api-1.6/polypheny_prism_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 12:00:34.000000 polypheny-prism-api-1.6/polypheny_prism_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 12:00:34.000000 polypheny-prism-api-1.6/polypheny_prism_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 12:00:34.770534 polypheny-prism-api-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-17 12:00:32.000000 polypheny-prism-api-1.6/setup.py
```

### Comparing `polypheny-prism-api-1.5/LICENSE` & `polypheny-prism-api-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/PKG-INFO` & `polypheny-prism-api-1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: polypheny-prism-api
-Version: 1.5
+Version: 1.6
 Summary: Polypheny Prism API files for Python
-Home-page: UNKNOWN
-License: UNKNOWN
+Home-page: https://polypheny.com/
+Author: The Polypheny Project
+Author-email: mail@polypheny.org
+License: Apache License, Version 2.0
+Project-URL: Documentation, https://docs.polypheny.com/en/latest/query_interfaces/prism/protocol
+Project-URL: Code, https://github.com/polypheny/Polypheny-Prism-API
 Description: # Polypheny-Prism-API
         The definition files for the Polypheny Prism API, a multi-model, multi-language query interface.
         
         The Prism Interface uses Protocol Buffer (protobuf) messages to define it's services. To keep things clear and well-organized, the message definitions are grouped into several files. This simplifies finding specific messages, based on what they do or what part of the system they relate to. The files itself are grouped in categories. Those are expressed in the file names.
         Two kinds of categories exist:
         
         ### Request Response Category
```

### Comparing `polypheny-prism-api-1.5/README.md` & `polypheny-prism-api-1.6/README.md`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/connection_requests_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/connection_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/connection_responses_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/connection_responses_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/document_frame_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/document_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/error_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/error_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/graph_frame_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/graph_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/meta_requests_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/meta_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/meta_responses_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/meta_responses_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/namespace_meta_requests_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/namespace_meta_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/namespace_meta_responses_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/namespace_meta_responses_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/protointerface_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/protointerface_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/relational_frame_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/relational_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/statement_requests_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/statement_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/statement_responses_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/statement_responses_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/transaction_requests_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/transaction_requests_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/transaction_responses_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/transaction_responses_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/org/polypheny/prism/value_pb2.py` & `polypheny-prism-api-1.6/org/polypheny/prism/value_pb2.py`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/polypheny_prism_api.egg-info/PKG-INFO` & `polypheny-prism-api-1.6/polypheny_prism_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 Metadata-Version: 2.1
 Name: polypheny-prism-api
-Version: 1.5
+Version: 1.6
 Summary: Polypheny Prism API files for Python
-Home-page: UNKNOWN
-License: UNKNOWN
+Home-page: https://polypheny.com/
+Author: The Polypheny Project
+Author-email: mail@polypheny.org
+License: Apache License, Version 2.0
+Project-URL: Documentation, https://docs.polypheny.com/en/latest/query_interfaces/prism/protocol
+Project-URL: Code, https://github.com/polypheny/Polypheny-Prism-API
 Description: # Polypheny-Prism-API
         The definition files for the Polypheny Prism API, a multi-model, multi-language query interface.
         
         The Prism Interface uses Protocol Buffer (protobuf) messages to define it's services. To keep things clear and well-organized, the message definitions are grouped into several files. This simplifies finding specific messages, based on what they do or what part of the system they relate to. The files itself are grouped in categories. Those are expressed in the file names.
         Two kinds of categories exist:
         
         ### Request Response Category
```

### Comparing `polypheny-prism-api-1.5/polypheny_prism_api.egg-info/SOURCES.txt` & `polypheny-prism-api-1.6/polypheny_prism_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polypheny-prism-api-1.5/setup.py` & `polypheny-prism-api-1.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 import sys
 
 from setuptools import setup
 
 # Retrieve 'VERSION' environment variable, default to '0.0' if not found.
 version = os.getenv('VERSION', '0.0')
 
+print(f"Building version: {version}")
+
+if version == '0.0':
+    raise ValueError("Version not set or defaulting to '0.0'. Please set the VERSION environment variable.")
+
 # Attempt to split the version number, default to '0' for both if it fails
 try:
     major, minor = version.split('.')
 except ValueError:
-    major, minor = '0', '0'  # Default to '0.0' if the version isn't in a 'major.minor' format
+    raise ValueError(f"Invalid version format: {version}. Expected 'major.minor' format.")
 
 
 with open('org/polypheny/prism/version.py', 'w') as f:
     f.write(f'MAJOR_VERSION = {major}\n')
     f.write(f'MINOR_VERSION = {minor}\n')
 
 
@@ -22,12 +27,20 @@
     long_description = f.read()
 
 setup(name='polypheny-prism-api',
       version=version,
       description='Polypheny Prism API files for Python',
       long_description=long_description,
       long_description_content_type='text/markdown',
+      author="The Polypheny Project",
+      author_email="mail@polypheny.org",
+      url="https://polypheny.com/",
+      project_urls={
+        "Documentation": "https://docs.polypheny.com/en/latest/query_interfaces/prism/protocol",
+        "Code": "https://github.com/polypheny/Polypheny-Prism-API"
+      },
+      license="Apache License, Version 2.0",
       packages=['org/polypheny/prism'],
       install_requires=[
           "protobuf==4.24.3",
       ],
-      )
+)
```

