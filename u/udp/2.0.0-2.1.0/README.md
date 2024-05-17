# Comparing `tmp/udp-2.0.0.tar.gz` & `tmp/udp-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/udp-2.0.0.tar", last modified: Fri May 10 15:33:25 2024, max compression
+gzip compressed data, was "dist/udp-2.1.0.tar", last modified: Fri May 17 17:29:27 2024, max compression
```

## Comparing `udp-2.0.0.tar` & `udp-2.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-10 15:33:25.000000 udp-2.0.0/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-2.0.0/README.md
--rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-10 15:33:25.000000 udp-2.0.0/setup.cfg
--rw-r--r--   0 moky       (501) staff       (20)      835 2024-05-10 15:32:29.000000 udp-2.0.0/setup.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp/
--rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-2.0.0/udp/__init__.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp/ba/
--rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-2.0.0/udp/ba/array.py
--rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/convert.py
--rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-2.0.0/udp/ba/data.py
--rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-2.0.0/udp/ba/helper.py
--rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/integer.py
--rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-2.0.0/udp/ba/mutable.py
--rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-2.0.0/udp/ba/utils.py
--rw-r--r--   0 moky       (501) staff       (20)     9489 2024-05-07 14:50:50.000000 udp-2.0.0/udp/channel.py
--rw-r--r--   0 moky       (501) staff       (20)     8265 2024-05-09 15:46:48.000000 udp-2.0.0/udp/hub.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp/mtp/
--rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-2.0.0/udp/mtp/__init__.py
--rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-2.0.0/udp/mtp/header.py
--rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-2.0.0/udp/mtp/package.py
--rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-2.0.0/udp/mtp/packer.py
--rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-2.0.0/udp/mtp/protocol.py
--rw-r--r--   0 moky       (501) staff       (20)    11702 2024-05-07 15:14:23.000000 udp-2.0.0/udp/startrek.py
-drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/
--rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/PKG-INFO
--rw-r--r--   0 moky       (501) staff       (20)      442 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/SOURCES.txt
--rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/dependency_links.txt
--rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/requires.txt
--rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-10 15:33:25.000000 udp-2.0.0/udp.egg-info/top_level.txt
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-17 17:29:27.000000 udp-2.1.0/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)       19 2020-07-17 14:54:20.000000 udp-2.1.0/README.md
+-rw-r--r--   0 moky       (501) staff       (20)       38 2024-05-17 17:29:27.000000 udp-2.1.0/setup.cfg
+-rw-r--r--   0 moky       (501) staff       (20)      835 2024-05-17 10:41:38.000000 udp-2.1.0/setup.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp/
+-rw-r--r--   0 moky       (501) staff       (20)     2832 2023-01-13 16:49:26.000000 udp-2.1.0/udp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     5490 2024-05-17 11:58:03.000000 udp-2.1.0/udp/aio.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp/ba/
+-rw-r--r--   0 moky       (501) staff       (20)     1944 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)     9574 2024-02-26 16:22:28.000000 udp-2.1.0/udp/ba/array.py
+-rw-r--r--   0 moky       (501) staff       (20)     3345 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/convert.py
+-rw-r--r--   0 moky       (501) staff       (20)     7763 2023-01-13 16:00:06.000000 udp-2.1.0/udp/ba/data.py
+-rw-r--r--   0 moky       (501) staff       (20)     7219 2023-01-13 15:58:57.000000 udp-2.1.0/udp/ba/helper.py
+-rw-r--r--   0 moky       (501) staff       (20)     8436 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/integer.py
+-rw-r--r--   0 moky       (501) staff       (20)     4852 2021-09-16 08:10:15.000000 udp-2.1.0/udp/ba/mutable.py
+-rw-r--r--   0 moky       (501) staff       (20)    15161 2023-01-13 16:00:39.000000 udp-2.1.0/udp/ba/utils.py
+-rw-r--r--   0 moky       (501) staff       (20)    12515 2024-05-17 11:57:45.000000 udp-2.1.0/udp/channel.py
+-rw-r--r--   0 moky       (501) staff       (20)     8271 2024-05-17 11:15:19.000000 udp-2.1.0/udp/hub.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp/mtp/
+-rw-r--r--   0 moky       (501) staff       (20)     1678 2021-09-16 08:10:15.000000 udp-2.1.0/udp/mtp/__init__.py
+-rw-r--r--   0 moky       (501) staff       (20)    15551 2023-01-02 14:11:01.000000 udp-2.1.0/udp/mtp/header.py
+-rw-r--r--   0 moky       (501) staff       (20)     4505 2023-01-02 14:11:01.000000 udp-2.1.0/udp/mtp/package.py
+-rw-r--r--   0 moky       (501) staff       (20)     8003 2023-01-02 14:11:01.000000 udp-2.1.0/udp/mtp/packer.py
+-rw-r--r--   0 moky       (501) staff       (20)     6708 2021-09-16 08:10:15.000000 udp-2.1.0/udp/mtp/protocol.py
+-rw-r--r--   0 moky       (501) staff       (20)    11702 2024-05-07 15:14:23.000000 udp-2.1.0/udp/startrek.py
+drwxr-xr-x   0 moky       (501) staff       (20)        0 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/
+-rw-r--r--   0 moky       (501) staff       (20)      438 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/PKG-INFO
+-rw-r--r--   0 moky       (501) staff       (20)      453 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/SOURCES.txt
+-rw-r--r--   0 moky       (501) staff       (20)        1 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/dependency_links.txt
+-rw-r--r--   0 moky       (501) staff       (20)       16 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/requires.txt
+-rw-r--r--   0 moky       (501) staff       (20)        4 2024-05-17 17:29:27.000000 udp-2.1.0/udp.egg-info/top_level.txt
```

### Comparing `udp-2.0.0/setup.py` & `udp-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     ~~~
 
     User Datagram Protocol
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

