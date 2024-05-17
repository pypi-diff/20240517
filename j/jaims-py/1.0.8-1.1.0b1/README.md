# Comparing `tmp/jaims-py-1.0.8.tar.gz` & `tmp/jaims-py-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaims-py-1.0.8.tar", last modified: Tue Mar 19 15:03:56 2024, max compression
+gzip compressed data, was "jaims-py-1.1.0b1.tar", last modified: Tue Dec 12 17:01:37 2023, max compression
```

## Comparing `jaims-py-1.0.8.tar` & `jaims-py-1.1.0b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-03-19 15:03:56.805718 jaims-py-1.0.8/
--rw-r--r--   0 mush       (501) staff       (20)     4148 2024-03-19 15:03:56.805583 jaims-py-1.0.8/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)     3838 2023-11-28 15:46:12.000000 jaims-py-1.0.8/README.md
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-03-19 15:03:56.804460 jaims-py-1.0.8/jaims/
--rw-r--r--   0 mush       (501) staff       (20)      352 2024-02-22 15:03:29.000000 jaims-py-1.0.8/jaims/__init__.py
--rw-r--r--   0 mush       (501) staff       (20)    14674 2024-02-22 15:03:29.000000 jaims-py-1.0.8/jaims/agent.py
--rw-r--r--   0 mush       (501) staff       (20)     2066 2024-02-22 15:03:29.000000 jaims-py-1.0.8/jaims/exceptions.py
--rw-r--r--   0 mush       (501) staff       (20)     8967 2024-02-22 15:04:04.000000 jaims-py-1.0.8/jaims/function_handler.py
--rw-r--r--   0 mush       (501) staff       (20)     8980 2024-02-22 15:03:29.000000 jaims-py-1.0.8/jaims/history_manager.py
--rw-r--r--   0 mush       (501) staff       (20)    14112 2024-03-19 14:58:47.000000 jaims-py-1.0.8/jaims/openai_wrappers.py
--rw-r--r--   0 mush       (501) staff       (20)      293 2023-11-28 15:46:12.000000 jaims-py-1.0.8/jaims/transaction_storage.py
-drwxr-xr-x   0 mush       (501) staff       (20)        0 2024-03-19 15:03:56.805358 jaims-py-1.0.8/jaims_py.egg-info/
--rw-r--r--   0 mush       (501) staff       (20)     4148 2024-03-19 15:03:56.000000 jaims-py-1.0.8/jaims_py.egg-info/PKG-INFO
--rw-r--r--   0 mush       (501) staff       (20)      335 2024-03-19 15:03:56.000000 jaims-py-1.0.8/jaims_py.egg-info/SOURCES.txt
--rw-r--r--   0 mush       (501) staff       (20)        1 2024-03-19 15:03:56.000000 jaims-py-1.0.8/jaims_py.egg-info/dependency_links.txt
--rw-r--r--   0 mush       (501) staff       (20)       46 2024-03-19 15:03:56.000000 jaims-py-1.0.8/jaims_py.egg-info/requires.txt
--rw-r--r--   0 mush       (501) staff       (20)        6 2024-03-19 15:03:56.000000 jaims-py-1.0.8/jaims_py.egg-info/top_level.txt
--rw-r--r--   0 mush       (501) staff       (20)       38 2024-03-19 15:03:56.805763 jaims-py-1.0.8/setup.cfg
--rw-r--r--   0 mush       (501) staff       (20)      606 2024-03-19 15:01:07.000000 jaims-py-1.0.8/setup.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-12-12 17:01:37.115554 jaims-py-1.1.0b1/
+-rw-r--r--   0 mush       (501) staff       (20)     4170 2023-12-12 17:01:37.115430 jaims-py-1.1.0b1/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)     3838 2023-11-28 15:46:12.000000 jaims-py-1.1.0b1/README.md
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-12-12 17:01:37.114695 jaims-py-1.1.0b1/jaims/
+-rw-r--r--   0 mush       (501) staff       (20)      366 2023-12-12 16:58:26.000000 jaims-py-1.1.0b1/jaims/__init__.py
+-rw-r--r--   0 mush       (501) staff       (20)    14915 2023-12-12 17:00:49.000000 jaims-py-1.1.0b1/jaims/agent.py
+-rw-r--r--   0 mush       (501) staff       (20)     2066 2023-08-20 20:05:09.000000 jaims-py-1.1.0b1/jaims/exceptions.py
+-rw-r--r--   0 mush       (501) staff       (20)     8592 2023-11-28 15:46:12.000000 jaims-py-1.1.0b1/jaims/function_handler.py
+-rw-r--r--   0 mush       (501) staff       (20)     8980 2023-12-01 15:21:35.000000 jaims-py-1.1.0b1/jaims/history_manager.py
+-rw-r--r--   0 mush       (501) staff       (20)    14217 2023-12-12 16:58:26.000000 jaims-py-1.1.0b1/jaims/openai_wrappers.py
+-rw-r--r--   0 mush       (501) staff       (20)      293 2023-11-28 15:46:12.000000 jaims-py-1.1.0b1/jaims/transaction_storage.py
+drwxr-xr-x   0 mush       (501) staff       (20)        0 2023-12-12 17:01:37.115259 jaims-py-1.1.0b1/jaims_py.egg-info/
+-rw-r--r--   0 mush       (501) staff       (20)     4170 2023-12-12 17:01:37.000000 jaims-py-1.1.0b1/jaims_py.egg-info/PKG-INFO
+-rw-r--r--   0 mush       (501) staff       (20)      335 2023-12-12 17:01:37.000000 jaims-py-1.1.0b1/jaims_py.egg-info/SOURCES.txt
+-rw-r--r--   0 mush       (501) staff       (20)        1 2023-12-12 17:01:37.000000 jaims-py-1.1.0b1/jaims_py.egg-info/dependency_links.txt
+-rw-r--r--   0 mush       (501) staff       (20)       45 2023-12-12 17:01:37.000000 jaims-py-1.1.0b1/jaims_py.egg-info/requires.txt
+-rw-r--r--   0 mush       (501) staff       (20)        6 2023-12-12 17:01:37.000000 jaims-py-1.1.0b1/jaims_py.egg-info/top_level.txt
+-rw-r--r--   0 mush       (501) staff       (20)       38 2023-12-12 17:01:37.115600 jaims-py-1.1.0b1/setup.cfg
+-rw-r--r--   0 mush       (501) staff       (20)      613 2023-12-12 17:01:06.000000 jaims-py-1.1.0b1/setup.py
```

### Comparing `jaims-py-1.0.8/PKG-INFO` & `jaims-py-1.1.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 1.0.8
+Version: 1.1.0b1
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: OpenAI GPT-3 and GPT-4 function enabled agent
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img width="300" src="https://github.com/dev-mush/jaims-py/assets/669003/5c53381f-25b5-4141-bcd2-7457863eafb9" >
 </p>
 
 
