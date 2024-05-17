# Comparing `tmp/ebb_time_series-0.2.2.tar.gz` & `tmp/ebb_time_series-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebb_time_series-0.2.2.tar", max compression
+gzip compressed data, was "ebb_time_series-0.2.3.tar", max compression
```

## Comparing `ebb_time_series-0.2.2.tar` & `ebb_time_series-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.2.2/LICENSE
--rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.2.2/README.md
--rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.2.2/ebb_time_series/__init__.py
--rw-r--r--   0        0        0      431 2024-05-16 21:52:46.364371 ebb_time_series-0.2.2/ebb_time_series/constants.py
--rw-r--r--   0        0        0      233 2024-05-16 16:14:33.959702 ebb_time_series-0.2.2/ebb_time_series/data_schema.py
--rw-r--r--   0        0        0     1195 2024-05-16 16:14:33.959938 ebb_time_series-0.2.2/ebb_time_series/event_parser_helpers.py
--rw-r--r--   0        0        0      305 2024-05-16 21:52:46.364838 ebb_time_series-0.2.2/ebb_time_series/exceptions.py
--rw-r--r--   0        0        0    10492 2024-05-16 22:02:38.398938 ebb_time_series-0.2.2/ebb_time_series/writers/aws_timestream_data_writer.py
--rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.2.2/ebb_time_series/writers/base_data_writer.py
--rw-r--r--   0        0        0      551 2024-05-16 22:02:52.989844 ebb_time_series-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 22:25:27.000848 ebb_time_series-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2264 2024-05-13 22:11:05.101506 ebb_time_series-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 22:25:27.006306 ebb_time_series-0.2.3/ebb_time_series/__init__.py
+-rw-r--r--   0        0        0      431 2024-05-16 21:52:46.364371 ebb_time_series-0.2.3/ebb_time_series/constants.py
+-rw-r--r--   0        0        0      233 2024-05-16 16:14:33.959702 ebb_time_series-0.2.3/ebb_time_series/data_schema.py
+-rw-r--r--   0        0        0     1195 2024-05-16 16:14:33.959938 ebb_time_series-0.2.3/ebb_time_series/event_parser_helpers.py
+-rw-r--r--   0        0        0      305 2024-05-16 21:52:46.364838 ebb_time_series-0.2.3/ebb_time_series/exceptions.py
+-rw-r--r--   0        0        0    10305 2024-05-16 22:09:22.619720 ebb_time_series-0.2.3/ebb_time_series/writers/aws_timestream_data_writer.py
+-rw-r--r--   0        0        0     2110 2024-05-16 16:14:33.960966 ebb_time_series-0.2.3/ebb_time_series/writers/base_data_writer.py
+-rw-r--r--   0        0        0      551 2024-05-16 22:09:53.744474 ebb_time_series-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 ebb_time_series-0.2.3/PKG-INFO
```

### Comparing `ebb_time_series-0.2.2/LICENSE` & `ebb_time_series-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.2/README.md` & `ebb_time_series-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.2/ebb_time_series/event_parser_helpers.py` & `ebb_time_series-0.2.3/ebb_time_series/event_parser_helpers.py`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.2/ebb_time_series/writers/aws_timestream_data_writer.py` & `ebb_time_series-0.2.3/ebb_time_series/writers/aws_timestream_data_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,15 +131,14 @@
         Exceptions:
             Raises ebb_events `PayloadFormatException` or marshmallow `ValidationError` if format does not match expected structure.
         """
         list_of_records = []
 
         # Raises PayloadFormatException or marshmallow.ValidationError if incorrect format
         event_data: dict = event_consumer.get_event_message(metadata_included=False)
-        event_timestamp_ms = event_consumer.get_event_time().timestamp() * 1000
         # Raises ValidationError if any value isn't of format {"value": ___, "units": ___}
         try:
             DataSchema(many=True).load(list(event_data.values()))
         except ValidationError as error:
             logging.error(
                 f"Payload data does not match expected data schema: {str(error)}."
             )
@@ -156,16 +155,15 @@
             }
             list_of_records.append(record)
 
         return [
             {
                 AwsTimestreamFields.MEASURENAME.value: "measurement",
                 AwsTimestreamFields.MEASURVALUES.value: list_of_records,
-                AwsTimestreamFields.MEASUREVALUETYPE.value: AwsTimestreamValueTypes.MULTI.value,
-                AwsTimestreamFields.TIME.value: str(event_timestamp_ms)
+                AwsTimestreamFields.MEASUREVALUETYPE.value: AwsTimestreamValueTypes.MULTI.value
             }
         ]
 
     def write_event_record(self, event_consumer: EventConsumer) -> bool:
         """
         Main writer method that takes in the consumed event payload, parses the data, and writes
         records to the desired database table.
@@ -199,15 +197,15 @@
                 EVENT_ID_FIELDNAME: event_id,
             }
             dimensions = self._build_aws_dimensions(dimensions_dict=dimensions_data)
 
             # Build common attributes dict for aws timestream writer
             common_attributes = {
                 AwsTimestreamFields.DIMENSIONS.value: dimensions,
-                # AwsTimestreamFields.TIME.value: str(timestamp_ms),
+                AwsTimestreamFields.TIME.value: str(timestamp_ms),
                 AwsTimestreamFields.TIMEUNIT.value: AwsTimestreamTimeUnitTypes.MILLISECONDS.value,
             }
 
             # Parse event message data to build records
             records = self._parse_event_data(event_consumer=event_consumer)
             # Initialize the timestream writer and write to database
             timestream_writer = boto3.client("timestream-write", config=config)
@@ -229,15 +227,15 @@
                     "error_resposne": str(error.response.get("Error")),
                     "event_id": event_id,
                     "db_name": self.db_name,
                     "table_name": self.table_name,
                 },
             )
             raise TimeSeriesWriteException(
-                f"Unable to write records to database: {str(error.response.get('Error', error))}. Timestamp: {str(timestamp_ms)}", response=error.response
+                f"Unable to write records to database: {str(error.response.get('Error', error))}", response=error.response
             ) from error
         except Exception as error:
             logging.error(
                 f"Error writting event data {event_id} to database.",
                 extra={
                     "error": str(error),
                     "event_id": event_id,
```

### Comparing `ebb_time_series-0.2.2/ebb_time_series/writers/base_data_writer.py` & `ebb_time_series-0.2.3/ebb_time_series/writers/base_data_writer.py`

 * *Files identical despite different names*

### Comparing `ebb_time_series-0.2.2/pyproject.toml` & `ebb_time_series-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ebb-time-series"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["Ryan Bloom <ryan.bloom@ebbcarbon.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ebb-events = "^0.3.2"
```

### Comparing `ebb_time_series-0.2.2/PKG-INFO` & `ebb_time_series-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebb-time-series
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Ryan Bloom
 Author-email: ryan.bloom@ebbcarbon.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

