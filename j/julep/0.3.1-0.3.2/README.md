# Comparing `tmp/julep-0.3.1.tar.gz` & `tmp/julep-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "julep-0.3.1.tar", max compression
+gzip compressed data, was "julep-0.3.2.tar", max compression
```

## Comparing `julep-0.3.1.tar` & `julep-0.3.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0      121 2024-04-09 11:11:10.306527 julep-0.3.1/README.md
--rw-r--r--   0        0        0      326 2024-04-05 09:31:45.036791 julep-0.3.1/julep/__init__.py
--rw-r--r--   0        0        0     4325 2024-04-26 08:42:15.216117 julep-0.3.1/julep/api/__init__.py
--rw-r--r--   0        0        0   134983 2024-04-26 08:49:16.342805 julep-0.3.1/julep/api/client.py
--rw-r--r--   0        0        0      519 2024-04-26 08:42:15.212117 julep-0.3.1/julep/api/core/__init__.py
--rw-r--r--   0        0        0      440 2024-04-26 08:42:28.515936 julep-0.3.1/julep/api/core/api_error.py
--rw-r--r--   0        0        0      972 2024-04-26 08:42:15.212117 julep-0.3.1/julep/api/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-04-26 08:42:28.519936 julep-0.3.1/julep/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-04-26 08:42:28.591935 julep-0.3.1/julep/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-26 08:42:15.212117 julep-0.3.1/julep/api/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      164 2024-04-26 08:42:15.212117 julep-0.3.1/julep/api/environment.py
--rw-r--r--   0        0        0     6647 2024-04-26 08:42:15.236117 julep-0.3.1/julep/api/types/__init__.py
--rw-r--r--   0        0        0     2024 2024-04-26 08:42:28.583935 julep-0.3.1/julep/api/types/agent.py
--rw-r--r--   0        0        0     3189 2024-04-26 08:42:28.587935 julep-0.3.1/julep/api/types/agent_default_settings.py
--rw-r--r--   0        0        0     1883 2024-04-26 08:42:15.232117 julep-0.3.1/julep/api/types/agent_default_settings_preset.py
--rw-r--r--   0        0        0      136 2024-04-26 08:42:15.232117 julep-0.3.1/julep/api/types/agent_instructions.py
--rw-r--r--   0        0        0      988 2024-04-26 08:42:28.535936 julep-0.3.1/julep/api/types/agent_metadata.py
--rw-r--r--   0        0        0     1675 2024-04-26 08:42:28.539936 julep-0.3.1/julep/api/types/chat_input_data.py
--rw-r--r--   0        0        0      251 2024-04-26 08:47:12.544293 julep-0.3.1/julep/api/types/chat_input_data_tool_choice.py
--rw-r--r--   0        0        0     1530 2024-04-26 08:42:28.539936 julep-0.3.1/julep/api/types/chat_ml_message.py
--rw-r--r--   0        0        0     1062 2024-04-26 08:42:15.240116 julep-0.3.1/julep/api/types/chat_ml_message_role.py
--rw-r--r--   0        0        0     2118 2024-04-26 08:42:28.531936 julep-0.3.1/julep/api/types/chat_response.py
--rw-r--r--   0        0        0     1479 2024-04-26 08:42:15.224117 julep-0.3.1/julep/api/types/chat_response_finish_reason.py
--rw-r--r--   0        0        0     6427 2024-04-26 08:42:28.587935 julep-0.3.1/julep/api/types/chat_settings.py
--rw-r--r--   0        0        0     1787 2024-04-26 08:42:15.240116 julep-0.3.1/julep/api/types/chat_settings_preset.py
--rw-r--r--   0        0        0     2352 2024-04-26 08:42:28.523936 julep-0.3.1/julep/api/types/chat_settings_response_format.py
--rw-r--r--   0        0        0     1037 2024-04-26 08:42:28.511936 julep-0.3.1/julep/api/types/chat_settings_response_format_schema.py
--rw-r--r--   0        0        0      786 2024-04-26 08:42:15.220117 julep-0.3.1/julep/api/types/chat_settings_response_format_type.py
--rw-r--r--   0        0        0      152 2024-04-26 08:42:15.220117 julep-0.3.1/julep/api/types/chat_settings_stop.py
--rw-r--r--   0        0        0     1358 2024-04-26 08:42:28.535936 julep-0.3.1/julep/api/types/completion_usage.py
--rw-r--r--   0        0        0      149 2024-04-26 08:42:15.244116 julep-0.3.1/julep/api/types/create_agent_request_instructions.py
--rw-r--r--   0        0        0     1003 2024-04-26 08:42:28.527936 julep-0.3.1/julep/api/types/create_agent_request_metadata.py
--rw-r--r--   0        0        0     1295 2024-04-26 08:42:28.543936 julep-0.3.1/julep/api/types/create_doc.py
--rw-r--r--   0        0        0      992 2024-04-26 08:42:28.527936 julep-0.3.1/julep/api/types/create_doc_metadata.py
--rw-r--r--   0        0        0     1003 2024-04-26 08:42:28.527936 julep-0.3.1/julep/api/types/create_session_request_metadata.py
--rw-r--r--   0        0        0     1329 2024-04-26 08:42:28.539936 julep-0.3.1/julep/api/types/create_tool_request.py
--rw-r--r--   0        0        0      646 2024-04-26 08:42:28.527936 julep-0.3.1/julep/api/types/create_tool_request_type.py
--rw-r--r--   0        0        0     1002 2024-04-26 08:42:28.539936 julep-0.3.1/julep/api/types/create_user_request_metadata.py
--rw-r--r--   0        0        0     1399 2024-04-26 08:42:28.555935 julep-0.3.1/julep/api/types/doc.py
--rw-r--r--   0        0        0      986 2024-04-26 08:42:28.543936 julep-0.3.1/julep/api/types/doc_metadata.py
--rw-r--r--   0        0        0     1159 2024-04-26 08:42:28.559935 julep-0.3.1/julep/api/types/function_call_option.py
--rw-r--r--   0        0        0     1493 2024-04-26 08:42:28.563935 julep-0.3.1/julep/api/types/function_def.py
--rw-r--r--   0        0        0      130 2024-04-26 08:42:15.236117 julep-0.3.1/julep/api/types/function_parameters.py
--rw-r--r--   0        0        0      485 2024-04-26 08:42:28.539936 julep-0.3.1/julep/api/types/get_agent_docs_request_order.py
--rw-r--r--   0        0        0      570 2024-04-26 08:42:28.539936 julep-0.3.1/julep/api/types/get_agent_docs_request_sort_by.py
--rw-r--r--   0        0        0     1023 2024-04-26 08:42:28.555935 julep-0.3.1/julep/api/types/get_agent_docs_response.py
--rw-r--r--   0        0        0     1036 2024-04-26 08:42:28.559935 julep-0.3.1/julep/api/types/get_agent_memories_response.py
--rw-r--r--   0        0        0     1027 2024-04-26 08:42:28.567935 julep-0.3.1/julep/api/types/get_agent_tools_response.py
--rw-r--r--   0        0        0     1053 2024-04-26 08:42:28.563935 julep-0.3.1/julep/api/types/get_history_response.py
--rw-r--r--   0        0        0     1046 2024-04-26 08:42:28.567935 julep-0.3.1/julep/api/types/get_suggestions_response.py
--rw-r--r--   0        0        0      482 2024-04-26 08:42:28.555935 julep-0.3.1/julep/api/types/get_user_docs_request_order.py
--rw-r--r--   0        0        0      567 2024-04-26 08:42:28.551936 julep-0.3.1/julep/api/types/get_user_docs_request_sort_by.py
--rw-r--r--   0        0        0     1022 2024-04-26 08:42:28.571935 julep-0.3.1/julep/api/types/get_user_docs_response.py
--rw-r--r--   0        0        0     1615 2024-04-26 08:42:28.579935 julep-0.3.1/julep/api/types/input_chat_ml_message.py
--rw-r--r--   0        0        0     1234 2024-04-26 08:42:15.240116 julep-0.3.1/julep/api/types/input_chat_ml_message_role.py
--rw-r--r--   0        0        0     1819 2024-04-26 08:42:28.587935 julep-0.3.1/julep/api/types/job_status.py
--rw-r--r--   0        0        0     1361 2024-04-26 08:42:15.224117 julep-0.3.1/julep/api/types/job_status_state.py
--rw-r--r--   0        0        0      479 2024-04-26 08:42:28.559935 julep-0.3.1/julep/api/types/list_agents_request_order.py
--rw-r--r--   0        0        0      564 2024-04-26 08:42:28.563935 julep-0.3.1/julep/api/types/list_agents_request_sort_by.py
--rw-r--r--   0        0        0     1010 2024-04-26 08:42:28.579935 julep-0.3.1/julep/api/types/list_agents_response.py
--rw-r--r--   0        0        0      485 2024-04-26 08:42:28.567935 julep-0.3.1/julep/api/types/list_sessions_request_order.py
--rw-r--r--   0        0        0      570 2024-04-26 08:42:28.571935 julep-0.3.1/julep/api/types/list_sessions_request_sort_by.py
--rw-r--r--   0        0        0     1018 2024-04-26 08:42:28.583935 julep-0.3.1/julep/api/types/list_sessions_response.py
--rw-r--r--   0        0        0      476 2024-04-26 08:42:28.571935 julep-0.3.1/julep/api/types/list_users_request_order.py
--rw-r--r--   0        0        0      561 2024-04-26 08:42:28.575935 julep-0.3.1/julep/api/types/list_users_request_sort_by.py
--rw-r--r--   0        0        0     1006 2024-04-26 08:42:28.591935 julep-0.3.1/julep/api/types/list_users_response.py
--rw-r--r--   0        0        0     1907 2024-04-26 08:42:28.611935 julep-0.3.1/julep/api/types/memory.py
--rw-r--r--   0        0        0     1365 2024-04-26 08:42:28.599935 julep-0.3.1/julep/api/types/memory_access_options.py
--rw-r--r--   0        0        0      954 2024-04-26 08:42:28.607935 julep-0.3.1/julep/api/types/memory_entities_item.py
--rw-r--r--   0        0        0     1240 2024-04-26 08:42:28.599935 julep-0.3.1/julep/api/types/named_tool_choice.py
--rw-r--r--   0        0        0     1040 2024-04-26 08:42:28.595935 julep-0.3.1/julep/api/types/named_tool_choice_function.py
--rw-r--r--   0        0        0     1534 2024-04-26 08:42:28.611935 julep-0.3.1/julep/api/types/partial_function_def.py
--rw-r--r--   0        0        0      148 2024-04-26 08:42:15.236117 julep-0.3.1/julep/api/types/patch_agent_request_instructions.py
--rw-r--r--   0        0        0     1000 2024-04-26 08:42:28.595935 julep-0.3.1/julep/api/types/patch_agent_request_metadata.py
--rw-r--r--   0        0        0     1002 2024-04-26 08:42:28.595935 julep-0.3.1/julep/api/types/patch_session_request_metadata.py
--rw-r--r--   0        0        0      999 2024-04-26 08:42:28.603935 julep-0.3.1/julep/api/types/patch_user_request_metadata.py
--rw-r--r--   0        0        0     1143 2024-04-26 08:42:28.603935 julep-0.3.1/julep/api/types/resource_created_response.py
--rw-r--r--   0        0        0     1143 2024-04-26 08:42:28.607935 julep-0.3.1/julep/api/types/resource_deleted_response.py
--rw-r--r--   0        0        0     1143 2024-04-26 08:42:28.607935 julep-0.3.1/julep/api/types/resource_updated_response.py
--rw-r--r--   0        0        0     2107 2024-04-26 08:42:28.627935 julep-0.3.1/julep/api/types/session.py
--rw-r--r--   0        0        0      990 2024-04-26 08:42:28.615935 julep-0.3.1/julep/api/types/session_metadata.py
--rw-r--r--   0        0        0     1502 2024-04-26 08:42:28.615935 julep-0.3.1/julep/api/types/suggestion.py
--rw-r--r--   0        0        0      546 2024-04-26 08:42:28.603935 julep-0.3.1/julep/api/types/suggestion_target.py
--rw-r--r--   0        0        0     1327 2024-04-26 08:42:28.619935 julep-0.3.1/julep/api/types/tool.py
--rw-r--r--   0        0        0       88 2024-04-26 08:42:15.224117 julep-0.3.1/julep/api/types/tool_choice_option.py
--rw-r--r--   0        0        0      607 2024-04-26 08:42:28.607935 julep-0.3.1/julep/api/types/tool_type.py
--rw-r--r--   0        0        0      149 2024-04-26 08:42:15.232117 julep-0.3.1/julep/api/types/update_agent_request_instructions.py
--rw-r--r--   0        0        0     1001 2024-04-26 08:42:28.619935 julep-0.3.1/julep/api/types/update_agent_request_metadata.py
--rw-r--r--   0        0        0     1003 2024-04-26 08:42:28.615935 julep-0.3.1/julep/api/types/update_session_request_metadata.py
--rw-r--r--   0        0        0     1000 2024-04-26 08:42:28.619935 julep-0.3.1/julep/api/types/update_user_request_metadata.py
--rw-r--r--   0        0        0     1559 2024-04-26 08:42:28.627935 julep-0.3.1/julep/api/types/user.py
--rw-r--r--   0        0        0      989 2024-04-26 08:42:28.619935 julep-0.3.1/julep/api/types/user_metadata.py
--rw-r--r--   0        0        0    11638 2024-04-16 05:25:00.535880 julep-0.3.1/julep/client.py
--rw-r--r--   0        0        0      527 2024-04-18 03:57:55.434983 julep-0.3.1/julep/env.py
--rw-r--r--   0        0        0        0 2024-04-05 09:31:45.040791 julep-0.3.1/julep/managers/__init__.py
--rw-r--r--   0        0        0    32129 2024-04-18 06:05:18.506024 julep-0.3.1/julep/managers/agent.py
--rw-r--r--   0        0        0     1249 2024-04-18 06:05:18.506024 julep-0.3.1/julep/managers/base.py
--rw-r--r--   0        0        0    21222 2024-04-26 06:24:15.533309 julep-0.3.1/julep/managers/doc.py
--rw-r--r--   0        0        0     7707 2024-04-18 05:08:06.874967 julep-0.3.1/julep/managers/memory.py
--rw-r--r--   0        0        0    47059 2024-04-18 06:05:18.510024 julep-0.3.1/julep/managers/session.py
--rw-r--r--   0        0        0    18899 2024-04-26 06:24:15.533309 julep-0.3.1/julep/managers/tool.py
--rw-r--r--   0        0        0     1758 2024-04-18 06:05:18.510024 julep-0.3.1/julep/managers/types.py
--rw-r--r--   0        0        0    19731 2024-04-16 05:25:00.535880 julep-0.3.1/julep/managers/user.py
--rw-r--r--   0        0        0     1628 2024-04-18 06:05:18.510024 julep-0.3.1/julep/managers/utils.py
--rw-r--r--   0        0        0        0 2024-04-05 09:31:45.040791 julep-0.3.1/julep/utils/__init__.py
--rw-r--r--   0        0        0    14233 2024-04-18 06:05:18.510024 julep-0.3.1/julep/utils/openai_patch.py
--rw-r--r--   0        0        0     1668 2024-04-26 08:54:27.515232 julep-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 julep-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      121 2024-04-09 11:11:10.306527 julep-0.3.2/README.md
+-rw-r--r--   0        0        0      326 2024-04-05 09:31:45.036791 julep-0.3.2/julep/__init__.py
+-rw-r--r--   0        0        0     4325 2024-04-26 08:42:15.216117 julep-0.3.2/julep/api/__init__.py
+-rw-r--r--   0        0        0   134983 2024-04-26 08:49:16.342805 julep-0.3.2/julep/api/client.py
+-rw-r--r--   0        0        0      519 2024-04-26 08:42:15.212117 julep-0.3.2/julep/api/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-26 08:42:28.515936 julep-0.3.2/julep/api/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-04-26 08:42:15.212117 julep-0.3.2/julep/api/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-04-26 08:42:28.519936 julep-0.3.2/julep/api/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-04-26 08:42:28.591935 julep-0.3.2/julep/api/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-26 08:42:15.212117 julep-0.3.2/julep/api/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      164 2024-04-26 08:42:15.212117 julep-0.3.2/julep/api/environment.py
+-rw-r--r--   0        0        0     6647 2024-04-26 08:42:15.236117 julep-0.3.2/julep/api/types/__init__.py
+-rw-r--r--   0        0        0     2024 2024-04-26 08:42:28.583935 julep-0.3.2/julep/api/types/agent.py
+-rw-r--r--   0        0        0     3189 2024-04-26 08:42:28.587935 julep-0.3.2/julep/api/types/agent_default_settings.py
+-rw-r--r--   0        0        0     1883 2024-04-26 08:42:15.232117 julep-0.3.2/julep/api/types/agent_default_settings_preset.py
+-rw-r--r--   0        0        0      136 2024-04-26 08:42:15.232117 julep-0.3.2/julep/api/types/agent_instructions.py
+-rw-r--r--   0        0        0      988 2024-04-26 08:42:28.535936 julep-0.3.2/julep/api/types/agent_metadata.py
+-rw-r--r--   0        0        0     1675 2024-04-26 08:42:28.539936 julep-0.3.2/julep/api/types/chat_input_data.py
+-rw-r--r--   0        0        0      251 2024-04-26 08:47:12.544293 julep-0.3.2/julep/api/types/chat_input_data_tool_choice.py
+-rw-r--r--   0        0        0     1530 2024-04-26 08:42:28.539936 julep-0.3.2/julep/api/types/chat_ml_message.py
+-rw-r--r--   0        0        0     1062 2024-04-26 08:42:15.240116 julep-0.3.2/julep/api/types/chat_ml_message_role.py
+-rw-r--r--   0        0        0     2118 2024-04-26 08:42:28.531936 julep-0.3.2/julep/api/types/chat_response.py
+-rw-r--r--   0        0        0     1479 2024-04-26 08:42:15.224117 julep-0.3.2/julep/api/types/chat_response_finish_reason.py
+-rw-r--r--   0        0        0     6427 2024-04-26 08:42:28.587935 julep-0.3.2/julep/api/types/chat_settings.py
+-rw-r--r--   0        0        0     1787 2024-04-26 08:42:15.240116 julep-0.3.2/julep/api/types/chat_settings_preset.py
+-rw-r--r--   0        0        0     2352 2024-04-26 08:42:28.523936 julep-0.3.2/julep/api/types/chat_settings_response_format.py
+-rw-r--r--   0        0        0     1037 2024-04-26 08:42:28.511936 julep-0.3.2/julep/api/types/chat_settings_response_format_schema.py
+-rw-r--r--   0        0        0      786 2024-04-26 08:42:15.220117 julep-0.3.2/julep/api/types/chat_settings_response_format_type.py
+-rw-r--r--   0        0        0      152 2024-04-26 08:42:15.220117 julep-0.3.2/julep/api/types/chat_settings_stop.py
+-rw-r--r--   0        0        0     1358 2024-04-26 08:42:28.535936 julep-0.3.2/julep/api/types/completion_usage.py
+-rw-r--r--   0        0        0      149 2024-04-26 08:42:15.244116 julep-0.3.2/julep/api/types/create_agent_request_instructions.py
+-rw-r--r--   0        0        0     1003 2024-04-26 08:42:28.527936 julep-0.3.2/julep/api/types/create_agent_request_metadata.py
+-rw-r--r--   0        0        0     1295 2024-04-26 08:42:28.543936 julep-0.3.2/julep/api/types/create_doc.py
+-rw-r--r--   0        0        0      992 2024-04-26 08:42:28.527936 julep-0.3.2/julep/api/types/create_doc_metadata.py
+-rw-r--r--   0        0        0     1003 2024-04-26 08:42:28.527936 julep-0.3.2/julep/api/types/create_session_request_metadata.py
+-rw-r--r--   0        0        0     1329 2024-04-26 08:42:28.539936 julep-0.3.2/julep/api/types/create_tool_request.py
+-rw-r--r--   0        0        0      646 2024-04-26 08:42:28.527936 julep-0.3.2/julep/api/types/create_tool_request_type.py
+-rw-r--r--   0        0        0     1002 2024-04-26 08:42:28.539936 julep-0.3.2/julep/api/types/create_user_request_metadata.py
+-rw-r--r--   0        0        0     1399 2024-04-26 08:42:28.555935 julep-0.3.2/julep/api/types/doc.py
+-rw-r--r--   0        0        0      986 2024-04-26 08:42:28.543936 julep-0.3.2/julep/api/types/doc_metadata.py
+-rw-r--r--   0        0        0     1159 2024-04-26 08:42:28.559935 julep-0.3.2/julep/api/types/function_call_option.py
+-rw-r--r--   0        0        0     1493 2024-04-26 08:42:28.563935 julep-0.3.2/julep/api/types/function_def.py
+-rw-r--r--   0        0        0      130 2024-04-26 08:42:15.236117 julep-0.3.2/julep/api/types/function_parameters.py
+-rw-r--r--   0        0        0      485 2024-04-26 08:42:28.539936 julep-0.3.2/julep/api/types/get_agent_docs_request_order.py
+-rw-r--r--   0        0        0      570 2024-04-26 08:42:28.539936 julep-0.3.2/julep/api/types/get_agent_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1023 2024-04-26 08:42:28.555935 julep-0.3.2/julep/api/types/get_agent_docs_response.py
+-rw-r--r--   0        0        0     1036 2024-04-26 08:42:28.559935 julep-0.3.2/julep/api/types/get_agent_memories_response.py
+-rw-r--r--   0        0        0     1027 2024-04-26 08:42:28.567935 julep-0.3.2/julep/api/types/get_agent_tools_response.py
+-rw-r--r--   0        0        0     1053 2024-04-26 08:42:28.563935 julep-0.3.2/julep/api/types/get_history_response.py
+-rw-r--r--   0        0        0     1046 2024-04-26 08:42:28.567935 julep-0.3.2/julep/api/types/get_suggestions_response.py
+-rw-r--r--   0        0        0      482 2024-04-26 08:42:28.555935 julep-0.3.2/julep/api/types/get_user_docs_request_order.py
+-rw-r--r--   0        0        0      567 2024-04-26 08:42:28.551936 julep-0.3.2/julep/api/types/get_user_docs_request_sort_by.py
+-rw-r--r--   0        0        0     1022 2024-04-26 08:42:28.571935 julep-0.3.2/julep/api/types/get_user_docs_response.py
+-rw-r--r--   0        0        0     1615 2024-04-26 08:42:28.579935 julep-0.3.2/julep/api/types/input_chat_ml_message.py
+-rw-r--r--   0        0        0     1234 2024-04-26 08:42:15.240116 julep-0.3.2/julep/api/types/input_chat_ml_message_role.py
+-rw-r--r--   0        0        0     1819 2024-04-26 08:42:28.587935 julep-0.3.2/julep/api/types/job_status.py
+-rw-r--r--   0        0        0     1361 2024-04-26 08:42:15.224117 julep-0.3.2/julep/api/types/job_status_state.py
+-rw-r--r--   0        0        0      479 2024-04-26 08:42:28.559935 julep-0.3.2/julep/api/types/list_agents_request_order.py
+-rw-r--r--   0        0        0      564 2024-04-26 08:42:28.563935 julep-0.3.2/julep/api/types/list_agents_request_sort_by.py
+-rw-r--r--   0        0        0     1010 2024-04-26 08:42:28.579935 julep-0.3.2/julep/api/types/list_agents_response.py
+-rw-r--r--   0        0        0      485 2024-04-26 08:42:28.567935 julep-0.3.2/julep/api/types/list_sessions_request_order.py
+-rw-r--r--   0        0        0      570 2024-04-26 08:42:28.571935 julep-0.3.2/julep/api/types/list_sessions_request_sort_by.py
+-rw-r--r--   0        0        0     1018 2024-04-26 08:42:28.583935 julep-0.3.2/julep/api/types/list_sessions_response.py
+-rw-r--r--   0        0        0      476 2024-04-26 08:42:28.571935 julep-0.3.2/julep/api/types/list_users_request_order.py
+-rw-r--r--   0        0        0      561 2024-04-26 08:42:28.575935 julep-0.3.2/julep/api/types/list_users_request_sort_by.py
+-rw-r--r--   0        0        0     1006 2024-04-26 08:42:28.591935 julep-0.3.2/julep/api/types/list_users_response.py
+-rw-r--r--   0        0        0     1907 2024-04-26 08:42:28.611935 julep-0.3.2/julep/api/types/memory.py
+-rw-r--r--   0        0        0     1365 2024-04-26 08:42:28.599935 julep-0.3.2/julep/api/types/memory_access_options.py
+-rw-r--r--   0        0        0      954 2024-04-26 08:42:28.607935 julep-0.3.2/julep/api/types/memory_entities_item.py
+-rw-r--r--   0        0        0     1240 2024-04-26 08:42:28.599935 julep-0.3.2/julep/api/types/named_tool_choice.py
+-rw-r--r--   0        0        0     1040 2024-04-26 08:42:28.595935 julep-0.3.2/julep/api/types/named_tool_choice_function.py
+-rw-r--r--   0        0        0     1534 2024-04-26 08:42:28.611935 julep-0.3.2/julep/api/types/partial_function_def.py
+-rw-r--r--   0        0        0      148 2024-04-26 08:42:15.236117 julep-0.3.2/julep/api/types/patch_agent_request_instructions.py
+-rw-r--r--   0        0        0     1000 2024-04-26 08:42:28.595935 julep-0.3.2/julep/api/types/patch_agent_request_metadata.py
+-rw-r--r--   0        0        0     1002 2024-04-26 08:42:28.595935 julep-0.3.2/julep/api/types/patch_session_request_metadata.py
+-rw-r--r--   0        0        0      999 2024-04-26 08:42:28.603935 julep-0.3.2/julep/api/types/patch_user_request_metadata.py
+-rw-r--r--   0        0        0     1143 2024-04-26 08:42:28.603935 julep-0.3.2/julep/api/types/resource_created_response.py
+-rw-r--r--   0        0        0     1143 2024-04-26 08:42:28.607935 julep-0.3.2/julep/api/types/resource_deleted_response.py
+-rw-r--r--   0        0        0     1143 2024-04-26 08:42:28.607935 julep-0.3.2/julep/api/types/resource_updated_response.py
+-rw-r--r--   0        0        0     2107 2024-04-26 09:03:40.526682 julep-0.3.2/julep/api/types/session.py
+-rw-r--r--   0        0        0      990 2024-04-26 08:42:28.615935 julep-0.3.2/julep/api/types/session_metadata.py
+-rw-r--r--   0        0        0     1502 2024-04-26 08:42:28.615935 julep-0.3.2/julep/api/types/suggestion.py
+-rw-r--r--   0        0        0      546 2024-04-26 08:42:28.603935 julep-0.3.2/julep/api/types/suggestion_target.py
+-rw-r--r--   0        0        0     1327 2024-04-26 08:42:28.619935 julep-0.3.2/julep/api/types/tool.py
+-rw-r--r--   0        0        0       88 2024-04-26 08:42:15.224117 julep-0.3.2/julep/api/types/tool_choice_option.py
+-rw-r--r--   0        0        0      607 2024-04-26 08:42:28.607935 julep-0.3.2/julep/api/types/tool_type.py
+-rw-r--r--   0        0        0      149 2024-04-26 08:42:15.232117 julep-0.3.2/julep/api/types/update_agent_request_instructions.py
+-rw-r--r--   0        0        0     1001 2024-04-26 08:42:28.619935 julep-0.3.2/julep/api/types/update_agent_request_metadata.py
+-rw-r--r--   0        0        0     1003 2024-04-26 08:42:28.615935 julep-0.3.2/julep/api/types/update_session_request_metadata.py
+-rw-r--r--   0        0        0     1000 2024-04-26 08:42:28.619935 julep-0.3.2/julep/api/types/update_user_request_metadata.py
+-rw-r--r--   0        0        0     1559 2024-04-26 08:42:28.627935 julep-0.3.2/julep/api/types/user.py
+-rw-r--r--   0        0        0      989 2024-04-26 08:42:28.619935 julep-0.3.2/julep/api/types/user_metadata.py
+-rw-r--r--   0        0        0    11638 2024-04-16 05:25:00.535880 julep-0.3.2/julep/client.py
+-rw-r--r--   0        0        0      527 2024-04-18 03:57:55.434983 julep-0.3.2/julep/env.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:31:45.040791 julep-0.3.2/julep/managers/__init__.py
+-rw-r--r--   0        0        0    32129 2024-04-18 06:05:18.506024 julep-0.3.2/julep/managers/agent.py
+-rw-r--r--   0        0        0     1249 2024-04-18 06:05:18.506024 julep-0.3.2/julep/managers/base.py
+-rw-r--r--   0        0        0    21222 2024-04-26 06:24:15.533309 julep-0.3.2/julep/managers/doc.py
+-rw-r--r--   0        0        0     7707 2024-04-18 05:08:06.874967 julep-0.3.2/julep/managers/memory.py
+-rw-r--r--   0        0        0    47327 2024-04-26 17:22:25.305723 julep-0.3.2/julep/managers/session.py
+-rw-r--r--   0        0        0    18899 2024-04-26 06:24:15.533309 julep-0.3.2/julep/managers/tool.py
+-rw-r--r--   0        0        0     1758 2024-04-18 06:05:18.510024 julep-0.3.2/julep/managers/types.py
+-rw-r--r--   0        0        0    19731 2024-04-16 05:25:00.535880 julep-0.3.2/julep/managers/user.py
+-rw-r--r--   0        0        0     1628 2024-04-18 06:05:18.510024 julep-0.3.2/julep/managers/utils.py
+-rw-r--r--   0        0        0        0 2024-04-05 09:31:45.040791 julep-0.3.2/julep/utils/__init__.py
+-rw-r--r--   0        0        0    14233 2024-04-18 06:05:18.510024 julep-0.3.2/julep/utils/openai_patch.py
+-rw-r--r--   0        0        0     1668 2024-04-27 04:39:57.545775 julep-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 julep-0.3.2/PKG-INFO
```

### Comparing `julep-0.3.1/julep/api/__init__.py` & `julep-0.3.2/julep/api/__init__.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/client.py` & `julep-0.3.2/julep/api/client.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/core/__init__.py` & `julep-0.3.2/julep/api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/core/client_wrapper.py` & `julep-0.3.2/julep/api/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/core/datetime_utils.py` & `julep-0.3.2/julep/api/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/core/jsonable_encoder.py` & `julep-0.3.2/julep/api/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/__init__.py` & `julep-0.3.2/julep/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/agent.py` & `julep-0.3.2/julep/api/types/agent.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/agent_default_settings.py` & `julep-0.3.2/julep/api/types/agent_default_settings.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/agent_default_settings_preset.py` & `julep-0.3.2/julep/api/types/agent_default_settings_preset.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/agent_metadata.py` & `julep-0.3.2/julep/api/types/agent_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_input_data.py` & `julep-0.3.2/julep/api/types/chat_input_data.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_ml_message.py` & `julep-0.3.2/julep/api/types/chat_ml_message.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_ml_message_role.py` & `julep-0.3.2/julep/api/types/chat_ml_message_role.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_response.py` & `julep-0.3.2/julep/api/types/chat_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_response_finish_reason.py` & `julep-0.3.2/julep/api/types/chat_response_finish_reason.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_settings.py` & `julep-0.3.2/julep/api/types/chat_settings.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_settings_preset.py` & `julep-0.3.2/julep/api/types/chat_settings_preset.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_settings_response_format.py` & `julep-0.3.2/julep/api/types/chat_settings_response_format.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_settings_response_format_schema.py` & `julep-0.3.2/julep/api/types/chat_settings_response_format_schema.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/chat_settings_response_format_type.py` & `julep-0.3.2/julep/api/types/chat_settings_response_format_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/completion_usage.py` & `julep-0.3.2/julep/api/types/completion_usage.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/create_agent_request_metadata.py` & `julep-0.3.2/julep/api/types/create_agent_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/create_doc.py` & `julep-0.3.2/julep/api/types/create_doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/create_doc_metadata.py` & `julep-0.3.2/julep/api/types/create_doc_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/create_session_request_metadata.py` & `julep-0.3.2/julep/api/types/create_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/create_tool_request.py` & `julep-0.3.2/julep/api/types/create_tool_request.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/create_tool_request_type.py` & `julep-0.3.2/julep/api/types/create_tool_request_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/create_user_request_metadata.py` & `julep-0.3.2/julep/api/types/create_user_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/doc.py` & `julep-0.3.2/julep/api/types/doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/doc_metadata.py` & `julep-0.3.2/julep/api/types/doc_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/function_call_option.py` & `julep-0.3.2/julep/api/types/function_call_option.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/function_def.py` & `julep-0.3.2/julep/api/types/function_def.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_agent_docs_request_sort_by.py` & `julep-0.3.2/julep/api/types/get_agent_docs_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_agent_docs_response.py` & `julep-0.3.2/julep/api/types/get_agent_docs_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_agent_memories_response.py` & `julep-0.3.2/julep/api/types/get_agent_memories_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_agent_tools_response.py` & `julep-0.3.2/julep/api/types/get_agent_tools_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_history_response.py` & `julep-0.3.2/julep/api/types/get_history_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_suggestions_response.py` & `julep-0.3.2/julep/api/types/get_suggestions_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_user_docs_request_sort_by.py` & `julep-0.3.2/julep/api/types/get_user_docs_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/get_user_docs_response.py` & `julep-0.3.2/julep/api/types/get_user_docs_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/input_chat_ml_message.py` & `julep-0.3.2/julep/api/types/input_chat_ml_message.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/input_chat_ml_message_role.py` & `julep-0.3.2/julep/api/types/input_chat_ml_message_role.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/job_status.py` & `julep-0.3.2/julep/api/types/job_status.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/job_status_state.py` & `julep-0.3.2/julep/api/types/job_status_state.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/list_agents_request_sort_by.py` & `julep-0.3.2/julep/api/types/list_agents_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/list_agents_response.py` & `julep-0.3.2/julep/api/types/list_agents_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/list_sessions_request_sort_by.py` & `julep-0.3.2/julep/api/types/list_sessions_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/list_sessions_response.py` & `julep-0.3.2/julep/api/types/list_sessions_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/list_users_request_sort_by.py` & `julep-0.3.2/julep/api/types/list_users_request_sort_by.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/list_users_response.py` & `julep-0.3.2/julep/api/types/list_users_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/memory.py` & `julep-0.3.2/julep/api/types/memory.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/memory_access_options.py` & `julep-0.3.2/julep/api/types/memory_access_options.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/memory_entities_item.py` & `julep-0.3.2/julep/api/types/memory_entities_item.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/named_tool_choice.py` & `julep-0.3.2/julep/api/types/named_tool_choice.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/named_tool_choice_function.py` & `julep-0.3.2/julep/api/types/named_tool_choice_function.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/partial_function_def.py` & `julep-0.3.2/julep/api/types/partial_function_def.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/patch_agent_request_metadata.py` & `julep-0.3.2/julep/api/types/patch_agent_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/patch_session_request_metadata.py` & `julep-0.3.2/julep/api/types/patch_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/patch_user_request_metadata.py` & `julep-0.3.2/julep/api/types/patch_user_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/resource_created_response.py` & `julep-0.3.2/julep/api/types/resource_created_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/resource_deleted_response.py` & `julep-0.3.2/julep/api/types/resource_deleted_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/resource_updated_response.py` & `julep-0.3.2/julep/api/types/resource_updated_response.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/session.py` & `julep-0.3.2/julep/api/types/session.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/session_metadata.py` & `julep-0.3.2/julep/api/types/session_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/suggestion.py` & `julep-0.3.2/julep/api/types/suggestion.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/suggestion_target.py` & `julep-0.3.2/julep/api/types/suggestion_target.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/tool.py` & `julep-0.3.2/julep/api/types/tool.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/tool_type.py` & `julep-0.3.2/julep/api/types/tool_type.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/update_agent_request_metadata.py` & `julep-0.3.2/julep/api/types/update_agent_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/update_session_request_metadata.py` & `julep-0.3.2/julep/api/types/update_session_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/update_user_request_metadata.py` & `julep-0.3.2/julep/api/types/update_user_request_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/user.py` & `julep-0.3.2/julep/api/types/user.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/api/types/user_metadata.py` & `julep-0.3.2/julep/api/types/user_metadata.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/client.py` & `julep-0.3.2/julep/client.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/env.py` & `julep-0.3.2/julep/env.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/agent.py` & `julep-0.3.2/julep/managers/agent.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/base.py` & `julep-0.3.2/julep/managers/base.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/doc.py` & `julep-0.3.2/julep/managers/doc.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/memory.py` & `julep-0.3.2/julep/managers/memory.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/session.py` & `julep-0.3.2/julep/managers/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,23 @@
 
 
 class SessionCreateArgs(TypedDict):
     user_id: Optional[Union[str, UUID]]
     agent_id: Union[str, UUID]
     situation: Optional[str] = None
     metadata: Dict[str, Any] = {}
