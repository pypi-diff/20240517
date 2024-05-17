# Comparing `tmp/langchain_community-0.2.0.tar.gz` & `tmp/langchain_community-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_community-0.2.0.tar", max compression
+gzip compressed data, was "langchain_community-0.2.0rc1.tar", max compression
```

## Comparing `langchain_community-0.2.0.tar` & `langchain_community-0.2.0rc1.tar`

### file list

```diff
@@ -1,1147 +1,1142 @@
--rw-r--r--   0        0        0     1352 2024-05-17 20:49:58.703865 langchain_community-0.2.0/README.md
--rw-r--r--   0        0        0      307 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/__init__.py
--rw-r--r--   0        0        0      336 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/adapters/__init__.py
--rw-r--r--   0        0        0    12347 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/adapters/openai.py
--rw-r--r--   0        0        0     6498 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/__init__.py
--rw-r--r--   0        0        0       25 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/ainetwork/__init__.py
--rw-r--r--   0        0        0     1762 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/ainetwork/toolkit.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/amadeus/__init__.py
--rw-r--r--   0        0        0     1084 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/amadeus/toolkit.py
--rw-r--r--   0        0        0     1057 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/azure_ai_services.py
--rw-r--r--   0        0        0     1114 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/azure_cognitive_services.py
--rw-r--r--   0        0        0       99 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/base.py
--rw-r--r--   0        0        0       32 2024-05-17 20:49:58.703865 langchain_community-0.2.0/langchain_community/agent_toolkits/cassandra_database/__init__.py
--rw-r--r--   0        0        0     1026 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/cassandra_database/toolkit.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/clickup/__init__.py
--rw-r--r--   0        0        0     3602 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/clickup/toolkit.py
--rw-r--r--   0        0        0       26 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/cogniswitch/__init__.py
--rw-r--r--   0        0        0     1322 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/cogniswitch/toolkit.py
--rw-r--r--   0        0        0      116 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/connery/__init__.py
--rw-r--r--   0        0        0     1393 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/connery/toolkit.py
--rw-r--r--   0        0        0     1091 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/csv/__init__.py
--rw-r--r--   0        0        0      177 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/file_management/__init__.py
--rw-r--r--   0        0        0     3196 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/file_management/toolkit.py
--rw-r--r--   0        0        0       22 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/github/__init__.py
--rw-r--r--   0        0        0    10142 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/github/toolkit.py
--rw-r--r--   0        0        0       22 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/gitlab/__init__.py
--rw-r--r--   0        0        0     2912 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/gitlab/toolkit.py
--rw-r--r--   0        0        0       21 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/gmail/__init__.py
--rw-r--r--   0        0        0     2026 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/gmail/toolkit.py
--rw-r--r--   0        0        0       20 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/jira/__init__.py
--rw-r--r--   0        0        0     2235 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/jira/toolkit.py
--rw-r--r--   0        0        0       18 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/json/__init__.py
--rw-r--r--   0        0        0     1894 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/json/base.py
--rw-r--r--   0        0        0     1819 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/json/prompt.py
--rw-r--r--   0        0        0      577 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/json/toolkit.py
--rw-r--r--   0        0        0    28945 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/load_tools.py
--rw-r--r--   0        0        0       23 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/multion/__init__.py
--rw-r--r--   0        0        0     1172 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/multion/toolkit.py
--rw-r--r--   0        0        0       19 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/nasa/__init__.py
--rw-r--r--   0        0        0     1939 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/nasa/toolkit.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/nla/__init__.py
--rw-r--r--   0        0        0     2006 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/nla/tool.py
--rw-r--r--   0        0        0     4177 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/nla/toolkit.py
--rw-r--r--   0        0        0       25 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/office365/__init__.py
--rw-r--r--   0        0        0     1793 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/office365/toolkit.py
--rw-r--r--   0        0        0       26 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/__init__.py
--rw-r--r--   0        0        0     2870 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/base.py
--rw-r--r--   0        0        0    13974 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/planner.py
--rw-r--r--   0        0        0    11686 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/planner_prompt.py
--rw-r--r--   0        0        0     1770 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/prompt.py
--rw-r--r--   0        0        0     2557 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/spec.py
--rw-r--r--   0        0        0     4238 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/toolkit.py
--rw-r--r--   0        0        0      174 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/playwright/__init__.py
--rw-r--r--   0        0        0     4223 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/playwright/toolkit.py
--rw-r--r--   0        0        0       22 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/polygon/__init__.py
--rw-r--r--   0        0        0     1107 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/polygon/toolkit.py
--rw-r--r--   0        0        0       22 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/__init__.py
--rw-r--r--   0        0        0     2491 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/base.py
--rw-r--r--   0        0        0     2649 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/chat_base.py
--rw-r--r--   0        0        0     2773 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/prompt.py
--rw-r--r--   0        0        0     3778 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/toolkit.py
--rw-r--r--   0        0        0       21 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/slack/__init__.py
--rw-r--r--   0        0        0     1095 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/slack/toolkit.py
--rw-r--r--   0        0        0       23 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/spark_sql/__init__.py
--rw-r--r--   0        0        0     2355 2024-05-17 20:49:58.707865 langchain_community-0.2.0/langchain_community/agent_toolkits/spark_sql/base.py
--rw-r--r--   0        0        0     1202 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/spark_sql/prompt.py
--rw-r--r--   0        0        0     1065 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/spark_sql/toolkit.py
--rw-r--r--   0        0        0       17 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/sql/__init__.py
--rw-r--r--   0        0        0     9398 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/sql/base.py
--rw-r--r--   0        0        0     1428 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/sql/prompt.py
--rw-r--r--   0        0        0     2983 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/sql/toolkit.py
--rw-r--r--   0        0        0       21 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/steam/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/steam/toolkit.py
--rw-r--r--   0        0        0     1095 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/xorbits/__init__.py
--rw-r--r--   0        0        0       22 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/zapier/__init__.py
--rw-r--r--   0        0        0     1966 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/agent_toolkits/zapier/toolkit.py
--rw-r--r--   0        0        0    91226 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/cache.py
--rw-r--r--   0        0        0     5635 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/__init__.py
--rw-r--r--   0        0        0    14597 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/aim_callback.py
--rw-r--r--   0        0        0    14738 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/argilla_callback.py
--rw-r--r--   0        0        0     7480 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/arize_callback.py
--rw-r--r--   0        0        0    11242 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/arthur_callback.py
--rw-r--r--   0        0        0     3906 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/bedrock_anthropic_callback.py
--rw-r--r--   0        0        0    18634 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/clearml_callback.py
--rw-r--r--   0        0        0    22975 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/comet_ml_callback.py
--rw-r--r--   0        0        0     6382 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/confident_callback.py
--rw-r--r--   0        0        0     6496 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/context_callback.py
--rw-r--r--   0        0        0    11430 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/fiddler_callback.py
--rw-r--r--   0        0        0    12769 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/flyte_callback.py
--rw-r--r--   0        0        0     2587 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/human.py
--rw-r--r--   0        0        0     8764 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/infino_callback.py
--rw-r--r--   0        0        0    13879 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/labelstudio_callback.py
--rw-r--r--   0        0        0    20555 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/llmonitor_callback.py
--rw-r--r--   0        0        0     3201 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/manager.py
--rw-r--r--   0        0        0    27406 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/mlflow_callback.py
--rw-r--r--   0        0        0     8575 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/openai_info.py
--rw-r--r--   0        0        0     5535 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/promptlayer_callback.py
--rw-r--r--   0        0        0     8787 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/sagemaker_callback.py
--rw-r--r--   0        0        0     3183 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/streamlit/__init__.py
--rw-r--r--   0        0        0     5395 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/streamlit/mutable_expander.py
--rw-r--r--   0        0        0    15562 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/streamlit/streamlit_callback_handler.py
--rw-r--r--   0        0        0      498 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/tracers/__init__.py
--rw-r--r--   0        0        0     4547 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/tracers/comet.py
--rw-r--r--   0        0        0    19020 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/tracers/wandb.py
--rw-r--r--   0        0        0     4526 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/trubrics_callback.py
--rw-r--r--   0        0        0    14446 2024-05-17 20:49:58.711865 langchain_community-0.2.0/langchain_community/callbacks/uptrain_callback.py
--rw-r--r--   0        0        0     7879 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/callbacks/utils.py
--rw-r--r--   0        0        0    20385 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/callbacks/wandb_callback.py
--rw-r--r--   0        0        0     7881 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/callbacks/whylabs_callback.py
--rw-r--r--   0        0        0      618 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/__init__.py
--rw-r--r--   0        0        0      465 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/ernie_functions/__init__.py
--rw-r--r--   0        0        0    23323 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/ernie_functions/base.py
--rw-r--r--   0        0        0       49 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/__init__.py
--rw-r--r--   0        0        0     8407 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/arangodb.py
--rw-r--r--   0        0        0     3699 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/base.py
--rw-r--r--   0        0        0    10589 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/cypher.py
--rw-r--r--   0        0        0     9625 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/cypher_utils.py
--rw-r--r--   0        0        0     5295 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/falkordb.py
--rw-r--r--   0        0        0     7818 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/gremlin.py
--rw-r--r--   0        0        0     3727 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/hugegraph.py
--rw-r--r--   0        0        0     5516 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/kuzu.py
--rw-r--r--   0        0        0     3715 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/nebulagraph.py
--rw-r--r--   0        0        0     6908 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/neptune_cypher.py
--rw-r--r--   0        0        0     6818 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/neptune_sparql.py
--rw-r--r--   0        0        0     7197 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/ontotext_graphdb.py
--rw-r--r--   0        0        0    16640 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/prompts.py
--rw-r--r--   0        0        0     5848 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/graph_qa/sparql.py
--rw-r--r--   0        0        0     3251 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/llm_requests.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/openapi/__init__.py
--rw-r--r--   0        0        0     8786 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/openapi/chain.py
--rw-r--r--   0        0        0     1791 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/openapi/prompts.py
--rw-r--r--   0        0        0     1974 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/openapi/requests_chain.py
--rw-r--r--   0        0        0     1846 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/openapi/response_chain.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/pebblo_retrieval/__init__.py
--rw-r--r--   0        0        0     7715 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/pebblo_retrieval/base.py
--rw-r--r--   0        0        0    10334 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/pebblo_retrieval/enforcement_filters.py
--rw-r--r--   0        0        0     1707 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chains/pebblo_retrieval/models.py
--rw-r--r--   0        0        0     2748 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/__init__.py
--rw-r--r--   0        0        0       85 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/base.py
--rw-r--r--   0        0        0     2694 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/facebook_messenger.py
--rw-r--r--   0        0        0     4213 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/gmail.py
--rw-r--r--   0        0        0     7925 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/imessage.py
--rw-r--r--   0        0        0     5736 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/langsmith.py
--rw-r--r--   0        0        0     3127 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/slack.py
--rw-r--r--   0        0        0     5379 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/telegram.py
--rw-r--r--   0        0        0     3296 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/utils.py
--rw-r--r--   0        0        0     4295 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_loaders/whatsapp.py
--rw-r--r--   0        0        0     5677 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_message_histories/__init__.py
--rw-r--r--   0        0        0     5874 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_message_histories/astradb.py
--rw-r--r--   0        0        0     3016 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_message_histories/cassandra.py
--rw-r--r--   0        0        0     6510 2024-05-17 20:49:58.715865 langchain_community-0.2.0/langchain_community/chat_message_histories/cosmos_db.py
--rw-r--r--   0        0        0     7250 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/dynamodb.py
--rw-r--r--   0        0        0     7177 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/elasticsearch.py
--rw-r--r--   0        0        0     1402 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/file.py
--rw-r--r--   0        0        0     3349 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/firestore.py
--rw-r--r--   0        0        0      130 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/in_memory.py
--rw-r--r--   0        0        0     7112 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/momento.py
--rw-r--r--   0        0        0     3107 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/mongodb.py
--rw-r--r--   0        0        0     5129 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/neo4j.py
--rw-r--r--   0        0        0     3345 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/postgres.py
--rw-r--r--   0        0        0     2192 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/redis.py
--rw-r--r--   0        0        0     9529 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/rocksetdb.py
--rw-r--r--   0        0        0    10331 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/singlestoredb.py
--rw-r--r--   0        0        0     4722 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/sql.py
--rw-r--r--   0        0        0     1444 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/streamlit.py
--rw-r--r--   0        0        0     5255 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/tidb.py
--rw-r--r--   0        0        0     2148 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/upstash_redis.py
--rw-r--r--   0        0        0     4639 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/xata.py
--rw-r--r--   0        0        0     8910 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_message_histories/zep.py
--rw-r--r--   0        0        0     9183 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/__init__.py
--rw-r--r--   0        0        0     8210 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/anthropic.py
--rw-r--r--   0        0        0     8250 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/anyscale.py
--rw-r--r--   0        0        0    11341 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/azure_openai.py
--rw-r--r--   0        0        0    15437 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/azureml_endpoint.py
--rw-r--r--   0        0        0     9987 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/baichuan.py
--rw-r--r--   0        0        0    23064 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0    10959 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/bedrock.py
--rw-r--r--   0        0        0     8226 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/cohere.py
--rw-r--r--   0        0        0     8513 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/coze.py
--rw-r--r--   0        0        0     5396 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/dappier.py
--rw-r--r--   0        0        0     1532 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/databricks.py
--rw-r--r--   0        0        0    16723 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/deepinfra.py
--rw-r--r--   0        0        0    13134 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/edenai.py
--rw-r--r--   0        0        0     8039 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/ernie.py
--rw-r--r--   0        0        0     5587 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/everlyai.py
--rw-r--r--   0        0        0     3217 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/fake.py
--rw-r--r--   0        0        0    12018 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/fireworks.py
--rw-r--r--   0        0        0     7114 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/friendli.py
--rw-r--r--   0        0        0     9738 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/gigachat.py
--rw-r--r--   0        0        0    11608 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/google_palm.py
--rw-r--r--   0        0        0    13080 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/gpt_router.py
--rw-r--r--   0        0        0     7933 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/huggingface.py
--rw-r--r--   0        0        0     3741 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/human.py
--rw-r--r--   0        0        0    10653 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/hunyuan.py
--rw-r--r--   0        0        0     7628 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/javelin_ai_gateway.py
--rw-r--r--   0        0        0    15316 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/jinachat.py
--rw-r--r--   0        0        0    20267 2024-05-17 20:49:58.719865 langchain_community-0.2.0/langchain_community/chat_models/kinetica.py
--rw-r--r--   0        0        0    10026 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/konko.py
--rw-r--r--   0        0        0    15832 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/litellm.py
--rw-r--r--   0        0        0     8077 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/litellm_router.py
--rw-r--r--   0        0        0     8616 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/llama_edge.py
--rw-r--r--   0        0        0    13406 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/maritalk.py
--rw-r--r--   0        0        0      967 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/meta.py
--rw-r--r--   0        0        0     3284 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/minimax.py
--rw-r--r--   0        0        0     9874 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/mlflow.py
--rw-r--r--   0        0        0     6711 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/mlflow_ai_gateway.py
--rw-r--r--   0        0        0     6166 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/mlx.py
--rw-r--r--   0        0        0     1927 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/moonshot.py
--rw-r--r--   0        0        0     3308 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/octoai.py
--rw-r--r--   0        0        0    13444 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/ollama.py
--rw-r--r--   0        0        0    26842 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/openai.py
--rw-r--r--   0        0        0    10504 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/pai_eas_endpoint.py
--rw-r--r--   0        0        0    10717 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/perplexity.py
--rw-r--r--   0        0        0    14623 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/premai.py
--rw-r--r--   0        0        0     5256 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/promptlayer_openai.py
--rw-r--r--   0        0        0     2322 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/solar.py
--rw-r--r--   0        0        0    16900 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/sparkllm.py
--rw-r--r--   0        0        0    21549 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/tongyi.py
--rw-r--r--   0        0        0    14583 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/vertexai.py
--rw-r--r--   0        0        0     5296 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/volcengine_maas.py
--rw-r--r--   0        0        0    10740 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/yandex.py
--rw-r--r--   0        0        0    17252 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/yuan2.py
--rw-r--r--   0        0        0    16839 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/chat_models/zhipuai.py
--rw-r--r--   0        0        0     1468 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/cross_encoders/__init__.py
--rw-r--r--   0        0        0      117 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/cross_encoders/base.py
--rw-r--r--   0        0        0      525 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/cross_encoders/fake.py
--rw-r--r--   0        0        0     1946 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/cross_encoders/huggingface.py
--rw-r--r--   0        0        0     5335 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/cross_encoders/sagemaker_endpoint.py
--rw-r--r--   0        0        0     1176 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/docstore/__init__.py
--rw-r--r--   0        0        0     1080 2024-05-17 20:49:58.723865 langchain_community-0.2.0/langchain_community/docstore/arbitrary_fn.py
--rw-r--r--   0        0        0      833 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/docstore/base.py
--rw-r--r--   0        0        0       70 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/docstore/document.py
--rw-r--r--   0        0        0     1610 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/docstore/in_memory.py
--rw-r--r--   0        0        0     1472 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/docstore/wikipedia.py
--rw-r--r--   0        0        0     1215 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/document_compressors/__init__.py
--rw-r--r--   0        0        0     2444 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/document_compressors/flashrank_rerank.py
--rw-r--r--   0        0        0     4342 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/document_compressors/jina_rerank.py
--rw-r--r--   0        0        0     6695 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/document_compressors/llmlingua_filter.py
--rw-r--r--   0        0        0     5704 2024-05-17 20:49:58.727865 langchain_community-0.2.0/langchain_community/document_compressors/openvino_rerank.py
--rw-r--r--   0        0        0    35823 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/__init__.py
--rw-r--r--   0        0        0     2803 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/acreom.py
--rw-r--r--   0        0        0    10157 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/airbyte.py
--rw-r--r--   0        0        0      865 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/airbyte_json.py
--rw-r--r--   0        0        0     1157 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/airtable.py
--rw-r--r--   0        0        0     2759 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/apify_dataset.py
--rw-r--r--   0        0        0     5129 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/arcgis_loader.py
--rw-r--r--   0        0        0      907 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/arxiv.py
--rw-r--r--   0        0        0     8134 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/assemblyai.py
--rw-r--r--   0        0        0     4642 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/astradb.py
--rw-r--r--   0        0        0     8589 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/async_html.py
--rw-r--r--   0        0        0     5886 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/athena.py
--rw-r--r--   0        0        0      563 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/azlyrics.py
--rw-r--r--   0        0        0     1432 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/azure_ai_data.py
--rw-r--r--   0        0        0     1566 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/azure_blob_storage_container.py
--rw-r--r--   0        0        0     1644 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/azure_blob_storage_file.py
--rw-r--r--   0        0        0     1774 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/baiducloud_bos_directory.py
--rw-r--r--   0        0        0     1848 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/baiducloud_bos_file.py
--rw-r--r--   0        0        0      126 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/base.py
--rw-r--r--   0        0        0     7248 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/base_o365.py
--rw-r--r--   0        0        0     3540 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/bibtex.py
--rw-r--r--   0        0        0     3852 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/bigquery.py
--rw-r--r--   0        0        0     4401 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/bilibili.py
--rw-r--r--   0        0        0    10288 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/blackboard.py
--rw-r--r--   0        0        0      948 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/blob_loaders/__init__.py
--rw-r--r--   0        0        0     5390 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/blob_loaders/file_system.py
--rw-r--r--   0        0        0      145 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/blob_loaders/schema.py
--rw-r--r--   0        0        0     1526 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/blob_loaders/youtube_audio.py
--rw-r--r--   0        0        0     5709 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/blockchain.py
--rw-r--r--   0        0        0     1047 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/brave_search.py
--rw-r--r--   0        0        0     1540 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/browserbase.py
--rw-r--r--   0        0        0     2007 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/browserless.py
--rw-r--r--   0        0        0     5142 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/cassandra.py
--rw-r--r--   0        0        0     1986 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/chatgpt.py
--rw-r--r--   0        0        0     3031 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/chm.py
--rw-r--r--   0        0        0     3410 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/chromium.py
--rw-r--r--   0        0        0      527 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/college_confidential.py
--rw-r--r--   0        0        0     3416 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/concurrent.py
--rw-r--r--   0        0        0    29324 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/confluence.py
--rw-r--r--   0        0        0     1102 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/conllu.py
--rw-r--r--   0        0        0     3515 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/couchbase.py
--rw-r--r--   0        0        0     5835 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/csv_loader.py
--rw-r--r--   0        0        0     6589 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/cube_semantic.py
--rw-r--r--   0        0        0     4937 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/datadog_logs.py
--rw-r--r--   0        0        0     2176 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/dataframe.py
--rw-r--r--   0        0        0     2054 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/diffbot.py
--rw-r--r--   0        0        0     8446 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/directory.py
--rw-r--r--   0        0        0     1237 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/discord.py
--rw-r--r--   0        0        0     3859 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/doc_intelligence.py
--rw-r--r--   0        0        0    13621 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/docugami.py
--rw-r--r--   0        0        0     1852 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/docusaurus.py
--rw-r--r--   0        0        0     6271 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/dropbox.py
--rw-r--r--   0        0        0     3150 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/duckdb_loader.py
--rw-r--r--   0        0        0     3835 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/email.py
--rw-r--r--   0        0        0     1496 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/epub.py
--rw-r--r--   0        0        0     7753 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/etherscan.py
--rw-r--r--   0        0        0     5930 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/evernote.py
--rw-r--r--   0        0        0     1753 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/excel.py
--rw-r--r--   0        0        0     1270 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/facebook_chat.py
--rw-r--r--   0        0        0     2171 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/fauna.py
--rw-r--r--   0        0        0     1543 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/figma.py
--rw-r--r--   0        0        0     2453 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/firecrawl.py
--rw-r--r--   0        0        0     3041 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/gcs_directory.py
--rw-r--r--   0        0        0     3316 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/gcs_file.py
--rw-r--r--   0        0        0     6374 2024-05-17 20:49:58.731865 langchain_community-0.2.0/langchain_community/document_loaders/generic.py
--rw-r--r--   0        0        0     2400 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/geodataframe.py
--rw-r--r--   0        0        0     4018 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/git.py
--rw-r--r--   0        0        0     3451 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/gitbook.py
--rw-r--r--   0        0        0     8676 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/github.py
--rw-r--r--   0        0        0     4459 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/glue_catalog.py
--rw-r--r--   0        0        0     5279 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/google_speech_to_text.py
--rw-r--r--   0        0        0    14435 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/googledrive.py
--rw-r--r--   0        0        0      928 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/gutenberg.py
--rw-r--r--   0        0        0     1640 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/helpers.py
--rw-r--r--   0        0        0     2075 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/hn.py
--rw-r--r--   0        0        0     1158 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/html.py
--rw-r--r--   0        0        0     2098 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/html_bs.py
--rw-r--r--   0        0        0     3095 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/hugging_face_dataset.py
--rw-r--r--   0        0        0     3628 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/hugging_face_model.py
--rw-r--r--   0        0        0     7642 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/ifixit.py
--rw-r--r--   0        0        0     1173 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/image.py
--rw-r--r--   0        0        0     3707 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/image_captions.py
--rw-r--r--   0        0        0      477 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/imsdb.py
--rw-r--r--   0        0        0     1688 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/iugu.py
--rw-r--r--   0        0        0     3628 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/joplin.py
--rw-r--r--   0        0        0     7366 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/json_loader.py
--rw-r--r--   0        0        0     3919 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/kinetica_loader.py
--rw-r--r--   0        0        0     6058 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/lakefs.py
--rw-r--r--   0        0        0     2959 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/larksuite.py
--rw-r--r--   0        0        0     4881 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/llmsherpa.py
--rw-r--r--   0        0        0     1818 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/markdown.py
--rw-r--r--   0        0        0     3079 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/mastodon.py
--rw-r--r--   0        0        0     3199 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/max_compute.py
--rw-r--r--   0        0        0     3859 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/mediawikidump.py
--rw-r--r--   0        0        0      999 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/merge.py
--rw-r--r--   0        0        0     2658 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/mhtml.py
--rw-r--r--   0        0        0     8923 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/mintbase.py
--rw-r--r--   0        0        0     3074 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/modern_treasury.py
--rw-r--r--   0        0        0     3182 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/mongodb.py
--rw-r--r--   0        0        0     4283 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/news.py
--rw-r--r--   0        0        0     4296 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/notebook.py
--rw-r--r--   0        0        0      834 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/notion.py
--rw-r--r--   0        0        0     7715 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/notiondb.py
--rw-r--r--   0        0        0     1102 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/nuclia.py
--rw-r--r--   0        0        0     3593 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/obs_directory.py
--rw-r--r--   0        0        0     4768 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/obs_file.py
--rw-r--r--   0        0        0     6132 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/obsidian.py
--rw-r--r--   0        0        0     1840 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/odt.py
--rw-r--r--   0        0        0     3270 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/onedrive.py
--rw-r--r--   0        0        0     1154 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/onedrive_file.py
--rw-r--r--   0        0        0     7833 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/onenote.py
--rw-r--r--   0        0        0     1219 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/open_city_data.py
--rw-r--r--   0        0        0     4221 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/oracleadb_loader.py
--rw-r--r--   0        0        0    15573 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/oracleai.py
--rw-r--r--   0        0        0     1818 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/org_mode.py
--rw-r--r--   0        0        0     1283 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/__init__.py
--rw-r--r--   0        0        0    16911 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/audio.py
--rw-r--r--   0        0        0     4050 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/doc_intelligence.py
--rw-r--r--   0        0        0    15457 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/docai.py
--rw-r--r--   0        0        0     2502 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/generic.py
--rw-r--r--   0        0        0     5903 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/grobid.py
--rw-r--r--   0        0        0      109 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/html/__init__.py
--rw-r--r--   0        0        0     1608 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/html/bs4.py
--rw-r--r--   0        0        0      136 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/__init__.py
--rw-r--r--   0        0        0      877 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/c.py
--rw-r--r--   0        0        0     3745 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/cobol.py
--rw-r--r--   0        0        0      495 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/code_segmenter.py
--rw-r--r--   0        0        0      893 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/cpp.py
--rw-r--r--   0        0        0      893 2024-05-17 20:49:58.735865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/csharp.py
--rw-r--r--   0        0        0      693 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/go.py
--rw-r--r--   0        0        0      736 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/java.py
--rw-r--r--   0        0        0     2185 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/javascript.py
--rw-r--r--   0        0        0      707 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/kotlin.py
--rw-r--r--   0        0        0     7538 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/language_parser.py
--rw-r--r--   0        0        0      790 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/lua.py
--rw-r--r--   0        0        0      666 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/perl.py
--rw-r--r--   0        0        0      850 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/php.py
--rw-r--r--   0        0        0     1731 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/python.py
--rw-r--r--   0        0        0      697 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/ruby.py
--rw-r--r--   0        0        0      774 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/rust.py
--rw-r--r--   0        0        0      772 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/scala.py
--rw-r--r--   0        0        0     3473 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/tree_sitter_segmenter.py
--rw-r--r--   0        0        0      795 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/typescript.py
--rw-r--r--   0        0        0     1812 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/msword.py
--rw-r--r--   0        0        0    22511 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/pdf.py
--rw-r--r--   0        0        0     1214 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/registry.py
--rw-r--r--   0        0        0      563 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/txt.py
--rw-r--r--   0        0        0     7902 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/parsers/vsdx.py
--rw-r--r--   0        0        0    27775 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/pdf.py
--rw-r--r--   0        0        0    19160 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/pebblo.py
--rw-r--r--   0        0        0     1161 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/polars_dataframe.py
--rw-r--r--   0        0        0     2508 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/powerpoint.py
--rw-r--r--   0        0        0     1315 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/psychic.py
--rw-r--r--   0        0        0     1118 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/pubmed.py
--rw-r--r--   0        0        0     3388 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/pyspark_dataframe.py
--rw-r--r--   0        0        0      590 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/python.py
--rw-r--r--   0        0        0     8426 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/quip.py
--rw-r--r--   0        0        0     6821 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/readthedocs.py
--rw-r--r--   0        0        0    14800 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/recursive_url_loader.py
--rw-r--r--   0        0        0     4584 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/reddit.py
--rw-r--r--   0        0        0      725 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/roam.py
--rw-r--r--   0        0        0     4527 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/rocksetdb.py
--rw-r--r--   0        0        0     4859 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/rspace.py
--rw-r--r--   0        0        0     4882 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/rss.py
--rw-r--r--   0        0        0     1902 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/rst.py
--rw-r--r--   0        0        0     2131 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/rtf.py
--rw-r--r--   0        0        0     5871 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/s3_directory.py
--rw-r--r--   0        0        0     5956 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/s3_file.py
--rw-r--r--   0        0        0     3002 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/sharepoint.py
--rw-r--r--   0        0        0     8524 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/sitemap.py
--rw-r--r--   0        0        0     4027 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/slack_directory.py
--rw-r--r--   0        0        0     4733 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/snowflake_loader.py
--rw-r--r--   0        0        0     3412 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/spider.py
--rw-r--r--   0        0        0     2004 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/spreedly.py
--rw-r--r--   0        0        0     5581 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/sql_database.py
--rw-r--r--   0        0        0      901 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/srt.py
--rw-r--r--   0        0        0     1811 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/stripe.py
--rw-r--r--   0        0        0     2965 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/surrealdb.py
--rw-r--r--   0        0        0     9079 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/telegram.py
--rw-r--r--   0        0        0     1700 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/tencent_cos_directory.py
--rw-r--r--   0        0        0     1617 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/tencent_cos_file.py
--rw-r--r--   0        0        0     2993 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/tensorflow_datasets.py
--rw-r--r--   0        0        0     2070 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/text.py
--rw-r--r--   0        0        0     2610 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/tidb.py
--rw-r--r--   0        0        0      842 2024-05-17 20:49:58.739865 langchain_community-0.2.0/langchain_community/document_loaders/tomarkdown.py
--rw-r--r--   0        0        0     1458 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/toml.py
--rw-r--r--   0        0        0     6584 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/trello.py
--rw-r--r--   0        0        0     1363 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/tsv.py
--rw-r--r--   0        0        0     3438 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/twitter.py
--rw-r--r--   0        0        0    14328 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/unstructured.py
--rw-r--r--   0        0        0     6019 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/url.py
--rw-r--r--   0        0        0     8527 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/url_playwright.py
--rw-r--r--   0        0        0     6640 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/url_selenium.py
--rw-r--r--   0        0        0     1946 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/vsdx.py
--rw-r--r--   0        0        0     1553 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/weather.py
--rw-r--r--   0        0        0    10115 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/web_base.py
--rw-r--r--   0        0        0     1750 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/whatsapp_chat.py
--rw-r--r--   0        0        0     2227 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/wikipedia.py
--rw-r--r--   0        0        0     4633 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/word_document.py
--rw-r--r--   0        0        0     1594 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/xml.py
--rw-r--r--   0        0        0     1119 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/xorbits.py
--rw-r--r--   0        0        0    15500 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/youtube.py
--rw-r--r--   0        0        0     2958 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_loaders/yuque.py
--rw-r--r--   0        0        0     3903 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/__init__.py
--rw-r--r--   0        0        0     6821 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/beautiful_soup_transformer.py
--rw-r--r--   0        0        0     4240 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/doctran_text_extract.py
--rw-r--r--   0        0        0     2155 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/doctran_text_qa.py
--rw-r--r--   0        0        0     2331 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/doctran_text_translate.py
--rw-r--r--   0        0        0     7882 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/embeddings_redundant_filter.py
--rw-r--r--   0        0        0     4309 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/google_translate.py
--rw-r--r--   0        0        0     1834 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/html2text.py
--rw-r--r--   0        0        0     1437 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/long_context_reorder.py
--rw-r--r--   0        0        0     3154 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/markdownify.py
--rw-r--r--   0        0        0     1500 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/nuclia_text_transform.py
--rw-r--r--   0        0        0     6243 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/openai_functions.py
--rw-r--r--   0        0        0     6033 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt
--rw-r--r--   0        0        0    15650 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/__init__.py
--rw-r--r--   0        0        0     9614 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/aleph_alpha.py
--rw-r--r--   0        0        0     2609 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/anyscale.py
--rw-r--r--   0        0        0     1865 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/awa.py
--rw-r--r--   0        0        0     7239 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/azure_openai.py
--rw-r--r--   0        0        0     4583 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/baichuan.py
--rw-r--r--   0        0        0     5201 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     7274 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/bedrock.py
--rw-r--r--   0        0        0     2725 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/bookend.py
--rw-r--r--   0        0        0     4677 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/clarifai.py
--rw-r--r--   0        0        0     2869 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/cloudflare_workersai.py
--rw-r--r--   0        0        0     5514 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/cohere.py
--rw-r--r--   0        0        0     5216 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/dashscope.py
--rw-r--r--   0        0        0     1271 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/databricks.py
--rw-r--r--   0        0        0     5002 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/deepinfra.py
--rw-r--r--   0        0        0     3699 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/edenai.py
--rw-r--r--   0        0        0     8546 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/elasticsearch.py
--rw-r--r--   0        0        0     5528 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/embaas.py
--rw-r--r--   0        0        0     4997 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/ernie.py
--rw-r--r--   0        0        0     1512 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/fake.py
--rw-r--r--   0        0        0     3770 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/fastembed.py
--rw-r--r--   0        0        0     5989 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/gigachat.py
--rw-r--r--   0        0        0     3272 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/google_palm.py
--rw-r--r--   0        0        0     2223 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/gpt4all.py
--rw-r--r--   0        0        0     5306 2024-05-17 20:49:58.743865 langchain_community-0.2.0/langchain_community/embeddings/gradient_ai.py
--rw-r--r--   0        0        0    13675 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/huggingface.py
--rw-r--r--   0        0        0     5078 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/huggingface_hub.py
--rw-r--r--   0        0        0    10290 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/infinity.py
--rw-r--r--   0        0        0     5196 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/infinity_local.py
--rw-r--r--   0        0        0     8168 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/itrex.py
--rw-r--r--   0        0        0     3669 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/javelin_ai_gateway.py
--rw-r--r--   0        0        0     2607 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/jina.py
--rw-r--r--   0        0        0     2873 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/johnsnowlabs.py
--rw-r--r--   0        0        0     3064 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/laser.py
--rw-r--r--   0        0        0     4157 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/llamacpp.py
--rw-r--r--   0        0        0     4009 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/llamafile.py
--rw-r--r--   0        0        0     2321 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/llm_rails.py
--rw-r--r--   0        0        0    12261 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/localai.py
--rw-r--r--   0        0        0     4826 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/minimax.py
--rw-r--r--   0        0        0     3047 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/mlflow.py
--rw-r--r--   0        0        0     2447 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/mlflow_gateway.py
--rw-r--r--   0        0        0     2384 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/modelscope_hub.py
--rw-r--r--   0        0        0     5115 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/mosaicml.py
--rw-r--r--   0        0        0     5753 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/nemo.py
--rw-r--r--   0        0        0     2203 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/nlpcloud.py
--rw-r--r--   0        0        0     7015 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/oci_generative_ai.py
--rw-r--r--   0        0        0     3799 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/octoai_embeddings.py
--rw-r--r--   0        0        0     7953 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/ollama.py
--rw-r--r--   0        0        0    29239 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/openai.py
--rw-r--r--   0        0        0    12346 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/openvino.py
--rw-r--r--   0        0        0     7663 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/optimum_intel.py
--rw-r--r--   0        0        0     5208 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/oracleai.py
--rw-r--r--   0        0        0     4481 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/premai.py
--rw-r--r--   0        0        0     7596 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/sagemaker_endpoint.py
--rw-r--r--   0        0        0     5251 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/sambanova.py
--rw-r--r--   0        0        0     3807 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/self_hosted.py
--rw-r--r--   0        0        0     6583 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/self_hosted_hugging_face.py
--rw-r--r--   0        0        0      189 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/sentence_transformer.py
--rw-r--r--   0        0        0     4282 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/solar.py
--rw-r--r--   0        0        0     3955 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/spacy_embeddings.py
--rw-r--r--   0        0        0     6967 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/sparkllm.py
--rw-r--r--   0        0        0     2413 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/tensorflow_hub.py
--rw-r--r--   0        0        0     2364 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/text2vec.py
--rw-r--r--   0        0        0     7685 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/titan_takeoff.py
--rw-r--r--   0        0        0    14681 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/vertexai.py
--rw-r--r--   0        0        0     4198 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/volcengine.py
--rw-r--r--   0        0        0     7487 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/voyageai.py
--rw-r--r--   0        0        0     3303 2024-05-17 20:49:58.747865 langchain_community-0.2.0/langchain_community/embeddings/xinference.py
--rw-r--r--   0        0        0     8005 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/embeddings/yandex.py
--rw-r--r--   0        0        0      608 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/example_selectors/__init__.py
--rw-r--r--   0        0        0     3842 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/example_selectors/ngram_overlap.py
--rw-r--r--   0        0        0     3024 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/__init__.py
--rw-r--r--   0        0        0    26675 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/age_graph.py
--rw-r--r--   0        0        0     6961 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/arangodb_graph.py
--rw-r--r--   0        0        0     6951 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/falkordb_graph.py
--rw-r--r--   0        0        0     1584 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/graph_document.py
--rw-r--r--   0        0        0      993 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/graph_store.py
--rw-r--r--   0        0        0     8189 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/gremlin_graph.py
--rw-r--r--   0        0        0     2511 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/hugegraph.py
--rw-r--r--   0        0        0     3970 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/index_creator.py
--rw-r--r--   0        0        0     3918 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/kuzu_graph.py
--rw-r--r--   0        0        0     2575 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/memgraph_graph.py
--rw-r--r--   0        0        0     8113 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/nebula_graph.py
--rw-r--r--   0        0        0    29853 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/neo4j_graph.py
--rw-r--r--   0        0        0    14357 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/neptune_graph.py
--rw-r--r--   0        0        0    10315 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/neptune_rdf_graph.py
--rw-r--r--   0        0        0     7896 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/networkx_graph.py
--rw-r--r--   0        0        0     7646 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/ontotext_graphdb_graph.py
--rw-r--r--   0        0        0    10577 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/rdf_graph.py
--rw-r--r--   0        0        0     3543 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/graphs/tigergraph_graph.py
--rw-r--r--   0        0        0      488 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/indexes/__init__.py
--rw-r--r--   0        0        0     8199 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/indexes/_document_manager.py
--rw-r--r--   0        0        0    21089 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0     5191 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/indexes/base.py
--rw-r--r--   0        0        0    27750 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/__init__.py
--rw-r--r--   0        0        0     5292 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/ai21.py
--rw-r--r--   0        0        0    11540 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/aleph_alpha.py
--rw-r--r--   0        0        0     3061 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/amazon_api_gateway.py
--rw-r--r--   0        0        0    12760 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/anthropic.py
--rw-r--r--   0        0        0    11930 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/anyscale.py
--rw-r--r--   0        0        0     9619 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/aphrodite.py
--rw-r--r--   0        0        0     4356 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/arcee.py
--rw-r--r--   0        0        0     6007 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/aviary.py
--rw-r--r--   0        0        0    20617 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/azureml_endpoint.py
--rw-r--r--   0        0        0     3051 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/baichuan.py
--rw-r--r--   0        0        0     7729 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/baidu_qianfan_endpoint.py
--rw-r--r--   0        0        0     4830 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/bananadev.py
--rw-r--r--   0        0        0     3187 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/baseten.py
--rw-r--r--   0        0        0     9113 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/beam.py
--rw-r--r--   0        0        0    31549 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/bedrock.py
--rw-r--r--   0        0        0     5515 2024-05-17 20:49:58.751865 langchain_community-0.2.0/langchain_community/llms/bigdl_llm.py
--rw-r--r--   0        0        0     6232 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/bittensor.py
--rw-r--r--   0        0        0     4044 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/cerebriumai.py
--rw-r--r--   0        0        0     3950 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/chatglm.py
--rw-r--r--   0        0        0     4884 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/chatglm3.py
--rw-r--r--   0        0        0     6578 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/clarifai.py
--rw-r--r--   0        0        0     4239 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/cloudflare_workersai.py
--rw-r--r--   0        0        0     8709 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/cohere.py
--rw-r--r--   0        0        0     4241 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/ctransformers.py
--rw-r--r--   0        0        0     4135 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/ctranslate2.py
--rw-r--r--   0        0        0    20535 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/databricks.py
--rw-r--r--   0        0        0     7006 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/deepinfra.py
--rw-r--r--   0        0        0     8657 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/deepsparse.py
--rw-r--r--   0        0        0     9448 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/edenai.py
--rw-r--r--   0        0        0     6459 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/exllamav2.py
--rw-r--r--   0        0        0     2444 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/fake.py
--rw-r--r--   0        0        0    11938 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/fireworks.py
--rw-r--r--   0        0        0     3762 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/forefrontai.py
--rw-r--r--   0        0        0    14570 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/friendli.py
--rw-r--r--   0        0        0    11659 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/gigachat.py
--rw-r--r--   0        0        0     8860 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/google_palm.py
--rw-r--r--   0        0        0     5301 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/gooseai.py
--rw-r--r--   0        0        0     6605 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/gpt4all.py
--rw-r--r--   0        0        0    14199 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/gradient_ai.py
--rw-r--r--   0        0        0      664 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/grammars/json.gbnf
--rw-r--r--   0        0        0      167 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/grammars/list.gbnf
--rw-r--r--   0        0        0    14634 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/huggingface_endpoint.py
--rw-r--r--   0        0        0     5382 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/huggingface_hub.py
--rw-r--r--   0        0        0    11127 2024-05-17 20:49:58.755865 langchain_community-0.2.0/langchain_community/llms/huggingface_pipeline.py
--rw-r--r--   0        0        0    11653 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/huggingface_text_gen_inference.py
--rw-r--r--   0        0        0     2575 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/human.py
--rw-r--r--   0        0        0     9521 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/ipex_llm.py
--rw-r--r--   0        0        0     4723 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/javelin_ai_gateway.py
--rw-r--r--   0        0        0     5094 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/koboldai.py
--rw-r--r--   0        0        0     6554 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/konko.py
--rw-r--r--   0        0        0     3477 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/layerup_security.py
--rw-r--r--   0        0        0    12476 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/llamacpp.py
--rw-r--r--   0        0        0    10422 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/llamafile.py
--rw-r--r--   0        0        0     1709 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/loading.py
--rw-r--r--   0        0        0     1965 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/manifest.py
--rw-r--r--   0        0        0     5471 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/minimax.py
--rw-r--r--   0        0        0     3431 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/mlflow.py
--rw-r--r--   0        0        0     3240 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/mlflow_ai_gateway.py
--rw-r--r--   0        0        0     6254 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/mlx_pipeline.py
--rw-r--r--   0        0        0     3288 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/modal.py
--rw-r--r--   0        0        0     4619 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/moonshot.py
--rw-r--r--   0        0        0     6157 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/mosaicml.py
--rw-r--r--   0        0        0     5053 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/nlpcloud.py
--rw-r--r--   0        0        0    12182 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/oci_data_science_model_deployment_endpoint.py
--rw-r--r--   0        0        0     9398 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/oci_generative_ai.py
--rw-r--r--   0        0        0     3909 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/octoai_endpoint.py
--rw-r--r--   0        0        0    17623 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/ollama.py
--rw-r--r--   0        0        0     4110 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/opaqueprompts.py
--rw-r--r--   0        0        0    47742 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/openai.py
--rw-r--r--   0        0        0    11062 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/openllm.py
--rw-r--r--   0        0        0      902 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/openlm.py
--rw-r--r--   0        0        0     8059 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/pai_eas_endpoint.py
--rw-r--r--   0        0        0     5402 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/petals.py
--rw-r--r--   0        0        0     4210 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/pipelineai.py
--rw-r--r--   0        0        0     8403 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/predibase.py
--rw-r--r--   0        0        0     4417 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/predictionguard.py
--rw-r--r--   0        0        0     8806 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/promptlayer_openai.py
--rw-r--r--   0        0        0     8392 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/replicate.py
--rw-r--r--   0        0        0     7401 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/rwkv.py
--rw-r--r--   0        0        0    13165 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0    30454 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/sambanova.py
--rw-r--r--   0        0        0     8477 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/self_hosted.py
--rw-r--r--   0        0        0     7744 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/self_hosted_hugging_face.py
--rw-r--r--   0        0        0     4107 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/solar.py
--rw-r--r--   0        0        0    12601 2024-05-17 20:49:58.759865 langchain_community-0.2.0/langchain_community/llms/sparkllm.py
--rw-r--r--   0        0        0     4776 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/stochasticai.py
--rw-r--r--   0        0        0     7552 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/symblai_nebula.py
--rw-r--r--   0        0        0    14379 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/textgen.py
--rw-r--r--   0        0        0     9307 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/titan_takeoff.py
--rw-r--r--   0        0        0     7680 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/together.py
--rw-r--r--   0        0        0    13156 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/tongyi.py
--rw-r--r--   0        0        0      258 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/utils.py
--rw-r--r--   0        0        0    19330 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/vertexai.py
--rw-r--r--   0        0        0     5592 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/vllm.py
--rw-r--r--   0        0        0     6591 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/volcengine_maas.py
--rw-r--r--   0        0        0    15085 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/watsonxllm.py
--rw-r--r--   0        0        0     8924 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/weight_only_quantization.py
--rw-r--r--   0        0        0     4970 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/writer.py
--rw-r--r--   0        0        0     6358 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/xinference.py
--rw-r--r--   0        0        0    13008 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/yandex.py
--rw-r--r--   0        0        0     5968 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/llms/yuan2.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/memory/__init__.py
--rw-r--r--   0        0        0     5632 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/memory/kg.py
--rw-r--r--   0        0        0     3600 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/memory/motorhead_memory.py
--rw-r--r--   0        0        0     5623 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/memory/zep_memory.py
--rw-r--r--   0        0        0      292 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/output_parsers/__init__.py
--rw-r--r--   0        0        0     6701 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/output_parsers/ernie_functions.py
--rw-r--r--   0        0        0     3283 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/output_parsers/rail_parser.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/py.typed
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/astradb.py
--rw-r--r--   0        0        0     1468 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/chroma.py
--rw-r--r--   0        0        0     1912 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/dashvector.py
--rw-r--r--   0        0        0     3144 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/databricks_vector_search.py
--rw-r--r--   0        0        0     2625 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/deeplake.py
--rw-r--r--   0        0        0     1343 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/dingo.py
--rw-r--r--   0        0        0     3267 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/elasticsearch.py
--rw-r--r--   0        0        0     3346 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/milvus.py
--rw-r--r--   0        0        0     2297 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/mongodb_atlas.py
--rw-r--r--   0        0        0     3630 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/myscale.py
--rw-r--r--   0        0        0     3265 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/opensearch.py
--rw-r--r--   0        0        0     1523 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/pgvector.py
--rw-r--r--   0        0        0     1704 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/pinecone.py
--rw-r--r--   0        0        0     3162 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/qdrant.py
--rw-r--r--   0        0        0     3370 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/redis.py
--rw-r--r--   0        0        0     2968 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/supabase.py
--rw-r--r--   0        0        0     3703 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/tencentvectordb.py
--rw-r--r--   0        0        0     2627 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/timescalevector.py
--rw-r--r--   0        0        0     2158 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/vectara.py
--rw-r--r--   0        0        0     2613 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/query_constructors/weaviate.py
--rw-r--r--   0        0        0     9161 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/__init__.py
--rw-r--r--   0        0        0     4297 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/arcee.py
--rw-r--r--   0        0        0      773 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/arxiv.py
--rw-r--r--   0        0        0     5098 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/azure_ai_search.py
--rw-r--r--   0        0        0     4766 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/bedrock.py
--rw-r--r--   0        0        0     3713 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/bm25.py
--rw-r--r--   0        0        0     1550 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/breebs.py
--rw-r--r--   0        0        0     2684 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/chaindesk.py
--rw-r--r--   0        0        0     3024 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/chatgpt_plugin_retriever.py
--rw-r--r--   0        0        0     3088 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/cohere_rag_retriever.py
--rw-r--r--   0        0        0     2338 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/databerry.py
--rw-r--r--   0        0        0     6778 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/docarray.py
--rw-r--r--   0        0        0     2789 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/dria_index.py
--rw-r--r--   0        0        0     4640 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/elastic_search_bm25.py
--rw-r--r--   0        0        0     2087 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/embedchain.py
--rw-r--r--   0        0        0     4763 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/google_cloud_documentai_warehouse.py
--rw-r--r--   0        0        0    18798 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/google_vertex_ai_search.py
--rw-r--r--   0        0        0     1985 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/kay.py
--rw-r--r--   0        0        0    15685 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/kendra.py
--rw-r--r--   0        0        0     3323 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/knn.py
--rw-r--r--   0        0        0     3166 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/llama_index.py
--rw-r--r--   0        0        0     1486 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/metal.py
--rw-r--r--   0        0        0     2523 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/milvus.py
--rw-r--r--   0        0        0      644 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/outline.py
--rw-r--r--   0        0        0     5733 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/pinecone_hybrid_search.py
--rw-r--r--   0        0        0      643 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/pubmed.py
--rw-r--r--   0        0        0      104 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/pupmed.py
--rw-r--r--   0        0        0     7539 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/qdrant_sparse_vector_retriever.py
--rw-r--r--   0        0        0      670 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/rememberizer.py
--rw-r--r--   0        0        0     1935 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/remote_retriever.py
--rw-r--r--   0        0        0     4131 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/svm.py
--rw-r--r--   0        0        0     2855 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/tavily_search_api.py
--rw-r--r--   0        0        0     5569 2024-05-17 20:49:58.763865 langchain_community-0.2.0/langchain_community/retrievers/tfidf.py
--rw-r--r--   0        0        0     9340 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/thirdai_neuraldb.py
--rw-r--r--   0        0        0     4555 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/vespa_retriever.py
--rw-r--r--   0        0        0     6195 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/weaviate_hybrid_search.py
--rw-r--r--   0        0        0     8197 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/web_research.py
--rw-r--r--   0        0        0      656 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/wikipedia.py
--rw-r--r--   0        0        0     1124 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/you.py
--rw-r--r--   0        0        0     5904 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/zep.py
--rw-r--r--   0        0        0     2719 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/retrievers/zilliz.py
--rw-r--r--   0        0        0     1643 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/storage/__init__.py
--rw-r--r--   0        0        0     8691 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/storage/astradb.py
--rw-r--r--   0        0        0       89 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/storage/exceptions.py
--rw-r--r--   0        0        0     4375 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/storage/mongodb.py
--rw-r--r--   0        0        0     4802 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/storage/redis.py
--rw-r--r--   0        0        0     5762 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/storage/upstash_redis.py
--rw-r--r--   0        0        0    23154 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/__init__.py
--rw-r--r--   0        0        0     3185 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/app.py
--rw-r--r--   0        0        0     2109 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/base.py
--rw-r--r--   0        0        0     4140 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/owner.py
--rw-r--r--   0        0        0     2746 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/rule.py
--rw-r--r--   0        0        0     1074 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/transfer.py
--rw-r--r--   0        0        0     2314 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/utils.py
--rw-r--r--   0        0        0     2624 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ainetwork/value.py
--rw-r--r--   0        0        0      257 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/amadeus/__init__.py
--rw-r--r--   0        0        0      435 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/amadeus/base.py
--rw-r--r--   0        0        0     2338 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/amadeus/closest_airport.py
--rw-r--r--   0        0        0     5771 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/amadeus/flight_search.py
--rw-r--r--   0        0        0     1276 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/amadeus/utils.py
--rw-r--r--   0        0        0       25 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/arxiv/__init__.py
--rw-r--r--   0        0        0     1254 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/arxiv/tool.py
--rw-r--r--   0        0        0      188 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/audio/__init__.py
--rw-r--r--   0        0        0     3750 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/audio/huggingface_text_to_speech_inference.py
--rw-r--r--   0        0        0      858 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_ai_services/__init__.py
--rw-r--r--   0        0        0     5486 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_ai_services/document_intelligence.py
--rw-r--r--   0        0        0     5735 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_ai_services/image_analysis.py
--rw-r--r--   0        0        0     4430 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_ai_services/speech_to_text.py
--rw-r--r--   0        0        0     3601 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_ai_services/text_analytics_for_health.py
--rw-r--r--   0        0        0     3811 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_ai_services/text_to_speech.py
--rw-r--r--   0        0        0      776 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_ai_services/utils.py
--rw-r--r--   0        0        0      802 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/__init__.py
--rw-r--r--   0        0        0     5375 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/form_recognizer.py
--rw-r--r--   0        0        0     5304 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/image_analysis.py
--rw-r--r--   0        0        0     4336 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/speech2text.py
--rw-r--r--   0        0        0     3675 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/text2speech.py
--rw-r--r--   0        0        0     3542 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/text_analytics_health.py
--rw-r--r--   0        0        0      776 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/utils.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/bearly/__init__.py
--rw-r--r--   0        0        0     5562 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/bearly/tool.py
--rw-r--r--   0        0        0      170 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/bing_search/__init__.py
--rw-r--r--   0        0        0     1463 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/bing_search/tool.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/brave_search/__init__.py
--rw-r--r--   0        0        0     1354 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/brave_search/tool.py
--rw-r--r--   0        0        0       23 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/cassandra_database/__init__.py
--rw-r--r--   0        0        0     1221 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/cassandra_database/prompt.py
--rw-r--r--   0        0        0     4924 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/cassandra_database/tool.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/clickup/__init__.py
--rw-r--r--   0        0        0     8298 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/clickup/prompt.py
--rw-r--r--   0        0        0     1230 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/clickup/tool.py
--rw-r--r--   0        0        0       20 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/cogniswitch/__init__.py
--rw-r--r--   0        0        0    13896 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/cogniswitch/tool.py
--rw-r--r--   0        0        0      188 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/connery/__init__.py
--rw-r--r--   0        0        0      647 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/connery/models.py
--rw-r--r--   0        0        0     5741 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/connery/service.py
--rw-r--r--   0        0        0     5552 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/connery/tool.py
--rw-r--r--   0        0        0      198 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/convert_to_openai.py
--rw-r--r--   0        0        0      268 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/dataforseo_api_search/__init__.py
--rw-r--r--   0        0        0     2214 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/dataforseo_api_search/tool.py
--rw-r--r--   0        0        0      148 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/dataherald/__init__.py
--rw-r--r--   0        0        0     1063 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/dataherald/tool.py
--rw-r--r--   0        0        0      147 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ddg_search/__init__.py
--rw-r--r--   0        0        0     2641 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/ddg_search/tool.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.767865 langchain_community-0.2.0/langchain_community/tools/e2b_data_analysis/__init__.py
--rw-r--r--   0        0        0     8015 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/e2b_data_analysis/tool.py
--rw-r--r--   0        0        0    20667 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/e2b_data_analysis/unparse.py
--rw-r--r--   0        0        0     1024 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/__init__.py
--rw-r--r--   0        0        0     3465 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/audio_speech_to_text.py
--rw-r--r--   0        0        0     3885 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/audio_text_to_speech.py
--rw-r--r--   0        0        0     5386 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/edenai_base_tool.py
--rw-r--r--   0        0        0     2249 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/image_explicitcontent.py
--rw-r--r--   0        0        0     2476 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/image_objectdetection.py
--rw-r--r--   0        0        0     1966 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/ocr_identityparser.py
--rw-r--r--   0        0        0     2187 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/ocr_invoiceparser.py
--rw-r--r--   0        0        0     2407 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/edenai/text_moderation.py
--rw-r--r--   0        0        0      164 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/eleven_labs/__init__.py
--rw-r--r--   0        0        0      203 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/eleven_labs/models.py
--rw-r--r--   0        0        0     2709 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/eleven_labs/text2speech.py
--rw-r--r--   0        0        0      723 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/__init__.py
--rw-r--r--   0        0        0     1749 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/copy.py
--rw-r--r--   0        0        0     1345 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/delete.py
--rw-r--r--   0        0        0     1965 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/file_search.py
--rw-r--r--   0        0        0     1432 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/list_dir.py
--rw-r--r--   0        0        0     1889 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/move.py
--rw-r--r--   0        0        0     1340 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/read.py
--rw-r--r--   0        0        0     1726 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/utils.py
--rw-r--r--   0        0        0     1614 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/file_management/write.py
--rw-r--r--   0        0        0       20 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/github/__init__.py
--rw-r--r--   0        0        0     6220 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/github/prompt.py
--rw-r--r--   0        0        0     1220 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/github/tool.py
--rw-r--r--   0        0        0       20 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gitlab/__init__.py
--rw-r--r--   0        0        0     3438 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gitlab/prompt.py
--rw-r--r--   0        0        0      998 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gitlab/tool.py
--rw-r--r--   0        0        0      601 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/base.py
--rw-r--r--   0        0        0     2564 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/create_draft.py
--rw-r--r--   0        0        0     2258 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/get_message.py
--rw-r--r--   0        0        0     1560 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/get_thread.py
--rw-r--r--   0        0        0     5195 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/search.py
--rw-r--r--   0        0        0     2939 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/send_message.py
--rw-r--r--   0        0        0     4109 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/gmail/utils.py
--rw-r--r--   0        0        0      136 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/golden_query/__init__.py
--rw-r--r--   0        0        0     1108 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/golden_query/tool.py
--rw-r--r--   0        0        0      171 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_cloud/__init__.py
--rw-r--r--   0        0        0     3354 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_cloud/texttospeech.py
--rw-r--r--   0        0        0      152 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_finance/__init__.py
--rw-r--r--   0        0        0      854 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_finance/tool.py
--rw-r--r--   0        0        0      140 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_jobs/__init__.py
--rw-r--r--   0        0        0      826 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_jobs/tool.py
--rw-r--r--   0        0        0      140 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_lens/__init__.py
--rw-r--r--   0        0        0      822 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_lens/tool.py
--rw-r--r--   0        0        0      140 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_places/__init__.py
--rw-r--r--   0        0        0     1348 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_places/tool.py
--rw-r--r--   0        0        0      152 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_scholar/__init__.py
--rw-r--r--   0        0        0      847 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_scholar/tool.py
--rw-r--r--   0        0        0      195 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_search/__init__.py
--rw-r--r--   0        0        0     1798 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_search/tool.py
--rw-r--r--   0        0        0      243 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_serper/__init__.py
--rw-r--r--   0        0        0     2113 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_serper/tool.py
--rw-r--r--   0        0        0      148 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_trends/__init__.py
--rw-r--r--   0        0        0      844 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/google_trends/tool.py
--rw-r--r--   0        0        0       47 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/graphql/__init__.py
--rw-r--r--   0        0        0     1204 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/graphql/tool.py
--rw-r--r--   0        0        0      132 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/human/__init__.py
--rw-r--r--   0        0        0     1011 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/human/tool.py
--rw-r--r--   0        0        0     2286 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/ifttt.py
--rw-r--r--   0        0        0       43 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/interaction/__init__.py
--rw-r--r--   0        0        0      464 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/interaction/tool.py
--rw-r--r--   0        0        0       17 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/jira/__init__.py
--rw-r--r--   0        0        0     3170 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/jira/prompt.py
--rw-r--r--   0        0        0     1368 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/jira/tool.py
--rw-r--r--   0        0        0       46 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/json/__init__.py
--rw-r--r--   0        0        0     4139 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/json/tool.py
--rw-r--r--   0        0        0      134 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/memorize/__init__.py
--rw-r--r--   0        0        0     1828 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/memorize/tool.py
--rw-r--r--   0        0        0       35 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/merriam_webster/__init__.py
--rw-r--r--   0        0        0      854 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/merriam_webster/tool.py
--rw-r--r--   0        0        0      154 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/metaphor_search/__init__.py
--rw-r--r--   0        0        0     2851 2024-05-17 20:49:58.771865 langchain_community-0.2.0/langchain_community/tools/metaphor_search/tool.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/mojeek_search/__init__.py
--rw-r--r--   0        0        0     1307 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/mojeek_search/tool.py
--rw-r--r--   0        0        0      359 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/multion/__init__.py
--rw-r--r--   0        0        0     1765 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/multion/close_session.py
--rw-r--r--   0        0        0     2199 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/multion/create_session.py
--rw-r--r--   0        0        0     2415 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/multion/update_session.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/nasa/__init__.py
--rw-r--r--   0        0        0     5197 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/nasa/prompt.py
--rw-r--r--   0        0        0      831 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/nasa/tool.py
--rw-r--r--   0        0        0      111 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/nuclia/__init__.py
--rw-r--r--   0        0        0     7941 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/nuclia/tool.py
--rw-r--r--   0        0        0      654 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/__init__.py
--rw-r--r--   0        0        0      508 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/base.py
--rw-r--r--   0        0        0     1858 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/create_draft_message.py
--rw-r--r--   0        0        0     4821 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/events_search.py
--rw-r--r--   0        0        0     4235 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/messages_search.py
--rw-r--r--   0        0        0     2898 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/send_event.py
--rw-r--r--   0        0        0     1777 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/send_message.py
--rw-r--r--   0        0        0     2228 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/office365/utils.py
--rw-r--r--   0        0        0      219 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openai_dalle_image_generation/__init__.py
--rw-r--r--   0        0        0      953 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openai_dalle_image_generation/tool.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openapi/__init__.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openapi/utils/__init__.py
--rw-r--r--   0        0        0    21314 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openapi/utils/api_models.py
--rw-r--r--   0        0        0      191 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openapi/utils/openapi_utils.py
--rw-r--r--   0        0        0      162 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openweathermap/__init__.py
--rw-r--r--   0        0        0      994 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/openweathermap/tool.py
--rw-r--r--   0        0        0      142 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/passio_nutrition_ai/__init__.py
--rw-r--r--   0        0        0     1143 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/passio_nutrition_ai/tool.py
--rw-r--r--   0        0        0      763 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/__init__.py
--rw-r--r--   0        0        0     1950 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/base.py
--rw-r--r--   0        0        0     3083 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/click.py
--rw-r--r--   0        0        0     1340 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/current_page.py
--rw-r--r--   0        0        0     3051 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/extract_hyperlinks.py
--rw-r--r--   0        0        0     2383 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/extract_text.py
--rw-r--r--   0        0        0     3743 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/get_elements.py
--rw-r--r--   0        0        0     2878 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/navigate.py
--rw-r--r--   0        0        0     1926 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/navigate_back.py
--rw-r--r--   0        0        0     3049 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/playwright/utils.py
--rw-r--r--   0        0        0     2902 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/plugin.py
--rw-r--r--   0        0        0      439 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/polygon/__init__.py
--rw-r--r--   0        0        0     2558 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/polygon/aggregates.py
--rw-r--r--   0        0        0     1197 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/polygon/financials.py
--rw-r--r--   0        0        0     1070 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/polygon/last_quote.py
--rw-r--r--   0        0        0     1076 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/polygon/ticker_news.py
--rw-r--r--   0        0        0       52 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/powerbi/__init__.py
--rw-r--r--   0        0        0     7339 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/powerbi/prompt.py
--rw-r--r--   0        0        0    11075 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/powerbi/tool.py
--rw-r--r--   0        0        0       26 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/pubmed/__init__.py
--rw-r--r--   0        0        0      971 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/pubmed/tool.py
--rw-r--r--   0        0        0     1991 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/reddit_search/tool.py
--rw-r--r--   0        0        0      198 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/render.py
--rw-r--r--   0        0        0       52 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/requests/__init__.py
--rw-r--r--   0        0        0     7445 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/requests/tool.py
--rw-r--r--   0        0        0       31 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/scenexplain/__init__.py
--rw-r--r--   0        0        0     1126 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/scenexplain/tool.py
--rw-r--r--   0        0        0      214 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/searchapi/__init__.py
--rw-r--r--   0        0        0     2114 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/searchapi/tool.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/searx_search/__init__.py
--rw-r--r--   0        0        0     2261 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/searx_search/tool.py
--rw-r--r--   0        0        0       36 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/semanticscholar/__init__.py
--rw-r--r--   0        0        0     1216 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/semanticscholar/tool.py
--rw-r--r--   0        0        0      103 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/shell/__init__.py
--rw-r--r--   0        0        0     3143 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/shell/tool.py
--rw-r--r--   0        0        0      502 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/slack/__init__.py
--rw-r--r--   0        0        0      460 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/slack/base.py
--rw-r--r--   0        0        0     1193 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/slack/get_channel.py
--rw-r--r--   0        0        0     1422 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/slack/get_message.py
--rw-r--r--   0        0        0     2071 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/slack/schedule_message.py
--rw-r--r--   0        0        0     1222 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/slack/send_message.py
--rw-r--r--   0        0        0     1135 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/slack/utils.py
--rw-r--r--   0        0        0       18 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/sleep/__init__.py
--rw-r--r--   0        0        0     1229 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/sleep/tool.py
--rw-r--r--   0        0        0       44 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/spark_sql/__init__.py
--rw-r--r--   0        0        0      550 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/spark_sql/prompt.py
--rw-r--r--   0        0        0     4402 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/spark_sql/tool.py
--rw-r--r--   0        0        0       49 2024-05-17 20:49:58.775864 langchain_community-0.2.0/langchain_community/tools/sql_database/__init__.py
--rw-r--r--   0        0        0      597 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/sql_database/prompt.py
--rw-r--r--   0        0        0     5352 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/sql_database/tool.py
--rw-r--r--   0        0        0       33 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/stackexchange/__init__.py
--rw-r--r--   0        0        0      869 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/stackexchange/tool.py
--rw-r--r--   0        0        0       24 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/steam/__init__.py
--rw-r--r--   0        0        0     1657 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/steam/prompt.py
--rw-r--r--   0        0        0      842 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/steam/tool.py
--rw-r--r--   0        0        0      186 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/steamship_image_generation/__init__.py
--rw-r--r--   0        0        0     3378 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/steamship_image_generation/tool.py
--rw-r--r--   0        0        0     1395 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/steamship_image_generation/utils.py
--rw-r--r--   0        0        0      189 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/tavily_search/__init__.py
--rw-r--r--   0        0        0     3427 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/tavily_search/tool.py
--rw-r--r--   0        0        0       51 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/vectorstore/__init__.py
--rw-r--r--   0        0        0     4717 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/vectorstore/tool.py
--rw-r--r--   0        0        0       28 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/wikidata/__init__.py
--rw-r--r--   0        0        0      926 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/wikidata/tool.py
--rw-r--r--   0        0        0       29 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/wikipedia/__init__.py
--rw-r--r--   0        0        0      867 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/wikipedia/tool.py
--rw-r--r--   0        0        0      156 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/wolfram_alpha/__init__.py
--rw-r--r--   0        0        0      887 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/wolfram_alpha/tool.py
--rw-r--r--   0        0        0     2753 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/yahoo_finance_news.py
--rw-r--r--   0        0        0      126 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/you/__init__.py
--rw-r--r--   0        0        0     1355 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/you/tool.py
--rw-r--r--   0        0        0        0 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/youtube/__init__.py
--rw-r--r--   0        0        0     1729 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/youtube/search.py
--rw-r--r--   0        0        0      193 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/zapier/__init__.py
--rw-r--r--   0        0        0     1182 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/zapier/prompt.py
--rw-r--r--   0        0        0     7864 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/tools/zapier/tool.py
--rw-r--r--   0        0        0    11061 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/__init__.py
--rw-r--r--   0        0        0     5918 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/alpha_vantage.py
--rw-r--r--   0        0        0      844 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/anthropic.py
--rw-r--r--   0        0        0     8458 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/apify.py
--rw-r--r--   0        0        0     8710 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/arcee.py
--rw-r--r--   0        0        0    10021 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/arxiv.py
--rw-r--r--   0        0        0     6104 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/astradb.py
--rw-r--r--   0        0        0     2437 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/awslambda.py
--rw-r--r--   0        0        0     2499 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/bibtex.py
--rw-r--r--   0        0        0     3294 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/bing_search.py
--rw-r--r--   0        0        0     2382 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/brave_search.py
--rw-r--r--   0        0        0     1164 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/cassandra.py
--rw-r--r--   0        0        0    24429 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/cassandra_database.py
--rw-r--r--   0        0        0    19876 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/clickup.py
--rw-r--r--   0        0        0     6377 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/dalle_image_generator.py
--rw-r--r--   0        0        0     7854 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/dataforseo_api_search.py
--rw-r--r--   0        0        0     2067 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/dataherald.py
--rw-r--r--   0        0        0     3351 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/dria_index.py
--rw-r--r--   0        0        0     4310 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/duckduckgo_search.py
--rw-r--r--   0        0        0    32246 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/github.py
--rw-r--r--   0        0        0    11975 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/gitlab.py
--rw-r--r--   0        0        0     1858 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/golden_query.py
--rw-r--r--   0        0        0     3400 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_finance.py
--rw-r--r--   0        0        0     2804 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_jobs.py
--rw-r--r--   0        0        0     3017 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_lens.py
--rw-r--r--   0        0        0     4293 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_places_api.py
--rw-r--r--   0        0        0     5171 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_scholar.py
--rw-r--r--   0        0        0     5236 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_search.py
--rw-r--r--   0        0        0     6503 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_serper.py
--rw-r--r--   0        0        0     4164 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/google_trends.py
--rw-r--r--   0        0        0     2089 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/graphql.py
--rw-r--r--   0        0        0     5891 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/infobip.py
--rw-r--r--   0        0        0     6195 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/jira.py
--rw-r--r--   0        0        0     2647 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/max_compute.py
--rw-r--r--   0        0        0     3748 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/merriam_webster.py
--rw-r--r--   0        0        0     6809 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/metaphor_search.py
--rw-r--r--   0        0        0     1319 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/mojeek_search.py
--rw-r--r--   0        0        0     1820 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/nasa.py
--rw-r--r--   0        0        0    21608 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/nvidia_riva.py
--rw-r--r--   0        0        0     3287 2024-05-17 20:49:58.779864 langchain_community-0.2.0/langchain_community/utilities/opaqueprompts.py
--rw-r--r--   0        0        0    11017 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/openapi.py
--rw-r--r--   0        0        0     2462 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/openweathermap.py
--rw-r--r--   0        0        0     6224 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/oracleai.py
--rw-r--r--   0        0        0     3351 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/outline.py
--rw-r--r--   0        0        0     5613 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/passio_nutrition_ai.py
--rw-r--r--   0        0        0     8856 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/pebblo.py
--rw-r--r--   0        0        0     4309 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/polygon.py
--rw-r--r--   0        0        0     2355 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/portkey.py
--rw-r--r--   0        0        0    11245 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/powerbi.py
--rw-r--r--   0        0        0     6950 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/pubmed.py
--rw-r--r--   0        0        0     2159 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/python.py
--rw-r--r--   0        0        0     4474 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/reddit_search.py
--rw-r--r--   0        0        0     8251 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/redis.py
--rw-r--r--   0        0        0     1650 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/rememberizer.py
--rw-r--r--   0        0        0     8793 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/requests.py
--rw-r--r--   0        0        0     2220 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/scenexplain.py
--rw-r--r--   0        0        0     5226 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/searchapi.py
--rw-r--r--   0        0        0    16653 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/searx_search.py
--rw-r--r--   0        0        0     2789 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/semanticscholar.py
--rw-r--r--   0        0        0     8704 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/serpapi.py
--rw-r--r--   0        0        0     7520 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/spark_sql.py
--rw-r--r--   0        0        0    22814 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/sql_database.py
--rw-r--r--   0        0        0     2639 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/stackexchange.py
--rw-r--r--   0        0        0     5857 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/steam.py
--rw-r--r--   0        0        0     6889 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/tavily_search.py
--rw-r--r--   0        0        0     4006 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/tensorflow_datasets.py
--rw-r--r--   0        0        0     3441 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/twilio.py
--rw-r--r--   0        0        0     4087 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/vertexai.py
--rw-r--r--   0        0        0     5346 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/wikidata.py
--rw-r--r--   0        0        0     4270 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/wikipedia.py
--rw-r--r--   0        0        0     2011 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/wolfram_alpha.py
--rw-r--r--   0        0        0     7951 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/you.py
--rw-r--r--   0        0        0    11666 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utilities/zapier.py
--rw-r--r--   0        0        0       45 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utils/__init__.py
--rw-r--r--   0        0        0     1509 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utils/ernie_functions.py
--rw-r--r--   0        0        0      775 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utils/google.py
--rw-r--r--   0        0        0     2724 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utils/math.py
--rw-r--r--   0        0        0      264 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utils/openai.py
--rw-r--r--   0        0        0      377 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/utils/openai_functions.py
--rw-r--r--   0        0        0    16943 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/__init__.py
--rw-r--r--   0        0        0    19806 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/alibabacloud_opensearch.py
--rw-r--r--   0        0        0    15752 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/analyticdb.py
--rw-r--r--   0        0        0    17735 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/annoy.py
--rw-r--r--   0        0        0    17067 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/apache_doris.py
--rw-r--r--   0        0        0    46743 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/astradb.py
--rw-r--r--   0        0        0    12136 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/atlas.py
--rw-r--r--   0        0        0    21155 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/awadb.py
--rw-r--r--   0        0        0    20882 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/azure_cosmos_db.py
--rw-r--r--   0        0        0    30059 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/azuresearch.py
--rw-r--r--   0        0        0    15245 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/bagel.py
--rw-r--r--   0        0        0       78 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/bageldb.py
--rw-r--r--   0        0        0    16548 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/baiducloud_vector_search.py
--rw-r--r--   0        0        0    15271 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/baiduvectordb.py
--rw-r--r--   0        0        0    34562 2024-05-17 20:49:58.783865 langchain_community-0.2.0/langchain_community/vectorstores/bigquery_vector_search.py
--rw-r--r--   0        0        0    38804 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/cassandra.py
--rw-r--r--   0        0        0    31090 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/chroma.py
--rw-r--r--   0        0        0    12095 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/clarifai.py
--rw-r--r--   0        0        0    22074 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/clickhouse.py
--rw-r--r--   0        0        0    22766 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/couchbase.py
--rw-r--r--   0        0        0    13946 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/dashvector.py
--rw-r--r--   0        0        0    23115 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/databricks_vector_search.py
--rw-r--r--   0        0        0    43000 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/deeplake.py
--rw-r--r--   0        0        0    13208 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/dingo.py
--rw-r--r--   0        0        0      236 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/docarray/__init__.py
--rw-r--r--   0        0        0     7021 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/docarray/base.py
--rw-r--r--   0        0        0     4042 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/docarray/hnsw.py
--rw-r--r--   0        0        0     2418 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/docarray/in_memory.py
--rw-r--r--   0        0        0    11947 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/documentdb.py
--rw-r--r--   0        0        0     9991 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/duckdb.py
--rw-r--r--   0        0        0    20611 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/ecloud_vector_search.py
--rw-r--r--   0        0        0    29007 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/elastic_vector_search.py
--rw-r--r--   0        0        0    48577 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/elasticsearch.py
--rw-r--r--   0        0        0    14183 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/epsilla.py
--rw-r--r--   0        0        0    45888 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/faiss.py
--rw-r--r--   0        0        0    25861 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/hanavector.py
--rw-r--r--   0        0        0    26837 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/hippo.py
--rw-r--r--   0        0        0    13642 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/hologres.py
--rw-r--r--   0        0        0    21348 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/infinispanvs.py
--rw-r--r--   0        0        0     6299 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/inmemory.py
--rw-r--r--   0        0        0    14581 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/jaguar.py
--rw-r--r--   0        0        0     9087 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/kdbai.py
--rw-r--r--   0        0        0    34973 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/kinetica.py
--rw-r--r--   0        0        0    10720 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/lancedb.py
--rw-r--r--   0        0        0    38505 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/lantern.py
--rw-r--r--   0        0        0     7745 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/llm_rails.py
--rw-r--r--   0        0        0    17075 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/marqo.py
--rw-r--r--   0        0        0    21617 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/matching_engine.py
--rw-r--r--   0        0        0    12086 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/meilisearch.py
--rw-r--r--   0        0        0    41955 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/milvus.py
--rw-r--r--   0        0        0    19047 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/momento_vector_index.py
--rw-r--r--   0        0        0    13700 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/mongodb_atlas.py
--rw-r--r--   0        0        0    22612 2024-05-17 20:49:58.787865 langchain_community-0.2.0/langchain_community/vectorstores/myscale.py
--rw-r--r--   0        0        0    53077 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/neo4j_vector.py
--rw-r--r--   0        0        0     5404 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/nucliadb.py
--rw-r--r--   0        0        0    51650 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/opensearch_vector_search.py
--rw-r--r--   0        0        0    32081 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/oraclevs.py
--rw-r--r--   0        0        0     7709 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/pathway.py
--rw-r--r--   0        0        0    17949 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/pgembedding.py
--rw-r--r--   0        0        0     7838 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/pgvecto_rs.py
--rw-r--r--   0        0        0    51715 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/pgvector.py
--rw-r--r--   0        0        0    17678 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/pinecone.py
--rw-r--r--   0        0        0    94285 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/qdrant.py
--rw-r--r--   0        0        0      265 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/redis/__init__.py
--rw-r--r--   0        0        0    56021 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/redis/base.py
--rw-r--r--   0        0        0      420 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/redis/constants.py
--rw-r--r--   0        0        0    16219 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/redis/filters.py
--rw-r--r--   0        0        0    10418 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/redis/schema.py
--rw-r--r--   0        0        0    18388 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/relyt.py
--rw-r--r--   0        0        0    15235 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/rocksetdb.py
--rw-r--r--   0        0        0    20719 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/scann.py
--rw-r--r--   0        0        0     9721 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/semadb.py
--rw-r--r--   0        0        0    45305 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/singlestoredb.py
--rw-r--r--   0        0        0    12372 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/sklearn.py
--rw-r--r--   0        0        0     7302 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/sqlitevss.py
--rw-r--r--   0        0        0    17220 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/starrocks.py
--rw-r--r--   0        0        0    15689 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/supabase.py
--rw-r--r--   0        0        0    15428 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/surrealdb.py
--rw-r--r--   0        0        0     9559 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/tair.py
--rw-r--r--   0        0        0    20524 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/tencentvectordb.py
--rw-r--r--   0        0        0    17534 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/thirdai_neuraldb.py
--rw-r--r--   0        0        0    13630 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/tidb_vector.py
--rw-r--r--   0        0        0     4927 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/tigris.py
--rw-r--r--   0        0        0    29797 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/tiledb.py
--rw-r--r--   0        0        0    29831 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/timescalevector.py
--rw-r--r--   0        0        0     9713 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/typesense.py
--rw-r--r--   0        0        0    33147 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/upstash.py
--rw-r--r--   0        0        0     5737 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/usearch.py
--rw-r--r--   0        0        0     2474 2024-05-17 20:49:58.791864 langchain_community-0.2.0/langchain_community/vectorstores/utils.py
--rw-r--r--   0        0        0    12898 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/vald.py
--rw-r--r--   0        0        0    53231 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/vdms.py
--rw-r--r--   0        0        0    19845 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/vearch.py
--rw-r--r--   0        0        0    21908 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/vectara.py
--rw-r--r--   0        0        0     9785 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/vespa.py
--rw-r--r--   0        0        0    15510 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/vikingdb.py
--rw-r--r--   0        0        0     8145 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/vlite.py
--rw-r--r--   0        0        0    19253 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/weaviate.py
--rw-r--r--   0        0        0     9018 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/xata.py
--rw-r--r--   0        0        0    34543 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/yellowbrick.py
--rw-r--r--   0        0        0    23192 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/zep.py
--rw-r--r--   0        0        0     8255 2024-05-17 20:49:58.795864 langchain_community-0.2.0/langchain_community/vectorstores/zilliz.py
--rw-r--r--   0        0        0    11096 2024-05-17 20:49:58.795864 langchain_community-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     8780 1970-01-01 00:00:00.000000 langchain_community-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1352 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/README.md
+-rw-r--r--   0        0        0      307 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/__init__.py
+-rw-r--r--   0        0        0      336 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/adapters/__init__.py
+-rw-r--r--   0        0        0    12269 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/adapters/openai.py
+-rw-r--r--   0        0        0     6498 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/ainetwork/__init__.py
+-rw-r--r--   0        0        0     1762 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/ainetwork/toolkit.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/amadeus/__init__.py
+-rw-r--r--   0        0        0     1084 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/amadeus/toolkit.py
+-rw-r--r--   0        0        0      927 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/azure_ai_services.py
+-rw-r--r--   0        0        0      984 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/azure_cognitive_services.py
+-rw-r--r--   0        0        0       99 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/base.py
+-rw-r--r--   0        0        0       32 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/cassandra_database/__init__.py
+-rw-r--r--   0        0        0     1026 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/cassandra_database/toolkit.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/clickup/__init__.py
+-rw-r--r--   0        0        0     3576 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/clickup/toolkit.py
+-rw-r--r--   0        0        0       26 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/cogniswitch/__init__.py
+-rw-r--r--   0        0        0     1322 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/cogniswitch/toolkit.py
+-rw-r--r--   0        0        0      116 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/connery/__init__.py
+-rw-r--r--   0        0        0     1367 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/connery/toolkit.py
+-rw-r--r--   0        0        0     1091 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/csv/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/file_management/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/file_management/toolkit.py
+-rw-r--r--   0        0        0       22 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/github/__init__.py
+-rw-r--r--   0        0        0    10116 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/github/toolkit.py
+-rw-r--r--   0        0        0       22 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/gitlab/__init__.py
+-rw-r--r--   0        0        0     2886 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/gitlab/toolkit.py
+-rw-r--r--   0        0        0       21 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/gmail/__init__.py
+-rw-r--r--   0        0        0     2026 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/gmail/toolkit.py
+-rw-r--r--   0        0        0       20 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/jira/__init__.py
+-rw-r--r--   0        0        0     2209 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/jira/toolkit.py
+-rw-r--r--   0        0        0       18 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/json/__init__.py
+-rw-r--r--   0        0        0     1894 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/json/base.py
+-rw-r--r--   0        0        0     1819 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/json/prompt.py
+-rw-r--r--   0        0        0      577 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/json/toolkit.py
+-rw-r--r--   0        0        0    28945 2024-05-09 22:13:05.458945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/load_tools.py
+-rw-r--r--   0        0        0       23 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/multion/__init__.py
+-rw-r--r--   0        0        0     1172 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/multion/toolkit.py
+-rw-r--r--   0        0        0       19 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nasa/__init__.py
+-rw-r--r--   0        0        0     1913 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nasa/toolkit.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nla/__init__.py
+-rw-r--r--   0        0        0     2038 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nla/tool.py
+-rw-r--r--   0        0        0     4177 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nla/toolkit.py
+-rw-r--r--   0        0        0       25 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/office365/__init__.py
+-rw-r--r--   0        0        0     1793 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/office365/toolkit.py
+-rw-r--r--   0        0        0       26 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/__init__.py
+-rw-r--r--   0        0        0     2870 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/base.py
+-rw-r--r--   0        0        0    13922 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/planner.py
+-rw-r--r--   0        0        0    11686 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/planner_prompt.py
+-rw-r--r--   0        0        0     1770 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/prompt.py
+-rw-r--r--   0        0        0     2557 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/spec.py
+-rw-r--r--   0        0        0     4238 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/toolkit.py
+-rw-r--r--   0        0        0      174 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/playwright/__init__.py
+-rw-r--r--   0        0        0     4223 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/playwright/toolkit.py
+-rw-r--r--   0        0        0       22 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/polygon/__init__.py
+-rw-r--r--   0        0        0     1107 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/polygon/toolkit.py
+-rw-r--r--   0        0        0       22 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/__init__.py
+-rw-r--r--   0        0        0     2491 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/base.py
+-rw-r--r--   0        0        0     2649 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/chat_base.py
+-rw-r--r--   0        0        0     2773 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/prompt.py
+-rw-r--r--   0        0        0     3752 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/toolkit.py
+-rw-r--r--   0        0        0       21 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/slack/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/slack/toolkit.py
+-rw-r--r--   0        0        0       23 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/spark_sql/__init__.py
+-rw-r--r--   0        0        0     2355 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/spark_sql/base.py
+-rw-r--r--   0        0        0     1202 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/spark_sql/prompt.py
+-rw-r--r--   0        0        0     1065 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/spark_sql/toolkit.py
+-rw-r--r--   0        0        0       17 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/sql/__init__.py
+-rw-r--r--   0        0        0     9372 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/sql/base.py
+-rw-r--r--   0        0        0     1428 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/sql/prompt.py
+-rw-r--r--   0        0        0     2983 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/sql/toolkit.py
+-rw-r--r--   0        0        0       21 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/steam/__init__.py
+-rw-r--r--   0        0        0     1447 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/steam/toolkit.py
+-rw-r--r--   0        0        0     1095 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/xorbits/__init__.py
+-rw-r--r--   0        0        0       22 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/zapier/__init__.py
+-rw-r--r--   0        0        0     1914 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/agent_toolkits/zapier/toolkit.py
+-rw-r--r--   0        0        0    87618 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/cache.py
+-rw-r--r--   0        0        0     5635 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/__init__.py
+-rw-r--r--   0        0        0    14597 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/aim_callback.py
+-rw-r--r--   0        0        0    14738 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/argilla_callback.py
+-rw-r--r--   0        0        0     7480 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/arize_callback.py
+-rw-r--r--   0        0        0    11242 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/arthur_callback.py
+-rw-r--r--   0        0        0     3906 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/bedrock_anthropic_callback.py
+-rw-r--r--   0        0        0    18634 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/clearml_callback.py
+-rw-r--r--   0        0        0    22975 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/comet_ml_callback.py
+-rw-r--r--   0        0        0     6382 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/confident_callback.py
+-rw-r--r--   0        0        0     6496 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/context_callback.py
+-rw-r--r--   0        0        0    11430 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/fiddler_callback.py
+-rw-r--r--   0        0        0    12769 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/flyte_callback.py
+-rw-r--r--   0        0        0     2587 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/human.py
+-rw-r--r--   0        0        0     8764 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/infino_callback.py
+-rw-r--r--   0        0        0    13879 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/labelstudio_callback.py
+-rw-r--r--   0        0        0    20555 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/llmonitor_callback.py
+-rw-r--r--   0        0        0     3201 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/manager.py
+-rw-r--r--   0        0        0    27406 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/mlflow_callback.py
+-rw-r--r--   0        0        0     8408 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/openai_info.py
+-rw-r--r--   0        0        0     5535 2024-05-09 22:13:05.462945 langchain_community-0.2.0rc1/langchain_community/callbacks/promptlayer_callback.py
+-rw-r--r--   0        0        0     8787 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/sagemaker_callback.py
+-rw-r--r--   0        0        0     3183 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/streamlit/__init__.py
+-rw-r--r--   0        0        0     5395 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/streamlit/mutable_expander.py
+-rw-r--r--   0        0        0    15562 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/streamlit/streamlit_callback_handler.py
+-rw-r--r--   0        0        0      498 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/tracers/__init__.py
+-rw-r--r--   0        0        0     4547 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/tracers/comet.py
+-rw-r--r--   0        0        0    19020 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/tracers/wandb.py
+-rw-r--r--   0        0        0     4526 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/trubrics_callback.py
+-rw-r--r--   0        0        0    14446 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/uptrain_callback.py
+-rw-r--r--   0        0        0     7879 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/utils.py
+-rw-r--r--   0        0        0    20385 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/wandb_callback.py
+-rw-r--r--   0        0        0     7881 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/callbacks/whylabs_callback.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/ernie_functions/__init__.py
+-rw-r--r--   0        0        0    23245 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/ernie_functions/base.py
+-rw-r--r--   0        0        0       49 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/__init__.py
+-rw-r--r--   0        0        0     8407 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/arangodb.py
+-rw-r--r--   0        0        0     3699 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/base.py
+-rw-r--r--   0        0        0    10589 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/cypher.py
+-rw-r--r--   0        0        0     9625 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/cypher_utils.py
+-rw-r--r--   0        0        0     5295 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/falkordb.py
+-rw-r--r--   0        0        0     7818 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/gremlin.py
+-rw-r--r--   0        0        0     3727 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/hugegraph.py
+-rw-r--r--   0        0        0     4702 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/kuzu.py
+-rw-r--r--   0        0        0     3715 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/nebulagraph.py
+-rw-r--r--   0        0        0     6908 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/neptune_cypher.py
+-rw-r--r--   0        0        0     6818 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/neptune_sparql.py
+-rw-r--r--   0        0        0     7197 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/ontotext_graphdb.py
+-rw-r--r--   0        0        0    16687 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/prompts.py
+-rw-r--r--   0        0        0     5848 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/sparql.py
+-rw-r--r--   0        0        0     3251 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/llm_requests.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/openapi/__init__.py
+-rw-r--r--   0        0        0     8786 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/openapi/chain.py
+-rw-r--r--   0        0        0     1791 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/openapi/prompts.py
+-rw-r--r--   0        0        0     1974 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/openapi/requests_chain.py
+-rw-r--r--   0        0        0     1846 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chains/openapi/response_chain.py
+-rw-r--r--   0        0        0     2748 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/__init__.py
+-rw-r--r--   0        0        0       85 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/base.py
+-rw-r--r--   0        0        0     2694 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/facebook_messenger.py
+-rw-r--r--   0        0        0     4213 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/gmail.py
+-rw-r--r--   0        0        0     7899 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/imessage.py
+-rw-r--r--   0        0        0     5736 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/langsmith.py
+-rw-r--r--   0        0        0     3101 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/slack.py
+-rw-r--r--   0        0        0     5379 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/telegram.py
+-rw-r--r--   0        0        0     3270 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/utils.py
+-rw-r--r--   0        0        0     4269 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_loaders/whatsapp.py
+-rw-r--r--   0        0        0     5677 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/__init__.py
+-rw-r--r--   0        0        0     5874 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/astradb.py
+-rw-r--r--   0        0        0     3016 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/cassandra.py
+-rw-r--r--   0        0        0     6510 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/cosmos_db.py
+-rw-r--r--   0        0        0     7250 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/dynamodb.py
+-rw-r--r--   0        0        0     7177 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/elasticsearch.py
+-rw-r--r--   0        0        0     1402 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/file.py
+-rw-r--r--   0        0        0     3349 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/firestore.py
+-rw-r--r--   0        0        0      130 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/in_memory.py
+-rw-r--r--   0        0        0     7112 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/momento.py
+-rw-r--r--   0        0        0     3107 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/mongodb.py
+-rw-r--r--   0        0        0     5129 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/neo4j.py
+-rw-r--r--   0        0        0     3345 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/postgres.py
+-rw-r--r--   0        0        0     2192 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/redis.py
+-rw-r--r--   0        0        0     9529 2024-05-09 22:13:05.466946 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/rocksetdb.py
+-rw-r--r--   0        0        0    10331 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/singlestoredb.py
+-rw-r--r--   0        0        0     4722 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/sql.py
+-rw-r--r--   0        0        0     1444 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/streamlit.py
+-rw-r--r--   0        0        0     5255 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/tidb.py
+-rw-r--r--   0        0        0     2148 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/upstash_redis.py
+-rw-r--r--   0        0        0     4639 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/xata.py
+-rw-r--r--   0        0        0     8910 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_message_histories/zep.py
+-rw-r--r--   0        0        0     9183 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/__init__.py
+-rw-r--r--   0        0        0     8210 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/anthropic.py
+-rw-r--r--   0        0        0     8250 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/anyscale.py
+-rw-r--r--   0        0        0    11341 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/azure_openai.py
+-rw-r--r--   0        0        0    15411 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/azureml_endpoint.py
+-rw-r--r--   0        0        0     9935 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/baichuan.py
+-rw-r--r--   0        0        0    22941 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0    10959 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/bedrock.py
+-rw-r--r--   0        0        0     8226 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/cohere.py
+-rw-r--r--   0        0        0     8487 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/coze.py
+-rw-r--r--   0        0        0     5396 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/dappier.py
+-rw-r--r--   0        0        0     1532 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/databricks.py
+-rw-r--r--   0        0        0    16671 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/deepinfra.py
+-rw-r--r--   0        0        0    13134 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/edenai.py
+-rw-r--r--   0        0        0     8039 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/ernie.py
+-rw-r--r--   0        0        0     5587 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/everlyai.py
+-rw-r--r--   0        0        0     3217 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/fake.py
+-rw-r--r--   0        0        0    11992 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/fireworks.py
+-rw-r--r--   0        0        0     7114 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/friendli.py
+-rw-r--r--   0        0        0     9686 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/gigachat.py
+-rw-r--r--   0        0        0    11608 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/google_palm.py
+-rw-r--r--   0        0        0    13080 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/gpt_router.py
+-rw-r--r--   0        0        0     7707 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/huggingface.py
+-rw-r--r--   0        0        0     3741 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/human.py
+-rw-r--r--   0        0        0    10601 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/hunyuan.py
+-rw-r--r--   0        0        0     7628 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/javelin_ai_gateway.py
+-rw-r--r--   0        0        0    15264 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/jinachat.py
+-rw-r--r--   0        0        0    20267 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/kinetica.py
+-rw-r--r--   0        0        0    10026 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/konko.py
+-rw-r--r--   0        0        0    15780 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/litellm.py
+-rw-r--r--   0        0        0     8077 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/litellm_router.py
+-rw-r--r--   0        0        0     8564 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/llama_edge.py
+-rw-r--r--   0        0        0    13406 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/maritalk.py
+-rw-r--r--   0        0        0      967 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/meta.py
+-rw-r--r--   0        0        0     3262 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/minimax.py
+-rw-r--r--   0        0        0     9874 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/mlflow.py
+-rw-r--r--   0        0        0     6711 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0     6166 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/mlx.py
+-rw-r--r--   0        0        0     1927 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/moonshot.py
+-rw-r--r--   0        0        0     3308 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/octoai.py
+-rw-r--r--   0        0        0    13444 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/ollama.py
+-rw-r--r--   0        0        0    26774 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/openai.py
+-rw-r--r--   0        0        0    10504 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/pai_eas_endpoint.py
+-rw-r--r--   0        0        0    10665 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/perplexity.py
+-rw-r--r--   0        0        0    14597 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/premai.py
+-rw-r--r--   0        0        0     5256 2024-05-09 22:13:05.470945 langchain_community-0.2.0rc1/langchain_community/chat_models/promptlayer_openai.py
+-rw-r--r--   0        0        0     2296 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/solar.py
+-rw-r--r--   0        0        0    16754 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/sparkllm.py
+-rw-r--r--   0        0        0    16377 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/tongyi.py
+-rw-r--r--   0        0        0    14583 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/vertexai.py
+-rw-r--r--   0        0        0     5296 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/volcengine_maas.py
+-rw-r--r--   0        0        0    10740 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/yandex.py
+-rw-r--r--   0        0        0    17174 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/yuan2.py
+-rw-r--r--   0        0        0    16761 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/chat_models/zhipuai.py
+-rw-r--r--   0        0        0     1468 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/cross_encoders/__init__.py
+-rw-r--r--   0        0        0      117 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/cross_encoders/base.py
+-rw-r--r--   0        0        0      525 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/cross_encoders/fake.py
+-rw-r--r--   0        0        0     1946 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/cross_encoders/huggingface.py
+-rw-r--r--   0        0        0     5335 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/cross_encoders/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     1176 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/docstore/__init__.py
+-rw-r--r--   0        0        0     1080 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/docstore/arbitrary_fn.py
+-rw-r--r--   0        0        0      833 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/docstore/base.py
+-rw-r--r--   0        0        0       70 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/docstore/document.py
+-rw-r--r--   0        0        0     1610 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/docstore/in_memory.py
+-rw-r--r--   0        0        0     1472 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/docstore/wikipedia.py
+-rw-r--r--   0        0        0     1005 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_compressors/__init__.py
+-rw-r--r--   0        0        0     4342 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_compressors/jina_rerank.py
+-rw-r--r--   0        0        0     6695 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_compressors/llmlingua_filter.py
+-rw-r--r--   0        0        0     5704 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_compressors/openvino_rerank.py
+-rw-r--r--   0        0        0    35823 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2803 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/acreom.py
+-rw-r--r--   0        0        0    10157 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/airbyte.py
+-rw-r--r--   0        0        0      865 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/airbyte_json.py
+-rw-r--r--   0        0        0     1157 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/airtable.py
+-rw-r--r--   0        0        0     2759 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/apify_dataset.py
+-rw-r--r--   0        0        0     5129 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/arcgis_loader.py
+-rw-r--r--   0        0        0      907 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/arxiv.py
+-rw-r--r--   0        0        0     8134 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/assemblyai.py
+-rw-r--r--   0        0        0     4642 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/astradb.py
+-rw-r--r--   0        0        0     8129 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/async_html.py
+-rw-r--r--   0        0        0     5886 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/athena.py
+-rw-r--r--   0        0        0      563 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/azlyrics.py
+-rw-r--r--   0        0        0     1432 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/azure_ai_data.py
+-rw-r--r--   0        0        0     1566 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/azure_blob_storage_container.py
+-rw-r--r--   0        0        0     1644 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/azure_blob_storage_file.py
+-rw-r--r--   0        0        0     1774 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/baiducloud_bos_directory.py
+-rw-r--r--   0        0        0     1848 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/baiducloud_bos_file.py
+-rw-r--r--   0        0        0      126 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/base.py
+-rw-r--r--   0        0        0     7222 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/base_o365.py
+-rw-r--r--   0        0        0     3540 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/bibtex.py
+-rw-r--r--   0        0        0     3852 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/bigquery.py
+-rw-r--r--   0        0        0     4401 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/bilibili.py
+-rw-r--r--   0        0        0    10288 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/blackboard.py
+-rw-r--r--   0        0        0      948 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/blob_loaders/__init__.py
+-rw-r--r--   0        0        0     5390 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/blob_loaders/file_system.py
+-rw-r--r--   0        0        0      145 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/blob_loaders/schema.py
+-rw-r--r--   0        0        0     1526 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/blob_loaders/youtube_audio.py
+-rw-r--r--   0        0        0     5709 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/blockchain.py
+-rw-r--r--   0        0        0     1047 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/brave_search.py
+-rw-r--r--   0        0        0     1340 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/browserbase.py
+-rw-r--r--   0        0        0     2007 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/browserless.py
+-rw-r--r--   0        0        0     4984 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/cassandra.py
+-rw-r--r--   0        0        0     1986 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/chatgpt.py
+-rw-r--r--   0        0        0     3031 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/chm.py
+-rw-r--r--   0        0        0     3410 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/chromium.py
+-rw-r--r--   0        0        0      527 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/college_confidential.py
+-rw-r--r--   0        0        0     3416 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/concurrent.py
+-rw-r--r--   0        0        0    29324 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/confluence.py
+-rw-r--r--   0        0        0     1102 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/conllu.py
+-rw-r--r--   0        0        0     3515 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/couchbase.py
+-rw-r--r--   0        0        0     5835 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/csv_loader.py
+-rw-r--r--   0        0        0     6589 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/cube_semantic.py
+-rw-r--r--   0        0        0     4937 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/datadog_logs.py
+-rw-r--r--   0        0        0     2176 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/dataframe.py
+-rw-r--r--   0        0        0     2054 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/diffbot.py
+-rw-r--r--   0        0        0     8446 2024-05-09 22:13:05.474945 langchain_community-0.2.0rc1/langchain_community/document_loaders/directory.py
+-rw-r--r--   0        0        0     1237 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/discord.py
+-rw-r--r--   0        0        0     3859 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/doc_intelligence.py
+-rw-r--r--   0        0        0    13621 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/docugami.py
+-rw-r--r--   0        0        0     1852 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/docusaurus.py
+-rw-r--r--   0        0        0     6271 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/dropbox.py
+-rw-r--r--   0        0        0     3150 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/duckdb_loader.py
+-rw-r--r--   0        0        0     3835 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/email.py
+-rw-r--r--   0        0        0     1496 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/epub.py
+-rw-r--r--   0        0        0     7753 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/etherscan.py
+-rw-r--r--   0        0        0     5930 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/evernote.py
+-rw-r--r--   0        0        0     1753 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/excel.py
+-rw-r--r--   0        0        0     1270 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/facebook_chat.py
+-rw-r--r--   0        0        0     2171 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/fauna.py
+-rw-r--r--   0        0        0     1543 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/figma.py
+-rw-r--r--   0        0        0     2453 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/firecrawl.py
+-rw-r--r--   0        0        0     3041 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/gcs_directory.py
+-rw-r--r--   0        0        0     3316 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/gcs_file.py
+-rw-r--r--   0        0        0     6374 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/generic.py
+-rw-r--r--   0        0        0     2400 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/geodataframe.py
+-rw-r--r--   0        0        0     4018 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/git.py
+-rw-r--r--   0        0        0     3451 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/gitbook.py
+-rw-r--r--   0        0        0     8676 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/github.py
+-rw-r--r--   0        0        0     4459 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/glue_catalog.py
+-rw-r--r--   0        0        0     5279 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/google_speech_to_text.py
+-rw-r--r--   0        0        0    14435 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/googledrive.py
+-rw-r--r--   0        0        0      928 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/gutenberg.py
+-rw-r--r--   0        0        0     1640 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/helpers.py
+-rw-r--r--   0        0        0     2075 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/hn.py
+-rw-r--r--   0        0        0     1158 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/html.py
+-rw-r--r--   0        0        0     2098 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/html_bs.py
+-rw-r--r--   0        0        0     3095 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/hugging_face_dataset.py
+-rw-r--r--   0        0        0     3628 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/hugging_face_model.py
+-rw-r--r--   0        0        0     7642 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/ifixit.py
+-rw-r--r--   0        0        0     1173 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/image.py
+-rw-r--r--   0        0        0     3707 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/image_captions.py
+-rw-r--r--   0        0        0      477 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/imsdb.py
+-rw-r--r--   0        0        0     1688 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/iugu.py
+-rw-r--r--   0        0        0     3628 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/joplin.py
+-rw-r--r--   0        0        0     7366 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/json_loader.py
+-rw-r--r--   0        0        0     3889 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/kinetica_loader.py
+-rw-r--r--   0        0        0     6058 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/lakefs.py
+-rw-r--r--   0        0        0     2959 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/larksuite.py
+-rw-r--r--   0        0        0     4881 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/llmsherpa.py
+-rw-r--r--   0        0        0     1818 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/markdown.py
+-rw-r--r--   0        0        0     3079 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/mastodon.py
+-rw-r--r--   0        0        0     3199 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/max_compute.py
+-rw-r--r--   0        0        0     3859 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/mediawikidump.py
+-rw-r--r--   0        0        0      999 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/merge.py
+-rw-r--r--   0        0        0     2602 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/mhtml.py
+-rw-r--r--   0        0        0     8923 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/mintbase.py
+-rw-r--r--   0        0        0     3074 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/modern_treasury.py
+-rw-r--r--   0        0        0     3182 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/mongodb.py
+-rw-r--r--   0        0        0     4283 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/news.py
+-rw-r--r--   0        0        0     4296 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/notebook.py
+-rw-r--r--   0        0        0      834 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/notion.py
+-rw-r--r--   0        0        0     7715 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/notiondb.py
+-rw-r--r--   0        0        0     1102 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/nuclia.py
+-rw-r--r--   0        0        0     3593 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/obs_directory.py
+-rw-r--r--   0        0        0     4768 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/obs_file.py
+-rw-r--r--   0        0        0     6132 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/obsidian.py
+-rw-r--r--   0        0        0     1840 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/odt.py
+-rw-r--r--   0        0        0     3270 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/onedrive.py
+-rw-r--r--   0        0        0     1154 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/onedrive_file.py
+-rw-r--r--   0        0        0     7807 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/onenote.py
+-rw-r--r--   0        0        0     1219 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/open_city_data.py
+-rw-r--r--   0        0        0     4221 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/oracleadb_loader.py
+-rw-r--r--   0        0        0    15573 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/oracleai.py
+-rw-r--r--   0        0        0     1818 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/org_mode.py
+-rw-r--r--   0        0        0     1283 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/__init__.py
+-rw-r--r--   0        0        0    16911 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/audio.py
+-rw-r--r--   0        0        0     4050 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/doc_intelligence.py
+-rw-r--r--   0        0        0    15457 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/docai.py
+-rw-r--r--   0        0        0     2502 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/generic.py
+-rw-r--r--   0        0        0     5903 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/grobid.py
+-rw-r--r--   0        0        0      109 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/html/__init__.py
+-rw-r--r--   0        0        0     1608 2024-05-09 22:13:05.478945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/html/bs4.py
+-rw-r--r--   0        0        0      136 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/__init__.py
+-rw-r--r--   0        0        0      877 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/c.py
+-rw-r--r--   0        0        0     3745 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/cobol.py
+-rw-r--r--   0        0        0      495 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/code_segmenter.py
+-rw-r--r--   0        0        0      893 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/cpp.py
+-rw-r--r--   0        0        0      893 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/csharp.py
+-rw-r--r--   0        0        0      693 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/go.py
+-rw-r--r--   0        0        0      736 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/java.py
+-rw-r--r--   0        0        0     2185 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/javascript.py
+-rw-r--r--   0        0        0      707 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/kotlin.py
+-rw-r--r--   0        0        0     7538 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/language_parser.py
+-rw-r--r--   0        0        0      790 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/lua.py
+-rw-r--r--   0        0        0      666 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/perl.py
+-rw-r--r--   0        0        0      850 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/php.py
+-rw-r--r--   0        0        0     1731 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/python.py
+-rw-r--r--   0        0        0      697 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/ruby.py
+-rw-r--r--   0        0        0      774 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/rust.py
+-rw-r--r--   0        0        0      772 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/scala.py
+-rw-r--r--   0        0        0     3473 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/tree_sitter_segmenter.py
+-rw-r--r--   0        0        0      795 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/typescript.py
+-rw-r--r--   0        0        0     1812 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/msword.py
+-rw-r--r--   0        0        0    22511 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/pdf.py
+-rw-r--r--   0        0        0     1214 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/registry.py
+-rw-r--r--   0        0        0      563 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/txt.py
+-rw-r--r--   0        0        0     7902 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/vsdx.py
+-rw-r--r--   0        0        0    27750 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/pdf.py
+-rw-r--r--   0        0        0    19160 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/pebblo.py
+-rw-r--r--   0        0        0     1161 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/polars_dataframe.py
+-rw-r--r--   0        0        0     2508 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/powerpoint.py
+-rw-r--r--   0        0        0     1315 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/psychic.py
+-rw-r--r--   0        0        0     1066 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/pubmed.py
+-rw-r--r--   0        0        0     3388 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/pyspark_dataframe.py
+-rw-r--r--   0        0        0      590 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/python.py
+-rw-r--r--   0        0        0     8426 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/quip.py
+-rw-r--r--   0        0        0     6821 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/readthedocs.py
+-rw-r--r--   0        0        0    14800 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/recursive_url_loader.py
+-rw-r--r--   0        0        0     4584 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/reddit.py
+-rw-r--r--   0        0        0      725 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/roam.py
+-rw-r--r--   0        0        0     4527 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/rocksetdb.py
+-rw-r--r--   0        0        0     4859 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/rspace.py
+-rw-r--r--   0        0        0     4882 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/rss.py
+-rw-r--r--   0        0        0     1902 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/rst.py
+-rw-r--r--   0        0        0     2131 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/rtf.py
+-rw-r--r--   0        0        0     5871 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/s3_directory.py
+-rw-r--r--   0        0        0     5956 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/s3_file.py
+-rw-r--r--   0        0        0     3002 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/sharepoint.py
+-rw-r--r--   0        0        0     8524 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/sitemap.py
+-rw-r--r--   0        0        0     4027 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/slack_directory.py
+-rw-r--r--   0        0        0     4703 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/snowflake_loader.py
+-rw-r--r--   0        0        0     3412 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/spider.py
+-rw-r--r--   0        0        0     2004 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/spreedly.py
+-rw-r--r--   0        0        0     5581 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/sql_database.py
+-rw-r--r--   0        0        0      901 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/srt.py
+-rw-r--r--   0        0        0     1811 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/stripe.py
+-rw-r--r--   0        0        0     2965 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/surrealdb.py
+-rw-r--r--   0        0        0     9079 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/telegram.py
+-rw-r--r--   0        0        0     1700 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/tencent_cos_directory.py
+-rw-r--r--   0        0        0     1617 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/tencent_cos_file.py
+-rw-r--r--   0        0        0     2941 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/tensorflow_datasets.py
+-rw-r--r--   0        0        0     2070 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/text.py
+-rw-r--r--   0        0        0     2610 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/tidb.py
+-rw-r--r--   0        0        0      842 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/tomarkdown.py
+-rw-r--r--   0        0        0     1458 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/toml.py
+-rw-r--r--   0        0        0     6584 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/trello.py
+-rw-r--r--   0        0        0     1363 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/tsv.py
+-rw-r--r--   0        0        0     3438 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/twitter.py
+-rw-r--r--   0        0        0    14328 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/unstructured.py
+-rw-r--r--   0        0        0     6019 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/url.py
+-rw-r--r--   0        0        0     8527 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/url_playwright.py
+-rw-r--r--   0        0        0     6640 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/url_selenium.py
+-rw-r--r--   0        0        0     1946 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/vsdx.py
+-rw-r--r--   0        0        0     1527 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/weather.py
+-rw-r--r--   0        0        0    10115 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/web_base.py
+-rw-r--r--   0        0        0     1750 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/whatsapp_chat.py
+-rw-r--r--   0        0        0     2123 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/wikipedia.py
+-rw-r--r--   0        0        0     4633 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/word_document.py
+-rw-r--r--   0        0        0     1594 2024-05-09 22:13:05.482945 langchain_community-0.2.0rc1/langchain_community/document_loaders/xml.py
+-rw-r--r--   0        0        0     1119 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_loaders/xorbits.py
+-rw-r--r--   0        0        0    15500 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_loaders/youtube.py
+-rw-r--r--   0        0        0     2958 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_loaders/yuque.py
+-rw-r--r--   0        0        0     3903 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/__init__.py
+-rw-r--r--   0        0        0     6821 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/beautiful_soup_transformer.py
+-rw-r--r--   0        0        0     4240 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/doctran_text_extract.py
+-rw-r--r--   0        0        0     2155 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/doctran_text_qa.py
+-rw-r--r--   0        0        0     2331 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/doctran_text_translate.py
+-rw-r--r--   0        0        0     7882 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/embeddings_redundant_filter.py
+-rw-r--r--   0        0        0     4309 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/google_translate.py
+-rw-r--r--   0        0        0     1834 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/html2text.py
+-rw-r--r--   0        0        0     1437 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/long_context_reorder.py
+-rw-r--r--   0        0        0     3154 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/markdownify.py
+-rw-r--r--   0        0        0     1500 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/nuclia_text_transform.py
+-rw-r--r--   0        0        0     6243 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/openai_functions.py
+-rw-r--r--   0        0        0     6033 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt
+-rw-r--r--   0        0        0    15650 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/__init__.py
+-rw-r--r--   0        0        0     9614 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/aleph_alpha.py
+-rw-r--r--   0        0        0     2609 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/anyscale.py
+-rw-r--r--   0        0        0     1865 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/awa.py
+-rw-r--r--   0        0        0     7239 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/azure_openai.py
+-rw-r--r--   0        0        0     4585 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/baichuan.py
+-rw-r--r--   0        0        0     5201 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     7274 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/bedrock.py
+-rw-r--r--   0        0        0     2725 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/bookend.py
+-rw-r--r--   0        0        0     4677 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/clarifai.py
+-rw-r--r--   0        0        0     2869 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/cloudflare_workersai.py
+-rw-r--r--   0        0        0     5514 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/cohere.py
+-rw-r--r--   0        0        0     5216 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/dashscope.py
+-rw-r--r--   0        0        0     1271 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/databricks.py
+-rw-r--r--   0        0        0     5002 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/deepinfra.py
+-rw-r--r--   0        0        0     3699 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/edenai.py
+-rw-r--r--   0        0        0     8546 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/elasticsearch.py
+-rw-r--r--   0        0        0     5528 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/embaas.py
+-rw-r--r--   0        0        0     4997 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/ernie.py
+-rw-r--r--   0        0        0     1512 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/fake.py
+-rw-r--r--   0        0        0     3770 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/fastembed.py
+-rw-r--r--   0        0        0     5989 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/gigachat.py
+-rw-r--r--   0        0        0     3272 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/google_palm.py
+-rw-r--r--   0        0        0     2223 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/gpt4all.py
+-rw-r--r--   0        0        0     5306 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/gradient_ai.py
+-rw-r--r--   0        0        0    13675 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/huggingface.py
+-rw-r--r--   0        0        0     5078 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/huggingface_hub.py
+-rw-r--r--   0        0        0    10290 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/infinity.py
+-rw-r--r--   0        0        0     5196 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/infinity_local.py
+-rw-r--r--   0        0        0     8168 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/itrex.py
+-rw-r--r--   0        0        0     3669 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/javelin_ai_gateway.py
+-rw-r--r--   0        0        0     2607 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/jina.py
+-rw-r--r--   0        0        0     2873 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/johnsnowlabs.py
+-rw-r--r--   0        0        0     3064 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/laser.py
+-rw-r--r--   0        0        0     4157 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/llamacpp.py
+-rw-r--r--   0        0        0     4009 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/llamafile.py
+-rw-r--r--   0        0        0     2321 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/llm_rails.py
+-rw-r--r--   0        0        0    12261 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/localai.py
+-rw-r--r--   0        0        0     4826 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/minimax.py
+-rw-r--r--   0        0        0     3047 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/mlflow.py
+-rw-r--r--   0        0        0     2447 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/mlflow_gateway.py
+-rw-r--r--   0        0        0     2384 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/modelscope_hub.py
+-rw-r--r--   0        0        0     5115 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/mosaicml.py
+-rw-r--r--   0        0        0     5753 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/nemo.py
+-rw-r--r--   0        0        0     2203 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/nlpcloud.py
+-rw-r--r--   0        0        0     7015 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/oci_generative_ai.py
+-rw-r--r--   0        0        0     3799 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/octoai_embeddings.py
+-rw-r--r--   0        0        0     7953 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/ollama.py
+-rw-r--r--   0        0        0    29239 2024-05-09 22:13:05.486945 langchain_community-0.2.0rc1/langchain_community/embeddings/openai.py
+-rw-r--r--   0        0        0    12346 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/openvino.py
+-rw-r--r--   0        0        0     7663 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/optimum_intel.py
+-rw-r--r--   0        0        0     5208 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/oracleai.py
+-rw-r--r--   0        0        0     4481 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/premai.py
+-rw-r--r--   0        0        0     7596 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/sagemaker_endpoint.py
+-rw-r--r--   0        0        0     5251 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/sambanova.py
+-rw-r--r--   0        0        0     3807 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/self_hosted.py
+-rw-r--r--   0        0        0     6583 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0      189 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/sentence_transformer.py
+-rw-r--r--   0        0        0     4282 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/solar.py
+-rw-r--r--   0        0        0     3955 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/spacy_embeddings.py
+-rw-r--r--   0        0        0     6967 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/sparkllm.py
+-rw-r--r--   0        0        0     2413 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/tensorflow_hub.py
+-rw-r--r--   0        0        0     2364 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/text2vec.py
+-rw-r--r--   0        0        0     7685 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/titan_takeoff.py
+-rw-r--r--   0        0        0    14681 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/vertexai.py
+-rw-r--r--   0        0        0     4198 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/volcengine.py
+-rw-r--r--   0        0        0     7487 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/voyageai.py
+-rw-r--r--   0        0        0     3303 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/xinference.py
+-rw-r--r--   0        0        0     8005 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/embeddings/yandex.py
+-rw-r--r--   0        0        0      608 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/example_selectors/__init__.py
+-rw-r--r--   0        0        0     3842 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/example_selectors/ngram_overlap.py
+-rw-r--r--   0        0        0     3024 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/__init__.py
+-rw-r--r--   0        0        0    26675 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/age_graph.py
+-rw-r--r--   0        0        0     6961 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/arangodb_graph.py
+-rw-r--r--   0        0        0     6951 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/falkordb_graph.py
+-rw-r--r--   0        0        0     1584 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/graph_document.py
+-rw-r--r--   0        0        0      993 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/graph_store.py
+-rw-r--r--   0        0        0     8189 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/gremlin_graph.py
+-rw-r--r--   0        0        0     2511 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/hugegraph.py
+-rw-r--r--   0        0        0     3970 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/index_creator.py
+-rw-r--r--   0        0        0     3918 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/kuzu_graph.py
+-rw-r--r--   0        0        0     2575 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/memgraph_graph.py
+-rw-r--r--   0        0        0     8113 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/nebula_graph.py
+-rw-r--r--   0        0        0    29849 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/neo4j_graph.py
+-rw-r--r--   0        0        0    14357 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/neptune_graph.py
+-rw-r--r--   0        0        0    10315 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/neptune_rdf_graph.py
+-rw-r--r--   0        0        0     7896 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/networkx_graph.py
+-rw-r--r--   0        0        0     7646 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/ontotext_graphdb_graph.py
+-rw-r--r--   0        0        0    10577 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/rdf_graph.py
+-rw-r--r--   0        0        0     3543 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/graphs/tigergraph_graph.py
+-rw-r--r--   0        0        0      488 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/indexes/__init__.py
+-rw-r--r--   0        0        0     8199 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/indexes/_document_manager.py
+-rw-r--r--   0        0        0    21011 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0     5191 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/indexes/base.py
+-rw-r--r--   0        0        0    27750 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/__init__.py
+-rw-r--r--   0        0        0     5292 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/ai21.py
+-rw-r--r--   0        0        0    11514 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/aleph_alpha.py
+-rw-r--r--   0        0        0     3061 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/amazon_api_gateway.py
+-rw-r--r--   0        0        0    12760 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/anthropic.py
+-rw-r--r--   0        0        0    11930 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/anyscale.py
+-rw-r--r--   0        0        0     9619 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/aphrodite.py
+-rw-r--r--   0        0        0     4356 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/arcee.py
+-rw-r--r--   0        0        0     6007 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/aviary.py
+-rw-r--r--   0        0        0    20617 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/azureml_endpoint.py
+-rw-r--r--   0        0        0     3051 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/baichuan.py
+-rw-r--r--   0        0        0     7729 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/baidu_qianfan_endpoint.py
+-rw-r--r--   0        0        0     4830 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/bananadev.py
+-rw-r--r--   0        0        0     3187 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/baseten.py
+-rw-r--r--   0        0        0     9113 2024-05-09 22:13:05.490945 langchain_community-0.2.0rc1/langchain_community/llms/beam.py
+-rw-r--r--   0        0        0    31549 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/bedrock.py
+-rw-r--r--   0        0        0     5515 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/bigdl_llm.py
+-rw-r--r--   0        0        0     6232 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/bittensor.py
+-rw-r--r--   0        0        0     4044 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/cerebriumai.py
+-rw-r--r--   0        0        0     3950 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/chatglm.py
+-rw-r--r--   0        0        0     4884 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/chatglm3.py
+-rw-r--r--   0        0        0     6578 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/clarifai.py
+-rw-r--r--   0        0        0     4239 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/cloudflare_workersai.py
+-rw-r--r--   0        0        0     8709 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/cohere.py
+-rw-r--r--   0        0        0     4241 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/ctransformers.py
+-rw-r--r--   0        0        0     4135 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/ctranslate2.py
+-rw-r--r--   0        0        0    20509 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/databricks.py
+-rw-r--r--   0        0        0     7006 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/deepinfra.py
+-rw-r--r--   0        0        0     8657 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/deepsparse.py
+-rw-r--r--   0        0        0     9448 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/edenai.py
+-rw-r--r--   0        0        0     6459 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/exllamav2.py
+-rw-r--r--   0        0        0     2444 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/fake.py
+-rw-r--r--   0        0        0    11938 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/fireworks.py
+-rw-r--r--   0        0        0     3762 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/forefrontai.py
+-rw-r--r--   0        0        0    14570 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/friendli.py
+-rw-r--r--   0        0        0    11659 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/gigachat.py
+-rw-r--r--   0        0        0     8860 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/google_palm.py
+-rw-r--r--   0        0        0     5301 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/gooseai.py
+-rw-r--r--   0        0        0     6605 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/gpt4all.py
+-rw-r--r--   0        0        0    14199 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/gradient_ai.py
+-rw-r--r--   0        0        0      664 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/grammars/json.gbnf
+-rw-r--r--   0        0        0      167 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/grammars/list.gbnf
+-rw-r--r--   0        0        0    14440 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/huggingface_endpoint.py
+-rw-r--r--   0        0        0     5382 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/huggingface_hub.py
+-rw-r--r--   0        0        0    10932 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/huggingface_pipeline.py
+-rw-r--r--   0        0        0    11653 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/huggingface_text_gen_inference.py
+-rw-r--r--   0        0        0     2575 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/human.py
+-rw-r--r--   0        0        0     9521 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/ipex_llm.py
+-rw-r--r--   0        0        0     4723 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/javelin_ai_gateway.py
+-rw-r--r--   0        0        0     5094 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/koboldai.py
+-rw-r--r--   0        0        0     6554 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/konko.py
+-rw-r--r--   0        0        0     3477 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/layerup_security.py
+-rw-r--r--   0        0        0    12476 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/llamacpp.py
+-rw-r--r--   0        0        0    10422 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/llamafile.py
+-rw-r--r--   0        0        0     1709 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/loading.py
+-rw-r--r--   0        0        0     1965 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/manifest.py
+-rw-r--r--   0        0        0     5445 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/minimax.py
+-rw-r--r--   0        0        0     3431 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/mlflow.py
+-rw-r--r--   0        0        0     3240 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/mlflow_ai_gateway.py
+-rw-r--r--   0        0        0     6254 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/mlx_pipeline.py
+-rw-r--r--   0        0        0     3288 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/modal.py
+-rw-r--r--   0        0        0     4619 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/moonshot.py
+-rw-r--r--   0        0        0     6157 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/mosaicml.py
+-rw-r--r--   0        0        0     5053 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/nlpcloud.py
+-rw-r--r--   0        0        0    12182 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/oci_data_science_model_deployment_endpoint.py
+-rw-r--r--   0        0        0     9398 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/oci_generative_ai.py
+-rw-r--r--   0        0        0     3909 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/octoai_endpoint.py
+-rw-r--r--   0        0        0    17571 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/ollama.py
+-rw-r--r--   0        0        0     4110 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/opaqueprompts.py
+-rw-r--r--   0        0        0    47742 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/openai.py
+-rw-r--r--   0        0        0    11010 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/openllm.py
+-rw-r--r--   0        0        0      902 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/openlm.py
+-rw-r--r--   0        0        0     8059 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/pai_eas_endpoint.py
+-rw-r--r--   0        0        0     5402 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/petals.py
+-rw-r--r--   0        0        0     4210 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/pipelineai.py
+-rw-r--r--   0        0        0     8403 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/predibase.py
+-rw-r--r--   0        0        0     4417 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/predictionguard.py
+-rw-r--r--   0        0        0     8806 2024-05-09 22:13:05.494945 langchain_community-0.2.0rc1/langchain_community/llms/promptlayer_openai.py
+-rw-r--r--   0        0        0     8392 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/replicate.py
+-rw-r--r--   0        0        0     7401 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/rwkv.py
+-rw-r--r--   0        0        0    13165 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0    29410 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/sambanova.py
+-rw-r--r--   0        0        0     8477 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/self_hosted.py
+-rw-r--r--   0        0        0     7744 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/self_hosted_hugging_face.py
+-rw-r--r--   0        0        0     4107 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/solar.py
+-rw-r--r--   0        0        0    12481 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/sparkllm.py
+-rw-r--r--   0        0        0     4776 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/stochasticai.py
+-rw-r--r--   0        0        0     7552 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/symblai_nebula.py
+-rw-r--r--   0        0        0    14151 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/textgen.py
+-rw-r--r--   0        0        0     9281 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/titan_takeoff.py
+-rw-r--r--   0        0        0     7680 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/together.py
+-rw-r--r--   0        0        0    13132 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/tongyi.py
+-rw-r--r--   0        0        0      258 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/utils.py
+-rw-r--r--   0        0        0    19304 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/vertexai.py
+-rw-r--r--   0        0        0     5592 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/vllm.py
+-rw-r--r--   0        0        0     6591 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/volcengine_maas.py
+-rw-r--r--   0        0        0    15085 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/watsonxllm.py
+-rw-r--r--   0        0        0     8924 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/weight_only_quantization.py
+-rw-r--r--   0        0        0     4970 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/writer.py
+-rw-r--r--   0        0        0     6332 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/xinference.py
+-rw-r--r--   0        0        0    13008 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/yandex.py
+-rw-r--r--   0        0        0     5968 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/llms/yuan2.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/memory/__init__.py
+-rw-r--r--   0        0        0     5632 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/memory/kg.py
+-rw-r--r--   0        0        0     3600 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/memory/motorhead_memory.py
+-rw-r--r--   0        0        0     5623 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/memory/zep_memory.py
+-rw-r--r--   0        0        0      292 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/output_parsers/__init__.py
+-rw-r--r--   0        0        0     6701 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/output_parsers/ernie_functions.py
+-rw-r--r--   0        0        0     3283 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/output_parsers/rail_parser.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/py.typed
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/astradb.py
+-rw-r--r--   0        0        0     1468 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/chroma.py
+-rw-r--r--   0        0        0     1912 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/dashvector.py
+-rw-r--r--   0        0        0     3144 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/databricks_vector_search.py
+-rw-r--r--   0        0        0     2625 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/deeplake.py
+-rw-r--r--   0        0        0     1343 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/dingo.py
+-rw-r--r--   0        0        0     3267 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/elasticsearch.py
+-rw-r--r--   0        0        0     3346 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/milvus.py
+-rw-r--r--   0        0        0     2297 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/mongodb_atlas.py
+-rw-r--r--   0        0        0     3630 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/myscale.py
+-rw-r--r--   0        0        0     3265 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/opensearch.py
+-rw-r--r--   0        0        0     1523 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/pgvector.py
+-rw-r--r--   0        0        0     1704 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/pinecone.py
+-rw-r--r--   0        0        0     3162 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/qdrant.py
+-rw-r--r--   0        0        0     3370 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/redis.py
+-rw-r--r--   0        0        0     2968 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/supabase.py
+-rw-r--r--   0        0        0     3703 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/tencentvectordb.py
+-rw-r--r--   0        0        0     2627 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/timescalevector.py
+-rw-r--r--   0        0        0     2158 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/vectara.py
+-rw-r--r--   0        0        0     2613 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/query_constructors/weaviate.py
+-rw-r--r--   0        0        0     9161 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/__init__.py
+-rw-r--r--   0        0        0     4297 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/arcee.py
+-rw-r--r--   0        0        0      773 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/arxiv.py
+-rw-r--r--   0        0        0     5098 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/azure_ai_search.py
+-rw-r--r--   0        0        0     4766 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/bedrock.py
+-rw-r--r--   0        0        0     3713 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/bm25.py
+-rw-r--r--   0        0        0     1524 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/breebs.py
+-rw-r--r--   0        0        0     2684 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/chaindesk.py
+-rw-r--r--   0        0        0     3024 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/chatgpt_plugin_retriever.py
+-rw-r--r--   0        0        0     3088 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/cohere_rag_retriever.py
+-rw-r--r--   0        0        0     2338 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/databerry.py
+-rw-r--r--   0        0        0     6778 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/docarray.py
+-rw-r--r--   0        0        0     2763 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/dria_index.py
+-rw-r--r--   0        0        0     4640 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/elastic_search_bm25.py
+-rw-r--r--   0        0        0     2087 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/embedchain.py
+-rw-r--r--   0        0        0     4763 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/google_cloud_documentai_warehouse.py
+-rw-r--r--   0        0        0    18798 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/google_vertex_ai_search.py
+-rw-r--r--   0        0        0     1985 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/kay.py
+-rw-r--r--   0        0        0    15685 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/kendra.py
+-rw-r--r--   0        0        0     3323 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/knn.py
+-rw-r--r--   0        0        0     3166 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/llama_index.py
+-rw-r--r--   0        0        0     1486 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/metal.py
+-rw-r--r--   0        0        0     2523 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/milvus.py
+-rw-r--r--   0        0        0      644 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/outline.py
+-rw-r--r--   0        0        0     5733 2024-05-09 22:13:05.498945 langchain_community-0.2.0rc1/langchain_community/retrievers/pinecone_hybrid_search.py
+-rw-r--r--   0        0        0      643 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/pubmed.py
+-rw-r--r--   0        0        0      104 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/pupmed.py
+-rw-r--r--   0        0        0     7539 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/qdrant_sparse_vector_retriever.py
+-rw-r--r--   0        0        0      670 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/rememberizer.py
+-rw-r--r--   0        0        0     1935 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/remote_retriever.py
+-rw-r--r--   0        0        0     4131 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/svm.py
+-rw-r--r--   0        0        0     2855 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/tavily_search_api.py
+-rw-r--r--   0        0        0     5569 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/tfidf.py
+-rw-r--r--   0        0        0     9288 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/thirdai_neuraldb.py
+-rw-r--r--   0        0        0     4555 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/vespa_retriever.py
+-rw-r--r--   0        0        0     6195 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/weaviate_hybrid_search.py
+-rw-r--r--   0        0        0     8197 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/web_research.py
+-rw-r--r--   0        0        0      656 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/wikipedia.py
+-rw-r--r--   0        0        0     1124 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/you.py
+-rw-r--r--   0        0        0     5904 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/zep.py
+-rw-r--r--   0        0        0     2719 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/retrievers/zilliz.py
+-rw-r--r--   0        0        0     1643 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/storage/__init__.py
+-rw-r--r--   0        0        0     8691 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/storage/astradb.py
+-rw-r--r--   0        0        0       89 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/storage/exceptions.py
+-rw-r--r--   0        0        0     4375 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/storage/mongodb.py
+-rw-r--r--   0        0        0     4802 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/storage/redis.py
+-rw-r--r--   0        0        0     5762 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/storage/upstash_redis.py
+-rw-r--r--   0        0        0    23154 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/__init__.py
+-rw-r--r--   0        0        0     3185 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/app.py
+-rw-r--r--   0        0        0     2109 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/base.py
+-rw-r--r--   0        0        0     4140 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/owner.py
+-rw-r--r--   0        0        0     2746 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/rule.py
+-rw-r--r--   0        0        0     1074 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/transfer.py
+-rw-r--r--   0        0        0     2314 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/utils.py
+-rw-r--r--   0        0        0     2624 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/value.py
+-rw-r--r--   0        0        0      257 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/amadeus/__init__.py
+-rw-r--r--   0        0        0      435 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/amadeus/base.py
+-rw-r--r--   0        0        0     2338 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/amadeus/closest_airport.py
+-rw-r--r--   0        0        0     5771 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/amadeus/flight_search.py
+-rw-r--r--   0        0        0     1276 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/amadeus/utils.py
+-rw-r--r--   0        0        0       25 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/arxiv/__init__.py
+-rw-r--r--   0        0        0     1228 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/arxiv/tool.py
+-rw-r--r--   0        0        0      188 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/audio/__init__.py
+-rw-r--r--   0        0        0     3724 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/audio/huggingface_text_to_speech_inference.py
+-rw-r--r--   0        0        0      858 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/__init__.py
+-rw-r--r--   0        0        0     5486 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/document_intelligence.py
+-rw-r--r--   0        0        0     5735 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/image_analysis.py
+-rw-r--r--   0        0        0     4430 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/speech_to_text.py
+-rw-r--r--   0        0        0     3601 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/text_analytics_for_health.py
+-rw-r--r--   0        0        0     3811 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/text_to_speech.py
+-rw-r--r--   0        0        0      776 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/utils.py
+-rw-r--r--   0        0        0      802 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/__init__.py
+-rw-r--r--   0        0        0     5375 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/form_recognizer.py
+-rw-r--r--   0        0        0     5304 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/image_analysis.py
+-rw-r--r--   0        0        0     4336 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/speech2text.py
+-rw-r--r--   0        0        0     3675 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/text2speech.py
+-rw-r--r--   0        0        0     3542 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/text_analytics_health.py
+-rw-r--r--   0        0        0      776 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/utils.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/bearly/__init__.py
+-rw-r--r--   0        0        0     5562 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/bearly/tool.py
+-rw-r--r--   0        0        0      170 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/bing_search/__init__.py
+-rw-r--r--   0        0        0     1463 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/bing_search/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/brave_search/__init__.py
+-rw-r--r--   0        0        0     1354 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/brave_search/tool.py
+-rw-r--r--   0        0        0       23 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/cassandra_database/__init__.py
+-rw-r--r--   0        0        0     1221 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/cassandra_database/prompt.py
+-rw-r--r--   0        0        0     4924 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/cassandra_database/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/clickup/__init__.py
+-rw-r--r--   0        0        0     8298 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/clickup/prompt.py
+-rw-r--r--   0        0        0     1230 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/clickup/tool.py
+-rw-r--r--   0        0        0       20 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/cogniswitch/__init__.py
+-rw-r--r--   0        0        0    13896 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/cogniswitch/tool.py
+-rw-r--r--   0        0        0      188 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/connery/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/connery/models.py
+-rw-r--r--   0        0        0     5741 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/connery/service.py
+-rw-r--r--   0        0        0     5552 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/connery/tool.py
+-rw-r--r--   0        0        0      198 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/convert_to_openai.py
+-rw-r--r--   0        0        0      268 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/dataforseo_api_search/__init__.py
+-rw-r--r--   0        0        0     2214 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/dataforseo_api_search/tool.py
+-rw-r--r--   0        0        0      148 2024-05-09 22:13:05.502945 langchain_community-0.2.0rc1/langchain_community/tools/dataherald/__init__.py
+-rw-r--r--   0        0        0     1063 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/dataherald/tool.py
+-rw-r--r--   0        0        0      147 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/ddg_search/__init__.py
+-rw-r--r--   0        0        0     2641 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/ddg_search/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/e2b_data_analysis/__init__.py
+-rw-r--r--   0        0        0     8015 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/e2b_data_analysis/tool.py
+-rw-r--r--   0        0        0    20667 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/e2b_data_analysis/unparse.py
+-rw-r--r--   0        0        0     1024 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/__init__.py
+-rw-r--r--   0        0        0     3465 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/audio_speech_to_text.py
+-rw-r--r--   0        0        0     3885 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/audio_text_to_speech.py
+-rw-r--r--   0        0        0     5386 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/edenai_base_tool.py
+-rw-r--r--   0        0        0     2249 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/image_explicitcontent.py
+-rw-r--r--   0        0        0     2476 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/image_objectdetection.py
+-rw-r--r--   0        0        0     1966 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/ocr_identityparser.py
+-rw-r--r--   0        0        0     2187 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/ocr_invoiceparser.py
+-rw-r--r--   0        0        0     2407 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/edenai/text_moderation.py
+-rw-r--r--   0        0        0      164 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/eleven_labs/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/eleven_labs/models.py
+-rw-r--r--   0        0        0     2709 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/eleven_labs/text2speech.py
+-rw-r--r--   0        0        0      723 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/__init__.py
+-rw-r--r--   0        0        0     1749 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/copy.py
+-rw-r--r--   0        0        0     1345 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/delete.py
+-rw-r--r--   0        0        0     1965 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/file_search.py
+-rw-r--r--   0        0        0     1432 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/list_dir.py
+-rw-r--r--   0        0        0     1889 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/move.py
+-rw-r--r--   0        0        0     1340 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/read.py
+-rw-r--r--   0        0        0     1726 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/utils.py
+-rw-r--r--   0        0        0     1614 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/file_management/write.py
+-rw-r--r--   0        0        0       20 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/github/__init__.py
+-rw-r--r--   0        0        0     6220 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/github/prompt.py
+-rw-r--r--   0        0        0     1194 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/github/tool.py
+-rw-r--r--   0        0        0       20 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gitlab/__init__.py
+-rw-r--r--   0        0        0     3438 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gitlab/prompt.py
+-rw-r--r--   0        0        0      972 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gitlab/tool.py
+-rw-r--r--   0        0        0      601 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/__init__.py
+-rw-r--r--   0        0        0     1004 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/base.py
+-rw-r--r--   0        0        0     2564 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/create_draft.py
+-rw-r--r--   0        0        0     2202 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/get_message.py
+-rw-r--r--   0        0        0     1560 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/get_thread.py
+-rw-r--r--   0        0        0     5111 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/search.py
+-rw-r--r--   0        0        0     2939 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/send_message.py
+-rw-r--r--   0        0        0     4109 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/gmail/utils.py
+-rw-r--r--   0        0        0      136 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/golden_query/__init__.py
+-rw-r--r--   0        0        0     1108 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/golden_query/tool.py
+-rw-r--r--   0        0        0      171 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_cloud/__init__.py
+-rw-r--r--   0        0        0     3354 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_cloud/texttospeech.py
+-rw-r--r--   0        0        0      152 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_finance/__init__.py
+-rw-r--r--   0        0        0      854 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_finance/tool.py
+-rw-r--r--   0        0        0      140 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_jobs/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_jobs/tool.py
+-rw-r--r--   0        0        0      140 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_lens/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_lens/tool.py
+-rw-r--r--   0        0        0      140 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_places/__init__.py
+-rw-r--r--   0        0        0     1322 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_places/tool.py
+-rw-r--r--   0        0        0      152 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_scholar/__init__.py
+-rw-r--r--   0        0        0      847 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_scholar/tool.py
+-rw-r--r--   0        0        0      195 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_search/__init__.py
+-rw-r--r--   0        0        0     1798 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_search/tool.py
+-rw-r--r--   0        0        0      243 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_serper/__init__.py
+-rw-r--r--   0        0        0     2113 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_serper/tool.py
+-rw-r--r--   0        0        0      148 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_trends/__init__.py
+-rw-r--r--   0        0        0      844 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/google_trends/tool.py
+-rw-r--r--   0        0        0       47 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/graphql/__init__.py
+-rw-r--r--   0        0        0     1204 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/graphql/tool.py
+-rw-r--r--   0        0        0      132 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/human/__init__.py
+-rw-r--r--   0        0        0     1011 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/human/tool.py
+-rw-r--r--   0        0        0     2286 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/ifttt.py
+-rw-r--r--   0        0        0       43 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/interaction/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/interaction/tool.py
+-rw-r--r--   0        0        0       17 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/jira/__init__.py
+-rw-r--r--   0        0        0     3170 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/jira/prompt.py
+-rw-r--r--   0        0        0     1342 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/jira/tool.py
+-rw-r--r--   0        0        0       46 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/json/__init__.py
+-rw-r--r--   0        0        0     4139 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/json/tool.py
+-rw-r--r--   0        0        0      134 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/memorize/__init__.py
+-rw-r--r--   0        0        0     1828 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/memorize/tool.py
+-rw-r--r--   0        0        0       35 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/merriam_webster/__init__.py
+-rw-r--r--   0        0        0      854 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/merriam_webster/tool.py
+-rw-r--r--   0        0        0      154 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/metaphor_search/__init__.py
+-rw-r--r--   0        0        0     2851 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/metaphor_search/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.506945 langchain_community-0.2.0rc1/langchain_community/tools/mojeek_search/__init__.py
+-rw-r--r--   0        0        0     1307 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/mojeek_search/tool.py
+-rw-r--r--   0        0        0      359 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/multion/__init__.py
+-rw-r--r--   0        0        0     1765 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/multion/close_session.py
+-rw-r--r--   0        0        0     2199 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/multion/create_session.py
+-rw-r--r--   0        0        0     2415 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/multion/update_session.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/nasa/__init__.py
+-rw-r--r--   0        0        0     5197 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/nasa/prompt.py
+-rw-r--r--   0        0        0      831 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/nasa/tool.py
+-rw-r--r--   0        0        0      111 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/nuclia/__init__.py
+-rw-r--r--   0        0        0     7915 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/nuclia/tool.py
+-rw-r--r--   0        0        0      654 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/__init__.py
+-rw-r--r--   0        0        0      508 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/base.py
+-rw-r--r--   0        0        0     1858 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/create_draft_message.py
+-rw-r--r--   0        0        0     4821 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/events_search.py
+-rw-r--r--   0        0        0     4235 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/messages_search.py
+-rw-r--r--   0        0        0     2898 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/send_event.py
+-rw-r--r--   0        0        0     1777 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/send_message.py
+-rw-r--r--   0        0        0     2228 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/office365/utils.py
+-rw-r--r--   0        0        0      219 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openai_dalle_image_generation/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openai_dalle_image_generation/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openapi/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openapi/utils/__init__.py
+-rw-r--r--   0        0        0    21288 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openapi/utils/api_models.py
+-rw-r--r--   0        0        0      191 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openapi/utils/openapi_utils.py
+-rw-r--r--   0        0        0      162 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openweathermap/__init__.py
+-rw-r--r--   0        0        0      968 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/openweathermap/tool.py
+-rw-r--r--   0        0        0      142 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/passio_nutrition_ai/__init__.py
+-rw-r--r--   0        0        0     1143 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/passio_nutrition_ai/tool.py
+-rw-r--r--   0        0        0      763 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/__init__.py
+-rw-r--r--   0        0        0     1924 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/base.py
+-rw-r--r--   0        0        0     3083 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/click.py
+-rw-r--r--   0        0        0     1340 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/current_page.py
+-rw-r--r--   0        0        0     3051 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/extract_hyperlinks.py
+-rw-r--r--   0        0        0     2383 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/extract_text.py
+-rw-r--r--   0        0        0     3743 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/get_elements.py
+-rw-r--r--   0        0        0     2878 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/navigate.py
+-rw-r--r--   0        0        0     1926 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/navigate_back.py
+-rw-r--r--   0        0        0     3049 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/playwright/utils.py
+-rw-r--r--   0        0        0     2902 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/plugin.py
+-rw-r--r--   0        0        0      439 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/polygon/__init__.py
+-rw-r--r--   0        0        0     2558 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/polygon/aggregates.py
+-rw-r--r--   0        0        0     1197 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/polygon/financials.py
+-rw-r--r--   0        0        0     1070 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/polygon/last_quote.py
+-rw-r--r--   0        0        0     1076 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/polygon/ticker_news.py
+-rw-r--r--   0        0        0       52 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/powerbi/__init__.py
+-rw-r--r--   0        0        0     7339 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/powerbi/prompt.py
+-rw-r--r--   0        0        0    11075 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/powerbi/tool.py
+-rw-r--r--   0        0        0       26 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/pubmed/__init__.py
+-rw-r--r--   0        0        0      945 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/pubmed/tool.py
+-rw-r--r--   0        0        0     1965 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/reddit_search/tool.py
+-rw-r--r--   0        0        0      198 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/render.py
+-rw-r--r--   0        0        0       52 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/requests/__init__.py
+-rw-r--r--   0        0        0     7445 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/requests/tool.py
+-rw-r--r--   0        0        0       31 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/scenexplain/__init__.py
+-rw-r--r--   0        0        0     1100 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/scenexplain/tool.py
+-rw-r--r--   0        0        0      214 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/searchapi/__init__.py
+-rw-r--r--   0        0        0     2114 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/searchapi/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/searx_search/__init__.py
+-rw-r--r--   0        0        0     2261 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/searx_search/tool.py
+-rw-r--r--   0        0        0       36 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/semanticscholar/__init__.py
+-rw-r--r--   0        0        0     1190 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/semanticscholar/tool.py
+-rw-r--r--   0        0        0      103 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/shell/__init__.py
+-rw-r--r--   0        0        0     3143 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/shell/tool.py
+-rw-r--r--   0        0        0      502 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/slack/__init__.py
+-rw-r--r--   0        0        0      460 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/slack/base.py
+-rw-r--r--   0        0        0     1193 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/slack/get_channel.py
+-rw-r--r--   0        0        0     1422 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/slack/get_message.py
+-rw-r--r--   0        0        0     2071 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/slack/schedule_message.py
+-rw-r--r--   0        0        0     1222 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/slack/send_message.py
+-rw-r--r--   0        0        0     1135 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/slack/utils.py
+-rw-r--r--   0        0        0       18 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/sleep/__init__.py
+-rw-r--r--   0        0        0     1229 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/sleep/tool.py
+-rw-r--r--   0        0        0       44 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/spark_sql/__init__.py
+-rw-r--r--   0        0        0      550 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/spark_sql/prompt.py
+-rw-r--r--   0        0        0     4376 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/spark_sql/tool.py
+-rw-r--r--   0        0        0       49 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/sql_database/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-09 22:13:05.510945 langchain_community-0.2.0rc1/langchain_community/tools/sql_database/prompt.py
+-rw-r--r--   0        0        0     5326 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/sql_database/tool.py
+-rw-r--r--   0        0        0       33 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/stackexchange/__init__.py
+-rw-r--r--   0        0        0      869 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/stackexchange/tool.py
+-rw-r--r--   0        0        0       24 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/steam/__init__.py
+-rw-r--r--   0        0        0     1657 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/steam/prompt.py
+-rw-r--r--   0        0        0      842 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/steam/tool.py
+-rw-r--r--   0        0        0      186 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/steamship_image_generation/__init__.py
+-rw-r--r--   0        0        0     3378 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/steamship_image_generation/tool.py
+-rw-r--r--   0        0        0     1395 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/steamship_image_generation/utils.py
+-rw-r--r--   0        0        0      189 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/tavily_search/__init__.py
+-rw-r--r--   0        0        0     3375 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/tavily_search/tool.py
+-rw-r--r--   0        0        0       51 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/vectorstore/__init__.py
+-rw-r--r--   0        0        0     4717 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/vectorstore/tool.py
+-rw-r--r--   0        0        0       28 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/wikidata/__init__.py
+-rw-r--r--   0        0        0      926 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/wikidata/tool.py
+-rw-r--r--   0        0        0       29 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/wikipedia/__init__.py
+-rw-r--r--   0        0        0      867 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/wikipedia/tool.py
+-rw-r--r--   0        0        0      156 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/wolfram_alpha/tool.py
+-rw-r--r--   0        0        0     2753 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/yahoo_finance_news.py
+-rw-r--r--   0        0        0      126 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/you/__init__.py
+-rw-r--r--   0        0        0     1355 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/you/tool.py
+-rw-r--r--   0        0        0        0 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/youtube/__init__.py
+-rw-r--r--   0        0        0     1729 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/youtube/search.py
+-rw-r--r--   0        0        0      193 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/zapier/__init__.py
+-rw-r--r--   0        0        0     1182 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/zapier/prompt.py
+-rw-r--r--   0        0        0     7812 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/tools/zapier/tool.py
+-rw-r--r--   0        0        0    11061 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/__init__.py
+-rw-r--r--   0        0        0     5918 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/alpha_vantage.py
+-rw-r--r--   0        0        0      844 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/anthropic.py
+-rw-r--r--   0        0        0     8458 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/apify.py
+-rw-r--r--   0        0        0     8710 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/arcee.py
+-rw-r--r--   0        0        0    10021 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/arxiv.py
+-rw-r--r--   0        0        0     6104 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/astradb.py
+-rw-r--r--   0        0        0     2437 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/awslambda.py
+-rw-r--r--   0        0        0     2499 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/bibtex.py
+-rw-r--r--   0        0        0     3608 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/bing_search.py
+-rw-r--r--   0        0        0     2382 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/brave_search.py
+-rw-r--r--   0        0        0     1164 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/cassandra.py
+-rw-r--r--   0        0        0    24429 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/cassandra_database.py
+-rw-r--r--   0        0        0    19876 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/clickup.py
+-rw-r--r--   0        0        0     6377 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/dalle_image_generator.py
+-rw-r--r--   0        0        0     7854 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/dataforseo_api_search.py
+-rw-r--r--   0        0        0     2067 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/dataherald.py
+-rw-r--r--   0        0        0     3351 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/dria_index.py
+-rw-r--r--   0        0        0     4310 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/duckduckgo_search.py
+-rw-r--r--   0        0        0    32246 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/github.py
+-rw-r--r--   0        0        0    11975 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/gitlab.py
+-rw-r--r--   0        0        0     1858 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/golden_query.py
+-rw-r--r--   0        0        0     3400 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_finance.py
+-rw-r--r--   0        0        0     2804 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_jobs.py
+-rw-r--r--   0        0        0     3017 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_lens.py
+-rw-r--r--   0        0        0     4293 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_places_api.py
+-rw-r--r--   0        0        0     5171 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_scholar.py
+-rw-r--r--   0        0        0     5236 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_search.py
+-rw-r--r--   0        0        0     6503 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_serper.py
+-rw-r--r--   0        0        0     4164 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/google_trends.py
+-rw-r--r--   0        0        0     2089 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/graphql.py
+-rw-r--r--   0        0        0     5891 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/infobip.py
+-rw-r--r--   0        0        0     6195 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/jira.py
+-rw-r--r--   0        0        0     2647 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/max_compute.py
+-rw-r--r--   0        0        0     3748 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/merriam_webster.py
+-rw-r--r--   0        0        0     6809 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/metaphor_search.py
+-rw-r--r--   0        0        0     1319 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/mojeek_search.py
+-rw-r--r--   0        0        0     1820 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/nasa.py
+-rw-r--r--   0        0        0    21608 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/nvidia_riva.py
+-rw-r--r--   0        0        0     3287 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/opaqueprompts.py
+-rw-r--r--   0        0        0    11017 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/openapi.py
+-rw-r--r--   0        0        0     2462 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/openweathermap.py
+-rw-r--r--   0        0        0     6224 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/oracleai.py
+-rw-r--r--   0        0        0     3351 2024-05-09 22:13:05.514945 langchain_community-0.2.0rc1/langchain_community/utilities/outline.py
+-rw-r--r--   0        0        0     5613 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/passio_nutrition_ai.py
+-rw-r--r--   0        0        0     8856 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/pebblo.py
+-rw-r--r--   0        0        0     4309 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/polygon.py
+-rw-r--r--   0        0        0     2355 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/portkey.py
+-rw-r--r--   0        0        0    11245 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/powerbi.py
+-rw-r--r--   0        0        0     6950 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/pubmed.py
+-rw-r--r--   0        0        0     2159 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/python.py
+-rw-r--r--   0        0        0     4474 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/reddit_search.py
+-rw-r--r--   0        0        0     8221 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/redis.py
+-rw-r--r--   0        0        0     1650 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/rememberizer.py
+-rw-r--r--   0        0        0     8793 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/requests.py
+-rw-r--r--   0        0        0     2220 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/scenexplain.py
+-rw-r--r--   0        0        0     5226 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/searchapi.py
+-rw-r--r--   0        0        0    16653 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/searx_search.py
+-rw-r--r--   0        0        0     2789 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/semanticscholar.py
+-rw-r--r--   0        0        0     8704 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/serpapi.py
+-rw-r--r--   0        0        0     7520 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/spark_sql.py
+-rw-r--r--   0        0        0    22814 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/sql_database.py
+-rw-r--r--   0        0        0     2639 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/stackexchange.py
+-rw-r--r--   0        0        0     5857 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/steam.py
+-rw-r--r--   0        0        0     6889 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/tavily_search.py
+-rw-r--r--   0        0        0     4006 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/tensorflow_datasets.py
+-rw-r--r--   0        0        0     3441 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/twilio.py
+-rw-r--r--   0        0        0     4087 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/vertexai.py
+-rw-r--r--   0        0        0     5346 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/wikidata.py
+-rw-r--r--   0        0        0     4270 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/wikipedia.py
+-rw-r--r--   0        0        0     2011 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/wolfram_alpha.py
+-rw-r--r--   0        0        0     7951 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/you.py
+-rw-r--r--   0        0        0    11666 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utilities/zapier.py
+-rw-r--r--   0        0        0       45 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utils/__init__.py
+-rw-r--r--   0        0        0     1509 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utils/ernie_functions.py
+-rw-r--r--   0        0        0      775 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utils/google.py
+-rw-r--r--   0        0        0     2724 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utils/math.py
+-rw-r--r--   0        0        0      264 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utils/openai.py
+-rw-r--r--   0        0        0      377 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/utils/openai_functions.py
+-rw-r--r--   0        0        0    16943 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/__init__.py
+-rw-r--r--   0        0        0    19806 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/alibabacloud_opensearch.py
+-rw-r--r--   0        0        0    15752 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/analyticdb.py
+-rw-r--r--   0        0        0    17889 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/annoy.py
+-rw-r--r--   0        0        0    17067 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/apache_doris.py
+-rw-r--r--   0        0        0    46743 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/astradb.py
+-rw-r--r--   0        0        0    12136 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/atlas.py
+-rw-r--r--   0        0        0    21155 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/awadb.py
+-rw-r--r--   0        0        0    20882 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/azure_cosmos_db.py
+-rw-r--r--   0        0        0    28996 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/azuresearch.py
+-rw-r--r--   0        0        0    15245 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/bagel.py
+-rw-r--r--   0        0        0       78 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/bageldb.py
+-rw-r--r--   0        0        0    16548 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/baiducloud_vector_search.py
+-rw-r--r--   0        0        0    15271 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/baiduvectordb.py
+-rw-r--r--   0        0        0    34562 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/bigquery_vector_search.py
+-rw-r--r--   0        0        0    34718 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/cassandra.py
+-rw-r--r--   0        0        0    31090 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/chroma.py
+-rw-r--r--   0        0        0    12095 2024-05-09 22:13:05.518945 langchain_community-0.2.0rc1/langchain_community/vectorstores/clarifai.py
+-rw-r--r--   0        0        0    22074 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/clickhouse.py
+-rw-r--r--   0        0        0    22766 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/couchbase.py
+-rw-r--r--   0        0        0    13946 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/dashvector.py
+-rw-r--r--   0        0        0    23115 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/databricks_vector_search.py
+-rw-r--r--   0        0        0    43000 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/deeplake.py
+-rw-r--r--   0        0        0    13208 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/dingo.py
+-rw-r--r--   0        0        0      236 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/docarray/__init__.py
+-rw-r--r--   0        0        0     7021 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/docarray/base.py
+-rw-r--r--   0        0        0     4042 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/docarray/hnsw.py
+-rw-r--r--   0        0        0     2418 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/docarray/in_memory.py
+-rw-r--r--   0        0        0    11947 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/documentdb.py
+-rw-r--r--   0        0        0     9991 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/duckdb.py
+-rw-r--r--   0        0        0    20611 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/ecloud_vector_search.py
+-rw-r--r--   0        0        0    29007 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/elastic_vector_search.py
+-rw-r--r--   0        0        0    48577 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/elasticsearch.py
+-rw-r--r--   0        0        0    14183 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/epsilla.py
+-rw-r--r--   0        0        0    45886 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/faiss.py
+-rw-r--r--   0        0        0    25861 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/hanavector.py
+-rw-r--r--   0        0        0    26837 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/hippo.py
+-rw-r--r--   0        0        0    13642 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/hologres.py
+-rw-r--r--   0        0        0    21348 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/infinispanvs.py
+-rw-r--r--   0        0        0     6299 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/inmemory.py
+-rw-r--r--   0        0        0    14581 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/jaguar.py
+-rw-r--r--   0        0        0     9087 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/kdbai.py
+-rw-r--r--   0        0        0    34973 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/kinetica.py
+-rw-r--r--   0        0        0    10875 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/lancedb.py
+-rw-r--r--   0        0        0    38505 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/lantern.py
+-rw-r--r--   0        0        0     7745 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/llm_rails.py
+-rw-r--r--   0        0        0    17075 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/marqo.py
+-rw-r--r--   0        0        0    21617 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/matching_engine.py
+-rw-r--r--   0        0        0    12086 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/meilisearch.py
+-rw-r--r--   0        0        0    41955 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/milvus.py
+-rw-r--r--   0        0        0    19047 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/momento_vector_index.py
+-rw-r--r--   0        0        0    13700 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/mongodb_atlas.py
+-rw-r--r--   0        0        0    22612 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/myscale.py
+-rw-r--r--   0        0        0    53077 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/neo4j_vector.py
+-rw-r--r--   0        0        0     5404 2024-05-09 22:13:05.522945 langchain_community-0.2.0rc1/langchain_community/vectorstores/nucliadb.py
+-rw-r--r--   0        0        0    51650 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/opensearch_vector_search.py
+-rw-r--r--   0        0        0    32081 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/oraclevs.py
+-rw-r--r--   0        0        0     7709 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/pathway.py
+-rw-r--r--   0        0        0    17949 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/pgembedding.py
+-rw-r--r--   0        0        0     7838 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/pgvecto_rs.py
+-rw-r--r--   0        0        0    51715 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/pgvector.py
+-rw-r--r--   0        0        0    17678 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/pinecone.py
+-rw-r--r--   0        0        0    94133 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      265 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/__init__.py
+-rw-r--r--   0        0        0    56021 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/base.py
+-rw-r--r--   0        0        0      420 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/constants.py
+-rw-r--r--   0        0        0    16219 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/filters.py
+-rw-r--r--   0        0        0    10418 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/schema.py
+-rw-r--r--   0        0        0    18388 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/relyt.py
+-rw-r--r--   0        0        0    15235 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/rocksetdb.py
+-rw-r--r--   0        0        0    20867 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/scann.py
+-rw-r--r--   0        0        0     9721 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/semadb.py
+-rw-r--r--   0        0        0    45305 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/singlestoredb.py
+-rw-r--r--   0        0        0    12372 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/sklearn.py
+-rw-r--r--   0        0        0     7302 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/sqlitevss.py
+-rw-r--r--   0        0        0    17220 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/starrocks.py
+-rw-r--r--   0        0        0    15689 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/supabase.py
+-rw-r--r--   0        0        0    15428 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/surrealdb.py
+-rw-r--r--   0        0        0     9559 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/tair.py
+-rw-r--r--   0        0        0    20524 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/tencentvectordb.py
+-rw-r--r--   0        0        0    17534 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/thirdai_neuraldb.py
+-rw-r--r--   0        0        0    13630 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/tidb_vector.py
+-rw-r--r--   0        0        0     4927 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/tigris.py
+-rw-r--r--   0        0        0    29856 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/tiledb.py
+-rw-r--r--   0        0        0    29831 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/timescalevector.py
+-rw-r--r--   0        0        0     9713 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/typesense.py
+-rw-r--r--   0        0        0    33147 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/upstash.py
+-rw-r--r--   0        0        0     5888 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/usearch.py
+-rw-r--r--   0        0        0     2474 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/utils.py
+-rw-r--r--   0        0        0    12898 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/vald.py
+-rw-r--r--   0        0        0    53231 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/vdms.py
+-rw-r--r--   0        0        0    19845 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/vearch.py
+-rw-r--r--   0        0        0    21908 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/vectara.py
+-rw-r--r--   0        0        0     9785 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/vespa.py
+-rw-r--r--   0        0        0    15510 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/vikingdb.py
+-rw-r--r--   0        0        0     8145 2024-05-09 22:13:05.526945 langchain_community-0.2.0rc1/langchain_community/vectorstores/vlite.py
+-rw-r--r--   0        0        0    19253 2024-05-09 22:13:05.530945 langchain_community-0.2.0rc1/langchain_community/vectorstores/weaviate.py
+-rw-r--r--   0        0        0     9018 2024-05-09 22:13:05.530945 langchain_community-0.2.0rc1/langchain_community/vectorstores/xata.py
+-rw-r--r--   0        0        0    34543 2024-05-09 22:13:05.530945 langchain_community-0.2.0rc1/langchain_community/vectorstores/yellowbrick.py
+-rw-r--r--   0        0        0    23192 2024-05-09 22:13:05.530945 langchain_community-0.2.0rc1/langchain_community/vectorstores/zep.py
+-rw-r--r--   0        0        0     8255 2024-05-09 22:13:05.530945 langchain_community-0.2.0rc1/langchain_community/vectorstores/zilliz.py
+-rw-r--r--   0        0        0    11111 2024-05-09 22:13:05.530945 langchain_community-0.2.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     8792 1970-01-01 00:00:00.000000 langchain_community-0.2.0rc1/PKG-INFO
```

### Comparing `langchain_community-0.2.0/README.md` & `langchain_community-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/adapters/openai.py` & `langchain_community-0.2.0rc1/langchain_community/adapters/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,26 +91,26 @@
             additional_kwargs["function_call"] = dict(function_call)
         if tool_calls := _dict.get("tool_calls"):
             additional_kwargs["tool_calls"] = tool_calls
         return AIMessage(content=content, additional_kwargs=additional_kwargs)
     elif role == "system":
         return SystemMessage(content=_dict.get("content", ""))
     elif role == "function":
-        return FunctionMessage(content=_dict.get("content", ""), name=_dict.get("name"))  # type: ignore[arg-type]
+        return FunctionMessage(content=_dict.get("content", ""), name=_dict.get("name"))
     elif role == "tool":
         additional_kwargs = {}
         if "name" in _dict:
             additional_kwargs["name"] = _dict["name"]
         return ToolMessage(
             content=_dict.get("content", ""),
-            tool_call_id=_dict.get("tool_call_id"),  # type: ignore[arg-type]
+            tool_call_id=_dict.get("tool_call_id"),
             additional_kwargs=additional_kwargs,
         )
     else:
-        return ChatMessage(content=_dict.get("content", ""), role=role)  # type: ignore[arg-type]
+        return ChatMessage(content=_dict.get("content", ""), role=role)
 
 
 def convert_message_to_dict(message: BaseMessage) -> dict:
     """Convert a LangChain message to a dictionary.
 
     Args:
         message: The LangChain message.
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/ainetwork/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/ainetwork/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/amadeus/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/amadeus/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/azure_cognitive_services.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/connery/toolkit.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,50 @@
-from __future__ import annotations
-
-import sys
 from typing import List
 
+from langchain_core.pydantic_v1 import root_validator
 from langchain_core.tools import BaseTool, BaseToolkit
 
-from langchain_community.tools.azure_cognitive_services import (
-    AzureCogsFormRecognizerTool,
-    AzureCogsImageAnalysisTool,
-    AzureCogsSpeech2TextTool,
-    AzureCogsText2SpeechTool,
-    AzureCogsTextAnalyticsHealthTool,
-)
+from langchain_community.tools.connery import ConneryService
+
 
+class ConneryToolkit(BaseToolkit):
+    """
+    Toolkit with a list of Connery Actions as tools.
+    """
 
-class AzureCognitiveServicesToolkit(BaseToolkit):
-    """Toolkit for Azure Cognitive Services."""
+    tools: List[BaseTool]
 
     def get_tools(self) -> List[BaseTool]:
-        """Get the tools in the toolkit."""
+        """
+        Returns the list of Connery Actions.
+        """
+        return self.tools
+
+    @root_validator()
+    def validate_attributes(cls, values: dict) -> dict:
+        """
+        Validate the attributes of the ConneryToolkit class.
+        Parameters:
+            values (dict): The arguments to validate.
+        Returns:
+            dict: The validated arguments.
+        """
+
+        if not values.get("tools"):
+            raise ValueError("The attribute 'tools' must be set.")
+
+        return values
+
+    @classmethod
+    def create_instance(cls, connery_service: ConneryService) -> "ConneryToolkit":
+        """
+        Creates a Connery Toolkit using a Connery Service.
+        Parameters:
+            connery_service (ConneryService): The Connery Service
+            to to get the list of Connery Actions.
+        Returns:
+            ConneryToolkit: The Connery Toolkit.
+        """
+
+        instance = cls(tools=connery_service.list_actions())
 
-        tools: List[BaseTool] = [
-            AzureCogsFormRecognizerTool(),  # type: ignore[call-arg]
-            AzureCogsSpeech2TextTool(),  # type: ignore[call-arg]
-            AzureCogsText2SpeechTool(),  # type: ignore[call-arg]
-            AzureCogsTextAnalyticsHealthTool(),  # type: ignore[call-arg]
-        ]
-
-        # TODO: Remove check once azure-ai-vision supports MacOS.
-        if sys.platform.startswith("linux") or sys.platform.startswith("win"):
-            tools.append(AzureCogsImageAnalysisTool())  # type: ignore[call-arg]
-        return tools
+        return instance
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/cassandra_database/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/cassandra_database/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/clickup/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/clickup/toolkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,12 +98,12 @@
                 name=action["name"],
                 description=action["description"],
                 mode=action["mode"],
                 api_wrapper=clickup_api_wrapper,
             )
             for action in operations
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return self.tools
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/cogniswitch/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/cogniswitch/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/csv/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/file_management/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/file_management/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,12 +69,12 @@
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         allowed_tools = self.selected_tools or _FILE_TOOLS_MAP
         tools: List[BaseTool] = []
         for tool in allowed_tools:
             tool_cls = _FILE_TOOLS_MAP[tool]
-            tools.append(tool_cls(root_dir=self.root_dir))  # type: ignore[call-arg]
+            tools.append(tool_cls(root_dir=self.root_dir))
         return tools
 
 
 __all__ = ["FileManagementToolkit"]
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/github/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/github/toolkit.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,12 +304,12 @@
                 description=action["description"],
                 mode=action["mode"],
                 api_wrapper=github_api_wrapper,
                 args_schema=action.get("args_schema", None),
             )
             for action in operations
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return self.tools
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/gitlab/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/gitlab/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,12 +84,12 @@
                 name=action["name"],
                 description=action["description"],
                 mode=action["mode"],
                 api_wrapper=gitlab_api_wrapper,
             )
             for action in operations
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return self.tools
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/gmail/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/gmail/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/jira/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/jira/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,12 +60,12 @@
                 name=action["name"],
                 description=action["description"],
                 mode=action["mode"],
                 api_wrapper=jira_api_wrapper,
             )
             for action in operations
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return self.tools
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/json/base.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/json/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/json/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/json/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/json/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/json/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/load_tools.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/load_tools.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/multion/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/multion/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/nasa/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nasa/toolkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,12 +47,12 @@
                 name=action["name"],
                 description=action["description"],
                 mode=action["mode"],
                 api_wrapper=nasa_api_wrapper,
             )
             for action in operations
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return self.tools
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/nla/tool.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nla/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Tool for interacting with a single API with natural language definition."""
 
 from __future__ import annotations
 
-from typing import Any, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 from langchain_core.language_models import BaseLanguageModel
 from langchain_core.tools import Tool
 
-from langchain_community.chains.openapi.chain import OpenAPIEndpointChain
 from langchain_community.tools.openapi.utils.api_models import APIOperation
 from langchain_community.tools.openapi.utils.openapi_utils import OpenAPISpec
 from langchain_community.utilities.requests import Requests
 
+if TYPE_CHECKING:
+    from langchain.chains.api.openapi.chain import OpenAPIEndpointChain
+
 
 class NLATool(Tool):
     """Natural Language API Tool."""
 
     @classmethod
     def from_open_api_endpoint_chain(
         cls, chain: OpenAPIEndpointChain, api_title: str
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/nla/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/nla/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/office365/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/office365/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/base.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/planner.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,20 +258,20 @@
     from langchain.agents.agent import AgentExecutor
     from langchain.agents.mrkl.base import ZeroShotAgent
     from langchain.chains.llm import LLMChain
 
     get_llm_chain = LLMChain(llm=llm, prompt=PARSING_GET_PROMPT)
     post_llm_chain = LLMChain(llm=llm, prompt=PARSING_POST_PROMPT)
     tools: List[BaseTool] = [
-        RequestsGetToolWithParsing(  # type: ignore[call-arg]
+        RequestsGetToolWithParsing(
             requests_wrapper=requests_wrapper,
             llm_chain=get_llm_chain,
             allow_dangerous_requests=allow_dangerous_requests,
         ),
-        RequestsPostToolWithParsing(  # type: ignore[call-arg]
+        RequestsPostToolWithParsing(
             requests_wrapper=requests_wrapper,
             llm_chain=post_llm_chain,
             allow_dangerous_requests=allow_dangerous_requests,
         ),
     ]
     prompt = PromptTemplate(
         template=API_CONTROLLER_PROMPT,
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/planner_prompt.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/planner_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/spec.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/spec.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/openapi/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/openapi/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/playwright/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/playwright/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/polygon/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/polygon/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/base.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/chat_base.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/chat_base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/powerbi/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/powerbi/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """Get the tools in the toolkit."""
         return [
             QueryPowerBITool(
                 llm_chain=self._get_chain(),
                 powerbi=self.powerbi,
                 examples=self.examples,
                 max_iterations=self.max_iterations,
-                output_token_limit=self.output_token_limit,  # type: ignore[arg-type]
+                output_token_limit=self.output_token_limit,
                 tiktoken_model_name=self.tiktoken_model_name,
             ),
             InfoPowerBITool(powerbi=self.powerbi),
             ListPowerBITool(powerbi=self.powerbi),
         ]
 
     def _get_chain(self) -> LLMChain:
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/slack/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/slack/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/spark_sql/base.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/spark_sql/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/spark_sql/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/spark_sql/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/spark_sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/sql/base.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/sql/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             "Must provide exactly one of 'toolkit' or 'db'. Received neither."
         )
     if toolkit and db:
         raise ValueError(
             "Must provide exactly one of 'toolkit' or 'db'. Received both."
         )
 
-    toolkit = toolkit or SQLDatabaseToolkit(llm=llm, db=db)  # type: ignore[arg-type]
+    toolkit = toolkit or SQLDatabaseToolkit(llm=llm, db=db)
     agent_type = agent_type or AgentType.ZERO_SHOT_REACT_DESCRIPTION
     tools = toolkit.get_tools() + list(extra_tools)
     if prompt is None:
         prefix = prefix or SQL_PREFIX
         prefix = prefix.format(dialect=toolkit.dialect, top_k=top_k)
     else:
         if "top_k" in prompt.input_variables:
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/sql/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/sql/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/sql/toolkit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/steam/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/steam/toolkit.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,12 +38,12 @@
                 name=action["name"],
                 description=action["description"],
                 mode=action["mode"],
                 api_wrapper=steam_api_wrapper,
             )
             for action in operations
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         return self.tools
```

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/xorbits/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/xorbits/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/agent_toolkits/zapier/toolkit.py` & `langchain_community-0.2.0rc1/langchain_community/agent_toolkits/zapier/toolkit.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                 action_id=action["id"],
                 zapier_description=action["description"],
                 params_schema=action["params"],
                 api_wrapper=zapier_nla_wrapper,
             )
             for action in actions
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     @classmethod
     async def async_from_zapier_nla_wrapper(
         cls, zapier_nla_wrapper: ZapierNLAWrapper
     ) -> "ZapierToolkit":
         """Create a toolkit from a ZapierNLAWrapper."""
         actions = await zapier_nla_wrapper.alist()
@@ -42,15 +42,15 @@
                 action_id=action["id"],
                 zapier_description=action["description"],
                 params_schema=action["params"],
                 api_wrapper=zapier_nla_wrapper,
             )
             for action in actions
         ]
-        return cls(tools=tools)  # type: ignore[arg-type]
+        return cls(tools=tools)
 
     def get_tools(self) -> List[BaseTool]:
         """Get the tools in the toolkit."""
         warn_deprecated(
             since="0.0.319",
             message=(
                 "This tool will be deprecated on 2023-11-17. See "
```

### Comparing `langchain_community-0.2.0/langchain_community/cache.py` & `langchain_community-0.2.0rc1/langchain_community/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -416,15 +416,15 @@
                         "Retrieving a cache value that could not be deserialized "
                         "properly. This is likely due to the cache being in an "
                         "older format. Please recreate your cache to avoid this "
                         "error."
                     )
                     # In a previous life we stored the raw text directly
                     # in the table, so assume it's in that format.
-                    generations.append(Generation(text=text))  # type: ignore[arg-type]
+                    generations.append(Generation(text=text))
         return generations if generations else None
 
     @staticmethod
     def _configure_pipeline_for_update(
         key: str, pipe: Any, return_val: RETURN_VAL_TYPE, ttl: Optional[int] = None
     ) -> None:
         pipe.hset(
@@ -1041,77 +1041,49 @@
 CASSANDRA_CACHE_DEFAULT_TTL_SECONDS = None
 
 
 class CassandraCache(BaseCache):
     """
     Cache that uses Cassandra / Astra DB as a backend.
 
-    Example:
-
-        .. code-block:: python
-
-            import cassio
-
-            from langchain_community.cache import CassandraCache
-            from langchain_core.globals import set_llm_cache
-
-            cassio.init(auto=True)  # Requires env. variables, see CassIO docs
-
-            set_llm_cache(CassandraCache())
-
     It uses a single Cassandra table.
     The lookup keys (which get to form the primary key) are:
         - prompt, a string
         - llm_string, a deterministic str representation of the model parameters.
-          (needed to prevent same-prompt-different-model collisions)
-
-    Args:
-        session: an open Cassandra session.
-            Leave unspecified to use the global cassio init (see below)
-        keyspace: the keyspace to use for storing the cache.
-            Leave unspecified to use the global cassio init (see below)
-        table_name: name of the Cassandra table to use as cache
-        ttl_seconds: time-to-live for cache entries
-            (default: None, i.e. forever)
-        setup_mode: a value in langchain_community.utilities.cassandra.SetupMode.
-            Choose between SYNC, ASYNC and OFF - the latter if the Cassandra
-            table is guaranteed to exist already, for a faster initialization.
-
-    Note:
-        The session and keyspace parameters, when left out (or passed as None),
-        fall back to the globally-available cassio settings if any are available.
-        In other words, if a previously-run 'cassio.init(...)' has been
-        executed previously anywhere in the code, Cassandra-based objects
-        need not specify the connection parameters at all.
+          (needed to prevent collisions same-prompt-different-model collisions)
     """
 
     def __init__(
         self,
         session: Optional[CassandraSession] = None,
         keyspace: Optional[str] = None,
         table_name: str = CASSANDRA_CACHE_DEFAULT_TABLE_NAME,
         ttl_seconds: Optional[int] = CASSANDRA_CACHE_DEFAULT_TTL_SECONDS,
         skip_provisioning: bool = False,
         setup_mode: CassandraSetupMode = CassandraSetupMode.SYNC,
     ):
+        """
+        Initialize with a ready session and a keyspace name.
+        Args:
+            session (cassandra.cluster.Session): an open Cassandra session
+            keyspace (str): the keyspace to use for storing the cache
+            table_name (str): name of the Cassandra table to use as cache
+            ttl_seconds (optional int): time-to-live for cache entries
+                (default: None, i.e. forever)
+        """
         if skip_provisioning:
             warn_deprecated(
-                "0.0.33",
-                name="skip_provisioning",
-                alternative=(
-                    "setup_mode=langchain_community.utilities.cassandra.SetupMode.OFF"
-                ),
-                pending=True,
+                "0.0.33", alternative="Use setup_mode=CassandraSetupMode.OFF instead."
             )
         try:
             from cassio.table import ElasticCassandraTable
         except (ImportError, ModuleNotFoundError):
             raise ImportError(
                 "Could not import cassio python package. "
-                "Please install it with `pip install -U cassio`."
+                "Please install it with `pip install cassio`."
             )
 
         self.session = session
         self.keyspace = keyspace
         self.table_name = table_name
         self.ttl_seconds = ttl_seconds
 
@@ -1194,138 +1166,80 @@
         self.kv_cache.clear()
 
     async def aclear(self, **kwargs: Any) -> None:
         """Clear cache. This is for all LLMs at once."""
         await self.kv_cache.aclear()
 
 
-# This constant is in fact a similarity - the 'distance' name is kept for compatibility:
 CASSANDRA_SEMANTIC_CACHE_DEFAULT_DISTANCE_METRIC = "dot"
 CASSANDRA_SEMANTIC_CACHE_DEFAULT_SCORE_THRESHOLD = 0.85
 CASSANDRA_SEMANTIC_CACHE_DEFAULT_TABLE_NAME = "langchain_llm_semantic_cache"
 CASSANDRA_SEMANTIC_CACHE_DEFAULT_TTL_SECONDS = None
 CASSANDRA_SEMANTIC_CACHE_EMBEDDING_CACHE_SIZE = 16
 
 
 class CassandraSemanticCache(BaseCache):
     """
     Cache that uses Cassandra as a vector-store backend for semantic
     (i.e. similarity-based) lookup.
 
-    Example:
-
-        .. code-block:: python
-
-            import cassio
-
-            from langchain_community.cache import CassandraSemanticCache
-            from langchain_core.globals import set_llm_cache
-
-            cassio.init(auto=True)  # Requires env. variables, see CassIO docs
-
-            my_embedding = ...
-
-            set_llm_cache(CassandraSemanticCache(
-                embedding=my_embedding,
-                table_name="my_semantic_cache",
-            ))
-
     It uses a single (vector) Cassandra table and stores, in principle,
     cached values from several LLMs, so the LLM's llm_string is part
     of the rows' primary keys.
 
-    One can choose a similarity measure (default: "dot" for dot-product).
-    Choosing another one ("cos", "l2") almost certainly requires threshold tuning.
-    (which may be in order nevertheless, even if sticking to "dot").
-
-    Args:
-        session: an open Cassandra session.
-            Leave unspecified to use the global cassio init (see below)
-        keyspace: the keyspace to use for storing the cache.
-            Leave unspecified to use the global cassio init (see below)
-        embedding: Embedding provider for semantic
-            encoding and search.
-        table_name: name of the Cassandra (vector) table
-            to use as cache. There is a default for "simple" usage, but
-            remember to explicitly specify different tables if several embedding
-            models coexist in your app (they cannot share one cache table).
-        distance_metric: an alias for the 'similarity_measure' parameter (see below).
-            As the "distance" terminology is misleading, please prefer
-            'similarity_measure' for clarity.
-        score_threshold: numeric value to use as
-            cutoff for the similarity searches
-        ttl_seconds: time-to-live for cache entries
-            (default: None, i.e. forever)
-        similarity_measure: which measure to adopt for similarity searches.
-            Note: this parameter is aliased by 'distance_metric' - however,
-            it is suggested to use the "similarity" terminology since this value
-            is in fact a similarity (i.e. higher means closer).
-            Note that at most one of the two parameters 'distance_metric'
-            and 'similarity_measure' can be provided.
-        setup_mode: a value in langchain_community.utilities.cassandra.SetupMode.
-            Choose between SYNC, ASYNC and OFF - the latter if the Cassandra
-            table is guaranteed to exist already, for a faster initialization.
-
-    Note:
-        The session and keyspace parameters, when left out (or passed as None),
-        fall back to the globally-available cassio settings if any are available.
-        In other words, if a previously-run 'cassio.init(...)' has been
-        executed previously anywhere in the code, Cassandra-based objects
-        need not specify the connection parameters at all.
+    The similarity is based on one of several distance metrics (default: "dot").
+    If choosing another metric, the default threshold is to be re-tuned accordingly.
     """
 
     def __init__(
         self,
-        session: Optional[CassandraSession] = None,
-        keyspace: Optional[str] = None,
-        embedding: Optional[Embeddings] = None,
+        session: Optional[CassandraSession],
+        keyspace: Optional[str],
+        embedding: Embeddings,
         table_name: str = CASSANDRA_SEMANTIC_CACHE_DEFAULT_TABLE_NAME,
-        distance_metric: Optional[str] = None,
+        distance_metric: str = CASSANDRA_SEMANTIC_CACHE_DEFAULT_DISTANCE_METRIC,
         score_threshold: float = CASSANDRA_SEMANTIC_CACHE_DEFAULT_SCORE_THRESHOLD,
         ttl_seconds: Optional[int] = CASSANDRA_SEMANTIC_CACHE_DEFAULT_TTL_SECONDS,
         skip_provisioning: bool = False,
-        similarity_measure: str = CASSANDRA_SEMANTIC_CACHE_DEFAULT_DISTANCE_METRIC,
         setup_mode: CassandraSetupMode = CassandraSetupMode.SYNC,
     ):
+        """
+        Initialize the cache with all relevant parameters.
+        Args:
+            session (cassandra.cluster.Session): an open Cassandra session
+            keyspace (str): the keyspace to use for storing the cache
+            embedding (Embedding): Embedding provider for semantic
+                encoding and search.
+            table_name (str): name of the Cassandra (vector) table
+                to use as cache
+            distance_metric (str, 'dot'): which measure to adopt for
+                similarity searches
+            score_threshold (optional float): numeric value to use as
+                cutoff for the similarity searches
+            ttl_seconds (optional int): time-to-live for cache entries
+                (default: None, i.e. forever)
+        The default score threshold is tuned to the default metric.
+        Tune it carefully yourself if switching to another distance metric.
+        """
         if skip_provisioning:
             warn_deprecated(
-                "0.0.33",
-                name="skip_provisioning",
-                alternative=(
-                    "setup_mode=langchain_community.utilities.cassandra.SetupMode.OFF"
-                ),
-                pending=True,
+                "0.0.33", alternative="Use setup_mode=CassandraSetupMode.OFF instead."
             )
         try:
             from cassio.table import MetadataVectorCassandraTable
         except (ImportError, ModuleNotFoundError):
             raise ImportError(
                 "Could not import cassio python package. "
-                "Please install it with `pip install -U cassio`."
+                "Please install it with `pip install cassio`."
             )
-
-        if not embedding:
-            raise ValueError("Missing required parameter 'embedding'.")
-
-        # detect if legacy 'distance_metric' parameter used
-        if distance_metric is not None:
-            # if passed, takes precedence over 'similarity_measure', but we warn:
-            warn_deprecated(
-                "0.0.33",
-                name="distance_metric",
-                alternative="similarity_measure",
-                pending=True,
-            )
-            similarity_measure = distance_metric
-
         self.session = session
         self.keyspace = keyspace
         self.embedding = embedding
         self.table_name = table_name
-        self.similarity_measure = similarity_measure
+        self.distance_metric = distance_metric
         self.score_threshold = score_threshold
         self.ttl_seconds = ttl_seconds
 
         # The contract for this class has separate lookup and update:
         # in order to spare some embedding calculations we cache them between
         # the two calls.
         # Note: each instance of this class has its own `_get_embedding` with
@@ -1429,15 +1343,15 @@
         """
         prompt_embedding: List[float] = self._get_embedding(text=prompt)
         hits = list(
             self.table.metric_ann_search(
                 vector=prompt_embedding,
                 metadata={"_llm_string_hash": _hash(llm_string)},
                 n=1,
-                metric=self.similarity_measure,
+                metric=self.distance_metric,
                 metric_threshold=self.score_threshold,
             )
         )
         if hits:
             hit = hits[0]
             generations = _loads_generations(hit["body_blob"])
             if generations is not None:
@@ -1460,15 +1374,15 @@
         """
         prompt_embedding: List[float] = await self._aget_embedding(text=prompt)
         hits = list(
             await self.table.ametric_ann_search(
                 vector=prompt_embedding,
                 metadata={"_llm_string_hash": _hash(llm_string)},
                 n=1,
-                metric=self.similarity_measure,
+                metric=self.distance_metric,
                 metric_threshold=self.score_threshold,
             )
         )
         if hits:
             hit = hits[0]
             generations = _loads_generations(hit["body_blob"])
             if generations is not None:
```

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/aim_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/aim_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/argilla_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/argilla_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/arize_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/arize_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/arthur_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/arthur_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/bedrock_anthropic_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/bedrock_anthropic_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/clearml_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/clearml_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/comet_ml_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/comet_ml_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/confident_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/confident_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/context_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/context_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/fiddler_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/fiddler_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/flyte_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/flyte_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/human.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/human.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/infino_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/infino_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/labelstudio_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/labelstudio_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/llmonitor_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/llmonitor_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/manager.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/mlflow_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/mlflow_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/openai_info.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/openai_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,14 @@
 import threading
 from typing import Any, Dict, List
 
 from langchain_core.callbacks import BaseCallbackHandler
 from langchain_core.outputs import LLMResult
 
 MODEL_COST_PER_1K_TOKENS = {
-    # GPT-4o input
-    "gpt-4o": 0.005,
-    "gpt-4o-2024-05-13": 0.005,
-    # GPT-4o output
-    "gpt-4o-completion": 0.015,
-    "gpt-4o-2024-05-13-completion": 0.015,
     # GPT-4 input
     "gpt-4": 0.03,
     "gpt-4-0314": 0.03,
     "gpt-4-0613": 0.03,
     "gpt-4-32k": 0.06,
     "gpt-4-32k-0314": 0.06,
     "gpt-4-32k-0613": 0.06,
```

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/promptlayer_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/promptlayer_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/sagemaker_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/sagemaker_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/streamlit/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/streamlit/mutable_expander.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/streamlit/mutable_expander.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/streamlit/streamlit_callback_handler.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/streamlit/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/tracers/comet.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/tracers/comet.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/tracers/wandb.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/tracers/wandb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/trubrics_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/trubrics_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/uptrain_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/uptrain_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/utils.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/wandb_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/callbacks/whylabs_callback.py` & `langchain_community-0.2.0rc1/langchain_community/callbacks/whylabs_callback.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/ernie_functions/base.py` & `langchain_community-0.2.0rc1/langchain_community/chains/ernie_functions/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,15 +372,15 @@
     functions: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable]],
     llm: BaseLanguageModel,
     prompt: BasePromptTemplate,
     *,
     output_key: str = "function",
     output_parser: Optional[BaseLLMOutputParser] = None,
     **kwargs: Any,
-) -> LLMChain:  # type: ignore[valid-type]
+) -> LLMChain:
     """[Legacy] Create an LLM chain that uses Ernie functions.
 
     Args:
         functions: A sequence of either dictionaries, pydantic.BaseModels classes, or
             Python functions. If dictionaries are passed in, they are assumed to
             already be a valid Ernie functions. If only a single
             function is passed in, then it will be enforced that the model use that
@@ -449,15 +449,15 @@
     ernie_functions = [convert_to_ernie_function(f) for f in functions]
     output_parser = output_parser or get_ernie_output_parser(functions)
     llm_kwargs: Dict[str, Any] = {
         "functions": ernie_functions,
     }
     if len(ernie_functions) == 1:
         llm_kwargs["function_call"] = {"name": ernie_functions[0]["name"]}
-    llm_chain = LLMChain(  # type: ignore[misc]
+    llm_chain = LLMChain(
         llm=llm,
         prompt=prompt,
         output_parser=output_parser,
         llm_kwargs=llm_kwargs,
         output_key=output_key,
         **kwargs,
     )
@@ -468,15 +468,15 @@
     output_schema: Union[Dict[str, Any], Type[BaseModel]],
     llm: BaseLanguageModel,
     prompt: BasePromptTemplate,
     *,
     output_key: str = "function",
     output_parser: Optional[BaseLLMOutputParser] = None,
     **kwargs: Any,
-) -> LLMChain:  # type: ignore[valid-type]
+) -> LLMChain:
     """[Legacy] Create an LLMChain that uses an Ernie function to get a structured output.
 
     Args:
         output_schema: Either a dictionary or pydantic.BaseModel class. If a dictionary
             is passed in, it's assumed to already be a valid JsonSchema.
             For best results, pydantic.BaseModels should have docstrings describing what
             the schema represents and descriptions for the parameters.
```

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/arangodb.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/arangodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/base.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/cypher.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/cypher.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/cypher_utils.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/cypher_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/falkordb.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/falkordb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/gremlin.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/gremlin.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/hugegraph.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/hugegraph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/kuzu.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/kuzu.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,44 +88,23 @@
         """
         _output_keys = [self.output_key]
         return _output_keys
 
     @classmethod
     def from_llm(
         cls,
-        llm: Optional[BaseLanguageModel] = None,
+        llm: BaseLanguageModel,
         *,
         qa_prompt: BasePromptTemplate = CYPHER_QA_PROMPT,
         cypher_prompt: BasePromptTemplate = KUZU_GENERATION_PROMPT,
-        cypher_llm: Optional[BaseLanguageModel] = None,
-        qa_llm: Optional[BaseLanguageModel] = None,
         **kwargs: Any,
     ) -> KuzuQAChain:
         """Initialize from LLM."""
-        if not cypher_llm and not llm:
-            raise ValueError("Either `llm` or `cypher_llm` parameters must be provided")
-        if not qa_llm and not llm:
-            raise ValueError(
-                "Either `llm` or `qa_llm` parameters must be provided along with"
-                " `cypher_llm`"
-            )
-        if cypher_llm and qa_llm and llm:
-            raise ValueError(
-                "You can specify up to two of 'cypher_llm', 'qa_llm'"
-                ", and 'llm', but not all three simultaneously."
-            )
-
-        qa_chain = LLMChain(
-            llm=qa_llm or llm,  # type: ignore[arg-type]
-            prompt=qa_prompt,
-        )
-        cypher_generation_chain = LLMChain(
-            llm=cypher_llm or llm,  # type: ignore[arg-type]
-            prompt=cypher_prompt,
-        )
+        qa_chain = LLMChain(llm=llm, prompt=qa_prompt)
+        cypher_generation_chain = LLMChain(llm=llm, prompt=cypher_prompt)
 
         return cls(
             qa_chain=qa_chain,
             cypher_generation_chain=cypher_generation_chain,
             **kwargs,
         )
```

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/nebulagraph.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/neptune_cypher.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/neptune_cypher.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/neptune_sparql.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/neptune_sparql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/ontotext_graphdb.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/ontotext_graphdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/prompts.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,21 @@
 
 NGQL_GENERATION_PROMPT = PromptTemplate(
     input_variables=["schema", "question"], template=NGQL_GENERATION_TEMPLATE
 )
 
 KUZU_EXTRA_INSTRUCTIONS = """
 Instructions:
+
 Generate the Kùzu dialect of Cypher with the following rules in mind:
-1. Do not omit the relationship pattern. Always use `()-[]->()` instead of `()->()`.
-2. Do not include triple backticks ``` in your response. Return only Cypher.
-3. Do not return any notes or comments in your response.
-\n"""
+
+1. Do not use a `WHERE EXISTS` clause to check the existence of a property.
+2. Do not omit the relationship pattern. Always use `()-[]->()` instead of `()->()`.
+3. Do not include any notes or comments even if the statement does not produce the expected result.
+```\n"""
 
 KUZU_GENERATION_TEMPLATE = CYPHER_GENERATION_TEMPLATE.replace(
     "Generate Cypher", "Generate Kùzu Cypher"
 ).replace("Instructions:", KUZU_EXTRA_INSTRUCTIONS)
 
 KUZU_GENERATION_PROMPT = PromptTemplate(
     input_variables=["schema", "question"], template=KUZU_GENERATION_TEMPLATE
```

### Comparing `langchain_community-0.2.0/langchain_community/chains/graph_qa/sparql.py` & `langchain_community-0.2.0rc1/langchain_community/chains/graph_qa/sparql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/llm_requests.py` & `langchain_community-0.2.0rc1/langchain_community/chains/llm_requests.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/openapi/chain.py` & `langchain_community-0.2.0rc1/langchain_community/chains/openapi/chain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/openapi/prompts.py` & `langchain_community-0.2.0rc1/langchain_community/chains/openapi/prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/openapi/requests_chain.py` & `langchain_community-0.2.0rc1/langchain_community/chains/openapi/requests_chain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chains/openapi/response_chain.py` & `langchain_community-0.2.0rc1/langchain_community/chains/openapi/response_chain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/facebook_messenger.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/facebook_messenger.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/gmail.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/gmail.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/imessage.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/imessage.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 content = text
             elif attributedBody:
                 content = self._parse_attributedBody(attributedBody)
             else:  # Skip messages with no content
                 continue
 
             results.append(
-                HumanMessage(  # type: ignore[call-arg]
+                HumanMessage(
                     role=sender,
                     content=content,
                     additional_kwargs={
                         "message_time": date,
                         "message_time_as_datetime": nanoseconds_from_2001_to_datetime(
                             date
                         ),
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/langsmith.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/langsmith.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/slack.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             if sender == previous_sender:
                 results[-1].content += "\n\n" + text
                 results[-1].additional_kwargs["events"].append(
                     {"message_time": timestamp}
                 )
             else:
                 results.append(
-                    HumanMessage(  # type: ignore[call-arg]
+                    HumanMessage(
                         role=sender,
                         content=text,
                         additional_kwargs={
                             "sender": sender,
                             "events": [{"message_time": timestamp}],
                         },
                     )
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/telegram.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/utils.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     messages = []
     num_converted = 0
     for message in chat_sessions["messages"]:
         if message.additional_kwargs.get("sender") == sender:
             message = AIMessage(
                 content=message.content,
                 additional_kwargs=message.additional_kwargs.copy(),
-                example=getattr(message, "example", None),  # type: ignore[arg-type]
+                example=getattr(message, "example", None),
             )
             num_converted += 1
         messages.append(message)
     return ChatSession(messages=messages)
 
 
 def map_ai_messages(
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_loaders/whatsapp.py` & `langchain_community-0.2.0rc1/langchain_community/chat_loaders/whatsapp.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         results: List[Union[HumanMessage, AIMessage]] = []
         for line in chat_lines:
             result = self._message_line_regex.match(line.strip())
             if result:
                 timestamp, sender, text = result.groups()
                 if not self._ignore_lines.match(text.strip()):
                     results.append(
-                        HumanMessage(  # type: ignore[call-arg]
+                        HumanMessage(
                             role=sender,
                             content=text,
                             additional_kwargs={
                                 "sender": sender,
                                 "events": [{"message_time": timestamp}],
                             },
                         )
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/astradb.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/cassandra.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/cassandra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/cosmos_db.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/dynamodb.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/dynamodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/elasticsearch.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/file.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/firestore.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/firestore.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/momento.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/momento.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/mongodb.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/mongodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/neo4j.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/neo4j.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/postgres.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/postgres.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/redis.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/rocksetdb.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/singlestoredb.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/sql.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/sql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/streamlit.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/streamlit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/tidb.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/tidb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/upstash_redis.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/xata.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/xata.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_message_histories/zep.py` & `langchain_community-0.2.0rc1/langchain_community/chat_message_histories/zep.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/anthropic.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/anyscale.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/anyscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/azure_openai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/azureml_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/azureml_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,8 +415,8 @@
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"])
     elif role == "tool" or default_class == ToolMessageChunk:
         return ToolMessageChunk(content=content, tool_call_id=_dict["tool_call_id"])
     elif role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/baichuan.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/baichuan.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     content = _dict.get("content") or ""
 
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content)
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 class ChatBaichuan(BaseChatModel):
     """Baichuan chat models API by Baichuan Intelligent Technology.
 
     For more information, see https://platform.baichuan-ai.com/docs/api
     """
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/baidu_qianfan_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/baidu_qianfan_endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,15 +379,15 @@
         params["stream"] = True
         for res in self.client.do(**params):
             if res:
                 msg = _convert_dict_to_message(res)
                 additional_kwargs = msg.additional_kwargs.get("function_call", {})
                 chunk = ChatGenerationChunk(
                     text=res["result"],
-                    message=AIMessageChunk(  # type: ignore[call-arg]
+                    message=AIMessageChunk(
                         content=msg.content,
                         role="assistant",
                         additional_kwargs=additional_kwargs,
                     ),
                     generation_info=msg.additional_kwargs,
                 )
                 if run_manager:
@@ -406,15 +406,15 @@
         params["stream"] = True
         async for res in await self.client.ado(**params):
             if res:
                 msg = _convert_dict_to_message(res)
                 additional_kwargs = msg.additional_kwargs.get("function_call", {})
                 chunk = ChatGenerationChunk(
                     text=res["result"],
-                    message=AIMessageChunk(  # type: ignore[call-arg]
+                    message=AIMessageChunk(
                         content=msg.content,
                         role="assistant",
                         additional_kwargs=additional_kwargs,
                     ),
                     generation_info=msg.additional_kwargs,
                 )
                 if run_manager:
@@ -548,16 +548,15 @@
         """  # noqa: E501
         if kwargs:
             raise ValueError(f"Received unsupported arguments {kwargs}")
         is_pydantic_schema = isinstance(schema, type) and issubclass(schema, BaseModel)
         llm = self.bind_tools([schema])
         if is_pydantic_schema:
             output_parser: OutputParserLike = PydanticToolsParser(
-                tools=[schema],  # type: ignore[list-item]
-                first_tool_only=True,  # type: ignore[list-item]
+                tools=[schema], first_tool_only=True
             )
         else:
             key_name = convert_to_openai_tool(schema)["function"]["name"]
             output_parser = JsonOutputKeyToolsParser(
                 key_name=key_name, first_tool_only=True
             )
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/bedrock.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/cohere.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/coze.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/coze.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     content = _dict.get("content") or ""
 
     if role == "user":
         return HumanMessageChunk(content=content)
     elif role == "assistant":
         return AIMessageChunk(content=content)
     else:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
 
 
 class ChatCoze(BaseChatModel):
     """ChatCoze chat models API by coze.com
 
     For more information, see https://www.coze.com/open/docs/chat
     """
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/dappier.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/dappier.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/databricks.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/deepinfra.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/deepinfra.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,17 +114,17 @@
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content, additional_kwargs=additional_kwargs)
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"])
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 def _convert_message_to_dict(message: BaseMessage) -> dict:
     if isinstance(message, ChatMessage):
         message_dict = {"role": message.role, "content": message.content}
     elif isinstance(message, HumanMessage):
         message_dict = {"role": "user", "content": message.content}
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/edenai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/edenai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/ernie.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/ernie.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/everlyai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/everlyai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/fake.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/fake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/fireworks.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/fireworks.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict.name)
     elif role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 def convert_dict_to_message(_dict: Any) -> BaseMessage:
     """Convert a dict response to a message."""
     role = _dict.role
     content = _dict.content or ""
     if role == "user":
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/friendli.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/friendli.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/gigachat.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/gigachat.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,17 +104,17 @@
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content, additional_kwargs=additional_kwargs)
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"])
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 class GigaChat(_BaseGigaChat, BaseChatModel):
     """`GigaChat` large language models API.
 
     To use, you should pass login and password to access GigaChat API or use token.
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/google_palm.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/gpt_router.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/gpt_router.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/huggingface.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/huggingface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Hugging Face Chat Wrapper."""
-
 from typing import Any, AsyncIterator, Iterator, List, Optional
 
-from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks.manager import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
     agenerate_from_stream,
@@ -32,21 +30,14 @@
 from langchain_community.llms.huggingface_text_gen_inference import (
     HuggingFaceTextGenInference,
 )
 
 DEFAULT_SYSTEM_PROMPT = """You are a helpful, respectful, and honest assistant."""
 
 
-@deprecated(
-    since="0.0.37",
-    removal="0.3",
-    alternative_import=(
-        "from langchain_huggingface.chat_models.huggingface import ChatHuggingFace"
-    ),
-)
 class ChatHuggingFace(BaseChatModel):
     """
     Wrapper for using Hugging Face LLM's as ChatModels.
 
     Works with `HuggingFaceTextGenInference`, `HuggingFaceEndpoint`,
     and `HuggingFaceHub` LLMs.
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/human.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/human.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/hunyuan.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/hunyuan.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,17 +68,17 @@
     content = _dict.get("content") or ""
 
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content)
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 # signature generation
 # https://cloud.tencent.com/document/product/1729/97732#532252ce-e960-48a7-8821-940a9ce2ccf3
 def _signature(secret_key: SecretStr, url: str, payload: Dict[str, Any]) -> str:
     sorted_keys = sorted(payload.keys())
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/javelin_ai_gateway.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/jinachat.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/jinachat.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content)
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 def _convert_dict_to_message(_dict: Mapping[str, Any]) -> BaseMessage:
     role = _dict["role"]
     if role == "user":
         return HumanMessage(content=_dict["content"])
     elif role == "assistant":
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/kinetica.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/kinetica.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/konko.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/konko.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/litellm.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/litellm.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,17 @@
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content, additional_kwargs=additional_kwargs)
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"])
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 def _convert_message_to_dict(message: BaseMessage) -> dict:
     if isinstance(message, ChatMessage):
         message_dict = {"role": message.role, "content": message.content}
     elif isinstance(message, HumanMessage):
         message_dict = {"role": "user", "content": message.content}
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/litellm_router.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/litellm_router.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/llama_edge.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/llama_edge.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,17 +60,17 @@
     content = _dict.get("content") or ""
 
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content)
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 class LlamaEdgeChatService(BaseChatModel):
     """Chat with LLMs via `llama-api-server`
 
     For the information about `llama-api-server`, visit https://github.com/second-state/LlamaEdge
     """
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/maritalk.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/maritalk.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/meta.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/meta.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/minimax.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/minimax.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         history = _parse_chat_history(messages)
         payload = self._default_params
         payload["messages"] = history
         text = self._client.post(payload)
 
         # This is required since the stop are not enforced by the model parameters
         text = text if stop is None else enforce_stop_tokens(text, stop)
-        return ChatResult(generations=[ChatGeneration(message=AIMessage(text))])  # type: ignore[misc]
+        return ChatResult(generations=[ChatGeneration(message=AIMessage(text))])
 
     async def _agenerate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
         **kwargs: Any,
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/mlflow.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/mlflow_ai_gateway.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/mlx.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/mlx.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/moonshot.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/moonshot.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/octoai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/octoai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/ollama.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/openai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/openai.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """OpenAI chat wrapper."""
-
 from __future__ import annotations
 
 import logging
 import os
 import sys
 from typing import (
     TYPE_CHECKING,
@@ -136,17 +135,17 @@
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role == "function" or default_class == FunctionMessageChunk:
         return FunctionMessageChunk(content=content, name=_dict["name"])
     elif role == "tool" or default_class == ToolMessageChunk:
         return ToolMessageChunk(content=content, tool_call_id=_dict["tool_call_id"])
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 @deprecated(
     since="0.0.10", removal="0.3.0", alternative_import="langchain_openai.ChatOpenAI"
 )
 class ChatOpenAI(BaseChatModel):
     """`OpenAI` Chat large language models API.
@@ -214,15 +213,15 @@
     # to support explicit proxy for OpenAI
     openai_proxy: Optional[str] = None
     request_timeout: Union[float, Tuple[float, float], Any, None] = Field(
         default=None, alias="timeout"
     )
     """Timeout for requests to OpenAI completion API. Can be float, httpx.Timeout or 
         None."""
-    max_retries: int = Field(default=2)
+    max_retries: int = 2
     """Maximum number of retries to make when generating."""
     streaming: bool = False
     """Whether to stream the results or not."""
     n: int = 1
     """Number of chat completions to generate for each prompt."""
     max_tokens: Optional[int] = None
     """Maximum number of tokens to generate."""
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/pai_eas_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/perplexity.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/perplexity.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,17 +194,17 @@
         elif role == "system" or default_class == SystemMessageChunk:
             return SystemMessageChunk(content=content)
         elif role == "function" or default_class == FunctionMessageChunk:
             return FunctionMessageChunk(content=content, name=_dict["name"])
         elif role == "tool" or default_class == ToolMessageChunk:
             return ToolMessageChunk(content=content, tool_call_id=_dict["tool_call_id"])
         elif role or default_class == ChatMessageChunk:
-            return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+            return ChatMessageChunk(content=content, role=role)
         else:
-            return default_class(content=content)  # type: ignore[call-arg]
+            return default_class(content=content)
 
     def _stream(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/premai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/premai.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             finish_reasons,
         )
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content), finish_reasons
     elif role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=content, role=role), finish_reasons
     else:
-        return default_class(content=content), finish_reasons  # type: ignore[call-arg]
+        return default_class(content=content), finish_reasons
 
 
 def _messages_to_prompt_dict(
     input_messages: List[BaseMessage],
 ) -> Tuple[Optional[str], List[Dict[str, str]]]:
     """Converts a list of LangChain Messages into a simple dict
     which is the message structure in Prem"""
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/promptlayer_openai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/solar.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/solar.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from langchain_core.pydantic_v1 import Field, root_validator
 from langchain_core.utils import get_from_dict_or_env
 
 from langchain_community.chat_models import ChatOpenAI
 from langchain_community.llms.solar import SOLAR_SERVICE_URL_BASE, SolarCommon
 
 
-@deprecated(  # type: ignore[arg-type]
+@deprecated(
     since="0.0.34", removal="0.3.0", alternative_import="langchain_upstage.ChatUpstage"
 )
 class SolarChat(SolarCommon, ChatOpenAI):
     """Wrapper around Solar large language models.
     To use, you should have the ``openai`` python package installed, and the
     environment variable ``SOLAR_API_KEY`` set with your API key.
     (Solar's chat API is compatible with OpenAI's SDK.)
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/sparkllm.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/sparkllm.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     if msg_role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=msg_content)
     elif msg_role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=msg_content)
     elif msg_role or default_class == ChatMessageChunk:
         return ChatMessageChunk(content=msg_content, role=msg_role)
     else:
-        return default_class(content=msg_content)  # type: ignore[call-arg]
+        return default_class(content=msg_content)
 
 
 class ChatSparkLLM(BaseChatModel):
     """iFlyTek Spark large language model.
 
     To use, you should pass `app_id`, `api_key`, `api_secret`
     as a named parameter to the constructor OR set environment
@@ -378,18 +378,18 @@
                 self.api_secret,
             ),
             on_message=self.on_message,
             on_error=self.on_error,
             on_close=self.on_close,
             on_open=self.on_open,
         )
-        ws.messages = messages  # type: ignore[attr-defined]
-        ws.user_id = user_id  # type: ignore[attr-defined]
-        ws.model_kwargs = self.model_kwargs if model_kwargs is None else model_kwargs  # type: ignore[attr-defined]
-        ws.streaming = streaming  # type: ignore[attr-defined]
+        ws.messages = messages
+        ws.user_id = user_id
+        ws.model_kwargs = self.model_kwargs if model_kwargs is None else model_kwargs
+        ws.streaming = streaming
         ws.run_forever()
 
     def arun(
         self,
         messages: List[Dict],
         user_id: str,
         model_kwargs: Optional[dict] = None,
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/tongyi.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/tongyi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,53 @@
 from __future__ import annotations
 
 import asyncio
 import functools
-import json
 import logging
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
     List,
     Mapping,
     Optional,
-    Sequence,
-    Type,
     Union,
     cast,
 )
 
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
-from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import BaseChatModel
 from langchain_core.messages import (
     AIMessage,
     AIMessageChunk,
     BaseMessage,
     BaseMessageChunk,
     ChatMessage,
     ChatMessageChunk,
     HumanMessage,
     HumanMessageChunk,
     SystemMessage,
     SystemMessageChunk,
-    ToolMessage,
-    ToolMessageChunk,
 )
 from langchain_core.output_parsers.openai_tools import (
     make_invalid_tool_call,
     parse_tool_call,
 )
 from langchain_core.outputs import (
     ChatGeneration,
     ChatGenerationChunk,
     ChatResult,
 )
-from langchain_core.pydantic_v1 import BaseModel, Field, SecretStr, root_validator
-from langchain_core.runnables import Runnable
-from langchain_core.tools import BaseTool
+from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.utils import convert_to_secret_str, get_from_dict_or_env
-from langchain_core.utils.function_calling import convert_to_openai_tool
 from requests.exceptions import HTTPError
 from tenacity import (
     before_sleep_log,
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
@@ -73,139 +64,84 @@
 
 def convert_dict_to_message(
     _dict: Mapping[str, Any], is_chunk: bool = False
 ) -> Union[BaseMessage, BaseMessageChunk]:
     """Convert a dict to a message."""
     role = _dict["role"]
     content = _dict["content"]
-
     if role == "user":
         return (
             HumanMessageChunk(content=content)
             if is_chunk
             else HumanMessage(content=content)
         )
     elif role == "assistant":
         tool_calls = []
         invalid_tool_calls = []
         if "tool_calls" in _dict:
             additional_kwargs = {"tool_calls": _dict["tool_calls"]}
-
-            for index, value in enumerate(_dict["tool_calls"]):
-                if is_chunk:
-                    try:
-                        tool_calls.append(
-                            {
-                                "name": value["function"].get("name"),
-                                "args": value["function"].get("arguments"),
-                                "id": value.get("id"),
-                                # Tongyi does not respond with index,
-                                # use index in the list instead
-                                "index": index,
-                            }
-                        )
-                    except KeyError:
-                        pass
-                else:
-                    try:
-                        parsed_tool = parse_tool_call(value, return_id=True)
-                        if parsed_tool:
-                            tool_calls.append(parsed_tool)
-                    except Exception as e:
-                        invalid_tool_calls.append(make_invalid_tool_call(value, str(e)))
+            for raw_tool_call in _dict["tool_calls"]:
+                try:
+                    tool_calls.append(parse_tool_call(raw_tool_call, return_id=True))
+                except Exception as e:
+                    invalid_tool_calls.append(
+                        make_invalid_tool_call(raw_tool_call, str(e))
+                    )
         else:
             additional_kwargs = {}
-
         return (
-            AIMessageChunk(
-                content=content,
-                additional_kwargs=additional_kwargs,
-                tool_call_chunks=tool_calls,  # type: ignore[arg-type]
-                id=_dict.get("id"),
-            )
+            AIMessageChunk(content=content)
             if is_chunk
             else AIMessage(
                 content=content,
                 additional_kwargs=additional_kwargs,
-                tool_calls=tool_calls,  # type: ignore[arg-type]
+                tool_calls=tool_calls,
                 invalid_tool_calls=invalid_tool_calls,
             )
         )
     elif role == "system":
         return (
             SystemMessageChunk(content=content)
             if is_chunk
             else SystemMessage(content=content)
         )
-    elif role == "tool":
-        additional_kwargs = {}
-        if "name" in _dict:
-            additional_kwargs["name"] = _dict["name"]
-        return (
-            ToolMessageChunk(
-                content=_dict.get("content", ""),
-                tool_call_id=_dict.get("tool_call_id"),  # type: ignore[arg-type]
-                additional_kwargs=additional_kwargs,
-            )
-            if is_chunk
-            else ToolMessage(
-                content=_dict.get("content", ""),
-                tool_call_id=_dict.get("tool_call_id"),  # type: ignore[arg-type]
-                additional_kwargs=additional_kwargs,
-            )
-        )
     else:
         return (
             ChatMessageChunk(role=role, content=content)
             if is_chunk
             else ChatMessage(role=role, content=content)
         )
 
 
 def convert_message_chunk_to_message(message_chunk: BaseMessageChunk) -> BaseMessage:
-    """Convert a message chunk to a message.
-
-    Args:
-        chunk: Message chunk to convert.
-
-    Returns:
-        Message.
-    """
-    if not isinstance(message_chunk, BaseMessageChunk):
-        return message_chunk
-    # chunk classes always have the equivalent non-chunk class as their first parent
-    ignore_keys = ["type"]
-    if isinstance(message_chunk, AIMessageChunk):
-        ignore_keys.append("tool_call_chunks")
-    return message_chunk.__class__.__mro__[1](
-        **{k: v for k, v in message_chunk.__dict__.items() if k not in ignore_keys}
-    )
+    """Convert a message chunk to a message."""
+    if isinstance(message_chunk, HumanMessageChunk):
+        return HumanMessage(content=message_chunk.content)
+    elif isinstance(message_chunk, AIMessageChunk):
+        return AIMessage(content=message_chunk.content)
+    elif isinstance(message_chunk, SystemMessageChunk):
+        return SystemMessage(content=message_chunk.content)
+    elif isinstance(message_chunk, ChatMessageChunk):
+        return ChatMessage(role=message_chunk.role, content=message_chunk.content)
+    else:
+        raise TypeError(f"Got unknown type {message_chunk}")
 
 
 def convert_message_to_dict(message: BaseMessage) -> dict:
     """Convert a message to a dict."""
 
     message_dict: Dict[str, Any]
     if isinstance(message, ChatMessage):
         message_dict = {"role": message.role, "content": message.content}
     elif isinstance(message, HumanMessage):
         message_dict = {"role": "user", "content": message.content}
     elif isinstance(message, AIMessage):
         message_dict = {"role": "assistant", "content": message.content}
-        if "tool_calls" in message.additional_kwargs:
-            message_dict["tool_calls"] = message.additional_kwargs["tool_calls"]
     elif isinstance(message, SystemMessage):
         message_dict = {"role": "system", "content": message.content}
-    elif isinstance(message, ToolMessage):
-        message_dict = {
-            "role": "tool",
-            "tool_call_id": message.tool_call_id,
-            "content": message.content,
-            "name": message.name,
-        }
     else:
         raise TypeError(f"Got unknown type {message}")
     return message_dict
 
 
 def _create_retry_decorator(llm: ChatTongyi) -> Callable[[Any], Any]:
     min_seconds = 1
@@ -316,65 +252,19 @@
     def stream_completion_with_retry(self, **kwargs: Any) -> Any:
         """Use tenacity to retry the completion call."""
         retry_decorator = _create_retry_decorator(self)
 
         @retry_decorator
         def _stream_completion_with_retry(**_kwargs: Any) -> Any:
             responses = self.client.call(**_kwargs)
-            prev_resp = None
-
             for resp in responses:
-                # If we are streaming without `incremental_output = True`,
-                # we need to calculate the delta response manually
-                if _kwargs.get("stream") and not _kwargs.get(
-                    "incremental_output", False
-                ):
-                    if prev_resp is None:
-                        delta_resp = resp
-                    else:
-                        delta_resp = self.subtract_client_response(resp, prev_resp)
-                    prev_resp = resp
-                    yield check_response(delta_resp)
-                else:
-                    yield check_response(resp)
+                yield check_response(resp)
 
         return _stream_completion_with_retry(**kwargs)
 
-    def subtract_client_response(self, resp: Any, prev_resp: Any) -> Any:
-        """Subtract prev response from curr response.
-
-        Useful when streaming without `incremental_output = True`
-        """
-
-        resp_copy = json.loads(json.dumps(resp))
-        choice = resp_copy["output"]["choices"][0]
-        message = choice["message"]
-
-        prev_resp_copy = json.loads(json.dumps(prev_resp))
-        prev_choice = prev_resp_copy["output"]["choices"][0]
-        prev_message = prev_choice["message"]
-
-        message["content"] = message["content"].replace(prev_message["content"], "")
-
-        if message.get("tool_calls"):
-            for index, tool_call in enumerate(message["tool_calls"]):
-                function = tool_call["function"]
-
-                if prev_message.get("tool_calls"):
-                    prev_function = prev_message["tool_calls"][index]["function"]
-
-                    function["name"] = function["name"].replace(
-                        prev_function["name"], ""
-                    )
-                    function["arguments"] = function["arguments"].replace(
-                        prev_function["arguments"], ""
-                    )
-
-        return resp_copy
-
     async def astream_completion_with_retry(self, **kwargs: Any) -> Any:
         """Because the dashscope SDK doesn't provide an async API,
         we wrap `stream_generate_with_retry` with an async generator."""
 
         class _AioTongyiGenerator:
             def __init__(self, generator: Any):
                 self.generator = generator
@@ -407,24 +297,24 @@
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> ChatResult:
         generations = []
         if self.streaming:
-            generation_chunk: Optional[ChatGenerationChunk] = None
+            generation: Optional[ChatGenerationChunk] = None
             for chunk in self._stream(
                 messages, stop=stop, run_manager=run_manager, **kwargs
             ):
-                if generation_chunk is None:
-                    generation_chunk = chunk
+                if generation is None:
+                    generation = chunk
                 else:
-                    generation_chunk += chunk
-            assert generation_chunk is not None
-            generations.append(self._chunk_to_generation(generation_chunk))
+                    generation += chunk
+            assert generation is not None
+            generations.append(self._chunk_to_generation(generation))
         else:
             params: Dict[str, Any] = self._invocation_params(
                 messages=messages, stop=stop, **kwargs
             )
             resp = self.completion_with_retry(**params)
             generations.append(
                 ChatGeneration(**self._chat_generation_from_qwen_resp(resp))
@@ -479,27 +369,17 @@
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         params: Dict[str, Any] = self._invocation_params(
             messages=messages, stop=stop, stream=True, **kwargs
         )
-
         for stream_resp, is_last_chunk in generate_with_last_element_mark(
             self.stream_completion_with_retry(**params)
         ):
-            choice = stream_resp["output"]["choices"][0]
-            message = choice["message"]
-            if (
-                choice["finish_reason"] == "null"
-                and message["content"] == ""
-                and "tool_calls" not in message
-            ):
-                continue
-
             chunk = ChatGenerationChunk(
                 **self._chat_generation_from_qwen_resp(
                     stream_resp, is_chunk=True, is_last_chunk=is_last_chunk
                 )
             )
             if run_manager:
                 run_manager.on_llm_new_token(chunk.text, chunk=chunk)
@@ -529,21 +409,22 @@
 
     def _invocation_params(
         self, messages: List[BaseMessage], stop: Any, **kwargs: Any
     ) -> Dict[str, Any]:
         params = {**self._default_params, **kwargs}
         if stop is not None:
             params["stop"] = stop
-        # According to the Tongyi official docs,
-        # `incremental_output` with `tools` is not supported yet
-        if params.get("stream") and not params.get("tools"):
+        if params.get("stream"):
             params["incremental_output"] = True
 
         message_dicts = [convert_message_to_dict(m) for m in messages]
 
+        # According to the docs, the last message should be a `user` message
+        if message_dicts[-1]["role"] != "user":
+            raise ValueError("Last message should be user message.")
         # And the `system` message should be the first message if present
         system_message_indices = [
             i for i, m in enumerate(message_dicts) if m["role"] == "system"
         ]
         if len(system_message_indices) == 1 and system_message_indices[0] != 0:
             raise ValueError("System message can only be the first message.")
         elif len(system_message_indices) > 1:
@@ -585,26 +466,7 @@
 
     @staticmethod
     def _chunk_to_generation(chunk: ChatGenerationChunk) -> ChatGeneration:
         return ChatGeneration(
             message=convert_message_chunk_to_message(chunk.message),
             generation_info=chunk.generation_info,
         )
-
-    def bind_tools(
-        self,
-        tools: Sequence[Union[Dict[str, Any], Type[BaseModel], Callable, BaseTool]],
-        **kwargs: Any,
-    ) -> Runnable[LanguageModelInput, BaseMessage]:
-        """Bind tool-like objects to this chat model.
-
-        Args:
-            tools: A list of tool definitions to bind to this chat model.
-                Can be  a dictionary, pydantic model, callable, or BaseTool. Pydantic
-                models, callables, and BaseTools will be automatically converted to
-                their schema dictionary representation.
-            **kwargs: Any additional parameters to pass to the
-                :class:`~langchain.runnable.Runnable` constructor.
-        """
-
-        formatted_tools = [convert_to_openai_tool(tool) for tool in tools]
-        return super().bind(tools=formatted_tools, **kwargs)
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/vertexai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/volcengine_maas.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/yandex.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/yuan2.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/yuan2.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,29 +433,29 @@
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     elif role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content)
     elif role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     elif role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
+        return ChatMessageChunk(content=content, role=role)
     else:
-        return default_class(content=content)  # type: ignore[call-arg]
+        return default_class(content=content)
 
 
 def _convert_dict_to_message(_dict: Mapping[str, Any]) -> BaseMessage:
     role = _dict.get("role")
     if role == "user":
         return HumanMessage(content=_dict.get("content", ""))
     elif role == "assistant":
         return AIMessage(content=_dict.get("content", ""))
     elif role == "system":
         return SystemMessage(content=_dict.get("content", ""))
     else:
-        return ChatMessage(content=_dict.get("content", ""), role=role)  # type: ignore[arg-type]
+        return ChatMessage(content=_dict.get("content", ""), role=role)
 
 
 def _convert_message_to_dict(message: BaseMessage) -> dict:
     """Convert a LangChain message to a dictionary.
 
     Args:
         message: The LangChain message.
```

### Comparing `langchain_community-0.2.0/langchain_community/chat_models/zhipuai.py` & `langchain_community-0.2.0rc1/langchain_community/chat_models/zhipuai.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return HumanMessage(content=content)
     if role == "assistant":
         additional_kwargs = {}
         tool_calls = dct.get("tool_calls", None)
         if tool_calls is not None:
             additional_kwargs["tool_calls"] = tool_calls
         return AIMessage(content=content, additional_kwargs=additional_kwargs)
-    return ChatMessage(role=role, content=content)  # type: ignore[arg-type]
+    return ChatMessage(role=role, content=content)
 
 
 def _convert_message_to_dict(message: BaseMessage) -> Dict[str, Any]:
     """Convert a LangChain message to a dictionary.
 
     Args:
         message: The LangChain message.
@@ -140,16 +140,16 @@
     if role == "system" or default_class == SystemMessageChunk:
         return SystemMessageChunk(content=content)
     if role == "user" or default_class == HumanMessageChunk:
         return HumanMessageChunk(content=content)
     if role == "assistant" or default_class == AIMessageChunk:
         return AIMessageChunk(content=content, additional_kwargs=additional_kwargs)
     if role or default_class == ChatMessageChunk:
-        return ChatMessageChunk(content=content, role=role)  # type: ignore[arg-type]
-    return default_class(content=content)  # type: ignore[call-arg]
+        return ChatMessageChunk(content=content, role=role)
+    return default_class(content=content)
 
 
 def _truncate_params(payload: Dict[str, Any]) -> None:
     """Truncate temperature and top_p parameters between [0.01, 0.99].
 
     ZhipuAI only support temperature / top_p between (0, 1) open interval,
     so we truncate them to [0.01, 0.99].
```

### Comparing `langchain_community-0.2.0/langchain_community/cross_encoders/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/cross_encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/cross_encoders/fake.py` & `langchain_community-0.2.0rc1/langchain_community/cross_encoders/fake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/cross_encoders/huggingface.py` & `langchain_community-0.2.0rc1/langchain_community/cross_encoders/huggingface.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/cross_encoders/sagemaker_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/cross_encoders/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/docstore/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/docstore/arbitrary_fn.py` & `langchain_community-0.2.0rc1/langchain_community/docstore/arbitrary_fn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/docstore/base.py` & `langchain_community-0.2.0rc1/langchain_community/docstore/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/docstore/in_memory.py` & `langchain_community-0.2.0rc1/langchain_community/docstore/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/docstore/wikipedia.py` & `langchain_community-0.2.0rc1/langchain_community/docstore/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_compressors/flashrank_rerank.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/llama_index.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-from __future__ import annotations
+from typing import Any, Dict, List, cast
 
-from typing import TYPE_CHECKING, Dict, Optional, Sequence
+from langchain_core.callbacks import CallbackManagerForRetrieverRun
+from langchain_core.documents import Document
+from langchain_core.pydantic_v1 import Field
+from langchain_core.retrievers import BaseRetriever
 
-from langchain_core.callbacks.manager import Callbacks
-from langchain_core.documents import BaseDocumentCompressor, Document
-from langchain_core.pydantic_v1 import Extra, root_validator
-
-if TYPE_CHECKING:
-    from flashrank import Ranker, RerankRequest
-else:
-    # Avoid pydantic annotation issues when actually instantiating
-    # while keeping this import optional
-    try:
-        from flashrank import Ranker, RerankRequest
-    except ImportError:
-        pass
-
-DEFAULT_MODEL_NAME = "ms-marco-MultiBERT-L-12"
-
-
-class FlashrankRerank(BaseDocumentCompressor):
-    """Document compressor using Flashrank interface."""
-
-    client: Ranker
-    """Flashrank client to use for compressing documents"""
-    top_n: int = 3
-    """Number of documents to return."""
-    model: Optional[str] = None
-    """Model to use for reranking."""
-
-    class Config:
-        """Configuration for this pydantic object."""
-
-        extra = Extra.forbid
-        arbitrary_types_allowed = True
-
-    @root_validator(pre=True)
-    def validate_environment(cls, values: Dict) -> Dict:
-        """Validate that api key and python package exists in environment."""
+
+class LlamaIndexRetriever(BaseRetriever):
+    """`LlamaIndex` retriever.
+
+    It is used for the question-answering with sources over
+    an LlamaIndex data structure."""
+
+    index: Any
+    """LlamaIndex index to query."""
+    query_kwargs: Dict = Field(default_factory=dict)
+    """Keyword arguments to pass to the query method."""
+
+    def _get_relevant_documents(
+        self, query: str, *, run_manager: CallbackManagerForRetrieverRun
+    ) -> List[Document]:
+        """Get documents relevant for a query."""
+        try:
+            from llama_index.core.base.response.schema import Response
+            from llama_index.core.indices.base import BaseGPTIndex
+        except ImportError:
+            raise ImportError(
+                "You need to install `pip install llama-index` to use this retriever."
+            )
+        index = cast(BaseGPTIndex, self.index)
+
+        response = index.query(query, **self.query_kwargs)
+        response = cast(Response, response)
+        # parse source nodes
+        docs = []
+        for source_node in response.source_nodes:
+            metadata = source_node.metadata or {}
+            docs.append(
+                Document(page_content=source_node.get_content(), metadata=metadata)
+            )
+        return docs
+
+
+class LlamaIndexGraphRetriever(BaseRetriever):
+    """`LlamaIndex` graph data structure retriever.
+
+    It is used for question-answering with sources over an LlamaIndex
+    graph data structure."""
+
+    graph: Any
+    """LlamaIndex graph to query."""
+    query_configs: List[Dict] = Field(default_factory=list)
+    """List of query configs to pass to the query method."""
+
+    def _get_relevant_documents(
+        self, query: str, *, run_manager: CallbackManagerForRetrieverRun
+    ) -> List[Document]:
+        """Get documents relevant for a query."""
         try:
-            from flashrank import Ranker
+            from llama_index.core.base.response.schema import Response
+            from llama_index.core.composability.base import (
+                QUERY_CONFIG_TYPE,
+                ComposableGraph,
+            )
         except ImportError:
             raise ImportError(
-                "Could not import flashrank python package. "
-                "Please install it with `pip install flashrank`."
+                "You need to install `pip install llama-index` to use this retriever."
             )
+        graph = cast(ComposableGraph, self.graph)
 
-        values["model"] = values.get("model", DEFAULT_MODEL_NAME)
-        values["client"] = Ranker(model_name=values["model"])
-        return values
-
-    def compress_documents(
-        self,
-        documents: Sequence[Document],
-        query: str,
-        callbacks: Optional[Callbacks] = None,
-    ) -> Sequence[Document]:
-        passages = [
-            {"id": i, "text": doc.page_content, "meta": doc.metadata}
-            for i, doc in enumerate(documents)
-        ]
-
-        rerank_request = RerankRequest(query=query, passages=passages)
-        rerank_response = self.client.rerank(rerank_request)[: self.top_n]
-        final_results = []
-
-        for r in rerank_response:
-            metadata = r["meta"]
-            metadata["relevance_score"] = r["score"]
-            doc = Document(
-                page_content=r["text"],
-                metadata=metadata,
+        # for now, inject response_mode="no_text" into query configs
+        for query_config in self.query_configs:
+            query_config["response_mode"] = "no_text"
+        query_configs = cast(List[QUERY_CONFIG_TYPE], self.query_configs)
+        response = graph.query(query, query_configs=query_configs)
+        response = cast(Response, response)
+
+        # parse source nodes
+        docs = []
+        for source_node in response.source_nodes:
+            metadata = source_node.metadata or {}
+            docs.append(
+                Document(page_content=source_node.get_content(), metadata=metadata)
             )
-            final_results.append(doc)
-        return final_results
+        return docs
```

### Comparing `langchain_community-0.2.0/langchain_community/document_compressors/jina_rerank.py` & `langchain_community-0.2.0rc1/langchain_community/document_compressors/jina_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_compressors/llmlingua_filter.py` & `langchain_community-0.2.0rc1/langchain_community/document_compressors/llmlingua_filter.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_compressors/openvino_rerank.py` & `langchain_community-0.2.0rc1/langchain_community/document_compressors/openvino_rerank.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/acreom.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/acreom.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/airbyte.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/airbyte.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/airbyte_json.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/airbyte_json.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/airtable.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/airtable.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/apify_dataset.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/apify_dataset.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/arcgis_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/arcgis_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/arxiv.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/assemblyai.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/assemblyai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/astradb.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/async_html.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/async_html.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 import asyncio
 import logging
 import warnings
-from concurrent.futures import Future, ThreadPoolExecutor
-from typing import (
-    Any,
-    AsyncIterator,
-    Dict,
-    Iterator,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    cast,
-)
+from concurrent.futures import ThreadPoolExecutor
+from typing import Any, Dict, Iterator, List, Optional, Union, cast
 
 import aiohttp
 import requests
 from langchain_core.documents import Document
 
 from langchain_community.document_loaders.base import BaseLoader
 
@@ -58,16 +48,14 @@
         autoset_encoding: bool = True,
         encoding: Optional[str] = None,
         default_parser: str = "html.parser",
         requests_per_second: int = 2,
         requests_kwargs: Optional[Dict[str, Any]] = None,
         raise_for_status: bool = False,
         ignore_load_errors: bool = False,
-        *,
-        preserve_order: bool = True,
     ):
         """Initialize with a webpage path."""
 
         # TODO: Deprecate web_path in favor of web_paths, and remove this
         # left like this because there are a number of loaders that expect single
         # urls
         if isinstance(web_path, str):
@@ -98,15 +86,14 @@
         self.requests_per_second = requests_per_second
         self.default_parser = default_parser
         self.requests_kwargs = requests_kwargs or {}
         self.raise_for_status = raise_for_status
         self.autoset_encoding = autoset_encoding
         self.encoding = encoding
         self.ignore_load_errors = ignore_load_errors
-        self.preserve_order = preserve_order
 
     def _fetch_valid_connection_docs(self, url: str) -> Any:
         if self.ignore_load_errors:
             try:
                 return self.session.get(url, **self.requests_kwargs)
             except Exception as e:
                 warnings.warn(str(e))
@@ -119,14 +106,43 @@
         """Check that parser is valid for bs4."""
         valid_parsers = ["html.parser", "lxml", "xml", "lxml-xml", "html5lib"]
         if parser not in valid_parsers:
             raise ValueError(
                 "`parser` must be one of " + ", ".join(valid_parsers) + "."
             )
 
+    def _scrape(
+        self,
+        url: str,
+        parser: Union[str, None] = None,
+        bs_kwargs: Optional[dict] = None,
+    ) -> Any:
+        from bs4 import BeautifulSoup
+
+        if parser is None:
+            if url.endswith(".xml"):
+                parser = "xml"
+            else:
+                parser = self.default_parser
+
+        self._check_parser(parser)
+
+        html_doc = self._fetch_valid_connection_docs(url)
+        if not getattr(html_doc, "ok", False):
+            return None
+
+        if self.raise_for_status:
+            html_doc.raise_for_status()
+
+        if self.encoding is not None:
+            html_doc.encoding = self.encoding
+        elif self.autoset_encoding:
+            html_doc.encoding = html_doc.apparent_encoding
+        return BeautifulSoup(html_doc.text, parser, **(bs_kwargs or {}))
+
     async def _fetch(
         self, url: str, retries: int = 3, cooldown: int = 2, backoff: float = 1.5
     ) -> str:
         async with aiohttp.ClientSession() as session:
             for i in range(retries):
                 try:
                     async with session.get(
@@ -152,83 +168,55 @@
                             f"{i + 1}/{retries}: {e}. Retrying..."
                         )
                         await asyncio.sleep(cooldown * backoff**i)
         raise ValueError("retry count exceeded")
 
     async def _fetch_with_rate_limit(
         self, url: str, semaphore: asyncio.Semaphore
-    ) -> Tuple[str, str]:
+    ) -> str:
         async with semaphore:
-            return url, await self._fetch(url)
+            return await self._fetch(url)
 
-    async def _lazy_fetch_all(
-        self, urls: List[str], preserve_order: bool
-    ) -> AsyncIterator[Tuple[str, str]]:
+    async def fetch_all(self, urls: List[str]) -> Any:
+        """Fetch all urls concurrently with rate limiting."""
         semaphore = asyncio.Semaphore(self.requests_per_second)
-        tasks = [
-            asyncio.create_task(self._fetch_with_rate_limit(url, semaphore))
-            for url in urls
-        ]
+        tasks = []
+        for url in urls:
+            task = asyncio.ensure_future(self._fetch_with_rate_limit(url, semaphore))
+            tasks.append(task)
         try:
             from tqdm.asyncio import tqdm_asyncio
 
-            if preserve_order:
-                for task in tqdm_asyncio(
-                    tasks, desc="Fetching pages", ascii=True, mininterval=1
-                ):
-                    yield await task
-            else:
-                for task in tqdm_asyncio.as_completed(
-                    tasks, desc="Fetching pages", ascii=True, mininterval=1
-                ):
-                    yield await task
+            return await tqdm_asyncio.gather(
+                *tasks, desc="Fetching pages", ascii=True, mininterval=1
+            )
         except ImportError:
             warnings.warn("For better logging of progress, `pip install tqdm`")
-            if preserve_order:
-                for result in await asyncio.gather(*tasks):
-                    yield result
-            else:
-                for task in asyncio.as_completed(tasks):
-                    yield await task
-
-    async def fetch_all(self, urls: List[str]) -> List[str]:
-        """Fetch all urls concurrently with rate limiting."""
-        return [doc async for _, doc in self._lazy_fetch_all(urls, True)]
-
-    def _to_document(self, url: str, text: str) -> Document:
-        from bs4 import BeautifulSoup
-
-        if url.endswith(".xml"):
-            parser = "xml"
-        else:
-            parser = self.default_parser
-        self._check_parser(parser)
-        soup = BeautifulSoup(text, parser)
-        metadata = _build_metadata(soup, url)
-        return Document(page_content=text, metadata=metadata)
+            return await asyncio.gather(*tasks)
 
     def lazy_load(self) -> Iterator[Document]:
         """Lazy load text from the url(s) in web_path."""
-        results: List[str]
+        for doc in self.load():
+            yield doc
+
+    def load(self) -> List[Document]:
+        """Load text from the url(s) in web_path."""
+
         try:
             # Raises RuntimeError if there is no current event loop.
             asyncio.get_running_loop()
             # If there is a current event loop, we need to run the async code
             # in a separate loop, in a separate thread.
             with ThreadPoolExecutor(max_workers=1) as executor:
-                future: Future[List[str]] = executor.submit(
-                    asyncio.run,  # type: ignore[arg-type]
-                    self.fetch_all(self.web_paths),  # type: ignore[arg-type]
-                )
+                future = executor.submit(asyncio.run, self.fetch_all(self.web_paths))
                 results = future.result()
         except RuntimeError:
             results = asyncio.run(self.fetch_all(self.web_paths))
-
+        docs = []
         for i, text in enumerate(cast(List[str], results)):
-            yield self._to_document(self.web_paths[i], text)
+            soup = self._scrape(self.web_paths[i])
+            if not soup:
+                continue
+            metadata = _build_metadata(soup, self.web_paths[i])
+            docs.append(Document(page_content=text, metadata=metadata))
 
-    async def alazy_load(self) -> AsyncIterator[Document]:
-        """Lazy load text from the url(s) in web_path."""
-        async for url, text in self._lazy_fetch_all(
-            self.web_paths, self.preserve_order
-        ):
-            yield self._to_document(url, text)
+        return docs
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/athena.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/athena.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/azlyrics.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/azlyrics.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/azure_ai_data.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/azure_ai_data.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/azure_blob_storage_container.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/azure_blob_storage_container.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/azure_blob_storage_file.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/azure_blob_storage_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/baiducloud_bos_directory.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/baiducloud_bos_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/baiducloud_bos_file.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/baiducloud_bos_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/base_o365.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/base_o365.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             mime_types_mapping[file_type.value] = "application/pdf"
     return mime_types_mapping
 
 
 class O365BaseLoader(BaseLoader, BaseModel):
     """Base class for all loaders that uses O365 Package"""
 
-    settings: _O365Settings = Field(default_factory=_O365Settings)  # type: ignore[arg-type]
+    settings: _O365Settings = Field(default_factory=_O365Settings)
     """Settings for the Office365 API client."""
     auth_with_token: bool = False
     """Whether to authenticate with a token or not. Defaults to False."""
     chunk_size: Union[int, str] = CHUNK_SIZE
     """Number of bytes to retrieve from each api call to the server. int or 'auto'."""
     recursive: bool = False
     """Should the loader recursively load subfolders?"""
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/bibtex.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/bibtex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/bigquery.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/bigquery.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/bilibili.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/bilibili.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/blackboard.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/blackboard.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/blob_loaders/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/blob_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/blob_loaders/file_system.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/blob_loaders/file_system.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/blob_loaders/youtube_audio.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/blob_loaders/youtube_audio.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/blockchain.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/blockchain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/brave_search.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/brave_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/browserbase.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/browserbase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Iterator, Optional, Sequence
+from typing import Iterator, List, Optional, Tuple, Union
 
 from langchain_core.documents import Document
 
 from langchain_community.document_loaders.base import BaseLoader
 
 
 class BrowserbaseLoader(BaseLoader):
@@ -10,43 +10,37 @@
 
     Depends on `browserbase` package.
     Get your API key from https://browserbase.com
     """
 
     def __init__(
         self,
-        urls: Sequence[str],
-        text_content: bool = False,
+        urls: Union[List[str], Tuple[str, ...]],
+        *,
         api_key: Optional[str] = None,
-        project_id: Optional[str] = None,
-        session_id: Optional[str] = None,
-        proxy: Optional[bool] = None,
+        text_content: bool = False,
     ):
         self.urls = urls
         self.text_content = text_content
-        self.session_id = session_id
-        self.proxy = proxy
 
         try:
             from browserbase import Browserbase
         except ImportError:
             raise ImportError(
                 "You must run "
                 "`pip install --upgrade "
                 "browserbase` "
                 "to use the Browserbase loader."
             )
 
-        self.browserbase = Browserbase(api_key, project_id)
+        self.browserbase = Browserbase(api_key=api_key)
 
     def lazy_load(self) -> Iterator[Document]:
         """Load pages from URLs"""
-        pages = self.browserbase.load_urls(
-            self.urls, self.text_content, self.session_id, self.proxy
-        )
+        pages = self.browserbase.load_urls(self.urls, self.text_content)
 
         for i, page in enumerate(pages):
             yield Document(
                 page_content=page,
                 metadata={
                     "url": self.urls[i],
                 },
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/browserless.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/browserless.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/cassandra.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/cassandra.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,16 @@
                 If not provided, the cassio resolved session will be used.
             keyspace: The keyspace of the table.
                 If not provided, the cassio resolved keyspace will be used.
             query: The query used to load the data.
                 (do not use together with the table parameter)
             page_content_mapper: a function to convert a row to string page content.
                 Defaults to the str representation of the row.
-            metadata_mapper: a function to convert a row to document metadata.
             query_parameters: The query parameters used when calling session.execute .
             query_timeout: The query timeout used when calling session.execute .
-            query_trace: Whether to use tracing when calling session.execute .
             query_custom_payload: The query custom_payload used when calling
                 session.execute .
             query_execution_profile: The query execution_profile used when calling
                 session.execute .
             query_host: The query host used when calling session.execute .
             query_execute_as: The query execute_as used when calling session.execute .
         """
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/chatgpt.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/chatgpt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/chm.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/chm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/chromium.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/chromium.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/college_confidential.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/college_confidential.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/concurrent.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/concurrent.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/confluence.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/confluence.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/conllu.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/conllu.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/couchbase.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/couchbase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/csv_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/csv_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/cube_semantic.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/cube_semantic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/datadog_logs.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/datadog_logs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/dataframe.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/diffbot.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/diffbot.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/directory.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/discord.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/discord.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/doc_intelligence.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/docugami.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/docugami.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/docusaurus.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/docusaurus.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/dropbox.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/dropbox.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/duckdb_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/duckdb_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/email.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/email.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/epub.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/epub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/etherscan.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/etherscan.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/evernote.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/evernote.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/excel.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/excel.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/facebook_chat.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/facebook_chat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/fauna.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/fauna.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/figma.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/figma.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/firecrawl.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/firecrawl.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/gcs_directory.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/gcs_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/gcs_file.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/gcs_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/generic.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/generic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/geodataframe.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/geodataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/git.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/git.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/gitbook.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/gitbook.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/github.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/github.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/glue_catalog.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/glue_catalog.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/google_speech_to_text.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/google_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/googledrive.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/googledrive.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/gutenberg.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/gutenberg.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/helpers.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/helpers.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/hn.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/hn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/html.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/html.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/html_bs.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/html_bs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/hugging_face_dataset.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/hugging_face_dataset.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/hugging_face_model.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/hugging_face_model.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/ifixit.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/ifixit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/image.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/image.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/image_captions.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/image_captions.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/iugu.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/iugu.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/joplin.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/joplin.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/json_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/kinetica_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/kinetica_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             metadata_columns = []
         return page_content_columns or [], metadata_columns
 
     def lazy_load(self) -> Iterator[Document]:
         query_result = self._execute_query()
         if isinstance(query_result, Exception):
             print(f"An error occurred during the query: {query_result}")  # noqa: T201
-            return []  # type: ignore[return-value]
+            return []
         page_content_columns, metadata_columns = self._get_columns(query_result)
         if "*" in page_content_columns:
             page_content_columns = list(query_result[0].keys())
         for row in query_result:
             page_content = "\n".join(
                 f"{k}: {v}" for k, v in row.items() if k in page_content_columns
             )
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/lakefs.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/lakefs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/larksuite.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/larksuite.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/llmsherpa.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/llmsherpa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/markdown.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/markdown.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/mastodon.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/mastodon.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/max_compute.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/max_compute.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/mediawikidump.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/mediawikidump.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/merge.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/merge.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/mhtml.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/mhtml.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,16 +54,16 @@
             message = email.message_from_string(f.read())
             parts = message.get_payload()
 
             if not isinstance(parts, list):
                 parts = [message]
 
             for part in parts:
-                if part.get_content_type() == "text/html":  # type: ignore[union-attr]
-                    html = part.get_payload(decode=True).decode()  # type: ignore[union-attr]
+                if part.get_content_type() == "text/html":
+                    html = part.get_payload(decode=True).decode()
 
                     soup = BeautifulSoup(html, **self.bs_kwargs)
                     text = soup.get_text(self.get_text_separator)
 
                     if soup.title:
                         title = str(soup.title.string)
                     else:
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/mintbase.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/mintbase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/modern_treasury.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/modern_treasury.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/mongodb.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/mongodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/news.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/news.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/notebook.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/notebook.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/notion.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/notion.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/notiondb.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/notiondb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/nuclia.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/nuclia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/obs_directory.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/obs_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/obs_file.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/obs_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/obsidian.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/obsidian.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/odt.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/odt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/onedrive.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/onedrive.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/onedrive_file.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/onedrive_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/onenote.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/onenote.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         case_sentive = False
         env_file = ".env"
 
 
 class OneNoteLoader(BaseLoader, BaseModel):
     """Load pages from OneNote notebooks."""
 
-    settings: _OneNoteGraphSettings = Field(default_factory=_OneNoteGraphSettings)  # type: ignore[arg-type]
+    settings: _OneNoteGraphSettings = Field(default_factory=_OneNoteGraphSettings)
     """Settings for the Microsoft Graph API client."""
     auth_with_token: bool = False
     """Whether to authenticate with a token or not. Defaults to False."""
     access_token: str = ""
     """Personal access token"""
     onenote_api_base_url: str = "https://graph.microsoft.com/v1.0/me/onenote"
     """URL of Microsoft Graph API for OneNote"""
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/open_city_data.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/open_city_data.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/oracleadb_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/oracleadb_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/oracleai.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/oracleai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/org_mode.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/org_mode.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/audio.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/audio.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/doc_intelligence.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/doc_intelligence.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/docai.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/docai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/generic.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/grobid.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/grobid.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/html/bs4.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/html/bs4.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/c.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/c.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/cobol.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/cobol.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/cpp.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/cpp.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/csharp.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/csharp.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/go.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/go.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/java.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/java.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/javascript.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/javascript.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/kotlin.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/kotlin.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/language_parser.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/language_parser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/lua.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/lua.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/perl.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/perl.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/php.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/php.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/python.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/python.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/ruby.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/ruby.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/rust.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/rust.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/scala.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/scala.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/tree_sitter_segmenter.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/tree_sitter_segmenter.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/language/typescript.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/language/typescript.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/msword.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/msword.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/pdf.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/pdf.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/registry.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/registry.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/txt.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/txt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/parsers/vsdx.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/parsers/vsdx.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/pdf.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/pdf.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,15 +687,15 @@
     ) -> Iterator[Document]:
         """Lazy load documents"""
         # the self.file_path is local, but the blob has to include
         # the S3 location if the file originated from S3 for multi-page documents
         # raises ValueError when multi-page and not on S3"""
 
         if self.web_path and self._is_s3_url(self.web_path):
-            blob = Blob(path=self.web_path)  # type: ignore[call-arg] # type: ignore[misc]
+            blob = Blob(path=self.web_path)  # type: ignore[misc]
         else:
             blob = Blob.from_path(self.file_path)  # type: ignore[attr-defined]
             if AmazonTextractPDFLoader._get_number_of_pages(blob) > 1:
                 raise ValueError(
                     f"the file {blob.path} is a multi-page document, \
                     but not stored on S3. \
                     Textract requires multi-page documents to be on S3."
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/pebblo.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/pebblo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/polars_dataframe.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/polars_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/powerpoint.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/powerpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/psychic.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/psychic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/pyspark_dataframe.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/pyspark_dataframe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/python.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/python.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/quip.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/quip.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/readthedocs.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/readthedocs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/recursive_url_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/recursive_url_loader.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/reddit.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/reddit.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/roam.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/roam.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/rocksetdb.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/rspace.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/rspace.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/rss.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/rss.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/rst.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/rst.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/rtf.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/rtf.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/s3_directory.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/s3_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/s3_file.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/s3_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/sharepoint.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/sharepoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/sitemap.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/sitemap.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/slack_directory.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/slack_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/snowflake_loader.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/snowflake_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             metadata_columns = []
         return page_content_columns or [], metadata_columns
 
     def lazy_load(self) -> Iterator[Document]:
         query_result = self._execute_query()
         if isinstance(query_result, Exception):
             print(f"An error occurred during the query: {query_result}")  # noqa: T201
-            return []  # type: ignore[return-value]
+            return []
         page_content_columns, metadata_columns = self._get_columns(query_result)
         if "*" in page_content_columns:
             page_content_columns = list(query_result[0].keys())
         for row in query_result:
             page_content = "\n".join(
                 f"{k}: {v}" for k, v in row.items() if k in page_content_columns
             )
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/spider.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/spider.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/spreedly.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/spreedly.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/sql_database.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/sql_database.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/srt.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/srt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/stripe.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/stripe.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/surrealdb.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/surrealdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/telegram.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/telegram.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/tencent_cos_directory.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/tencent_cos_directory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/tencent_cos_file.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/tencent_cos_file.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/tensorflow_datasets.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/tensorflow_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,16 +62,16 @@
         self.load_max_docs = load_max_docs
         """The maximum number of documents to load."""
         self.sample_to_document_function: Optional[
             Callable[[Dict], Document]
         ] = sample_to_document_function
         """Custom function that transform a dataset sample into a Document."""
 
-        self._tfds_client = TensorflowDatasets(  # type: ignore[call-arg]
+        self._tfds_client = TensorflowDatasets(
             dataset_name=self.dataset_name,
             split_name=self.split_name,
-            load_max_docs=self.load_max_docs,  # type: ignore[arg-type]
+            load_max_docs=self.load_max_docs,
             sample_to_document_function=self.sample_to_document_function,
         )
 
     def lazy_load(self) -> Iterator[Document]:
         yield from self._tfds_client.lazy_load()
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/text.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/tidb.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/tidb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/tomarkdown.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/tomarkdown.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/toml.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/toml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/trello.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/trello.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/tsv.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/tsv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/twitter.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/twitter.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/unstructured.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/unstructured.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/url.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/url.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/url_playwright.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/url_playwright.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/url_selenium.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/url_selenium.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/vsdx.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/vsdx.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/weather.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/weather.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.client = client
         self.places = places
 
     @classmethod
     def from_params(
         cls, places: Sequence[str], *, openweathermap_api_key: Optional[str] = None
     ) -> WeatherDataLoader:
-        client = OpenWeatherMapAPIWrapper(openweathermap_api_key=openweathermap_api_key)  # type: ignore[call-arg]
+        client = OpenWeatherMapAPIWrapper(openweathermap_api_key=openweathermap_api_key)
         return cls(client, places)
 
     def lazy_load(
         self,
     ) -> Iterator[Document]:
         """Lazily load weather data for the given locations."""
         for place in self.places:
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/web_base.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/web_base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/whatsapp_chat.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/whatsapp_chat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/wikipedia.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/wikipedia.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,14 +46,14 @@
         """
         Loads the query result from Wikipedia into a list of Documents.
 
         Returns:
             A list of Document objects representing the loaded
                 Wikipedia pages.
         """
-        client = WikipediaAPIWrapper(  # type: ignore[call-arg]
+        client = WikipediaAPIWrapper(
             lang=self.lang,
-            top_k_results=self.load_max_docs,  # type: ignore[arg-type]
-            load_all_available_meta=self.load_all_available_meta,  # type: ignore[arg-type]
-            doc_content_chars_max=self.doc_content_chars_max,  # type: ignore[arg-type]
+            top_k_results=self.load_max_docs,
+            load_all_available_meta=self.load_all_available_meta,
+            doc_content_chars_max=self.doc_content_chars_max,
         )
         yield from client.load(self.query)
```

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/word_document.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/word_document.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/xml.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/xml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/xorbits.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/xorbits.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/youtube.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/youtube.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_loaders/yuque.py` & `langchain_community-0.2.0rc1/langchain_community/document_loaders/yuque.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/beautiful_soup_transformer.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/beautiful_soup_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/doctran_text_extract.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/doctran_text_extract.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/doctran_text_qa.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/doctran_text_qa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/doctran_text_translate.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/doctran_text_translate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/embeddings_redundant_filter.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/embeddings_redundant_filter.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/google_translate.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/google_translate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/html2text.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/html2text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/long_context_reorder.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/markdownify.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/markdownify.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/nuclia_text_transform.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/nuclia_text_transform.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/openai_functions.py` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/openai_functions.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt` & `langchain_community-0.2.0rc1/langchain_community/document_transformers/xsl/html_chunks_with_headers.xslt`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/aleph_alpha.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/aleph_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/anyscale.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/anyscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/awa.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/awa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/azure_openai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/azure_openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/baichuan.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/baichuan.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,16 @@
                 # Sort resulting embeddings by index
                 sorted_embeddings = sorted(embeddings, key=lambda e: e.get("index", 0))
                 # Return just the embeddings
                 return [result.get("embedding", []) for result in sorted_embeddings]
             else:
                 # Log error or handle unsuccessful response appropriately
                 print(  # noqa: T201
-                    f"Error: Received status code {response.status_code} from "
-                    "embedding API"
+                    f"""Error: Received status code {response.status_code} from 
+                    embedding API"""
                 )
                 return None
         except Exception as e:
             # Log the exception or handle it as needed
             print(f"Exception occurred while trying to get embeddings: {str(e)}")  # noqa: T201
             return None
```

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/baidu_qianfan_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/bedrock.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/bookend.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/bookend.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/clarifai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/cloudflare_workersai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/cohere.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/dashscope.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/dashscope.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/databricks.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/databricks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/deepinfra.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/deepinfra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/edenai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/edenai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/elasticsearch.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/embaas.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/embaas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/ernie.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/ernie.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/fake.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/fake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/fastembed.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/fastembed.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/gigachat.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/gigachat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/google_palm.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/gpt4all.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/gradient_ai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/huggingface.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/huggingface_hub.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/infinity.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/infinity.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/infinity_local.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/infinity_local.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/itrex.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/itrex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/javelin_ai_gateway.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/jina.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/jina.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/johnsnowlabs.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/johnsnowlabs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/laser.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/laser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/llamacpp.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/llamafile.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/llamafile.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/llm_rails.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/llm_rails.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/localai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/localai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/minimax.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/minimax.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/mlflow.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/mlflow_gateway.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/mlflow_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/modelscope_hub.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/modelscope_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/mosaicml.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/mosaicml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/nemo.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/nemo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/nlpcloud.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/oci_generative_ai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/oci_generative_ai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/octoai_embeddings.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/octoai_embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/ollama.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/ollama.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/openai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/openvino.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/openvino.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/optimum_intel.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/optimum_intel.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/oracleai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/oracleai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/premai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/premai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/sagemaker_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/sambanova.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/sambanova.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/self_hosted.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/self_hosted.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/self_hosted_hugging_face.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/solar.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/solar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/spacy_embeddings.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/spacy_embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/sparkllm.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/sparkllm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/tensorflow_hub.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/tensorflow_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/text2vec.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/text2vec.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/titan_takeoff.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/titan_takeoff.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/vertexai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/volcengine.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/volcengine.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/voyageai.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/voyageai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/xinference.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/xinference.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/embeddings/yandex.py` & `langchain_community-0.2.0rc1/langchain_community/embeddings/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/example_selectors/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/example_selectors/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/example_selectors/ngram_overlap.py` & `langchain_community-0.2.0rc1/langchain_community/example_selectors/ngram_overlap.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/age_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/age_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/arangodb_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/arangodb_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/falkordb_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/falkordb_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/graph_document.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/graph_document.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/graph_store.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/graph_store.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/gremlin_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/gremlin_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/hugegraph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/hugegraph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/index_creator.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/index_creator.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/kuzu_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/kuzu_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/memgraph_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/memgraph_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/nebula_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/nebula_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/neo4j_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/neo4j_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,17 +569,17 @@
         self,
         label_or_type: str,
         properties: List[Dict[str, Any]],
         exhaustive: bool,
         is_relationship: bool = False,
     ) -> str:
         if is_relationship:
-            match_clause = f"MATCH ()-[n:`{label_or_type}`]->()"
+            match_clause = f"MATCH ()-[n:{label_or_type}]->()"
         else:
-            match_clause = f"MATCH (n:`{label_or_type}`)"
+            match_clause = f"MATCH (n:{label_or_type})"
 
         with_clauses = []
         return_clauses = []
         output_dict = {}
         if exhaustive:
             for prop in properties:
                 prop_name = prop["property"]
```

### Comparing `langchain_community-0.2.0/langchain_community/graphs/neptune_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/neptune_rdf_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/neptune_rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/networkx_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/networkx_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/ontotext_graphdb_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/ontotext_graphdb_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/rdf_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/graphs/tigergraph_graph.py` & `langchain_community-0.2.0rc1/langchain_community/graphs/tigergraph_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/indexes/_document_manager.py` & `langchain_community-0.2.0rc1/langchain_community/indexes/_document_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/indexes/_sql_record_manager.py` & `langchain_community-0.2.0rc1/langchain_community/indexes/_sql_record_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
                     ),
                 )
             elif self.dialect == "postgresql":
                 from sqlalchemy.dialects.postgresql import insert as pg_insert
 
                 # Note: uses SQLite insert to make on_conflict_do_update work.
                 # This code needs to be generalized a bit to work with more dialects.
-                insert_stmt = pg_insert(UpsertionRecord).values(records_to_upsert)  # type: ignore[assignment]
+                insert_stmt = pg_insert(UpsertionRecord).values(records_to_upsert)
                 stmt = insert_stmt.on_conflict_do_update(  # type: ignore[attr-defined]
                     "uix_key_namespace",  # Name of constraint
                     set_=dict(
                         # attr-defined type ignore
                         updated_at=insert_stmt.excluded.updated_at,  # type: ignore
                         group_id=insert_stmt.excluded.group_id,  # type: ignore
                     ),
@@ -383,15 +383,15 @@
                     ),
                 )
             elif self.dialect == "postgresql":
                 from sqlalchemy.dialects.postgresql import insert as pg_insert
 
                 # Note: uses SQLite insert to make on_conflict_do_update work.
                 # This code needs to be generalized a bit to work with more dialects.
-                insert_stmt = pg_insert(UpsertionRecord).values(records_to_upsert)  # type: ignore[assignment]
+                insert_stmt = pg_insert(UpsertionRecord).values(records_to_upsert)
                 stmt = insert_stmt.on_conflict_do_update(  # type: ignore[attr-defined]
                     "uix_key_namespace",  # Name of constraint
                     set_=dict(
                         # attr-defined type ignore
                         updated_at=insert_stmt.excluded.updated_at,  # type: ignore
                         group_id=insert_stmt.excluded.group_id,  # type: ignore
                     ),
@@ -466,15 +466,15 @@
                 query = query.filter(  # type: ignore[attr-defined]
                     UpsertionRecord.group_id.in_(group_ids)
                 )
 
             if limit:
                 query = query.limit(limit)  # type: ignore[attr-defined]
             records = query.all()  # type: ignore[attr-defined]
-        return [r.key for r in records]  # type: ignore[misc]
+        return [r.key for r in records]
 
     async def alist_keys(
         self,
         *,
         before: Optional[float] = None,
         after: Optional[float] = None,
         group_ids: Optional[Sequence[str]] = None,
```

### Comparing `langchain_community-0.2.0/langchain_community/indexes/base.py` & `langchain_community-0.2.0rc1/langchain_community/indexes/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/ai21.py` & `langchain_community-0.2.0rc1/langchain_community/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/aleph_alpha.py` & `langchain_community-0.2.0rc1/langchain_community/llms/aleph_alpha.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,10 +278,10 @@
         # In order to make this consistent with other endpoints, we strip them.
         if stop is not None or self.stop_sequences is not None:
             text = enforce_stop_tokens(text, params["stop_sequences"])
         return text
 
 
 if __name__ == "__main__":
-    aa = AlephAlpha()  # type: ignore[call-arg]
+    aa = AlephAlpha()
 
     print(aa.invoke("How are you?"))  # noqa: T201
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/amazon_api_gateway.py` & `langchain_community-0.2.0rc1/langchain_community/llms/amazon_api_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/anthropic.py` & `langchain_community-0.2.0rc1/langchain_community/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/anyscale.py` & `langchain_community-0.2.0rc1/langchain_community/llms/anyscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/aphrodite.py` & `langchain_community-0.2.0rc1/langchain_community/llms/aphrodite.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/arcee.py` & `langchain_community-0.2.0rc1/langchain_community/llms/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/aviary.py` & `langchain_community-0.2.0rc1/langchain_community/llms/aviary.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/azureml_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/llms/azureml_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/baichuan.py` & `langchain_community-0.2.0rc1/langchain_community/llms/baichuan.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/baidu_qianfan_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/llms/baidu_qianfan_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/bananadev.py` & `langchain_community-0.2.0rc1/langchain_community/llms/bananadev.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/baseten.py` & `langchain_community-0.2.0rc1/langchain_community/llms/baseten.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/beam.py` & `langchain_community-0.2.0rc1/langchain_community/llms/beam.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/bedrock.py` & `langchain_community-0.2.0rc1/langchain_community/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/bigdl_llm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/bigdl_llm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/bittensor.py` & `langchain_community-0.2.0rc1/langchain_community/llms/bittensor.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/cerebriumai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/cerebriumai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/chatglm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/chatglm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/chatglm3.py` & `langchain_community-0.2.0rc1/langchain_community/llms/chatglm3.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/clarifai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/cloudflare_workersai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/cloudflare_workersai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/cohere.py` & `langchain_community-0.2.0rc1/langchain_community/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/ctransformers.py` & `langchain_community-0.2.0rc1/langchain_community/llms/ctransformers.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/ctranslate2.py` & `langchain_community-0.2.0rc1/langchain_community/llms/ctranslate2.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/databricks.py` & `langchain_community-0.2.0rc1/langchain_community/llms/databricks.py`

 * *Files 0% similar despite different names*

```diff
@@ -486,15 +486,15 @@
                 host=self.host,
                 api_token=self.api_token,
                 endpoint_name=self.endpoint_name,
                 databricks_uri=self.databricks_uri,
                 task=self.task,
             )
         elif self.cluster_id and self.cluster_driver_port:
-            self._client = _DatabricksClusterDriverProxyClient(  # type: ignore[call-arg]
+            self._client = _DatabricksClusterDriverProxyClient(
                 host=self.host,
                 api_token=self.api_token,
                 cluster_id=self.cluster_id,
                 cluster_driver_port=self.cluster_driver_port,
             )
         else:
             raise ValueError(
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/deepinfra.py` & `langchain_community-0.2.0rc1/langchain_community/llms/deepinfra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/deepsparse.py` & `langchain_community-0.2.0rc1/langchain_community/llms/deepsparse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/edenai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/edenai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/exllamav2.py` & `langchain_community-0.2.0rc1/langchain_community/llms/exllamav2.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/fake.py` & `langchain_community-0.2.0rc1/langchain_community/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/fireworks.py` & `langchain_community-0.2.0rc1/langchain_community/llms/fireworks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/forefrontai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/forefrontai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/friendli.py` & `langchain_community-0.2.0rc1/langchain_community/llms/friendli.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/gigachat.py` & `langchain_community-0.2.0rc1/langchain_community/llms/gigachat.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/google_palm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/google_palm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/gooseai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/gooseai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/gpt4all.py` & `langchain_community-0.2.0rc1/langchain_community/llms/gpt4all.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/gradient_ai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/gradient_ai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/grammars/json.gbnf` & `langchain_community-0.2.0rc1/langchain_community/llms/grammars/json.gbnf`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/huggingface_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/llms/huggingface_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import logging
 from typing import Any, AsyncIterator, Dict, Iterator, List, Mapping, Optional
 
-from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models.llms import LLM
 from langchain_core.outputs import GenerationChunk
 from langchain_core.pydantic_v1 import Extra, Field, root_validator
@@ -18,19 +17,14 @@
     "text2text-generation",
     "text-generation",
     "summarization",
     "conversational",
 )
 
 
-@deprecated(
-    since="0.0.37",
-    removal="0.3",
-    alternative_import="from langchain_huggingface.llms import HuggingFaceEndpoint",
-)
 class HuggingFaceEndpoint(LLM):
     """
     HuggingFace Endpoint.
 
     To use this class, you should have installed the ``huggingface_hub`` package, and
     the environment variable ``HUGGINGFACEHUB_API_TOKEN`` set with your API token,
     or given as a named parameter to the constructor.
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/huggingface_hub.py` & `langchain_community-0.2.0rc1/langchain_community/llms/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/huggingface_pipeline.py` & `langchain_community-0.2.0rc1/langchain_community/llms/huggingface_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
 import importlib.util
 import logging
 from typing import Any, List, Mapping, Optional
 
-from langchain_core._api.deprecation import deprecated
 from langchain_core.callbacks import CallbackManagerForLLMRun
 from langchain_core.language_models.llms import BaseLLM
 from langchain_core.outputs import Generation, LLMResult
 from langchain_core.pydantic_v1 import Extra
 
 DEFAULT_MODEL_ID = "gpt2"
 DEFAULT_TASK = "text-generation"
@@ -19,19 +18,14 @@
     "translation",
 )
 DEFAULT_BATCH_SIZE = 4
 
 logger = logging.getLogger(__name__)
 
 
-@deprecated(
-    since="0.0.37",
-    removal="0.3",
-    alternative_import="from rom langchain_huggingface.llms import HuggingFacePipeline",
-)
 class HuggingFacePipeline(BaseLLM):
     """HuggingFace Pipeline API.
 
     To use, you should have the ``transformers`` python package installed.
 
     Only supports `text-generation`, `text2text-generation`, `summarization` and
     `translation`  for now.
@@ -208,15 +202,15 @@
                     "Device has %d GPUs available. "
                     "Provide device={deviceId} to `from_model_id` to use available"
                     "GPUs for execution. deviceId is -1 (default) for CPU and "
                     "can be a positive integer associated with CUDA device id.",
                     cuda_device_count,
                 )
         if device is not None and device_map is not None and backend == "openvino":
-            logger.warning("Please set device for OpenVINO through: `model_kwargs`")
+            logger.warning("Please set device for OpenVINO through: " "'model_kwargs'")
         if "trust_remote_code" in _model_kwargs:
             _model_kwargs = {
                 k: v for k, v in _model_kwargs.items() if k != "trust_remote_code"
             }
         _pipeline_kwargs = pipeline_kwargs or {}
         pipeline = hf_pipeline(
             task=task,
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/huggingface_text_gen_inference.py` & `langchain_community-0.2.0rc1/langchain_community/llms/huggingface_text_gen_inference.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/human.py` & `langchain_community-0.2.0rc1/langchain_community/llms/human.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/ipex_llm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/ipex_llm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/javelin_ai_gateway.py` & `langchain_community-0.2.0rc1/langchain_community/llms/javelin_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/koboldai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/koboldai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/konko.py` & `langchain_community-0.2.0rc1/langchain_community/llms/konko.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/layerup_security.py` & `langchain_community-0.2.0rc1/langchain_community/llms/layerup_security.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/llamacpp.py` & `langchain_community-0.2.0rc1/langchain_community/llms/llamacpp.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/llamafile.py` & `langchain_community-0.2.0rc1/langchain_community/llms/llamafile.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/loading.py` & `langchain_community-0.2.0rc1/langchain_community/llms/loading.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/manifest.py` & `langchain_community-0.2.0rc1/langchain_community/llms/manifest.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/minimax.py` & `langchain_community-0.2.0rc1/langchain_community/llms/minimax.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         # Get custom api url from environment.
         values["minimax_api_host"] = get_from_dict_or_env(
             values,
             "minimax_api_host",
             "MINIMAX_API_HOST",
             default="https://api.minimax.chat",
         )
-        values["_client"] = _MinimaxEndpointClient(  # type: ignore[call-arg]
+        values["_client"] = _MinimaxEndpointClient(
             host=values["minimax_api_host"],
             api_key=values["minimax_api_key"],
             group_id=values["minimax_group_id"],
         )
         return values
 
     @property
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/mlflow.py` & `langchain_community-0.2.0rc1/langchain_community/llms/mlflow.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/mlflow_ai_gateway.py` & `langchain_community-0.2.0rc1/langchain_community/llms/mlflow_ai_gateway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/mlx_pipeline.py` & `langchain_community-0.2.0rc1/langchain_community/llms/mlx_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/modal.py` & `langchain_community-0.2.0rc1/langchain_community/llms/modal.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/moonshot.py` & `langchain_community-0.2.0rc1/langchain_community/llms/moonshot.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/mosaicml.py` & `langchain_community-0.2.0rc1/langchain_community/llms/mosaicml.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/nlpcloud.py` & `langchain_community-0.2.0rc1/langchain_community/llms/nlpcloud.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/oci_data_science_model_deployment_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/llms/oci_data_science_model_deployment_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/oci_generative_ai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/oci_generative_ai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/octoai_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/llms/octoai_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/ollama.py` & `langchain_community-0.2.0rc1/langchain_community/llms/ollama.py`

 * *Files 1% similar despite different names*

```diff
@@ -419,15 +419,15 @@
                 stop=stop,
                 images=images,
                 run_manager=run_manager,
                 verbose=self.verbose,
                 **kwargs,
             )
             generations.append([final_chunk])
-        return LLMResult(generations=generations)  # type: ignore[arg-type]
+        return LLMResult(generations=generations)
 
     async def _agenerate(  # type: ignore[override]
         self,
         prompts: List[str],
         stop: Optional[List[str]] = None,
         images: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
@@ -455,15 +455,15 @@
                 stop=stop,
                 images=images,
                 run_manager=run_manager,  # type: ignore[arg-type]
                 verbose=self.verbose,
                 **kwargs,
             )
             generations.append([final_chunk])
-        return LLMResult(generations=generations)  # type: ignore[arg-type]
+        return LLMResult(generations=generations)
 
     def _stream(
         self,
         prompt: str,
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/opaqueprompts.py` & `langchain_community-0.2.0rc1/langchain_community/llms/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/openai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/openllm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/openllm.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
                 openllm.client.HTTPClient
                 if server_type == "http"
                 else openllm.client.GrpcClient
             )
             client = client_cls(server_url, timeout)
 
             super().__init__(
-                **{  # type: ignore[arg-type]
+                **{
                     "server_url": server_url,
                     "timeout": timeout,
                     "server_type": server_type,
                     "llm_kwargs": llm_kwargs,
                 }
             )
             self._runner = None  # type: ignore
@@ -176,15 +176,15 @@
                 model_name=model_name,
                 model_id=model_id,
                 init_local=embedded,
                 ensure_available=True,
                 **llm_kwargs,
             )
             super().__init__(
-                **{  # type: ignore[arg-type]
+                **{
                     "model_name": model_name,
                     "model_id": model_id,
                     "embedded": embedded,
                     "llm_kwargs": llm_kwargs,
                 }
             )
             self._client = None  # type: ignore
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/openlm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/openlm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/pai_eas_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/llms/pai_eas_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/petals.py` & `langchain_community-0.2.0rc1/langchain_community/llms/petals.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/pipelineai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/pipelineai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/predibase.py` & `langchain_community-0.2.0rc1/langchain_community/llms/predibase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/predictionguard.py` & `langchain_community-0.2.0rc1/langchain_community/llms/predictionguard.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/promptlayer_openai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/promptlayer_openai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/replicate.py` & `langchain_community-0.2.0rc1/langchain_community/llms/replicate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/rwkv.py` & `langchain_community-0.2.0rc1/langchain_community/llms/rwkv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/sagemaker_endpoint.py` & `langchain_community-0.2.0rc1/langchain_community/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/sambanova.py` & `langchain_community-0.2.0rc1/langchain_community/llms/sambanova.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,49 +43,44 @@
 
         :param requests.Response response: the response object to process
         :return: the response dict
         :rtype: dict
         """
         result: Dict[str, Any] = {}
         try:
-            lines_result = response.text.strip().split("\n")
-            text_result = lines_result[-1]
-            if response.status_code == 200 and json.loads(text_result).get("error"):
-                completion = ""
-                for line in lines_result[:-1]:
-                    completion += json.loads(line)["result"]["responses"][0][
-                        "stream_token"
-                    ]
-                text_result = lines_result[-2]
-                result = json.loads(text_result)
-                result["result"]["responses"][0]["completion"] = completion
-            else:
-                result = json.loads(text_result)
+            text_result = response.text.strip().split("\n")[-1]
+            result = {"data": json.loads("".join(text_result.split("data: ")[1:]))}
         except Exception as e:
             result["detail"] = str(e)
         if "status_code" not in result:
             result["status_code"] = response.status_code
         return result
 
     @staticmethod
     def _process_streaming_response(
         response: requests.Response,
-    ) -> Generator[Dict, None, None]:
+    ) -> Generator[GenerationChunk, None, None]:
         """Process the streaming response"""
         try:
-            for line in response.iter_lines():
-                chunk = json.loads(line)
-                if "status_code" not in chunk:
-                    chunk["status_code"] = response.status_code
-                if chunk["status_code"] == 200 and chunk.get("error"):
-                    chunk["result"] = {"responses": [{"stream_token": ""}]}
-                    return chunk
-                yield chunk
-        except Exception as e:
-            raise RuntimeError(f"Error processing streaming response: {e}")
+            import sseclient
+        except ImportError:
+            raise ImportError(
+                "could not import sseclient library"
+                "Please install it with `pip install sseclient-py`."
+            )
+        client = sseclient.SSEClient(response)
+        close_conn = False
+        for event in client.events():
+            if event.event == "error_event":
+                close_conn = True
+            text = json.dumps({"event": event.event, "data": event.data})
+            chunk = GenerationChunk(text=text)
+            yield chunk
+        if close_conn:
+            client.close()
 
     def _get_full_url(self) -> str:
         """
         Return the full API URL for a given path.
         :returns: the full API URL for the sub-path
         :rtype: str
         """
@@ -106,29 +101,33 @@
         :param str endpoint: Endpoint ID
         :param str key: API Key
         :param str input_str: Input string
         :param str params: Input params string
         :returns: Prediction results
         :rtype: dict
         """
-        parsed_element = {
-            "conversation_id": "sambaverse-conversation-id",
-            "messages": [
-                {
-                    "message_id": 0,
-                    "role": "user",
-                    "content": input,
-                }
-            ],
-        }
-        parsed_input = json.dumps(parsed_element)
+        if isinstance(input, str):
+            input = [input]
+        parsed_input = []
+        for element in input:
+            parsed_element = {
+                "conversation_id": "sambaverse-conversation-id",
+                "messages": [
+                    {
+                        "message_id": 0,
+                        "role": "user",
+                        "content": element,
+                    }
+                ],
+            }
+            parsed_input.append(json.dumps(parsed_element))
         if params:
-            data = {"instance": parsed_input, "params": json.loads(params)}
+            data = {"inputs": parsed_input, "params": json.loads(params)}
         else:
-            data = {"instance": parsed_input}
+            data = {"inputs": parsed_input}
         response = self.http_session.post(
             self._get_full_url(),
             headers={
                 "key": key,
                 "Content-Type": "application/json",
                 "modelName": sambaverse_model_name,
             },
@@ -138,41 +137,45 @@
 
     def nlp_predict_stream(
         self,
         key: str,
         sambaverse_model_name: Optional[str],
         input: Union[List[str], str],
         params: Optional[str] = "",
-    ) -> Iterator[Dict]:
+    ) -> Iterator[GenerationChunk]:
         """
         NLP predict using inline input string.
 
         :param str project: Project ID in which the endpoint exists
         :param str endpoint: Endpoint ID
         :param str key: API Key
         :param str input_str: Input string
         :param str params: Input params string
         :returns: Prediction results
         :rtype: dict
         """
-        parsed_element = {
-            "conversation_id": "sambaverse-conversation-id",
-            "messages": [
-                {
-                    "message_id": 0,
-                    "role": "user",
-                    "content": input,
-                }
-            ],
-        }
-        parsed_input = json.dumps(parsed_element)
+        if isinstance(input, str):
+            input = [input]
+        parsed_input = []
+        for element in input:
+            parsed_element = {
+                "conversation_id": "sambaverse-conversation-id",
+                "messages": [
+                    {
+                        "message_id": 0,
+                        "role": "user",
+                        "content": element,
+                    }
+                ],
+            }
+            parsed_input.append(json.dumps(parsed_element))
         if params:
-            data = {"instance": parsed_input, "params": json.loads(params)}
+            data = {"inputs": parsed_input, "params": json.loads(params)}
         else:
-            data = {"instance": parsed_input}
+            data = {"inputs": parsed_input}
         # Streaming output
         response = self.http_session.post(
             self._get_full_url(),
             headers={
                 "key": key,
                 "Content-Type": "application/json",
                 "modelName": sambaverse_model_name,
@@ -197,24 +200,23 @@
 
     Example:
     .. code-block:: python
 
         from langchain_community.llms.sambanova  import Sambaverse
         Sambaverse(
             sambaverse_url="https://sambaverse.sambanova.ai",
-            sambaverse_api_key="your-sambaverse-api-key",
-            sambaverse_model_name="Meta/llama-2-7b-chat-hf",
+            sambaverse_api_key: "your sambaverse api key",
+            sambaverse_model_name: "Meta/llama-2-7b-chat-hf",
             streaming: = False
             model_kwargs={
-                "select_expert": "llama-2-7b-chat-hf",
                 "do_sample": False,
                 "max_tokens_to_generate": 100,
                 "temperature": 0.7,
                 "top_p": 1.0,
-                "repetition_penalty": 1.0,
+                "repetition_penalty": 1,
                 "top_k": 50,
             },
         )
     """
 
     sambaverse_url: str = "https://sambaverse.sambanova.ai"
     """Sambaverse url to use"""
@@ -272,25 +274,21 @@
             stop: Stop words to use when generating. Model output is cut off at the
                 first occurrence of any of the stop substrings.
 
         Returns:
             The tuning parameters as a JSON string.
         """
         _model_kwargs = self.model_kwargs or {}
-        _kwarg_stop_sequences = _model_kwargs.get("stop_sequences", [])
-        _stop_sequences = stop or _kwarg_stop_sequences
-        if not _kwarg_stop_sequences:
-            _model_kwargs["stop_sequences"] = ",".join(
-                f'"{x}"' for x in _stop_sequences
-            )
+        _stop_sequences = _model_kwargs.get("stop_sequences", [])
+        _stop_sequences = stop or _stop_sequences
+        _model_kwargs["stop_sequences"] = ",".join(f'"{x}"' for x in _stop_sequences)
         tuning_params_dict = {
             k: {"type": type(v).__name__, "value": str(v)}
             for k, v in (_model_kwargs.items())
         }
-        _model_kwargs["stop_sequences"] = _kwarg_stop_sequences
         tuning_params = json.dumps(tuning_params_dict)
         return tuning_params
 
     def _handle_nlp_predict(
         self,
         sdk: SVEndpointHandler,
         prompt: Union[List[str], str],
@@ -310,25 +308,22 @@
         Raises:
             ValueError: If the prediction fails.
         """
         response = sdk.nlp_predict(
             self.sambaverse_api_key, self.sambaverse_model_name, prompt, tuning_params
         )
         if response["status_code"] != 200:
-            optional_code = response["error"].get("code")
-            optional_details = response["error"].get("details")
-            optional_message = response["error"].get("message")
+            optional_details = response["details"]
+            optional_message = response["message"]
             raise ValueError(
                 f"Sambanova /complete call failed with status code "
-                f"{response['status_code']}."
-                f"Message: {optional_message}"
-                f"Details: {optional_details}"
-                f"Code: {optional_code}"
+                f"{response['status_code']}. Details: {optional_details}"
+                f"{response['status_code']}. Message: {optional_message}"
             )
-        return response["result"]["responses"][0]["completion"]
+        return response["data"]["completion"]
 
     def _handle_completion_requests(
         self, prompt: Union[List[str], str], stop: Optional[List[str]]
     ) -> str:
         """
         Perform a prediction using the Sambaverse endpoint handler.
 
@@ -359,28 +354,15 @@
 
         Returns:
             An iterator of GenerationChunks.
         """
         for chunk in sdk.nlp_predict_stream(
             self.sambaverse_api_key, self.sambaverse_model_name, prompt, tuning_params
         ):
-            if chunk["status_code"] != 200:
-                optional_code = chunk["error"].get("code")
-                optional_details = chunk["error"].get("details")
-                optional_message = chunk["error"].get("message")
-                raise ValueError(
-                    f"Sambanova /complete call failed with status code "
-                    f"{chunk['status_code']}."
-                    f"Message: {optional_message}"
-                    f"Details: {optional_details}"
-                    f"Code: {optional_code}"
-                )
-            text = chunk["result"]["responses"][0]["stream_token"]
-            generated_chunk = GenerationChunk(text=text)
-            yield generated_chunk
+            yield chunk
 
     def _stream(
         self,
         prompt: Union[List[str], str],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
@@ -632,19 +614,19 @@
     read extra documentation in https://docs.sambanova.ai/sambastudio/latest/index.html
 
     Example:
     .. code-block:: python
 
         from langchain_community.llms.sambanova  import Sambaverse
         SambaStudio(
-            sambastudio_base_url="your-SambaStudio-environment-URL",
-            sambastudio_project_id="your-SambaStudio-project-ID",
-            sambastudio_endpoint_id="your-SambaStudio-endpoint-ID",
-            sambastudio_api_key="your-SambaStudio-endpoint-API-key,
-            streaming=False
+            sambastudio_base_url="your SambaStudio environment URL",
+            sambastudio_project_id=set with your SambaStudio project ID.,
+            sambastudio_endpoint_id=set with your SambaStudio endpoint ID.,
+            sambastudio_api_key= set with your SambaStudio endpoint API key.,
+            streaming=false
             model_kwargs={
                 "do_sample": False,
                 "max_tokens_to_generate": 1000,
                 "temperature": 0.7,
                 "top_p": 1.0,
                 "repetition_penalty": 1,
                 "top_k": 50,
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/self_hosted.py` & `langchain_community-0.2.0rc1/langchain_community/llms/self_hosted.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/self_hosted_hugging_face.py` & `langchain_community-0.2.0rc1/langchain_community/llms/self_hosted_hugging_face.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/solar.py` & `langchain_community-0.2.0rc1/langchain_community/llms/solar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/sparkllm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/sparkllm.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,18 +270,18 @@
                 self.api_secret,
             ),
             on_message=self.on_message,
             on_error=self.on_error,
             on_close=self.on_close,
             on_open=self.on_open,
         )
-        ws.messages = messages  # type: ignore[attr-defined]
-        ws.user_id = user_id  # type: ignore[attr-defined]
-        ws.model_kwargs = self.model_kwargs if model_kwargs is None else model_kwargs  # type: ignore[attr-defined]
-        ws.streaming = streaming  # type: ignore[attr-defined]
+        ws.messages = messages
+        ws.user_id = user_id
+        ws.model_kwargs = self.model_kwargs if model_kwargs is None else model_kwargs
+        ws.streaming = streaming
         ws.run_forever()
 
     def arun(
         self,
         messages: List[Dict],
         user_id: str,
         model_kwargs: Optional[dict] = None,
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/stochasticai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/stochasticai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/symblai_nebula.py` & `langchain_community-0.2.0rc1/langchain_community/llms/symblai_nebula.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/textgen.py` & `langchain_community-0.2.0rc1/langchain_community/llms/textgen.py`

 * *Files 4% similar despite different names*

```diff
@@ -326,21 +326,21 @@
 
         websocket_client.send(json.dumps(request))
 
         while True:
             result = websocket_client.recv()
             result = json.loads(result)
 
-            if result["event"] == "text_stream":  # type: ignore[call-overload, index]
+            if result["event"] == "text_stream":
                 chunk = GenerationChunk(
-                    text=result["text"],  # type: ignore[call-overload, index]
+                    text=result["text"],
                     generation_info=None,
                 )
                 yield chunk
-            elif result["event"] == "stream_end":  # type: ignore[call-overload, index]
+            elif result["event"] == "stream_end":
                 websocket_client.close()
                 return
 
             if run_manager:
                 run_manager.on_llm_new_token(token=chunk.text)
 
     async def _astream(
@@ -399,19 +399,19 @@
 
         websocket_client.send(json.dumps(request))
 
         while True:
             result = websocket_client.recv()
             result = json.loads(result)
 
-            if result["event"] == "text_stream":  # type: ignore[call-overload, index]
+            if result["event"] == "text_stream":
                 chunk = GenerationChunk(
-                    text=result["text"],  # type: ignore[call-overload, index]
+                    text=result["text"],
                     generation_info=None,
                 )
                 yield chunk
-            elif result["event"] == "stream_end":  # type: ignore[call-overload, index]
+            elif result["event"] == "stream_end":
                 websocket_client.close()
                 return
 
             if run_manager:
                 await run_manager.on_llm_new_token(token=chunk.text)
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/titan_takeoff.py` & `langchain_community-0.2.0rc1/langchain_community/llms/titan_takeoff.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             models (List[ReaderConfig], optional): Any readers you'd like to
                 spin up on. Defaults to [].
 
         Raises:
             ImportError: If you haven't installed takeoff-client, you will
             get an ImportError. To remedy run `pip install 'takeoff-client==0.4.0'`
         """
-        super().__init__(  # type: ignore[call-arg]
+        super().__init__(
             base_url=base_url, port=port, mgmt_port=mgmt_port, streaming=streaming
         )
         try:
             from takeoff_client import TakeoffClient
         except ImportError:
             raise ImportError(
                 "takeoff-client is required for TitanTakeoff. "
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/together.py` & `langchain_community-0.2.0rc1/langchain_community/llms/together.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/tongyi.py` & `langchain_community-0.2.0rc1/langchain_community/llms/tongyi.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,25 +51,25 @@
         retry=(retry_if_exception_type(HTTPError)),
         before_sleep=before_sleep_log(logger, logging.WARNING),
     )
 
 
 def check_response(resp: Any) -> Any:
     """Check the response from the completion call."""
-    if resp["status_code"] == 200:
+    if resp.status_code == 200:
         return resp
-    elif resp["status_code"] in [400, 401]:
+    elif resp.status_code in [400, 401]:
         raise ValueError(
-            f"status_code: {resp['status_code']} \n "
-            f"code: {resp['code']} \n message: {resp['message']}"
+            f"status_code: {resp.status_code} \n "
+            f"code: {resp.code} \n message: {resp.message}"
         )
     else:
         raise HTTPError(
-            f"HTTP error occurred: status_code: {resp['status_code']} \n "
-            f"code: {resp['code']} \n message: {resp['message']}",
+            f"HTTP error occurred: status_code: {resp.status_code} \n "
+            f"code: {resp.code} \n message: {resp.message}",
             response=resp,
         )
 
 
 def generate_with_retry(llm: Tongyi, **kwargs: Any) -> Any:
     """Use tenacity to retry the completion call."""
     retry_decorator = _create_retry_decorator(llm)
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/vertexai.py` & `langchain_community-0.2.0rc1/langchain_community/llms/vertexai.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,15 +359,15 @@
                 is_gemini=self._is_gemini_model,
                 run_manager=run_manager,
                 **params,
             )
             generations.append(
                 [self._response_to_generation(r) for r in res.candidates]
             )
-        return LLMResult(generations=generations)  # type: ignore[arg-type]
+        return LLMResult(generations=generations)
 
     def _stream(
         self,
         prompt: str,
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/vllm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/volcengine_maas.py` & `langchain_community-0.2.0rc1/langchain_community/llms/volcengine_maas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/watsonxllm.py` & `langchain_community-0.2.0rc1/langchain_community/llms/watsonxllm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/weight_only_quantization.py` & `langchain_community-0.2.0rc1/langchain_community/llms/weight_only_quantization.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/writer.py` & `langchain_community-0.2.0rc1/langchain_community/llms/writer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/xinference.py` & `langchain_community-0.2.0rc1/langchain_community/llms/xinference.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
                 "Could not import RESTfulClient from xinference. Please install it"
                 " with `pip install xinference`."
             ) from e
 
         model_kwargs = model_kwargs or {}
 
         super().__init__(
-            **{  # type: ignore[arg-type]
+            **{
                 "server_url": server_url,
                 "model_uid": model_uid,
                 "model_kwargs": model_kwargs,
             }
         )
 
         if self.server_url is None:
```

### Comparing `langchain_community-0.2.0/langchain_community/llms/yandex.py` & `langchain_community-0.2.0rc1/langchain_community/llms/yandex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/llms/yuan2.py` & `langchain_community-0.2.0rc1/langchain_community/llms/yuan2.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/memory/kg.py` & `langchain_community-0.2.0rc1/langchain_community/memory/kg.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/memory/motorhead_memory.py` & `langchain_community-0.2.0rc1/langchain_community/memory/motorhead_memory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/memory/zep_memory.py` & `langchain_community-0.2.0rc1/langchain_community/memory/zep_memory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/output_parsers/ernie_functions.py` & `langchain_community-0.2.0rc1/langchain_community/output_parsers/ernie_functions.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/output_parsers/rail_parser.py` & `langchain_community-0.2.0rc1/langchain_community/output_parsers/rail_parser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/astradb.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/chroma.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/chroma.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/dashvector.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/dashvector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/databricks_vector_search.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/databricks_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/deeplake.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/deeplake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/dingo.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/dingo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/elasticsearch.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/milvus.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/mongodb_atlas.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/myscale.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/myscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/opensearch.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/opensearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/pgvector.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/pgvector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/pinecone.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/pinecone.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/qdrant.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/qdrant.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/redis.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/supabase.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/supabase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/tencentvectordb.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/tencentvectordb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/timescalevector.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/timescalevector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/vectara.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/vectara.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/query_constructors/weaviate.py` & `langchain_community-0.2.0rc1/langchain_community/query_constructors/weaviate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/arcee.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/arxiv.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/azure_ai_search.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/azure_ai_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/bedrock.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/bm25.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/bm25.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/breebs.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/breebs.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     To retrieve the list of all available Breebs : you can call https://breebs.promptbreeders.com/web/listbreebs
     """
 
     breeb_key: str
     url = "https://breebs.promptbreeders.com/knowledge"
 
     def __init__(self, breeb_key: str):
-        super().__init__(breeb_key=breeb_key)  # type: ignore[call-arg]
+        super().__init__(breeb_key=breeb_key)
         self.breeb_key = breeb_key
 
     def _get_relevant_documents(
         self, query: str, *, run_manager: CallbackManagerForRetrieverRun
     ) -> List[Document]:
         """Retrieve context for given query.
         Note that for time being there is no score."""
```

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/chaindesk.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/chaindesk.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/chatgpt_plugin_retriever.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/chatgpt_plugin_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/cohere_rag_retriever.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/cohere_rag_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/databerry.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/databerry.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/docarray.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/docarray.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/dria_index.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/dria_index.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         Initialize the DriaRetriever with a DriaAPIWrapper instance.
 
         Args:
             api_key: The API key for Dria.
             contract_id: The contract ID of the knowledge base to interact with.
         """
         api_wrapper = DriaAPIWrapper(api_key=api_key, contract_id=contract_id)
-        super().__init__(api_wrapper=api_wrapper, **kwargs)  # type: ignore[call-arg]
+        super().__init__(api_wrapper=api_wrapper, **kwargs)
 
     def create_knowledge_base(
         self,
         name: str,
         description: str,
         category: str = "Unspecified",
         embedding: str = "jina",
```

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/elastic_search_bm25.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/elastic_search_bm25.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/embedchain.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/embedchain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/google_cloud_documentai_warehouse.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/google_cloud_documentai_warehouse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/google_vertex_ai_search.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/google_vertex_ai_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/kay.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/kay.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/kendra.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/knn.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/knn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/metal.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/metal.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/milvus.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/outline.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/outline.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/pinecone_hybrid_search.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/pinecone_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/pubmed.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/qdrant_sparse_vector_retriever.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/qdrant_sparse_vector_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/rememberizer.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/rememberizer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/remote_retriever.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/remote_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/svm.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/svm.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/tavily_search_api.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/tavily_search_api.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/tfidf.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/tfidf.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/thirdai_neuraldb.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/thirdai_neuraldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 ])
 
                 documents = retriever.invoke("AI-driven music therapy")
         """
         NeuralDBRetriever._verify_thirdai_library(thirdai_key)
         from thirdai import neural_db as ndb
 
-        return cls(thirdai_key=thirdai_key, db=ndb.NeuralDB(**model_kwargs))  # type: ignore[arg-type]
+        return cls(thirdai_key=thirdai_key, db=ndb.NeuralDB(**model_kwargs))
 
     @classmethod
     def from_checkpoint(
         cls,
         checkpoint: Union[str, Path],
         thirdai_key: Optional[str] = None,
     ) -> NeuralDBRetriever:
@@ -104,15 +104,15 @@
                 ])
 
                 documents = retriever.invoke("AI-driven music therapy")
         """
         NeuralDBRetriever._verify_thirdai_library(thirdai_key)
         from thirdai import neural_db as ndb
 
-        return cls(thirdai_key=thirdai_key, db=ndb.NeuralDB.from_checkpoint(checkpoint))  # type: ignore[arg-type]
+        return cls(thirdai_key=thirdai_key, db=ndb.NeuralDB.from_checkpoint(checkpoint))
 
     @root_validator()
     def validate_environments(cls, values: Dict) -> Dict:
         """Validate ThirdAI environment variables."""
         values["thirdai_key"] = convert_to_secret_str(
             get_from_dict_or_env(
                 values,
```

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/vespa_retriever.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/vespa_retriever.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/weaviate_hybrid_search.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/weaviate_hybrid_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/web_research.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/web_research.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/wikipedia.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/you.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/you.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/zep.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/zep.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/retrievers/zilliz.py` & `langchain_community-0.2.0rc1/langchain_community/retrievers/zilliz.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/storage/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/storage/astradb.py` & `langchain_community-0.2.0rc1/langchain_community/storage/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/storage/mongodb.py` & `langchain_community-0.2.0rc1/langchain_community/storage/mongodb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/storage/redis.py` & `langchain_community-0.2.0rc1/langchain_community/storage/redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/storage/upstash_redis.py` & `langchain_community-0.2.0rc1/langchain_community/storage/upstash_redis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ainetwork/app.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/app.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ainetwork/base.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ainetwork/owner.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/owner.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ainetwork/rule.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/rule.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ainetwork/transfer.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/transfer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ainetwork/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ainetwork/value.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ainetwork/value.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/amadeus/closest_airport.py` & `langchain_community-0.2.0rc1/langchain_community/tools/amadeus/closest_airport.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/amadeus/flight_search.py` & `langchain_community-0.2.0rc1/langchain_community/tools/amadeus/flight_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/amadeus/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/amadeus/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/arxiv/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/arxiv/tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         "A wrapper around Arxiv.org "
         "Useful for when you need to answer questions about Physics, Mathematics, "
         "Computer Science, Quantitative Biology, Quantitative Finance, Statistics, "
         "Electrical Engineering, and Economics "
         "from scientific articles on arxiv.org. "
         "Input should be a search query."
     )
-    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: ArxivAPIWrapper = Field(default_factory=ArxivAPIWrapper)
     args_schema: Type[BaseModel] = ArxivInput
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/audio/huggingface_text_to_speech_inference.py` & `langchain_community-0.2.0rc1/langchain_community/tools/audio/huggingface_text_to_speech_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         elif file_naming_func == "timestamp":
             file_namer = lambda: str(int(datetime.now().timestamp()))  # noqa: E731
         else:
             raise ValueError(
                 f"Invalid value for 'file_naming_func': {file_naming_func}"
             )
 
-        super().__init__(  # type: ignore[call-arg]
+        super().__init__(
             model=model,
             file_extension=file_extension,
             api_url=f"{self._HUGGINGFACE_API_URL_ROOT}/{model}",
             destination_dir=destination_dir,
             file_namer=file_namer,
             huggingface_api_key=huggingface_api_key,
         )
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_ai_services/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_ai_services/document_intelligence.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/document_intelligence.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_ai_services/image_analysis.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/image_analysis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_ai_services/speech_to_text.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_ai_services/text_analytics_for_health.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/text_analytics_for_health.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_ai_services/text_to_speech.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_ai_services/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_ai_services/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/form_recognizer.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/image_analysis.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/image_analysis.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/speech2text.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/speech2text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/text2speech.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/text2speech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/text_analytics_health.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/text_analytics_health.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/azure_cognitive_services/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/azure_cognitive_services/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/bearly/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/bearly/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/bing_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/brave_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/brave_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/cassandra_database/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/cassandra_database/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/cassandra_database/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/cassandra_database/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/clickup/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/clickup/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/clickup/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/clickup/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/cogniswitch/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/cogniswitch/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/connery/models.py` & `langchain_community-0.2.0rc1/langchain_community/tools/connery/models.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/connery/service.py` & `langchain_community-0.2.0rc1/langchain_community/tools/connery/service.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/connery/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/connery/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/dataforseo_api_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/dataforseo_api_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/dataherald/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/dataherald/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ddg_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ddg_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/e2b_data_analysis/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/e2b_data_analysis/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/e2b_data_analysis/unparse.py` & `langchain_community-0.2.0rc1/langchain_community/tools/e2b_data_analysis/unparse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/audio_speech_to_text.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/audio_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/audio_text_to_speech.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/audio_text_to_speech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/edenai_base_tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/edenai_base_tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/image_explicitcontent.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/image_explicitcontent.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/image_objectdetection.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/image_objectdetection.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/ocr_identityparser.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/ocr_identityparser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/ocr_invoiceparser.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/ocr_invoiceparser.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/edenai/text_moderation.py` & `langchain_community-0.2.0rc1/langchain_community/tools/edenai/text_moderation.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/eleven_labs/text2speech.py` & `langchain_community-0.2.0rc1/langchain_community/tools/eleven_labs/text2speech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/copy.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/copy.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/delete.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/delete.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/file_search.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/file_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/list_dir.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/list_dir.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/move.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/move.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/read.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/read.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/file_management/write.py` & `langchain_community-0.2.0rc1/langchain_community/tools/file_management/write.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/github/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/github/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/github/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/github/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from langchain_community.utilities.github import GitHubAPIWrapper
 
 
 class GitHubAction(BaseTool):
     """Tool for interacting with the GitHub API."""
 
-    api_wrapper: GitHubAPIWrapper = Field(default_factory=GitHubAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: GitHubAPIWrapper = Field(default_factory=GitHubAPIWrapper)
     mode: str
     name: str = ""
     description: str = ""
     args_schema: Optional[Type[BaseModel]] = None
 
     def _run(
         self,
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/gitlab/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gitlab/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/gitlab/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gitlab/tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from langchain_community.utilities.gitlab import GitLabAPIWrapper
 
 
 class GitLabAction(BaseTool):
     """Tool for interacting with the GitLab API."""
 
-    api_wrapper: GitLabAPIWrapper = Field(default_factory=GitLabAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: GitLabAPIWrapper = Field(default_factory=GitLabAPIWrapper)
     mode: str
     name: str = ""
     description: str = ""
 
     def _run(
         self,
         instructions: str,
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/base.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 
         Args:
             api_resource: The api resource to use.
 
         Returns:
             A tool.
         """
-        return cls(service=api_resource)  # type: ignore[call-arg]
+        return cls(service=api_resource)
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/create_draft.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/create_draft.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/get_message.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/get_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 
         message_body = ""
         if email_msg.is_multipart():
             for part in email_msg.walk():
                 ctype = part.get_content_type()
                 cdispo = str(part.get("Content-Disposition"))
                 if ctype == "text/plain" and "attachment" not in cdispo:
-                    message_body = part.get_payload(decode=True).decode("utf-8")  # type: ignore[union-attr]
+                    message_body = part.get_payload(decode=True).decode("utf-8")
                     break
         else:
-            message_body = email_msg.get_payload(decode=True).decode("utf-8")  # type: ignore[union-attr]
+            message_body = email_msg.get_payload(decode=True).decode("utf-8")
 
         body = clean_email_body(message_body)
 
         return {
             "id": message_id,
             "threadId": message_data["threadId"],
             "snippet": message_data["snippet"],
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/get_thread.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/get_thread.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/search.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,22 +95,22 @@
             message_body = ""
             if email_msg.is_multipart():
                 for part in email_msg.walk():
                     ctype = part.get_content_type()
                     cdispo = str(part.get("Content-Disposition"))
                     if ctype == "text/plain" and "attachment" not in cdispo:
                         try:
-                            message_body = part.get_payload(decode=True).decode("utf-8")  # type: ignore[union-attr]
+                            message_body = part.get_payload(decode=True).decode("utf-8")
                         except UnicodeDecodeError:
-                            message_body = part.get_payload(decode=True).decode(  # type: ignore[union-attr]
+                            message_body = part.get_payload(decode=True).decode(
                                 "latin-1"
                             )
                         break
             else:
-                message_body = email_msg.get_payload(decode=True).decode("utf-8")  # type: ignore[union-attr]
+                message_body = email_msg.get_payload(decode=True).decode("utf-8")
 
             body = clean_email_body(message_body)
 
             results.append(
                 {
                     "id": message["id"],
                     "threadId": message_data["threadId"],
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/send_message.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/gmail/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/gmail/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/golden_query/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/golden_query/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_cloud/texttospeech.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_cloud/texttospeech.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_finance/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_finance/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_jobs/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_jobs/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_lens/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_lens/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_places/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_places/tool.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     name: str = "google_places"
     description: str = (
         "A wrapper around Google Places. "
         "Useful for when you need to validate or "
         "discover addressed from ambiguous text. "
         "Input should be a search query."
     )
-    api_wrapper: GooglePlacesAPIWrapper = Field(default_factory=GooglePlacesAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: GooglePlacesAPIWrapper = Field(default_factory=GooglePlacesAPIWrapper)
     args_schema: Type[BaseModel] = GooglePlacesSchema
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_scholar/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_scholar/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_serper/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_serper/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/google_trends/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/google_trends/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/graphql/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/graphql/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/human/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/human/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/ifttt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/ifttt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/jira/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/jira/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/jira/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/jira/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 from langchain_community.utilities.jira import JiraAPIWrapper
 
 
 class JiraAction(BaseTool):
     """Tool that queries the Atlassian Jira API."""
 
-    api_wrapper: JiraAPIWrapper = Field(default_factory=JiraAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: JiraAPIWrapper = Field(default_factory=JiraAPIWrapper)
     mode: str
     name: str = ""
     description: str = ""
 
     def _run(
         self,
         instructions: str,
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/json/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/json/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/memorize/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/memorize/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/merriam_webster/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/merriam_webster/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/metaphor_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/metaphor_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/mojeek_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/mojeek_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/multion/close_session.py` & `langchain_community-0.2.0rc1/langchain_community/tools/multion/close_session.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/multion/create_session.py` & `langchain_community-0.2.0rc1/langchain_community/tools/multion/create_session.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/multion/update_session.py` & `langchain_community-0.2.0rc1/langchain_community/tools/multion/update_session.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/nasa/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/nasa/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/nasa/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/nasa/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/nuclia/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/nuclia/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self._config["BACKEND"] = f"https://{zone}.nuclia.cloud/api/v1"
         key = os.environ.get("NUCLIA_NUA_KEY")
         if not key:
             raise ValueError("NUCLIA_NUA_KEY environment variable not set")
         else:
             self._config["NUA_KEY"] = key
         self._config["enable_ml"] = enable_ml
-        super().__init__()  # type: ignore[call-arg]
+        super().__init__()
 
     def _run(
         self,
         action: str,
         id: str,
         path: Optional[str],
         text: Optional[str],
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/office365/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/office365/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/office365/create_draft_message.py` & `langchain_community-0.2.0rc1/langchain_community/tools/office365/create_draft_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/office365/events_search.py` & `langchain_community-0.2.0rc1/langchain_community/tools/office365/events_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/office365/messages_search.py` & `langchain_community-0.2.0rc1/langchain_community/tools/office365/messages_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/office365/send_event.py` & `langchain_community-0.2.0rc1/langchain_community/tools/office365/send_event.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/office365/send_message.py` & `langchain_community-0.2.0rc1/langchain_community/tools/office365/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/office365/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/office365/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/openai_dalle_image_generation/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/openai_dalle_image_generation/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/openapi/utils/api_models.py` & `langchain_community-0.2.0rc1/langchain_community/tools/openapi/utils/api_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
         if not description and spec.paths is not None:
             description = spec.paths[path].description or spec.paths[path].summary
         return cls(
             operation_id=operation_id,
             description=description or "",
             base_url=spec.base_url,
             path=path,
-            method=method,  # type: ignore[arg-type]
+            method=method,
             properties=properties,
             request_body=api_request_body,
         )
 
     @staticmethod
     def ts_type_from_python(type_: SCHEMA_TYPE) -> str:
         if type_ is None:
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/openweathermap/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/openweathermap/tool.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from langchain_community.utilities.openweathermap import OpenWeatherMapAPIWrapper
 
 
 class OpenWeatherMapQueryRun(BaseTool):
     """Tool that queries the OpenWeatherMap API."""
 
     api_wrapper: OpenWeatherMapAPIWrapper = Field(
-        default_factory=OpenWeatherMapAPIWrapper  # type: ignore[arg-type]
+        default_factory=OpenWeatherMapAPIWrapper
     )
 
     name: str = "open_weather_map"
     description: str = (
         "A wrapper around OpenWeatherMap API. "
         "Useful for fetching current weather information for a specified location. "
         "Input should be a location string (e.g. London,GB)."
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/passio_nutrition_ai/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/passio_nutrition_ai/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/base.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,8 +50,8 @@
     def from_browser(
         cls,
         sync_browser: Optional[SyncBrowser] = None,
         async_browser: Optional[AsyncBrowser] = None,
     ) -> BaseBrowserTool:
         """Instantiate the tool."""
         lazy_import_playwright_browsers()
-        return cls(sync_browser=sync_browser, async_browser=async_browser)  # type: ignore[call-arg]
+        return cls(sync_browser=sync_browser, async_browser=async_browser)
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/click.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/click.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/current_page.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/current_page.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/extract_hyperlinks.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/extract_hyperlinks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/extract_text.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/extract_text.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/get_elements.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/get_elements.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/navigate.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/navigate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/navigate_back.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/navigate_back.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/playwright/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/playwright/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/plugin.py` & `langchain_community-0.2.0rc1/langchain_community/tools/plugin.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/polygon/aggregates.py` & `langchain_community-0.2.0rc1/langchain_community/tools/polygon/aggregates.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/polygon/financials.py` & `langchain_community-0.2.0rc1/langchain_community/tools/polygon/financials.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/polygon/last_quote.py` & `langchain_community-0.2.0rc1/langchain_community/tools/polygon/last_quote.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/polygon/ticker_news.py` & `langchain_community-0.2.0rc1/langchain_community/tools/polygon/ticker_news.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/powerbi/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/powerbi/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/powerbi/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/powerbi/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/pubmed/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/pubmed/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     description: str = (
         "A wrapper around PubMed. "
         "Useful for when you need to answer questions about medicine, health, "
         "and biomedical topics "
         "from biomedical literature, MEDLINE, life science journals, and online books. "
         "Input should be a search query."
     )
-    api_wrapper: PubMedAPIWrapper = Field(default_factory=PubMedAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: PubMedAPIWrapper = Field(default_factory=PubMedAPIWrapper)
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         """Use the PubMed tool."""
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/reddit_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/reddit_search/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """Tool that queries for posts on a subreddit."""
 
     name: str = "reddit_search"
     description: str = (
         "A tool that searches for posts on Reddit."
         "Useful when you need to know post information on a subreddit."
     )
-    api_wrapper: RedditSearchAPIWrapper = Field(default_factory=RedditSearchAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: RedditSearchAPIWrapper = Field(default_factory=RedditSearchAPIWrapper)
     args_schema: Type[BaseModel] = RedditSearchSchema
 
     def _run(
         self,
         query: str,
         sort: str,
         time_filter: str,
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/requests/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/requests/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/scenexplain/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/scenexplain/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
     name: str = "image_explainer"
     description: str = (
         "An Image Captioning Tool: Use this tool to generate a detailed caption "
         "for an image. The input can be an image file of any format, and "
         "the output will be a text description that covers every detail of the image."
     )
-    api_wrapper: SceneXplainAPIWrapper = Field(default_factory=SceneXplainAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: SceneXplainAPIWrapper = Field(default_factory=SceneXplainAPIWrapper)
 
     def _run(
         self, query: str, run_manager: Optional[CallbackManagerForToolRun] = None
     ) -> str:
         """Use the tool."""
         return self.api_wrapper.run(query)
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/searchapi/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/searchapi/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/searx_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/searx_search/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/semanticscholar/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/semanticscholar/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     description: str = (
         "A wrapper around semantischolar.org "
         "Useful for when you need to answer to questions"
         "from research papers."
         "Input should be a search query."
     )
     api_wrapper: SemanticScholarAPIWrapper = Field(
-        default_factory=SemanticScholarAPIWrapper  # type: ignore[arg-type]
+        default_factory=SemanticScholarAPIWrapper
     )
     args_schema: Type[BaseModel] = SemantscholarInput
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/shell/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/shell/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/slack/get_channel.py` & `langchain_community-0.2.0rc1/langchain_community/tools/slack/get_channel.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/slack/get_message.py` & `langchain_community-0.2.0rc1/langchain_community/tools/slack/get_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/slack/schedule_message.py` & `langchain_community-0.2.0rc1/langchain_community/tools/slack/schedule_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/slack/send_message.py` & `langchain_community-0.2.0rc1/langchain_community/tools/slack/send_message.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/slack/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/slack/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/sleep/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/sleep/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/spark_sql/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/spark_sql/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/spark_sql/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/spark_sql/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
     @root_validator(pre=True)
     def initialize_llm_chain(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if "llm_chain" not in values:
             from langchain.chains.llm import LLMChain
 
             values["llm_chain"] = LLMChain(
-                llm=values.get("llm"),  # type: ignore[arg-type]
+                llm=values.get("llm"),
                 prompt=PromptTemplate(
                     template=QUERY_CHECKER, input_variables=["query"]
                 ),
             )
 
         if values["llm_chain"].prompt.input_variables != ["query"]:
             raise ValueError(
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/sql_database/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/sql_database/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/sql_database/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/sql_database/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 
     @root_validator(pre=True)
     def initialize_llm_chain(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if "llm_chain" not in values:
             from langchain.chains.llm import LLMChain
 
             values["llm_chain"] = LLMChain(
-                llm=values.get("llm"),  # type: ignore[arg-type]
+                llm=values.get("llm"),
                 prompt=PromptTemplate(
                     template=QUERY_CHECKER, input_variables=["dialect", "query"]
                 ),
             )
 
         if values["llm_chain"].prompt.input_variables != ["dialect", "query"]:
             raise ValueError(
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/stackexchange/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/stackexchange/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/steam/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/steam/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/steam/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/steam/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/steamship_image_generation/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/steamship_image_generation/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/steamship_image_generation/utils.py` & `langchain_community-0.2.0rc1/langchain_community/tools/steamship_image_generation/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/tavily_search/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/tavily_search/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     name: str = "tavily_search_results_json"
     description: str = (
         "A search engine optimized for comprehensive, accurate, and trusted results. "
         "Useful for when you need to answer questions about current events. "
         "Input should be a search query."
     )
-    api_wrapper: TavilySearchAPIWrapper = Field(default_factory=TavilySearchAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: TavilySearchAPIWrapper = Field(default_factory=TavilySearchAPIWrapper)
     max_results: int = 5
     args_schema: Type[BaseModel] = TavilyInput
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
@@ -66,15 +66,15 @@
     name: str = "tavily_answer"
     description: str = (
         "A search engine optimized for comprehensive, accurate, and trusted results. "
         "Useful for when you need to answer questions about current events. "
         "Input should be a search query. "
         "This returns only the answer - not the original source data."
     )
-    api_wrapper: TavilySearchAPIWrapper = Field(default_factory=TavilySearchAPIWrapper)  # type: ignore[arg-type]
+    api_wrapper: TavilySearchAPIWrapper = Field(default_factory=TavilySearchAPIWrapper)
     args_schema: Type[BaseModel] = TavilyInput
 
     def _run(
         self,
         query: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> Union[List[Dict], str]:
```

### Comparing `langchain_community-0.2.0/langchain_community/tools/vectorstore/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/vectorstore/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/wikidata/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/wikidata/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/wikipedia/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/wikipedia/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/wolfram_alpha/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/wolfram_alpha/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/yahoo_finance_news.py` & `langchain_community-0.2.0rc1/langchain_community/tools/yahoo_finance_news.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/you/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/you/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/youtube/search.py` & `langchain_community-0.2.0rc1/langchain_community/tools/youtube/search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/zapier/prompt.py` & `langchain_community-0.2.0rc1/langchain_community/tools/zapier/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/tools/zapier/tool.py` & `langchain_community-0.2.0rc1/langchain_community/tools/zapier/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
             (eg. "get the latest email from Mike Knoop" for "Gmail: find email" action)
         params: a dict, optional. Any params provided will *override* AI guesses
             from `instructions` (see "understanding the AI guessing flow" here:
             https://nla.zapier.com/docs/using-the-api#ai-guessing)
 
     """
 
-    api_wrapper: ZapierNLAWrapper = Field(default_factory=ZapierNLAWrapper)  # type: ignore[arg-type]
+    api_wrapper: ZapierNLAWrapper = Field(default_factory=ZapierNLAWrapper)
     action_id: str
     params: Optional[dict] = None
     base_prompt: str = BASE_ZAPIER_TOOL_PROMPT
     zapier_description: str
     params_schema: Dict[str, str] = Field(default_factory=dict)
     name: str = ""
     description: str = ""
@@ -170,15 +170,15 @@
 class ZapierNLAListActions(BaseTool):
     """Tool to list all exposed actions for the user."""
 
     name: str = "ZapierNLA_list_actions"
     description: str = BASE_ZAPIER_TOOL_PROMPT + (
         "This tool returns a list of the user's exposed actions."
     )
-    api_wrapper: ZapierNLAWrapper = Field(default_factory=ZapierNLAWrapper)  # type: ignore[arg-type]
+    api_wrapper: ZapierNLAWrapper = Field(default_factory=ZapierNLAWrapper)
 
     def _run(
         self,
         _: str = "",
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         """Use the Zapier NLA tool to return a list of all exposed user actions."""
```

### Comparing `langchain_community-0.2.0/langchain_community/utilities/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/alpha_vantage.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/alpha_vantage.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/anthropic.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/anthropic.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/apify.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/apify.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/arcee.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/arcee.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/arxiv.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/arxiv.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/astradb.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/awslambda.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/awslambda.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/bibtex.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/bibtex.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/bing_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/bing_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-"""Util that calls Bing Search."""
+"""Util that calls Bing Search.
+
+In order to set this up, follow instructions at:
+https://levelup.gitconnected.com/api-tutorial-how-to-use-bing-web-search-api-in-python-4165d5592a7e
+"""
 from typing import Dict, List
 
 import requests
 from langchain_core.pydantic_v1 import BaseModel, Extra, Field, root_validator
 from langchain_core.utils import get_from_dict_or_env
 
 
 class BingSearchAPIWrapper(BaseModel):
-    """Wrapper for Bing Search API."""
+    """Wrapper for Bing Search API.
+
+    In order to set this up, follow instructions at:
+    https://levelup.gitconnected.com/api-tutorial-how-to-use-bing-web-search-api-in-python-4165d5592a7e
+    """
 
     bing_subscription_key: str
     bing_search_url: str
     k: int = 10
     search_kwargs: dict = Field(default_factory=dict)
     """Additional keyword arguments to pass to the search request."""
```

### Comparing `langchain_community-0.2.0/langchain_community/utilities/brave_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/brave_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/cassandra.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/cassandra.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/cassandra_database.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/cassandra_database.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/clickup.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/clickup.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/dalle_image_generator.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/dalle_image_generator.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/dataforseo_api_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/dataforseo_api_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/dataherald.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/dataherald.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/dria_index.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/dria_index.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/duckduckgo_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/github.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/github.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/gitlab.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/gitlab.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/golden_query.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/golden_query.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_finance.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_finance.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_jobs.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_jobs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_lens.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_lens.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_places_api.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_places_api.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_scholar.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_scholar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_serper.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_serper.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/google_trends.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/google_trends.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/graphql.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/infobip.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/infobip.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/jira.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/jira.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/max_compute.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/max_compute.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/merriam_webster.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/merriam_webster.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/metaphor_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/metaphor_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/mojeek_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/mojeek_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/nasa.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/nasa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/nvidia_riva.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/nvidia_riva.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/opaqueprompts.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/opaqueprompts.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/openapi.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/openweathermap.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/openweathermap.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/oracleai.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/oracleai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/outline.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/outline.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/passio_nutrition_ai.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/passio_nutrition_ai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/pebblo.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/pebblo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/polygon.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/polygon.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/portkey.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/portkey.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/powerbi.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/powerbi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/pubmed.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/pubmed.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/python.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/python.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/reddit_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/reddit_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/redis.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,8 +210,8 @@
     except redis.exceptions.RedisError:
         return False
 
 
 def _redis_cluster_client(redis_url: str, **kwargs: Any) -> RedisType:
     from redis.cluster import RedisCluster
 
-    return RedisCluster.from_url(redis_url, **kwargs)  # type: ignore[return-value]
+    return RedisCluster.from_url(redis_url, **kwargs)
```

### Comparing `langchain_community-0.2.0/langchain_community/utilities/rememberizer.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/rememberizer.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/requests.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/requests.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/scenexplain.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/scenexplain.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/searchapi.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/searchapi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/searx_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/searx_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/semanticscholar.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/semanticscholar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/serpapi.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/serpapi.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/spark_sql.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/spark_sql.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/sql_database.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/sql_database.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/stackexchange.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/stackexchange.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/steam.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/steam.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/tavily_search.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/tavily_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/tensorflow_datasets.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/tensorflow_datasets.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/twilio.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/twilio.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/vertexai.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/vertexai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/wikidata.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/wikidata.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/wikipedia.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/wikipedia.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/wolfram_alpha.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/you.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/you.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utilities/zapier.py` & `langchain_community-0.2.0rc1/langchain_community/utilities/zapier.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utils/ernie_functions.py` & `langchain_community-0.2.0rc1/langchain_community/utils/ernie_functions.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utils/google.py` & `langchain_community-0.2.0rc1/langchain_community/utils/google.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/utils/math.py` & `langchain_community-0.2.0rc1/langchain_community/utils/math.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/__init__.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/alibabacloud_opensearch.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/alibabacloud_opensearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/analyticdb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/analyticdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/annoy.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/annoy.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,34 @@
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 
 import numpy as np
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
-from langchain_core.utils import guard_import
 from langchain_core.vectorstores import VectorStore
 
 from langchain_community.docstore.base import Docstore
 from langchain_community.docstore.in_memory import InMemoryDocstore
 from langchain_community.vectorstores.utils import maximal_marginal_relevance
 
 INDEX_METRICS = frozenset(["angular", "euclidean", "manhattan", "hamming", "dot"])
 DEFAULT_METRIC = "angular"
 
 
 def dependable_annoy_import() -> Any:
     """Import annoy if available, otherwise raise error."""
-    return guard_import("annoy")
+    try:
+        import annoy
+    except ImportError:
+        raise ImportError(
+            "Could not import annoy python package. "
+            "Please install it with `pip install --user annoy` "
+        )
+    return annoy
 
 
 class Annoy(VectorStore):
     """`Annoy` vector store.
 
     To use, you should have the ``annoy`` python package installed.
 
@@ -290,15 +296,15 @@
         if metric not in INDEX_METRICS:
             raise ValueError(
                 (
                     f"Unsupported distance metric: {metric}. "
                     f"Expected one of {list(INDEX_METRICS)}"
                 )
             )
-        annoy = guard_import("annoy")
+        annoy = dependable_annoy_import()
         if not embeddings:
             raise ValueError("embeddings must be provided to build AnnoyIndex")
         f = len(embeddings[0])
         index = annoy.AnnoyIndex(f, metric=metric)
         for i, emb in enumerate(embeddings):
             index.add_item(i, emb)
         index.build(trees, n_jobs=n_jobs)
@@ -442,22 +448,22 @@
             raise ValueError(
                 "The de-serialization relies loading a pickle file. "
                 "Pickle files can be modified to deliver a malicious payload that "
                 "results in execution of arbitrary code on your machine."
                 "You will need to set `allow_dangerous_deserialization` to `True` to "
                 "enable deserialization. If you do this, make sure that you "
                 "trust the source of the data. For example, if you are loading a "
-                "file that you created, and know that no one else has modified the "
-                "file, then this is safe to do. Do not set this to `True` if you are "
-                "loading a file from an untrusted source (e.g., some random site on "
-                "the internet.)."
+                "file that you created, and no that no one else has modified the file, "
+                "then this is safe to do. Do not set this to `True` if you are loading "
+                "a file from an untrusted source (e.g., some random site on the "
+                "internet.)."
             )
         path = Path(folder_path)
         # load index separately since it is not picklable
-        annoy = guard_import("annoy")
+        annoy = dependable_annoy_import()
         # load docstore and index_to_docstore_id
         with open(path / "index.pkl", "rb") as file:
             docstore, index_to_docstore_id, config_object = pickle.load(file)
 
         f = int(config_object["ANNOY"]["f"])
         metric = config_object["ANNOY"]["metric"]
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/apache_doris.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/apache_doris.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/astradb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/atlas.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/atlas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/awadb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/awadb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/azure_cosmos_db.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/azure_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/azuresearch.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/azuresearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Any,
     Callable,
     ClassVar,
     Collection,
     Dict,
     Iterable,
     List,
-    Literal,
     Optional,
     Tuple,
     Type,
     Union,
 )
 
 import numpy as np
@@ -564,49 +563,30 @@
         """
         docs_and_scores = self.semantic_hybrid_search_with_score_and_rerank(
             query, k=k, filters=kwargs.get("filters", None)
         )
         return [doc for doc, _, _ in docs_and_scores]
 
     def semantic_hybrid_search_with_score(
-        self,
-        query: str,
-        k: int = 4,
-        score_type: Literal["score", "reranker_score"] = "score",
-        **kwargs: Any,
+        self, query: str, k: int = 4, **kwargs: Any
     ) -> List[Tuple[Document, float]]:
         """
         Returns the most similar indexed documents to the query text.
 
         Args:
             query (str): The query text for which to find similar documents.
             k (int): The number of documents to return. Default is 4.
-            score_type: Must either be "score" or "reranker_score".
-                Defaulted to "score".
 
         Returns:
-            List[Tuple[Document, float]]: A list of documents and their
-                corresponding scores.
+            List[Document]: A list of documents that are most similar to the query text.
         """
-        score_threshold = kwargs.pop("score_threshold", None)
         docs_and_scores = self.semantic_hybrid_search_with_score_and_rerank(
             query, k=k, filters=kwargs.get("filters", None)
         )
-        if score_type == "score":
-            return [
-                (doc, score)
-                for doc, score, _ in docs_and_scores
-                if score_threshold is None or score >= score_threshold
-            ]
-        elif score_type == "reranker_score":
-            return [
-                (doc, reranker_score)
-                for doc, _, reranker_score in docs_and_scores
-                if score_threshold is None or reranker_score >= score_threshold
-            ]
+        return [(doc, score) for doc, score, _ in docs_and_scores]
 
     def semantic_hybrid_search_with_score_and_rerank(
         self, query: str, k: int = 4, filters: Optional[str] = None
     ) -> List[Tuple[Document, float, float]]:
         """Return docs most similar to query with a hybrid query.
 
         Args:
@@ -732,25 +712,23 @@
 class AzureSearchVectorStoreRetriever(BaseRetriever):
     """Retriever that uses `Azure Cognitive Search`."""
 
     vectorstore: AzureSearch
     """Azure Search instance used to find similar documents."""
     search_type: str = "hybrid"
     """Type of search to perform. Options are "similarity", "hybrid",
-    "semantic_hybrid", "similarity_score_threshold", "hybrid_score_threshold", 
-    or "semantic_hybrid_score_threshold"."""
+    "semantic_hybrid", "similarity_score_threshold", "hybrid_score_threshold"."""
     k: int = 4
     """Number of documents to return."""
     allowed_search_types: ClassVar[Collection[str]] = (
         "similarity",
         "similarity_score_threshold",
         "hybrid",
         "hybrid_score_threshold",
         "semantic_hybrid",
-        "semantic_hybrid_score_threshold",
     )
 
     class Config:
         """Configuration for this pydantic object."""
 
         arbitrary_types_allowed = True
 
@@ -788,21 +766,14 @@
                 doc
                 for doc, _ in self.vectorstore.hybrid_search_with_relevance_scores(
                     query, k=self.k, **kwargs
                 )
             ]
         elif self.search_type == "semantic_hybrid":
             docs = self.vectorstore.semantic_hybrid_search(query, k=self.k, **kwargs)
-        elif self.search_type == "semantic_hybrid_score_threshold":
-            docs = [
-                doc
-                for doc, _ in self.vectorstore.semantic_hybrid_search_with_score(
-                    query, k=self.k, **kwargs
-                )
-            ]
         else:
             raise ValueError(f"search_type of {self.search_type} not allowed.")
         return docs
 
     async def _aget_relevant_documents(
         self,
         query: str,
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/bagel.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/bagel.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/baiducloud_vector_search.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/baiducloud_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/baiduvectordb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/baiduvectordb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/bigquery_vector_search.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/bigquery_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/cassandra.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/cassandra.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,43 @@
 from langchain_community.utilities.cassandra import SetupMode
 from langchain_community.vectorstores.utils import maximal_marginal_relevance
 
 CVST = TypeVar("CVST", bound="Cassandra")
 
 
 class Cassandra(VectorStore):
+    """Apache Cassandra(R) for vector-store workloads.
+
+    To use it, you need a recent installation of the `cassio` library
+    and a Cassandra cluster / Astra DB instance supporting vector capabilities.
+
+    Visit the cassio.org website for extensive quickstarts and code examples.
+
+    Example:
+        .. code-block:: python
+
+                from langchain_community.vectorstores import Cassandra
+                from langchain_community.embeddings.openai import OpenAIEmbeddings
+
+                embeddings = OpenAIEmbeddings()
+                session = ...             # create your Cassandra session object
+                keyspace = 'my_keyspace'  # the keyspace should exist already
+                table_name = 'my_vector_store'
+                vectorstore = Cassandra(embeddings, session, keyspace, table_name)
+
+    Args:
+        embedding: Embedding function to use.
+        session: Cassandra driver session. If not provided, it is resolved from cassio.
+        keyspace: Cassandra key space. If not provided, it is resolved from cassio.
+        table_name: Cassandra table (required).
+        ttl_seconds: Optional time-to-live for the added texts.
+        body_index_options: Optional options used to create the body index.
+            Eg. body_index_options = [cassio.table.cql.STANDARD_ANALYZER]
+    """
+
     _embedding_dimension: Union[int, None]
 
     def _get_embedding_dimension(self) -> int:
         if self._embedding_dimension is None:
             self._embedding_dimension = len(
                 self.embedding.embed_query("This is a sample sentence.")
             )
@@ -56,45 +85,14 @@
         keyspace: Optional[str] = None,
         table_name: str = "",
         ttl_seconds: Optional[int] = None,
         *,
         body_index_options: Optional[List[Tuple[str, Any]]] = None,
         setup_mode: SetupMode = SetupMode.SYNC,
     ) -> None:
-        """Apache Cassandra(R) for vector-store workloads.
-
-        To use it, you need a recent installation of the `cassio` library
-        and a Cassandra cluster / Astra DB instance supporting vector capabilities.
-
-        Visit the cassio.org website for extensive quickstarts and code examples.
-
-        Example:
-            .. code-block:: python
-
-                    from langchain_community.vectorstores import Cassandra
-                    from langchain_openai import OpenAIEmbeddings
-
-                    embeddings = OpenAIEmbeddings()
-                    session = ...             # create your Cassandra session object
-                    keyspace = 'my_keyspace'  # the keyspace should exist already
-                    table_name = 'my_vector_store'
-                    vectorstore = Cassandra(embeddings, session, keyspace, table_name)
-
-        Args:
-            embedding: Embedding function to use.
-            session: Cassandra driver session. If not provided, it is resolved from
-                cassio.
-            keyspace: Cassandra key space. If not provided, it is resolved from cassio.
-            table_name: Cassandra table (required).
-            ttl_seconds: Optional time-to-live for the added texts.
-            body_index_options: Optional options used to create the body index.
-                Eg. body_index_options = [cassio.table.cql.STANDARD_ANALYZER]
-            setup_mode: mode used to create the Cassandra table (SYNC,
-                ASYNC or OFF).
-        """
         try:
             from cassio.table import MetadataVectorCassandraTable
         except (ImportError, ModuleNotFoundError):
             raise ImportError(
                 "Could not import cassio python package. "
                 "Please install it with `pip install cassio`."
             )
@@ -162,27 +160,17 @@
         self.table.clear()
 
     async def aclear(self) -> None:
         """Empty the table."""
         await self.table.aclear()
 
     def delete_by_document_id(self, document_id: str) -> None:
-        """Delete by document ID.
-
-        Args:
-            document_id: the document ID to delete.
-        """
         return self.table.delete(row_id=document_id)
 
     async def adelete_by_document_id(self, document_id: str) -> None:
-        """Delete by document ID.
-
-        Args:
-            document_id: the document ID to delete.
-        """
         return await self.table.adelete(row_id=document_id)
 
     def delete(self, ids: Optional[List[str]] = None, **kwargs: Any) -> Optional[bool]:
         """Delete by vector IDs.
 
         Args:
             ids: List of ids to delete.
@@ -378,16 +366,16 @@
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
     ) -> List[Tuple[Document, float, str]]:
         """Return docs most similar to embedding vector.
 
         Args:
-            embedding: Embedding to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
+            embedding (str): Embedding to look up documents similar to.
+            k (int): Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
             body_search: Document textual search terms to apply.
                 Only supported by Astra DB at the moment.
         Returns:
             List of (Document, score, id), the most similar to the query vector.
         """
         kwargs: Dict[str, Any] = {}
@@ -407,25 +395,14 @@
     def similarity_search_with_score_id(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
     ) -> List[Tuple[Document, float, str]]:
-        """Return docs most similar to query.
-
-        Args:
-            query: Text to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of (Document, score, id), the most similar to the query vector.
-        """
         embedding_vector = self.embedding.embed_query(query)
         return self.similarity_search_with_score_id_by_vector(
             embedding=embedding_vector,
             k=k,
             filter=filter,
             body_search=body_search,
         )
@@ -433,25 +410,14 @@
     async def asimilarity_search_with_score_id(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
     ) -> List[Tuple[Document, float, str]]:
-        """Return docs most similar to query.
-
-        Args:
-            query: Text to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of (Document, score, id), the most similar to the query vector.
-        """
         embedding_vector = await self.embedding.aembed_query(query)
         return await self.asimilarity_search_with_score_id_by_vector(
             embedding=embedding_vector,
             k=k,
             filter=filter,
             body_search=body_search,
         )
@@ -491,16 +457,16 @@
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
     ) -> List[Tuple[Document, float]]:
         """Return docs most similar to embedding vector.
 
         Args:
-            embedding: Embedding to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
+            embedding (str): Embedding to look up documents similar to.
+            k (int): Number of Documents to return. Defaults to 4.
             filter: Filter on the metadata to apply.
             body_search: Document textual search terms to apply.
                 Only supported by Astra DB at the moment.
         Returns:
             List of (Document, score), the most similar to the query vector.
         """
         return [
@@ -521,25 +487,14 @@
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
         **kwargs: Any,
     ) -> List[Document]:
-        """Return docs most similar to query.
-
-        Args:
-            query: Text to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of Document, the most similar to the query vector.
-        """
         embedding_vector = self.embedding.embed_query(query)
         return self.similarity_search_by_vector(
             embedding_vector,
             k,
             filter=filter,
             body_search=body_search,
         )
@@ -548,25 +503,14 @@
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
         **kwargs: Any,
     ) -> List[Document]:
-        """Return docs most similar to query.
-
-        Args:
-            query: Text to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of Document, the most similar to the query vector.
-        """
         embedding_vector = await self.embedding.aembed_query(query)
         return await self.asimilarity_search_by_vector(
             embedding_vector,
             k,
             filter=filter,
             body_search=body_search,
         )
@@ -575,25 +519,14 @@
         self,
         embedding: List[float],
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
         **kwargs: Any,
     ) -> List[Document]:
-        """Return docs most similar to embedding vector.
-
-        Args:
-            embedding: Embedding to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of Document, the most similar to the query vector.
-        """
         return [
             doc
             for doc, _ in self.similarity_search_with_score_by_vector(
                 embedding,
                 k,
                 filter=filter,
                 body_search=body_search,
@@ -604,25 +537,14 @@
         self,
         embedding: List[float],
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
         **kwargs: Any,
     ) -> List[Document]:
-        """Return docs most similar to embedding vector.
-
-        Args:
-            embedding: Embedding to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of Document, the most similar to the query vector.
-        """
         return [
             doc
             for doc, _ in await self.asimilarity_search_with_score_by_vector(
                 embedding,
                 k,
                 filter=filter,
                 body_search=body_search,
@@ -632,25 +554,14 @@
     def similarity_search_with_score(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
     ) -> List[Tuple[Document, float]]:
-        """Return docs most similar to query.
-
-        Args:
-            query: Text to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of (Document, score), the most similar to the query vector.
-        """
         embedding_vector = self.embedding.embed_query(query)
         return self.similarity_search_with_score_by_vector(
             embedding_vector,
             k,
             filter=filter,
             body_search=body_search,
         )
@@ -658,25 +569,14 @@
     async def asimilarity_search_with_score(
         self,
         query: str,
         k: int = 4,
         filter: Optional[Dict[str, str]] = None,
         body_search: Optional[Union[str, List[str]]] = None,
     ) -> List[Tuple[Document, float]]:
-        """Return docs most similar to query.
-
-        Args:
-            query: Text to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            filter: Filter on the metadata to apply.
-            body_search: Document textual search terms to apply.
-                Only supported by Astra DB at the moment.
-        Returns:
-            List of (Document, score), the most similar to the query vector.
-        """
         embedding_vector = await self.embedding.aembed_query(query)
         return await self.asimilarity_search_with_score_by_vector(
             embedding_vector,
             k,
             filter=filter,
             body_search=body_search,
         )
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/chroma.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/clarifai.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/clarifai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/clickhouse.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/clickhouse.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/couchbase.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/couchbase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/dashvector.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/dashvector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/databricks_vector_search.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/databricks_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/deeplake.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/deeplake.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/dingo.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/dingo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/docarray/base.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/docarray/hnsw.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/docarray/in_memory.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/documentdb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/documentdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/duckdb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/duckdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/ecloud_vector_search.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/ecloud_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/elastic_vector_search.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/elastic_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/elasticsearch.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/epsilla.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/epsilla.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/faiss.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/faiss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1078,18 +1078,18 @@
             raise ValueError(
                 "The de-serialization relies loading a pickle file. "
                 "Pickle files can be modified to deliver a malicious payload that "
                 "results in execution of arbitrary code on your machine."
                 "You will need to set `allow_dangerous_deserialization` to `True` to "
                 "enable deserialization. If you do this, make sure that you "
                 "trust the source of the data. For example, if you are loading a "
-                "file that you created, and know that no one else has modified the "
-                "file, then this is safe to do. Do not set this to `True` if you are "
-                "loading a file from an untrusted source (e.g., some random site on "
-                "the internet.)."
+                "file that you created, and no that no one else has modified the file, "
+                "then this is safe to do. Do not set this to `True` if you are loading "
+                "a file from an untrusted source (e.g., some random site on the "
+                "internet.)."
             )
         path = Path(folder_path)
         # load index separately since it is not picklable
         faiss = dependable_faiss_import()
         index = faiss.read_index(str(path / f"{index_name}.faiss"))
 
         # load docstore and index_to_docstore_id
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/hanavector.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/hanavector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/hippo.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/hippo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/hologres.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/hologres.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/infinispanvs.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/infinispanvs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/inmemory.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/inmemory.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/jaguar.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/jaguar.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/kdbai.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/kdbai.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/kinetica.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/kinetica.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/lancedb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/lancedb.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,28 @@
 import os
 import uuid
 import warnings
 from typing import Any, Iterable, List, Optional
 
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
-from langchain_core.utils import guard_import
 from langchain_core.vectorstores import VectorStore
 
 
 def import_lancedb() -> Any:
     """Import lancedb package."""
-    return guard_import("lancedb")
+
+    try:
+        import lancedb
+    except ImportError as e:
+        raise ImportError(
+            "Could not import pinecone lancedb package. "
+            "Please install it with `pip install lancedb`."
+        ) from e
+    return lancedb
 
 
 class LanceDB(VectorStore):
     """`LanceDB` vector store.
 
     To use, you should have ``lancedb`` python package installed.
     You can install it with ``pip install lancedb``.
@@ -53,15 +60,15 @@
         text_key: Optional[str] = "text",
         table_name: Optional[str] = "vectorstore",
         api_key: Optional[str] = None,
         region: Optional[str] = None,
         mode: Optional[str] = "overwrite",
     ):
         """Initialize with Lance DB vectorstore"""
-        lancedb = guard_import("lancedb")
+        lancedb = import_lancedb()
         self._embedding = embedding
         self._vector_key = vector_key
         self._id_key = id_key
         self._text_key = text_key
         self._table_name = table_name
         self.api_key = api_key or os.getenv("LANCE_API_KEY") if api_key != "" else None
         self.region = region
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/lantern.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/lantern.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/llm_rails.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/llm_rails.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/marqo.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/marqo.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/matching_engine.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/matching_engine.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/meilisearch.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/meilisearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/milvus.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/milvus.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/momento_vector_index.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/momento_vector_index.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/mongodb_atlas.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/mongodb_atlas.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/myscale.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/myscale.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/neo4j_vector.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/neo4j_vector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/nucliadb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/nucliadb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/opensearch_vector_search.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/opensearch_vector_search.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/oraclevs.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/oraclevs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/pathway.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/pathway.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/pgembedding.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/pgembedding.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/pgvecto_rs.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/pgvecto_rs.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/pgvector.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/pgvector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/pinecone.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/qdrant.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/qdrant.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     Sequence,
     Tuple,
     Type,
     Union,
 )
 
 import numpy as np
-from langchain_core._api.deprecation import deprecated
 from langchain_core.embeddings import Embeddings
 from langchain_core.runnables.config import run_in_executor
 from langchain_core.vectorstores import VectorStore
 
 from langchain_community.docstore.document import Document
 from langchain_community.vectorstores.utils import maximal_marginal_relevance
 
@@ -62,17 +61,14 @@
             return await run_in_executor(
                 None, getattr(self, method.__name__[1:]), *args, **kwargs
             )
 
     return wrapper
 
 
-@deprecated(
-    since="0.0.37", removal="0.3.0", alternative_import="langchain_qdrant.Qdrant"
-)
 class Qdrant(VectorStore):
     """`Qdrant` vector store.
 
     To use you should have the ``qdrant-client`` package installed.
 
     Example:
         .. code-block:: python
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/redis/base.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/base.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/redis/filters.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/filters.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/redis/schema.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/redis/schema.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/relyt.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/relyt.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/rocksetdb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/rocksetdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/scann.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/scann.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import uuid
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple
 
 import numpy as np
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
-from langchain_core.utils import guard_import
 from langchain_core.vectorstores import VectorStore
 
 from langchain_community.docstore.base import AddableMixin, Docstore
 from langchain_community.docstore.in_memory import InMemoryDocstore
 from langchain_community.vectorstores.utils import DistanceStrategy
 
 
@@ -23,15 +22,22 @@
     return x
 
 
 def dependable_scann_import() -> Any:
     """
     Import `scann` if available, otherwise raise error.
     """
-    return guard_import("scann")
+    try:
+        import scann
+    except ImportError:
+        raise ImportError(
+            "Could not import scann python package. "
+            "Please install it with `pip install scann` "
+        )
+    return scann
 
 
 class ScaNN(VectorStore):
     """`ScaNN` vector store.
 
     To use, you should have the ``scann`` python package installed.
 
@@ -302,15 +308,15 @@
         embeddings: List[List[float]],
         embedding: Embeddings,
         metadatas: Optional[List[dict]] = None,
         ids: Optional[List[str]] = None,
         normalize_L2: bool = False,
         **kwargs: Any,
     ) -> ScaNN:
-        scann = guard_import("scann")
+        scann = dependable_scann_import()
         distance_strategy = kwargs.get(
             "distance_strategy", DistanceStrategy.EUCLIDEAN_DISTANCE
         )
         scann_config = kwargs.get("scann_config", None)
 
         vector = np.array(embeddings, dtype=np.float32)
         if normalize_L2:
@@ -459,15 +465,15 @@
         **kwargs: Any,
     ) -> ScaNN:
         """Load ScaNN index, docstore, and index_to_docstore_id from disk.
 
         Args:
             folder_path: folder path to load index, docstore,
                 and index_to_docstore_id from.
-            embedding: Embeddings to use when generating queries
+            embeddings: Embeddings to use when generating queries
             index_name: for saving with a specific index file name
             allow_dangerous_deserialization: whether to allow deserialization
                 of the data which involves loading a pickle file.
                 Pickle files can be modified by malicious actors to deliver a
                 malicious payload that results in execution of
                 arbitrary code on your machine.
         """
@@ -475,24 +481,24 @@
             raise ValueError(
                 "The de-serialization relies loading a pickle file. "
                 "Pickle files can be modified to deliver a malicious payload that "
                 "results in execution of arbitrary code on your machine."
                 "You will need to set `allow_dangerous_deserialization` to `True` to "
                 "enable deserialization. If you do this, make sure that you "
                 "trust the source of the data. For example, if you are loading a "
-                "file that you created, and know that no one else has modified the "
-                "file, then this is safe to do. Do not set this to `True` if you are "
-                "loading a file from an untrusted source (e.g., some random site on "
-                "the internet.)."
+                "file that you created, and no that no one else has modified the file, "
+                "then this is safe to do. Do not set this to `True` if you are loading "
+                "a file from an untrusted source (e.g., some random site on the "
+                "internet.)."
             )
         path = Path(folder_path)
         scann_path = path / "{index_name}.scann".format(index_name=index_name)
         scann_path.mkdir(exist_ok=True, parents=True)
         # load index separately since it is not picklable
-        scann = guard_import("scann")
+        scann = dependable_scann_import()
         index = scann.scann_ops_pybind.load_searcher(str(scann_path))
 
         # load docstore and index_to_docstore_id
         with open(path / "{index_name}.pkl".format(index_name=index_name), "rb") as f:
             docstore, index_to_docstore_id = pickle.load(f)
         return cls(embedding, index, docstore, index_to_docstore_id, **kwargs)
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/semadb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/semadb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/singlestoredb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/singlestoredb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/sklearn.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/sklearn.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/sqlitevss.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/sqlitevss.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/starrocks.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/starrocks.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/supabase.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/supabase.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/surrealdb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/surrealdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/tair.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/tair.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/tencentvectordb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/tencentvectordb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/thirdai_neuraldb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/thirdai_neuraldb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/tidb_vector.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/tidb_vector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/tigris.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/tigris.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/tiledb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/tiledb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Wrapper around TileDB vector database."""
-
 from __future__ import annotations
 
 import pickle
 import random
 import sys
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Tuple
 
 import numpy as np
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
-from langchain_core.utils import guard_import
 from langchain_core.vectorstores import VectorStore
 
 from langchain_community.vectorstores.utils import maximal_marginal_relevance
 
 INDEX_METRICS = frozenset(["euclidean"])
 DEFAULT_METRIC = "euclidean"
 DOCUMENTS_ARRAY_NAME = "documents"
@@ -22,18 +20,24 @@
 MAX_UINT64 = np.iinfo(np.dtype("uint64")).max
 MAX_FLOAT_32 = np.finfo(np.dtype("float32")).max
 MAX_FLOAT = sys.float_info.max
 
 
 def dependable_tiledb_import() -> Any:
     """Import tiledb-vector-search if available, otherwise raise error."""
-    return (
-        guard_import("tiledb.vector_search"),
-        guard_import("tiledb"),
-    )
+    try:
+        import tiledb as tiledb
+        import tiledb.vector_search as tiledb_vs
+    except ImportError:
+        raise ImportError(
+            "Could not import tiledb-vector-search python package. "
+            "Please install it with `conda install -c tiledb tiledb-vector-search` "
+            "or `pip install tiledb-vector-search`"
+        )
+    return tiledb_vs, tiledb
 
 
 def get_vector_index_uri_from_group(group: Any) -> str:
     """Get the URI of the vector index."""
     return group[VECTOR_INDEX_NAME].uri
 
 
@@ -107,18 +111,15 @@
             )
         self.embedding = embedding
         self.embedding_function = embedding.embed_query
         self.index_uri = index_uri
         self.metric = metric
         self.config = config
 
-        tiledb_vs, tiledb = (
-            guard_import("tiledb.vector_search"),
-            guard_import("tiledb"),
-        )
+        tiledb_vs, tiledb = dependable_tiledb_import()
         with tiledb.scope_ctx(ctx_or_config=config):
             index_group = tiledb.Group(self.index_uri, "r")
             self.vector_index_uri = (
                 vector_index_uri
                 if vector_index_uri != ""
                 else get_vector_index_uri_from_group(index_group)
             )
@@ -168,15 +169,15 @@
             k: Number of Documents to return. Defaults to 4.
             filter (Optional[Dict[str, Any]]): Filter by metadata. Defaults to None.
             score_threshold: Optional, a floating point value to filter the
                 resulting set of retrieved docs
         Returns:
             List of Documents and scores.
         """
-        tiledb = guard_import("tiledb")
+        tiledb_vs, tiledb = dependable_tiledb_import()
         docs = []
         docs_array = tiledb.open(
             self.docs_array_uri, "r", timestamp=self.timestamp, config=self.config
         )
         for idx, score in zip(ids, scores):
             if idx == 0 and score == 0:
                 continue
@@ -472,18 +473,15 @@
         index_type: str,
         dimensions: int,
         vector_type: np.dtype,
         *,
         metadatas: bool = True,
         config: Optional[Mapping[str, Any]] = None,
     ) -> None:
-        tiledb_vs, tiledb = (
-            guard_import("tiledb.vector_search"),
-            guard_import("tiledb"),
-        )
+        tiledb_vs, tiledb = dependable_tiledb_import()
         with tiledb.scope_ctx(ctx_or_config=config):
             try:
                 tiledb.group_create(index_uri)
             except tiledb.TileDBError as err:
                 raise err
             group = tiledb.Group(index_uri, "w")
             vector_index_uri = get_vector_index_uri(group.uri)
@@ -548,18 +546,15 @@
         if metric not in INDEX_METRICS:
             raise ValueError(
                 (
                     f"Unsupported distance metric: {metric}. "
                     f"Expected one of {list(INDEX_METRICS)}"
                 )
             )
-        tiledb_vs, tiledb = (
-            guard_import("tiledb.vector_search"),
-            guard_import("tiledb"),
-        )
+        tiledb_vs, tiledb = dependable_tiledb_import()
         input_vectors = np.array(embeddings).astype(np.float32)
         cls.create(
             index_uri=index_uri,
             index_type=index_type,
             dimensions=input_vectors.shape[1],
             vector_type=input_vectors.dtype,
             metadatas=metadatas is not None,
@@ -647,15 +642,15 @@
             ids: Optional ids of each text object.
             timestamp: Optional timestamp to write new texts with.
             kwargs: vectorstore specific parameters
 
         Returns:
             List of ids from adding the texts into the vectorstore.
         """
-        tiledb = guard_import("tiledb")
+        tiledb_vs, tiledb = dependable_tiledb_import()
         embeddings = self.embedding.embed_documents(list(texts))
         if ids is None:
             ids = [str(random.randint(0, MAX_UINT64 - 1)) for _ in texts]
 
         external_ids = np.array(ids).astype(np.uint64)
         vectors = np.empty((len(embeddings)), dtype="O")
         for i in range(len(embeddings)):
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/timescalevector.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/timescalevector.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/typesense.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/typesense.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/upstash.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/upstash.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/usearch.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/usearch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 from __future__ import annotations
 
 from typing import Any, Dict, Iterable, List, Optional, Tuple
 
 import numpy as np
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
-from langchain_core.utils import guard_import
 from langchain_core.vectorstores import VectorStore
 
 from langchain_community.docstore.base import AddableMixin, Docstore
 from langchain_community.docstore.in_memory import InMemoryDocstore
 
 
 def dependable_usearch_import() -> Any:
     """
     Import usearch if available, otherwise raise error.
     """
-    return guard_import("usearch.index")
+    try:
+        import usearch.index
+    except ImportError:
+        raise ImportError(
+            "Could not import usearch python package. "
+            "Please install it with `pip install usearch` "
+        )
+    return usearch.index
 
 
 class USearch(VectorStore):
     """`USearch` vector store.
 
     To use, you should have the ``usearch`` python package installed.
     """
@@ -160,11 +166,11 @@
         if ids is None:
             ids = np.array([str(id) for id, _ in enumerate(texts)])
         for i, text in enumerate(texts):
             metadata = metadatas[i] if metadatas else {}
             documents.append(Document(page_content=text, metadata=metadata))
 
         docstore = InMemoryDocstore(dict(zip(ids, documents)))
-        usearch = guard_import("usearch.index")
+        usearch = dependable_usearch_import()
         index = usearch.Index(ndim=len(embeddings[0]), metric=metric)
         index.add(np.array(ids), np.array(embeddings))
         return cls(embedding, index, docstore, ids.tolist())
```

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/utils.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/vald.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/vald.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/vdms.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/vdms.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/vearch.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/vearch.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/vectara.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/vectara.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/vespa.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/vespa.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/vikingdb.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/vikingdb.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/vlite.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/vlite.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/weaviate.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/weaviate.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/xata.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/xata.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/yellowbrick.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/yellowbrick.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/zep.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/zep.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/langchain_community/vectorstores/zilliz.py` & `langchain_community-0.2.0rc1/langchain_community/vectorstores/zilliz.py`

 * *Files identical despite different names*

### Comparing `langchain_community-0.2.0/pyproject.toml` & `langchain_community-0.2.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "langchain-community"
-version = "0.2.0"
+version = "0.2.0rc1"
 description = "Community contributed LangChain integrations."
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.2.0"
-langchain = "^0.2.0"
-SQLAlchemy = ">=1.4,<3"
+langchain-core = "^0.1.52"
+langchain = "^0.2.0rc2"
+SQLAlchemy = ">=1.4,<2.0.29"
 requests = "^2"
 PyYAML = ">=5.3"
 numpy = "^1"
 aiohttp = "^3.8.3"
 tenacity = "^8.1.0"
 dataclasses-json = ">= 0.5.7, < 0.7"
 langsmith = "^0.1.0"
@@ -111,15 +111,15 @@
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
 pytest-cov = "^4.1.0"
 pytest-dotenv = "^0.5.2"
-duckdb-engine = "^0.11.0"
+duckdb-engine = "^0.9.2"
 pytest-watcher = "^0.2.6"
 freezegun = "^1.2.2"
 responses = "^0.22.0"
 pytest-asyncio = "^0.20.3"
 lark = "^1.1.5"
 pandas = "^2.0.0"
 pytest-mock  = "^3.10.0"
@@ -170,15 +170,15 @@
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
-mypy = "^1"
+mypy = "^0.991"
 types-pyyaml = "^6.0.12.2"
 types-requests = "^2.28.11.5"
 types-toml = "^0.10.8.1"
 types-pytz = "^2023.3.0.0"
 types-chardet = "^5.0.4.6"
 types-redis = "^4.3.21.6"
 mypy-protobuf = "^3.0.0"
```

### Comparing `langchain_community-0.2.0/PKG-INFO` & `langchain_community-0.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: langchain-community
-Version: 0.2.0
+Version: 0.2.0rc1
 Summary: Community contributed LangChain integrations.
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Provides-Extra: extended-testing
 Requires-Dist: PyYAML (>=5.3)
-Requires-Dist: SQLAlchemy (>=1.4,<3)
+Requires-Dist: SQLAlchemy (>=1.4,<2.0.29)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiosqlite (>=0.19.0,<0.20.0) ; extra == "extended-testing"
 Requires-Dist: aleph-alpha-client (>=2.15.0,<3.0.0) ; extra == "extended-testing"
 Requires-Dist: anthropic (>=0.3.11,<0.4.0) ; extra == "extended-testing"
 Requires-Dist: arxiv (>=1.4,<2.0) ; extra == "extended-testing"
 Requires-Dist: assemblyai (>=0.17.0,<0.18.0) ; extra == "extended-testing"
 Requires-Dist: atlassian-python-api (>=3.36.0,<4.0.0) ; extra == "extended-testing"
@@ -51,16 +51,16 @@
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0) ; extra == "extended-testing"
 Requires-Dist: httpx (>=0.24.1,<0.25.0) ; extra == "extended-testing"
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0) ; extra == "extended-testing"
 Requires-Dist: javelin-sdk (>=0.1.8,<0.2.0) ; extra == "extended-testing"
 Requires-Dist: jinja2 (>=3,<4) ; extra == "extended-testing"
 Requires-Dist: jq (>=1.4.1,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: jsonschema (>1) ; extra == "extended-testing"
-Requires-Dist: langchain (>=0.2.0,<0.3.0)
-Requires-Dist: langchain-core (>=0.2.0,<0.3.0)
+Requires-Dist: langchain (>=0.2.0rc2,<0.3.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.2.0)
 Requires-Dist: langsmith (>=0.1.0,<0.2.0)
 Requires-Dist: lxml (>=4.9.3,<6.0) ; extra == "extended-testing"
 Requires-Dist: markdownify (>=0.11.6,<0.12.0) ; extra == "extended-testing"
 Requires-Dist: motor (>=3.3.1,<4.0.0) ; extra == "extended-testing"
 Requires-Dist: msal (>=1.25.0,<2.0.0) ; extra == "extended-testing"
 Requires-Dist: mwparserfromhell (>=0.6.4,<0.7.0) ; extra == "extended-testing"
 Requires-Dist: mwxml (>=0.3.3,<0.4.0) ; extra == "extended-testing"
```

