# Comparing `tmp/autogencap_rajan_jedi-0.0.6.tar.gz` & `tmp/autogencap_rajan_jedi-0.0.7.tar.gz`

## Comparing `autogencap_rajan_jedi-0.0.6.tar` & `autogencap_rajan_jedi-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,38 @@
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/Actor.py
--rw-r--r--   0        0        0     6092 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ActorConnector.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/Broker.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/Config.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/Constants.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/DebugLog.py
--rw-r--r--   0        0        0     8877 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/DirectorySvc.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/LocalActorNetwork.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/requirements.txt
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/setup.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/utility.py
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/AG2CAP.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/AGActor.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/AutoGenConnector.py
--rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAP2AG.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAPGroupChat.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAPGroupChatManager.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAPPair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/__init__.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/agent.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/Autogen.proto
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/Autogen_pb2.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/Autogen_pb2.pyi
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/CAP.proto
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/CAP_pb2.py
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/CAP_pb2.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/autogencap/proto/proto-instructions.txt
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/.gitignore
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/README.md
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Actor.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ActorConnector.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Broker.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Config.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/Constants.py
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/DebugLog.py
+-rw-r--r--   0        0        0     8917 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/DirectorySvc.py
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/LocalActorNetwork.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/requirements.txt
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/setup.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/utility.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AG2CAP.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AGActor.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AutoGenConnector.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAP2AG.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChat.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChatManager.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPPair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/__init__.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/agent.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen.proto
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.py
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.pyi
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP.proto
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAPAgents_pb2.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAPAgents_pb2.pyi
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/proto-instructions.txt
+-rwxr-xr-x   0        0        0 11783121 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/protoc.exe
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/autogencap/proto/test.seqdiag
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/README.md
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 autogencap_rajan_jedi-0.0.7/PKG-INFO
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/Actor.py` & `autogencap_rajan_jedi-0.0.7/autogencap/Actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import zmq
 import threading
-import traceback
 import time
-from .DebugLog import Debug, Info, Error
+import traceback
+
+import zmq
+
 from .Config import xpub_url
+from .DebugLog import Debug, Error, Info
 
 
 class Actor:
     def __init__(self, agent_name: str, description: str):
         self.actor_name: str = agent_name
         self.agent_description: str = description
         self.run = False
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/ActorConnector.py` & `autogencap_rajan_jedi-0.0.7/autogencap/ActorConnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Agent_Sender takes a zmq context, Topic and creates a
 # socket that can publish to that topic. It exposes this functionality
 # using send_msg method
-import zmq
-from zmq.utils.monitor import recv_monitor_message
 import time
 import uuid
-from .DebugLog import Debug, Error, Info
-from .Config import xsub_url, xpub_url, router_url
 from typing import Any, Dict
 
+import zmq
+from zmq.utils.monitor import recv_monitor_message
+
+from .Config import router_url, xpub_url, xsub_url
+from .DebugLog import Debug, Error, Info
+
 
 class ActorSender:
     def __init__(self, context, topic):
         self._context = context
         self._topic = topic
         self._connect_pub_socket()
 
@@ -128,22 +130,23 @@
             self._sender.send_bin_request_msg(msg_type, msg, self._resp_topic)
             while num_attempts == -1 or num_attempts > 0:
                 try:
                     topic, resp_msg_type, _, resp = self._resp_socket.recv_multipart()
                     return topic, resp_msg_type, resp
                 except zmq.Again:
                     Debug(
-                        "ActorConnector", f"{self._topic}: No response received. retry_count={num_attempts}, max_retry={num_attempts}"
+                        "ActorConnector",
+                        f"{self._topic}: No response received. retry_count={num_attempts}, max_retry={num_attempts}",
                     )
                     time.sleep(0.01)
                     if num_attempts != -1:
                         num_attempts -= 1
         finally:
             if num_attempts == -1:
                 self._resp_socket.setsockopt(zmq.RCVTIMEO, original_timeout)
 
         Error("ActorConnector", f"{self._topic}: No response received. Giving up.")
         return None, None, None
 
     def close(self):
-        self._sender.close()
+        self._pub_socket.close()
         self._resp_socket.close()
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/Broker.py` & `autogencap_rajan_jedi-0.0.7/autogencap/Broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import threading
 import time
+
 import zmq
