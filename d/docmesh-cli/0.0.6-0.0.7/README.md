# Comparing `tmp/docmesh_cli-0.0.6.tar.gz` & `tmp/docmesh_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_cli-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_cli-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_cli-0.0.6.tar` & `docmesh_cli-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.6/README.md
--rw-r--r--   0        0        0       83 2024-05-15 03:02:58.425080 docmesh_cli-0.0.6/docmesh_cli/__init__.py
--rw-r--r--   0        0        0     6368 2024-05-15 03:00:43.919410 docmesh_cli-0.0.6/docmesh_cli/client.py
--rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.6/docmesh_cli/logos.py
--rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.7/README.md
+-rw-r--r--   0        0        0       83 2024-05-17 06:28:46.358197 docmesh_cli-0.0.7/docmesh_cli/__init__.py
+-rw-r--r--   0        0        0     6917 2024-05-17 06:16:22.637165 docmesh_cli-0.0.7/docmesh_cli/client.py
+-rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.7/docmesh_cli/logos.py
+-rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.7/PKG-INFO
```

### Comparing `docmesh_cli-0.0.6/docmesh_cli/client.py` & `docmesh_cli-0.0.7/docmesh_cli/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 SHORTCUTS = {
     "/add": {
         "path": "/add_paper",
         "args": "paper",
         "description": "add a new paper, usage: /add PAPER_TITLE/ARXIV_ID",
     },
-    "/read": {
-        "path": "/read_paper",
+    "/mark": {
+        "path": "/mark_paper",
         "args": "paper_id",
-        "description": "read a paper, usage: /read PAPER_ID",
+        "description": "read a paper, usage: /mark PAPER_ID",
     },
     "/help": {
         "description": "show this help menu",
     },
     "/clear": {
         "description": "clear the session memory",
     },
@@ -152,14 +152,24 @@
 
     # setup headers
     headers = {"Authorization": f"Bearer {access_token}"}
 
     # retreive session_id
     session_id = _login(server, headers, clear=False)
 
+    # switch on/off streaming mode
+    streaming = input(f"{TermColor.red}Streaming mode [y/n]: {TermColor.end}")
+    if streaming.lower() == "y":
+        streaming = True
+    elif streaming.lower() == "n":
+        streaming = False
+    else:
+        print(f"You enter an invalid option {streaming}, turn off streaming mode.")
+        streaming = False
+
     # send query
     while True:
         query = input(f"{TermColor.blue}query: {TermColor.end}")
 
         if query.startswith("/"):
             # trigger shortcut
             if query == "/help":
@@ -195,14 +205,17 @@
                     shortcut_kwargs = {args: shortcut_args}
                 _shortcut(server, path, headers, **shortcut_kwargs)
             except Exception:
                 print(f"{TermColor.red}You enter an invalid shortcut {query}\n{_show_shortcut()}{TermColor.end}")
                 continue
         else:
             data = {"session_id": session_id, "query": query}
-            rsp = requests.post(url=f"{server}/agent", headers=headers, json=data, timeout=300)
-
-            output = rsp.json()["data"]["output"]
-            if rsp.status_code == 200:
-                print(f"{TermColor.green}{output}{TermColor.end}")
+            if streaming:
+                with requests.post(
+                    url=f"{server}/async_agent", headers=headers, json=data, stream=True, timeout=300
+                ) as r:
+                    for chunk in r.iter_content(chunk_size=64):
+                        print(chunk.decode(), end="", flush=True)
             else:
-                print(f"{TermColor.red}{output}{TermColor.end}")
+                rsp = requests.post(url=f"{server}/agent", headers=headers, json=data, timeout=300)
+                msg = rsp.json()["data"]["msg"]
+                print(msg, end="", flush=True)
```

### Comparing `docmesh_cli-0.0.6/docmesh_cli/logos.py` & `docmesh_cli-0.0.7/docmesh_cli/logos.py`

 * *Files identical despite different names*

### Comparing `docmesh_cli-0.0.6/pyproject.toml` & `docmesh_cli-0.0.7/pyproject.toml`

 * *Files identical despite different names*