### Comparing `udp-2.0.0/udp/__init__.py` & `udp-2.1.0/udp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/__init__.py` & `udp-2.1.0/udp/ba/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/array.py` & `udp-2.1.0/udp/ba/array.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/convert.py` & `udp-2.1.0/udp/ba/convert.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/data.py` & `udp-2.1.0/udp/ba/data.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/helper.py` & `udp-2.1.0/udp/ba/helper.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/integer.py` & `udp-2.1.0/udp/ba/integer.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/mutable.py` & `udp-2.1.0/udp/ba/mutable.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/ba/utils.py` & `udp-2.1.0/udp/ba/utils.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/channel.py` & `udp-2.1.0/udp/channel.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,22 +28,26 @@
 # SOFTWARE.
 # ==============================================================================
 
 import socket
 from typing import Optional, Tuple
 
 from startrek.types import SocketAddress
-from startrek.net.channel import is_blocking, is_closed
 from startrek import BaseChannel, ChannelReader, ChannelWriter
 
+from .aio import is_blocking, is_closed, is_available
+from .aio import socket_send, socket_receive
+from .aio import socket_send_to, socket_receive_from
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
@@ -54,29 +58,29 @@
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
@@ -89,99 +93,152 @@
                 # print('[NET] socket error: remote peer reset socket %s' % sock)
                 return socket.error('remote peer reset socket %s' % sock)
 
 
 class PacketChannelReader(ChannelReader):
     """ Datagram Packet Channel Reader """
 
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
+    # noinspection PyMethodMayBeStatic
+    async def _socket_receive_from(self, sock: socket.socket, max_len: int
+                                   ) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+        if await is_closed(sock=sock):
+            raise ConnectionError('socket closed')
+        elif not await is_available(sock=sock):
+            # TODO: check 'broken pipe'
+            return None, None
+        else:
+            # return sock.recvfrom(max_len)
+            return await socket_receive_from(sock=sock, max_len=max_len)
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
 
     # noinspection PyMethodMayBeStatic
     async def _try_receive(self, max_len: int, sock: socket.socket) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
         try:
