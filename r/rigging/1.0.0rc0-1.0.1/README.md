# Comparing `tmp/rigging-1.0.0rc0.tar.gz` & `tmp/rigging-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rigging-1.0.0rc0.tar", max compression
+gzip compressed data, was "rigging-1.0.1.tar", max compression
```

## Comparing `rigging-1.0.0rc0.tar` & `rigging-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1066 2024-05-06 23:20:05.140907 rigging-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     1477 2024-05-06 23:20:05.140907 rigging-1.0.0rc0/README.md
--rw-r--r--   0        0        0     2146 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0      684 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/__init__.py
--rw-r--r--   0        0        0    39816 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/chat.py
--rw-r--r--   0        0        0    21074 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/completion.py
--rw-r--r--   0        0        0      865 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/error.py
--rw-r--r--   0        0        0    19110 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/generator.py
--rw-r--r--   0        0        0     2349 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/logging.py
--rw-r--r--   0        0        0    13107 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/message.py
--rw-r--r--   0        0        0    12573 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/model.py
--rw-r--r--   0        0        0     3748 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/parsing.py
--rw-r--r--   0        0        0     1090 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/prompt.py
--rw-r--r--   0        0        0        0 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/py.typed
--rw-r--r--   0        0        0    10210 2024-05-06 23:20:05.144907 rigging-1.0.0rc0/rigging/tool.py
--rw-r--r--   0        0        0     2213 1970-01-01 00:00:00.000000 rigging-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-16 22:53:46.951126 rigging-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1477 2024-05-16 22:53:46.951126 rigging-1.0.1/README.md
+-rw-r--r--   0        0        0     2392 2024-05-16 22:53:46.955127 rigging-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      818 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/__init__.py
+-rw-r--r--   0        0        0    41725 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/chat.py
+-rw-r--r--   0        0        0    26509 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/completion.py
+-rw-r--r--   0        0        0     3028 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/data.py
+-rw-r--r--   0        0        0      865 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/error.py
+-rw-r--r--   0        0        0    19086 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/generator.py
+-rw-r--r--   0        0        0     1791 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/logging.py
+-rw-r--r--   0        0        0    13768 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/message.py
+-rw-r--r--   0        0        0    12579 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/model.py
+-rw-r--r--   0        0        0     3748 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/parsing.py
+-rw-r--r--   0        0        0     1090 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/py.typed
+-rw-r--r--   0        0        0    10466 2024-05-16 22:53:46.955127 rigging-1.0.1/rigging/tool.py
+-rw-r--r--   0        0        0     2249 1970-01-01 00:00:00.000000 rigging-1.0.1/PKG-INFO
```

### Comparing `rigging-1.0.0rc0/LICENSE` & `rigging-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rigging-1.0.0rc0/README.md` & `rigging-1.0.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - Chat templating, forking, continuations, generation parameter overloads, stripping segments, etc.
 - Modern python with type hints, async support, pydantic validation, serialization, etc.
 
 ```py
 import rigging as rg
 from rigging.model import CommaDelimitedAnswer as Answer
 
-answer = rg.get_generator('gpt-4') \
+chat = rg.get_generator('gpt-4') \
     .chat(f"Give me 3 famous authors between {Answer.xml_tags()} tags.") \
     .until_parsed_as(Answer) \
     .run()
 
 answer = chat.last.parse(Answer)
 print(answer.items)
 
@@ -36,8 +36,8 @@
 ```bash
 cd rigging/
 poetry install
 ```
 
 ## Getting Started
 
-Head over to **[our documentation](https://rigging.dreadnode.io) for more information.
+Head over to **[our documentation](https://rigging.dreadnode.io)** for more information.
```

