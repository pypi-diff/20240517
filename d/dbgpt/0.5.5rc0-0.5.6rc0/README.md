# Comparing `tmp/dbgpt-0.5.5rc0.tar.gz` & `tmp/dbgpt-0.5.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbgpt-0.5.5rc0.tar", last modified: Thu Apr 18 03:05:22 2024, max compression
+gzip compressed data, was "dbgpt-0.5.6rc0.tar", last modified: Mon May  6 06:24:51 2024, max compression
```

## Comparing `dbgpt-0.5.5rc0.tar` & `dbgpt-0.5.6rc0.tar`

### file list

```diff
@@ -1,462 +1,485 @@
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.085496 dbgpt-0.5.5rc0/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.5rc0/LICENSE
--rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.5rc0/MANIFEST.in
--rw-r--r--   0 staneyffer   (501) staff       (20)    30253 2024-04-18 03:05:22.084796 dbgpt-0.5.5rc0/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    11946 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/README.md
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.797715 dbgpt-0.5.5rc0/dbgpt/
--rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.801427 dbgpt-0.5.5rc0/dbgpt/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14183 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/config.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1693 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/llm_metadata.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2234 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/_private/pydantic.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-10 15:09:52.000000 dbgpt-0.5.5rc0/dbgpt/_version.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.801728 dbgpt-0.5.5rc0/dbgpt/agent/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1125 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/agent/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.806821 dbgpt-0.5.5rc0/dbgpt/agent/actions/
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5354 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      890 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/blank_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3746 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/chart_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5097 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/code_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4461 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/dashboard_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5443 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/indicator_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5491 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/actions/plugin_action.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.810930 dbgpt-0.5.5rc0/dbgpt/agent/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9497 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5364 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/agent_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    35815 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/base_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5544 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/base_team.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.812142 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3473 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm_client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.813235 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/priority.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3715 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/role.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      466 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/core/user_proxy_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.817278 dbgpt-0.5.5rc0/dbgpt/agent/expand/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1675 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7025 2024-04-16 17:14:04.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/code_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2207 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5415 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/data_scientist_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2715 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/plugin_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22055 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1685 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/expand/summary_assistant_agent.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.819411 dbgpt-0.5.5rc0/dbgpt/agent/memory/
--rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6850 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5803 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/default_gpts_memory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7170 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/memory/gpts_memory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.821740 dbgpt-0.5.5rc0/dbgpt/agent/plan/
--rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.823998 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10852 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6014 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator_resource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8258 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/team_awel_layout.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4732 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/plan_action.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7582 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/planner_agent.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12459 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plan/team_auto_plan.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.825803 dbgpt-0.5.5rc0/dbgpt/agent/plugin/
--rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.827682 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/
--rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.828088 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/
--rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.830121 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/
--rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5226 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    22485 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command_manage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/generator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/plugin/plugins_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.832787 dbgpt-0.5.5rc0/dbgpt/agent/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3721 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_db_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_knowledge_api.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3224 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_plugin_api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.834142 dbgpt-0.5.5rc0/dbgpt/agent/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/agent/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/agent/util/cmp.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.835035 dbgpt-0.5.5rc0/dbgpt/cli/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/cli/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/cli/cli_scripts.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.838920 dbgpt-0.5.5rc0/dbgpt/client/
--rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.5rc0/dbgpt/client/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-04-17 10:27:40.000000 dbgpt-0.5.5rc0/dbgpt/client/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.5rc0/dbgpt/client/app.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14335 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3784 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3568 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/flow.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7003 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9487 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/client/schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10759 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/component.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.839908 dbgpt-0.5.5rc0/dbgpt/configs/
--rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/configs/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10186 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/configs/model_config.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.840591 dbgpt-0.5.5rc0/dbgpt/core/
--rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.842026 dbgpt-0.5.5rc0/dbgpt/core/_private/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/example_base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/_private/prompt_registry.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.842690 dbgpt-0.5.5rc0/dbgpt/core/awel/
--rw-r--r--   0 staneyffer   (501) staff       (20)     6061 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.845836 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4143 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/dag_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/dag/loader.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.849896 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    33942 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1084 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/compat.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/exceptions.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    29039 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/flow/flow_factory.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.852865 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11154 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/common_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/operators/stream_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.854341 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/
--rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/resource/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.856561 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/
--rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/job_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/runner/local_runner.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.859147 dbgpt-0.5.5rc0/dbgpt/core/awel/task/
--rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14193 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/task/task_impl.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.863491 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/
--rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    37988 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/http_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/iterator_trigger.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/trigger_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.866415 dbgpt-0.5.5rc0/dbgpt/core/awel/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/_typing_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/http_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2328 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/awel/util/parameter_util.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.873538 dbgpt-0.5.5rc0/dbgpt/core/interface/
--rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/embeddings.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3818 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31110 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/llm.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    42803 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/message.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.878118 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/message_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    16465 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/prompt_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/operators/retriever.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/output_parser.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    26575 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/prompt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1748 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15126 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/interface/storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.878848 dbgpt-0.5.5rc0/dbgpt/core/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.881201 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/
--rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/composer_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/core/operators/flow/dict_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.882453 dbgpt-0.5.5rc0/dbgpt/core/schema/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/core/schema/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8246 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/core/schema/api.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.885625 dbgpt-0.5.5rc0/dbgpt/datasource/
--rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6653 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/conn_spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/db_conn_info.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.887735 dbgpt-0.5.5rc0/dbgpt/datasource/manages/
--rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/connect_config_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8392 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/manages/connector_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.888451 dbgpt-0.5.5rc0/dbgpt/datasource/nosql/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/nosql/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.889918 dbgpt-0.5.5rc0/dbgpt/datasource/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.5rc0/dbgpt/datasource/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/operators/datasource_operator.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.897610 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12585 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_doris.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_duckdb.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_hive.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mssql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mysql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_postgresql.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_sqlite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_starrocks.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.898231 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/
--rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.898831 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/
--rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.900469 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
--rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.5rc0/dbgpt/datasource/redis.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.903268 dbgpt-0.5.5rc0/dbgpt/model/
--rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.912503 dbgpt-0.5.5rc0/dbgpt/model/adapter/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3071 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/embeddings_loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/fschat_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9327 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/hf_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/model_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/old_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9783 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/proxy_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/adapter/vllm_adapter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/cli.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.914015 dbgpt-0.5.5rc0/dbgpt/model/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/model/operators/llm_operator.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18163 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/parameter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.915211 dbgpt-0.5.5rc0/dbgpt/model/proxy/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1013 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.923920 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/
--rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/baichuan.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/bard.py
--rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/chatgpt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/claude.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/gemini.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/moonshot.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/proxy_model.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/spark.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/tongyi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/wenxin.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/yi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/zhipu.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.926322 dbgpt-0.5.5rc0/dbgpt/model/utils/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/chatgpt_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/llm_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/model/utils/token_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.927912 dbgpt-0.5.5rc0/dbgpt/rag/
--rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.931570 dbgpt-0.5.5rc0/dbgpt/rag/assembler/
--rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/assembler/summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/chunk_manager.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.934462 dbgpt-0.5.5rc0/dbgpt/rag/embedding/
--rw-r--r--   0 staneyffer   (501) staff       (20)      725 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/_wrapped.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/embedding_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    24261 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/rag/embedding/embeddings.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.935766 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/
--rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/evaluation/retriever.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.938265 dbgpt-0.5.5rc0/dbgpt/rag/extractor/
--rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/extractor/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.938914 dbgpt-0.5.5rc0/dbgpt/rag/graph/
--rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/graph/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.947645 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/
--rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/csv.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2131 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/docx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/html.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/json.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/markdown.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pdf.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pptx.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/string.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/txt.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/knowledge/url.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.953454 dbgpt-0.5.5rc0/dbgpt/rag/operators/
--rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/assembler.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/datasource.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/evaluation.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/knowledge.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/rewrite.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/schema_linking.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/operators/summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.957440 dbgpt-0.5.5rc0/dbgpt/rag/retriever/
--rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4107 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/db_schema.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8548 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/embedding.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4242 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/rerank.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/rag/retriever/rewrite.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.959293 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/
--rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/base_linker.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/schema_linking.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.961655 dbgpt-0.5.5rc0/dbgpt/rag/summary/
--rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4057 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary_client.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-13 17:38:21.000000 dbgpt-0.5.5rc0/dbgpt/rag/summary/rdbms_db_summary.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.964496 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/
--rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    31787 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/text_splitter.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/token_splitter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.965560 dbgpt-0.5.5rc0/dbgpt/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.973084 dbgpt-0.5.5rc0/dbgpt/storage/cache/
--rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/embedding_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/llm_cache.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-04-17 10:41:53.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/operators.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.973881 dbgpt-0.5.5rc0/dbgpt/storage/cache/protocol/
--rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/protocol/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.975078 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/
--rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/base.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.976473 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/
--rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.978356 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/
--rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/chat_history_db.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/chat_history/storage_adapter.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.982178 dbgpt-0.5.5rc0/dbgpt/storage/metadata/
--rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9345 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/_base_dao.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_factory.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_manager.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1860 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/schema.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.986115 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/
--rw-r--r--   0 staneyffer   (501) staff       (20)      960 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7923 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8233 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/chroma_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6622 2024-04-10 06:34:08.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/connector.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1234 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/filters.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    21288 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/milvus_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3440 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/pgvector_store.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     6727 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/storage/vector_store/weaviate_store.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.010463 dbgpt-0.5.5rc0/dbgpt/util/
--rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/_db_migration_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2868 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/annotations.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/api_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.011350 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/__init__.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.013055 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9317 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/chat_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    19203 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/code_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-04-12 06:30:46.000000 dbgpt-0.5.5rc0/dbgpt/util/command_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/config_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.014455 dbgpt-0.5.5rc0/dbgpt/util/console/
--rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/console/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/console/console.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/custom_data_structure.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.5rc0/dbgpt/util/date_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.019006 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11198 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/loader.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    11883 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/repo.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    10560 2024-04-15 03:42:53.000000 dbgpt-0.5.5rc0/dbgpt/util/dbgpts/template.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/error_types.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/executor_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3929 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/fastapi.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/formatting.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/function_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/global_helper.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.5rc0/dbgpt/util/i18n_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/util/json_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/memory_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/model_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/module_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/net_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.020208 dbgpt-0.5.5rc0/dbgpt/util/network/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/util/network/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     9818 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/network/_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/openai_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      618 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/pagination_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/parameter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/path_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/pd_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     8747 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/prompt_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1676 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/dbgpt/util/retry.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.021012 dbgpt-0.5.5rc0/dbgpt/util/serialization/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/serialization/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-04-17 10:39:42.000000 dbgpt-0.5.5rc0/dbgpt/util/serialization/json_serialization.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1219 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/similarity_util.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/singleton.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.025755 dbgpt-0.5.5rc0/dbgpt/util/speech/
--rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/brian.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/eleven_labs.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/gtts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/macos_tts.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/speech/say.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/splitter_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/util/string_utils.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.5rc0/dbgpt/util/system_utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.030555 dbgpt-0.5.5rc0/dbgpt/util/tracer/
--rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/span_storage.py
--rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_cli.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-17 04:06:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_impl.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_middleware.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.5rc0/dbgpt/util/utils.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.032504 dbgpt-0.5.5rc0/dbgpt/vis/
--rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 14:37:18.000000 dbgpt-0.5.5rc0/dbgpt/vis/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/base.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/client.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:22.038159 dbgpt-0.5.5rc0/dbgpt/vis/tags/
--rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/__init__.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_agent_message.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_agent_plans.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_chart.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_code.py
--rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_dashboard.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_gpts_execution.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_gpts_result.py
--rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_plugin.py
-drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-04-18 03:05:21.799891 dbgpt-0.5.5rc0/dbgpt.egg-info/
--rw-r--r--   0 staneyffer   (501) staff       (20)    30253 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/PKG-INFO
--rw-r--r--   0 staneyffer   (501) staff       (20)    12658 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/SOURCES.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/dependency_links.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/entry_points.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)     4987 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/requires.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-04-18 03:05:21.000000 dbgpt-0.5.5rc0/dbgpt.egg-info/top_level.txt
--rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-04-18 03:05:22.085629 dbgpt-0.5.5rc0/setup.cfg
--rw-r--r--   0 staneyffer   (501) staff       (20)    24009 2024-04-18 02:11:54.000000 dbgpt-0.5.5rc0/setup.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.134457 dbgpt-0.5.6rc0/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1067 2023-10-24 06:24:09.000000 dbgpt-0.5.6rc0/LICENSE
+-rw-r--r--   0 staneyffer   (501) staff       (20)       59 2023-12-16 11:45:45.000000 dbgpt-0.5.6rc0/MANIFEST.in
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31466 2024-05-06 06:24:51.133822 dbgpt-0.5.6rc0/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12437 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/README.md
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.808346 dbgpt-0.5.6rc0/dbgpt/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      638 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.813573 dbgpt-0.5.6rc0/dbgpt/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       83 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14757 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/_private/config.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1693 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/_private/llm_metadata.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2234 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/_private/pydantic.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       18 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/_version.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.814326 dbgpt-0.5.6rc0/dbgpt/agent/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1259 2024-05-06 03:59:41.000000 dbgpt-0.5.6rc0/dbgpt/agent/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.821354 dbgpt-0.5.6rc0/dbgpt/agent/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1008 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.823886 dbgpt-0.5.6rc0/dbgpt/agent/core/action/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      744 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/action/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5892 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/action/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      936 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/action/blank_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9734 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5336 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/agent_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    37924 2024-05-06 03:36:27.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/base_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6063 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/base_team.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.830006 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      540 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9235 2024-05-06 03:24:52.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/agent_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24306 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.832886 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      554 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6837 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5799 2024-05-06 03:59:42.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/default_gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7169 2024-05-06 03:59:42.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/gpts_memory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10793 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/hybrid.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5629 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6836 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/long_term.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8549 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/memory/short_term.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.835976 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      914 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.838948 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       60 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10720 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6272 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator_resource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8700 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/team_awel_layout.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4730 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/plan_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8730 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/planner_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13138 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/plan/team_auto_plan.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.840571 dbgpt-0.5.6rc0/dbgpt/agent/core/profile/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      951 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/profile/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12666 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/profile/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7380 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/role.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      456 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      560 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/core/user_proxy_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.847129 dbgpt-0.5.6rc0/dbgpt/agent/expand/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2560 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/Indicator_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.852273 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       32 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3761 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/chart_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5249 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/code_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4476 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/dashboard_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5457 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/indicator_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5583 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/plugin_action.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8090 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/code_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3054 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/dashboard_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6358 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/data_scientist_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3512 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/plugin_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22221 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2560 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/expand/summary_assistant_agent.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.855671 dbgpt-0.5.6rc0/dbgpt/agent/plugin/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      214 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.860058 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       23 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.860861 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       36 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.863406 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       88 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10775 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      687 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1188 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5535 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/command.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    22485 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/command_manage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1166 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6159 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/generator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1240 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7625 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/plugin/plugins_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.867631 dbgpt-0.5.6rc0/dbgpt/agent/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      665 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3721 2024-04-20 08:03:40.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_db_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      782 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_knowledge_api.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3225 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_plugin_api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.868868 dbgpt-0.5.6rc0/dbgpt/agent/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      114 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      850 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/cmp.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.870630 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3473 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6745 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm_client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.872136 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1291 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/priority.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.873116 dbgpt-0.5.6rc0/dbgpt/cli/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/cli/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5794 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/cli/cli_scripts.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.880221 dbgpt-0.5.6rc0/dbgpt/client/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      154 2024-03-22 07:58:46.000000 dbgpt-0.5.6rc0/dbgpt/client/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7280 2024-04-17 10:27:40.000000 dbgpt-0.5.6rc0/dbgpt/client/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1413 2024-03-22 07:58:46.000000 dbgpt-0.5.6rc0/dbgpt/client/app.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14335 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3784 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3568 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/flow.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7003 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9487 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/client/schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10759 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/component.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.881874 dbgpt-0.5.6rc0/dbgpt/configs/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      530 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/configs/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10962 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/configs/model_config.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.882809 dbgpt-0.5.6rc0/dbgpt/core/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2672 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.884810 dbgpt-0.5.6rc0/dbgpt/core/_private/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/_private/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1225 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/_private/example_base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3753 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/_private/prompt_registry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.885666 dbgpt-0.5.6rc0/dbgpt/core/awel/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6061 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.889271 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29536 2024-03-26 04:37:36.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4143 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/dag_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3309 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/dag/loader.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.893395 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      752 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    33942 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1506 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/compat.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1577 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/exceptions.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29039 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/flow/flow_factory.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.896919 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11174 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11132 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/common_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4262 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/operators/stream_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.898405 dbgpt-0.5.6rc0/dbgpt/core/awel/resource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       58 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/resource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/resource/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.900727 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      118 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4203 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/job_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7648 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/runner/local_runner.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.903284 dbgpt-0.5.6rc0/dbgpt/core/awel/task/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       26 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/task/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14271 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/task/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    20591 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/task/task_impl.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.909529 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       34 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      519 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6462 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/ext_http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    37988 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/http_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6040 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/iterator_trigger.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7886 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/trigger_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.912683 dbgpt-0.5.6rc0/dbgpt/core/awel/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      228 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/_typing_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      500 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/http_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2328 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/awel/util/parameter_util.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.922466 dbgpt-0.5.6rc0/dbgpt/core/interface/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      102 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3546 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1018 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/embeddings.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7410 2024-03-23 08:18:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3818 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31110 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/llm.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    42803 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/message.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.928278 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       55 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4438 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18962 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23685 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/message_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    16465 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/prompt_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      767 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/operators/retriever.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10805 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/output_parser.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    26575 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/prompt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1748 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15126 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/interface/storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.929232 dbgpt-0.5.6rc0/dbgpt/core/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1509 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.931647 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      340 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9546 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/composer_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2601 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/core/operators/flow/dict_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.932886 dbgpt-0.5.6rc0/dbgpt/core/schema/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/core/schema/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8246 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/core/schema/api.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.937972 dbgpt-0.5.6rc0/dbgpt/datasource/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      412 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6802 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/datasource/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3909 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/conn_spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4454 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/datasource/conn_tugraph.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      923 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/db_conn_info.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.940091 dbgpt-0.5.6rc0/dbgpt/datasource/manages/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      157 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/manages/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9173 2024-03-28 01:32:30.000000 dbgpt-0.5.6rc0/dbgpt/datasource/manages/connect_config_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8623 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/datasource/manages/connector_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.940902 dbgpt-0.5.6rc0/dbgpt/datasource/nosql/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/nosql/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.942250 dbgpt-0.5.6rc0/dbgpt/datasource/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      128 2024-03-28 01:32:23.000000 dbgpt-0.5.6rc0/dbgpt/datasource/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      770 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/operators/datasource_operator.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.951460 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    23230 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12710 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_clickhouse.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6407 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_doris.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2473 2024-03-25 06:53:38.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_duckdb.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1417 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_hive.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1329 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_mssql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      295 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_mysql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8185 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_postgresql.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9677 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_sqlite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5681 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_starrocks.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.952403 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       33 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.953368 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      648 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.955106 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      820 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3186 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7507 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      116 2024-03-22 07:58:44.000000 dbgpt-0.5.6rc0/dbgpt/datasource/redis.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.958311 dbgpt-0.5.6rc0/dbgpt/model/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      320 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.968349 dbgpt-0.5.6rc0/dbgpt/model/adapter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19868 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3589 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/embeddings_loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8687 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/fschat_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11521 2024-04-22 03:12:53.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/hf_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    15595 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5520 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/model_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    17037 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/old_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10399 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/proxy_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3587 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3495 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/adapter/vllm_adapter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3050 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13971 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/cli.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.969947 dbgpt-0.5.6rc0/dbgpt/model/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      341 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4981 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/model/operators/llm_operator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18176 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/parameter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.971605 dbgpt-0.5.6rc0/dbgpt/model/proxy/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1096 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7967 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.983222 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      306 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3077 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/baichuan.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)     2325 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/bard.py
+-rwxr-xr-x   0 staneyffer   (501) staff       (20)    10636 2024-04-10 19:49:14.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/chatgpt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/claude.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6485 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/gemini.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3336 2024-04-10 19:49:14.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/moonshot.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3279 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/ollama.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1350 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/proxy_model.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7602 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/spark.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3720 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/tongyi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7011 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/wenxin.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2859 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/yi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3796 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/zhipu.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.986533 dbgpt-0.5.6rc0/dbgpt/model/utils/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9274 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/chatgpt_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2365 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/llm_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3101 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/model/utils/token_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.988231 dbgpt-0.5.6rc0/dbgpt/rag/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      200 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.992159 dbgpt-0.5.6rc0/dbgpt/rag/assembler/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      431 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2648 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4815 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4199 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4611 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/assembler/summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6792 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/chunk_manager.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.995761 dbgpt-0.5.6rc0/dbgpt/rag/embedding/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      771 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1167 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/_wrapped.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8826 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/embedding_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    28119 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/embedding/embeddings.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.997994 dbgpt-0.5.6rc0/dbgpt/rag/evaluation/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      271 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/evaluation/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8772 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/evaluation/retriever.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.000176 dbgpt-0.5.6rc0/dbgpt/rag/extractor/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      152 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/extractor/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1314 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/extractor/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6352 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/extractor/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.000914 dbgpt-0.5.6rc0/dbgpt/rag/graph/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       28 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/graph/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.009299 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1338 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5582 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3541 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/csv.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2389 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2580 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/docx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6600 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3024 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/html.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       22 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/json.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2600 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/markdown.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3378 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pdf.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pptx.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/string.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2504 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/txt.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2143 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/knowledge/url.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.014824 dbgpt-0.5.6rc0/dbgpt/rag/operators/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      971 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      654 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/assembler.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      743 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/datasource.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2956 2024-03-28 01:32:23.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6584 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2085 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/evaluation.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4534 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/knowledge.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1268 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3199 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1466 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/schema_linking.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4156 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/operators/summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.018875 dbgpt-0.5.6rc0/dbgpt/rag/retriever/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      503 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4379 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7270 2024-04-10 06:34:08.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/db_schema.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8888 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/embedding.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7113 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/rerank.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5223 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/rewrite.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5186 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/rag/retriever/time_weighted.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.020831 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       30 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1624 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/base_linker.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3392 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/schema_linking.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.023830 dbgpt-0.5.6rc0/dbgpt/rag/summary/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      420 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1226 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5210 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary_client.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4575 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/gdbms_db_summary.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4443 2024-04-13 17:38:21.000000 dbgpt-0.5.6rc0/dbgpt/rag/summary/rdbms_db_summary.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.026406 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      539 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1497 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/pre_text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    32461 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/text_splitter.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6913 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/token_splitter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.027754 dbgpt-0.5.6rc0/dbgpt/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       67 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.031269 dbgpt-0.5.6rc0/dbgpt/storage/cache/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      384 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)       24 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/embedding_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6185 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/llm_cache.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4472 2024-04-17 10:41:53.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9995 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/operators.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.031896 dbgpt-0.5.6rc0/dbgpt/storage/cache/protocol/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       27 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/protocol/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.032930 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       47 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8913 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.034108 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       41 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3254 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/disk_storage.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.035844 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      438 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4736 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/chat_history_db.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5829 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/chat_history/storage_adapter.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.039514 dbgpt-0.5.6rc0/dbgpt/storage/metadata/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      476 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9345 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/_base_dao.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1041 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_factory.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18854 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_manager.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5503 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1892 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/schema.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.046483 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1173 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7923 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8233 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/chroma_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7445 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/connector.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1234 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/filters.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    21229 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/milvus_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    29140 2024-04-30 09:57:48.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/oceanbase_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3440 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/pgvector_store.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     6727 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/storage/vector_store/weaviate_store.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.069856 dbgpt-0.5.6rc0/dbgpt/util/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      413 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    14058 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/_db_migration_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3861 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/annotations.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4659 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/api_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.070516 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/__init__.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.071495 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10778 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9317 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1703 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/chat_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    19326 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/code_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5840 2024-04-12 06:30:46.000000 dbgpt-0.5.6rc0/dbgpt/util/command_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1791 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/config_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.072630 dbgpt-0.5.6rc0/dbgpt/util/configure/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       56 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/configure/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     4719 2024-05-06 03:51:05.000000 dbgpt-0.5.6rc0/dbgpt/util/configure/base.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.074252 dbgpt-0.5.6rc0/dbgpt/util/console/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       70 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/util/console/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1827 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/util/console/console.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      780 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/custom_data_structure.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      247 2024-04-09 19:22:04.000000 dbgpt-0.5.6rc0/dbgpt/util/date_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.077668 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1936 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5982 2024-03-27 07:42:00.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11198 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/loader.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    11883 2024-04-15 03:42:53.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/repo.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    10560 2024-04-15 03:42:53.000000 dbgpt-0.5.6rc0/dbgpt/util/dbgpts/template.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      533 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/error_types.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2886 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/executor_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3929 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/fastapi.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1807 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/formatting.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3340 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/function_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    12937 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/global_helper.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1976 2024-03-25 14:27:11.000000 dbgpt-0.5.6rc0/dbgpt/util/i18n_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2612 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/id_generator.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3673 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/util/json_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      238 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/memory_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2679 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/model_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      893 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/module_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      704 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/net_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.078464 dbgpt-0.5.6rc0/dbgpt/util/network/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/util/network/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     9818 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/network/_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3488 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/openai_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      618 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/pagination_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    27652 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/parameter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      105 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/path_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      629 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/pd_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     8747 2024-04-20 08:03:41.000000 dbgpt-0.5.6rc0/dbgpt/util/prompt_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1676 2024-04-18 02:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/retry.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.079322 dbgpt-0.5.6rc0/dbgpt/util/serialization/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/serialization/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1859 2024-04-17 10:39:42.000000 dbgpt-0.5.6rc0/dbgpt/util/serialization/json_serialization.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2399 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/similarity_util.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      697 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/singleton.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.083752 dbgpt-0.5.6rc0/dbgpt/util/speech/
+-rw-r--r--   0 staneyffer   (501) staff       (20)        0 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1119 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1180 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/brian.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2985 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/eleven_labs.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      467 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/gtts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      523 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/macos_tts.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1441 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/speech/say.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     2526 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/splitter_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3006 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/util/string_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7537 2024-04-09 19:22:18.000000 dbgpt-0.5.6rc0/dbgpt/util/system_utils.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1019 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/dbgpt/util/time_utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.088031 dbgpt-0.5.6rc0/dbgpt/util/tracer/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      723 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7264 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5743 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/span_storage.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)    18465 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_cli.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     7846 2024-04-17 04:06:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_impl.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1504 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_middleware.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5246 2024-03-22 07:58:45.000000 dbgpt-0.5.6rc0/dbgpt/util/utils.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.089932 dbgpt-0.5.6rc0/dbgpt/vis/
+-rw-r--r--   0 staneyffer   (501) staff       (20)      602 2024-04-11 14:37:18.000000 dbgpt-0.5.6rc0/dbgpt/vis/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1050 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/base.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1220 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/client.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:51.094192 dbgpt-0.5.6rc0/dbgpt/vis/tags/
+-rw-r--r--   0 staneyffer   (501) staff       (20)       16 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/__init__.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      284 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_agent_message.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      257 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_agent_plans.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     3080 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_chart.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      256 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_code.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)     1957 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_dashboard.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      258 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_gpts_execution.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      311 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_gpts_result.py
+-rw-r--r--   0 staneyffer   (501) staff       (20)      253 2024-04-10 14:49:01.000000 dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_plugin.py
+drwxr-xr-x   0 staneyffer   (501) staff       (20)        0 2024-05-06 06:24:50.811025 dbgpt-0.5.6rc0/dbgpt.egg-info/
+-rw-r--r--   0 staneyffer   (501) staff       (20)    31466 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/PKG-INFO
+-rw-r--r--   0 staneyffer   (501) staff       (20)    13441 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        1 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       53 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/entry_points.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)     5169 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/requires.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)        6 2024-05-06 06:24:50.000000 dbgpt-0.5.6rc0/dbgpt.egg-info/top_level.txt
+-rw-r--r--   0 staneyffer   (501) staff       (20)       38 2024-05-06 06:24:51.134553 dbgpt-0.5.6rc0/setup.cfg
+-rw-r--r--   0 staneyffer   (501) staff       (20)    24345 2024-05-06 03:11:54.000000 dbgpt-0.5.6rc0/setup.py
```

### Comparing `dbgpt-0.5.5rc0/LICENSE` & `dbgpt-0.5.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/PKG-INFO` & `dbgpt-0.5.6rc0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.5rc0
+Version: 0.5.6rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -12,137 +12,144 @@
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
+Requires-Dist: snowflake-id
 Provides-Extra: core
-Requires-Dist: chardet==5.1.0; extra == "core"
-Requires-Dist: importlib-resources==5.12.0; extra == "core"
 Requires-Dist: cachetools; extra == "core"
-Requires-Dist: typeguard; extra == "core"
-Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: importlib-resources==5.12.0; extra == "core"
 Requires-Dist: python-dotenv==1.0.0; extra == "core"
+Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: snowflake-id; extra == "core"
+Requires-Dist: chardet==5.1.0; extra == "core"
+Requires-Dist: typeguard; extra == "core"
 Requires-Dist: pydantic>=2.6.0; extra == "core"
 Provides-Extra: client
-Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: cachetools; extra == "client"
+Requires-Dist: fastapi>=0.100.0; extra == "client"
 Requires-Dist: httpx; extra == "client"
 Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: fastapi>=0.100.0; extra == "client"
-Requires-Dist: cachetools; extra == "client"
-Requires-Dist: typeguard; extra == "client"
-Requires-Dist: aiohttp==3.8.4; extra == "client"
 Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: aiohttp==3.8.4; extra == "client"
+Requires-Dist: snowflake-id; extra == "client"
+Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: typeguard; extra == "client"
 Requires-Dist: pydantic>=2.6.0; extra == "client"
 Provides-Extra: cli
-Requires-Dist: click; extra == "cli"
-Requires-Dist: chardet==5.1.0; extra == "cli"
-Requires-Dist: httpx; extra == "cli"
+Requires-Dist: cachetools; extra == "cli"
+Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
 Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: python-dotenv==1.0.0; extra == "cli"
 Requires-Dist: prettytable; extra == "cli"
-Requires-Dist: cachetools; extra == "cli"
-Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: rich; extra == "cli"
-Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: snowflake-id; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: rich; extra == "cli"
+Requires-Dist: click; extra == "cli"
+Requires-Dist: chardet==5.1.0; extra == "cli"
+Requires-Dist: typeguard; extra == "cli"
 Requires-Dist: pydantic>=2.6.0; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: click; extra == "agent"
-Requires-Dist: chardet==5.1.0; extra == "agent"
-Requires-Dist: httpx; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: psutil==5.9.4; extra == "agent"
 Requires-Dist: tomlkit; extra == "agent"
 Requires-Dist: termcolor; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
 Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: prettytable; extra == "agent"
-Requires-Dist: cachetools; extra == "agent"
-Requires-Dist: typeguard; extra == "agent"
-Requires-Dist: pandas==2.0.3; extra == "agent"
-Requires-Dist: rich; extra == "agent"
-Requires-Dist: psutil==5.9.4; extra == "agent"
 Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: snowflake-id; extra == "agent"
 Requires-Dist: colorama==0.4.6; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: rich; extra == "agent"
+Requires-Dist: click; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: typeguard; extra == "agent"
 Requires-Dist: pydantic>=2.6.0; extra == "agent"
 Provides-Extra: simple-framework
-Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: schedule; extra == "simple-framework"
+Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
 Requires-Dist: msgpack; extra == "simple-framework"
-Requires-Dist: uvicorn; extra == "simple-framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: typeguard; extra == "simple-framework"
+Requires-Dist: termcolor; extra == "simple-framework"
 Requires-Dist: rich; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: colorama==0.4.6; extra == "simple-framework"
-Requires-Dist: pympler; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: shortuuid; extra == "simple-framework"
+Requires-Dist: typeguard; extra == "simple-framework"
 Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
-Requires-Dist: schedule; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
-Requires-Dist: httpx; extra == "simple-framework"
-Requires-Dist: tomlkit; extra == "simple-framework"
 Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
 Requires-Dist: psutil==5.9.4; extra == "simple-framework"
-Requires-Dist: termcolor; extra == "simple-framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
 Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
+Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: click; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
 Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: uvicorn; extra == "simple-framework"
+Requires-Dist: httpx; extra == "simple-framework"
 Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
+Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: snowflake-id; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: shortuuid; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
 Provides-Extra: framework
-Requires-Dist: click; extra == "framework"
-Requires-Dist: fschat; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: sqlparse==0.4.4; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
 Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "framework"
-Requires-Dist: typeguard; extra == "framework"
-Requires-Dist: rich; extra == "framework"
-Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
 Requires-Dist: alembic==1.12.0; extra == "framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
-Requires-Dist: coloredlogs; extra == "framework"
-Requires-Dist: aiofiles; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: rich; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: typeguard; extra == "framework"
 Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: fastapi>=0.100.0; extra == "framework"
-Requires-Dist: GitPython; extra == "framework"
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: pymysql; extra == "framework"
 Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
-Requires-Dist: pydantic>=2.6.0; extra == "framework"
 Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "framework"
 Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
+Requires-Dist: fschat; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
+Requires-Dist: click; extra == "framework"
+Requires-Dist: duckdb-engine; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
 Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: uvicorn; extra == "framework"
+Requires-Dist: auto-gpt-plugin-template; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
+Requires-Dist: coloredlogs; extra == "framework"
 Requires-Dist: python-dotenv==1.0.0; extra == "framework"
-Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: snowflake-id; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: aiofiles; extra == "framework"
+Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
 Requires-Dist: duckdb; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: pydantic>=2.6.0; extra == "framework"
 Provides-Extra: torch
 Requires-Dist: torchvision==0.17.1; extra == "torch"
 Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
 Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
 Requires-Dist: torch==2.2.1; extra == "torch-cpu"
@@ -153,253 +160,262 @@
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
 Requires-Dist: cpm_kernels; extra == "quantization"
+Requires-Dist: bitsandbytes; extra == "quantization"
 Provides-Extra: vstore
 Requires-Dist: chromadb>=0.4.22; extra == "vstore"
 Provides-Extra: vstore-weaviate
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
 Requires-Dist: weaviate-client; extra == "vstore-weaviate"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
 Provides-Extra: vstore-milvus
 Requires-Dist: pymilvus; extra == "vstore-milvus"
 Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
 Provides-Extra: vstore-all
 Requires-Dist: pymilvus; extra == "vstore-all"
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Requires-Dist: weaviate-client; extra == "vstore-all"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
+Requires-Dist: pymysql; extra == "datasource-all"
+Requires-Dist: thrift; extra == "datasource-all"
 Requires-Dist: pymssql; extra == "datasource-all"
-Requires-Dist: pyspark; extra == "datasource-all"
 Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: thrift_sasl; extra == "datasource-all"
-Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
+Requires-Dist: neo4j; extra == "datasource-all"
 Requires-Dist: pyhive; extra == "datasource-all"
