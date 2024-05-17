# Comparing `tmp/xiaogpt-2.71.tar.gz` & `tmp/xiaogpt-2.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaogpt-2.71.tar", last modified: Tue May 14 03:27:27 2024, max compression
+gzip compressed data, was "xiaogpt-2.80.tar", last modified: Fri May 17 04:40:21 2024, max compression
```

## Comparing `xiaogpt-2.71.tar` & `xiaogpt-2.80.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1063 2024-05-14 03:27:23.184762 xiaogpt-2.71/LICENSE
--rw-r--r--   0        0        0    23909 2024-05-14 03:27:23.184762 xiaogpt-2.71/README.md
--rw-r--r--   0        0        0     3829 2024-05-14 03:27:27.328760 xiaogpt-2.71/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/__init__.py
--rw-r--r--   0        0        0       61 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/__main__.py
--rw-r--r--   0        0        0     1160 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/base_bot.py
--rw-r--r--   0        0        0     3660 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/chatgptapi_bot.py
--rw-r--r--   0        0        0     2773 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/doubao_bot.py
--rw-r--r--   0        0        0     2516 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/gemini_bot.py
--rw-r--r--   0        0        0     1825 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/glm_bot.py
--rw-r--r--   0        0        0     1944 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/langchain_bot.py
--rw-r--r--   0        0        0      708 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/llama_bot.py
--rw-r--r--   0        0        0      822 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/moonshot_bot.py
--rw-r--r--   0        0        0     3657 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/qwen_bot.py
--rw-r--r--   0        0        0      784 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/bot/yi_bot.py
--rw-r--r--   0        0        0     5711 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/cli.py
--rw-r--r--   0        0        0     6734 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/config.py
--rw-r--r--   0        0        0     2616 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/langchain/callbacks.py
--rw-r--r--   0        0        0     1495 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/langchain/chain.py
--rw-r--r--   0        0        0     6372 2024-05-14 03:27:23.184762 xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_box.py
--rw-r--r--   0        0        0     1561 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_summary_tools.py
--rw-r--r--   0        0        0      145 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/base.py
--rw-r--r--   0        0        0     1095 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/mi.py
--rw-r--r--   0        0        0     1058 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/tts/tetos.py
--rw-r--r--   0        0        0     2072 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/utils.py
--rw-r--r--   0        0        0    16525 2024-05-14 03:27:23.188762 xiaogpt-2.71/xiaogpt/xiaogpt.py
--rw-r--r--   0        0        0    29638 1970-01-01 00:00:00.000000 xiaogpt-2.71/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 04:40:14.908027 xiaogpt-2.80/LICENSE
+-rw-r--r--   0        0        0    23909 2024-05-17 04:40:14.908027 xiaogpt-2.80/README.md
+-rw-r--r--   0        0        0     3829 2024-05-17 04:40:21.132065 xiaogpt-2.80/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/__main__.py
+-rw-r--r--   0        0        0     1160 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/base_bot.py
+-rw-r--r--   0        0        0     3660 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/chatgptapi_bot.py
+-rw-r--r--   0        0        0     2773 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/doubao_bot.py
+-rw-r--r--   0        0        0     2516 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/gemini_bot.py
+-rw-r--r--   0        0        0     1825 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/glm_bot.py
+-rw-r--r--   0        0        0     1944 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/langchain_bot.py
+-rw-r--r--   0        0        0      708 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/llama_bot.py
+-rw-r--r--   0        0        0      822 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/moonshot_bot.py
+-rw-r--r--   0        0        0     3657 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/qwen_bot.py
+-rw-r--r--   0        0        0      784 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/bot/yi_bot.py
+-rw-r--r--   0        0        0     5711 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/cli.py
+-rw-r--r--   0        0        0     6734 2024-05-17 04:40:14.908027 xiaogpt-2.80/xiaogpt/config.py
+-rw-r--r--   0        0        0     2616 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/callbacks.py
+-rw-r--r--   0        0        0     1495 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/chain.py
+-rw-r--r--   0        0        0     6372 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_box.py
+-rw-r--r--   0        0        0     1561 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_summary_tools.py
+-rw-r--r--   0        0        0      145 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/base.py
+-rw-r--r--   0        0        0     1095 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/mi.py
+-rw-r--r--   0        0        0     1058 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/tts/tetos.py
+-rw-r--r--   0        0        0     2072 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/utils.py
+-rw-r--r--   0        0        0    16524 2024-05-17 04:40:14.912027 xiaogpt-2.80/xiaogpt/xiaogpt.py
+-rw-r--r--   0        0        0    29638 1970-01-01 00:00:00.000000 xiaogpt-2.80/PKG-INFO
```

### Comparing `xiaogpt-2.71/LICENSE` & `xiaogpt-2.80/LICENSE`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/README.md` & `xiaogpt-2.80/README.md`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/pyproject.toml` & `xiaogpt-2.80/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "numexpr>=2.8.6",
     "dashscope>=1.10.0",
     "tetos>=0.2.1",
     "groq>=0.5.0",
     "pyyaml>=6.0.1",
 ]
 dynamic = []
