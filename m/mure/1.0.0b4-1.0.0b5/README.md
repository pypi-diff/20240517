# Comparing `tmp/mure-1.0.0b4.tar.gz` & `tmp/mure-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mure-1.0.0b4.tar", max compression
+gzip compressed data, was "mure-1.0.0b5.tar", max compression
```

## Comparing `mure-1.0.0b4.tar` & `mure-1.0.0b5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11345 2024-04-25 14:48:40.624935 mure-1.0.0b4/LICENSE
--rw-r--r--   0        0        0     5557 2024-04-25 14:48:40.624935 mure-1.0.0b4/README.md
--rw-r--r--   0        0        0      212 2024-04-25 14:48:40.624935 mure-1.0.0b4/mure/__init__.py
--rw-r--r--   0        0        0     4264 2024-04-25 14:48:40.624935 mure-1.0.0b4/mure/cache.py
--rw-r--r--   0        0        0     4419 2024-04-25 14:48:40.624935 mure-1.0.0b4/mure/core.py
--rw-r--r--   0        0        0     8074 2024-04-25 14:48:40.624935 mure-1.0.0b4/mure/iterator.py
--rw-r--r--   0        0        0     4272 2024-04-25 14:48:40.624935 mure-1.0.0b4/mure/logging.py
--rw-r--r--   0        0        0     3463 2024-04-25 14:48:40.624935 mure-1.0.0b4/mure/models.py
--rw-r--r--   0        0        0     2794 2024-04-25 14:48:40.624935 mure-1.0.0b4/pyproject.toml
--rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 mure-1.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-07 14:49:16.533473 mure-1.0.0b5/LICENSE
+-rw-r--r--   0        0        0     5557 2024-05-07 14:49:16.533473 mure-1.0.0b5/README.md
+-rw-r--r--   0        0        0      212 2024-05-07 14:49:16.533473 mure-1.0.0b5/mure/__init__.py
+-rw-r--r--   0        0        0     3106 2024-05-07 14:49:16.533473 mure-1.0.0b5/mure/cache.py
+-rw-r--r--   0        0        0     4419 2024-05-07 14:49:16.533473 mure-1.0.0b5/mure/core.py
+-rw-r--r--   0        0        0     8772 2024-05-07 14:49:16.533473 mure-1.0.0b5/mure/iterator.py
+-rw-r--r--   0        0        0     4272 2024-05-07 14:49:16.533473 mure-1.0.0b5/mure/logging.py
+-rw-r--r--   0        0        0     3510 2024-05-07 14:49:16.533473 mure-1.0.0b5/mure/models.py
+-rw-r--r--   0        0        0     2794 2024-05-07 14:49:16.537473 mure-1.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 mure-1.0.0b5/PKG-INFO
```

### Comparing `mure-1.0.0b4/LICENSE` & `mure-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b4/README.md` & `mure-1.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b4/mure/cache.py` & `mure-1.0.0b5/mure/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -99,62 +99,22 @@
             Request to save to the cache.
         response : Response
             Response to save to the cache.
         """
         self._cache[request.id] = response
 
 
-class DiskCache(Cache):
+class DiskCache(MemoryCache):
     """Simple on-disk cache."""
 
     def __init__(self, path: Path = Path("mure-cache.shelve")):
+        super().__init__()
+
         self.path = path.resolve()
         if self.path.exists():
             LOGGER.warning(f"Cache ({self.path}) already exists")
 
         self._cache = shelve.open(str(self.path))
 
     def __del__(self):
         """Close the cache."""
         self._cache.close()
-
-    def has(self, request: Request) -> bool:
-        """Check if a request (and its corresponding response) is in the cache.
-
-        Parameters
-        ----------
-        request : Request
-            Request to check if it's in the cache.
-
-        Returns
-        -------
-        bool
-            True if the request is in the cache; otherwise, False.
-        """
-        return request.id in self._cache
-
-    def get(self, request: Request) -> Response | None:
-        """Get the response for the specified request from the cache.
-
-        Parameters
-        ----------
-        request : Request
-            Request to get response from the cache.
-
-        Returns
-        -------
-        Response | None
-            Response from the cache or None if the request is not in the cache.
-        """
-        return self._cache.get(request.id)
-
-    def set(self, request: Request, response: Response):
-        """Save a request and its response to the cache.
-
-        Parameters
-        ----------
-        request : Request
-            Request to save to the cache.
-        response : Response
-            Response to save to the cache.
-        """
-        self._cache[request.id] = response
```

### Comparing `mure-1.0.0b4/mure/core.py` & `mure-1.0.0b5/mure/core.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b4/mure/iterator.py` & `mure-1.0.0b5/mure/iterator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import os
-from asyncio import Event, PriorityQueue, Task
+from asyncio import Event, Lock, PriorityQueue, Task
 from collections.abc import AsyncGenerator, Iterator
 from typing import Self
 
 import chardet
 from aiohttp import ClientSession
 
 from mure.cache import Cache
@@ -39,15 +39,15 @@
         self.num_requests = len(requests)
         self.pending = len(requests)
         self.batch_size = batch_size
         self.cache = cache
 
         self._log_errors = bool(os.environ.get("MURE_LOG_ERRORS"))
         self._loop = asyncio.get_event_loop()
-        self._session = ClientSession()
+        self._lock = Lock()
         self._queue = PriorityQueue()
         self._events = [Event() for _ in requests]
         self._tasks: set[Task] = set()
         self._responses = self._fetch_responses()
         self._generator = None
 
     def __repr__(self) -> str:
@@ -86,26 +86,14 @@
         Returns
         -------
         Response
             Next response.
         """
         return next(self._responses)
 
