# Comparing `tmp/gpt_fn-0.1.4.tar.gz` & `tmp/gpt_fn-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_fn-0.1.4.tar", max compression
+gzip compressed data, was "gpt_fn-0.1.5.tar", max compression
```

## Comparing `gpt_fn-0.1.4.tar` & `gpt_fn-0.1.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1066 2024-05-15 07:19:33.974989 gpt_fn-0.1.4/LICENSE
--rw-r--r--   0        0        0     4102 2024-05-15 07:19:33.974989 gpt_fn-0.1.4/README.md
--rw-r--r--   0        0        0      919 2024-05-15 07:19:52.563025 gpt_fn-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 07:19:33.974989 gpt_fn-0.1.4/src/gpt_fn/__init__.py
--rw-r--r--   0        0        0     1204 2024-05-15 07:19:33.974989 gpt_fn-0.1.4/src/gpt_fn/ai_function.py
--rw-r--r--   0        0        0    14089 2024-05-15 07:19:33.974989 gpt_fn-0.1.4/src/gpt_fn/completion.py
--rw-r--r--   0        0        0      537 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/conftest.py
--rw-r--r--   0        0        0      508 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/exceptions.py
--rw-r--r--   0        0        0      883 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/prompt.py
--rw-r--r--   0        0        0        0 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/py.typed
--rw-r--r--   0        0        0        0 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/__init__.py
--rw-r--r--   0        0        0    60815 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
--rw-r--r--   0        0        0    32594 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/__snapshots__/test_completion.ambr
--rw-r--r--   0        0        0      713 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
--rw-r--r--   0        0        0    13985 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fabnocci.yaml
--rw-r--r--   0        0        0    16272 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fake_hero.yaml
--rw-r--r--   0        0        0   142193 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml
--rw-r--r--   0        0        0     2930 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     2866 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3144 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[OpenAI API].yaml
--rw-r--r--   0        0        0     3156 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     3254 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3846 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[OpenAI API].yaml
--rw-r--r--   0        0        0     3675 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     3687 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     4685 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[OpenAI API].yaml
--rw-r--r--   0        0        0     2921 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     2849 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3125 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[OpenAI API].yaml
--rw-r--r--   0        0        0     2812 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     2812 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3021 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[OpenAI API].yaml
--rw-r--r--   0        0        0     3145 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     3243 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3835 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[OpenAI API].yaml
--rw-r--r--   0        0        0     3261 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     3289 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3496 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[OpenAI API].yaml
--rw-r--r--   0        0        0     3352 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     3450 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3530 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[OpenAI API].yaml
--rw-r--r--   0        0        0     3628 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     3676 2024-05-15 07:19:33.978989 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     4252 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[OpenAI API].yaml
--rw-r--r--   0        0        0     3181 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-07-01 API].yaml
--rw-r--r--   0        0        0     3312 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-12-01 API].yaml
--rw-r--r--   0        0        0     3894 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[OpenAI API].yaml
--rw-r--r--   0        0        0     1499 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/tests/test_ai_function.py
--rw-r--r--   0        0        0    14371 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/tests/test_completion.py
--rw-r--r--   0        0        0     1557 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/tests/test_prompt.py
--rw-r--r--   0        0        0        0 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/__init__.py
--rw-r--r--   0        0        0     1951 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/pydantic_parser.py
--rw-r--r--   0        0        0     3827 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/signature.py
--rw-r--r--   0        0        0        0 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/__init__.py
--rw-r--r--   0        0        0     7891 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr
--rw-r--r--   0        0        0     6264 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
--rw-r--r--   0        0        0    15635 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
--rw-r--r--   0        0        0     8147 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser/test_pydantic_parser_with_prompt[email.txt-Email].yaml
--rw-r--r--   0        0        0     2186 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt
--rw-r--r--   0        0        0     3011 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/test_pydantic_parser.py
--rw-r--r--   0        0        0     2890 2024-05-15 07:19:33.982988 gpt_fn-0.1.4/src/gpt_fn/utils/tests/test_signature.py
--rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 gpt_fn-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4102 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/README.md
+-rw-r--r--   0        0        0      919 2024-05-17 01:45:29.082422 gpt_fn-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/__init__.py
+-rw-r--r--   0        0        0     1204 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/ai_function.py
+-rw-r--r--   0        0        0    14047 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/completion.py
+-rw-r--r--   0        0        0      537 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/conftest.py
+-rw-r--r--   0        0        0      508 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/exceptions.py
+-rw-r--r--   0        0        0      883 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/prompt.py
+-rw-r--r--   0        0        0        0 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/py.typed
+-rw-r--r--   0        0        0        0 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/__init__.py
+-rw-r--r--   0        0        0    60815 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr
+-rw-r--r--   0        0        0    32594 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/__snapshots__/test_completion.ambr
+-rw-r--r--   0        0        0      713 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/__snapshots__/test_prompt.ambr
+-rw-r--r--   0        0        0    13985 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fabnocci.yaml
+-rw-r--r--   0        0        0    16272 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fake_hero.yaml
+-rw-r--r--   0        0        0   142193 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml
+-rw-r--r--   0        0        0     2930 2024-05-17 01:45:11.974455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     2866 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3144 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3156 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3254 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3846 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3675 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3687 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     4685 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     2921 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     2849 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3125 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     2812 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     2812 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3021 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[OpenAI API].yaml
+-rw-r--r--   0        0        0     3145 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3243 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3835 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3261 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3289 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3496 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[OpenAI API].yaml
+-rw-r--r--   0        0        0     3352 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3450 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3530 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[OpenAI API].yaml
+-rw-r--r--   0        0        0     3628 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3676 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     4252 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[OpenAI API].yaml
+-rw-r--r--   0        0        0     3181 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-07-01 API].yaml
+-rw-r--r--   0        0        0     3312 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-12-01 API].yaml
+-rw-r--r--   0        0        0     3894 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[OpenAI API].yaml
+-rw-r--r--   0        0        0     1499 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/test_ai_function.py
+-rw-r--r--   0        0        0    14371 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/test_completion.py
+-rw-r--r--   0        0        0     1557 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/tests/test_prompt.py
+-rw-r--r--   0        0        0        0 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/__init__.py
+-rw-r--r--   0        0        0     1951 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/pydantic_parser.py
+-rw-r--r--   0        0        0     3827 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/signature.py
+-rw-r--r--   0        0        0        0 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/__init__.py
+-rw-r--r--   0        0        0     7891 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr
+-rw-r--r--   0        0        0     6264 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr
+-rw-r--r--   0        0        0    15635 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr
+-rw-r--r--   0        0        0     8147 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser/test_pydantic_parser_with_prompt[email.txt-Email].yaml
+-rw-r--r--   0        0        0     2186 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt
+-rw-r--r--   0        0        0     3011 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/test_pydantic_parser.py
+-rw-r--r--   0        0        0     2890 2024-05-17 01:45:11.978455 gpt_fn-0.1.5/src/gpt_fn/utils/tests/test_signature.py
+-rw-r--r--   0        0        0     4625 1970-01-01 00:00:00.000000 gpt_fn-0.1.5/PKG-INFO
```

### Comparing `gpt_fn-0.1.4/LICENSE` & `gpt_fn-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/README.md` & `gpt_fn-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/pyproject.toml` & `gpt_fn-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gpt-fn"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["lucemia <lucemia@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gpt_fn", from = "src" }]
 include = ["fn/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `gpt_fn-0.1.4/src/gpt_fn/ai_function.py` & `gpt_fn-0.1.5/src/gpt_fn/ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/completion.py` & `gpt_fn-0.1.5/src/gpt_fn/completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,34 +18,34 @@
     content: str
 
 
 class FunctionMessage(Message):
     name: str
 
 
-def infer_api_type() -> str:
+def infer_api_type() -> str | None:
     """
     Infers the API type based on environment variables and sets the api_type attribute accordingly.
 
     Raises:
         ValueError: If the API type cannot be determined.
     """
     if os.environ.get("OPENAI_API_KEY"):
         return "open_ai"
     elif os.environ.get("AZURE_OPENAI_API_KEY"):
         return "azure"
     else:
-        raise ValueError("API type could not be inferred from environment variables.")
+        return openai.api_type
 
 
 class APISettings(pydantic.BaseModel):
     api_key: str = pydantic.Field(default_factory=lambda: openai.api_key)
     api_base: str = pydantic.Field(default_factory=lambda: openai.azure_endpoint)
     api_version: str | None = pydantic.Field(default_factory=lambda: openai.api_version)
-    api_type: str = pydantic.Field(default_factory=infer_api_type)
+    api_type: str | None = pydantic.Field(default_factory=infer_api_type)
 
     def check_functions_required(self) -> bool:
         if self.api_version is None:
             assert self.api_type != "azure", "api_version is required for azure"
             return False
         if self.api_type == "azure" and datetime.strptime(str(self.api_version)[:10], "%Y-%m-%d") >= datetime(2023, 12, 1):
             return False
```

### Comparing `gpt_fn-0.1.4/src/gpt_fn/conftest.py` & `gpt_fn-0.1.5/src/gpt_fn/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/prompt.py` & `gpt_fn-0.1.5/src/gpt_fn/prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr` & `gpt_fn-0.1.5/src/gpt_fn/tests/__snapshots__/test_ai_function.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/__snapshots__/test_completion.ambr` & `gpt_fn-0.1.5/src/gpt_fn/tests/__snapshots__/test_completion.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/__snapshots__/test_prompt.ambr` & `gpt_fn-0.1.5/src/gpt_fn/tests/__snapshots__/test_prompt.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fabnocci.yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fabnocci.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fake_hero.yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fake_hero.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_ai_function/test_ai_fn_max_token.yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_achat_completion[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_afunction_completion[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_astructural_completion[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_chat_completion_incomplete[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_enough_tokens[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_function_completion_without_neccess_function[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-07-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-07-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-12-01 API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[Azure 2023-12-01 API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[OpenAI API].yaml` & `gpt_fn-0.1.5/src/gpt_fn/tests/cassettes/test_completion/test_structural_completion_without_enough_tokens[OpenAI API].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/test_ai_function.py` & `gpt_fn-0.1.5/src/gpt_fn/tests/test_ai_function.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/test_completion.py` & `gpt_fn-0.1.5/src/gpt_fn/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/tests/test_prompt.py` & `gpt_fn-0.1.5/src/gpt_fn/tests/test_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/pydantic_parser.py` & `gpt_fn-0.1.5/src/gpt_fn/utils/pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/signature.py` & `gpt_fn-0.1.5/src/gpt_fn/utils/signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr` & `gpt_fn-0.1.5/src/gpt_fn/utils/tests/__snapshots__/test_json_decode.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr` & `gpt_fn-0.1.5/src/gpt_fn/utils/tests/__snapshots__/test_pydantic_parser.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr` & `gpt_fn-0.1.5/src/gpt_fn/utils/tests/__snapshots__/test_signature.ambr`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser/test_pydantic_parser_with_prompt[email.txt-Email].yaml` & `gpt_fn-0.1.5/src/gpt_fn/utils/tests/cassettes/test_pydantic_parser/test_pydantic_parser_with_prompt[email.txt-Email].yaml`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt` & `gpt_fn-0.1.5/src/gpt_fn/utils/tests/test_pydantic_parser/email.txt`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/tests/test_pydantic_parser.py` & `gpt_fn-0.1.5/src/gpt_fn/utils/tests/test_pydantic_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/src/gpt_fn/utils/tests/test_signature.py` & `gpt_fn-0.1.5/src/gpt_fn/utils/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `gpt_fn-0.1.4/PKG-INFO` & `gpt_fn-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-fn
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: lucemia
 Author-email: lucemia@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