-version = "2.71"
+version = "2.80"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/yihong0618/xiaogpt"
 
@@ -57,26 +57,26 @@
     "colorama==0.4.6 ; platform_system == \"Windows\"",
     "dashscope==1.19.0",
     "dataclasses-json==0.6.3",
     "distro==1.9.0",
     "edge-tts==6.1.10",
     "exceptiongroup==1.2.0 ; python_version < \"3.11\"",
     "frozenlist==1.4.1",
-    "google-ai-generativelanguage==0.6.3",
+    "google-ai-generativelanguage==0.6.4",
     "google-api-core==2.15.0",
     "google-api-core[grpc]==2.15.0",
     "google-api-python-client==2.125.0",
     "google-auth==2.26.1",
     "google-auth-httplib2==0.2.0",
     "google-cloud-texttospeech==2.16.3",
-    "google-generativeai==0.5.3",
+    "google-generativeai==0.5.4",
     "google-search-results==2.4.2",
     "googleapis-common-protos==1.62.0",
     "greenlet==3.0.3 ; platform_machine == \"win32\" or platform_machine == \"WIN32\" or platform_machine == \"AMD64\" or platform_machine == \"amd64\" or platform_machine == \"x86_64\" or platform_machine == \"ppc64le\" or platform_machine == \"aarch64\"",
-    "groq==0.5.0",
+    "groq==0.6.0",
     "grpcio==1.60.0",
     "grpcio-status==1.60.0",
     "h11==0.14.0",
     "httpcore==1.0.5",
     "httplib2==0.22.0",
     "httpx==0.27.0",
     "httpx[socks]==0.27.0",
@@ -87,21 +87,21 @@
     "langchain-community==0.0.38",
     "langchain-core==0.1.52",
     "langchain-text-splitters==0.0.1",
     "langsmith==0.1.45",
     "markdown-it-py==3.0.0",
     "marshmallow==3.20.1",
     "mdurl==0.1.2",
-    "miservice-fork==2.4.3",
+    "miservice-fork==2.5.0",
     "multidict==6.0.5",
     "mutagen==1.47.0",
     "mypy-extensions==1.0.0",
     "numexpr==2.10.0",
     "numpy==1.26.3",
-    "openai==1.29.0",
+    "openai==1.30.1",
     "orjson==3.10.0",
     "packaging==23.2",
     "proto-plus==1.23.0",
     "protobuf==4.25.1",
     "pyasn1==0.5.1",
     "pyasn1-modules==0.3.0",
     "pydantic==2.5.3",
```

### Comparing `xiaogpt-2.71/xiaogpt/bot/__init__.py` & `xiaogpt-2.80/xiaogpt/bot/__init__.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/base_bot.py` & `xiaogpt-2.80/xiaogpt/bot/base_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/chatgptapi_bot.py` & `xiaogpt-2.80/xiaogpt/bot/chatgptapi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/doubao_bot.py` & `xiaogpt-2.80/xiaogpt/bot/doubao_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/gemini_bot.py` & `xiaogpt-2.80/xiaogpt/bot/gemini_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/glm_bot.py` & `xiaogpt-2.80/xiaogpt/bot/glm_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/langchain_bot.py` & `xiaogpt-2.80/xiaogpt/bot/langchain_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/llama_bot.py` & `xiaogpt-2.80/xiaogpt/bot/llama_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/moonshot_bot.py` & `xiaogpt-2.80/xiaogpt/bot/moonshot_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/qwen_bot.py` & `xiaogpt-2.80/xiaogpt/bot/qwen_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/bot/yi_bot.py` & `xiaogpt-2.80/xiaogpt/bot/yi_bot.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/cli.py` & `xiaogpt-2.80/xiaogpt/cli.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/config.py` & `xiaogpt-2.80/xiaogpt/config.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/langchain/callbacks.py` & `xiaogpt-2.80/xiaogpt/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/langchain/chain.py` & `xiaogpt-2.80/xiaogpt/langchain/chain.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_box.py` & `xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_box.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/langchain/examples/email/mail_summary_tools.py` & `xiaogpt-2.80/xiaogpt/langchain/examples/email/mail_summary_tools.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/tts/base.py` & `xiaogpt-2.80/xiaogpt/tts/base.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/tts/mi.py` & `xiaogpt-2.80/xiaogpt/tts/mi.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/tts/tetos.py` & `xiaogpt-2.80/xiaogpt/tts/tetos.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/utils.py` & `xiaogpt-2.80/xiaogpt/utils.py`

 * *Files identical despite different names*

### Comparing `xiaogpt-2.71/xiaogpt/xiaogpt.py` & `xiaogpt-2.80/xiaogpt/xiaogpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,23 +321,23 @@
         task.cancel()
 
     async def get_if_xiaoai_is_playing(self):
         playing_info = await self.mina_service.player_get_status(self.device_id)
         # WTF xiaomi api
         is_playing = (
             json.loads(playing_info.get("data", {}).get("info", "{}")).get("status", -1)
-            == 1
+            >= 1
         )
         return is_playing
 
     async def stop_if_xiaoai_is_playing(self):
         is_playing = await self.get_if_xiaoai_is_playing()
         if is_playing:
             # stop it
