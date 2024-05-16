# Comparing `tmp/ebb_time_series-0.2.0.tar.gz` & `tmp/ebb_time_series-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_time_series-0.2.0.tar", max compression
+gzip compressed data, was "ebb_time_series-0.2.1.tar", max compression
```

## Comparing `ebb_time_series-0.2.0.tar` & `ebb_time_series-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.2.0/LICENSE
--rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.2.0/ebb_time_series/__init__.py
--rw-r--r--   0        0        0      399 2024-05-16 16:14:33.959351 ebb_time_series-0.2.0/ebb_time_series/constants.py
--rw-r--r--   0        0        0      233 2024-05-16 16:14:33.959702 ebb_time_series-0.2.0/ebb_time_series/data_schema.py
--rw-r--r--   0        0        0     1195 2024-05-16 16:14:33.959938 ebb_time_series-0.2.0/ebb_time_series/event_parser_helpers.py
--rw-r--r--   0        0        0      259 2024-05-16 16:14:33.960286 ebb_time_series-0.2.0/ebb_time_series/exceptions.py
--rw-r--r--   0        0        0     9582 2024-05-16 17:01:44.194983 ebb_time_series-0.2.0/ebb_time_series/writers/aws_timestream_data_writer.py
--rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.2.0/ebb_time_series/writers/base_data_writer.py
--rw-r--r--   0        0        0      551 2024-05-16 17:01:44.195330 ebb_time_series-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.2.1/ebb_time_series/__init__.py
+-rw-r--r--   0        0        0      431 2024-05-16 21:52:46.364371 ebb_time_series-0.2.1/ebb_time_series/constants.py
+-rw-r--r--   0        0        0      233 2024-05-16 16:14:33.959702 ebb_time_series-0.2.1/ebb_time_series/data_schema.py
+-rw-r--r--   0        0        0     1195 2024-05-16 16:14:33.959938 ebb_time_series-0.2.1/ebb_time_series/event_parser_helpers.py
+-rw-r--r--   0        0        0      305 2024-05-16 21:52:46.364838 ebb_time_series-0.2.1/ebb_time_series/exceptions.py
+-rw-r--r--   0        0        0    10281 2024-05-16 21:52:46.365337 ebb_time_series-0.2.1/ebb_time_series/writers/aws_timestream_data_writer.py
+-rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.2.1/ebb_time_series/writers/base_data_writer.py
+-rw-r--r--   0        0        0      551 2024-05-16 21:52:46.365725 ebb_time_series-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.2.1/PKG-INFO
```

### Comparing `ebb_time_series-0.2.0/LICENSE` & `ebb_time_series-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.0/README.md` & `ebb_time_series-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.0/ebb_time_series/event_parser_helpers.py` & `ebb_time_series-0.2.1/ebb_time_series/event_parser_helpers.py`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.0/ebb_time_series/writers/aws_timestream_data_writer.py` & `ebb_time_series-0.2.1/ebb_time_series/writers/aws_timestream_data_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import boto3
 import logging
 from botocore.config import Config
+from botocore.exceptions import ClientError
 from enum import Enum
 from ebb_events.consumers.event_consumer import EventConsumer
 from ebb_time_series.constants import (
     DATA_VALUE_FIELDNAME,
     MAX_ATTEMPTS,
     MAX_POOL_CONNECTIONS,
     ORGANIZATION_FIELDNAME,
     READ_TIMEOUT,
     SYSTEM_FIELDNAME,
     SUBSYSTEM_FIELDNAME,
     DEVICE_FIELDNAME,
     SERIAL_NUMBER_FIELDNAME,
+    EVENT_ID_FIELDNAME,
 )
 from ebb_time_series.data_schema import DataSchema
 from ebb_time_series.event_parser_helpers import slugify_name_and_units
 from ebb_time_series.exceptions import TimeSeriesWriteException
 from ebb_time_series.writers.base_data_writer import BaseDataWriter
 from marshmallow import ValidationError
 
@@ -178,31 +180,32 @@
             region_name=self.aws_region,
             read_timeout=READ_TIMEOUT,
             max_pool_connections=MAX_POOL_CONNECTIONS,
             retries={"max_attempts": MAX_ATTEMPTS},
         )
         try:
             event_id = event_consumer.get_event_id()
-            # Timestamp in milliseconds - must be string for boto3 write
-            timestamp_str = str(event_consumer.get_event_time().timestamp() * 1000)
+            # Timestamp in milliseconds
+            timestamp_ms = event_consumer.get_event_time().timestamp() * 1000
 
             # Build dimension data dict from event_envelope fields and values
             dimensions_data = {
                 ORGANIZATION_FIELDNAME: event_consumer.get_event_organization(),
                 SYSTEM_FIELDNAME: event_consumer.get_event_system_id(),
                 SUBSYSTEM_FIELDNAME: event_consumer.get_event_subsystem_id(),
                 DEVICE_FIELDNAME: event_consumer.get_event_device_id(),
                 SERIAL_NUMBER_FIELDNAME: event_consumer.get_device_serial_number(),
+                EVENT_ID_FIELDNAME: event_id,
             }
             dimensions = self._build_aws_dimensions(dimensions_dict=dimensions_data)
 
             # Build common attributes dict for aws timestream writer
             common_attributes = {
                 AwsTimestreamFields.DIMENSIONS.value: dimensions,
-                AwsTimestreamFields.TIME.value: timestamp_str,
+                AwsTimestreamFields.TIME.value: str(timestamp_ms),
                 AwsTimestreamFields.TIMEUNIT.value: AwsTimestreamTimeUnitTypes.MILLISECONDS.value,
             }
 
             # Parse event message data to build records
             records = self._parse_event_data(event_consumer=event_consumer)
             # Initialize the timestream writer and write to database
             timestream_writer = boto3.client("timestream-write", config=config)
@@ -212,20 +215,34 @@
                 Records=records,
                 CommonAttributes=common_attributes,
             )
             logging.info(
                 f"Successfully wrote event {event_id} data to database {self.db_name}, table {self.table_name}."
             )
             return True
+        except ClientError as error:
+            logging.error(
+                f"Error writting event data {event_id} to database.",
+                extra={
+                    "error": str(error),
+                    "error_resposne": str(error.response.get("Error")),
+                    "event_id": event_id,
+                    "db_name": self.db_name,
+                    "table_name": self.table_name,
+                },
+            )
+            raise TimeSeriesWriteException(
+                f"Unable to write records to database: {str(error.response.get('Error', error))}"
+            ) from error
         except Exception as error:
             logging.error(
                 f"Error writting event data {event_id} to database.",
                 extra={
                     "error": str(error),
                     "event_id": event_id,
                     "db_name": self.db_name,
                     "table_name": self.table_name,
                 },
             )
             raise TimeSeriesWriteException(
                 f"Unable to write records to database: {str(error)}"
-            )
+            ) from error
```

### Comparing `ebb_time_series-0.2.0/ebb_time_series/writers/base_data_writer.py` & `ebb_time_series-0.2.1/ebb_time_series/writers/base_data_writer.py`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.0/pyproject.toml` & `ebb_time_series-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-time-series"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ebb-events = "^0.3.2"
```

### Comparing `ebb_time_series-0.2.0/PKG-INFO` & `ebb_time_series-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-time-series
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