@@ -138,7 +139,9 @@
 - [ ] Add more chat history optimization strategies
 - [ ] Add function calling callbacks 
 - [ ] Add history persistance
 
 ## 📝 License
 
 The license will be MIT, but I need to add this properly.
+
+
```

### Comparing `jaims-py-1.0.8/README.md` & `jaims-py-1.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `jaims-py-1.0.8/jaims/agent.py` & `jaims-py-1.1.0b1/jaims/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,21 +78,25 @@
     """
 
     def __init__(
         self,
         openai_kwargs: JAImsOpenaiKWArgs = JAImsOpenaiKWArgs(),
         options: JAImsOptions = JAImsOptions(),
         openai_api_key: Optional[str] = None,
+        openai_base_url: Optional[str] = None,
         transaction_storage: Optional[JAImsTransactionStorageInterface] = None,
     ):
         openai_api_key = openai_api_key or os.getenv("OPENAI_API_KEY")
         if not openai_api_key:
             raise JAImsMissingOpenaiAPIKeyException()
-        openai.api_key = openai_api_key
 
+        self.__openai_client = openai.OpenAI(
+            api_key=openai_api_key,
+            base_url=openai_base_url,
+        )
         self.__openai_kwargs = openai_kwargs
         self.__options = options
         self.__expense = JAImsAgent.__init_expense_dictionary()
         self.__last_run_expense = JAImsAgent.__init_expense_dictionary()
         self.__function_handler = JAImsFunctionHandler()
         self.__history_manager = HistoryManager()
         if transaction_storage is None:
@@ -136,14 +140,15 @@
             options=call_context.options,
             openai_kwargs=call_context.openai_kwargs,
         )
 
         call_context.openai_kwargs.messages = messages
 
         response = get_openai_response(
+            self.__openai_client,
             call_context.openai_kwargs,
             call_context.options,
         )
 
         if isinstance(response, openai.Stream):
             return self.__handle_streaming_response(response, call_context)
         else:
@@ -217,15 +222,15 @@
 
         message_dict = message.model_dump(exclude_none=True)
         self.__history_manager.add_messages([message_dict])
 
         if message.tool_calls:
             result_messages = self.__function_handler.handle_from_message(
                 message=message_dict,
-                function_wrappers=call_context.openai_kwargs.tools or [],
+                functions=call_context.openai_kwargs.tools or [],
             )
             if call_context.openai_kwargs.tool_choice == "auto":
                 self.__history_manager.add_messages(result_messages)
                 return self.__call_openai(call_context)
 
         # if the response was streaming only an empty string must be returned
         # because the streaming generator already yielded the response, otherwise
@@ -268,14 +273,16 @@
                 gpt_model=call_context.openai_kwargs.model,
                 prompt_tokens=prompt_tokens,
                 completion_tokens=completion_tokens,
                 total_tokens=total_tokens,
                 rough_estimate=True,
             )
 
+        if expense.gpt_model.string not in self.__expense:
+            return
         self.__last_run_expense[expense.gpt_model.string].add_from(expense)
         self.__expense[expense.gpt_model.string].add_from(expense)
 
     def get_expenses(self):
         """
         Returns the tokens spent in the current session in an array, one for each model.
         """
```

