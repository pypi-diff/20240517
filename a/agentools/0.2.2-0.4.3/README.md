# Comparing `tmp/agentools-0.2.2.tar.gz` & `tmp/agentools-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentools-0.2.2.tar", max compression
+gzip compressed data, was "agentools-0.4.3.tar", max compression
```

## Comparing `agentools-0.2.2.tar` & `agentools-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,27 @@
--rw-r--r--   0        0        0    15316 2024-01-31 03:57:58.013424 agentools-0.2.2/README.md
--rw-r--r--   0        0        0       90 2024-01-30 21:45:23.508392 agentools-0.2.2/agentools/__init__.py
--rw-r--r--   0        0        0      172 2024-02-20 17:28:05.915391 agentools-0.2.2/agentools/api/__init__.py
--rw-r--r--   0        0        0     4224 2024-02-20 22:27:10.749363 agentools-0.2.2/agentools/api/mocking.py
--rw-r--r--   0        0        0     7500 2024-03-01 10:48:37.911940 agentools-0.2.2/agentools/api/openai.py
--rw-r--r--   0        0        0       95 2024-01-30 23:11:24.048128 agentools-0.2.2/agentools/assistants/__init__.py
--rw-r--r--   0        0        0     9662 2024-01-31 03:16:20.080068 agentools-0.2.2/agentools/assistants/chatgpt.py
--rw-r--r--   0        0        0     3809 2024-01-30 21:43:47.651229 agentools-0.2.2/agentools/assistants/core.py
--rw-r--r--   0        0        0     3349 2024-01-31 00:42:23.033098 agentools-0.2.2/agentools/assistants/structgpt.py
--rw-r--r--   0        0        0      479 2024-01-31 00:46:51.984904 agentools-0.2.2/agentools/assistants/utils.py
--rw-r--r--   0        0        0       53 2024-01-30 23:26:30.062762 agentools-0.2.2/agentools/messages/__init__.py
--rw-r--r--   0        0        0     3647 2024-01-30 23:26:26.257492 agentools-0.2.2/agentools/messages/core.py
--rw-r--r--   0        0        0      125 2024-01-30 21:42:28.281814 agentools-0.2.2/agentools/tools/__init__.py
--rw-r--r--   0        0        0     4419 2024-01-30 21:44:18.131309 agentools-0.2.2/agentools/tools/core.py
--rw-r--r--   0        0        0     4061 2024-01-30 21:27:19.199229 agentools-0.2.2/agentools/tools/decorators.py
--rw-r--r--   0        0        0     4827 2024-01-30 21:20:33.206798 agentools-0.2.2/agentools/tools/utils.py
--rw-r--r--   0        0        0      144 2024-01-30 21:37:42.863031 agentools-0.2.2/agentools/utils/tokens.py
--rw-r--r--   0        0        0     2339 2024-01-30 21:38:26.556744 agentools-0.2.2/agentools/utils/trackers.py
--rw-r--r--   0        0        0      467 2024-03-01 10:54:40.553305 agentools-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    16013 1970-01-01 00:00:00.000000 agentools-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    20214 2024-05-17 15:19:29.218333 agentools-0.4.3/README.md
+-rw-r--r--   0        0        0     1867 2024-05-03 06:37:11.682106 agentools-0.4.3/agentools/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-03 06:23:27.168756 agentools-0.4.3/agentools/api/__init__.py
+-rw-r--r--   0        0        0     4224 2024-03-31 00:37:28.264533 agentools-0.4.3/agentools/api/mocking.py
+-rw-r--r--   0        0        0     7658 2024-05-03 06:22:53.797079 agentools-0.4.3/agentools/api/openai.py
+-rw-r--r--   0        0        0      151 2024-04-02 02:06:29.901315 agentools-0.4.3/agentools/assistants/__init__.py
+-rw-r--r--   0        0        0    11730 2024-05-03 05:54:10.067310 agentools-0.4.3/agentools/assistants/chatgpt.py
+-rw-r--r--   0        0        0     4328 2024-04-02 02:02:02.825310 agentools-0.4.3/agentools/assistants/core.py
+-rw-r--r--   0        0        0     3595 2024-04-27 13:12:23.439238 agentools-0.4.3/agentools/assistants/structgpt.py
+-rw-r--r--   0        0        0      479 2024-03-31 00:37:46.713979 agentools-0.4.3/agentools/assistants/utils.py
+-rw-r--r--   0        0        0      107 2024-05-03 06:24:56.023734 agentools-0.4.3/agentools/messages/__init__.py
+-rw-r--r--   0        0        0     3631 2024-03-31 00:37:53.927940 agentools-0.4.3/agentools/messages/core.py
+-rw-r--r--   0        0        0      309 2024-05-03 06:29:28.435564 agentools-0.4.3/agentools/retrieval/__init__.py
+-rw-r--r--   0        0        0      327 2024-05-01 18:11:26.493421 agentools-0.4.3/agentools/retrieval/db/__init__.py
+-rw-r--r--   0        0        0     5659 2024-04-27 00:41:29.844323 agentools-0.4.3/agentools/retrieval/db/collection.py
+-rw-r--r--   0        0        0     3163 2024-04-27 00:41:29.846068 agentools-0.4.3/agentools/retrieval/db/data.py
+-rw-r--r--   0        0        0     1188 2024-04-27 00:41:29.850286 agentools-0.4.3/agentools/retrieval/db/embedding.py
+-rw-r--r--   0        0        0      496 2024-04-02 04:27:33.809212 agentools-0.4.3/agentools/tools/__init__.py
+-rw-r--r--   0        0        0     6001 2024-04-02 06:57:54.540986 agentools-0.4.3/agentools/tools/core.py
+-rw-r--r--   0        0        0     1354 2024-03-31 01:24:18.875057 agentools-0.4.3/agentools/tools/decorators/fail_with_message.py
+-rw-r--r--   0        0        0     5194 2024-04-02 04:07:23.757891 agentools-0.4.3/agentools/tools/decorators/function_tool.py
+-rw-r--r--   0        0        0     3770 2024-04-02 07:01:15.990059 agentools-0.4.3/agentools/tools/decorators/streaming_function_tool.py
+-rw-r--r--   0        0        0     4903 2024-03-31 01:11:04.598758 agentools-0.4.3/agentools/tools/decorators/utils.py
+-rw-r--r--   0        0        0      144 2024-03-31 00:38:13.569875 agentools-0.4.3/agentools/utils/tokens.py
+-rw-r--r--   0        0        0     2339 2024-03-31 00:38:15.875070 agentools-0.4.3/agentools/utils/trackers.py
+-rw-r--r--   0        0        0      554 2024-05-17 15:20:55.636851 agentools-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    20966 1970-01-01 00:00:00.000000 agentools-0.4.3/PKG-INFO
```

### Comparing `agentools-0.2.2/README.md` & `agentools-0.4.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 # [AgenTools](https://github.com/JoongWonSeo/agentools) - Async Generator Tools for LLMs
 
 A simple set of modules, wrappers and utils that are essential for LLM-based assistants and agents using the OpenAI API and function tools. It is useful for:
+
 - **OpenAI API:** Simple wrapper for the OpenAI API to provide mocked endpoints for easy testing without costing money, accumulating the delta chunks from streamed responses into partial responses, and easier token counting/tracking.
 - **Function Tools:** Easily convert any (async) python function into a function tool that the LLM model can call, with automatic validation and retrying with error messages.
 - **Structured Data:** Easily define a Pydantic model that can be generated by the LLM model, also with validation and retries.
 - **Assistants:** Event-based architecture with async generators that yield events that you can iterate through and handle only the events you care about, such as whether you want to stream the response or not, cancel the generation prematurely, or wait for user input (human-in-the-loop) before continuing, etc.
 - **Copilots:** Integrate right into an editor with stateful system messages to allow the copilot to see the latest state of the editor and function tools to interact with the editor.
 
 **Yet to come:**
+
 - **Agents:** Autoprompting, self-prompting, chain-of-thought, sketchpads, memory management, planning, and more.
 - **Multi-Agents**: Communication channels, organization structuring, and more.
 
-
 ## Quick Start
 
 ### Installation
 
 ```bash
 pip install agentools
 ```
 
+
 ### Assistant and ChatGPT
 
 A high-level interface to use ChatGPT or other LLM-based assistants! The default implementation of ChatGPT has:
+
 - a message history to remember the conversation so far (including the system prompt)
 - ability to use tools
 - efficient async streaming support
 - simple way to customize/extend/override the default behavior
 
 
+
 ```python
 from agentools import *
 
 # empty chat history and default model (gpt-3.5)
 model = ChatGPT()
 ```
 
 You can then simply call the model as if it was a function, with a prompt:
 
 
+
 ```python
 await model("Hey!")
 ```
 
 
 
 
@@ -51,45 +56,47 @@
 
 
 As you can see, the model is async and it simply returns the resonse as a string.
 
 Both your prompt and the response are stored in the history, so you can keep calling the model with new prompts and it will remember the conversation so far.
 
 
+
 ```python
 await model("Can you repeat my last message please?")
 ```
 
 
 
 
 
