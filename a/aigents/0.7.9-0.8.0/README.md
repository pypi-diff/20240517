# Comparing `tmp/aigents-0.7.9.tar.gz` & `tmp/aigents-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.7.9.tar", max compression
+gzip compressed data, was "aigents-0.8.0.tar", max compression
```

## Comparing `aigents-0.7.9.tar` & `aigents-0.8.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.7.9/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.7.9/README.md
--rw-r--r--   0        0        0     1044 2024-05-10 17:25:02.079544 aigents-0.7.9/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.7.9/src/aigents/__init__.py
--rw-r--r--   0        0        0    19383 2024-03-15 16:50:10.476341 aigents-0.7.9/src/aigents/base.py
--rw-r--r--   0        0        0     1144 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.7.9/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.7.9/src/aigents/context/base.py
--rw-r--r--   0        0        0    13079 2024-05-06 23:50:53.193957 aigents-0.7.9/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.7.9/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.7.9/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.7.9/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.7.9/src/aigents/context/utils.py
--rw-r--r--   0        0        0    31095 2024-03-14 11:18:28.044644 aigents-0.7.9/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.7.9/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.7.9/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.7.9/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.7.9/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.7.9/src/aigents/utils.py
--rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.8.0/README.md
+-rw-r--r--   0        0        0     1044 2024-05-17 18:43:57.599711 aigents-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.8.0/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19580 2024-05-17 17:53:53.908658 aigents-0.8.0/src/aigents/base.py
+-rw-r--r--   0        0        0     1238 2024-05-17 18:41:32.446222 aigents-0.8.0/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.8.0/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.8.0/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13227 2024-05-15 19:26:29.333058 aigents-0.8.0/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.8.0/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.8.0/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.8.0/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.8.0/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    32013 2024-05-17 18:47:54.121371 aigents-0.8.0/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.8.0/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.8.0/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.8.0/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.8.0/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/utils.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.8.0/PKG-INFO
```

### Comparing `aigents-0.7.9/LICENSE` & `aigents-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/README.md` & `aigents-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/pyproject.toml` & `aigents-0.8.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.7.9"
+version = "0.8.0"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -15,22 +15,22 @@
 repository = "https://github.com/bessavagner/aigents.git"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^1.12.0"
 tiktoken = "^0.6.0"
 python-dotenv = "^1.0.1"
-google-generativeai = "^0.3.2"
 tomlkit = "^0.12.4"
 pillow = "^10.2.0"
 g4f = {extras = ["all"], version = "^0.2.4.1"}
 spacy = "^3.7.4"
 pandas = "^2.2.2"
 scipy = "^1.13.0"
 nltk = "^3.8.1"
+google-generativeai = "^0.5.4"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.22.1"
 ipykernel = "^6.29.2"
 tomlkit = "^0.12.3"
 
 [build-system]
