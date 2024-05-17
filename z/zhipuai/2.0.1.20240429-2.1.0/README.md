# Comparing `tmp/zhipuai-2.0.1.20240429.tar.gz` & `tmp/zhipuai-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhipuai-2.0.1.20240429.tar", max compression
+gzip compressed data, was "zhipuai-2.1.0.tar", max compression
```

## Comparing `zhipuai-2.0.1.20240429.tar` & `zhipuai-2.1.0.tar`

### file list

```diff
@@ -1,51 +1,61 @@
--rw-r--r--   0        0        0     7810 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/README.md
--rw-r--r--   0        0        0     3267 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/pyproject.toml
--rw-r--r--   0        0        0      359 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/__init__.py
--rw-r--r--   0        0        0       23 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/__version__.py
--rw-r--r--   0        0        0     2435 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/_client.py
--rw-r--r--   0        0        0      358 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/__init__.py
--rw-r--r--   0        0        0      200 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/__init__.py
--rw-r--r--   0        0        0     3285 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/async_completions.py
--rw-r--r--   0        0        0      464 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/chat.py
--rw-r--r--   0        0        0     4591 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/completions.py
--rw-r--r--   0        0        0     1757 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/embeddings.py
--rw-r--r--   0        0        0     2422 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/files.py
--rw-r--r--   0        0        0      188 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/__init__.py
--rw-r--r--   0        0        0      413 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0       48 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/jobs/__init__.py
--rw-r--r--   0        0        0     5537 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/jobs/jobs.py
--rw-r--r--   0        0        0       77 2024-04-30 05:57:30.368182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/models/__init__.py
--rw-r--r--   0        0        0     1309 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py
--rw-r--r--   0        0        0     1948 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/api_resource/images.py
--rw-r--r--   0        0        0     2040 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/__init__.py
--rw-r--r--   0        0        0      406 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_api.py
--rw-r--r--   0        0        0     6405 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_compat.py
--rw-r--r--   0        0        0    13547 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_models.py
--rw-r--r--   0        0        0     4551 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_base_type.py
--rw-r--r--   0        0        0     2230 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_errors.py
--rw-r--r--   0        0        0     1384 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_files.py
--rw-r--r--   0        0        0    22877 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_http_client.py
--rw-r--r--   0        0        0      713 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_jwt_token.py
--rw-r--r--   0        0        0     3349 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_request_opt.py
--rw-r--r--   0        0        0     3606 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_response.py
--rw-r--r--   0        0        0     4085 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_sse_client.py
--rw-r--r--   0        0        0     1451 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_utils/__init__.py
--rw-r--r--   0        0        0     3858 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_utils/_typing.py
--rw-r--r--   0        0        0    11363 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/_utils/_utils.py
--rw-r--r--   0        0        0     2618 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/core/logs.py
--rw-r--r--   0        0        0        0 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/__init__.py
--rw-r--r--   0        0        0      568 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/async_chat_completion.py
--rw-r--r--   0        0        0      859 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1249 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      171 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completions_create_param.py
--rw-r--r--   0        0        0      426 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/embeddings.py
--rw-r--r--   0        0        0      550 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/file_object.py
--rw-r--r--   0        0        0      244 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     1005 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0     1064 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0      339 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0       53 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/models/__init__.py
--rw-r--r--   0        0        0      456 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/models/fine_tuned_models.py
--rw-r--r--   0        0        0      374 2024-04-30 05:57:30.372182 zhipuai-2.0.1.20240429/zhipuai/types/image.py
--rw-r--r--   0        0        0     8547 1970-01-01 00:00:00.000000 zhipuai-2.0.1.20240429/PKG-INFO
+-rw-r--r--   0        0        0     8583 2024-05-17 12:31:23.820003 zhipuai-2.1.0/README.md
+-rw-r--r--   0        0        0     3275 2024-05-17 12:31:23.820003 zhipuai-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      359 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/__version__.py
+-rw-r--r--   0        0        0     2822 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/_client.py
+-rw-r--r--   0        0        0      412 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/__init__.py
+-rw-r--r--   0        0        0     5055 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/batches.py
+-rw-r--r--   0        0        0      200 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/__init__.py
+-rw-r--r--   0        0        0     3285 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/async_completions.py
+-rw-r--r--   0        0        0      464 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/chat.py
+-rw-r--r--   0        0        0     4503 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/chat/completions.py
+-rw-r--r--   0        0        0     1757 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/embeddings.py
+-rw-r--r--   0        0        0     4868 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/files.py
+-rw-r--r--   0        0        0      188 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/__init__.py
+-rw-r--r--   0        0        0      413 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0       48 2024-05-17 12:31:23.820003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/jobs/__init__.py
+-rw-r--r--   0        0        0     5537 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/jobs/jobs.py
+-rw-r--r--   0        0        0       77 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/models/__init__.py
+-rw-r--r--   0        0        0     1309 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py
+-rw-r--r--   0        0        0     1948 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/api_resource/images.py
+-rw-r--r--   0        0        0     2134 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/__init__.py
+-rw-r--r--   0        0        0      455 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_api.py
+-rw-r--r--   0        0        0     6405 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_compat.py
+-rw-r--r--   0        0        0    13647 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_models.py
+-rw-r--r--   0        0        0     4901 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_base_type.py
+-rw-r--r--   0        0        0      583 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_constants.py
+-rw-r--r--   0        0        0     2256 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_errors.py
+-rw-r--r--   0        0        0     1586 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_files.py
+-rw-r--r--   0        0        0    30519 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_http_client.py
+-rw-r--r--   0        0        0      774 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_jwt_token.py
+-rw-r--r--   0        0        0    14681 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_legacy_response.py
+-rw-r--r--   0        0        0     3443 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_request_opt.py
+-rw-r--r--   0        0        0    14044 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_response.py
+-rw-r--r--   0        0        0     6582 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_sse_client.py
+-rw-r--r--   0        0        0     1675 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/__init__.py
+-rw-r--r--   0        0        0    13099 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/_transform.py
+-rw-r--r--   0        0        0     3858 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/_typing.py
+-rw-r--r--   0        0        0    11363 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/_utils/_utils.py
+-rw-r--r--   0        0        0     2618 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/logs.py
+-rw-r--r--   0        0        0     1562 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/core/pagination.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/__init__.py
+-rw-r--r--   0        0        0     2427 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch.py
+-rw-r--r--   0        0        0     1096 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_create_params.py
+-rw-r--r--   0        0        0      488 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_error.py
+-rw-r--r--   0        0        0      536 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_list_params.py
+-rw-r--r--   0        0        0      298 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/batch_request_counts.py
+-rw-r--r--   0        0        0        0 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/__init__.py
+-rw-r--r--   0        0        0      568 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/async_chat_completion.py
+-rw-r--r--   0        0        0      859 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1272 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      171 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/chat/chat_completions_create_param.py
+-rw-r--r--   0        0        0      426 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/embeddings.py
+-rw-r--r--   0        0        0      550 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/file_object.py
+-rw-r--r--   0        0        0      244 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0     1064 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0      339 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0       53 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/models/__init__.py
+-rw-r--r--   0        0        0      456 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/fine_tuning/models/fine_tuned_models.py
+-rw-r--r--   0        0        0      374 2024-05-17 12:31:23.824003 zhipuai-2.1.0/zhipuai/types/image.py
+-rw-r--r--   0        0        0     9311 1970-01-01 00:00:00.000000 zhipuai-2.1.0/PKG-INFO
```

### Comparing `zhipuai-2.0.1.20240429/README.md` & `zhipuai-2.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,33 @@
 ```python
 from zhipuai import ZhipuAI
 
 client = ZhipuAI(
     api_key="", # 填写您的 APIKey
 ) 
 ```
