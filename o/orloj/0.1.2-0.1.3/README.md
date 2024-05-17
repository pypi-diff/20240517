# Comparing `tmp/orloj-0.1.2.tar.gz` & `tmp/orloj-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orloj-0.1.2.tar", max compression
+gzip compressed data, was "orloj-0.1.3.tar", max compression
```

## Comparing `orloj-0.1.2.tar` & `orloj-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2023-12-06 15:48:59.770410 orloj-0.1.2/LICENSE
--rw-r--r--   0        0        0     3730 2023-12-07 09:35:41.847561 orloj-0.1.2/README.md
--rw-r--r--   0        0        0      471 2024-05-07 05:31:23.277165 orloj-0.1.2/orloj/__init__.py
--rw-r--r--   0        0        0     1998 2024-05-07 05:31:29.130410 orloj-0.1.2/orloj/core.py
--rw-r--r--   0        0        0      921 2024-05-07 05:26:14.825068 orloj-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4408 1970-01-01 00:00:00.000000 orloj-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-12-06 15:48:59.770410 orloj-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3730 2023-12-07 09:35:41.847561 orloj-0.1.3/README.md
+-rw-r--r--   0        0        0      472 2024-05-17 07:41:57.499425 orloj-0.1.3/orloj/__init__.py
+-rw-r--r--   0        0        0     1930 2024-05-17 07:41:46.364960 orloj-0.1.3/orloj/core.py
+-rw-r--r--   0        0        0      922 2024-05-17 07:41:42.538618 orloj-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4409 1970-01-01 00:00:00.000000 orloj-0.1.3/PKG-INFO
```

### Comparing `orloj-0.1.2/LICENSE` & `orloj-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `orloj-0.1.2/README.md` & `orloj-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `orloj-0.1.2/orloj/core.py` & `orloj-0.1.3/orloj/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,66 @@
 #!/usr/bin/env python3.9
 # coding:utf-8
 # Copyright (C) 2023-2024 All rights reserved.
 # FILENAME:    ~~/orloj/core.py
-# VERSION:     0.1.2
+# VERSION:     0.1.3
 # CREATED:     2023-12-06 21:54
 # AUTHOR:      Sitt Guruvanich <aekazitt+github@gmail.com>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
 """Module defining `OrlojMiddleware` class
 """
 
 ### Standard packages ###
 from typing import Any, Callable, Dict
 
 ### Third-party packages ###
-### v3.10.4 API ###
-from apscheduler.schedulers.asyncio import AsyncIOScheduler as AsyncScheduler
-
-### TODO: v4.0.0a4 API ###
-# from apscheduler import AsyncScheduler
-# from apscheduler.triggers.interval import IntervalTrigger
+from apscheduler import AsyncScheduler, RunState
+from apscheduler.triggers.interval import IntervalTrigger
 from starlette.types import ASGIApp, Receive, Scope, Send
 
 
 class OrlojMiddleware:
     app: ASGIApp
-    args: Dict[str, Any]
     interval: int
+    kwargs: Dict[str, Any]
     job: Callable
+    job_id: str
     scheduler: AsyncScheduler
 
     def __init__(
         self,
         app: ASGIApp,
         job: Callable,
+        job_id: str,
         scheduler: AsyncScheduler = AsyncScheduler(),
         interval: int = 3_600,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         self.app = app
-        self.args = {key: value for key, value in args}
-        self.args.update(kwargs)
         self.interval = interval
+        self.kwargs = {key: value for key, value in args}
+        self.kwargs.update(kwargs)
         self.job = job
+        self.job_id = job_id
         self.scheduler = scheduler
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         if scope["type"] == "lifespan":
-            ### v3.10.4 API ###
-            self.scheduler.add_job(self.job, "interval", self.args.values(), seconds=self.interval)
-            self.scheduler.start()
-
-            ### TODO:: v4.0.0a4 API ###
-            # async with self.scheduler:
-            #     await self.scheduler.add_schedule(
-            #         self.job, IntervalTrigger(seconds=self.interval), self.args.values(), id=uuid()
-            #     )
-            #     await self.scheduler.start_in_background()
-
+            async with self.scheduler:
+                await self.scheduler.add_schedule(
+                    self.job,
+                    IntervalTrigger(seconds=self.interval),
+                    id=self.job_id,
+                    kwargs=self.kwargs,
+                )
+                if self.scheduler.state != RunState.started:
+                    await self.scheduler.start_in_background()
+                await self.app(scope, receive, send)
+        else:
             await self.app(scope, receive, send)
 
 
-__all__ = ["OrlojMiddleware"]
+__all__ = ("OrlojMiddleware",)
```

### Comparing `orloj-0.1.2/pyproject.toml` & `orloj-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 [tool.poetry]
 authors = ['Sitt Guruvanich <aekazitt+github@gmail.com>']
 description = 'Scheduler middleware for ASGI frameworks'
 license = 'MIT'
 name = 'orloj'
 packages = [{include='orloj'}]
 readme = 'README.md'
-version = '0.1.2'
+version = '0.1.3'
 
 
 [tool.poetry.dependencies]
-APScheduler = '>=3.10.4,<4.0.0'
+APScheduler = '>=4.0.0a4,<5.0.0'
 python = '^3.8'
 starlette = '<0.37.2'
 
 
 [tool.poetry.group.dev]
 optional = true
 
@@ -43,9 +43,9 @@
 
 
 [tool.poetry.group.examples]
 optional = true
 
 
 [tool.poetry.group.examples.dependencies]
-fastapi = '^0.104.0'
+fastapi = '^0.109.0'
 uvicorn = '^0.15.0'
```

### Comparing `orloj-0.1.2/PKG-INFO` & `orloj-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: orloj
-Version: 0.1.2
+Version: 0.1.3
 Summary: Scheduler middleware for ASGI frameworks
 License: MIT
 Author: Sitt Guruvanich
 Author-email: aekazitt+github@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: APScheduler (>=3.10.4,<4.0.0)
+Requires-Dist: APScheduler (>=4.0.0a4,<5.0.0)
 Requires-Dist: starlette (<0.37.2)
 Description-Content-Type: text/markdown
 
 # Orloj
 
 [![Format](https://img.shields.io/pypi/format/orloj)](https://pypi.org/project/orloj)
 [![Python version](https://img.shields.io/pypi/pyversions/orloj)](https://pypi.org/project/orloj)
```

