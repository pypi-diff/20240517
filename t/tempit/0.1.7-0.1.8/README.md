# Comparing `tmp/tempit-0.1.7.tar.gz` & `tmp/tempit-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempit-0.1.7.tar", last modified: Tue May 14 09:57:14 2024, max compression
+gzip compressed data, was "tempit-0.1.8.tar", last modified: Fri May 17 15:01:48 2024, max compression
```

## Comparing `tempit-0.1.7.tar` & `tempit-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 09:57:14.048917 tempit-0.1.7/
--rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     7657 2024-05-14 09:57:14.046950 tempit-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     7002 2024-05-14 09:53:27.000000 tempit-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-14 09:57:14.049425 tempit-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-05-14 09:55:03.000000 tempit-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:57:14.030428 tempit-0.1.7/tempit/
--rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.7/tempit/__init__.py
--rw-rw-rw-   0        0        0    11238 2024-05-13 16:16:07.000000 tempit-0.1.7/tempit/core.py
--rw-rw-rw-   0        0        0     5498 2024-05-10 06:26:45.000000 tempit-0.1.7/tempit/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-14 09:57:14.043429 tempit-0.1.7/tempit.egg-info/
--rw-rw-rw-   0        0        0     7657 2024-05-14 09:57:13.000000 tempit-0.1.7/tempit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-14 09:57:14.000000 tempit-0.1.7/tempit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 09:57:13.000000 tempit-0.1.7/tempit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-14 09:57:13.000000 tempit-0.1.7/tempit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-14 09:57:13.000000 tempit-0.1.7/tempit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 09:57:14.042427 tempit-0.1.7/tests/
--rw-rw-rw-   0        0        0    12853 2024-05-14 06:44:50.000000 tempit-0.1.7/tests/test_tempit.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.619592 tempit-0.1.8/
+-rw-rw-rw-   0        0        0     1068 2024-05-10 08:37:29.000000 tempit-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     7657 2024-05-17 15:01:48.617586 tempit-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7002 2024-05-14 09:53:27.000000 tempit-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:01:48.619592 tempit-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-05-17 15:00:30.000000 tempit-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.593976 tempit-0.1.8/tempit/
+-rw-rw-rw-   0        0        0       50 2024-05-09 20:06:13.000000 tempit-0.1.8/tempit/__init__.py
+-rw-rw-rw-   0        0        0    11326 2024-05-17 14:59:23.000000 tempit-0.1.8/tempit/core.py
+-rw-rw-rw-   0        0        0     5498 2024-05-17 14:59:23.000000 tempit-0.1.8/tempit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.616588 tempit-0.1.8/tempit.egg-info/
+-rw-rw-rw-   0        0        0     7657 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 15:01:48.000000 tempit-0.1.8/tempit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 15:01:48.615587 tempit-0.1.8/tests/
+-rw-rw-rw-   0        0        0    12853 2024-05-17 14:59:23.000000 tempit-0.1.8/tests/test_tempit.py
```

### Comparing `tempit-0.1.7/LICENSE` & `tempit-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tempit-0.1.7/PKG-INFO` & `tempit-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.7
+Version: 0.1.8
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tempit-0.1.7/README.md` & `tempit-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `tempit-0.1.7/setup.py` & `tempit-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.1.7"
+VERSION = "0.1.8"
 setup(
     name="tempit",
     version=VERSION,
     author="mcrespoae",
     author_email="info@mariocrespo.es",
     packages=["tempit"],
     description="A dead simple time decorator",
```

### Comparing `tempit-0.1.7/tempit/core.py` & `tempit-0.1.8/tempit/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,25 +54,29 @@
         run_times: int = 1,
         concurrent_execution: bool = True,
         verbose: bool = False,
         check_for_recursion: bool = False,
     ) -> Callable:
         @wraps(func)
         def tempit_wrapper(*args: Tuple, **kwargs: Dict) -> Any:
