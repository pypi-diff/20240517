# Comparing `tmp/promplate-0.3.4.5.tar.gz` & `tmp/promplate-0.3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate-0.3.4.5.tar", max compression
+gzip compressed data, was "promplate-0.3.4.6.tar", max compression
```

## Comparing `promplate-0.3.4.5.tar` & `promplate-0.3.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4.5/promplate/__init__.py
--rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4.5/promplate/chain/__init__.py
--rw-r--r--   0        0        0     2309 2024-05-15 23:19:13.328395 promplate-0.3.4.5/promplate/chain/callback.py
--rw-r--r--   0        0        0    17376 2024-05-15 23:19:13.328935 promplate-0.3.4.5/promplate/chain/node.py
--rw-r--r--   0        0        0     1320 2024-05-15 23:19:41.867068 promplate-0.3.4.5/promplate/chain/utils.py
--rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4.5/promplate/llm/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-15 23:19:13.329466 promplate-0.3.4.5/promplate/llm/base.py
--rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4.5/promplate/llm/openai/__init__.py
--rw-r--r--   0        0        0     4125 2024-05-15 23:19:13.330001 promplate-0.3.4.5/promplate/llm/openai/v0.py
--rw-r--r--   0        0        0     6002 2024-05-15 23:19:13.330001 promplate-0.3.4.5/promplate/llm/openai/v1.py
--rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4.5/promplate/prompt/__init__.py
--rw-r--r--   0        0        0     1633 2024-04-15 04:14:57.538290 promplate-0.3.4.5/promplate/prompt/builder.py
--rw-r--r--   0        0        0     3216 2024-05-15 23:19:13.330534 promplate-0.3.4.5/promplate/prompt/chat.py
--rw-r--r--   0        0        0     7362 2024-05-15 23:19:13.331068 promplate-0.3.4.5/promplate/prompt/template.py
--rw-r--r--   0        0        0     3285 2024-05-15 23:19:13.331068 promplate-0.3.4.5/promplate/prompt/utils.py
--rw-r--r--   0        0        0     1600 2024-05-15 23:19:47.396575 promplate-0.3.4.5/pyproject.toml
--rw-r--r--   0        0        0     1995 2024-04-15 04:14:57.536290 promplate-0.3.4.5/README.md
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 promplate-0.3.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1926 2024-05-17 19:21:07.427084 promplate-0.3.4.6/README.md
+-rw-r--r--   0        0        0       43 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/__init__.py
+-rw-r--r--   0        0        0     2250 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/callback.py
+-rw-r--r--   0        0        0    16908 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/node.py
+-rw-r--r--   0        0        0     1273 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/chain/utils.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/__init__.py
+-rw-r--r--   0        0        0     1007 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/base.py
+-rw-r--r--   0        0        0      114 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4007 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/openai/v0.py
+-rw-r--r--   0        0        0     5818 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/llm/openai/v1.py
+-rw-r--r--   0        0        0       85 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/__init__.py
+-rw-r--r--   0        0        0     1577 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/builder.py
+-rw-r--r--   0        0        0     3108 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/chat.py
+-rw-r--r--   0        0        0     7920 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/template.py
+-rw-r--r--   0        0        0     3680 2024-05-17 19:21:07.427084 promplate-0.3.4.6/promplate/prompt/utils.py
+-rw-r--r--   0        0        0     1538 2024-05-17 19:21:07.427084 promplate-0.3.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3188 1970-01-01 00:00:00.000000 promplate-0.3.4.6/PKG-INFO
```

### Comparing `promplate-0.3.4.5/promplate/chain/callback.py` & `promplate-0.3.4.6/promplate/chain/callback.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from typing import TYPE_CHECKING, Awaitable, Callable, Protocol
-
-from ..prompt import Context
-
-if TYPE_CHECKING:
-    from .node import AsyncProcess, ChainContext, Interruptable, Process
-
-
-class BaseCallback(Protocol):
-    def pre_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
-
-    def mid_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
-
-    def end_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
-
-    def on_enter(self, node: "Interruptable", context: Context | None, config: Context) -> tuple[Context | None, Context]:
-        return context, config
-
-    def on_leave(self, node: "Interruptable", context: "ChainContext", config: Context) -> tuple["ChainContext", Context]:
-        return context, config
-
-
-class Callback(BaseCallback):
-    def __init__(
-        self,
-        *,
-        pre_process: "Process | AsyncProcess | None" = None,
-        mid_process: "Process | AsyncProcess | None" = None,
-        end_process: "Process | AsyncProcess | None" = None,
-        on_enter: Callable[["Interruptable", Context | None, Context], tuple[Context | None, Context]] | None = None,
-        on_leave: Callable[["Interruptable", "ChainContext", Context], tuple["ChainContext", Context]] | None = None,
-    ):
-        self._pre_process = pre_process
-        self._mid_process = mid_process
-        self._end_process = end_process
-        self._on_enter = on_enter
-        self._on_leave = on_leave
-
-    def pre_process(self, context):
-        if self._pre_process is not None:
-            return self._pre_process(context)
-
-    def mid_process(self, context):
-        if self._mid_process is not None:
-            return self._mid_process(context)
-
-    def end_process(self, context):
-        if self._end_process is not None:
-            return self._end_process(context)
-
-    def on_enter(self, node, context, config):
-        if self._on_enter is not None:
-            return self._on_enter(node, context, config)
-        return context, config
-
-    def on_leave(self, node, context, config):
-        if self._on_leave is not None:
-            return self._on_leave(node, context, config)
-        return context, config
+from typing import TYPE_CHECKING, Awaitable, Callable, Protocol
+
+from ..prompt import Context
+
+if TYPE_CHECKING:
+    from .node import AsyncProcess, ChainContext, Interruptable, Process
+
+
+class BaseCallback(Protocol):
+    def pre_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
+
+    def mid_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
+
+    def end_process(self, context: "ChainContext") -> Context | Awaitable[Context | None] | None: ...
+
+    def on_enter(self, node: "Interruptable", context: Context | None, config: Context) -> tuple[Context | None, Context]:
+        return context, config
+
+    def on_leave(self, node: "Interruptable", context: "ChainContext", config: Context) -> tuple["ChainContext", Context]:
+        return context, config
+
+
+class Callback(BaseCallback):
+    def __init__(
+        self,
+        *,
+        pre_process: "Process | AsyncProcess | None" = None,
+        mid_process: "Process | AsyncProcess | None" = None,
+        end_process: "Process | AsyncProcess | None" = None,
+        on_enter: Callable[["Interruptable", Context | None, Context], tuple[Context | None, Context]] | None = None,
+        on_leave: Callable[["Interruptable", "ChainContext", Context], tuple["ChainContext", Context]] | None = None,
+    ):
+        self._pre_process = pre_process
+        self._mid_process = mid_process
+        self._end_process = end_process
+        self._on_enter = on_enter
+        self._on_leave = on_leave
+
+    def pre_process(self, context):
+        if self._pre_process is not None:
+            return self._pre_process(context)
+
+    def mid_process(self, context):
+        if self._mid_process is not None:
+            return self._mid_process(context)
+
+    def end_process(self, context):
+        if self._end_process is not None:
+            return self._end_process(context)
+
+    def on_enter(self, node, context, config):
+        if self._on_enter is not None:
+            return self._on_enter(node, context, config)
+        return context, config
+
+    def on_leave(self, node, context, config):
+        if self._on_leave is not None:
+            return self._on_leave(node, context, config)
+        return context, config
```

### Comparing `promplate-0.3.4.5/promplate/chain/node.py` & `promplate-0.3.4.6/promplate/chain/node.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,468 +1,468 @@
-from inspect import isclass
-from itertools import accumulate
-from typing import Callable, Mapping, MutableMapping, overload
-
-from ..llm.base import *
-from ..prompt.template import Context, Loader, SafeChainMapContext, Template
-from .callback import BaseCallback, Callback
-from .utils import accumulate_any, resolve
-
-
-class ChainContext(SafeChainMapContext):
-    @overload
-    def __init__(self): ...
-
-    @overload
-    def __init__(self, least: MutableMapping | None = None): ...
-
-    @overload
-    def __init__(self, least: MutableMapping | None = None, *maps: Mapping): ...
-
-    def __init__(self, least: MutableMapping | None = None, *maps: Mapping):
-        super().__init__({} if least is None else least, *maps)  # type: ignore
-
-    @classmethod
-    def ensure(cls, context):
-        return context if isinstance(context, cls) else cls(context)
-
-    @property
-    def result(self):
-        return self.__getitem__("__result__")
-
-    @result.setter
-    def result(self, result):
-        self.__setitem__("__result__", result)
-
-    @result.deleter
-    def result(self):
-        self.__delitem__("__result__")
-
-    def __str__(self):
-        return str({**self})
-
-
-Process = Callable[[ChainContext], Context | None]
-
-AsyncProcess = Callable[[ChainContext], Awaitable[Context | None]]
-
-
-class AbstractNode(Protocol):
-    def invoke(
-        self,
-        context: Context | None = None,
-        /,
-        complete: Complete | None = None,
-        **config,
-    ) -> ChainContext: ...
-
-    async def ainvoke(
-        self,
-        context: Context | None = None,
-        /,
-        complete: Complete | AsyncComplete | None = None,
-        **config,
-    ) -> ChainContext: ...
-
-    def stream(
-        self,
-        context: Context | None = None,
-        /,
-        generate: Generate | None = None,
-        **config,
-    ) -> Iterable[ChainContext]: ...
-
-    def astream(
-        self,
-        context: Context | None = None,
-        /,
-        generate: Generate | AsyncGenerate | None = None,
-        **config,
-    ) -> AsyncIterable[ChainContext]: ...
-
-    @classmethod
-    def _get_chain_type(cls):
-        return Chain
-
-    def __add__(self, chain: "AbstractNode"):
-        if isinstance(chain, Chain):
-            return self._get_chain_type()(self, *chain)
-        return self._get_chain_type()(self, chain)
-
-
-def ensure_callbacks(callbacks: list[BaseCallback | type[BaseCallback]]) -> list[BaseCallback]:
-    return [i() if isclass(i) else i for i in callbacks]
-
-
-class Interruptable(AbstractNode, Protocol):
-    def _invoke(
-        self,
-        context: ChainContext,
-        /,
-        complete: Complete | None,
-        callbacks: list[BaseCallback],
-        **config,
-    ): ...
-
-    async def _ainvoke(
-        self,
-        context: ChainContext,
-        /,
-        complete: Complete | AsyncComplete | None,
-        callbacks: list[BaseCallback],
-        **config,
-    ): ...
-
-    def _stream(
-        self,
-        context: ChainContext,
-        /,
-        generate: Generate | None,
-        callbacks: list[BaseCallback],
-        **config,
-    ) -> Iterable: ...
-
-    def _astream(
-        self,
-        context: ChainContext,
-        /,
-        generate: Generate | AsyncGenerate | None,
-        callbacks: list[BaseCallback],
-        **config,
-    ) -> AsyncIterable: ...
-
-    callbacks: list[BaseCallback | type[BaseCallback]]
-
-    def enter(self, context: Context | None, config: Context):
-        callbacks: list[BaseCallback] = ensure_callbacks(self.callbacks)
-        for callback in callbacks:
-            context, config = callback.on_enter(self, context, config)
-        return context, config, callbacks
-
-    def leave(self, context: ChainContext, config: Context, callbacks: list[BaseCallback]):
-        for callback in reversed(callbacks):
-            context, config = callback.on_leave(self, context, config)
-        return context, config
-
-    def add_pre_processes(self, *processes: Process | AsyncProcess):
-        self.callbacks.extend(Callback(pre_process=i) for i in processes)
-        return self
-
-    def add_mid_processes(self, *processes: Process | AsyncProcess):
-        self.callbacks.extend(Callback(mid_process=i) for i in processes)
-        return self
-
-    def add_end_processes(self, *processes: Process | AsyncProcess):
-        self.callbacks.extend(Callback(end_process=i) for i in processes)
-        return self
-
-    def add_callbacks(self, *callbacks: BaseCallback | type[BaseCallback]):
-        self.callbacks.extend(callbacks)
-        return self
-
-    def pre_process(self, process: Process | AsyncProcess):
-        self.add_pre_processes(process)
-        return process
-
-    def mid_process(self, process: Process | AsyncProcess):
-        self.add_mid_processes(process)
-        return process
-
-    def end_process(self, process: Process | AsyncProcess):
-        self.add_end_processes(process)
-        return process
-
-    def callback(self, callback: BaseCallback | type[BaseCallback]):
-        self.add_callbacks(callback)
-        return callback
-
-    @staticmethod
-    def _apply_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
-        for callback in callbacks:
-            context |= cast(Context, callback.pre_process(context) or {})
-
-    @staticmethod
-    def _apply_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
-        for callback in callbacks:
-            context |= cast(Context, callback.mid_process(context) or {})
-
-    @staticmethod
-    def _apply_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
-        for callback in reversed(callbacks):
-            context |= cast(Context, callback.end_process(context) or {})
-
-    @staticmethod
-    async def _apply_async_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
-        for callback in callbacks:
-            context |= cast(Context, await resolve(callback.pre_process(context)) or {})
-
-    @staticmethod
-    async def _apply_async_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
-        for callback in callbacks:
-            context |= cast(Context, await resolve(callback.mid_process(context)) or {})
-
-    @staticmethod
-    async def _apply_async_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
-        for callback in reversed(callbacks):
-            context |= cast(Context, await resolve(callback.end_process(context)) or {})
-
-    def invoke(self, context=None, /, complete=None, **config) -> ChainContext:
-        context, config, callbacks = self.enter(context, config)
-        context = ChainContext.ensure(context)
-
-        try:
-            self._invoke(ChainContext(context, self.context), complete, callbacks, **config)
-        except Jump as jump:
-            context, config = self.leave(context, config, callbacks)
-            if jump.out_of is not None and jump.out_of is not self:
-                raise jump from None
-            if jump.into is not None:
-                jump.into.invoke(context, complete, **config)
-        else:
-            context, config = self.leave(context, config, callbacks)
-
-        return context
-
-    async def ainvoke(self, context=None, /, complete=None, **config) -> ChainContext:
-        context, config, callbacks = self.enter(context, config)
-        context = ChainContext.ensure(context)
-
-        try:
-            await self._ainvoke(ChainContext(context, self.context), complete, callbacks, **config)
-        except Jump as jump:
-            context, config = self.leave(context, config, callbacks)
-            if jump.out_of is not None and jump.out_of is not self:
-                raise jump from None
-            if jump.into is not None:
-                await jump.into.ainvoke(context, complete, **config)
-        else:
-            context, config = self.leave(context, config, callbacks)
-
-        return context
-
-    def stream(self, context=None, /, generate=None, **config) -> Iterable[ChainContext]:
-        context, config, callbacks = self.enter(context, config)
-        context = ChainContext.ensure(context)
-
-        try:
-            for _ in self._stream(ChainContext(context, self.context), generate, callbacks, **config):
-                yield context
-        except Jump as jump:
-            context, config = self.leave(context, config, callbacks)
-            if jump.out_of is not None and jump.out_of is not self:
-                raise jump from None
-            if jump.into is not None:
-                yield from jump.into.stream(context, generate, **config)
-        else:
-            context, config = self.leave(context, config, callbacks)
-
-    async def astream(self, context=None, /, generate=None, **config) -> AsyncIterable[ChainContext]:
-        context, config, callbacks = self.enter(context, config)
-        context = ChainContext.ensure(context)
-
-        try:
-            async for _ in self._astream(ChainContext(context, self.context), generate, callbacks, **config):
-                yield context
-        except Jump as jump:
-            context, config = self.leave(context, config, callbacks)
-            if jump.out_of is not None and jump.out_of is not self:
-                raise jump from None
-            if jump.into is not None:
-                async for i in jump.into.astream(context, generate, **config):
-                    yield i
-        else:
-            context, config = self.leave(context, config, callbacks)
-
-    _context: Context | None
-
-    @property
-    def context(self):
-        if self._context is None:
-            self._context = {}
-        return self._context
-
-    @context.setter
-    def context(self, context: Context | None):
-        self._context = context
-
-    @context.deleter
-    def context(self):
-        self._context = None
-
-
-class Node(Loader, Interruptable):
-    def __init__(
-        self,
-        template: Template | str,
-        partial_context: Context | None = None,
-        llm: LLM | None = None,
-        **config,
-    ):
-        self.template = Template(template) if isinstance(template, str) else template
-        self._context = partial_context
-        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
-        self.llm = llm
-        self.run_config = config
-
-    def _invoke(self, context, /, complete, callbacks, **config):
-        complete = cast(Complete, self.llm.complete if self.llm else complete)
-        assert complete is not None
-
-        prompt = self.render(context, callbacks)
-
-        context.result = complete(prompt, **(self.run_config | config))
-
-        self._apply_mid_processes(context, callbacks)
-
-        self._apply_end_processes(context, callbacks)
-
-    def _stream(self, context, /, generate, callbacks, **config):
-        generate = cast(Generate, self.llm.generate if self.llm else generate)
-        assert generate is not None
-
-        prompt = self.render(context, callbacks)
-
-        for result in accumulate(generate(prompt, **(self.run_config | config))):
-            context.result = result
-            self._apply_mid_processes(context, callbacks)
-            yield
-
-        self._apply_end_processes(context, callbacks)
-
-    async def _ainvoke(self, context, /, complete, callbacks, **config):
-        complete = cast(Complete | AsyncComplete, self.llm.complete if self.llm else complete)
-        assert complete is not None
-
-        prompt = await self.arender(context, callbacks)
-
-        context.result = await resolve(complete(prompt, **(self.run_config | config)))
-
-        await self._apply_async_mid_processes(context, callbacks)
-
-        await self._apply_async_end_processes(context, callbacks)
-
-    async def _astream(self, context, /, generate, callbacks, **config):
-        generate = cast(Generate | AsyncGenerate, self.llm.generate if self.llm else generate)
-        assert generate is not None
-
-        prompt = await self.arender(context, callbacks)
-
-        async for result in accumulate_any(generate(prompt, **(self.run_config | config))):
-            context.result = result
-            await self._apply_async_mid_processes(context, callbacks)
-            yield
-
-        await self._apply_async_end_processes(context, callbacks)
-
-    def render(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
-        if callbacks is None:
-            callbacks = ensure_callbacks(self.callbacks)
-        context = ChainContext(context, self.context)
-        self._apply_pre_processes(context, callbacks)
-        return self.template.render(context)
-
-    async def arender(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
-        if callbacks is None:
-            callbacks = ensure_callbacks(self.callbacks)
-        context = ChainContext(context, self.context)
-        await self._apply_async_pre_processes(context, callbacks)
-        return await self.template.arender(context)
-
-    def __str__(self):
-        return f"</{self.name}/>"
-
-
-class Loop(Interruptable):
-    def __init__(self, chain: AbstractNode, partial_context: Context | None = None):
-        self.chain = chain
-        self._context = partial_context
-        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
-
-    def _invoke(self, context, /, complete, callbacks, **config):
-        while True:
-            self._apply_pre_processes(context, callbacks)
-            self.chain.invoke(context, complete, **config)
-            self._apply_mid_processes(context, callbacks)
-            self._apply_end_processes(context, callbacks)
-
-    async def _ainvoke(self, context, /, complete, callbacks, **config):
-        while True:
-            await self._apply_async_pre_processes(context, callbacks)
-            await self.chain.ainvoke(context, complete, **config)
-            await self._apply_async_mid_processes(context, callbacks)
-            await self._apply_async_end_processes(context, callbacks)
-
-    def _stream(self, context, /, generate, callbacks, **config):
-        while True:
-            self._apply_pre_processes(context, callbacks)
-            for _ in self.chain.stream(context, generate, **config):
-                self._apply_mid_processes(context, callbacks)
-                yield
-            self._apply_end_processes(context, callbacks)
-
-    async def _astream(self, context, /, generate, callbacks, **config):
-        while True:
-            await self._apply_async_pre_processes(context, callbacks)
-            async for _ in self.chain.astream(context, generate, **config):
-                await self._apply_async_mid_processes(context, callbacks)
-                yield
-            await self._apply_async_end_processes(context, callbacks)
-
-
-class Chain(Interruptable):
-    def __init__(self, *nodes: AbstractNode, partial_context: Context | None = None):
-        self.nodes = list(nodes)
-        self._context = partial_context
-        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
-
-    @classmethod
-    def _get_chain_type(cls):
-        return cls
-
-    def __iadd__(self, chain: AbstractNode):
-        self.nodes.append(chain)
-        return self
-
-    def __iter__(self):
-        return iter(self.nodes)
-
-    def _invoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
-        self._apply_pre_processes(context, callbacks)
-        for node in self.nodes:
-            node.invoke(context, complete, **config)
-            self._apply_mid_processes(context, callbacks)
-        self._apply_end_processes(context, callbacks)
-
-    async def _ainvoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
-        await self._apply_async_pre_processes(context, callbacks)
-        for node in self.nodes:
-            await node.ainvoke(context, complete, **config)
-            await self._apply_async_mid_processes(context, callbacks)
-        await self._apply_async_end_processes(context, callbacks)
-
-    def _stream(self, context, /, generate, callbacks: list[BaseCallback], **config):
-        self._apply_pre_processes(context, callbacks)
-        for node in self.nodes:
-            for _ in node.stream(context, generate, **config):
-                self._apply_mid_processes(context, callbacks)
-                yield
-        self._apply_end_processes(context, callbacks)
-
-    async def _astream(self, context, /, generate, callbacks: list[BaseCallback], **config):
-        await self._apply_async_pre_processes(context, callbacks)
-        for node in self.nodes:
-            async for _ in node.astream(context, generate, **config):
-                await self._apply_async_mid_processes(context, callbacks)
-                yield
-        await self._apply_async_end_processes(context, callbacks)
-
-    def __repr__(self):
-        return " + ".join(map(str, self.nodes))
-
-
-class Jump(Exception):
-    def __init__(self, into: Interruptable | None = None, out_of: Interruptable | None = None):
-        self.into = into
-        self.out_of = out_of
-
-    def __str__(self):
-        return f"{self.out_of} does not exist in the chain hierarchy"
+from inspect import isclass
+from itertools import accumulate
+from typing import Callable, Mapping, MutableMapping, overload
+
+from ..llm.base import *
+from ..prompt.template import Context, Loader, SafeChainMapContext, Template
+from .callback import BaseCallback, Callback
+from .utils import accumulate_any, resolve
+
+
+class ChainContext(SafeChainMapContext):
+    @overload
+    def __init__(self): ...
+
+    @overload
+    def __init__(self, least: MutableMapping | None = None): ...
+
+    @overload
+    def __init__(self, least: MutableMapping | None = None, *maps: Mapping): ...
+
+    def __init__(self, least: MutableMapping | None = None, *maps: Mapping):
+        super().__init__({} if least is None else least, *maps)  # type: ignore
+
+    @classmethod
+    def ensure(cls, context):
+        return context if isinstance(context, cls) else cls(context)
+
+    @property
+    def result(self):
+        return self.__getitem__("__result__")
+
+    @result.setter
+    def result(self, result):
+        self.__setitem__("__result__", result)
+
+    @result.deleter
+    def result(self):
+        self.__delitem__("__result__")
+
+    def __str__(self):
+        return str({**self})
+
+
+Process = Callable[[ChainContext], Context | None]
+
+AsyncProcess = Callable[[ChainContext], Awaitable[Context | None]]
+
+
+class AbstractNode(Protocol):
+    def invoke(
+        self,
+        context: Context | None = None,
+        /,
+        complete: Complete | None = None,
+        **config,
+    ) -> ChainContext: ...
+
+    async def ainvoke(
+        self,
+        context: Context | None = None,
+        /,
+        complete: Complete | AsyncComplete | None = None,
+        **config,
+    ) -> ChainContext: ...
+
+    def stream(
+        self,
+        context: Context | None = None,
+        /,
+        generate: Generate | None = None,
+        **config,
+    ) -> Iterable[ChainContext]: ...
+
+    def astream(
+        self,
+        context: Context | None = None,
+        /,
+        generate: Generate | AsyncGenerate | None = None,
+        **config,
+    ) -> AsyncIterable[ChainContext]: ...
+
+    @classmethod
+    def _get_chain_type(cls):
+        return Chain
+
+    def __add__(self, chain: "AbstractNode"):
+        if isinstance(chain, Chain):
+            return self._get_chain_type()(self, *chain)
+        return self._get_chain_type()(self, chain)
+
+
+def ensure_callbacks(callbacks: list[BaseCallback | type[BaseCallback]]) -> list[BaseCallback]:
+    return [i() if isclass(i) else i for i in callbacks]
+
+
+class Interruptable(AbstractNode, Protocol):
+    def _invoke(
+        self,
+        context: ChainContext,
+        /,
+        complete: Complete | None,
+        callbacks: list[BaseCallback],
+        **config,
+    ): ...
+
+    async def _ainvoke(
+        self,
+        context: ChainContext,
+        /,
+        complete: Complete | AsyncComplete | None,
+        callbacks: list[BaseCallback],
+        **config,
+    ): ...
+
+    def _stream(
+        self,
+        context: ChainContext,
+        /,
+        generate: Generate | None,
+        callbacks: list[BaseCallback],
+        **config,
+    ) -> Iterable: ...
+
+    def _astream(
+        self,
+        context: ChainContext,
+        /,
+        generate: Generate | AsyncGenerate | None,
+        callbacks: list[BaseCallback],
+        **config,
+    ) -> AsyncIterable: ...
+
+    callbacks: list[BaseCallback | type[BaseCallback]]
+
+    def enter(self, context: Context | None, config: Context):
+        callbacks: list[BaseCallback] = ensure_callbacks(self.callbacks)
+        for callback in callbacks:
+            context, config = callback.on_enter(self, context, config)
+        return context, config, callbacks
+
+    def leave(self, context: ChainContext, config: Context, callbacks: list[BaseCallback]):
+        for callback in reversed(callbacks):
+            context, config = callback.on_leave(self, context, config)
+        return context, config
+
+    def add_pre_processes(self, *processes: Process | AsyncProcess):
+        self.callbacks.extend(Callback(pre_process=i) for i in processes)
+        return self
+
+    def add_mid_processes(self, *processes: Process | AsyncProcess):
+        self.callbacks.extend(Callback(mid_process=i) for i in processes)
+        return self
+
+    def add_end_processes(self, *processes: Process | AsyncProcess):
+        self.callbacks.extend(Callback(end_process=i) for i in processes)
+        return self
+
+    def add_callbacks(self, *callbacks: BaseCallback | type[BaseCallback]):
+        self.callbacks.extend(callbacks)
+        return self
+
+    def pre_process(self, process: Process | AsyncProcess):
+        self.add_pre_processes(process)
+        return process
+
+    def mid_process(self, process: Process | AsyncProcess):
+        self.add_mid_processes(process)
+        return process
+
+    def end_process(self, process: Process | AsyncProcess):
+        self.add_end_processes(process)
+        return process
+
+    def callback(self, callback: BaseCallback | type[BaseCallback]):
+        self.add_callbacks(callback)
+        return callback
+
+    @staticmethod
+    def _apply_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
+        for callback in callbacks:
+            context |= cast(Context, callback.pre_process(context) or {})
+
+    @staticmethod
+    def _apply_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
+        for callback in callbacks:
+            context |= cast(Context, callback.mid_process(context) or {})
+
+    @staticmethod
+    def _apply_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
+        for callback in reversed(callbacks):
+            context |= cast(Context, callback.end_process(context) or {})
+
+    @staticmethod
+    async def _apply_async_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
+        for callback in callbacks:
+            context |= cast(Context, await resolve(callback.pre_process(context)) or {})
+
+    @staticmethod
+    async def _apply_async_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
+        for callback in callbacks:
+            context |= cast(Context, await resolve(callback.mid_process(context)) or {})
+
+    @staticmethod
+    async def _apply_async_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
+        for callback in reversed(callbacks):
+            context |= cast(Context, await resolve(callback.end_process(context)) or {})
+
+    def invoke(self, context=None, /, complete=None, **config) -> ChainContext:
+        context, config, callbacks = self.enter(context, config)
+        context = ChainContext.ensure(context)
+
+        try:
+            self._invoke(ChainContext(context, self.context), complete, callbacks, **config)
+        except Jump as jump:
+            context, config = self.leave(context, config, callbacks)
+            if jump.out_of is not None and jump.out_of is not self:
+                raise jump from None
+            if jump.into is not None:
+                jump.into.invoke(context, complete, **config)
+        else:
+            context, config = self.leave(context, config, callbacks)
+
+        return context
+
+    async def ainvoke(self, context=None, /, complete=None, **config) -> ChainContext:
+        context, config, callbacks = self.enter(context, config)
+        context = ChainContext.ensure(context)
+
+        try:
+            await self._ainvoke(ChainContext(context, self.context), complete, callbacks, **config)
+        except Jump as jump:
+            context, config = self.leave(context, config, callbacks)
+            if jump.out_of is not None and jump.out_of is not self:
+                raise jump from None
+            if jump.into is not None:
+                await jump.into.ainvoke(context, complete, **config)
+        else:
+            context, config = self.leave(context, config, callbacks)
+
+        return context
+
+    def stream(self, context=None, /, generate=None, **config) -> Iterable[ChainContext]:
+        context, config, callbacks = self.enter(context, config)
+        context = ChainContext.ensure(context)
+
+        try:
+            for _ in self._stream(ChainContext(context, self.context), generate, callbacks, **config):
+                yield context
+        except Jump as jump:
+            context, config = self.leave(context, config, callbacks)
+            if jump.out_of is not None and jump.out_of is not self:
+                raise jump from None
+            if jump.into is not None:
+                yield from jump.into.stream(context, generate, **config)
+        else:
+            context, config = self.leave(context, config, callbacks)
+
+    async def astream(self, context=None, /, generate=None, **config) -> AsyncIterable[ChainContext]:
+        context, config, callbacks = self.enter(context, config)
+        context = ChainContext.ensure(context)
+
+        try:
+            async for _ in self._astream(ChainContext(context, self.context), generate, callbacks, **config):
+                yield context
+        except Jump as jump:
+            context, config = self.leave(context, config, callbacks)
+            if jump.out_of is not None and jump.out_of is not self:
+                raise jump from None
+            if jump.into is not None:
+                async for i in jump.into.astream(context, generate, **config):
+                    yield i
+        else:
+            context, config = self.leave(context, config, callbacks)
+
+    _context: Context | None
+
+    @property
+    def context(self):
+        if self._context is None:
+            self._context = {}
+        return self._context
+
+    @context.setter
+    def context(self, context: Context | None):
+        self._context = context
+
+    @context.deleter
+    def context(self):
+        self._context = None
+
+
+class Node(Loader, Interruptable):
+    def __init__(
+        self,
+        template: Template | str,
+        partial_context: Context | None = None,
+        llm: LLM | None = None,
+        **config,
+    ):
+        self.template = Template(template) if isinstance(template, str) else template
+        self._context = partial_context
+        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
+        self.llm = llm
+        self.run_config = config
+
+    def _invoke(self, context, /, complete, callbacks, **config):
+        complete = cast(Complete, self.llm.complete if self.llm else complete)
+        assert complete is not None
+
+        prompt = self.render(context, callbacks)
+
+        context.result = complete(prompt, **(self.run_config | config))
+
+        self._apply_mid_processes(context, callbacks)
+
+        self._apply_end_processes(context, callbacks)
+
+    def _stream(self, context, /, generate, callbacks, **config):
+        generate = cast(Generate, self.llm.generate if self.llm else generate)
+        assert generate is not None
+
+        prompt = self.render(context, callbacks)
+
+        for result in accumulate(generate(prompt, **(self.run_config | config))):
+            context.result = result
+            self._apply_mid_processes(context, callbacks)
+            yield
+
+        self._apply_end_processes(context, callbacks)
+
+    async def _ainvoke(self, context, /, complete, callbacks, **config):
+        complete = cast(Complete | AsyncComplete, self.llm.complete if self.llm else complete)
+        assert complete is not None
+
+        prompt = await self.arender(context, callbacks)
+
+        context.result = await resolve(complete(prompt, **(self.run_config | config)))
+
+        await self._apply_async_mid_processes(context, callbacks)
+
+        await self._apply_async_end_processes(context, callbacks)
+
+    async def _astream(self, context, /, generate, callbacks, **config):
+        generate = cast(Generate | AsyncGenerate, self.llm.generate if self.llm else generate)
+        assert generate is not None
+
+        prompt = await self.arender(context, callbacks)
+
+        async for result in accumulate_any(generate(prompt, **(self.run_config | config))):
+            context.result = result
+            await self._apply_async_mid_processes(context, callbacks)
+            yield
+
+        await self._apply_async_end_processes(context, callbacks)
+
+    def render(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
+        if callbacks is None:
+            callbacks = ensure_callbacks(self.callbacks)
+        context = ChainContext(context, self.context)
+        self._apply_pre_processes(context, callbacks)
+        return self.template.render(context)
+
+    async def arender(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
+        if callbacks is None:
+            callbacks = ensure_callbacks(self.callbacks)
+        context = ChainContext(context, self.context)
+        await self._apply_async_pre_processes(context, callbacks)
+        return await self.template.arender(context)
+
+    def __str__(self):
+        return f"</{self.name}/>"
+
+
+class Loop(Interruptable):
+    def __init__(self, chain: AbstractNode, partial_context: Context | None = None):
+        self.chain = chain
+        self._context = partial_context
+        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
+
+    def _invoke(self, context, /, complete, callbacks, **config):
+        while True:
+            self._apply_pre_processes(context, callbacks)
+            self.chain.invoke(context, complete, **config)
+            self._apply_mid_processes(context, callbacks)
+            self._apply_end_processes(context, callbacks)
+
+    async def _ainvoke(self, context, /, complete, callbacks, **config):
+        while True:
+            await self._apply_async_pre_processes(context, callbacks)
+            await self.chain.ainvoke(context, complete, **config)
+            await self._apply_async_mid_processes(context, callbacks)
+            await self._apply_async_end_processes(context, callbacks)
+
+    def _stream(self, context, /, generate, callbacks, **config):
+        while True:
+            self._apply_pre_processes(context, callbacks)
+            for _ in self.chain.stream(context, generate, **config):
+                self._apply_mid_processes(context, callbacks)
+                yield
+            self._apply_end_processes(context, callbacks)
+
+    async def _astream(self, context, /, generate, callbacks, **config):
+        while True:
+            await self._apply_async_pre_processes(context, callbacks)
+            async for _ in self.chain.astream(context, generate, **config):
+                await self._apply_async_mid_processes(context, callbacks)
+                yield
+            await self._apply_async_end_processes(context, callbacks)
+
+
+class Chain(Interruptable):
+    def __init__(self, *nodes: AbstractNode, partial_context: Context | None = None):
+        self.nodes = list(nodes)
+        self._context = partial_context
+        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
+
+    @classmethod
+    def _get_chain_type(cls):
+        return cls
+
+    def __iadd__(self, chain: AbstractNode):
+        self.nodes.append(chain)
+        return self
+
+    def __iter__(self):
+        return iter(self.nodes)
+
+    def _invoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
+        self._apply_pre_processes(context, callbacks)
+        for node in self.nodes:
+            node.invoke(context, complete, **config)
+            self._apply_mid_processes(context, callbacks)
+        self._apply_end_processes(context, callbacks)
+
+    async def _ainvoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
+        await self._apply_async_pre_processes(context, callbacks)
+        for node in self.nodes:
+            await node.ainvoke(context, complete, **config)
+            await self._apply_async_mid_processes(context, callbacks)
+        await self._apply_async_end_processes(context, callbacks)
+
+    def _stream(self, context, /, generate, callbacks: list[BaseCallback], **config):
+        self._apply_pre_processes(context, callbacks)
+        for node in self.nodes:
+            for _ in node.stream(context, generate, **config):
+                self._apply_mid_processes(context, callbacks)
+                yield
+        self._apply_end_processes(context, callbacks)
+
+    async def _astream(self, context, /, generate, callbacks: list[BaseCallback], **config):
+        await self._apply_async_pre_processes(context, callbacks)
+        for node in self.nodes:
+            async for _ in node.astream(context, generate, **config):
+                await self._apply_async_mid_processes(context, callbacks)
+                yield
+        await self._apply_async_end_processes(context, callbacks)
+
+    def __repr__(self):
+        return " + ".join(map(str, self.nodes))
+
+
+class Jump(Exception):
+    def __init__(self, into: Interruptable | None = None, out_of: Interruptable | None = None):
+        self.into = into
+        self.out_of = out_of
+
+    def __str__(self):
+        return f"{self.out_of} does not exist in the chain hierarchy"
```

### Comparing `promplate-0.3.4.5/promplate/chain/utils.py` & `promplate-0.3.4.6/promplate/chain/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from inspect import Parameter, isawaitable, signature
-from itertools import accumulate
-from typing import AsyncIterable, Awaitable, Callable, Iterable, TypeVar, cast
-
-T = TypeVar("T")
-
-
-def appender(to_append: list[T]) -> Callable[[T], T]:
-    def append_processer(func: T) -> T:
-        to_append.append(func)
-
-        return func
-
-    return append_processer
-
-
-def is_positional_parameter(p: Parameter):
-    return p.kind is Parameter.POSITIONAL_OR_KEYWORD or p.kind is Parameter.KEYWORD_ONLY
-
-
-def count_position_parameters(func):
-    return sum(map(is_positional_parameter, signature(func).parameters.values()))
-
-
-async def resolve(maybe_awaitable: T | Awaitable[T], /) -> T:
-    while isawaitable(maybe_awaitable):
-        maybe_awaitable = await maybe_awaitable
-
-    return maybe_awaitable  # type: ignore
-
-
-async def async_accumulate(async_iterable: AsyncIterable[str]):
-    result = ""
-    async for delta in async_iterable:
-        result += delta
-        yield result
-
-
-def accumulate_any(any_iterable: Iterable[str] | AsyncIterable[str]):
-    if "__aiter__" in dir(any_iterable):
-        return async_accumulate(any_iterable)  # type: ignore
-
-    async def _():
-        for i in accumulate(cast(Iterable[str], any_iterable)):
-            yield i
-
-    return _()
+from inspect import Parameter, isawaitable, signature
+from itertools import accumulate
+from typing import AsyncIterable, Awaitable, Callable, Iterable, TypeVar, cast
+
+T = TypeVar("T")
+
+
+def appender(to_append: list[T]) -> Callable[[T], T]:
+    def append_processer(func: T) -> T:
+        to_append.append(func)
+
+        return func
+
+    return append_processer
+
+
+def is_positional_parameter(p: Parameter):
+    return p.kind is Parameter.POSITIONAL_OR_KEYWORD or p.kind is Parameter.KEYWORD_ONLY
+
+
+def count_position_parameters(func):
+    return sum(map(is_positional_parameter, signature(func).parameters.values()))
+
+
+async def resolve(maybe_awaitable: T | Awaitable[T], /) -> T:
+    while isawaitable(maybe_awaitable):
+        maybe_awaitable = await maybe_awaitable
+
+    return maybe_awaitable  # type: ignore
+
+
+async def async_accumulate(async_iterable: AsyncIterable[str]):
+    result = ""
+    async for delta in async_iterable:
+        result += delta
+        yield result
+
+
+def accumulate_any(any_iterable: Iterable[str] | AsyncIterable[str]):
+    if "__aiter__" in dir(any_iterable):
+        return async_accumulate(any_iterable)  # type: ignore
+
+    async def _():
+        for i in accumulate(cast(Iterable[str], any_iterable)):
+            yield i
+
+    return _()
```

### Comparing `promplate-0.3.4.5/promplate/llm/openai/v0.py` & `promplate-0.3.4.6/promplate/llm/openai/v0.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from importlib.metadata import metadata
-from typing import TYPE_CHECKING, Any
-
-import openai
-from openai import ChatCompletion, Completion  # type: ignore
-
-from ...prompt.chat import Message, ensure
-from ..base import *
-
-meta = metadata("promplate")
-
-if openai.api_key is None:
-    openai.api_key = ""
-
-openai.app_info = (openai.app_info or {}) | {  # type: ignore
-    "name": "Promplate",
-    "version": meta["version"],
-    "url": meta["home-page"],
-}
-
-
-if TYPE_CHECKING:
-
-    class Config(Configurable):
-        def __init__(
-            self,
-            model: str,
-            temperature: float | int | None = None,
-            top_p: float | int | None = None,
-            stop: str | list[str] | None = None,
-            max_tokens: int | None = None,
-            api_key: str | None = None,
-            api_base: str | None = None,
-            **other_config,
-        ):
-            self.model = model
-            self.temperature = temperature
-            self.top_p = top_p
-            self.stop = stop
-            self.max_tokens = max_tokens
-            self.api_key = api_key
-            self.api_base = api_base
-
-            for key, val in other_config.items():
-                setattr(self, key, val)
-
-        def __setattr__(self, *_): ...
-
-        def __getattr__(self, _): ...
-
-else:
-    Config = Configurable
-
-
-class TextComplete(Config, Complete):
-    def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": False, "prompt": text}
-        result: Any = Completion.create(**config)
-        return result["choices"][0]["text"]
-
-
-class AsyncTextComplete(Config, AsyncComplete):
-    async def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": False, "prompt": text}
-        result: Any = await Completion.acreate(**config)
-        return result["choices"][0]["text"]
-
-
-class TextGenerate(Config, Generate):
-    def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": True, "prompt": text}
-        stream: Any = Completion.create(**config)
-        for event in stream:
-            yield event["choices"][0]["text"]
-
-
-class AsyncTextGenerate(Config, AsyncGenerate):
-    async def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": True, "prompt": text}
-        stream: Any = await Completion.acreate(**config)
-        async for event in stream:
-            yield event["choices"][0]["text"]
-
-
-class ChatComplete(Config, Complete):
-    def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._config | config | {"stream": False, "messages": messages}
-        result: Any = ChatCompletion.create(**config)
-        return result["choices"][0]["message"]["content"]
-
-
-class AsyncChatComplete(Config, AsyncComplete):
-    async def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._config | config | {"stream": False, "messages": messages}
-        result: Any = await ChatCompletion.acreate(**config)
-        return result["choices"][0]["message"]["content"]
-
-
-class ChatGenerate(Config, Generate):
-    def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._config | config | {"stream": True, "messages": messages}
-        stream: Any = ChatCompletion.create(**config)
-        for event in stream:
-            delta: dict = event["choices"][0]["delta"]
-            yield delta.get("content", "")
-
-
-class AsyncChatGenerate(Config, AsyncGenerate):
-    async def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._config | config | {"stream": True, "messages": messages}
-        stream: Any = await ChatCompletion.acreate(**config)
-        async for event in stream:
-            delta: dict = event["choices"][0]["delta"]
-            yield delta.get("content", "")
+from importlib.metadata import metadata
+from typing import TYPE_CHECKING, Any
+
+import openai
+from openai import ChatCompletion, Completion  # type: ignore
+
+from ...prompt.chat import Message, ensure
+from ..base import *
+
+meta = metadata("promplate")
+
+if openai.api_key is None:
+    openai.api_key = ""
+
+openai.app_info = (openai.app_info or {}) | {  # type: ignore
+    "name": "Promplate",
+    "version": meta["version"],
+    "url": meta["home-page"],
+}
+
+
+if TYPE_CHECKING:
+
+    class Config(Configurable):
+        def __init__(
+            self,
+            model: str,
+            temperature: float | int | None = None,
+            top_p: float | int | None = None,
+            stop: str | list[str] | None = None,
+            max_tokens: int | None = None,
+            api_key: str | None = None,
+            api_base: str | None = None,
+            **other_config,
+        ):
+            self.model = model
+            self.temperature = temperature
+            self.top_p = top_p
+            self.stop = stop
+            self.max_tokens = max_tokens
+            self.api_key = api_key
+            self.api_base = api_base
+
+            for key, val in other_config.items():
+                setattr(self, key, val)
+
+        def __setattr__(self, *_): ...
+
+        def __getattr__(self, _): ...
+
+else:
+    Config = Configurable
+
+
+class TextComplete(Config, Complete):
+    def __call__(self, text: str, /, **config):
+        config = self._config | config | {"stream": False, "prompt": text}
+        result: Any = Completion.create(**config)
+        return result["choices"][0]["text"]
+
+
+class AsyncTextComplete(Config, AsyncComplete):
+    async def __call__(self, text: str, /, **config):
+        config = self._config | config | {"stream": False, "prompt": text}
+        result: Any = await Completion.acreate(**config)
+        return result["choices"][0]["text"]
+
+
+class TextGenerate(Config, Generate):
+    def __call__(self, text: str, /, **config):
+        config = self._config | config | {"stream": True, "prompt": text}
+        stream: Any = Completion.create(**config)
+        for event in stream:
+            yield event["choices"][0]["text"]
+
+
+class AsyncTextGenerate(Config, AsyncGenerate):
+    async def __call__(self, text: str, /, **config):
+        config = self._config | config | {"stream": True, "prompt": text}
+        stream: Any = await Completion.acreate(**config)
+        async for event in stream:
+            yield event["choices"][0]["text"]
+
+
+class ChatComplete(Config, Complete):
+    def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._config | config | {"stream": False, "messages": messages}
+        result: Any = ChatCompletion.create(**config)
+        return result["choices"][0]["message"]["content"]
+
+
+class AsyncChatComplete(Config, AsyncComplete):
+    async def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._config | config | {"stream": False, "messages": messages}
+        result: Any = await ChatCompletion.acreate(**config)
+        return result["choices"][0]["message"]["content"]
+
+
+class ChatGenerate(Config, Generate):
+    def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._config | config | {"stream": True, "messages": messages}
+        stream: Any = ChatCompletion.create(**config)
+        for event in stream:
+            delta: dict = event["choices"][0]["delta"]
+            yield delta.get("content", "")
+
+
+class AsyncChatGenerate(Config, AsyncGenerate):
+    async def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._config | config | {"stream": True, "messages": messages}
+        stream: Any = await ChatCompletion.acreate(**config)
+        async for event in stream:
+            delta: dict = event["choices"][0]["delta"]
+            yield delta.get("content", "")
```

### Comparing `promplate-0.3.4.5/promplate/llm/openai/v1.py` & `promplate-0.3.4.6/promplate/llm/openai/v1.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,184 +1,184 @@
-from copy import copy
-from functools import cached_property
-from types import MappingProxyType
-from typing import TYPE_CHECKING, Any, Callable, ParamSpec, TypeVar
-
-from openai import AsyncClient, Client  # type: ignore
-
-from ...prompt.chat import Message, ensure
-from ...prompt.utils import _get_aclient, _get_client, get_user_agent
-from ..base import *
-
-P = ParamSpec("P")
-T = TypeVar("T")
-
-
-def same_params_as(_: Callable[P, Any]):
-    def func(__init__: Callable[..., None]) -> Callable[P, None]:
-        return __init__  # type: ignore
-
-    return func
-
-
-class Config(Configurable):
-    def __init__(self, **config):
-        super().__init__(**config)
-        self._run_config = {}
-
-    def bind(self, **run_config):
-        obj = copy(self)
-        obj._run_config = self._run_config | run_config
-        return obj
-
-    @cached_property
-    def _user_agent(self):
-        from openai.version import VERSION
-
-        return get_user_agent(self, ("OpenAI", VERSION))
-
-    @property
-    def _config(self):  # type: ignore
-        ua_header = {"User-Agent": self._user_agent}
-        config = dict(super()._config)
-        config["default_headers"] = config.get("default_headers", {}) | ua_header
-        return MappingProxyType(config)
-
-    @cached_property
-    def _client(self):
-        if "http_client" in self._config:
-            return Client(**self._config)
-        else:
-            return Client(**self._config, http_client=_get_client())
-
-    @cached_property
-    def _aclient(self):
-        if "http_client" in self._config:
-            return AsyncClient(**self._config)
-        else:
-            return AsyncClient(**self._config, http_client=_get_aclient())
-
-
-if TYPE_CHECKING:
-
-    class ClientConfig(Config):
-        @same_params_as(Client)
-        def __init__(self, **config): ...
-
-    class AsyncClientConfig(Config):
-        @same_params_as(AsyncClient)
-        def __init__(self, **config): ...
-
-else:
-    ClientConfig = AsyncClientConfig = Config
-
-
-class TextComplete(ClientConfig):
-    def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": False, "prompt": text}
-        result = self._client.completions.create(**config)
-        return result.choices[0].text
-
-
-class AsyncTextComplete(AsyncClientConfig):
-    async def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": False, "prompt": text}
-        result = await self._aclient.completions.create(**config)
-        return result.choices[0].text
-
-
-class TextGenerate(ClientConfig):
-    def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": True, "prompt": text}
-        stream = self._client.completions.create(**config)
-        for event in stream:
-            try:
-                yield event.choices[0].text
-            except AttributeError:
-                pass
-
-
-class AsyncTextGenerate(AsyncClientConfig):
-    async def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": True, "prompt": text}
-        stream = await self._aclient.completions.create(**config)
-        async for event in stream:
-            try:
-                yield event.choices[0].text
-            except AttributeError:
-                pass
-
-
-class ChatComplete(ClientConfig):
-    def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._run_config | config | {"stream": False, "messages": messages}
-        result = self._client.chat.completions.create(**config)
-        return result.choices[0].message.content
-
-
-class AsyncChatComplete(AsyncClientConfig):
-    async def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._run_config | config | {"stream": False, "messages": messages}
-        result = await self._aclient.chat.completions.create(**config)
-        return result.choices[0].message.content
-
-
-class ChatGenerate(ClientConfig):
-    def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._run_config | config | {"stream": True, "messages": messages}
-        stream = self._client.chat.completions.create(**config)
-        for event in stream:
-            try:
-                yield event.choices[0].delta.content or ""
-            except AttributeError:
-                pass
-
-
-class AsyncChatGenerate(AsyncClientConfig):
-    async def __call__(self, messages: list[Message] | str, /, **config):
-        messages = ensure(messages)
-        config = self._run_config | config | {"stream": True, "messages": messages}
-        stream = await self._aclient.chat.completions.create(**config)
-        async for event in stream:
-            try:
-                yield event.choices[0].delta.content or ""
-            except AttributeError:
-                pass
-
-
-class SyncTextOpenAI(ClientConfig, LLM):
-    complete = TextComplete.__call__  # type: ignore
-    generate = TextGenerate.__call__  # type: ignore
-
-
-class AsyncTextOpenAI(AsyncClientConfig, LLM):
-    complete = AsyncTextComplete.__call__  # type: ignore
-    generate = AsyncTextGenerate.__call__  # type: ignore
-
-
-class SyncChatOpenAI(ClientConfig, LLM):
-    complete = ChatComplete.__call__  # type: ignore
-    generate = ChatGenerate.__call__  # type: ignore
-
-
-class AsyncChatOpenAI(AsyncClientConfig, LLM):
-    complete = AsyncChatComplete.__call__  # type: ignore
-    generate = AsyncChatGenerate.__call__  # type: ignore
-
-
-__all__ = (
-    "TextComplete",
-    "AsyncTextComplete",
-    "TextGenerate",
-    "AsyncTextGenerate",
-    "ChatComplete",
-    "AsyncChatComplete",
-    "ChatGenerate",
-    "AsyncChatGenerate",
-    "SyncTextOpenAI",
-    "AsyncTextOpenAI",
-    "SyncChatOpenAI",
-    "AsyncChatOpenAI",
-)
+from copy import copy
+from functools import cached_property
+from types import MappingProxyType
+from typing import TYPE_CHECKING, Any, Callable, ParamSpec, TypeVar
+
+from openai import AsyncClient, Client  # type: ignore
+
+from ...prompt.chat import Message, ensure
+from ...prompt.utils import _get_aclient, _get_client, get_user_agent
+from ..base import *
+
+P = ParamSpec("P")
+T = TypeVar("T")
+
+
+def same_params_as(_: Callable[P, Any]):
+    def func(__init__: Callable[..., None]) -> Callable[P, None]:
+        return __init__  # type: ignore
+
+    return func
+
+
+class Config(Configurable):
+    def __init__(self, **config):
+        super().__init__(**config)
+        self._run_config = {}
+
+    def bind(self, **run_config):
+        obj = copy(self)
+        obj._run_config = self._run_config | run_config
+        return obj
+
+    @cached_property
+    def _user_agent(self):
+        from openai.version import VERSION
+
+        return get_user_agent(self, ("OpenAI", VERSION))
+
+    @property
+    def _config(self):  # type: ignore
+        ua_header = {"User-Agent": self._user_agent}
+        config = dict(super()._config)
+        config["default_headers"] = config.get("default_headers", {}) | ua_header
+        return MappingProxyType(config)
+
+    @cached_property
+    def _client(self):
+        if "http_client" in self._config:
+            return Client(**self._config)
+        else:
+            return Client(**self._config, http_client=_get_client())
+
+    @cached_property
+    def _aclient(self):
+        if "http_client" in self._config:
+            return AsyncClient(**self._config)
+        else:
+            return AsyncClient(**self._config, http_client=_get_aclient())
+
+
+if TYPE_CHECKING:
+
+    class ClientConfig(Config):
+        @same_params_as(Client)
+        def __init__(self, **config): ...
+
+    class AsyncClientConfig(Config):
+        @same_params_as(AsyncClient)
+        def __init__(self, **config): ...
+
+else:
+    ClientConfig = AsyncClientConfig = Config
+
+
+class TextComplete(ClientConfig):
+    def __call__(self, text: str, /, **config):
+        config = self._run_config | config | {"stream": False, "prompt": text}
+        result = self._client.completions.create(**config)
+        return result.choices[0].text
+
+
+class AsyncTextComplete(AsyncClientConfig):
+    async def __call__(self, text: str, /, **config):
+        config = self._run_config | config | {"stream": False, "prompt": text}
+        result = await self._aclient.completions.create(**config)
+        return result.choices[0].text
+
+
+class TextGenerate(ClientConfig):
+    def __call__(self, text: str, /, **config):
+        config = self._run_config | config | {"stream": True, "prompt": text}
+        stream = self._client.completions.create(**config)
+        for event in stream:
+            try:
+                yield event.choices[0].text
+            except AttributeError:
+                pass
+
+
+class AsyncTextGenerate(AsyncClientConfig):
+    async def __call__(self, text: str, /, **config):
+        config = self._run_config | config | {"stream": True, "prompt": text}
+        stream = await self._aclient.completions.create(**config)
+        async for event in stream:
+            try:
+                yield event.choices[0].text
+            except AttributeError:
+                pass
+
+
+class ChatComplete(ClientConfig):
+    def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._run_config | config | {"stream": False, "messages": messages}
+        result = self._client.chat.completions.create(**config)
+        return result.choices[0].message.content
+
+
+class AsyncChatComplete(AsyncClientConfig):
+    async def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._run_config | config | {"stream": False, "messages": messages}
+        result = await self._aclient.chat.completions.create(**config)
+        return result.choices[0].message.content
+
+
+class ChatGenerate(ClientConfig):
+    def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._run_config | config | {"stream": True, "messages": messages}
+        stream = self._client.chat.completions.create(**config)
+        for event in stream:
+            try:
+                yield event.choices[0].delta.content or ""
+            except AttributeError:
+                pass
+
+
+class AsyncChatGenerate(AsyncClientConfig):
+    async def __call__(self, messages: list[Message] | str, /, **config):
+        messages = ensure(messages)
+        config = self._run_config | config | {"stream": True, "messages": messages}
+        stream = await self._aclient.chat.completions.create(**config)
+        async for event in stream:
+            try:
+                yield event.choices[0].delta.content or ""
+            except AttributeError:
+                pass
+
+
+class SyncTextOpenAI(ClientConfig, LLM):
+    complete = TextComplete.__call__  # type: ignore
+    generate = TextGenerate.__call__  # type: ignore
+
+
+class AsyncTextOpenAI(AsyncClientConfig, LLM):
+    complete = AsyncTextComplete.__call__  # type: ignore
+    generate = AsyncTextGenerate.__call__  # type: ignore
+
+
+class SyncChatOpenAI(ClientConfig, LLM):
+    complete = ChatComplete.__call__  # type: ignore
+    generate = ChatGenerate.__call__  # type: ignore
+
+
+class AsyncChatOpenAI(AsyncClientConfig, LLM):
+    complete = AsyncChatComplete.__call__  # type: ignore
+    generate = AsyncChatGenerate.__call__  # type: ignore
+
+
+__all__ = (
+    "TextComplete",
+    "AsyncTextComplete",
+    "TextGenerate",
+    "AsyncTextGenerate",
+    "ChatComplete",
+    "AsyncChatComplete",
+    "ChatGenerate",
+    "AsyncChatGenerate",
+    "SyncTextOpenAI",
+    "AsyncTextOpenAI",
+    "SyncChatOpenAI",
+    "AsyncChatOpenAI",
+)
```

### Comparing `promplate-0.3.4.5/promplate/prompt/builder.py` & `promplate-0.3.4.6/promplate/prompt/builder.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from types import FunctionType
-
-
-class CodeBuilder:
-    """Build source code conveniently."""
-
-    def __init__(self, indent_level=0, indent_str="\t"):
-        self.code = []
-        self.indent_level = indent_level
-        self.indent_str = indent_str
-
-    def __str__(self):
-        return "".join(map(str, self.code))
-
-    def add_line(self, line):
-        """Add a line of source to the code."""
-        self.code.extend((self.indent_str * self.indent_level, line, "\n"))
-
-        return self
-
-    def add_section(self):
-        """Add a section, a sub-CodeBuilder."""
-        section = CodeBuilder(self.indent_level, self.indent_str)
-        self.code.append(section)
-
-        return section
-
-    def indent(self):
-        """Increase the current indent for following lines."""
-        self.indent_level += 1
-
-        return self
-
-    def dedent(self):
-        """Decrease the current indent for following lines."""
-        self.indent_level -= 1
-
-        return self
-
-    def get_render_function(self) -> FunctionType:
-        """Execute the code, and return a dict of globals it defines."""
-        assert self.indent_level == 0
-        python_source = str(self)
-        global_namespace = {}
-        exec(python_source, global_namespace)
-        return global_namespace["render"]
-
-
-def get_base_builder(sync=True, indent_str="\t"):
-    return (
-        CodeBuilder(indent_str=indent_str)
-        .add_line("def render():" if sync else "async def render():")
-        .indent()
-        .add_line("__parts__ = []")
-        .add_line("__append__ = __parts__.append")
-    )
+from types import FunctionType
+
+
+class CodeBuilder:
+    """Build source code conveniently."""
+
+    def __init__(self, indent_level=0, indent_str="\t"):
+        self.code = []
+        self.indent_level = indent_level
+        self.indent_str = indent_str
+
+    def __str__(self):
+        return "".join(map(str, self.code))
+
+    def add_line(self, line):
+        """Add a line of source to the code."""
+        self.code.extend((self.indent_str * self.indent_level, line, "\n"))
+
+        return self
+
+    def add_section(self):
+        """Add a section, a sub-CodeBuilder."""
+        section = CodeBuilder(self.indent_level, self.indent_str)
+        self.code.append(section)
+
+        return section
+
+    def indent(self):
+        """Increase the current indent for following lines."""
+        self.indent_level += 1
+
+        return self
+
+    def dedent(self):
+        """Decrease the current indent for following lines."""
+        self.indent_level -= 1
+
+        return self
+
+    def get_render_function(self) -> FunctionType:
+        """Execute the code, and return a dict of globals it defines."""
+        assert self.indent_level == 0
+        python_source = str(self)
+        global_namespace = {}
+        exec(python_source, global_namespace)
+        return global_namespace["render"]
+
+
+def get_base_builder(sync=True, indent_str="\t"):
+    return (
+        CodeBuilder(indent_str=indent_str)
+        .add_line("def render():" if sync else "async def render():")
+        .indent()
+        .add_line("__parts__ = []")
+        .add_line("__append__ = __parts__.append")
+    )
```

### Comparing `promplate-0.3.4.5/promplate/prompt/chat.py` & `promplate-0.3.4.6/promplate/prompt/chat.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-from sys import version_info
-from typing import Literal
-
-from .utils import is_message_start
-
-Role = Literal["user", "assistant", "system"]
-
-if version_info >= (3, 12):
-    from typing import NotRequired, TypedDict
-
-    class Message(TypedDict):  # type: ignore
-        role: Role
-        content: str
-        name: NotRequired[str]
-
-else:
-    from typing_extensions import NotRequired, TypedDict
-
-    class Message(TypedDict):
-        role: Role
-        content: str
-        name: NotRequired[str]
-
-
-class MessageBuilder:
-    _initializing = True
-    __slots__ = ("role", "content", "name")
-
-    def __init__(self, role: Role, /, content: str = "", name: str | None = None):
-        self.role: Role = role
-        self.content = content
-        self.name = name
-
-    def __repr__(self):
-        if self.name is not None:
-            return f"<| {self.role} {self.name} |>"
-        return f"<| {self.role} |>"
-
-    def __getitem__(self, key):
-        return getattr(self, key)
-
-    def __setitem__(self, key, value):
-        return setattr(self, key, value)
-
-    def __setattr__(self, key, value):
-        if not self._initializing:
-            assert self is not U and self is not A and self is not S
-            assert isinstance(value, str)
-        return super().__setattr__(key, value)
-
-    def __matmul__(self, name: str):
-        assert isinstance(name, str) and name
-        return self.__class__(self.role, self.content, name)
-
-    def dict(self) -> Message:
-        if self.name:
-            return {"role": self.role, "content": self.content, "name": self.name}
-        return {"role": self.role, "content": self.content}
-
-    def __gt__(self, content: str) -> Message:
-        assert isinstance(content, str)
-        if self.name:
-            return {"role": self.role, "content": content, "name": self.name}
-        return {"role": self.role, "content": content}
-
-
-U = user = MessageBuilder("user")
-A = assistant = MessageBuilder("assistant")
-S = system = MessageBuilder("system")
-MessageBuilder._initializing = False
-
-
-def ensure(text_or_list: list[Message] | str) -> list[Message]:
-    return parse_chat_markup(text_or_list) if isinstance(text_or_list, str) else text_or_list
-
-
-def parse_chat_markup(text: str) -> list[Message]:
-    messages = []
-    current_message = None
-    buffer = []
-
-    for line in text.splitlines():
-        match = is_message_start.match(line)
-        if match:
-            role, name = match.group(1), match.group(2)
-
-            if current_message:
-                current_message["content"] = "\n".join(buffer)
-                messages.append(current_message)
-                buffer.clear()
-
-            current_message = {"role": role, "content": ""}
-
-            if name:
-                current_message["name"] = name
-
-        elif current_message:
-            buffer.append(line)
-
-    if current_message:
-        current_message["content"] = "\n".join(buffer)
-        messages.append(current_message)
-
-    if messages:
-        return messages
-    elif text and text != "\n":
-        return [{"role": "user", "content": text.removesuffix("\n")}]
-    return []
+from sys import version_info
+from typing import Literal
+
+from .utils import is_message_start
+
+Role = Literal["user", "assistant", "system"]
+
+if version_info >= (3, 12):
+    from typing import NotRequired, TypedDict
+
+    class Message(TypedDict):  # type: ignore
+        role: Role
+        content: str
+        name: NotRequired[str]
+
+else:
+    from typing_extensions import NotRequired, TypedDict
+
+    class Message(TypedDict):
+        role: Role
+        content: str
+        name: NotRequired[str]
+
+
+class MessageBuilder:
+    _initializing = True
+    __slots__ = ("role", "content", "name")
+
+    def __init__(self, role: Role, /, content: str = "", name: str | None = None):
+        self.role: Role = role
+        self.content = content
+        self.name = name
+
+    def __repr__(self):
+        if self.name is not None:
+            return f"<| {self.role} {self.name} |>"
+        return f"<| {self.role} |>"
+
+    def __getitem__(self, key):
+        return getattr(self, key)
+
+    def __setitem__(self, key, value):
+        return setattr(self, key, value)
+
+    def __setattr__(self, key, value):
+        if not self._initializing:
+            assert self is not U and self is not A and self is not S
+            assert isinstance(value, str)
+        return super().__setattr__(key, value)
+
+    def __matmul__(self, name: str):
+        assert isinstance(name, str) and name
+        return self.__class__(self.role, self.content, name)
+
+    def dict(self) -> Message:
+        if self.name:
+            return {"role": self.role, "content": self.content, "name": self.name}
+        return {"role": self.role, "content": self.content}
+
+    def __gt__(self, content: str) -> Message:
+        assert isinstance(content, str)
+        if self.name:
+            return {"role": self.role, "content": content, "name": self.name}
+        return {"role": self.role, "content": content}
+
+
+U = user = MessageBuilder("user")
+A = assistant = MessageBuilder("assistant")
+S = system = MessageBuilder("system")
+MessageBuilder._initializing = False
+
+
+def ensure(text_or_list: list[Message] | str) -> list[Message]:
+    return parse_chat_markup(text_or_list) if isinstance(text_or_list, str) else text_or_list
+
+
+def parse_chat_markup(text: str) -> list[Message]:
+    messages = []
+    current_message = None
+    buffer = []
+
+    for line in text.splitlines():
+        match = is_message_start.match(line)
+        if match:
+            role, name = match.group(1), match.group(2)
+
+            if current_message:
+                current_message["content"] = "\n".join(buffer)
+                messages.append(current_message)
+                buffer.clear()
+
+            current_message = {"role": role, "content": ""}
+
+            if name:
+                current_message["name"] = name
+
+        elif current_message:
+            buffer.append(line)
+
+    if current_message:
+        current_message["content"] = "\n".join(buffer)
+        messages.append(current_message)
+
+    if messages:
+        return messages
+    elif text and text != "\n":
+        return [{"role": "user", "content": text.removesuffix("\n")}]
+    return []
```

### Comparing `promplate-0.3.4.5/promplate/prompt/template.py` & `promplate-0.3.4.6/promplate/prompt/template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,222 +1,241 @@
-from ast import Expr, parse, unparse
-from collections import ChainMap
-from functools import cached_property
-from pathlib import Path
-from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Protocol
-
-from .builder import *
-from .utils import *
-
-Context = dict[str, Any]  # globals must be a real dict
-
-
-class Component(Protocol):
-    def render(self, context: Context) -> str: ...
-
-    async def arender(self, context: Context) -> str: ...
-
-
-class TemplateCore(AutoNaming):
-    """A simple template compiler, for a jinja2-like syntax."""
-
-    def __init__(self, text: str):
-        """Construct a Templite with the given `text`."""
-
-        self.text = text
-
-    def _flush(self):
-        for line in self._buffer:
-            self._builder.add_line(line)
-        self._buffer.clear()
-
-    @staticmethod
-    def _unwrap_token(token: str):
-        return dedent(token.strip()[2:-2].strip("-")).strip()
-
-    def _on_literal_token(self, token: str):
-        self._buffer.append(f"__append__({repr(token)})")
-
-    def _on_eval_token(self, token):
-        token = self._unwrap_token(token)
-        if "\n" in token:
-            mod = parse(token)
-            [*rest, last] = mod.body
-            assert isinstance(last, Expr), "{{ }} block must end with an expression, or you should use {# #} block"
-            self._buffer.extend(unparse(rest).splitlines())  # type: ignore
-            exp = unparse(last)
-        else:
-            exp = token
-        self._buffer.append(f"__append__({exp})")
-
-    def _on_exec_token(self, token):
-        self._buffer.extend(self._unwrap_token(token).splitlines())
-
-    def _on_special_token(self, token, sync: bool):
-        inner = self._unwrap_token(token)
-
-        if inner.startswith("end"):
-            last = self._ops_stack.pop()
-            assert last == inner.removeprefix("end")
-            self._flush()
-            self._builder.dedent()
-
-        else:
-            op = inner.split(" ", 1)[0]
-
-            if op == "if" or op == "for" or op == "while":
-                self._ops_stack.append(op)
-                self._flush()
-                self._builder.add_line(f"{inner}:")
-                self._builder.indent()
-
-            elif op == "else" or op == "elif":
-                self._flush()
-                self._builder.dedent()
-                self._builder.add_line(f"{inner}:")
-                self._builder.indent()
-
-            else:
-                params: str = self._make_context(inner)
-                if sync:
-                    self._buffer.append(f"__append__({op}.render({params}))")
-                else:
-                    self._buffer.append(f"__append__(await {op}.arender({params}))")
-
-    @staticmethod
-    def _make_context(text: str):
-        """generate context parameter if specified otherwise use locals() by default"""
-
-        return f"locals() | dict({text[text.index(' ') + 1:]})" if " " in text else "locals()"
-
-    def compile(self, sync=True, indent_str="\t"):
-        self._buffer = []
-        self._ops_stack = []
-        self._builder = get_base_builder(sync, indent_str)
-
-        for token in split_template_tokens(self.text):
-            if not token:
-                continue
-            s_token = token.strip()
-            if s_token.startswith("{{") and s_token.endswith("}}"):
-                self._on_eval_token(token)
-            elif s_token.startswith("{#") and s_token.endswith("#}"):
-                self._on_exec_token(token)
-            elif s_token.startswith("{%") and s_token.endswith("%}") and "\n" not in s_token:
-                self._on_special_token(token, sync)
-            else:
-                self._on_literal_token(token)
-
-        if self._ops_stack:
-            raise SyntaxError(self._ops_stack)
-
-        self._flush()
-        self._builder.add_line("return ''.join(map(str, __parts__))")
-        self._builder.dedent()
-
-    @cached_property
-    def _render_code(self):
-        self.compile()
-        return self._builder.get_render_function().__code__.replace(co_filename=str(self), co_name="render")
-
-    def render(self, context: Context) -> str:
-        return eval(self._render_code, context)
-
-    @cached_property
-    def _arender_code(self):
-        self.compile(sync=False)
-        return self._builder.get_render_function().__code__.replace(co_filename=str(self), co_name="arender")
-
-    async def arender(self, context: Context) -> str:
-        return await eval(self._arender_code, context)
-
-    def get_script(self, sync=True, indent_str="    "):
-        """compile template string into python script"""
-        self.compile(sync, indent_str)
-        return str(self._builder)
-
-
-class Loader(AutoNaming):
-    @classmethod
-    def read(cls, path: str | Path, encoding="utf-8"):
-        path = Path(path)
-        obj = cls(path.read_text(encoding))
-        obj.name = path.stem
-        return obj
-
-    @classmethod
-    async def aread(cls, path: str | Path, encoding="utf-8"):
-        from aiofiles import open
-
-        async with open(path, encoding=encoding) as f:
-            content = await f.read()
-
-        path = Path(path)
-        obj = cls(content)
-        obj.name = path.stem
-        return obj
-
-    @classmethod
-    def _patch_kwargs(cls, kwargs: dict) -> dict:
-        return {"headers": {"User-Agent": get_user_agent(cls)}} | kwargs
-
-    @staticmethod
-    def _join_url(url: str):
-        if url.startswith("http"):
-            return url
-
-        from urllib.parse import urljoin
-
-        return urljoin("https://promplate.dev/", url)
-
-    @classmethod
-    def fetch(cls, url: str, **kwargs):
-        from .utils import _get_client
-
-        response = _get_client().get(cls._join_url(url), **cls._patch_kwargs(kwargs))
-        obj = cls(response.raise_for_status().text)
-        obj.name = Path(url).stem
-        return obj
-
-    @classmethod
-    async def afetch(cls, url: str, **kwargs):
-        from .utils import _get_aclient
-
-        response = await _get_aclient().get(cls._join_url(url), **cls._patch_kwargs(kwargs))
-        obj = cls(response.raise_for_status().text)
-        obj.name = Path(url).stem
-        return obj
-
-
-class SafeChainMapContext(ChainMap, dict):
-    if TYPE_CHECKING:  # fix type from `collections.ChainMap`
-        from sys import version_info
-
-        if version_info >= (3, 11):
-            from typing_extensions import Self
-        else:
-            from typing import Self
-
-        copy: Callable[[Self], Self]
-
-
-class Template(TemplateCore, Loader):
-    def __init__(self, text: str, /, context: Context | None = None):
-        super().__init__(text)
-        self.context = {} if context is None else context
-
-    def render(self, context: Context | None = None):
-        if context is None:
-            context = SafeChainMapContext({}, self.context)
-        else:
-            context = SafeChainMapContext({}, context, self.context)
-
-        return super().render(context)
-
-    async def arender(self, context: Context | None = None):
-        if context is None:
-            context = SafeChainMapContext({}, self.context)
-        else:
-            context = SafeChainMapContext({}, context, self.context)
-
-        return await super().arender(context)
+from ast import Expr, parse, unparse
+from collections import ChainMap
+from functools import cached_property, partial
+from pathlib import Path
+from sys import path as sys_path
+from textwrap import dedent
+from typing import TYPE_CHECKING, Any, Literal, Protocol
+
+from .builder import *
+from .utils import *
+
+Context = dict[str, Any]  # globals must be a real dict
+
+
+class Component(Protocol):
+    def render(self, context: Context) -> str: ...
+
+    async def arender(self, context: Context) -> str: ...
+
+
+class TemplateCore(AutoNaming):
+    """A simple template compiler, for a jinja2-like syntax."""
+
+    def __init__(self, text: str):
+        """Construct a Templite with the given `text`."""
+
+        self.text = text
+
+    def _flush(self):
+        for line in self._buffer:
+            self._builder.add_line(line)
+        self._buffer.clear()
+
+    @staticmethod
+    def _unwrap_token(token: str):
+        return dedent(token.strip()[2:-2].strip("-")).strip()
+
+    def _on_literal_token(self, token: str):
+        self._buffer.append(f"__append__({repr(token)})")
+
+    def _on_eval_token(self, token):
+        token = self._unwrap_token(token)
+        if "\n" in token:
+            mod = parse(token)
+            [*rest, last] = mod.body
+            assert isinstance(last, Expr), "{{ }} block must end with an expression, or you should use {# #} block"
+            self._buffer.extend(unparse(rest).splitlines())  # type: ignore
+            exp = unparse(last)
+        else:
+            exp = token
+        self._buffer.append(f"__append__({exp})")
+
+    def _on_exec_token(self, token):
+        self._buffer.extend(self._unwrap_token(token).splitlines())
+
+    def _on_special_token(self, token, sync: bool):
+        inner = self._unwrap_token(token)
+
+        if inner.startswith("end"):
+            last = self._ops_stack.pop()
+            assert last == inner.removeprefix("end")
+            self._flush()
+            self._builder.dedent()
+
+        else:
+            op = inner.split(" ", 1)[0]
+
+            if op == "if" or op == "for" or op == "while":
+                self._ops_stack.append(op)
+                self._flush()
+                self._builder.add_line(f"{inner}:")
+                self._builder.indent()
+
+            elif op == "else" or op == "elif":
+                self._flush()
+                self._builder.dedent()
+                self._builder.add_line(f"{inner}:")
+                self._builder.indent()
+
+            else:
+                params: str = self._make_context(inner)
+                if sync:
+                    self._buffer.append(f"__append__({op}.render({params}))")
+                else:
+                    self._buffer.append(f"__append__(await {op}.arender({params}))")
+
+    @staticmethod
+    def _make_context(text: str):
+        """generate context parameter if specified otherwise use locals() by default"""
+
+        return f"locals() | dict({text[text.index(' ') + 1:]})" if " " in text else "locals()"
+
+    def compile(self, sync=True, indent_str="\t"):
+        self._buffer = []
+        self._ops_stack = []
+        self._builder = get_base_builder(sync, indent_str)
+
+        for token in split_template_tokens(self.text):
+            if not token:
+                continue
+            s_token = token.strip()
+            if s_token.startswith("{{") and s_token.endswith("}}"):
+                self._on_eval_token(token)
+            elif s_token.startswith("{#") and s_token.endswith("#}"):
+                self._on_exec_token(token)
+            elif s_token.startswith("{%") and s_token.endswith("%}") and "\n" not in s_token:
+                self._on_special_token(token, sync)
+            else:
+                self._on_literal_token(token)
+
+        if self._ops_stack:
+            raise SyntaxError(self._ops_stack)
+
+        self._flush()
+        self._builder.add_line("return ''.join(map(str, __parts__))")
+        self._builder.dedent()
+
+    error_handling: Literal["linecache", "tempfile", "file"] = "file" if __debug__ else "tempfile"
+
+    def _patch_for_error_handling(self, sync: bool):
+        match self.error_handling:
+            case "linecache":
+                add_linecache(self.name, partial(self.get_script, sync, "\t"))
+            case "file" | "tempfile":
+                file = save_tempfile(self.name, self.get_script(sync, "\t"), self.error_handling == "tempfile")
+                sys_path.append(str(file.parent))
+
+    @cached_property
+    def _render_code(self):
+        self.compile()
+        return self._builder.get_render_function().__code__.replace(co_filename=self.name, co_name="render")
+
+    def render(self, context: Context) -> str:
+        try:
+            return eval(self._render_code, context)
+        except Exception:
+            self._patch_for_error_handling(sync=True)
+            raise
+
+    @cached_property
+    def _arender_code(self):
+        self.compile(sync=False)
+        return self._builder.get_render_function().__code__.replace(co_filename=self.name, co_name="arender")
+
+    async def arender(self, context: Context) -> str:
+        try:
+            return await eval(self._arender_code, context)
+        except Exception:
+            self._patch_for_error_handling(sync=False)
+            raise
+
+    def get_script(self, sync=True, indent_str="    "):
+        """compile template string into python script"""
+        self.compile(sync, indent_str)
+        return str(self._builder)
+
+
+class Loader(AutoNaming):
+    @classmethod
+    def read(cls, path: str | Path, encoding="utf-8"):
+        path = Path(path)
+        obj = cls(path.read_text(encoding))
+        obj.name = path.stem
+        return obj
+
+    @classmethod
+    async def aread(cls, path: str | Path, encoding="utf-8"):
+        from aiofiles import open
+
+        async with open(path, encoding=encoding) as f:
+            content = await f.read()
+
+        path = Path(path)
+        obj = cls(content)
+        obj.name = path.stem
+        return obj
+
+    @classmethod
+    def _patch_kwargs(cls, kwargs: dict) -> dict:
+        return {"headers": {"User-Agent": get_user_agent(cls)}} | kwargs
+
+    @staticmethod
+    def _join_url(url: str):
+        if url.startswith("http"):
+            return url
+
+        from urllib.parse import urljoin
+
+        return urljoin("https://promplate.dev/", url)
+
+    @classmethod
+    def fetch(cls, url: str, **kwargs):
+        from .utils import _get_client
+
+        response = _get_client().get(cls._join_url(url), **cls._patch_kwargs(kwargs))
+        obj = cls(response.raise_for_status().text)
+        obj.name = Path(url).stem
+        return obj
+
+    @classmethod
+    async def afetch(cls, url: str, **kwargs):
+        from .utils import _get_aclient
+
+        response = await _get_aclient().get(cls._join_url(url), **cls._patch_kwargs(kwargs))
+        obj = cls(response.raise_for_status().text)
+        obj.name = Path(url).stem
+        return obj
+
+
+class SafeChainMapContext(ChainMap, dict):
+    if TYPE_CHECKING:  # fix type from `collections.ChainMap`
+        from sys import version_info
+
+        if version_info >= (3, 11):
+            from typing_extensions import Self
+        else:
+            from typing import Self
+
+        copy: Callable[[Self], Self]
+
+
+class Template(TemplateCore, Loader):
+    def __init__(self, text: str, /, context: Context | None = None):
+        super().__init__(text)
+        self.context = {} if context is None else context
+
+    def render(self, context: Context | None = None):
+        if context is None:
+            context = SafeChainMapContext({}, self.context)
+        else:
+            context = SafeChainMapContext({}, context, self.context)
+
+        return super().render(context)
+
+    async def arender(self, context: Context | None = None):
+        if context is None:
+            context = SafeChainMapContext({}, self.context)
+        else:
+            context = SafeChainMapContext({}, context, self.context)
+
+        return await super().arender(context)
```

### Comparing `promplate-0.3.4.5/promplate/prompt/utils.py` & `promplate-0.3.4.6/promplate/prompt/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,138 +1,162 @@
-from functools import cache, cached_property, wraps
-from inspect import currentframe, isclass
-from re import compile
-from typing import Any, Callable, ParamSpec, TypeVar
-
-split_template_tokens = compile(
-    r"((?:\s{%-|{%).*?(?:%}|-%}\s))|((?:\s{{-|{{)[\s\S]*?(?:}}|-}}\s))|((?:\s{#-|{#)[\s\S]*?(?:#}|-#}\s))"
-).split
-
-
-var_name_checker = compile(r"[_a-zA-Z]\w*$")
-
-is_message_start = compile(r"<\|\s?(user|system|assistant)\s?(\w{1,64})?\s?\|>")
-
-
-def is_not_valid(name: str):
-    return not var_name_checker.match(name)
-
-
-def ensure_valid(name):
-    if is_not_valid(name):
-        raise NameError(name)
-
-
-class AutoNaming:
-    def __new__(cls, *args, **kwargs):
-        obj = super().__new__(cls)
-        obj._bind_frame()
-        return obj
-
-    def _bind_frame(self):
-        self._frame = currentframe()
-
-    @cached_property
-    def _name(self):
-        f = self._frame
-        if f and f.f_back and (frame := f.f_back.f_back):
-            for name, var in frame.f_locals.items():
-                if var is self:
-                    return name
-
-    @property
-    def class_name(self):
-        return self.__class__.__name__
-
-    fallback_name = class_name
-
-    @property
-    def name(self):
-        return self._name or self.fallback_name
-
-    @name.setter
-    def name(self, name):
-        self._name = name
-        self._frame = None
-
-    @name.deleter
-    def name(self):
-        del self._name
-
-    def __repr__(self):
-        if self._name:
-            return f"<{self.class_name} {self.name}>"
-        else:
-            return f"<{self.class_name}>"
-
-    def __str__(self):
-        return f"<{self.name}>"
-
-
-P = ParamSpec("P")
-T = TypeVar("T")
-
-
-def cache_once(func: Callable[P, T]) -> Callable[P, T]:
-    result = None
-
-    @wraps(func)
-    def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
-        nonlocal result
-        if result is None:
-            result = func(*args, **kwargs)
-        return result
-
-    return wrapper
-
-
-@cache_once
-def get_builtins() -> dict[str, Any]:
-    return __builtins__ if isinstance(__builtins__, dict) else __builtins__.__dict__
-
-
-@cache
-def version(package: str):
-    from importlib.metadata import PackageNotFoundError, version
-
-    try:
-        return version(package)
-    except PackageNotFoundError:
-        return None
-
-
-@cache_once
-def get_user_agent(self, *additional_packages: tuple[str, str]):
-    from sys import version as py_version
-
-    return " ".join(
-        (
-            f"Promplate/{version('promplate')} ({self.__name__ if isclass(self) else self.__class__.__name__})",
-            *(f"{name}/{v}" for name, v in additional_packages),
-            f"HTTPX/{version('httpx') or '-'}",
-            f"Python/{py_version.split()[0]}",
-        )
-    )
-
-
-@cache_once
-def _is_http2_available():
-    try:
-        import h2  # type: ignore
-
-        return True
-    except ImportError:
-        return False
-
-
-@cache_once
-def _get_client():
-    from httpx import Client
-
-    return Client(follow_redirects=True, http2=_is_http2_available())
-
-
-@cache_once
-def _get_aclient():
-    from httpx import AsyncClient
-
-    return AsyncClient(follow_redirects=True, http2=_is_http2_available())
+from functools import cache, cached_property, wraps
+from inspect import currentframe, isclass
+from pathlib import Path
+from re import compile
+from typing import Any, Callable, ParamSpec, TypeVar
+
+split_template_tokens = compile(
+    r"((?:\s{%-|{%).*?(?:%}|-%}\s))|((?:\s{{-|{{)[\s\S]*?(?:}}|-}}\s))|((?:\s{#-|{#)[\s\S]*?(?:#}|-#}\s))"
+).split
+
+
+var_name_checker = compile(r"[_a-zA-Z]\w*$")
+
+is_message_start = compile(r"<\|\s?(user|system|assistant)\s?(\w{1,64})?\s?\|>")
+
+
+def is_not_valid(name: str):
+    return not var_name_checker.match(name)
+
+
+def ensure_valid(name):
+    if is_not_valid(name):
+        raise NameError(name)
+
+
+class AutoNaming:
+    def __new__(cls, *args, **kwargs):
+        obj = super().__new__(cls)
+        obj._bind_frame()
+        return obj
+
+    def _bind_frame(self):
+        self._frame = currentframe()
+
+    @cached_property
+    def _name(self):
+        f = self._frame
+        if f and f.f_back and (frame := f.f_back.f_back):
+            for name, var in frame.f_locals.items():
+                if var is self:
+                    return name
+
+    @property
+    def class_name(self):
+        return self.__class__.__name__
+
+    fallback_name = class_name
+
+    @property
+    def name(self):
+        return self._name or self.fallback_name
+
+    @name.setter
+    def name(self, name):
+        self._name = name
+        self._frame = None
+
+    @name.deleter
+    def name(self):
+        del self._name
+
+    def __repr__(self):
+        if self._name:
+            return f"<{self.class_name} {self.name}>"
+        else:
+            return f"<{self.class_name}>"
+
+    def __str__(self):
+        return f"<{self.name}>"
+
+
+P = ParamSpec("P")
+T = TypeVar("T")
+
+
+def cache_once(func: Callable[P, T]) -> Callable[P, T]:
+    result = None
+
+    @wraps(func)
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+        nonlocal result
+        if result is None:
+            result = func(*args, **kwargs)
+        return result
+
+    return wrapper
+
+
+@cache_once
+def get_builtins() -> dict[str, Any]:
+    return __builtins__ if isinstance(__builtins__, dict) else __builtins__.__dict__
+
+
+@cache
+def version(package: str):
+    from importlib.metadata import PackageNotFoundError, version
+
+    try:
+        return version(package)
+    except PackageNotFoundError:
+        return None
+
+
+@cache_once
+def get_user_agent(self, *additional_packages: tuple[str, str]):
+    from sys import version as py_version
+
+    return " ".join(
+        (
+            f"Promplate/{version('promplate')} ({self.__name__ if isclass(self) else self.__class__.__name__})",
+            *(f"{name}/{v}" for name, v in additional_packages),
+            f"HTTPX/{version('httpx') or '-'}",
+            f"Python/{py_version.split()[0]}",
+        )
+    )
+
+
+@cache_once
+def _is_http2_available():
+    try:
+        import h2  # type: ignore
+
+        return True
+    except ImportError:
+        return False
+
+
+@cache_once
+def _get_client():
+    from httpx import Client
+
+    return Client(follow_redirects=True, http2=_is_http2_available())
+
+
+@cache_once
+def _get_aclient():
+    from httpx import AsyncClient
+
+    return AsyncClient(follow_redirects=True, http2=_is_http2_available())
+
+
+def add_linecache(filename: str, source_getter: Callable[[], str]):
+    import linecache
+
+    linecache.cache[filename] = (source_getter,)
+
+
+def save_tempfile(filename: str, source: str, auto_deletion: bool):
+    from tempfile import mkdtemp
+
+    file = Path(mkdtemp(prefix="promplate-")) / filename
+    file.write_text(source)
+
+    if auto_deletion:
+        import atexit
+
+        @atexit.register
+        def _():
+            file.unlink(missing_ok=True)
+            file.parent.rmdir()
+
+    return file
```

### Comparing `promplate-0.3.4.5/pyproject.toml` & `promplate-0.3.4.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-[tool.poetry]
-name = "promplate"
-version = "0.3.4.5"
-description = "Prompt engineering framework for humans"
-homepage = "https://promplate.dev/"
-documentation = "https://docs.py.promplate.dev/"
-repository = "https://github.com/promplate/core"
-authors = ["Muspi Merol <me@promplate.dev>"]
-license = "MIT"
-readme = "README.md"
-keywords = ["prompt", "template", "nlp", "llm"]
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "Topic :: Text Processing :: Markup",
-    "Typing :: Typed",
-]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-typing-extensions = { version = "^4", python = "<3.12" }
-aiofiles = { version = "^23.2", optional = true }
-httpx = { version = ">=0.24, <1.0", optional = true }
-openai = { version = ">=0.27, <2.0", optional = true }
-
-[tool.poetry.extras]
-aiofiles = ["aiofiles"]
-httpx = ["httpx"]
-openai = ["openai"]
-all = ["aiofiles", "httpx", "openai"]
-
-[tool.poetry.group.dev.dependencies]
-isort = "^5"
-black = "^24"
-pytest = "^7"
-coverage = "^7"
-pytest-asyncio = "^0.23"
-
-[tool.pdm.scripts]
-format = { composite = ["isort ./{args}", "black ./{args}"] }
-test = "pytest"
-cov = { composite = ["coverage run -m pytest", "coverage report"] }
-
-[tool.isort]
-profile = "black"
-
-[tool.black]
-line-length = 130
-
-[tool.coverage.run]
-source = ["promplate"]
-branch = true
-
-[tool.coverage.report]
-fail_under = 45
-
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "promplate"
+version = "0.3.4.6"
+description = "Prompt engineering framework for humans"
+homepage = "https://promplate.dev/"
+documentation = "https://docs.py.promplate.dev/"
+repository = "https://github.com/promplate/core"
+authors = ["Muspi Merol <me@promplate.dev>"]
+license = "MIT"
+readme = "README.md"
+keywords = ["prompt", "template", "nlp", "llm"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence",
+    "Topic :: Text Processing :: Markup",
+    "Typing :: Typed",
+]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+typing-extensions = { version = "^4", python = "<3.12" }
+aiofiles = { version = "^23.2", optional = true }
+httpx = { version = ">=0.24, <1.0", optional = true }
+openai = { version = ">=0.27, <2.0", optional = true }
+
+[tool.poetry.extras]
+aiofiles = ["aiofiles"]
+httpx = ["httpx"]
+openai = ["openai"]
+all = ["aiofiles", "httpx", "openai"]
+
+[tool.poetry.group.dev.dependencies]
+isort = "^5"
+black = "^24"
+pytest = "^7"
+coverage = "^7"
+pytest-asyncio = "^0.23"
+
+[tool.pdm.scripts]
+format = { composite = ["isort ./{args}", "black ./{args}"] }
+test = "pytest"
+cov = { composite = ["coverage run -m pytest", "coverage report"] }
+
+[tool.isort]
+profile = "black"
+
+[tool.black]
+line-length = 130
+
+[tool.coverage.run]
+source = ["promplate"]
+branch = true
+
+[tool.coverage.report]
+fail_under = 45
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `promplate-0.3.4.5/README.md` & `promplate-0.3.4.6/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# Promplate
-
-```text
-</Promplate/> = <template> // prompt
-```
-
-**Promplate** is a prompting framework focusing on developing experience. However, it can also be a super-convenient SDK for simple LLM calls. Promplate progressively enhance your prompting workflow. And it values flexibility as well as perfect conventions. [Try online](https://promplate.dev/py)
-
-## Installation
-
-```shell
-pip install promplate
-```
-
-**Promplate** supports both CPython and PyPy, from `3.8` to `3.12`. It even supports running in browsers through wasm implementations of python.
-
-## Documentation
-
-You can visit our official docs site at [docs.py.promplate.dev](https://docs.py.promplate.dev/).
-
-## IDE Support 🌹
-
-**Promplate** is fully typed, which means static type checker will find bugs correctly (if you use `pyright` for type checking).
-
-We recommend using VS Code as your IDE when coding with promplate, because it natively uses pyright.
-
-The language design of promplate is similar to `Jinja2`. So you can use the `.j2` file extension for template files for syntax highlight.
-
-## Development
-
-- use `poetry` to manage dependencies.
-- use `isort` to sort import statements.
-- use `black` to format code.
-- use `pyright` to check type annotations.
-
-Development should be done on `dev` branch, using `>=3.10` language features. The `master` branch is used for `py3.8` compatible releases.
-
-**Promplate** is well tested with `pytest`. GitHub Actions are used to run tests and linting. And there are test results continually generated on [Vercel(py3.9)](https://promplate-core.vercel.app/) and [Netlify(py3.8)](https://promplate-core.netlify.app/). There is [a coverage report](https://promplate-python-coverage.onrender.com/) too.
-
-## Future Features (or TODOs?)
-
-- [ ] more documentation
-- [ ] javascript implementation
-- [ ] improve error handling
-  - possible ways would be similar to [`Jinja2`](https://github.com/pallets/jinja/blob/main/src/jinja2/debug.py)
+# Promplate
+
+```text
+</Promplate/> = <template> // prompt
+```
+
+**Promplate** is a prompting framework focusing on developing experience. However, it can also be a super-convenient SDK for simple LLM calls. Promplate progressively enhance your prompting workflow. And it values flexibility as well as perfect conventions. [Try online](https://promplate.dev/py)
+
+## Installation
+
+```shell
+pip install promplate
+```
+
+**Promplate** supports both CPython and PyPy, from `3.8` to `3.12`. It even supports running in browsers through wasm implementations of python.
+
+## Documentation
+
+You can visit our official docs site at [docs.py.promplate.dev](https://docs.py.promplate.dev/).
+
+## IDE Support 🌹
+
+**Promplate** is fully typed, which means static type checker will find bugs correctly (if you use `pyright` for type checking).
+
+We recommend using VS Code as your IDE when coding with promplate, because it natively uses pyright.
+
+The language design of promplate is similar to `Jinja2`. So you can use the `.j2` file extension for template files for syntax highlight.
+
+## Development
+
+- use `poetry` to manage dependencies.
+- use `isort` to sort import statements.
+- use `black` to format code.
+- use `pyright` to check type annotations.
+
+Development should be done on `dev` branch, using `>=3.10` language features. The `master` branch is used for `py3.8` compatible releases.
+
+**Promplate** is well tested with `pytest`. GitHub Actions are used to run tests and linting. And there are test results continually generated on [Vercel(py3.9)](https://promplate-core.vercel.app/) and [Netlify(py3.8)](https://promplate-core.netlify.app/). There is [a coverage report](https://promplate-python-coverage.onrender.com/) too.
+
+## Future Features (or TODOs?)
+
+- [ ] more documentation
+- [ ] javascript implementation
+- [x] improved error handling
+  - display compiled code when error occurs through `linecache` or `tempfile` (default)
```

### Comparing `promplate-0.3.4.5/PKG-INFO` & `promplate-0.3.4.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promplate
-Version: 0.3.4.5
+Version: 0.3.4.6
 Summary: Prompt engineering framework for humans
 Home-page: https://promplate.dev/
 License: MIT
 Keywords: prompt,template,nlp,llm
 Author: Muspi Merol
 Author-email: me@promplate.dev
 Requires-Python: >=3.10,<4.0
@@ -68,10 +68,10 @@
 
 **Promplate** is well tested with `pytest`. GitHub Actions are used to run tests and linting. And there are test results continually generated on [Vercel(py3.9)](https://promplate-core.vercel.app/) and [Netlify(py3.8)](https://promplate-core.netlify.app/). There is [a coverage report](https://promplate-python-coverage.onrender.com/) too.
 
 ## Future Features (or TODOs?)
 
 - [ ] more documentation
 - [ ] javascript implementation
-- [ ] improve error handling
-  - possible ways would be similar to [`Jinja2`](https://github.com/pallets/jinja/blob/main/src/jinja2/debug.py)
+- [x] improved error handling
+  - display compiled code when error occurs through `linecache` or `tempfile` (default)
```

