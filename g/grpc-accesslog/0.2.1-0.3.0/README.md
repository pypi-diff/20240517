# Comparing `tmp/grpc_accesslog-0.2.1.tar.gz` & `tmp/grpc_accesslog-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_accesslog-0.2.1.tar", max compression
+gzip compressed data, was "grpc_accesslog-0.3.0.tar", max compression
```

## Comparing `grpc_accesslog-0.2.1.tar` & `grpc_accesslog-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1086 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/LICENSE.rst
--rw-r--r--   0        0        0     3009 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/README.rst
--rw-r--r--   0        0        0     1965 2024-05-14 23:27:56.451378 grpc_accesslog-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      162 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/__init__.py
--rw-r--r--   0        0        0      340 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/_context.py
--rw-r--r--   0        0        0     6750 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/_server.py
--rw-r--r--   0        0        0     3358 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/handlers.py
--rw-r--r--   0        0        0        0 2024-05-14 23:27:43.247405 grpc_accesslog-0.2.1/src/grpc_accesslog/py.typed
--rw-r--r--   0        0        0     3874 1970-01-01 00:00:00.000000 grpc_accesslog-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/LICENSE.rst
+-rw-r--r--   0        0        0     2983 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/README.rst
+-rw-r--r--   0        0        0     2017 2024-05-17 02:52:34.376477 grpc_accesslog-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/src/grpc_accesslog/__init__.py
+-rw-r--r--   0        0        0     2595 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/src/grpc_accesslog/_async_server.py
+-rw-r--r--   0        0        0      340 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/src/grpc_accesslog/_context.py
+-rw-r--r--   0        0        0     6244 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/src/grpc_accesslog/_server.py
+-rw-r--r--   0        0        0     3543 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/src/grpc_accesslog/handlers.py
+-rw-r--r--   0        0        0        0 2024-05-17 02:52:21.916522 grpc_accesslog-0.3.0/src/grpc_accesslog/py.typed
+-rw-r--r--   0        0        0     3798 1970-01-01 00:00:00.000000 grpc_accesslog-0.3.0/PKG-INFO
```

### Comparing `grpc_accesslog-0.2.1/LICENSE.rst` & `grpc_accesslog-0.3.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `grpc_accesslog-0.2.1/README.rst` & `grpc_accesslog-0.3.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 * Write stdout logs for every RPC request
 * Log messages built with customizable callback handlers
 
 
 Requirements
 ------------
 
-* Python 3.8+
-* grpc-interceptors 0.13+
+* Python 3.9+
 
 
 Installation
 ------------
 
 You can install *gRPC Access Log* via pip_ from PyPI_:
```