-Requires-Dist: pymysql; extra == "datasource-all"
-Requires-Dist: thrift; extra == "datasource-all"
 Requires-Dist: psycopg2; extra == "datasource-all"
+Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
+Requires-Dist: pyspark; extra == "datasource-all"
 Provides-Extra: rag
-Requires-Dist: pypdf; extra == "rag"
-Requires-Dist: python-pptx; extra == "rag"
-Requires-Dist: python-docx; extra == "rag"
-Requires-Dist: spacy>=3.7; extra == "rag"
+Requires-Dist: bs4; extra == "rag"
 Requires-Dist: markdown; extra == "rag"
-Requires-Dist: python-multipart; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: sentence-transformers; extra == "rag"
-Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: bs4; extra == "rag"
+Requires-Dist: python-pptx; extra == "rag"
+Requires-Dist: python-docx; extra == "rag"
+Requires-Dist: pypdf; extra == "rag"
 Requires-Dist: chromadb>=0.4.22; extra == "rag"
+Requires-Dist: langchain>=0.0.286; extra == "rag"
+Requires-Dist: python-multipart; extra == "rag"
 Provides-Extra: openai
-Requires-Dist: click; extra == "openai"
-Requires-Dist: fschat; extra == "openai"
-Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: importlib-resources==5.12.0; extra == "openai"
-Requires-Dist: typeguard; extra == "openai"
-Requires-Dist: rich; extra == "openai"
-Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: spacy>=3.7; extra == "openai"
-Requires-Dist: pymysql; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: sqlparse==0.4.4; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
 Requires-Dist: markdown; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
+Requires-Dist: msgpack; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: sentence-transformers; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
 Requires-Dist: alembic==1.12.0; extra == "openai"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: coloredlogs; extra == "openai"
-Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: rich; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
 Requires-Dist: pypdf; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: chromadb>=0.4.22; extra == "openai"
+Requires-Dist: typeguard; extra == "openai"
 Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: python-multipart; extra == "openai"
-Requires-Dist: bs4; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: chromadb>=0.4.22; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
-Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: pymysql; extra == "openai"
 Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
-Requires-Dist: pydantic>=2.6.0; extra == "openai"
 Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: sentence-transformers; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
-Requires-Dist: openai; extra == "openai"
+Requires-Dist: importlib-resources==5.12.0; extra == "openai"
 Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: fschat; extra == "openai"
 Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
+Requires-Dist: click; extra == "openai"
+Requires-Dist: duckdb-engine; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: uvicorn; extra == "openai"
+Requires-Dist: auto-gpt-plugin-template; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
+Requires-Dist: coloredlogs; extra == "openai"
 Requires-Dist: python-dotenv==1.0.0; extra == "openai"
-Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
+Requires-Dist: snowflake-id; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: langchain>=0.0.286; extra == "openai"
+Requires-Dist: openai; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: bs4; extra == "openai"
 Requires-Dist: duckdb; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: pydantic>=2.6.0; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
-Requires-Dist: click; extra == "default"
-Requires-Dist: fschat; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
-Requires-Dist: msgpack; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
-Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
-Requires-Dist: typeguard; extra == "default"
-Requires-Dist: rich; extra == "default"
-Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: spacy>=3.7; extra == "default"
-Requires-Dist: pymysql; extra == "default"
+Requires-Dist: schedule; extra == "default"
+Requires-Dist: sqlparse==0.4.4; extra == "default"
+Requires-Dist: seaborn; extra == "default"
 Requires-Dist: markdown; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: rocksdict; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: pympler; extra == "default"
+Requires-Dist: msgpack; extra == "default"
+Requires-Dist: termcolor; extra == "default"
+Requires-Dist: sentence-transformers; extra == "default"
 Requires-Dist: alembic==1.12.0; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: coloredlogs; extra == "default"
-Requires-Dist: aiofiles; extra == "default"
+Requires-Dist: rich; extra == "default"
+Requires-Dist: ollama; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
 Requires-Dist: pypdf; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: chromadb>=0.4.22; extra == "default"
+Requires-Dist: cpm_kernels; extra == "default"
+Requires-Dist: typeguard; extra == "default"
 Requires-Dist: jinja2; extra == "default"
-Requires-Dist: fastapi>=0.100.0; extra == "default"
 Requires-Dist: python-multipart; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: schedule; extra == "default"
-Requires-Dist: GitPython; extra == "default"
-Requires-Dist: chromadb>=0.4.22; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
-Requires-Dist: httpx; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
-Requires-Dist: python-docx; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: pymysql; extra == "default"
 Requires-Dist: cachetools; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: dashscope; extra == "default"
-Requires-Dist: pydantic>=2.6.0; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
-Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: termcolor; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: dashscope; extra == "default"
+Requires-Dist: importlib-resources==5.12.0; extra == "default"
 Requires-Dist: prettytable; extra == "default"
-Requires-Dist: sqlparse==0.4.4; extra == "default"
 Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
+Requires-Dist: fschat; extra == "default"
+Requires-Dist: zhipuai; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
 Requires-Dist: graphviz; extra == "default"
-Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: click; extra == "default"
+Requires-Dist: duckdb-engine; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
 Requires-Dist: jsonschema; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: pympler; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: httpx; extra == "default"
+Requires-Dist: coloredlogs; extra == "default"
+Requires-Dist: tokenizers>=0.14; extra == "default"
 Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: snowflake-id; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: aiofiles; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: GitPython; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: langchain>=0.0.286; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: bs4; extra == "default"
 Requires-Dist: duckdb; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
+Requires-Dist: python-pptx; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: bitsandbytes; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
 Provides-Extra: all
-Requires-Dist: click; extra == "all"
-Requires-Dist: fschat; extra == "all"
+Requires-Dist: sqlparse==0.4.4; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: msgpack; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: auto-gpt-plugin-template; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: GitPython; extra == "all"
 Requires-Dist: gTTS==2.3.1; extra == "all"
 Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: duckdb; extra == "all"
+Requires-Dist: pydantic>=2.6.0; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: vllm; extra == "all"
+Requires-Dist: httpx; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: snowflake-id; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
+Requires-Dist: pyspark; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
 Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: neo4j; extra == "all"
+Requires-Dist: typeguard; extra == "all"
 Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: pymysql; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
 Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: pypdf; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: pympler; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
 Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: bs4; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: ollama; extra == "all"
 Requires-Dist: chromadb>=0.4.22; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: pymysql; extra == "all"
 Requires-Dist: cachetools; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: spacy>=3.7; extra == "all"
-Requires-Dist: pympler; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: fschat; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
 Requires-Dist: fastapi>=0.100.0; extra == "all"
-Requires-Dist: schedule; extra == "all"
 Requires-Dist: python-docx; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: pydantic>=2.6.0; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: msgpack; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: rich; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -553,14 +569,19 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Qwen1.5-110B-Chat](https://huggingface.co/Qwen/Qwen1.5-110B-Chat)
+    - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
+    - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
+    - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
+    - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
```

### Comparing `dbgpt-0.5.5rc0/README.md` & `dbgpt-0.5.6rc0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -154,14 +154,19 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Qwen1.5-110B-Chat](https://huggingface.co/Qwen/Qwen1.5-110B-Chat)
+    - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
+    - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
+    - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
+    - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
```

#### html2text {}

```diff
@@ -99,40 +99,46 @@
 tuning lightweight framework centred on large language models (LLMs), Text2SQL
 datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework
 simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly
 line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) - **SMMF
 (Service-oriented Multi-model Management Framework)** We offer extensive model
 support, including dozens of large language models (LLMs) from both open-source
 and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu,
