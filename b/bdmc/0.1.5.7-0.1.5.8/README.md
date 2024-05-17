# Comparing `tmp/bdmc-0.1.5.7.tar.gz` & `tmp/bdmc-0.1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.5.7.tar", last modified: Thu May 16 13:18:59 2024, max compression
+gzip compressed data, was "bdmc-0.1.5.8.tar", last modified: Fri May 17 16:06:13 2024, max compression
```

## Comparing `bdmc-0.1.5.7.tar` & `bdmc-0.1.5.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5466 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/README.md
--rw-r--r--   0        0        0      547 2024-05-16 13:18:59.334127 bdmc-0.1.5.7/pyproject.toml
--rw-r--r--   0        0        0      556 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/__init__.py
--rw-r--r--   0        0        0      419 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    17286 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7529 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-05-16 13:18:40.794090 bdmc-0.1.5.7/tests/find_tests.py
--rw-r--r--   0        0        0     4380 2024-05-16 13:18:40.794090 bdmc-0.1.5.7/tests/test_context.py
--rw-r--r--   0        0        0     1989 2024-05-16 13:18:40.794090 bdmc-0.1.5.7/tests/test_controller.py
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.7/PKG-INFO
+-rw-r--r--   0        0        0     5466 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/README.md
+-rw-r--r--   0        0        0      547 2024-05-17 16:06:13.764532 bdmc-0.1.5.8/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    15509 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-05-17 16:05:54.868493 bdmc-0.1.5.8/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7529 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/tests/find_tests.py
+-rw-r--r--   0        0        0     4380 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/tests/test_context.py
+-rw-r--r--   0        0        0     1989 2024-05-17 16:05:54.872493 bdmc-0.1.5.8/tests/test_controller.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.8/PKG-INFO
```

### Comparing `bdmc-0.1.5.7/README.md` & `bdmc-0.1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/pyproject.toml` & `bdmc-0.1.5.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.5.7"
+version = "0.1.5.8"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.5.7/src/bdmc/__init__.py` & `bdmc-0.1.5.8/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/src/bdmc/modules/controller.py` & `bdmc-0.1.5.8/src/bdmc/modules/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -187,14 +187,15 @@
                     for key, output_data in zip(all_output_keys, function(*frozen_input_data)):
                         context[key] = output_data
 
             case _:
                 raise ValueError(
                     f"Invalid arguments for register_context_updater function. got {input_keys} and {output_keys} and {freeze_inputs}"
                 )
+        self._context.update({key: None for key in output_keys})
         return _updater
 
     def register_context_getter(self, var_key: str) -> Callable[[], Any]:
         """
         Register a context getter function for a given variable key.
 
         Args:
@@ -344,81 +345,57 @@
         """
         self._cmd_queue.put(cmd.value)
         return self
 
     def delay_b(
         self,
         delay_sec: float,
-        breaker: Callable[[], Any],
+        breaker: Callable[[], bool] | Callable[[], int] | Callable[[], float] | Callable[[], Any],
         check_interval: float = 0.01,
     ) -> Self:
         """
-        Delays the execution of the function by a specified amount of time, while checking a breaker function periodically.
+        A function to introduce a delay of a specified time with a breaker function.
 
         Parameters:
-            delay_sec (float): The amount of time to delay the execution in seconds.
-            breaker (Callable[[], Any]): A function that returns a boolean value indicating whether the delay should be aborted.
-            check_interval (float, optional): The interval in seconds between each check of the breaker function. Defaults to 0.01.
+            delay_sec (float): The time in seconds to delay.
+            breaker (Callable[[], Any]): The breaker function that can abort the delay.
+            check_interval (float): The interval to check the breaker function.
 
         Returns:
-            Self: The instance of the class itself.
-
-        Raises:
-            ValueError: If the check_interval is not at least twice as large as the delay_sec.
-
-        Notes:
-            - The delay_sec parameter specifies the total amount of time to delay the execution,
-             including the initial delay and the time spent checking the breaker function.
-            - The check_interval parameter specifies the interval in seconds between each check of the breaker function.
-             It should be at least twice as large as the delay_sec parameter to ensure accurate timing.
-            - The breaker function is called periodically to check if the delay should be aborted.
-            If the breaker function returns True, the delay is aborted and the function returns immediately.
-            - If the breaker function returns False, the function continues to check the breaker function until either
-            the delay is completed or the breaker function returns True.
-            - If the delay is completed before the breaker function returns True, the function returns immediately.
+            Self: Returns the instance of the class.
         """
 
         ed_time = time() + delay_sec - check_interval
         # this is to add the first time check, since the timer waits before the check
         if alarm := breaker():
             return self
         while not alarm and time() < ed_time:
             alarm = breaker()
             sleep(check_interval)
         return self
 
     @staticmethod
     def delay_b_match(
         delay_sec: float,
-        breaker: Callable[[], GT],
+        breaker: Callable[[], bool] | Callable[[], int] | Callable[[], float] | Callable[[], GT],
         check_interval: float = 0.01,
     ) -> GT:
         """
-        Delays the execution of a function until a condition is met.
+        Delays the execution based on the specified delay time and checks a breaker function periodically.
 
-        Args:
-            delay_sec (float): The number of seconds to delay the execution.
-            breaker (Callable[[], GT]): The function to be executed after the delay.
-            check_interval (float, optional): The interval between each check. Defaults to 0.01.
-
-        Returns:
-            GT: The result of the `breaker` function after the delay.
-
-        Raises:
-            ValueError: If `check_interval` is not 2 times greater than `delay_sec`.
-
-        Note:
-            - The `delay_sec` parameter specifies the total amount of time to delay the execution,
-            including the initial delay and the time spent checking the `breaker` function.
-            - The `check_interval` parameter specifies the interval in seconds between each check.
-            It should be at least twice as large as the `delay_sec` parameter to ensure accurate timing.
-            - The `breaker` function is called periodically to check if the delay should be aborted.
-            If the `breaker` function returns True, the delay is aborted and the function returns immediately.
-            - If the `breaker` function returns False, the function continues to check the `breaker` function until
-            either the delay is completed or the `breaker` function returns True.
+        Parameters:
+            delay_sec (float): The amount of time to delay the execution in seconds.
+            breaker (Callable[[], GT]): A function that returns the status of the delay.
+            check_interval (float): The interval between each check of the breaker function.
+
+        Returns:
+            GT: The result of the breaker function.
+
+        Notes:
+            - The function delays the execution by the specified time and checks the breaker function periodically.
         """
 
         ed_time = time() + delay_sec - check_interval
         # this is to add the first time check, since the timer waits before the check
         if alarm := breaker():
             return alarm
         while not alarm and time() < ed_time:
```

### Comparing `bdmc-0.1.5.7/src/bdmc/modules/debug.py` & `bdmc-0.1.5.8/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/src/bdmc/modules/logger.py` & `bdmc-0.1.5.8/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/src/bdmc/modules/port.py` & `bdmc-0.1.5.8/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/src/bdmc/modules/seriald.py` & `bdmc-0.1.5.8/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/tests/find_tests.py` & `bdmc-0.1.5.8/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/tests/test_context.py` & `bdmc-0.1.5.8/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/tests/test_controller.py` & `bdmc-0.1.5.8/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.7/PKG-INFO` & `bdmc-0.1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.5.7
+Version: 0.1.5.8
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```