### Comparing `jaims-py-1.0.8/jaims/exceptions.py` & `jaims-py-1.1.0b1/jaims/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaims-py-1.0.8/jaims/function_handler.py` & `jaims-py-1.1.0b1/jaims/function_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,51 +91,65 @@
 
         if self.enum_values:
             schema["enum"] = self.enum_values
 
         return schema
 
 
-class JAImsToolDescriptor:
+class JAImsFuncWrapper:
     """
-    Describes a tool to be used in the OPENAI API. Supports only function tool for now.
+    Wraps a function call to be used in the OPENAI API.
+    Holds the function to be called as well as the function name, its description that the agent will understand,
+    and the response json schema.
 
     Attributes
     ----------
+        function : Callable[..., Any]
+            the function to be called
         name : str
-            the tool name
+            the function name
         description : str
-            the tool description
+            the function description
         params_descriptors: List[JAImsParamDescriptor]
             the list of parameters descriptors
+
+    Methods
+    -------
+        call(params: Dict[str, Any]) -> Any
+            calls the function with the given parameters
+        get_jsonapi_schema() -> Dict[str, Any]
+            returns the jsonapi schema for the function
     """
 
     def __init__(
         self,
+        function: Callable[..., Any],
         name: str,
         description: str,
         params_descriptors: List[JAImsParamDescriptor],
     ):
+        self.function = function
         self.name = name
         self.description = description
         self.params_descriptors = params_descriptors
 
-    def to_openai_function_tool(self):
-        return {
-            "type": "function",
-            "function": {
-                "name": self.name,
-                "description": self.description,
-                "parameters": self.get_jsonapi_schema(),
-            },
-        }
+    def call(self, params: Dict[str, Any]) -> Any:
+        """
+        Calls the function with the given parameters.
+
+        Parameters
+        ----------
+            params : dict
+                the parameters to be passed to the function
+        """
+        return self.function(**params)
 
     def get_jsonapi_schema(self) -> Dict[str, Any]:
         """
-        Returns the jsonapi schema for function.
+        Returns the jsonapi schema for the function.
         """
         schema = {
             "type": "object",
             "properties": {},
             "required": [],
         }
 
