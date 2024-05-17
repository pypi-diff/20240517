# Comparing `tmp/docmesh_agent-0.0.5.tar.gz` & `tmp/docmesh_agent-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_agent-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_agent-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_agent-0.0.5.tar` & `docmesh_agent-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.5/README.md
--rw-r--r--   0        0        0       22 2024-05-16 05:02:55.471515 docmesh_agent-0.0.5/docmesh_agent/__init__.py
--rw-r--r--   0        0        0     1799 2024-05-15 02:56:58.892615 docmesh_agent-0.0.5/docmesh_agent/agent.py
--rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.5/docmesh_agent/embeddings/__init__.py
--rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.5/docmesh_agent/embeddings/embeddings.py
--rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.5/docmesh_agent/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.5/docmesh_agent/parser/output_parser.py
--rw-r--r--   0        0        0      186 2024-05-10 11:02:39.301355 docmesh_agent-0.0.5/docmesh_agent/toolkit/__init__.py
--rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.5/docmesh_agent/toolkit/entity.py
--rw-r--r--   0        0        0     1035 2024-05-16 03:38:06.823760 docmesh_agent-0.0.5/docmesh_agent/toolkit/paper.py
--rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.5/docmesh_agent/toolkit/recommend.py
--rw-r--r--   0        0        0      881 2024-05-16 03:36:36.235578 docmesh_agent-0.0.5/docmesh_agent/tools/__init__.py
--rw-r--r--   0        0        0     1104 2024-05-10 11:02:39.301355 docmesh_agent-0.0.5/docmesh_agent/tools/base.py
--rw-r--r--   0        0        0     2304 2024-05-13 04:13:58.029801 docmesh_agent-0.0.5/docmesh_agent/tools/entity.py
--rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.5/docmesh_agent/tools/graph_tools.py
--rw-r--r--   0        0        0     8856 2024-05-16 03:35:20.727428 docmesh_agent-0.0.5/docmesh_agent/tools/paper.py
--rw-r--r--   0        0        0     4384 2024-05-16 02:53:38.522240 docmesh_agent-0.0.5/docmesh_agent/tools/recommend.py
--rw-r--r--   0        0        0      727 2024-05-15 11:38:47.189942 docmesh_agent-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 docmesh_agent-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.6/README.md
+-rw-r--r--   0        0        0       22 2024-05-17 06:26:10.956419 docmesh_agent-0.0.6/docmesh_agent/__init__.py
+-rw-r--r--   0        0        0     3757 2024-05-17 06:25:06.227662 docmesh_agent-0.0.6/docmesh_agent/agent.py
+-rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.6/docmesh_agent/embeddings/__init__.py
+-rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.6/docmesh_agent/embeddings/embeddings.py
+-rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.6/docmesh_agent/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.6/docmesh_agent/parser/output_parser.py
+-rw-r--r--   0        0        0      241 2024-05-16 11:24:43.283487 docmesh_agent-0.0.6/docmesh_agent/toolkit/__init__.py
+-rw-r--r--   0        0        0      344 2024-05-16 11:24:22.979445 docmesh_agent-0.0.6/docmesh_agent/toolkit/common.py
+-rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.6/docmesh_agent/toolkit/entity.py
+-rw-r--r--   0        0        0     1035 2024-05-16 03:38:06.823760 docmesh_agent-0.0.6/docmesh_agent/toolkit/paper.py
+-rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.6/docmesh_agent/toolkit/recommend.py
+-rw-r--r--   0        0        0      940 2024-05-16 11:23:32.443342 docmesh_agent-0.0.6/docmesh_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-16 10:38:39.849612 docmesh_agent-0.0.6/docmesh_agent/tools/base.py
+-rw-r--r--   0        0        0      721 2024-05-17 03:08:13.917254 docmesh_agent-0.0.6/docmesh_agent/tools/common.py
+-rw-r--r--   0        0        0     2021 2024-05-16 10:36:55.425382 docmesh_agent-0.0.6/docmesh_agent/tools/entity.py
+-rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.6/docmesh_agent/tools/graph_tools.py
+-rw-r--r--   0        0        0     8572 2024-05-16 10:44:03.526324 docmesh_agent-0.0.6/docmesh_agent/tools/paper.py
+-rw-r--r--   0        0        0     4351 2024-05-16 11:14:29.378232 docmesh_agent-0.0.6/docmesh_agent/tools/recommend.py
+-rw-r--r--   0        0        0      750 2024-05-17 06:25:49.500169 docmesh_agent-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 docmesh_agent-0.0.6/PKG-INFO
```

### Comparing `docmesh_agent-0.0.5/docmesh_agent/embeddings/embeddings.py` & `docmesh_agent-0.0.6/docmesh_agent/embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.5/docmesh_agent/parser/output_parser.py` & `docmesh_agent-0.0.6/docmesh_agent/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.5/docmesh_agent/toolkit/entity.py` & `docmesh_agent-0.0.6/docmesh_agent/toolkit/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.5/docmesh_agent/toolkit/paper.py` & `docmesh_agent-0.0.6/docmesh_agent/toolkit/paper.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.5/docmesh_agent/toolkit/recommend.py` & `docmesh_agent-0.0.6/docmesh_agent/toolkit/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.5/docmesh_agent/tools/base.py` & `docmesh_agent-0.0.6/docmesh_agent/tools/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 
 class BaseAgentTool(BaseTool):
     entity_name: str
 
     def _preporcess_input(self, s: str) -> str:
         # in some rare case, input may include the keyword
         # `Observation` in prompt.
