# Comparing `tmp/startrek-2.0.0.tar.gz` & `tmp/startrek-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/startrek-2.0.0.tar", last modified: Fri May 10 15:29:42 2024, max compression
+gzip compressed data, was "dist/startrek-2.1.0.tar", last modified: Fri May 17 11:40:32 2024, max compression
```

## Comparing `startrek-2.0.0.tar` & `startrek-2.1.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-10 15:29:42.000000 startrek-2.0.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-2.0.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:29:42.000000 startrek-2.0.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      826 2024-05-10 15:28:44.000000 startrek-2.0.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/
--rw-r--r--   0 moky       (501) staff       (20)     2520 2023-01-13 11:45:48.000000 startrek-2.0.0/startrek/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-2.0.0/startrek/arrival.py
--rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-2.0.0/startrek/departure.py
--rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-2.0.0/startrek/dock.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/fsm/
--rw-r--r--   0 moky       (501) staff       (20)     2109 2024-05-09 18:37:27.000000 startrek-2.0.0/startrek/fsm/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     2349 2024-05-07 05:04:10.000000 startrek-2.0.0/startrek/fsm/auto.py
--rw-r--r--   0 moky       (501) staff       (20)     8430 2024-05-07 05:02:58.000000 startrek-2.0.0/startrek/fsm/base.py
--rw-r--r--   0 moky       (501) staff       (20)     3845 2024-05-09 19:32:00.000000 startrek-2.0.0/startrek/fsm/daemon.py
--rw-r--r--   0 moky       (501) staff       (20)     5880 2024-05-07 04:58:28.000000 startrek-2.0.0/startrek/fsm/machine.py
--rw-r--r--   0 moky       (501) staff       (20)     4622 2024-05-09 18:45:29.000000 startrek-2.0.0/startrek/fsm/runner.py
--rw-r--r--   0 moky       (501) staff       (20)     4495 2024-05-09 18:40:20.000000 startrek-2.0.0/startrek/fsm/ticker.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/net/
--rw-r--r--   0 moky       (501) staff       (20)     3283 2023-01-13 11:39:06.000000 startrek-2.0.0/startrek/net/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9166 2024-05-07 05:08:01.000000 startrek-2.0.0/startrek/net/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     3384 2024-05-07 05:08:54.000000 startrek-2.0.0/startrek/net/connection.py
--rw-r--r--   0 moky       (501) staff       (20)     3416 2024-05-07 05:09:27.000000 startrek-2.0.0/startrek/net/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     3881 2024-05-07 15:28:01.000000 startrek-2.0.0/startrek/net/hub.py
--rw-r--r--   0 moky       (501) staff       (20)    17046 2024-05-07 05:11:00.000000 startrek-2.0.0/startrek/net/state.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/port/
--rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-2.0.0/startrek/port/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     3130 2024-05-07 05:12:48.000000 startrek-2.0.0/startrek/port/delegate.py
--rw-r--r--   0 moky       (501) staff       (20)     4442 2024-05-07 05:13:41.000000 startrek-2.0.0/startrek/port/docker.py
--rw-r--r--   0 moky       (501) staff       (20)     2643 2024-05-07 05:12:04.000000 startrek-2.0.0/startrek/port/gate.py
--rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-2.0.0/startrek/port/ship.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/socket/
--rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-2.0.0/startrek/socket/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     4446 2024-05-09 18:42:32.000000 startrek-2.0.0/startrek/socket/active_conn.py
--rw-r--r--   0 moky       (501) staff       (20)    11374 2024-05-07 14:40:01.000000 startrek-2.0.0/startrek/socket/base_channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10668 2024-05-07 05:24:27.000000 startrek-2.0.0/startrek/socket/base_conn.py
--rw-r--r--   0 moky       (501) staff       (20)    10165 2024-05-09 15:01:12.000000 startrek-2.0.0/startrek/socket/base_hub.py
--rw-r--r--   0 moky       (501) staff       (20)    10900 2024-05-07 14:34:30.000000 startrek-2.0.0/startrek/stardocker.py
--rw-r--r--   0 moky       (501) staff       (20)    11681 2024-05-09 15:01:24.000000 startrek-2.0.0/startrek/stargate.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek/types/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-2.0.0/startrek/types/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-2.0.0/startrek/types/mapping.py
--rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-2.0.0/startrek/types/pair.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      917 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)        9 2024-05-10 15:29:42.000000 startrek-2.0.0/startrek.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-17 11:40:32.000000 startrek-2.1.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       25 2021-05-06 07:15:56.000000 startrek-2.1.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 11:40:32.000000 startrek-2.1.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      826 2024-05-16 17:30:23.000000 startrek-2.1.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/
+-rw-r--r--   0 moky       (501) staff       (20)     2570 2024-05-17 03:38:09.000000 startrek-2.1.0/startrek/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5463 2024-03-06 13:31:40.000000 startrek-2.1.0/startrek/arrival.py
+-rw-r--r--   0 moky       (501) staff       (20)    11425 2024-03-06 13:32:13.000000 startrek-2.1.0/startrek/departure.py
+-rw-r--r--   0 moky       (501) staff       (20)     4960 2024-03-06 13:33:03.000000 startrek-2.1.0/startrek/dock.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/fsm/
+-rw-r--r--   0 moky       (501) staff       (20)     1806 2024-05-16 18:44:18.000000 startrek-2.1.0/startrek/fsm/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     2354 2024-05-16 18:44:59.000000 startrek-2.1.0/startrek/fsm/auto.py
+-rw-r--r--   0 moky       (501) staff       (20)     8430 2024-05-07 05:02:58.000000 startrek-2.1.0/startrek/fsm/base.py
+-rw-r--r--   0 moky       (501) staff       (20)     5884 2024-05-16 18:44:46.000000 startrek-2.1.0/startrek/fsm/machine.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/net/
+-rw-r--r--   0 moky       (501) staff       (20)     3310 2024-05-17 03:36:47.000000 startrek-2.1.0/startrek/net/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7022 2024-05-17 03:27:10.000000 startrek-2.1.0/startrek/net/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     3390 2024-05-16 18:45:43.000000 startrek-2.1.0/startrek/net/connection.py
+-rw-r--r--   0 moky       (501) staff       (20)     3416 2024-05-07 05:09:27.000000 startrek-2.1.0/startrek/net/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     3884 2024-05-17 10:08:40.000000 startrek-2.1.0/startrek/net/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)     4276 2024-05-17 10:11:09.000000 startrek-2.1.0/startrek/net/socket.py
+-rw-r--r--   0 moky       (501) staff       (20)    17046 2024-05-07 05:11:00.000000 startrek-2.1.0/startrek/net/state.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/port/
+-rw-r--r--   0 moky       (501) staff       (20)     3722 2024-03-06 09:27:29.000000 startrek-2.1.0/startrek/port/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3130 2024-05-07 05:12:48.000000 startrek-2.1.0/startrek/port/delegate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4448 2024-05-16 18:46:02.000000 startrek-2.1.0/startrek/port/docker.py
+-rw-r--r--   0 moky       (501) staff       (20)     2649 2024-05-16 18:46:09.000000 startrek-2.1.0/startrek/port/gate.py
+-rw-r--r--   0 moky       (501) staff       (20)     4127 2024-03-06 09:27:29.000000 startrek-2.1.0/startrek/port/ship.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/skywalker/
+-rw-r--r--   0 moky       (501) staff       (20)     1768 2024-05-16 18:51:08.000000 startrek-2.1.0/startrek/skywalker/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     3418 2024-05-16 18:33:35.000000 startrek-2.1.0/startrek/skywalker/daemon.py
+-rw-r--r--   0 moky       (501) staff       (20)     5038 2024-05-16 18:38:35.000000 startrek-2.1.0/startrek/skywalker/runner.py
+-rw-r--r--   0 moky       (501) staff       (20)     4524 2024-05-16 18:35:35.000000 startrek-2.1.0/startrek/skywalker/ticker.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/socket/
+-rw-r--r--   0 moky       (501) staff       (20)     1899 2024-03-06 13:22:07.000000 startrek-2.1.0/startrek/socket/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4456 2024-05-16 18:46:20.000000 startrek-2.1.0/startrek/socket/active_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    13048 2024-05-17 10:17:03.000000 startrek-2.1.0/startrek/socket/base_channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10668 2024-05-07 05:24:27.000000 startrek-2.1.0/startrek/socket/base_conn.py
+-rw-r--r--   0 moky       (501) staff       (20)    10182 2024-05-17 03:39:37.000000 startrek-2.1.0/startrek/socket/base_hub.py
+-rw-r--r--   0 moky       (501) staff       (20)    10900 2024-05-07 14:34:30.000000 startrek-2.1.0/startrek/stardocker.py
+-rw-r--r--   0 moky       (501) staff       (20)    11689 2024-05-16 18:47:32.000000 startrek-2.1.0/startrek/stargate.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek/types/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2024-03-06 07:44:45.000000 startrek-2.1.0/startrek/types/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     7196 2024-03-06 10:36:46.000000 startrek-2.1.0/startrek/types/mapping.py
+-rw-r--r--   0 moky       (501) staff       (20)     3721 2024-03-08 06:09:38.000000 startrek-2.1.0/startrek/types/pair.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      449 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      989 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)        9 2024-05-17 11:40:32.000000 startrek-2.1.0/startrek.egg-info/top_level.txt
```

### Comparing `startrek-2.0.0/setup.py` & `startrek-2.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~~~~~~~
 
     Interstellar Transport
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
```

### Comparing `startrek-2.0.0/startrek/__init__.py` & `startrek-2.1.0/startrek/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from .net import Hub, Channel
-from .net import Connection, ConnectionDelegate, ConnectionState
+from .net import Hub
+from .net import Channel, ChannelState
+from .net import Connection, ConnectionState, ConnectionDelegate
 
 from .socket import BaseChannel, ChannelReader, ChannelWriter
 from .socket import BaseHub, BaseConnection, ActiveConnection
 
 from .port import Ship, Arrival, Departure
 from .port import ShipStatus, DeparturePriority
 from .port import Docker, DockerStatus, DockerDelegate