@@ -143,70 +157,27 @@
             schema["properties"][param.name] = param.get_jsonapi_schema()
             if param.required:
                 schema["required"].append(param.name)
 
         return schema
 
 
-class JAImsFuncWrapper:
-    """
-    Wraps a tool used by the OPENAI API along with a function to be called locally when
-    the tool is invoked by openai.
-
-
-    Attributes
-    ----------
-        function : Callable[..., Any]
-            the function to be called
-        name : str
-            the function name
-        description : str
-            the function description
-        params_descriptors: List[JAImsParamDescriptor]
-            the list of parameters descriptors
-
-    Methods
-    -------
-        call(params: Dict[str, Any]) -> Any
-            calls the wrapped function with the given parameters
-    """
-
-    def __init__(
-        self,
-        function: Callable[..., Any],
-        function_tool: JAImsToolDescriptor,
-    ):
-        self.function = function
-        self.function_tool = function_tool
-
-    def call(self, params: Dict[str, Any]) -> Any:
-        """
-        Calls the function with the given parameters.
-
-        Parameters
-        ----------
-            params : dict
-                the parameters to be passed to the function
-        """
-        return self.function(**params)
-
-
 class JAImsFunctionHandler:
     """
     Handles the functions to be used in the OPENAI API.
     Holds a list of JAImsFuncWrapper instances.
 
     Attributes
     ----------
         functions : List[JAImsFuncWrapper]
             the list of functions to be called
     """
 
     def handle_from_message(
-        self, message: Dict[str, Any], function_wrappers: List[JAImsFuncWrapper]
+        self, message: Dict[str, Any], functions: List[JAImsFuncWrapper]
     ) -> List[Dict[str, Any]]:
         """
         Handles a function_call message, calling the appropriate function.
 
         Parameters
         ----------
             message : dict
@@ -228,32 +199,31 @@
             tool_call_id = tool_call["id"]
             function_name = tool_call["function"]["name"]
             function_args = tool_call["function"]["arguments"]
             function_calls.append(
                 {
                     "tool_call_id": tool_call_id,
                     "name": function_name,
-                    "args": json.loads(function_args, strict=False) if function_args else {},
+                    "args": json.loads(function_args) if function_args else {},
                 }
             )
 
         # invoke function
-        return self.__call_functions(function_calls, function_wrappers)
+        return self.__call_functions(function_calls, functions)
 
     def __call_functions(
-        self, function_calls: List[dict], function_wrappers: List[JAImsFuncWrapper]
+        self, function_calls: List[dict], functions
     ) -> List[dict[str, Any]]:
         # Check if function_name exists in functions, if not, raise UnexpectedFunctionCallException
 
         results = []
         for fc in function_calls:
             function_name = fc["name"]
             function_wrapper = next(
-                (f for f in function_wrappers if f.function_tool.name == function_name),
-                None,
+                (f for f in functions if f.name == function_name), None
             )
             if not function_wrapper:
                 raise JAImsUnexpectedFunctionCall(function_name)
 
             try:
                 fc_result = function_wrapper.function(**fc["args"])
                 results.append(
@@ -276,13 +246,24 @@
 
         # If the name of the current function matches the provided name
         # Call the function and return its result
         return results
 
 
 def parse_function_wrappers_to_tools(
-    func_wrappers: List[JAImsFuncWrapper],
+    functions: List[JAImsFuncWrapper],
 ) -> List[Dict[str, Any]]:
-    return [
-        func_wrapper.function_tool.to_openai_function_tool()
-        for func_wrapper in func_wrappers
-    ]
+    openai_functions = []
+    for function in functions:
+        function_data = {
+            k: v
+            for k, v in {
+                "name": function.name,
+                "description": function.description,
+                "parameters": function.get_jsonapi_schema(),
+            }.items()
+            if v is not None
+        }
+
+        openai_functions.append({"type": "function", "function": function_data})
+
+    return openai_functions
```

### Comparing `jaims-py-1.0.8/jaims/history_manager.py` & `jaims-py-1.1.0b1/jaims/history_manager.py`

 * *Files identical despite different names*

### Comparing `jaims-py-1.0.8/jaims/openai_wrappers.py` & `jaims-py-1.1.0b1/jaims/openai_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,39 @@
 from __future__ import annotations
 
 from enum import Enum
 import time
 from typing import Any, List, Optional, Dict, Union
 import openai
-from openai import OpenAI
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 from openai import Stream
 import tiktoken
 import logging
 import random
+import json
 
 from jaims.function_handler import JAImsFuncWrapper, parse_function_wrappers_to_tools
 
-DEFAULT_MAX_TOKENS = 1024
+DEFAULT_MAX_TOKENS = 512
 MAX_CONSECUTIVE_CALLS = 10
 
 
-class JAImsGPTModel(Enum):
+class BaseGPTModel:
+    def __init__(self, string, max_tokens, price_1k_tokens_in, price_1k_tokens_out, tokenizer):
+        self.string = string
+        self.max_tokens = max_tokens
+        self.price_1k_tokens_in = price_1k_tokens_in
+        self.price_1k_tokens_out = price_1k_tokens_out
+        self.tokenizer = tokenizer
+
+    def __str__(self):
+        return self.string
+
+
+class JAImsGPTModel(BaseGPTModel, Enum):
     """
     The OPENAI GPT models available.
     Only those that support functions are listed, so just:
     gpt-3.5-turbo-0613, gpt-3-5-turbo-16k-0613, gpt-4-0613
     """
 
     GPT_3_5_TURBO = ("gpt-3.5-turbo", 4096, 0.0015, 0.002)
@@ -30,27 +42,19 @@
     GPT_3_5_TURBO_16K_0613 = ("gpt-3.5-turbo-16k-0613", 16384, 0.003, 0.004)
     GPT_3_5_TURBO_1106 = ("gpt-3.5-turbo-1106", 16385, 0.001, 0.002)
     GPT_4 = ("gpt-4", 8192, 0.03, 0.06)
     GPT_4_32K = ("gpt-4-32k", 32768, 0.06, 0.12)
     GPT_4_0613 = ("gpt-4-0613", 8192, 0.03, 0.06)
     GPT_4_32K_0613 = ("gpt-4-32k-0613", 32768, 0.06, 0.12)
     GPT_4_1106_PREVIEW = ("gpt-4-1106-preview", 128000, 0.01, 0.03)
-    GPT_4_0125_PREVIEW = ("gpt-4-0125-preview", 128000, 0.01, 0.03)
-    GPT_4_TURBO_PREVIEW = ("gpt-4-turbo-preview", 128000, 0.01, 0.03)
-    GPT_4_1106_VISION_PREVIEW = ("gpt-4-1106-vision-preview", 128000, 0.01, 0.03)
     GPT_4_VISION_PREVIEW = ("gpt-4-vision-preview", 128000, 0.01, 0.03)
 
     def __init__(self, string, max_tokens, price_1k_tokens_in, price_1k_tokens_out):
-        self.string = string
-        self.max_tokens = max_tokens
-        self.price_1k_tokens_in = price_1k_tokens_in
-        self.price_1k_tokens_out = price_1k_tokens_out
-
-    def __str__(self):
-        return self.string
+        super().__init__(string, max_tokens, price_1k_tokens_in,
+                         price_1k_tokens_out, tiktoken.encoding_for_model)
 
 
 class JAImsTokensExpense:
     """
     Tracks the number of tokens spent on a job and on which GPTModel.
     """
 
@@ -119,16 +123,18 @@
             "cost": self.get_cost(),
             "rough_estimate": self.rough_estimate,
         }
 
 
 def estimate_token_count(string: str, model: JAImsGPTModel) -> int:
     """Returns the number of tokens in a text string."""
+    if not model.tokenizer:
+        return 0
 
-    encoding = tiktoken.encoding_for_model(model.string)
+    encoding = model.tokenizer(model.string)
     num_tokens = len(encoding.encode(string))
     return num_tokens
 
 
 class ErrorHandlingMethod(Enum):
     FAIL = "fail"
     RETRY = "retry"
@@ -221,15 +227,16 @@
             "seed": self.seed,
             "frequency_penalty": self.frequency_penalty,
             "presence_penalty": self.presence_penalty,
             "response_format": self.response_format,
             "stop": self.stop,
         }
 
-        kwargs = {key: value for key, value in kwargs.items() if value is not None}
+        kwargs = {key: value for key,
+                  value in kwargs.items() if value is not None}
 
         if self.logit_bias:
             kwargs["logit_bias"] = self.logit_bias
 
         if self.tools:
             kwargs["tools"] = parse_function_wrappers_to_tools(self.tools)
             kwargs["tool_choice"] = self.tool_choice
@@ -257,15 +264,15 @@
     """
 
     def __init__(
         self,
         leading_prompts: Optional[List[Dict]] = None,
         trailing_prompts: Optional[List[Dict]] = None,
         max_consecutive_function_calls: int = MAX_CONSECUTIVE_CALLS,
-        optimize_context: bool = False,
+        optimize_context: bool = True,
         message_history_size: Optional[int] = None,
         max_retries=15,
         retry_delay=10,
         exponential_base: int = 2,
         exponential_delay: int = 1,
         exponential_cap: Optional[int] = None,
         jitter: bool = True,
@@ -282,32 +289,31 @@
         self.exponential_delay = exponential_delay
         self.exponential_cap = exponential_cap
         self.jitter = jitter
         self.debug_stream_function_call = debug_stream_function_call
 
 
 def get_openai_response(
+    openai_client: openai.OpenAI,
     openai_kw_args: JAImsOpenaiKWArgs,
     call_options: JAImsOptions,
 ) -> Union[ChatCompletion, Stream[ChatCompletionChunk]]:
     retries = 0
     logger = logging.getLogger(__name__)
     # keeps how long to sleep between retries
     sleep_time = call_options.retry_delay
     # keeps track of the exponential backoff
     backoff_time = call_options.exponential_delay
 
     # print(json.dumps(openai_kw_args.messages, indent=4))
 
     while retries < call_options.max_retries:
         try:
-            client = OpenAI()
-            kwargs = openai_kw_args.to_dict()
-            response = client.chat.completions.create(
-                **kwargs,
+            response = openai_client.chat.completions.create(
+                **openai_kw_args.to_dict(),
             )
 
             return response
         except openai.OpenAIError as error:
             logger.error(f"OpenAI API error:\n{error}\n")
             error_handling_method = __handle_openai_error(error)
```

### Comparing `jaims-py-1.0.8/jaims_py.egg-info/PKG-INFO` & `jaims-py-1.1.0b1/jaims_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jaims-py
-Version: 1.0.8
+Version: 1.1.0b1
 Summary: A Python package for creating simple AI Agents using the OpenAI API.
 Home-page: https://github.com/dev-mush/jaims-py
 Author: Marco Musella
 License: MIT
 Keywords: OpenAI GPT-3 and GPT-4 function enabled agent
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img width="300" src="https://github.com/dev-mush/jaims-py/assets/669003/5c53381f-25b5-4141-bcd2-7457863eafb9" >
 </p>
 
 
@@ -138,7 +139,9 @@
 - [ ] Add more chat history optimization strategies
 - [ ] Add function calling callbacks 
 - [ ] Add history persistance
 
 ## 📝 License
 
 The license will be MIT, but I need to add this properly.
+
+
```

### Comparing `jaims-py-1.0.8/setup.py` & `jaims-py-1.1.0b1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read requirements.txt
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="jaims-py",
-    version="1.0.8",
+    version="1.1.0-beta.1",
     packages=find_packages(),
     description="A Python package for creating simple AI Agents using the OpenAI API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Marco Musella",
     url="https://github.com/dev-mush/jaims-py",
     license="MIT",
```