### Comparing `grpc_accesslog-0.2.1/pyproject.toml` & `grpc_accesslog-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grpc-accesslog"
-version = "0.2.1"
+version = "0.3.0"
 description = "gRPC Access Log"
 authors = ["Michael Morgan <git@morgan83.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/villainy/grpc-accesslog"
 repository = "https://github.com/villainy/grpc-accesslog"
 documentation = "https://grpc-accesslog.readthedocs.io"
@@ -12,42 +12,44 @@
     "Development Status :: 4 - Beta",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/villainy/grpc-accesslog/releases"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 grpcio = "^1.56.2"
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.7"
 black = ">=24.1.0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
-flake8 = ">=4.0.1"
+flake8 = ">=6.1.0"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.930"
 pep8-naming = ">=0.12.1"
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
-protobuf = "^4.23.4"
+protobuf = "^5.26.1"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
-sphinx = ">=4.3.2"
+sphinx = ">=7.3.7"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
 types-protobuf = "^4.23.0.2"
+grpc-stubs = "^1.53.0.5"
+pytest-asyncio = "^0.23.6"
 
 [tool.poetry.scripts]
 grpc-accesslog = "grpc_accesslog.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
```

### Comparing `grpc_accesslog-0.2.1/src/grpc_accesslog/_server.py` & `grpc_accesslog-0.3.0/src/grpc_accesslog/_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 """gRPC access log server interceptor."""
 
 import logging
 from datetime import datetime
 from datetime import timezone
 from typing import Any
 from typing import Callable
-from typing import Iterable
-from typing import Iterator
+from typing import List
 from typing import Optional
+from typing import TypeVar
 from typing import Union
 
 import grpc
 
-from . import handlers as _handlers
 from ._context import LogContext
+from .handlers import DEFAULT_HANDLERS
+from .handlers import THandler
+
+
+TRequest = TypeVar("TRequest")
+TResponse = TypeVar("TResponse")
 
 
 def _wrap_rpc_behavior(
     handler: Union[grpc.RpcMethodHandler, None],
     continuation: Callable[
         [
-            Callable[[Any, grpc.ServicerContext], Any],
+            Callable[[TRequest, grpc.ServicerContext], TResponse],
             bool,
             bool,
         ],
-        Callable[[Any, grpc.ServicerContext], Any],
+        Callable[[TRequest, grpc.ServicerContext], TResponse],
     ],
 ) -> Union[grpc.RpcMethodHandler, None]:
     """Wrap an RPC call.
 
     From https://github.com/grpc/grpc/issues/18191#issuecomment-574735994
     """
     if handler is None:
@@ -45,165 +50,146 @@
         handler_factory = grpc.unary_stream_rpc_method_handler
     else:
         behavior_fn = handler.unary_unary
         handler_factory = grpc.unary_unary_rpc_method_handler
 
     return handler_factory(
         continuation(
-            behavior_fn,
+            behavior_fn,  # type: ignore
             handler.request_streaming,
             handler.response_streaming,
         ),
         request_deserializer=handler.request_deserializer,
         response_serializer=handler.response_serializer,
     )
 
 
-class AccessLogInterceptor(grpc.ServerInterceptor):
-    """Generate a log line for each RPC invocation."""
+class AccessLogger:
+    """Access log writer."""
 
     def __init__(
         self,
         level: int = logging.INFO,
         name: str = __name__,
-        handlers: Optional[Iterable[Callable[[LogContext], str]]] = None,
+        handlers: List[THandler] = DEFAULT_HANDLERS,
         separator: str = " ",
         propagate: bool = False,
         logger: Optional[logging.Logger] = None,
     ) -> None:
-        """Create a logging interceptor.
+        """Create an access logging writer.
 
         Each provided handler will be called in order with a LogContext as
         the single positional argument. The resulting strings are joined
         using the provided separator to form the access log message.
 
         Args:
             level (int): Log level. Defaults to logging.INFO.
             name (str): Logger name. Defaults to __name__.
-            handlers (Iterable[Callable[[LogContext], str]]): LogContext
+            handlers (List[THandler]): LogContext
                 handlers collected in order. Defaults to None.
             separator (str): Log message separator. Defaults to " ".
             propagate (bool): Enable propagation to parent loggers. Defaults to False.
             logger (logging.Logger): The logger instance to use for access
                 logs. Optional, defaults to None.
         """
-        super().__init__()
-
         if logger is None:
             self._logger = logging.getLogger(name)
             self._logger.propagate = propagate
             self._logger.addHandler(logging.StreamHandler())
         else:
             self._logger = logger
 
         self._level = level
-        self._format = format
         self._handlers = handlers
         self._separator = separator
 
-        if handlers is None:
-            self._handlers = [
-                _handlers.peer,
-                _handlers.time_received(),
-                _handlers.request,
-                _handlers.status,
-                _handlers.response_size,
-                _handlers.user_agent,
-            ]
-
-    def _write_log(
+    def log(
         self,
         context: grpc.ServicerContext,
         method_name: str,
         request: Any,
         response: Optional[Any],
         start: datetime,
         end: datetime,
     ) -> None:
+        """Write a log line to stdout."""
         log_context = LogContext(
             context,
             method_name,
             request,
             response,
             start,
             end,
         )
 
-        if self._handlers is None:
+        if not self._handlers:
             return
 
         log_args = [handler(log_context) for handler in self._handlers]
 
         self._logger.log(
             self._level,
             self._separator.join(["%s"] * len(log_args)),
             *log_args,
         )
 
+
+class AccessLogInterceptor(grpc.ServerInterceptor, AccessLogger):
+    """Generate a log line for each RPC invocation."""
+
     def intercept_service(
         self,
         continuation: Callable[
             [grpc.HandlerCallDetails],
-            grpc.RpcMethodHandler,
+            Union[grpc.RpcMethodHandler, None],
         ],
         handler_call_details: grpc.HandlerCallDetails,
     ) -> Union[grpc.RpcMethodHandler, None]:
         """Intercept an RPC."""
 
         def logging_wrapper(
             behavior: Callable[[Any, grpc.ServicerContext], Any],
             request_streaming: bool,
             response_streaming: bool,
         ) -> Callable[[Any, grpc.ServicerContext], Any]:
             def logging_interceptor(
                 request_or_iterator: Any, context: grpc.ServicerContext
             ) -> Any:
-                # handle streaming responses specially
-                if response_streaming:
-                    return self._intercept_server_stream(
-                        behavior,
-                        handler_call_details,
-                        request_or_iterator,
-                        context,
-                    )
-
                 start = datetime.now(timezone.utc)
                 response = None
                 try:
                     response = behavior(request_or_iterator, context)
                     return response
                 finally:
                     end = datetime.now(timezone.utc)
-                    self._write_log(
+                    self.log(
                         context,
                         handler_call_details.method,
                         request_or_iterator,
                         response,
                         start,
                         end,
                     )
 
+            def logging_interceptor_stream(
+                request_or_iterator: Any, context: grpc.ServicerContext
+            ) -> Any:
+                start = datetime.now(timezone.utc)
+                try:
+                    yield from behavior(request_or_iterator, context)
+                finally:
+                    end = datetime.now(timezone.utc)
+                    self.log(
+                        context,
+                        handler_call_details.method,
+                        request_or_iterator,
+                        None,
+                        start,
+                        end,
+                    )
+
+            if response_streaming:
+                return logging_interceptor_stream
+
             return logging_interceptor
 
         return _wrap_rpc_behavior(continuation(handler_call_details), logging_wrapper)
-
-    def _intercept_server_stream(
-        self,
-        behavior: Callable[[Any, grpc.ServicerContext], Iterator[Any]],
-        handler_call_details: grpc.HandlerCallDetails,
-        request_or_iterator: Any,
-        context: grpc.ServicerContext,
-    ) -> Iterator[Any]:
-        start = datetime.now(timezone.utc)
-        try:
-            yield from behavior(request_or_iterator, context)
-        finally:
-            end = datetime.now(timezone.utc)
-            self._write_log(
-                context,
-                handler_call_details.method,
-                request_or_iterator,
-                # TODO what to do with streaming responses?
-                None,
-                start,
-                end,
-            )
```

### Comparing `grpc_accesslog-0.2.1/src/grpc_accesslog/handlers.py` & `grpc_accesslog-0.3.0/src/grpc_accesslog/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 """gRPC access log handlers."""
 
 from datetime import timedelta
 from typing import Callable
+from typing import List
 
 import grpc
 
 from ._context import LogContext
 
 
+THandler = Callable[[LogContext], str]
+
+
 def time_received(
     format: str = "[%d/%b/%Y:%H:%M:%S %z]",
-) -> Callable[[LogContext], str]:
+) -> THandler:
     """Parse RPC request received time into a strftime formatted string.
 
     Args:
         format (str): String format. Defaults to "[%d/%b/%Y:%H:%M:%S %z]".
 
     Returns:
-        Callable[[LogContext], str]: LogContext handler
+        THandler: LogContext handler
     """
 
     def inner(context: LogContext) -> str:
         return context.start.strftime(format)
 
     return inner
 
 
 def time_complete(
     format: str = "[%d/%b/%Y:%H:%M:%S %z]",
-) -> Callable[[LogContext], str]:
+) -> THandler:
     """Parse RPC request completion time into a strftime formatted string.
 
     Args:
         format (str): String format. Defaults to "[%d/%b/%Y:%H:%M:%S %z]".
 
     Returns:
-        Callable[[LogContext], str]: LogContext handler
+        THandler: LogContext handler
     """
 
     def inner(context: LogContext) -> str:
         return context.end.strftime(format)
 
     return inner
 
@@ -77,16 +81,17 @@
 
     Returns:
         str: gRPC status code name
     """
     code = grpc.StatusCode.OK.name
     # TODO gRPC status code is not exposed publicly anywhere in the server
     # interceptor's context
-    if context.server_context._state.code:  # type: ignore
-        code = context.server_context._state.code.name  # type: ignore
+    if getattr(context.server_context, "_state", None):
+        if context.server_context._state.code:  # type: ignore
+            code = context.server_context._state.code.name  # type: ignore
 
     return str(code)
 
 
 def peer(context: LogContext) -> str:
     """Return parsed client IP when available.
 
@@ -132,7 +137,17 @@
         str: User agent string
     """
     for metadata in context.server_context.invocation_metadata():
         if getattr(metadata, "key", "").lower() == "user-agent":
             return str(getattr(metadata, "value", "-"))
 
     return "-"
+
+
+DEFAULT_HANDLERS: List[THandler] = [
+    peer,
+    time_received(),
+    request,
+    status,
+    response_size,
+    user_agent,
+]
```

### Comparing `grpc_accesslog-0.2.1/PKG-INFO` & `grpc_accesslog-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: grpc-accesslog
-Version: 0.2.1
+Version: 0.3.0
 Summary: gRPC Access Log
 Home-page: https://github.com/villainy/grpc-accesslog
 License: MIT
 Author: Michael Morgan
 Author-email: git@morgan83.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: grpcio (>=1.56.2,<2.0.0)
 Project-URL: Changelog, https://github.com/villainy/grpc-accesslog/releases
 Project-URL: Documentation, https://grpc-accesslog.readthedocs.io
 Project-URL: Repository, https://github.com/villainy/grpc-accesslog
@@ -64,16 +63,15 @@
 * Write stdout logs for every RPC request
 * Log messages built with customizable callback handlers
 
 
 Requirements
 ------------
 
-* Python 3.8+
-* grpc-interceptors 0.13+
+* Python 3.9+
 
 
 Installation
 ------------
 
 You can install *gRPC Access Log* via pip_ from PyPI_:
```