-            is_recursive, run_times_final, concurrent_execution_final = check_is_recursive_func(check_for_recursion, func, run_times, concurrent_execution)
+            is_recursive, run_times_final, concurrent_execution_final = check_is_recursive_func(
+                check_for_recursion, func, run_times, concurrent_execution
+            )
             callable_func, args, args_to_print = extract_callable_and_args_if_method(func, *args)
             result, total_times, real_time = function_execution(
                 callable_func,
                 run_times_final,
                 concurrent_execution_final,
                 *args,
                 **kwargs,
             )
             if not is_recursive:
-                print_tempit_values(run_times, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs)
+                print_tempit_values(
+                    run_times_final, verbose, callable_func, total_times, real_time, *args_to_print, **kwargs
+                )
             return result
 
         return tempit_wrapper
 
     if args:  # If arguments are not provided, return a decorator
         return decorator(
             *args,
@@ -88,28 +92,31 @@
             run_times=run_times,
             concurrent_execution=concurrent_execution,
             verbose=verbose,
             check_for_recursion=check_for_recursion,
         )
 
 
-def check_is_recursive_func(check_for_recursion: bool, func: Callable, run_times: int, concurrent_execution: bool) -> Tuple[bool, int, bool]:
+def check_is_recursive_func(
+    check_for_recursion: bool, func: Callable, run_times: int, concurrent_execution: bool
+) -> Tuple[bool, int, bool]:
     """
     Checks if the function is being called recursively.
     Returns:
         Tuple[bool, int, bool]: A tuple containing True if the function is being called recursively, False otherwise.
         The second element is the number of times the function has been called, and the third element is a boolean indicating if the function has crashed.
     """
 
     if check_for_recursion:
         import sys
         from inspect import getframeinfo
+
         func_name = func.__name__
         func_filename = ""
-        if hasattr(func, '__code__'):
+        if hasattr(func, "__code__"):
             func_filename = func.__code__.co_filename
         frame = getframeinfo(sys._getframe(2), context=0)
         if frame.function == func_name and func_filename == frame.filename:
             return True, 1, False
     return False, run_times, concurrent_execution
```

### Comparing `tempit-0.1.7/tempit/utils.py` & `tempit-0.1.8/tempit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         *args (Tuple): Additional positional arguments to pass to the function.
         **kwargs (Dict): Additional keyword arguments to pass to the function.
     Returns:
         None
     """
     if verbose:
         print("*" * 5, f"tempit data for function {func.__name__}:", "*" * 5)
-    if run_times == 1:
+    if run_times <= 1:
         print_single_value(verbose, func, total_times[0], *args, **kwargs)
     else:
         print_several_values(verbose, func, total_times, real_time, *args, **kwargs)
     if verbose:
         print("*" * 5, "End of tempit data.", "*" * 5)
```

### Comparing `tempit-0.1.7/tempit.egg-info/PKG-INFO` & `tempit-0.1.8/tempit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempit
-Version: 0.1.7
+Version: 0.1.8
 Summary: A dead simple time decorator
 Home-page: https://github.com/mcrespoae/tempit
 Author: mcrespoae
 Author-email: info@mariocrespo.es
 Keywords: tempit,time,decorator,performance,concurrency,parallel,benchmark
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tempit-0.1.7/tests/test_tempit.py` & `tempit-0.1.8/tests/test_tempit.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
         my_function()
         end_time = time.perf_counter()
 
         execution_time = end_time - start_time
         self.assertLess(execution_time, 0.5)
 
     def test_tempit_args(self):
-        @tempit(run_times=2, concurrent_execution=True, verbose=True)
+        @tempit(run_times=0, concurrent_execution=True, verbose=True)
         def my_function(a: int = 1, b: int = 2):
             return a + b
 
         start_time = time.perf_counter()
         result = my_function(1, b=2)
         end_time = time.perf_counter()
```