### Comparing `rigging-1.0.0rc0/pyproject.toml` & `rigging-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rigging"
-version = "1.0.0rc0"
+version = "1.0.1"
 description = "LLM Interaction Framework"
 authors = ["Nick Landers <monoxgas@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/dreadnode/rigging"
 readme = "README.md"
 packages = [
     {include = "rigging"}
@@ -12,20 +12,24 @@
 
 [tool.poetry.dependencies]
 python = "<3.13,>=3.10"
 pydantic = "2.5.3"
 pydantic-xml = "2.7.0"
 loguru = "^0.7.2"
 litellm = "1.35.21"
+pandas = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.27.1"
 mypy = "^1.8.0"
 ruff = "^0.1.14"
 pytest = "^8.0.0"
+pandas = "^2.2.2"
+pandas-stubs = "^2.2.1.240316"
+coverage = "^7.5.1"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.6.0"
 mkdocs-material = {extras = ["imaging"], version = "^9.5.20"}
 mkdocstrings = "^0.25.0"
 mkdocstrings-python = "^1.10.0"
 mkdocs-section-index = "^0.3.9"
@@ -35,14 +39,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 filterwarnings = ["ignore::DeprecationWarning"]
 
+[tool.coverage.run]
+command_line = "-m pytest"
+
+[tool.coverage.report]
+include = ["rigging/*.py"]
+show_missing = true
+
+[tool.coverage.lcov]
+output = "lcov.info"
+
 [tool.mypy]
 plugins = "pydantic.mypy"
 strict = true
 
 [tool.ruff]
 select = [
     "E",   # pycodestyle errors
```

### Comparing `rigging-1.0.0rc0/rigging/chat.py` & `rigging-1.0.1/rigging/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,27 +18,25 @@
     ConfigDict,
     Field,
     ValidationError,
     computed_field,
 )
 
 from rigging.error import ExhaustedMaxRoundsError
+from rigging.generator import GenerateParams, Generator, get_generator
 from rigging.message import Message, MessageDict, Messages
 from rigging.model import (
     Model,
     ModelT,
     SystemErrorModel,
     ValidationErrorModel,
 )
 from rigging.prompt import system_tool_extension
 from rigging.tool import Tool, ToolCalls, ToolDescriptionList, ToolResult, ToolResults
 
-if t.TYPE_CHECKING:
-    from rigging.generator import GenerateParams, Generator
-
 DEFAULT_MAX_ROUNDS = 5
 
 
 class Chat(BaseModel):
     """
     Represents a completed chat conversation.
     """
@@ -57,15 +55,16 @@
     """Additional metadata for the chat."""
 
     generator: t.Optional["Generator"] = Field(None, exclude=True, repr=False)
     """The generator associated with the chat."""
     params: t.Optional["GenerateParams"] = Field(None, exclude=True, repr=False)
     """Any additional generation params used for this chat."""
 
-    @computed_field(repr=False)
+    @computed_field(repr=False)  # type: ignore[misc]
+    @property
     def generator_id(self) -> str | None:
         """The identifier of the generator used to create the chat"""
         if self.generator is not None:
             return self.generator.to_identifier(self.params)
         return None
 
     def __init__(
@@ -80,15 +79,14 @@
 
         Args:
             messages: The messages for the chat.
             generated: The next messages for the chat.
             generator: The generator associated with this chat.
             **kwargs: Additional keyword arguments (typically used for deserialization)
         """
-        from rigging.generator import get_generator
 
         if "generator_id" in kwargs and generator is None:
             # TODO: Should we move params to self.params?
             generator = get_generator(kwargs.pop("generator_id"))
 
         super().__init__(
             messages=Message.fit_as_list(messages),
@@ -121,14 +119,24 @@
         return self.generated[-1]
 
     @property
     def conversation(self) -> str:
         """Returns a string representation of the chat."""
         return "\n\n".join([str(m) for m in self.all])
 
+    @property
+    def message_dicts(self) -> list[MessageDict]:
+        """
+        Returns the chat as a minimal dictionary
+
+        Returns:
+            The chat as a list of messages with roles and content.
+        """
+        return [t.cast(MessageDict, m.model_dump(include={"role", "content"})) for m in self.all]
+
     def meta(self, **kwargs: t.Any) -> "Chat":
         """
         Updates the metadata of the chat with the provided key-value pairs.
 
         Args:
             **kwargs: Key-value pairs representing the metadata to be updated.
 
@@ -201,29 +209,32 @@
 
         Args:
             **kwargs: The string mapping of replacements.
 
         Returns:
             The modified Chat object.
         """
-        self.last.apply(**kwargs)
+        if self.generated:
+            self.generated[-1] = self.generated[-1].apply(**kwargs)
+        else:
+            self.messages[-1] = self.messages[-1].apply(**kwargs)
         return self
 
     def apply_to_all(self, **kwargs: str) -> "Chat":
         """
         Calls [rigging.message.Message.apply][] on all messages in the chat with the given keyword arguments.
 
         Args:
             **kwargs: The string mapping of replacements.
 
         Returns:
             The modified chat object.
         """
-        for message in self.all:
-            message.apply(**kwargs)
+        self.messages = Message.apply_to_list(self.messages, **kwargs)
+        self.generated = Message.apply_to_list(self.generated, **kwargs)
         return self
 
     def strip(self, model_type: type[Model], fail_on_missing: bool = False) -> "Chat":
         """
         Strips all parsed parts of a particular type from the message content.
 
         Args:
@@ -268,17 +279,18 @@
         """
         call_format = ToolCalls.xml_example()
         tool_description_list = ToolDescriptionList(tools=[t.get_description() for t in tools])
         tool_system_prompt = system_tool_extension(call_format, tool_description_list.to_pretty_xml())
         self.inject_system_content(tool_system_prompt)
 
 
-# Callbacks for pending chat
+# Callbacks
 
 
+@runtime_checkable
 class UntilMessageCallback(t.Protocol):
     def __call__(self, message: Message) -> tuple[bool, list[Message]]:
         """
         Passed the next message, returns whether or not to continue and an
         optional list of messages to append before continuing.
         """
         ...
@@ -317,15 +329,18 @@
     async def __call__(self, chats: list[Chat]) -> list[Chat]:
         """
         async variant of the [rigging.chat.MapChatCallback][] protocol.
         """
         ...
 
 
-PostRunCallbacks = ThenChatCallback | AsyncThenChatCallback | MapChatCallback | AsyncMapChatCallback
+ThenChatCallbacks = ThenChatCallback | AsyncThenChatCallback
+MapChatCallbacks = MapChatCallback | AsyncMapChatCallback
+
+# Generators
 
 MessageProducer = t.Generator[t.Sequence[Message], None, None]
 MessagesProducer = t.Generator[t.Sequence[t.Sequence[Message]], None, None]
 
 # Helper classes to manage complexity inside the run functions
 
 
@@ -344,14 +359,21 @@
     messages: list[Message]
     params: "GenerateParams"
     processor: t.Generator[list[Message], Message, list[Message]]
     chat: Chat | None = None
     done: bool = False
 
 
+@dataclass
+class BatchRunPool:
+    generator: "Generator"
+    finished_states: list[BatchRunState]
+    pending_states: list[BatchRunState]
+
+
 class PendingChat:
     """
     Represents a pending chat that can be modified and executed.
     """
 
     def __init__(
         self, generator: "Generator", messages: t.Sequence[Message], params: t.Optional["GenerateParams"] = None
@@ -367,33 +389,35 @@
 
         # (callback, attempt_recovery, drop_dialog, max_rounds)
         self.until_callbacks: list[tuple[UntilMessageCallback, bool, bool, int]] = []
         self.until_types: list[type[Model]] = []
         self.until_tools: list[Tool] = []
         self.inject_tool_prompt: bool = True
         self.force_tool: bool = False
-        self.post_run_callbacks: list[PostRunCallbacks] = []
+        self.then_chat_callbacks: list[ThenChatCallbacks] = []
+        self.map_chat_callbacks: list[MapChatCallbacks] = []
         # self.producer: MessageProducer | None = None
 
+    def __len__(self) -> int:
+        return len(self.chat)
+
     def with_(self, params: t.Optional["GenerateParams"] = None, **kwargs: t.Any) -> "PendingChat":
         """
         Assign specific generation parameter overloads for this chat.
 
         Note:
             This will trigger a `clone` if overload params have already been set.
 
         Args:
             params: The parameters to set for the chat.
             **kwargs: An alternative way to pass parameters as keyword arguments.
 
         Returns:
             A new instance of PendingChat with the updated parameters.
         """
-        from rigging.generator import GenerateParams
-
         if params is None:
             params = GenerateParams(**kwargs)
 
         if self.params is not None:
             new = self.clone()
             new.params = self.params.merge_with(params)
             return new
@@ -500,15 +524,15 @@
 
         Args:
             callback: The callback function to be executed.
 
         Returns:
             The current instance of the chat.
         """
-        self.post_run_callbacks.append(callback)
+        self.then_chat_callbacks.append(callback)
         return self
 
     def map(self, callback: MapChatCallback | AsyncMapChatCallback) -> "PendingChat":
         """
         Registers a callback to be executed after the generation process completes.
 
         Note:
@@ -528,15 +552,15 @@
 
         Args:
             callback: The callback function to be executed.
 
         Returns:
             The current instance of the chat.
         """
-        self.post_run_callbacks.append(callback)
+        self.map_chat_callbacks.append(callback)
         return self
 
     # def from_(self, producer: MessageProducer) -> "PendingChat":
     #     """
     #     Adds a generator to the chat to produce messages.
 
     #     Args:
@@ -581,22 +605,22 @@
         new.chat.apply_to_all(**kwargs)
         return new
 
     def until(
         self,
         callback: UntilMessageCallback,
         *,
-        attempt_recovery: bool = False,
+        attempt_recovery: bool = True,
         drop_dialog: bool = True,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
     ) -> "PendingChat":
         """
         Registers a callback to participate in validating the generation process.
 
-        ```python
+        ```py
         # Takes the next message being generated, and returns whether or not to continue
         # generating new messages in addition to a list of messages to append before continuing
 
         def callback(message: Message) -> tuple[bool, list[Message]]:
             if is_valid(message):
                 return (False, [message])
             else:
@@ -623,41 +647,40 @@
             The current instance of the chat.
         """
         self.until_callbacks.append((callback, attempt_recovery, drop_dialog, max_rounds))
         return self
 
     def using(
         self,
-        tool: Tool | t.Sequence[Tool],
-        *,
+        *tools: Tool,
         force: bool = False,
         attempt_recovery: bool = True,
         drop_dialog: bool = False,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
         inject_prompt: bool | None = None,
     ) -> "PendingChat":
         """
         Adds a tool or a sequence of tools to participate in the generation process.
 
         Args:
-            tool: The tool or sequence of tools to be added.
+            tools: The tool or sequence of tools to be added.
             force: Whether to force the use of the tool(s) at least once.
             attempt_recovery: Whether to attempt recovery if the tool(s) fail by providing
                 validation feedback to the model before the next round.
             drop_dialog: Whether to drop the intermediate dialog of recovery efforts
                 before returning the final chat to the caller.
             max_rounds: The maximum number of rounds to attempt recovery.
             inject_prompt: Whether to inject the tool guidance prompt into a
                 system message.and will override self.inject_tool_prompt if provided.
 
         Returns:
             The updated PendingChat object.
 
         """
-        self.until_tools += tool if isinstance(tool, t.Sequence) else [tool]
+        self.until_tools += tools
         self.inject_tool_prompt = inject_prompt or self.inject_tool_prompt
         self.force_tool = force
         if next((c for c in self.until_callbacks if c[0] == self._until_tools_callback), None) is None:
             self.until_callbacks.append(
                 (
                     self._until_tools_callback,
                     attempt_recovery,
@@ -796,42 +819,53 @@
     # TODO: Much like the PendingCompletion code, it's opaque
     # exactly how multiple callbacks should be blended together
     # when generating. I think we should look at limiting it to
     # one callback in total, but I'll leave the behavior as is
     # for now with the knowledge that behavior might be a bit
     # unpredictable.
     def _process(self) -> t.Generator[list[Message], Message, list[Message]]:
+        self._pre_run()
         first_response = yield []
         new_messages = [first_response]
         for callback, reset_between, drop_internal, max_rounds in self.until_callbacks:
             generated = yield from self._until(new_messages[-1], callback, reset_between, drop_internal, max_rounds)
             new_messages = new_messages[:-1] + generated
         return new_messages
 
     def _post_run(self, chats: list[Chat]) -> list[Chat]:
-        for callback in self.post_run_callbacks:
-            if isinstance(callback, ThenChatCallback):
-                chats = [callback(chat) or chat for chat in chats]
-            elif isinstance(callback, MapChatCallback):
-                chats = callback(chats)
+        for map_callback in self.map_chat_callbacks:
+            if asyncio.iscoroutinefunction(map_callback):
+                raise ValueError(
+                    f"Cannot use async map() callbacks inside a non-async run call: {map_callback.__name__}"
+                )
+            chats = map_callback(chats)  # type: ignore
+
+        for then_callback in self.then_chat_callbacks:
+            if asyncio.iscoroutinefunction(then_callback):
+                raise ValueError(
+                    f"Cannot use async then() callbacks inside a non-async run call: {then_callback.__name__}"
+                )
+            chats = [then_callback(chat) or chat for chat in chats]  # type: ignore
 
         return chats
 
     async def _apost_run(self, chats: list[Chat]) -> list[Chat]:
-        if not all(
-            isinstance(callback, AsyncThenChatCallback | AsyncMapChatCallback) for callback in self.post_run_callbacks
-        ):
-            raise ValueError("Cannot use async then()/map() callbacks inside a non-async run call")
-
-        for callback in self.post_run_callbacks:
-            if isinstance(callback, AsyncThenChatCallback):
-                updated = await asyncio.gather(*[callback(chat) for chat in chats])
-                chats = [updated[i] or chat for i, chat in enumerate(chats)]
-            elif isinstance(callback, AsyncMapChatCallback):
-                chats = await callback(chats)
+        for map_callback in self.map_chat_callbacks:
+            if not asyncio.iscoroutinefunction(map_callback):
+                raise ValueError(
+                    f"Cannot use non-async map() callbacks inside an async run call: {map_callback.__call__.__name__}"
+                )
+            chats = await map_callback(chats)
+
+        for then_callback in self.then_chat_callbacks:
+            if not asyncio.iscoroutinefunction(then_callback):
+                raise ValueError(
+                    f"Cannot use non-async then() callbacks inside an async run call: {then_callback.__call__.__name__}"
+                )
+            chats = [await then_callback(chat) or chat for chat in chats]
 
         return chats
 
     def _pre_run(self) -> None:
         if self.until_tools:
             if self.inject_tool_prompt:
                 self.chat.inject_tool_prompt(self.until_tools)
@@ -843,16 +877,14 @@
             # requesting a tool call, so we'll remove it for now.
             #
             # self.params.stop = [ToolCalls.xml_end_tag()]
 
     def _fit_params(
         self, count: int, params: t.Sequence[t.Optional["GenerateParams"] | None] | None = None
     ) -> list["GenerateParams"]:
-        from rigging.generator import GenerateParams
-
         params = [None] * count if params is None else list(params)
         if len(params) != count:
             raise ValueError(f"The number of params must be {count}")
         if self.params is not None:
             params = [self.params.merge_with(p) for p in params]
         return [(p or GenerateParams()) for p in params]
 
@@ -976,116 +1008,135 @@
 
         return await self._apost_run([s.chat for s in states if s.chat is not None])
 
     # Batch messages
 
     def run_batch(
         self,
-        many: t.Sequence[t.Sequence[Message]] | t.Sequence[Message] | t.Sequence[MessageDict] | t.Sequence[str],
+        many: t.Sequence[t.Sequence[Message]]
+        | t.Sequence[Message]
+        | t.Sequence[MessageDict]
+        | t.Sequence[str]
+        | MessageDict
+        | str,
         params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
         *,
+        size: int | None = None,
         skip_failed: bool = False,
     ) -> list[Chat]:
         """
         Executes the generation process accross multiple input messages.
 
         Note:
             Anything already in this pending chat will be used as the `prefix` parameter
             to [rigging.generator.Generator.generate_messages][].
 
         Parameters:
             many: A sequence of sequences of messages to be generated.
             params: A sequence of parameters to be used for each set of messages.
+            size: The max chunk size of messages to execute generation at once.
             skip_failed: Enable to ignore any max rounds errors and return only successful chats.
 
         Returns:
             A list of generatated Chats.
         """
-        if isinstance(many, str | dict):
-            raise ValueError("many must be a sequence, even if it only contains one item")
+        if isinstance(many, dict) or isinstance(many, str):  # Some strange typechecking here
+            many = t.cast(t.Sequence[str] | t.Sequence[MessageDict], [many])
 
         count = max(len(many), len(params) if params is not None else 0)
         many = self._fit_many(count, many)
         params = self._fit_params(count, params)
 
         states: list[BatchRunState] = [
             BatchRunState(m, [], p, self._process()) for m, p in zip(many, params, strict=True)
         ]
         _ = [next(state.processor) for state in states]
 
+        size = size or len(states)
+
         pending_states = states
         while pending_states:
-            inbounds = self.generator.generate_messages(
-                [s.inputs + s.messages for s in pending_states],
-                [s.params for s in pending_states],
-                prefix=self.chat.all,
-            )
+            for chunk in [pending_states[i : i + size] for i in range(0, len(pending_states), size)]:
+                inbounds = self.generator.generate_messages(
+                    [s.inputs + s.messages for s in chunk],
+                    [s.params for s in chunk],
+                    prefix=self.chat.all,
+                )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
-                try:
-                    state.messages = state.processor.send(inbound)
-                except StopIteration as stop:
-                    state.done = True
-                    state.chat = Chat(
-                        self.chat.all,
-                        t.cast(list[Message], stop.value),
-                        generator=self.generator,
-                        metadata=self.metadata,
-                        params=state.params,
-                    )
-                except ExhaustedMaxRoundsError:
-                    if not skip_failed:
-                        raise
-                    state.done = True
+                for inbound, state in zip(inbounds, chunk, strict=True):
+                    try:
+                        state.messages = state.processor.send(inbound)
+                    except StopIteration as stop:
+                        state.done = True
+                        state.chat = Chat(
+                            self.chat.all + state.inputs,
+                            t.cast(list[Message], stop.value),
+                            generator=self.generator,
+                            metadata=self.metadata,
+                            params=state.params,
+                        )
+                    except ExhaustedMaxRoundsError:
+                        if not skip_failed:
+                            raise
+                        state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return self._post_run([s.chat for s in states if s.chat is not None])
 
     async def arun_batch(
         self,
-        many: t.Sequence[t.Sequence[Message]] | t.Sequence[Message] | t.Sequence[MessageDict] | t.Sequence[str],
+        many: t.Sequence[t.Sequence[Message]]
+        | t.Sequence[Message]
+        | t.Sequence[MessageDict]
+        | t.Sequence[str]
+        | MessageDict
+        | str,
         params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
         *,
+        size: int | None = None,
         skip_failed: bool = False,
     ) -> list[Chat]:
         """async variant of the [rigging.chat.PendingChat.run_batch][] method."""
-        if isinstance(many, str | dict):
-            raise ValueError("many must be a sequence, even if it only contains one item")
+        if isinstance(many, dict) or isinstance(many, str):  # Some strange typechecking here
+            many = t.cast(t.Sequence[str] | t.Sequence[MessageDict], [many])
 
         count = max(len(many), len(params) if params is not None else 0)
         many = self._fit_many(count, many)
         params = self._fit_params(count, params)
 
         states: list[BatchRunState] = [
             BatchRunState(m, [], p, self._process()) for m, p in zip(many, params, strict=True)
         ]
         _ = [next(state.processor) for state in states]
 
+        size = size or len(states)
+
         pending_states = states
         while pending_states:
-            inbounds = await self.generator.agenerate_messages(
-                [s.inputs + s.messages for s in pending_states],
-                [s.params for s in pending_states],
-                prefix=self.chat.all,
-            )
+            for chunk in [pending_states[i : i + size] for i in range(0, len(pending_states), size)]:
+                inbounds = await self.generator.agenerate_messages(
+                    [s.inputs + s.messages for s in chunk],
+                    [s.params for s in chunk],
+                    prefix=self.chat.all,
+                )
 
-            for inbound, state in zip(inbounds, pending_states, strict=True):
-                try:
-                    state.messages = state.processor.send(inbound)
-                except StopIteration as stop:
-                    state.done = True
-                    state.chat = Chat(
-                        self.chat.all,
-                        t.cast(list[Message], stop.value),
-                        generator=self.generator,
-                        metadata=self.metadata,
-                        params=state.params,
-                    )
-                except ExhaustedMaxRoundsError:
-                    if not skip_failed:
-                        raise
-                    state.done = True
+                for inbound, state in zip(inbounds, chunk, strict=True):
+                    try:
+                        state.messages = state.processor.send(inbound)
+                    except StopIteration as stop:
+                        state.done = True
+                        state.chat = Chat(
+                            self.chat.all + state.inputs,
+                            t.cast(list[Message], stop.value),
+                            generator=self.generator,
+                            metadata=self.metadata,
+                            params=state.params,
+                        )
+                    except ExhaustedMaxRoundsError:
+                        if not skip_failed:
+                            raise
+                        state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
         return await self._apost_run([s.chat for s in states if s.chat is not None])
```

### Comparing `rigging-1.0.0rc0/rigging/completion.py` & `rigging-1.0.1/rigging/completion.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
 Completions work with isolated strings of text pre and post generation.
 """
 
+import asyncio
 import string
 import typing as t
 from copy import deepcopy
 from dataclasses import dataclass
 from datetime import datetime
+from typing import runtime_checkable
 from uuid import UUID, uuid4
 
 from loguru import logger
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     computed_field,
 )
 
 from rigging.error import ExhaustedMaxRoundsError
+from rigging.generator import GenerateParams, Generator, get_generator
 from rigging.model import (
     Model,
     ModelT,
 )
 from rigging.parsing import parse_many
 
-if t.TYPE_CHECKING:
-    from rigging.generator import GenerateParams, Generator
-
 DEFAULT_MAX_ROUNDS = 5
 
 # TODO: Chats and Completions share a lot of structure and code.
 # Ideally we should build out a base class which they both inherit from.
 
 
 class Completion(BaseModel):
@@ -45,52 +45,53 @@
     timestamp: datetime = Field(default_factory=datetime.now, repr=False)
     """The timestamp when the completion was created."""
     text: str
     """The original text."""
     generated: str
     """The generated text."""
     metadata: dict[str, t.Any] = Field(default_factory=dict)
-    """Additional metadata for the chat."""
+    """Additional metadata for the completion."""
 
-    pending: t.Optional["PendingCompletion"] = Field(None, exclude=True, repr=False)
-    """The pending completion associated with this completion."""
+    generator: t.Optional["Generator"] = Field(None, exclude=True, repr=False)
+    """The generator associated with the completion."""
+    params: t.Optional["GenerateParams"] = Field(None, exclude=True, repr=False)
+    """Any additional generation params used for this completion."""
 
-    @computed_field(repr=False)
+    @computed_field(repr=False)  # type: ignore[misc]
+    @property
     def generator_id(self) -> str | None:
         """The identifier of the generator used to create the completion"""
-        if self.pending is not None:
-            return self.pending.generator.to_identifier(self.pending.params)
+        if self.generator is not None:
+            return self.generator.to_identifier(self.params)
         return None
 
     def __init__(
         self,
         text: str,
         generated: str,
-        pending: t.Optional["PendingCompletion"] = None,
+        generator: t.Optional["Generator"] = None,
         **kwargs: t.Any,
     ):
         """
-        Initialize a Chat object.
+        Initialize a Completion object.
 
         Args:
             text: The original text.
             generated: The generated text.
-            pending: The pending completion associated with this completion.
+            generator: The generator associated with this completion.
             **kwargs: Additional keyword arguments (typically used for serialization).
         """
-        from rigging.generator import get_generator
-
-        if "generator_id" in kwargs and pending is None:
+        if "generator_id" in kwargs and generator is None:
+            # TODO: Should we move params to self.params?
             generator = get_generator(kwargs.pop("generator_id"))
-            pending = generator.complete(text)
 
         super().__init__(
             text=text,
             generated=generated,
-            pending=pending,
+            generator=generator,
             **kwargs,
         )
 
     def __len__(self) -> int:
         return len(self.text) + len(self.generated)
 
     @property
@@ -99,54 +100,121 @@
         return self.text + self.generated
 
     def restart(self, *, generator: t.Optional["Generator"] = None, include_all: bool = False) -> "PendingCompletion":
         """
         Attempt to convert back to a PendingCompletion for further generation.
 
         Args:
-            generator: The generator to use for the restarted chat. Otherwise
+            generator: The generator to use for the restarted completion. Otherwise
                 the generator from the original PendingCompletion will be used.
             include_all: Whether to include the generation before the next round.
 
         Returns:
             The restarted completion.
 
         Raises:
             ValueError: If the completion was not created with a PendingCompletion and no generator is provided.
         """
 
-        text = self.all if include_all else self.text
-        if generator is not None:
-            return generator.complete(text)
-        elif self.pending is None:
-            raise ValueError("Cannot restart Completion that was not created with a PendingCompletion")
-        return PendingCompletion(self.pending.generator, text, self.pending.params)
+        text = self.all if include_all else self.generated
+        if generator is None:
+            generator = self.generator
+        if generator is None:
+            raise ValueError("Cannot restart a completion without an associated generator")
+        return generator.complete(text, self.params)
 
-    def fork(self, text: str) -> "PendingCompletion":
+    def fork(self, text: str, *, include_all: bool = False) -> "PendingCompletion":
         """
         Forks the completion by creating calling [rigging.completion.Completion.restart][] and appends the specified text.
 
         Args:
             text: The text to append.
 
         Returns:
             A new instance of a pending competion with the specified messages added.
         """
-        return self.restart().add(text)
+        return self.restart(include_all=include_all).add(text)
 
-    def clone(self) -> "Completion":
-        """Creates a deep copy of the chat."""
-        return Completion(self.text, self.generated, self.pending)
+    def continue_(self, text: str) -> "PendingCompletion":
+        """Alias for the [rigging.completion.Completion.fork][] with `include_all=True`."""
+        return self.fork(text, include_all=True)
+
+    def clone(self, *, only_messages: bool = False) -> "Completion":
+        """Creates a deep copy of the completion."""
+        new = Completion(self.text, self.generated, self.generator)
+        if not only_messages:
+            new.metadata = deepcopy(self.metadata)
+        return new
+
+    def meta(self, **kwargs: t.Any) -> "Completion":
+        """
+        Updates the metadata of the completion with the provided key-value pairs.
 
+        Args:
+            **kwargs: Key-value pairs representing the metadata to be updated.
+
+        Returns:
+            The updated completion object.
+        """
+        new = self.clone()
+        new.metadata.update(kwargs)
+        return new
 
-# Passed the next message, returns whether or not to continue
-# and an optional list of messages to append before continuing
-UntilCompletionCallback = t.Callable[[str], bool]
 
-ThenCompletionCallback = t.Callable[[Completion], Completion | None]
+# Callbacks
+
+
+@runtime_checkable
+class UntilCompletionCallback(t.Protocol):
+    def __call__(self, text: str) -> bool:
+        """
+        A callback function that takes the generated text and returns whether or not to retry generation.
+        """
+        ...
+
+
+@runtime_checkable
+class ThenCompletionCallback(t.Protocol):
+    def __call__(self, completion: Completion) -> Completion | None:
+        """
+        Passed a finalized completion to process and can return a new completion to replace it.
+        """
+        ...
+
+
+@runtime_checkable
+class AsyncThenCompletionCallback(t.Protocol):
+    async def __call__(self, completion: Completion) -> Completion | None:
+        """
+        async variant of the [rigging.completion.ThenCompletionCallback][] protocol.
+        """
+        ...
+
+
+@runtime_checkable
+class MapCompletionCallback(t.Protocol):
+    def __call__(self, completions: list[Completion]) -> list[Completion]:
+        """
+        Passed a finalized completion to process. Can replace completions in the pipeline by returning
+        a new completion object.
+        """
+        ...
+
+
+@runtime_checkable
+class AsyncMapCompletionCallback(t.Protocol):
+    async def __call__(self, completions: list[Completion]) -> list[Completion]:
+        """
+        async variant of the [rigging.completion.MapCompletionCallback][] protocol.
+        """
+        ...
+
+
+ThenCompletionCallbacks = ThenCompletionCallback | AsyncThenCompletionCallback
+MapCompletionCallbacks = MapCompletionCallback | AsyncMapCompletionCallback
 
 
 @dataclass
 class RunState:
     text: str
     params: "GenerateParams"
     processor: t.Generator[None, str, str]
@@ -168,15 +236,19 @@
         """The parameters for generating the completion."""
         self.metadata: dict[str, t.Any] = {}
         """Additional metadata associated with the completion."""
 
         # (callback, all_text, max_rounds)
         self.until_callbacks: list[tuple[UntilCompletionCallback, bool, int]] = []
         self.until_types: list[type[Model]] = []
-        self.then_callbacks: list[ThenCompletionCallback] = []
+        self.then_callbacks: list[ThenCompletionCallbacks] = []
+        self.map_callbacks: list[MapCompletionCallbacks] = []
+
+    def __len__(self) -> int:
+        return len(self.text)
 
     def with_(self, params: t.Optional["GenerateParams"] = None, **kwargs: t.Any) -> "PendingCompletion":
         """
         Assign specific generation parameter overloads for this completion.
 
         Note:
             This will trigger a `clone` if overload params have already been set.
@@ -184,51 +256,77 @@
         Args:
             params: The parameters to set for the completion.
             **kwargs: An alternative way to pass parameters as keyword arguments.
 
         Returns:
             The current (or cloned) instance of the completion.
         """
-        from rigging.generator import GenerateParams
-
         if params is None:
             params = GenerateParams(**kwargs)
 
         if self.params is not None:
             new = self.clone()
-            new.params = params
+            new.params = self.params.merge_with(params)
             return new
 
         self.params = params
         return self
 
     def then(self, callback: ThenCompletionCallback) -> "PendingCompletion":
         """
         Registers a callback to be executed after the generation process completes.
 
         Note:
             Returning a Completion object from the callback will replace the current completion.
             for the remainder of the callbacks + return value of `run()`.
 
         ```
-        def process(chat: Completion) -> Completion | None:
+        def process(completion: Completion) -> Completion | None:
             ...
 
         pending.then(process).run()
         ```
 
         Args:
             callback: The callback function to be executed.
 
         Returns:
             The current instance of the pending completion.
         """
         self.then_callbacks.append(callback)
         return self
 
+    def map(self, callback: MapCompletionCallback | AsyncMapCompletionCallback) -> "PendingCompletion":
+        """
+        Registers a callback to be executed after the generation process completes.
+
+        Note:
+            You must return a list of completion objects from the callback which will
+            represent the state of completions for the remainder of the callbacks and return.
+
+        Warning:
+            If you implement an async callback, you must use the async variant of the
+            run methods when executing the generation process.
+
+        ```
+        def process(completions: list[Completion]) -> list[Completion]:
+            ...
+
+        pending.map(process).run()
+        ```
+
+        Args:
+            callback: The callback function to be executed.
+
+        Returns:
+            The current instance of the completion.
+        """
+        self.map_callbacks.append(callback)
+        return self
+
     def add(self, text: str) -> "PendingCompletion":
         """
         Appends new text to the internal text before generation.
 
         Args:
             text: The text to be added to the completion.
 
@@ -284,14 +382,17 @@
         self.metadata.update(kwargs)
         return self
 
     def apply(self, **kwargs: str) -> "PendingCompletion":
         """
         Applies keyword arguments to the text using string template substitution.
 
+        Note:
+            This produces a clone of the PendingCompletion, leaving the original unchanged.
+
         Args:
             **kwargs: Keyword arguments to be applied to the text.
 
         Returns:
             A new instance of PendingCompletion with the applied arguments.
         """
         new = self.clone()
@@ -305,15 +406,15 @@
         *,
         use_all_text: bool = False,
         max_rounds: int = DEFAULT_MAX_ROUNDS,
     ) -> "PendingCompletion":
         """
         Registers a callback to participate in validating the generation process.
 
-        ```python
+        ```py
         # Takes the generated text, and returns whether or not to retry generation.
 
         def callback(text: str) -> bool:
             if is_valid(text):
                 return False
             else:
                 return True
@@ -363,25 +464,53 @@
     def _until_parse_callback(self, text: str) -> bool:
         try:
             parse_many(text, *self.until_types)
         except Exception:
             return True
         return False
 
-    def _then(self, chat: Completion) -> Completion:
-        # TODO: Adding async support here would be nice
-        for callback in self.then_callbacks:
-            chat = callback(chat) or chat
-        return chat
+    def _post_run(self, completions: list[Completion]) -> list[Completion]:
+        for map_callback in self.map_callbacks:
+            if asyncio.iscoroutinefunction(map_callback):
+                raise ValueError(
+                    f"Cannot use async map() callbacks inside a non-async run call: {map_callback.__name__}"
+                )
+            completions = map_callback(completions)  # type: ignore
+
+        for then_callback in self.then_callbacks:
+            if asyncio.iscoroutinefunction(then_callback):
+                raise ValueError(
+                    f"Cannot use async then() callbacks inside a non-async run call: {then_callback.__name__}"
+                )
+            updated = [then_callback(completion) for completion in completions]
+            completions = [updated[i] or completion for i, completion in enumerate(completions)]  # type: ignore
+
+        return completions
+
+    async def _apost_run(self, completions: list[Completion]) -> list[Completion]:
+        for map_callback in self.map_callbacks:
+            if not asyncio.iscoroutinefunction(map_callback):
+                raise ValueError(
+                    f"Cannot use non-async map() callbacks inside an async run call: {map_callback.__call__.__name__}"
+                )
+            completions = await map_callback(completions)
+
+        for then_callback in self.then_callbacks:
+            if not asyncio.iscoroutinefunction(then_callback):
+                raise ValueError(
+                    f"Cannot use non-async then() callbacks inside an async run call: {then_callback.__call__.__name__}"
+                )
+            updated = [await then_callback(completion) for completion in completions]
+            completions = [updated[i] or completion for i, completion in enumerate(completions)]
+
+        return completions
 
     def _fit_params(
         self, count: int, params: t.Sequence[t.Optional["GenerateParams"] | None] | None = None
     ) -> list["GenerateParams"]:
-        from rigging.generator import GenerateParams
-
         params = [None] * count if params is None else list(params)
         if len(params) != count:
             raise ValueError(f"The number of params must be {count}")
         if self.params is not None:
             params = [self.params.merge_with(p) for p in params]
         return [(p or GenerateParams()) for p in params]
 
@@ -423,15 +552,15 @@
 
         Returns:
             The generated Completion.
         """
         return self.run_many(1)[0]
 
     async def arun(self) -> Completion:
-        """async variant of the [rigging.chat.PendingChat.run][] method."""
+        """async variant of the [rigging.completion.PendingCompletion.run][] method."""
         return (await self.arun_many(1))[0]
 
     __call__ = run
 
     # Many messages
 
     def run_many(
@@ -463,24 +592,28 @@
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
-                        self.text, t.cast(str, stop.value), pending=self, metadata=self.metadata
+                        self.text,
+                        t.cast(str, stop.value),
+                        generator=self.generator,
+                        params=state.params,
+                        metadata=self.metadata,
                     )
                 except ExhaustedMaxRoundsError:
                     if not skip_failed:
                         raise
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
-        return [self._then(s.completion) for s in states if s.completion is not None]
+        return self._post_run([s.completion for s in states if s.completion is not None])
 
     async def arun_many(
         self,
         count: int,
         *,
         params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
         skip_failed: bool = False,
@@ -497,24 +630,28 @@
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
-                        self.text, t.cast(str, stop.value), pending=self, metadata=self.metadata
+                        self.text,
+                        t.cast(str, stop.value),
+                        generator=self.generator,
+                        params=state.params,
+                        metadata=self.metadata,
                     )
                 except ExhaustedMaxRoundsError:
                     if not skip_failed:
                         raise
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
-        return [self._then(s.completion) for s in states if s.completion is not None]
+        return self._post_run([s.completion for s in states if s.completion is not None])
 
     # Batch completions
 
     def run_batch(
         self,
         many: t.Sequence[str],
         params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
@@ -550,33 +687,37 @@
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
-                        self.text, t.cast(str, stop.value), pending=self, metadata=self.metadata
+                        self.text,
+                        t.cast(str, stop.value),
+                        generator=self.generator,
+                        params=state.params,
+                        metadata=self.metadata,
                     )
                 except ExhaustedMaxRoundsError:
                     if not skip_failed:
                         raise
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
-        return [self._then(s.completion) for s in states if s.completion is not None]
+        return self._post_run([s.completion for s in states if s.completion is not None])
 
     async def arun_batch(
         self,
         many: t.Sequence[str],
         params: t.Sequence[t.Optional["GenerateParams"]] | None = None,
         *,
         skip_failed: bool = False,
     ) -> list[Completion]:
-        """async variant of the [rigging.chat.PendingChat.run_batch][] method."""
+        """async variant of the [rigging.completion.PendingCompletion.run_batch][] method."""
         params = self._fit_params(len(many), params)
         states: list[RunState] = [RunState(m, p, self._process()) for m, p in zip(many, params, strict=True)]
         _ = [next(state.processor) for state in states]
 
         pending_states = states
         while pending_states:
             inbounds = await self.generator.agenerate_texts(
@@ -587,17 +728,21 @@
 
             for inbound, state in zip(inbounds, pending_states, strict=True):
                 try:
                     state.processor.send(inbound)
                 except StopIteration as stop:
                     state.done = True
                     state.completion = Completion(
-                        self.text, t.cast(str, stop.value), pending=self, metadata=self.metadata
+                        self.text,
+                        t.cast(str, stop.value),
+                        generator=self.generator,
+                        params=state.params,
+                        metadata=self.metadata,
                     )
                 except ExhaustedMaxRoundsError:
                     if not skip_failed:
                         raise
                     state.done = True
 
             pending_states = [s for s in pending_states if not s.done]
 
-        return [self._then(s.completion) for s in states if s.completion is not None]
+        return self._post_run([s.completion for s in states if s.completion is not None])
```

### Comparing `rigging-1.0.0rc0/rigging/error.py` & `rigging-1.0.1/rigging/error.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.0rc0/rigging/generator.py` & `rigging-1.0.1/rigging/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 import asyncio
 import typing as t
 
 import litellm  # type: ignore
 from loguru import logger
 from pydantic import BaseModel, ConfigDict, Field, field_validator
 
-from rigging.chat import Chat, PendingChat
-from rigging.completion import Completion, PendingCompletion
 from rigging.error import InvalidModelSpecifiedError
 from rigging.message import (
     Message,
     MessageDict,
 )
 
+if t.TYPE_CHECKING:
+    from rigging.chat import PendingChat
+    from rigging.completion import PendingCompletion
+
 # We should probably let people configure
 # this independently, but for now we'll
 # fix it to prevent confusion
 litellm.drop_params = True
 
 # Global provider map
 g_providers: dict[str, type["Generator"]] = {}
@@ -235,81 +237,85 @@
     # params seem odd, but mypy doesn't like the TypedDict in a list otherwise
 
     @t.overload
     def chat(
         self,
         messages: t.Sequence[MessageDict],
         params: GenerateParams | None = None,
-    ) -> PendingChat:
+    ) -> "PendingChat":
         ...
 
     @t.overload
     def chat(
         self,
         messages: t.Sequence[Message] | MessageDict | Message | str | None = None,
         params: GenerateParams | None = None,
-    ) -> PendingChat:
+    ) -> "PendingChat":
         ...
 
     def chat(
         self,
         messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str | None = None,
         params: GenerateParams | None = None,
-    ) -> PendingChat:
+    ) -> "PendingChat":
         """
         Build a pending chat with the given messages and optional params overloads.
 
         Args:
             messages: The messages to be sent in the chat.
             params: Optional parameters for generating responses.
 
         Returns:
             Pending chat to run.
         """
+        from rigging.chat import PendingChat
+
         return PendingChat(self, Message.fit_as_list(messages) if messages else [], params)
 
     # Helper alternative to complete(generator) -> generator.complete(...)
 
-    def complete(self, text: str, params: GenerateParams | None = None) -> PendingCompletion:
+    def complete(self, text: str, params: GenerateParams | None = None) -> "PendingCompletion":
         """
         Build a pending string completion of the given text with optional param overloads.
 
         Args:
             text: The input text to be completed.
             params: The parameters to be used for completion.
 
         Returns:
             The completed text.
         """
+        from rigging.completion import PendingCompletion
+
         return PendingCompletion(self, text, params)
 
 
 @t.overload
 def chat(
     generator: "Generator",
     messages: t.Sequence[MessageDict],
     params: GenerateParams | None = None,
-) -> PendingChat:
+) -> "PendingChat":
     ...
 
 
 @t.overload
 def chat(
     generator: "Generator",
     messages: t.Sequence[Message] | MessageDict | Message | str | None = None,
     params: GenerateParams | None = None,
-) -> PendingChat:
+) -> "PendingChat":
     ...
 
 
 def chat(
     generator: "Generator",
     messages: t.Sequence[MessageDict] | t.Sequence[Message] | MessageDict | Message | str | None = None,
     params: GenerateParams | None = None,
-) -> PendingChat:
+) -> "PendingChat":
     """
     Creates a pending chat using the given generator, messages, and params.
 
     Args:
         generator: The generator to use for creating the chat.
         messages:
             The messages to include in the chat. Can be a single message or a sequence of messages.
@@ -321,15 +327,15 @@
     return generator.chat(messages, params)
 
 
 def complete(
     generator: Generator,
     text: str,
     params: GenerateParams | None = None,
-) -> PendingCompletion:
+) -> "PendingCompletion":
     return generator.complete(text, params)
 
 
 def get_identifier(generator: Generator, params: GenerateParams | None = None) -> str:
     """
     Converts the generator instance back into a rigging identifier string.
 