+    render_templates: bool = False
 
 
 class SessionUpdateArgs(TypedDict):
     session_id: Union[str, UUID]
     situation: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
     overwrite: bool = False
+    render_templates: bool = False
 
 
 class BaseSessionsManager(BaseManager):
     """
     A class to manage sessions using base API client methods.
 
     This manager handles CRUD operations and additional actions on the session data,
@@ -175,26 +177,28 @@
 
     def _create(
         self,
         agent_id: Union[str, UUID],
         user_id: Optional[Union[str, UUID]] = None,
         situation: Optional[str] = None,
         metadata: Dict[str, Any] = {},
+        render_templates: bool = False,
     ) -> Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]:
         # Cast instructions to a list of Instruction objects
         """
         Creates a session for a specified user and agent.
 
         This internal method is responsible for creating a session using the API client. It validates that both the user and agent IDs are valid UUID v4 strings before proceeding with session creation.
 
         Args:
             agent_id (Union[str, UUID]): The agent's identifier which could be a string or a UUID object.
             user_id (Optional[Union[str, UUID]]): The user's identifier which could be a string or a UUID object.
             situation (Optional[str], optional): An optional description of the situation.
             metadata (Dict[str, Any])
+            render_templates (bool, optional): Whether to render templates in the metadata. Defaults to False.
 
         Returns:
             Union[ResourceCreatedResponse, Awaitable[ResourceCreatedResponse]]: The response from the API client upon successful session creation, which can be a synchronous `ResourceCreatedResponse` or an asynchronous `Awaitable` of it.
 
         Raises:
             AssertionError: If either `user_id` or `agent_id` is not a valid UUID v4.
         """
@@ -204,14 +208,15 @@
             assert is_valid_uuid4(user_id), "user_id must be a valid UUID v4"
 
         return self.api_client.create_session(
             user_id=user_id,
             agent_id=agent_id,
             situation=situation,
             metadata=metadata,
+            render_templates=render_templates,
         )
 
     def _list_items(
         self,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         metadata_filter: str = "{}",
```

### Comparing `julep-0.3.1/julep/managers/tool.py` & `julep-0.3.2/julep/managers/tool.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/types.py` & `julep-0.3.2/julep/managers/types.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/user.py` & `julep-0.3.2/julep/managers/user.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/managers/utils.py` & `julep-0.3.2/julep/managers/utils.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/julep/utils/openai_patch.py` & `julep-0.3.2/julep/utils/openai_patch.py`

 * *Files identical despite different names*

### Comparing `julep-0.3.1/pyproject.toml` & `julep-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "julep"
-version = "0.3.1"
+version = "0.3.2"
 description = "Julep is a platform for creating agents with long-term memory"
 authors = ["Julep Developers <developers@julep.ai>"]
 license = "ISC"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.14"
```

### Comparing `julep-0.3.1/PKG-INFO` & `julep-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: julep
-Version: 0.3.1
+Version: 0.3.2
 Summary: Julep is a platform for creating agents with long-term memory
 License: ISC
 Author: Julep Developers
 Author-email: developers@julep.ai
 Requires-Python: >=3.8,<3.14
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
```

