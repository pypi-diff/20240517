# Comparing `tmp/tcp-2.0.0.tar.gz` & `tmp/tcp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tcp-2.0.0.tar", last modified: Fri May 10 15:31:18 2024, max compression
+gzip compressed data, was "dist/tcp-2.1.0.tar", last modified: Fri May 17 17:30:07 2024, max compression
```

## Comparing `tcp-2.0.0.tar` & `tcp-2.1.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:31:18.000000 tcp-2.0.0/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-10 15:31:18.000000 tcp-2.0.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-2.0.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:31:18.000000 tcp-2.0.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      849 2024-05-10 15:30:49.000000 tcp-2.0.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp/
--rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-2.0.0/tcp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     7631 2024-05-07 09:35:54.000000 tcp-2.0.0/tcp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)    10581 2024-05-09 18:52:45.000000 tcp-2.0.0/tcp/hub.py
--rw-r--r--   0 moky       (501) staff       (20)     4519 2024-05-07 14:35:33.000000 tcp-2.0.0/tcp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      210 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-10 15:31:18.000000 tcp-2.0.0/tcp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:30:07.000000 tcp-2.1.0/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-17 17:30:07.000000 tcp-2.1.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 tcp-2.1.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 17:30:07.000000 tcp-2.1.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      849 2024-05-17 03:47:56.000000 tcp-2.1.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp/
+-rw-r--r--   0 moky       (501) staff       (20)     2828 2023-01-13 12:35:58.000000 tcp-2.1.0/tcp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     4945 2024-05-17 11:53:44.000000 tcp-2.1.0/tcp/aio.py
+-rw-r--r--   0 moky       (501) staff       (20)     9327 2024-05-17 11:55:01.000000 tcp-2.1.0/tcp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)    10842 2024-05-17 09:40:31.000000 tcp-2.1.0/tcp/hub.py
+-rw-r--r--   0 moky       (501) staff       (20)     4519 2024-05-07 14:35:33.000000 tcp-2.1.0/tcp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      445 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      221 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-17 17:30:07.000000 tcp-2.1.0/tcp.egg-info/top_level.txt
```

### Comparing `tcp-2.0.0/setup.py` & `tcp-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     Transmission Control Protocol
 """
 
 from setuptools import setup, find_packages
 
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 __author__ = 'Albert Moky'
 __contact__ = 'albert.moky@gmail.com'
 
 with open('README.md', 'r') as fh:
     readme = fh.read()
 
 setup(
@@ -30,10 +30,10 @@
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     install_requires=[
-        'startrek>=2.0.0'
+        'startrek>=2.1.0'
     ]
 )
```

### Comparing `tcp-2.0.0/tcp/__init__.py` & `tcp-2.1.0/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `tcp-2.0.0/tcp/channel.py` & `tcp-2.1.0/tcp/channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,22 +28,25 @@
 # SOFTWARE.
 # ==============================================================================
 
 import socket
 from typing import Optional, Tuple
 
 from startrek.types import SocketAddress
-from startrek.net.channel import is_blocking, is_closed
 from startrek import BaseChannel, ChannelReader, ChannelWriter
 
+from .aio import is_blocking, is_closed, is_available
+from .aio import socket_send, socket_receive
+from .aio import socket_bind, socket_connect, socket_disconnect
+
 
 class ChannelChecker:
 
     @classmethod
-    def check_error(cls, error: socket.error, sock: socket.socket) -> Optional[socket.error]:
+    async def check_error(cls, error: socket.error, sock: socket.socket) -> Optional[socket.error]:
         """
             Check socket error
 
                (1) check E_AGAIN
                    the socket will raise 'Resource temporarily unavailable'
                    when received nothing in non-blocking mode,
                    or buffer overflow while sending too many bytes,
