# Comparing `tmp/docmesh_server-0.0.3.tar.gz` & `tmp/docmesh_server-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_server-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_server-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_server-0.0.3.tar` & `docmesh_server-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.3/README.md
--rw-r--r--   0        0        0       64 2024-05-16 05:16:57.517248 docmesh_server-0.0.3/docmesh_server/__init__.py
--rw-r--r--   0        0        0     6397 2024-05-15 11:05:11.588961 docmesh_server-0.0.3/docmesh_server/main.py
--rw-r--r--   0        0        0      673 2024-05-16 05:17:24.217304 docmesh_server-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 docmesh_server-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.4/README.md
+-rw-r--r--   0        0        0       64 2024-05-17 06:28:02.497701 docmesh_server-0.0.4/docmesh_server/__init__.py
+-rw-r--r--   0        0        0     6661 2024-05-17 06:06:54.871868 docmesh_server-0.0.4/docmesh_server/main.py
+-rw-r--r--   0        0        0      673 2024-05-17 06:27:09.409094 docmesh_server-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 docmesh_server-0.0.4/PKG-INFO
```

### Comparing `docmesh_server-0.0.3/docmesh_server/main.py` & `docmesh_server-0.0.4/docmesh_server/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 
 from typing import Any
 from pydantic import BaseModel
 
 from neomodel import config
 from sqlalchemy import create_engine
 from fastapi import status, Depends, HTTPException, Response, FastAPI
+from fastapi.responses import StreamingResponse
 from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
 
 from docmesh_core.utils.semantic_scholar import get_paper_id
 from docmesh_core.db.neo import add_entity, _add_paper, mark_paper_read, DuplicateEntity
 from docmesh_core.db.auth import get_entity_from_auth, add_auth_for_entity
-from docmesh_agent.agent import execute_docmesh_agent
+from docmesh_agent.agent import execute_docmesh_agent, aexecute_docmesh_agnet
 from docmesh_agent.embeddings.embeddings import update_paper_embeddings
 
 if (neo4j_url := os.getenv("NEO4J_URL")) is None:
     raise ValueError("You have not set neo4j database url using environment `NEO4J_URL`.")
 else:
     config.DATABASE_URL = neo4j_url
     # HACK: server may kill idle connection, to avoid being hung for
@@ -188,22 +189,31 @@
 @app.post("/agent")
 def execute_docmesh_agent_api(
     body: AgentBody,
     response: Response,
     token: HTTPAuthorizationCredentials = Depends(auth_scheme),
 ) -> dict[str, Any]:
     entity_name = _check_access_token(token.credentials)
+    msg = execute_docmesh_agent(
+        entity_name=entity_name,
+        query=body.query,
+        session_id=body.session_id,
+    )
+    data = {"query": body.query, "msg": msg}
+    return {"data": data}
 
-    try:
-        output = execute_docmesh_agent(
+
+@app.post("/async_agent")
+async def aexecute_docmesh_agnet_api(
+    body: AgentBody,
+    response: Response,
+    token: HTTPAuthorizationCredentials = Depends(auth_scheme),
+) -> StreamingResponse:
+    entity_name = _check_access_token(token.credentials)
+
+    return StreamingResponse(
+        aexecute_docmesh_agnet(
             entity_name=entity_name,
             query=body.query,
             session_id=body.session_id,
         )
-        data = {"input": body.query, "output": output}
-    except Exception as e:
-        output = f"Failed to answer with error:\n{e}"
-        data = {"input": body.query, "output": output}
-
-        response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
-
-    return {"data": data}
+    )
```

### Comparing `docmesh_server-0.0.3/pyproject.toml` & `docmesh_server-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "docmesh-core>=0.0.4",
-    "docmesh-agent>=0.0.5",
+    "docmesh-core>=0.0.5",
+    "docmesh-agent>=0.0.6",
     "fastapi==0.111.0",
     "uvicorn==0.29.0",
     "gunicorn==19.3.0",
 ]
 
 [tool.flake8]
 max-line-length = 120
```

### Comparing `docmesh_server-0.0.3/PKG-INFO` & `docmesh_server-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: docmesh_server
-Version: 0.0.3
+Version: 0.0.4
 Summary: Server of docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh-core>=0.0.4
-Requires-Dist: docmesh-agent>=0.0.5
+Requires-Dist: docmesh-core>=0.0.5
+Requires-Dist: docmesh-agent>=0.0.6
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: gunicorn==19.3.0
 
 # docemsh server
```

