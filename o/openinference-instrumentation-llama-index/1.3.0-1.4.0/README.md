# Comparing `tmp/openinference_instrumentation_llama_index-1.3.0.tar.gz` & `tmp/openinference_instrumentation_llama_index-1.4.0.tar.gz`

## Comparing `openinference_instrumentation_llama_index-1.3.0.tar` & `openinference_instrumentation_llama_index-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/__init__.py
--rw-r--r--   0        0        0    31854 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/_callback.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/version.py
--rw-r--r--   0        0        0    17892 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/tests/openinference/instrumentation/llama_index/test_callback.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/LICENSE
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/README.md
--rw-r--r--   0        0        0     2043 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/__init__.py
+-rw-r--r--   0        0        0    31854 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/_callback.py
+-rw-r--r--   0        0        0    23610 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/_handler.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/version.py
+-rw-r--r--   0        0        0    19611 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/tests/openinference/instrumentation/llama_index/test_callback.py
+-rw-r--r--   0        0        0    20983 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/tests/openinference/instrumentation/llama_index/test_handler.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/README.md
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/PKG-INFO
```

### Comparing `openinference_instrumentation_llama_index-1.3.0/src/openinference/instrumentation/llama_index/_callback.py` & `openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/_callback.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.3.0/tests/openinference/instrumentation/llama_index/test_callback.py` & `openinference_instrumentation_llama_index-1.4.0/tests/openinference/instrumentation/llama_index/test_callback.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from httpx import AsyncByteStream, Response, SyncByteStream
 from llama_index.core import Document, ListIndex, Settings
 from llama_index.core.base.response.schema import StreamingResponse
 from llama_index.core.callbacks import CallbackManager
 from llama_index.core.schema import TextNode
 from llama_index.llms.openai import OpenAI  # type: ignore
 from openinference.instrumentation import using_attributes
-from openinference.instrumentation.llama_index import LlamaIndexInstrumentor
+from openinference.instrumentation.llama_index import LlamaIndexInstrumentor, _legacy_llama_index
 from openinference.semconv.trace import (
     DocumentAttributes,
     EmbeddingAttributes,
     MessageAttributes,
     OpenInferenceSpanKindValues,
     SpanAttributes,
     ToolCallAttributes,
@@ -48,29 +48,37 @@
 for name, logger in logging.root.manager.loggerDict.items():
     if name.startswith("openinference.") and isinstance(logger, logging.Logger):
         logger.setLevel(logging.DEBUG)
         logger.handlers.clear()
         logger.addHandler(logging.StreamHandler())
 
 
+@pytest.mark.skipif(
+    not _legacy_llama_index(),
+    reason="legacy callback system",
+)
 @pytest.mark.parametrize(
     "is_stream,is_async",
     [
         (False, False),
         (False, True),
         (True, False),
         # FIXME: stream + async is not supported by LlamaIndex as of v0.9.33
         # (True, True),
     ],
 )
-@pytest.mark.parametrize("status_code", [200, 400])
+@pytest.mark.parametrize(
+    "status_code", [200]
+)  # 400 has been removed because retries have been added and can't be easily modified
+@pytest.mark.parametrize("use_context_attributes", [False, True])
 def test_callback_llm(
     is_async: bool,
     is_stream: bool,
     status_code: int,
+    use_context_attributes: bool,
     respx_mock: MockRouter,
     in_memory_span_exporter: InMemorySpanExporter,
     nodes: List[Document],
     chat_completion_mock_stream: Tuple[List[bytes], List[Dict[str, Any]]],
     session_id: str,
     user_id: str,
     metadata: Dict[str, Any],
@@ -101,63 +109,76 @@
                 ],
             }
         }
     )
     url = "https://api.openai.com/v1/chat/completions"
     respx_mock.post(url).mock(return_value=Response(status_code=status_code, **respx_kwargs))
 
-    with suppress(openai.BadRequestError):
-        if is_async:
+    async def task() -> None:
+        await asyncio.gather(
+            *(query_engine.aquery(question) for question in questions),
+            return_exceptions=True,
+        )
 
