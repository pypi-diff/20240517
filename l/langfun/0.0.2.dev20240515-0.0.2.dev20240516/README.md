# Comparing `tmp/langfun-0.0.2.dev20240515.tar.gz` & `tmp/langfun-0.0.2.dev20240516.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240515.tar", last modified: Wed May 15 08:04:19 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240516.tar", last modified: Thu May 16 08:03:28 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240515.tar` & `langfun-0.0.2.dev20240516.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.987388 langfun-0.0.2.dev20240515/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.995388 langfun-0.0.2.dev20240515/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.995388 langfun-0.0.2.dev20240515/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.995388 langfun-0.0.2.dev20240515/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.999389 langfun-0.0.2.dev20240515/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:18.999389 langfun-0.0.2.dev20240515/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.003389 langfun-0.0.2.dev20240515/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.003389 langfun-0.0.2.dev20240515/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.003389 langfun-0.0.2.dev20240515/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 08:04:18.000000 langfun-0.0.2.dev20240515/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 08:04:19.007388 langfun-0.0.2.dev20240515/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-15 08:03:39.000000 langfun-0.0.2.dev20240515/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.902238 langfun-0.0.2.dev20240516/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.910238 langfun-0.0.2.dev20240516/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.910238 langfun-0.0.2.dev20240516/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.910238 langfun-0.0.2.dev20240516/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.914238 langfun-0.0.2.dev20240516/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20202 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.914238 langfun-0.0.2.dev20240516/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.914238 langfun-0.0.2.dev20240516/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.918238 langfun-0.0.2.dev20240516/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.918238 langfun-0.0.2.dev20240516/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 08:03:28.000000 langfun-0.0.2.dev20240516/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:03:28.922238 langfun-0.0.2.dev20240516/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-16 08:02:56.000000 langfun-0.0.2.dev20240516/setup.py
```

### Comparing `langfun-0.0.2.dev20240515/LICENSE` & `langfun-0.0.2.dev20240516/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/PKG-INFO` & `langfun-0.0.2.dev20240516/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240515
+Version: 0.0.2.dev20240516
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240515/README.md` & `langfun-0.0.2.dev20240516/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/__init__.py` & `langfun-0.0.2.dev20240516/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240516/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/component.py` & `langfun-0.0.2.dev20240516/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/component_test.py` & `langfun-0.0.2.dev20240516/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240516/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240516/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/console.py` & `langfun-0.0.2.dev20240516/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/console_test.py` & `langfun-0.0.2.dev20240516/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240516/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240516/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240516/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/language_model.py` & `langfun-0.0.2.dev20240516/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240516/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,25 +29,26 @@
 # From https://platform.openai.com/settings/organization/limits
 _DEFAULT_TPM = 250000
 _DEFAULT_RPM = 3000
 
 SUPPORTED_MODELS_AND_SETTINGS = {
     # Models from https://platform.openai.com/docs/models
     # RPM is from https://platform.openai.com/docs/guides/rate-limits
-    'gpt-4o': pg.Dict(rpm=10000, tpm=1500000),
-    'gpt-4o-2024-05-13': pg.Dict(rpm=10000, tpm=1500000),
-    # GPT-4-Turbo models.
-    'gpt-4-turbo': pg.Dict(rpm=10000, tpm=1500000),
-    'gpt-4-turbo-2024-04-09': pg.Dict(rpm=10000, tpm=1500000),
-    'gpt-4-turbo-preview': pg.Dict(rpm=10000, tpm=1500000),
-    'gpt-4-0125-preview': pg.Dict(rpm=10000, tpm=1500000),
-    'gpt-4-1106-preview': pg.Dict(rpm=10000, tpm=1500000),
-    'gpt-4-vision-preview': pg.Dict(rpm=10000, tpm=1500000),
+    # GPT-4o models
+    'gpt-4o': pg.Dict(rpm=10000, tpm=5000000),
+    'gpt-4o-2024-05-13': pg.Dict(rpm=10000, tpm=5000000),
+    # GPT-4-Turbo models
+    'gpt-4-turbo': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-4-turbo-2024-04-09': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-4-turbo-preview': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-4-0125-preview': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-4-1106-preview': pg.Dict(rpm=10000, tpm=2000000),
+    'gpt-4-vision-preview': pg.Dict(rpm=10000, tpm=2000000),
     'gpt-4-1106-vision-preview': pg.Dict(
-        rpm=10000, tpm=1500000
+        rpm=10000, tpm=2000000
     ),
     # GPT-4 models
     'gpt-4': pg.Dict(rpm=10000, tpm=300000),
     'gpt-4-0613': pg.Dict(rpm=10000, tpm=300000),
     'gpt-4-0314': pg.Dict(rpm=10000, tpm=300000),
     'gpt-4-32k': pg.Dict(rpm=10000, tpm=300000),
     'gpt-4-32k-0613': pg.Dict(rpm=10000, tpm=300000),
```

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/vertexai.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,15 +95,15 @@
       raise ValueError(
           'Please specify `location` during `__init__` or set environment '
           'variable `VERTEXAI_LOCATION` with your Vertex AI service location.'
       )
 
     credentials = self.credentials
     # Placeholder for Google-internal credentials.
-    from google.cloud.aiplatform import vertexai  # pylint: disable=g-import-not-at-top
+    import vertexai
     vertexai.init(project=project, location=location, credentials=credentials)
     return True
 
   @property
   def model_id(self) -> str:
     """Returns a string to identify the model."""
     return f'VertexAI({self.model})'
@@ -121,28 +121,28 @@
         tokens_per_min=0,
     )
 
   def _generation_config(
       self, options: lf.LMSamplingOptions
   ) -> Any:  # generative_models.GenerationConfig
     """Creates generation config from langfun sampling options."""
-    from google.cloud.aiplatform.vertexai.preview import generative_models  # pylint: disable=g-import-not-at-top
+    from vertexai import generative_models
     return generative_models.GenerationConfig(
         temperature=options.temperature,
         top_p=options.top_p,
         top_k=options.top_k,
         max_output_tokens=options.max_tokens,
         stop_sequences=options.stop,
     )
 
   def _content_from_message(
       self, prompt: lf.Message
   ) -> list[str | Any]:
     """Gets generation input from langfun message."""
-    from google.cloud.aiplatform.vertexai.preview import generative_models  # pylint: disable=g-import-not-at-top
+    from vertexai import generative_models
     chunks = []
     for lf_chunk in prompt.chunk():
       if isinstance(lf_chunk, str):
         chunk = lf_chunk
       elif self.multimodal and isinstance(lf_chunk, lf_modalities.Image):
         chunk = generative_models.Image.from_bytes(lf_chunk.to_bytes())
       else:
@@ -235,26 +235,26 @@
 
   def get_generative_model(
       self, model_id: str
   ) -> Any:  # generative_models.GenerativeModel:
     """Gets a generative model by model id."""
     model = self._generative_model_cache.get(model_id, None)
     if model is None:
-      from google.cloud.aiplatform.vertexai.preview import generative_models  # pylint: disable=g-import-not-at-top
+      from vertexai import generative_models
       model = generative_models.GenerativeModel(model_id)
       self._generative_model_cache[model_id] = model
     return model
 
   def get_text_generation_model(
       self, model_id: str
   ) -> Any:  # language_models.TextGenerationModel
     """Gets a text generation model by model id."""
     model = self._text_generation_model_cache.get(model_id, None)
     if model is None:
-      from google.cloud.aiplatform.vertexai import language_models  # pylint: disable=g-import-not-at-top
+      from vertexai import language_models
       model = language_models.TextGenerationModel.from_pretrained(model_id)
       self._text_generation_model_cache[model_id] = model
     return model
 
 
 _VERTEXAI_MODEL_HUB = _ModelHub()
```

### Comparing `langfun-0.0.2.dev20240515/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240516/langfun/core/llms/vertexai_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Tests for Gemini models."""
 
 import os
 import unittest
 from unittest import mock
 
-from google.cloud.aiplatform.vertexai.preview import generative_models
+from vertexai import generative_models
 import langfun.core as lf
 from langfun.core import modalities as lf_modalities
 from langfun.core.llms import vertexai
 import pyglove as pg
 
 
 example_image = (
@@ -35,15 +35,14 @@
     b'\xdao\xd0|\x00\x00\x00\x00IEND\xaeB`\x82'
 )
 
 
 def mock_generate_content(content, generation_config, **kwargs):
   del kwargs
   c = pg.Dict(generation_config.to_dict())
-  print('zzz', c)
   return generative_models.GenerationResponse.from_dict({
       'candidates': [
           {
               'index': 0,
               'content': {
                   'role': 'model',
                   'parts': [
@@ -107,29 +106,29 @@
     })
     model = vertexai.VertexAIGeminiPro1()
     message = model._generation_response_to_message(response)
     self.assertEqual(message, lf.AIMessage('hello world'))
 
   def test_model_hub(self):
     with mock.patch(
-        'google.cloud.aiplatform.vertexai.preview.generative_models.'
+        'vertexai.generative_models.'
         'GenerativeModel.__init__'
     ) as mock_model_init:
       mock_model_init.side_effect = lambda *args, **kwargs: None
       model = vertexai._VERTEXAI_MODEL_HUB.get_generative_model(
           'gemini-1.0-pro'
       )
       self.assertIsNotNone(model)
       self.assertIs(
           vertexai._VERTEXAI_MODEL_HUB.get_generative_model('gemini-1.0-pro'),
           model,
       )
 
     with mock.patch(
-        'google.cloud.aiplatform.vertexai.language_models.'
+        'vertexai.language_models.'
         'TextGenerationModel.from_pretrained'
     ) as mock_model_init:
 
       class TextGenerationModel:
         pass
 
       mock_model_init.side_effect = lambda *args, **kw: TextGenerationModel()
@@ -159,21 +158,21 @@
     os.environ['VERTEXAI_LOCATION'] = 'us-central1'
     self.assertTrue(vertexai.VertexAIGeminiPro1()._api_initialized)
     del os.environ['VERTEXAI_PROJECT']
     del os.environ['VERTEXAI_LOCATION']
 
   def test_call_generative_model(self):
     with mock.patch(
-        'google.cloud.aiplatform.vertexai.preview.generative_models.'
+        'vertexai.generative_models.'
         'GenerativeModel.__init__'
     ) as mock_model_init:
       mock_model_init.side_effect = lambda *args, **kwargs: None
 
       with mock.patch(
-          'google.cloud.aiplatform.vertexai.preview.generative_models.'
+          'vertexai.generative_models.'
           'GenerativeModel.generate_content'
       ) as mock_generate:
         mock_generate.side_effect = mock_generate_content
 
         lm = vertexai.VertexAIGeminiPro1(project='abc', location='us-central1')
         self.assertEqual(
             lm(
@@ -188,15 +187,15 @@
                 'This is a response to hello with temperature=2.0, '
                 'top_p=1.0, top_k=20.0, max_tokens=1024, stop=\n.'
             ),
         )
 
   def test_call_text_generation_model(self):
     with mock.patch(
-        'google.cloud.aiplatform.vertexai.language_models.'
+        'vertexai.language_models.'
         'TextGenerationModel.from_pretrained'
     ) as mock_model_init:
 
       class TextGenerationModel:
 
         def predict(self, prompt, **kwargs):
           c = pg.Dict(kwargs)
```

### Comparing `langfun-0.0.2.dev20240515/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240516/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/memory.py` & `langfun-0.0.2.dev20240516/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/message.py` & `langfun-0.0.2.dev20240516/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/message_test.py` & `langfun-0.0.2.dev20240516/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240516/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240516/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240516/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240516/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240516/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240516/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modality.py` & `langfun-0.0.2.dev20240516/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240516/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240516/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240516/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/sampling.py` & `langfun-0.0.2.dev20240516/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240516/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240516/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/subscription.py` & `langfun-0.0.2.dev20240516/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240516/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/template.py` & `langfun-0.0.2.dev20240516/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/template_test.py` & `langfun-0.0.2.dev20240516/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240516/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240516/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240516/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240516/langfun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240515
+Version: 0.0.2.dev20240516
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240515/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240516/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240515/setup.py` & `langfun-0.0.2.dev20240516/setup.py`

 * *Files identical despite different names*