-    def __del__(self):
-        """Close the generator gracefully."""
-        self._close()
-
-    def _close(self):
-        """Close the generator gracefully."""
-        if self._session:
-            self._loop.run_until_complete(self._session.close())
-
-        if self._generator:
-            self._loop.run_until_complete(self._generator.aclose())
-
     def _fetch_responses(self) -> Iterator[Response]:
         """Fetch responses concurrently.
 
         Yields
         ------
         Response
             One response at a time.
@@ -114,54 +102,71 @@
         self._generator = self._afetch_responses()
 
         # run the event loop until a response is available and yield it
         while True:
             try:
                 yield self._loop.run_until_complete(anext(self._generator))
             except StopAsyncIteration:
-                self._close()
+                self._generator = None
                 break
 
-    def _create_tasks(self) -> Iterator[Task]:
+    def _create_tasks(self, session: ClientSession) -> Iterator[Task]:
         """Create tasks for each resource.
 
+        Parameters
+        ----------
+        session : ClientSession
+            HTTP session to use.
+
         Yields
         ------
         Iterator[Task]
             Tasks to fetch resources.
         """
         for i, (request, event) in enumerate(zip(self.requests, self._events, strict=False)):
             # create task in the background
-            yield self._loop.create_task(self._aprocess_request(i, request, event))
+            yield self._loop.create_task(self._aprocess_request(session, i, request, event))
 
-    async def _aprocess_request(self, priority: int, request: Request, event: Event):
+    async def _aprocess_request(
+        self,
+        session: ClientSession,
+        priority: int,
+        request: Request,
+        event: Event,
+    ):
         """Process a request by fetching and putting it in the queue.
 
         Parameters
         ----------
+        session : ClientSession
+            HTTP session to use.
         priority : int
             Priority of the request.
         request. : Request
             Resource to request.
         event : Event
             Event to set when the response is ready.
         """
         LOGGER.debug(f"Started {priority}")
 
         # if cache is given and has response for the request, use it
         if self.cache and self.cache.has(request):
-            LOGGER.debug("Found response in cache")
-            response = self.cache.get(request)
+            LOGGER.debug(f"Found response {priority} in cache")
+            async with self._lock:
+                response = self.cache.get(request)
+            LOGGER.debug(f"Used response {priority} from cache")
         else:
-            response = await self._afetch(request)
+            response = await self._afetch(session, request)
 
             # save response to cache
             if self.cache:
-                self.cache.set(request, response)
-                LOGGER.debug("Saved response in cache")
+                LOGGER.debug(f"Saving response {priority} in cache")
+                async with self._lock:
+                    self.cache.set(request, response)
+                LOGGER.debug(f"Saved response {priority} in cache")
 
         # put response in the queue
         await self._queue.put((priority, response))
 
         # set event to notify that the response is ready
         event.set()
 
@@ -191,16 +196,19 @@
 
         Yields
         ------
         Response
             The server's response.
         """
         try:
+            # create session
+            session = ClientSession()
+
             # create tasks (lazy)