-import threading
+
+from autogencap.Config import router_url, xpub_url, xsub_url
 from autogencap.DebugLog import Debug, Info, Warn
-from autogencap.Config import xsub_url, xpub_url, router_url
 
 
 class Broker:
     def __init__(self, context: zmq.Context = zmq.Context()):
         self._context: zmq.Context = context
         self._run: bool = False
         self._xpub: zmq.Socket = None
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/DebugLog.py` & `autogencap_rajan_jedi-0.0.7/autogencap/DebugLog.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,76 @@
-import threading
 import datetime
-import autogencap.Config as Config
+import threading
+
 from termcolor import colored
 
+import autogencap.Config as Config
+
 # Define log levels as constants
 DEBUG = 0
 INFO = 1
 WARN = 2
 ERROR = 3
 
 # Map log levels to their names
 LEVEL_NAMES = ["DBG", "INF", "WRN", "ERR"]
 LEVEL_COLOR = ["dark_grey", "green", "yellow", "red"]
 
-console_lock = threading.Lock()
+
+class BaseLogger:
+    def __init__(self):
+        self._lock = threading.Lock()
+
+    def Log(self, level, context, msg):
+        # Check if the current level meets the threshold
+        if level >= Config.LOG_LEVEL:  # Use the LOG_LEVEL from the Config module
+            # Check if the context is in the list of ignored contexts
+            if context in Config.IGNORED_LOG_CONTEXTS:
+                return
+            with self._lock:
+                self.WriteLog(level, context, msg)
+
+    def WriteLog(self, level, context, msg):
+        raise NotImplementedError("Subclasses must implement this method")
+
+
+class ConsoleLogger(BaseLogger):
+    def __init__(self):
+        super().__init__()
+
+    def WriteLog(self, level, context, msg):
+        timestamp = colored(datetime.datetime.now().strftime("%m/%d/%y %H:%M:%S"), "pink")
+        # Translate level number to name and color
+        level_name = colored(LEVEL_NAMES[level], LEVEL_COLOR[level])
+        # Left justify the context and color it blue
+        context = colored(context.ljust(14), "blue")
+        # Left justify the threadid and color it blue
+        thread_id = colored(str(threading.get_ident()).ljust(5), "blue")
+        # color the msg based on the level
+        msg = colored(msg, LEVEL_COLOR[level])
+        print(f"{thread_id} {timestamp} {level_name}: [{context}] {msg}")
 
 
-def Log(level, context, msg):
-    # Check if the current level meets the threshold
-    if level >= Config.LOG_LEVEL:  # Use the LOG_LEVEL from the Config module
-        # Check if the context is in the list of ignored contexts
-        if context in Config.IGNORED_LOG_CONTEXTS:
-            return
-        with console_lock:
-            timestamp = colored(datetime.datetime.now().strftime("%m/%d/%y %H:%M:%S"), "dark_grey")
-            # Translate level number to name and color
-            level_name = colored(LEVEL_NAMES[level], LEVEL_COLOR[level])
-            # Left justify the context and color it blue
-            context = colored(context.ljust(14), "blue")
-            # Left justify the threadid and color it blue
-            thread_id = colored(str(threading.get_ident()).ljust(5), "blue")
-            # color the msg based on the level
-            msg = colored(msg, LEVEL_COLOR[level])
-            print(f"{thread_id} {timestamp} {level_name}: [{context}] {msg}")
+LOGGER = ConsoleLogger()
 
 
 def Debug(context, message):
-    Log(DEBUG, context, message)
+    LOGGER.Log(DEBUG, context, message)
 
 
 def Info(context, message):
-    Log(INFO, context, message)
+    LOGGER.Log(INFO, context, message)
 
 
 def Warn(context, message):
-    Log(WARN, context, message)
+    LOGGER.Log(WARN, context, message)
 
 
 def Error(context, message):
-    Log(ERROR, context, message)
+    LOGGER.Log(ERROR, context, message)
 
 
 def shorten(msg, num_parts=5, max_len=100):
     # Remove new lines
     msg = msg.replace("\n", " ")
 
     # If the message is shorter than or equal to max_len characters, return it as is
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/DirectorySvc.py` & `autogencap_rajan_jedi-0.0.7/autogencap/DirectorySvc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from autogencap.Constants import Directory_Svc_Topic
-from autogencap.Config import xpub_url, xsub_url, router_url
-from autogencap.DebugLog import Debug, Info, Error
-from autogencap.ActorConnector import ActorConnector, ActorSender
+import re
+import threading
+import time
+
+import zmq
+
 from autogencap.Actor import Actor