+### 客户端网络链接配置
+在`core/_http_client.py`中，可以配置网络链接的超时时间，重试次数，限制等参数
+```python
+# 通过 `Timeout` 控制接口`connect` 和 `read` 超时时间，默认为`timeout=300.0, connect=8.0`
+ZHIPUAI_DEFAULT_TIMEOUT = httpx.Timeout(timeout=300.0, connect=8.0)
+# 通过 `retry` 参数控制重试次数，默认为3次
+ZHIPUAI_DEFAULT_MAX_RETRIES = 3
+# 通过 `Limits` 控制最大连接数和保持连接数，默认为`max_connections=50, max_keepalive_connections=10`
+ZHIPUAI_DEFAULT_LIMITS = httpx.Limits(max_connections=50, max_keepalive_connections=10)
+ 
+```
+同样在`ZhipuAI`入参中可以配置
+```python
+client = ZhipuAI(
+    timeout= httpx.Timeout(timeout=300.0, connect=8.0),
+    max_retries=3,
+)
+```
+
 
 ### 同步调用
 
 ```python
 from zhipuai import ZhipuAI 
  
 client = ZhipuAI()  # 填写您自己的APIKey
```

### Comparing `zhipuai-2.0.1.20240429/pyproject.toml` & `zhipuai-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zhipuai"
-version = "2.0.1.20240429"
+version = "2.1.0"
 description = "A SDK library for accessing big model apis from ZhipuAI"
 authors = ["Zhipu AI"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7.1,<3.12,!=3.9.7 "
 httpx = ">=0.23.0"
@@ -27,14 +27,15 @@
 pytest-asyncio = { version = "^0.23.2", python = "^3.8" }
 lark = "^1.1.5"
 pandas = { version = "^2.0.0", python = "^3.8" }
 pytest-mock = "^3.10.0"
 pytest-socket = "^0.6.0"
 syrupy = { version = "^4.0.2", python = ">=3.8.1,<3.9.7 || >3.9.7,<3.12" }
 requests-mock = "^1.11.0"
+respx = "0.21.1"
 
 [tool.poetry.group.test_langchain.dependencies]
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-dotenv = "^0.5.2"
 duckdb-engine = "^0.9.2"
 pytest-watcher = "^0.2.6"
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/_client.py` & `zhipuai-2.1.0/zhipuai/_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,56 +13,64 @@
 import httpx
 from httpx import Timeout
 
 
 class ZhipuAI(HttpClient):
     chat: api_resource.chat.Chat
     api_key: str
+    _disable_token_cache: bool = True
 
     def __init__(
             self,
             *,
             api_key: str | None = None,
             base_url: str | httpx.URL | None = None,
             timeout: Union[float, Timeout, None, NotGiven] = NOT_GIVEN,
             max_retries: int = ZHIPUAI_DEFAULT_MAX_RETRIES,
             http_client: httpx.Client | None = None,
-            custom_headers: Mapping[str, str] | None = None
+            custom_headers: Mapping[str, str] | None = None,
+            disable_token_cache: bool = True,
+            _strict_response_validation: bool = False,
     ) -> None:
         if api_key is None:
             api_key = os.environ.get("ZHIPUAI_API_KEY")
         if api_key is None:
             raise ZhipuAIError("未提供api_key，请通过参数或环境变量提供")
         self.api_key = api_key
+        self._disable_token_cache = disable_token_cache
 
         if base_url is None:
             base_url = os.environ.get("ZHIPUAI_BASE_URL")
         if base_url is None:
             base_url = f"https://open.bigmodel.cn/api/paas/v4"
         from .__version__ import __version__
         super().__init__(
             version=__version__,
             base_url=base_url,
             max_retries=max_retries,
             timeout=timeout,
             custom_httpx_client=http_client,
             custom_headers=custom_headers,
+            _strict_response_validation=_strict_response_validation,
         )
         self.chat = api_resource.chat.Chat(self)
         self.images = api_resource.images.Images(self)
         self.embeddings = api_resource.embeddings.Embeddings(self)
         self.files = api_resource.files.Files(self)
         self.fine_tuning = api_resource.fine_tuning.FineTuning(self)
+        self.batches = api_resource.Batches(self)
 
     @property
     @override
     def auth_headers(self) -> dict[str, str]:
         api_key = self.api_key
-        # return {"Authorization": f"{_jwt_token.generate_token(api_key)}"}
-        return {"Authorization": f"{api_key}"}
+        if self._disable_token_cache:
+            return {"Authorization": f"Bearer {api_key}"}
+        else:
+            return {"Authorization": f"Bearer {_jwt_token.generate_token(api_key)}"}
 
     def __del__(self) -> None:
         if (not hasattr(self, "_has_custom_http_client")
                 or not hasattr(self, "close")
                 or not hasattr(self, "_client")):
             # if the '__init__' method raised an error, self would not have client attr
             return
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/async_completions.py` & `zhipuai-2.1.0/zhipuai/api_resource/chat/async_completions.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/api_resource/chat/completions.py` & `zhipuai-2.1.0/zhipuai/api_resource/chat/completions.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,35 +40,34 @@
             tools: Optional[object] | NotGiven = NOT_GIVEN,
             tool_choice: str | NotGiven = NOT_GIVEN,
             meta: Optional[Dict[str,str]] | NotGiven = NOT_GIVEN,
             extra_headers: Headers | None = None,
             extra_body: Body | None = None,
             timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> Completion | StreamResponse[ChatCompletionChunk]:
-        logger.info(f"temperature:{temperature}, top_p:{top_p}")
+        logger.debug(f"temperature:{temperature}, top_p:{top_p}")
         if temperature is not None and temperature != NOT_GIVEN:
 
             if temperature <= 0:
                 do_sample = False
                 temperature = 0.01
-                logger.warning("temperature:取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
+                # logger.warning("temperature:取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
             if temperature >= 1:
-                do_sample = False
                 temperature = 0.99
-                logger.warning("temperature:取值范围是：(0.0, 1.0) 开区间，do_sample重写为:false（参数top_p temperture不生效）")
+                # logger.warning("temperature:取值范围是：(0.0, 1.0) 开区间")
         if top_p is not None and top_p != NOT_GIVEN:
 
             if top_p >= 1:
                 top_p = 0.99
-                logger.warning("top_p:取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
+                # logger.warning("top_p:取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
             if top_p <= 0:
                 top_p = 0.01
-                logger.warning("top_p:取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
+                # logger.warning("top_p:取值范围是：(0.0, 1.0) 开区间，不能等于 0 或 1")
 
-        logger.info(f"temperature:{temperature}, top_p:{top_p}")
+        logger.debug(f"temperature:{temperature}, top_p:{top_p}")
         if isinstance(messages, List):
             for item in messages:
                 if item.get('content'):
                     item['content'] = self._drop_prefix_image_data(item['content'])
 
         return self._post(
             "/chat/completions",
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/api_resource/embeddings.py` & `zhipuai-2.1.0/zhipuai/api_resource/embeddings.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/jobs/jobs.py` & `zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py` & `zhipuai-2.1.0/zhipuai/api_resource/fine_tuning/models/fine_tuned_models.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/api_resource/images.py` & `zhipuai-2.1.0/zhipuai/api_resource/images.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/__init__.py` & `zhipuai-2.1.0/zhipuai/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,24 +40,34 @@
     APIResponseError,
     APIResponseValidationError,
     APIConnectionError,
     APITimeoutError,
 )
 from ._http_client import (
     make_request_options,
-    HttpClient,
-    ZHIPUAI_DEFAULT_TIMEOUT,
-    ZHIPUAI_DEFAULT_MAX_RETRIES,
-    ZHIPUAI_DEFAULT_LIMITS,
+    HttpClient
 
 )
-from ._utils import (is_list, is_mapping, parse_date, parse_datetime, is_given)
+from ._utils import (
+    is_list,
+    is_mapping,
+    parse_date,
+    parse_datetime,
+    is_given,
+    maybe_transform
+)
 
 from ._sse_client import StreamResponse
 
+from ._constants import (
+
+    ZHIPUAI_DEFAULT_TIMEOUT,
+    ZHIPUAI_DEFAULT_MAX_RETRIES,
+    ZHIPUAI_DEFAULT_LIMITS,
+)
 __all__ = [
     "BaseModel",
     "construct_type",
     "BaseAPI",
     "NOT_GIVEN",
     "Headers",
     "NotGiven",
@@ -99,11 +109,12 @@
     "ZHIPUAI_DEFAULT_LIMITS",
 
     "is_list",
     "is_mapping",
     "parse_date",
     "parse_datetime",
     "is_given",
+    "maybe_transform",
 
     "StreamResponse",
 
 ]
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_base_compat.py` & `zhipuai-2.1.0/zhipuai/core/_base_compat.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_base_models.py` & `zhipuai-2.1.0/zhipuai/core/_base_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,21 +34,21 @@
     field_get_default,
 )
 
 __all__ = ["BaseModel", "GenericModel"]
 
 _T = TypeVar("_T")
 
+
 @runtime_checkable
 class _ConfigProtocol(Protocol):
     allow_population_by_field_name: bool
 
 
 class BaseModel(pydantic.BaseModel):
-
     if PYDANTIC_V2:
         model_config: ClassVar[ConfigDict] = ConfigDict(extra="allow")
     else:
 
         @property
         @override
         def model_fields_set(self) -> set[str]:
@@ -64,17 +64,17 @@
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'  # type: ignore[misc]
 
     # Override the 'construct' method in a way that supports recursive parsing without validation.
     # Based on https://github.com/samuelcolvin/pydantic/issues/1168#issuecomment-817742836.
     @classmethod
     @override
     def construct(
-        cls: Type[ModelT],
-        _fields_set: set[str] | None = None,
-        **values: object,
+            cls: Type[ModelT],
+            _fields_set: set[str] | None = None,
+            **values: object,
     ) -> ModelT:
         m = cls.__new__(cls)
         fields_values: dict[str, object] = {}
 
         config = get_model_config(cls)
         populate_by_name = (
             config.allow_population_by_field_name
@@ -132,25 +132,25 @@
         # we define aliases for some of the new pydantic v2 methods so
         # that we can just document these methods without having to specify
         # a specific pydantic version as some users may not know which
         # pydantic version they are currently using
 
         @override
         def model_dump(
-            self,
-            *,
-            mode: Literal["json", "python"] | str = "python",
-            include: IncEx = None,
-            exclude: IncEx = None,
-            by_alias: bool = False,
-            exclude_unset: bool = False,
-            exclude_defaults: bool = False,
-            exclude_none: bool = False,
-            round_trip: bool = False,
-            warnings: bool = True,
+                self,
+                *,
+                mode: Literal["json", "python"] | str = "python",
+                include: IncEx = None,
+                exclude: IncEx = None,
+                by_alias: bool = False,
+                exclude_unset: bool = False,
+                exclude_defaults: bool = False,
+                exclude_none: bool = False,
+                round_trip: bool = False,
+                warnings: bool = True,
         ) -> dict[str, Any]:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump
 
             Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
             Args:
                 mode: The mode in which `to_python` should run.
@@ -181,25 +181,25 @@
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
                 exclude_none=exclude_none,
             )
 
         @override
         def model_dump_json(
-            self,
-            *,
-            indent: int | None = None,
-            include: IncEx = None,
-            exclude: IncEx = None,
-            by_alias: bool = False,
-            exclude_unset: bool = False,
-            exclude_defaults: bool = False,
-            exclude_none: bool = False,
-            round_trip: bool = False,
-            warnings: bool = True,
+                self,
+                *,
+                indent: int | None = None,
+                include: IncEx = None,
+                exclude: IncEx = None,
+                by_alias: bool = False,
+                exclude_unset: bool = False,
+                exclude_defaults: bool = False,
+                exclude_none: bool = False,
+                round_trip: bool = False,
+                warnings: bool = True,
         ) -> str:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump_json
 
             Generates a JSON representation of the model using Pydantic's `to_json` method.
 
             Args:
                 indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
@@ -345,15 +345,14 @@
 if TYPE_CHECKING:
     GenericModel = BaseModel
 else:
 
     class GenericModel(BaseGenericModel, BaseModel):
         pass
 
-
 if PYDANTIC_V2:
     from pydantic import TypeAdapter
 
 
     def _validate_non_model_type(*, type_: type[_T], value: object) -> _T:
         return TypeAdapter(type_).validate_python(value)
 
@@ -365,18 +364,19 @@
 
            For example:
            ```py
            validated = RootModel[int](__root__="5").__root__
            # validated: 5
            ```
            """
+
         def __init__(self, type_: Type[_T]):
             self.type_ = type_
 
         def validate_python(self, value: Any) -> _T:
             if not isinstance(value, self.type_):
                 raise ValueError(f"Invalid type: {value} is not of type {self.type_}")
             return value
 
+
     def _validate_non_model_type(*, type_: type[_T], value: object) -> _T:
         return TypeAdapter(type_).validate_python(value)
-
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_base_type.py` & `zhipuai-2.1.0/zhipuai/core/_base_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Callable,
     Optional,
     Sequence,
 )
 import pydantic
 from httpx import Response
 from typing_extensions import Literal, Protocol, TypeAlias, TypedDict, override, runtime_checkable
+
 Query = Mapping[str, object]
 Body = object
 AnyMapping = Mapping[str, object]
 PrimitiveData = Union[str, int, float, bool, None]
 Data = Union[PrimitiveData, List[Any], Tuple[Any], "Mapping[str, Any]"]
 ModelT = TypeVar("ModelT", bound=pydantic.BaseModel)
 _T = TypeVar("_T")
@@ -133,33 +134,42 @@
 class _GenericAlias(Protocol):
     __origin__: type[object]
 
 
 class HttpxSendArgs(TypedDict, total=False):
     auth: httpx.Auth
 
+
 # for user input files
 if TYPE_CHECKING:
+    Base64FileInput = Union[IO[bytes], PathLike[str]]
     FileContent = Union[IO[bytes], bytes, PathLike[str]]
 else:
+    Base64FileInput = Union[IO[bytes], PathLike]
     FileContent = Union[IO[bytes], bytes, PathLike]
 
 FileTypes = Union[
-    FileContent,  # file content
-    Tuple[str, FileContent],  # (filename, file)
-    Tuple[str, FileContent, str],  # (filename, file , content_type)
-    Tuple[str, FileContent, str, Mapping[str, str]],  # (filename, file , content_type, headers)
+    # file (or bytes)
+    FileContent,
+        # (filename, file (or bytes))
+    Tuple[Optional[str], FileContent],
+        # (filename, file (or bytes), content_type)
+    Tuple[Optional[str], FileContent, Optional[str]],
+        # (filename, file (or bytes), content_type, headers)
+    Tuple[Optional[str], FileContent, Optional[str], Mapping[str, str]],
 ]
-
 RequestFiles = Union[Mapping[str, FileTypes], Sequence[Tuple[str, FileTypes]]]
 
-# for httpx client supported files
-
+# duplicate of the above but without our custom file support
 HttpxFileContent = Union[bytes, IO[bytes]]
 HttpxFileTypes = Union[
-    FileContent,  # file content
-    Tuple[str, HttpxFileContent],  # (filename, file)
-    Tuple[str, HttpxFileContent, str],  # (filename, file , content_type)
-    Tuple[str, HttpxFileContent, str, Mapping[str, str]],  # (filename, file , content_type, headers)
+    # file (or bytes)
+    HttpxFileContent,
+        # (filename, file (or bytes))
+    Tuple[Optional[str], HttpxFileContent],
+        # (filename, file (or bytes), content_type)
+    Tuple[Optional[str], HttpxFileContent, Optional[str]],
+        # (filename, file (or bytes), content_type, headers)
+    Tuple[Optional[str], HttpxFileContent, Optional[str], Mapping[str, str]],
 ]
 
 HttpxRequestFiles = Union[Mapping[str, HttpxFileTypes], Sequence[Tuple[str, HttpxFileTypes]]]
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_errors.py` & `zhipuai-2.1.0/zhipuai/core/_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     "APIAuthenticationError",
     "APIReachLimitError",
     "APIInternalError",
     "APIServerFlowExceedError",
     "APIResponseError",
     "APIResponseValidationError",
     "APITimeoutError",
+    "APIConnectionError",
 ]
 
 
 class ZhipuAIError(Exception):
     def __init__(self, message: str, ) -> None:
         super().__init__(message)
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_files.py` & `zhipuai-2.1.0/zhipuai/core/_files.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from __future__ import annotations
 
 import io
 import os
 from pathlib import Path
 from typing import Mapping, Sequence
+from typing_extensions import TypeGuard
 
 from ._base_type import (
     FileTypes,
     HttpxFileTypes,
     HttpxRequestFiles,
     RequestFiles,
+    Base64FileInput,
 )
 
 
+def is_base64_file_input(obj: object) -> TypeGuard[Base64FileInput]:
+    return isinstance(obj, io.IOBase) or isinstance(obj, os.PathLike)
+
+
 def is_file_content(obj: object) -> bool:
     return isinstance(obj, (bytes, tuple, io.IOBase, os.PathLike))
 
 
 def _transform_file(file: FileTypes) -> HttpxFileTypes:
     if is_file_content(file):
         if isinstance(file, os.PathLike):
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_http_client.py` & `zhipuai-2.1.0/zhipuai/core/_http_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,244 @@
 # -*- coding:utf-8 -*-
 from __future__ import annotations
 
 import inspect
+import warnings
 from typing import (
     Any,
     Type,
     Union,
     cast,
     Mapping,
     TypeVar,
     Dict,
-    overload
+    overload, Optional, Literal, Generic, Iterator, TYPE_CHECKING
 )
 
 from random import random
 import time
 import httpx
 import pydantic
 from httpx import URL, Timeout
 
-from . import _errors
+from . import _errors, get_origin
+from ._base_compat import model_copy
 from ._base_type import (
     NotGiven,
     ResponseT,
     Body,
     Headers,
     NOT_GIVEN,
     RequestFiles,
     Query,
     Data,
     Omit,
     AnyMapping,
     ModelBuilderProtocol,
-    HttpxSendArgs,
+    HttpxSendArgs, PostParser,
 )
+from ._constants import ZHIPUAI_DEFAULT_MAX_RETRIES, ZHIPUAI_DEFAULT_LIMITS, ZHIPUAI_DEFAULT_TIMEOUT, \
+    INITIAL_RETRY_DELAY, MAX_RETRY_DELAY, RAW_RESPONSE_HEADER
 from ._errors import APIResponseValidationError, APIStatusError, APITimeoutError, APIConnectionError
 from ._files import make_httpx_files
 from ._request_opt import FinalRequestOptions, UserRequestInput
-from ._response import HttpResponse
+from ._response import BaseAPIResponse, APIResponse, extract_response_type
 from ._sse_client import StreamResponse
 from ._utils import flatten, is_mapping, is_given
-from ._base_models import construct_type
+from ._base_models import construct_type, GenericModel, validate_type
 import logging
+
+
+log: logging.Logger = logging.getLogger(__name__)
+
+# TODO: make base page type vars covariant
+SyncPageT = TypeVar("SyncPageT", bound="BaseSyncPage[Any]")
+# AsyncPageT = TypeVar("AsyncPageT", bound="BaseAsyncPage[Any]")
+
 _T = TypeVar("_T")
 _T_co = TypeVar("_T_co", covariant=True)
 
-log: logging.Logger = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    from httpx._config import DEFAULT_TIMEOUT_CONFIG as HTTPX_DEFAULT_TIMEOUT
+else:
+    try:
+        from httpx._config import DEFAULT_TIMEOUT_CONFIG as HTTPX_DEFAULT_TIMEOUT
+    except ImportError:
+        # taken from https://github.com/encode/httpx/blob/3ba5fe0d7ac70222590e759c31442b1cab263791/httpx/_config.py#L366
+        HTTPX_DEFAULT_TIMEOUT = Timeout(5.0)
 
 
 headers = {
     "Accept": "application/json",
     "Content-Type": "application/json; charset=UTF-8",
 }
 
 
-from httpx._config import DEFAULT_TIMEOUT_CONFIG as HTTPX_DEFAULT_TIMEOUT
-RAW_RESPONSE_HEADER = "X-Stainless-Raw-Response"
-ZHIPUAI_DEFAULT_TIMEOUT = httpx.Timeout(timeout=300.0, connect=8.0)
-ZHIPUAI_DEFAULT_MAX_RETRIES = 3
-ZHIPUAI_DEFAULT_LIMITS = httpx.Limits(max_connections=50, max_keepalive_connections=10)
 
-INITIAL_RETRY_DELAY = 0.5
-MAX_RETRY_DELAY = 8.0
+class PageInfo:
+    """Stores the necessary information to build the request to retrieve the next page.
+
+    Either `url` or `params` must be set.
+    """
+
+    url: URL | NotGiven
+    params: Query | NotGiven
+
+    @overload
+    def __init__(
+            self,
+            *,
+            url: URL,
+    ) -> None:
+        ...
+
+    @overload
+    def __init__(
+            self,
+            *,
+            params: Query,
+    ) -> None:
+        ...
+
+    def __init__(
+            self,
+            *,
+            url: URL | NotGiven = NOT_GIVEN,
+            params: Query | NotGiven = NOT_GIVEN,
+    ) -> None:
+        self.url = url
+        self.params = params
+
+
+class BasePage(GenericModel, Generic[_T]):
+    """
+    Defines the core interface for pagination.
+
+    Type Args:
+        ModelT: The pydantic model that represents an item in the response.
+
+    Methods:
+        has_next_page(): Check if there is another page available
+        next_page_info(): Get the necessary information to make a request for the next page
+    """
+
+    _options: FinalRequestOptions = pydantic.PrivateAttr()
+    _model: Type[_T] = pydantic.PrivateAttr()
+
+    def has_next_page(self) -> bool:
+        items = self._get_page_items()
+        if not items:
+            return False
+        return self.next_page_info() is not None
+
+    def next_page_info(self) -> Optional[PageInfo]:
+        ...
+
+    def _get_page_items(self) -> Iterable[_T]:  # type: ignore[empty-body]
+        ...
+
+    def _params_from_url(self, url: URL) -> httpx.QueryParams:
+        # TODO: do we have to preprocess params here?
+        return httpx.QueryParams(cast(Any, self._options.params)).merge(url.params)
+
+    def _info_to_options(self, info: PageInfo) -> FinalRequestOptions:
+        options = model_copy(self._options)
+        options._strip_raw_response_header()
+
+        if not isinstance(info.params, NotGiven):
+            options.params = {**options.params, **info.params}
+            return options
+
+        if not isinstance(info.url, NotGiven):
+            params = self._params_from_url(info.url)
+            url = info.url.copy_with(params=params)
+            options.params = dict(url.params)
+            options.url = str(url)
+            return options
+
+        raise ValueError("Unexpected PageInfo state")
+
+
+class BaseSyncPage(BasePage[_T], Generic[_T]):
+    _client: HttpClient = pydantic.PrivateAttr()
+
+    def _set_private_attributes(
+            self,
+            client: HttpClient,
+            model: Type[_T],
+            options: FinalRequestOptions,
+    ) -> None:
+        self._model = model
+        self._client = client
+        self._options = options
+
+    # Pydantic uses a custom `__iter__` method to support casting BaseModels
+    # to dictionaries. e.g. dict(model).
+    # As we want to support `for item in page`, this is inherently incompatible
+    # with the default pydantic behaviour. It is not possible to support both
+    # use cases at once. Fortunately, this is not a big deal as all other pydantic
+    # methods should continue to work as expected as there is an alternative method
+    # to cast a model to a dictionary, model.dict(), which is used internally
+    # by pydantic.
+    def __iter__(self) -> Iterator[_T]:  # type: ignore
+        for page in self.iter_pages():
+            for item in page._get_page_items():
+                yield item
+
+    def iter_pages(self: SyncPageT) -> Iterator[SyncPageT]:
+        page = self
+        while True:
+            yield page
+            if page.has_next_page():
+                page = page.get_next_page()
+            else:
+                return
+
+    def get_next_page(self: SyncPageT) -> SyncPageT:
+        info = self.next_page_info()
+        if not info:
+            raise RuntimeError(
+                "No next page expected; please check `.has_next_page()` before calling `.get_next_page()`."
+            )
+
+        options = self._info_to_options(info)
+        return self._client._request_api_list(self._model, page=self.__class__, options=options)
+
 
 class HttpClient:
     _client: httpx.Client
     _version: str
     _base_url: URL
     max_retries: int
     timeout: Union[float, Timeout, None]
     _limits: httpx.Limits
     _has_custom_http_client: bool
-    _default_stream_cls: type[StreamResponse[Any]] | None = None
+    _default_stream_cls: Type[StreamResponse[Any]] | None = None
+
+    _strict_response_validation: bool
 
     def __init__(
             self,
             *,
             version: str,
             base_url: URL,
+            _strict_response_validation: bool,
             max_retries: int = ZHIPUAI_DEFAULT_MAX_RETRIES,
             timeout: Union[float, Timeout, None],
-            limits: Limits | None = None,
+            limits: httpx.Limits | None = None,
             custom_httpx_client: httpx.Client | None = None,
             custom_headers: Mapping[str, str] | None = None,
     ) -> None:
         if limits is not None:
             warnings.warn(
                 "The `connection_pool_limits` argument is deprecated. The `http_client` argument should be passed instead",
                 category=DeprecationWarning,
                 stacklevel=3,
             )
-            if http_client is not None:
+            if custom_httpx_client is not None:
                 raise ValueError("The `http_client` argument is mutually exclusive with `connection_pool_limits`")
         else:
             limits = ZHIPUAI_DEFAULT_LIMITS
 
         if not is_given(timeout):
             if custom_httpx_client and custom_httpx_client.timeout != HTTPX_DEFAULT_TIMEOUT:
                 timeout = custom_httpx_client.timeout
@@ -111,14 +255,15 @@
         )
         self._version = version
         url = URL(url=base_url)
         if not url.raw_path.endswith(b"/"):
             url = url.copy_with(raw_path=url.raw_path + b"/")
         self._base_url = url
         self._custom_headers = custom_headers or {}
+        self._strict_response_validation = _strict_response_validation
 
     def _prepare_url(self, url: str) -> URL:
 
         sub_url = URL(url)
         if sub_url.is_relative_url:
             request_raw_url = self._base_url.raw_path + sub_url.raw_path.lstrip(b"/")
             return self._base_url.copy_with(raw_path=request_raw_url)
@@ -133,14 +278,15 @@
                 "Content-Type": "application/json; charset=UTF-8",
                 "ZhipuAI-SDK-Ver": self._version,
                 "source_type": "zhipu-sdk-python",
                 "x-request-sdk": "zhipu-sdk-python",
                 **self.auth_headers,
                 **self._custom_headers,
             }
+
     @property
     def custom_auth(self) -> httpx.Auth | None:
         return None
 
     @property
     def auth_headers(self):
         return {}
@@ -256,51 +402,36 @@
         serialized: dict[str, object] = {}
         for key, value in items:
             if key in serialized:
                 raise ValueError(f"存在重复的键: {key};")
             serialized[key] = value
         return serialized
 
-    def _parse_response(
-            self,
-            *,
-            cast_type: Type[ResponseT],
-            response: httpx.Response,
-            stream: bool,
-            options: FinalRequestOptions,
-            stream_cls: type[StreamResponse[Any]] | None = None,
-    ) -> HttpResponse:
-
-        http_response = HttpResponse(
-            raw_response=response,
-            cast_type=cast_type,
-            client=self,
-            stream=stream,
-            stream_cls=stream_cls
-        )
-        return http_response.parse()
 
     def _process_response_data(
             self,
             *,
             data: object,
-            cast_type: type[ResponseT],
+            cast_type: Type[ResponseT],
             response: httpx.Response,
     ) -> ResponseT:
 
         if data is None:
             return cast(ResponseT, None)
 
         if cast_type is object:
             return cast(ResponseT, data)
 
         try:
             if inspect.isclass(cast_type) and issubclass(cast_type, ModelBuilderProtocol):
                 return cast(ResponseT, cast_type.build(response=response, data=data))
 
+            if self._strict_response_validation:
+                return cast(ResponseT, validate_type(type_=cast_type, value=data))
+
             return cast(ResponseT, construct_type(type_=cast_type, value=data))
         except pydantic.ValidationError as err:
             raise APIResponseValidationError(response=response, json_data=data) from err
 
     def _should_stream_response_body(self, request: httpx.Request) -> bool:
         return request.headers.get(RAW_RESPONSE_HEADER) == "stream"  # type: ignore[no-any-return]
 
@@ -354,15 +485,15 @@
     def request(
             self,
             cast_type: Type[ResponseT],
             options: FinalRequestOptions,
             remaining_retries: Optional[int] = None,
             *,
             stream: bool = False,
-            stream_cls: type[StreamResponse] | None = None,
+            stream_cls: Type[StreamResponse] | None = None,
     ) -> ResponseT | StreamResponse:
         return self._request(
             cast_type=cast_type,
             options=options,
             stream=stream,
             stream_cls=stream_cls,
             remaining_retries=remaining_retries,
@@ -371,15 +502,15 @@
     def _request(
             self,
             *,
             cast_type: Type[ResponseT],
             options: FinalRequestOptions,
             remaining_retries: int | None,
             stream: bool,
-            stream_cls: type[StreamResponse] | None,
+            stream_cls: Type[StreamResponse] | None,
     ) -> ResponseT | StreamResponse:
 
         retries = self._remaining_retries(remaining_retries, options)
         request = self._build_request(options)
 
         kwargs: HttpxSendArgs = {}
         if self.custom_auth is not None:
@@ -445,16 +576,22 @@
             # to completion before attempting to access the response text.
             if not err.response.is_closed:
                 err.response.read()
 
             log.debug("Re-raising status error")
             raise self._make_status_error(err.response) from None
 
-
-        return self._parse_response(
+        # return self._parse_response(
+        #     cast_type=cast_type,
+        #     options=options,
+        #     response=response,
+        #     stream=stream,
+        #     stream_cls=stream_cls,
+        # )
+        return self._process_response(
             cast_type=cast_type,
             options=options,
             response=response,
             stream=stream,
             stream_cls=stream_cls,
         )
 
@@ -462,15 +599,15 @@
             self,
             options: FinalRequestOptions,
             cast_type: Type[ResponseT],
             remaining_retries: int,
             response_headers: httpx.Headers | None,
             *,
             stream: bool,
-            stream_cls: type[StreamResponse] | None,
+            stream_cls: Type[StreamResponse] | None,
     ) -> ResponseT | StreamResponse:
         remaining = remaining_retries - 1
         if remaining == 1:
             log.debug("1 retry left")
         else:
             log.debug("%i retries left", remaining)
 
@@ -485,14 +622,90 @@
             options=options,
             cast_type=cast_type,
             remaining_retries=remaining,
             stream=stream,
             stream_cls=stream_cls,
         )
 
+    def _process_response(
+            self,
+            *,
+            cast_type: Type[ResponseT],
+            options: FinalRequestOptions,
+            response: httpx.Response,
+            stream: bool,
+            stream_cls: Type[StreamResponse] | None,
+    ) -> ResponseT:
+        # TODO 服务器支持
+        # if response.request.headers.get(RAW_RESPONSE_HEADER) == "true":
+        #     return cast(
+        #         ResponseT,
+        #         LegacyAPIResponse(
+        #             raw=response,
+        #             client=self,
+        #             cast_type=cast_type,
+        #             stream=stream,
+        #             stream_cls=stream_cls,
+        #             options=options,
+        #         ),
+        #     )
+
+        origin = get_origin(cast_type) or cast_type
+
+        if inspect.isclass(origin) and issubclass(origin, BaseAPIResponse):
+            if not issubclass(origin, APIResponse):
+                raise TypeError(f"API Response types must subclass {APIResponse}; Received {origin}")
+
+            response_cls = cast("type[BaseAPIResponse[Any]]", cast_type)
+            return cast(
+                ResponseT,
+                response_cls(
+                    raw=response,
+                    client=self,
+                    cast_type=extract_response_type(response_cls),
+                    stream=stream,
+                    stream_cls=stream_cls,
+                    options=options,
+                ),
+            )
+
+        if cast_type == httpx.Response:
+            return cast(ResponseT, response)
+
+        api_response = APIResponse(
+            raw=response,
+            client=self,
+            cast_type=cast("type[ResponseT]", cast_type),  # pyright: ignore[reportUnnecessaryCast]
+            stream=stream,
+            stream_cls=stream_cls,
+            options=options,
+        )
+        if bool(response.request.headers.get(RAW_RESPONSE_HEADER)):
+            return cast(ResponseT, api_response)
+
+        return api_response.parse()
+
+    def _request_api_list(
+            self,
+            model: Type[object],
+            page: Type[SyncPageT],
+            options: FinalRequestOptions,
+    ) -> SyncPageT:
+        def _parser(resp: SyncPageT) -> SyncPageT:
+            resp._set_private_attributes(
+                client=self,
+                model=model,
+                options=options,
+            )
+            return resp
+
+        options.post_parser = _parser
+
+        return self.request(page, options, stream=False)
+
     @overload
     def get(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             options: UserRequestInput = {},
@@ -504,39 +717,39 @@
     def get(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             options: UserRequestInput = {},
             stream: Literal[True],
-            stream_cls: type[StreamResponse],
+            stream_cls: Type[StreamResponse],
     ) -> StreamResponse:
         ...
 
     @overload
     def get(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             options: UserRequestInput = {},
             stream: bool,
-            stream_cls: type[StreamResponse] | None = None,
+            stream_cls: Type[StreamResponse] | None = None,
     ) -> ResponseT | StreamResponse:
         ...
 
     def get(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             options: UserRequestInput = {},
             stream: bool = False,
-            stream_cls: type[StreamResponse] | None = None,
-    ) -> ResponseT | _AsyncStreamT:
+            stream_cls: Type[StreamResponse] | None = None,
+    ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="get", url=path, **options)
         return cast(ResponseT, self.request(cast_type, opts, stream=stream, stream_cls=stream_cls))
 
     @overload
     def post(
             self,
             path: str,
@@ -555,48 +768,48 @@
             path: str,
             *,
             cast_type: Type[ResponseT],
             body: Body | None = None,
             options: UserRequestInput = {},
             files: RequestFiles | None = None,
             stream: Literal[True],
-            stream_cls: type[StreamResponse],
+            stream_cls: Type[StreamResponse],
     ) -> StreamResponse:
         ...
 
     @overload
     def post(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             body: Body | None = None,
             options: UserRequestInput = {},
             files: RequestFiles | None = None,
             stream: bool,
-            stream_cls: type[StreamResponse] | None = None,
+            stream_cls: Type[StreamResponse] | None = None,
     ) -> ResponseT | StreamResponse:
         ...
 
     def post(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             body: Body | None = None,
             options: UserRequestInput = {},
             files: RequestFiles | None = None,
             stream: bool = False,
-            stream_cls: type[StreamResponse[Any]] | None = None,
+            stream_cls: Type[StreamResponse[Any]] | None = None,
     ) -> ResponseT | StreamResponse:
         opts = FinalRequestOptions.construct(
             method="post", url=path, json_data=body, files=make_httpx_files(files), **options
         )
 
-        return cast(ResponseT,  self.request(cast_type, opts, stream=stream, stream_cls=stream_cls))
+        return cast(ResponseT, self.request(cast_type, opts, stream=stream, stream_cls=stream_cls))
 
     def patch(
             self,
             path: str,
             *,
             cast_type: Type[ResponseT],
             body: Body | None = None,
@@ -614,15 +827,15 @@
             *,
             cast_type: Type[ResponseT],
             body: Body | None = None,
             options: UserRequestInput = {},
             files: RequestFiles | None = None,
     ) -> ResponseT | StreamResponse:
         opts = FinalRequestOptions.construct(method="put", url=path, json_data=body, files=make_httpx_files(files),
-                                            **options)
+                                             **options)
 
         return self.request(
             cast_type=cast_type, options=opts,
         )
 
     def delete(
             self,
@@ -634,14 +847,27 @@
     ) -> ResponseT | StreamResponse:
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
 
         return self.request(
             cast_type=cast_type, options=opts,
         )
 
+    def get_api_list(
+            self,
+            path: str,
+            *,
+            model: Type[object],
+            page: Type[SyncPageT],
+            body: Body | None = None,
+            options: UserRequestInput = {},
+            method: str = "get",
+    ) -> SyncPageT:
+        opts = FinalRequestOptions.construct(method=method, url=path, json_data=body, **options)
+        return self._request_api_list(model, page, opts)
+
     def _make_status_error(self, response) -> APIStatusError:
         response_text = response.text.strip()
         status_code = response.status_code
         error_msg = f"Error code: {status_code}, with error text {response_text}"
 
         if status_code == 400:
             return _errors.APIRequestFailedError(message=error_msg, response=response)
@@ -658,15 +884,16 @@
 
 def make_request_options(
         *,
         query: Query | None = None,
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
-        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN
+        timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
+        post_parser: PostParser | NotGiven = NOT_GIVEN,
 ) -> UserRequestInput:
     """Create a dict of type RequestOptions without keys of NotGiven values."""
     options: UserRequestInput = {}
     if extra_headers is not None:
         options["headers"] = extra_headers
 
     if extra_body is not None:
@@ -677,14 +904,18 @@
 
     if extra_query is not None:
         options["params"] = {**options.get("params", {}), **extra_query}
 
     if not isinstance(timeout, NotGiven):
         options["timeout"] = timeout
 
+    if is_given(post_parser):
+        # internal
+        options["post_parser"] = post_parser  # type: ignore
+
     return options
 
 
 def _merge_mappings(
         obj1: Mapping[_T_co, Union[_T, Omit]],
         obj2: Mapping[_T_co, Union[_T, Omit]],
 ) -> Dict[_T_co, _T]:
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_jwt_token.py` & `zhipuai-2.1.0/zhipuai/core/_jwt_token.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding:utf-8 -*-
 import time
 
 import cachetools.func
 import jwt
 
-API_TOKEN_TTL_SECONDS = 3 * 60
+# 缓存时间 3分钟
+CACHE_TTL_SECONDS = 3 * 60
 
-CACHE_TTL_SECONDS = API_TOKEN_TTL_SECONDS - 30
+# token 有效期比缓存时间 多30秒
+API_TOKEN_TTL_SECONDS = CACHE_TTL_SECONDS + 30
 
 
 @cachetools.func.ttl_cache(maxsize=10, ttl=CACHE_TTL_SECONDS)
 def generate_token(apikey: str):
     try:
         api_key, secret = apikey.split(".")
     except Exception as e:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_request_opt.py` & `zhipuai-2.1.0/zhipuai/core/_request_opt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 from __future__ import annotations
 
 from typing import Union, Any, cast, TYPE_CHECKING
 
+from ._constants import RAW_RESPONSE_HEADER
+from ._utils import is_given
 from ._base_compat import ConfigDict, PYDANTIC_V2
 import pydantic.generics
 from httpx import Timeout
 from typing_extensions import (
-    final, Unpack, ClassVar, TypedDict
+    final, Unpack, ClassVar, TypedDict, Required, Callable
 
 )
 
 from ._base_type import Body, NotGiven, Headers, HttpxRequestFiles, Query, AnyMapping
 from ._utils import remove_notgiven_indict, strip_not_given
 
 
 class UserRequestInput(TypedDict, total=False):
     headers: Headers
     max_retries: int
     timeout: float | Timeout | None
     params: Query
     extra_json: AnyMapping
 
+
 class FinalRequestOptionsInput(TypedDict, total=False):
     method: Required[str]
     url: Required[str]
     params: Query
     headers: Headers
     max_retries: int
     timeout: float | Timeout | None
     files: HttpxRequestFiles | None
     json_data: Body
     extra_json: AnyMapping
 
+
 @final
 class FinalRequestOptions(pydantic.BaseModel):
     method: str
     url: str
     params: Query = {}
     headers: Union[Headers, NotGiven] = NotGiven()
     max_retries: Union[int, NotGiven] = NotGiven()
@@ -45,15 +49,14 @@
     post_parser: Union[Callable[[Any], Any], NotGiven] = NotGiven()
 
     # It should be noted that we cannot use `json` here as that would override
     # a BaseModel method in an incompatible fashion.
     json_data: Union[Body, None] = None
     extra_json: Union[AnyMapping, None] = None
 
-
     if PYDANTIC_V2:
         model_config: ClassVar[ConfigDict] = ConfigDict(arbitrary_types_allowed=True)
     else:
 
         class Config(pydantic.BaseConfig):  # pyright: ignore[reportDeprecated]
             arbitrary_types_allowed: bool = True
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_utils/__init__.py` & `zhipuai-2.1.0/zhipuai/core/_utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,8 +37,16 @@
     is_union_type as is_union_type,
     extract_type_arg as extract_type_arg,
     is_iterable_type as is_iterable_type,
     is_required_type as is_required_type,
     is_annotated_type as is_annotated_type,
     strip_annotated_type as strip_annotated_type,
     extract_type_var_from_base as extract_type_var_from_base,
-)
+)
+
+from ._transform import (
+    PropertyInfo as PropertyInfo,
+    transform as transform,
+    async_transform as async_transform,
+    maybe_transform as maybe_transform,
+    async_maybe_transform as async_maybe_transform,
+)
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_utils/_typing.py` & `zhipuai-2.1.0/zhipuai/core/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/_utils/_utils.py` & `zhipuai-2.1.0/zhipuai/core/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/core/logs.py` & `zhipuai-2.1.0/zhipuai/core/logs.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/types/chat/async_chat_completion.py` & `zhipuai-2.1.0/zhipuai/types/chat/async_chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion.py` & `zhipuai-2.1.0/zhipuai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/types/chat/chat_completion_chunk.py` & `zhipuai-2.1.0/zhipuai/types/chat/chat_completion_chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List, Optional, Dict, Any
 
 from ...core import BaseModel
 
 __all__ = [
+    "CompletionUsage",
     "ChatCompletionChunk",
     "Choice",
     "ChoiceDelta",
     "ChoiceDeltaFunctionCall",
     "ChoiceDeltaToolCall",
     "ChoiceDeltaToolCallFunction",
 ]
```

### Comparing `zhipuai-2.0.1.20240429/zhipuai/types/file_object.py` & `zhipuai-2.1.0/zhipuai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job.py` & `zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/zhipuai/types/fine_tuning/fine_tuning_job_event.py` & `zhipuai-2.1.0/zhipuai/types/fine_tuning/fine_tuning_job_event.py`

 * *Files identical despite different names*

### Comparing `zhipuai-2.0.1.20240429/PKG-INFO` & `zhipuai-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhipuai
-Version: 2.0.1.20240429
+Version: 2.1.0
 Summary: A SDK library for accessing big model apis from ZhipuAI
 Author: Zhipu AI
 Requires-Python: >=3.7, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.12.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -59,14 +59,33 @@
 ```python
 from zhipuai import ZhipuAI
 
 client = ZhipuAI(
     api_key="", # 填写您的 APIKey
 ) 
 ```
+### 客户端网络链接配置
+在`core/_http_client.py`中，可以配置网络链接的超时时间，重试次数，限制等参数
+```python
+# 通过 `Timeout` 控制接口`connect` 和 `read` 超时时间，默认为`timeout=300.0, connect=8.0`
+ZHIPUAI_DEFAULT_TIMEOUT = httpx.Timeout(timeout=300.0, connect=8.0)
+# 通过 `retry` 参数控制重试次数，默认为3次
+ZHIPUAI_DEFAULT_MAX_RETRIES = 3
+# 通过 `Limits` 控制最大连接数和保持连接数，默认为`max_connections=50, max_keepalive_connections=10`
+ZHIPUAI_DEFAULT_LIMITS = httpx.Limits(max_connections=50, max_keepalive_connections=10)
+ 
+```
+同样在`ZhipuAI`入参中可以配置
+```python
+client = ZhipuAI(
+    timeout= httpx.Timeout(timeout=300.0, connect=8.0),
+    max_retries=3,
+)
+```
+
 
 ### 同步调用
 
 ```python
 from zhipuai import ZhipuAI 
  
 client = ZhipuAI()  # 填写您自己的APIKey
```

