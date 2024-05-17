# Comparing `tmp/WrenchCL-1.9.1.tar.gz` & `tmp/WrenchCL-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WrenchCL-1.9.1.tar", last modified: Wed Mar  6 21:33:46 2024, max compression
+gzip compressed data, was "WrenchCL-2.0.0.tar", last modified: Fri May 17 06:29:11 2024, max compression
```

## Comparing `WrenchCL-1.9.1.tar` & `WrenchCL-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.109665 WrenchCL-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/WrenchCL/
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/ApiSuperClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/ChatGptSuperClass.py
--rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/RdsSuperClass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/WrenchCL/Utility/
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/Utility/ConsoleAnimation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/Utility/MaybeMonad.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/Utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24808 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/WrenchLogger.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-06 21:33:13.000000 WrenchCL-1.9.1/WrenchCL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:46.105665 WrenchCL-1.9.1/WrenchCL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9770 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 21:33:46.000000 WrenchCL-1.9.1/WrenchCL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:33:46.109665 WrenchCL-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-03-06 21:33:44.000000 WrenchCL-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21640 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.692785 WrenchCL-2.0.0/WrenchCL/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Classes/_ConfigurationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Classes/_SshTunnelManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Connect/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/AWSClientHub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/RdsServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/S3ServiceGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)     3654 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/Retryable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/SingletonClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/TimedMethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Decorators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/build_return_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9119 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/handle_lambda_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Helpers/trigger_dataflow_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/OpenAIFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/OpenAIGateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/_ConversationManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/WrenchCL/Tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/Coalesce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/DictValidator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/FetchMetaData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/FileTyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/Image2B64.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/MaybeMonad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26396 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/WrenchLogger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-17 06:28:45.000000 WrenchCL-2.0.0/WrenchCL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:29:11.692785 WrenchCL-2.0.0/WrenchCL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22310 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 06:29:11.000000 WrenchCL-2.0.0/WrenchCL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:29:11.696785 WrenchCL-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-17 06:29:10.000000 WrenchCL-2.0.0/setup.py
```

### Comparing `WrenchCL-1.9.1/WrenchCL/WrenchLogger.py` & `WrenchCL-2.0.0/WrenchCL/Tools/WrenchLogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,49 @@
+#  Copyright (c) $YEAR$. Copyright (c) $YEAR$ Wrench.AI., Willem van der Schans, Jeong Kim
+#
+#  MIT License
+#
+#  Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+#
+#  The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+#
+#  THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+#
+#  All works within the Software are owned by their respective creators and are distributed by Wrench.AI.
+#
+#  For inquiries, please contact Willem van der Schans through the official Wrench.AI channels or directly via GitHub at [Kydoimos97](https://github.com/Kydoimos97).
+#
+
 import json
 import logging
 import os
 import random
 import string
 import sys
 import time
-from datetime import datetime, timedelta
 import traceback
+from datetime import datetime, timedelta
 from textwrap import fill
 from typing import Any, Optional
 
-import pandas as pd
+from Decorators.SingletonClass import SingletonClass
 
 try:
     from colorama import init, Fore as ColoramaFore, Style as ColoramaStyle
 
     colorama_imported = True
 except ImportError:
     colorama_imported = False
     logging.warning("colorama package not found. Colored logging is disabled.")
 
-
+@SingletonClass
 class _wrench_logger:
-    _instance = None
-
-    # Lifecycle Methods
-    def __new__(cls, *args: Any, **kwargs: Any) -> 'log':
-        """
-        Implement the Singleton pattern to ensure a single instance per unique combination of `level` and `file_name_append_mode`.
-        """
-        if cls._instance is None:
-            cls._instance = super(_wrench_logger, cls).__new__(cls)
-        return cls._instance
 
     def __init__(self, level: str = 'INFO', file_logging=False, file_name_append_mode: Optional[str] = None) -> None:
         self._start_time = None
-        if hasattr(self, '_initialized'):  # Check if __init__ has been called before
-            return  # If yes, do nothing
-
         self.run_id = self._generate_run_id()
         self.running_on_lambda = 'AWS_LAMBDA_FUNCTION_NAME' in os.environ
         self.previous_level = None
         self.file_logging = file_logging
         self.base_format = self._get_base_format()
         self.logging_level = self._set_logging_level(level)
         if self.file_logging:
@@ -156,149 +158,158 @@
     # Main Functional Methods
     def _log(self, level: int, msg: str, stack_info: bool = False) -> None:
         # Initialize stack_level_index
         stack_level_index = 1
         stack_trace = " --> InternalLogFrames"
         last_level = ""
         write_flag = False
+        match_counter = 0
         filepath_out, line_no_out, func_name_out, sinfo_out = self.logger.findCaller(stack_info=stack_info,
                                                                                      stacklevel=stack_level_index)
+        if stack_level_index == 1:
+            first_index = f"{filepath_out}:{func_name_out}:{line_no_out}"
         # Loop to find the caller
-        while stack_level_index < (1000 if str(traceback.format_exc()) != "NoneType: None\n" else 1000):
+        while stack_level_index:
             filepath, line_no, func_name, sinfo = self.logger.findCaller(stack_info=stack_info,
                                                                          stacklevel=stack_level_index)
-            if f"{filepath}:{func_name}:{line_no}" != last_level:
+            if f"{filepath}:{func_name}:{line_no}" != last_level and (
+                    f"{filepath}:{func_name}:{line_no}" != first_index or stack_level_index == 1):
+                match_counter = 0
                 if self.running_on_lambda:
                     stack_trace = stack_trace + f" <-- {stack_level_index}|{os.path.basename(filepath)}:{func_name}:{line_no}"
                 else:
                     stack_trace = stack_trace + f"\n -- {stack_level_index}|{os.path.basename(filepath)}:{func_name}:{line_no}"
-                stack_level_index += 1
                 last_level = f"{filepath}:{func_name}:{line_no}"
 
-                if write_flag is False:
+                if write_flag is False and not self._is_internal_frame(os.path.normpath(filepath)):
                     filepath_out, line_no_out, func_name_out, sinfo_out = self.logger.findCaller(stack_info=stack_info,
                                                                                                  stacklevel=stack_level_index)
                     write_flag = True
-                if stack_info is True:
-                    continue
-                else:
-                    break
-            if self._is_internal_frame(os.path.normpath(filepath)):
+            else:
+                match_counter += 1
+            if self._is_internal_frame(os.path.normpath(filepath)) and match_counter <= 5:
                 stack_level_index += 1
                 continue
             else:
                 break
 
         # Handle stack_info
         if stack_info:
             if str(traceback.format_exc()) != "NoneType: None\n":
-                sinfo = f"\n ---Stack Trace--- {stack_trace[4:]} \n {traceback.format_exc()}"
+                if colorama_imported:
+                    sinfo = f"\n ---Stack Trace--- \n {ColoramaFore.LIGHTBLACK_EX} {stack_trace[4:]} \n {ColoramaFore.RESET} ---Python Traceback--- {ColoramaFore.LIGHTBLACK_EX}\n {traceback.format_exc()} {ColoramaFore.RESET}"
+                else:
+                    sinfo = f"\n ---Stack Trace--- \n {stack_trace[4:]} \n ---Python Traceback--- \n {traceback.format_exc()}"
             else:
-                sinfo = f"Stack Trace: {self._format_data(stack_trace[4:], stack_trace = True)}"
+                sinfo = f"Stack Trace: {self._format_data(stack_trace[4:], stack_trace=True)}"
         else:
             sinfo = None
 
         # Create and handle the log record
-        record = self.logger.makeRecord(
-            name=self.logger.name,
-            level=level,
-            fn=filepath_out,
-            lno=line_no_out,
-            msg=msg,
-            args=None,
-            exc_info=None,
-            func=func_name_out,
-            sinfo=sinfo
-        )
+        record = self.logger.makeRecord(name=self.logger.name, level=level, fn=filepath_out, lno=line_no_out, msg=msg,
+            args=None, exc_info=None, func=func_name_out, sinfo=sinfo)
         self.logger.handle(record)
 
     def _log_with_color(self, level: int, text: str, color: Optional[str] = None,
-                        stack_info: Optional[bool] = False) -> None:
+            stack_info: Optional[bool] = False) -> None:
         if colorama_imported and color and not self.running_on_lambda:
             self._handlerFormat(color)
 
         if self.force_stack_trace and level >= 30:
             stack_info = True
         self._log(level, text, stack_info)
 
         if colorama_imported or self.running_on_lambda:
             self._handlerFormat()
 
