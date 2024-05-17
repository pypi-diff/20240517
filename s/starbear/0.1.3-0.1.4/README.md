# Comparing `tmp/starbear-0.1.3.tar.gz` & `tmp/starbear-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbear-0.1.3.tar", max compression
+gzip compressed data, was "starbear-0.1.4.tar", max compression
```

## Comparing `starbear-0.1.3.tar` & `starbear-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      804 2024-04-02 15:08:35.685190 starbear-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      314 2024-02-29 00:44:16.645421 starbear-0.1.3/starbear/__init__.py
--rw-r--r--   0        0        0      276 2023-12-18 19:59:00.300414 starbear-0.1.3/starbear/bearlib-template.html
--rw-r--r--   0        0        0    23868 2024-03-28 03:45:42.824944 starbear-0.1.3/starbear/bearlib.js
--rw-r--r--   0        0        0     1049 2024-02-02 19:46:01.148155 starbear-0.1.3/starbear/bearstyle.css
--rw-r--r--   0        0        0     2206 2024-02-29 00:50:48.026310 starbear-0.1.3/starbear/constructors.py
--rw-r--r--   0        0        0      322 2024-02-12 21:08:30.565978 starbear-0.1.3/starbear/page-template.html
--rw-r--r--   0        0        0    10202 2024-02-01 21:21:51.768382 starbear-0.1.3/starbear/page.py
--rw-r--r--   0        0        0     2264 2024-02-01 21:13:07.770061 starbear-0.1.3/starbear/ref.py
--rw-r--r--   0        0        0     7708 2024-02-01 21:14:06.522289 starbear-0.1.3/starbear/repr.py
--rw-r--r--   0        0        0    18401 2024-02-29 01:06:30.383219 starbear-0.1.3/starbear/serve.py
--rw-r--r--   0        0        0     4117 2024-01-19 16:02:41.325613 starbear-0.1.3/starbear/templating.py
--rw-r--r--   0        0        0     4819 2024-02-02 19:44:20.515869 starbear-0.1.3/starbear/utils.py
--rw-r--r--   0        0        0       18 2024-04-02 15:08:35.705934 starbear-0.1.3/starbear/version.py
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 starbear-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      708 2024-05-17 18:53:54.379104 starbear-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      383 2024-05-02 20:10:45.559615 starbear-0.1.4/starbear/__init__.py
+-rw-r--r--   0        0        0      276 2023-12-18 19:59:00.300414 starbear-0.1.4/starbear/bearlib-template.html
+-rw-r--r--   0        0        0    23883 2024-04-26 19:04:39.586276 starbear-0.1.4/starbear/bearlib.js
+-rw-r--r--   0        0        0     1049 2024-02-02 19:46:01.148155 starbear-0.1.4/starbear/bearstyle.css
+-rw-r--r--   0        0        0     2206 2024-02-29 00:50:48.026310 starbear-0.1.4/starbear/constructors.py
+-rw-r--r--   0        0        0      322 2024-02-12 21:08:30.565978 starbear-0.1.4/starbear/page-template.html
+-rw-r--r--   0        0        0    10370 2024-05-02 20:12:38.546585 starbear-0.1.4/starbear/page.py
+-rw-r--r--   0        0        0     2226 2024-05-02 20:12:38.548759 starbear-0.1.4/starbear/ref.py
+-rw-r--r--   0        0        0     7708 2024-02-01 21:14:06.522289 starbear-0.1.4/starbear/repr.py
+-rw-r--r--   0        0        0    19006 2024-05-02 20:22:05.098297 starbear-0.1.4/starbear/serve.py
+-rw-r--r--   0        0        0     4117 2024-01-19 16:02:41.325613 starbear-0.1.4/starbear/templating.py
+-rw-r--r--   0        0        0     4831 2024-05-17 18:44:07.443188 starbear-0.1.4/starbear/utils.py
+-rw-r--r--   0        0        0       18 2024-05-17 18:53:54.400658 starbear-0.1.4/starbear/version.py
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 starbear-0.1.4/PKG-INFO
```

### Comparing `starbear-0.1.3/pyproject.toml` & `starbear-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 [tool.poetry]
 name = "starbear"
