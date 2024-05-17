# Comparing `tmp/langtrace_python_sdk-2.0.7.tar.gz` & `tmp/langtrace_python_sdk-2.0.8.tar.gz`

## Comparing `langtrace_python_sdk-2.0.7.tar` & `langtrace_python_sdk-2.0.8.tar`

### file list

```diff
@@ -1,131 +1,140 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     6724 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    37263 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/LICENSE
--rw-r--r--   0        0        0     8370 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     9582 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     7015 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     6839 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    26068 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5192 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3751 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    37263 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     4832 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     3883 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/types/__init__.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/prompt_registry.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/silently_fail.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/types.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/chroma/conftest.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/pinecone/conftest.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0   103821 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/pinecone/cassettes/test_query.yaml
+-rw-r--r--   0        0        0    38607 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/pinecone/cassettes/test_upsert.yaml
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/qdrant/conftest.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/src/tests/qdrant/test_qdrant.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/LICENSE
+-rw-r--r--   0        0        0     8740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/README.md
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.8/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.0.7/src/run_example.py` & `langtrace_python_sdk-2.0.8/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.0.8/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.0.8/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.0.8/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.0.8/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.0.8/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.0.8/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.0.8/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.0.8/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.0.8/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.0.8/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.0.8/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.0.8/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.0.8/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.0.8/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.0.8/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.8/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.0.8/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.0.8/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.0.8/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.0.8/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.8/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.0.8/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.0.8/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.0.8/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from langtrace_python_sdk import langtrace
 from langtrace_python_sdk.utils.with_root_span import with_langtrace_root_span
+from langtrace_python_sdk.utils.prompt_registry import get_prompt_from_registry
 
-__all__ = ["langtrace", "with_langtrace_root_span"]
+__all__ = ["langtrace", "with_langtrace_root_span", "get_prompt_from_registry"]
```

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/langtrace.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from opentelemetry import trace
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import (
     BatchSpanProcessor,
     ConsoleSpanExporter,
     SimpleSpanProcessor,
 )
+import sys
+from opentelemetry.sdk.resources import Resource
 
 from langtrace_python_sdk.extensions.langtrace_exporter import LangTraceExporter
 from langtrace_python_sdk.instrumentation.anthropic.instrumentation import (
     AnthropicInstrumentation,
 )
 from langtrace_python_sdk.instrumentation.chroma.instrumentation import (
     ChromaInstrumentation,
@@ -68,15 +70,15 @@
     api_key: str = None,
     batch: bool = True,
     write_spans_to_console: bool = False,
     custom_remote_exporter=None,
     api_host: Optional[str] = None,
     disable_instrumentations: Optional[DisableInstrumentations] = None,
 ):
-    provider = TracerProvider()
+    provider = TracerProvider(resource=Resource.create({"service.name": sys.argv[0]}))
 
     remote_write_exporter = (
         LangTraceExporter(api_key=api_key, api_host=api_host)
         if custom_remote_exporter is None
         else custom_remote_exporter
     )
     console_exporter = ConsoleSpanExporter()
```

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/types/__init__.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/types/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,7 +54,15 @@
     cost_table = OPENAI_COST_TABLE.get(model)
     if cost_table:
         return (
             cost_table["input"] * usage["prompt_tokens"]
             + cost_table["output"] * usage["completion_tokens"]
         ) / 1000
     return 0
+
+
+def set_span_attributes(span, name, value):
+    if value is not None:
+        if value != "":
+            span.set_attribute(name, value)
+    return
+
```

### Comparing `langtrace_python_sdk-2.0.7/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.0.8/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/conftest.py` & `langtrace_python_sdk-2.0.8/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/utils.py` & `langtrace_python_sdk-2.0.8/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.0.8/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.0.8/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.0.8/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.8/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.8/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.0.8/src/tests/langchain/test_langchain.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,82 @@
-from unittest.mock import MagicMock, patch, call
-from langtrace_python_sdk.constants.instrumentation.common import SERVICE_PROVIDERS
-from langtrace_python_sdk.constants.instrumentation.openai import APIS
-from opentelemetry.trace.status import StatusCode, Status
-from langtrace_python_sdk.instrumentation.chroma.patch import collection_patch
+import unittest
+from unittest.mock import MagicMock, call
+from langtrace_python_sdk.instrumentation.langchain.patch import generic_patch
 from opentelemetry.trace import SpanKind
+from opentelemetry.trace import get_tracer
+import importlib.metadata
+from langtrace_python_sdk.constants.instrumentation.openai import APIS
+from opentelemetry.trace.status import Status, StatusCode
 from tests.utils import common_setup
-import unittest
 import json
 
 
