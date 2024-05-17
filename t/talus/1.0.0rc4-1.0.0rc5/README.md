# Comparing `tmp/talus-1.0.0rc4.tar.gz` & `tmp/talus-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-1.0.0rc4.tar", last modified: Wed May 15 21:18:11 2024, max compression
+gzip compressed data, was "talus-1.0.0rc5.tar", last modified: Fri May 17 21:40:12 2024, max compression
```

## Comparing `talus-1.0.0rc4.tar` & `talus-1.0.0rc5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:18:11.805712 talus-1.0.0rc4/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-15 21:17:58.000000 talus-1.0.0rc4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-15 21:17:58.000000 talus-1.0.0rc4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-15 21:17:58.000000 talus-1.0.0rc4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-15 21:17:58.000000 talus-1.0.0rc4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-15 21:18:11.805712 talus-1.0.0rc4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-15 21:17:58.000000 talus-1.0.0rc4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-15 21:17:58.000000 talus-1.0.0rc4/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-15 21:17:58.000000 talus-1.0.0rc4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-15 21:18:11.805712 talus-1.0.0rc4/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:18:11.801712 talus-1.0.0rc4/talus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-15 21:18:11.000000 talus-1.0.0rc4/talus/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/consumer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:18:11.801712 talus-1.0.0rc4/talus/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/binding.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     2393 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/models/retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:18:11.801712 talus-1.0.0rc4/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4660 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:18:11.805712 talus-1.0.0rc4/talus/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/models/test_binding.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/models/test_connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3935 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/models/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     6266 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/models/test_processor.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/models/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/models/test_retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-15 21:17:58.000000 talus-1.0.0rc4/talus/tests/test_producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-15 21:18:11.805712 talus-1.0.0rc4/talus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-15 21:18:11.000000 talus-1.0.0rc4/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-15 21:18:11.000000 talus-1.0.0rc4/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-15 21:18:11.000000 talus-1.0.0rc4/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-15 21:18:11.000000 talus-1.0.0rc4/talus.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-15 21:18:11.000000 talus-1.0.0rc4/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-15 21:18:11.000000 talus-1.0.0rc4/talus.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-15 21:17:58.000000 talus-1.0.0rc4/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-17 21:40:00.000000 talus-1.0.0rc5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-17 21:40:00.000000 talus-1.0.0rc5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-17 21:40:00.000000 talus-1.0.0rc5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-17 21:40:00.000000 talus-1.0.0rc5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-17 21:40:12.355312 talus-1.0.0rc5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-17 21:40:00.000000 talus-1.0.0rc5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-17 21:40:00.000000 talus-1.0.0rc5/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-17 21:40:00.000000 talus-1.0.0rc5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-17 21:40:12.355312 talus-1.0.0rc5/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.351312 talus-1.0.0rc5/talus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4660 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3935 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-17 21:40:00.000000 talus-1.0.0rc5/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-17 21:40:12.355312 talus-1.0.0rc5/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3201 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-17 21:40:12.000000 talus-1.0.0rc5/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-17 21:40:00.000000 talus-1.0.0rc5/tox.ini
```

### Comparing `talus-1.0.0rc4/.gitignore` & `talus-1.0.0rc5/.gitignore`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/.pre-commit-config.yaml` & `talus-1.0.0rc5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/LICENSE` & `talus-1.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/PKG-INFO` & `talus-1.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc4/README.rst` & `talus-1.0.0rc5/README.rst`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/bitbucket-pipelines.yml` & `talus-1.0.0rc5/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/pyproject.toml` & `talus-1.0.0rc5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/base.py` & `talus-1.0.0rc5/talus/base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/consumer.py` & `talus-1.0.0rc5/talus/consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/models/binding.py` & `talus-1.0.0rc5/talus/models/binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/models/connection_parameters.py` & `talus-1.0.0rc5/talus/models/connection_parameters.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/models/message.py` & `talus-1.0.0rc5/talus/models/message.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/models/processor.py` & `talus-1.0.0rc5/talus/models/processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 import logging
 from abc import ABC
 from abc import abstractmethod
 from typing import Type
 
 import pika
 from pydantic import BaseModel
+from pydantic import ConfigDict
 from pydantic import Field
 from pydantic import ValidationError
 
 from talus.models.message import ConsumeMessageBase
+from talus.producer import DurableProducer
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_DEAD_LETTER_EXCEPTIONS = (ValidationError,)
 
 
 class MessageProcessorBase(BaseModel, ABC):
+    model_config = ConfigDict(arbitrary_types_allowed=True)
+
     message_cls: Type[ConsumeMessageBase]
     dead_letter_exceptions: Type[Exception] | tuple[Type[Exception]] = Field(
         default=DEFAULT_DEAD_LETTER_EXCEPTIONS
     )