+from autogencap.ActorConnector import ActorConnector, ActorSender
 from autogencap.Broker import Broker
+from autogencap.Config import router_url, xpub_url, xsub_url
+from autogencap.Constants import Directory_Svc_Topic
+from autogencap.DebugLog import Debug, Error, Info
 from autogencap.proto.CAP_pb2 import (
-    ActorRegistration,
     ActorInfo,
+    ActorInfoCollection,
     ActorLookup,
     ActorLookupResponse,
+    ActorRegistration,
+    ErrorCode,
     Ping,
     Pong,
-    ActorInfoCollection,
+)
+from autogencap.proto.CAP_pb2 import (
     Error as ErrorMsg,
-    ErrorCode,
 )
 from autogencap.utility import report_error_msg
 
-import zmq
-import threading
-import time
-import re
-
 # TODO (Future DirectorySv PR) use actor description, network_id, other properties to make directory
 # service more generic and powerful
 
 
 class DirectoryActor(Actor):
     def __init__(self, topic: str, name: str):
         super().__init__(topic, name)
@@ -93,25 +96,26 @@
         else:
             Error("DirectorySvc", f"Actor not found: {actor_lookup.actor_info.name}")
 
         sender_connection = ActorSender(self._context, sender_topic)
         serialized_msg = actor_lookup_resp.SerializeToString()
         sender_connection.send_bin_msg(ActorLookupResponse.__name__, serialized_msg)
 
+
 class DirectorySvc:
     def __init__(self, context: zmq.Context = zmq.Context()):
         self._context: zmq.Context = context
         self._directory_connector: ActorConnector = None
         self._directory_actor: DirectoryActor = None
 
     def _no_other_directory(self) -> bool:
         Debug("DirectorySvc", "Pinging existing DirectorySvc")
         ping = Ping()
         serialized_msg = ping.SerializeToString()
-        _, _, resp = self._directory_connector.binary_request(Ping.__name__, serialized_msg, num_attempts=1)
+        _, _, resp = self._directory_connector.binary_request(Ping.__name__, serialized_msg, retry=1)
         if resp is None:
             return True
         return False
 
     def start(self):
         Debug("DirectorySvc", "Starting.")
         self._directory_connector = ActorConnector(self._context, Directory_Svc_Topic)
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/LocalActorNetwork.py` & `autogencap_rajan_jedi-0.0.7/autogencap/LocalActorNetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+import time
+from typing import List
+
 import zmq
-from .DebugLog import Debug, Warn
+
+from .Actor import Actor
 from .ActorConnector import ActorConnector
 from .Broker import Broker
-from .DirectorySvc import DirectorySvc
 from .Constants import Termination_Topic
-from .Actor import Actor
+from .DebugLog import Debug, Warn
+from .DirectorySvc import DirectorySvc
 from .proto.CAP_pb2 import ActorInfo, ActorInfoCollection
-from typing import List
-import time
 
 # TODO: remove time import
 
 
 class LocalActorNetwork:
     def __init__(self, name: str = "Local Actor Network", start_broker: bool = True):
         self.local_actors = {}
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/AG2CAP.py` & `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AG2CAP.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import time
 from typing import Callable, Dict, List, Optional, Union
+
 from autogen import Agent, ConversableAgent
-from .AutoGenConnector import AutoGenConnector
+
 from ..LocalActorNetwork import LocalActorNetwork
+from .AutoGenConnector import AutoGenConnector
 
 
 class AG2CAP(ConversableAgent):
     """
     A conversable agent proxy that sends messages to CAN when called
     """
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/AutoGenConnector.py` & `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/AutoGenConnector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import json
 from typing import Dict, Optional, Union
+
 from autogen import Agent
+
 from ..ActorConnector import ActorConnector
 from ..proto.Autogen_pb2 import GenReplyReq, GenReplyResp, PrepChat, ReceiveReq, Terminate
 