-class TestChromaPatch(unittest.TestCase):
-    data = {
-        "status": "success",
-    }
+class TestGenericPatch(unittest.TestCase):
+    data = {"key": "value"}
 
     def setUp(self):
-        self.chroma_mock, self.tracer, self.span = common_setup(
-            self.data, "chromadb.Collection.add"
-        )
-        self.wrapped_method = MagicMock(return_value="mocked method result")
-        self.instance = MagicMock()
-        self.instance.name = "aa"
+        self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
 
     def tearDown(self):
-        self.chroma_mock.stop()
+        # Clean up after each test case
+        pass
 
-    def test_collection_patch_success(self):
+    def test_generic_patch(self):
         # Arrange
-        traced_method = collection_patch("ADD", "1.2.3", self.tracer)
+        method_name = "example_method"
+        trace_output = False
+        trace_input = False  # Change as per your requirement
+        args = (1, 2, 3)
+        task = "split_text"
+        kwargs = {"key": "value"}
+        version = importlib.metadata.version("langchain")
 
         # Act
-        result = traced_method(self.wrapped_method, self.instance, (), {})
+        wrapped_function = generic_patch(
+            "langchain.text_splitter",
+            task,
+            self.tracer,
+            version,
+            trace_output,
+            trace_input,
+        )
+        result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
 
         # Assert
-        # Assert the result of the original method is returned
-        self.assertEqual(result, "mocked method result")
-
-        # Assert the span is started with the correct parameters
         self.assertTrue(
             self.tracer.start_as_current_span.called_once_with(
-                "chromadb.Collection.add", kind=SpanKind.CLIENT
+                method_name, kind=SpanKind.CLIENT
             )
         )
 
-        # Verify span attributes are set as expected
+        service_provider = "Langchain"
         expected_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
-            "langtrace.service.name": "Chroma",
-            "langtrace.service.type": "vectordb",
-            "langtrace.service.version": "1.2.3",
+            "langtrace.service.name": service_provider,
+            "langtrace.service.type": "framework",
+            "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
-            "db.system": "chromadb",
-            "db.operation": "add",
-            "db.collection.name": "aa",
+            "langchain.task.name": task,
         }
-        for key, value in expected_attributes.items():
-            self.span.set_attribute.assert_has_calls([call(key, value)], any_order=True)
+
+        self.assertTrue(
+            self.span.set_attribute.has_calls(
+                [call(key, value) for key, value in expected_attributes.items()],
+                any_order=True,
+            )
+        )
 
         actual_calls = self.span.set_attribute.call_args_list
 
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
 
-        # Assert the span status is set to OK
-        self.span.set_status.assert_called_with(StatusCode.OK)
+        self.assertEqual(self.span.set_status.call_count, 1)
+        self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
+
+        expected_result_data = {"key": "value"}
+
+        self.assertEqual(result.key, expected_result_data["key"])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.0.8/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.0.8/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.0.8/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.0.8/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.0.8/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.0.8/src/tests/langchain/test_langchain_community.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import unittest
-from unittest.mock import MagicMock, call
-from langtrace_python_sdk.instrumentation.langchain.patch import generic_patch
+from unittest.mock import MagicMock, Mock, patch, call
+from langtrace_python_sdk.instrumentation.langchain_community.patch import generic_patch
 from opentelemetry.trace import SpanKind
 from opentelemetry.trace import get_tracer
 import importlib.metadata
+import openai
 from langtrace_python_sdk.constants.instrumentation.openai import APIS
 from opentelemetry.trace.status import Status, StatusCode
-from tests.utils import common_setup
 import json
+from tests.utils import common_setup
 
 
 class TestGenericPatch(unittest.TestCase):
     data = {"key": "value"}
 
     def setUp(self):
         self.langchain_mock, self.tracer, self.span = common_setup(self.data, None)
@@ -20,23 +21,23 @@
         # Clean up after each test case
         pass
 
     def test_generic_patch(self):
         # Arrange
         method_name = "example_method"
         trace_output = False
-        trace_input = False  # Change as per your requirement
+        trace_input = False
         args = (1, 2, 3)
-        task = "split_text"
+        task = "vector_store"
         kwargs = {"key": "value"}
-        version = importlib.metadata.version("langchain")
+        version = importlib.metadata.version("langchain-community")
 
         # Act
         wrapped_function = generic_patch(
-            "langchain.text_splitter",
+            "langchain_community.vectorstores.faiss",
             task,
             self.tracer,
             version,
             trace_output,
             trace_input,
         )
         result = wrapped_function(self.langchain_mock, MagicMock(), args, kwargs)