+    producer: DurableProducer | None = None
 
     @abstractmethod
     def process_message(self, message: ConsumeMessageBase):
         pass  # pragma: no cover
 
     @classmethod
     def dlq_message(
@@ -58,14 +63,21 @@
             message = self.message_cls(method=method, properties=properties, body=body)
             self.process_message(message)
             self.acknowledge_message(channel=channel, message=message)
         except self.dead_letter_exceptions as e:
             self.dlq_message(channel=channel, method=method, properties=properties, exception=e)
         return self
 
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if self.producer is not None:
+            self.producer.disconnect()
+
 
 class DLQMessageProcessor(MessageProcessorBase):
     message_cls: Type[ConsumeMessageBase] = ConsumeMessageBase
     dead_letter_exceptions: Type[Exception] | tuple[Type[Exception]] = Field(
         default_factory=lambda: DEFAULT_DEAD_LETTER_EXCEPTIONS + (ValueError,)
     )
```

### Comparing `talus-1.0.0rc4/talus/models/retryer.py` & `talus-1.0.0rc5/talus/models/retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/producer.py` & `talus-1.0.0rc5/talus/producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/conftest.py` & `talus-1.0.0rc5/talus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/models/test_binding.py` & `talus-1.0.0rc5/talus/tests/models/test_binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/models/test_message.py` & `talus-1.0.0rc5/talus/tests/models/test_message.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/models/test_processor.py` & `talus-1.0.0rc5/talus/tests/models/test_processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 """Tests for the message processor models."""
 from typing import Type
 from uuid import uuid4
 
 import pika
 import pytest
+from pydantic import Field
 
+from talus.models.connection_parameters import ProducerConnectionParameterFactory
 from talus.models.message import ConsumeMessageBase
 from talus.models.processor import DLQMessageProcessor
 from talus.models.processor import MessageProcessorBase
 from talus.models.processor import MessageProcessorRoutingKeySelector
+from talus.models.retryer import ConnectionRetryerFactory
+from talus.producer import DurableProducer
 
 
 @pytest.fixture()
 def successful_message_processor(consume_message_cls) -> MessageProcessorBase:
     """
     A message processor that does not raise an exception.
     """
 
     class SuccessfulMessageProcessor(MessageProcessorBase):
         message_cls: Type[ConsumeMessageBase] = consume_message_cls
 
         def process_message(self, message: ConsumeMessageBase):
             self._message_was_processed = True
 
-    yield SuccessfulMessageProcessor()
+    with SuccessfulMessageProcessor() as processor:
+        yield processor
 
 
 @pytest.fixture()
 def consumed_message(
     publish_message_cls,
     producer,
     consumer,
@@ -66,15 +71,16 @@
     class ErroringMessageProcessor(MessageProcessorBase):
         message_cls: Type[ConsumeMessageBase] = consume_message_cls
         dead_letter_exceptions: Type[Exception] = ValueError
 
         def process_message(self, message: ConsumeMessageBase):
             raise RuntimeError("A bad message processor raised an exception that is not DLQ'd.")
 
-    yield ErroringMessageProcessor()
+    with ErroringMessageProcessor() as processor:
+        yield processor
 
 
 def test_message_processor_failure(erroring_message_processor, consumed_message, consumer):
     """
     :given: A message processor that raises an exception.
     :when: The message processor is called.
     :then: Expected exception is raised.
@@ -98,15 +104,16 @@
         message_cls: Type[ConsumeMessageBase] = consume_message_cls
         dead_letter_exceptions: Type[Exception] = RuntimeError
 
         def process_message(self, message: ConsumeMessageBase):
             self._raised_run_time_error = True
             raise RuntimeError("A bad message processor raised an exception that is DLQ'd.")
 
-    yield AutoDLQMessageProcessor()
+    with AutoDLQMessageProcessor() as processor:
+        yield processor
 
 
 def test_dlq_message_processor(dlq_message_processor, consumed_message, consumer):
     """
     :given: A message processor that raises an exception identified as for DLQ.
     :when: The message processor is called.
     :then: The message processor should DLQ the message.
@@ -168,7 +175,48 @@
     # when/then
     message_processor = message_processor_routing_key_selector(
         channel=consumer.channel, method=method, properties=properties, body=body
     )
     # then
     assert not consumer.channel.get_waiting_message_count()  # no messages left in the queue
     assert isinstance(message_processor, DLQMessageProcessor)
+
+
+@pytest.fixture()
+def message_processor_cls_with_producer(producer, queue_bindings, direct_exchange):
+    """
+    A message processor that has a producer.
+    """
+    durable_producer = producer
+
+    class MessageProcessorWithProducer(MessageProcessorBase):
+        message_cls: Type[ConsumeMessageBase] = ConsumeMessageBase
+        producer: DurableProducer = Field(default_factory=lambda: durable_producer)
+
+        def process_message(self, message: ConsumeMessageBase):
+            pass
+
+    return MessageProcessorWithProducer
+
+
+@pytest.mark.parametrize(
+    "connect_producer",
+    [
+        pytest.param(True, id="connect_producer"),
+        pytest.param(False, id="no_connect_producer"),
+    ],
+)
+def test_message_processor_producer_disconnect(
+    message_processor_cls_with_producer, producer, connect_producer
+):
+    """
+    :given: A message processor that has a producer.
+    :when: The message processor is exited.
+    :then: The producer should be disconnected.
+    """
+    # given
+    with message_processor_cls_with_producer() as processor:
+        # when
+        if connect_producer:
+            processor.producer.connect()
+    # then
+    assert producer.connection.is_closed
```

### Comparing `talus-1.0.0rc4/talus/tests/models/test_queue.py` & `talus-1.0.0rc5/talus/tests/models/test_queue.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/models/test_retryer.py` & `talus-1.0.0rc5/talus/tests/models/test_retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/test_base.py` & `talus-1.0.0rc5/talus/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/test_consumer.py` & `talus-1.0.0rc5/talus/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus/tests/test_producer.py` & `talus-1.0.0rc5/talus/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/talus.egg-info/PKG-INFO` & `talus-1.0.0rc5/talus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc4/talus.egg-info/SOURCES.txt` & `talus-1.0.0rc5/talus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc4/tox.ini` & `talus-1.0.0rc5/tox.ini`

 * *Files identical despite different names*