+
 class AutoGenConnector:
     """
     A specialized ActorConnector class for sending and receiving Autogen messages
     to/from the CAP system.
     """
 
     def __init__(self, cap_sender: ActorConnector):
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAP2AG.py` & `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAP2AG.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import json
 from enum import Enum
 from typing import Optional
+
+from autogen import ConversableAgent
+
 from ..DebugLog import Debug, Error, Info, Warn, shorten
 from ..LocalActorNetwork import LocalActorNetwork
 from ..proto.Autogen_pb2 import GenReplyReq, GenReplyResp, PrepChat, ReceiveReq, Terminate
-from .AGActor import AGActor
 from .AG2CAP import AG2CAP
-from autogen import ConversableAgent
+from .AGActor import AGActor
 
 
 class CAP2AG(AGActor):
     """
     A CAN actor that acts as an adapter for the AutoGen system.
     """
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAPGroupChat.py` & `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from typing import List
+
 from autogen import Agent, AssistantAgent, GroupChat
 from autogencap.ag_adapter.AG2CAP import AG2CAP
 from autogencap.ag_adapter.CAP2AG import CAP2AG
 from autogencap.LocalActorNetwork import LocalActorNetwork
-from typing import List
 
 
 class CAPGroupChat(GroupChat):
     def __init__(
         self,
         agents: List[AssistantAgent],
         messages: List[str],
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAPGroupChatManager.py` & `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPGroupChatManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import time
+
 from autogen import GroupChatManager
 from autogencap.ActorConnector import ActorConnector
-from autogencap.LocalActorNetwork import LocalActorNetwork
 from autogencap.ag_adapter.CAP2AG import CAP2AG
 from autogencap.ag_adapter.CAPGroupChat import CAPGroupChat
-import time
+from autogencap.LocalActorNetwork import LocalActorNetwork
 
 
 class CAPGroupChatManager:
     def __init__(self, groupchat: CAPGroupChat, llm_config: dict, network: LocalActorNetwork):
         self._network: LocalActorNetwork = network
         self._cap_group_chat: CAPGroupChat = groupchat
         self._ag_group_chat_manager: GroupChatManager = GroupChatManager(
```

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/ag_adapter/CAPPair.py` & `autogencap_rajan_jedi-0.0.7/autogencap/ag_adapter/CAPPair.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/proto/Autogen.proto` & `autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen.proto`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/proto/Autogen_pb2.py` & `autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/proto/Autogen_pb2.pyi` & `autogencap_rajan_jedi-0.0.7/autogencap/proto/Autogen_pb2.pyi`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/proto/CAP.proto` & `autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP.proto`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/proto/CAP_pb2.py` & `autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.py`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/autogencap/proto/CAP_pb2.pyi` & `autogencap_rajan_jedi-0.0.7/autogencap/proto/CAP_pb2.pyi`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/.gitignore` & `autogencap_rajan_jedi-0.0.7/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -168,18 +168,25 @@
 # DB on disk for Teachability
 tmp/
 test/my_tmp/*
 
 # Storage for the AgentEval output
 test/test_files/agenteval-in-out/out/
 
+# local cache or coding foler
+local_cache/
+coding/
+
 # Files created by tests
 *tmp_code_*
 test/agentchat/test_agent_scripts/*
 
 # test cache
 .cache_test
 .db
+local_cache
 
 
 notebook/result.png
 samples/apps/autogen-studio/autogenstudio/models/test/
+
+notebook/coding
```

### Comparing `autogencap_rajan_jedi-0.0.6/README.md` & `autogencap_rajan_jedi-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `autogencap_rajan_jedi-0.0.6/pyproject.toml` & `autogencap_rajan_jedi-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autogencap_rajan.jedi"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Rajan Chari", email="rajan.jedi@gmail.com" },
 ]
 dependencies = [
     "pyzmq >= 25.1.2",
     "protobuf >= 4.25.3",
     "termcolor >= 2.4.0",
```

### Comparing `autogencap_rajan_jedi-0.0.6/PKG-INFO` & `autogencap_rajan_jedi-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autogencap_rajan.jedi
-Version: 0.0.6
+Version: 0.0.7
 Summary: CAP w/ autogen bindings
 Project-URL: Homepage, https://github.com/microsoft/autogen
 Project-URL: Bug Tracker, https://github.com/microsoft/autogen/issues
 Author-email: Rajan Chari <rajan.jedi@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