@@ -47,16 +48,17 @@
 
 name = "StarTrek"
 
 __author__ = 'Albert Moky'
 
 __all__ = [
 
-    'Hub', 'Channel',
-    'Connection', 'ConnectionDelegate', 'ConnectionState',
+    'Hub',
+    'Channel', 'ChannelState',
+    'Connection', 'ConnectionState', 'ConnectionDelegate',
 
     'BaseChannel', 'ChannelReader', 'ChannelWriter',
     'BaseHub', 'BaseConnection', 'ActiveConnection',
 
     'Ship', 'Arrival', 'Departure',
     'ShipStatus', 'DeparturePriority',
     'Docker', 'DockerStatus', 'DockerDelegate',
```

### Comparing `startrek-2.0.0/startrek/arrival.py` & `startrek-2.1.0/startrek/arrival.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/departure.py` & `startrek-2.1.0/startrek/departure.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/dock.py` & `startrek-2.1.0/startrek/dock.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/fsm/__init__.py` & `startrek-2.1.0/startrek/fsm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,29 +29,21 @@
 # ==============================================================================
 
 """
     Finite State Machine
     ~~~~~~~~~~~~~~~~~~~~
 """
 
-from .ticker import Ticker, Metronome, PrimeMetronome, Singleton
-from .runner import Processor, Handler, Runnable, Runner
-from .daemon import Daemon, DaemonRunner
 from .machine import Context, Transition, State, Machine, Delegate
 from .base import BaseTransition, BaseState, BaseMachine
 from .auto import AutoMachine
 
 name = "FSM"
 
 __author__ = 'Albert Moky'
 
 __all__ = [
 
-    'Ticker', 'Metronome', 'PrimeMetronome', 'Singleton',
-
-    'Processor', 'Handler', 'Runnable', 'Runner',
-    'Daemon', 'DaemonRunner',
-
     'Context', 'Transition', 'State', 'Machine', 'Delegate',
     'BaseTransition', 'BaseState', 'BaseMachine',
     'AutoMachine',
 ]
```

### Comparing `startrek-2.0.0/startrek/fsm/auto.py` & `startrek-2.1.0/startrek/fsm/auto.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from abc import ABC  # , abstractmethod
 
-from .ticker import PrimeMetronome
+from ..skywalker import PrimeMetronome
+
 from .machine import S, C, U, T
 from .base import BaseMachine
 
 
 # noinspection PyAbstractClass
 class AutoMachine(BaseMachine[C, T, S], ABC):
```

### Comparing `startrek-2.0.0/startrek/fsm/base.py` & `startrek-2.1.0/startrek/fsm/base.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/fsm/machine.py` & `startrek-2.1.0/startrek/fsm/machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
 from abc import ABC, abstractmethod
 from typing import Optional, TypeVar, Generic
 
-from .ticker import Ticker
+from ..skywalker import Ticker
 
 S = TypeVar('S')  # State
 C = TypeVar('C')  # Context
 U = TypeVar('U')
 T = TypeVar('T')  # Transition
```

### Comparing `startrek-2.0.0/startrek/fsm/runner.py` & `startrek-2.1.0/startrek/port/docker.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-#   Finite State Machine
+#   Star Trek: Interstellar Transport
 #
 #                                Written in 2021 by Moky <albert.moky@gmail.com>
 #
 # ==============================================================================
 # MIT License
 #
 # Copyright (c) 2021 Albert Moky
@@ -24,133 +24,133 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-import asyncio
-from abc import ABC, abstractmethod
+from abc import abstractmethod
+from enum import IntEnum
+from typing import Optional, Union
+
+from ..types import SocketAddress
+from ..skywalker import Processor
+from ..net import ConnectionState
+from ..net.state import StateOrder
+
+from .ship import Departure
+
+
+class DockerStatus(IntEnum):
+    """ Docker Status """
+    ERROR = -1
+    INIT = 0
+    PREPARING = 1
+    READY = 2
+
+
+READY_STATUS = [
+    StateOrder.READY,
+    StateOrder.EXPIRED,
+    StateOrder.MAINTAINING
+]
+
+
+def status_from_state(state: Optional[ConnectionState]) -> DockerStatus:
+    """ Convert connection state to docker status """
+    if state is None:
+        return DockerStatus.ERROR
+    index = state.index
+    if index in READY_STATUS:
+        return DockerStatus.READY
+    if index == StateOrder.PREPARING:
+        return DockerStatus.PREPARING
+    if index == StateOrder.ERROR:
+        return DockerStatus.ERROR
+    return DockerStatus.INIT
 
 
-class Processor(ABC):
+class Docker(Processor):
+    """
+        Star Worker
+        ~~~~~~~~~~~
 
-    @abstractmethod
-    async def process(self) -> bool:
-        """
-        Do the job
+        Processor for Star Ships
+    """
 
-        :return: False on nothing to do
-        """
+    @property
+    @abstractmethod
+    def closed(self) -> bool:
+        """ Connection closed """
         raise NotImplemented
 
-
-class Handler(ABC):
-
+    @property
     @abstractmethod
-    async def setup(self):
-        """ Prepare for Handling """
+    def alive(self) -> bool:
+        """ Connection alive """
         raise NotImplemented
-    
+
+    @property
     @abstractmethod
-    async def handle(self):
-        """ Handling run loop """
+    def status(self) -> DockerStatus:
+        """ Connection state """
         raise NotImplemented
 
+    @property
     @abstractmethod
-    async def finish(self):
-        """ Cleanup after handled """
+    def remote_address(self) -> SocketAddress:
+        """ Remote address of connection """
         raise NotImplemented
 
-
-class Runnable(ABC):
-
+    @property
     @abstractmethod
-    async def run(self):
-        """ Run in an async task """
+    def local_address(self) -> Optional[SocketAddress]:
+        """ Local address of connection """
         raise NotImplemented
 
+    @abstractmethod
+    async def send_data(self, payload: Union[bytes, bytearray]) -> bool:
+        """
+        Pack data to an outgo ship (with normal priority), and
+        append to the waiting queue for sending out
 
-# noinspection PyAbstractClass
-class Runner(Runnable, Handler, Processor, ABC):
-    """
-        Runner
-        ~~~~~~
+        :param payload: data to be sent
+        :return: False on error
+        """
+        raise NotImplemented
 
-        @abstract methods:
-            - setup()
-            - finish()
-            - process()
-    """
+    @abstractmethod
+    async def send_ship(self, ship: Departure) -> bool:
+        """
+        Append outgo ship (carrying data package, with priority)
+        to the waiting queue for sending out
 
-    # Frames Per Second
-    # ~~~~~~~~~~~~~~~~~
-    # (1) The human eye can process 10-12 still images per second,
-    #     and the dynamic compensation function can also deceive us.
-    # (2) At a frame rate of 12fps or lower, we can quickly distinguish between
-    #     a pile of still images and not animations.
-    # (3) Once the playback rate (frames per second) of the images reaches 16-24 fps,
-    #     our brain will assume that these images are a continuously moving scene
-    #     and will appear like the effect of a movie.
-    # (4) At 24fps, there is a feeling of 'motion blur',
-    #     while at 60fps, the image is the smoothest and cleanest.
-    INTERVAL_SLOW = 1.0/10
-    INTERVAL_NORMAL = 1.0/25
-    INTERVAL_FAST = 1.0/60
-
-    def __init__(self, interval: float):
-        super().__init__()
-        assert interval > 0, 'interval error: %s' % interval
-        self.__interval = interval
-        self.__running = False
+        :param ship: outgo ship carrying data package/fragment
+        :return: False on duplicated
+        """
+        raise NotImplemented
 
-    @property
-    def interval(self) -> float:
-        return self.__interval
+    @abstractmethod
+    async def process_received(self, data: bytes):
+        """
+        Called when received data
 
-    @property
-    def running(self) -> bool:
-        return self.__running
+        :param data: received data package
+        """
+        raise NotImplemented
 
-    async def start(self):
-        self.__running = True
+    @abstractmethod
+    async def heartbeat(self):
+        """
+        Send 'PING' for keeping connection alive
+        """
+        raise NotImplemented
 
-    async def stop(self):
-        self.__running = False
+    @abstractmethod
+    def purge(self, now: float) -> int:
+        """ Clear all expired tasks """
+        raise NotImplemented
 
-    # Override
-    async def run(self):
-        await self.setup()
-        try:
-            await self.handle()
-        finally:
-            await self.finish()
-
-    # Override
-    async def handle(self):
-        while self.running:
-            if await self.process():
-                # runner is busy, return True to go on.
-                pass
-            else:
-                # if nothing to do now, return False here
-                # to let the thread have a rest.
-                await self._idle()
-
-    # protected
-    async def _idle(self):
-        await self.sleep(seconds=self.interval)
-        # time.sleep(self.interval)
-
-    @classmethod
-    async def sleep(cls, seconds: float):
-        await asyncio.sleep(seconds)
-
-    @classmethod
-    def sync_run(cls, main):
-        """ Run main coroutine until complete """
-        asyncio.run(main)
-
-    @classmethod
-    def async_run(cls, coroutine) -> asyncio.Task:
-        """ Create an async task to run the coroutine """
-        return asyncio.create_task(coroutine)
+    @abstractmethod
+    async def close(self):
+        """ Close connection for this docker """
+        raise NotImplemented
```

### Comparing `startrek-2.0.0/startrek/fsm/ticker.py` & `startrek-2.1.0/startrek/skywalker/ticker.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 import time
 import traceback
 from weakref import WeakSet
 from abc import ABC, abstractmethod
 from typing import Set
 
 from .runner import Runner
-from .daemon import DaemonRunner
 
 
 class Ticker(ABC):
 
     @abstractmethod
     async def tick(self, now: float, elapsed: float):
         """
@@ -48,31 +47,35 @@
 
         :param now:     current time (seconds from Jan 1, 1970 UTC)
         :param elapsed: seconds from previous tick
         """
         raise NotImplemented
 
 
-class Metronome(DaemonRunner):
+class Metronome(Runner):
 
     # at least wait 1/60 of a second
     MIN_INTERVAL = 1.0/60
 
     def __init__(self, interval: float):
         super().__init__(interval=interval)
-        self.__last_time = 0
+        self.__last_time = 0  # last process time
         self.__lock = threading.Lock()
         self.__tickers = WeakSet()
 
     # Override
     async def setup(self):
-        await super().setup()
+        # update process time
         self.__last_time = time.time()
 
     # Override
+    async def finish(self):
+        pass
+
+    # Override
     async def process(self) -> bool:
         tickers = self.tickers
         if len(tickers) == 0:
             # nothing to do now,
             # return False to have a rest ^_^
             return False
         # 1. check time
@@ -136,15 +139,15 @@
 
 @Singleton
 class PrimeMetronome:
 
     def __init__(self):
         super().__init__()
         metronome = Metronome(interval=Runner.INTERVAL_SLOW)
-        Runner.async_run(coroutine=metronome.start())
+        Runner.thread_run(runner=metronome)
         self.__metronome = metronome
 
     def add_ticker(self, ticker: Ticker):
         self.__metronome.add_ticker(ticker=ticker)
 
     def remove_ticker(self, ticker: Ticker):
         self.__metronome.remove_ticker(ticker=ticker)
```

### Comparing `startrek-2.0.0/startrek/net/__init__.py` & `startrek-2.1.0/startrek/net/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,22 +56,22 @@
           ~ ~ ~ ~ ~ ~ ~ ~:~ ~ ~ ~ ~ ~ ~ ~:~ ~ ~ ~ ~ ~ ~ ~:~ ~ ~ ~ ~ ~ ~
                          :               :               :
                          V               V               V
                     Remote Peer     Remote Peer     Remote Peer
 """
 
 from .hub import Hub
-from .channel import Channel
+from .channel import Channel, ChannelState
 from .connection import Connection
-from .delegate import ConnectionDelegate
 from .state import ConnectionState
+from .delegate import ConnectionDelegate
 
 __all__ = [
 
     'Hub',
 
-    'Channel',
+    'Channel', 'ChannelState',
 
-    'Connection',
+    'Connection', 'ConnectionState',
     'ConnectionDelegate',
-    'ConnectionState',
+
 ]
```

### Comparing `startrek-2.0.0/startrek/net/connection.py` & `startrek-2.1.0/startrek/net/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # SOFTWARE.
 # ==============================================================================
 
 from abc import ABC, abstractmethod
 from typing import Optional
 
 from ..types import SocketAddress
-from ..fsm import Ticker
+from ..skywalker import Ticker
 
 
 class Connection(Ticker, ABC):
 
     #
     #   Flags
     #
```

### Comparing `startrek-2.0.0/startrek/net/delegate.py` & `startrek-2.1.0/startrek/net/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/net/hub.py` & `startrek-2.1.0/startrek/net/hub.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 # ==============================================================================
 
 import socket
 from abc import ABC, abstractmethod
 from typing import Optional, Iterable
 
 from ..types import SocketAddress
-from ..fsm import Processor
+from ..skywalker import Processor
 
-from .channel import is_closed
+from .socket import socket_disconnect
 from .channel import Channel
 from .connection import Connection
 
 
 class Hub(Processor, ABC):
     """ Connections & Channels Container """
 
@@ -104,10 +104,10 @@
         sock = None
         try:
             sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             remote = ('8.8.8.8', 8888)
             sock.connect(remote)
             ip = sock.getsockname()[0]
         finally:
-            if not (sock is None or is_closed(sock=sock)):
-                sock.close()
+            if sock is not None:
+                socket_disconnect(sock=sock)
         return ip
```

### Comparing `startrek-2.0.0/startrek/net/state.py` & `startrek-2.1.0/startrek/net/state.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/port/__init__.py` & `startrek-2.1.0/startrek/port/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/port/delegate.py` & `startrek-2.1.0/startrek/port/delegate.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/port/docker.py` & `startrek-2.1.0/startrek/port/ship.py`

 * *Files 26% similar despite different names*

```diff
@@ -24,133 +24,133 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from enum import IntEnum
-from typing import Optional, Union
+from typing import Any, List
 
-from ..types import SocketAddress
-from ..fsm import Processor
-from ..net import ConnectionState
-from ..net.state import StateOrder
-
-from .ship import Departure
-
-
-class DockerStatus(IntEnum):
-    """ Docker Status """
-    ERROR = -1
-    INIT = 0
-    PREPARING = 1
-    READY = 2
-
-
-READY_STATUS = [
-    StateOrder.READY,
-    StateOrder.EXPIRED,
-    StateOrder.MAINTAINING
-]
-
-
-def status_from_state(state: Optional[ConnectionState]) -> DockerStatus:
-    """ Convert connection state to docker status """
-    if state is None:
-        return DockerStatus.ERROR
-    index = state.index
-    if index in READY_STATUS:
-        return DockerStatus.READY
-    if index == StateOrder.PREPARING:
-        return DockerStatus.PREPARING
-    if index == StateOrder.ERROR:
-        return DockerStatus.ERROR
-    return DockerStatus.INIT
-
-
-class Docker(Processor):
-    """
-        Star Worker
-        ~~~~~~~~~~~
+"""
+    Star Ship
+    ~~~~~~~~~
+    
+    Container carrying data package
+"""
+
+
+class DeparturePriority(IntEnum):
+    """ Departure Ship Priority """
+
+    URGENT = -1
+    NORMAL = 0
+    SLOWER = 1
+
+
+class ShipStatus(IntEnum):
+    """ Ship Status """
+    #
+    #  Departure Status
+    #
+    NEW = 0x00      # not try yet
+    WAITING = 0x01  # sent, waiting for responses
+    TIMEOUT = 0x02  # waiting to send again
+    DONE = 0x03     # all fragments responded (or no need respond)
+    FAILED = 0x04   # tried 3 times and missed response(s)
+    #
+    #  Arrival Status
+    #
+    ASSEMBLING = 0x10  # waiting for more fragments
+    EXPIRED = 0x11     # failed to received all fragments
 
-        Processor for Star Ships
-    """
 
-    @property
-    @abstractmethod
-    def closed(self) -> bool:
-        """ Connection closed """
-        raise NotImplemented
+class Ship(ABC):
 
     @property
     @abstractmethod
-    def alive(self) -> bool:
-        """ Connection alive """
-        raise NotImplemented
+    def sn(self) -> Any:
+        """
+        Get ID for this ship
 
-    @property
-    @abstractmethod
-    def status(self) -> DockerStatus:
-        """ Connection state """
+        :return: SN
+        """
         raise NotImplemented
 
-    @property
     @abstractmethod
-    def remote_address(self) -> SocketAddress:
-        """ Remote address of connection """
-        raise NotImplemented
+    def touch(self, now: float):
+        """
+        Update expired time
 
-    @property
-    @abstractmethod
-    def local_address(self) -> Optional[SocketAddress]:
-        """ Local address of connection """
+        :param now: current time
+        """
         raise NotImplemented
 
     @abstractmethod
-    async def send_data(self, payload: Union[bytes, bytearray]) -> bool:
+    def get_status(self, now: float) -> ShipStatus:
         """
-        Pack data to an outgo ship (with normal priority), and
-        append to the waiting queue for sending out
+        Check ship state
 
-        :param payload: data to be sent
-        :return: False on error
+        :param now: current time
+        :return: current status
         """
         raise NotImplemented
 
+
+class Arrival(Ship):
+    """ Incoming Ship """
+
     @abstractmethod
-    async def send_ship(self, ship: Departure) -> bool:
+    def assemble(self, ship):  # -> Optional[Arrival]:
         """
-        Append outgo ship (carrying data package, with priority)
-        to the waiting queue for sending out
+        Data package can be sent as separated batches
 
-        :param ship: outgo ship carrying data package/fragment
-        :return: False on duplicated
+        :param ship: arrival ship carrying with data package/fragment
+        :return new ship carrying the whole data package
         """
         raise NotImplemented
 
+
+class Departure(Ship):
+    """ Outgoing Ship """
+
+    @property
+    @abstractmethod
+    def priority(self) -> int:
+        """ Task priority, default is 0, smaller is faster """
+        raise NotImplemented
+
+    @property
     @abstractmethod
-    async def process_received(self, data: bytes):
+    def fragments(self) -> List[bytes]:
         """
-        Called when received data
+        Get fragments to sent
 
-        :param data: received data package
+        :return remaining (separated) data package
         """
         raise NotImplemented
 
     @abstractmethod
-    async def heartbeat(self):
+    def check_response(self, ship: Arrival) -> bool:
         """
-        Send 'PING' for keeping connection alive
+        The received ship may carried a response for the departure
+        if all fragments responded, means this task is finished.
+
+        :param ship: income ship carrying response
+        :return True on task finished
         """
         raise NotImplemented
 
-    @abstractmethod
-    def purge(self, now: float) -> int:
-        """ Clear all expired tasks """
-        raise NotImplemented
+    #
+    #   task states
+    #
 
+    @property
     @abstractmethod
-    async def close(self):
-        """ Close connection for this docker """
+    def is_important(self) -> bool:
+        """
+        Whether needs to wait for responses
+
+        :return false for disposable
+        """
         raise NotImplemented
```

### Comparing `startrek-2.0.0/startrek/port/gate.py` & `startrek-2.1.0/startrek/port/gate.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # SOFTWARE.
 # ==============================================================================
 
 from abc import ABC, abstractmethod
 from typing import Optional, Union
 
 from ..types import SocketAddress
-from ..fsm import Processor
+from ..skywalker import Processor
 
 from .ship import Departure
 
 
 class Gate(Processor, ABC):
     """
         Star Gate
```

### Comparing `startrek-2.0.0/startrek/socket/__init__.py` & `startrek-2.1.0/startrek/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/socket/active_conn.py` & `startrek-2.1.0/startrek/socket/active_conn.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,27 +29,26 @@
 # ==============================================================================
 
 import time
 import weakref
 from typing import Optional
 
 from ..types import SocketAddress
-from ..fsm import Runnable, Runner, Daemon
+from ..skywalker import Runnable, Runner
 from ..net import Hub
 
 from .base_conn import BaseConnection
 
 
 class ActiveConnection(BaseConnection, Runnable):
     """ Active connection for client """
 
     def __init__(self, remote: SocketAddress, local: Optional[SocketAddress]):
         super().__init__(remote=remote, local=local)
         self.__hub_ref = None
-        self.__daemon = Daemon(target=self)
 
     @property  # protected
     def hub(self) -> Optional[Hub]:
         ref = self.__hub_ref
         if ref is not None:
             return ref()
 
@@ -59,24 +58,26 @@
 
     # Override
     async def start(self, hub: Hub):
         self.__hub_ref = weakref.ref(hub)
         # 1. start state machine
         await self._start_machine()
         # 2. start an async task to check channel
-        self.__daemon.start()
+        Runner.async_run(coroutine=self.run())
         # await self.run()
 
     # Override
     async def run(self):
         expired = 0
         last_time = 0
         interval = 8
-        while not self.closed:
+        while True:
             await Runner.sleep(seconds=1.0)
+            if self.closed:
+                break
             now = time.time()
             try:
                 sock = self.channel
                 if sock is None or sock.closed:
                     # first time to try connecting (last_time == 0)?
                     # or connection lost, then try to reconnect again.
                     # check time interval for the trying here
```

### Comparing `startrek-2.0.0/startrek/socket/base_channel.py` & `startrek-2.1.0/startrek/socket/base_channel.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 # ==============================================================================
 
-import select
 import socket
 import weakref
 from abc import ABC, abstractmethod
 from typing import Optional, Tuple
 
 from ..types import SocketAddress, AddressPairObject
 
-from ..net.channel import is_blocking, is_closed, is_connected, is_bound
-from ..net.channel import bind_socket, connect_socket, disconnect_socket
-from ..net.channel import ChannelState
-from ..net import Channel
+from ..net.socket import is_blocking, is_closed, is_connected, is_bound
+from ..net.socket import is_available, is_vacant
+from ..net.socket import socket_bind, socket_connect, socket_disconnect
+from ..net.socket import socket_send, socket_receive
+from ..net import Channel, ChannelState
 
 
 class SocketReader(ABC):
 
     @abstractmethod
     async def read(self, max_len: int) -> Optional[bytes]:
         """ read data from socket """
@@ -93,45 +93,57 @@
 
     @property
     def sock(self) -> Optional[socket.socket]:
         channel = self.channel
         if isinstance(channel, BaseChannel):
             return channel.sock
 
+    # noinspection PyMethodMayBeStatic
+    async def _socket_receive(self, sock: socket.socket, max_len: int) -> Optional[bytes]:
+        # TODO: override for async receiving
+        # return sock.recv(max_len)
+        return socket_receive(sock=sock, max_len=max_len)
+
+    # noinspection PyMethodMayBeStatic
+    async def _socket_send(self, sock: socket.socket, data: bytes) -> int:
+        # TODO: override for async sending
+        # return sock.send(data)
+        # return sock.sendall(data)
+        return socket_send(sock=sock, data=data)
+
 
 # noinspection PyAbstractClass
 class ChannelReader(Controller, SocketReader, ABC):
 
     # Override
     async def read(self, max_len: int) -> Optional[bytes]:
         sock = self.sock
         if sock is None or is_closed(sock=sock):
             raise ConnectionError('socket closed')
         else:
-            return sock.recv(max_len)
+            return await self._socket_receive(sock=sock, max_len=max_len)
 
     # @abstractmethod  # Override
     # async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
     #     """ receive data via socket, and return it with remote address """
     #     raise NotImplemented
 
 
 # noinspection PyAbstractClass
 class ChannelWriter(Controller, SocketWriter, ABC):
 
     # Override
     async def write(self, data: bytes) -> int:
         """ Return the number of bytes sent;
             this may be less than len(data) if the network is busy. """
-        # sent = sock.sendall(data)
         sock = self.sock
         if sock is None or is_closed(sock=sock):
             raise ConnectionError('socket closed')
         else:
-            return sock.send(data)
+            return await self._socket_send(sock=sock, data=data)
 
     # @abstractmethod  # Override
     # async def send(self, data: bytes, target: SocketAddress) -> int:
     #     """ send data via socket with remote address """
     #     raise NotImplemented
 
 
@@ -185,15 +197,15 @@
             self.__sock = sock
             self.__closed = False
         else:
             self.__sock = None
             self.__closed = True
         # 2. close old socket
         if old is not None and old is not sock:
-            await disconnect_socket(sock=old)
+            await self._socket_disconnect(sock=old)
 
     #
     #   States
     #
 
     @property
     def state(self) -> ChannelState:
@@ -231,31 +243,37 @@
 
     @property  # Override
     def alive(self) -> bool:
         return (not self.closed) and (self.connected or self.bound)
 
     @property
     def available(self) -> bool:
-        if not self.alive:
-            return False
         sock = self.sock
-        if sock is None:
+        if sock is None or is_closed(sock=sock):
             return False
-        ready, _, _ = select.select([sock], [], [], 0)
-        return sock in ready
+        elif is_bound(sock=sock) or is_connected(sock=sock):
+            # alive, check reading buffer
+            return self._socket_available(sock=sock)
+
+    # noinspection PyMethodMayBeStatic
+    def _socket_available(self, sock: socket.socket) -> bool:
+        return is_available(sock=sock)
 
     @property
     def vacant(self) -> bool:
-        if not self.alive:
-            return False
         sock = self.sock
-        if sock is None:
+        if sock is None or is_closed(sock=sock):
             return False
-        _, ready, _ = select.select([], [sock], [], 0)
-        return sock in ready
+        elif is_bound(sock=sock) or is_connected(sock=sock):
+            # alive, check writing buffer
+            return self._socket_vacant(sock=sock)
+
+    # noinspection PyMethodMayBeStatic
+    def _socket_vacant(self, sock: socket.socket) -> bool:
+        return is_vacant(sock=sock)
 
     @property  # Override
     def blocking(self) -> bool:
         sock = self.sock
         return sock is not None and is_blocking(sock=sock)
 
     def __str__(self) -> str:
@@ -272,26 +290,41 @@
 
     # Override
     def configure_blocking(self, blocking: bool):
         sock = self.sock
         sock.setblocking(blocking)
         return sock
 
+    # noinspection PyMethodMayBeStatic
+    async def _socket_bind(self, sock: socket.socket, local: SocketAddress) -> bool:
+        # TODO: override for async binding
+        return socket_bind(sock=sock, local=local)
+
+    # noinspection PyMethodMayBeStatic
+    async def _socket_connect(self, sock: socket.socket, remote: SocketAddress) -> bool:
+        # TODO: override for async connecting
+        return socket_connect(sock=sock, remote=remote)
+
+    # noinspection PyMethodMayBeStatic
+    async def _socket_disconnect(self, sock: socket.socket) -> bool:
+        # TODO: override for async disconnecting
+        return socket_disconnect(sock=sock)
+
     # Override
     async def bind(self, address: Optional[SocketAddress] = None,
                    host: Optional[str] = '0.0.0.0', port: Optional[int] = 0):
         if address is None:
             if port > 0:
                 assert host is not None, 'host should not be empty'
                 address = (host, port)
             else:
                 address = self._local
                 assert address is not None, 'local address not set'
         sock = self.sock
-        ok = await bind_socket(sock=sock, local=address)
+        ok = await self._socket_bind(sock=sock, local=address)
         assert ok, 'failed to bind socket: %s' % str(address)
         self._local = address
         return sock
 
     # Override
     async def connect(self, address: Optional[SocketAddress] = None,
                       host: Optional[str] = '127.0.0.1', port: Optional[int] = 0) -> socket.socket:
@@ -299,24 +332,24 @@
             if port > 0:
                 assert host is not None, 'host should not be empty'
                 address = (host, port)
             else:
                 address = self._remote
                 assert address is not None, 'remote address not set'
         sock = self.sock
-        ok = await connect_socket(sock=sock, remote=address)
+        ok = await self._socket_connect(sock=sock, remote=address)
         assert ok, 'failed to connect socket: %s' % str(address)
         self._remote = address
         return sock
 
     # Override
     async def disconnect(self) -> Optional[socket.socket]:
         sock = self.__sock
         if sock is not None:
-            ok = await disconnect_socket(sock=sock)
+            ok = await self._socket_disconnect(sock=sock)
             assert ok, 'failed to disconnect socket: %s' % sock
         return sock
 
     # Override
     async def close(self):
         await self.set_socket(sock=None)
```

### Comparing `startrek-2.0.0/startrek/socket/base_conn.py` & `startrek-2.1.0/startrek/socket/base_conn.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/socket/base_hub.py` & `startrek-2.1.0/startrek/socket/base_hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,18 +31,21 @@
 import socket
 import threading
 import time
 import weakref
 from abc import ABC, abstractmethod
 from typing import Optional, Iterable
 
-from ..fsm import Runner
 from ..types import SocketAddress, AddressPairMap
-from ..net.channel import ChannelState
-from ..net import Hub, Channel, Connection, ConnectionDelegate
+from ..skywalker import Runner
+
+from ..net import Hub
+from ..net import Channel, ChannelState
+from ..net import Connection, ConnectionDelegate
+
 from .base_conn import BaseConnection
 
 
 class ConnectionPool(AddressPairMap[Connection]):
 
     # Override
     def set(self, item: Optional[Connection],
```

### Comparing `startrek-2.0.0/startrek/stardocker.py` & `startrek-2.1.0/startrek/stardocker.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/stargate.py` & `startrek-2.1.0/startrek/stargate.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 import socket
 import threading
 import time
 import weakref
 from abc import ABC, abstractmethod
 from typing import Optional, List, Iterable, Union
 
-from .fsm import Runner
 from .types import SocketAddress, AddressPairMap
+from .skywalker import Runner
+
 from .net import Connection, ConnectionDelegate, ConnectionState
 from .net.state import StateOrder
 from .port import Departure, Gate
 from .port import Docker, DockerStatus, DockerDelegate
 from .port.docker import status_from_state
+
 from .stardocker import StarDocker
 
 
 class DockerPool(AddressPairMap[Docker]):
 
     # Override
     def set(self, item: Optional[Docker],
```

### Comparing `startrek-2.0.0/startrek/types/__init__.py` & `startrek-2.1.0/startrek/types/__init__.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/types/mapping.py` & `startrek-2.1.0/startrek/types/mapping.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek/types/pair.py` & `startrek-2.1.0/startrek/types/pair.py`

 * *Files identical despite different names*

### Comparing `startrek-2.0.0/startrek.egg-info/SOURCES.txt` & `startrek-2.1.0/startrek.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 startrek.egg-info/PKG-INFO
 startrek.egg-info/SOURCES.txt
 startrek.egg-info/dependency_links.txt
 startrek.egg-info/top_level.txt
 startrek/fsm/__init__.py
 startrek/fsm/auto.py
 startrek/fsm/base.py
-startrek/fsm/daemon.py
 startrek/fsm/machine.py
-startrek/fsm/runner.py
-startrek/fsm/ticker.py
 startrek/net/__init__.py
 startrek/net/channel.py
 startrek/net/connection.py
 startrek/net/delegate.py
 startrek/net/hub.py
+startrek/net/socket.py
 startrek/net/state.py
 startrek/port/__init__.py
 startrek/port/delegate.py
 startrek/port/docker.py
 startrek/port/gate.py
 startrek/port/ship.py
+startrek/skywalker/__init__.py
+startrek/skywalker/daemon.py
+startrek/skywalker/runner.py
+startrek/skywalker/ticker.py
 startrek/socket/__init__.py
 startrek/socket/active_conn.py
 startrek/socket/base_channel.py
 startrek/socket/base_conn.py
 startrek/socket/base_hub.py
 startrek/types/__init__.py
 startrek/types/mapping.py
```