-> <code>'Of course! Your last message was: "Hey!"'</code><br/>
+> <code>'Of course! Your last message was "Hey!"'</code><br/>
 
 
 
 ```python
 model.messages.history
 ```
 
 
 
 
 
 > <code>[{'role': 'user', 'content': 'Hey!'},</code><br/>
 > <code> {'content': 'Hello! How can I assist you today?', 'role': 'assistant'},</code><br/>
 > <code> {'role': 'user', 'content': 'Can you repeat my last message please?'},</code><br/>
-> <code> {'content': 'Of course! Your last message was: "Hey!"', 'role': 'assistant'}]</code><br/>
+> <code> {'content': 'Of course! Your last message was "Hey!"', 'role': 'assistant'}]</code><br/>
 
 
 ### System prompt and more on `MessageHistory`
 
 Notice that our model has no system prompt in the beginning. `ChatGPT`'s constructor by default creates an empty chat history, but you can explicitly create a `MessageHistory` object and pass it to the constructor:
 
 
+
 ```python
 translate = ChatGPT(
     messages=SimpleHistory.system("Translate the user message to English")
 )
 # SimpleHistory.system(s) is just shorthand for SimpleHistory([msg(system=s)])
 
 print(await translate("Ich liebe Katzen!"))
@@ -114,14 +121,15 @@
 > <code> {'role': 'user', 'content': '고양이랑 강아지 둘다 좋아!'},</code><br/>
 > <code> {'content': 'I like both cats and dogs!', 'role': 'assistant'}]</code><br/>
 
 
 Notice that here, we're wasting tokens by remembering the chat history, since it's not really a conversation. There's a simple `GPT` class, which simply resets the message history after each prompt:
 
 
+
 ```python
 translate = GPT(messages=SimpleHistory.system("Translate the user message to English"))
 
 await translate("Ich liebe Katzen!")
 await translate("고양이랑 강아지 둘다 좋아!")
 
 translate.messages.history
@@ -135,14 +143,15 @@
 
 
 ### OpenAI API: changing the model and mocked API
 
 You can set the default model in the constructor, or override it for each prompt:
 
 
+
 ```python
 # default model is now gpt-4 💸
 model = ChatGPT(model="gpt-4")
 
 # but you can override it for each prompt anyways
 await model("Heyo!", model="mocked")
 ```
@@ -153,63 +162,70 @@
 
 > <code>'Hello, world!'</code><br/>
 
 
 As you see, our wrapper provides a simple mocked "model", which will simply return `"Hello, world!"` for any prompt, with some simulated latency. This will also work with streaming responses, and in either cases, you won't be able to tell the difference between the real API and the mocked one.
 
 There are more mocked models for your convinience:
+
 - `mocked`: always returns `"Hello, world!"`
 - `mocked:TEST123`: returns the string after the colon, e.g. `"TEST123"`
 - `echo`: returns the user prompt itself
 
 Let's print all events to the console to take a peek at the event-based generator:
 
 
+
 ```python
 await model("Heya!", model="echo", event_logger=print)
 ```
 
 
 > <code>[ResponseStartEvent]: prompt=Heya!, tools=None, model=echo, max_function_calls=100, openai_kwargs={}</code><br/>
 > <code>[CompletionStartEvent]: call_index=0</code><br/>
-> <code>[CompletionEvent]: completion=ChatCompletion(id='mock', choices=[Choice(finish_reason='stop', index=0, logprobs=None, message=ChatCompletionMessage(content='Heya!', role='assistant', function_call=None, tool_calls=None))], created=1706671307, model='mock', object='chat.completion', system_fingerprint=None, usage=None), call_index=0</code><br/>
+> <code>[CompletionEvent]: completion=ChatCompletion(id='mock', choices=[Choice(finish_reason='stop', index=0, logprobs=None, message=ChatCompletionMessage(content='Heya!', role='assistant', function_call=None, tool_calls=None))], created=1715958919, model='mock', object='chat.completion', system_fingerprint=None, usage=None), call_index=0</code><br/>
 > <code>[FullMessageEvent]: message=ChatCompletionMessage(content='Heya!', role='assistant', function_call=None, tool_calls=None), choice_index=0</code><br/>
 > <code>[TextMessageEvent]: content=Heya!</code><br/>
 > <code>[ResponseEndEvent]: content=Heya!</code><br/>
 
 
 
 
 > <code>'Heya!'</code><br/>
 
 
 Wow, quite a lot going on for a simple prompt! While it might seem like too many events, this offers a lot of flexibility and customizability.
 
 You can easily handle only the events you are interested in, useful when e.g:
+
 - updating the frontend when streaming the responses,
 - cancelling the generation early,
 - or implementing human-in-the-loop for function calls.
 
 For instance, the `GPT` class from above is as simple as:
+
 ```python
 async for event in self.response_events(prompt, **openai_kwargs):
     match event:
         case self.ResponseEndEvent():
             await self.messages.reset()
             return event.content
 ```
 
 This generator-based architecture is a good balance between flexibility and simplicity!
 
 While we won't go deeper into the low-level API in this quickstart, you can look at the `advanced.ipynb` notebook for more details.
 
+
 ### Tools: `@function_tool`
+
 You can turn any function into a tool usable by the model by decorating it with `@function_tool`:
 
 
+
 ```python
 @function_tool
 def print_to_console(text: str) -> str:
     """
     Print text to console
 
     Args:
@@ -231,42 +247,46 @@
 
 > <code>'success'</code><br/>
 
 
 You can use the tool from python as you normally would, and the model will also be able to use it simply by passing it to the `tools` parameter during init (as default) or prompting it (as a one-off).
 
 
+
 ```python
 model = ChatGPT(tools=print_to_console)
 await model("Say 'hello from GPT' to console!")
 ```
 
 
-> <code>Hello from GPT!</code><br/>
+> <code>hello from GPT</code><br/>
 
 
 
 
-> <code>'I have successfully printed "Hello from GPT!" to the console.'</code><br/>
+> <code>"I have printed 'hello from GPT' to the console."</code><br/>
 
 
 To make the function a `@function_tool`, you must do the following:
+
 - The parameters must be type annotated, and all parameters must be JSON-serializable (e.g. `str`, `int`, `float`, `bool`, `list`, `dict`, `None`, etc).
 - The return type should be a `str` or something that can be converted to a `str`.
 - It must be documented with a `'''docstring'''`, including each parameter (most [formats supported](https://github.com/rr-/docstring_parser), e.g. [Google-style](https://gist.github.com/redlotus/3bc387c2591e3e908c9b63b97b11d24e#file-docstrings-py-L67), [NumPy-style](https://gist.github.com/eikonomega/910512d92769b0cc382a09ae4de41771), sphinx-style, etc, see [this overview](https://gist.github.com/nipunsadvilkar/fec9d2a40f9c83ea7fd97be59261c400))
 
 
 Showing off some more goodies:
+
 - Even async functions should seamlessly work, just don't forget to `await` them.
 - `@fail_with_message(err)` is a decorator that will catch any exceptions thrown by the function and instead return the error message. This is useful for when you want to handle errors in a more graceful way than just crashing the model. It also takes an optional logger, which by default takes the `print` function, but any callable that takes a string will work, such as `logger.error` from the `logging` module.
 - Usually, the `@function_tool` decorator will throw an assertion error if you forget to provide the description for any of the function or their parameters. If you really don't want to provide descriptions for some (or all), maybe because it's so self-explanatory or you need to save tokens, then you can explicitly turn off the docstring parsing by passing `@function_tool(check_description=False)`. This is not recommended, but it's there if you need it.
 
 Note that by returning descriptive error strings, the model can read the error message and retry, increasing the robustness!
 
 
+
 ```python
 import asyncio
 import logging
 
 
 @function_tool(name="Fibonacci", require_doc=False)
 @fail_with_message("Error", logger=logging.error)
@@ -289,18 +309,20 @@
 
 
 
 > <code>'Error: n must be >= 0'</code><br/>
 
 
 ### Toolkits: `class Toolkit`
+
 Toolkits are a collection of related function tools, esp. useful when they share a state. Also good for keeping the state bound to a single instance of the toolkit, rather than a global state.
 To create a toolkit, simply subclass `Toolkit` and decorate its methods with `@function_tool`.
 
 
+
 ```python
 class Notepad(Toolkit):
     def __init__(self):
         super().__init__()
         self.content = "<Fill me in>"
 
     @function_tool
@@ -329,71 +351,165 @@
 
 > <code>"Shhh... here's a secret: 42"</code><br/>
 
 
 As before, simply pass the toolkit to the model. To use multiple tools and toolkits, simply use the `ToolList` class:
 
 
+
 ```python
