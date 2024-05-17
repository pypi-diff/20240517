# Comparing `tmp/ibm-watson-8.0.0.tar.gz` & `tmp/ibm_watson-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-watson-8.0.0.tar", last modified: Mon Feb 26 17:37:48 2024, max compression
+gzip compressed data, was "ibm_watson-8.1.0.tar", last modified: Fri May 17 16:52:54 2024, max compression
```

## Comparing `ibm-watson-8.0.0.tar` & `ibm_watson-8.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:37:48.155794 ibm-watson-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19769 2024-02-26 17:37:48.155794 ibm-watson-8.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    18467 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:37:48.147794 ibm-watson-8.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/assistant_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/assistant_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/discovery_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/discovery_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/language_translator_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3871 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/microphone-speech-to-text.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/natural_language_understanding_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/speaker_text_to_speech.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/speech_to_text_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/examples/text_to_speech_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:37:48.151794 ibm-watson-8.0.0/ibm_watson/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1255 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   630179 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/assistant_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)   620976 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/assistant_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/common.py
--rw-r--r--   0 runner    (1001) docker     (127)   619879 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/discovery_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)   580286 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/discovery_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    95870 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/language_translator_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)   239955 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/natural_language_understanding_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)   469273 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/speech_to_text_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    25704 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/speech_to_text_v1_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/text_to_speech_adapter_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)   161892 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/text_to_speech_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-26 17:37:17.000000 ibm-watson-8.0.0/ibm_watson/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:37:48.155794 ibm-watson-8.0.0/ibm_watson/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/websocket/audio_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/websocket/recognize_abstract_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8388 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/websocket/recognize_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/websocket/synthesize_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/ibm_watson/websocket/synthesize_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 17:37:48.155794 ibm-watson-8.0.0/ibm_watson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19769 2024-02-26 17:37:48.000000 ibm-watson-8.0.0/ibm_watson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-26 17:37:48.000000 ibm-watson-8.0.0/ibm_watson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 17:37:48.000000 ibm-watson-8.0.0/ibm_watson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-26 17:37:48.000000 ibm-watson-8.0.0/ibm_watson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-26 17:37:48.000000 ibm-watson-8.0.0/ibm_watson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 17:37:48.000000 ibm-watson-8.0.0/ibm_watson.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-26 17:36:24.000000 ibm-watson-8.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 17:37:48.155794 ibm-watson-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-02-26 17:37:17.000000 ibm-watson-8.0.0/setup.py
+drwxr-xr-x   0 Home       (501) staff       (20)        0 2024-05-17 16:52:54.768720 ibm_watson-8.1.0/
+-rw-r--r--   0 Home       (501) staff       (20)    10174 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/LICENSE
+-rw-r--r--   0 Home       (501) staff       (20)      157 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/MANIFEST.in
+-rw-r--r--   0 Home       (501) staff       (20)    20390 2024-05-17 16:52:54.768377 ibm_watson-8.1.0/PKG-INFO
+-rwxr-xr-x   0 Home       (501) staff       (20)    19088 2024-03-13 18:02:55.000000 ibm_watson-8.1.0/README.md
+drwxr-xr-x   0 Home       (501) staff       (20)        0 2024-05-17 16:52:54.749390 ibm_watson-8.1.0/examples/
+-rw-r--r--   0 Home       (501) staff       (20)      421 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/examples/README.md
+-rw-r--r--   0 Home       (501) staff       (20)      585 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/examples/__init__.py
+-rw-r--r--   0 Home       (501) staff       (20)    10742 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/assistant_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)     1017 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/assistant_v2.py
+-rw-r--r--   0 Home       (501) staff       (20)     2772 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/discovery_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)     3254 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/examples/discovery_v2.py
+-rw-r--r--   0 Home       (501) staff       (20)     2485 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/language_translator_v3.py
+-rw-r--r--   0 Home       (501) staff       (20)     3804 2024-05-17 16:20:24.000000 ibm_watson-8.1.0/examples/microphone-speech-to-text.py
+-rw-r--r--   0 Home       (501) staff       (20)     1030 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/natural_language_understanding_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)     3336 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/speaker_text_to_speech.py
+-rw-r--r--   0 Home       (501) staff       (20)     1918 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/speech_to_text_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)     3180 2023-05-16 14:20:24.000000 ibm_watson-8.1.0/examples/text_to_speech_v1.py
+drwxr-xr-x   0 Home       (501) staff       (20)        0 2024-05-17 16:52:54.762884 ibm_watson-8.1.0/ibm_watson/
+-rwxr-xr-x   0 Home       (501) staff       (20)     1255 2023-05-16 14:20:43.000000 ibm_watson-8.1.0/ibm_watson/__init__.py
+-rw-r--r--   0 Home       (501) staff       (20)   630179 2024-02-26 17:25:35.000000 ibm_watson-8.1.0/ibm_watson/assistant_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)   620976 2024-02-26 17:25:35.000000 ibm_watson-8.1.0/ibm_watson/assistant_v2.py
+-rw-r--r--   0 Home       (501) staff       (20)     1645 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/ibm_watson/common.py
+-rw-r--r--   0 Home       (501) staff       (20)   619879 2024-02-26 17:25:35.000000 ibm_watson-8.1.0/ibm_watson/discovery_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)   587024 2024-05-17 16:20:24.000000 ibm_watson-8.1.0/ibm_watson/discovery_v2.py
+-rw-r--r--   0 Home       (501) staff       (20)    95870 2024-02-26 17:25:35.000000 ibm_watson-8.1.0/ibm_watson/language_translator_v3.py
+-rw-r--r--   0 Home       (501) staff       (20)   239955 2024-02-26 17:25:35.000000 ibm_watson-8.1.0/ibm_watson/natural_language_understanding_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)   475462 2024-05-17 16:20:24.000000 ibm_watson-8.1.0/ibm_watson/speech_to_text_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)    24619 2024-05-17 16:20:24.000000 ibm_watson-8.1.0/ibm_watson/speech_to_text_v1_adapter.py
+-rw-r--r--   0 Home       (501) staff       (20)     9132 2023-08-07 16:12:45.000000 ibm_watson-8.1.0/ibm_watson/text_to_speech_adapter_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)   161892 2024-05-15 19:16:18.000000 ibm_watson-8.1.0/ibm_watson/text_to_speech_v1.py
+-rw-r--r--   0 Home       (501) staff       (20)       22 2024-05-17 16:20:24.000000 ibm_watson-8.1.0/ibm_watson/version.py
+drwxr-xr-x   0 Home       (501) staff       (20)        0 2024-05-17 16:52:54.765508 ibm_watson-8.1.0/ibm_watson/websocket/
+-rw-r--r--   0 Home       (501) staff       (20)      854 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/ibm_watson/websocket/__init__.py
+-rw-r--r--   0 Home       (501) staff       (20)     1299 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/ibm_watson/websocket/audio_source.py
+-rw-r--r--   0 Home       (501) staff       (20)     1638 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/ibm_watson/websocket/recognize_abstract_callback.py
+-rw-r--r--   0 Home       (501) staff       (20)     8286 2024-05-17 16:20:24.000000 ibm_watson-8.1.0/ibm_watson/websocket/recognize_listener.py
+-rw-r--r--   0 Home       (501) staff       (20)     1614 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/ibm_watson/websocket/synthesize_callback.py
+-rw-r--r--   0 Home       (501) staff       (20)     4109 2023-08-07 16:12:48.000000 ibm_watson-8.1.0/ibm_watson/websocket/synthesize_listener.py
+drwxr-xr-x   0 Home       (501) staff       (20)        0 2024-05-17 16:52:54.768001 ibm_watson-8.1.0/ibm_watson.egg-info/
+-rw-r--r--   0 Home       (501) staff       (20)    20390 2024-05-17 16:52:54.000000 ibm_watson-8.1.0/ibm_watson.egg-info/PKG-INFO
+-rw-r--r--   0 Home       (501) staff       (20)     1261 2024-05-17 16:52:54.000000 ibm_watson-8.1.0/ibm_watson.egg-info/SOURCES.txt
+-rw-r--r--   0 Home       (501) staff       (20)        1 2024-05-17 16:52:54.000000 ibm_watson-8.1.0/ibm_watson.egg-info/dependency_links.txt
+-rw-r--r--   0 Home       (501) staff       (20)       98 2024-05-17 16:52:54.000000 ibm_watson-8.1.0/ibm_watson.egg-info/requires.txt
+-rw-r--r--   0 Home       (501) staff       (20)       11 2024-05-17 16:52:54.000000 ibm_watson-8.1.0/ibm_watson.egg-info/top_level.txt
+-rw-r--r--   0 Home       (501) staff       (20)        1 2023-02-13 20:24:27.000000 ibm_watson-8.1.0/ibm_watson.egg-info/zip-safe
+-rw-r--r--   0 Home       (501) staff       (20)       89 2022-09-15 20:06:16.000000 ibm_watson-8.1.0/pyproject.toml
+-rw-r--r--   0 Home       (501) staff       (20)       38 2024-05-17 16:52:54.768766 ibm_watson-8.1.0/setup.cfg
+-rw-r--r--   0 Home       (501) staff       (20)     2539 2024-05-17 16:20:24.000000 ibm_watson-8.1.0/setup.py
```

### Comparing `ibm-watson-8.0.0/LICENSE` & `ibm_watson-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/PKG-INFO` & `ibm_watson-8.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson
-Version: 8.0.0
+Version: 8.1.0
 Summary: Client library to use the IBM Watson Services
 Home-page: https://github.com/watson-developer-cloud/python-sdk
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 License: Apache 2.0
 Keywords: language,vision,question and answer tone_analyzer,natural language classifier,text to speech,language translation,language identification,concept expansion,machine translation,personality insights,message resonance,watson developer cloud,wdc,watson,ibm,dialog,user modeling,tone analyzer,speech to text,visual recognition
 Classifier: Programming Language :: Python
