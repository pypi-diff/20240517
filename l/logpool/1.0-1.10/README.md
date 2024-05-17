# Comparing `tmp/logpool-1.0-py3-none-any.whl.zip` & `tmp/logpool-1.10-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 16322 bytes, number of entries: 7
+Zip file size: 16076 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       31 b- defN 24-May-06 17:31 logpool/__init__.py
--rw-r--r--  2.0 unx     8233 b- defN 24-May-06 17:27 logpool/log.py
--rw-r--r--  2.0 unx    35149 b- defN 24-May-06 17:32 logpool-1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      373 b- defN 24-May-06 17:32 logpool-1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-06 17:32 logpool-1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-06 17:32 logpool-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      520 b- defN 24-May-06 17:32 logpool-1.0.dist-info/RECORD
-7 files, 44406 bytes uncompressed, 15404 bytes compressed:  65.3%
+-rw-r--r--  2.0 unx     7740 b- defN 24-May-17 17:15 logpool/log.py
+-rw-r--r--  2.0 unx    35149 b- defN 24-May-17 21:10 logpool-1.10.dist-info/LICENSE
+-rw-r--r--  2.0 unx      374 b- defN 24-May-17 21:10 logpool-1.10.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-17 21:10 logpool-1.10.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-17 21:10 logpool-1.10.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      525 b- defN 24-May-17 21:10 logpool-1.10.dist-info/RECORD
+7 files, 43919 bytes uncompressed, 15148 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: logpool/__init__.py
 Comment: 
 
 Filename: logpool/log.py
 Comment: 
 
-Filename: logpool-1.0.dist-info/LICENSE
+Filename: logpool-1.10.dist-info/LICENSE
 Comment: 
 
-Filename: logpool-1.0.dist-info/METADATA
+Filename: logpool-1.10.dist-info/METADATA
 Comment: 
 
-Filename: logpool-1.0.dist-info/WHEEL
+Filename: logpool-1.10.dist-info/WHEEL
 Comment: 
 
-Filename: logpool-1.0.dist-info/top_level.txt
+Filename: logpool-1.10.dist-info/top_level.txt
 Comment: 
 
-Filename: logpool-1.0.dist-info/RECORD
+Filename: logpool-1.10.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## logpool/log.py