-        s = s.strip().replace("Observation:", "").replace("Observation", "").strip()
+        if isinstance(s, str):
+            s = s.strip().replace("Observation:", "").replace("Observation", "").strip()
         return s
 
     def _raise_tool_error(self, err_msg: str) -> None:
         raise ToolException(err_msg)
 
     def _dataframe_to_msg(self, df: DataFrame) -> str:
         columns = df.columns.to_list()
```

### Comparing `docmesh_agent-0.0.5/docmesh_agent/tools/entity.py` & `docmesh_agent-0.0.6/docmesh_agent/tools/entity.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,33 +39,25 @@
     ) -> str:
         df = list_follows(entity_name=self.entity_name)
         msg = self._dataframe_to_msg(df)
         return f"\n{msg}\n"
 
 
 class ListPopularEntitiesToolInput(BaseModel):
-    n: str = Field(description="number of entities")
+    n: int = Field(description="number of entities")
 
 
 class ListPopularEntitiesTool(BaseAgentTool):
     name: str = "list_popular_entities"
     description: str = "useful when you need to list popular entities"
     args_schema: Optional[Type[BaseModel]] = ListPopularEntitiesToolInput
     handle_tool_error: bool = True
 
     def _run(
         self,
-        n: str,
+        n: int,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         n = self._preporcess_input(n)
-        try:
-            n = int(n)
-        except Exception:
-            self._raise_tool_error(
-                "Input argument `n` should be an integer, please check your input. "
-                "Pay attention that you MUST ONLY input the number, like 1, 3, 5.\n"
-            )
-
         df = list_popular_entities(n=n)
         msg = self._dataframe_to_msg(df)
         return f"\n{msg}\n"
```

### Comparing `docmesh_agent-0.0.5/docmesh_agent/tools/graph_tools.py` & `docmesh_agent-0.0.6/docmesh_agent/tools/graph_tools.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.5/docmesh_agent/tools/paper.py` & `docmesh_agent-0.0.6/docmesh_agent/tools/paper.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,36 +235,28 @@
                 "Pay attention that paper_id is not arxiv id."
             )
         msg = paper.summary
         return f"\n{msg}\n"
 
 
 class ListLatestPaperToolInput(BaseModel):
-    n: str = Field(description="number of papers")
+    n: int = Field(description="number of papers")
 
 
 class ListLatestPaperTool(BaseAgentTool):
     name: str = "list_latest_papers"
     description: str = (
         "useful when you need to find out latest reading papers, "
         "return a list of paper ids and titles for a given number."
     )
     args_schema: Optional[Type[BaseModel]] = ListLatestPaperToolInput
     handle_tool_error: bool = True
 
     def _run(
         self,
-        n: str,
+        n: int,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         n = self._preporcess_input(n)
-        try:
-            n = int(n)
-        except Exception:
-            self._raise_tool_error(
-                "Input argument `n` should be an integer, please check your inputt. "
-                "Pay attention that you MUST ONLY input the number, like 1, 3, 5.\n"
-            )
-
         df = list_latest_papers(entity_name=self.entity_name, n=n)
         msg = self._dataframe_to_msg(df)
         return f"\n{msg}\n"
```

### Comparing `docmesh_agent-0.0.5/docmesh_agent/tools/recommend.py` & `docmesh_agent-0.0.6/docmesh_agent/tools/recommend.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,118 +14,120 @@
     list_unread_semantic_papers,
 )
 from docmesh_agent.tools.base import BaseAgentTool
 from docmesh_agent.embeddings.embeddings import query_embeddings
 
 
 class UnreadFollowsToolInput(BaseModel):