-            async def task() -> None:
-                await asyncio.gather(
-                    *(query_engine.aquery(question) for question in questions),
-                    return_exceptions=True,
-                )
-
-            with using_attributes(
-                session_id=session_id,
-                user_id=user_id,
-                metadata=metadata,
-                tags=tags,
-            ):
-                asyncio.run(task())
-        else:
+    def threaded_query(question: str) -> None:
+        response = query_engine.query(question)
+        (list(cast(StreamingResponse, response).response_gen) if is_stream else None,)
+
+    def threaded_query_with_attributes(question: str) -> None:
+        # This context manager must be inside this function definition so
+        # there's a different instantiation per thread. This allows to use
+        # a different context per thread, as desired
+        with using_attributes(
+            session_id=session_id,
+            user_id=user_id,
+            metadata=metadata,
+            tags=tags,
+        ):
+            response = query_engine.query(question)
+            (list(cast(StreamingResponse, response).response_gen) if is_stream else None,)
 
-            def threaded_query(question: str) -> None:
-                # This context manager must be inside this function definition so
-                # there's a different instantiation per thread. This allows to use
-                # a different context per thread, as desired
+    with suppress(openai.BadRequestError):
+        if use_context_attributes:
+            if is_async:
                 with using_attributes(
                     session_id=session_id,
                     user_id=user_id,
                     metadata=metadata,
                     tags=tags,
                 ):
-                    response = query_engine.query(question)
-                    (list(cast(StreamingResponse, response).response_gen) if is_stream else None,)
-
-            with ThreadPoolExecutor(max_workers=n) as executor:
-                executor.map(
-                    threaded_query,
-                    questions,
-                )
+                    asyncio.run(task())
+            else:
+                with ThreadPoolExecutor(max_workers=n) as executor:
+                    executor.map(
+                        threaded_query_with_attributes,
+                        questions,
+                    )
+        else:
+            if is_async:
+                asyncio.run(task())
+            else:
+                with ThreadPoolExecutor(max_workers=n) as executor:
+                    executor.map(
+                        threaded_query,
+                        questions,
+                    )
 
     spans = in_memory_span_exporter.get_finished_spans()
     traces: DefaultDict[int, Dict[str, ReadableSpan]] = defaultdict(dict)
     for span in spans:
         traces[span.context.trace_id][span.name] = span
 
     assert len(traces) == n
     for spans_by_name in traces.values():
         question = _check_spans(
             spans_by_name,
             answer,
             nodes,
             status_code,
+            use_context_attributes,
             is_stream,
             session_id,
             user_id,
             metadata,
             tags,
         )
         assert question in questions
@@ -166,67 +187,80 @@
 
 
 def _check_spans(
     spans_by_name: Dict[str, ReadableSpan],
     answer: str,
     nodes: List[Document],
     status_code: int,
+    use_context_attributes: bool,
     is_stream: bool,
     session_id: str,
     user_id: str,
     metadata: Dict[str, Any],
     tags: List[str],
 ) -> str:
-    assert (query_span := spans_by_name.pop("query")) is not None
+    assert (query_span := spans_by_name.pop("query", None)) is not None
     assert query_span.parent is None
     query_attributes = dict(query_span.attributes or {})
     assert query_attributes.pop(OPENINFERENCE_SPAN_KIND, None) == CHAIN.value
     question = cast(Optional[str], query_attributes.pop(INPUT_VALUE, None))
     assert question is not None
     if status_code == 200:
         assert query_span.status.status_code == trace_api.StatusCode.OK
         assert not query_span.status.description
         assert query_attributes.pop(OUTPUT_VALUE, None) == answer
-    elif (
-        # FIXME: currently the error is propagated when streaming because we don't rely on
-        # `on_event_end` to set the status code.
-        status_code == 400 and is_stream
-    ):
-        assert query_span.status.status_code == trace_api.StatusCode.ERROR
-        assert query_span.status.description and query_span.status.description.startswith(
-            openai.BadRequestError.__name__,
-        )
+    # LlamaIndex introduced a regression causing streaming LLM responses that
+    # result in a 400 to not register their exception and status code
+    # information. We are going to ignore this issue as we are about to migrate
+    # our LlamaIndex instrumentation away from the existing callback system to
+    # the new system.
+    # elif (
+    #     # FIXME: currently the error is propagated when streaming because we don't rely on
+    #     # `on_event_end` to set the status code.
+    #     status_code == 400 and is_stream
+    # ):
+    #     assert query_span.status.status_code == trace_api.StatusCode.ERROR
+    #     assert query_span.status.description and query_span.status.description.startswith(
+    #         openai.BadRequestError.__name__,
+    #     )
 