-    def info(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def info(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log information that might be helpful but isn't essential."""
+        text = ' '.join(args)
         self._log_with_color(logging.INFO, text, ColoramaFore.LIGHTGREEN_EX if colorama_imported else None, stack_info)
 
     log_info = INFO = info  # Aliases for info
 
-    def context(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def context(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log contextual information for better understanding of the flow."""
+        text = ' '.join(args)
         self._log_with_color(21, text, ColoramaFore.LIGHTMAGENTA_EX if colorama_imported else None, stack_info)
 
     log_context = CONTEXT = context  # Aliases for context
 
-    def warning(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def warning(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log issues that aren't errors but might warrant investigation."""
+        text = ' '.join(args)
         self._log_with_color(logging.WARNING, text, ColoramaFore.YELLOW if colorama_imported else None, stack_info)
 
     log_warning = WARNING = warning  # Aliases for warning
 
-    def HDL_WARN(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def HDL_WARN(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log warnings that have been handled and do not require further action."""
+        text = ' '.join(args)
         self._log_with_color(31, text, ColoramaFore.MAGENTA if colorama_imported else None, stack_info)
 
     log_handled_warning = log_hdl_warn = HDL_WARN  # Aliases for HDL_WARN
 
-    def error(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def error(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log errors that could disrupt normal program flow."""
+        text = ' '.join(args)
         self._log_with_color(logging.ERROR, text, ColoramaFore.RED if colorama_imported else None, stack_info)
 
     log_error = ERROR = error  # Aliases for error
 
     def data(self, data: Any, wrap_length: Optional[int] = None, max_rows: Optional[int] = None,
-             stack_info: Optional[bool] = False) -> None:
+            stack_info: Optional[bool] = False) -> None:
         """Log Data in a lower contrast, handling formatting for readability."""
         formatted_data = self._format_data(data, wrap_length, max_rows)
         self._log_with_color(41, formatted_data, ColoramaFore.LIGHTWHITE_EX if colorama_imported else None, stack_info)
 
     log_data = print_data = DATA = data
 
-    def HDL_ERR(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def HDL_ERR(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log errors that have been handled but still need to be reported."""
+        text = ' '.join(args)
         self._log_with_color(42, text, ColoramaFore.LIGHTMAGENTA_EX if colorama_imported else None, stack_info)
 
     log_handled_error = log_hdl_err = HDL_ERR  # Aliases for HDL_ERR
 
-    def RECV_ERR(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def RECV_ERR(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log errors from which the system can recover with or without manual intervention."""
+        text = ' '.join(args)
         self._log_with_color(43, text, ColoramaFore.LIGHTRED_EX if colorama_imported else None, stack_info)
 
     log_recoverable_error = log_recv_err = RECV_ERR  # Aliases for RECV_ERR
 
-    def critical(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def critical(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log critical issues that require immediate attention."""
-        self._log_with_color(logging.CRITICAL, text, ColoramaFore.RED if colorama_imported else None,
-                             stack_info)
+        text = ' '.join(args)
+        self._log_with_color(logging.CRITICAL, text, ColoramaFore.RED if colorama_imported else None, stack_info)
 
     log_critical = CRITICAL = critical  # Aliases for critical
 
-    def debug(self, text: str, stack_info: Optional[bool] = False) -> None:
+    def debug(self, *args: str, stack_info: Optional[bool] = False) -> None:
         """Log detailed information, typically of interest only when diagnosing problems."""
+        text = ' '.join(args)
         self._log_with_color(logging.DEBUG, text, ColoramaFore.CYAN if colorama_imported else None, stack_info)
 
     log_debug = DEBUG = debug  # Aliases for debug
 
     # Formatting Methods
 
     def _format_data(self, data, wrap_length=None, max_rows=None, color=True, stack_trace=False):
         """Format data for logging, applying wrapping and color formatting where applicable."""
         # Determine the prefix based on the data type
+        try:
+            import pandas as pd
+        except ImportError:
+            pd = None
+
         if isinstance(data, dict):
             prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
             formatted_text = json.dumps(data, indent=4)
-        elif isinstance(data, pd.DataFrame):
+        elif pd and isinstance(data, pd.DataFrame):
             prefix_str = f"DataType: {type(data).__name__} | Shape: {data.shape[0]} rows | {data.shape[1]} columns"
             with pd.option_context('display.max_rows', max_rows, 'display.max_columns', None):
                 formatted_text = str(data)
         elif isinstance(data, (list, tuple, set)):
             prefix_str = f"DataType: {type(data).__name__} | Length: {len(data)}"
             formatted_text = '\n'.join([str(item) for item in data])
         else:
@@ -402,18 +413,19 @@
 
     def compact_header(self, text, size=40):
         self.header(text, size, False, )
 
     # Private Utility Methods
     @staticmethod
     def _is_internal_frame(filepath: str) -> bool:
-        check_strs = ['logging', 'wrenchlogger', 'pycaller', 'wrench_logger']
+        check_strs = ['WrenchLogger.py', '_pytest']
         end_strs = ['__init__.py']
+
         for cstr in check_strs:
-            if cstr in filepath.lower():
+            if cstr in filepath:
                 return True
 
         for estr in end_strs:
             if filepath.lower().endswith(estr):
                 return True
 
         return False
@@ -424,16 +436,15 @@
 
         Returns:
             logging.Formatter: A logging formatter with a predefined format and date format.
         """
         return logging.Formatter(f"%(levelname)-8s: [{self.run_id}]"
                                  f"%(filename)s:%(funcName)s:%(lineno)d | "
                                  f"%(asctime)s | "
-                                 f"%(message)s",
-                                 datefmt='%Y-%m-%d %H:%M:%S')
+                                 f"%(message)s", datefmt='%Y-%m-%d %H:%M:%S')
 
     @staticmethod
     def _set_logging_level(level: str) -> int:
         """
         Converts a logging level string to its corresponding logging level constant.
 
         Parameters:
@@ -542,15 +553,15 @@
             self.logger.addHandler(self.file_handler)
 
         self.logger.addHandler(self.console_handler)
 
         # Initialize colorama for colorful output if not running on AWS Lambda
         if colorama_imported and not self.running_on_lambda:
             init()
-        
+
     def start_time(self):
         """Start a timer for performance measurement."""
         self._start_time = time.time()
 
     def log_time(self, message: str = "Elapsed time", format: str = "seconds", stack_info: Optional[bool] = False):
         """
         Log the elapsed time since start_time() was called with an optional message.
@@ -574,11 +585,10 @@
 
             self.info(f"{message}: {time_str}", stack_info)
         else:
             self.warning("Timer was not started with start_time() before calling log_time().")
 
     # Alias for log_time
     Time = log_time
-        
-        
 
-wrench_logger = _wrench_logger()
+
+logger = _wrench_logger()
```

### Comparing `WrenchCL-1.9.1/setup.py` & `WrenchCL-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,16 +25,22 @@
         requires_path = os.path.join(egg_info_folder, 'requires.txt')
         if os.path.exists(requires_path):
             with open(requires_path, "r") as f:
                 required = f.read().splitlines()
 
 setup(
     name='WrenchCL',
-    version='v1.9.1',
+    version='v2.0.0',
     author='willem@wrench.ai',
-    description='This is a code library designed to improve code re-usability and standardize access to APIs, RDS, and logging functionalities',
+    description='WrenchCL is a comprehensive library designed to facilitate seamless interactions with AWS services, OpenAI models, and various utility tools. This package aims to streamline the development process by providing robust components for database interactions, cloud storage, and AI-powered functionalities.',
     long_description=long_description,
     long_description_content_type="text/markdown",
+    url='https://github.com/WrenchAI/WrenchCL',
     packages=find_packages(),
     install_requires=required,
-    python_requires='>=3.9',
-)
+    python_requires='>=3.11',
+    classifiers=[
+        'Programming Language :: Python :: 3',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+    ],
+)
```