-    n: str = Field(description="number of papers")
+    n: int = Field(description="number of papers")
 
 
 class UnreadFollowsTool(BaseAgentTool):
     name: str = "recommend_papers_from_follows"
     description: str = "useful when you need to get some recommanded papers from follows"
     args_schema: Optional[Type[BaseModel]] = UnreadFollowsToolInput
     handle_tool_error: bool = True
 
     def _run(
         self,
-        n: str,
+        n: int,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         n = self._preporcess_input(n)
-        try:
-            n = int(n)
-        except Exception:
-            self._raise_tool_error(
-                "Input argument `n` should be an integer, please check your inputt. "
-                "Pay attention that you MUST ONLY input the number, like 1, 3, 5.\n"
-            )
-
         df = list_unread_follows_papers(entity_name=self.entity_name, n=n)
         msg = self._dataframe_to_msg(df)
         return f"\n{msg}\n"
 
 
 class UnreadInfluentialToolInput(BaseModel):
     date_time: str = Field(description="publication date time of papers")
+    n: int = Field(description="number of papers")
 
 
 class UnreadInfluentialTool(BaseAgentTool):
     name: str = "recommend_latest_influential_papers"
     description: str = "useful when you need to get some influential papers from a given date"
     args_schema: Optional[Type[BaseModel]] = UnreadInfluentialToolInput
     handle_tool_error: bool = True
 
     def _run(
         self,
         date_time: str,
+        n: int,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         date_time = self._preporcess_input(date_time)
         try:
             datetime.strptime(date_time, "%Y-%m-%d")
         except Exception:
             self._raise_tool_error(
                 "Input argument `date_time` should be written in format `YYYY-MM-DD`, "
                 "please check your input, valid input can be 1995-03-01, 2024-01-01.\n"
             )
 
-        df = list_unread_influential_papers(entity_name=self.entity_name, date_time=date_time)
+        df = list_unread_influential_papers(
+            entity_name=self.entity_name,
+            date_time=date_time,
+            n=n,
+        )
         msg = self._dataframe_to_msg(df)
         return f"\n{msg}\n"
 
 
 class UnreadSimilarToolInput(BaseModel):
     paper_id: str = Field(description="paper id")
+    n: int = Field(description="number of papers")
 
 
 class UnreadSimilarTool(BaseAgentTool):
     name: str = "recommend_similar_papers"
     description: str = "useful when you need to get some similar papers from provided paper id"
     args_schema: Optional[Type[BaseModel]] = UnreadSimilarToolInput
     handle_tool_error: bool = True
 
     def _run(
         self,
         paper_id: str,
+        n: int,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         paper_id = self._preporcess_input(paper_id)
         df = list_unread_similar_papers(
             entity_name=self.entity_name,
             paper_id=paper_id,
-            n=10,
+            n=n,
         )
         # keep score over 0.5 and drop the column
         df = df[df["score"] > 0.5].drop(columns="score")
         msg = self._dataframe_to_msg(df)
         return f"\n{msg}\n"
 
 
 class UnreadSemanticToolInput(BaseModel):
     query: str = Field(description="search query")
+    n: int = Field(description="number of papers")
 
 
 class UnreadSemanticTool(BaseAgentTool):
     name: str = "recommend_queried_papers"
     description: str = "useful when you need to get some papers from a query"
     args_schema: Optional[Type[BaseModel]] = UnreadSemanticToolInput
     handle_tool_error: bool = True
 
     def _run(
         self,
         query: str,
+        n: int,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         query = self._preporcess_input(query)
         query_embedded = query_embeddings(query)
 
         df = list_unread_semantic_papers(
             entity_name=self.entity_name,
             semantic_embedding=query_embedded,
-            n=10,
+            n=n,
         )
         # keep score over 0.5 and drop the column
         df = df[df["score"] > 0.5].drop(columns="score")
         msg = self._dataframe_to_msg(df)
         return f"\n{msg}\n"
```

### Comparing `docmesh_agent-0.0.5/pyproject.toml` & `docmesh_agent-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "docmesh-core>=0.0.2",
+    "docmesh-core>=0.0.5",
+    "colorama>=0.4.6",
     "pymupdf>=1.24.3",
     "faiss-cpu>=1.8.0",
     "langchain>=0.1.15",
     "langchain-openai>=0.1.3",
     "langchainhub>=0.1.15",
 ]
```

### Comparing `docmesh_agent-0.0.5/PKG-INFO` & `docmesh_agent-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: docmesh_agent
-Version: 0.0.5
+Version: 0.0.6
 Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh-core>=0.0.2
+Requires-Dist: docmesh-core>=0.0.5
+Requires-Dist: colorama>=0.4.6
 Requires-Dist: pymupdf>=1.24.3
 Requires-Dist: faiss-cpu>=1.8.0
 Requires-Dist: langchain>=0.1.15
 Requires-Dist: langchain-openai>=0.1.3
 Requires-Dist: langchainhub>=0.1.15
 
 # docmesh agent
```