-version = "0.1.3"
+version = "0.1.4"
 description = "Framework for easy small local web apps or programs"
 authors = ["Olivier Breuleux <breuleux@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uvicorn = ">=0.17.6"
 starlette = ">=0.27.0"
 websockets = "^10.3"
 hrepr = "^0.6.1"
 lxml = "^4.9.3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.8.0"
-isort = "^5.10.1"
-flake8-pyproject = "^1.2.2"
+ruff = "^0.4.2"
 sphinx = "^5.3.0"
 sphinx-rtd-theme = "^1.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-known_first_party = "starbear"
-known_third_party = ""
-multi_line_output = 3
-include_trailing_comma = true
-combine_as_imports = true
-
-[tool.flake8]
-ignore = "E501,E203,W503,F722"
-per-file-ignores = [
-  "__init__.py:F401"
-]
+[tool.ruff]
+line-length = 99
+
+[tool.ruff.lint]
+extend-select = ["I"]
+
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = ["F401", "F403"]
+
+[tool.ruff.lint.isort]
+combine-as-imports = true
```

### Comparing `starbear-0.1.3/starbear/bearlib.js` & `starbear-0.1.4/starbear/bearlib.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -170,15 +170,15 @@
         this.ex.classList.remove("bear--hidden");
     }
 
     write(tab, node, append = false) {
         let area = this.areaData[tab];
         if (!append) {
             area.element.innerHTML = "";
-            if (!node) {
+            if (!node || node === "") {
                 area.button.classList.add("bear--empty");
                 return;
             }
         }
         let container = document.createElement("div");
         area.element.append(container);
         container.append(node);
```

### Comparing `starbear-0.1.3/starbear/bearstyle.css` & `starbear-0.1.4/starbear/bearstyle.css`

 * *Files identical despite different names*

### Comparing `starbear-0.1.3/starbear/constructors.py` & `starbear-0.1.4/starbear/constructors.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.3/starbear/page.py` & `starbear-0.1.4/starbear/page.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,42 @@
 from hrepr.hgen import ResourceDeduplicator
 from hrepr.resource import Resource
 
 from .ref import Reference
 from .utils import format_error
 
 
+def selector_for(x):
+    if isinstance(x, Tag):
+        tid = x.attributes.get("id", None)
+        if not tid:
+            raise Exception("Cannot locate element because it has no id.")
+        return f"#{tid}"
+    elif isinstance(x, str):
+        return x
+    elif isinstance(x, Reference):
+        return f'[--ref="obj#{x.id}"]'
+    elif (selector := getattr(x, "selector", None)) and isinstance(selector, str):
+        return selector
+    else:
+        raise TypeError(
+            "A valid selector must be a str, Tag, Reference or an object"
+            " with a string attribute named `selector`."
+        )
+
+
+class Component:
+    @property
+    def selector(self):
+        return selector_for(self.node)
+
+    def __hrepr__(self, H, hrepr):
+        return self.node
+
+
 class Page:
     def __init__(
         self,
         instance,
         selector=None,
         track_history=True,
         sent_resources=None,
@@ -32,30 +60,17 @@
         self.debug = debug
         self.loop = loop or aio.get_running_loop()
         self.js = JavaScriptOperation(self, [])
         self.window = JavaScriptOperation(self, [], root="window")
         self.bearlib = JavaScriptOperation(self, [], root="$$BEAR")
 
     def __getitem__(self, selector):
-        def _map_selector(x):
-            if isinstance(x, Tag):
-                tid = x.attributes.get("id", None)
-                if not tid:
-                    raise Exception("Cannot locate element because it has no id.")
-                return f"#{tid}"
-            elif isinstance(x, str):
-                return x
-            elif isinstance(x, Reference):
-                return f'[--ref="obj#{x.id}"]'
-            else:
-                raise TypeError("Only str or Tag can be used as a selector")
-
         if not isinstance(selector, tuple):
             selector = (selector,)
-        selector = " ".join(map(_map_selector, selector))
+        selector = " ".join(map(selector_for, selector))
 
         if self.selector is not None:
             selector = f"{self.selector} {selector}"
 
         return self.page_select(selector)
 
     def page_select(self, selector):
@@ -149,28 +164,24 @@
             (
                 list(self._generate_put_commands(element, method, send_resources)),
                 history,
             )
         )
 
     def put_nowait(self, element, method, history=None, send_resources=True):
-        self._push(
-            self.put(element, method, history=history, send_resources=send_resources)
-        )
+        self._push(self.put(element, method, history=history, send_resources=send_resources))
 
     def queue_command(self, command, /, history=None, **arguments):
         if history is None:
             history = self.track_history
         arguments["command"] = command
         self._push(self.oq.put((arguments, history)))
 
     def set_title(self, title):
-        self.queue_command(
-            "put", selector="head title", content=title, method="innerHTML"
-        )
+        self.queue_command("put", selector="head title", content=title, method="innerHTML")
 
     def add_resources(self, *resources, type=None):
         def _build(resource, name):
             if name.endswith(".css") or type == "text/css":
                 return H.link(rel="stylesheet", href=resource)
             elif name.endswith(".js") or type == "text/javascript":
                 return H.script(src=resource)
@@ -199,17 +210,15 @@
         for element in elements:
             element = self._to_element(element)
             self.put_nowait(element, method)
 
     def error(self, message, debug=None, exception=None):
         if not isinstance(message, str):
             message = str(self.representer.hrepr(message))
-        self.queue_command(
-            "error", content=format_error(message, debug, exception, self.debug)
-        )
+        self.queue_command("error", content=format_error(message, debug, exception, self.debug))
 
     def log(self, message):
         if not isinstance(message, str):
             message = self.representer.hrepr(message)
         self.queue_command("log", content=str(message))
 
     def print_html(self, html, selector=None, method="beforeend", history=None):
@@ -260,17 +269,15 @@
             title="Page",
             fields=[["selector", self.selector]],
             delimiter=":",
         )
 
     def __js_embed__(self, representer):
         if self.selector is None:
-            raise Exception(
-                "Cannot send page reference to JS because it has no selector."
-            )
+            raise Exception("Cannot send page reference to JS because it has no selector.")
         return f"document.querySelector('{self.selector}')"
 
     async def recv(self):
         return await self.iq.get()
 
 
 def _extractor(root, sequence):
```

### Comparing `starbear-0.1.3/starbear/ref.py` & `starbear-0.1.4/starbear/ref.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,17 +35,15 @@
         self.map[currid] = obj
         self.ids.append(currid)
         if len(self.ids) > self.keep >= 0:
             if self.rotate:
                 rm = self.ids.popleft()
                 del self.map[rm]
             else:
-                raise Exception(
-                    "Exceeded limit for keeping strong references to objects."
-                )
+                raise Exception("Exceeded limit for keeping strong references to objects.")
         return currid
 
     def resolve(self, id):
         return self.map[id]
 
 
 class WeakRegistry:
```

### Comparing `starbear-0.1.3/starbear/repr.py` & `starbear-0.1.4/starbear/repr.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.3/starbear/serve.py` & `starbear-0.1.4/starbear/serve.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from contextvars import ContextVar
 from functools import cached_property, wraps
 from itertools import count
 from pathlib import Path
 from uuid import uuid4 as uuid
 
 from hrepr import H, Tag
+from more_itertools import take
 from starlette.exceptions import HTTPException
 from starlette.responses import (
     FileResponse,
     HTMLResponse,
     JSONResponse,
     PlainTextResponse,
     RedirectResponse,
@@ -76,15 +77,15 @@
             method = getattr(obj, method_name)
             routeinfo = method.routeinfo
             yield method, routeinfo
 
 
 def autoroutes(defns, prefix, mangle, wrap=None):
     routes = []
-    for (method, routeinfo) in defns:
+    for method, routeinfo in defns:
         wmeth = wrap(method, routeinfo) if wrap else method
         mname = mangle(routeinfo["name"])
         route = routeinfo["cls"](
             prefix + routeinfo["path"] + routeinfo["params"],
             wmeth,
             name=mname,
             **routeinfo["keywords"],
@@ -167,19 +168,15 @@
         }
 
     ###################
     # Basic functions #
     ###################
 
     def template_asset(self, name, where):
-        return (
-            self.route
-            + "/file/"
-            + self.representer.file_registry.register(where / name)
-        )
+        return self.route + "/file/" + self.representer.file_registry.register(where / name)
 
     def template(self, template_path=None, **params):
         template_path = template_path or self._template
         location = template_path.parent
         agg_params = {
             **self._template_params,
             "route": self.route,
@@ -258,21 +255,17 @@
             qid=data["reqid"],
             value=data["value"],
         )
         return JSONResponse({"status": "ok"})
 
     @routeinfo("/{path:path}")
     async def route_file(self, request):
-        pth = self.representer.file_registry.get_file_from_url(
-            request.path_params["path"]
-        )
+        pth = self.representer.file_registry.get_file_from_url(request.path_params["path"])
         if pth is None:
-            raise HTTPException(
-                status_code=404, detail="File not found or not available."
-            )
+            raise HTTPException(status_code=404, detail="File not found or not available.")
         return FileResponse(pth, headers={"Cache-Control": "no-cache"})
 
     @routeinfo("/{path:path}")
     async def route_vfile(self, request):
         vf = self.representer.vfile_registry.get(request.path_params["path"])
         return Response(content=vf.content, media_type=vf.type)
 
@@ -352,51 +345,42 @@
         self.iq = Queue()
         self.oq = Queue()
         self.history = []
         self.reset = False
         self.ws = None
         self.page = Page(instance=self, debug=debug_mode.get())
         self.coro = aio.create_task(self.run())
-        self._sd_coro = None
         self.log("info", "Created process")
 
     def log(self, level, msg, **extra):
         try:
             user = self.session.get("user", {}).get("email", None)
-        except:
+        except:  # noqa: E722
             logger.error("Could not get user")
         getattr(logger, level)(msg, extra={"proc": self.process, "user": user, **extra})
 
-    def schedule_selfdestruct(self):
-        async def sd():
-            await aio.sleep(self.mother.process_timeout)
-            del self.mother.cubs[self.process]
-            self.coro.cancel()
-            self.log("info", "Destroyed process")
-
-        if self.mother.process_timeout is not None:
-            self._sd_coro = aio.create_task(sd())
-
-    def unschedule_selfdestruct(self):
-        if self._sd_coro:
-            self._sd_coro.cancel()
-            self._sd_coro = None
+    def destroy(self):
+        self.coro.cancel()
 
     async def run(self):
+        reason = "done"
         try:
             await self.fn(self.page)
             await self.page.sync()
+        except aio.CancelledError:
+            reason = "cancelled"
         except Exception as exc:
+            reason = "error"
             self.log("error", str(exc), traceback=traceback)
             self.page.error(
                 message=H.b("An error occurred. You may need to refresh the page."),
                 exception=exc,
             )
         finally:
-            self.log("info", "Finished process")
+            self.log("info", f"Finished process ({reason})")
 
     def object_pairs_hook(self, pairs):
         dct = NamespaceDict(pairs)
         if "%" in dct:
             return construct(self.page, dct)
         else:
             return dct
@@ -419,30 +403,30 @@
 
     ##############
     # Cub routes #
     ##############
 
     @routeinfo(root=True)
     async def route_main(self, request):
-        self.unschedule_selfdestruct()
+        self.mother.declare_active(self)
         node = self.template()
         self.reset = True
         html = self.representer.generate_string(node)
         return HTMLResponse(
             f"<!DOCTYPE html>\n{html}",
             headers={
                 "Cache-Control": "no-cache, no-store, must-revalidate",
                 "Pragma": "no-cache",
                 "Expires": "0",
             },
         )
 
     @routeinfo(cls=WebSocketRoute)
     async def route_socket(self, ws):
-        self.unschedule_selfdestruct()
+        self.mother.declare_active(self)
 
         async def recv():
             while True:
                 try:
                     data = await ws.receive_json()
                     self.iq.put_nowait(data)
                 except WebSocketDisconnect:
@@ -474,49 +458,86 @@
                 await ws.send_text(entry)
             self.reset = False
 
         await aio.wait(
             [aio.create_task(recv()), aio.create_task(send())],
             return_when=aio.FIRST_COMPLETED,
         )
-        self.schedule_selfdestruct()
+        self.mother.declare_dormant(self)
 
 
 def get_process_from_request(request):
     process_base = request.path_params.get("process", None)
     if process_base is None:
         process_base = base64.urlsafe_b64encode(uuid().bytes).decode("utf8").strip("=")
     return process_base
 
 
 class MotherBear(AbstractBear):
-    def __init__(self, fn, process_timeout=60, hide_processes=True, **cub_params):
+    def __init__(
+        self,
+        fn,
+        soft_process_cap=1_000,
+        hard_process_cap=1_000_000,
+        hide_processes=True,
+        **cub_params,
+    ):
         super().__init__()
         self.fn = fn
         self.__doc__ = getattr(fn, "__doc__", None)
         self.router = None
-        self.process_timeout = process_timeout
+        self.hard_process_cap = hard_process_cap
+        self.soft_process_cap = soft_process_cap
         self.hide_processes = hide_processes
         self.cub_params = cub_params
         self.cubs = {}
+        self.dormant_cubs = {}
+
+    #############
+    # Utilities #
+    #############
+
+    def _create_new_cub(self, proc, query_params, session):
+        reclaims = max(0, min(len(self.dormant_cubs), len(self.cubs) - self.soft_process_cap))
+        processes = take(n=reclaims, iterable=self.dormant_cubs)
+
+        for p in processes:
+            cub = self.dormant_cubs.pop(p)
+            cub.destroy()
+            del self.cubs[p]
+
+        if len(self.cubs) > self.hard_process_cap:
+            raise Exception("Cannot serve request: too many processes exist.")
+
+        self.cubs[proc] = Cub(
+            self,
+            proc,
+            query_params=query_params,
+            session=session,
+            **self.cub_params,
+        )
 
     def _get(self, proc, query_params={}, session={}, ensure=False):
         if proc not in self.cubs:
             if ensure:
-                self.cubs[proc] = Cub(
-                    self,
+                self._create_new_cub(
                     proc,
                     query_params=query_params,
                     session=session,
-                    **self.cub_params,
                 )
             else:
                 return None
         return self.cubs[proc]
 
+    def declare_active(self, cub):
+        self.dormant_cubs.pop(cub.process, None)
+
+    def declare_dormant(self, cub):
+        self.dormant_cubs[cub.process] = cub
+
     #################
     # Mother routes #
     #################
 
     @routeinfo(root=True)
     async def route_dispatch(self, request):
         self.ensure_router(request)
```

### Comparing `starbear-0.1.3/starbear/templating.py` & `starbear-0.1.4/starbear/templating.py`

 * *Files identical despite different names*

### Comparing `starbear-0.1.3/starbear/utils.py` & `starbear-0.1.4/starbear/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         return await self.get()
 
+    def __call__(self, value):
+        return self.put(value)
+
 
 def format_error(message, debug=None, exception=None, show_debug=False):
     if show_debug:
         tb = exception and traceback.format_exception(
             type(exception),
             exception,
             exception.__traceback__,
@@ -109,15 +112,14 @@
         self.type = type
         self.content = content
         self.name = md5(content.encode("utf8")).hexdigest()
         if name is not None:
             self.name += f"/{name}"
 
 
-@dataclass
 class ClientWrap:
     FIELDS = {
         "debounce",
         "extract",
         "form",
         "refs",
         "pack",
@@ -148,17 +150,15 @@
 
         for x in ["pre", "post"]:
             result = options.get(x, None)
             if result is not None:
                 if not isinstance(result, (list, tuple)):
                     result = [result]
                 result = [
-                    JSExpression(f"function (result) {{ {p} }}")
-                    if isinstance(p, str)
-                    else p
+                    JSExpression(f"function (result) {{ {p} }}") if isinstance(p, str) else p
                     for p in result
                 ]
                 options[x] = result
 
         self.func = func
         self.options = options
```

### Comparing `starbear-0.1.3/PKG-INFO` & `starbear-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: starbear
-Version: 0.1.3
+Version: 0.1.4
 Summary: Framework for easy small local web apps or programs
 License: MIT
 Author: Olivier Breuleux
 Author-email: breuleux@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: hrepr (>=0.6.1,<0.7.0)
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: starlette (>=0.27.0)
 Requires-Dist: uvicorn (>=0.17.6)
 Requires-Dist: websockets (>=10.3,<11.0)
```

