# Comparing `tmp/akatosh-3.0.6.tar.gz` & `tmp/akatosh-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akatosh-3.0.6.tar", max compression
+gzip compressed data, was "akatosh-3.0.7.tar", max compression
```

## Comparing `akatosh-3.0.6.tar` & `akatosh-3.0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      544 2024-05-08 01:04:21.582527 akatosh-3.0.6/Akatosh/__init__.py
--rw-r--r--   0        0        0     5333 2024-05-08 01:04:21.583527 akatosh-3.0.6/Akatosh/entity.py
--rw-r--r--   0        0        0     6273 2024-05-08 01:05:22.105174 akatosh-3.0.6/Akatosh/event.py
--rw-r--r--   0        0        0     5230 2024-04-22 03:53:18.056982 akatosh-3.0.6/Akatosh/resource.py
--rw-r--r--   0        0        0     6052 2024-05-08 01:04:21.585530 akatosh-3.0.6/Akatosh/universe.py
--rw-r--r--   0        0        0      321 2024-05-08 01:06:10.955605 akatosh-3.0.6/pyproject.toml
--rw-r--r--   0        0        0     2324 2024-04-19 03:36:27.289023 akatosh-3.0.6/README.md
--rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.6/PKG-INFO
+-rw-r--r--   0        0        0      544 2024-05-08 01:04:21.582527 akatosh-3.0.7/Akatosh/__init__.py
+-rw-r--r--   0        0        0     5333 2024-05-08 01:04:21.583527 akatosh-3.0.7/Akatosh/entity.py
+-rw-r--r--   0        0        0     6375 2024-05-17 03:52:58.399245 akatosh-3.0.7/Akatosh/event.py
+-rw-r--r--   0        0        0     5230 2024-04-22 03:53:18.056982 akatosh-3.0.7/Akatosh/resource.py
+-rw-r--r--   0        0        0     6109 2024-05-17 03:56:22.573448 akatosh-3.0.7/Akatosh/universe.py
+-rw-r--r--   0        0        0      321 2024-05-17 03:56:29.523927 akatosh-3.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2324 2024-04-19 03:36:27.289023 akatosh-3.0.7/README.md
+-rw-r--r--   0        0        0     2879 1970-01-01 00:00:00.000000 akatosh-3.0.7/PKG-INFO
```

### Comparing `akatosh-3.0.6/Akatosh/__init__.py` & `akatosh-3.0.7/Akatosh/__init__.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.6/Akatosh/entity.py` & `akatosh-3.0.7/Akatosh/entity.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.6/Akatosh/event.py` & `akatosh-3.0.7/Akatosh/event.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,50 +61,50 @@
                     await asyncio.sleep(0)
 
             if self.started == False:
                 if isinstance(self.at, Event):
                     if self.at.ended == True:
                         self._started = True
                         self._next = Mundus.time
-                        logger.debug(f"Event {self} started.")
+                        logger.debug(f"Event {self} started at {Mundus.time}.")
                 else:
                     if self.at <= Mundus.time:
                         self._started = True
                         self._next = Mundus.time
-                        logger.debug(f"Event {self} started.")
+                        logger.debug(f"Event {self} started at {Mundus.time}.")
 
             if (
                 self.started == True
                 and self.ended == False
                 and self.paused == False
-                and self.next == Mundus.time
+                and self.next <= Mundus.time
             ):
                 if asyncio.iscoroutinefunction(self._action):
                     await self._action()
                 else:
                     self._action()
                 self._acted = True
                 self._next += max(Mundus.time_step, self.step)
                 self._next = round(self._next, Mundus.time_resolution)
-                logger.debug(f"Event {self} acted.")
+                logger.debug(f"Event {self} acted at {Mundus.time}.")
                 if self._once == True:
                     self._ended = True
-                    logger.debug(f"Event {self} ended.")
+                    logger.debug(f"Event {self} ended at {Mundus.time}.")
                     return
 
             if self.ended == False:
                 if isinstance(self.till, Event):
                     if self.till.ended == True:
                         self._ended = True
-                        logger.debug(f"Event {self} ended.")
+                        logger.debug(f"Event {self} ended at {Mundus.time}.")
                         return
                 else:
                     if self.till <= Mundus.time:
                         self._ended = True
-                        logger.debug(f"Event {self} ended.")
+                        logger.debug(f"Event {self} ended at {Mundus.time}.")
                         return
             await asyncio.sleep(0)
 
     def __str__(self) -> str:
         """Return the label of the event if it has one, otherwise return the id of the event."""
         if self.label is None:
             return f"Event {id(self)}"
```

### Comparing `akatosh-3.0.6/Akatosh/resource.py` & `akatosh-3.0.7/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.6/Akatosh/universe.py` & `akatosh-3.0.7/Akatosh/universe.py`

 * *Files 13% similar despite different names*

```diff
@@ -40,30 +40,31 @@
             self._simulation_start_time = time.perf_counter()
             while self.time < till:
                 logger.debug(f"Simulation time:\t{self.time}")
                 for event in self.pending_events:
                     asyncio.create_task(event())
                 self.pending_events.clear()
                 if self.realtime:
-                    logger.debug(f"Iteration started at Real Time: {time.perf_counter() - self.simulation_start_time:0.6f}")
+                    iteration_start_time = time.perf_counter() - self.simulation_start_time
+                    logger.debug(f"Iteration started at Real Time: {iteration_start_time:0.6f}")
                     # iterate through all event priorities
                     self._current_event_priority = 0
                     while self.current_event_priority <= self._max_event_priority:
                         logger.debug(
                             f"Current Event Priority: {self.current_event_priority}"
                         )
                         await asyncio.sleep(0)
                         self._current_event_priority += 1
-                    # wait for the time step
-                    self._time += self.time_step
-                    self._time = round(self.time, self.time_resolution)
-                    logger.debug(f"Iteration finished at Real Time: {time.perf_counter() - self.simulation_start_time:0.6f}")
-                    logger.debug(f"Waiting for next interation...")
-                    while time.perf_counter() - self.simulation_start_time < self.time:
-                        await asyncio.sleep(0)
+                    # finish the iteration
+                    iteration_end_time = time.perf_counter() - self.simulation_start_time
+                    logger.debug(f"Iteration finished at Real Time: {iteration_end_time:0.6f}")
+                    logger.debug(f"FPS: {1/(iteration_end_time - iteration_start_time):0.6f}")
+                    # update the time
+                    self._time = time.perf_counter() - self.simulation_start_time
+                    await asyncio.sleep(0)
                     
                 else:
                     # iterate through all event priorities
                     self._current_event_priority = 0
                     while self.current_event_priority <= self._max_event_priority:
                         logger.debug(
                             f"Current Event Priority: {self.current_event_priority}"
```

### Comparing `akatosh-3.0.6/README.md` & `akatosh-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `akatosh-3.0.6/PKG-INFO` & `akatosh-3.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 3.0.6
+Version: 3.0.7
 Summary: 
 Author: Innovation Central Perth Maintainer
 Author-email: ryf0510@live.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