```

### Comparing `aigents-0.7.9/src/aigents/__init__.py` & `aigents-0.8.0/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/base.py` & `aigents-0.8.0/src/aigents/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,23 +472,28 @@
                 large messages
             agent (Agent):
                 Any agent instance that has 'answer' method implemented.
 
         Returns:
             None
         """
-        n_tokens = self.client.count_tokens(self.messages)
+        client = self.client
+        if self.model == MODELS[6]:
+            n_tokens = self.client.count_tokens(self.messages)
+        else:
+            client = genai.GenerativeModel(model_name=MODELS[6])
+            n_tokens = client.count_tokens(self.messages)
         while n_tokens.total_tokens > self.max_tokens:
             if use_agent and len(self.messages) > 2:
                 # Attempt to summarize the conversation
                 summary_prompt = (
                     "Please summarize the following conversation "
                     "(IMPORTANT: keep the user's language):\n"
                 )
-                if self.set_up:
+                if self.setup:
                     summary_prompt += "\n".join(
                         message['parts'] for message in self.messages[1:-1]
                     )
                 else:
                     summary_prompt += "\n".join(
                         message['parts'] for message in self.messages[:-1]
                     )
@@ -497,15 +502,15 @@
                     prompt=summary_prompt,
                     use_agent=False,
                     conversation=False
                 )
 
                 # Replace the conversation with the summary and the
                 # last message
-                if self.set_up:
+                if self.setup:
                     self.messages = [
                         self.messages[0],
                         {'role': ROLES[1], 'parts': [summary_content]},
                         self.messages[-1]
                     ]
                 else:
                     self.messages = [
@@ -516,33 +521,33 @@
                 if DEBUG:
                     logger.info(
                         'Conversation summarized: %s', summary_content
                     )
             else:
                 # Remove the oldest message if summarization is not possible
                 # or did not help
-                if self.set_up:
+                if self.setup:
                     removed_message = self.messages.pop(1)
                 else:
                     removed_message = self.messages.pop(0)
                 if DEBUG:
                     logger.warning(
                         'Oldest removed message: %s',
                         removed_message['parts']
                     )
 
             # Recalculate the number of tokens after modification
-            n_tokens = self.client.count_tokens(self.messages)
+            n_tokens = client.count_tokens(self.messages)
 
             if n_tokens.total_tokens <= self.max_tokens:
                 break  # Exit the loop if we are within the token limit
 
             if len(self.messages) <= 2:
                 # If we cannot reduce further, raise an error
-                if self.set_up or len(self.messages) == 1:
+                if self.setup or len(self.messages) == 1:
                     raise MessageError(
                         'Conversation exceeds maximum number of '
                         'tokens and cannot be reduced further.'
                     )
 
 
 class BingChatterMixin(OpenAIChatterMixin):
```

### Comparing `aigents-0.7.9/src/aigents/constants.py` & `aigents-0.8.0/src/aigents/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,34 @@
 https://platform.openai.com/docs/models
 """
 
 MODELS = (
     'gpt-3.5-turbo-0125',
     'gpt-3.5-turbo-1106',
     'gpt-4-turbo-preview',
-    'gpt-4-0125-preview',  # 3
+    'gpt-4o',  # 3
     'gpt-4-1106-preview',
     'gpt-4-vision-preview',
-    'gemini-pro',  # Google # 6
-    'gemini-pro-vision'
+    'gemini-1.0-pro',  # Google # 6
+    'gemini-1.0-pro-vision',
+    'gemini-1.5-flash',
+    'gemini-1.5-pro'
 )
 
 MAX_TOKENS = (
     (MODELS[0], 16385),
     (MODELS[1], 16385),
     (MODELS[2], 8192),
     (MODELS[3], 128000),
     (MODELS[4], 128000),
     (MODELS[5], 128000),
     (MODELS[6], 30720),
     (MODELS[7], 12288),
+    (MODELS[8], 1048576),
+    (MODELS[9], 1048576),
 )
 
 ROLES = (  # roles for messages objects
     'system',
     'user',
     'assistant',
     'model'  # Google gemini
```

### Comparing `aigents-0.7.9/src/aigents/context/base.py` & `aigents-0.8.0/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/context/core.py` & `aigents-0.8.0/src/aigents/context/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             organization=organization,
             **kwargs
         )
         self.question_embedding = None
         self.pipeline: str = None
         self.embeddings_generator: str = None
         self.embedding_model: str = None