-gpt = ChatGPT(
+model = ChatGPT(
     tools=ToolList(notes, print_to_console, fib),
 )
 
-await gpt("What's on my notepad?")
+await model("What's on my notepad?")
 ```
 
 
 
 
 
-> <code>'On your notepad, there is a secret written: 42.'</code><br/>
+> <code>'The secret on your notepad is: 42'</code><br/>
 
 
 
 ```python
-await gpt(
+await model(
     "Can you calculate the 8th fibonacci number, add it to the number in my notes, and write it? also print it to console as well.",
     event_logger=lambda x: print(x) if x.startswith("[Tool") else None,
 )
 ```
 
 
-> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_Uj8VIxhCxvHUnbIH1CK50Qmo', function=Function(arguments='{\n  "n": 8\n}', name='Fibonacci'), type='function')]</code><br/>
-> <code>[ToolResultEvent]: result=21, tool_call=ChatCompletionMessageToolCall(id='call_Uj8VIxhCxvHUnbIH1CK50Qmo', function=Function(arguments='{\n  "n": 8\n}', name='Fibonacci'), type='function'), index=0</code><br/>
-> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_0F0alwZitumJTU3QlPxuoJNW', function=Function(arguments='{\n  "text": "63"\n}', name='write'), type='function')]</code><br/>
-> <code>[ToolResultEvent]: result=None, tool_call=ChatCompletionMessageToolCall(id='call_0F0alwZitumJTU3QlPxuoJNW', function=Function(arguments='{\n  "text": "63"\n}', name='write'), type='function'), index=0</code><br/>
-> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_KoSyY1LZQYVfEpMDPUZlt2pc', function=Function(arguments='{\n  "text": "63"\n}', name='print_to_console'), type='function')]</code><br/>
-> <code>63</code><br/>
-> <code>[ToolResultEvent]: result=success, tool_call=ChatCompletionMessageToolCall(id='call_KoSyY1LZQYVfEpMDPUZlt2pc', function=Function(arguments='{\n  "text": "63"\n}', name='print_to_console'), type='function'), index=0</code><br/>
+> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_gDhzb8aiNmaJkUB6Z8tHZ7EU', function=Function(arguments='{"n": 8}', name='Fibonacci'), type='function'), ChatCompletionMessageToolCall(id='call_c9TjP8fWKTBrzie2TrzzOZeQ', function=Function(arguments='{}', name='read'), type='function')]</code><br/>
+> <code>[ToolResultEvent]: result=Shhh... here's a secret: 42, tool_call=ChatCompletionMessageToolCall(id='call_c9TjP8fWKTBrzie2TrzzOZeQ', function=Function(arguments='{}', name='read'), type='function'), index=1</code><br/>
+> <code>[ToolResultEvent]: result=21, tool_call=ChatCompletionMessageToolCall(id='call_gDhzb8aiNmaJkUB6Z8tHZ7EU', function=Function(arguments='{"n": 8}', name='Fibonacci'), type='function'), index=0</code><br/>
+> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_EU9GTOVIQHeF2LeXxlVcjYlk', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='write'), type='function')]</code><br/>
+> <code>[ToolResultEvent]: result=None, tool_call=ChatCompletionMessageToolCall(id='call_EU9GTOVIQHeF2LeXxlVcjYlk', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='write'), type='function'), index=0</code><br/>
+> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_uIp1BSsPlmYc6dl0xgYX4s2h', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='print_to_console'), type='function')]</code><br/>
+> <code>The sum of the 8th Fibonacci number and the secret on your notepad: 63</code><br/>
+> <code>[ToolResultEvent]: result=success, tool_call=ChatCompletionMessageToolCall(id='call_uIp1BSsPlmYc6dl0xgYX4s2h', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='print_to_console'), type='function'), index=0</code><br/>
 
 
 
 
-> <code>'I have calculated the 8th Fibonacci number to be 21. I have added it to the number on your notepad, which is 42, and the result is 63.\n\nI have written the result, 63, on your notepad. However, it seems that there was an issue with writing it. My apologies for the inconvenience.\n\nI have also printed the result, 63, to the console.'</code><br/>
+> <code>'I have written the sum of the 8th Fibonacci number (21) and the secret on your notepad (42), which totals to 63. It has also been printed to the console.'</code><br/>
 
 
 
 ```python
 notes.read()
 ```
 
 
 
 
 
-> <code>'63'</code><br/>
+> <code>'The sum of the 8th Fibonacci number and the secret on your notepad: 63'</code><br/>
 
 
 Notice how since our `write` function doesn't return anything, it defaults to `None` and our model gets confused! So don't forget to return an encouraging success message to make our model happy :)
 
+
+### Tool Previews
+
+When using streaming, and you're using function tools with a long input, you might want to preview the tool's output before it's fully processed. With the help of the `json_autocomplete` package, the JSON argument generated by the model can be parsed before it's fully complete, and the preview can be shown to the user.
+
+
+
+```python
+@function_tool(require_doc=False)
+async def create_slogan(title: str, content: str):
+    print(f"\n\n[Final Slogan] {title}: {content}")
+    return "Slogan created and shown to user! Simply tell the user that it was created."
+
+
+@create_slogan.preview
+async def preview(title: str = "", content: str = ""):
+    assert isinstance(title, str) and isinstance(content, str)
+    print(f"[Preview] {title}: {content}", flush=True)
+```
+
+
+```python
+model = ChatGPT(tools=create_slogan)
+await model(
+    "Create a 1-sentence slogan about how ducks can help with debugging.", stream=True
+)
+```
+
+
+> <code>[Preview] : </code><br/>
+> <code>[Preview] D: </code><br/>
+> <code>[Preview] Ducks: </code><br/>
+> <code>[Preview] Ducks and: </code><br/>
+> <code>[Preview] Ducks and Debug: </code><br/>
+> <code>[Preview] Ducks and Debugging: </code><br/>
+> <code>[Preview] Ducks and Debugging: </code><br/>
+> <code>[Preview] Ducks and Debugging: Qu</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feather</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends.</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends.</code><br/>
+> <code>[Final Slogan] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends.</code><br/>
+
+
+
+
+> <code>'I have created a slogan about how ducks can help with debugging.'</code><br/>
+
+
+If you need a more coherent logic shared between the `@preview` and the final `@function_tool`, e.g. do something at the start of the function call, share some data between previews, etc... It gets messy very fast!
+
+Instead, you can use the `@streaming_function_tool()` decorator, which receives a single `arg_stream` parameter, which is an async generator that yields the partial arguments, as streamed from the model. Therefore, you simply need to iterate through it, and perform the actual function call at the end of the iteration. The following is the equivalent of the previous example:
+
+> _Note that currently, you must pass the parameter as a `json_schema`. Soon, this could be parsed from the docstring as usual._
+
+
+
+```python
+from pydantic import BaseModel
+
+
+class Slogan(BaseModel):
+    title: str
+    content: str
+
+
+@streaming_function_tool(json_schema=Slogan.model_json_schema())
+async def create_slogan(arg_stream):
+    print("Starting slogan creation...")
+
+    async for args in arg_stream:
+        title, content = args.get("title", ""), args.get("content", "")
+        print(f'{args} -> "{title}", "{content}"')
+
+    print(f"\n\n[Final Slogan] {title}: {content}")
+    return "Slogan created and shown to user! Simply tell the user that it was created."
+```
+
 ### Structured Data
 
 We can very easily define a Pydantic model that can be generated by the LLM model, with validation and retries:
 
 
+
 ```python
 from pydantic import BaseModel, Field
 
 
 class Song(BaseModel):
     title: str
     genres: list[str] = Field(description="AT LEAST 3 genres!")
@@ -410,27 +526,30 @@
 
 > <code>Song(title='Hello', genres=['pop'], duration=3.5)</code><br/>
 
 
 Create a `StructGPT` object with your pydantic model, and prompting it will always return a valid instance of the model, or raise an exception if it fails to generate a valid instance after the maximum number of retries. Your docstring and field descriptions will also be visible to the model, so make sure to write good descriptions!
 
 
+
 ```python
 generate_song = StructGPT(Song)
 
 await generate_song("Come up with an all-time best K-hiphop song")
 ```
 
 
 
 
 
-> <code>Song(title='Respect My Name', genres=['Hip-Hop', 'K-Rap', 'Trap'], duration=240.0)</code><br/>
+> <code>Song(title='Eung Freestyle', genres=['K-HipHop', 'Rap', 'Hip-Hop'], duration=192.0)</code><br/>
 
 
 ## Misc.
 
 Streaming can be enabled as usual by passing `stream=True` when prompting, and handle the partial events as they come in. Check the `Assistant` class for a list of events including the ones for streaming.
 
 There are some other useful utilities in the `utils` module, such as:
+
 - `tokens`: for token counting
 - `trackers`: for transparent token tracking and prompt/response logging
+
```

### Comparing `agentools-0.2.2/agentools/api/mocking.py` & `agentools-0.4.3/agentools/api/mocking.py`

 * *Files identical despite different names*

### Comparing `agentools-0.2.2/agentools/api/openai.py` & `agentools-0.4.3/agentools/api/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """
 Interactions with the OpenAI API and wrappers around the API.
 """
 
 from typing import AsyncIterator
 
-from openai import OpenAI, AsyncOpenAI, AsyncStream
-from openai.types import CompletionUsage
-from openai.resources.chat.completions import NOT_GIVEN
-from openai.types.chat.chat_completion import (
-    ChatCompletion,  # Overall Completion, has id, stats, choices
-    ChatCompletionMessage,  # completion.choice[0].message, has role, content, tool_calls
-)
+from openai import AsyncOpenAI, AsyncStream
+from groq import AsyncGroq
 import openai.types.chat.chat_completion as Normal
+from openai.types.chat.chat_completion import (
+    ChatCompletion as ChatCompletion,
+    ChatCompletionMessage as ChatCompletionMessage,
+)  # re-export to __init__.py
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_message_tool_call import (
     ChatCompletionMessageToolCall as ToolCall,
     Function,
 )
 
 
 from .mocking import mock_response, mock_streaming_response, GLOBAL_RECORDINGS
 
 
-async def openai_chat(client: AsyncOpenAI | None = None, **openai_kwargs):
+async def openai_chat(client: AsyncOpenAI | AsyncGroq | None = None, **openai_kwargs):
     """
     Thin wrapper around openai with mocking and potential for other features/backend
     - Use model='mock' to simply return "Hello, world"
     - Use model="mock:<message>" to return the message
     - Use model='echo' to echo the last message
 
     Args:
@@ -57,20 +56,26 @@
 
     elif openai_kwargs["model"].startswith("replay"):
         r = openai_kwargs["model"].split(":", 1)[1]
         replay_model = GLOBAL_RECORDINGS.recordings[int(r)]
         gen = await replay_model.replay()
 
     else:
-        client = client or AsyncOpenAI()
+        if openai_kwargs["model"].startswith("llama"):
+            client = client or AsyncGroq()
+        else:
+            client = client or AsyncOpenAI()
         gen = await client.chat.completions.create(**openai_kwargs)
 
     # Record the response if recording
     if GLOBAL_RECORDINGS.current_recorder:
-        return await GLOBAL_RECORDINGS.current_recorder.record(gen)
+        if openai_kwargs.get("stream"):
+            return await GLOBAL_RECORDINGS.current_recorder.record(gen)
+        else:
+            raise ValueError("Recording non-streaming responses is not supported yet.")
     else:
         return gen
 
 
 async def accumulate_partial(
     stream: AsyncStream[ChatCompletionChunk],
 ) -> AsyncIterator[tuple[ChatCompletionChunk, Normal.ChatCompletion]]:
```

### Comparing `agentools-0.2.2/agentools/assistants/chatgpt.py` & `agentools-0.4.3/agentools/assistants/chatgpt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
+import json
 from typing import Callable, Optional, AsyncIterator
-from collections.abc import Iterator
+
+from json_autocomplete import json_autocomplete
 
 from ..api.openai import (
     openai_chat,
     accumulate_partial,
-    NOT_GIVEN,
     ChatCompletion,
     ToolCall,
 )
-from ..tools import Tools, call_requested_function
+from ..tools import Tools, call_requested_function, call_function_preview
 from ..messages import MessageHistory, SimpleHistory, msg
 from .utils import atuple, format_event
 from .core import Assistant
 
 
 class ChatGPT(Assistant):
     """ChatGPT with default model and toolkit"""
@@ -70,15 +71,15 @@
         self,
         prompt: str,
         tools: Optional[Tools] = None,
         model: Optional[str] = None,
         max_function_calls: int = MAX_FUNCTION_CALLS,
         parallel_calls=True,
         **openai_kwargs,
-    ) -> Iterator[Assistant.Event]:
+    ) -> AsyncIterator[Assistant.Event]:
         """
         Generate events from a single user prompt, yielding each message and tool call and everything else as it is received.
         This is the overall generalized form, and you would likely only override the smaller *_events() generators to customize each aspect instead.
         """
         model = model or self.default_model
         tools = tools or self.default_tools
 
@@ -94,15 +95,15 @@
             # call the underlying API and handle the events
             completion_events = self.completion_events(
                 call_index,
                 tools,
                 parallel_calls,
                 openai_args=dict(
                     messages=self.messages.history,
-                    tools=tools.schema if tools else NOT_GIVEN,
+                    tools=tools.schema if tools else None,
                     model=model,
                     **openai_kwargs,
                 ),
             )
             completion: ChatCompletion = None
             async for partial_event in completion_events:
                 yield partial_event
@@ -191,37 +192,84 @@
         self, tool_calls: list[ToolCall], tools: Tools, parallel_calls: bool
     ) -> AsyncIterator[Assistant.Event]:
         """
         Generate events from a list of tool calls, yielding each tool call, executing them, and yielding the result. You should override this to customize the tool call handling, also defining your own events to yield.
         """
         yield self.ToolCallsEvent(tool_calls)
 
+        lookup = tools.lookup
+
         # awaitables for each tool call
-        calls = [
-            atuple(i, call, call_requested_function(call.function, tools.lookup))
-            for i, call in enumerate(tool_calls)
-        ]
+        calls = []
+        for i, call in enumerate(tool_calls):
+            call_id = call.id
+            name = call.function.name
+            args = call.function.arguments
+            task = atuple(i, call, call_requested_function(name, args, lookup, call_id))
+            calls.append(task)
+
         # handle each call results as they come in (or in order)
         calls = asyncio.as_completed(calls) if parallel_calls else calls
         for completed in calls:
             i, call, result = await completed
-            # stringify the result
-            result = str(result)
+            result = str(result)  # stringify the result
             await self.messages.append(msg(tool=result, tool_call_id=call.id))
             yield self.ToolResultEvent(result, call, i)
 
     async def partial_tool_events(
         self, tool_calls: list[ToolCall], tools: Tools, parallel_calls: bool
     ) -> AsyncIterator[Assistant.Event]:
         """
-        Generate events from a list of tool calls, yielding each tool call, executing them, and yielding the result. You should override this to customize the tool call handling, also defining your own events to yield.
+        Generate events from a list of tool preview calls, yielding each partial tool call, executing them, and yielding the result of the preview function. You should override this to customize the tool preview call handling, also defining your own events to yield.
         """
         yield self.PartialToolCallsEvent(tool_calls)
 
-        # TODO: call function preview functions
+        lookup_preview = tools.lookup_preview
+
+        if not lookup_preview:
+            return
+
+        # create preview function tasks
+        calls = []
+        for i, call in enumerate(tool_calls):
+            # TODO: in theory, since this is streaming, we can do the following optimizations for all i < last_i, since they are already completed:
+            # - we can skip the preview call
+            # - we could in theory already start the final call task, and gather in the final call later
+            # easier if chunk/delta is also passed, since ca__id is always included in each chunk, i.e. use that to detect which call was changed.
+            # to help coordinate between partial and final, we can have a dict of call_id to task, so that partial may already kickstart the final task
+            call_id = call.id
+            func = call.function.name
+            partial = call.function.arguments
+
+            if func not in lookup_preview or not partial.strip():
+                continue
+            try:
+                autocompleted = json_autocomplete(call.function.arguments)
+                args = json.loads(autocompleted)
+            except Exception:
+                continue
+
+            yield self.PartialFunctionToolCallEvent(
+                function_name=func,
+                partial=partial,
+                autocompleted=autocompleted,
+                arguments=args,
+                index=i,
+            )
+
+            task = atuple(
+                i, call, call_function_preview(func, args, lookup_preview, call_id)
+            )
+            calls.append(task)
+
+        # handle each call results as they come in (or in order)
+        calls = asyncio.as_completed(calls) if parallel_calls else calls
+        for completed in calls:
+            i, call, result = await completed
+            yield self.PartialToolResultEvent(result, call, i)
 
 
 class GPT(ChatGPT):
     """
     GPT with no memory, i.e. the chat history resets after each prompt
     """
```

### Comparing `agentools-0.2.2/agentools/assistants/core.py` & `agentools-0.4.3/agentools/assistants/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from typing import Any, Optional
 from abc import ABC
 from dataclasses import dataclass
 
 from ..api import (
     ChatCompletion,
     ChatCompletionMessage,
     ToolCall,
@@ -17,15 +17,15 @@
     Uses an event-based system and offers high-level overridable methods for flexible customization.
     You can essentially iterate over the events and only handle the ones you care about.
     You can also override the *_events() generators to emit your own events.
     For passing events to a frontend, you could create an "adapter" generator that converts the events to whichever format the frontend expects, and simply use that generator for Server-Sent Events or StreamedResponses.
     """
 
     class Event(ABC):
-        """Event base class for Assistant events"""
+        """Event base class for Assistant events that occur during a prompt response."""
 
         pass
 
     # ================ Full Response Events =================#
     @dataclass
     class ResponseStartEvent(Event):
         """Assistant was prompted with the following args"""
@@ -106,14 +106,32 @@
 
     @dataclass
     class PartialToolCallsEvent(Event):
         """Partial tool call was updated"""
 
         tool_calls: list[ToolCall]
 
+    @dataclass
+    class PartialFunctionToolCallEvent(Event):
+        """One tool call, with autocompleted arguments"""
+
+        function_name: str
+        partial: str
+        autocompleted: str
+        arguments: dict
+        index: int = 0
+
+    @dataclass
+    class PartialToolResultEvent(Event):
+        """Result of a partial tool (preview) call"""
+
+        result: Any
+        tool_call: ToolCall
+        index: int = 0  # index of this tool call in the tool_calls list
+
     # ================ Error Events =================#
     @dataclass
     class MaxCallsExceededEvent(Event):
         """Maximum number of function calls exceeded"""
 
         num_calls: int
```

### Comparing `agentools-0.2.2/agentools/assistants/structgpt.py` & `agentools-0.4.3/agentools/assistants/structgpt.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,23 @@
     class StructFailedEvent(Assistant.Event):
         result: str
 
     def __init__(
         self, struct: BaseModel, model: str = "gpt-3.5-turbo", tool_name: str = None
     ):
         @function_tool(
-            name=tool_name, require_doc=False, json_schema=struct.model_json_schema()
+            name=tool_name,
+            require_doc=False,
+            json_schema=struct.model_json_schema(),
         )
         async def create(**kwargs):
             return struct(**kwargs)
 
+        # TODO: define preview function for struct
+
         super().__init__(SimpleHistory(), tools=create, model=model)
 
         self.struct = struct
 
     async def __call__(
         self,
         prompt: str,
@@ -73,19 +77,25 @@
         self, tool_calls: list[ToolCall], tools: Tools, parallel_calls: bool
     ) -> AsyncIterator[Assistant.Event]:
         """
         Generate events from a list of tool calls, yielding each tool call, executing them, and yielding the result. You should override this to customize the tool call handling, also defining your own events to yield.
         """
         yield self.ToolCallsEvent(tool_calls)
 
+        lookup = tools.lookup
+
         # awaitables for each tool call
-        calls = [
-            atuple(i, call, call_requested_function(call.function, tools.lookup))
-            for i, call in enumerate(tool_calls)
-        ]
+        calls = []
+        for i, call in enumerate(tool_calls):
+            call_id = call.id
+            name = call.function.name
+            args = call.function.arguments
+            task = atuple(i, call, call_requested_function(name, args, lookup, call_id))
+            calls.append(task)
+
         # handle each call results as they come in (or in order)
         calls = asyncio.as_completed(calls) if parallel_calls else calls
         for completed in calls:
             i, call, result = await completed
 
             # if the result successfully executed, yield it
             if type(result) is self.struct:
```

### Comparing `agentools-0.2.2/agentools/messages/core.py` & `agentools-0.4.3/agentools/messages/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,27 @@
 from abc import ABC, abstractmethod
 from copy import deepcopy
 
 from openai.types.chat import ChatCompletionMessage
 
 
 @overload
-def msg(*, system: str) -> dict[str, str]:
-    ...
+def msg(*, system: str) -> dict[str, str]: ...
 
 
 @overload
-def msg(*, user: str) -> dict[str, str]:
-    ...
+def msg(*, user: str) -> dict[str, str]: ...
 
 
 @overload
-def msg(*, assistant: str) -> dict[str, str]:
-    ...
+def msg(*, assistant: str) -> dict[str, str]: ...
 
 
 @overload
-def msg(*, tool: str, tool_call_id: str) -> dict[str, str]:
-    ...
+def msg(*, tool: str, tool_call_id: str) -> dict[str, str]: ...
 
 
 def msg(*, system=None, user=None, assistant=None, tool=None, tool_call_id=None):
     """
     Define a system/user/assistant/tool message by keyword arguments.
     """
     assert (
```

### Comparing `agentools-0.2.2/agentools/tools/core.py` & `agentools-0.4.3/agentools/tools/core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from abc import ABC
 import asyncio
 from typing import Callable
 from functools import wraps
 from itertools import chain
 import json
 
-from ..api.openai import Function
+
+class CallableTool(ABC):
+    """A (fake) interface for any tool that can be invoked by the assistant."""
+
+    in_thread: bool  # whether to run the function in a separate thread
+    include_call_id: bool  # whether to include the call_id in the function arguments
+
+    def __call__(args: dict) -> str: ...
 
 
 class Tools(ABC):
     """A (fake) interface for any tool (function/ToolList/Toolkit) that can be used by the assistant."""
 
     tool_enabled: bool  # whether this tool is enabled
     schema: list[dict]  # list of OpenAI function schemas
-    lookup: dict[str, Callable]  # dict of tool name to function implementation
+    lookup: dict[str, CallableTool]  # dict of tool name to function implementation
+    lookup_preview: dict[str, CallableTool]  # dict of tool name to preview function
 
 
 class ToolList(Tools):
     """A simple collection of tools/toolkits"""
 
     def __init__(self, *tools: Tools, tool_enabled=True):
         self.tools = list(tools)
@@ -28,59 +36,75 @@
         """list of OpenAI function schemas"""
         if not self.tool_enabled:
             return []
 
         return list(chain(*[t.schema for t in self.tools if t.tool_enabled]))
 
     @property
-    def lookup(self) -> dict[str, Callable]:
+    def lookup(self) -> dict[str, CallableTool]:
         """dict of TOOL NAME to argument-validated function"""
         if not self.tool_enabled:
             return {}
 
         lookups = [t.lookup for t in self.tools if t.tool_enabled]
         assert len(set(chain(*[lookup.keys() for lookup in lookups]))) == sum(
             [len(lookup) for lookup in lookups]
         ), "Duplicate tool names detected!"
         return {k: v for lookup in lookups for k, v in lookup.items()}
 
+    @property
+    def lookup_preview(self) -> dict[str, CallableTool]:
+        """dict of TOOL NAME to argument-validated function"""
+        if not self.tool_enabled:
+            return {}
+
+        lookups = [t.lookup_preview for t in self.tools if t.tool_enabled]
+        return {k: v for lookup in lookups for k, v in lookup.items()}
+
 
 class Toolkit(Tools):
     """
     A base class for a collection of tools and their shared states.
     Simply inherit this class and mark your methods as tools with the `@function_tool` decorator.
     After instantiating your toolkit, you can either:
     - [Code]: Simply use the functions as normal, e.g. `toolkit.my_tool(**args)`
     - [Model]: Use the `toolkit.lookup` dict to call the function by name, e.g. `toolkit.lookup['my_tool'](args)`
     """
 
     def __init__(self):
         self.tool_enabled = True
-        self.registered_tools = (
-            {}
-        )  # explicitly registered, i.e. dynamically defined tools
+        self.registered_tools = {}  # explicitly registered, i.e. dynamically defined tools
 
     def register_tool(self, tool):
         """Explicitly register a tool if it's not in the class definition"""
         self.registered_tools[tool.name] = tool
 
     @property
     def schema(self) -> list[dict]:
         """list of OpenAI function schemas"""
         return list(chain(*[tool.schema for tool in self._function_tools.values()]))
 
     @property
-    def lookup(self) -> dict[str, Callable]:
+    def lookup(self) -> dict[str, CallableTool]:
         """dict of TOOL NAME to argument-validated function"""
         return {
             tool.name: self._with_self(tool.validate_and_call)
             for tool in self._function_tools.values()
         }
 
     @property
+    def lookup_preview(self) -> dict[str, CallableTool]:
+        """dict of TOOL NAME to argument-validated function"""
+        return {
+            tool.name: self._with_self(tool.lookup_preview[tool.name])
+            for tool in self._function_tools.values()
+            if tool.name in tool.lookup_preview
+        }
+
+    @property
     def _function_tools(self) -> dict[str, Callable]:
         """dict of RAW FUNCTION NAME to function"""
         return (
             self.registered_tools
             | {
                 attr: getattr(self, attr)
                 for attr in dir(type(self))
@@ -102,32 +126,57 @@
             return func({"self": self, **kwargs})
 
         return wrapper
 
 
 # ========== Model ========== #
 async def call_requested_function(
-    call_request: Function, func_lookup: dict[str, Callable]
+    func_name: str,
+    json_args: str,
+    func_lookup: dict[str, CallableTool],
+    call_id: str | None = None,
 ):
     """
     Call the requested function generated by the model.
     """
     # parse function call
-    func_name = call_request.name
-    arguments = call_request.arguments
-
     if func_name not in func_lookup:
         return f"Error: Function {func_name} does not exist."
     try:
-        args = json.loads(arguments)
+        args = json.loads(json_args)
     except Exception as e:
         return f"Error: Failed to parse arguments, make sure your arguments is a valid JSON object: {e}"
 
     # call function
+    f = func_lookup[func_name]
+
+    if f.include_call_id:
+        args = args | {"call_id": call_id}
+
+    if not f.in_thread:
+        return await f(args)
+    else:
+        return await asyncio.to_thread(f, args)
+
+
+async def call_function_preview(
+    func_name: str,
+    args: dict,
+    func_lookup_preview: dict[str, CallableTool],
+    call_id: str | None = None,
+):
+    """
+    Call the requested function preview from the *autocompleted* JSON of the partial arguments while being generated by the model.
+    """
+    # call function
     try:
-        f = func_lookup[func_name]
-        if not getattr(f, "in_thread", True):
+        f = func_lookup_preview[func_name]
+
+        if f.include_call_id:
+            args = args | {"call_id": call_id}
+
+        if not f.in_thread:
             return await f(args)
         else:
             return await asyncio.to_thread(f, args)
-    except Exception as e:
-        return f"Error: {e}"
+    except Exception:
+        pass
```

### Comparing `agentools-0.2.2/agentools/tools/decorators.py` & `agentools-0.4.3/agentools/tools/decorators/streaming_function_tool.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,119 +1,119 @@
 import asyncio
-from typing import Optional, Callable
-from functools import wraps
-from copy import deepcopy
-
-from .utils import (
-    ValidationError,
-    validator_from_doc,
-    validator_from_schema,
-    schema_to_openai_func,
-)
+from typing import Callable
 
+from .function_tool import function_tool
 
-def function_tool(
-    function=None,
+
+class AsyncStream:
+    def __init__(self):
+        self.queue = asyncio.Queue()
+        self.closed = False
+
+    async def send(self, data, is_final=False):
+        """
+        Send data through the tunnel, which the receiver can read using `async for`.
+        """
+        await self.queue.put(data)
+        if is_final:
+            self.closed = True
+
+    def __aiter__(self):
+        """
+        Returns the iterator object itself.
+        """
+        return self
+
+    async def __anext__(self):
+        """
+        Returns the next item from the queue.
+        """
+        if self.closed and self.queue.empty():
+            raise StopAsyncIteration
+        data = await self.queue.get()
+        return data
+
+
+def streaming_function_tool(
+    function: Callable = None,
     *,
-    name: Optional[str] = None,
+    name: str | None = None,
     require_doc: bool = True,
-    json_schema: Optional[dict] = None,
-    in_thread: Optional[bool] = None,
+    json_schema: dict,
+    in_thread: bool | None = None,
+    include_call_id: bool = False,
 ):
     """
-    Simple decorator that:
-    - Marks a function as a tool and enables it: `func.tool_enabled = True`
-    - Attaches a lookup dict for OpenAI: `func.lookup = {func.name: func}`
-    - Attaches a list of OpenAI tool schema: `func.schema = [{...}]`
-    - Attaches a pydantic argument validator: `func.validator`
-    - Attaches a validate and call function: `func.validate_and_call(args)`
-    - If a name is not specified, use the function name as the tool name
+
+
+    Args:
+        name: The name that the model will see. If not provided, the function name will be used.
+        require_doc: Whether to require a docstring to be present for the function.
+        json_schema: A JSON schema given to model and for validation. If not provided, the docstring will be used.
+        in_thread: Whether to run the function in a separate thread, regardless of whether it is async or not.
+        include_call_id: Whether to include the call_id in the function arguments.
     """
 
     def decorator(func):
-        def validate_and_call(args: dict) -> str:
-            try:
-                args_without_self = {k: v for k, v in args.items() if k != "self"}
-                func.validator(**args_without_self)
-            except ValidationError as e:
-                # if the underlying function is async make sure to return a coroutine
-                if asyncio.iscoroutinefunction(func):
+        func_name = name or func.__name__
 
-                    async def async_error(e):
-                        return f"Invalid Argument: {e}"
+        @function_tool(
+            name=func_name,
+            require_doc=require_doc,
+            json_schema=json_schema,
+            in_thread=in_thread,
+            include_call_id=True,
+        )
+        async def function_final(call_id, **args):
+            task, stream = func.tasks[call_id]
 
-                    return async_error(e)
-                else:
-                    return f"Invalid Argument: {e}"
-            return func(**args)
+            if include_call_id:
+                args = args | {"call_id": call_id}
 
-        func.name = name or func.__name__
-        func.tool_enabled = True
+            if "self" in args:
+                args.pop("self")
+            await stream.send(args, is_final=True)
+
+            await task  # wait for the task to finish
+            del func.tasks[call_id]
+            return task.result()
+
+        @function_final.preview
+        async def function_preview(call_id, **args):
+            if call_id not in func.tasks:
+                # function is now starting
+                stream = AsyncStream()
+                if "self" in args:
+                    self = args.pop("self")
+                    task = asyncio.create_task(func(self, stream))
+                else:
+                    task = asyncio.create_task(func(stream))
+                func.tasks[call_id] = (task, stream)
+            else:
+                task, stream = func.tasks[call_id]
+
+            if include_call_id:
+                args = args | {"call_id": call_id}
+
+            if "self" in args:  # self has already been passed
+                args.pop("self")
+            await stream.send(args)
+
+        # ========== Attach the tool attributes ========== #
+        func.name = function_final.name
+        func.tool_enabled = function_final.tool_enabled
+        func.schema = function_final.schema
+        func.validator = function_final.validator
+        func.validate_and_call = function_final.validate_and_call
+        func.lookup = {func.name: func.validate_and_call}
+        func.lookup_preview = {func.name: function_preview}
 
-        if json_schema:
-            # take the given json schema
-            schema_copy = deepcopy(json_schema)
-            func.validator = validator_from_schema(
-                schema_copy,
-                name=func.name,
-                override_with_doc_from=func if require_doc else None,
-            )
-            func.schema = [schema_to_openai_func(schema_copy)]
-        else:
-            # parse the docstring and create a pydantic model as validator
-            model, func.validator = validator_from_doc(
-                func, name=func.name, require_doc=require_doc
-            )
-            func.schema = [schema_to_openai_func(model)]
+        func.tasks = {}  # {call_id: (task, stream)}
 
-        func.validate_and_call = validate_and_call
-        func.lookup = {func.name: func.validate_and_call}
-        func.validate_and_call.in_thread = (
-            not asyncio.iscoroutinefunction(func) if in_thread is None else in_thread
-        )
         return func
 
-    if function:  # user did `@function_tool`, i.e. we were used directly as a decorator
-        return decorator(function)
-    else:  # user did `@function_tool()` or `@function_tool(name='foo')`
+    if function:  # user did `@streaming_function_tool`
+        raise ValueError(
+            "Please provide the JSON schema for the streaming function tool."
+        )
+    else:  # user did `@streaming_function_tool()`
         return decorator
-
-
-def fail_with_message(
-    message="[Internal Error] ", include_exception=True, logger: Callable = print
-):
-    """A decorator that catches exceptions from synchronous and asynchronous functions and returns the given message instead. Useful for agent tools."""
-
-    def log_exception(func, args, kwargs, e):
-        if logger:
-            logger(
-                f"""
-Tool call {func.__name__}({
-    ', '.join(list(map(repr, args)) + [f'{k}={repr(v)}' for k,v in kwargs.items()])
-}) failed: {e}
-""".strip()
-            )
-        return (message + (f": {str(e)}" if include_exception else "")).strip()
-
-    def decorator(func):
-        if asyncio.iscoroutinefunction(func):
-
-            @wraps(func)
-            async def async_wrapper(*args, **kwargs):
-                try:
-                    return await func(*args, **kwargs)
-                except Exception as e:
-                    return log_exception(func, args, kwargs, e)
-
-            return async_wrapper
-        else:
-
-            @wraps(func)
-            def sync_wrapper(*args, **kwargs):
-                try:
-                    return func(*args, **kwargs)
-                except Exception as e:
-                    return log_exception(func, args, kwargs, e)
-
-            return sync_wrapper
-
-    return decorator
```

### Comparing `agentools-0.2.2/agentools/tools/utils.py` & `agentools-0.4.3/agentools/tools/decorators/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,17 +93,17 @@
     name: Optional[str] = None,
     override_with_doc_from: Optional[Callable] = None,
 ) -> Callable:
     if name:
         json_schema["title"] = name
     if override_with_doc_from:
         doc = parse(inspect.getdoc(override_with_doc_from) or "")
-        json_schema[
-            "description"
-        ] = f"{doc.short_description or ''}\n{doc.long_description or ''}".strip()
+        json_schema["description"] = (
+            f"{doc.short_description or ''}\n{doc.long_description or ''}".strip()
+        )
 
     # Validate json against schema
     def validate_json(**state):
         v = Draft202012Validator(json_schema)
         if errors := "\n".join({e.message for e in v.iter_errors(state)}):
             raise ValidationError(errors)
         return True
@@ -154,7 +154,12 @@
             d.pop("title")
         for v in d.values():
             remove_title(v)
     elif isinstance(d, list):
         for v in d:
             remove_title(v)
     return d
+
+
+# ========== Misc ========== #
+async def awaitable(val):
+    return val
```

### Comparing `agentools-0.2.2/agentools/utils/trackers.py` & `agentools-0.4.3/agentools/utils/trackers.py`

 * *Files identical despite different names*

### Comparing `agentools-0.2.2/PKG-INFO` & `agentools-0.4.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 Metadata-Version: 2.1
 Name: agentools
-Version: 0.2.2
+Version: 0.4.3
 Summary: 
 Author: Joong-Won Seo
 Author-email: joong.won.seo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docstring-parser (>=0.15,<0.16)
-Requires-Dist: json-autocomplete (>=0.1.0,<0.2.0)
-Requires-Dist: jsonref (>=1.1.0,<2.0.0)
-Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
-Requires-Dist: openai (>=1.5.0,<2.0.0)
-Requires-Dist: pydantic (>=2.5.1,<3.0.0)
-Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
+Requires-Dist: groq (>=0.5,<0.6)
+Requires-Dist: json-autocomplete (>=0.2,<0.3)
+Requires-Dist: jsonref (>=1.1,<2.0)
+Requires-Dist: jsonschema (>=4.20,<5.0)
+Requires-Dist: openai (>=1.5,<2.0)
+Requires-Dist: pydantic (>=2.5,<3.0)
+Requires-Dist: qdrant-client (>=1.9,<2.0)
+Requires-Dist: tiktoken (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # [AgenTools](https://github.com/JoongWonSeo/agentools) - Async Generator Tools for LLMs
 
 A simple set of modules, wrappers and utils that are essential for LLM-based assistants and agents using the OpenAI API and function tools. It is useful for:
+
 - **OpenAI API:** Simple wrapper for the OpenAI API to provide mocked endpoints for easy testing without costing money, accumulating the delta chunks from streamed responses into partial responses, and easier token counting/tracking.
 - **Function Tools:** Easily convert any (async) python function into a function tool that the LLM model can call, with automatic validation and retrying with error messages.
 - **Structured Data:** Easily define a Pydantic model that can be generated by the LLM model, also with validation and retries.
 - **Assistants:** Event-based architecture with async generators that yield events that you can iterate through and handle only the events you care about, such as whether you want to stream the response or not, cancel the generation prematurely, or wait for user input (human-in-the-loop) before continuing, etc.
 - **Copilots:** Integrate right into an editor with stateful system messages to allow the copilot to see the latest state of the editor and function tools to interact with the editor.
 
 **Yet to come:**
+
 - **Agents:** Autoprompting, self-prompting, chain-of-thought, sketchpads, memory management, planning, and more.
 - **Multi-Agents**: Communication channels, organization structuring, and more.
 
-
 ## Quick Start
 
 ### Installation
 
 ```bash
 pip install agentools
 ```
 
+
 ### Assistant and ChatGPT
 
 A high-level interface to use ChatGPT or other LLM-based assistants! The default implementation of ChatGPT has:
+
 - a message history to remember the conversation so far (including the system prompt)
 - ability to use tools
 - efficient async streaming support
 - simple way to customize/extend/override the default behavior
 
 
+
 ```python
 from agentools import *
 
 # empty chat history and default model (gpt-3.5)
 model = ChatGPT()
 ```
 
 You can then simply call the model as if it was a function, with a prompt:
 
 
+
 ```python
 await model("Hey!")
 ```
 
 
 
 
@@ -71,45 +78,47 @@
 
 
 As you can see, the model is async and it simply returns the resonse as a string.
 
 Both your prompt and the response are stored in the history, so you can keep calling the model with new prompts and it will remember the conversation so far.
 
 
+
 ```python
 await model("Can you repeat my last message please?")
 ```
 
 
 
 
 
-> <code>'Of course! Your last message was: "Hey!"'</code><br/>
+> <code>'Of course! Your last message was "Hey!"'</code><br/>
 
 
 
 ```python
 model.messages.history
 ```
 
 
 
 
 
 > <code>[{'role': 'user', 'content': 'Hey!'},</code><br/>
 > <code> {'content': 'Hello! How can I assist you today?', 'role': 'assistant'},</code><br/>
 > <code> {'role': 'user', 'content': 'Can you repeat my last message please?'},</code><br/>
-> <code> {'content': 'Of course! Your last message was: "Hey!"', 'role': 'assistant'}]</code><br/>
+> <code> {'content': 'Of course! Your last message was "Hey!"', 'role': 'assistant'}]</code><br/>
 
 
 ### System prompt and more on `MessageHistory`
 
 Notice that our model has no system prompt in the beginning. `ChatGPT`'s constructor by default creates an empty chat history, but you can explicitly create a `MessageHistory` object and pass it to the constructor:
 
 
+
 ```python
 translate = ChatGPT(
     messages=SimpleHistory.system("Translate the user message to English")
 )
 # SimpleHistory.system(s) is just shorthand for SimpleHistory([msg(system=s)])
 
 print(await translate("Ich liebe Katzen!"))
@@ -134,14 +143,15 @@
 > <code> {'role': 'user', 'content': '고양이랑 강아지 둘다 좋아!'},</code><br/>
 > <code> {'content': 'I like both cats and dogs!', 'role': 'assistant'}]</code><br/>
 
 
 Notice that here, we're wasting tokens by remembering the chat history, since it's not really a conversation. There's a simple `GPT` class, which simply resets the message history after each prompt:
 
 
+
 ```python
 translate = GPT(messages=SimpleHistory.system("Translate the user message to English"))
 
 await translate("Ich liebe Katzen!")
 await translate("고양이랑 강아지 둘다 좋아!")
 
 translate.messages.history
@@ -155,14 +165,15 @@
 
 
 ### OpenAI API: changing the model and mocked API
 
 You can set the default model in the constructor, or override it for each prompt:
 
 
+
 ```python
 # default model is now gpt-4 💸
 model = ChatGPT(model="gpt-4")
 
 # but you can override it for each prompt anyways
 await model("Heyo!", model="mocked")
 ```
@@ -173,63 +184,70 @@
 
 > <code>'Hello, world!'</code><br/>
 
 
 As you see, our wrapper provides a simple mocked "model", which will simply return `"Hello, world!"` for any prompt, with some simulated latency. This will also work with streaming responses, and in either cases, you won't be able to tell the difference between the real API and the mocked one.
 
 There are more mocked models for your convinience:
+
 - `mocked`: always returns `"Hello, world!"`
 - `mocked:TEST123`: returns the string after the colon, e.g. `"TEST123"`
 - `echo`: returns the user prompt itself
 
 Let's print all events to the console to take a peek at the event-based generator:
 
 
+
 ```python
 await model("Heya!", model="echo", event_logger=print)
 ```
 
 
 > <code>[ResponseStartEvent]: prompt=Heya!, tools=None, model=echo, max_function_calls=100, openai_kwargs={}</code><br/>
 > <code>[CompletionStartEvent]: call_index=0</code><br/>
-> <code>[CompletionEvent]: completion=ChatCompletion(id='mock', choices=[Choice(finish_reason='stop', index=0, logprobs=None, message=ChatCompletionMessage(content='Heya!', role='assistant', function_call=None, tool_calls=None))], created=1706671307, model='mock', object='chat.completion', system_fingerprint=None, usage=None), call_index=0</code><br/>
+> <code>[CompletionEvent]: completion=ChatCompletion(id='mock', choices=[Choice(finish_reason='stop', index=0, logprobs=None, message=ChatCompletionMessage(content='Heya!', role='assistant', function_call=None, tool_calls=None))], created=1715958919, model='mock', object='chat.completion', system_fingerprint=None, usage=None), call_index=0</code><br/>
 > <code>[FullMessageEvent]: message=ChatCompletionMessage(content='Heya!', role='assistant', function_call=None, tool_calls=None), choice_index=0</code><br/>
 > <code>[TextMessageEvent]: content=Heya!</code><br/>
 > <code>[ResponseEndEvent]: content=Heya!</code><br/>
 
 
 
 
 > <code>'Heya!'</code><br/>
 
 
 Wow, quite a lot going on for a simple prompt! While it might seem like too many events, this offers a lot of flexibility and customizability.
 
 You can easily handle only the events you are interested in, useful when e.g:
+
 - updating the frontend when streaming the responses,
 - cancelling the generation early,
 - or implementing human-in-the-loop for function calls.
 
 For instance, the `GPT` class from above is as simple as:
+
 ```python
 async for event in self.response_events(prompt, **openai_kwargs):
     match event:
         case self.ResponseEndEvent():
             await self.messages.reset()
             return event.content
 ```
 
 This generator-based architecture is a good balance between flexibility and simplicity!
 
 While we won't go deeper into the low-level API in this quickstart, you can look at the `advanced.ipynb` notebook for more details.
 
+
 ### Tools: `@function_tool`
+
 You can turn any function into a tool usable by the model by decorating it with `@function_tool`:
 
 
+
 ```python
 @function_tool
 def print_to_console(text: str) -> str:
     """
     Print text to console
 
     Args:
@@ -251,42 +269,46 @@
 
 > <code>'success'</code><br/>
 
 
 You can use the tool from python as you normally would, and the model will also be able to use it simply by passing it to the `tools` parameter during init (as default) or prompting it (as a one-off).
 
 
+
 ```python
 model = ChatGPT(tools=print_to_console)
 await model("Say 'hello from GPT' to console!")
 ```
 
 
-> <code>Hello from GPT!</code><br/>
+> <code>hello from GPT</code><br/>
 
 
 
 
-> <code>'I have successfully printed "Hello from GPT!" to the console.'</code><br/>
+> <code>"I have printed 'hello from GPT' to the console."</code><br/>
 
 
 To make the function a `@function_tool`, you must do the following:
+
 - The parameters must be type annotated, and all parameters must be JSON-serializable (e.g. `str`, `int`, `float`, `bool`, `list`, `dict`, `None`, etc).
 - The return type should be a `str` or something that can be converted to a `str`.
 - It must be documented with a `'''docstring'''`, including each parameter (most [formats supported](https://github.com/rr-/docstring_parser), e.g. [Google-style](https://gist.github.com/redlotus/3bc387c2591e3e908c9b63b97b11d24e#file-docstrings-py-L67), [NumPy-style](https://gist.github.com/eikonomega/910512d92769b0cc382a09ae4de41771), sphinx-style, etc, see [this overview](https://gist.github.com/nipunsadvilkar/fec9d2a40f9c83ea7fd97be59261c400))
 
 
 Showing off some more goodies:
+
 - Even async functions should seamlessly work, just don't forget to `await` them.
 - `@fail_with_message(err)` is a decorator that will catch any exceptions thrown by the function and instead return the error message. This is useful for when you want to handle errors in a more graceful way than just crashing the model. It also takes an optional logger, which by default takes the `print` function, but any callable that takes a string will work, such as `logger.error` from the `logging` module.
 - Usually, the `@function_tool` decorator will throw an assertion error if you forget to provide the description for any of the function or their parameters. If you really don't want to provide descriptions for some (or all), maybe because it's so self-explanatory or you need to save tokens, then you can explicitly turn off the docstring parsing by passing `@function_tool(check_description=False)`. This is not recommended, but it's there if you need it.
 
 Note that by returning descriptive error strings, the model can read the error message and retry, increasing the robustness!
 
 
+
 ```python
 import asyncio
 import logging
 
 
 @function_tool(name="Fibonacci", require_doc=False)
 @fail_with_message("Error", logger=logging.error)
@@ -309,18 +331,20 @@
 
 
 
 > <code>'Error: n must be >= 0'</code><br/>
 
 
 ### Toolkits: `class Toolkit`
+
 Toolkits are a collection of related function tools, esp. useful when they share a state. Also good for keeping the state bound to a single instance of the toolkit, rather than a global state.
 To create a toolkit, simply subclass `Toolkit` and decorate its methods with `@function_tool`.
 
 
+
 ```python
 class Notepad(Toolkit):
     def __init__(self):
         super().__init__()
         self.content = "<Fill me in>"
 
     @function_tool
@@ -349,71 +373,165 @@
 
 > <code>"Shhh... here's a secret: 42"</code><br/>
 
 
 As before, simply pass the toolkit to the model. To use multiple tools and toolkits, simply use the `ToolList` class:
 
 
+
 ```python
-gpt = ChatGPT(
+model = ChatGPT(
     tools=ToolList(notes, print_to_console, fib),
 )
 
-await gpt("What's on my notepad?")
+await model("What's on my notepad?")
 ```
 
 
 
 
 
-> <code>'On your notepad, there is a secret written: 42.'</code><br/>
+> <code>'The secret on your notepad is: 42'</code><br/>
 
 
 
 ```python
-await gpt(
+await model(
     "Can you calculate the 8th fibonacci number, add it to the number in my notes, and write it? also print it to console as well.",
     event_logger=lambda x: print(x) if x.startswith("[Tool") else None,
 )
 ```
 
 
-> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_Uj8VIxhCxvHUnbIH1CK50Qmo', function=Function(arguments='{\n  "n": 8\n}', name='Fibonacci'), type='function')]</code><br/>
-> <code>[ToolResultEvent]: result=21, tool_call=ChatCompletionMessageToolCall(id='call_Uj8VIxhCxvHUnbIH1CK50Qmo', function=Function(arguments='{\n  "n": 8\n}', name='Fibonacci'), type='function'), index=0</code><br/>
-> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_0F0alwZitumJTU3QlPxuoJNW', function=Function(arguments='{\n  "text": "63"\n}', name='write'), type='function')]</code><br/>
-> <code>[ToolResultEvent]: result=None, tool_call=ChatCompletionMessageToolCall(id='call_0F0alwZitumJTU3QlPxuoJNW', function=Function(arguments='{\n  "text": "63"\n}', name='write'), type='function'), index=0</code><br/>
-> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_KoSyY1LZQYVfEpMDPUZlt2pc', function=Function(arguments='{\n  "text": "63"\n}', name='print_to_console'), type='function')]</code><br/>
-> <code>63</code><br/>
-> <code>[ToolResultEvent]: result=success, tool_call=ChatCompletionMessageToolCall(id='call_KoSyY1LZQYVfEpMDPUZlt2pc', function=Function(arguments='{\n  "text": "63"\n}', name='print_to_console'), type='function'), index=0</code><br/>
+> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_gDhzb8aiNmaJkUB6Z8tHZ7EU', function=Function(arguments='{"n": 8}', name='Fibonacci'), type='function'), ChatCompletionMessageToolCall(id='call_c9TjP8fWKTBrzie2TrzzOZeQ', function=Function(arguments='{}', name='read'), type='function')]</code><br/>
+> <code>[ToolResultEvent]: result=Shhh... here's a secret: 42, tool_call=ChatCompletionMessageToolCall(id='call_c9TjP8fWKTBrzie2TrzzOZeQ', function=Function(arguments='{}', name='read'), type='function'), index=1</code><br/>
+> <code>[ToolResultEvent]: result=21, tool_call=ChatCompletionMessageToolCall(id='call_gDhzb8aiNmaJkUB6Z8tHZ7EU', function=Function(arguments='{"n": 8}', name='Fibonacci'), type='function'), index=0</code><br/>
+> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_EU9GTOVIQHeF2LeXxlVcjYlk', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='write'), type='function')]</code><br/>
+> <code>[ToolResultEvent]: result=None, tool_call=ChatCompletionMessageToolCall(id='call_EU9GTOVIQHeF2LeXxlVcjYlk', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='write'), type='function'), index=0</code><br/>
+> <code>[ToolCallsEvent]: tool_calls=[ChatCompletionMessageToolCall(id='call_uIp1BSsPlmYc6dl0xgYX4s2h', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='print_to_console'), type='function')]</code><br/>
+> <code>The sum of the 8th Fibonacci number and the secret on your notepad: 63</code><br/>
+> <code>[ToolResultEvent]: result=success, tool_call=ChatCompletionMessageToolCall(id='call_uIp1BSsPlmYc6dl0xgYX4s2h', function=Function(arguments='{"text":"The sum of the 8th Fibonacci number and the secret on your notepad: 63"}', name='print_to_console'), type='function'), index=0</code><br/>
 
 
 
 
-> <code>'I have calculated the 8th Fibonacci number to be 21. I have added it to the number on your notepad, which is 42, and the result is 63.\n\nI have written the result, 63, on your notepad. However, it seems that there was an issue with writing it. My apologies for the inconvenience.\n\nI have also printed the result, 63, to the console.'</code><br/>
+> <code>'I have written the sum of the 8th Fibonacci number (21) and the secret on your notepad (42), which totals to 63. It has also been printed to the console.'</code><br/>
 
 
 
 ```python
 notes.read()
 ```
 
 
 
 
 
-> <code>'63'</code><br/>
+> <code>'The sum of the 8th Fibonacci number and the secret on your notepad: 63'</code><br/>
 
 
 Notice how since our `write` function doesn't return anything, it defaults to `None` and our model gets confused! So don't forget to return an encouraging success message to make our model happy :)
 
+
+### Tool Previews
+
+When using streaming, and you're using function tools with a long input, you might want to preview the tool's output before it's fully processed. With the help of the `json_autocomplete` package, the JSON argument generated by the model can be parsed before it's fully complete, and the preview can be shown to the user.
+
+
+
+```python
+@function_tool(require_doc=False)
+async def create_slogan(title: str, content: str):
+    print(f"\n\n[Final Slogan] {title}: {content}")
+    return "Slogan created and shown to user! Simply tell the user that it was created."
+
+
+@create_slogan.preview
+async def preview(title: str = "", content: str = ""):
+    assert isinstance(title, str) and isinstance(content, str)
+    print(f"[Preview] {title}: {content}", flush=True)
+```
+
+
+```python
+model = ChatGPT(tools=create_slogan)
+await model(
+    "Create a 1-sentence slogan about how ducks can help with debugging.", stream=True
+)
+```
+
+
+> <code>[Preview] : </code><br/>
+> <code>[Preview] D: </code><br/>
+> <code>[Preview] Ducks: </code><br/>
+> <code>[Preview] Ducks and: </code><br/>
+> <code>[Preview] Ducks and Debug: </code><br/>
+> <code>[Preview] Ducks and Debugging: </code><br/>
+> <code>[Preview] Ducks and Debugging: </code><br/>
+> <code>[Preview] Ducks and Debugging: Qu</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feather</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends.</code><br/>
+> <code>[Preview] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends.</code><br/>
+> <code>[Final Slogan] Ducks and Debugging: Quack your way to bug-free code with the help of our feathered friends.</code><br/>
+
+
+
+
+> <code>'I have created a slogan about how ducks can help with debugging.'</code><br/>
+
+
+If you need a more coherent logic shared between the `@preview` and the final `@function_tool`, e.g. do something at the start of the function call, share some data between previews, etc... It gets messy very fast!
+
+Instead, you can use the `@streaming_function_tool()` decorator, which receives a single `arg_stream` parameter, which is an async generator that yields the partial arguments, as streamed from the model. Therefore, you simply need to iterate through it, and perform the actual function call at the end of the iteration. The following is the equivalent of the previous example:
+
+> _Note that currently, you must pass the parameter as a `json_schema`. Soon, this could be parsed from the docstring as usual._
+
+
+
+```python
+from pydantic import BaseModel
+
+
+class Slogan(BaseModel):
+    title: str
+    content: str
+
+
+@streaming_function_tool(json_schema=Slogan.model_json_schema())
+async def create_slogan(arg_stream):
+    print("Starting slogan creation...")
+
+    async for args in arg_stream:
+        title, content = args.get("title", ""), args.get("content", "")
+        print(f'{args} -> "{title}", "{content}"')
+
+    print(f"\n\n[Final Slogan] {title}: {content}")
+    return "Slogan created and shown to user! Simply tell the user that it was created."
+```
+
 ### Structured Data
 
 We can very easily define a Pydantic model that can be generated by the LLM model, with validation and retries:
 
 
+
 ```python
 from pydantic import BaseModel, Field
 
 
 class Song(BaseModel):
     title: str
     genres: list[str] = Field(description="AT LEAST 3 genres!")
@@ -430,28 +548,31 @@
 
 > <code>Song(title='Hello', genres=['pop'], duration=3.5)</code><br/>
 
 
 Create a `StructGPT` object with your pydantic model, and prompting it will always return a valid instance of the model, or raise an exception if it fails to generate a valid instance after the maximum number of retries. Your docstring and field descriptions will also be visible to the model, so make sure to write good descriptions!
 
 
+
 ```python
 generate_song = StructGPT(Song)
 
 await generate_song("Come up with an all-time best K-hiphop song")
 ```
 
 
 
 
 
-> <code>Song(title='Respect My Name', genres=['Hip-Hop', 'K-Rap', 'Trap'], duration=240.0)</code><br/>
+> <code>Song(title='Eung Freestyle', genres=['K-HipHop', 'Rap', 'Hip-Hop'], duration=192.0)</code><br/>
 
 
 ## Misc.
 
 Streaming can be enabled as usual by passing `stream=True` when prompting, and handle the partial events as they come in. Check the `Assistant` class for a list of events including the ones for streaming.
 
 There are some other useful utilities in the `utils` module, such as:
+
 - `tokens`: for token counting
 - `trackers`: for transparent token tracking and prompt/response logging
 
+
```