@@ -584,13 +590,7 @@
             trace_str(text, f"Text {i+1}/{len(texts)}")
             trace_str(response, f"Generated {i+1}/{len(texts)}")
 
         return generated
 
 
 g_providers["litellm"] = LiteLLMGenerator
-
-# TODO: This fixes some almost-circular import issues and
-# typed forwardrefs we use in the other module
-
-Chat.model_rebuild()
-Completion.model_rebuild()
```

### Comparing `rigging-1.0.0rc0/rigging/logging.py` & `rigging-1.0.1/rigging/logging.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 """
-We use loguru for logging. This module provides a function to configure the logging settings.
+We use loguru for logging. This module provides a function to configure logging handlers.
 
-To enable rigging logging, call `logger.enable("rigging")` after importing the module.
+To just enable rigging logs to flow, call `logger.enable("rigging")` after importing the module.
 """
 
 import pathlib
 import sys
 import typing as t
 
 from loguru import logger
 
 g_configured: bool = False
 
 LogLevelList = ["trace", "debug", "info", "success", "warning", "error", "critical"]
 LogLevelLiteral = t.Literal["trace", "debug", "info", "success", "warning", "error", "critical"]
+"""Valid logging levels."""
 
 
 def configure_logging(
-    log_level: str,
+    log_level: LogLevelLiteral,
     log_file: pathlib.Path | None = None,
     log_file_level: LogLevelLiteral = "debug",
 ) -> None:
     """
-    Configures the loguru settings for the rigging module.
-
-    This is optional, and calling `logger.enable("rigging")` will enable the logging
-    and you can control the formatting and log levels using the loguru API.
+    Configures common loguru handlers.
 
     Args:
-        log_level: The desired log level. Valid values are 'TRACE', 'DEBUG', 'INFO',
-            'SUCCESS', 'WARNING', 'ERROR', and 'CRITICAL'.
+        log_level: The desired log level.
         log_file: The path to the log file. If None, logging
             will only be done to the console.
-        log_file_level: The log level for the log file. Valid values
-            are 'TRACE', 'DEBUG', 'INFO', 'SUCCESS', 'WARNING', 'ERROR', and 'CRITICAL'.
+        log_file_level: The log level for the log file.
     """
     global g_configured
 
     if g_configured:
         return
 
     logger.enable("rigging")