@@ -197,36 +197,51 @@
 # in the constructor, assuming control of managing the token
 authenticator = BearerTokenAuthenticator('your bearer token')
 discovery = DiscoveryV1(version='2019-04-30',
                         authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
-### Username and password
+#### Username and password
 
 ```python
 from ibm_watson import DiscoveryV1
 from ibm_cloud_sdk_core.authenticators import BasicAuthenticator
 
 authenticator = BasicAuthenticator('username', 'password')
 discovery = DiscoveryV1(version='2019-04-30', authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
-### No Authentication
+#### No Authentication
 
 ```python
 from ibm_watson import DiscoveryV1
 from ibm_cloud_sdk_core.authenticators import NoAuthAuthenticator
 
 authenticator = NoAuthAuthenticator()
 discovery = DiscoveryV1(version='2019-04-30', authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
+### MCSP
+
+To use the SDK through a third party cloud provider (such as AWS), use the `MCSPAuthenticator`. This will require the base endpoint URL for the MCSP token service (e.g. https://iam.platform.saas.ibm.com) and an apikey. 
+
+```python
+from ibm_watson import AssistantV2
+from ibm_cloud_sdk_core.authenticators import MCSPAuthenticator
+
+# In the constructor, letting the SDK manage the token
+authenticator = MCSPAuthenticator('apikey', 'token_service_endpoint')
+assistant = AssistantV2(version='2023-06-15',
+                        authenticator=authenticator)
+assistant.set_service_url('<url_as_per_region>')
+```
+
 ## Python version
 
 Tested on Python 3.9, 3.10, and 3.11.
 
 ## Questions
 
 If you have issues with the APIs or have a question about the Watson services, see [Stack Overflow](https://stackoverflow.com/questions/tagged/ibm-watson+python).
```

### Comparing `ibm-watson-8.0.0/README.md` & `ibm_watson-8.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -172,36 +172,51 @@
 # in the constructor, assuming control of managing the token
 authenticator = BearerTokenAuthenticator('your bearer token')
 discovery = DiscoveryV1(version='2019-04-30',
                         authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
-### Username and password
+#### Username and password
 
 ```python
 from ibm_watson import DiscoveryV1
 from ibm_cloud_sdk_core.authenticators import BasicAuthenticator
 
 authenticator = BasicAuthenticator('username', 'password')
 discovery = DiscoveryV1(version='2019-04-30', authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
-### No Authentication
+#### No Authentication
 
 ```python
 from ibm_watson import DiscoveryV1
 from ibm_cloud_sdk_core.authenticators import NoAuthAuthenticator
 
 authenticator = NoAuthAuthenticator()
 discovery = DiscoveryV1(version='2019-04-30', authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
+### MCSP
+
+To use the SDK through a third party cloud provider (such as AWS), use the `MCSPAuthenticator`. This will require the base endpoint URL for the MCSP token service (e.g. https://iam.platform.saas.ibm.com) and an apikey. 
+
+```python
+from ibm_watson import AssistantV2
+from ibm_cloud_sdk_core.authenticators import MCSPAuthenticator
+
+# In the constructor, letting the SDK manage the token
+authenticator = MCSPAuthenticator('apikey', 'token_service_endpoint')
+assistant = AssistantV2(version='2023-06-15',
+                        authenticator=authenticator)
+assistant.set_service_url('<url_as_per_region>')
+```
+
 ## Python version
 
 Tested on Python 3.9, 3.10, and 3.11.
 
 ## Questions
 
 If you have issues with the APIs or have a question about the Watson services, see [Stack Overflow](https://stackoverflow.com/questions/tagged/ibm-watson+python).
```

### Comparing `ibm-watson-8.0.0/examples/__init__.py` & `ibm_watson-8.1.0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/assistant_v1.py` & `ibm_watson-8.1.0/examples/assistant_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/assistant_v2.py` & `ibm_watson-8.1.0/examples/assistant_v2.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/discovery_v1.py` & `ibm_watson-8.1.0/examples/discovery_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/discovery_v2.py` & `ibm_watson-8.1.0/examples/discovery_v2.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/language_translator_v3.py` & `ibm_watson-8.1.0/examples/language_translator_v3.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/microphone-speech-to-text.py` & `ibm_watson-8.1.0/examples/microphone-speech-to-text.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,15 @@
         print("Connection closed")
 
 # this function will initiate the recognize service and pass in the AudioSource
 def recognize_using_weboscket(*args):
     mycallback = MyRecognizeCallback()
     speech_to_text.recognize_using_websocket(audio=audio_source,
                                              content_type='audio/l16; rate=44100',
-                                             recognize_callback=mycallback,
-                                             interim_results=True)
+                                             recognize_callback=mycallback)
 
 ###############################################
 #### Prepare the for recording using Pyaudio ##
 ###############################################
 
 # Variables for recording the speech
 FORMAT = pyaudio.paInt16
```

### Comparing `ibm-watson-8.0.0/examples/natural_language_understanding_v1.py` & `ibm_watson-8.1.0/examples/natural_language_understanding_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/speaker_text_to_speech.py` & `ibm_watson-8.1.0/examples/speaker_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/speech_to_text_v1.py` & `ibm_watson-8.1.0/examples/speech_to_text_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/examples/text_to_speech_v1.py` & `ibm_watson-8.1.0/examples/text_to_speech_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/__init__.py` & `ibm_watson-8.1.0/ibm_watson/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/assistant_v1.py` & `ibm_watson-8.1.0/ibm_watson/assistant_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/assistant_v2.py` & `ibm_watson-8.1.0/ibm_watson/assistant_v2.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/common.py` & `ibm_watson-8.1.0/ibm_watson/common.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/discovery_v1.py` & `ibm_watson-8.1.0/ibm_watson/discovery_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/discovery_v2.py` & `ibm_watson-8.1.0/ibm_watson/discovery_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,16 @@
 
         :param str name: The human readable name of this project.
         :param str type: The type of project.
                The `content_intelligence` type is a *Document Retrieval for Contracts*
                project and the `other` type is a *Custom* project.
                The `content_mining` and `content_intelligence` types are available with
                Premium plan managed deployments and installed deployments only.
+               The Intelligent Document Processing (IDP) project type is available from
+               IBM Cloud-managed instances only.
         :param DefaultQueryParams default_query_parameters: (optional) Default
                query parameters for this project.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ProjectDetails` object
         """
 
@@ -200,16 +202,17 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Get project.
 
         Get details on the specified project.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ProjectDetails` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -252,16 +255,17 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Update a project.
 
         Update the specified project's name.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str name: (optional) The new name to give this project.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ProjectDetails` object
         """
 
         if not project_id:
@@ -313,16 +317,17 @@
         """
         Delete a project.
 
         Deletes the specified project.
         **Important:** Deleting a project deletes everything that is part of the specified
         project, including all collections.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -365,16 +370,17 @@
     ) -> DetailedResponse:
         """
         List fields.
 
         Gets a list of the unique fields (and their types) stored in the specified
         collections.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param List[str] collection_ids: (optional) Comma separated list of the
                collection IDs. If this parameter is not specified, all collections in the
                project are used.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ListFieldsResponse` object
         """
@@ -423,16 +429,17 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         List collections.
 
         Lists existing collections for the specified project.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ListCollectionsResponse` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -470,29 +477,34 @@
     def create_collection(
         self,
         project_id: str,
         name: str,
         *,
         description: Optional[str] = None,
         language: Optional[str] = None,
+        ocr_enabled: Optional[bool] = None,
         enrichments: Optional[List['CollectionEnrichment']] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Create a collection.
 
         Create a new collection in the specified project.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str name: The name of the collection.
         :param str description: (optional) A description of the collection.
         :param str language: (optional) The language of the collection. For a list
                of supported languages, see the [product
                documentation](/docs/discovery-data?topic=discovery-data-language-support).
+        :param bool ocr_enabled: (optional) If set to `true`, optical character
+               recognition (OCR) is enabled. For more information, see [Optical character
+               recognition](/docs/discovery-data?topic=discovery-data-collections#ocr).
         :param List[CollectionEnrichment] enrichments: (optional) An array of
                enrichments that are applied to this collection. To get a list of
                enrichments that are available for a project, use the [List
                enrichments](#listenrichments) method.
                If no enrichments are specified when the collection is created, the default
                enrichments for the project type are applied. For more information about
                project default settings, see the [product
@@ -520,14 +532,15 @@
             'version': self.version,
         }
 
         data = {
             'name': name,
             'description': description,
             'language': language,
+            'ocr_enabled': ocr_enabled,
             'enrichments': enrichments,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
@@ -557,17 +570,19 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Get collection details.
 
         Get details about the specified collection.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `CollectionDetails` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -608,14 +623,15 @@
     def update_collection(
         self,
         project_id: str,
         collection_id: str,
         *,
         name: Optional[str] = None,
         description: Optional[str] = None,
+        ocr_enabled: Optional[bool] = None,
         enrichments: Optional[List['CollectionEnrichment']] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Update a collection.
 
         Updates the specified collection's name, description, enrichments, and
@@ -628,19 +644,24 @@
         To remove a configuration that applies JSON normalization operations as part of
         the conversion phase of ingestion, specify an empty `json_normalizations` object
         (`[]`) in the request.
         To remove a configuration that applies JSON normalization operations after
         enrichments are applied, specify an empty `normalizations` object (`[]`) in the
         request.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param str name: (optional) The new name of the collection.
         :param str description: (optional) The new description of the collection.
+        :param bool ocr_enabled: (optional) If set to `true`, optical character
+               recognition (OCR) is enabled. For more information, see [Optical character
+               recognition](/docs/discovery-data?topic=discovery-data-collections#ocr).
         :param List[CollectionEnrichment] enrichments: (optional) An array of
                enrichments that are applied to this collection.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `CollectionDetails` object
         """
 
@@ -661,14 +682,15 @@
         params = {
             'version': self.version,
         }
 
         data = {
             'name': name,
             'description': description,
+            'ocr_enabled': ocr_enabled,
             'enrichments': enrichments,
         }
         data = {k: v for (k, v) in data.items() if v is not None}
         data = json.dumps(data)
         headers['content-type'] = 'application/json'
 
         if 'headers' in kwargs:
@@ -700,17 +722,19 @@
     ) -> DetailedResponse:
         """
         Delete a collection.
 
         Deletes the specified collection from the project. All documents stored in the
         specified collection and not shared is also deleted.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -768,17 +792,19 @@
         List documents.
 
         Lists the documents in the specified collection. The list includes only the
         document ID of each document and returns information for up to 10,000 documents.
         **Note**: This method is available only from Cloud Pak for Data version 4.0.9 and
         later installed instances, and from IBM Cloud-managed instances.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param int count: (optional) The maximum number of documents to return. Up
                to 1,000 documents are returned by default. The maximum number allowed is
                10,000.
         :param str status: (optional) Filters the documents to include only
                documents with the specified ingestion status. The options include:
                * `available`: Ingestion is finished and the document is indexed.
                * `failed`: Ingestion is finished, but the document is not indexed because
@@ -889,17 +915,19 @@
         appending the ID to the endpoint
         (`/v2/projects/{project_id}/collections/{collection_id}/documents/{document_id}`).
         If a document already exists with the specified ID, it is replaced.
         For more information about how certain file types and field names are handled when
         a file is added to a collection, see the [product
         documentation](/docs/discovery-data?topic=discovery-data-index-overview#field-name-limits).
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param BinaryIO file: (optional) **Add a document**: The content of the
                document to ingest. For the supported file types and maximum supported file
                size limits when adding a document, see [the
                documentation](/docs/discovery-data?topic=discovery-data-collections#supportedfiletypes).
                **Analyze a document**: The content of the document to analyze but not
                ingest. Only the `application/json` content type is supported by the
                Analyze API. For maximum supported file size limits, see [the product
@@ -985,17 +1013,19 @@
         Get document details.
 
         Get details about a specific document, whether the document is added by uploading
         a file or by crawling an external data source.
         **Note**: This method is available only from Cloud Pak for Data version 4.0.9 and
         later installed instances, and from IBM Cloud-managed instances.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param str document_id: The ID of the document.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DocumentDetails` object
         """
 
         if not project_id:
@@ -1062,17 +1092,19 @@
         **Notes:**
          * Uploading a new document with this method automatically replaces any existing
         document stored with the same document ID.
          * If an uploaded document is split into child documents during ingestion, all
         existing child documents are overwritten, even if the updated version of the
         document has fewer child documents.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param str document_id: The ID of the document.
         :param BinaryIO file: (optional) **Add a document**: The content of the
                document to ingest. For the supported file types and maximum supported file
                size limits when adding a document, see [the
                documentation](/docs/discovery-data?topic=discovery-data-collections#supportedfiletypes).
                **Analyze a document**: The content of the document to analyze but not
                ingest. Only the `application/json` content type is supported by the
@@ -1171,17 +1203,19 @@
         **Note:** Files such as CSV or JSON files generate subdocuments when they are
         added to a collection. If you delete a subdocument, and then repeat the action
         that created it, the deleted document is added back in to your collection. To
         remove subdocuments that are generated by an uploaded file, delete the original
         document instead. You can get the document ID of the original document from the
         `parent_document_id` of the subdocument result.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param str document_id: The ID of the document.
         :param bool x_watson_discovery_force: (optional) When `true`, the uploaded
                document is added to the collection even if the data for that collection is
                shared with other collections.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DeleteDocumentResponse` object
@@ -1265,16 +1299,17 @@
         project default settings, see the [Discovery
         documentation](/docs/discovery-data?topic=discovery-data-query-defaults). See [the
         Projects API documentation](#create-project) for details about how to set custom
         default query settings.
         The length of the UTF-8 encoding of the POST body cannot exceed 10,000 bytes,
         which is roughly equivalent to 10,000 characters in English.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param List[str] collection_ids: (optional) A comma-separated list of
                collection IDs to be queried against.
         :param str filter: (optional) Searches for documents that match the
                Discovery Query Language criteria that is specified as input. Filter calls
                are cached and are faster than query calls because the results are not
                ordered by relevance. When used with the **aggregation**, **query**, or
                **natural_language_query** parameters, the **filter** parameter runs first.
@@ -1415,16 +1450,17 @@
         Get Autocomplete Suggestions.
 
         Returns completion query suggestions for the specified prefix.
         Suggested words are based on terms from the project documents. Suggestions are not
         based on terms from the project's search history, and the project does not learn
         from previous user choices.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str prefix: The prefix to use for autocompletion. For example, the
                prefix `Ho` could autocomplete to `hot`, `housing`, or `how`.
         :param List[str] collection_ids: (optional) Comma separated list of the
                collection IDs. If this parameter is not specified, all collections in the
                project are used.
         :param str field: (optional) The field in the result documents that
                autocompletion suggestions are identified from.
@@ -1489,17 +1525,19 @@
     ) -> DetailedResponse:
         """
         Query collection notices.
 
         Finds collection-level notices (errors and warnings) that are generated when
         documents are ingested.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param str filter: (optional) Searches for documents that match the
                Discovery Query Language criteria that is specified as input. Filter calls
                are cached and are faster than query calls because the results are not
                ordered by relevance. When used with the `aggregation`, `query`, or
                `natural_language_query` parameters, the `filter` parameter runs first.
                This parameter is useful for limiting results to those that contain
                specific metadata values.
@@ -1580,16 +1618,17 @@
     ) -> DetailedResponse:
         """
         Query project notices.
 
         Finds project-level notices (errors and warnings). Currently, project-level
         notices are generated by relevancy training.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str filter: (optional) Searches for documents that match the
                Discovery Query Language criteria that is specified as input. Filter calls
                are cached and are faster than query calls because the results are not
                ordered by relevance. When used with the `aggregation`, `query`, or
                `natural_language_query` parameters, the `filter` parameter runs first.
                This parameter is useful for limiting results to those that contain
                specific metadata values.
@@ -1667,17 +1706,19 @@
         """
         Get a custom stop words list.
 
         Returns the custom stop words list that is used by the collection. For information
         about the default stop words lists that are applied to queries, see [the product
         documentation](/docs/discovery-data?topic=discovery-data-stopwords).
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `StopWordList` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -1733,17 +1774,19 @@
         A default stop words list is used by all collections. The default list is applied
         both at indexing time and at query time. A custom stop words list that you add is
         used at query time only.
         The custom stop words list augments the default stop words list; you cannot remove
         stop words. For information about the default stop words lists per language, see
         [the product documentation](/docs/discovery-data?topic=discovery-data-stopwords).
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param List[str] stopwords: (optional) List of stop words.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `StopWordList` object
         """
 
         if not project_id:
@@ -1799,17 +1842,19 @@
         """
         Delete a custom stop words list.
 
         Deletes a custom stop words list to stop using it in queries against the
         collection. After a custom stop words list is deleted, the default stop words list
         is used.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -1854,17 +1899,19 @@
     ) -> DetailedResponse:
         """
         Get the expansion list.
 
         Returns the current expansion list for the specified collection. If an expansion
         list is not specified, an empty expansions array is returned.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Expansions` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -1914,17 +1961,19 @@
 
         Creates or replaces the expansion list for this collection. An expansion list
         introduces alternative wording for key terms that are mentioned in your
         collection. By identifying synonyms or common misspellings, you expand the scope
         of a query beyond exact matches. The maximum number of expanded terms allowed per
         collection is 5,000.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param List[Expansion] expansions: An array of query expansion definitions.
                 Each object in the **expansions** array represents a term or set of terms
                that will be expanded into other terms. Each expansion object can be
                configured as `bidirectional` or `unidirectional`.
                * **Bidirectional**: Each entry in the `expanded_terms` list expands to
                include all expanded terms. For example, a query for `ibm` expands to `ibm
                OR international business machines OR big blue`.
@@ -1994,17 +2043,19 @@
     ) -> DetailedResponse:
         """
         Delete the expansion list.
 
         Removes the expansion information for this collection. To disable query expansion
         for a collection, delete the expansion list.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2051,16 +2102,17 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         List component settings.
 
         Returns default configuration settings for components.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `ComponentSettingsResponse` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2106,16 +2158,17 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         List training queries.
 
         List the training queries for the specified project.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `TrainingQuerySet` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2157,16 +2210,17 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Delete training queries.
 
         Removes all training queries for the specified project.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2213,16 +2267,17 @@
         """
         Create a training query.
 
         Add a query to the training data for this project. The query can contain a filter
         and natural language query.
         **Note**: You cannot apply relevancy training to a `content_mining` project type.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str natural_language_query: The natural text query that is used as
                the training query.
         :param List[TrainingExample] examples: Array of training examples.
         :param str filter: (optional) The filter used on the collection before the
                **natural_language_query** is applied. Only specify a filter if the
                documents that you consider to be most relevant are not included in the top
                100 results when you submit test queries. If you specify a filter during
@@ -2290,16 +2345,17 @@
     ) -> DetailedResponse:
         """
         Get a training data query.
 
         Get details for a specific training data query, including the query string and all
         examples.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str query_id: The ID of the query used for training.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `TrainingQuery` object
         """
 
         if not project_id:
@@ -2350,16 +2406,17 @@
     ) -> DetailedResponse:
         """
         Update a training query.
 
         Updates an existing training query and its examples. You must resubmit all of the
         examples with the update request.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str query_id: The ID of the query used for training.
         :param str natural_language_query: The natural text query that is used as
                the training query.
         :param List[TrainingExample] examples: Array of training examples.
         :param str filter: (optional) The filter used on the collection before the
                **natural_language_query** is applied. Only specify a filter if the
                documents that you consider to be most relevant are not included in the top
@@ -2432,16 +2489,17 @@
         Delete a training data query.
 
         Removes details from a training data query, including the query string and all
         examples.
         To delete an example, use the *Update a training query* method and omit the
         example that you want to delete from the example set.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param str query_id: The ID of the query used for training.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
@@ -2491,16 +2549,17 @@
         """
         List enrichments.
 
         Lists the enrichments available to this project. The *Part of Speech* and
         *Sentiment of Phrases* enrichments might be listed, but are reserved for internal
         use only.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Enrichments` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2546,16 +2605,17 @@
         """
         Create an enrichment.
 
         Create an enrichment for use with the specified project. To apply the enrichment
         to a collection in the project, use the [Collections
         API](/apidocs/discovery-data#createcollection).
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param CreateEnrichment enrichment: Information about a specific
                enrichment.
         :param BinaryIO file: (optional) The enrichment file to upload. Expected
                file types per enrichment are as follows:
                * CSV for `dictionary` and `sentence_classifier` (the training data CSV
                file to upload).
                * PEAR for `uima_annotator` and `rule_based` (Explorer)
@@ -2615,17 +2675,19 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Get enrichment.
 
         Get details about a specific enrichment.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str enrichment_id: The ID of the enrichment.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str enrichment_id: The Universally Unique Identifier (UUID) of the
+               enrichment.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Enrichment` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2673,17 +2735,19 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Update an enrichment.
 
         Updates an existing enrichment's name and description.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str enrichment_id: The ID of the enrichment.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str enrichment_id: The Universally Unique Identifier (UUID) of the
+               enrichment.
         :param str name: A new name for the enrichment.
         :param str description: (optional) A new description for the enrichment.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `Enrichment` object
         """
 
@@ -2742,17 +2806,19 @@
     ) -> DetailedResponse:
         """
         Delete an enrichment.
 
         Deletes an existing enrichment from the specified project.
         **Note:** Only enrichments that have been manually created can be deleted.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str enrichment_id: The ID of the enrichment.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str enrichment_id: The Universally Unique Identifier (UUID) of the
+               enrichment.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2800,16 +2866,17 @@
     ) -> DetailedResponse:
         """
         List document classifiers.
 
         Get a list of the document classifiers in a project. Returns only the name and
         classifier ID of each document classifier.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DocumentClassifiers` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2860,16 +2927,17 @@
         Create a document classifier. You can use the API to create a document classifier
         in any project type. After you create a document classifier, you can use the
         Enrichments API to create a classifier enrichment, and then the Collections API to
         apply the enrichment to a collection in the project.
         **Note:** This method is supported on installed instances (IBM Cloud Pak for Data)
         or IBM Cloud-managed Premium or Enterprise plan instances.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
         :param BinaryIO training_data: The training data CSV file to upload. The
                CSV file must have headers. The file must include a field that contains the
                text you want to classify and a field that contains the classification
                labels that you want to use to classify your data. If you want to specify
                multiple values in a single field, use a semicolon as the value separator.
                For a sample file, see [the product
                documentation](/docs/discovery-data?topic=discovery-data-cm-doc-classifier).
@@ -2938,17 +3006,19 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Get a document classifier.
 
         Get details about a specific document classifier.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DocumentClassifier` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -2998,17 +3068,19 @@
     ) -> DetailedResponse:
         """
         Update a document classifier.
 
         Update the document classifier name or description, update the training data, or
         add or update the test data.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
         :param UpdateDocumentClassifier classifier: An object that contains a new
                name or description for a document classifier, updated training data, or
                new or updated test data.
         :param BinaryIO training_data: (optional) The training data CSV file to
                upload. The CSV file must have headers. The file must include a field that
                contains the text you want to classify and a field that contains the
                classification labels that you want to use to classify your data. If you
@@ -3079,17 +3151,19 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Delete a document classifier.
 
         Deletes an existing document classifier from the specified project.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -3138,17 +3212,19 @@
     ) -> DetailedResponse:
         """
         List document classifier models.
 
         Get a list of the document classifier models in a project. Returns only the name
         and model ID of each document classifier model.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DocumentClassifierModels` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -3204,17 +3280,19 @@
         Create a document classifier model.
 
         Create a document classifier model by training a model that uses the data and
         classifier settings defined in the specified document classifier.
         **Note:** This method is supported on installed intances (IBM Cloud Pak for Data)
         or IBM Cloud-managed Premium or Enterprise plan instances.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
         :param str name: The name of the document classifier model.
         :param str description: (optional) A description of the document classifier
                model.
         :param float learning_rate: (optional) A tuning parameter in an
                optimization algorithm that determines the step size at each iteration of
                the training process. It influences how much of any newly acquired
                information overrides the existing information, and therefore is said to
@@ -3300,18 +3378,21 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Get a document classifier model.
 
         Get details about a specific document classifier model.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
-        :param str model_id: The ID of the classifier model.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
+        :param str model_id: The Universally Unique Identifier (UUID) of the
+               classifier model.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DocumentClassifierModel` object
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -3363,18 +3444,21 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Update a document classifier model.
 
         Update the document classifier model name or description.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
-        :param str model_id: The ID of the classifier model.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
+        :param str model_id: The Universally Unique Identifier (UUID) of the
+               classifier model.
         :param str name: (optional) A new name for the enrichment.
         :param str description: (optional) A new description for the enrichment.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse with `dict` result representing a `DocumentClassifierModel` object
         """
 
@@ -3434,18 +3518,21 @@
         **kwargs,
     ) -> DetailedResponse:
         """
         Delete a document classifier model.
 
         Deletes an existing document classifier model from the specified project.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str classifier_id: The ID of the classifier.
-        :param str model_id: The ID of the classifier model.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str classifier_id: The Universally Unique Identifier (UUID) of the
+               classifier.
+        :param str model_id: The Universally Unique Identifier (UUID) of the
+               classifier model.
         :param dict headers: A `dict` containing the request headers
         :return: A `DetailedResponse` containing the result, headers and HTTP status code.
         :rtype: DetailedResponse
         """
 
         if not project_id:
             raise ValueError('project_id must be provided')
@@ -3514,17 +3601,19 @@
         Submit a request against only one collection at a time. Remember, the documents in
         the collection are not significant. It is the enrichments that are defined for the
         collection that matter. If you submit requests to several collections, then
         several models are initiated at the same time, which can cause request failures.
         **Note:** This method is supported with Enterprise plan deployments and installed
         deployments only.
 
-        :param str project_id: The ID of the project. This information can be found
-               from the *Integrate and Deploy* page in Discovery.
-        :param str collection_id: The ID of the collection.
+        :param str project_id: The Universally Unique Identifier (UUID) of the
+               project. This information can be found from the *Integrate and Deploy* page
+               in Discovery.
+        :param str collection_id: The Universally Unique Identifier (UUID) of the
+               collection.
         :param BinaryIO file: (optional) **Add a document**: The content of the
                document to ingest. For the supported file types and maximum supported file
                size limits when adding a document, see [the
                documentation](/docs/discovery-data?topic=discovery-data-collections#supportedfiletypes).
                **Analyze a document**: The content of the document to analyze but not
                ingest. Only the `application/json` content type is supported by the
                Analyze API. For maximum supported file size limits, see [the product
@@ -4065,15 +4154,16 @@
         return not self == other
 
 
 class Collection:
     """
     A collection for storing documents.
 
-    :param str collection_id: (optional) The unique identifier of the collection.
+    :param str collection_id: (optional) The Universally Unique Identifier (UUID) of
+          the collection.
     :param str name: (optional) The name of the collection.
     """
 
     def __init__(
         self,
         *,
         collection_id: Optional[str] = None,
@@ -4131,21 +4221,25 @@
         return not self == other
 
 
 class CollectionDetails:
     """
     A collection for storing documents.
 
-    :param str collection_id: (optional) The unique identifier of the collection.
+    :param str collection_id: (optional) The Universally Unique Identifier (UUID) of
+          the collection.
     :param str name: The name of the collection.
     :param str description: (optional) A description of the collection.
     :param datetime created: (optional) The date that the collection was created.
     :param str language: (optional) The language of the collection. For a list of
           supported languages, see the [product
           documentation](/docs/discovery-data?topic=discovery-data-language-support).
+    :param bool ocr_enabled: (optional) If set to `true`, optical character
+          recognition (OCR) is enabled. For more information, see [Optical character
+          recognition](/docs/discovery-data?topic=discovery-data-collections#ocr).
     :param List[CollectionEnrichment] enrichments: (optional) An array of
           enrichments that are applied to this collection. To get a list of enrichments
           that are available for a project, use the [List enrichments](#listenrichments)
           method.
           If no enrichments are specified when the collection is created, the default
           enrichments for the project type are applied. For more information about project
           default settings, see the [product
@@ -4159,40 +4253,45 @@
         self,
         name: str,
         *,
         collection_id: Optional[str] = None,
         description: Optional[str] = None,
         created: Optional[datetime] = None,
         language: Optional[str] = None,
+        ocr_enabled: Optional[bool] = None,
         enrichments: Optional[List['CollectionEnrichment']] = None,
         smart_document_understanding: Optional[
             'CollectionDetailsSmartDocumentUnderstanding'] = None,
     ) -> None:
         """
         Initialize a CollectionDetails object.
 
         :param str name: The name of the collection.
         :param str description: (optional) A description of the collection.
         :param str language: (optional) The language of the collection. For a list
                of supported languages, see the [product
                documentation](/docs/discovery-data?topic=discovery-data-language-support).
+        :param bool ocr_enabled: (optional) If set to `true`, optical character
+               recognition (OCR) is enabled. For more information, see [Optical character
+               recognition](/docs/discovery-data?topic=discovery-data-collections#ocr).
         :param List[CollectionEnrichment] enrichments: (optional) An array of
                enrichments that are applied to this collection. To get a list of
                enrichments that are available for a project, use the [List
                enrichments](#listenrichments) method.
                If no enrichments are specified when the collection is created, the default
                enrichments for the project type are applied. For more information about
                project default settings, see the [product
                documentation](/docs/discovery-data?topic=discovery-data-project-defaults).
         """
         self.collection_id = collection_id
         self.name = name
         self.description = description
         self.created = created
         self.language = language
+        self.ocr_enabled = ocr_enabled
         self.enrichments = enrichments
         self.smart_document_understanding = smart_document_understanding
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'CollectionDetails':
         """Initialize a CollectionDetails object from a json dictionary."""
         args = {}
@@ -4206,14 +4305,16 @@
             )
         if (description := _dict.get('description')) is not None:
             args['description'] = description
         if (created := _dict.get('created')) is not None:
             args['created'] = string_to_datetime(created)
         if (language := _dict.get('language')) is not None:
             args['language'] = language
+        if (ocr_enabled := _dict.get('ocr_enabled')) is not None:
+            args['ocr_enabled'] = ocr_enabled
         if (enrichments := _dict.get('enrichments')) is not None:
             args['enrichments'] = [
                 CollectionEnrichment.from_dict(v) for v in enrichments
             ]
         if (smart_document_understanding :=
                 _dict.get('smart_document_understanding')) is not None:
             args[
@@ -4236,14 +4337,16 @@
             _dict['name'] = self.name
         if hasattr(self, 'description') and self.description is not None:
             _dict['description'] = self.description
         if hasattr(self, 'created') and getattr(self, 'created') is not None:
             _dict['created'] = datetime_to_string(getattr(self, 'created'))
         if hasattr(self, 'language') and self.language is not None:
             _dict['language'] = self.language
+        if hasattr(self, 'ocr_enabled') and self.ocr_enabled is not None:
+            _dict['ocr_enabled'] = self.ocr_enabled
         if hasattr(self, 'enrichments') and self.enrichments is not None:
             enrichments_list = []
             for v in self.enrichments:
                 if isinstance(v, dict):
                     enrichments_list.append(v)
                 else:
                     enrichments_list.append(v.to_dict())
@@ -5945,16 +6048,16 @@
         return not self == other
 
 
 class DocumentClassifier:
     """
     Information about a document classifier.
 
-    :param str classifier_id: (optional) A unique identifier of the document
-          classifier.
+    :param str classifier_id: (optional) The Universally Unique Identifier (UUID) of
+          the document classifier.
     :param str name: A human-readable name of the document classifier.
     :param str description: (optional) A description of the document classifier.
     :param datetime created: (optional) The date that the document classifier was
           created.
     :param str language: (optional) The language of the training data that is
           associated with the document classifier. Language is specified by using the ISO
           639-1 language code, such as `en` for English or `ja` for Japanese.
@@ -6139,28 +6242,30 @@
 
 
 class DocumentClassifierEnrichment:
     """
     An object that describes enrichments that are applied to the training and test data
     that is used by the document classifier.
 
-    :param str enrichment_id: A unique identifier of the enrichment.
+    :param str enrichment_id: The Universally Unique Identifier (UUID) of the
+          enrichment.
     :param List[str] fields: An array of field names where the enrichment is
           applied.
     """
 
     def __init__(
         self,
         enrichment_id: str,
         fields: List[str],
     ) -> None:
         """
         Initialize a DocumentClassifierEnrichment object.
 
-        :param str enrichment_id: A unique identifier of the enrichment.
+        :param str enrichment_id: The Universally Unique Identifier (UUID) of the
+               enrichment.
         :param List[str] fields: An array of field names where the enrichment is
                applied.
         """
         self.enrichment_id = enrichment_id
         self.fields = fields
 
     @classmethod
@@ -6214,16 +6319,16 @@
         return not self == other
 
 
 class DocumentClassifierModel:
     """
     Information about a document classifier model.
 
-    :param str model_id: (optional) A unique identifier of the document classifier
-          model.
+    :param str model_id: (optional) The Universally Unique Identifier (UUID) of the
+          document classifier model.
     :param str name: A human-readable name of the document classifier model.
     :param str description: (optional) A description of the document classifier
           model.
     :param datetime created: (optional) The date that the document classifier model
           was created.
     :param datetime updated: (optional) The date that the document classifier model
           was last updated.
@@ -6231,16 +6336,16 @@
           training data that is used to train the document classifier model.
     :param str test_data_file: (optional) Name of the CSV file that contains data
           that is used to test the document classifier model. If no test data is provided,
           a subset of the training data is used for testing purposes.
     :param str status: (optional) The status of the training run.
     :param ClassifierModelEvaluation evaluation: (optional) An object that contains
           information about a trained document classifier model.
-    :param str enrichment_id: (optional) A unique identifier of the enrichment that
-          is generated by this document classifier model.
+    :param str enrichment_id: (optional) The Universally Unique Identifier (UUID) of
+          the enrichment that is generated by this document classifier model.
     :param datetime deployed_at: (optional) The date that the document classifier
           model was deployed.
     """
 
     def __init__(
         self,
         name: str,
@@ -6267,16 +6372,17 @@
                model.
         :param str test_data_file: (optional) Name of the CSV file that contains
                data that is used to test the document classifier model. If no test data is
                provided, a subset of the training data is used for testing purposes.
         :param str status: (optional) The status of the training run.
         :param ClassifierModelEvaluation evaluation: (optional) An object that
                contains information about a trained document classifier model.
-        :param str enrichment_id: (optional) A unique identifier of the enrichment
-               that is generated by this document classifier model.
+        :param str enrichment_id: (optional) The Universally Unique Identifier
+               (UUID) of the enrichment that is generated by this document classifier
+               model.
         """
         self.model_id = model_id
         self.name = name
         self.description = description
         self.created = created
         self.updated = updated
         self.training_data_file = training_data_file
@@ -6771,15 +6877,16 @@
         return not self == other
 
 
 class Enrichment:
     """
     Information about a specific enrichment.
 
-    :param str enrichment_id: (optional) The unique identifier of this enrichment.
+    :param str enrichment_id: (optional) The Universally Unique Identifier (UUID) of
+          this enrichment.
     :param str name: (optional) The human readable name for this enrichment.
     :param str description: (optional) The description of this enrichment.
     :param str type: (optional) The type of this enrichment.
     :param EnrichmentOptions options: (optional) An object that contains options for
           the current enrichment. Starting with version `2020-08-30`, the enrichment
           options are not included in responses from the List Enrichments method.
     """
@@ -6902,20 +7009,20 @@
           `regular_expression`. Not valid when creating any other type of enrichment.
     :param str regular_expression: (optional) The regular expression to apply for
           this enrichment. Required when **type** is `regular_expression`. Not valid when
           creating any other type of enrichment.
     :param str result_field: (optional) The name of the result document field that
           this enrichment creates. Required when **type** is `rule_based` or `classifier`.
           Not valid when creating any other type of enrichment.
-    :param str classifier_id: (optional) A unique identifier of the document
-          classifier. Required when **type** is `classifier`. Not valid when creating any
-          other type of enrichment.
-    :param str model_id: (optional) A unique identifier of the document classifier
-          model. Required when **type** is `classifier`. Not valid when creating any other
-          type of enrichment.
+    :param str classifier_id: (optional) The Universally Unique Identifier (UUID) of
+          the document classifier. Required when **type** is `classifier`. Not valid when
+          creating any other type of enrichment.
+    :param str model_id: (optional) The Universally Unique Identifier (UUID) of the
+          document classifier model. Required when **type** is `classifier`. Not valid
+          when creating any other type of enrichment.
     :param float confidence_threshold: (optional) Specifies a threshold. Only
           classes with evaluation confidence scores that are higher than the specified
           threshold are included in the output. Optional when **type** is `classifier`.
           Not valid when creating any other type of enrichment.
     :param int top_k: (optional) Evaluates only the classes that fall in the top set
           of results when ranked by confidence. For example, if set to `5`, then the top
           five classes for each document are evaluated. If set to 0, the
@@ -6974,20 +7081,20 @@
                type of enrichment.
         :param str regular_expression: (optional) The regular expression to apply
                for this enrichment. Required when **type** is `regular_expression`. Not
                valid when creating any other type of enrichment.
         :param str result_field: (optional) The name of the result document field
                that this enrichment creates. Required when **type** is `rule_based` or
                `classifier`. Not valid when creating any other type of enrichment.
-        :param str classifier_id: (optional) A unique identifier of the document
-               classifier. Required when **type** is `classifier`. Not valid when creating
-               any other type of enrichment.
-        :param str model_id: (optional) A unique identifier of the document
-               classifier model. Required when **type** is `classifier`. Not valid when
-               creating any other type of enrichment.
+        :param str classifier_id: (optional) The Universally Unique Identifier
+               (UUID) of the document classifier. Required when **type** is `classifier`.
+               Not valid when creating any other type of enrichment.
+        :param str model_id: (optional) The Universally Unique Identifier (UUID) of
+               the document classifier model. Required when **type** is `classifier`. Not
+               valid when creating any other type of enrichment.
         :param float confidence_threshold: (optional) Specifies a threshold. Only
                classes with evaluation confidence scores that are higher than the
                specified threshold are included in the output. Optional when **type** is
                `classifier`. Not valid when creating any other type of enrichment.
         :param int top_k: (optional) Evaluates only the classes that fall in the
                top set of results when ranked by confidence. For example, if set to `5`,
                then the top five classes for each document are evaluated. If set to 0, the
@@ -8181,21 +8288,24 @@
         return not self == other
 
 
 class ProjectDetails:
     """
     Detailed information about the specified project.
 
-    :param str project_id: (optional) The unique identifier of this project.
+    :param str project_id: (optional) The Universally Unique Identifier (UUID) of
+          this project.
     :param str name: (optional) The human readable name of this project.
     :param str type: (optional) The type of project.
           The `content_intelligence` type is a *Document Retrieval for Contracts* project
           and the `other` type is a *Custom* project.
           The `content_mining` and `content_intelligence` types are available with Premium
           plan managed deployments and installed deployments only.
+          The Intelligent Document Processing (IDP) project type is available from IBM
+          Cloud-managed instances only.
     :param ProjectListDetailsRelevancyTrainingStatus relevancy_training_status:
           (optional) Relevancy training status information for this project.
     :param int collection_count: (optional) The number of collections configured in
           this project.
     :param DefaultQueryParams default_query_parameters: (optional) Default query
           parameters for this project.
     """
@@ -8216,14 +8326,16 @@
 
         :param str name: (optional) The human readable name of this project.
         :param str type: (optional) The type of project.
                The `content_intelligence` type is a *Document Retrieval for Contracts*
                project and the `other` type is a *Custom* project.
                The `content_mining` and `content_intelligence` types are available with
                Premium plan managed deployments and installed deployments only.
+               The Intelligent Document Processing (IDP) project type is available from
+               IBM Cloud-managed instances only.
         :param DefaultQueryParams default_query_parameters: (optional) Default
                query parameters for this project.
         """
         self.project_id = project_id
         self.name = name
         self.type = type
         self.relevancy_training_status = relevancy_training_status
@@ -8311,34 +8423,40 @@
     class TypeEnum(str, Enum):
         """
         The type of project.
         The `content_intelligence` type is a *Document Retrieval for Contracts* project
         and the `other` type is a *Custom* project.
         The `content_mining` and `content_intelligence` types are available with Premium
         plan managed deployments and installed deployments only.
+        The Intelligent Document Processing (IDP) project type is available from IBM
+        Cloud-managed instances only.
         """
 
+        INTELLIGENT_DOCUMENT_PROCESSING = 'intelligent_document_processing'
         DOCUMENT_RETRIEVAL = 'document_retrieval'
         CONVERSATIONAL_SEARCH = 'conversational_search'
         CONTENT_MINING = 'content_mining'
         CONTENT_INTELLIGENCE = 'content_intelligence'
         OTHER = 'other'
 
 
 class ProjectListDetails:
     """
     Details about a specific project.
 
-    :param str project_id: (optional) The unique identifier of this project.
+    :param str project_id: (optional) The Universally Unique Identifier (UUID) of
+          this project.
     :param str name: (optional) The human readable name of this project.
     :param str type: (optional) The type of project.
           The `content_intelligence` type is a *Document Retrieval for Contracts* project
           and the `other` type is a *Custom* project.
           The `content_mining` and `content_intelligence` types are available with Premium
           plan managed deployments and installed deployments only.
+          The Intelligent Document Processing (IDP) project type is available from IBM
+          Cloud-managed instances only.
     :param ProjectListDetailsRelevancyTrainingStatus relevancy_training_status:
           (optional) Relevancy training status information for this project.
     :param int collection_count: (optional) The number of collections configured in
           this project.
     """
 
     def __init__(
@@ -8356,14 +8474,16 @@
 
         :param str name: (optional) The human readable name of this project.
         :param str type: (optional) The type of project.
                The `content_intelligence` type is a *Document Retrieval for Contracts*
                project and the `other` type is a *Custom* project.
                The `content_mining` and `content_intelligence` types are available with
                Premium plan managed deployments and installed deployments only.
+               The Intelligent Document Processing (IDP) project type is available from
+               IBM Cloud-managed instances only.
         """
         self.project_id = project_id
         self.name = name
         self.type = type
         self.relevancy_training_status = relevancy_training_status
         self.collection_count = collection_count
 
@@ -8435,16 +8555,19 @@
     class TypeEnum(str, Enum):
         """
         The type of project.
         The `content_intelligence` type is a *Document Retrieval for Contracts* project
         and the `other` type is a *Custom* project.
         The `content_mining` and `content_intelligence` types are available with Premium
         plan managed deployments and installed deployments only.
+        The Intelligent Document Processing (IDP) project type is available from IBM
+        Cloud-managed instances only.
         """
 
+        INTELLIGENT_DOCUMENT_PROCESSING = 'intelligent_document_processing'
         DOCUMENT_RETRIEVAL = 'document_retrieval'
         CONVERSATIONAL_SEARCH = 'conversational_search'
         CONTENT_MINING = 'content_mining'
         CONTENT_INTELLIGENCE = 'content_intelligence'
         OTHER = 'other'
```

### Comparing `ibm-watson-8.0.0/ibm_watson/language_translator_v3.py` & `ibm_watson-8.1.0/ibm_watson/language_translator_v3.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/natural_language_understanding_v1.py` & `ibm_watson-8.1.0/ibm_watson/natural_language_understanding_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/speech_to_text_v1.py` & `ibm_watson-8.1.0/ibm_watson/speech_to_text_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 terms `Broadband` and `Narrowband` in their names, and next-generation models that include
 the terms `Multimedia` and `Telephony` in their names. Broadband and multimedia models
 have minimum sampling rates of 16 kHz. Narrowband and telephony models have minimum
 sampling rates of 8 kHz. The next-generation models offer high throughput and greater
 transcription accuracy.
 Effective **31 July 2023**, all previous-generation models will be removed from the
 service and the documentation. Most previous-generation models were deprecated on 15 March
-2022. You must migrate to the equivalent next-generation model by 31 July 2023. For more
-information, see [Migrating to next-generation
+2022. You must migrate to the equivalent large speech model or next-generation model by 31
+July 2023. For more information, see [Migrating to large speech
 models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-migrate).{:
 deprecated}
 For speech recognition, the service supports synchronous and asynchronous HTTP
 Representational State Transfer (REST) interfaces. It also supports a WebSocket interface
 that provides a full-duplex, low-latency communication channel: Clients send requests and
 audio to the service and receive results over a single connection asynchronously.
 The service also offers two customization interfaces. Use language model customization to
@@ -192,28 +192,29 @@
 
     def recognize(
         self,
         audio: BinaryIO,
         *,
         content_type: Optional[str] = None,
         model: Optional[str] = None,
+        speech_begin_event: Optional[bool] = None,
         language_customization_id: Optional[str] = None,
         acoustic_customization_id: Optional[str] = None,
         base_model_version: Optional[str] = None,
         customization_weight: Optional[float] = None,
         inactivity_timeout: Optional[int] = None,
         keywords: Optional[List[str]] = None,
         keywords_threshold: Optional[float] = None,
         max_alternatives: Optional[int] = None,
         word_alternatives_threshold: Optional[float] = None,
         word_confidence: Optional[bool] = None,
         timestamps: Optional[bool] = None,
         profanity_filter: Optional[bool] = None,
         smart_formatting: Optional[bool] = None,
-        smart_formatting_version: Optional[bool] = None,
+        smart_formatting_version: Optional[int] = None,
         speaker_labels: Optional[bool] = None,
         grammar_name: Optional[str] = None,
         redaction: Optional[bool] = None,
         audio_metrics: Optional[bool] = None,
         end_of_phrase_silence_time: Optional[float] = None,
         split_transcript_at_phrase_end: Optional[bool] = None,
         speech_detector_sensitivity: Optional[float] = None,
@@ -277,39 +278,44 @@
         recognition request: for broadband models, at least 16 kHz; for narrowband models,
         at least 8 kHz. If the sampling rate of the audio is higher than the minimum
         required rate, the service down-samples the audio to the appropriate rate. If the
         sampling rate of the audio is lower than the minimum required rate, the request
         fails.
          **See also:** [Supported audio
         formats](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-audio-formats).
-        ### Next-generation models
-         The service supports next-generation `Multimedia` (16 kHz) and `Telephony` (8
-        kHz) models for many languages. Next-generation models have higher throughput than
-        the service's previous generation of `Broadband` and `Narrowband` models. When you
-        use next-generation models, the service can return transcriptions more quickly and
-        also provide noticeably better transcription accuracy.
-        You specify a next-generation model by using the `model` query parameter, as you
-        do a previous-generation model. Most next-generation models support the
-        `low_latency` parameter, and all next-generation models support the
-        `character_insertion_bias` parameter. These parameters are not available with
-        previous-generation models.
-        Next-generation models do not support all of the speech recognition parameters
-        that are available for use with previous-generation models. Next-generation models
-        do not support the following parameters:
+        ### Large speech models and Next-generation models
+         The service supports large speech models and next-generation `Multimedia` (16
+        kHz) and `Telephony` (8 kHz) models for many languages. Large speech models and
+        next-generation models have higher throughput than the service's previous
+        generation of `Broadband` and `Narrowband` models. When you use large speech
+        models and next-generation models, the service can return transcriptions more
+        quickly and also provide noticeably better transcription accuracy.
+        You specify a large speech model or next-generation model by using the `model`
+        query parameter, as you do a previous-generation model. Only the next-generation
+        models support the `low_latency` parameter, and all large speech models and
+        next-generation models support the `character_insertion_bias` parameter. These
+        parameters are not available with previous-generation models.
+        Large speech models and next-generation models do not support all of the speech
+        recognition parameters that are available for use with previous-generation models.
+        Next-generation models do not support the following parameters:
         * `acoustic_customization_id`
         * `keywords` and `keywords_threshold`
         * `processing_metrics` and `processing_metrics_interval`
         * `word_alternatives_threshold`
         **Important:** Effective **31 July 2023**, all previous-generation models will be
         removed from the service and the documentation. Most previous-generation models
-        were deprecated on 15 March 2022. You must migrate to the equivalent
-        next-generation model by 31 July 2023. For more information, see [Migrating to
-        next-generation
+        were deprecated on 15 March 2022. You must migrate to the equivalent large speech
+        model or next-generation model by 31 July 2023. For more information, see
+        [Migrating to large speech
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-migrate).
         **See also:**
+        * [Large speech languages and
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-large-speech-languages)
+        * [Supported features for large speech
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-large-speech-languages#models-lsm-supported-features)
         * [Next-generation languages and
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng)
         * [Supported features for next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng#models-ng-features)
         ### Multipart speech recognition
          **Note:** The asynchronous HTTP interface, WebSocket interface, and Watson SDKs
         do not support multipart speech recognition.
@@ -336,14 +342,22 @@
                `en-US_BroadbandModel`, you must either specify a model with the request or
                specify a new default model for your installation of the service.
                **See also:**
                * [Using a model for speech
                recognition](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-use)
                * [Using the default
                model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-use#models-use-default).
+        :param bool speech_begin_event: (optional) If `true`, the service returns a
+               response object `SpeechActivity` which contains the time when a speech
+               activity is detected in the stream. This can be used both in standard and
+               low latency mode. This feature enables client applications to know that
+               some words/speech has been detected and the service is in the process of
+               decoding. This can be used in lieu of interim results in standard mode. See
+               [Using speech recognition
+               parameters](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-service-features#features-parameters).
         :param str language_customization_id: (optional) The customization ID
                (GUID) of a custom language model that is to be used with the recognition
                request. The base model of the specified custom language model must match
                the model specified with the `model` parameter. You must make the request
                with credentials for the instance of the service that owns the custom
                model. By default, no custom language model is used. See [Using a custom
                language model for speech
@@ -370,14 +384,15 @@
                customization ID (GUID) of a custom language model with the recognition
                request, the customization weight tells the service how much weight to give
                to words from the custom language model compared to those from the base
                model for the current request.
                Specify a value between 0.0 and 1.0. Unless a different customization
                weight was specified for the custom model when the model was trained, the
                default value is:
+               * 0.5 for large speech models
                * 0.3 for previous-generation models
                * 0.2 for most next-generation models
                * 0.1 for next-generation English and Japanese models
                A customization weight that you specify overrides a weight that was
                specified when the custom model was trained. The default value yields the
                best performance in general. Assign a higher value if your audio makes
                frequent use of OOV words from the custom model. Use caution when setting
@@ -443,29 +458,29 @@
                the final transcript of a recognition request. For US English, the service
                also converts certain keyword strings to punctuation symbols. By default,
                the service performs no smart formatting.
                **Note:** The parameter can be used with US English, Japanese, and Spanish
                (all dialects) transcription only.
                See [Smart
                formatting](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-formatting#smart-formatting).
-        :param bool smart_formatting_version: (optional) Smart formatting version
-               is for next-generation models and that is supported in US English,
-               Brazilian Portuguese, French and German languages.
+        :param int smart_formatting_version: (optional) Smart formatting version
+               for large speech models and next-generation models is supported in US
+               English, Brazilian Portuguese, French, German, Spanish and French Canadian
+               languages.
         :param bool speaker_labels: (optional) If `true`, the response includes
                labels that identify which words were spoken by which participants in a
                multi-person exchange. By default, the service returns no speaker labels.
                Setting `speaker_labels` to `true` forces the `timestamps` parameter to be
                `true`, regardless of whether you specify `false` for the parameter.
                * _For previous-generation models,_ the parameter can be used with
                Australian English, US English, German, Japanese, Korean, and Spanish (both
                broadband and narrowband models) and UK English (narrowband model)
                transcription only.
-               * _For next-generation models,_ the parameter can be used with Czech,
-               English (Australian, Indian, UK, and US), German, Japanese, Korean, and
-               Spanish transcription only.
+               * _For large speech models and next-generation models,_ the parameter can
+               be used with all available languages.
                See [Speaker
                labels](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-speaker-labels).
         :param str grammar_name: (optional) The name of a grammar that is to be
                used with the recognition request. If you specify a grammar, you must also
                use the `language_customization_id` parameter to specify the name of the
                custom language model for which the grammar is defined. The service
                recognizes only strings that are recognized by the specified grammar; it
@@ -531,16 +546,16 @@
                * 0.0 suppresses all audio (no speech is transcribed).
                * 0.5 (the default) provides a reasonable compromise for the level of
                sensitivity.
                * 1.0 suppresses no audio (speech detection sensitivity is disabled).
                The values increase on a monotonic curve. Specifying one or two decimal
                places of precision (for example, `0.55`) is typically more than
                sufficient.
-               The parameter is supported with all next-generation models and with most
-               previous-generation models. See [Speech detector
+               The parameter is supported with all large speech models, next-generation
+               models and with most previous-generation models. See [Speech detector
                sensitivity](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-parameters-sensitivity)
                and [Language model
                support](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-support).
         :param float background_audio_suppression: (optional) The level to which
                the service is to suppress background audio based on its volume to prevent
                it from being transcribed as speech. Use the parameter to suppress side
                conversations or background noise.
@@ -548,38 +563,39 @@
                * 0.0 (the default) provides no suppression (background audio suppression
                is disabled).
                * 0.5 provides a reasonable level of audio suppression for general usage.
                * 1.0 suppresses all audio (no audio is transcribed).
                The values increase on a monotonic curve. Specifying one or two decimal
                places of precision (for example, `0.55`) is typically more than
                sufficient.
-               The parameter is supported with all next-generation models and with most
-               previous-generation models. See [Background audio
+               The parameter is supported with all large speech models, next-generation
+               models and with most previous-generation models. See [Background audio
                suppression](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-parameters-suppression)
                and [Language model
                support](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-support).
         :param bool low_latency: (optional) If `true` for next-generation
                `Multimedia` and `Telephony` models that support low latency, directs the
                service to produce results even more quickly than it usually does.
                Next-generation models produce transcription results faster than
                previous-generation models. The `low_latency` parameter causes the models
                to produce results even more quickly, though the results might be less
                accurate when the parameter is used.
-               The parameter is not available for previous-generation `Broadband` and
-               `Narrowband` models. It is available for most next-generation models.
+               The parameter is not available for large speech models and
+               previous-generation `Broadband` and `Narrowband` models. It is available
+               for most next-generation models.
                * For a list of next-generation models that support low latency, see
                [Supported next-generation language
                models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng#models-ng-supported).
                * For more information about the `low_latency` parameter, see [Low
                latency](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-interim#low-latency).
-        :param float character_insertion_bias: (optional) For next-generation
-               models, an indication of whether the service is biased to recognize shorter
-               or longer strings of characters when developing transcription hypotheses.
-               By default, the service is optimized to produce the best balance of strings
-               of different lengths.
+        :param float character_insertion_bias: (optional) For large speech models
+               and next-generation models, an indication of whether the service is biased
+               to recognize shorter or longer strings of characters when developing
+               transcription hypotheses. By default, the service is optimized to produce
+               the best balance of strings of different lengths.
                The default bias is 0.0. The allowable range of values is -1.0 to 1.0.
                * Negative values bias the service to favor hypotheses with shorter strings
                of characters.
                * Positive values bias the service to favor hypotheses with longer strings
                of characters.
                As the value approaches -1.0 or 1.0, the impact of the parameter becomes
                more pronounced. To determine the most effective value for your scenario,
@@ -605,14 +621,15 @@
             service_version='V1',
             operation_id='recognize',
         )
         headers.update(sdk_headers)
 
         params = {
             'model': model,
+            'speech_begin_event': speech_begin_event,
             'language_customization_id': language_customization_id,
             'acoustic_customization_id': acoustic_customization_id,
             'base_model_version': base_model_version,
             'customization_weight': customization_weight,
             'inactivity_timeout': inactivity_timeout,
             'keywords': convert_list(keywords),
             'keywords_threshold': keywords_threshold,
@@ -814,15 +831,15 @@
         keywords_threshold: Optional[float] = None,
         max_alternatives: Optional[int] = None,
         word_alternatives_threshold: Optional[float] = None,
         word_confidence: Optional[bool] = None,
         timestamps: Optional[bool] = None,
         profanity_filter: Optional[bool] = None,
         smart_formatting: Optional[bool] = None,
-        smart_formatting_version: Optional[bool] = None,
+        smart_formatting_version: Optional[int] = None,
         speaker_labels: Optional[bool] = None,
         grammar_name: Optional[str] = None,
         redaction: Optional[bool] = None,
         processing_metrics: Optional[bool] = None,
         processing_metrics_interval: Optional[float] = None,
         audio_metrics: Optional[bool] = None,
         end_of_phrase_silence_time: Optional[float] = None,
@@ -914,39 +931,44 @@
         recognition request: for broadband models, at least 16 kHz; for narrowband models,
         at least 8 kHz. If the sampling rate of the audio is higher than the minimum
         required rate, the service down-samples the audio to the appropriate rate. If the
         sampling rate of the audio is lower than the minimum required rate, the request
         fails.
          **See also:** [Supported audio
         formats](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-audio-formats).
-        ### Next-generation models
-         The service supports next-generation `Multimedia` (16 kHz) and `Telephony` (8
-        kHz) models for many languages. Next-generation models have higher throughput than
-        the service's previous generation of `Broadband` and `Narrowband` models. When you
-        use next-generation models, the service can return transcriptions more quickly and
-        also provide noticeably better transcription accuracy.
-        You specify a next-generation model by using the `model` query parameter, as you
-        do a previous-generation model. Most next-generation models support the
-        `low_latency` parameter, and all next-generation models support the
-        `character_insertion_bias` parameter. These parameters are not available with
-        previous-generation models.
-        Next-generation models do not support all of the speech recognition parameters
-        that are available for use with previous-generation models. Next-generation models
-        do not support the following parameters:
+        ### Large speech models and Next-generation models
+         The service supports large speech models and next-generation `Multimedia` (16
+        kHz) and `Telephony` (8 kHz) models for many languages. Large speech models and
+        next-generation models have higher throughput than the service's previous
+        generation of `Broadband` and `Narrowband` models. When you use large speech
+        models and next-generation models, the service can return transcriptions more
+        quickly and also provide noticeably better transcription accuracy.
+        You specify a large speech model or next-generation model by using the `model`
+        query parameter, as you do a previous-generation model. Only the next-generation
+        models support the `low_latency` parameter, and all large speech models and
+        next-generation models support the `character_insertion_bias` parameter. These
+        parameters are not available with previous-generation models.
+        Large speech models and next-generation models do not support all of the speech
+        recognition parameters that are available for use with previous-generation models.
+        Next-generation models do not support the following parameters:
         * `acoustic_customization_id`
         * `keywords` and `keywords_threshold`
         * `processing_metrics` and `processing_metrics_interval`
         * `word_alternatives_threshold`
         **Important:** Effective **31 July 2023**, all previous-generation models will be
         removed from the service and the documentation. Most previous-generation models
-        were deprecated on 15 March 2022. You must migrate to the equivalent
-        next-generation model by 31 July 2023. For more information, see [Migrating to
-        next-generation
+        were deprecated on 15 March 2022. You must migrate to the equivalent large speech
+        model or next-generation model by 31 July 2023. For more information, see
+        [Migrating to large speech
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-migrate).
         **See also:**
+        * [Large speech languages and
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-large-speech-languages)
+        * [Supported features for large speech
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-large-speech-languages#models-lsm-supported-features)
         * [Next-generation languages and
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng)
         * [Supported features for next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng#models-ng-features).
 
         :param BinaryIO audio: The audio to transcribe.
         :param str content_type: (optional) The format (MIME type) of the audio.
@@ -1029,14 +1051,15 @@
                customization ID (GUID) of a custom language model with the recognition
                request, the customization weight tells the service how much weight to give
                to words from the custom language model compared to those from the base
                model for the current request.
                Specify a value between 0.0 and 1.0. Unless a different customization
                weight was specified for the custom model when the model was trained, the
                default value is:
+               * 0.5 for large speech models
                * 0.3 for previous-generation models
                * 0.2 for most next-generation models
                * 0.1 for next-generation English and Japanese models
                A customization weight that you specify overrides a weight that was
                specified when the custom model was trained. The default value yields the
                best performance in general. Assign a higher value if your audio makes
                frequent use of OOV words from the custom model. Use caution when setting
@@ -1102,29 +1125,29 @@
                the final transcript of a recognition request. For US English, the service
                also converts certain keyword strings to punctuation symbols. By default,
                the service performs no smart formatting.
                **Note:** The parameter can be used with US English, Japanese, and Spanish
                (all dialects) transcription only.
                See [Smart
                formatting](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-formatting#smart-formatting).
-        :param bool smart_formatting_version: (optional) Smart formatting version
-               is for next-generation models and that is supported in US English,
-               Brazilian Portuguese, French and German languages.
+        :param int smart_formatting_version: (optional) Smart formatting version
+               for large speech models and next-generation models is supported in US
+               English, Brazilian Portuguese, French, German, Spanish and French Canadian
+               languages.
         :param bool speaker_labels: (optional) If `true`, the response includes
                labels that identify which words were spoken by which participants in a
                multi-person exchange. By default, the service returns no speaker labels.
                Setting `speaker_labels` to `true` forces the `timestamps` parameter to be
                `true`, regardless of whether you specify `false` for the parameter.
                * _For previous-generation models,_ the parameter can be used with
                Australian English, US English, German, Japanese, Korean, and Spanish (both
                broadband and narrowband models) and UK English (narrowband model)
                transcription only.
-               * _For next-generation models,_ the parameter can be used with Czech,
-               English (Australian, Indian, UK, and US), German, Japanese, Korean, and
-               Spanish transcription only.
+               * _For large speech models and next-generation models,_ the parameter can
+               be used with all available languages.
                See [Speaker
                labels](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-speaker-labels).
         :param str grammar_name: (optional) The name of a grammar that is to be
                used with the recognition request. If you specify a grammar, you must also
                use the `language_customization_id` parameter to specify the name of the
                custom language model for which the grammar is defined. The service
                recognizes only strings that are recognized by the specified grammar; it
@@ -1212,16 +1235,16 @@
                * 0.0 suppresses all audio (no speech is transcribed).
                * 0.5 (the default) provides a reasonable compromise for the level of
                sensitivity.
                * 1.0 suppresses no audio (speech detection sensitivity is disabled).
                The values increase on a monotonic curve. Specifying one or two decimal
                places of precision (for example, `0.55`) is typically more than
                sufficient.
-               The parameter is supported with all next-generation models and with most
-               previous-generation models. See [Speech detector
+               The parameter is supported with all large speech models, next-generation
+               models and with most previous-generation models. See [Speech detector
                sensitivity](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-parameters-sensitivity)
                and [Language model
                support](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-support).
         :param float background_audio_suppression: (optional) The level to which
                the service is to suppress background audio based on its volume to prevent
                it from being transcribed as speech. Use the parameter to suppress side
                conversations or background noise.
@@ -1229,38 +1252,39 @@
                * 0.0 (the default) provides no suppression (background audio suppression
                is disabled).
                * 0.5 provides a reasonable level of audio suppression for general usage.
                * 1.0 suppresses all audio (no audio is transcribed).
                The values increase on a monotonic curve. Specifying one or two decimal
                places of precision (for example, `0.55`) is typically more than
                sufficient.
-               The parameter is supported with all next-generation models and with most
-               previous-generation models. See [Background audio
+               The parameter is supported with all large speech models, next-generation
+               models and with most previous-generation models. See [Background audio
                suppression](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-parameters-suppression)
                and [Language model
                support](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-support).
         :param bool low_latency: (optional) If `true` for next-generation
                `Multimedia` and `Telephony` models that support low latency, directs the
                service to produce results even more quickly than it usually does.
                Next-generation models produce transcription results faster than
                previous-generation models. The `low_latency` parameter causes the models
                to produce results even more quickly, though the results might be less
                accurate when the parameter is used.
-               The parameter is not available for previous-generation `Broadband` and
-               `Narrowband` models. It is available for most next-generation models.
+               The parameter is not available for large speech models and
+               previous-generation `Broadband` and `Narrowband` models. It is available
+               for most next-generation models.
                * For a list of next-generation models that support low latency, see
                [Supported next-generation language
                models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng#models-ng-supported).
                * For more information about the `low_latency` parameter, see [Low
                latency](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-interim#low-latency).
-        :param float character_insertion_bias: (optional) For next-generation
-               models, an indication of whether the service is biased to recognize shorter
-               or longer strings of characters when developing transcription hypotheses.
-               By default, the service is optimized to produce the best balance of strings
-               of different lengths.
+        :param float character_insertion_bias: (optional) For large speech models
+               and next-generation models, an indication of whether the service is biased
+               to recognize shorter or longer strings of characters when developing
+               transcription hypotheses. By default, the service is optimized to produce
+               the best balance of strings of different lengths.
                The default bias is 0.0. The allowable range of values is -1.0 to 1.0.
                * Negative values bias the service to favor hypotheses with shorter strings
                of characters.
                * Positive values bias the service to favor hypotheses with longer strings
                of characters.
                As the value approaches -1.0 or 1.0, the impact of the parameter becomes
                more pronounced. To determine the most effective value for your scenario,
@@ -1517,23 +1541,57 @@
         it.
         You can create a maximum of 1024 custom language models per owning credentials.
         The service returns an error if you attempt to create more than 1024 models. You
         do not lose any models, but you cannot create any more until your model count is
         below the limit.
         **Important:** Effective **31 July 2023**, all previous-generation models will be
         removed from the service and the documentation. Most previous-generation models
-        were deprecated on 15 March 2022. You must migrate to the equivalent
-        next-generation model by 31 July 2023. For more information, see [Migrating to
-        next-generation
+        were deprecated on 15 March 2022. You must migrate to the equivalent large speech
+        model or next-generation model by 31 July 2023. For more information, see
+        [Migrating to large speech
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-migrate).
         **See also:**
         * [Create a custom language
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-languageCreate#createModel-language)
         * [Language support for
-        customization](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-custom-support).
+        customization](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-custom-support)
+        ### Large speech models and Next-generation models
+         The service supports large speech models and next-generation `Multimedia` (16
+        kHz) and `Telephony` (8 kHz) models for many languages. Large speech models and
+        next-generation models have higher throughput than the service's previous
+        generation of `Broadband` and `Narrowband` models. When you use large speech
+        models and next-generation models, the service can return transcriptions more
+        quickly and also provide noticeably better transcription accuracy.
+        You specify a large speech model or next-generation model by using the `model`
+        query parameter, as you do a previous-generation model. Only the next-generation
+        models support the `low_latency` parameter, and all large speech models and
+        next-generation models support the `character_insertion_bias` parameter. These
+        parameters are not available with previous-generation models.
+        Large speech models and next-generation models do not support all of the speech
+        recognition parameters that are available for use with previous-generation models.
+        Next-generation models do not support the following parameters:
+        * `acoustic_customization_id`
+        * `keywords` and `keywords_threshold`
+        * `processing_metrics` and `processing_metrics_interval`
+        * `word_alternatives_threshold`
+        **Important:** Effective **31 July 2023**, all previous-generation models will be
+        removed from the service and the documentation. Most previous-generation models
+        were deprecated on 15 March 2022. You must migrate to the equivalent large speech
+        model or next-generation model by 31 July 2023. For more information, see
+        [Migrating to large speech
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-migrate).
+        **See also:**
+        * [Large speech languages and
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-large-speech-languages)
+        * [Supported features for large speech
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-large-speech-languages#models-lsm-supported-features)
+        * [Next-generation languages and
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng)
+        * [Supported features for next-generation
+        models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng#models-ng-features).
 
         :param str name: A user-defined name for the new custom language model. Use
                a localized name that matches the language of the custom model. Use a name
                that describes the domain of the custom model, such as `Medical custom
                model` or `Legal custom model`. Use a name that is unique among all custom
                language models that you own.
                Include a maximum of 256 characters in the name. Do not use backslashes,
@@ -1843,22 +1901,24 @@
                model's words resource on which to train the model:
                * `all` (the default) trains the model on all new words, regardless of
                whether they were extracted from corpora or grammars or were added or
                modified by the user.
                * `user` trains the model only on custom words that were added or modified
                by the user directly. The model is not trained on new words extracted from
                corpora or grammars.
-               _For custom models that are based on next-generation models_, the service
-               ignores the parameter. The words resource contains only custom words that
-               the user adds or modifies directly, so the parameter is unnecessary.
+               _For custom models that are based on large speech models and
+               next-generation models_, the service ignores the `word_type_to_add`
+               parameter. The words resource contains only custom words that the user adds
+               or modifies directly, so the parameter is unnecessary.
         :param float customization_weight: (optional) Specifies a customization
                weight for the custom language model. The customization weight tells the
                service how much weight to give to words from the custom language model
                compared to those from the base model for speech recognition. Specify a
                value between 0.0 and 1.0. The default value is:
+               * 0.5 for large speech models
                * 0.3 for previous-generation models
                * 0.2 for most next-generation models
                * 0.1 for next-generation English and Japanese models
                The default value yields the best performance in general. Assign a higher
                value if your audio makes frequent use of OOV words from the custom model.
                Use caution when setting the weight: a higher value can improve the
                accuracy of phrases from the custom model's domain, but it can negatively
@@ -2141,14 +2201,17 @@
         the corpus. This operation can take on the order of minutes to complete depending
         on the current load on the service, the total number of words in the corpus, and,
         _for custom models that are based on previous-generation models_, the number of
         new (out-of-vocabulary) words in the corpus. You cannot submit requests to add
         additional resources to the custom model or to train the model until the service's
         analysis of the corpus for the current request completes. Use the [Get a
         corpus](#getcorpus) method to check the status of the analysis.
+        _For custom models that are based on large speech models_, the service parses and
+        extracts word sequences from one or multiple corpora files. The characters help
+        the service learn and predict character sequences from audio.
         _For custom models that are based on previous-generation models_, the service
         auto-populates the model's words resource with words from the corpus that are not
         found in its base vocabulary. These words are referred to as out-of-vocabulary
         (OOV) words. After adding a corpus, you must validate the words resource to ensure
         that each OOV word's definition is complete and valid. You can use the [List
         custom words](#listwords) method to examine the words resource. You can use other
         words method to eliminate typos and modify how words are pronounced and displayed
@@ -2167,19 +2230,19 @@
         thousand custom (OOV) words to a model. This includes words that the service
         extracts from corpora and grammars, and words that you add directly.
         **See also:**
         * [Add a corpus to the custom language
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-languageCreate#addCorpus)
         * [Working with corpora for previous-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords#workingCorpora)
-        * [Working with corpora for next-generation
+        * [Working with corpora for large speech models and next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords-ng#workingCorpora-ng)
         * [Validating a words resource for previous-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords#validateModel)
-        * [Validating a words resource for next-generation
+        * [Validating a words resource for large speech models and next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords-ng#validateModel-ng).
 
         :param str customization_id: The customization ID (GUID) of the custom
                language model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
         :param str corpus_name: The name of the new corpus for the custom language
@@ -2539,19 +2602,19 @@
         words-related methods to correct errors, eliminate typos, and modify how words are
         pronounced as needed.
         **See also:**
         * [Add words to the custom language
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-languageCreate#addWords)
         * [Working with custom words for previous-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords#workingWords)
-        * [Working with custom words for next-generation
+        * [Working with custom words for large speech models and next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords-ng#workingWords-ng)
         * [Validating a words resource for previous-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords#validateModel)
-        * [Validating a words resource for next-generation
+        * [Validating a words resource for large speech models and next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords-ng#validateModel-ng).
 
         :param str customization_id: The customization ID (GUID) of the custom
                language model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
         :param List[CustomWord] words: An array of `CustomWord` objects that
@@ -2651,19 +2714,19 @@
         service encounters an error, it does not add the word to the words resource. Use
         the [Get a custom word](#getword) method to review the word that you add.
         **See also:**
         * [Add words to the custom language
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-languageCreate#addWords)
         * [Working with custom words for previous-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords#workingWords)
-        * [Working with custom words for next-generation
+        * [Working with custom words for large speech models and next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords-ng#workingWords-ng)
         * [Validating a words resource for previous-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords#validateModel)
-        * [Validating a words resource for next-generation
+        * [Validating a words resource for large speech models and next-generation
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-corporaWords-ng#validateModel-ng).
 
         :param str customization_id: The customization ID (GUID) of the custom
                language model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
         :param str word_name: The custom word that is to be added to or updated in
@@ -3234,20 +3297,21 @@
         model is owned by the instance of the service whose credentials are used to create
         it.
         You can create a maximum of 1024 custom acoustic models per owning credentials.
         The service returns an error if you attempt to create more than 1024 models. You
         do not lose any models, but you cannot create any more until your model count is
         below the limit.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **Important:** Effective **31 July 2023**, all previous-generation models will be
         removed from the service and the documentation. Most previous-generation models
-        were deprecated on 15 March 2022. You must migrate to the equivalent
-        next-generation model by 31 July 2023. For more information, see [Migrating to
-        next-generation
+        were deprecated on 15 March 2022. You must migrate to the equivalent large speech
+        model or next-generation model by 31 July 2023. For more information, see
+        [Migrating to large speech
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-migrate).
         **See also:** [Create a custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-acoustic#createModel-acoustic).
 
         :param str name: A user-defined name for the new custom acoustic model. Use
                a localized name that matches the language of the custom model. Use a name
                that describes the acoustic environment of the custom model, such as
@@ -3318,15 +3382,16 @@
 
         Lists information about all custom acoustic models that are owned by an instance
         of the service. Use the `language` parameter to see all custom acoustic models for
         the specified language. Omit the parameter to see all custom acoustic models for
         all languages. You must use credentials for the instance of the service that owns
         a model to list information about it.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Listing custom acoustic
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-manageAcousticModels#listModels-acoustic).
 
         :param str language: (optional) The identifier of the language for which
                custom language or custom acoustic models are to be returned. Specify the
                five-character language identifier; for example, specify `en-US` to see all
                custom language or custom acoustic models that are based on US English
@@ -3375,15 +3440,16 @@
     ) -> DetailedResponse:
         """
         Get a custom acoustic model.
 
         Gets information about a specified custom acoustic model. You must use credentials
         for the instance of the service that owns a model to list information about it.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Listing custom acoustic
         models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-manageAcousticModels#listModels-acoustic).
 
         :param str customization_id: The customization ID (GUID) of the custom
                acoustic model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
@@ -3430,15 +3496,16 @@
         Delete a custom acoustic model.
 
         Deletes an existing custom acoustic model. The custom model cannot be deleted if
         another request, such as adding an audio resource to the model, is currently being
         processed. You must use credentials for the instance of the service that owns a
         model to delete it.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Deleting a custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-manageAcousticModels#deleteModel-acoustic).
 
         :param str customization_id: The customization ID (GUID) of the custom
                acoustic model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
@@ -3514,15 +3581,16 @@
         Train with a custom language model if you have verbatim transcriptions of the
         audio files that you have added to the custom model or you have either corpora
         (text files) or a list of words that are relevant to the contents of the audio
         files. For training to succeed, both of the custom models must be based on the
         same version of the same base model, and the custom language model must be fully
         trained and available.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:**
         * [Train the custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-acoustic#trainModel-acoustic)
         * [Using custom acoustic and custom language models
         together](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-useBoth#useBoth)
         ### Training failures
          Training can fail to start for the following reasons:
@@ -3618,15 +3686,16 @@
         first created. Metadata such as the name and language of the model are preserved,
         but the model's audio resources are removed and must be re-created. The service
         cannot reset a model while it is handling another request for the model. The
         service cannot accept subsequent requests for the model until the existing reset
         request completes. You must use credentials for the instance of the service that
         owns a model to reset it.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Resetting a custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-manageAcousticModels#resetModel-acoustic).
 
         :param str customization_id: The customization ID (GUID) of the custom
                acoustic model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
@@ -3694,15 +3763,16 @@
         existing upgrade request completes.
         If the custom acoustic model was trained with a separately created custom language
         model, you must use the `custom_language_model_id` parameter to specify the GUID
         of that custom language model. The custom language model must be upgraded before
         the custom acoustic model can be upgraded. Omit the parameter if the custom
         acoustic model was not trained with a custom language model.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Upgrading a custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-custom-upgrade#custom-upgrade-acoustic).
 
         :param str customization_id: The customization ID (GUID) of the custom
                acoustic model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
@@ -3774,15 +3844,16 @@
         Lists information about all audio resources from a custom acoustic model. The
         information includes the name of the resource and information about its audio
         data, such as its duration. It also includes the status of the audio resource,
         which is important for checking the service's analysis of the resource in response
         to a request to add it to the custom acoustic model. You must use credentials for
         the instance of the service that owns a model to list its audio resources.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Listing audio resources for a custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-manageAudio#listAudio).
 
         :param str customization_id: The customization ID (GUID) of the custom
                acoustic model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
@@ -3866,15 +3937,16 @@
         requests completes.
         To determine the status of the service's analysis of the audio, use the [Get an
         audio resource](#getaudio) method to poll the status of the audio. The method
         accepts the customization ID of the custom model and the name of the audio
         resource, and it returns the status of the resource. Use a loop to check the
         status of the audio every few seconds until it becomes `ok`.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Add audio to the custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-acoustic#addAudio).
         ### Content types for audio-type resources
          You can add an individual audio file in any format that the service supports for
         speech recognition. For an audio-type resource, use the `Content-Type` parameter
         to specify the audio format (MIME type) of the audio file, including specifying
         the sampling rate, channels, and endianness where indicated.
@@ -4042,15 +4114,16 @@
         * _For an audio-type resource_, the `status` field is located in the
         `AudioListing` object.
         * _For an archive-type resource_, the `status` field is located in the
         `AudioResource` object that is returned in the `container` field.
         You must use credentials for the instance of the service that owns a model to list
         its audio resources.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Listing audio resources for a custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-manageAudio#listAudio).
 
         :param str customization_id: The customization ID (GUID) of the custom
                acoustic model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
@@ -4107,15 +4180,16 @@
         Removing an audio resource does not affect the custom model until you train the
         model on its updated data by using the [Train a custom acoustic
         model](#trainacousticmodel) method. You can delete an existing audio resource from
         a model while a different resource is being added to the model. You must use
         credentials for the instance of the service that owns a model to delete its audio
         resources.
         **Note:** Acoustic model customization is supported only for use with
-        previous-generation models. It is not supported for next-generation models.
+        previous-generation models. It is not supported for large speech models and
+        next-generation models.
         **See also:** [Deleting an audio resource from a custom acoustic
         model](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-manageAudio#deleteAudio).
 
         :param str customization_id: The customization ID (GUID) of the custom
                acoustic model that is to be used for the request. You must make the
                request with credentials for the instance of the service that owns the
                custom model.
@@ -4235,23 +4309,27 @@
         AR_MS_BROADBANDMODEL = 'ar-MS_BroadbandModel'
         AR_MS_TELEPHONY = 'ar-MS_Telephony'
         CS_CZ_TELEPHONY = 'cs-CZ_Telephony'
         DE_DE_BROADBANDMODEL = 'de-DE_BroadbandModel'
         DE_DE_MULTIMEDIA = 'de-DE_Multimedia'
         DE_DE_NARROWBANDMODEL = 'de-DE_NarrowbandModel'
         DE_DE_TELEPHONY = 'de-DE_Telephony'
+        EN_AU = 'en-AU'
         EN_AU_BROADBANDMODEL = 'en-AU_BroadbandModel'
         EN_AU_MULTIMEDIA = 'en-AU_Multimedia'
         EN_AU_NARROWBANDMODEL = 'en-AU_NarrowbandModel'
         EN_AU_TELEPHONY = 'en-AU_Telephony'
+        EN_GB = 'en-GB'
         EN_GB_BROADBANDMODEL = 'en-GB_BroadbandModel'
         EN_GB_MULTIMEDIA = 'en-GB_Multimedia'
         EN_GB_NARROWBANDMODEL = 'en-GB_NarrowbandModel'
         EN_GB_TELEPHONY = 'en-GB_Telephony'
+        EN_IN = 'en-IN'
         EN_IN_TELEPHONY = 'en-IN_Telephony'
+        EN_US = 'en-US'
         EN_US_BROADBANDMODEL = 'en-US_BroadbandModel'
         EN_US_MULTIMEDIA = 'en-US_Multimedia'
         EN_US_NARROWBANDMODEL = 'en-US_NarrowbandModel'
         EN_US_SHORTFORM_NARROWBANDMODEL = 'en-US_ShortForm_NarrowbandModel'
         EN_US_TELEPHONY = 'en-US_Telephony'
         EN_WW_MEDICAL_TELEPHONY = 'en-WW_Medical_Telephony'
         ES_AR_BROADBANDMODEL = 'es-AR_BroadbandModel'
@@ -4265,27 +4343,30 @@
         ES_ES_MULTIMEDIA = 'es-ES_Multimedia'
         ES_ES_TELEPHONY = 'es-ES_Telephony'
         ES_LA_TELEPHONY = 'es-LA_Telephony'
         ES_MX_BROADBANDMODEL = 'es-MX_BroadbandModel'
         ES_MX_NARROWBANDMODEL = 'es-MX_NarrowbandModel'
         ES_PE_BROADBANDMODEL = 'es-PE_BroadbandModel'
         ES_PE_NARROWBANDMODEL = 'es-PE_NarrowbandModel'
+        FR_CA = 'fr-CA'
         FR_CA_BROADBANDMODEL = 'fr-CA_BroadbandModel'
         FR_CA_MULTIMEDIA = 'fr-CA_Multimedia'
         FR_CA_NARROWBANDMODEL = 'fr-CA_NarrowbandModel'
         FR_CA_TELEPHONY = 'fr-CA_Telephony'
+        FR_FR = 'fr-FR'
         FR_FR_BROADBANDMODEL = 'fr-FR_BroadbandModel'
         FR_FR_MULTIMEDIA = 'fr-FR_Multimedia'
         FR_FR_NARROWBANDMODEL = 'fr-FR_NarrowbandModel'
         FR_FR_TELEPHONY = 'fr-FR_Telephony'
         HI_IN_TELEPHONY = 'hi-IN_Telephony'
         IT_IT_BROADBANDMODEL = 'it-IT_BroadbandModel'
         IT_IT_NARROWBANDMODEL = 'it-IT_NarrowbandModel'
         IT_IT_MULTIMEDIA = 'it-IT_Multimedia'
         IT_IT_TELEPHONY = 'it-IT_Telephony'
+        JA_JP = 'ja-JP'
         JA_JP_BROADBANDMODEL = 'ja-JP_BroadbandModel'
         JA_JP_MULTIMEDIA = 'ja-JP_Multimedia'
         JA_JP_NARROWBANDMODEL = 'ja-JP_NarrowbandModel'
         JA_JP_TELEPHONY = 'ja-JP_Telephony'
         KO_KR_BROADBANDMODEL = 'ko-KR_BroadbandModel'
         KO_KR_MULTIMEDIA = 'ko-KR_Multimedia'
         KO_KR_NARROWBANDMODEL = 'ko-KR_NarrowbandModel'
@@ -4350,23 +4431,27 @@
         AR_MS_BROADBANDMODEL = 'ar-MS_BroadbandModel'
         AR_MS_TELEPHONY = 'ar-MS_Telephony'
         CS_CZ_TELEPHONY = 'cs-CZ_Telephony'
         DE_DE_BROADBANDMODEL = 'de-DE_BroadbandModel'
         DE_DE_MULTIMEDIA = 'de-DE_Multimedia'
         DE_DE_NARROWBANDMODEL = 'de-DE_NarrowbandModel'
         DE_DE_TELEPHONY = 'de-DE_Telephony'
+        EN_AU = 'en-AU'
         EN_AU_BROADBANDMODEL = 'en-AU_BroadbandModel'
         EN_AU_MULTIMEDIA = 'en-AU_Multimedia'
         EN_AU_NARROWBANDMODEL = 'en-AU_NarrowbandModel'
         EN_AU_TELEPHONY = 'en-AU_Telephony'
+        EN_IN = 'en-IN'
         EN_IN_TELEPHONY = 'en-IN_Telephony'
+        EN_GB = 'en-GB'
         EN_GB_BROADBANDMODEL = 'en-GB_BroadbandModel'
         EN_GB_MULTIMEDIA = 'en-GB_Multimedia'
         EN_GB_NARROWBANDMODEL = 'en-GB_NarrowbandModel'
         EN_GB_TELEPHONY = 'en-GB_Telephony'
+        EN_US = 'en-US'
         EN_US_BROADBANDMODEL = 'en-US_BroadbandModel'
         EN_US_MULTIMEDIA = 'en-US_Multimedia'
         EN_US_NARROWBANDMODEL = 'en-US_NarrowbandModel'
         EN_US_SHORTFORM_NARROWBANDMODEL = 'en-US_ShortForm_NarrowbandModel'
         EN_US_TELEPHONY = 'en-US_Telephony'
         EN_WW_MEDICAL_TELEPHONY = 'en-WW_Medical_Telephony'
         ES_AR_BROADBANDMODEL = 'es-AR_BroadbandModel'
@@ -4380,27 +4465,30 @@
         ES_ES_MULTIMEDIA = 'es-ES_Multimedia'
         ES_ES_TELEPHONY = 'es-ES_Telephony'
         ES_LA_TELEPHONY = 'es-LA_Telephony'
         ES_MX_BROADBANDMODEL = 'es-MX_BroadbandModel'
         ES_MX_NARROWBANDMODEL = 'es-MX_NarrowbandModel'
         ES_PE_BROADBANDMODEL = 'es-PE_BroadbandModel'
         ES_PE_NARROWBANDMODEL = 'es-PE_NarrowbandModel'
+        FR_CA = 'fr-CA'
         FR_CA_BROADBANDMODEL = 'fr-CA_BroadbandModel'
         FR_CA_MULTIMEDIA = 'fr-CA_Multimedia'
         FR_CA_NARROWBANDMODEL = 'fr-CA_NarrowbandModel'
         FR_CA_TELEPHONY = 'fr-CA_Telephony'
+        FR_FR = 'fr-FR'
         FR_FR_BROADBANDMODEL = 'fr-FR_BroadbandModel'
         FR_FR_MULTIMEDIA = 'fr-FR_Multimedia'
         FR_FR_NARROWBANDMODEL = 'fr-FR_NarrowbandModel'
         FR_FR_TELEPHONY = 'fr-FR_Telephony'
         HI_IN_TELEPHONY = 'hi-IN_Telephony'
         IT_IT_BROADBANDMODEL = 'it-IT_BroadbandModel'
         IT_IT_NARROWBANDMODEL = 'it-IT_NarrowbandModel'
         IT_IT_MULTIMEDIA = 'it-IT_Multimedia'
         IT_IT_TELEPHONY = 'it-IT_Telephony'
+        JA_JP = 'ja-JP'
         JA_JP_BROADBANDMODEL = 'ja-JP_BroadbandModel'
         JA_JP_MULTIMEDIA = 'ja-JP_Multimedia'
         JA_JP_NARROWBANDMODEL = 'ja-JP_NarrowbandModel'
         JA_JP_TELEPHONY = 'ja-JP_Telephony'
         KO_KR_BROADBANDMODEL = 'ko-KR_BroadbandModel'
         KO_KR_MULTIMEDIA = 'ko-KR_Multimedia'
         KO_KR_NARROWBANDMODEL = 'ko-KR_NarrowbandModel'
@@ -4465,23 +4553,27 @@
         AR_MS_BROADBANDMODEL = 'ar-MS_BroadbandModel'
         AR_MS_TELEPHONY = 'ar-MS_Telephony'
         CS_CZ_TELEPHONY = 'cs-CZ_Telephony'
         DE_DE_BROADBANDMODEL = 'de-DE_BroadbandModel'
         DE_DE_MULTIMEDIA = 'de-DE_Multimedia'
         DE_DE_NARROWBANDMODEL = 'de-DE_NarrowbandModel'
         DE_DE_TELEPHONY = 'de-DE_Telephony'
+        EN_AU = 'en-AU'
         EN_AU_BROADBANDMODEL = 'en-AU_BroadbandModel'
         EN_AU_MULTIMEDIA = 'en-AU_Multimedia'
         EN_AU_NARROWBANDMODEL = 'en-AU_NarrowbandModel'
         EN_AU_TELEPHONY = 'en-AU_Telephony'
+        EN_IN = 'en-IN'
         EN_IN_TELEPHONY = 'en-IN_Telephony'
+        EN_GB = 'en-GB'
         EN_GB_BROADBANDMODEL = 'en-GB_BroadbandModel'
         EN_GB_MULTIMEDIA = 'en-GB_Multimedia'
         EN_GB_NARROWBANDMODEL = 'en-GB_NarrowbandModel'
         EN_GB_TELEPHONY = 'en-GB_Telephony'
+        EN_US = 'en-US'
         EN_US_BROADBANDMODEL = 'en-US_BroadbandModel'
         EN_US_MULTIMEDIA = 'en-US_Multimedia'
         EN_US_NARROWBANDMODEL = 'en-US_NarrowbandModel'
         EN_US_SHORTFORM_NARROWBANDMODEL = 'en-US_ShortForm_NarrowbandModel'
         EN_US_TELEPHONY = 'en-US_Telephony'
         EN_WW_MEDICAL_TELEPHONY = 'en-WW_Medical_Telephony'
         ES_AR_BROADBANDMODEL = 'es-AR_BroadbandModel'
@@ -4495,27 +4587,30 @@
         ES_ES_MULTIMEDIA = 'es-ES_Multimedia'
         ES_ES_TELEPHONY = 'es-ES_Telephony'
         ES_LA_TELEPHONY = 'es-LA_Telephony'
         ES_MX_BROADBANDMODEL = 'es-MX_BroadbandModel'
         ES_MX_NARROWBANDMODEL = 'es-MX_NarrowbandModel'
         ES_PE_BROADBANDMODEL = 'es-PE_BroadbandModel'
         ES_PE_NARROWBANDMODEL = 'es-PE_NarrowbandModel'
+        FR_CA = 'fr-CA'
         FR_CA_BROADBANDMODEL = 'fr-CA_BroadbandModel'
         FR_CA_MULTIMEDIA = 'fr-CA_Multimedia'
         FR_CA_NARROWBANDMODEL = 'fr-CA_NarrowbandModel'
         FR_CA_TELEPHONY = 'fr-CA_Telephony'
+        FR_FR = 'fr-FR'
         FR_FR_BROADBANDMODEL = 'fr-FR_BroadbandModel'
         FR_FR_MULTIMEDIA = 'fr-FR_Multimedia'
         FR_FR_NARROWBANDMODEL = 'fr-FR_NarrowbandModel'
         FR_FR_TELEPHONY = 'fr-FR_Telephony'
         HI_IN_TELEPHONY = 'hi-IN_Telephony'
         IT_IT_BROADBANDMODEL = 'it-IT_BroadbandModel'
         IT_IT_NARROWBANDMODEL = 'it-IT_NarrowbandModel'
         IT_IT_MULTIMEDIA = 'it-IT_Multimedia'
         IT_IT_TELEPHONY = 'it-IT_Telephony'
+        JA_JP = 'ja-JP'
         JA_JP_BROADBANDMODEL = 'ja-JP_BroadbandModel'
         JA_JP_MULTIMEDIA = 'ja-JP_Multimedia'
         JA_JP_NARROWBANDMODEL = 'ja-JP_NarrowbandModel'
         JA_JP_TELEPHONY = 'ja-JP_Telephony'
         KO_KR_BROADBANDMODEL = 'ko-KR_BroadbandModel'
         KO_KR_MULTIMEDIA = 'ko-KR_Multimedia'
         KO_KR_NARROWBANDMODEL = 'ko-KR_NarrowbandModel'
@@ -4617,17 +4712,18 @@
         words from the custom language model's words resource on which to train the model:
         * `all` (the default) trains the model on all new words, regardless of whether
         they were extracted from corpora or grammars or were added or modified by the
         user.
         * `user` trains the model only on custom words that were added or modified by the
         user directly. The model is not trained on new words extracted from corpora or
         grammars.
-        _For custom models that are based on next-generation models_, the service ignores
-        the parameter. The words resource contains only custom words that the user adds or
-        modifies directly, so the parameter is unnecessary.
+        _For custom models that are based on large speech models and next-generation
+        models_, the service ignores the `word_type_to_add` parameter. The words resource
+        contains only custom words that the user adds or modifies directly, so the
+        parameter is unnecessary.
         """
 
         ALL = 'all'
         USER = 'user'
 
 
 class ListWordsEnums:
@@ -6163,17 +6259,17 @@
 class Corpus:
     """
     Information about a corpus from a custom language model.
 
     :param str name: The name of the corpus.
     :param int total_words: The total number of words in the corpus. The value is
           `0` while the corpus is being processed.
-    :param int out_of_vocabulary_words: _For custom models that are based on
-          previous-generation models_, the number of OOV words extracted from the corpus.
-          The value is `0` while the corpus is being processed.
+    :param int out_of_vocabulary_words: _For custom models that are based on large
+          speech models and previous-generation models_, the number of OOV words extracted
+          from the corpus. The value is `0` while the corpus is being processed.
           _For custom models that are based on next-generation models_, no OOV words are
           extracted from corpora, so the value is always `0`.
     :param str status: The status of the corpus:
           * `analyzed`: The service successfully analyzed the corpus. The custom model can
           be trained with data from the corpus.
           * `being_processed`: The service is still analyzing the corpus. The service
           cannot accept requests to add new resources or to train the custom model.
@@ -6196,16 +6292,17 @@
         """
         Initialize a Corpus object.
 
         :param str name: The name of the corpus.
         :param int total_words: The total number of words in the corpus. The value
                is `0` while the corpus is being processed.
         :param int out_of_vocabulary_words: _For custom models that are based on
-               previous-generation models_, the number of OOV words extracted from the
-               corpus. The value is `0` while the corpus is being processed.
+               large speech models and previous-generation models_, the number of OOV
+               words extracted from the corpus. The value is `0` while the corpus is being
+               processed.
                _For custom models that are based on next-generation models_, no OOV words
                are extracted from corpora, so the value is always `0`.
         :param str status: The status of the corpus:
                * `analyzed`: The service successfully analyzed the corpus. The custom
                model can be trained with data from the corpus.
                * `being_processed`: The service is still analyzing the corpus. The service
                cannot accept requests to add new resources or to train the custom model.
```

### Comparing `ibm-watson-8.0.0/ibm_watson/speech_to_text_v1_adapter.py` & `ibm_watson-8.1.0/ibm_watson/speech_to_text_v1_adapter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 
-# (C) Copyright IBM Corp. 2018, 2021.
+# (C) Copyright IBM Corp. 2018, 2024.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -29,36 +29,35 @@
                                   recognize_callback,
                                   model=None,
                                   language_customization_id=None,
                                   acoustic_customization_id=None,
                                   customization_weight=None,
                                   base_model_version=None,
                                   inactivity_timeout=None,
-                                  interim_results=None,
                                   keywords=None,
                                   keywords_threshold=None,
                                   max_alternatives=None,
                                   word_alternatives_threshold=None,
                                   word_confidence=None,
                                   timestamps=None,
                                   profanity_filter=None,
                                   smart_formatting=None,
+                                  smart_formatting_version=None,
                                   speaker_labels=None,
                                   http_proxy_host=None,
                                   http_proxy_port=None,
                                   grammar_name=None,
                                   redaction=None,
                                   processing_metrics=None,
                                   processing_metrics_interval=None,
                                   audio_metrics=None,
                                   end_of_phrase_silence_time=None,
                                   split_transcript_at_phrase_end=None,
                                   speech_detector_sensitivity=None,
                                   background_audio_suppression=None,
-                                  low_latency=None,
                                   character_insertion_bias=None,
                                   **kwargs):
         """
         Sends audio for speech recognition using web sockets.
 
         
         :param AudioSource audio: The audio to transcribe in the format specified by the
@@ -171,14 +170,17 @@
                and internet addresses into more readable, conventional representations in
                the final transcript of a recognition request. For US English, the service
                also converts certain keyword strings to punctuation symbols. By default,
                the service performs no smart formatting.
                **Note:** Applies to US English, Japanese, and Spanish transcription only.
                See [Smart
                formatting](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-formatting#smart-formatting).
+       :param  int smart_formatting_version: (optional) Smart formatting version is
+               for next-generation models and that is supported in US English, Brazilian
+               Portuguese, French and German languages.
         :param bool speaker_labels: (optional) If `true`, the response includes
                labels that identify which words were spoken by which participants in a
                multi-person exchange. By default, the service returns no speaker labels.
                Setting `speaker_labels` to `true` forces the `timestamps` parameter to be
                `true`, regardless of whether you specify `false` for the parameter.
                * For previous-generation models, can be used for US English, Australian
                English, German, Japanese, Korean, and Spanish (both broadband and
@@ -263,30 +265,14 @@
                Specify a value in the range of 0.0 to 1.0:
                * 0.0 (the default) provides no suppression (background audio suppression
                is disabled).
                * 0.5 provides a reasonable level of audio suppression for general usage.
                * 1.0 suppresses all audio (no audio is transcribed).
                The values increase on a monotonic curve. See [Background audio
                suppression](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-detection#detection-parameters-suppression).
-        :param bool low_latency: (optional) If `true` for next-generation
-               `Multimedia` and `Telephony` models that support low latency, directs the
-               service to produce results even more quickly than it usually does.
-               Next-generation models produce transcription results faster than
-               previous-generation models. The `low_latency` parameter causes the models
-               to produce results even more quickly, though the results might be less
-               accurate when the parameter is used.
-               **Note:** The parameter is beta functionality. It is not available for
-               previous-generation `Broadband` and `Narrowband` models. It is available
-               only for some next-generation models.
-               * For a list of next-generation models that support low latency, see
-               [Supported language
-               models](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-models-ng#models-ng-supported)
-               for next-generation models.
-               * For more information about the `low_latency` parameter, see [Low
-               latency](https://cloud.ibm.com/docs/speech-to-text?topic=speech-to-text-interim#low-latency).
         :param float character_insertion_bias: (optional) For next-generation
                `Multimedia` and `Telephony` models, an indication of whether the service
                is biased to recognize shorter or longer strings of characters when
                developing transcription hypotheses. By default, the service is optimized
                for each individual model to balance its recognition of strings of
                different lengths. The model-specific bias is equivalent to 0.0.
                The value that you specify represents a change from a model's default bias.
@@ -347,34 +333,33 @@
         url += '/v1/recognize?{0}'.format(urlencode(params))
         request['url'] = url
 
         options = {
             'customization_weight': customization_weight,
             'content_type': content_type,
             'inactivity_timeout': inactivity_timeout,
-            'interim_results': interim_results,
             'keywords': keywords,
             'keywords_threshold': keywords_threshold,
             'max_alternatives': max_alternatives,
             'word_alternatives_threshold': word_alternatives_threshold,
             'word_confidence': word_confidence,
             'timestamps': timestamps,
             'profanity_filter': profanity_filter,
             'smart_formatting': smart_formatting,
+            'smart_formatting_version': smart_formatting_version,
             'speaker_labels': speaker_labels,
             'grammar_name': grammar_name,
             'redaction': redaction,
             'processing_metrics': processing_metrics,
             'processing_metrics_interval': processing_metrics_interval,
             'audio_metrics': audio_metrics,
             'end_of_phrase_silence_time': end_of_phrase_silence_time,
             'split_transcript_at_phrase_end': split_transcript_at_phrase_end,
             'speech_detector_sensitivity': speech_detector_sensitivity,
             'background_audio_suppression': background_audio_suppression,
-            'low_latency': low_latency,
             'character_insertion_bias': character_insertion_bias
         }
         options = {k: v for k, v in options.items() if v is not None}
         request['options'] = options
 
         RecognizeListener(audio, request.get('options'), recognize_callback,
                           request.get('url'), request.get('headers'),
```

### Comparing `ibm-watson-8.0.0/ibm_watson/text_to_speech_adapter_v1.py` & `ibm_watson-8.1.0/ibm_watson/text_to_speech_adapter_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/text_to_speech_v1.py` & `ibm_watson-8.1.0/ibm_watson/text_to_speech_v1.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/websocket/__init__.py` & `ibm_watson-8.1.0/ibm_watson/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/websocket/audio_source.py` & `ibm_watson-8.1.0/ibm_watson/websocket/audio_source.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/websocket/recognize_abstract_callback.py` & `ibm_watson-8.1.0/ibm_watson/websocket/recognize_abstract_callback.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/websocket/recognize_listener.py` & `ibm_watson-8.1.0/ibm_watson/websocket/recognize_listener.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,24 +192,23 @@
 
         # if in streaming
         elif 'results' in json_object or 'speaker_labels' in json_object:
             # If results are present, extract the hypothesis and, if finalized, the full
             # set of transcriptions and send them to the appropriate callbacks.
             results = json_object.get('results')
             if results:
-                if (self.options.get('interim_results') is True):
-                    b_final = (results[0].get('final') is True)
-                    alternatives = results[0].get('alternatives')
-                    if alternatives:
-                        hypothesis = alternatives[0].get('transcript')
-                        transcripts = self.extract_transcripts(alternatives)
-                        if b_final:
-                            self.callback.on_transcription(transcripts)
-                        if hypothesis:
-                            self.callback.on_hypothesis(hypothesis)
+                b_final = (results[0].get('final') is True)
+                alternatives = results[0].get('alternatives')
+                if alternatives:
+                    hypothesis = alternatives[0].get('transcript')
+                    transcripts = self.extract_transcripts(alternatives)
+                    if b_final:
+                        self.callback.on_transcription(transcripts)
+                    if hypothesis:
+                        self.callback.on_hypothesis(hypothesis)
                 else:
                     final_transcript = []
                     for result in results:
                         transcript = self.extract_transcripts(
                             result.get('alternatives'))
                         final_transcript.append(transcript)
```

### Comparing `ibm-watson-8.0.0/ibm_watson/websocket/synthesize_callback.py` & `ibm_watson-8.1.0/ibm_watson/websocket/synthesize_callback.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson/websocket/synthesize_listener.py` & `ibm_watson-8.1.0/ibm_watson/websocket/synthesize_listener.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/ibm_watson.egg-info/PKG-INFO` & `ibm_watson-8.1.0/ibm_watson.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson
-Version: 8.0.0
+Version: 8.1.0
 Summary: Client library to use the IBM Watson Services
 Home-page: https://github.com/watson-developer-cloud/python-sdk
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 License: Apache 2.0
 Keywords: language,vision,question and answer tone_analyzer,natural language classifier,text to speech,language translation,language identification,concept expansion,machine translation,personality insights,message resonance,watson developer cloud,wdc,watson,ibm,dialog,user modeling,tone analyzer,speech to text,visual recognition
 Classifier: Programming Language :: Python
@@ -197,36 +197,51 @@
 # in the constructor, assuming control of managing the token
 authenticator = BearerTokenAuthenticator('your bearer token')
 discovery = DiscoveryV1(version='2019-04-30',
                         authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
-### Username and password
+#### Username and password
 
 ```python
 from ibm_watson import DiscoveryV1
 from ibm_cloud_sdk_core.authenticators import BasicAuthenticator
 
 authenticator = BasicAuthenticator('username', 'password')
 discovery = DiscoveryV1(version='2019-04-30', authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
-### No Authentication
+#### No Authentication
 
 ```python
 from ibm_watson import DiscoveryV1
 from ibm_cloud_sdk_core.authenticators import NoAuthAuthenticator
 
 authenticator = NoAuthAuthenticator()
 discovery = DiscoveryV1(version='2019-04-30', authenticator=authenticator)
 discovery.set_service_url('<url_as_per_region>')
 ```
 
+### MCSP
+
+To use the SDK through a third party cloud provider (such as AWS), use the `MCSPAuthenticator`. This will require the base endpoint URL for the MCSP token service (e.g. https://iam.platform.saas.ibm.com) and an apikey. 
+
+```python
+from ibm_watson import AssistantV2
+from ibm_cloud_sdk_core.authenticators import MCSPAuthenticator
+
+# In the constructor, letting the SDK manage the token
+authenticator = MCSPAuthenticator('apikey', 'token_service_endpoint')
+assistant = AssistantV2(version='2023-06-15',
+                        authenticator=authenticator)
+assistant.set_service_url('<url_as_per_region>')
+```
+
 ## Python version
 
 Tested on Python 3.9, 3.10, and 3.11.
 
 ## Questions
 
 If you have issues with the APIs or have a question about the Watson services, see [Stack Overflow](https://stackoverflow.com/questions/tagged/ibm-watson+python).
```

### Comparing `ibm-watson-8.0.0/ibm_watson.egg-info/SOURCES.txt` & `ibm_watson-8.1.0/ibm_watson.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-watson-8.0.0/setup.py` & `ibm_watson-8.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from setuptools import setup
 from os import path
 
-__version__ = '8.0.0'
+__version__ = '8.1.0'
 
 # read contents of README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as file:
     readme_file = file.read()
 
 setup(name='ibm-watson',
```

