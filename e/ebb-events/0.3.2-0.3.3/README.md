# Comparing `tmp/ebb_events-0.3.2.tar.gz` & `tmp/ebb_events-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_events-0.3.2.tar", max compression
+gzip compressed data, was "ebb_events-0.3.3.tar", max compression
```

## Comparing `ebb_events-0.3.2.tar` & `ebb_events-0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.2/LICENSE
--rw-r--r--   0        0        0     8842 2024-05-14 16:56:47.897263 ebb_events-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.2/ebb_events/__init__.py
--rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.2/ebb_events/builders/event_builder.py
--rw-r--r--   0        0        0    10366 2024-05-15 20:31:26.931154 ebb_events-0.3.2/ebb_events/consumers/event_consumer.py
--rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.2/ebb_events/enums.py
--rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.3.2/ebb_events/event_payload_utils.py
--rw-r--r--   0        0        0     2668 2024-05-13 20:48:51.509330 ebb_events-0.3.2/ebb_events/event_schema.py
--rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.2/ebb_events/exceptions.py
--rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.2/ebb_events/field_constants.py
--rw-r--r--   0        0        0      571 2024-05-15 20:31:26.931473 ebb_events-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 ebb_events-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-06 20:14:00.489414 ebb_events-0.3.3/LICENSE
+-rw-r--r--   0        0        0     8842 2024-05-14 16:56:47.897263 ebb_events-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-19 21:49:16.587650 ebb_events-0.3.3/ebb_events/__init__.py
+-rw-r--r--   0        0        0     8886 2024-05-15 20:31:26.930793 ebb_events-0.3.3/ebb_events/builders/event_builder.py
+-rw-r--r--   0        0        0    10777 2024-05-17 17:46:46.038249 ebb_events-0.3.3/ebb_events/consumers/event_consumer.py
+-rw-r--r--   0        0        0      174 2024-04-22 19:12:51.110543 ebb_events-0.3.3/ebb_events/enums.py
+-rw-r--r--   0        0        0      414 2024-05-10 21:40:45.943826 ebb_events-0.3.3/ebb_events/event_payload_utils.py
+-rw-r--r--   0        0        0     2668 2024-05-13 20:48:51.509330 ebb_events-0.3.3/ebb_events/event_schema.py
+-rw-r--r--   0        0        0      383 2024-05-06 17:16:47.746622 ebb_events-0.3.3/ebb_events/exceptions.py
+-rw-r--r--   0        0        0      263 2024-05-14 16:56:47.898608 ebb_events-0.3.3/ebb_events/field_constants.py
+-rw-r--r--   0        0        0      571 2024-05-17 17:46:46.038517 ebb_events-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9340 1970-01-01 00:00:00.000000 ebb_events-0.3.3/PKG-INFO
```

### Comparing `ebb_events-0.3.2/LICENSE` & `ebb_events-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.2/README.md` & `ebb_events-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.2/ebb_events/builders/event_builder.py` & `ebb_events-0.3.3/ebb_events/builders/event_builder.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.2/ebb_events/consumers/event_consumer.py` & `ebb_events-0.3.3/ebb_events/consumers/event_consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,25 @@
         Raises:
             PayloadFormatException: Raised if event does not match ebb_event structure.
 
         Returns:
             datetime: event's time field.
         """
         if self.is_ebb_event_structure:
-            return datetime.fromisoformat(self.raw_payload.get(TIME))
+            raw_time = self.raw_payload.get(TIME)
+            try:
+                return datetime.fromisoformat(raw_time)
+            except ValueError as error:
+                logging.error(
+                    f"Time is invalid isoformat string: {raw_time}",
+                    extra={"error": str(error)},
+                )
+                raise PayloadFormatException(
+                    message=f"Time is invalid isoformat string: {raw_time}"
+                ) from error
         logging.error(self.error_log_message % "event_time")
         raise PayloadFormatException()
 
     def get_event_source(self) -> str:
         """
         Helper to fetch event's source as string. For ebb_events, the `source` field matches the MQTT `topic`.
```

### Comparing `ebb_events-0.3.2/ebb_events/event_schema.py` & `ebb_events-0.3.3/ebb_events/event_schema.py`

 * *Files identical despite different names*

### Comparing `ebb_events-0.3.2/pyproject.toml` & `ebb_events-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-events"
-version = "0.3.2"
+version = "0.3.3"
 description = "Package for building and standardizing MQTT event messages."
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 marshmallow = "^3.21.1"
```

### Comparing `ebb_events-0.3.2/PKG-INFO` & `ebb_events-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-events
-Version: 0.3.2
+Version: 0.3.3
 Summary: Package for building and standardizing MQTT event messages.
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