-and many more. - News - ð¥ð¥ð¥ [Qwen1.5-32B-Chat](https://huggingface.co/
-Qwen/Qwen1.5-32B-Chat) - ð¥ð¥ð¥ [Starling-LM-7B-beta](https://
-huggingface.co/Nexusflow/Starling-LM-7B-beta) - ð¥ð¥ð¥ [gemma-7b-it]
-(https://huggingface.co/google/gemma-7b-it) - ð¥ð¥ð¥ [gemma-2b-it](https:
-//huggingface.co/google/gemma-2b-it) - ð¥ð¥ð¥ [SOLAR-10.7B](https://
-huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0) - ð¥ð¥ð¥ [Mixtral-8x7B]
-(https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1) - ð¥ð¥ð¥
-[Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat) - ð¥ð¥ð¥ [Yi-
-34B-Chat](https://huggingface.co/01-ai/Yi-34B-Chat) - [More Supported LLMs]
-(http://docs.dbgpt.site/docs/modules/smmf) - **Privacy and Security** We ensure
-the privacy and security of data through the implementation of various
-technologies, including privatized large models and proxy desensitization. -
-Support Datasources - [Datasources](http://docs.dbgpt.site/docs/modules/
-connections) ## Image ð [AutoDL Image](https://www.codewithgpu.com/i/
-eosphoros-ai/DB-GPT/dbgpt) ### Language Switching In the .env configuration
-file, modify the LANGUAGE parameter to switch to different languages. The
-default is English (Chinese: zh, English: en, other languages to be added
-later). ## Contribution - To check detailed guidelines for new contributions,
-please refer [how to contribute](https://github.com/eosphoros-ai/DB-GPT/blob/
-main/CONTRIBUTING.md) ### Contributors Wall _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
-_i_m_a_g_e_?_r_e_p_o_=_e_o_s_p_h_o_r_o_s_-_a_i_/_D_B_-_G_P_T_&_m_a_x_=_2_0_0_]## Licence The MIT License (MIT) ##
-Citation If you find `DB-GPT` useful for your research or development, please
-cite the following _p_a_p_e_r: ```bibtex @article{xue2023dbgpt, title={DB-GPT:
-Empowering Database Interactions with Private Large Language Models}, author=
-{Siqiao Xue and Caigao Jiang and Wenhui Shi and Fangyin Cheng and Keting Chen
-and Hongjun Yang and Zhiping Zhang and Jianshan He and Hongyang Zhang and
+and many more. - News - ð¥ð¥ð¥ [Qwen1.5-110B-Chat](https://
+huggingface.co/Qwen/Qwen1.5-110B-Chat) - ð¥ð¥ð¥ [Qwen1.5-MoE-A2.7B-Chat]
+(https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat) - ð¥ð¥ð¥ [Meta-
+Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-
+Instruct) - ð¥ð¥ð¥ [Meta-Llama-3-8B-Instruct](https://huggingface.co/
+meta-llama/Meta-Llama-3-8B-Instruct) - ð¥ð¥ð¥ [CodeQwen1.5-7B-Chat]
+(https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat) - ð¥ð¥ð¥ [Qwen1.5-32B-
+Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat) - ð¥ð¥ð¥ [Starling-
+LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta) -
+ð¥ð¥ð¥ [gemma-7b-it](https://huggingface.co/google/gemma-7b-it) -
+ð¥ð¥ð¥ [gemma-2b-it](https://huggingface.co/google/gemma-2b-it) -
+ð¥ð¥ð¥ [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-
+v1.0) - ð¥ð¥ð¥ [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-
+8x7B-Instruct-v0.1) - ð¥ð¥ð¥ [Qwen-72B-Chat](https://huggingface.co/Qwen/
+Qwen-72B-Chat) - ð¥ð¥ð¥ [Yi-34B-Chat](https://huggingface.co/01-ai/Yi-
+34B-Chat) - [More Supported LLMs](http://docs.dbgpt.site/docs/modules/smmf) -
+**Privacy and Security** We ensure the privacy and security of data through the
+implementation of various technologies, including privatized large models and
+proxy desensitization. - Support Datasources - [Datasources](http://
+docs.dbgpt.site/docs/modules/connections) ## Image ð [AutoDL Image](https://
+www.codewithgpu.com/i/eosphoros-ai/DB-GPT/dbgpt) ### Language Switching In the
+.env configuration file, modify the LANGUAGE parameter to switch to different
+languages. The default is English (Chinese: zh, English: en, other languages to
+be added later). ## Contribution - To check detailed guidelines for new
+contributions, please refer [how to contribute](https://github.com/eosphoros-
+ai/DB-GPT/blob/main/CONTRIBUTING.md) ### Contributors Wall _[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_e_o_s_p_h_o_r_o_s_-_a_i_/_D_B_-_G_P_T_&_m_a_x_=_2_0_0_]## Licence The MIT License
+(MIT) ## Citation If you find `DB-GPT` useful for your research or development,
+please cite the following _p_a_p_e_r: ```bibtex @article{xue2023dbgpt, title={DB-
+GPT: Empowering Database Interactions with Private Large Language Models},
+author={Siqiao Xue and Caigao Jiang and Wenhui Shi and Fangyin Cheng and Keting
+Chen and Hongjun Yang and Zhiping Zhang and Jianshan He and Hongyang Zhang and
 Ganglin Wei and Wang Zhao and Fan Zhou and Danrui Qi and Hong Yi and Shaodong
 Liu and Faqiang Chen}, year={2023}, journal={arXiv preprint arXiv:2312.17449},
 url={https://arxiv.org/abs/2312.17449} } ``` ## Contact Information We are
 working on building a community, if you have any ideas for building the
 community, feel free to contact us. [![](https://dcbadge.vercel.app/api/server/
 7uQnPuveTY?compact=true&style=flat)](https://discord.gg/7uQnPuveTY) [![Star
 History Chart](https://api.star-history.com/svg?repos=csunny/DB-GPT&type=Date)]
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/_private/config.py` & `dbgpt-0.5.6rc0/dbgpt/_private/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,14 +234,26 @@
         ### Vector Store Configuration
         self.VECTOR_STORE_TYPE = os.getenv("VECTOR_STORE_TYPE", "Chroma")
         self.MILVUS_URL = os.getenv("MILVUS_URL", "127.0.0.1")
         self.MILVUS_PORT = os.getenv("MILVUS_PORT", "19530")
         self.MILVUS_USERNAME = os.getenv("MILVUS_USERNAME", None)
         self.MILVUS_PASSWORD = os.getenv("MILVUS_PASSWORD", None)
 
+        ## OceanBase Configuration
+        self.OB_HOST = os.getenv("OB_HOST", "127.0.0.1")
+        self.OB_PORT = int(os.getenv("OB_PORT", "2881"))
+        self.OB_USER = os.getenv("OB_USER", "root")
+        self.OB_PASSWORD = os.getenv("OB_PASSWORD", "")
+        self.OB_DATABASE = os.getenv("OB_DATABASE", "test")
+        self.OB_SQL_DBG_LOG_PATH = os.getenv("OB_SQL_DBG_LOG_PATH", "")
+        self.OB_ENABLE_NORMALIZE_VECTOR = bool(
+            os.getenv("OB_ENABLE_NORMALIZE_VECTOR", "")
+        )
+        self.OB_ENABLE_INDEX = bool(os.getenv("OB_ENABLE_INDEX", ""))
+
         # QLoRA
         self.QLoRA = os.getenv("QUANTIZE_QLORA", "True")
         self.IS_LOAD_8BIT = os.getenv("QUANTIZE_8bit", "True").lower() == "true"
         self.IS_LOAD_4BIT = os.getenv("QUANTIZE_4bit", "False").lower() == "true"
         if self.IS_LOAD_8BIT and self.IS_LOAD_4BIT:
             self.IS_LOAD_8BIT = False
         # In order to be compatible with the new and old model parameter design
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/_private/llm_metadata.py` & `dbgpt-0.5.6rc0/dbgpt/_private/llm_metadata.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/_private/pydantic.py` & `dbgpt-0.5.6rc0/dbgpt/_private/pydantic.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/agent/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """DB-GPT Multi-Agents Module."""
 
-from .actions.action import Action, ActionOutput  # noqa: F401
+from .core.action import *  # noqa: F401, F403
 from .core.agent import (  # noqa: F401
     Agent,
     AgentContext,
     AgentGenerateContext,
     AgentMessage,
 )
 from .core.agent_manage import (  # noqa: F401
     AgentManager,
     get_agent_manager,
     initialize_agent,
 )
 from .core.base_agent import ConversableAgent  # noqa: F401
-from .core.llm.llm import LLMConfig  # noqa: F401
+from .core.memory import *  # noqa: F401, F403
+from .core.memory.gpts.gpts_memory import GptsMemory  # noqa: F401
+from .core.plan import *  # noqa: F401, F403
+from .core.profile import *  # noqa: F401, F403
 from .core.schema import PluginStorageType  # noqa: F401
 from .core.user_proxy_agent import UserProxyAgent  # noqa: F401
-from .memory.gpts_memory import GptsMemory  # noqa: F401
 from .resource.resource_api import AgentResource, ResourceType  # noqa: F401
 from .resource.resource_loader import ResourceLoader  # noqa: F401
+from .util.llm.llm import LLMConfig  # noqa: F401
 
 __ALL__ = [
     "Agent",
     "AgentContext",
     "AgentGenerateContext",
     "AgentMessage",
     "AgentManager",
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/actions/action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/action/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Base Action class for defining agent actions."""
+
 import json
 from abc import ABC, abstractmethod
 from typing import (
     Any,
     Dict,
     Generic,
     List,
@@ -17,34 +18,49 @@
 
 from dbgpt._private.pydantic import (
     BaseModel,
     field_default,
     field_description,
     model_fields,
     model_to_dict,
+    model_validator,
 )
 from dbgpt.util.json_utils import find_json_objects
+from dbgpt.vis.base import Vis
 
-from ...vis.base import Vis
-from ..resource.resource_api import AgentResource, ResourceType
-from ..resource.resource_loader import ResourceLoader
+from ...resource.resource_api import AgentResource, ResourceType
+from ...resource.resource_loader import ResourceLoader
 
 T = TypeVar("T", bound=Union[BaseModel, List[BaseModel], None])
 
 JsonMessageType = Union[Dict[str, Any], List[Dict[str, Any]]]
 
 
 class ActionOutput(BaseModel):
     """Action output model."""
 
     content: str
     is_exe_success: bool = True
     view: Optional[str] = None
     resource_type: Optional[str] = None
     resource_value: Optional[Any] = None
+    action: Optional[str] = None
+    thoughts: Optional[str] = None
+    observations: Optional[str] = None
+
+    @model_validator(mode="before")
+    @classmethod
+    def pre_fill(cls, values: Any) -> Any:
+        """Pre-fill the values."""
+        if not isinstance(values, dict):
+            return values
+        is_exe_success = values.get("is_exe_success", True)
+        if not is_exe_success and "observations" not in values:
+            values["observations"] = values.get("content")
+        return values
 
     @classmethod
     def from_dict(
         cls: Type["ActionOutput"], param: Optional[Dict]
     ) -> Optional["ActionOutput"]:
         """Convert dict to ActionOutput object."""
         if not param:
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/actions/blank_action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/action/blank_action.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Blank Action for the Agent."""
 
 import logging
 from typing import Optional
 
-from ..resource.resource_api import AgentResource
-from .action import Action, ActionOutput
+from ...resource.resource_api import AgentResource
+from .base import Action, ActionOutput
 
 logger = logging.getLogger(__name__)
 
 
 class BlankAction(Action):
     """Blank action class."""
 
@@ -29,8 +29,12 @@
         need_vis_render: bool = True,
         **kwargs,
     ) -> ActionOutput:
         """Perform the action.
 
         Just return the AI message.
         """
-        return ActionOutput(is_exe_success=True, content=ai_message, view=ai_message)
+        return ActionOutput(
+            is_exe_success=True,
+            content=ai_message,
+            view=ai_message,
+        )
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/actions/chart_action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/chart_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Chart Action for SQL execution and rendering."""
+
 import json
 import logging
 from typing import Optional
 
 from dbgpt._private.pydantic import BaseModel, Field, model_to_json
 from dbgpt.vis.tags.vis_chart import Vis, VisChart
 
-from ..resource.resource_api import AgentResource, ResourceType
-from ..resource.resource_db_api import ResourceDbClient
-from .action import Action, ActionOutput
+from ...core.action.base import Action, ActionOutput
+from ...resource.resource_api import AgentResource, ResourceType
+from ...resource.resource_db_api import ResourceDbClient
 
 logger = logging.getLogger(__name__)
 
 
 class SqlInput(BaseModel):
     """SQL input model."""
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/actions/code_action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/code_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Code Action Module."""
+
 import logging
 from typing import Optional, Union
 
 from dbgpt.util.code_utils import UNKNOWN, execute_code, extract_code, infer_lang
 from dbgpt.util.utils import colored
 from dbgpt.vis.tags.vis_code import Vis, VisCode
 
-from ..resource.resource_api import AgentResource
-from .action import Action, ActionOutput
+from ...core.action.base import Action, ActionOutput
+from ...resource.resource_api import AgentResource
 
 logger = logging.getLogger(__name__)
 
 
 class CodeAction(Action[None]):
     """Code Action Module."""
 
@@ -69,15 +70,21 @@
                 "language": code_blocks[0][0],
                 "code": code_blocks,
                 "log": logs,
             }
             if not self.render_protocol:
                 raise NotImplementedError("The render_protocol should be implemented.")
             view = await self.render_protocol.display(content=param)
-            return ActionOutput(is_exe_success=exit_success, content=content, view=view)
+            return ActionOutput(
+                is_exe_success=exit_success,
+                content=content,
+                view=view,
+                thoughts=ai_message,
+                observations=content,
+            )
         except Exception as e:
             logger.exception("Code Action Run Failed！")
             return ActionOutput(
                 is_exe_success=False, content="Code execution exception，" + str(e)
             )
 
     def execute_code_blocks(self, code_blocks):
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/actions/dashboard_action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/dashboard_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Dashboard Action Module."""
+
 import json
 import logging
 from typing import List, Optional
 
 from dbgpt._private.pydantic import BaseModel, Field, model_to_dict
 from dbgpt.vis.tags.vis_dashboard import Vis, VisDashboard
 
-from ..resource.resource_api import AgentResource, ResourceType
-from ..resource.resource_db_api import ResourceDbClient
-from .action import Action, ActionOutput
+from ...core.action.base import Action, ActionOutput
+from ...resource.resource_api import AgentResource, ResourceType
+from ...resource.resource_db_api import ResourceDbClient
 
 logger = logging.getLogger(__name__)
 
 
 class ChartItem(BaseModel):
     """Chart item model."""
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/actions/indicator_action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/indicator_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import json
 import logging
 from typing import Optional
 
 from dbgpt._private.pydantic import BaseModel, Field
 from dbgpt.vis.tags.vis_plugin import Vis, VisPlugin
 
-from ..core.schema import Status
-from ..resource.resource_api import AgentResource, ResourceType
-from .action import Action, ActionOutput
+from ...core.action.base import Action, ActionOutput
+from ...core.schema import Status
+from ...resource.resource_api import AgentResource, ResourceType
 
 logger = logging.getLogger(__name__)
 
 
 class IndicatorInput(BaseModel):
     """Indicator input model."""
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/actions/plugin_action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/actions/plugin_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Plugin Action Module."""
+
 import json
 import logging
 from typing import Optional
 
 from dbgpt._private.pydantic import BaseModel, Field
 from dbgpt.vis.tags.vis_plugin import Vis, VisPlugin
 
-from ..core.schema import Status
-from ..plugin.generator import PluginPromptGenerator
-from ..resource.resource_api import AgentResource, ResourceType
-from ..resource.resource_plugin_api import ResourcePluginClient
-from .action import Action, ActionOutput
+from ...core.action.base import Action, ActionOutput
+from ...core.schema import Status
+from ...plugin.generator import PluginPromptGenerator
+from ...resource.resource_api import AgentResource, ResourceType
+from ...resource.resource_plugin_api import ResourcePluginClient
 
 logger = logging.getLogger(__name__)
 
 
 class PluginInput(BaseModel):
     """Plugin input model."""
 
@@ -140,14 +141,17 @@
             }
             if not self.render_protocol:
                 raise NotImplementedError("The render_protocol should be implemented.")
 
             view = await self.render_protocol.display(content=plugin_param)
 
             return ActionOutput(
-                is_exe_success=response_success, content=tool_result, view=view
+                is_exe_success=response_success,
+                content=tool_result,
+                view=view,
+                observations=tool_result,
             )
         except Exception as e:
             logger.exception("Tool Action Run Failed！")
             return ActionOutput(
                 is_exe_success=False, content=f"Tool action run failed!{str(e)}"
             )
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/core/agent.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import dataclasses
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from dbgpt.core import LLMClient
 from dbgpt.util.annotations import PublicAPI
 
-from ..actions.action import ActionOutput
-from ..memory.gpts_memory import GptsMemory
 from ..resource.resource_loader import ResourceLoader
+from .action.base import ActionOutput
+from .memory.agent_memory import AgentMemory
 
 
 class Agent(ABC):
     """Agent Interface."""
 
     @abstractmethod
     async def send(
@@ -156,25 +156,28 @@
             **kwargs:
 
         Returns:
             Tuple[bool, Optional[str]]: whether the verification is successful and the
                 verification result.
         """
 
+    @property
     @abstractmethod
-    def get_name(self) -> str:
-        """Return name of the agent."""
+    def name(self) -> str:
+        """Return the name of the agent."""
 
+    @property
     @abstractmethod
-    def get_profile(self) -> str:
-        """Return profile of the agent."""
+    def role(self) -> str:
+        """Return the role of the agent."""
 
+    @property
     @abstractmethod
-    def get_describe(self) -> str:
-        """Return describe of the agent."""
+    def desc(self) -> Optional[str]:
+        """Return the description of the agent."""
 
 
 @dataclasses.dataclass
 class AgentContext:
     """A class to represent the context of an Agent."""
 
     conv_id: str
@@ -200,15 +203,15 @@
     sender: Optional[Agent] = None
     reviewer: Optional[Agent] = None
     silent: Optional[bool] = False
 
     rely_messages: List[AgentMessage] = dataclasses.field(default_factory=list)
     final: Optional[bool] = True
 
-    memory: Optional[GptsMemory] = None
+    memory: Optional[AgentMemory] = None
     agent_context: Optional[AgentContext] = None
     resource_loader: Optional[ResourceLoader] = None
     llm_client: Optional[LLMClient] = None
 
     round_index: Optional[int] = None
 
     def to_dict(self) -> Dict:
@@ -298,7 +301,13 @@
             action_report=copied_action_report,
             review_info=copied_review_info,
             current_goal=self.current_goal,
             model_name=self.model_name,
             role=self.role,
             success=self.success,
         )
+
+    def get_dict_context(self) -> Dict[str, Any]:
+        """Return the context as a dictionary."""
+        if isinstance(self.context, dict):
+            return self.context
+        return {}
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/core/agent_manage.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/agent_manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 def participant_roles(agents: List[Agent]) -> str:
     """Return a string listing the roles of the agents."""
     # Default to all agents registered
     roles = []
     for agent in agents:
-        roles.append(f"{agent.get_name()}: {agent.get_describe()}")
+        roles.append(f"{agent.name}: {agent.desc}")
     return "\n".join(roles)
 
 
 def mentioned_agents(message_content: str, agents: List[Agent]) -> Dict:
     """Return a dictionary mapping agent names to mention counts.
 
     Finds and counts agent mentions in the string message_content, taking word
@@ -30,21 +30,21 @@
 
     Returns: A dictionary mapping agent names to mention counts (to be included,
     at least one mention must occur)
     """
     mentions = dict()
     for agent in agents:
         regex = (
-            r"(?<=\W)" + re.escape(agent.get_name()) + r"(?=\W)"
+            r"(?<=\W)" + re.escape(agent.name) + r"(?=\W)"
         )  # Finds agent mentions, taking word boundaries into account
         count = len(
             re.findall(regex, " " + message_content + " ")
         )  # Pad the message to help with matching
         if count > 0:
-            mentions[agent.get_name()] = count
+            mentions[agent.name] = count
     return mentions
 
 
 class AgentManager(BaseComponent):
     """Manages the registration and retrieval of agents."""
 
     name = ComponentType.AGENT_MANAGER
@@ -80,15 +80,15 @@
         self._core_agents = core_agents
 
     def register_agent(
         self, cls: Type[ConversableAgent], ignore_duplicate: bool = False
     ) -> str:
         """Register an agent."""
         inst = cls()
-        profile = inst.get_profile()
+        profile = inst.role
         if profile in self._agents and (
             profile in self._core_agents or not ignore_duplicate
         ):
             raise ValueError(f"Agent:{profile} already register!")
         self._agents[profile] = (cls, inst)
         return profile
 
@@ -106,30 +106,30 @@
         """
         if name not in self._agents:
             raise ValueError(f"Agent:{name} not register!")
         return self._agents[name][0]
 
     def get_describe_by_name(self, name: str) -> str:
         """Return the description of an agent by name."""
-        return self._agents[name][1].desc
+        return self._agents[name][1].desc or ""
 
     def all_agents(self) -> Dict[str, str]:
         """Return a dictionary of all registered agents and their descriptions."""
         result = {}
         for name, value in self._agents.items():
-            result[name] = value[1].desc
+            result[name] = value[1].desc or ""
         return result
 
     def list_agents(self):
         """Return a list of all registered agents and their descriptions."""
         result = []
         for name, value in self._agents.items():
             result.append(
                 {
-                    "name": value[1].profile,
+                    "name": value[1].role,
                     "desc": value[1].goal,
                 }
             )
         return result
 
 
 _SYSTEM_APP: Optional[SystemApp] = None
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/core/base_agent.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/base_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,64 @@
 """Base agent class for conversable agents."""
 
 import asyncio
 import json
 import logging
-from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, Type, cast
 
 from dbgpt._private.pydantic import ConfigDict, Field
 from dbgpt.core import LLMClient, ModelMessageRoleType
 from dbgpt.util.error_types import LLMChatError
 from dbgpt.util.tracer import SpanType, root_tracer
 from dbgpt.util.utils import colored
 
-from ..actions.action import Action, ActionOutput
-from ..memory.base import GptsMessage
-from ..memory.gpts_memory import GptsMemory
 from ..resource.resource_api import AgentResource, ResourceClient
 from ..resource.resource_loader import ResourceLoader
+from ..util.llm.llm import LLMConfig, LLMStrategyType
+from ..util.llm.llm_client import AIWrapper
+from .action.base import Action, ActionOutput
 from .agent import Agent, AgentContext, AgentMessage, AgentReviewInfo
-from .llm.llm import LLMConfig, LLMStrategyType
-from .llm.llm_client import AIWrapper
+from .memory.agent_memory import AgentMemory
+from .memory.gpts.base import GptsMessage
+from .memory.gpts.gpts_memory import GptsMemory
 from .role import Role
 
 logger = logging.getLogger(__name__)
 
 
 class ConversableAgent(Role, Agent):
     """ConversableAgent is an agent that can communicate with other agents."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     agent_context: Optional[AgentContext] = Field(None, description="Agent context")
     actions: List[Action] = Field(default_factory=list)
     resources: List[AgentResource] = Field(default_factory=list)
     llm_config: Optional[LLMConfig] = None
-    memory: GptsMemory = Field(default_factory=GptsMemory)
     resource_loader: Optional[ResourceLoader] = None
     max_retry_count: int = 3
     consecutive_auto_reply_counter: int = 0
     llm_client: Optional[AIWrapper] = None
-    oai_system_message: List[Dict] = Field(default_factory=list)
 
     def __init__(self, **kwargs):
         """Create a new agent."""
         Role.__init__(self, **kwargs)
         Agent.__init__(self)
 
-    def init_system_message(self) -> None:
-        """Initialize the system message."""
-        content = self.prompt_template()
-        # TODO: Don't modify the original data, need to be optimized
-        self.oai_system_message = [
-            {"content": content, "role": ModelMessageRoleType.SYSTEM}
-        ]
-
     def check_available(self) -> None:
         """Check if the agent is available.
 
         Raises:
             ValueError: If the agent is not available.
         """
         self.identity_check()
         # check run context
         if self.agent_context is None:
             raise ValueError(
-                f"{self.name}[{self.profile}] Missing context in which agent is "
+                f"{self.name}[{self.role}] Missing context in which agent is "
                 f"running!"
             )
 
         # resource check
         for resource in self.resources:
             if (
                 self.resource_loader is None
@@ -86,28 +77,28 @@
             have_resource_types = [item.type for item in self.resources]
             for action in self.actions:
                 if (
                     action.resource_need
                     and action.resource_need not in have_resource_types
                 ):
                     raise ValueError(
-                        f"{self.name}[{self.profile}] Missing resources required for "
+                        f"{self.name}[{self.role}] Missing resources required for "
                         "runtime！"
                     )
         else:
             if not self.is_human and not self.is_team:
                 raise ValueError(
-                    f"This agent {self.name}[{self.profile}] is missing action modules."
+                    f"This agent {self.name}[{self.role}] is missing action modules."
                 )
         # llm check
         if not self.is_human and (
             self.llm_config is None or self.llm_config.llm_client is None
         ):
             raise ValueError(
-                f"{self.name}[{self.profile}] Model configuration is missing or model "
+                f"{self.name}[{self.role}] Model configuration is missing or model "
                 "service is unavailable！"
             )
 
     @property
     def not_null_agent_context(self) -> AgentContext:
         """Get the agent context.
 
@@ -157,56 +148,63 @@
 
         # Preload resources
         await self.preload_resource()
         # Initialize resource loader
         for action in self.actions:
             action.init_resource_loader(self.resource_loader)
 
-        # Initialize system messages
-        self.init_system_message()
-
         # Initialize LLM Server
         if not self.is_human:
             if not self.llm_config or not self.llm_config.llm_client:
                 raise ValueError("LLM client is not initialized！")
             self.llm_client = AIWrapper(llm_client=self.llm_config.llm_client)
+            self.memory.initialize(
+                self.name,
+                self.llm_config.llm_client,
+                importance_scorer=self.memory_importance_scorer,
+                insight_extractor=self.memory_insight_extractor,
+            )
+            # Clone the memory structure
+            self.memory = self.memory.structure_clone()
         return self
 
     def bind(self, target: Any) -> "ConversableAgent":
         """Bind the resources to the agent."""
         if isinstance(target, LLMConfig):
             self.llm_config = target
         elif isinstance(target, GptsMemory):
-            self.memory = target
+            raise ValueError("GptsMemory is not supported!")
         elif isinstance(target, AgentContext):
             self.agent_context = target
         elif isinstance(target, ResourceLoader):
             self.resource_loader = target
         elif isinstance(target, list) and target and len(target) > 0:
             if _is_list_of_type(target, Action):
                 self.actions.extend(target)
             elif _is_list_of_type(target, AgentResource):
                 self.resources = target
+        elif isinstance(target, AgentMemory):
+            self.memory = target
         return self
 
     async def send(
         self,
         message: AgentMessage,
         recipient: Agent,
         reviewer: Optional[Agent] = None,
         request_reply: Optional[bool] = True,
         is_recovery: Optional[bool] = False,
     ) -> None:
         """Send a message to recipient agent."""
         with root_tracer.start_span(
             "agent.send",
             metadata={
-                "sender": self.get_name(),
-                "recipient": recipient.get_name(),
-                "reviewer": reviewer.get_name() if reviewer else None,
+                "sender": self.name,
+                "recipient": recipient.name,
+                "reviewer": reviewer.name if reviewer else None,
                 "agent_message": message.to_dict(),
                 "request_reply": request_reply,
                 "is_recovery": is_recovery,
                 "conv_uid": self.not_null_agent_context.conv_id,
             },
         ):
             await recipient.receive(
@@ -226,17 +224,17 @@
         silent: Optional[bool] = False,
         is_recovery: Optional[bool] = False,
     ) -> None:
         """Receive a message from another agent."""
         with root_tracer.start_span(
             "agent.receive",
             metadata={
-                "sender": sender.get_name(),
-                "recipient": self.get_name(),
-                "reviewer": reviewer.get_name() if reviewer else None,
+                "sender": sender.name,
+                "recipient": self.name,
+                "reviewer": reviewer.name if reviewer else None,
                 "agent_message": message.to_dict(),
                 "request_reply": request_reply,
                 "silent": silent,
                 "is_recovery": is_recovery,
                 "conv_uid": self.not_null_agent_context.conv_id,
                 "is_human": self.is_human,
             },
@@ -267,22 +265,22 @@
         """Generate a reply based on the received messages."""
         logger.info(
             f"generate agent reply!sender={sender}, rely_messages_len={rely_messages}"
         )
         root_span = root_tracer.start_span(
             "agent.generate_reply",
             metadata={
-                "sender": sender.get_name(),
-                "recipient": self.get_name(),
-                "reviewer": reviewer.get_name() if reviewer else None,
+                "sender": sender.name,
+                "recipient": self.name,
+                "reviewer": reviewer.name if reviewer else None,
                 "received_message": received_message.to_dict(),
                 "conv_uid": self.not_null_agent_context.conv_id,
-                "rely_messages": [msg.to_dict() for msg in rely_messages]
-                if rely_messages
-                else None,
+                "rely_messages": (
+                    [msg.to_dict() for msg in rely_messages] if rely_messages else None
+                ),
             },
         )
 
         try:
             with root_tracer.start_span(
                 "agent.generate_reply._init_reply_message",
                 metadata={
@@ -291,26 +289,14 @@
             ) as span:
                 # initialize reply message
                 reply_message: AgentMessage = self._init_reply_message(
                     received_message=received_message
                 )
                 span.metadata["reply_message"] = reply_message.to_dict()
 
-            with root_tracer.start_span(
-                "agent.generate_reply._system_message_assembly",
-                metadata={
-                    "reply_message": reply_message.to_dict(),
-                },
-            ) as span:
-                # assemble system message
-                await self._system_message_assembly(
-                    received_message.content, reply_message.context
-                )
-                span.metadata["assembled_system_messages"] = self.oai_system_message
-
             fail_reason = None
             current_retry_counter = 0
             is_success = True
             while current_retry_counter < self.max_retry_count:
                 if current_retry_counter > 0:
                     retry_message = self._init_reply_message(
                         received_message=received_message
@@ -321,16 +307,19 @@
                     # recorded.
                     # It is temporarily set to be initiated by the originating end to
                     # facilitate the organization of historical memory context.
                     await sender.send(
                         retry_message, self, reviewer, request_reply=False
                     )
 
-                thinking_messages = self._load_thinking_messages(
-                    received_message, sender, rely_messages
+                thinking_messages = await self._load_thinking_messages(
+                    received_message,
+                    sender,
+                    rely_messages,
+                    context=reply_message.get_dict_context(),
                 )
                 with root_tracer.start_span(
                     "agent.generate_reply.thinking",
                     metadata={
                         "thinking_messages": [
                             msg.to_dict() for msg in thinking_messages
                         ],
@@ -341,15 +330,15 @@
                     reply_message.model_name = model_name
                     reply_message.content = llm_reply
                     span.metadata["llm_reply"] = llm_reply
                     span.metadata["model_name"] = model_name
 
                 with root_tracer.start_span(
                     "agent.generate_reply.review",
-                    metadata={"llm_reply": llm_reply, "censored": self.get_name()},
+                    metadata={"llm_reply": llm_reply, "censored": self.name},
                 ) as span:
                     # 2.Review whether what is being done is legal
                     approve, comments = await self.review(llm_reply, self)
                     reply_message.review_info = AgentReviewInfo(
                         approve=approve,
                         comments=comments,
                     )
@@ -357,16 +346,16 @@
                     span.metadata["comments"] = comments
 
                 act_extent_param = self.prepare_act_param()
                 with root_tracer.start_span(
                     "agent.generate_reply.act",
                     metadata={
                         "llm_reply": llm_reply,
-                        "sender": sender.get_name(),
-                        "reviewer": reviewer.get_name() if reviewer else None,
+                        "sender": sender.name,
+                        "reviewer": reviewer.name if reviewer else None,
                         "act_extent_param": act_extent_param,
                     },
                 ) as span:
                     # 3.Act based on the results of your thinking
                     act_out: Optional[ActionOutput] = await self.act(
                         message=llm_reply,
                         sender=sender,
@@ -379,35 +368,51 @@
                         act_out.to_dict() if act_out else None
                     )
 
                 with root_tracer.start_span(
                     "agent.generate_reply.verify",
                     metadata={
                         "llm_reply": llm_reply,
-                        "sender": sender.get_name(),
-                        "reviewer": reviewer.get_name() if reviewer else None,
+                        "sender": sender.name,
+                        "reviewer": reviewer.name if reviewer else None,
                     },
                 ) as span:
                     # 4.Reply information verification
                     check_pass, reason = await self.verify(
                         reply_message, sender, reviewer
                     )
                     is_success = check_pass
                     span.metadata["check_pass"] = check_pass
                     span.metadata["reason"] = reason
+
+                question: str = received_message.content or ""
+                ai_message: str = llm_reply or ""
                 # 5.Optimize wrong answers myself
                 if not check_pass:
                     current_retry_counter += 1
                     # Send error messages and issue new problem-solving instructions
                     if current_retry_counter < self.max_retry_count:
                         await self.send(
                             reply_message, sender, reviewer, request_reply=False
                         )
                     fail_reason = reason
+                    await self.save_to_memory(
+                        question=question,
+                        ai_message=ai_message,
+                        action_output=act_out,
+                        check_pass=check_pass,
+                        check_fail_reason=fail_reason,
+                    )
                 else:
+                    await self.save_to_memory(
+                        question=question,
+                        ai_message=ai_message,
+                        action_output=act_out,
+                        check_pass=check_pass,
+                    )
                     break
             reply_message.success = is_success
             return reply_message
 
         except Exception as e:
             logger.exception("Generate reply exception!")
             err_message = AgentMessage(content=str(e))
@@ -433,16 +438,14 @@
         # LLM inference automatically retries 3 times to reduce interruption
         # probability caused by speed limit and network stability
         while retry_count < 3:
             llm_model = await self._a_select_llm_model(last_model)
             try:
                 if prompt:
                     llm_messages = _new_system_message(prompt) + llm_messages
-                else:
-                    llm_messages = self.oai_system_message + llm_messages
 
                 if not self.llm_client:
                     raise ValueError("LLM client is not initialized!")
                 response = await self.llm_client.create(
                     context=llm_messages[-1].pop("context", None),
                     messages=llm_messages,
                     llm_model=llm_model,
@@ -487,17 +490,17 @@
             if not message:
                 raise ValueError("The message content is empty!")
 
             with root_tracer.start_span(
                 "agent.act.run",
                 metadata={
                     "message": message,
-                    "sender": sender.get_name() if sender else None,
-                    "recipient": self.get_name(),
-                    "reviewer": reviewer.get_name() if reviewer else None,
+                    "sender": sender.name if sender else None,
+                    "recipient": self.name,
+                    "reviewer": reviewer.name if reviewer else None,
                     "need_resource": need_resource.to_dict() if need_resource else None,
                     "rely_action_out": last_out.to_dict() if last_out else None,
                     "conv_uid": self.not_null_agent_context.conv_id,
                     "action_index": i,
                     "total_action": len(self.actions),
                 },
             ) as span:
@@ -559,17 +562,17 @@
             message (str): The message to send.
         """
         agent_message = AgentMessage(content=message, current_goal=message)
         with root_tracer.start_span(
             "agent.initiate_chat",
             span_type=SpanType.AGENT,
             metadata={
-                "sender": self.get_name(),
-                "recipient": recipient.get_name(),
-                "reviewer": reviewer.get_name() if reviewer else None,
+                "sender": self.name,
+                "recipient": recipient.name,
+                "reviewer": reviewer.name if reviewer else None,
                 "agent_message": agent_message.to_dict(),
                 "conv_uid": self.not_null_agent_context.conv_id,
             },
         ):
             await self.send(
                 agent_message,
                 recipient,
@@ -608,29 +611,35 @@
                 "model_name",
             )
             if k in message_dict
         }
 
         gpts_message: GptsMessage = GptsMessage(
             conv_id=self.not_null_agent_context.conv_id,
-            sender=sender.get_profile(),
-            receiver=self.profile,
+            sender=sender.role,
+            receiver=self.role,
             role=role,
             rounds=self.consecutive_auto_reply_counter,
             current_goal=oai_message.get("current_goal", None),
             content=oai_message.get("content", None),
-            context=json.dumps(oai_message["context"], ensure_ascii=False)
-            if "context" in oai_message
-            else None,
-            review_info=json.dumps(oai_message["review_info"], ensure_ascii=False)
-            if "review_info" in oai_message
-            else None,
-            action_report=json.dumps(oai_message["action_report"], ensure_ascii=False)
-            if "action_report" in oai_message
-            else None,
+            context=(
+                json.dumps(oai_message["context"], ensure_ascii=False)
+                if "context" in oai_message
+                else None
+            ),
+            review_info=(
+                json.dumps(oai_message["review_info"], ensure_ascii=False)
+                if "review_info" in oai_message
+                else None
+            ),
+            action_report=(
+                json.dumps(oai_message["action_report"], ensure_ascii=False)
+                if "action_report" in oai_message
+                else None
+            ),
             model_name=oai_message.get("model_name", None),
         )
 
         with root_tracer.start_span(
             "agent.save_message_to_memory",
             metadata={
                 "gpts_message": gpts_message.to_dict(),
@@ -639,40 +648,40 @@
         ):
             self.memory.message_memory.append(gpts_message)
             return True
 
     def _print_received_message(self, message: AgentMessage, sender: Agent):
         # print the message received
         print("\n", "-" * 80, flush=True, sep="")
-        _print_name = self.name if self.name else self.profile
+        _print_name = self.name if self.name else self.role
         print(
             colored(
-                sender.get_name() if sender.get_name() else sender.get_profile(),
+                sender.name if sender.name else sender.role,
                 "yellow",
             ),
             "(to",
             f"{_print_name})-[{message.model_name or ''}]:\n",
             flush=True,
         )
 
         content = json.dumps(message.content, ensure_ascii=False)
         if content is not None:
             print(content, flush=True)
 
         review_info = message.review_info
         if review_info:
-            name = sender.get_name() if sender.get_name() else sender.get_profile()
+            name = sender.name if sender.name else sender.role
             pass_msg = "Pass" if review_info.approve else "Reject"
             review_msg = f"{pass_msg}({review_info.comments})"
             approve_print = f">>>>>>>>{name} Review info: \n{review_msg}"
             print(colored(approve_print, "green"), flush=True)
 
         action_report = message.action_report
         if action_report:
-            name = sender.get_name() if sender.get_name() else sender.get_profile()
+            name = sender.name if sender.name else sender.role
             action_msg = (
                 "execution succeeded"
                 if action_report["is_exe_success"]
                 else "execution failed"
             )
             action_report_msg = f"{action_msg},\n{action_report['content']}"
             action_print = f">>>>>>>>{name} Action report: \n{action_report_msg}"
@@ -686,50 +695,40 @@
             raise ValueError(
                 "Received message can't be converted into a valid ChatCompletion"
                 " message. Either content or function_call must be provided."
             )
 
         self._print_received_message(message, sender)
 
-    async def _system_message_assembly(
-        self, question: Optional[str], context: Optional[Union[str, Dict]] = None
-    ):
-        # system message
-        self.init_system_message()
-        if len(self.oai_system_message) > 0:
-            resource_prompt_list = []
-            for item in self.resources:
-                resource_client = self.not_null_resource_loader.get_resource_api(
-                    item.type, ResourceClient
-                )
-                if not resource_client:
-                    raise ValueError(
-                        f"Resource {item.type}:{item.value} missing resource loader"
-                        f" implementation,unable to read resources!"
-                    )
-                resource_prompt_list.append(
-                    await resource_client.get_resource_prompt(item, question)
+    async def generate_resource_variables(
+        self, question: Optional[str] = None
+    ) -> Dict[str, Any]:
+        """Generate the resource variables."""
+        resource_prompt_list = []
+        for item in self.resources:
+            resource_client = self.not_null_resource_loader.get_resource_api(
+                item.type, ResourceClient
+            )
+            if not resource_client:
+                raise ValueError(
+                    f"Resource {item.type}:{item.value} missing resource loader"
+                    f" implementation,unable to read resources!"
                 )
-            if context is None or not isinstance(context, dict):
-                context = {}
+            resource_prompt_list.append(
+                await resource_client.get_resource_prompt(item, question)
+            )
 
-            resource_prompt = ""
-            if len(resource_prompt_list) > 0:
-                resource_prompt = "RESOURCES:" + "\n".join(resource_prompt_list)
-
-            out_schema: Optional[str] = ""
-            if self.actions and len(self.actions) > 0:
-                out_schema = self.actions[0].ai_out_schema
-            for message in self.oai_system_message:
-                new_content = message["content"].format(
-                    resource_prompt=resource_prompt,
-                    out_schema=out_schema,
-                    **context,
-                )
-                message["content"] = new_content
+        resource_prompt = ""
+        if len(resource_prompt_list) > 0:
+            resource_prompt = "RESOURCES:" + "\n".join(resource_prompt_list)
+
+        out_schema: Optional[str] = ""
+        if self.actions and len(self.actions) > 0:
+            out_schema = self.actions[0].ai_out_schema
+        return {"resource_prompt": resource_prompt, "out_schema": out_schema}
 
     def _excluded_models(
         self,
         all_models: List[str],
         order_llms: Optional[List[str]] = None,
         excluded_models: Optional[List[str]] = None,
     ):
@@ -770,15 +769,15 @@
             else:
                 can_uses = self._excluded_models(all_model_names, None, excluded_models)
             if can_uses and len(can_uses) > 0:
                 return can_uses[0]
             else:
                 raise ValueError("No model service available!")
         except Exception as e:
-            logger.error(f"{self.profile} get next llm failed!{str(e)}")
+            logger.error(f"{self.role} get next llm failed!{str(e)}")
             raise ValueError(f"Failed to allocate model service,{str(e)}!")
 
     def _init_reply_message(self, received_message: AgentMessage) -> AgentMessage:
         """Create a new message from the received message.
 
         Initialize a new message from the received message
 
@@ -799,17 +798,17 @@
         oai_messages: List[AgentMessage] = []
         # Based on the current agent, all messages received are user, and all messages
         # sent are assistant.
         for item in gpts_messages:
             if item.role:
                 role = item.role
             else:
-                if item.receiver == self.profile:
+                if item.receiver == self.role:
                     role = ModelMessageRoleType.HUMAN
-                elif item.sender == self.profile:
+                elif item.sender == self.role:
                     role = ModelMessageRoleType.AI
                 else:
                     continue
 
             # Message conversion, priority is given to converting execution results,
             # and only model output results will be used if not.
             content = item.content
@@ -821,46 +820,112 @@
                     and action_out.content is not None
                 ):
                     content = action_out.content
             oai_messages.append(
                 AgentMessage(
                     content=content,
                     role=role,
-                    context=json.loads(item.context)
-                    if item.context is not None
-                    else None,
+                    context=(
+                        json.loads(item.context) if item.context is not None else None
+                    ),
                 )
             )
         return oai_messages
 
-    def _load_thinking_messages(
+    async def _load_thinking_messages(
+        self,
+        received_message: AgentMessage,
+        sender: Agent,
+        rely_messages: Optional[List[AgentMessage]] = None,
+        context: Optional[Dict[str, Any]] = None,
+    ) -> List[AgentMessage]:
+        observation = received_message.content
+        if not observation:
+            raise ValueError("The received message content is empty!")
+        memories = await self.read_memories(observation)
+        reply_message_str = ""
+        if context is None:
+            context = {}
+        if rely_messages:
+            copied_rely_messages = [m.copy() for m in rely_messages]
+            # When directly relying on historical messages, use the execution result
+            # content as a dependency
+            for message in copied_rely_messages:
+                action_report: Optional[ActionOutput] = ActionOutput.from_dict(
+                    message.action_report
+                )
+                if action_report:
+                    # TODO: Modify in-place, need to be optimized
+                    message.content = action_report.content
+                if message.name != self.role:
+                    # TODO, use name
+                    # Rely messages are not from the current agent
+                    if message.role == ModelMessageRoleType.HUMAN:
+                        reply_message_str += f"Question: {message.content}\n"
+                    elif message.role == ModelMessageRoleType.AI:
+                        reply_message_str += f"Observation: {message.content}\n"
+        if reply_message_str:
+            memories += "\n" + reply_message_str
+
+        system_prompt = await self.build_prompt(
+            question=observation,
+            is_system=True,
+            most_recent_memories=memories,
+            **context,
+        )
+        user_prompt = await self.build_prompt(
+            question=observation,
+            is_system=False,
+            most_recent_memories=memories,
+            **context,
+        )
+
+        agent_messages = []
+        if system_prompt:
+            agent_messages.append(
+                AgentMessage(
+                    content=system_prompt,
+                    role=ModelMessageRoleType.SYSTEM,
+                )
+            )
+        if user_prompt:
+            agent_messages.append(
+                AgentMessage(
+                    content=user_prompt,
+                    role=ModelMessageRoleType.HUMAN,
+                )
+            )
+
+        return agent_messages
+
+    def _old_load_thinking_messages(
         self,
         received_message: AgentMessage,
         sender: Agent,
         rely_messages: Optional[List[AgentMessage]] = None,
     ) -> List[AgentMessage]:
         current_goal = received_message.current_goal
 
         # Convert and tailor the information in collective memory into contextual
         # memory available to the current Agent
 
         with root_tracer.start_span(
             "agent._load_thinking_messages",
             metadata={
-                "sender": sender.get_name(),
-                "recipient": self.get_name(),
+                "sender": sender.name,
+                "recipient": self.name,
                 "conv_uid": self.not_null_agent_context.conv_id,
                 "current_goal": current_goal,
             },
         ) as span:
             # Get historical information from the memory
             memory_messages = self.memory.message_memory.get_between_agents(
                 self.not_null_agent_context.conv_id,
-                self.profile,
-                sender.get_profile(),
+                self.role,
+                sender.role,
                 current_goal,
             )
             span.metadata["memory_messages"] = [
                 message.to_dict() for message in memory_messages
             ]
         current_goal_messages = self._convert_to_ai_message(memory_messages)
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/core/base_team.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/base_team.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Base classes for managing a group of agents in a team chat."""
 
 import logging
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from dbgpt._private.pydantic import BaseModel, ConfigDict, Field
 
-from ..actions.action import ActionOutput
+from .action.base import ActionOutput
 from .agent import Agent, AgentMessage
 from .base_agent import ConversableAgent
+from .profile import ProfileConfig
 
 logger = logging.getLogger(__name__)
 
 
 def _content_str(content: Union[str, List, None]) -> str:
     """Convert content into a string format.
 
@@ -82,15 +83,15 @@
     def hire(self, agents: List[Agent]):
         """Hire roles to cooperate."""
         self.agents.extend(agents)
 
     @property
     def agent_names(self) -> List[str]:
         """Return the names of the agents in the group chat."""
-        return [agent.get_profile() for agent in self.agents]
+        return [agent.role for agent in self.agents]
 
     def agent_by_name(self, name: str) -> Agent:
         """Return the agent with a given name."""
         return self.agents[self.agent_names.index(name)]
 
     async def select_speaker(
         self,
@@ -117,18 +118,22 @@
 
 
 class ManagerAgent(ConversableAgent, Team):
     """Manager Agent class."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    profile: str = "TeamManager"
-    goal: str = "manage all hired intelligent agents to complete mission objectives"
-    constraints: List[str] = []
-    desc: str = goal
+    profile: ProfileConfig = ProfileConfig(
+        name="ManagerAgent",
+        profile="TeamManager",
+        goal="manage all hired intelligent agents to complete mission objectives",
+        constraints=[],
+        desc="manage all hired intelligent agents to complete mission objectives",
+    )
+
     is_team: bool = True
 
     # The management agent does not need to retry the exception. The actual execution
     # of the agent has already been retried.
     max_retry_count: int = 1
 
     def __init__(self, **kwargs):
@@ -145,14 +150,24 @@
         if messages is None or len(messages) <= 0:
             return None, None
         else:
             message = messages[-1]
             self.messages.append(message.to_llm_message())
             return message.content, None
 
+    async def _load_thinking_messages(
+        self,
+        received_message: AgentMessage,
+        sender: Agent,
+        rely_messages: Optional[List[AgentMessage]] = None,
+        context: Optional[Dict[str, Any]] = None,
+    ) -> List[AgentMessage]:
+        """Load messages for thinking."""
+        return [AgentMessage(content=received_message.content)]
+
     async def act(
         self,
         message: Optional[str],
         sender: Optional[Agent] = None,
         reviewer: Optional[Agent] = None,
         **kwargs,
     ) -> Optional[ActionOutput]:
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm.py` & `dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/llm_client.py` & `dbgpt-0.5.6rc0/dbgpt/agent/util/llm/llm_client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/core/llm/strategy/priority.py` & `dbgpt-0.5.6rc0/dbgpt/agent/util/llm/strategy/priority.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/expand/code_assistant_agent.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/code_assistant_agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Code Assistant Agent."""
-from typing import List, Optional, Tuple
+
+from typing import Optional, Tuple
 
 from dbgpt.core import ModelMessageRoleType
 from dbgpt.util.string_utils import str_to_bool
 
-from ..actions.code_action import CodeAction
 from ..core.agent import AgentMessage
 from ..core.base_agent import ConversableAgent
+from ..core.profile import DynConfig, ProfileConfig
+from .actions.code_action import CodeAction
 
 CHECK_RESULT_SYSTEM_MESSAGE = (
     "You are an expert in analyzing the results of task execution. Your responsibility "
     "is to analyze the task goals and execution results provided by the user, and "
     "then make a judgment. You need to answer according to the following rules:\n"
     "          Rule 1: Determine whether the content of the focused execution results "
     "is related to the task target content and whether it can be used as the answer to "
@@ -38,62 +40,83 @@
     "computational goals of the mission.\n"
 )
 
 
 class CodeAssistantAgent(ConversableAgent):
     """Code Assistant Agent."""
 
-    name: str = "Turing"
-    profile: str = "CodeEngineer"
-    goal: str = (
-        "Solve tasks using your coding and language skills.\n"
-        "In the following cases, suggest python code (in a python coding block) or "
-        "shell script (in a sh coding block) for the user to execute.\n"
-        "    1. When you need to collect info, use the code to output the info you "
-        "need, for example, browse or search the web, download/read a file, print the "
-        "content of a webpage or a file, get the current date/time, check the "
-        "operating system. After sufficient info is printed and the task is ready to be"
-        " solved based on your language skill, you can solve the task by yourself.\n"
-        "    2. When you need to perform some task with code, use the code to perform "
-        "the task and output the result. Finish the task smartly."
-    )
-    constraints: List[str] = [
-        "The user cannot provide any other feedback or perform any other action beyond"
-        " executing the code you suggest. The user can't modify your code. So do not "
-        "suggest incomplete code which requires users to modify. Don't use a code block"
-        " if it's not intended to be executed by the user.Don't ask users to copy and "
-        "paste results. Instead, the 'Print' function must be used for output when "
-        "relevant.",
-        "When using code, you must indicate the script type in the code block. Please "
-        "don't include multiple code blocks in one response.",
-        "If you want the user to save the code in a file before executing it, put "
-        "# filename: <filename> inside the code block as the first line.",
-        "If you receive user input that indicates an error in the code execution, fix "
-        "the error and output the complete code again. It is recommended to use the "
-        "complete code rather than partial code or code changes. If the error cannot be"
-        " fixed, or the task is not resolved even after the code executes successfully,"
-        " analyze the problem, revisit your assumptions, gather additional information"
-        " you need from historical conversation records, and consider trying a "
-        "different approach.",
-        "Unless necessary, give priority to solving problems with python code. If it "
-        "involves downloading files or storing data locally, please use 'Print' to "
-        "output the full file path of the stored data and a brief introduction to the "
-        "data.",
-        "The output content of the 'print' function will be passed to other LLM agents "
-        "as dependent data. Please control the length of the output content of the "
-        "'print' function. The 'print' function only outputs part of the key data "
-        "information that is relied on, and is as concise as possible.",
-        "The code is executed without user participation. It is forbidden to use "
-        "methods that will block the process or need to be shut down, such as the "
-        "plt.show() method of matplotlib.pyplot as plt.",
-        "It is prohibited to fabricate non-existent data to achieve goals.",
-    ]
-    desc: str = (
-        "Can independently write and execute python/shell code to solve various"
-        " problems"
+    profile: ProfileConfig = ProfileConfig(
+        name=DynConfig(
+            "Turing",
+            category="agent",
+            key="dbgpt_agent_expand_code_assistant_agent_profile_name",
+        ),
+        role=DynConfig(
+            "CodeEngineer",
+            category="agent",
+            key="dbgpt_agent_expand_code_assistant_agent_profile_role",
+        ),
+        goal=DynConfig(
+            "Solve tasks using your coding and language skills.\n"
+            "In the following cases, suggest python code (in a python coding block) or "
+            "shell script (in a sh coding block) for the user to execute.\n"
+            "    1. When you need to collect info, use the code to output the info you "
+            "need, for example, browse or search the web, download/read a file, print "
+            "the content of a webpage or a file, get the current date/time, check the "
+            "operating system. After sufficient info is printed and the task is ready "
+            "to be solved based on your language skill, you can solve the task by "
+            "yourself.\n"
+            "    2. When you need to perform some task with code, use the code to "
+            "perform the task and output the result. Finish the task smartly.",
+            category="agent",
+            key="dbgpt_agent_expand_code_assistant_agent_profile_goal",
+        ),
+        constraints=DynConfig(
+            [
+                "The user cannot provide any other feedback or perform any other "
+                "action beyond executing the code you suggest. The user can't modify "
+                "your code. So do not suggest incomplete code which requires users to "
+                "modify. Don't use a code block if it's not intended to be executed "
+                "by the user.Don't ask users to copy and paste results. Instead, "
+                "the 'Print' function must be used for output when relevant.",
+                "When using code, you must indicate the script type in the code block. "
+                "Please don't include multiple code blocks in one response.",
+                "If you want the user to save the code in a file before executing it, "
+                "put # filename: <filename> inside the code block as the first line.",
+                "If you receive user input that indicates an error in the code "
+                "execution, fix the error and output the complete code again. It is "
+                "recommended to use the complete code rather than partial code or "
+                "code changes. If the error cannot be fixed, or the task is not "
+                "resolved even after the code executes successfully, analyze the "
+                "problem, revisit your assumptions, gather additional information you "
+                "need from historical conversation records, and consider trying a "
+                "different approach.",
+                "Unless necessary, give priority to solving problems with python "
+                "code. If it involves downloading files or storing data locally, "
+                "please use 'Print' to output the full file path of the stored data "
+                "and a brief introduction to the data.",
+                "The output content of the 'print' function will be passed to other "
+                "LLM agents as dependent data. Please control the length of the "
+                "output content of the 'print' function. The 'print' function only "
+                "outputs part of the key data information that is relied on, "
+                "and is as concise as possible.",
+                "The code is executed without user participation. It is forbidden to "
+                "use methods that will block the process or need to be shut down, "
+                "such as the plt.show() method of matplotlib.pyplot as plt.",
+                "It is prohibited to fabricate non-existent data to achieve goals.",
+            ],
+            category="agent",
+            key="dbgpt_agent_expand_code_assistant_agent_profile_constraints",
+        ),
+        desc=DynConfig(
+            "Can independently write and execute python/shell code to solve various"
+            " problems",
+            category="agent",
+            key="dbgpt_agent_expand_code_assistant_agent_profile_desc",
+        ),
     )
 
     def __init__(self, **kwargs):
         """Create a new CodeAssistantAgent instance."""
         super().__init__(**kwargs)
         self._init_actions([CodeAction])
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/expand/data_scientist_agent.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/data_scientist_agent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,74 @@
 """Data Scientist Agent."""
 
 import json
 import logging
-from typing import List, Optional, Tuple, cast
+from typing import Optional, Tuple, cast
 
-from ..actions.action import ActionOutput
-from ..actions.chart_action import ChartAction
+from ..core.action.base import ActionOutput
 from ..core.agent import AgentMessage
 from ..core.base_agent import ConversableAgent
+from ..core.profile import DynConfig, ProfileConfig
 from ..resource.resource_api import ResourceType
 from ..resource.resource_db_api import ResourceDbClient
+from .actions.chart_action import ChartAction
 
 logger = logging.getLogger(__name__)
 
 
 class DataScientistAgent(ConversableAgent):
     """Data Scientist Agent."""
 
-    name: str = "Edgar"
-    profile: str = "DataScientist"
-    goal: str = (
-        "Use correct {dialect} SQL to analyze and solve tasks based on the data"
-        " structure information of the database given in the resource."
-    )
-    constraints: List[str] = [
-        "Please check the generated SQL carefully. Please strictly abide by the data "
-        "structure definition given. It is prohibited to use non-existent fields and "
-        "data values. Do not use fields from table A to table B. You can perform "
-        "multi-table related queries.",
-        "If the data and fields that need to be analyzed in the target are in different"
-        " tables, it is recommended to use multi-table correlation queries first, and "
-        "pay attention to the correlation between multiple table structures.",
-        "It is forbidden to construct data by yourself as a query condition. If you "
-        "want to query a specific field, if the value of the field is provided, then "
-        "you can perform a group statistical query on the field.",
-        "Please select an appropriate one from the supported display methods for data "
-        "display. If no suitable display type is found, table display is used by "
-        "default. Supported display types: \n {display_type}",
-    ]
-    desc: str = (
-        "Use database resources to conduct data analysis, analyze SQL, and "
-        "provide recommended rendering methods."
+    profile: ProfileConfig = ProfileConfig(
+        name=DynConfig(
+            "Edgar",
+            category="agent",
+            key="dbgpt_agent_expand_dashboard_assistant_agent_profile_name",
+        ),
+        role=DynConfig(
+            "DataScientist",
+            category="agent",
+            key="dbgpt_agent_expand_dashboard_assistant_agent_profile_role",
+        ),
+        goal=DynConfig(
+            "Use correct {{ dialect }} SQL to analyze and solve tasks based on the data"
+            " structure information of the database given in the resource.",
+            category="agent",
+            key="dbgpt_agent_expand_dashboard_assistant_agent_profile_goal",
+        ),
+        constraints=DynConfig(
+            [
+                "Please check the generated SQL carefully. Please strictly abide by "
+                "the data structure definition given. It is prohibited to use "
+                "non-existent fields and data values. Do not use fields from table A "
+                "to table B. You can perform multi-table related queries.",
+                "If the data and fields that need to be analyzed in the target are in "
+                "different tables, it is recommended to use multi-table correlation "
+                "queries first, and pay attention to the correlation between multiple "
+                "table structures.",
+                "It is forbidden to construct data by yourself as a query condition. "
+                "If you want to query a specific field, if the value of the field is "
+                "provided, then you can perform a group statistical query on the "
+                "field.",
+                "Please select an appropriate one from the supported display methods "
+                "for data display. If no suitable display type is found, "
+                "table display is used by default. Supported display types: \n"
+                "{{ display_type }}",
+            ],
+            category="agent",
+            key="dbgpt_agent_expand_dashboard_assistant_agent_profile_constraints",
+        ),
+        desc=DynConfig(
+            "Use database resources to conduct data analysis, analyze SQL, and provide "
+            "recommended rendering methods.",
+            category="agent",
+            key="dbgpt_agent_expand_dashboard_assistant_agent_profile_desc",
+        ),
     )
+
     max_retry_count: int = 5
 
     def __init__(self, **kwargs):
         """Create a new DataScientistAgent instance."""
         super().__init__(**kwargs)
         self._init_actions([ChartAction])
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/expand/plugin_assistant_agent.py` & `dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_plugin_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,90 @@
-"""Plugin Assistant Agent."""
+"""Resource plugin client API."""
 import logging
-from typing import Any, Dict, List, Optional
+import os
+from typing import Any, Dict, List, Optional, Union, cast
 
-from ..actions.plugin_action import PluginAction
-from ..core.base_agent import ConversableAgent
+from ..plugin.commands.command_manage import execute_command
 from ..plugin.generator import PluginPromptGenerator
-from ..resource.resource_api import ResourceType
-from ..resource.resource_plugin_api import ResourcePluginClient
+from ..plugin.plugins_util import scan_plugin_file, scan_plugins
+from ..resource.resource_api import AgentResource
+from .resource_api import ResourceClient, ResourceType
 
 logger = logging.getLogger(__name__)
 
 
-class PluginAssistantAgent(ConversableAgent):
-    """Plugin Assistant Agent."""
-
-    plugin_generator: Optional[PluginPromptGenerator] = None
-
-    name: str = "LuBan"
-    profile: str = "ToolExpert"
-    goal: str = (
-        "Read and understand the tool information given in the resources below to "
-        "understand their capabilities and how to use them,and choosing the right tools"
-        " to achieve the user's goals."
-    )
-    constraints: List[str] = [
-        "Please read the parameter definition of the tool carefully and extract the "
-        "specific parameters required to execute the tool from the user goal.",
-        "Please output the selected tool name and specific parameter information in "
-        "json format according to the following required format. If there is an "
-        "example, please refer to the sample format output.",
-    ]
-    desc: str = (
-        "You can use the following tools to complete the task objectives, tool "
-        "information: {tool_infos}"
-    )
-
-    def __init__(self, **kwargs):
-        """Create a new instance of PluginAssistantAgent."""
-        super().__init__(**kwargs)
-        self._init_actions([PluginAction])
+class ResourcePluginClient(ResourceClient):
+    """Resource plugin client."""
 
     @property
-    def introduce(self, **kwargs) -> str:
-        """Introduce the agent."""
-        if not self.plugin_generator:
-            raise ValueError("PluginGenerator is not loaded.")
-        return self.desc.format(
-            tool_infos=self.plugin_generator.generate_commands_string()
-        )
-
-    async def preload_resource(self):
-        """Preload the resource."""
-        plugin_loader_client: ResourcePluginClient = (
-            self.not_null_resource_loader.get_resource_api(
-                ResourceType.Plugin, ResourcePluginClient
+    def type(self):
+        """Return the resource type."""
+        return ResourceType.Plugin
+
+    def get_data_type(self, resource: AgentResource) -> str:
+        """Return the data type of the specified resource."""
+        return "Tools"
+
+    async def get_data_introduce(
+        self, resource: AgentResource, question: Optional[str] = None
+    ) -> Union[str, List[str]]:
+        """Get the content introduction prompt of the specified resource."""
+        return await self.plugins_prompt(resource.value)
+
+    async def load_plugin(
+        self,
+        value: str,
+        plugin_generator: Optional[PluginPromptGenerator] = None,
+    ) -> PluginPromptGenerator:
+        """Load the plugin."""
+        raise NotImplementedError("The run method should be implemented in a subclass.")
+
+    async def plugins_prompt(
+        self, value: str, plugin_generator: Optional[PluginPromptGenerator] = None
+    ) -> str:
+        """Get the plugin commands prompt."""
+        plugin_generator = await self.load_plugin(value)
+        return plugin_generator.generate_commands_string()
+
+    async def execute_command(
+        self,
+        command_name: str,
+        arguments: Dict[str, Any],
+        plugin_generator: PluginPromptGenerator,
+    ):
+        """Execute the command."""
+        if plugin_generator is None:
+            raise ValueError("No plugin commands loaded into the executable！")
+        return execute_command(command_name, arguments, plugin_generator)
+
+
+class PluginFileLoadClient(ResourcePluginClient):
+    """File plugin load client.
+
+    Load the plugin from the local file.
+    """
+
+    async def load_plugin(
+        self, value: str, plugin_generator: Optional[PluginPromptGenerator] = None
+    ) -> PluginPromptGenerator:
+        """Load the plugin."""
+        logger.info(f"PluginFileLoadClient load plugin:{value}")
+        if plugin_generator is None:
+            plugin_generator = PluginPromptGenerator()
+        plugins = []
+        if os.path.isabs(value):
+            if not os.path.exists(value):
+                raise ValueError(f"Wrong plugin file path configured {value}!")
+            if os.path.isfile(value):
+                plugins.extend(scan_plugin_file(value))
+            else:
+                plugins.extend(scan_plugins(value))
+        else:
+            raise ValueError(
+                f"The current mode cannot support plug-in loading with relative "
+                f"paths: {value}"
             )
-        )
-        item_list = []
-        for item in self.resources:
-            if item.type == ResourceType.Plugin:
-                item_list.append(item.value)
-        plugin_generator = self.plugin_generator
-        for item in item_list:
-            plugin_generator = await plugin_loader_client.load_plugin(
-                item, plugin_generator
-            )
-        self.plugin_generator = plugin_generator
-
-    def prepare_act_param(self) -> Dict[str, Any]:
-        """Prepare the act parameter."""
-        return {"plugin_generator": self.plugin_generator}
+        for plugin in plugins:
+            if not plugin.can_handle_post_prompt():
+                continue
+            plugin_generator = plugin.post_prompt(plugin_generator)
+        return cast(PluginPromptGenerator, plugin_generator)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py` & `dbgpt-0.5.6rc0/dbgpt/agent/expand/retrieve_summary_assistant_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Retrieve Summary Assistant Agent."""
+
 import glob
 import json
 import logging
 import os
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 from dbgpt.configs.model_config import PILOT_PATH
 from dbgpt.core import ModelMessageRoleType
 
-from ..actions.action import Action, ActionOutput
+from ..core.action.base import Action, ActionOutput
 from ..core.agent import Agent, AgentMessage, AgentReviewInfo
 from ..core.base_agent import ConversableAgent
+from ..core.profile import ProfileConfig
 from ..resource.resource_api import AgentResource
 from ..util.cmp import cmp_string_equal
 
 try:
     from unstructured.partition.auto import partition
 
     HAS_UNSTRUCTURED = True
@@ -82,26 +84,15 @@
 
     AssistantAgent is a subclass of ConversableAgent configured with a default
     system message.
     The default system message is designed to solve a task with LLM,
     including suggesting python code blocks and debugging.
     """
 
-    goal = (
-        "You're an extraction expert. You need to extract Please complete this task "
-        "step by step following instructions below:\n"
-        "   1. You need to first ONLY extract user's question that you need to answer "
-        "without ANY file paths and URLs. \n"
-        "   2. Extract the provided file paths and URLs.\n"
-        "   3. Construct the extracted file paths and URLs as a list of strings.\n"
-        "   4. ONLY output the extracted results with the following json format: "
-        "{response}."
-    )
-
-    PROMPT_QA = (
+    PROMPT_QA: str = (
         "You are a great summary writer to summarize the provided text content "
         "according to user questions.\n"
         "User's Question is: {input_question}\n\n"
         "Provided text content is: {input_context}\n\n"
         "Please complete this task step by step following instructions below:\n"
         "   1. You need to first detect user's question that you need to answer with "
         "your summarization.\n"
@@ -114,41 +105,51 @@
         "must be the same to user's question language!! You must give as short an "
         "summarization as possible!!! DO NOT CREATE ANY SUMMARIZATION WITH YOUR OWN "
         "KNOWLEDGE!!!\n\n"
         "####Important Notice####\n"
         "If the provided text content CAN NOT ANSWER user's question, ONLY output "
         "'NO RELATIONSHIP.UPDATE TEXT CONTENT.'!!."
     )
-    CHECK_RESULT_SYSTEM_MESSAGE = (
+    CHECK_RESULT_SYSTEM_MESSAGE: str = (
         "You are an expert in analyzing the results of a summary task."
         "Your responsibility is to check whether the summary results can summarize the "
         "input provided by the user, and then make a judgment. You need to answer "
         "according to the following rules:\n"
         "    Rule 1: If you think the summary results can summarize the input provided"
         " by the user, only return True.\n"
         "    Rule 2: If you think the summary results can NOT summarize the input "
         "provided by the user, return False and the reason, split by | and ended "
         "by TERMINATE. For instance: False|Some important concepts in the input are "
         "not summarized. TERMINATE"
     )
 
-    DEFAULT_DESCRIBE = (
+    DEFAULT_DESCRIBE: str = (
         "Summarize provided content according to user's questions and "
         "the provided file paths."
     )
-
-    name = "RetrieveSummarizer"
-    desc = DEFAULT_DESCRIBE
+    profile: ProfileConfig = ProfileConfig(
+        name="RetrieveSummarizer",
+        role="Assistant",
+        goal="You're an extraction expert. You need to extract Please complete this "
+        "task step by step following instructions below:\n"
+        "   1. You need to first ONLY extract user's question that you need to answer "
+        "without ANY file paths and URLs. \n"
+        "   2. Extract the provided file paths and URLs.\n"
+        "   3. Construct the extracted file paths and URLs as a list of strings.\n"
+        "   4. ONLY output the extracted results with the following json format: "
+        "{{ response }}.",
+        desc=DEFAULT_DESCRIBE,
+    )
 
     chunk_token_size: int = 4000
     chunk_mode: str = "multi_lines"
 
-    _model = "gpt-3.5-turbo-16k"
-    _max_tokens = _get_max_tokens(_model)
-    context_max_tokens = _max_tokens * 0.8
+    _model: str = "gpt-3.5-turbo-16k"
+    _max_tokens: int = _get_max_tokens(_model)
+    context_max_tokens: int = int(_max_tokens * 0.8)
 
     def __init__(
         self,
         **kwargs,
     ):
         """Create a new instance of the agent."""
         super().__init__(
@@ -170,20 +171,22 @@
         rely_messages: Optional[List[AgentMessage]] = None,
         **kwargs,
     ):
         """Generate a reply based on the received messages."""
         reply_message: AgentMessage = self._init_reply_message(
             received_message=received_message
         )
-        await self._system_message_assembly(
-            received_message.content, reply_message.context
-        )
         # 1.Think about how to do things
         llm_reply, model_name = await self.thinking(
-            self._load_thinking_messages(received_message, sender, rely_messages)
+            await self._load_thinking_messages(
+                received_message,
+                sender,
+                rely_messages,
+                context=reply_message.get_dict_context(),
+            )
         )
 
         if not llm_reply:
             raise ValueError("No reply from LLM.")
         ai_reply_dic = json.loads(llm_reply)
         user_question = ai_reply_dic["user_question"]
         file_list = ai_reply_dic["file_list"]
@@ -450,24 +453,24 @@
                     lines_tokens[0] = await self._count_token(lines[0])
                 else:
                     logger.warning(
                         "Failed to split docs with must_break_at_empty_line being True,"
                         " set to False."
                     )
                     must_break_at_empty_line = False
-            chunks.append(prev) if len(
-                prev
-            ) > 10 else None  # don't add chunks less than 10 characters
+            (
+                chunks.append(prev) if len(prev) > 10 else None
+            )  # don't add chunks less than 10 characters
             lines = lines[cnt:]
             lines_tokens = lines_tokens[cnt:]
             sum_tokens = sum(lines_tokens)
         text_to_chunk = "\n".join(lines)
-        chunks.append(text_to_chunk) if len(
-            text_to_chunk
-        ) > 10 else None  # don't add chunks less than 10 characters
+        (
+            chunks.append(text_to_chunk) if len(text_to_chunk) > 10 else None
+        )  # don't add chunks less than 10 characters
         return chunks
 
     def _extract_text_from_pdf(self, file: str) -> str:
         """Extract text from PDF files."""
         text = ""
         import pypdf
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/memory/base.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Base memory interface for agents."""
+
 import dataclasses
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
-from dbgpt.agent.core.schema import Status
+from ...schema import Status
 
 
 @dataclasses.dataclass
 class GptsPlan:
     """Gpts plan."""
 
     conv_id: str
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/memory/default_gpts_memory.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/default_gpts_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Default memory for storing plans and messages."""
 
 from dataclasses import fields
 from typing import List, Optional
 
 import pandas as pd
 
-from ..core.schema import Status
+from ...schema import Status
 from .base import GptsMessage, GptsMessageMemory, GptsPlan, GptsPlansMemory
 
 
 class DefaultGptsPlansMemory(GptsPlansMemory):
     """Default memory for storing plans."""
 
     def __init__(self):
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/memory/gpts_memory.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/memory/gpts/gpts_memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """GPTs memory."""
+
 import json
 from collections import OrderedDict, defaultdict
 from typing import Dict, List, Optional
 
 from dbgpt.vis.client import VisAgentMessages, VisAgentPlans, vis_client
 
-from ..actions.action import ActionOutput
+from ...action.base import ActionOutput
 from .base import GptsMessage, GptsMessageMemory, GptsPlansMemory
 from .default_gpts_memory import DefaultGptsMessageMemory, DefaultGptsPlansMemory
 
 NONE_GOAL_PREFIX: str = "none_goal_count_"
 
 
 class GptsMemory:
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plan/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Agent Operator for AWEL."""
+
 from abc import ABC
 from typing import List, Optional, Type
 
 from dbgpt.core.awel import MapOperator
 from dbgpt.core.awel.flow import (
     IOField,
     OperatorCategory,
@@ -12,18 +13,18 @@
 )
 from dbgpt.core.awel.trigger.base import Trigger
 from dbgpt.core.interface.message import ModelMessageRoleType
 
 # TODO: Don't dependent on MixinLLMOperator
 from dbgpt.model.operators.llm_operator import MixinLLMOperator
 
-from ...core.agent import Agent, AgentGenerateContext, AgentMessage
-from ...core.agent_manage import get_agent_manager
-from ...core.base_agent import ConversableAgent
-from ...core.llm.llm import LLMConfig
+from ....util.llm.llm import LLMConfig
+from ...agent import Agent, AgentGenerateContext, AgentMessage
+from ...agent_manage import get_agent_manager
+from ...base_agent import ConversableAgent
 from .agent_operator_resource import AWELAgent
 
 
 class BaseAgentOperator:
     """The abstract operator for an Agent."""
 
     SHARE_DATA_KEY_MODEL_NAME = "share_data_key_agent_name"
@@ -57,17 +58,15 @@
         """Trigger agent to generate a reply."""
         now_rely_messages: List[AgentMessage] = []
         if not input_value.message:
             raise ValueError("The message is empty.")
         input_message = input_value.message.copy()
 
         # Isolate the message delivery mechanism and pass it to the operator
-        _goal = (
-            self.agent.get_name() if self.agent.get_name() else self.agent.get_profile()
-        )
+        _goal = self.agent.name if self.agent.name else self.agent.role
         current_goal = f"[{_goal}]:"
 
         if input_message.content:
             current_goal += input_message.content
         input_message.current_goal = current_goal
 
         # What was received was the User message
@@ -91,15 +90,15 @@
             reviewer=input_value.reviewer,
             rely_messages=input_value.rely_messages,
         )
         is_success = agent_reply_message.success
 
         if not is_success:
             raise ValueError(
-                f"The task failed at step {self.agent.get_profile()} and the attempt "
+                f"The task failed at step {self.agent.role} and the attempt "
                 f"to repair it failed. The final reason for "
                 f"failure:{agent_reply_message.content}!"
             )
 
         # What is sent is an AI message
         ai_message = agent_reply_message.copy()
         ai_message.role = ModelMessageRoleType.AI
@@ -166,26 +165,22 @@
         """Trigger agent to generate a reply."""
         if not input_value.message:
             raise ValueError("The message is empty.")
         input_message = input_value.message.copy()
         agent = await self.get_agent(input_value)
         if agent.fixed_subgoal and len(agent.fixed_subgoal) > 0:
             # Isolate the message delivery mechanism and pass it to the operator
-            current_goal = (
-                f"[{agent.get_name() if agent.get_name() else agent.get_profile()}]:"
-            )
+            current_goal = f"[{agent.name if agent.name else agent.role}]:"
             if agent.fixed_subgoal:
                 current_goal += agent.fixed_subgoal
             input_message.current_goal = current_goal
             input_message.content = agent.fixed_subgoal
         else:
             # Isolate the message delivery mechanism and pass it to the operator
-            current_goal = (
-                f"[{agent.get_name() if agent.get_name() else agent.get_profile()}]:"
-            )
+            current_goal = f"[{agent.name if agent.name else agent.role}]:"
             if input_message.content:
                 current_goal += input_message.content
             input_message.current_goal = current_goal
 
         now_rely_messages: List[AgentMessage] = []
         # What was received was the User message
         human_message = input_message.copy()
@@ -209,15 +204,15 @@
             rely_messages=input_value.rely_messages,
         )
 
         is_success = agent_reply_message.success
 
         if not is_success:
             raise ValueError(
-                f"The task failed at step {agent.get_profile()} and the attempt to "
+                f"The task failed at step {agent.role} and the attempt to "
                 f"repair it failed. The final reason for "
                 f"failure:{agent_reply_message.content}!"
             )
 
         # What is sent is an AI message
         ai_message: AgentMessage = agent_reply_message.copy()
         ai_message.role = ModelMessageRoleType.AI
@@ -227,15 +222,15 @@
         return AgentGenerateContext(
             message=input_message,
             sender=agent,
             reviewer=input_value.reviewer,
             # Default single step transfer of information
             rely_messages=now_rely_messages,
             silent=input_value.silent,
-            memory=input_value.memory,
+            memory=input_value.memory.structure_clone() if input_value.memory else None,
             agent_context=input_value.agent_context,
             resource_loader=input_value.resource_loader,
             llm_client=input_value.llm_client,
             round_index=agent.consecutive_auto_reply_counter,
         )
 
     async def get_agent(
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/agent_operator_resource.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/agent_operator_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """The AWEL Agent Operator Resource."""
+
 from typing import Any, Dict, List, Optional
 
 from dbgpt._private.pydantic import BaseModel, ConfigDict, Field, model_validator
 from dbgpt.core import LLMClient
 from dbgpt.core.awel.flow import (
     FunctionDynamicOptions,
     OptionValue,
     Parameter,
     ResourceCategory,
     register_resource,
 )
 
-from ...core.agent_manage import get_agent_manager
-from ...core.llm.llm import LLMConfig, LLMStrategyType
-from ...resource.resource_api import AgentResource, ResourceType
+from ....resource.resource_api import AgentResource, ResourceType
+from ....util.llm.llm import LLMConfig, LLMStrategyType
+from ...agent_manage import get_agent_manager
 
 
 @register_resource(
     label="AWEL Agent Resource",
     name="agent_operator_resource",
     description="The Agent Resource.",
     category=ResourceCategory.AGENT,
@@ -46,15 +47,18 @@
             name="agent_resource_value",
             type=str,
             optional=True,
             default=None,
             description="The agent resource value.",
         ),
     ],
-    alias=["dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgentResource"],
+    alias=[
+        "dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgentResource",
+        "dbgpt.agent.plan.awel.agent_operator_resource.AWELAgentResource",
+    ],
 )
 class AWELAgentResource(AgentResource):
     """AWEL Agent Resource."""
 
     @model_validator(mode="before")
     @classmethod
     def pre_fill(cls, values: Dict[str, Any]) -> Dict[str, Any]:
@@ -103,15 +107,18 @@
             name="strategy_context",
             type=str,
             optional=True,
             default=None,
             description="The agent LLM Strategy Value.",
         ),
     ],
-    alias=["dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgentConfig"],
+    alias=[
+        "dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgentConfig",
+        "dbgpt.agent.plan.awel.agent_operator_resource.AWELAgentConfig",
+    ],
 )
 class AWELAgentConfig(LLMConfig):
     """AWEL Agent Config."""
 
     pass
 
 
@@ -164,15 +171,18 @@
             name="agent_llm_Config",
             type=AWELAgentConfig,
             optional=True,
             default=None,
             description="The agent llm config.",
         ),
     ],
-    alias=["dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgent"],
+    alias=[
+        "dbgpt.serve.agent.team.layout.agent_operator_resource.AwelAgent",
+        "dbgpt.agent.plan.awel.agent_operator_resource.AWELAgent",
+    ],
 )
 class AWELAgent(BaseModel):
     """AWEL Agent."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     agent_profile: str
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plan/awel/team_awel_layout.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/awel/team_awel_layout.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """The manager of the team for the AWEL layout."""
 
 import logging
 from abc import ABC, abstractmethod
-from typing import List, Optional, cast
+from typing import Optional, cast
 
 from dbgpt._private.config import Config
 from dbgpt._private.pydantic import (
     BaseModel,
     ConfigDict,
     Field,
     model_to_dict,
     validator,
 )
 from dbgpt.core.awel import DAG
 from dbgpt.core.awel.dag.dag_manager import DAGManager
 
-from ...actions.action import ActionOutput
-from ...core.agent import Agent, AgentGenerateContext, AgentMessage
-from ...core.base_team import ManagerAgent
+from ...action.base import ActionOutput
+from ...agent import Agent, AgentGenerateContext, AgentMessage
+from ...base_team import ManagerAgent
+from ...profile import DynConfig, ProfileConfig
 from .agent_operator import AWELAgentOperator, WrappedAgentOperator
 
 logger = logging.getLogger(__name__)
 
 
 class AWELTeamContext(BaseModel):
     """The context of the team for the AWEL layout."""
@@ -80,19 +81,32 @@
 
 
 class AWELBaseManager(ManagerAgent, ABC):
     """AWEL base manager."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    goal: str = (
-        "Promote and solve user problems according to the process arranged by AWEL."
+    profile: ProfileConfig = ProfileConfig(
+        name="AWELBaseManager",
+        role=DynConfig(
+            "PlanManager", category="agent", key="dbgpt_agent_plan_awel_profile_name"
+        ),
+        goal=DynConfig(
+            "Promote and solve user problems according to the process arranged "
+            "by AWEL.",
+            category="agent",
+            key="dbgpt_agent_plan_awel_profile_goal",
+        ),
+        desc=DynConfig(
+            "Promote and solve user problems according to the process arranged "
+            "by AWEL.",
+            category="agent",
+            key="dbgpt_agent_plan_awel_profile_desc",
+        ),
     )
-    constraints: List[str] = []
-    desc: str = goal
 
     async def _a_process_received_message(self, message: AgentMessage, sender: Agent):
         """Process the received message."""
         pass
 
     @abstractmethod
     def get_dag(self) -> DAG:
@@ -112,15 +126,15 @@
                 AWELAgentOperator, agent_dag.leaf_nodes[0]
             )
 
             start_message_context: AgentGenerateContext = AgentGenerateContext(
                 message=AgentMessage(content=message, current_goal=message),
                 sender=sender,
                 reviewer=reviewer,
-                memory=self.memory,
+                memory=self.memory.structure_clone(),
                 agent_context=self.agent_context,
                 resource_loader=self.resource_loader,
                 llm_client=self.not_null_llm_config.llm_client,
             )
             final_generate_context: AgentGenerateContext = await last_node.call(
                 call_data=start_message_context
             )
@@ -158,16 +172,14 @@
     """The manager of the team for the AWEL layout.
 
     Receives a DAG or builds a DAG from the agents.
     """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    profile: str = "WrappedAWELLayoutManager"
-
     dag: Optional[DAG] = Field(None, description="The DAG of the manager")
 
     def get_dag(self) -> DAG:
         """Get the DAG of the manager."""
         if self.dag:
             return self.dag
         conv_id = self.not_null_agent_context.conv_id
@@ -234,16 +246,14 @@
 
 
 class DefaultAWELLayoutManager(AWELBaseManager):
     """The manager of the team for the AWEL layout."""
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
-    profile: str = "DefaultAWELLayoutManager"
-
     dag: AWELTeamContext = Field(...)
 
     @validator("dag")
     def check_dag(cls, value):
         """Check the DAG of the manager."""
         assert value is not None and value != "", "dag must not be empty"
         return value
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plan/plan_action.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/plan_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import logging
 from typing import List, Optional
 
 from dbgpt._private.pydantic import BaseModel, Field
 from dbgpt.vis.tags.vis_agent_plans import Vis, VisAgentPlans
 
-from ..actions.action import Action, ActionOutput
-from ..core.agent import AgentContext
-from ..core.schema import Status
-from ..memory.base import GptsPlan
-from ..memory.gpts_memory import GptsPlansMemory
-from ..resource.resource_api import AgentResource
+from ...resource.resource_api import AgentResource
+from ..action.base import Action, ActionOutput
+from ..agent import AgentContext
+from ..memory.gpts.base import GptsPlan
+from ..memory.gpts.gpts_memory import GptsPlansMemory
+from ..schema import Status
 
 logger = logging.getLogger(__name__)
 
 
 class PlanInput(BaseModel):
     """Plan input model."""
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plan/planner_agent.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/planner_agent.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,92 +1,119 @@
 """Planner Agent."""
 
 from typing import Any, Dict, List
 
 from dbgpt._private.pydantic import Field
 
-from ..core.agent import AgentMessage
-from ..core.base_agent import ConversableAgent
-from .plan_action import PlanAction
+from ..agent import AgentMessage
+from ..base_agent import ConversableAgent
+from ..plan.plan_action import PlanAction
+from ..profile import DynConfig, ProfileConfig
 
 
 class PlannerAgent(ConversableAgent):
     """Planner Agent.
 
     Planner agent, realizing task goal planning decomposition through LLM.
     """
 
     agents: List[ConversableAgent] = Field(default_factory=list)
 
-    profile: str = "Planner"
+    profile: ProfileConfig = ProfileConfig(
+        name=DynConfig(
+            "Planner",
+            category="agent",
+            key="dbgpt_agent_plan_planner_agent_profile_name",
+        ),
+        role=DynConfig(
+            "Planner",
+            category="agent",
+            key="dbgpt_agent_plan_planner_agent_profile_role",
+        ),
+        goal=DynConfig(
+            "Understand each of the following intelligent agents and their "
+            "capabilities, using the provided resources, solve user problems by "
+            "coordinating intelligent agents. Please utilize your LLM's knowledge "
+            "and understanding ability to comprehend the intent and goals of the "
+            "user's problem, generating a task plan that can be completed through"
+            " the collaboration of intelligent agents without user assistance.",
+            category="agent",
+            key="dbgpt_agent_plan_planner_agent_profile_goal",
+        ),
+        expand_prompt=DynConfig(
+            "Available Intelligent Agents:\n {{ agents }}",
+            category="agent",
+            key="dbgpt_agent_plan_planner_agent_profile_expand_prompt",
+        ),
+        constraints=DynConfig(
+            [
+                "Every step of the task plan should exist to advance towards solving "
+                "the user's goals. Do not generate meaningless task steps; ensure "
+                "that each step has a clear goal and its content is complete.",
+                "Pay attention to the dependencies and logic of each step in the task "
+                "plan. For the steps that are depended upon, consider the data they "
+                "depend on and whether it can be obtained based on the current goal. "
+                "If it cannot be obtained, please indicate in the goal that the "
+                "dependent data needs to be generated.",
+                "Each step must be an independently achievable goal. Ensure that the "
+                "logic and information are complete. Avoid steps with unclear "
+                "objectives, like 'Analyze the retrieved issues data,' where it's "
+                "unclear what specific content needs to be analyzed.",
+                "Please ensure that only the intelligent agents mentioned above are "
+                "used, and you may use only the necessary parts of them. Allocate "
+                "them to appropriate steps strictly based on their described "
+                "capabilities and limitations. Each intelligent agent can be reused.",
+                "Utilize the provided resources to assist in generating the plan "
+                "steps according to the actual needs of the user's goals. Do not use "
+                "unnecessary resources.",
+                "Each step should ideally use only one type of resource to accomplish "
+                "a sub-goal. If the current goal can be broken down into multiple "
+                "subtasks of the same type, you can create mutually independent "
+                "parallel tasks.",
+                "Data resources can be loaded and utilized by the appropriate "
+                "intelligent agents without the need to consider the issues related "
+                "to data loading links.",
+                "Try to merge continuous steps that have sequential dependencies. If "
+                "the user's goal does not require splitting, you can create a "
+                "single-step task with content that is the user's goal.",
+                "Carefully review the plan to ensure it comprehensively covers all "
+                "information involved in the user's problem and can ultimately "
+                "achieve the goal. Confirm whether each step includes the necessary "
+                "resource information, such as URLs, resource names, etc.",
+            ],
+            category="agent",
+            key="dbgpt_agent_plan_planner_agent_profile_constraints",
+        ),
+        desc=DynConfig(
+            "You are a task planning expert! You can coordinate intelligent agents"
+            " and allocate resources to achieve complex task goals.",
+            category="agent",
+            key="dbgpt_agent_plan_planner_agent_profile_desc",
+        ),
+    )
     goal_zh: str = (
         "理解下面每个智能体(agent)和他们的能力，使用给出的资源，通过协调智能体来解决"
         "用户问题。 请发挥你LLM的知识和理解能力，理解用户问题的意图和目标，生成一个可以在没有用户帮助"
         "下，由智能体协作完成目标的任务计划。"
     )
-    goal: str = (
-        "Understand each of the following intelligent agents and their "
-        "capabilities, using the provided resources, solve user problems by "
-        "coordinating intelligent agents. Please utilize your LLM's knowledge "
-        "and understanding ability to comprehend the intent and goals of the "
-        "user's problem, generating a task plan that can be completed through"
-        " the collaboration of intelligent agents without user assistance."
-    )
-    expand_prompt_zh: str = "可用智能体(agent):\n {agents}"
-    expand_prompt: str = "Available Intelligent Agents:\n {agents}"
+    expand_prompt_zh: str = "可用智能体(agent):\n {{ agents }}"
 
     constraints_zh: List[str] = [
         "任务计划的每个步骤都应该是为了推进解决用户目标而存在，不要生成无意义的任务步骤，确保每个步骤内目标明确内容完整。",
         "关注任务计划每个步骤的依赖关系和逻辑，被依赖步骤要考虑被依赖的数据，是否能基于当前目标得到，如果不能请在目标中提示要生成被依赖数据。",
         "每个步骤都是一个独立可完成的目标，一定要确保逻辑和信息完整，不要出现类似:"
         "'Analyze the retrieved issues data'这样目标不明确，不知道具体要分析啥内容的步骤",
         "请确保只使用上面提到的智能体，并且可以只使用其中需要的部分，严格根据描述能力和限制分配给合适的步骤，每个智能体都可以重复使用。",
         "根据用户目标的实际需要使用提供的资源来协助生成计划步骤，不要使用不需要的资源。",
         "每个步骤最好只使用一种资源完成一个子目标，如果当前目标可以分解为同类型的多个子任务，可以生成相互不依赖的并行任务。",
         "数据资源可以被合适的智能体加载使用，不用考虑数据资源的加载链接问题",
         "尽量合并有顺序依赖的连续相同步骤,如果用户目标无拆分必要，可以生成内容为用户目标的单步任务。",
         "仔细检查计划，确保计划完整的包含了用户问题所涉及的所有信息，并且最终能完成目标，确认每个步骤是否包含了需要用到的资源信息,如URL、资源名等. ",
     ]
-    constraints: List[str] = [
-        "Every step of the task plan should exist to advance towards solving the user's"
-        " goals. Do not generate meaningless task steps; ensure that each step has a "
-        "clear goal and its content is complete.",
-        "Pay attention to the dependencies and logic of each step in the task plan. "
-        "For the steps that are depended upon, consider the data they depend on and "
-        "whether it can be obtained based on the current goal. If it cannot be obtained"
-        ", please indicate in the goal that the dependent data needs to be generated.",
-        "Each step must be an independently achievable goal. Ensure that the logic and"
-        " information are complete. Avoid steps with unclear objectives, like "
-        "'Analyze the retrieved issues data,' where it's unclear what specific content"
-        " needs to be analyzed.",
-        "Please ensure that only the intelligent agents mentioned above are used, and"
-        " you may use only the necessary parts of them. Allocate them to appropriate "
-        "steps strictly based on their described capabilities and limitations. Each "
-        "intelligent agent can be reused.",
-        "Utilize the provided resources to assist in generating the plan steps "
-        "according to the actual needs of the user's goals. Do not use unnecessary "
-        "resources.",
-        "Each step should ideally use only one type of resource to accomplish a "
-        "sub-goal. If the current goal can be broken down into multiple subtasks of the"
-        " same type, you can create mutually independent parallel tasks.",
-        "Data resources can be loaded and utilized by the appropriate intelligent "
-        "agents without the need to consider the issues related to data loading links.",
-        "Try to merge continuous steps that have sequential dependencies. If the "
-        "user's goal does not require splitting, you can create a single-step task with"
-        " content that is the user's goal.",
-        "Carefully review the plan to ensure it comprehensively covers all information"
-        " involved in the user's problem and can ultimately achieve the goal. Confirm"
-        " whether each step includes the necessary resource information, such as URLs,"
-        " resource names, etc.",
-    ]
     desc_zh: str = "你是一个任务规划专家！可以协调智能体，分配资源完成复杂的任务目标。"
-    desc: str = (
-        "You are a task planning expert! You can coordinate intelligent agents"
-        " and allocate resources to achieve complex task goals."
-    )
 
     examples: str = """
     user:help me build a sales report summarizing our key metrics and trends
     assistants:[
         {{
             "serial_number": "1",
             "agent": "DataScientist",
@@ -112,17 +139,15 @@
         """Create a new PlannerAgent instance."""
         super().__init__(**kwargs)
         self._init_actions([PlanAction])
 
     def _init_reply_message(self, received_message: AgentMessage):
         reply_message = super()._init_reply_message(received_message)
         reply_message.context = {
-            "agents": "\n".join(
-                [f"- {item.profile}:{item.desc}" for item in self.agents]
-            ),
+            "agents": "\n".join([f"- {item.role}:{item.desc}" for item in self.agents]),
         }
         return reply_message
 
     def bind_agents(self, agents: List[ConversableAgent]) -> ConversableAgent:
         """Bind the agents to the planner agent."""
         self.agents = agents
         for agent in self.agents:
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plan/team_auto_plan.py` & `dbgpt-0.5.6rc0/dbgpt/agent/core/plan/team_auto_plan.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,54 @@
 """Auto plan chat manager agent."""
 
 import logging
 from typing import Dict, List, Optional, Tuple
 
 from dbgpt.core.interface.message import ModelMessageRoleType
 
-from ..actions.action import ActionOutput
-from ..core.agent import Agent, AgentMessage
-from ..core.agent_manage import mentioned_agents, participant_roles
-from ..core.base_agent import ConversableAgent
-from ..core.base_team import ManagerAgent
-from ..core.schema import Status
-from ..memory.base import GptsPlan
-from .planner_agent import PlannerAgent
+from ..action.base import ActionOutput
+from ..agent import Agent, AgentMessage
+from ..agent_manage import mentioned_agents, participant_roles
+from ..base_agent import ConversableAgent
+from ..base_team import ManagerAgent
+from ..memory.gpts.base import GptsPlan
+from ..plan.planner_agent import PlannerAgent
+from ..profile import DynConfig, ProfileConfig
+from ..schema import Status
 
 logger = logging.getLogger(__name__)
 
 
 class AutoPlanChatManager(ManagerAgent):
     """A chat manager agent that can manage a team chat of multiple agents."""
 
-    profile: str = "PlanManager"
-    goal: str = (
-        "Advance the task plan generated by the planning agent. If the plan "
-        "does not pre-allocate an agent, it needs to be coordinated with the "
-        "appropriate agent to complete."
+    profile: ProfileConfig = ProfileConfig(
+        name=DynConfig(
+            "AutoPlanChatManager",
+            category="agent",
+            key="dbgpt_agent_plan_team_auto_plan_profile_name",
+        ),
+        role=DynConfig(
+            "PlanManager",
+            category="agent",
+            key="dbgpt_agent_plan_team_auto_plan_profile_role",
+        ),
+        goal=DynConfig(
+            "Advance the task plan generated by the planning agent. If the plan "
+            "does not pre-allocate an agent, it needs to be coordinated with the "
+            "appropriate agent to complete.",
+            category="agent",
+            key="dbgpt_agent_plan_team_auto_plan_profile_goal",
+        ),
+        desc=DynConfig(
+            "Advance the task plan generated by the planning agent.",
+            category="agent",
+            key="dbgpt_agent_plan_team_auto_plan_profile_desc",
+        ),
     )
-    constraints: List[str] = []
-    desc: str = "Advance the task plan generated by the planning agent."
 
     def __init__(self, **kwargs):
         """Create a new AutoPlanChatManager instance."""
         super().__init__(**kwargs)
 
     async def process_rely_message(
         self, conv_id: str, now_plan: GptsPlan, speaker: Agent
@@ -52,27 +69,29 @@
                     " historical message to complete the current goal:"
                 )
                 for rely_task in rely_tasks:
                     rely_messages.append(
                         {
                             "content": rely_task.sub_task_content,
                             "role": ModelMessageRoleType.HUMAN,
+                            "name": rely_task.sub_task_agent,
                         }
                     )
                     rely_messages.append(
                         {
                             "content": rely_task.result,
                             "role": ModelMessageRoleType.AI,
+                            "name": rely_task.sub_task_agent,
                         }
                     )
         return rely_prompt, rely_messages
 
     def select_speaker_msg(self, agents: List[Agent]) -> str:
         """Return the message for selecting the next speaker."""
-        agent_names = [agent.get_name() for agent in agents]
+        agent_names = [agent.name for agent in agents]
         return (
             "You are in a role play game. The following roles are available:\n"
             f"   {participant_roles(agents)}.\n"
             "   Read the following conversation.\n"
             f"   Then select the next role from {agent_names} to play.\n"
             "   The role can be selected repeatedly.Only return the role."
         )
@@ -91,24 +110,24 @@
             # Preselect speakers
             logger.info(f"Preselect speakers:{pre_allocated}")
             name = pre_allocated
             model = None
         else:
             # auto speaker selection
             # TODO selector a_thinking It has been overwritten and cannot be used.
-            agent_names = [agent.get_name() for agent in agents]
+            agent_names = [agent.name for agent in agents]
             fina_name, model = await selector.thinking(
                 messages=[
                     AgentMessage(
                         role=ModelMessageRoleType.HUMAN,
                         content="Read and understand the following task content and"
                         " assign the appropriate role to complete the task.\n"
                         f"Task content: {now_goal_context},\n"
                         f"Select the role from: {agent_names},\n"
-                        f"Please only return the role, such as: {agents[0].get_name()}",
+                        f"Please only return the role, such as: {agents[0].name}",
                     )
                 ],
                 prompt=self.select_speaker_msg(agents),
             )
             if not fina_name:
                 raise ValueError("Unable to select next speaker!")
             else:
@@ -265,15 +284,15 @@
                         else:
                             plan_result = reply_message["content"]
                             self.memory.plans_memory.update_task(
                                 self.not_null_agent_context.conv_id,
                                 now_plan.sub_task_num,
                                 Status.FAILED.value,
                                 now_plan.retry_times + 1,
-                                speaker.get_name(),
+                                speaker.name,
                                 "",
                                 plan_result,
                             )
                             return ActionOutput(
                                 is_exe_success=False, content=plan_result
                             )
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_chart_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_table_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/built_in/display_type/show_text_gen.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/command.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,22 +66,23 @@
         )
         result = f"{command_result}"
     return result
 
 
 def execute_command(
     command_name: str,
-    arguments,
+    arguments: Dict[str, Any],
     plugin_generator: PluginPromptGenerator,
 ) -> Any:
     """Execute the command and return the result.
 
     Args:
         command_name (str): The name of the command to execute
         arguments (dict): The arguments for the command
+        plugin_generator (PluginPromptGenerator): The plugin generator
 
     Returns:
         str: The result of the command
 
     Raises:
         NotCommandException: If the command is not found
         ExecutionCommandException: If an error occurs while executing the command
@@ -99,26 +100,31 @@
             # return f"Error: {str(e)}"
     # TODO: Change these to take in a file rather than pasted code, if
     # non-file is given, return instructions "Input should be a python
     # filepath, write your code to file and try again
     else:
         for command in plugin_generator.commands:
             if (
-                command_name == command["label"].lower()
-                or command_name == command["name"].lower()
+                command_name == command.label.lower()
+                or command_name == command.name.lower()
             ):
                 try:
-                    # 删除非定义参数
+                    # Delete non-defined parameters
                     diff_ags = list(
-                        set(arguments.keys()).difference(set(command["args"].keys()))
+                        set(arguments.keys()).difference(set(command.args.keys()))
                     )
                     for arg_name in diff_ags:
                         del arguments[arg_name]
                     print(str(arguments))
-                    return command["function"](**arguments)
+                    func = command.function
+                    if not func:
+                        raise ExecutionCommandException(
+                            f"Function not found for command: {command_name}"
+                        )
+                    return func(**arguments)
                 except Exception as e:
                     raise ExecutionCommandException(f"Execution error: {str(e)}")
         raise NotCommandException("Invalid command: " + command_name)
 
 
 def get_command(response_json: Dict):
     """Create a command from the response JSON.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/command_manage.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/command_manage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/commands/exceptions.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/commands/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/generator.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,107 @@
 """A module for generating custom prompt strings."""
-from typing import Any, Callable, Dict, List, Optional
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
+
+from dbgpt._private.pydantic import BaseModel, Field
+
+if TYPE_CHECKING:
+    from .commands.command_manage import CommandRegistry
+
+
+class CommandEntry(BaseModel):
+    """CommandEntry class.
+
+    A class for storing information about a command.
+    """
+
+    label: str = Field(
+        ...,
+        description="The label of the command.",
+    )
+    name: str = Field(
+        ...,
+        description="The name of the command.",
+    )
+    args: Dict[str, Any] = Field(
+        default_factory=dict,
+        description="A dictionary containing argument names and their values.",
+    )
+    function: Optional[Callable] = Field(
+        None,
+        description="A callable function to be called when the command is executed.",
+    )
 
 
 class PluginPromptGenerator:
     """PluginPromptGenerator class.
 
     A class for generating custom prompt strings based on constraints, commands,
         resources, and performance evaluations.
     """
 
-    def __init__(self) -> None:
+    def __init__(self):
         """Create a new PromptGenerator object.
 
         Initialize the PromptGenerator object with empty lists of constraints,
         commands, resources, and performance evaluations.
         """
         from .commands.command_manage import CommandRegistry
 
-        self.constraints: List[str] = []
-        self.commands: List[Dict[str, Any]] = []
-        self.resources: List[str] = []
-        self.performance_evaluation: List[str] = []
-        self.command_registry: CommandRegistry = CommandRegistry()
+        self._constraints: List[str] = []
+        self._commands: List[CommandEntry] = []
+        self._resources: List[str] = []
+        self._performance_evaluation: List[str] = []
+        self._command_registry: CommandRegistry = CommandRegistry()
+
+    @property
+    def constraints(self) -> List[str]:
+        """Return the list of constraints."""
+        return self._constraints
+
+    @property
+    def commands(self) -> List[CommandEntry]:
+        """Return the list of commands."""
+        return self._commands
+
+    @property
+    def resources(self) -> List[str]:
+        """Return the list of resources."""
+        return self._resources
+
+    @property
+    def performance_evaluation(self) -> List[str]:
+        """Return the list of performance evaluations."""
+        return self._performance_evaluation
+
+    @property
+    def command_registry(self) -> "CommandRegistry":
+        """Return the command registry."""
+        return self._command_registry
+
+    def set_command_registry(self, command_registry: "CommandRegistry") -> None:
+        """Set the command registry.
+
+        Args:
+            command_registry: CommandRegistry
+        """
+        self._command_registry = command_registry
 
     def add_constraint(self, constraint: str) -> None:
         """Add a constraint to the constraints list.
 
         Args:
             constraint (str): The constraint to be added.
         """
-        self.constraints.append(constraint)
+        self._constraints.append(constraint)
 
     def add_command(
         self,
         command_label: str,
         command_name: str,
-        args=None,
+        args: Optional[Dict[str, Any]] = None,
         function: Optional[Callable] = None,
     ) -> None:
         """Add a command to the commands.
 
         Add a command to the commands list with a label, name, and optional arguments.
 
         Args:
@@ -51,55 +113,54 @@
                 the command is executed. Defaults to None.
         """
         if args is None:
             args = {}
 
         command_args = {arg_key: arg_value for arg_key, arg_value in args.items()}
 
-        command = {
-            "label": command_label,
-            "name": command_name,
-            "args": command_args,
-            "function": function,
-        }
-
-        self.commands.append(command)
+        command = CommandEntry(
+            label=command_label,
+            name=command_name,
+            args=command_args,
+            function=function,
+        )
+        self._commands.append(command)
 
-    def _generate_command_string(self, command: Dict[str, Any]) -> str:
+    def _generate_command_string(self, command: CommandEntry) -> str:
         """
         Generate a formatted string representation of a command.
 
         Args:
             command (dict): A dictionary containing command information.
 
         Returns:
             str: The formatted command string.
         """
         args_string = ", ".join(
-            f'"{key}": "{value}"' for key, value in command["args"].items()
+            f'"{key}": "{value}"' for key, value in command.args.items()
         )
-        return f'"{command["name"]}": {command["label"]} , args: {args_string}'
+        return f'"{command.name}": {command.label} , args: {args_string}'
 
     def add_resource(self, resource: str) -> None:
         """
         Add a resource to the resources list.
 
         Args:
             resource (str): The resource to be added.
         """
-        self.resources.append(resource)
+        self._resources.append(resource)
 
     def add_performance_evaluation(self, evaluation: str) -> None:
         """
         Add a performance evaluation item to the performance_evaluation list.
 
         Args:
             evaluation (str): The evaluation item to be added.
         """
-        self.performance_evaluation.append(evaluation)
+        self._performance_evaluation.append(evaluation)
 
     def _generate_numbered_list(self, items: List[Any], item_type="list") -> str:
         """
         Generate a numbered list from given items based on the item_type.
 
         Args:
             items (list): A list of items to be numbered.
@@ -107,22 +168,22 @@
                 Defaults to 'list'.
 
         Returns:
             str: The formatted numbered list.
         """
         if item_type == "command":
             command_strings = []
-            if self.command_registry:
+            if self._command_registry:
                 command_strings += [
                     str(item)
-                    for item in self.command_registry.commands.values()
+                    for item in self._command_registry.commands.values()
                     if item.enabled
                 ]
             # terminate command is added manually
             command_strings += [self._generate_command_string(item) for item in items]
             return "\n".join(f"{i+1}. {item}" for i, item in enumerate(command_strings))
         else:
             return "\n".join(f"{i+1}. {item}" for i, item in enumerate(items))
 
     def generate_commands_string(self) -> str:
         """Return a formatted string representation of the commands list."""
-        return f"{self._generate_numbered_list(self.commands, item_type='command')}"
+        return f"{self._generate_numbered_list(self._commands, item_type='command')}"
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/loader.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/plugin/plugins_util.py` & `dbgpt-0.5.6rc0/dbgpt/agent/plugin/plugins_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/resource/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/agent/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_api.py` & `dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_db_api.py` & `dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_db_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_knowledge_api.py` & `dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_knowledge_api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/resource/resource_loader.py` & `dbgpt-0.5.6rc0/dbgpt/agent/resource/resource_loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/agent/util/cmp.py` & `dbgpt-0.5.6rc0/dbgpt/agent/util/cmp.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/cli/cli_scripts.py` & `dbgpt-0.5.6rc0/dbgpt/cli/cli_scripts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/client/_cli.py` & `dbgpt-0.5.6rc0/dbgpt/client/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/client/app.py` & `dbgpt-0.5.6rc0/dbgpt/client/app.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/client/client.py` & `dbgpt-0.5.6rc0/dbgpt/client/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/client/datasource.py` & `dbgpt-0.5.6rc0/dbgpt/client/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/client/flow.py` & `dbgpt-0.5.6rc0/dbgpt/client/flow.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/client/knowledge.py` & `dbgpt-0.5.6rc0/dbgpt/client/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/client/schema.py` & `dbgpt-0.5.6rc0/dbgpt/client/schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/component.py` & `dbgpt-0.5.6rc0/dbgpt/component.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/configs/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/configs/model_config.py` & `dbgpt-0.5.6rc0/dbgpt/configs/model_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,17 +65,22 @@
     "gemini_proxyllm": "gemini_proxyllm",
     "bc_proxyllm": "bc_proxyllm",
     "spark_proxyllm": "spark_proxyllm",
     # https://platform.lingyiwanwu.com/docs/
     "yi_proxyllm": "yi_proxyllm",
     # https://platform.moonshot.cn/docs/
     "moonshot_proxyllm": "moonshot_proxyllm",
+    "ollama_proxyllm": "ollama_proxyllm",
     "llama-2-7b": os.path.join(MODEL_PATH, "Llama-2-7b-chat-hf"),
     "llama-2-13b": os.path.join(MODEL_PATH, "Llama-2-13b-chat-hf"),
     "llama-2-70b": os.path.join(MODEL_PATH, "Llama-2-70b-chat-hf"),
+    # https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct
+    "meta-llama-3-8b-instruct": os.path.join(MODEL_PATH, "Meta-Llama-3-8B-Instruct"),
+    # https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct
+    "meta-llama-3-70b-instruct": os.path.join(MODEL_PATH, "Meta-Llama-3-70B-Instruct"),
     "baichuan-13b": os.path.join(MODEL_PATH, "Baichuan-13B-Chat"),
     # please rename "fireballoon/baichuan-vicuna-chinese-7b" to "baichuan-7b"
     "baichuan-7b": os.path.join(MODEL_PATH, "baichuan-7b"),
     "baichuan2-7b": os.path.join(MODEL_PATH, "Baichuan2-7B-Chat"),
     "baichuan2-13b": os.path.join(MODEL_PATH, "Baichuan2-13B-Chat"),
     # https://huggingface.co/Qwen/Qwen-7B-Chat
     "qwen-7b-chat": os.path.join(MODEL_PATH, "Qwen-7B-Chat"),
@@ -104,14 +109,20 @@
     # https://huggingface.co/Qwen/Qwen1.5-1.8B-Chat
     "qwen1.5-1.8b-chat": os.path.join(MODEL_PATH, "Qwen1.5-1.8B-Chat"),
     "qwen1.5-7b-chat": os.path.join(MODEL_PATH, "Qwen1.5-7B-Chat"),
     "qwen1.5-14b-chat": os.path.join(MODEL_PATH, "Qwen1.5-14B-Chat"),
     # https://huggingface.co/Qwen/Qwen1.5-32B-Chat
     "qwen1.5-32b-chat": os.path.join(MODEL_PATH, "Qwen1.5-32B-Chat"),
     "qwen1.5-72b-chat": os.path.join(MODEL_PATH, "Qwen1.5-72B-Chat"),
+    # https://huggingface.co/Qwen/Qwen1.5-110B-Chat
+    "qwen1.5-110b-chat": os.path.join(MODEL_PATH, "Qwen1.5-110B-Chat"),
+    # https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat
+    "codeqwen1.5-7b-chat": os.path.join(MODEL_PATH, "CodeQwen1.5-7B-Chat"),
+    # https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat
+    "qwen1.5-moe-a2.7b-chat": os.path.join(MODEL_PATH, "Qwen1.5-MoE-A2.7B-Chat"),
     # (Llama2 based) We only support WizardLM-13B-V1.2 for now, which is trained from Llama-2 13b, see https://huggingface.co/WizardLM/WizardLM-13B-V1.2
     "wizardlm-13b": os.path.join(MODEL_PATH, "WizardLM-13B-V1.2"),
     # wget https://huggingface.co/TheBloke/vicuna-13B-v1.5-GGUF/resolve/main/vicuna-13b-v1.5.Q4_K_M.gguf -O models/ggml-model-q4_0.gguf
     "llama-cpp": os.path.join(MODEL_PATH, "ggml-model-q4_0.gguf"),
     # https://huggingface.co/internlm/internlm-chat-7b-v1_1, 7b vs 7b-v1.1: https://github.com/InternLM/InternLM/issues/288
     "internlm-7b": os.path.join(MODEL_PATH, "internlm-chat-7b"),
     "internlm-7b-8k": os.path.join(MODEL_PATH, "internlm-chat-7b-8k"),
@@ -186,11 +197,12 @@
     "gte-large-zh": os.path.join(MODEL_PATH, "gte-large-zh"),
     "gte-base-zh": os.path.join(MODEL_PATH, "gte-base-zh"),
     "sentence-transforms": os.path.join(MODEL_PATH, "all-MiniLM-L6-v2"),
     "proxy_openai": "proxy_openai",
     "proxy_azure": "proxy_azure",
     # Common HTTP embedding model
     "proxy_http_openapi": "proxy_http_openapi",
+    "proxy_ollama": "proxy_ollama",
 }
 
 
 KNOWLEDGE_UPLOAD_ROOT_PATH = DATA_DIR
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/_private/example_base.py` & `dbgpt-0.5.6rc0/dbgpt/core/_private/example_base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/_private/prompt_registry.py` & `dbgpt-0.5.6rc0/dbgpt/core/_private/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/base.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/dag/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/dag_manager.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/dag/dag_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/dag/loader.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/dag/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/base.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/exceptions.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/flow/flow_factory.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/flow/flow_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/base.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/operators/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     AsyncToSyncIterator,
     BlockingFunction,
     DefaultExecutorFactory,
     blocking_func_to_async,
 )
 
 from ..dag.base import DAG, DAGContext, DAGNode, DAGVar
-from ..task.base import EMPTY_DATA, OUT, T, TaskOutput
+from ..task.base import EMPTY_DATA, OUT, T, TaskOutput, is_empty_data
 
 F = TypeVar("F", bound=FunctionType)
 
 CALL_DATA = Union[Dict[str, Any], Any]
 CURRENT_DAG_CONTEXT: ContextVar[Optional[DAGContext]] = ContextVar(
     "current_dag_context", default=None
 )
@@ -209,15 +209,15 @@
         Args:
             call_data (CALL_DATA): The data pass to root operator node.
             dag_ctx (DAGContext): The context of the DAG when this node is run,
                 Defaults to None.
         Returns:
             OUT: The output of the node after execution.
         """
-        if call_data != EMPTY_DATA:
+        if not is_empty_data(call_data):
             call_data = {"data": call_data}
         out_ctx = await self._runner.execute_workflow(
             self, call_data, exist_dag_ctx=dag_ctx
         )
         return out_ctx.current_task_context.task_output.output
 
     def _blocking_call(
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/common_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/operators/common_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/operators/stream_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/operators/stream_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/runner/job_manager.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/runner/job_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/runner/local_runner.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/runner/local_runner.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/task/base.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/task/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 PLACEHOLDER_DATA = _EMPTY_DATA_TYPE("PLACEHOLDER_DATA")
 
 
 def is_empty_data(data: Any):
     """Check if the data is empty."""
     if isinstance(data, _EMPTY_DATA_TYPE):
         return data in (EMPTY_DATA, SKIP_DATA)
+    elif hasattr(data, "empty"):
+        return getattr(data, "empty", False)
     return False
 
 
 MapFunc = Union[Callable[[IN], OUT], Callable[[IN], Awaitable[OUT]]]
 ReduceFunc = Union[Callable[[IN, IN], OUT], Callable[[IN, IN], Awaitable[OUT]]]
 StreamFunc = Callable[[IN], Awaitable[AsyncIterator[OUT]]]
 UnStreamFunc = Callable[[AsyncIterator[IN]], OUT]
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/task/task_impl.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/task/task_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/base.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/ext_http_trigger.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/ext_http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/http_trigger.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/http_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/iterator_trigger.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/iterator_trigger.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/trigger/trigger_manager.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/trigger/trigger_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/awel/util/parameter_util.py` & `dbgpt-0.5.6rc0/dbgpt/core/awel/util/parameter_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/cache.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/embeddings.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/embeddings.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/evaluation.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/knowledge.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/llm.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/llm.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/message.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/message.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/composer_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/llm_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/message_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/message_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/prompt_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/prompt_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/operators/retriever.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/operators/retriever.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/output_parser.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/output_parser.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/prompt.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/prompt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/serialization.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/interface/storage.py` & `dbgpt-0.5.6rc0/dbgpt/core/interface/storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/operators/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/core/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/operators/flow/composer_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/operators/flow/composer_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/operators/flow/dict_operator.py` & `dbgpt-0.5.6rc0/dbgpt/core/operators/flow/dict_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/core/schema/api.py` & `dbgpt-0.5.6rc0/dbgpt/core/schema/api.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/base.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -212,7 +212,12 @@
         """
         raise NotImplementedError("Current connector does not support get_indexes")
 
     @classmethod
     def is_normal_type(cls) -> bool:
         """Return whether the connector is a normal type."""
         return True
+
+    @classmethod
+    def is_graph_type(cls) -> bool:
+        """Return whether the connector is a graph database connector."""
+        return False
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/conn_spark.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/conn_spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/db_conn_info.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/db_conn_info.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/manages/connect_config_db.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/manages/connect_config_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/manages/connector_manager.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/manages/connector_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
     def on_init(self):
         """Execute on init.
 
         Load all connector classes.
         """
         from dbgpt.datasource.conn_spark import SparkConnector  # noqa: F401
+        from dbgpt.datasource.conn_tugraph import TuGraphConnector  # noqa: F401
         from dbgpt.datasource.rdbms.base import RDBMSConnector  # noqa: F401
         from dbgpt.datasource.rdbms.conn_clickhouse import (  # noqa: F401
             ClickhouseConnector,
         )
         from dbgpt.datasource.rdbms.conn_doris import DorisConnector  # noqa: F401
         from dbgpt.datasource.rdbms.conn_duckdb import DuckDbConnector  # noqa: F401
         from dbgpt.datasource.rdbms.conn_hive import HiveConnector  # noqa: F401
@@ -181,16 +182,19 @@
             db_info.db_user,
             db_info.db_pwd,
             db_info.comment,
         )
 
     async def async_db_summary_embedding(self, db_name, db_type):
         """Async db summary embedding."""
-        # TODO: async embedding
-        self.db_summary_client.db_summary_embedding(db_name, db_type)
+        executor = self.system_app.get_component(
+            ComponentType.EXECUTOR_DEFAULT, ExecutorFactory
+        ).create()  # type: ignore
+        executor.submit(self.db_summary_client.db_summary_embedding, db_name, db_type)
+        return True
 
     def add_db(self, db_info: DBConfig):
         """Add db connect info.
 
         Args:
             db_info (DBConfig): db connect info.
         """
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/operators/datasource_operator.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/operators/datasource_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/base.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_clickhouse.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_clickhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,19 @@
         """
         fields = self.get_fields(table_name)
         return [
             {"name": name, "comment": comment, "type": column_type}
             for name, column_type, _, _, comment in fields[0]
         ]
 
+    @property
+    def dialect(self) -> str:
+        """Return string representation of dialect to use."""
+        return ""
+
     def get_fields(self, table_name) -> List[Tuple]:
         """Get column fields about specified table."""
         session = self.client
 
         _query_sql = f"""
             SELECT name, type, default_expression, is_in_primary_key, comment
                 from system.columns where table='{table_name}'
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_doris.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_doris.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_duckdb.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_duckdb.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_hive.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_hive.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_mssql.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_mssql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_postgresql.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_postgresql.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_sqlite.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_sqlite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/conn_starrocks.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/conn_starrocks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py` & `dbgpt-0.5.6rc0/dbgpt/datasource/rdbms/dialect/starrocks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/base.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/embeddings_loader.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/embeddings_loader.py`

 * *Files 20% similar despite different names*

```diff
@@ -46,14 +46,24 @@
                 if proxy_param.proxy_server_url:
                     openapi_param["api_url"] = proxy_param.proxy_server_url
                 if proxy_param.proxy_api_key:
                     openapi_param["api_key"] = proxy_param.proxy_api_key
                 if proxy_param.proxy_backend:
                     openapi_param["model_name"] = proxy_param.proxy_backend
                 return OpenAPIEmbeddings(**openapi_param)
+            elif model_name in ["proxy_ollama"]:
+                from dbgpt.rag.embedding import OllamaEmbeddings
+
+                proxy_param = cast(ProxyEmbeddingParameters, param)
+                ollama_param = {}
+                if proxy_param.proxy_server_url:
+                    ollama_param["api_url"] = proxy_param.proxy_server_url
+                if proxy_param.proxy_backend:
+                    ollama_param["model_name"] = proxy_param.proxy_backend
+                return OllamaEmbeddings(**ollama_param)
             else:
                 from dbgpt.rag.embedding import HuggingFaceEmbeddings
 
                 kwargs = param.build_kwargs(model_name=param.model_path)
                 return HuggingFaceEmbeddings(**kwargs)
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/fschat_adapter.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/fschat_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/hf_adapter.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/hf_adapter.py`

 * *Files 11% similar despite different names*

```diff
@@ -263,16 +263,83 @@
             )
 
     def do_match(self, lower_model_name_or_path: Optional[str] = None):
         return (
             lower_model_name_or_path
             and "qwen" in lower_model_name_or_path
             and "1.5" in lower_model_name_or_path
+            and "moe" not in lower_model_name_or_path
         )
 
 
+class QwenMoeAdapter(NewHFChatModelAdapter):
+    """
+    https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B
+
+    TODO: There are problems with quantization.
+    """
+
+    support_4bit: bool = False
+    support_8bit: bool = False
+
+    def check_transformer_version(self, current_version: str) -> None:
+        print(f"Checking version: Current version {current_version}")
+        if not current_version >= "4.40.0":
+            raise ValueError(
+                "Qwen 1.5 Moe require transformers.__version__>=4.40.0, please upgrade your transformers package."
+            )
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return (
+            lower_model_name_or_path
+            and "qwen" in lower_model_name_or_path
+            and "1.5" in lower_model_name_or_path
+            and "moe" in lower_model_name_or_path
+        )
+
+
+class Llama3Adapter(NewHFChatModelAdapter):
+    """
+    https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct
+    https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct
+    """
+
+    support_4bit: bool = True
+    support_8bit: bool = True
+
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return lower_model_name_or_path and "llama-3" in lower_model_name_or_path
+
+    def get_str_prompt(
+        self,
+        params: Dict,
+        messages: List[ModelMessage],
+        tokenizer: Any,
+        prompt_template: str = None,
+        convert_to_compatible_format: bool = False,
+    ) -> Optional[str]:
+        str_prompt = super().get_str_prompt(
+            params,
+            messages,
+            tokenizer,
+            prompt_template,
+            convert_to_compatible_format,
+        )
+        terminators = [
+            tokenizer.eos_token_id,
+            tokenizer.convert_tokens_to_ids("<|eot_id|>"),
+        ]
+        exist_token_ids = params.get("stop_token_ids", [])
+        terminators.extend(exist_token_ids)
+        # TODO(fangyinc): We should modify the params in the future
+        params["stop_token_ids"] = terminators
+        return str_prompt
+
+
 register_model_adapter(YiAdapter)
 register_model_adapter(Mixtral8x7BAdapter)
 register_model_adapter(SOLARAdapter)
 register_model_adapter(GemmaAdapter)
 register_model_adapter(StarlingLMAdapter)
 register_model_adapter(QwenAdapter)
+register_model_adapter(QwenMoeAdapter)
+register_model_adapter(Llama3Adapter)
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/loader.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/model_adapter.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/model_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/old_adapter.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/old_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/proxy_adapter.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/proxy_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,31 @@
 
     def get_generate_stream_function(self, model, model_path: str):
         from dbgpt.model.proxy.llms.tongyi import tongyi_generate_stream
 
         return tongyi_generate_stream
 
 
+class OllamaLLMModelAdapter(ProxyLLMModelAdapter):
+    def do_match(self, lower_model_name_or_path: Optional[str] = None):
+        return lower_model_name_or_path == "ollama_proxyllm"
+
+    def get_llm_client_class(
+        self, params: ProxyModelParameters
+    ) -> Type[ProxyLLMClient]:
+        from dbgpt.model.proxy.llms.ollama import OllamaLLMClient
+
+        return OllamaLLMClient
+
+    def get_generate_stream_function(self, model, model_path: str):
+        from dbgpt.model.proxy.llms.ollama import ollama_generate_stream
+
+        return ollama_generate_stream
+
+
 class ZhipuProxyLLMModelAdapter(ProxyLLMModelAdapter):
     support_system_message = False
 
     def do_match(self, lower_model_name_or_path: Optional[str] = None):
         return lower_model_name_or_path == "zhipu_proxyllm"
 
     def get_llm_client_class(
@@ -275,14 +292,15 @@
         from dbgpt.model.proxy.llms.moonshot import moonshot_generate_stream
 
         return moonshot_generate_stream
 
 
 register_model_adapter(OpenAIProxyLLMModelAdapter)
 register_model_adapter(TongyiProxyLLMModelAdapter)
+register_model_adapter(OllamaLLMModelAdapter)
 register_model_adapter(ZhipuProxyLLMModelAdapter)
 register_model_adapter(WenxinProxyLLMModelAdapter)
 register_model_adapter(GeminiProxyLLMModelAdapter)
 register_model_adapter(SparkProxyLLMModelAdapter)
 register_model_adapter(BardProxyLLMModelAdapter)
 register_model_adapter(BaichuanProxyLLMModelAdapter)
 register_model_adapter(YiProxyLLMModelAdapter)
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/template.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/adapter/vllm_adapter.py` & `dbgpt-0.5.6rc0/dbgpt/model/adapter/vllm_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/base.py` & `dbgpt-0.5.6rc0/dbgpt/model/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/cli.py` & `dbgpt-0.5.6rc0/dbgpt/model/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/operators/llm_operator.py` & `dbgpt-0.5.6rc0/dbgpt/model/operators/llm_operator.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/parameter.py` & `dbgpt-0.5.6rc0/dbgpt/model/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,15 +552,15 @@
         }
         for k, v in kwargs:
             params[k] = v
         return params
 
 
 _EMBEDDING_PARAMETER_CLASS_TO_NAME_CONFIG = {
-    ProxyEmbeddingParameters: "proxy_openai,proxy_azure,proxy_http_openapi",
+    ProxyEmbeddingParameters: "proxy_openai,proxy_azure,proxy_http_openapi,proxy_ollama",
 }
 
 EMBEDDING_NAME_TO_PARAMETER_CLASS_CONFIG = {}
 
 
 def _update_embedding_config():
     global EMBEDDING_NAME_TO_PARAMETER_CLASS_CONFIG
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         "GeminiLLMClient": "dbgpt.model.proxy.llms.gemini",
         "SparkLLMClient": "dbgpt.model.proxy.llms.spark",
         "TongyiLLMClient": "dbgpt.model.proxy.llms.tongyi",
         "WenxinLLMClient": "dbgpt.model.proxy.llms.wenxin",
         "ZhipuLLMClient": "dbgpt.model.proxy.llms.zhipu",
         "YiLLMClient": "dbgpt.model.proxy.llms.yi",
         "MoonshotLLMClient": "dbgpt.model.proxy.llms.moonshot",
+        "OllamaLLMClient": "dbgpt.model.proxy.llms.ollama",
     }
 
     if name in module_path:
         module = __import__(module_path[name], fromlist=[name])
         return getattr(module, name)
     else:
         raise AttributeError(f"module {__name__} has no attribute {name}")
@@ -29,8 +30,9 @@
     "GeminiLLMClient",
     "TongyiLLMClient",
     "ZhipuLLMClient",
     "WenxinLLMClient",
     "SparkLLMClient",
     "YiLLMClient",
     "MoonshotLLMClient",
+    "OllamaLLMClient",
 ]
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/base.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/baichuan.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/baichuan.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/bard.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/bard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/chatgpt.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/chatgpt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/gemini.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/gemini.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/moonshot.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/moonshot.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/proxy_model.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/proxy_model.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/spark.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/spark.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/tongyi.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/tongyi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/wenxin.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/wenxin.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/yi.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/yi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/proxy/llms/zhipu.py` & `dbgpt-0.5.6rc0/dbgpt/model/proxy/llms/zhipu.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/utils/chatgpt_utils.py` & `dbgpt-0.5.6rc0/dbgpt/model/utils/chatgpt_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/utils/llm_utils.py` & `dbgpt-0.5.6rc0/dbgpt/model/utils/llm_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/model/utils/token_utils.py` & `dbgpt-0.5.6rc0/dbgpt/model/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/assembler/base.py` & `dbgpt-0.5.6rc0/dbgpt/rag/assembler/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/assembler/db_schema.py` & `dbgpt-0.5.6rc0/dbgpt/rag/assembler/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/assembler/embedding.py` & `dbgpt-0.5.6rc0/dbgpt/rag/assembler/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/assembler/summary.py` & `dbgpt-0.5.6rc0/dbgpt/rag/assembler/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/chunk_manager.py` & `dbgpt-0.5.6rc0/dbgpt/rag/chunk_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/embedding/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/rag/embedding/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 from .embeddings import (  # noqa: F401
     Embeddings,
     HuggingFaceBgeEmbeddings,
     HuggingFaceEmbeddings,
     HuggingFaceInferenceAPIEmbeddings,
     HuggingFaceInstructEmbeddings,
     JinaEmbeddings,
+    OllamaEmbeddings,
     OpenAPIEmbeddings,
 )
 
 __ALL__ = [
     "Embeddings",
     "HuggingFaceBgeEmbeddings",
     "HuggingFaceEmbeddings",
     "HuggingFaceInferenceAPIEmbeddings",
     "HuggingFaceInstructEmbeddings",
     "JinaEmbeddings",
     "OpenAPIEmbeddings",
+    "OllamaEmbeddings",
     "DefaultEmbeddingFactory",
     "EmbeddingFactory",
     "WrappedEmbeddingFactory",
 ]
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/embedding/_wrapped.py` & `dbgpt-0.5.6rc0/dbgpt/rag/embedding/_wrapped.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/embedding/embedding_factory.py` & `dbgpt-0.5.6rc0/dbgpt/rag/embedding/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/embedding/embeddings.py` & `dbgpt-0.5.6rc0/dbgpt/rag/embedding/embeddings.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,39 +65,41 @@
     """
 
     model_config = ConfigDict(extra=EXTRA_FORBID, protected_namespaces=())
 
     client: Any  #: :meta private:
     model_name: str = DEFAULT_MODEL_NAME
     """Model name to use."""
-    cache_folder: Optional[str] = None
+    cache_folder: Optional[str] = Field(None, description="Path of the cache folder.")
     """Path to store models. Can be also set by SENTENCE_TRANSFORMERS_HOME
     environment variable."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
     """Keyword arguments to pass to the model."""
     encode_kwargs: Dict[str, Any] = Field(default_factory=dict)
     """Keyword arguments to pass when calling the `encode` method of the model."""
     multi_process: bool = False
     """Run encode() on multiple GPUs."""
 
     def __init__(self, **kwargs: Any):
         """Initialize the sentence_transformer."""
-        super().__init__(**kwargs)
         try:
             import sentence_transformers
 
         except ImportError as exc:
             raise ImportError(
                 "Could not import sentence_transformers python package. "
                 "Please install it with `pip install sentence-transformers`."
             ) from exc
 
-        self.client = sentence_transformers.SentenceTransformer(
-            self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
+        kwargs["client"] = sentence_transformers.SentenceTransformer(
+            kwargs.get("model_name"),
+            cache_folder=kwargs.get("cache_folder"),
+            **kwargs.get("model_kwargs"),
         )
+        super().__init__(**kwargs)
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace transformer model.
 
         Args:
             texts: The list of texts to embed.
 
@@ -196,24 +198,27 @@
     embed_instruction: str = DEFAULT_EMBED_INSTRUCTION
     """Instruction to use for embedding documents."""
     query_instruction: str = DEFAULT_QUERY_INSTRUCTION
     """Instruction to use for embedding query."""
 
     def __init__(self, **kwargs: Any):
         """Initialize the sentence_transformer."""
-        super().__init__(**kwargs)
         try:
             from InstructorEmbedding import INSTRUCTOR
 
-            self.client = INSTRUCTOR(
-                self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
+            kwargs["client"] = INSTRUCTOR(
+                kwargs.get("model_name"),
+                cache_folder=kwargs.get("cache_folder"),
+                **kwargs.get("model_kwargs"),
             )
         except ImportError as e:
             raise ImportError("Dependencies for InstructorEmbedding not found.") from e
 
+        super().__init__(**kwargs)
+
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace instruct model.
 
         Args:
             texts: The list of texts to embed.
 
         Returns:
@@ -274,27 +279,30 @@
     encode_kwargs: Dict[str, Any] = Field(default_factory=dict)
     """Keyword arguments to pass when calling the `encode` method of the model."""
     query_instruction: str = DEFAULT_QUERY_BGE_INSTRUCTION_EN
     """Instruction to use for embedding query."""
 
     def __init__(self, **kwargs: Any):
         """Initialize the sentence_transformer."""
-        super().__init__(**kwargs)
         try:
             import sentence_transformers
 
         except ImportError as exc:
             raise ImportError(
                 "Could not import sentence_transformers python package. "
                 "Please install it with `pip install sentence_transformers`."
             ) from exc
 
-        self.client = sentence_transformers.SentenceTransformer(
-            self.model_name, cache_folder=self.cache_folder, **self.model_kwargs
+        kwargs["client"] = sentence_transformers.SentenceTransformer(
+            kwargs.get("model_name"),
+            cache_folder=kwargs.get("cache_folder"),
+            **kwargs.get("model_kwargs"),
         )
+
+        super().__init__(**kwargs)
         if "-zh" in self.model_name:
             self.query_instruction = DEFAULT_QUERY_BGE_INSTRUCTION_ZH
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Compute doc embeddings using a HuggingFace transformer model.
 
         Args:
@@ -476,27 +484,38 @@
     """API key for the Jina AI API.."""
     model_name: str = "jina-embeddings-v2-base-en"
     """The name of the model to use for text embeddings. Defaults to
     "jina-embeddings-v2-base-en"."""
 
     def __init__(self, **kwargs):
         """Create a new JinaEmbeddings instance."""
-        super().__init__(**kwargs)
         try:
             import requests
         except ImportError:
             raise ValueError(
                 "The requests python package is not installed. Please install it with "
                 "`pip install requests`"
             )
-        self.api_url = "https://api.jina.ai/v1/embeddings"
-        self.session = requests.Session()
-        self.session.headers.update(
-            {"Authorization": f"Bearer {self.api_key}", "Accept-Encoding": "identity"}
-        )
+        if "api_url" not in kwargs:
+            kwargs["api_url"] = "https://api.jina.ai/v1/embeddings"
+        if "session" not in kwargs:  # noqa: SIM401
+            session = requests.Session()
+        else:
+            session = kwargs["session"]
+        api_key = kwargs.get("api_key")
+        if api_key:
+            session.headers.update(
+                {
+                    "Authorization": f"Bearer {api_key}",
+                    "Accept-Encoding": "identity",
+                }
+            )
+        kwargs["session"] = session
+
+        super().__init__(**kwargs)
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Get the embeddings for a list of texts.
 
         Args:
             texts (Documents): A list of texts to get embeddings for.
 
@@ -638,24 +657,30 @@
         default=60, description="The timeout for the request in seconds."
     )
 
     session: Optional[requests.Session] = None
 
     def __init__(self, **kwargs):
         """Initialize the OpenAPIEmbeddings."""
-        super().__init__(**kwargs)
         try:
             import requests
         except ImportError:
             raise ValueError(
                 "The requests python package is not installed. "
                 "Please install it with `pip install requests`"
             )
-        self.session = requests.Session()
-        self.session.headers.update({"Authorization": f"Bearer {self.api_key}"})
+        if "session" not in kwargs:  # noqa: SIM401
+            session = requests.Session()
+        else:
+            session = kwargs["session"]
+        api_key = kwargs.get("api_key")
+        if api_key:
+            session.headers.update({"Authorization": f"Bearer {api_key}"})
+        kwargs["session"] = session
+        super().__init__(**kwargs)
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
         """Get the embeddings for a list of texts.
 
         Args:
             texts (Documents): A list of texts to get embeddings for.
 
@@ -707,7 +732,98 @@
                 sorted_embeddings = sorted(embeddings, key=lambda e: e["index"])
                 return [result["embedding"] for result in sorted_embeddings]
 
     async def aembed_query(self, text: str) -> List[float]:
         """Asynchronous Embed query text."""
         embeddings = await self.aembed_documents([text])
         return embeddings[0]
+
+
+class OllamaEmbeddings(BaseModel, Embeddings):
+    """Ollama proxy embeddings.
+
+    This class is used to get embeddings for a list of texts using the Ollama API.
+    It requires a proxy server url `api_url` and a model name `model_name`.
+    The default model name is "llama2".
+    """
+
+    api_url: str = Field(
+        default="http://localhost:11434",
+        description="The URL of the embeddings API.",
+    )
+    model_name: str = Field(
+        default="llama2", description="The name of the model to use."
+    )
+
+    def __init__(self, **kwargs):
+        """Initialize the OllamaEmbeddings."""
+        super().__init__(**kwargs)
+
+    def embed_documents(self, texts: List[str]) -> List[List[float]]:
+        """Get the embeddings for a list of texts.
+
+        Args:
+            texts (Documents): A list of texts to get embeddings for.
+
+        Returns:
+            Embedded texts as List[List[float]], where each inner List[float]
+                corresponds to a single input text.
+        """
+        return [self.embed_query(text) for text in texts]
+
+    def embed_query(self, text: str) -> List[float]:
+        """Compute query embeddings using a OpenAPI embedding model.
+
+        Args:
+            text: The text to embed.
+
+        Returns:
+            Embeddings for the text.
+        """
+        try:
+            import ollama
+            from ollama import Client
+        except ImportError as e:
+            raise ValueError(
+                "Could not import python package: ollama "
+                "Please install ollama by command `pip install ollama"
+            ) from e
+        try:
+            return (
+                Client(self.api_url).embeddings(model=self.model_name, prompt=text)
+            )["embedding"]
+        except ollama.ResponseError as e:
+            raise ValueError(f"**Ollama Response Error, Please CheckErrorInfo.**: {e}")
+
+    async def aembed_documents(self, texts: List[str]) -> List[List[float]]:
+        """Asynchronous Embed search docs.
+
+        Args:
+            texts: A list of texts to get embeddings for.
+
+        Returns:
+            List[List[float]]: Embedded texts as List[List[float]], where each inner
+                List[float] corresponds to a single input text.
+        """
+        embeddings = []
+        for text in texts:
+            embedding = await self.aembed_query(text)
+            embeddings.append(embedding)
+        return embeddings
+
+    async def aembed_query(self, text: str) -> List[float]:
+        """Asynchronous Embed query text."""
+        try:
+            import ollama
+            from ollama import AsyncClient
+        except ImportError:
+            raise ValueError(
+                "The ollama python package is not installed. "
+                "Please install it with `pip install ollama`"
+            )
+        try:
+            embedding = await AsyncClient(host=self.api_url).embeddings(
+                model=self.model_name, prompt=text
+            )
+            return embedding["embedding"]
+        except ollama.ResponseError as e:
+            raise ValueError(f"**Ollama Response Error, Please CheckErrorInfo.**: {e}")
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/extractor/base.py` & `dbgpt-0.5.6rc0/dbgpt/rag/extractor/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/extractor/summary.py` & `dbgpt-0.5.6rc0/dbgpt/rag/extractor/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/base.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/csv.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/csv.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/datasource.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/string.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,61 @@
-"""Datasource Knowledge."""
+"""String Knowledge."""
 from typing import Any, Dict, List, Optional, Union
 
 from dbgpt.core import Document
-from dbgpt.datasource import BaseConnector
+from dbgpt.rag.knowledge.base import ChunkStrategy, Knowledge, KnowledgeType
 
-from ..summary.rdbms_db_summary import _parse_db_summary
-from .base import ChunkStrategy, DocumentType, Knowledge, KnowledgeType
 
-
-class DatasourceKnowledge(Knowledge):
-    """Datasource Knowledge."""
+class StringKnowledge(Knowledge):
+    """String Knowledge."""
 
     def __init__(
         self,
-        connector: BaseConnector,
-        summary_template: str = "{table_name}({columns})",
-        knowledge_type: Optional[KnowledgeType] = KnowledgeType.DOCUMENT,
+        text: str = "",
+        knowledge_type: KnowledgeType = KnowledgeType.TEXT,
+        encoding: Optional[str] = "utf-8",
+        loader: Optional[Any] = None,
         metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create Datasource Knowledge with Knowledge arguments.
+        """Create String knowledge parameters.
 
         Args:
-            connector(BaseConnector): connector
-            summary_template(str, optional): summary template
-            knowledge_type(KnowledgeType, optional): knowledge type
-            metadata(Dict[str, Union[str, List[str]], optional): metadata
+            text(str): text
+            knowledge_type(KnowledgeType): knowledge type
+            encoding(str): encoding
+            loader(Any): loader
         """
-        self._connector = connector
-        self._summary_template = summary_template
-        super().__init__(knowledge_type=knowledge_type, metadata=metadata, **kwargs)
+        super().__init__(
+            knowledge_type=knowledge_type,
+            data_loader=loader,
+            metadata=metadata,
+            **kwargs,
+        )
+        self._text = text
+        self._encoding = encoding
 
     def _load(self) -> List[Document]:
-        """Load datasource document from data_loader."""
-        docs = []
-        for table_summary in _parse_db_summary(self._connector, self._summary_template):
-            metadata = {"source": "database"}
-            if self._metadata:
-                metadata.update(self._metadata)  # type: ignore
-            docs.append(Document(content=table_summary, metadata=metadata))
+        """Load raw text from loader."""
+        metadata = {"source": "raw text"}
+        if self._metadata:
+            metadata.update(self._metadata)  # type: ignore
+        docs = [Document(content=self._text, metadata=metadata)]
         return docs
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
         ]
 
     @classmethod
-    def type(cls) -> KnowledgeType:
-        """Knowledge type of Datasource."""
-        return KnowledgeType.DOCUMENT
+    def default_chunk_strategy(cls) -> ChunkStrategy:
+        """Return default chunk strategy."""
+        return ChunkStrategy.CHUNK_BY_SIZE
 
     @classmethod
-    def document_type(cls) -> DocumentType:
-        """Return document type."""
-        return DocumentType.DATASOURCE
+    def type(cls):
+        """Return knowledge type."""
+        return KnowledgeType.TEXT
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/docx.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/docx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/factory.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/html.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/html.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/markdown.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/markdown.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pdf.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pdf.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/pptx.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/pptx.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/string.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/url.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,55 @@
-"""String Knowledge."""
-from typing import Any, Dict, List, Optional, Union
+"""URL Knowledge."""
+from typing import Any, List, Optional
 
 from dbgpt.core import Document
 from dbgpt.rag.knowledge.base import ChunkStrategy, Knowledge, KnowledgeType
 
 
-class StringKnowledge(Knowledge):
-    """String Knowledge."""
+class URLKnowledge(Knowledge):
+    """URL Knowledge."""
 
     def __init__(
         self,
-        text: str = "",
-        knowledge_type: KnowledgeType = KnowledgeType.TEXT,
+        url: str = "",
+        knowledge_type: KnowledgeType = KnowledgeType.URL,
+        source_column: Optional[str] = None,
         encoding: Optional[str] = "utf-8",
         loader: Optional[Any] = None,
-        metadata: Optional[Dict[str, Union[str, List[str]]]] = None,
         **kwargs: Any,
     ) -> None:
-        """Create String knowledge parameters.
+        """Create URL Knowledge with Knowledge arguments.
 
         Args:
-            text(str): text
-            knowledge_type(KnowledgeType): knowledge type
-            encoding(str): encoding
-            loader(Any): loader
+            url(str,  optional): url
+            knowledge_type(KnowledgeType, optional): knowledge type
+            source_column(str, optional): source column
+            encoding(str, optional): csv encoding
+            loader(Any, optional): loader
         """
         super().__init__(
-            knowledge_type=knowledge_type,
-            data_loader=loader,
-            metadata=metadata,
-            **kwargs,
+            path=url, knowledge_type=knowledge_type, loader=loader, **kwargs
         )
-        self._text = text
         self._encoding = encoding
+        self._source_column = source_column
 
     def _load(self) -> List[Document]:
-        """Load raw text from loader."""
-        metadata = {"source": "raw text"}
-        if self._metadata:
-            metadata.update(self._metadata)  # type: ignore
-        docs = [Document(content=self._text, metadata=metadata)]
-        return docs
+        """Fetch URL document from loader."""
+        if self._loader:
+            documents = self._loader.load()
+        else:
+            from langchain.document_loaders import WebBaseLoader
+
+            if self._path is not None:
+                web_reader = WebBaseLoader(web_path=self._path)
+                documents = web_reader.load()
+            else:
+                # Handle the case where self._path is None
+                raise ValueError("web_path cannot be None")
+        return [Document.langchain2doc(lc_document) for lc_document in documents]
 
     @classmethod
     def support_chunk_strategy(cls) -> List[ChunkStrategy]:
         """Return support chunk strategy."""
         return [
             ChunkStrategy.CHUNK_BY_SIZE,
             ChunkStrategy.CHUNK_BY_SEPARATOR,
@@ -54,8 +59,8 @@
     def default_chunk_strategy(cls) -> ChunkStrategy:
         """Return default chunk strategy."""
         return ChunkStrategy.CHUNK_BY_SIZE
 
     @classmethod
     def type(cls):
         """Return knowledge type."""
-        return KnowledgeType.TEXT
+        return KnowledgeType.URL
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/knowledge/txt.py` & `dbgpt-0.5.6rc0/dbgpt/rag/knowledge/txt.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/assembler.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/assembler.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/datasource.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/datasource.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/db_schema.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/embedding.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/embedding.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/evaluation.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/evaluation.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/knowledge.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/knowledge.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/rerank.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/rerank.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/rewrite.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/schema_linking.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/operators/summary.py` & `dbgpt-0.5.6rc0/dbgpt/rag/operators/summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/retriever/base.py` & `dbgpt-0.5.6rc0/dbgpt/rag/retriever/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Base retriever module."""
 from abc import ABC, abstractmethod
 from enum import Enum
-from typing import List, Optional
+from typing import Any, Dict, List, Optional
 
 from dbgpt.core import Chunk
 from dbgpt.storage.vector_store.filters import MetadataFilters
 
 
 class RetrieverStrategy(str, Enum):
     """Retriever strategy.
@@ -20,14 +20,23 @@
     KEYWORD = "keyword"
     HYBRID = "hybrid"
 
 
 class BaseRetriever(ABC):
     """Base retriever."""
 
+    def load_document(self, chunks: List[Chunk], **kwargs: Dict[str, Any]) -> List[str]:
+        """Load document in vector database.
+
+        Args:
+            - chunks: document chunks.
+        Return chunk ids.
+        """
+        raise NotImplementedError
+
     def retrieve(
         self, query: str, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Retrieve knowledge chunks.
 
         Args:
             query (str): query text.
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/retriever/db_schema.py` & `dbgpt-0.5.6rc0/dbgpt/rag/retriever/db_schema.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/retriever/embedding.py` & `dbgpt-0.5.6rc0/dbgpt/rag/retriever/embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Embedding retriever."""
 from functools import reduce
-from typing import List, Optional, cast
+from typing import Any, Dict, List, Optional, cast
 
 from dbgpt.core import Chunk
 from dbgpt.rag.retriever.base import BaseRetriever
 from dbgpt.rag.retriever.rerank import DefaultRanker, Ranker
 from dbgpt.rag.retriever.rewrite import QueryRewrite
 from dbgpt.storage.vector_store.connector import VectorStoreConnector
 from dbgpt.storage.vector_store.filters import MetadataFilters
@@ -62,14 +62,24 @@
                 )
         """
         self._top_k = top_k
         self._query_rewrite = query_rewrite
         self._vector_store_connector = vector_store_connector
         self._rerank = rerank or DefaultRanker(self._top_k)
 
+    def load_document(self, chunks: List[Chunk], **kwargs: Dict[str, Any]) -> List[str]:
+        """Load document in vector database.
+
+        Args:
+            chunks (List[Chunk]): document chunks.
+        Return:
+            List[str]: chunk ids.
+        """
+        return self._vector_store_connector.load_document(chunks)
+
     def _retrieve(
         self, query: str, filters: Optional[MetadataFilters] = None
     ) -> List[Chunk]:
         """Retrieve knowledge chunks.
 
         Args:
             query (str): query text
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/retriever/rerank.py` & `dbgpt-0.5.6rc0/dbgpt/rag/retriever/rerank.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,26 +20,27 @@
             topk: int
             rank_fn: Optional[callable]
         """
         self.topk = topk
         self.rank_fn = rank_fn
 
     @abstractmethod
-    def rank(self, candidates_with_scores: List) -> List[Chunk]:
+    def rank(
+        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
+    ) -> List[Chunk]:
         """Return top k chunks after ranker.
 
         Rank algorithm implementation return topk documents by candidates
         similarity score
 
         Args:
             candidates_with_scores: List[Tuple]
-            topk: int
-
+            query: Optional[str]
         Return:
-            List[Document]
+            List[Chunk]
         """
 
     def _filter(self, candidates_with_scores: List) -> List[Chunk]:
         """Filter duplicate candidates documents."""
         candidates_with_scores = sorted(
             candidates_with_scores, key=lambda x: x.score, reverse=True
         )
@@ -73,19 +74,25 @@
         #     default=None,
         # ),
     ],
 )
 class DefaultRanker(Ranker):
     """Default Ranker."""
 
-    def __init__(self, topk: int, rank_fn: Optional[RANK_FUNC] = None):
+    def __init__(
+        self,
+        topk: int = 4,
+        rank_fn: Optional[RANK_FUNC] = None,
+    ):
         """Create Default Ranker with topk and rank_fn."""
         super().__init__(topk, rank_fn)
 
-    def rank(self, candidates_with_scores: List[Chunk]) -> List[Chunk]:
+    def rank(
+        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
+    ) -> List[Chunk]:
         """Return top k chunks after ranker.
 
         Return top k documents by candidates similarity score
 
         Args:
             candidates_with_scores: List[Tuple]
 
@@ -101,19 +108,25 @@
             )
         return candidates_with_scores[: self.topk]
 
 
 class RRFRanker(Ranker):
     """RRF(Reciprocal Rank Fusion) Ranker."""
 
-    def __init__(self, topk: int, rank_fn: Optional[RANK_FUNC] = None):
+    def __init__(
+        self,
+        topk: int = 4,
+        rank_fn: Optional[RANK_FUNC] = None,
+    ):
         """RRF rank algorithm implementation."""
         super().__init__(topk, rank_fn)
 
-    def rank(self, candidates_with_scores: List[Chunk]) -> List[Chunk]:
+    def rank(
+        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
+    ) -> List[Chunk]:
         """RRF rank algorithm implementation.
 
         This code implements an algorithm called Reciprocal Rank Fusion (RRF), is a
         method for combining multiple result sets with different relevance indicators
         into a single result set. RRF requires no tuning, and the different relevance
         indicators do not have to be related to each other to achieve high-quality
         results.
@@ -124,7 +137,91 @@
             if d in result(q):
                 score += 1.0 / ( k + rank( result(q), d ) )
         return score
         reference:https://www.elastic.co/guide/en/elasticsearch/reference/current/rrf.html
         """
         # it will be implemented soon when multi recall is implemented
         return candidates_with_scores
+
+
+@register_resource(
+    _("CrossEncoder Rerank"),
+    "cross_encoder_ranker",
+    category=ResourceCategory.RAG,
+    description=_("CrossEncoder ranker."),
+    parameters=[
+        Parameter.build_from(
+            _("Top k"),
+            "topk",
+            int,
+            description=_("The number of top k documents."),
+        ),
+        Parameter.build_from(
+            _("Rerank Model"),
+            "model",
+            str,
+            description=_("rerank model name, e.g., 'BAAI/bge-reranker-base'."),
+        ),
+        Parameter.build_from(
+            _("device"),
+            "device",
+            str,
+            description=_("device name, e.g., 'cpu'."),
+        ),
+    ],
+)
+class CrossEncoderRanker(Ranker):
+    """CrossEncoder Ranker."""
+
+    def __init__(
+        self,
+        topk: int = 4,
+        model: str = "BAAI/bge-reranker-base",
+        device: str = "cpu",
+        rank_fn: Optional[RANK_FUNC] = None,
+    ):
+        """Cross Encoder rank algorithm implementation.
+
+        Args:
+            topk: int - The number of top k documents.
+            model: str - rerank model name, e.g., 'BAAI/bge-reranker-base'.
+            device: str - device name, e.g., 'cpu'.
+            rank_fn: Optional[callable] - The rank function.
+        Refer: https://www.sbert.net/examples/applications/cross-encoder/README.html
+        """
+        try:
+            from sentence_transformers import CrossEncoder
+        except ImportError:
+            raise ImportError(
+                "please `pip install sentence-transformers`",
+            )
+        self._model = CrossEncoder(model, max_length=512, device=device)
+        super().__init__(topk, rank_fn)
+
+    def rank(
+        self, candidates_with_scores: List[Chunk], query: Optional[str] = None
+    ) -> List[Chunk]:
+        """Cross Encoder rank algorithm implementation.
+
+        Args:
+            candidates_with_scores: List[Chunk], candidates with scores
+            query: Optional[str], query text
+        Returns:
+            List[Chunk], reranked candidates
+        """
+        contents = [candidate.content for candidate in candidates_with_scores]
+        query_content_pairs = [
+            [
+                query,
+                content,
+            ]
+            for content in contents
+        ]
+        rank_scores = self._model.predict(sentences=query_content_pairs)
+
+        for candidate, score in zip(candidates_with_scores, rank_scores):
+            candidate.score = score
+
+        new_candidates_with_scores = sorted(
+            candidates_with_scores, key=lambda x: x.score, reverse=True
+        )
+        return new_candidates_with_scores[: self.topk]
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/retriever/rewrite.py` & `dbgpt-0.5.6rc0/dbgpt/rag/retriever/rewrite.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/base_linker.py` & `dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/base_linker.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/schemalinker/schema_linking.py` & `dbgpt-0.5.6rc0/dbgpt/rag/schemalinker/schema_linking.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary.py` & `dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/summary/db_summary_client.py` & `dbgpt-0.5.6rc0/dbgpt/rag/summary/db_summary_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import traceback
 
 from dbgpt._private.config import Config
 from dbgpt.component import SystemApp
 from dbgpt.configs.model_config import EMBEDDING_MODEL_CONFIG
+from dbgpt.rag.summary.gdbms_db_summary import GdbmsSummary
 from dbgpt.rag.summary.rdbms_db_summary import RdbmsSummary
 
 logger = logging.getLogger(__name__)
 
 CFG = Config()
 
 
@@ -35,15 +36,15 @@
         )
         self.embeddings = embedding_factory.create(
             model_name=EMBEDDING_MODEL_CONFIG[CFG.EMBEDDING_MODEL]
         )
 
     def db_summary_embedding(self, dbname, db_type):
         """Put db profile and table profile summary into vector store."""
-        db_summary_client = RdbmsSummary(dbname, db_type)
+        db_summary_client = self.create_summary_client(dbname, db_type)
 
         self.init_db_profile(db_summary_client, dbname)
 
         logger.info("db summary embedding success")
 
     def get_db_summary(self, dbname, query, topk):
         """Get user query related tables info."""
@@ -103,7 +104,36 @@
                 connector=db_summary_client.db, vector_store_connector=vector_connector
             )
             if len(db_assembler.get_chunks()) > 0:
                 db_assembler.persist()
         else:
             logger.info(f"Vector store name {vector_store_name} exist")
         logger.info("initialize db summary profile success...")
+
+    def delete_db_profile(self, dbname):
+        """Delete db profile."""
+        vector_store_name = dbname + "_profile"
+        from dbgpt.storage.vector_store.base import VectorStoreConfig
+        from dbgpt.storage.vector_store.connector import VectorStoreConnector
+
+        vector_store_config = VectorStoreConfig(name=vector_store_name)
+        vector_connector = VectorStoreConnector.from_default(
+            CFG.VECTOR_STORE_TYPE,
+            self.embeddings,
+            vector_store_config=vector_store_config,
+        )
+        vector_connector.delete_vector_name(vector_store_name)
+        logger.info(f"delete db profile {dbname} success")
+
+    @staticmethod
+    def create_summary_client(dbname: str, db_type: str):
+        """
+        Create a summary client based on the database type.
+
+        Args:
+            dbname (str): The name of the database.
+            db_type (str): The type of the database.
+        """
+        if "graph" in db_type:
+            return GdbmsSummary(dbname, db_type)
+        else:
+            return RdbmsSummary(dbname, db_type)
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/summary/rdbms_db_summary.py` & `dbgpt-0.5.6rc0/dbgpt/rag/summary/rdbms_db_summary.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/pre_text_splitter.py` & `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/pre_text_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/text_splitter.py` & `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/text_splitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -511,15 +511,16 @@
             ):
                 # If the last line in the aggregated list
                 # has the same metadata as the current line,
                 # append the current content to the last lines's content
                 aggregated_chunks[-1]["content"] += "  \n" + line["content"]
             else:
                 # Otherwise, append the current line to the aggregated list
-                line["content"] = f"{line['metadata']}, " + line["content"]
+                subtitles = "-".join((list(line["metadata"].values())))
+                line["content"] = f'"{subtitles}": ' + line["content"]
                 aggregated_chunks.append(line)
 
         return [
             Chunk(content=chunk["content"], metadata=chunk["metadata"])
             for chunk in aggregated_chunks
         ]
 
@@ -553,24 +554,36 @@
         # Content and metadata of the chunk currently being processed
         current_content: List[str] = []
         current_metadata: Dict[str, str] = {}
         # Keep track of the nested header structure
         # header_stack: List[Dict[str, Union[int, str]]] = []
         header_stack: List[HeaderType] = []
         initial_metadata: Dict[str, str] = {}
+        # Determine whether a line is within a markdown code block.
+        in_code_block = False
         for line in lines:
             stripped_line = line.strip()
+            # A code frame starts with "```"
+            with_code_frame = stripped_line.startswith("```") and (
+                stripped_line != "```"
+            )
+            if (not in_code_block) and with_code_frame:
+                in_code_block = True
             # Check each line against each of the header types (e.g., #, ##)
             for sep, name in self.headers_to_split_on:
                 # Check if line starts with a header that we intend to split on
-                if stripped_line.startswith(sep) and (
-                    # Header with no text OR header is followed by space
-                    # Both are valid conditions that sep is being used a header
-                    len(stripped_line) == len(sep)
-                    or stripped_line[len(sep)] == " "
+                if (
+                    (not in_code_block)
+                    and stripped_line.startswith(sep)
+                    and (
+                        # Header with no text OR header is followed by space
+                        # Both are valid conditions that sep is being used a header
+                        len(stripped_line) == len(sep)
+                        or stripped_line[len(sep)] == " "
+                    )
                 ):
                     # Ensure we are tracking the header as metadata
                     if name is not None:
                         # Get the current header level
                         current_header_level = sep.count("#")
 
                         # Pop out headers of lower or same level from the stack
@@ -616,14 +629,18 @@
                         {
                             "content": separator.join(current_content),
                             "metadata": current_metadata.copy(),
                         }
                     )
                     current_content.clear()
 
+            # Code block ends
+            if in_code_block and stripped_line == "```":
+                in_code_block = False
+
             current_metadata = initial_metadata.copy()
         if current_content:
             lines_with_metadata.append(
                 {
                     "content": separator.join(current_content),
                     "metadata": current_metadata,
                 }
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/rag/text_splitter/token_splitter.py` & `dbgpt-0.5.6rc0/dbgpt/rag/text_splitter/token_splitter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/cache/llm_cache.py` & `dbgpt-0.5.6rc0/dbgpt/storage/cache/llm_cache.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/cache/manager.py` & `dbgpt-0.5.6rc0/dbgpt/storage/cache/manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/cache/operators.py` & `dbgpt-0.5.6rc0/dbgpt/storage/cache/operators.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/base.py` & `dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/cache/storage/disk/disk_storage.py` & `dbgpt-0.5.6rc0/dbgpt/storage/cache/storage/disk/disk_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/chat_history/chat_history_db.py` & `dbgpt-0.5.6rc0/dbgpt/storage/chat_history/chat_history_db.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/chat_history/storage_adapter.py` & `dbgpt-0.5.6rc0/dbgpt/storage/chat_history/storage_adapter.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/metadata/_base_dao.py` & `dbgpt-0.5.6rc0/dbgpt/storage/metadata/_base_dao.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_factory.py` & `dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_factory.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_manager.py` & `dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_manager.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/metadata/db_storage.py` & `dbgpt-0.5.6rc0/dbgpt/storage/metadata/db_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/schema.py` & `dbgpt-0.5.6rc0/dbgpt/storage/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     MSSQL = DbInfo("mssql")
     Postgresql = DbInfo("postgresql")
     Clickhouse = DbInfo("clickhouse")
     StarRocks = DbInfo("starrocks")
     Spark = DbInfo("spark", True)
     Doris = DbInfo("doris")
     Hive = DbInfo("hive")
+    TuGraph = DbInfo("tugraph")
 
     def value(self) -> str:
         """Return the name of the database type."""
         return self._value_.name
 
     def is_file_db(self) -> bool:
         """Return whether the database is a file database."""
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/base.py` & `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/chroma_store.py` & `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/connector.py` & `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Connector for vector store."""
 
+import copy
 import os
 from typing import Any, Dict, List, Optional, Type, cast
 
-from dbgpt.core import Chunk
+from dbgpt.core import Chunk, Embeddings
 from dbgpt.core.awel.flow import (
     FunctionDynamicOptions,
     OptionValue,
     Parameter,
     ResourceCategory,
     register_resource,
 )
-from dbgpt.storage import vector_store
 from dbgpt.storage.vector_store.base import VectorStoreBase, VectorStoreConfig
 from dbgpt.storage.vector_store.filters import MetadataFilters
 from dbgpt.util.i18n_utils import _
 
 connector: Dict[str, Type] = {}
 
 
 def _load_vector_options() -> List[OptionValue]:
+    from dbgpt.storage import vector_store
+
     return [
         OptionValue(label=cls, name=cls, value=cls)
         for cls in vector_store.__all__
         if issubclass(getattr(vector_store, cls), VectorStoreBase)
     ]
 
 
@@ -84,14 +86,18 @@
 
         if self._match(vector_store_type):
             self.connector_class = connector[vector_store_type]
         else:
             raise Exception(f"Vector Store Type Not support. {0}", vector_store_type)
 
         print(self.connector_class)
+        self._vector_store_type = vector_store_type
+        self._embeddings = (
+            vector_store_config.embedding_fn if vector_store_config else None
+        )
         self.client = self.connector_class(vector_store_config)
 
     @classmethod
     def from_default(
         cls,
         vector_store_type: Optional[str] = None,
         embedding_fn: Optional[Any] = None,
@@ -191,15 +197,35 @@
         """Delete vector by ids.
 
         Args:
             - ids: vector ids
         """
         return self.client.delete_by_ids(ids=ids)
 
+    @property
+    def current_embeddings(self) -> Optional[Embeddings]:
+        """Return the current embeddings."""
+        return self._embeddings
+
+    def new_connector(self, name: str, **kwargs) -> "VectorStoreConnector":
+        """Create a new connector.
+
+        New connector based on the current connector.
+        """
+        config = copy.copy(self.vector_store_config)
+        for k, v in kwargs.items():
+            if v is not None:
+                setattr(config, k, v)
+        config.name = name
+
+        return self.__class__(self._vector_store_type, config)
+
     def _match(self, vector_store_type) -> bool:
         return bool(connector.get(vector_store_type))
 
     def _register(self):
+        from dbgpt.storage import vector_store
+
         for cls in vector_store.__all__:
             if issubclass(getattr(vector_store, cls), VectorStoreBase):
                 _k, _v = cls, getattr(vector_store, cls)
                 connector.update({_k: _v})
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/filters.py` & `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/filters.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/milvus_store.py` & `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/milvus_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,16 +350,15 @@
                 insert_dict.setdefault("props_field", []).append(d)
         # Convert dict to list of lists for insertion
         insert_list = [insert_dict[x] for x in self.fields]
         # Insert into the collection.
         res = self.col.insert(
             insert_list, partition_name=partition_name, timeout=timeout
         )
-        # make sure data is searchable.
-        self.col.flush()
+
         return res.primary_keys
 
     def load_document(self, chunks: List[Chunk]) -> List[str]:
         """Load document in vector database."""
         batch_size = 500
         batched_list = [
             chunks[i : i + batch_size] for i in range(0, len(chunks), batch_size)
@@ -446,15 +445,15 @@
 
         if score_threshold is not None:
             docs_and_scores = [
                 Chunk(
                     metadata=doc.metadata,
                     content=doc.content,
                     score=score,
-                    chunk_id=id,
+                    chunk_id=str(id),
                 )
                 for doc, score, id in docs_and_scores
                 if score >= score_threshold
             ]
             if len(docs_and_scores) == 0:
                 logger.warning(
                     "No relevant docs were retrieved using the relevance score"
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/pgvector_store.py` & `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/pgvector_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/storage/vector_store/weaviate_store.py` & `dbgpt-0.5.6rc0/dbgpt/storage/vector_store/weaviate_store.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/_db_migration_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/_db_migration_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/api_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/api_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py` & `dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py` & `dbgpt-0.5.6rc0/dbgpt/util/benchmarks/llm/llm_benchmarks.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/chat_util.py` & `dbgpt-0.5.6rc0/dbgpt/util/chat_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/code_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/code_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,34 +66,36 @@
 
 # TODO: In the future move, to better support https://spec.commonmark.org/0.30/#fenced-code-blocks
 #       perhaps by using a full Markdown parser.
 def extract_code(
     text: Union[str, List],
     pattern: str = CODE_BLOCK_PATTERN,
     detect_single_line_code: bool = False,
+    default_lang: str = "python",
 ) -> List[Tuple[str, str]]:
     """Extract code from a text.
 
     Args:
         text (str or List): The content to extract code from. The content can be
             a string or a list, as returned by standard GPT or multimodal GPT.
         pattern (str, optional): The regular expression pattern for finding the
             code block. Defaults to CODE_BLOCK_PATTERN.
         detect_single_line_code (bool, optional): Enable the new feature for
             extracting single line code. Defaults to False.
+        default_lang (str, optional): The default language to use when the language
 
     Returns:
         list: A list of tuples, each containing the language and the code.
           If there is no code block in the input text, the language would be "unknown".
           If there is code block but the language is not specified, the language would be "".
     """
     text = content_str(text)
     if not detect_single_line_code:
         match = re.findall(pattern, text, flags=re.DOTALL)
-        return match if match else [(UNKNOWN, text)]
+        return match if match else [(default_lang, text)]
 
     # Extract both multi-line and single-line code block, separated by the | operator
     # `([^`]+)`: Matches inline code.
     code_pattern = re.compile(CODE_BLOCK_PATTERN + r"|`([^`]+)`")
     code_blocks = code_pattern.findall(text)
 
     # Extract the individual code blocks and languages from the matched groups
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/command_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/command_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/config_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/config_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/console/console.py` & `dbgpt-0.5.6rc0/dbgpt/util/console/console.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/custom_data_structure.py` & `dbgpt-0.5.6rc0/dbgpt/util/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/base.py` & `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/cli.py` & `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/loader.py` & `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/loader.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/repo.py` & `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/repo.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/dbgpts/template.py` & `dbgpt-0.5.6rc0/dbgpt/util/dbgpts/template.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/error_types.py` & `dbgpt-0.5.6rc0/dbgpt/util/error_types.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/executor_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/executor_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/fastapi.py` & `dbgpt-0.5.6rc0/dbgpt/util/fastapi.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/formatting.py` & `dbgpt-0.5.6rc0/dbgpt/util/formatting.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/function_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/function_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/global_helper.py` & `dbgpt-0.5.6rc0/dbgpt/util/global_helper.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/i18n_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/i18n_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/json_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/json_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/model_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/model_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/module_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/module_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/net_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/net_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/network/_cli.py` & `dbgpt-0.5.6rc0/dbgpt/util/network/_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/openai_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/openai_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/pagination_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/pagination_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/parameter_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/parameter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/pd_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/pd_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/prompt_util.py` & `dbgpt-0.5.6rc0/dbgpt/util/prompt_util.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/retry.py` & `dbgpt-0.5.6rc0/dbgpt/util/retry.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/serialization/json_serialization.py` & `dbgpt-0.5.6rc0/dbgpt/util/serialization/json_serialization.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/similarity_util.py` & `dbgpt-0.5.6rc0/dbgpt/util/similarity_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,57 @@
 """Utility functions for calculating similarity."""
-from typing import TYPE_CHECKING, Any, Sequence
+from typing import TYPE_CHECKING, Any, List, Sequence
 
 if TYPE_CHECKING:
     from dbgpt.core.interface.embeddings import Embeddings
 
 
+def cosine_similarity(embedding1: List[float], embedding2: List[float]) -> float:
+    """Calculate the cosine similarity between two vectors.
+
+    Args:
+        embedding1(List[float]): The first vector.
+        embedding2(List[float]): The second vector.
+
+    Returns:
+        float: The cosine similarity.
+    """
+    try:
+        import numpy as np
+    except ImportError:
+        raise ImportError("numpy is required for SimilarityMetric")
+    dot_product = np.dot(embedding1, embedding2)
+    norm1 = np.linalg.norm(embedding1)
+    norm2 = np.linalg.norm(embedding2)
+    similarity = dot_product / (norm1 * norm2)
+    return similarity
+
+
+def sigmoid_function(x: float) -> float:
+    """Calculate the sigmoid function.
+
+    The sigmoid function is defined as:
+    .. math::
+        f(x) = \\frac{1}{1 + e^{-x}}
+
+    It is used to map the input to a value between 0 and 1.
+
+    Args:
+        x(float): The input to the sigmoid function.
+
+    Returns:
+        float: The output of the sigmoid function.
+    """
+    try:
+        import numpy as np
+    except ImportError:
+        raise ImportError("numpy is required for sigmoid_function")
+    return 1 / (1 + np.exp(-x))
+
+
 def calculate_cosine_similarity(
     embeddings: "Embeddings", prediction: str, contexts: Sequence[str]
 ) -> Any:
     """Calculate the cosine similarity between a prediction and a list of contexts.
 
     Args:
         embeddings(Embeddings): The embeddings to use.
```

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/singleton.py` & `dbgpt-0.5.6rc0/dbgpt/util/singleton.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/speech/base.py` & `dbgpt-0.5.6rc0/dbgpt/util/speech/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/speech/brian.py` & `dbgpt-0.5.6rc0/dbgpt/util/speech/brian.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/speech/eleven_labs.py` & `dbgpt-0.5.6rc0/dbgpt/util/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/speech/macos_tts.py` & `dbgpt-0.5.6rc0/dbgpt/util/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/speech/say.py` & `dbgpt-0.5.6rc0/dbgpt/util/speech/say.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/splitter_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/splitter_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/string_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/system_utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/system_utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/tracer/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/util/tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/tracer/base.py` & `dbgpt-0.5.6rc0/dbgpt/util/tracer/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/tracer/span_storage.py` & `dbgpt-0.5.6rc0/dbgpt/util/tracer/span_storage.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_cli.py` & `dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_cli.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_impl.py` & `dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_impl.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/tracer/tracer_middleware.py` & `dbgpt-0.5.6rc0/dbgpt/util/tracer/tracer_middleware.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/util/utils.py` & `dbgpt-0.5.6rc0/dbgpt/util/utils.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/vis/__init__.py` & `dbgpt-0.5.6rc0/dbgpt/vis/__init__.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/vis/base.py` & `dbgpt-0.5.6rc0/dbgpt/vis/base.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/vis/client.py` & `dbgpt-0.5.6rc0/dbgpt/vis/client.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_chart.py` & `dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_chart.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt/vis/tags/vis_dashboard.py` & `dbgpt-0.5.6rc0/dbgpt/vis/tags/vis_dashboard.py`

 * *Files identical despite different names*

### Comparing `dbgpt-0.5.5rc0/dbgpt.egg-info/PKG-INFO` & `dbgpt-0.5.6rc0/dbgpt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbgpt
-Version: 0.5.5rc0
+Version: 0.5.6rc0
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/eosphoros-ai/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -12,137 +12,144 @@
 Requires-Dist: aiohttp==3.8.4
 Requires-Dist: chardet==5.1.0
 Requires-Dist: importlib-resources==5.12.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: cachetools
 Requires-Dist: pydantic>=2.6.0
 Requires-Dist: typeguard
+Requires-Dist: snowflake-id
 Provides-Extra: core
-Requires-Dist: chardet==5.1.0; extra == "core"
-Requires-Dist: importlib-resources==5.12.0; extra == "core"
 Requires-Dist: cachetools; extra == "core"
-Requires-Dist: typeguard; extra == "core"
-Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: importlib-resources==5.12.0; extra == "core"
 Requires-Dist: python-dotenv==1.0.0; extra == "core"
+Requires-Dist: aiohttp==3.8.4; extra == "core"
+Requires-Dist: snowflake-id; extra == "core"
+Requires-Dist: chardet==5.1.0; extra == "core"
+Requires-Dist: typeguard; extra == "core"
 Requires-Dist: pydantic>=2.6.0; extra == "core"
 Provides-Extra: client
-Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: cachetools; extra == "client"
+Requires-Dist: fastapi>=0.100.0; extra == "client"
 Requires-Dist: httpx; extra == "client"
 Requires-Dist: importlib-resources==5.12.0; extra == "client"
-Requires-Dist: fastapi>=0.100.0; extra == "client"
-Requires-Dist: cachetools; extra == "client"
-Requires-Dist: typeguard; extra == "client"
-Requires-Dist: aiohttp==3.8.4; extra == "client"
 Requires-Dist: python-dotenv==1.0.0; extra == "client"
+Requires-Dist: aiohttp==3.8.4; extra == "client"
+Requires-Dist: snowflake-id; extra == "client"
+Requires-Dist: chardet==5.1.0; extra == "client"
+Requires-Dist: typeguard; extra == "client"
 Requires-Dist: pydantic>=2.6.0; extra == "client"
 Provides-Extra: cli
-Requires-Dist: click; extra == "cli"
-Requires-Dist: chardet==5.1.0; extra == "cli"
-Requires-Dist: httpx; extra == "cli"
+Requires-Dist: cachetools; extra == "cli"
+Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: tomlkit; extra == "cli"
+Requires-Dist: httpx; extra == "cli"
 Requires-Dist: importlib-resources==5.12.0; extra == "cli"
-Requires-Dist: fastapi>=0.100.0; extra == "cli"
+Requires-Dist: python-dotenv==1.0.0; extra == "cli"
 Requires-Dist: prettytable; extra == "cli"
-Requires-Dist: cachetools; extra == "cli"
-Requires-Dist: typeguard; extra == "cli"
-Requires-Dist: rich; extra == "cli"
-Requires-Dist: psutil==5.9.4; extra == "cli"
 Requires-Dist: aiohttp==3.8.4; extra == "cli"
+Requires-Dist: snowflake-id; extra == "cli"
 Requires-Dist: colorama==0.4.6; extra == "cli"
-Requires-Dist: python-dotenv==1.0.0; extra == "cli"
+Requires-Dist: rich; extra == "cli"
+Requires-Dist: click; extra == "cli"
+Requires-Dist: chardet==5.1.0; extra == "cli"
+Requires-Dist: typeguard; extra == "cli"
 Requires-Dist: pydantic>=2.6.0; extra == "cli"
 Provides-Extra: agent
-Requires-Dist: click; extra == "agent"
-Requires-Dist: chardet==5.1.0; extra == "agent"
-Requires-Dist: httpx; extra == "agent"
+Requires-Dist: pandas==2.0.3; extra == "agent"
+Requires-Dist: cachetools; extra == "agent"
+Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: psutil==5.9.4; extra == "agent"
 Requires-Dist: tomlkit; extra == "agent"
 Requires-Dist: termcolor; extra == "agent"
+Requires-Dist: httpx; extra == "agent"
 Requires-Dist: importlib-resources==5.12.0; extra == "agent"
-Requires-Dist: fastapi>=0.100.0; extra == "agent"
+Requires-Dist: python-dotenv==1.0.0; extra == "agent"
 Requires-Dist: prettytable; extra == "agent"
-Requires-Dist: cachetools; extra == "agent"
-Requires-Dist: typeguard; extra == "agent"
-Requires-Dist: pandas==2.0.3; extra == "agent"
-Requires-Dist: rich; extra == "agent"
-Requires-Dist: psutil==5.9.4; extra == "agent"
 Requires-Dist: aiohttp==3.8.4; extra == "agent"
+Requires-Dist: snowflake-id; extra == "agent"
 Requires-Dist: colorama==0.4.6; extra == "agent"
-Requires-Dist: python-dotenv==1.0.0; extra == "agent"
+Requires-Dist: rich; extra == "agent"
+Requires-Dist: click; extra == "agent"
+Requires-Dist: chardet==5.1.0; extra == "agent"
+Requires-Dist: typeguard; extra == "agent"
 Requires-Dist: pydantic>=2.6.0; extra == "agent"
 Provides-Extra: simple-framework
-Requires-Dist: click; extra == "simple-framework"
-Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: schedule; extra == "simple-framework"
+Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
 Requires-Dist: msgpack; extra == "simple-framework"
-Requires-Dist: uvicorn; extra == "simple-framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
-Requires-Dist: typeguard; extra == "simple-framework"
+Requires-Dist: termcolor; extra == "simple-framework"
 Requires-Dist: rich; extra == "simple-framework"
-Requires-Dist: duckdb-engine; extra == "simple-framework"
-Requires-Dist: colorama==0.4.6; extra == "simple-framework"
-Requires-Dist: pympler; extra == "simple-framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: shortuuid; extra == "simple-framework"
+Requires-Dist: typeguard; extra == "simple-framework"
 Requires-Dist: jinja2; extra == "simple-framework"
-Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
-Requires-Dist: schedule; extra == "simple-framework"
-Requires-Dist: chardet==5.1.0; extra == "simple-framework"
-Requires-Dist: httpx; extra == "simple-framework"
-Requires-Dist: tomlkit; extra == "simple-framework"
 Requires-Dist: cachetools; extra == "simple-framework"
-Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
 Requires-Dist: psutil==5.9.4; extra == "simple-framework"
-Requires-Dist: termcolor; extra == "simple-framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "simple-framework"
 Requires-Dist: prettytable; extra == "simple-framework"
-Requires-Dist: sqlparse==0.4.4; extra == "simple-framework"
+Requires-Dist: fschat; extra == "simple-framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "simple-framework"
+Requires-Dist: click; extra == "simple-framework"
+Requires-Dist: duckdb-engine; extra == "simple-framework"
 Requires-Dist: pandas==2.0.3; extra == "simple-framework"
-Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: fastapi>=0.100.0; extra == "simple-framework"
+Requires-Dist: pympler; extra == "simple-framework"
+Requires-Dist: tomlkit; extra == "simple-framework"
+Requires-Dist: uvicorn; extra == "simple-framework"
+Requires-Dist: httpx; extra == "simple-framework"
 Requires-Dist: python-dotenv==1.0.0; extra == "simple-framework"
+Requires-Dist: colorama==0.4.6; extra == "simple-framework"
+Requires-Dist: snowflake-id; extra == "simple-framework"
+Requires-Dist: chardet==5.1.0; extra == "simple-framework"
 Requires-Dist: duckdb; extra == "simple-framework"
-Requires-Dist: shortuuid; extra == "simple-framework"
+Requires-Dist: aiohttp==3.8.4; extra == "simple-framework"
+Requires-Dist: pydantic>=2.6.0; extra == "simple-framework"
 Provides-Extra: framework
-Requires-Dist: click; extra == "framework"
-Requires-Dist: fschat; extra == "framework"
+Requires-Dist: schedule; extra == "framework"
+Requires-Dist: sqlparse==0.4.4; extra == "framework"
+Requires-Dist: seaborn; extra == "framework"
 Requires-Dist: msgpack; extra == "framework"
-Requires-Dist: uvicorn; extra == "framework"
-Requires-Dist: importlib-resources==5.12.0; extra == "framework"
-Requires-Dist: typeguard; extra == "framework"
-Requires-Dist: rich; extra == "framework"
-Requires-Dist: duckdb-engine; extra == "framework"
-Requires-Dist: pymysql; extra == "framework"
-Requires-Dist: colorama==0.4.6; extra == "framework"
-Requires-Dist: pympler; extra == "framework"
+Requires-Dist: termcolor; extra == "framework"
 Requires-Dist: alembic==1.12.0; extra == "framework"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
-Requires-Dist: coloredlogs; extra == "framework"
-Requires-Dist: aiofiles; extra == "framework"
-Requires-Dist: seaborn; extra == "framework"
-Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: rich; extra == "framework"
+Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: typeguard; extra == "framework"
 Requires-Dist: jinja2; extra == "framework"
-Requires-Dist: fastapi>=0.100.0; extra == "framework"
-Requires-Dist: GitPython; extra == "framework"
-Requires-Dist: schedule; extra == "framework"
-Requires-Dist: chardet==5.1.0; extra == "framework"
-Requires-Dist: httpx; extra == "framework"
-Requires-Dist: tomlkit; extra == "framework"
-Requires-Dist: gTTS==2.3.1; extra == "framework"
+Requires-Dist: pymysql; extra == "framework"
 Requires-Dist: cachetools; extra == "framework"
-Requires-Dist: auto-gpt-plugin-template; extra == "framework"
-Requires-Dist: transformers>=4.34.0; extra == "framework"
-Requires-Dist: pydantic>=2.6.0; extra == "framework"
 Requires-Dist: psutil==5.9.4; extra == "framework"
-Requires-Dist: termcolor; extra == "framework"
+Requires-Dist: importlib-resources==5.12.0; extra == "framework"
 Requires-Dist: prettytable; extra == "framework"
-Requires-Dist: sqlparse==0.4.4; extra == "framework"
-Requires-Dist: pandas==2.0.3; extra == "framework"
+Requires-Dist: fschat; extra == "framework"
 Requires-Dist: graphviz; extra == "framework"
-Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "framework"
+Requires-Dist: click; extra == "framework"
+Requires-Dist: duckdb-engine; extra == "framework"
+Requires-Dist: pandas==2.0.3; extra == "framework"
+Requires-Dist: fastapi>=0.100.0; extra == "framework"
 Requires-Dist: jsonschema; extra == "framework"
+Requires-Dist: pympler; extra == "framework"
+Requires-Dist: tomlkit; extra == "framework"
+Requires-Dist: uvicorn; extra == "framework"
+Requires-Dist: auto-gpt-plugin-template; extra == "framework"
+Requires-Dist: httpx; extra == "framework"
+Requires-Dist: coloredlogs; extra == "framework"
 Requires-Dist: python-dotenv==1.0.0; extra == "framework"
-Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: colorama==0.4.6; extra == "framework"
+Requires-Dist: snowflake-id; extra == "framework"
+Requires-Dist: transformers>=4.34.0; extra == "framework"
+Requires-Dist: aiofiles; extra == "framework"
+Requires-Dist: GitPython; extra == "framework"
+Requires-Dist: chardet==5.1.0; extra == "framework"
+Requires-Dist: gTTS==2.3.1; extra == "framework"
 Requires-Dist: duckdb; extra == "framework"
-Requires-Dist: shortuuid; extra == "framework"
+Requires-Dist: xlrd==2.0.1; extra == "framework"
+Requires-Dist: aiohttp==3.8.4; extra == "framework"
+Requires-Dist: openpyxl==3.1.2; extra == "framework"
+Requires-Dist: pydantic>=2.6.0; extra == "framework"
 Provides-Extra: torch
 Requires-Dist: torchvision==0.17.1; extra == "torch"
 Requires-Dist: torch==2.2.1; extra == "torch"
 Requires-Dist: torchaudio==2.2.1; extra == "torch"
 Provides-Extra: torch-cpu
 Requires-Dist: torchvision==0.17.1; extra == "torch-cpu"
 Requires-Dist: torch==2.2.1; extra == "torch-cpu"
@@ -153,253 +160,262 @@
 Requires-Dist: torchaudio==2.2.1; extra == "torch-cuda"
 Provides-Extra: llama-cpp
 Requires-Dist: llama-cpp-python; extra == "llama-cpp"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes; extra == "bitsandbytes"
 Provides-Extra: quantization
 Requires-Dist: cpm_kernels; extra == "quantization"
+Requires-Dist: bitsandbytes; extra == "quantization"
 Provides-Extra: vstore
 Requires-Dist: chromadb>=0.4.22; extra == "vstore"
 Provides-Extra: vstore-weaviate
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
 Requires-Dist: weaviate-client; extra == "vstore-weaviate"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-weaviate"
 Provides-Extra: vstore-milvus
 Requires-Dist: pymilvus; extra == "vstore-milvus"
 Requires-Dist: chromadb>=0.4.22; extra == "vstore-milvus"
 Provides-Extra: vstore-all
 Requires-Dist: pymilvus; extra == "vstore-all"
-Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Requires-Dist: weaviate-client; extra == "vstore-all"
+Requires-Dist: chromadb>=0.4.22; extra == "vstore-all"
 Provides-Extra: datasource
 Requires-Dist: pymysql; extra == "datasource"
 Provides-Extra: datasource-all
+Requires-Dist: pymysql; extra == "datasource-all"
+Requires-Dist: thrift; extra == "datasource-all"
 Requires-Dist: pymssql; extra == "datasource-all"
-Requires-Dist: pyspark; extra == "datasource-all"
 Requires-Dist: clickhouse-connect; extra == "datasource-all"
 Requires-Dist: thrift_sasl; extra == "datasource-all"
-Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "datasource-all"
+Requires-Dist: neo4j; extra == "datasource-all"
 Requires-Dist: pyhive; extra == "datasource-all"
-Requires-Dist: pymysql; extra == "datasource-all"
-Requires-Dist: thrift; extra == "datasource-all"
 Requires-Dist: psycopg2; extra == "datasource-all"
+Requires-Dist: mysqlclient==2.1.0; extra == "datasource-all"
+Requires-Dist: pyspark; extra == "datasource-all"
 Provides-Extra: rag
-Requires-Dist: pypdf; extra == "rag"
-Requires-Dist: python-pptx; extra == "rag"
-Requires-Dist: python-docx; extra == "rag"
-Requires-Dist: spacy>=3.7; extra == "rag"
+Requires-Dist: bs4; extra == "rag"
 Requires-Dist: markdown; extra == "rag"
-Requires-Dist: python-multipart; extra == "rag"
+Requires-Dist: spacy>=3.7; extra == "rag"
 Requires-Dist: sentence-transformers; extra == "rag"
-Requires-Dist: langchain>=0.0.286; extra == "rag"
-Requires-Dist: bs4; extra == "rag"
+Requires-Dist: python-pptx; extra == "rag"
+Requires-Dist: python-docx; extra == "rag"
+Requires-Dist: pypdf; extra == "rag"
 Requires-Dist: chromadb>=0.4.22; extra == "rag"
+Requires-Dist: langchain>=0.0.286; extra == "rag"
+Requires-Dist: python-multipart; extra == "rag"
 Provides-Extra: openai
-Requires-Dist: click; extra == "openai"
-Requires-Dist: fschat; extra == "openai"
-Requires-Dist: msgpack; extra == "openai"
-Requires-Dist: uvicorn; extra == "openai"
-Requires-Dist: importlib-resources==5.12.0; extra == "openai"
-Requires-Dist: typeguard; extra == "openai"
-Requires-Dist: rich; extra == "openai"
-Requires-Dist: duckdb-engine; extra == "openai"
-Requires-Dist: spacy>=3.7; extra == "openai"
-Requires-Dist: pymysql; extra == "openai"
+Requires-Dist: schedule; extra == "openai"
+Requires-Dist: sqlparse==0.4.4; extra == "openai"
+Requires-Dist: seaborn; extra == "openai"
 Requires-Dist: markdown; extra == "openai"
-Requires-Dist: colorama==0.4.6; extra == "openai"
-Requires-Dist: langchain>=0.0.286; extra == "openai"
-Requires-Dist: pympler; extra == "openai"
+Requires-Dist: msgpack; extra == "openai"
+Requires-Dist: termcolor; extra == "openai"
+Requires-Dist: sentence-transformers; extra == "openai"
+Requires-Dist: tiktoken; extra == "openai"
 Requires-Dist: alembic==1.12.0; extra == "openai"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
-Requires-Dist: coloredlogs; extra == "openai"
-Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: rich; extra == "openai"
+Requires-Dist: shortuuid; extra == "openai"
 Requires-Dist: pypdf; extra == "openai"
-Requires-Dist: seaborn; extra == "openai"
-Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: chromadb>=0.4.22; extra == "openai"
+Requires-Dist: typeguard; extra == "openai"
 Requires-Dist: jinja2; extra == "openai"
-Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: python-multipart; extra == "openai"
-Requires-Dist: bs4; extra == "openai"
-Requires-Dist: GitPython; extra == "openai"
-Requires-Dist: schedule; extra == "openai"
-Requires-Dist: chromadb>=0.4.22; extra == "openai"
-Requires-Dist: chardet==5.1.0; extra == "openai"
-Requires-Dist: httpx; extra == "openai"
-Requires-Dist: tomlkit; extra == "openai"
-Requires-Dist: gTTS==2.3.1; extra == "openai"
-Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: pymysql; extra == "openai"
 Requires-Dist: cachetools; extra == "openai"
-Requires-Dist: auto-gpt-plugin-template; extra == "openai"
-Requires-Dist: transformers>=4.34.0; extra == "openai"
-Requires-Dist: pydantic>=2.6.0; extra == "openai"
 Requires-Dist: psutil==5.9.4; extra == "openai"
-Requires-Dist: sentence-transformers; extra == "openai"
-Requires-Dist: python-pptx; extra == "openai"
-Requires-Dist: termcolor; extra == "openai"
-Requires-Dist: openai; extra == "openai"
+Requires-Dist: importlib-resources==5.12.0; extra == "openai"
 Requires-Dist: prettytable; extra == "openai"
-Requires-Dist: sqlparse==0.4.4; extra == "openai"
-Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: fschat; extra == "openai"
 Requires-Dist: graphviz; extra == "openai"
-Requires-Dist: tiktoken; extra == "openai"
-Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "openai"
+Requires-Dist: click; extra == "openai"
+Requires-Dist: duckdb-engine; extra == "openai"
+Requires-Dist: pandas==2.0.3; extra == "openai"
+Requires-Dist: fastapi>=0.100.0; extra == "openai"
 Requires-Dist: jsonschema; extra == "openai"
+Requires-Dist: spacy>=3.7; extra == "openai"
+Requires-Dist: pympler; extra == "openai"
+Requires-Dist: tomlkit; extra == "openai"
+Requires-Dist: uvicorn; extra == "openai"
+Requires-Dist: auto-gpt-plugin-template; extra == "openai"
+Requires-Dist: httpx; extra == "openai"
+Requires-Dist: coloredlogs; extra == "openai"
 Requires-Dist: python-dotenv==1.0.0; extra == "openai"
-Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: colorama==0.4.6; extra == "openai"
+Requires-Dist: snowflake-id; extra == "openai"
+Requires-Dist: transformers>=4.34.0; extra == "openai"
+Requires-Dist: aiofiles; extra == "openai"
+Requires-Dist: python-docx; extra == "openai"
+Requires-Dist: GitPython; extra == "openai"
+Requires-Dist: chardet==5.1.0; extra == "openai"
+Requires-Dist: langchain>=0.0.286; extra == "openai"
+Requires-Dist: openai; extra == "openai"
+Requires-Dist: gTTS==2.3.1; extra == "openai"
+Requires-Dist: bs4; extra == "openai"
 Requires-Dist: duckdb; extra == "openai"
-Requires-Dist: shortuuid; extra == "openai"
+Requires-Dist: python-pptx; extra == "openai"
+Requires-Dist: xlrd==2.0.1; extra == "openai"
+Requires-Dist: aiohttp==3.8.4; extra == "openai"
+Requires-Dist: openpyxl==3.1.2; extra == "openai"
+Requires-Dist: pydantic>=2.6.0; extra == "openai"
 Provides-Extra: gpt4all
 Requires-Dist: gpt4all; extra == "gpt4all"
 Provides-Extra: vllm
 Requires-Dist: vllm; extra == "vllm"
 Provides-Extra: cache
 Requires-Dist: rocksdict; extra == "cache"
 Provides-Extra: default
-Requires-Dist: click; extra == "default"
-Requires-Dist: fschat; extra == "default"
-Requires-Dist: torchaudio==2.2.1; extra == "default"
-Requires-Dist: msgpack; extra == "default"
-Requires-Dist: uvicorn; extra == "default"
-Requires-Dist: importlib-resources==5.12.0; extra == "default"
-Requires-Dist: sentencepiece; extra == "default"
-Requires-Dist: typeguard; extra == "default"
-Requires-Dist: rich; extra == "default"
-Requires-Dist: duckdb-engine; extra == "default"
-Requires-Dist: spacy>=3.7; extra == "default"
-Requires-Dist: pymysql; extra == "default"
+Requires-Dist: schedule; extra == "default"
+Requires-Dist: sqlparse==0.4.4; extra == "default"
+Requires-Dist: seaborn; extra == "default"
 Requires-Dist: markdown; extra == "default"
-Requires-Dist: colorama==0.4.6; extra == "default"
-Requires-Dist: rocksdict; extra == "default"
-Requires-Dist: langchain>=0.0.286; extra == "default"
-Requires-Dist: pympler; extra == "default"
+Requires-Dist: msgpack; extra == "default"
+Requires-Dist: termcolor; extra == "default"
+Requires-Dist: sentence-transformers; extra == "default"
 Requires-Dist: alembic==1.12.0; extra == "default"
-Requires-Dist: torch==2.2.1; extra == "default"
-Requires-Dist: chardet; extra == "default"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
-Requires-Dist: coloredlogs; extra == "default"
-Requires-Dist: aiofiles; extra == "default"
+Requires-Dist: rich; extra == "default"
+Requires-Dist: ollama; extra == "default"
+Requires-Dist: shortuuid; extra == "default"
 Requires-Dist: pypdf; extra == "default"
-Requires-Dist: seaborn; extra == "default"
-Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: chromadb>=0.4.22; extra == "default"
+Requires-Dist: cpm_kernels; extra == "default"
+Requires-Dist: typeguard; extra == "default"
 Requires-Dist: jinja2; extra == "default"
-Requires-Dist: fastapi>=0.100.0; extra == "default"
 Requires-Dist: python-multipart; extra == "default"
-Requires-Dist: bs4; extra == "default"
-Requires-Dist: tokenizers>=0.14; extra == "default"
-Requires-Dist: schedule; extra == "default"
-Requires-Dist: GitPython; extra == "default"
-Requires-Dist: chromadb>=0.4.22; extra == "default"
-Requires-Dist: chardet==5.1.0; extra == "default"
-Requires-Dist: httpx; extra == "default"
-Requires-Dist: tomlkit; extra == "default"
-Requires-Dist: gTTS==2.3.1; extra == "default"
-Requires-Dist: python-docx; extra == "default"
+Requires-Dist: torchvision==0.17.1; extra == "default"
+Requires-Dist: pymysql; extra == "default"
 Requires-Dist: cachetools; extra == "default"
-Requires-Dist: auto-gpt-plugin-template; extra == "default"
-Requires-Dist: dashscope; extra == "default"
-Requires-Dist: pydantic>=2.6.0; extra == "default"
 Requires-Dist: psutil==5.9.4; extra == "default"
-Requires-Dist: transformers>=4.34.0; extra == "default"
-Requires-Dist: sentence-transformers; extra == "default"
-Requires-Dist: zhipuai; extra == "default"
-Requires-Dist: python-pptx; extra == "default"
-Requires-Dist: cpm_kernels; extra == "default"
-Requires-Dist: termcolor; extra == "default"
+Requires-Dist: torch==2.2.1; extra == "default"
+Requires-Dist: torchaudio==2.2.1; extra == "default"
+Requires-Dist: dashscope; extra == "default"
+Requires-Dist: importlib-resources==5.12.0; extra == "default"
 Requires-Dist: prettytable; extra == "default"
-Requires-Dist: sqlparse==0.4.4; extra == "default"
 Requires-Dist: accelerate>=0.20.3; extra == "default"
-Requires-Dist: pandas==2.0.3; extra == "default"
+Requires-Dist: fschat; extra == "default"
+Requires-Dist: zhipuai; extra == "default"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "default"
 Requires-Dist: graphviz; extra == "default"
-Requires-Dist: torchvision==0.17.1; extra == "default"
-Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: rocksdict; extra == "default"
+Requires-Dist: click; extra == "default"
+Requires-Dist: duckdb-engine; extra == "default"
+Requires-Dist: pandas==2.0.3; extra == "default"
+Requires-Dist: fastapi>=0.100.0; extra == "default"
 Requires-Dist: jsonschema; extra == "default"
+Requires-Dist: spacy>=3.7; extra == "default"
+Requires-Dist: pympler; extra == "default"
+Requires-Dist: tomlkit; extra == "default"
+Requires-Dist: uvicorn; extra == "default"
+Requires-Dist: auto-gpt-plugin-template; extra == "default"
+Requires-Dist: httpx; extra == "default"
+Requires-Dist: coloredlogs; extra == "default"
+Requires-Dist: tokenizers>=0.14; extra == "default"
 Requires-Dist: python-dotenv==1.0.0; extra == "default"
-Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: snowflake-id; extra == "default"
+Requires-Dist: colorama==0.4.6; extra == "default"
+Requires-Dist: transformers>=4.34.0; extra == "default"
+Requires-Dist: sentencepiece; extra == "default"
+Requires-Dist: aiofiles; extra == "default"
+Requires-Dist: python-docx; extra == "default"
+Requires-Dist: GitPython; extra == "default"
+Requires-Dist: chardet==5.1.0; extra == "default"
+Requires-Dist: langchain>=0.0.286; extra == "default"
+Requires-Dist: gTTS==2.3.1; extra == "default"
+Requires-Dist: bs4; extra == "default"
 Requires-Dist: duckdb; extra == "default"
-Requires-Dist: shortuuid; extra == "default"
+Requires-Dist: python-pptx; extra == "default"
+Requires-Dist: chardet; extra == "default"
+Requires-Dist: xlrd==2.0.1; extra == "default"
+Requires-Dist: aiohttp==3.8.4; extra == "default"
+Requires-Dist: bitsandbytes; extra == "default"
+Requires-Dist: openpyxl==3.1.2; extra == "default"
+Requires-Dist: pydantic>=2.6.0; extra == "default"
 Provides-Extra: all
-Requires-Dist: click; extra == "all"
-Requires-Dist: fschat; extra == "all"
+Requires-Dist: sqlparse==0.4.4; extra == "all"
+Requires-Dist: markdown; extra == "all"
+Requires-Dist: sentence-transformers; extra == "all"
+Requires-Dist: msgpack; extra == "all"
+Requires-Dist: alembic==1.12.0; extra == "all"
+Requires-Dist: rich; extra == "all"
+Requires-Dist: pypdf; extra == "all"
+Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: python-multipart; extra == "all"
 Requires-Dist: importlib-resources==5.12.0; extra == "all"
-Requires-Dist: typeguard; extra == "all"
-Requires-Dist: thrift; extra == "all"
-Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
-Requires-Dist: gpt4all; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: prettytable; extra == "all"
+Requires-Dist: thrift_sasl; extra == "all"
+Requires-Dist: auto-gpt-plugin-template; extra == "all"
+Requires-Dist: sentencepiece; extra == "all"
 Requires-Dist: GitPython; extra == "all"
 Requires-Dist: gTTS==2.3.1; extra == "all"
 Requires-Dist: clickhouse-connect; extra == "all"
-Requires-Dist: dashscope; extra == "all"
-Requires-Dist: sentence-transformers; extra == "all"
-Requires-Dist: cpm_kernels; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: sqlparse==0.4.4; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: python-dotenv==1.0.0; extra == "all"
-Requires-Dist: duckdb; extra == "all"
+Requires-Dist: pydantic>=2.6.0; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: psutil==5.9.4; extra == "all"
+Requires-Dist: gpt4all; extra == "all"
+Requires-Dist: zhipuai; extra == "all"
+Requires-Dist: click; extra == "all"
+Requires-Dist: pandas==2.0.3; extra == "all"
+Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: vllm; extra == "all"
+Requires-Dist: httpx; extra == "all"
+Requires-Dist: colorama==0.4.6; extra == "all"
+Requires-Dist: snowflake-id; extra == "all"
+Requires-Dist: pyhive; extra == "all"
+Requires-Dist: chardet==5.1.0; extra == "all"
+Requires-Dist: weaviate-client; extra == "all"
+Requires-Dist: pyspark; extra == "all"
+Requires-Dist: termcolor; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
 Requires-Dist: shortuuid; extra == "all"
+Requires-Dist: cpm_kernels; extra == "all"
+Requires-Dist: neo4j; extra == "all"
+Requires-Dist: typeguard; extra == "all"
 Requires-Dist: torchaudio==2.2.1; extra == "all"
-Requires-Dist: duckdb-engine; extra == "all"
-Requires-Dist: markdown; extra == "all"
-Requires-Dist: pymysql; extra == "all"
+Requires-Dist: accelerate>=0.20.3; extra == "all"
 Requires-Dist: rocksdict; extra == "all"
-Requires-Dist: bitsandbytes; extra == "all"
-Requires-Dist: pypdf; extra == "all"
+Requires-Dist: spacy>=3.7; extra == "all"
+Requires-Dist: pympler; extra == "all"
+Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
+Requires-Dist: coloredlogs; extra == "all"
+Requires-Dist: tokenizers>=0.14; extra == "all"
+Requires-Dist: python-dotenv==1.0.0; extra == "all"
+Requires-Dist: duckdb; extra == "all"
+Requires-Dist: xlrd==2.0.1; extra == "all"
+Requires-Dist: aiohttp==3.8.4; extra == "all"
 Requires-Dist: openpyxl==3.1.2; extra == "all"
-Requires-Dist: bs4; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: tiktoken; extra == "all"
+Requires-Dist: ollama; extra == "all"
 Requires-Dist: chromadb>=0.4.22; extra == "all"
-Requires-Dist: pyspark; extra == "all"
-Requires-Dist: chardet==5.1.0; extra == "all"
-Requires-Dist: httpx; extra == "all"
-Requires-Dist: tomlkit; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: torchvision==0.17.1; extra == "all"
+Requires-Dist: pymysql; extra == "all"
 Requires-Dist: cachetools; extra == "all"
-Requires-Dist: transformers>=4.34.0; extra == "all"
-Requires-Dist: pymssql; extra == "all"
-Requires-Dist: termcolor; extra == "all"
-Requires-Dist: accelerate>=0.20.3; extra == "all"
-Requires-Dist: aiohttp==3.8.4; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: sentencepiece; extra == "all"
-Requires-Dist: spacy>=3.7; extra == "all"
-Requires-Dist: pympler; extra == "all"
-Requires-Dist: alembic==1.12.0; extra == "all"
-Requires-Dist: chardet; extra == "all"
-Requires-Dist: psycopg2; extra == "all"
+Requires-Dist: thrift; extra == "all"
+Requires-Dist: torch==2.2.1; extra == "all"
+Requires-Dist: dashscope; extra == "all"
+Requires-Dist: fschat; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: SQLAlchemy<2.0.29,>=2.0.25; extra == "all"
+Requires-Dist: duckdb-engine; extra == "all"
 Requires-Dist: fastapi>=0.100.0; extra == "all"
-Requires-Dist: schedule; extra == "all"
 Requires-Dist: python-docx; extra == "all"
-Requires-Dist: pyhive; extra == "all"
-Requires-Dist: pydantic>=2.6.0; extra == "all"
-Requires-Dist: python-pptx; extra == "all"
-Requires-Dist: zhipuai; extra == "all"
-Requires-Dist: pandas==2.0.3; extra == "all"
-Requires-Dist: torchvision==0.17.1; extra == "all"
-Requires-Dist: tiktoken; extra == "all"
-Requires-Dist: xlrd==2.0.1; extra == "all"
-Requires-Dist: msgpack; extra == "all"
-Requires-Dist: mysqlclient==2.1.0; extra == "all"
-Requires-Dist: rich; extra == "all"
+Requires-Dist: pymssql; extra == "all"
+Requires-Dist: llama-cpp-python; extra == "all"
+Requires-Dist: transformers>=4.34.0; extra == "all"
+Requires-Dist: aiofiles; extra == "all"
 Requires-Dist: pydoris<2.0.0,>=1.0.2; extra == "all"
-Requires-Dist: colorama==0.4.6; extra == "all"
 Requires-Dist: langchain>=0.0.286; extra == "all"
-Requires-Dist: torch==2.2.1; extra == "all"
-Requires-Dist: coloredlogs; extra == "all"
-Requires-Dist: aiofiles; extra == "all"
-Requires-Dist: llama-cpp-python; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: python-multipart; extra == "all"
-Requires-Dist: tokenizers>=0.14; extra == "all"
-Requires-Dist: vllm; extra == "all"
-Requires-Dist: auto-gpt-plugin-template; extra == "all"
-Requires-Dist: psutil==5.9.4; extra == "all"
-Requires-Dist: thrift_sasl; extra == "all"
-Requires-Dist: prettytable; extra == "all"
-Requires-Dist: weaviate-client; extra == "all"
-Requires-Dist: jsonschema; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: bs4; extra == "all"
+Requires-Dist: python-pptx; extra == "all"
+Requires-Dist: chardet; extra == "all"
+Requires-Dist: bitsandbytes; extra == "all"
+Requires-Dist: mysqlclient==2.1.0; extra == "all"
 
 # DB-GPT: Revolutionizing Database Interactions with Private LLM Technology
  
 <p align="left">
   <img src="./assets/LOGO.png" width="100%" />
 </p>
 
@@ -553,14 +569,19 @@
   We've also developed an automated fine-tuning lightweight framework centred on large language models (LLMs), Text2SQL datasets, LoRA/QLoRA/Pturning, and other fine-tuning methods. This framework simplifies Text-to-SQL fine-tuning, making it as straightforward as an assembly line process. [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub)
 
 - **SMMF(Service-oriented Multi-model Management Framework)**
 
   We offer extensive model support, including dozens of large language models (LLMs) from both open-source and API agents, such as LLaMA/LLaMA2, Baichuan, ChatGLM, Wenxin, Tongyi, Zhipu, and many more. 
 
   - News
+    - 🔥🔥🔥  [Qwen1.5-110B-Chat](https://huggingface.co/Qwen/Qwen1.5-110B-Chat)
+    - 🔥🔥🔥  [Qwen1.5-MoE-A2.7B-Chat](https://huggingface.co/Qwen/Qwen1.5-MoE-A2.7B-Chat)
+    - 🔥🔥🔥  [Meta-Llama-3-70B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-70B-Instruct)
+    - 🔥🔥🔥  [Meta-Llama-3-8B-Instruct](https://huggingface.co/meta-llama/Meta-Llama-3-8B-Instruct)
+    - 🔥🔥🔥  [CodeQwen1.5-7B-Chat](https://huggingface.co/Qwen/CodeQwen1.5-7B-Chat)
     - 🔥🔥🔥  [Qwen1.5-32B-Chat](https://huggingface.co/Qwen/Qwen1.5-32B-Chat)
     - 🔥🔥🔥  [Starling-LM-7B-beta](https://huggingface.co/Nexusflow/Starling-LM-7B-beta)
     - 🔥🔥🔥  [gemma-7b-it](https://huggingface.co/google/gemma-7b-it)
     - 🔥🔥🔥  [gemma-2b-it](https://huggingface.co/google/gemma-2b-it)
     - 🔥🔥🔥  [SOLAR-10.7B](https://huggingface.co/upstage/SOLAR-10.7B-Instruct-v1.0)
     - 🔥🔥🔥  [Mixtral-8x7B](https://huggingface.co/mistralai/Mixtral-8x7B-Instruct-v0.1)
     - 🔥🔥🔥  [Qwen-72B-Chat](https://huggingface.co/Qwen/Qwen-72B-Chat)
```

### Comparing `dbgpt-0.5.5rc0/dbgpt.egg-info/SOURCES.txt` & `dbgpt-0.5.6rc0/dbgpt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,55 +12,60 @@
 dbgpt.egg-info/requires.txt
 dbgpt.egg-info/top_level.txt
 dbgpt/_private/__init__.py
 dbgpt/_private/config.py
 dbgpt/_private/llm_metadata.py
 dbgpt/_private/pydantic.py
 dbgpt/agent/__init__.py
-dbgpt/agent/actions/__init__.py
-dbgpt/agent/actions/action.py
-dbgpt/agent/actions/blank_action.py
-dbgpt/agent/actions/chart_action.py
-dbgpt/agent/actions/code_action.py
-dbgpt/agent/actions/dashboard_action.py
-dbgpt/agent/actions/indicator_action.py
-dbgpt/agent/actions/plugin_action.py
 dbgpt/agent/core/__init__.py
 dbgpt/agent/core/agent.py
 dbgpt/agent/core/agent_manage.py
 dbgpt/agent/core/base_agent.py
 dbgpt/agent/core/base_team.py
 dbgpt/agent/core/role.py
 dbgpt/agent/core/schema.py
 dbgpt/agent/core/user_proxy_agent.py
-dbgpt/agent/core/llm/__init__.py
-dbgpt/agent/core/llm/llm.py
-dbgpt/agent/core/llm/llm_client.py
-dbgpt/agent/core/llm/strategy/__init__.py
-dbgpt/agent/core/llm/strategy/priority.py
+dbgpt/agent/core/action/__init__.py
+dbgpt/agent/core/action/base.py
+dbgpt/agent/core/action/blank_action.py
+dbgpt/agent/core/memory/__init__.py
+dbgpt/agent/core/memory/agent_memory.py
+dbgpt/agent/core/memory/base.py
+dbgpt/agent/core/memory/hybrid.py
+dbgpt/agent/core/memory/llm.py
+dbgpt/agent/core/memory/long_term.py
+dbgpt/agent/core/memory/short_term.py
+dbgpt/agent/core/memory/gpts/__init__.py
+dbgpt/agent/core/memory/gpts/base.py
+dbgpt/agent/core/memory/gpts/default_gpts_memory.py
+dbgpt/agent/core/memory/gpts/gpts_memory.py
+dbgpt/agent/core/plan/__init__.py
+dbgpt/agent/core/plan/plan_action.py
+dbgpt/agent/core/plan/planner_agent.py
+dbgpt/agent/core/plan/team_auto_plan.py
+dbgpt/agent/core/plan/awel/__init__.py
+dbgpt/agent/core/plan/awel/agent_operator.py
+dbgpt/agent/core/plan/awel/agent_operator_resource.py
+dbgpt/agent/core/plan/awel/team_awel_layout.py
+dbgpt/agent/core/profile/__init__.py
+dbgpt/agent/core/profile/base.py
 dbgpt/agent/expand/Indicator_assistant_agent.py
 dbgpt/agent/expand/__init__.py
 dbgpt/agent/expand/code_assistant_agent.py
 dbgpt/agent/expand/dashboard_assistant_agent.py
 dbgpt/agent/expand/data_scientist_agent.py
 dbgpt/agent/expand/plugin_assistant_agent.py
 dbgpt/agent/expand/retrieve_summary_assistant_agent.py
 dbgpt/agent/expand/summary_assistant_agent.py
-dbgpt/agent/memory/__init__.py
-dbgpt/agent/memory/base.py
-dbgpt/agent/memory/default_gpts_memory.py
-dbgpt/agent/memory/gpts_memory.py
-dbgpt/agent/plan/__init__.py
-dbgpt/agent/plan/plan_action.py
-dbgpt/agent/plan/planner_agent.py
-dbgpt/agent/plan/team_auto_plan.py
-dbgpt/agent/plan/awel/__init__.py
-dbgpt/agent/plan/awel/agent_operator.py
-dbgpt/agent/plan/awel/agent_operator_resource.py
-dbgpt/agent/plan/awel/team_awel_layout.py
+dbgpt/agent/expand/actions/__init__.py
+dbgpt/agent/expand/actions/chart_action.py
+dbgpt/agent/expand/actions/code_action.py
+dbgpt/agent/expand/actions/dashboard_action.py
+dbgpt/agent/expand/actions/indicator_action.py
+dbgpt/agent/expand/actions/plugin_action.py
 dbgpt/agent/plugin/__init__.py
 dbgpt/agent/plugin/generator.py
 dbgpt/agent/plugin/loader.py
 dbgpt/agent/plugin/plugins_util.py
 dbgpt/agent/plugin/commands/__init__.py
 dbgpt/agent/plugin/commands/command.py
 dbgpt/agent/plugin/commands/command_manage.py
@@ -74,14 +79,19 @@
 dbgpt/agent/resource/resource_api.py
 dbgpt/agent/resource/resource_db_api.py
 dbgpt/agent/resource/resource_knowledge_api.py
 dbgpt/agent/resource/resource_loader.py
 dbgpt/agent/resource/resource_plugin_api.py
 dbgpt/agent/util/__init__.py
 dbgpt/agent/util/cmp.py
+dbgpt/agent/util/llm/__init__.py
+dbgpt/agent/util/llm/llm.py
+dbgpt/agent/util/llm/llm_client.py
+dbgpt/agent/util/llm/strategy/__init__.py
+dbgpt/agent/util/llm/strategy/priority.py
 dbgpt/cli/__init__.py
 dbgpt/cli/cli_scripts.py
 dbgpt/client/__init__.py
 dbgpt/client/_cli.py
 dbgpt/client/app.py
 dbgpt/client/client.py
 dbgpt/client/datasource.py
@@ -148,14 +158,15 @@
 dbgpt/core/operators/flow/composer_operator.py
 dbgpt/core/operators/flow/dict_operator.py
 dbgpt/core/schema/__init__.py
 dbgpt/core/schema/api.py
 dbgpt/datasource/__init__.py
 dbgpt/datasource/base.py
 dbgpt/datasource/conn_spark.py
+dbgpt/datasource/conn_tugraph.py
 dbgpt/datasource/db_conn_info.py
 dbgpt/datasource/redis.py
 dbgpt/datasource/manages/__init__.py
 dbgpt/datasource/manages/connect_config_db.py
 dbgpt/datasource/manages/connector_manager.py
 dbgpt/datasource/nosql/__init__.py
 dbgpt/datasource/operators/__init__.py
@@ -198,14 +209,15 @@
 dbgpt/model/proxy/llms/__init__.py
 dbgpt/model/proxy/llms/baichuan.py
 dbgpt/model/proxy/llms/bard.py
 dbgpt/model/proxy/llms/chatgpt.py
 dbgpt/model/proxy/llms/claude.py
 dbgpt/model/proxy/llms/gemini.py
 dbgpt/model/proxy/llms/moonshot.py
+dbgpt/model/proxy/llms/ollama.py
 dbgpt/model/proxy/llms/proxy_model.py
 dbgpt/model/proxy/llms/spark.py
 dbgpt/model/proxy/llms/tongyi.py
 dbgpt/model/proxy/llms/wenxin.py
 dbgpt/model/proxy/llms/yi.py
 dbgpt/model/proxy/llms/zhipu.py
 dbgpt/model/utils/__init__.py
@@ -256,20 +268,22 @@
 dbgpt/rag/operators/summary.py
 dbgpt/rag/retriever/__init__.py
 dbgpt/rag/retriever/base.py
 dbgpt/rag/retriever/db_schema.py
 dbgpt/rag/retriever/embedding.py
 dbgpt/rag/retriever/rerank.py
 dbgpt/rag/retriever/rewrite.py
+dbgpt/rag/retriever/time_weighted.py
 dbgpt/rag/schemalinker/__init__.py
 dbgpt/rag/schemalinker/base_linker.py
 dbgpt/rag/schemalinker/schema_linking.py
 dbgpt/rag/summary/__init__.py
 dbgpt/rag/summary/db_summary.py
 dbgpt/rag/summary/db_summary_client.py
+dbgpt/rag/summary/gdbms_db_summary.py
 dbgpt/rag/summary/rdbms_db_summary.py
 dbgpt/rag/text_splitter/__init__.py
 dbgpt/rag/text_splitter/pre_text_splitter.py
 dbgpt/rag/text_splitter/text_splitter.py
 dbgpt/rag/text_splitter/token_splitter.py
 dbgpt/storage/__init__.py
 dbgpt/storage/schema.py
@@ -293,14 +307,15 @@
 dbgpt/storage/metadata/db_storage.py
 dbgpt/storage/vector_store/__init__.py
 dbgpt/storage/vector_store/base.py
 dbgpt/storage/vector_store/chroma_store.py
 dbgpt/storage/vector_store/connector.py
 dbgpt/storage/vector_store/filters.py
 dbgpt/storage/vector_store/milvus_store.py
+dbgpt/storage/vector_store/oceanbase_store.py
 dbgpt/storage/vector_store/pgvector_store.py
 dbgpt/storage/vector_store/weaviate_store.py
 dbgpt/util/__init__.py
 dbgpt/util/_db_migration_utils.py
 dbgpt/util/annotations.py
 dbgpt/util/api_utils.py
 dbgpt/util/chat_util.py
@@ -312,14 +327,15 @@
 dbgpt/util/error_types.py
 dbgpt/util/executor_utils.py
 dbgpt/util/fastapi.py
 dbgpt/util/formatting.py
 dbgpt/util/function_utils.py
 dbgpt/util/global_helper.py
 dbgpt/util/i18n_utils.py
+dbgpt/util/id_generator.py
 dbgpt/util/json_utils.py
 dbgpt/util/memory_utils.py
 dbgpt/util/model_utils.py
 dbgpt/util/module_utils.py
 dbgpt/util/net_utils.py
 dbgpt/util/openai_utils.py
 dbgpt/util/pagination_utils.py
@@ -329,19 +345,22 @@
 dbgpt/util/prompt_util.py
 dbgpt/util/retry.py
 dbgpt/util/similarity_util.py
 dbgpt/util/singleton.py
 dbgpt/util/splitter_utils.py
 dbgpt/util/string_utils.py
 dbgpt/util/system_utils.py
+dbgpt/util/time_utils.py
 dbgpt/util/utils.py
 dbgpt/util/benchmarks/__init__.py
 dbgpt/util/benchmarks/llm/__init__.py
 dbgpt/util/benchmarks/llm/fastchat_benchmarks_inference.py
 dbgpt/util/benchmarks/llm/llm_benchmarks.py
+dbgpt/util/configure/__init__.py
+dbgpt/util/configure/base.py
 dbgpt/util/console/__init__.py
 dbgpt/util/console/console.py
 dbgpt/util/dbgpts/__init__.py
 dbgpt/util/dbgpts/base.py
 dbgpt/util/dbgpts/cli.py
 dbgpt/util/dbgpts/loader.py
 dbgpt/util/dbgpts/repo.py
```

### Comparing `dbgpt-0.5.5rc0/dbgpt.egg-info/requires.txt` & `dbgpt-0.5.6rc0/dbgpt.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,385 +1,401 @@
 aiohttp==3.8.4
 chardet==5.1.0
 importlib-resources==5.12.0
 python-dotenv==1.0.0
 cachetools
 pydantic>=2.6.0
 typeguard
+snowflake-id
 
 [agent]
-click
-chardet==5.1.0
-httpx
+pandas==2.0.3
+cachetools
+fastapi>=0.100.0
+psutil==5.9.4
 tomlkit
 termcolor
+httpx
 importlib-resources==5.12.0
-fastapi>=0.100.0
+python-dotenv==1.0.0
 prettytable
-cachetools
-typeguard
-pandas==2.0.3
-rich
-psutil==5.9.4
 aiohttp==3.8.4
+snowflake-id
 colorama==0.4.6
-python-dotenv==1.0.0
+rich
+click
+chardet==5.1.0
+typeguard
 pydantic>=2.6.0
 
 [all]
-click
-fschat
+sqlparse==0.4.4
+markdown
+sentence-transformers
+msgpack
+alembic==1.12.0
+rich
+pypdf
+psycopg2
+python-multipart
 importlib-resources==5.12.0
-typeguard
-thrift
-SQLAlchemy<2.0.29,>=2.0.25
-gpt4all
-pymilvus
+prettytable
+thrift_sasl
+auto-gpt-plugin-template
+sentencepiece
 GitPython
 gTTS==2.3.1
 clickhouse-connect
-dashscope
-sentence-transformers
-cpm_kernels
-openai
-sqlparse==0.4.4
-graphviz
-python-dotenv==1.0.0
-duckdb
+pydantic>=2.6.0
+seaborn
+psutil==5.9.4
+gpt4all
+zhipuai
+click
+pandas==2.0.3
+jsonschema
+vllm
+httpx
+colorama==0.4.6
+snowflake-id
+pyhive
+chardet==5.1.0
+weaviate-client
+pyspark
+termcolor
+pymilvus
 shortuuid
+cpm_kernels
+neo4j
+typeguard
 torchaudio==2.2.1
-duckdb-engine
-markdown
-pymysql
+accelerate>=0.20.3
 rocksdict
-bitsandbytes
-pypdf
+spacy>=3.7
+pympler
+tomlkit
+uvicorn
+coloredlogs
+tokenizers>=0.14
+python-dotenv==1.0.0
+duckdb
+xlrd==2.0.1
+aiohttp==3.8.4
 openpyxl==3.1.2
-bs4
+schedule
+tiktoken
+ollama
 chromadb>=0.4.22
-pyspark
-chardet==5.1.0
-httpx
-tomlkit
+jinja2
+torchvision==0.17.1
+pymysql
 cachetools
-transformers>=4.34.0
-pymssql
-termcolor
-accelerate>=0.20.3
-aiohttp==3.8.4
-uvicorn
-sentencepiece
-spacy>=3.7
-pympler
-alembic==1.12.0
-chardet
-psycopg2
+thrift
+torch==2.2.1
+dashscope
+fschat
+graphviz
+SQLAlchemy<2.0.29,>=2.0.25
+duckdb-engine
 fastapi>=0.100.0
-schedule
 python-docx
-pyhive
-pydantic>=2.6.0
-python-pptx
-zhipuai
-pandas==2.0.3
-torchvision==0.17.1
-tiktoken
-xlrd==2.0.1
-msgpack
-mysqlclient==2.1.0
-rich
+pymssql
+llama-cpp-python
+transformers>=4.34.0
+aiofiles
 pydoris<2.0.0,>=1.0.2
-colorama==0.4.6
 langchain>=0.0.286
-torch==2.2.1
-coloredlogs
-aiofiles
-llama-cpp-python
-seaborn
-jinja2
-python-multipart
-tokenizers>=0.14
-vllm
-auto-gpt-plugin-template
-psutil==5.9.4
-thrift_sasl
-prettytable
-weaviate-client
-jsonschema
+openai
+bs4
+python-pptx
+chardet
+bitsandbytes
+mysqlclient==2.1.0
 
 [bitsandbytes]
 bitsandbytes
 
 [cache]
 rocksdict
 
 [cli]
-click
-chardet==5.1.0
-httpx
+cachetools
+fastapi>=0.100.0
+psutil==5.9.4
 tomlkit
+httpx
 importlib-resources==5.12.0
-fastapi>=0.100.0
+python-dotenv==1.0.0
 prettytable
-cachetools
-typeguard
-rich
-psutil==5.9.4
 aiohttp==3.8.4
+snowflake-id
 colorama==0.4.6
-python-dotenv==1.0.0
+rich
+click
+chardet==5.1.0
+typeguard
 pydantic>=2.6.0
 
 [client]
-chardet==5.1.0
+cachetools
+fastapi>=0.100.0
 httpx
 importlib-resources==5.12.0
-fastapi>=0.100.0
-cachetools
-typeguard
-aiohttp==3.8.4
 python-dotenv==1.0.0
+aiohttp==3.8.4
+snowflake-id
+chardet==5.1.0
+typeguard
 pydantic>=2.6.0
 
 [core]
-chardet==5.1.0
-importlib-resources==5.12.0
 cachetools
-typeguard
-aiohttp==3.8.4
+importlib-resources==5.12.0
 python-dotenv==1.0.0
+aiohttp==3.8.4
+snowflake-id
+chardet==5.1.0
+typeguard
 pydantic>=2.6.0
 
 [datasource]
 pymysql
 
 [datasource_all]
+pymysql
+thrift
 pymssql
-pyspark
 clickhouse-connect
 thrift_sasl
-mysqlclient==2.1.0
 pydoris<2.0.0,>=1.0.2
+neo4j
 pyhive
-pymysql
-thrift
 psycopg2
+mysqlclient==2.1.0
+pyspark
 
 [default]
-click
-fschat
-torchaudio==2.2.1
-msgpack
-uvicorn
-importlib-resources==5.12.0
-sentencepiece
-typeguard
-rich
-duckdb-engine
-spacy>=3.7
-pymysql
+schedule
+sqlparse==0.4.4
+seaborn
 markdown
-colorama==0.4.6
-rocksdict
-langchain>=0.0.286
-pympler
+msgpack
+termcolor
+sentence-transformers
 alembic==1.12.0
-torch==2.2.1
-chardet
-SQLAlchemy<2.0.29,>=2.0.25
-coloredlogs
-aiofiles
+rich
+ollama
+shortuuid
 pypdf
-seaborn
-openpyxl==3.1.2
+chromadb>=0.4.22
+cpm_kernels
+typeguard
 jinja2
-fastapi>=0.100.0
 python-multipart
-bs4
-tokenizers>=0.14
-schedule
-GitPython
-chromadb>=0.4.22
-chardet==5.1.0
-httpx
-tomlkit
-gTTS==2.3.1
-python-docx
+torchvision==0.17.1
+pymysql
 cachetools
-auto-gpt-plugin-template
-dashscope
-pydantic>=2.6.0
 psutil==5.9.4
-transformers>=4.34.0
-sentence-transformers
-zhipuai
-python-pptx
-cpm_kernels
-termcolor
+torch==2.2.1
+torchaudio==2.2.1
+dashscope
+importlib-resources==5.12.0
 prettytable
-sqlparse==0.4.4
 accelerate>=0.20.3
-pandas==2.0.3
+fschat
+zhipuai
+SQLAlchemy<2.0.29,>=2.0.25
 graphviz
-torchvision==0.17.1
-aiohttp==3.8.4
-jsonschema
-python-dotenv==1.0.0
-xlrd==2.0.1
-duckdb
-shortuuid
-
-[framework]
+rocksdict
 click
-fschat
-msgpack
-uvicorn
-importlib-resources==5.12.0
-typeguard
-rich
 duckdb-engine
-pymysql
-colorama==0.4.6
+pandas==2.0.3
+fastapi>=0.100.0
+jsonschema
+spacy>=3.7
 pympler
-alembic==1.12.0
-SQLAlchemy<2.0.29,>=2.0.25
+tomlkit
+uvicorn
+auto-gpt-plugin-template
+httpx
 coloredlogs
+tokenizers>=0.14
+python-dotenv==1.0.0
+snowflake-id
+colorama==0.4.6
+transformers>=4.34.0
+sentencepiece
 aiofiles
-seaborn
-openpyxl==3.1.2
-jinja2
-fastapi>=0.100.0
+python-docx
 GitPython
-schedule
 chardet==5.1.0
-httpx
-tomlkit
+langchain>=0.0.286
 gTTS==2.3.1
-cachetools
-auto-gpt-plugin-template
-transformers>=4.34.0
+bs4
+duckdb
+python-pptx
+chardet
+xlrd==2.0.1
+aiohttp==3.8.4
+bitsandbytes
+openpyxl==3.1.2
 pydantic>=2.6.0
-psutil==5.9.4
+
+[framework]
+schedule
+sqlparse==0.4.4
+seaborn
+msgpack
 termcolor
+alembic==1.12.0
+rich
+shortuuid
+typeguard
+jinja2
+pymysql
+cachetools
+psutil==5.9.4
+importlib-resources==5.12.0
 prettytable
-sqlparse==0.4.4
-pandas==2.0.3
+fschat
 graphviz
-aiohttp==3.8.4
+SQLAlchemy<2.0.29,>=2.0.25
+click
+duckdb-engine
+pandas==2.0.3
+fastapi>=0.100.0
 jsonschema
+pympler
+tomlkit
+uvicorn
+auto-gpt-plugin-template
+httpx
+coloredlogs
 python-dotenv==1.0.0
-xlrd==2.0.1
+colorama==0.4.6
+snowflake-id
+transformers>=4.34.0
+aiofiles
+GitPython
+chardet==5.1.0
+gTTS==2.3.1
 duckdb
-shortuuid
+xlrd==2.0.1
+aiohttp==3.8.4
+openpyxl==3.1.2
+pydantic>=2.6.0
 
 [gpt4all]
 gpt4all
 
 [llama_cpp]
 llama-cpp-python
 
 [openai]
-click
-fschat
-msgpack
-uvicorn
-importlib-resources==5.12.0
-typeguard
-rich
-duckdb-engine
-spacy>=3.7
-pymysql
+schedule
+sqlparse==0.4.4
+seaborn
 markdown
-colorama==0.4.6
-langchain>=0.0.286
-pympler
+msgpack
+termcolor
+sentence-transformers
+tiktoken
 alembic==1.12.0
-SQLAlchemy<2.0.29,>=2.0.25
-coloredlogs
-aiofiles
+rich
+shortuuid
 pypdf
-seaborn
-openpyxl==3.1.2
+chromadb>=0.4.22
+typeguard
 jinja2
-fastapi>=0.100.0
 python-multipart
-bs4
-GitPython
-schedule
-chromadb>=0.4.22
-chardet==5.1.0
-httpx
-tomlkit
-gTTS==2.3.1
-python-docx
+pymysql
 cachetools
-auto-gpt-plugin-template
-transformers>=4.34.0
-pydantic>=2.6.0
 psutil==5.9.4
-sentence-transformers
-python-pptx
-termcolor
-openai
+importlib-resources==5.12.0
 prettytable
-sqlparse==0.4.4
-pandas==2.0.3
+fschat
 graphviz
-tiktoken
-aiohttp==3.8.4
+SQLAlchemy<2.0.29,>=2.0.25
+click
+duckdb-engine
+pandas==2.0.3
+fastapi>=0.100.0
 jsonschema
+spacy>=3.7
+pympler
+tomlkit
+uvicorn
+auto-gpt-plugin-template
+httpx
+coloredlogs
 python-dotenv==1.0.0
-xlrd==2.0.1
+colorama==0.4.6
+snowflake-id
+transformers>=4.34.0
+aiofiles
+python-docx
+GitPython
+chardet==5.1.0
+langchain>=0.0.286
+openai
+gTTS==2.3.1
+bs4
 duckdb
-shortuuid
+python-pptx
+xlrd==2.0.1
+aiohttp==3.8.4
+openpyxl==3.1.2
+pydantic>=2.6.0
 
 [quantization]
 cpm_kernels
+bitsandbytes
 
 [rag]
-pypdf
-python-pptx
-python-docx
-spacy>=3.7
+bs4
 markdown
-python-multipart
+spacy>=3.7
 sentence-transformers
-langchain>=0.0.286
-bs4
+python-pptx
+python-docx
+pypdf
 chromadb>=0.4.22
+langchain>=0.0.286
+python-multipart
 
 [simple_framework]
-click
-fschat
+schedule
+sqlparse==0.4.4
 msgpack
-uvicorn
-importlib-resources==5.12.0
-typeguard
+termcolor
 rich
-duckdb-engine
-colorama==0.4.6
-pympler
-SQLAlchemy<2.0.29,>=2.0.25
+shortuuid
+typeguard
 jinja2
-fastapi>=0.100.0
-schedule
-chardet==5.1.0
-httpx
-tomlkit
 cachetools
-pydantic>=2.6.0
 psutil==5.9.4
-termcolor
+importlib-resources==5.12.0
 prettytable
-sqlparse==0.4.4
+fschat
+SQLAlchemy<2.0.29,>=2.0.25
+click
+duckdb-engine
 pandas==2.0.3
-aiohttp==3.8.4
+fastapi>=0.100.0
+pympler
+tomlkit
+uvicorn
+httpx
 python-dotenv==1.0.0
+colorama==0.4.6
+snowflake-id
+chardet==5.1.0
 duckdb
-shortuuid
+aiohttp==3.8.4
+pydantic>=2.6.0
 
 [torch]
 torchvision==0.17.1
 torch==2.2.1
 torchaudio==2.2.1
 
 [torch_cpu]
@@ -396,17 +412,17 @@
 vllm
 
 [vstore]
 chromadb>=0.4.22
 
 [vstore_all]
 pymilvus
-chromadb>=0.4.22
 weaviate-client
+chromadb>=0.4.22
 
 [vstore_milvus]
 pymilvus
 chromadb>=0.4.22
 
 [vstore_weaviate]
-chromadb>=0.4.22
 weaviate-client
+chromadb>=0.4.22
```

### Comparing `dbgpt-0.5.5rc0/setup.py` & `dbgpt-0.5.6rc0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 
 with open("README.md", mode="r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 IS_DEV_MODE = os.getenv("IS_DEV_MODE", "true").lower() == "true"
 # If you modify the version, please modify the version in the following files:
 # dbgpt/_version.py
-DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.4")
+DB_GPT_VERSION = os.getenv("DB_GPT_VERSION", "0.5.5")
 
 BUILD_NO_CACHE = os.getenv("BUILD_NO_CACHE", "true").lower() == "true"
 LLAMA_CPP_GPU_ACCELERATION = (
     os.getenv("LLAMA_CPP_GPU_ACCELERATION", "true").lower() == "true"
 )
 BUILD_FROM_SOURCE = os.getenv("BUILD_FROM_SOURCE", "false").lower() == "true"
 BUILD_FROM_SOURCE_URL_FAST_CHAT = os.getenv(
     "BUILD_FROM_SOURCE_URL_FAST_CHAT", "git+https://github.com/lm-sys/FastChat.git"
 )
 BUILD_VERSION_OPENAI = os.getenv("BUILD_VERSION_OPENAI")
+INCLUDE_QUANTIZATION = os.getenv("INCLUDE_QUANTIZATION", "true").lower() == "true"
 
 
 def parse_requirements(file_name: str) -> List[str]:
     with open(file_name) as f:
         return [
             require.strip()
             for require in f
@@ -411,14 +412,16 @@
         "chardet==5.1.0",
         "importlib-resources==5.12.0",
         "python-dotenv==1.0.0",
         "cachetools",
         "pydantic>=2.6.0",
         # For AWEL type checking
         "typeguard",
+        # Snowflake no additional dependencies.
+        "snowflake-id",
     ]
     # For DB-GPT python client SDK
     setup_spec.extras["client"] = setup_spec.extras["core"] + [
         "httpx",
         "fastapi>=0.100.0",
     ]
     # Simple command line dependencies
@@ -548,15 +551,17 @@
         autoawq_latest_version = get_latest_version("autoawq", "", "0.2.4")
         if cuda_version is None or cuda_version == "12.1":
             quantization_pkgs.extend(["autoawq", _build_autoawq_requires(), "optimum"])
         else:
             # TODO(yyhhyy): Add autoawq install method for CUDA version 11.8
             quantization_pkgs.extend(["autoawq", _build_autoawq_requires(), "optimum"])
 
-    setup_spec.extras["quantization"] = ["cpm_kernels"] + quantization_pkgs
+    setup_spec.extras["quantization"] = (
+        ["cpm_kernels"] + quantization_pkgs + setup_spec.extras["bitsandbytes"]
+    )
 
 
 def all_vector_store_requires():
     """
     pip install "dbgpt[vstore]"
     """
     setup_spec.extras["vstore"] = [
@@ -599,14 +604,15 @@
         "mysqlclient==2.1.0",
         # pydoris is too old, we should find a new package to replace it.
         "pydoris>=1.0.2,<2.0.0",
         "clickhouse-connect",
         "pyhive",
         "thrift",
         "thrift_sasl",
+        "neo4j",
     ]
 
 
 def openai_requires():
     """
     pip install "dbgpt[openai]"
     """
@@ -650,20 +656,23 @@
         # "tokenizers==0.13.3",
         "tokenizers>=0.14",
         "accelerate>=0.20.3",
         "zhipuai",
         "dashscope",
         "chardet",
         "sentencepiece",
+        "ollama",
     ]
     setup_spec.extras["default"] += setup_spec.extras["framework"]
     setup_spec.extras["default"] += setup_spec.extras["rag"]
     setup_spec.extras["default"] += setup_spec.extras["datasource"]
     setup_spec.extras["default"] += setup_spec.extras["torch"]
-    setup_spec.extras["default"] += setup_spec.extras["quantization"]
+    if INCLUDE_QUANTIZATION:
+        # Add quantization extra to default, default is True
+        setup_spec.extras["default"] += setup_spec.extras["quantization"]
     setup_spec.extras["default"] += setup_spec.extras["cache"]
 
 
 def all_requires():
     requires = set()
     for _, pkgs in setup_spec.extras.items():
         for pkg in pkgs:
```