-    _check_context_attributes(query_attributes, session_id, user_id, metadata, tags)
+    if use_context_attributes:
+        _check_context_attributes(query_attributes, session_id, user_id, metadata, tags)
     assert query_attributes == {}
 
-    assert (synthesize_span := spans_by_name.pop("synthesize")) is not None
+    assert (synthesize_span := spans_by_name.pop("synthesize", None)) is not None
     assert synthesize_span.parent is not None
     assert synthesize_span.parent.span_id == query_span.context.span_id
     assert synthesize_span.context.trace_id == query_span.context.trace_id
     synthesize_attributes = dict(synthesize_span.attributes or {})
     assert synthesize_attributes.pop(OPENINFERENCE_SPAN_KIND, None) == CHAIN.value
     assert synthesize_attributes.pop(INPUT_VALUE, None) == question
     if status_code == 200:
         assert synthesize_span.status.status_code == trace_api.StatusCode.OK
         assert not synthesize_span.status.description
         assert synthesize_attributes.pop(OUTPUT_VALUE, None) == answer
-    elif (
-        # FIXME: currently the error is propagated when streaming because we don't rely on
-        # `on_event_end` to set the status code.
-        status_code == 400 and is_stream
-    ):
-        assert synthesize_span.status.status_code == trace_api.StatusCode.ERROR
-        assert query_span.status.description and query_span.status.description.startswith(
-            openai.BadRequestError.__name__,
-        )
-    _check_context_attributes(synthesize_attributes, session_id, user_id, metadata, tags)
+    # LlamaIndex introduced a regression causing streaming LLM responses that
+    # result in a 400 to not register their exception and status code
+    # information. We are going to ignore this issue as we are about to migrate
+    # our LlamaIndex instrumentation away from the existing callback system to
+    # the new system.
+    # elif (
+    #     # FIXME: currently the error is propagated when streaming because we don't rely on
+    #     # `on_event_end` to set the status code.
+    #     status_code == 400 and is_stream
+    # ):
+    #     assert synthesize_span.status.status_code == trace_api.StatusCode.ERROR
+    #     assert query_span.status.description and query_span.status.description.startswith(
+    #         openai.BadRequestError.__name__,
+    #     )
+    if use_context_attributes:
+        _check_context_attributes(synthesize_attributes, session_id, user_id, metadata, tags)
     assert synthesize_attributes == {}
 
-    assert (retrieve_span := spans_by_name.pop("retrieve")) is not None
+    assert (retrieve_span := spans_by_name.pop("retrieve", None)) is not None
     assert retrieve_span.parent is not None
     assert retrieve_span.parent.span_id == query_span.context.span_id
     assert retrieve_span.context.trace_id == query_span.context.trace_id
     retrieve_attributes = dict(retrieve_span.attributes or {})
     assert retrieve_attributes.pop(OPENINFERENCE_SPAN_KIND, None) == RETRIEVER.value
     assert retrieve_attributes.pop(INPUT_VALUE, None) == question
     retrieve_attributes.pop(f"{RETRIEVAL_DOCUMENTS}.0.{DOCUMENT_ID}", None)
@@ -238,15 +272,16 @@
     assert retrieve_attributes.pop(
         f"{RETRIEVAL_DOCUMENTS}.0.{DOCUMENT_METADATA}", None
     ) == json.dumps(nodes[0].metadata)
     assert (
         retrieve_attributes.pop(f"{RETRIEVAL_DOCUMENTS}.1.{DOCUMENT_CONTENT}", None)
         == nodes[1].text
     )