-            tasks = self._create_tasks()
+            tasks = self._create_tasks(session)
 
             # process first batch of tasks
             self._process_batch(tasks)
 
             for event in self._events:
                 # wait for the specific event to be set to preserve order of the requests
                 await event.wait()
@@ -215,30 +223,40 @@
                 self._process_batch(tasks)
 
                 yield response
                 self._queue.task_done()
                 self.pending -= 1
         except GeneratorExit:
             return
+        finally:
+            # close session
+            await session.close()
+
+            # we have to wait here for the session to close
+            # see: https://docs.aiohttp.org/en/stable/client_advanced.html#graceful-shutdown
+            # TODO remove this once aiohttp 4.0 is released, because this will contain a fix
+            await asyncio.sleep(0.25)
 
-    async def _afetch(self, request: Request) -> Response:
+    async def _afetch(self, session: ClientSession, request: Request) -> Response:
         """Perform a HTTP request.
 
         Parameters
         ----------
+        session : ClientSession
+            HTTP session to use.
         request : Resource
             Resource to request.
 
         Returns
         -------
         Response
             The server's response.
         """
         try:
-            async with self._session.request(
+            async with session.request(
                 request.method,
                 request.url,
                 headers=request.headers,
                 params=request.params,
                 data=request.data,
                 json=request.json,
                 timeout=request.timeout,
```

### Comparing `mure-1.0.0b4/mure/logging.py` & `mure-1.0.0b5/mure/logging.py`

 * *Files identical despite different names*

### Comparing `mure-1.0.0b4/mure/models.py` & `mure-1.0.0b5/mure/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import json
 from functools import cached_property
 from hashlib import blake2b
 from typing import Any, Literal, Mapping, NotRequired, TypedDict
 
+# supported http methods
 Method = Literal["DELETE", "GET", "HEAD", "PATCH", "POST", "PUT"]
 
+# json serializable types
+Serializable = dict | list | str | int | float | bool | None
+
 
 class Resource(TypedDict):
     """Resource to request."""
 
     url: str
     headers: NotRequired[Mapping[str, str] | None]
     params: NotRequired[Mapping[str, str] | None]
-    data: NotRequired[Any | None]
-    json: NotRequired[Any | None]
+    data: NotRequired[Serializable]
+    json: NotRequired[Serializable]
     timeout: NotRequired[int | None]
 
 
 class Request:
     """HTTP request.
 
     Parameters
@@ -26,17 +30,17 @@
         HTTP method.
     url : str
         URL to request.
     headers : Mapping[str, str] | None, optional
         HTTP headers, by default None.
     params : Mapping[str, str] | None, optional
         URL parameters, by default None.
-    data : Any | None, optional
+    data : Serializable, optional
         Request body, by default None.
-    json : Any | None, optional
+    json : Serializable, optional
         JSON request body, by default None.
     timeout : int | None, optional
         Request timeout in seconds, by default None.
     """
 
     def __init__(
         self,
@@ -66,26 +70,27 @@
         """Return the unique identifier of the request.
 
         Returns
         -------
         str
             Unique identifier of the request.
         """
-        # TODO this could/should be improved somehow
         components: list[str] = [
             self.method,
             self.url,
-            json.dumps(self.params, sort_keys=True, ensure_ascii=False).lower(),
-            json.dumps(self.json, sort_keys=True, ensure_ascii=False).lower(),
-            json.dumps(self.data, sort_keys=True, ensure_ascii=False).lower(),
+            json.dumps(self.params, sort_keys=True),
+            json.dumps(self.json, sort_keys=True),
+            json.dumps(self.data, sort_keys=True),
         ]
 
+        # hash the components to generate a unique identifier
         key = blake2b(digest_size=8)
         for component in components:
             key.update(component.encode("utf-8"))
+
         return key.hexdigest()
 
 
 class Response:
     """HTTP response.
 
     Parameters
```

### Comparing `mure-1.0.0b4/pyproject.toml` & `mure-1.0.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mure"
-version = "1.0.0b4"
+version = "1.0.0b5"
 description = "Perform multiple HTTP requests concurrently – without worrying about async/await."
 authors = ["Severin Simmler <s.simmler@snapaddy.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = { extras = ["speedups"], version = "^3.8.5" }
```

### Comparing `mure-1.0.0b4/PKG-INFO` & `mure-1.0.0b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mure
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: Perform multiple HTTP requests concurrently – without worrying about async/await.
 Author: Severin Simmler
 Author-email: s.simmler@snapaddy.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