@@ -44,15 +45,15 @@
         # Assert
         self.assertTrue(
             self.tracer.start_as_current_span.called_once_with(
                 method_name, kind=SpanKind.CLIENT
             )
         )
 
-        service_provider = "Langchain"
+        service_provider = "Langchain Community"
         expected_attributes = {
             "langtrace.sdk.name": "langtrace-python-sdk",
             "langtrace.service.name": service_provider,
             "langtrace.service.type": "framework",
             "langtrace.service.version": version,
             "langtrace.version": "1.0.0",
             "langchain.task.name": task,
@@ -70,13 +71,12 @@
         for key, value in expected_attributes.items():
             self.assertIn(call(key, value), actual_calls)
 
         self.assertEqual(self.span.set_status.call_count, 1)
         self.assertTrue(self.span.set_status.has_calls([call(Status(StatusCode.OK))]))
 
         expected_result_data = {"key": "value"}
-
         self.assertEqual(result.key, expected_result_data["key"])
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `langtrace_python_sdk-2.0.7/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.0.8/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.0.8/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.0.8/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.0.8/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.0.8/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/.gitignore` & `langtrace_python_sdk-2.0.8/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -148,13 +148,16 @@
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
+# Test artifcats
+chroma.sqlite3
+
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
```

### Comparing `langtrace_python_sdk-2.0.7/LICENSE` & `langtrace_python_sdk-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.7/README.md` & `langtrace_python_sdk-2.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -180,14 +180,23 @@
 
 @with_langtrace_root_span()
 def chat_completion():
    api_call1()
    api_call2()
 ```
 
+- `get_prompt_from_registry` - this function is designed to fetch the desired prompt from the `Prompt Registry`. You can pass two options for filtering `prompt_version` & `variables`.
+
+
+```python
+from langtrace_python_sdk import get_prompt_from_registry
+
+prompt = get_prompt_from_registry(<Registry ID>, options={"prompt_version": 1, "variables": {"foo": "bar"} })
+```
+
 ## Supported integrations
 
 Langtrace automatically captures traces from the following vendors:
 
 | Vendor       | Type            | Typescript SDK     | Python SDK         |
 | ------------ | --------------- | ------------------ | ------------------ |
 | OpenAI       | LLM             | :white_check_mark: | :white_check_mark: |
```

### Comparing `langtrace_python_sdk-2.0.7/pyproject.toml` & `langtrace_python_sdk-2.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,21 +34,23 @@
     "anthropic",
     "python-dotenv",
     "langchain",
     "langchain-openai",
     "llama-index",
     "langchain-openai",
     "chromadb",
-    "cohere"
+    "cohere",
+    "qdrant_client"
 ]
 
 test = [
     "pytest",
     "pytest-vcr",
-    "pytest-asyncio"
+    "pytest-asyncio",
+    "protobuf==3.20.0",
 ]
 
 
 
 [project.urls]
 Homepage = "https://github.com/Scale3-Labs/langtrace-python-sdk"
```

### Comparing `langtrace_python_sdk-2.0.7/PKG-INFO` & `langtrace_python_sdk-2.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.0.7
+Version: 2.0.8
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,17 @@
 Requires-Dist: chromadb; extra == 'dev'
 Requires-Dist: cohere; extra == 'dev'
 Requires-Dist: langchain; extra == 'dev'
 Requires-Dist: langchain-openai; extra == 'dev'
 Requires-Dist: llama-index; extra == 'dev'
 Requires-Dist: openai; extra == 'dev'
 Requires-Dist: python-dotenv; extra == 'dev'
+Requires-Dist: qdrant-client; extra == 'dev'
 Provides-Extra: test
+Requires-Dist: protobuf==3.20.0; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
 Requires-Dist: pytest-vcr; extra == 'test'
 Description-Content-Type: text/markdown
 
 # [Langtrace](https://www.langtrace.ai)
 
@@ -213,14 +215,23 @@
 
 @with_langtrace_root_span()
 def chat_completion():
    api_call1()
    api_call2()
 ```
 
+- `get_prompt_from_registry` - this function is designed to fetch the desired prompt from the `Prompt Registry`. You can pass two options for filtering `prompt_version` & `variables`.
+
+
+```python
+from langtrace_python_sdk import get_prompt_from_registry
+
+prompt = get_prompt_from_registry(<Registry ID>, options={"prompt_version": 1, "variables": {"foo": "bar"} })
+```
+
 ## Supported integrations
 
 Langtrace automatically captures traces from the following vendors:
 
 | Vendor       | Type            | Typescript SDK     | Python SDK         |
 | ------------ | --------------- | ------------------ | ------------------ |
 | OpenAI       | LLM             | :white_check_mark: | :white_check_mark: |
```