-            await self.mina_service.player_pause(self.device_id)
+            await self.mina_service.player_stop(self.device_id)
 
     async def wakeup_xiaoai(self):
         return await miio_command(
             self.miio_service,
             self.config.mi_did,
             f"{self.config.wakeup_command} {WAKEUP_KEYWORD} 0",
         )
```

### Comparing `xiaogpt-2.71/PKG-INFO` & `xiaogpt-2.80/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaogpt
-Version: 2.71
+Version: 2.80
 Summary: Play ChatGPT or other LLM with xiaomi AI speaker
 Author-Email: yihong0618 <zouzou0208@gmail.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/yihong0618/xiaogpt
@@ -39,26 +39,26 @@
 Requires-Dist: colorama==0.4.6; platform_system == "Windows" and extra == "locked"
 Requires-Dist: dashscope==1.19.0; extra == "locked"
 Requires-Dist: dataclasses-json==0.6.3; extra == "locked"
 Requires-Dist: distro==1.9.0; extra == "locked"
 Requires-Dist: edge-tts==6.1.10; extra == "locked"
 Requires-Dist: exceptiongroup==1.2.0; python_version < "3.11" and extra == "locked"
 Requires-Dist: frozenlist==1.4.1; extra == "locked"
-Requires-Dist: google-ai-generativelanguage==0.6.3; extra == "locked"
+Requires-Dist: google-ai-generativelanguage==0.6.4; extra == "locked"
 Requires-Dist: google-api-core==2.15.0; extra == "locked"
 Requires-Dist: google-api-core[grpc]==2.15.0; extra == "locked"
 Requires-Dist: google-api-python-client==2.125.0; extra == "locked"
 Requires-Dist: google-auth==2.26.1; extra == "locked"
 Requires-Dist: google-auth-httplib2==0.2.0; extra == "locked"
 Requires-Dist: google-cloud-texttospeech==2.16.3; extra == "locked"
-Requires-Dist: google-generativeai==0.5.3; extra == "locked"
+Requires-Dist: google-generativeai==0.5.4; extra == "locked"
 Requires-Dist: google-search-results==2.4.2; extra == "locked"
 Requires-Dist: googleapis-common-protos==1.62.0; extra == "locked"
 Requires-Dist: greenlet==3.0.3; (platform_machine == "win32" or platform_machine == "WIN32" or platform_machine == "AMD64" or platform_machine == "amd64" or platform_machine == "x86_64" or platform_machine == "ppc64le" or platform_machine == "aarch64") and extra == "locked"
-Requires-Dist: groq==0.5.0; extra == "locked"
+Requires-Dist: groq==0.6.0; extra == "locked"
 Requires-Dist: grpcio==1.60.0; extra == "locked"
 Requires-Dist: grpcio-status==1.60.0; extra == "locked"
 Requires-Dist: h11==0.14.0; extra == "locked"
 Requires-Dist: httpcore==1.0.5; extra == "locked"
 Requires-Dist: httplib2==0.22.0; extra == "locked"
 Requires-Dist: httpx==0.27.0; extra == "locked"
 Requires-Dist: httpx[socks]==0.27.0; extra == "locked"
@@ -69,21 +69,21 @@
 Requires-Dist: langchain-community==0.0.38; extra == "locked"
 Requires-Dist: langchain-core==0.1.52; extra == "locked"
 Requires-Dist: langchain-text-splitters==0.0.1; extra == "locked"
 Requires-Dist: langsmith==0.1.45; extra == "locked"
 Requires-Dist: markdown-it-py==3.0.0; extra == "locked"
 Requires-Dist: marshmallow==3.20.1; extra == "locked"
 Requires-Dist: mdurl==0.1.2; extra == "locked"
-Requires-Dist: miservice-fork==2.4.3; extra == "locked"
+Requires-Dist: miservice-fork==2.5.0; extra == "locked"
 Requires-Dist: multidict==6.0.5; extra == "locked"
 Requires-Dist: mutagen==1.47.0; extra == "locked"
 Requires-Dist: mypy-extensions==1.0.0; extra == "locked"
 Requires-Dist: numexpr==2.10.0; extra == "locked"
 Requires-Dist: numpy==1.26.3; extra == "locked"
-Requires-Dist: openai==1.29.0; extra == "locked"
+Requires-Dist: openai==1.30.1; extra == "locked"
 Requires-Dist: orjson==3.10.0; extra == "locked"
 Requires-Dist: packaging==23.2; extra == "locked"
 Requires-Dist: proto-plus==1.23.0; extra == "locked"
 Requires-Dist: protobuf==4.25.1; extra == "locked"
 Requires-Dist: pyasn1==0.5.1; extra == "locked"
 Requires-Dist: pyasn1-modules==0.3.0; extra == "locked"
 Requires-Dist: pydantic==2.5.3; extra == "locked"
```