@@ -54,29 +57,29 @@
                    here we should ignore this exception
         """
         # the socket will raise 'Resource temporarily unavailable'
         # when received nothing in non-blocking mode,
         # or buffer overflow while sending too many bytes,
         # here we should ignore this exception.
         if error.errno == socket.EAGAIN:  # error.strerror == 'Resource temporarily unavailable':
-            if not is_blocking(sock=sock):
+            if not await is_blocking(sock=sock):
                 # ignore it
                 return None
         # in blocking mode, the socket wil wait until sent/received data,
         # but if timeout was set, it will raise 'timeout' error on timeout,
         # here we should ignore this exception.
         if isinstance(error, socket.timeout):
             if sock.gettimeout() is not None:  # or not self.blocking:
                 # ignore it
                 return None
         # print('[NET] socket error: %s' % error)
         return error
 
     @classmethod
-    def check_data(cls, data: Optional[bytes], sock: socket.socket) -> Optional[socket.error]:
+    async def check_data(cls, data: Optional[bytes], sock: socket.socket) -> Optional[socket.error]:
         """
             Check data received from socket
 
             (1) check timeout
                 in blocking mode, the socket will wait until received something,
                 but if timeout was set, it will return nothing too, it's normal;
                 otherwise, we know the connection was lost.
@@ -88,36 +91,49 @@
             if sock.gettimeout() is None:  # and self.blocking:
                 # print('[NET] socket error: remote peer reset socket %s' % sock)
                 return socket.error('remote peer reset socket %s' % sock)
 
 
 class StreamChannelReader(ChannelReader):
 
+    # Override
+    async def _socket_receive(self, sock: socket.socket, max_len: int) -> Optional[bytes]:
+        if await is_closed(sock=sock):
+            raise ConnectionError('socket closed')
+        elif not await is_available(sock=sock):
+            # TODO: check 'broken pipe'
+            return None
+        elif await is_blocking(sock=sock):
+            return await super()._socket_receive(sock=sock, max_len=max_len)
+        else:
+            return await socket_receive(sock=sock, max_len=max_len)
+
     # noinspection PyMethodMayBeStatic
     async def _try_read(self, max_len: int, sock: socket.socket) -> Optional[bytes]:
         try:
-            return sock.recv(max_len)
+            # return sock.recv(max_len)
+            return await self._socket_receive(sock=sock, max_len=max_len)
         except socket.error as error:
-            error = ChannelChecker.check_error(error=error, sock=sock)
+            error = await ChannelChecker.check_error(error=error, sock=sock)
             if error is None:
                 # received nothing
                 return None
             else:
                 # connection lost?
                 raise error
 
     # Override
     async def read(self, max_len: int) -> Optional[bytes]:
         sock = self.sock
-        if sock is None or is_closed(sock=sock):
-            raise ConnectionError('socket closed')
+        if sock is None:
+            raise ConnectionError('channel not ready')
         # 1. try to read data
         data = await self._try_read(max_len=max_len, sock=sock)
         # 2. check data
-        error = ChannelChecker.check_data(data=data, sock=sock)
+        error = await ChannelChecker.check_data(data=data, sock=sock)
         if error is not None:
             # connection lost!
             raise error
         # OK
         return data
 
     # Override
@@ -127,33 +143,46 @@
             return None, None
         else:
             return data, self.remote_address
 
 
 class StreamChannelWriter(ChannelWriter):
 
+    # Override
+    async def _socket_send(self, sock: socket.socket, data: bytes) -> int:
+        if await is_closed(sock=sock):
+            raise ConnectionError('socket closed')
+        # elif not await is_vacant(sock=sock):
+        #     # TODO: check 'broken pipe'
+        #     return -1
+        elif await is_blocking(sock=sock):
+            return await super()._socket_send(sock=sock, data=data)
+        else:
+            return await socket_send(sock=sock, data=data)
+
     # noinspection PyMethodMayBeStatic
     async def _try_write(self, data: bytes, sock: socket.socket) -> int:
         try:
-            return sock.send(data)
+            # return sock.send(data)
+            return await self._socket_send(sock=sock, data=data)
         except socket.error as error:
-            error = ChannelChecker.check_error(error=error, sock=sock)
+            error = await ChannelChecker.check_error(error=error, sock=sock)
             if error is not None:
                 # connection lost?
                 raise error
             # buffer overflow!
             return 0
 
     # Override
     async def write(self, data: bytes) -> int:
         """ Return the number of bytes sent;
             this may be less than len(data) if the network is busy. """
         sock = self.sock
-        if sock is None or is_closed(sock=sock):
-            raise ConnectionError('socket closed')
+        if sock is None:
+            raise ConnectionError('channel not ready')
         # sent = sock.sendall(data)
         sent = 0
         rest = len(data)
         # assert rest > 0, 'cannot send empty data'
         while True:  # while is_opened(sock=sock):
             cnt = await self._try_write(data=data, sock=sock)
             # check send result
@@ -193,7 +222,19 @@
     # Override
     def _create_reader(self):
         return StreamChannelReader(channel=self)
 
     # Override
     def _create_writer(self):
         return StreamChannelWriter(channel=self)
+
+    # Override
+    async def _socket_bind(self, sock: socket.socket, local: SocketAddress) -> bool:
+        return await socket_bind(sock=sock, local=local)
+
+    # Override
+    async def _socket_connect(self, sock: socket.socket, remote: SocketAddress) -> bool:
+        return await socket_connect(sock=sock, remote=remote)
+
+    # Override
+    async def _socket_disconnect(self, sock: socket.socket) -> bool:
+        return await socket_disconnect(sock=sock)
```

### Comparing `tcp-2.0.0/tcp/hub.py` & `tcp-2.1.0/tcp/hub.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,21 @@
 import socket
 import threading
 import time
 from abc import ABC
 from typing import Optional, Iterable
 
 from startrek.types import SocketAddress, AddressPairMap
-from startrek.fsm import Runnable, Runner, Daemon
+from startrek.skywalker import Runnable, Runner, Daemon
 from startrek import Channel, BaseChannel
 from startrek import Connection, ConnectionDelegate
 from startrek import BaseConnection, ActiveConnection
 from startrek import BaseHub
 
+from .aio import is_blocking
 from .channel import StreamChannel
 
 
 class ChannelPool(AddressPairMap[Channel]):
 
     # Override
     def set(self, item: Optional[Channel],
@@ -183,31 +184,35 @@
         # 3. cancel the async task
         self.__daemon.stop()
 
     # Override
     async def run(self):
         self.__running = True
         while self.running:
+            master = self._get_master()
             try:
-                master = self._get_master()
                 sock, address = master.accept()
                 if sock is None:
                     await Runner.sleep(seconds=Runner.INTERVAL_NORMAL)
                 else:
                     await self._accept(remote=address, local=self.local_address, sock=sock)
             except socket.error as error:
+                if error.errno == socket.EAGAIN:  # error.strerror == 'Resource temporarily unavailable':
+                    if not await is_blocking(sock=master):
+                        continue
                 print('[TCP] socket error: %s' % error)
             except Exception as error:
                 print('[TCP] accept error: %s' % error)
 
     async def _accept(self, remote: SocketAddress, local: SocketAddress, sock: socket.socket):
         # override for user-customized channel
         channel = self._create_channel(remote=remote, local=local)
         assert isinstance(channel, BaseChannel), 'channel error: %s, %s' % (remote, channel)
         # set socket for this channel
+        sock.setblocking(False)
         await channel.set_socket(sock=sock)
         self._set_channel(channel=channel, remote=channel.remote_address, local=channel.local_address)
 
     # Override
     async def open(self, remote: Optional[SocketAddress], local: Optional[SocketAddress]) -> Optional[Channel]:
         assert remote is not None, 'remote address empty: %s, %s' % (remote, local)
         return self._get_channel(remote=remote, local=local)
```

### Comparing `tcp-2.0.0/tcp/startrek.py` & `tcp-2.1.0/tcp/startrek.py`

 * *Files identical despite different names*