@@ -46,19 +42,14 @@
     logger.level("DEBUG", color="<blue>", icon="[_]")
     logger.level("INFO", color="<cyan>", icon="[=]")
     logger.level("SUCCESS", color="<green>", icon="[+]")
     logger.level("WARNING", color="<yellow>", icon="[-]")
     logger.level("ERROR", color="<red>", icon="[!]")
     logger.level("CRITICAL", color="<RED>", icon="[x]")
 
-    # Default format:
-    # "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
-    # "<level>{level: <8}</level> | "
-    # "<cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>",
-
     custom_format = "<green>{time:HH:mm:ss.SSS}</green> | <level>{level.icon}</level> {message}"
 
     logger.remove()
     logger.add(sys.stderr, format=custom_format, level=log_level.upper())
 
     if log_file is not None:
         logger.add(log_file, format=custom_format, level=log_file_level.upper())
```

### Comparing `rigging-1.0.0rc0/rigging/message.py` & `rigging-1.0.1/rigging/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 This module covers core message objects and handling.
 """
 
+import copy
 import string
 import typing as t
+from uuid import UUID, uuid4
 
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     FieldSerializationInfo,
     SerializeAsAny,
@@ -66,28 +68,50 @@
 
 
 class Message(BaseModel):
     """
     Represents a message with role, content, and parsed message parts.
     """
 
+    uuid: UUID = Field(default_factory=uuid4, repr=False)
+    """The unique identifier for the message."""
     role: Role
     """The role of the message."""
     parts: list[ParsedMessagePart] = Field(default_factory=list)
     """The parsed message parts."""
 
     _content: str = ""
 
-    def __init__(self, role: Role, content: str, parts: t.Sequence[ParsedMessagePart] | None = None):
-        super().__init__(role=role, parts=parts if parts is not None else [])
+    def __init__(self, role: Role, content: str, parts: t.Sequence[ParsedMessagePart] | None = None, **kwargs: t.Any):
+        super().__init__(role=role, parts=parts or [], **kwargs)
         self._content = content
 
     def __str__(self) -> str:
         return f"[{self.role}]: {self.content}"
 
+    @computed_field  # type: ignore[misc]
+    @property
+    def content(self) -> str:
+        """The content of the message."""
+        # We used to sync the models and content each time it was accessed,
+        # hence the getter. Now we just return the stored content.
+        # I'll leave it as is for now in case we want to add any
+        # logic here in the future.
+        return self._content
+
+    @content.setter
+    def content(self, value: str) -> None:
+        # TODO: Maintain any parsed parts which are
+        # still in the content - our move to slices for
+        # tracking parsed parts makes this more complicated
+        # so fow now I've opted to strip all parts
+        # when content is changed.
+        self.parts = []
+        self._content = value
+
     # TODO: In general the add/remove/sync_part methods are
     # overly complicated. We should probably just update content,
     # then reparse all the models to get their fresh slices.
     #
     # I don't like all this manual slice recalculation logic, seems brittle.
 
     def _remove_part(self, part: ParsedMessagePart) -> str:
@@ -113,16 +137,14 @@
         self.parts.append(part)
 
     # Looks more complicated than it is. We just want to clean all the models
     # in the message content by re-serializing them. As we do so, we'll need
     # to watch for the total size of our message shifting and update the slices
     # of the following parts accordingly. In other words, as A expands, B which
     # follows will have a new start slice and end slice.
-    #
-    # TODO: We should probably just re-trigger parsing for everything
     def _sync_parts(self) -> None:
         self.parts = sorted(self.parts, key=lambda p: p.slice_.start)
 
         shift = 0
         for part in self.parts:
             existing = self._content[part.slice_]
 
@@ -141,45 +163,34 @@
             self._content = self._content[: part.slice_.start] + xml_content + self._content[part.slice_.stop :]
             part.slice_ = slice(part.slice_.start, part.slice_.start + new_length)
 
             shift += new_length - old_length
 
         self.parts = sorted(self.parts, key=lambda p: p.slice_.start)
 
-    @computed_field  # type: ignore[misc]
-    @property
-    def content(self) -> str:
-        """The content of the message."""
-        # We used to sync the models and content each time it was accessed,
-        # hence the getter. Now we just return the stored content.
-        # I'll leave it as is for now in case we want to add any
-        # logic here in the future.
-        return self._content
+    def clone(self) -> "Message":
+        """Creates a copy of the message."""
+        return Message(self.role, self.content, parts=copy.deepcopy(self.parts))
 
-    @content.setter
-    def content(self, value: str) -> None:
-        # TODO: Maintain any parsed parts which are
-        # still in the content - our move to slices for
-        # tracking parsed parts makes this more complicated
-        # so fow now I've opted to strip all parts
-        # when content is changed.
-        self.parts = []
-        self._content = value
-
-    def apply(self, **kwargs: str) -> None:
+    def apply(self, **kwargs: str) -> "Message":
         """
         Applies the given keyword arguments with string templating to the content of the message.
 
         Uses [string.Template.safe_substitute](https://docs.python.org/3/library/string.html#string.Template.safe_substitute) underneath.
 
+        Note:
+            This call produces a clone of the message, leaving the original message unchanged.
+
         Args:
             **kwargs: Keyword arguments to substitute in the message content.
         """
-        template = string.Template(self.content)
-        self.content = template.safe_substitute(**kwargs)
+        new = self.clone()
+        template = string.Template(new.content)
+        new.content = template.safe_substitute(**kwargs)
+        return new
 
     def strip(self, model_type: type[Model], *, fail_on_missing: bool = False) -> list[ParsedMessagePart]:
         """
         Removes and returns a list of ParsedMessagePart objects from the message that match the specified model type.
 
         Args:
             model_type: The type of model to match.
@@ -352,9 +363,14 @@
     @classmethod
     def fit(cls, message: t.Union["Message", MessageDict, str]) -> "Message":
         """Helper function to convert various common types to a Message object."""
         if isinstance(message, str):
             return cls(role="user", content=message)
         return cls(**message) if isinstance(message, dict) else message
 
+    @classmethod
+    def apply_to_list(cls, messages: t.Sequence["Message"], **kwargs: str) -> list["Message"]:
+        """Helper function to apply keyword arguments to a list of Message objects."""
+        return [message.apply(**kwargs) for message in messages]
+
 
 Messages = t.Sequence[MessageDict] | t.Sequence[Message]
```

### Comparing `rigging-1.0.0rc0/rigging/model.py` & `rigging-1.0.1/rigging/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,28 @@
         # is handled internally, so we'll override it here so we
         # can always assume __xml_tag__ is set to a sane default.
         #
         # Some models appear to do better if the separator is a dash
         # instead of a underscore, and users are free to override
         # as needed.
         super().__init_subclass__(tag, ns, nsmap, ns_attrs, skip_empty, search_mode, **kwargs)
-        cls.__xml_tag__ = XmlTagDescriptor()  # type: ignore [assignment]
+        cls.__xml_tag__ = tag or XmlTagDescriptor()  # type: ignore [assignment]
 
     # to_xml() doesn't prettify normally, and extended
     # requirements like lxml seemed like poor form for
     # just this feature
     def to_pretty_xml(self) -> str:
         """
         Converts the model to a pretty XML string with indents and newlines.
 
         Returns:
             The pretty XML representation of the model.
         """
         tree = self.to_xml_tree()
-        ET.indent(tree, "   ")
+        ET.indent(tree, "  ")
         pretty_encoded_xml = ET.tostring(tree).decode()
 
         if self.__class__.is_simple():
             return unescape_xml(pretty_encoded_xml)
         else:
             return pretty_encoded_xml
 
@@ -270,19 +270,19 @@
     @field_validator("content", mode="before")
     def parse_exception(cls, value: t.Any) -> t.Any:
         if isinstance(value, Exception):
             return str(value)
         return value
 
 
-class SystemErrorModel(ErrorModel, tag="system_error"):
+class SystemErrorModel(ErrorModel, tag="system-error"):
     content: str
 
 
-class ValidationErrorModel(ErrorModel, tag="validation_error"):
+class ValidationErrorModel(ErrorModel, tag="validation-error"):
     content: str
 
 
 # Common structured helpers
 
 
 class Thinking(Model):
```

### Comparing `rigging-1.0.0rc0/rigging/parsing.py` & `rigging-1.0.1/rigging/parsing.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.0rc0/rigging/prompt.py` & `rigging-1.0.1/rigging/prompt.py`

 * *Files identical despite different names*

### Comparing `rigging-1.0.0rc0/rigging/tool.py` & `rigging-1.0.1/rigging/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 
 from pydantic import Field, computed_field, model_validator
 from pydantic_xml import attr, element, wrapped
 
 from rigging.model import Model
 
 SUPPORTED_TOOL_ARGUMENT_TYPES = int | float | str | bool
+"""Supported types for tool arguments."""
+
+SUPPORTED_TOOL_ARGUMENT_TYPES_LIST = [int, float, str, bool]
+"""Supported types for tool arguments as a list."""
+
 ToolArgumentTypesCast = {
     "int": int,
     "float": float,
     "bool": bool,
     "str": str,
 }
 
@@ -25,15 +30,16 @@
 
 
 class ToolCallParameter(Model):
     name: str = attr()
     attr_value: SUPPORTED_TOOL_ARGUMENT_TYPES | None = attr("value", default=None, exclude=True)
     text_value: SUPPORTED_TOOL_ARGUMENT_TYPES | None = Field(default=None, exclude=True)
 
-    @computed_field
+    @computed_field  # type: ignore[misc]
+    @property
     def value(self) -> SUPPORTED_TOOL_ARGUMENT_TYPES:
         return self.attr_value or self.text_value or ""
 
     @model_validator(mode="after")
     def validate_value(self) -> "ToolCallParameter":
         if self.value is None:
             raise ValueError("Missing parameter value")
@@ -130,15 +136,15 @@
 
 class Tool:
     """
     Base class for implementing tools in the Rigging system.
 
     You should subclass this to define your own tools:
 
-    ```python
+    ```py
     def Hammer(Tool):
         name = "Hammer"
         description = "A tool for hitting things."
 
         def hit(self, target: Annotated[str, "Target of the hit") -> str:
             return f"Hit {target} with a hammer."
 
@@ -266,16 +272,18 @@
                 annotation_args = t.get_args(param.annotation)
 
                 if len(annotation_args) != 2 or not isinstance(annotation_args[1], str):
                     raise TypeError(
                         f'Parameters must be annotated like Annotated[<type>, "<description>"] ({formatted_name})'
                     )
 
-                if annotation_args[0] not in SUPPORTED_TOOL_ARGUMENT_TYPES.__args__:  # type: ignore
-                    raise TypeError(f"Parameters must be annotated with supported types ({formatted_name})")
+                if annotation_args[0] not in SUPPORTED_TOOL_ARGUMENT_TYPES_LIST:
+                    raise TypeError(
+                        f"Parameters must be annotated with one of these types: {SUPPORTED_TOOL_ARGUMENT_TYPES_LIST} ({formatted_name})"
+                    )
 
                 type_name = annotation_args[0].__name__
                 description = annotation_args[1]
 
                 parameters.append(ToolParameter(name=param_name, type=type_name, description=description))
 
             functions.append(
```

### Comparing `rigging-1.0.0rc0/PKG-INFO` & `rigging-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rigging
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: LLM Interaction Framework
 Home-page: https://github.com/dreadnode/rigging
 License: MIT
 Author: Nick Landers
 Author-email: monoxgas@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: litellm (==1.35.21)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
+Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pydantic (==2.5.3)
 Requires-Dist: pydantic-xml (==2.7.0)
 Project-URL: Repository, https://github.com/dreadnode/rigging
 Description-Content-Type: text/markdown
 
 # Rigging
 
@@ -30,15 +31,15 @@
 - Chat templating, forking, continuations, generation parameter overloads, stripping segments, etc.
 - Modern python with type hints, async support, pydantic validation, serialization, etc.
 
 ```py
 import rigging as rg
 from rigging.model import CommaDelimitedAnswer as Answer
 
-answer = rg.get_generator('gpt-4') \
+chat = rg.get_generator('gpt-4') \
     .chat(f"Give me 3 famous authors between {Answer.xml_tags()} tags.") \
     .until_parsed_as(Answer) \
     .run()
 
 answer = chat.last.parse(Answer)
 print(answer.items)
 
@@ -57,8 +58,8 @@
 ```bash
 cd rigging/
 poetry install
 ```
 
 ## Getting Started
 
-Head over to **[our documentation](https://rigging.dreadnode.io) for more information.
+Head over to **[our documentation](https://rigging.dreadnode.io)** for more information.
```

