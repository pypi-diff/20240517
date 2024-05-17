# Comparing `tmp/modelmerge-0.4.3.tar.gz` & `tmp/modelmerge-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.4.3.tar", last modified: Fri May 17 03:25:43 2024, max compression
+gzip compressed data, was "modelmerge-0.4.4.tar", last modified: Fri May 17 03:47:17 2024, max compression
```

## Comparing `modelmerge-0.4.3.tar` & `modelmerge-0.4.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.579851 modelmerge-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 03:25:31.000000 modelmerge-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:25:43.579851 modelmerge-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-17 03:25:31.000000 modelmerge-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:25:43.579851 modelmerge-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 03:25:31.000000 modelmerge-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31202 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/tarvel.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11930 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.571852 modelmerge-0.4.3/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.575852 modelmerge-0.4.3/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 03:25:31.000000 modelmerge-0.4.3/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.579851 modelmerge-0.4.3/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 03:25:43.000000 modelmerge-0.4.3/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:25:43.575852 modelmerge-0.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_API.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_Web_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_claude_zh_char.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_google_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_jieba.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_langchain_search_old.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_tikitoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 03:25:31.000000 modelmerge-0.4.3/test/test_whisper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.988625 modelmerge-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 03:47:05.000000 modelmerge-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:47:17.988625 modelmerge-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-17 03:47:05.000000 modelmerge-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:47:17.988625 modelmerge-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-17 03:47:05.000000 modelmerge-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.980625 modelmerge-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.980625 modelmerge-0.4.4/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.980625 modelmerge-0.4.4/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29573 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.984625 modelmerge-0.4.4/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/tarvel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.984625 modelmerge-0.4.4/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.984625 modelmerge-0.4.4/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-17 03:47:05.000000 modelmerge-0.4.4/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.988625 modelmerge-0.4.4/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 03:47:17.000000 modelmerge-0.4.4/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:47:17.988625 modelmerge-0.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_API.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_Web_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_claude_zh_char.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_google_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_jieba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9066 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_langchain_search_old.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_tikitoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 03:47:05.000000 modelmerge-0.4.4/test/test_whisper.py
```

### Comparing `modelmerge-0.4.3/LICENSE` & `modelmerge-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/PKG-INFO` & `modelmerge-0.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.3
+Version: 0.4.4
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.3/README.md` & `modelmerge-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.4.4/src/ModelMerge/models/chatgpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -663,57 +663,8 @@
                     cookies=self.session.cookies,
                     headers=self.session.headers,
                 )
             if "session" in keys:
                 keys.remove("session")
             if "aclient" in keys:
                 keys.remove("aclient")
-            self.__dict__.update({key: loaded_config[key] for key in keys})
-
-class dalle3(BaseLLM):
-    def __init__(
-        self,
-        api_key: str,
-        api_url: str = (os.environ.get("API_URL") or "https://api.openai.com/v1/chat/completions"),
-        timeout: float = 20,
-    ):
-        super().__init__(api_key, api_url=api_url, timeout=timeout)
-        self.engine: str = "dall-e-3"
-
-    def generate(
-        self,
-        prompt: str,
-        model: str = None,
-        **kwargs,
-    ):
-        url = self.api_url.image_url
-        headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
-
-        json_post = {
-                "model": os.environ.get("IMAGE_MODEL_NAME") or model or self.engine,
-                "prompt": prompt,
-                "n": 1,
-                "size": "1024x1024",
-        }
-        try:
-            response = self.session.post(
-                url,
-                headers=headers,
-                json=json_post,
-                timeout=kwargs.get("timeout", self.timeout),
-                stream=True,
-            )
-        except ConnectionError:
-            print("连接错误，请检查服务器状态或网络连接。")
-            return
-        except requests.exceptions.ReadTimeout:
-            print("请求超时，请检查网络连接或增加超时时间。{e}")
-            return
-        except Exception as e:
-            print(f"发生了未预料的错误: {e}")
-            return
-
-        if response.status_code != 200:
-            raise Exception(f"{response.status_code} {response.reason} {response.text}")
-        json_data = json.loads(response.text)
-        url = json_data["data"][0]["url"]
-        yield url
+            self.__dict__.update({key: loaded_config[key] for key in keys})
```

### Comparing `modelmerge-0.4.3/src/ModelMerge/models/claude.py` & `modelmerge-0.4.4/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/models/config.py` & `modelmerge-0.4.4/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/models/genimi.py` & `modelmerge-0.4.4/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/models/groq.py` & `modelmerge-0.4.4/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/plugins/tarvel.py` & `modelmerge-0.4.4/src/ModelMerge/plugins/tarvel.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.4.4/src/ModelMerge/plugins/websearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 import threading
 import time as record_time
 from itertools import islice
 from bs4 import BeautifulSoup
 from duckduckgo_search import DDGS
 from googleapiclient.discovery import build
 
-from ..models import chatgpt
-
-
 class ThreadWithReturnValue(threading.Thread):
     def run(self):
         if self._target is not None:
             self._return = self._target(*self._args, **self._kwargs)
 
     def join(self):
         super().join()
@@ -229,16 +226,16 @@
 
     url_text_list = yield from get_url_text_list(keywords, search_url_num)
     useful_source_text = "\n\n".join(url_text_list)
     return useful_source_text
 
 if __name__ == "__main__":
     os.system("clear")
-    from ModelMerge.models import chatgpt
-    print(get_search_results("今天的微博热搜有哪些？", chatgpt.chatgpt_api_url.v1_url))
+    # from ModelMerge.models import chatgpt
+    # print(get_search_results("今天的微博热搜有哪些？", chatgpt.chatgpt_api_url.v1_url))
 
     # # 搜索
 
     # for i in search_web_and_summary("今天的微博热搜有哪些？"):
     # for i in search_web_and_summary("给出清华铊中毒案时间线，并作出你的评论。"):
     # for i in search_web_and_summary("红警hbk08是谁"):
     # for i in search_web_and_summary("国务院 2024 放假安排"):
```

### Comparing `modelmerge-0.4.3/src/ModelMerge/tools/function_call.py` & `modelmerge-0.4.4/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/utils/prompt.py` & `modelmerge-0.4.4/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/ModelMerge/utils/scripts.py` & `modelmerge-0.4.4/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.4.4/src/modelmerge.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.4.3
+Version: 0.4.4
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: PyExecJS
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
```

### Comparing `modelmerge-0.4.3/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.4.4/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_Web_crawler.py` & `modelmerge-0.4.4/test/test_Web_crawler.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_claude_zh_char.py` & `modelmerge-0.4.4/test/test_claude_zh_char.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_ddg_search.py` & `modelmerge-0.4.4/test/test_ddg_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_download_pdf.py` & `modelmerge-0.4.4/test/test_download_pdf.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_google_search.py` & `modelmerge-0.4.4/test/test_google_search.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_jieba.py` & `modelmerge-0.4.4/test/test_jieba.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_json.py` & `modelmerge-0.4.4/test/test_json.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_langchain_search_old.py` & `modelmerge-0.4.4/test/test_langchain_search_old.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_logging.py` & `modelmerge-0.4.4/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_ollama.py` & `modelmerge-0.4.4/test/test_ollama.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_tikitoken.py` & `modelmerge-0.4.4/test/test_tikitoken.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_token.py` & `modelmerge-0.4.4/test/test_token.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.4.3/test/test_url.py` & `modelmerge-0.4.4/test/test_url.py`

 * *Files identical despite different names*