```diff
@@ -1,55 +1,25 @@
-"""
-Written by Gustavo Schwarz
-https://github.com/schwarzam
-
-Repo
-https://github.com/Schwarzam/logpool
-
-Use:
-
-from log import control
-
-def some_function(x, y):
-    control.info(f"Inside function - {x} and {y} are being added.")
-    if x > 100:
-        control.warn(f"X is greater than 100: {x}")
-    
-for i in range(100):
-    control.submit(some_function, i**2, i*3, group="sum_func")
-
-control.wait(group="sum_func")
-control.info("Finished")
-control.time(content)
-
-"""
-
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
 import threading
 import inspect
-
 import os
 from datetime import datetime
-
 import time
-
 import psutil
 from threading import Lock
 
-class ControlThreads(ThreadPoolExecutor):
+class ControlThreads:
     """
-    A thread pool executor that extends concurrent.futures.ThreadPoolExecutor, providing
-    enhanced logging capabilities, group task management, and customized logging functionalities.
-    
-    Its important to mention that errors in threads are logged as critical and the thread is not stopped.
+    A thread and process pool executor that provides enhanced logging capabilities,
+    group task management, and customized logging functionalities.
     
     Methods
     -------
     submit(fn, *args, group="default", **kwargs):
-        Submit a function to be executed by the thread pool, optionally assigning it to a group.
+        Submit a function to be executed by the thread or process pool, optionally assigning it to a group.
     get_logs():
         Returns the content of the log file as a list of strings.
     get_queue(group='default'):
         Returns a list indicating the completion status of tasks in a specified group.
     info(content, **kwargs), time(content), warn(content), critical(content), debug(content):
         Methods to log messages of different severities.
     clear_logs():
@@ -64,73 +34,67 @@
     >>> def task(x):
     ...     control.info("Written from thread.") 
     ...     return x*x
     >>> future = control.submit(task, 2)
     >>> control.info("Task submitted.")
     >>> control.wait()
     >>> print(future.result())
-
-    Note: Replace 'your_script' with the actual name of your script file without the '.py' extension.
     """
     
-    
-    def __init__(self, log_file=None, print_log=True, debug=False, max_workers=psutil.cpu_count(logical=True) - 2):
+    def __init__(self, log_file=None, print_log=True, debug=False, max_workers=psutil.cpu_count(logical=True) - 2, use_process_pool=False):
         """
-        Initialize the Log object.
+        Initialize the ControlThreads object.
 
         Args:
             log_file (str): Path to the log file. If None, logging to a file is disabled.
             print_log (bool): Whether to print log messages to the console.
             debug (bool): Whether to enable debug mode.
-            max_workers (int): Maximum number of worker threads to use.
-
+            max_workers (int): Maximum number of worker threads or processes to use.
+            use_process_pool (bool): Whether to use a process pool instead of a thread pool.
         """
-        ThreadPoolExecutor.__init__(self, max_workers)
         self.lock = Lock()
-        
         self.tasks = {'default': []}
         self.log_file = log_file
-        
         if self.log_file is not None:
             self._init_log()
-        
         self.workers = max_workers
         self.print_log = print_log
         self.debug_mode = debug
-
+        self.use_process_pool = use_process_pool
+        self.executor = ProcessPoolExecutor(max_workers) if use_process_pool else ThreadPoolExecutor(max_workers)
+    
     def reconfigure(self, *args, **kwargs):
         """
-        Reconfigure the Log object with new settings.
+        Reconfigure the ControlThreads object with new settings.
 
         Args:
             log_file (str): Path to the log file. If None, logging to a file is disabled.
             print_log (bool): Whether to print log messages to the console.
             debug (bool): Whether to enable debug mode.
-            max_workers (int): Maximum number of worker threads to use.
-
+            max_workers (int): Maximum number of worker threads or processes to use.
+            use_process_pool (bool): Whether to use a process pool instead of a thread pool.
         """
-        # Reconfigure the Log object with new settings
-        return super().__call__(*args, **kwargs)
+        self.executor.shutdown(wait=False)
+        self.__init__(*args, **kwargs)
 
     def _init_log(self):
         io = open(self.log_file, 'a')
         io.close()
-        
+
     def submit(self, fn, *args, group="default", **kwargs):
         """
         Submits a task to the executor for execution.
 
         Args:
             fn: The function to be executed.
             *args: Positional arguments to be passed to the function.
             group: The group to which the task belongs (default is "default").
             **kwargs: Keyword arguments to be passed to the function.
-
         """
-        future = super().submit(fn, *args, **kwargs)
+        future = self.executor.submit(fn, *args, **kwargs)
         future.add_done_callback(worker_callbacks)
         if group not in self.tasks:
             self.tasks[group] = []
         self.tasks[group].append(future)
 
     def get_logs(self):
         """
@@ -140,63 +104,58 @@
             Exception: If no log file was defined.
 
         Returns:
             list: A list of lines read from the log file.
         """
         if self.log_file is None:
             raise Exception("No log file was defined")
-        f = open(self.log_file, 'r')
-        return f.readlines()
+        with open(self.log_file, 'r') as f:
+            return f.readlines()
 
-    def get_queue(self, group = 'default'):
+    def get_queue(self, group='default'):
         return [i.done() for i in self.tasks[group]]
-    
+
     def info(self, content, **kwargs):
         """ Logs an informational message. """
         self.wlog(content, "[info]")
-        
+
     def time(self, content):
-        """ Logs an time message. """
+        """ Logs a time message. """
         self.wlog(content, "[time]")
-        
+
     def warn(self, content):
-        """ Logs an warn message. """
+        """ Logs a warning message. """
         self.wlog(content, "[warning]")
-        
+
     def critical(self, content):
-        """ Logs an critical message. """
+        """ Logs a critical message. """
         self.wlog(content, "[critical]")
-        
+
     def debug(self, content):
-        """ Logs an debug message. """
+        """ Logs a debug message. """
         if self.debug_mode:
             self.wlog(content, "[debug]")
-    
-    def wlog(self, content, tipo="[info]", print_log = True):
+
+    def wlog(self, content, tipo="[info]", print_log=True):
         func = inspect.currentframe().f_back.f_back.f_code
         function = func.co_name
         filename = func.co_filename
-
         thread_id = threading.current_thread().native_id
-
         if tipo == "[critical]":
             log_message = f"{datetime.now().strftime('%d/%m/%Y %H:%M:%S')}  {tipo} - Thread {thread_id} - {str(content)}"
         elif tipo == "[time]":
             log_message = f"{datetime.now().strftime('%d/%m/%Y %H:%M:%S')}  {tipo} - {str(content)}"
         else:
             log_message = f"{datetime.now().strftime('%d/%m/%Y %H:%M:%S')}  {tipo} - {os.path.basename(filename)} - {function}() - {str(content)}"
-
-        if print_log: 
+        if print_log:
             print(log_message, end="\n")
-        
         if self.log_file is not None:
             with self.lock:
-                io = open(self.log_file, 'a')
-                io.write(log_message + "\n")
-                io.close()
+                with open(self.log_file, 'a') as io:
+                    io.write(log_message + "\n")
 
     def timer(self, func):
         """
         A decorator function that measures the execution time of a given function and writes to the log.
 
         @control.timer
         def my_function():
@@ -207,57 +166,50 @@
             result = func(*args, **kwargs)
             final = time.time() - start
             final = round(final, 4)
             self.time(f"{func.__name__}() executed in {final}s")
             return result
         return wrapper
 
-    def wait(self, group = "default"):
+    def wait(self, group="default"):
         """
         Waits for all tasks in the specified group to complete.
 
         Args:
             group (str, optional): The group name. Defaults to "default".
         """
         if group not in self.tasks:
             return
         queue = [i.done() for i in self.tasks[group]]
-        
         while False in queue:
             time.sleep(0.05)
             queue = [i.done() for i in self.tasks[group]]
 
     def clear_logs(self):
         """
         Clears the contents of the log file.
         """
-        io = open(self.log_file, 'w')
-        io.close()
+        with open(self.log_file, 'w') as io:
+            io.close()
 
-    
 def worker_callbacks(f):
     """
     Called to create trace of exceptions in threads.
     """
     e = f.exception()
-
     if e is None:
         return
-
     trace = []
     tb = e.__traceback__
     while tb is not None:
         trace.append({
             "filename": tb.tb_frame.f_code.co_filename,
             "name": tb.tb_frame.f_code.co_name,
             "lineno": tb.tb_lineno
         })
         tb = tb.tb_next
-        
     trace_str = ""
     for key, i in enumerate(trace):
         trace_str += f"[Trace {key}: {i['filename']} - {i['name']}() - line {i['lineno']}]"
-        
     control.critical(f"""{type(e).__name__}: {str(e)} -> {trace_str}""")
 
-
-control = ControlThreads(log_file=None, print_log = True, debug = True)
+control = ControlThreads(log_file=None, print_log=True, debug=True)
```