-            return sock.recvfrom(max_len)
+            # return sock.recvfrom(max_len)
+            return await self._socket_receive_from(sock=sock, max_len=max_len)
         except socket.error as error:
-            error = ChannelChecker.check_error(error=error, sock=sock)
+            error = await ChannelChecker.check_error(error=error, sock=sock)
             if error is None:
                 # received nothing
                 return None, None
             else:
                 # connection lost?
                 raise error
 
-    async def _receive_from(self, max_len: int, sock: socket.socket) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+    async def _receive_from(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
+        sock = self.sock
+        if sock is None:
+            raise ConnectionError('channel not ready')
         data, remote = await self._try_receive(max_len=max_len, sock=sock)
         # check data
-        error = ChannelChecker.check_data(data=data, sock=sock)
+        error = await ChannelChecker.check_data(data=data, sock=sock)
         if error is None:
             # OK
             return data, remote
         else:
             # connection lost!
             raise error
 
     # Override
     async def receive(self, max_len: int) -> Tuple[Optional[bytes], Optional[SocketAddress]]:
         remote = self.remote_address
         if remote is None:
             # not connect (UDP)
-            return await self._receive_from(max_len=max_len, sock=self.sock)
+            return await self._receive_from(max_len=max_len)
         else:
             # connected (TCP/UDP)
             return await self.read(max_len=max_len), remote
 
 
 class PacketChannelWriter(ChannelWriter):
     """ Datagram Packet Channel Writer """
 
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
+    # noinspection PyMethodMayBeStatic
+    async def _socket_send_to(self, sock: socket.socket, data: bytes, target: SocketAddress) -> int:
+        if await is_closed(sock=sock):
+            raise ConnectionError('socket closed')
+        # elif not await is_vacant(sock=sock):
+        #     # TODO: check 'broken pipe'
+        #     return -1
+        else:
+            # return sock.sendto(data, remote)
+            return await socket_send_to(sock=sock, data=data, target=target)
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
@@ -205,17 +262,18 @@
             return -1
         else:
             return 0
 
     # noinspection PyMethodMayBeStatic
     async def _try_send(self, data: bytes, target: SocketAddress, sock: socket.socket) -> int:
         try:
-            return sock.sendto(data, target)
+            # return sock.sendto(data, target)
+            return await self._socket_send_to(sock=sock, data=data, target=target)
         except socket.error as error:
-            error = ChannelChecker.check_error(error=error, sock=sock)
+            error = await ChannelChecker.check_error(error=error, sock=sock)
             if error is None:
                 # buffer overflow!
                 return -1
             else:
                 # connection lost?
                 raise error
 
@@ -240,7 +298,19 @@
     # Override
     def _create_reader(self):
         return PacketChannelReader(channel=self)
 
     # Override
     def _create_writer(self):
         return PacketChannelWriter(channel=self)
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

### Comparing `udp-2.0.0/udp/hub.py` & `udp-2.1.0/udp/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # ==============================================================================
 
 import socket
 from abc import ABC
 from typing import Optional, Iterable
 
 from startrek.types import SocketAddress, AddressPairMap
-from startrek.fsm import Runner
+from startrek.skywalker import Runner
 from startrek import Channel, BaseChannel
 from startrek import Connection, ConnectionDelegate
 from startrek import BaseConnection, ActiveConnection
 from startrek import BaseHub
 
 from .channel import PacketChannel
```

### Comparing `udp-2.0.0/udp/mtp/__init__.py` & `udp-2.1.0/udp/mtp/__init__.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/mtp/header.py` & `udp-2.1.0/udp/mtp/header.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/mtp/package.py` & `udp-2.1.0/udp/mtp/package.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/mtp/packer.py` & `udp-2.1.0/udp/mtp/packer.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/mtp/protocol.py` & `udp-2.1.0/udp/mtp/protocol.py`

 * *Files identical despite different names*

### Comparing `udp-2.0.0/udp/startrek.py` & `udp-2.1.0/udp/startrek.py`

 * *Files identical despite different names*