+        self.language: str = None
 
     async def generate_embeddings(
             self,
             source: str | pd.DataFrame | Path | dict = None,
             model: str = MODELS[0],
             max_tokens: int = None,  # tokens per chunk
             embeddings_generator: str | Coroutine = naive_text_to_embeddings_async,
@@ -199,22 +200,24 @@
                     except ValueError as err:
                         if 'unpack' in str(err):
                             message = (
                                 "`embeddings_generator` must be a spacy "
                                 "pipeline and a model (either `openai`or "
                                 "`gemini`) separated by a comma"
                             )
-                            message = f"{message}: {err.message}"
+                            err_message = getattr(err, 'message', str(err))
+                            message = f"{message}: {err_message}"
                             raise ContextError(message) from err
                     try:
                         self.embeddings = await to_embeddings_async(
                             source,
                             self.pipeline.strip(),
                             max_tokens=max_tokens,
-                            embedding_model=self.embedding_model.strip()
+                            embedding_model=self.embedding_model.strip(),
+                            **kwargs
                         )
                     except ProcessingError as err:
                         raise ContextError(err.message) from err
                 elif inspect.iscoroutinefunction(embeddings_generator):
                     self.embeddings = await embeddings_generator(
                         source,
                         model=model,
```

### Comparing `aigents-0.7.9/src/aigents/context/nlp/base.py` & `aigents-0.8.0/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/context/nlp/processors.py` & `aigents-0.8.0/src/aigents/context/nlp/processors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/context/nlp/utils.py` & `aigents-0.8.0/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/context/utils.py` & `aigents-0.8.0/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/core.py` & `aigents-0.8.0/src/aigents/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
 
 class GoogleChatter(GoogleChatterMixin, BaseChatter):
     def __init__(self,
                  *args,
                  setup: str = None,
                  api_key: str = None,
                  temperature: float = 0.0,
+                 model=MODELS[6],
                  **kwargs):
         """
         Initialize a Google based Chatter instance.
 
         Parameters
         ----------
         *args:
@@ -292,15 +293,15 @@
         -------
         None
         """
         super().__init__(*args,
                          setup=setup,
                          api_key=api_key,
                          temperature=temperature,
-                         model=MODELS[6],
+                         model=model,
                          **kwargs)
 
     def answer(self,
                prompt,
                use_agent=True,
                conversation=True,
                agent=None,
@@ -322,26 +323,32 @@
             ]
         else:
             messages = self.messages if conversation else self.messages[-2:]
 
         config = genai.types.GenerationConfig(temperature=self.temperature)
 
         response = self.client.generate_content(
-            messages, generation_config=config
+            messages, generation_config=config,**kwargs
         )
         self.last_response = response
         try:
             self._update(
                 ROLES[-1],
                 response.text,
                 use_agent=use_agent,
                 agent=agent
             )
             return response.text
         except ValueError:
+            if len(response.candidates[0].content.parts) == 0:
+                message = (
+                    "Model didn't return any message. "
+                    f"Finish reason: {response.candidates[0].finish_reason.name}"
+                )
+                raise AgentError(message) from err
             text = '\n'.join(
                 [part.text for part in response.candidates[0].content.parts]
             )
             self._update(
                 ROLES[-1],
                 text,
                 use_agent=use_agent,
@@ -391,17 +398,18 @@
                          setup=setup,
                          api_key=api_key,
                          temperature=temperature,
                          **kwargs)
 
     async def answer(self,
                      prompt,
-                     use_agent=True,
-                     conversation=True,
-                     agent=None,
+                     use_agent: bool = True,
+                     conversation: bool = True,
+                     agent: str = None,
+                     generation_config_dict: dict = None,
                      **kwargs):
         if use_agent and agent is None:
             setup = (
                 "You are a very skilled writer that can summarize any text "
                 "while preserving the whole meaning of its content."
             )
             agent = GoogleChatter(setup=setup, api_key=self.api_key)
@@ -412,26 +420,34 @@
         
         if self.setup:
             messages = self.messages if conversation else [
                 *self.messages[:2], self.messages[-1]
             ]
         else:
             messages = self.messages if conversation else self.messages[-2:]
-        
-        config = genai.types.GenerationConfig(temperature=self.temperature)
+        if generation_config_dict is None:
+            generation_config_dict = {}
+        generation_config_dict['temperature'] = self.temperature
+        config = genai.types.GenerationConfig(**generation_config_dict)
         response = await self.client.generate_content_async(
-            messages, generation_config=config
+            messages, generation_config=config, **kwargs
         )
-
+        self.last_response = response
         try:
             self._update(
                 ROLES[-1], response.text, use_agent=use_agent, agent=agent
             )
             return response.text
         except ValueError:
+            if len(response.candidates[0].content.parts) == 0:
+                message = (
+                    "Model didn't return any message. "
+                    f"Finish reason: {response.candidates[0].finish_reason.name}"
+                )
+                raise AgentError(message) from err
             text = '\n'.join(
                 [part.text for part in response.candidates[0].content.parts]
             )
             self._update(
                 ROLES[-1],
                 text,
                 use_agent=use_agent,
@@ -517,15 +533,15 @@
         # TODO: add messages system
         if isinstance(img, (str, Path)):
             img = Image.open(img)
         message = img
         if prompt:
             message = [prompt, img]
         response = self.client.generate_content(
-            message
+            message, **kwargs
         )
         try:
             return response.text
         except ValueError:
             if len(response.candidates) == 0:
                 logger.error(
                     "Prompt was blocked: %s.\nPrompt: %s",
@@ -616,15 +632,15 @@
         # TODO: add messages system
         if isinstance(img, (str, Path)):
             img = Image.open(img)
         message = img
         if prompt:
             message = [prompt, img]
         response = await self.client.generate_content_async(
-            message
+            message, **kwargs
         )
         try:
             return response.text
         except ValueError:
             if len(response.candidates) == 0:
                 logger.error(
                     "Prompt was blocked: %s.\nPrompt: %s",
```

### Comparing `aigents-0.7.9/src/aigents/errors.py` & `aigents-0.8.0/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/prompts.py` & `aigents-0.8.0/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/settings.py` & `aigents-0.8.0/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/src/aigents/utils.py` & `aigents-0.8.0/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.7.9/PKG-INFO` & `aigents-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.7.9
+Version: 0.8.0
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: g4f[all] (>=0.2.4.1,<0.3.0.0)
-Requires-Dist: google-generativeai (>=0.3.2,<0.4.0)
+Requires-Dist: google-generativeai (>=0.5.4,<0.6.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: openai (>=1.12.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pillow (>=10.2.0,<11.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: spacy (>=3.7.4,<4.0.0)
```