## Comparing `logpool-1.0.dist-info/LICENSE` & `logpool-1.10.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `logpool-1.0.dist-info/RECORD` & `logpool-1.10.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 logpool/__init__.py,sha256=s0XbuH7ltBa8oq2Kw8DpfjJ5xgRMjoKPhN_rr4cwqvE,31
-logpool/log.py,sha256=hdyey9Dy02AG1az_NlUPjsoZsQZvUjlAYq21IP8z4KM,8233
-logpool-1.0.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-logpool-1.0.dist-info/METADATA,sha256=BG9ExTO3UQ7pxxN3V6sEIF5GzQ_JneDVlLuTGfosCTw,373
-logpool-1.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-logpool-1.0.dist-info/top_level.txt,sha256=OaI0VfqXFQwCTTtO2GvkQopDtoti7OptNBlhE2FG0DU,8
-logpool-1.0.dist-info/RECORD,,
+logpool/log.py,sha256=Mr5uOw8q7-x2yz4BD9lmrTI6xBoAYkhBFV2SPppez5o,7740
+logpool-1.10.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+logpool-1.10.dist-info/METADATA,sha256=H2VLMDkc4XoArh_yJwR9zJ-AOIzCG-UVyUZpYCtFZ4M,374
+logpool-1.10.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+logpool-1.10.dist-info/top_level.txt,sha256=OaI0VfqXFQwCTTtO2GvkQopDtoti7OptNBlhE2FG0DU,8
+logpool-1.10.dist-info/RECORD,,
```