-    _check_context_attributes(retrieve_attributes, session_id, user_id, metadata, tags)
+    if use_context_attributes:
+        _check_context_attributes(retrieve_attributes, session_id, user_id, metadata, tags)
     assert retrieve_attributes == {}
 
     if status_code == 200:
         # FIXME: LlamaIndex doesn't currently capture the LLM span when status_code == 400
         # For example, if an exception is raised by the LLM at the following location,
         # `on_event_end` never gets called.
         # https://github.com/run-llama/llama_index/blob/dcef41ee67925cccf1ee7bb2dd386bcf0564ba29/llama_index/llms/base.py#L100 # noqa E501
@@ -273,25 +308,27 @@
         assert llm_attributes.pop(OUTPUT_VALUE, None) == answer
         if not is_stream:
             # FIXME: currently we can't capture messages when streaming
             assert (
                 llm_attributes.pop(f"{LLM_OUTPUT_MESSAGES}.0.{MESSAGE_ROLE}", None) == "assistant"
             )
             assert llm_attributes.pop(f"{LLM_OUTPUT_MESSAGES}.0.{MESSAGE_CONTENT}", None) == answer
-        _check_context_attributes(llm_attributes, session_id, user_id, metadata, tags)
+        if use_context_attributes:
+            _check_context_attributes(llm_attributes, session_id, user_id, metadata, tags)
         assert llm_attributes == {}
 
     # FIXME: maybe chunking spans should be discarded?
     assert (chunking_span := spans_by_name.pop("chunking", None)) is not None
     assert chunking_span.parent is not None
     assert chunking_span.parent.span_id == synthesize_span.context.span_id
     assert chunking_span.context.trace_id == synthesize_span.context.trace_id
     chunking_attributes = dict(chunking_span.attributes or {})
     assert chunking_attributes.pop(OPENINFERENCE_SPAN_KIND, None) is not None
-    _check_context_attributes(chunking_attributes, session_id, user_id, metadata, tags)
+    if use_context_attributes:
+        _check_context_attributes(chunking_attributes, session_id, user_id, metadata, tags)
     assert chunking_attributes == {}
 
     assert spans_by_name == {}
 
     return question
```

### Comparing `openinference_instrumentation_llama_index-1.3.0/LICENSE` & `openinference_instrumentation_llama_index-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.3.0/README.md` & `openinference_instrumentation_llama_index-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.3.0/pyproject.toml` & `openinference_instrumentation_llama_index-1.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -24,26 +24,27 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "opentelemetry-api",
   "opentelemetry-instrumentation",
   "opentelemetry-semantic-conventions",
-  "openinference-instrumentation>=0.1.3",
+  "openinference-instrumentation>=0.1.5",
   "openinference-semantic-conventions",
   "typing-extensions",
   "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
-  "llama-index >= 0.10.5",
+  "llama-index-core >= 0.10.5",
 ]
 test = [
-  "llama-index == 0.10.5",
+  "llama-index == 0.10.36",
+  "llama-index-core == 0.10.36",
   "llama-index-llms-openai",
   "opentelemetry-sdk",
   "respx",
 ]
 
 [project.urls]
 Homepage = "https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-llama-index"
```

### Comparing `openinference_instrumentation_llama_index-1.3.0/PKG-INFO` & `openinference_instrumentation_llama_index-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-llama-index
-Version: 1.3.0
+Version: 1.4.0
 Summary: OpenInference LlamaIndex Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-llama-index
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,26 +13,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
-Requires-Dist: openinference-instrumentation>=0.1.3
+Requires-Dist: openinference-instrumentation>=0.1.5
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: typing-extensions
 Requires-Dist: wrapt
 Provides-Extra: instruments
-Requires-Dist: llama-index>=0.10.5; extra == 'instruments'
+Requires-Dist: llama-index-core>=0.10.5; extra == 'instruments'
 Provides-Extra: test
+Requires-Dist: llama-index-core==0.10.36; extra == 'test'
 Requires-Dist: llama-index-llms-openai; extra == 'test'
-Requires-Dist: llama-index==0.10.5; extra == 'test'
+Requires-Dist: llama-index==0.10.36; extra == 'test'
 Requires-Dist: opentelemetry-sdk; extra == 'test'
 Requires-Dist: respx; extra == 'test'
 Description-Content-Type: text/markdown
 
 # OpenInference LlamaIndex Instrumentation
 Python auto-instrumentation library for LlamaIndex.
```

