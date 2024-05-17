# Comparing `tmp/predibase-2024.4.8.tar.gz` & `tmp/predibase-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predibase-2024.4.8.tar", last modified: Sat Apr 20 01:07:52 2024, max compression
+gzip compressed data, was "predibase-2024.5.1.tar", last modified: Fri May 17 00:14:21 2024, max compression
```

## Comparing `predibase-2024.4.8.tar` & `predibase-2024.5.1.tar`

### file list

```diff
@@ -1,99 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.652035 predibase-2024.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-20 01:06:03.000000 predibase-2024.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-20 01:07:52.648035 predibase-2024.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-20 01:06:03.000000 predibase-2024.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.628035 predibase-2024.4.8/predibase/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.632035 predibase-2024.4.8/predibase/cli_commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/finetune.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/list_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/cli_commands/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/connection_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/dataset_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/deployment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/engine_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/llm_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/model_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/permission_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.632035 predibase-2024.4.8/predibase/pql/
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/pql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/pql/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    34402 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/pql/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/pql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/query_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.640035 predibase-2024.4.8/predibase/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/connection_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/connection_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.640035 predibase-2024.4.8/predibase/resource/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28866 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.644035 predibase-2024.4.8/predibase/resource/llm/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/templates/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/templates/lora_bf16.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/templates/qlora_4bit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/llm/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    50487 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource/viz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resource_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.644035 predibase-2024.4.8/predibase/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11448 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/completions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/resources/repos.py
--rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/triton_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.648035 predibase-2024.4.8/predibase/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/util/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/util/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/util/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/util/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/util/url.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.628035 predibase-2024.4.8/predibase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-20 01:07:52.000000 predibase-2024.4.8/predibase.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.648035 predibase-2024.4.8/predibase_notebook/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase_notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase_notebook/env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:07:52.648035 predibase-2024.4.8/predibase_notebook/nbextension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:03.000000 predibase-2024.4.8/predibase_notebook/nbextension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-20 01:07:52.000000 predibase-2024.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:07:52.652035 predibase-2024.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-20 01:06:03.000000 predibase-2024.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.093695 predibase-2024.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-17 00:11:53.000000 predibase-2024.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-17 00:14:21.093695 predibase-2024.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-17 00:11:53.000000 predibase-2024.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.065694 predibase-2024.5.1/predibase/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.069695 predibase-2024.5.1/predibase/cli_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/finetune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/list_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/cli_commands/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/connection_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/dataset_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7375 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/deployment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/engine_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/llm_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/permission_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.073695 predibase-2024.5.1/predibase/pql/
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/pql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/pql/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34715 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/pql/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/pql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9419 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/query_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.077695 predibase-2024.5.1/predibase/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/connection_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/connection_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7729 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.081694 predibase-2024.5.1/predibase/resource/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28864 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3777 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.081694 predibase-2024.5.1/predibase/resource/llm/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/templates/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/templates/lora_bf16.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/templates/qlora_4bit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/llm/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50487 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource/viz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resource_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.089694 predibase-2024.5.1/predibase/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/finetuning_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/finetuning_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/repos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/resources/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/triton_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.089694 predibase-2024.5.1/predibase/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/util/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/util/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/util/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/util/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-17 00:14:20.000000 predibase-2024.5.1/predibase/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.065694 predibase-2024.5.1/predibase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-17 00:14:21.000000 predibase-2024.5.1/predibase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-17 00:14:21.000000 predibase-2024.5.1/predibase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:14:21.000000 predibase-2024.5.1/predibase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-17 00:14:21.000000 predibase-2024.5.1/predibase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 00:14:21.000000 predibase-2024.5.1/predibase.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-17 00:14:21.000000 predibase-2024.5.1/predibase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-17 00:14:21.000000 predibase-2024.5.1/predibase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.093695 predibase-2024.5.1/predibase_notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase_notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase_notebook/env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 00:14:21.093695 predibase-2024.5.1/predibase_notebook/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 00:11:53.000000 predibase-2024.5.1/predibase_notebook/nbextension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-17 00:14:20.000000 predibase-2024.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 00:14:21.093695 predibase-2024.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-17 00:11:53.000000 predibase-2024.5.1/setup.py
```

### Comparing `predibase-2024.4.8/predibase/__init__.py` & `predibase-2024.5.1/predibase/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+import logging
 import os
 
 from ._client import Predibase
 from .client import PredibaseClient
+from .config import FinetuningConfig, DeploymentConfig
 from .predictor import AsyncPredictor, Predictor
-from .version import __version__  # noqa: F401
 from .resource.llm.prompt import PromptTemplate
-
-import logging
+from .version import __version__  # noqa: F401
 
 logger = logging.getLogger(__name__)
 
-__all__ = ["Predibase", "PredibaseClient", "AsyncPredictor", "Predictor", "PromptTemplate"]
+__all__ = [
+    "Predibase",
+    "PredibaseClient",
+    "AsyncPredictor",
+    "Predictor",
+    "PromptTemplate",
+    "FinetuningConfig",
+    "DeploymentConfig",
+]
 
 
 def _configure_logging():
     log_level = os.getenv("PREDIBASE_LOG_LEVEL", "").lower()
     requests_logger = logging.getLogger("requests")
     urllib3_logger = logging.getLogger("urllib3")
```

### Comparing `predibase-2024.4.8/predibase/_errors.py` & `predibase-2024.5.1/predibase/_errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 import logging
-import os 
+import os
 from warnings import warn
 
 import semantic_version
 from decorator import decorator
 
 from predibase.version import __version__
 
-
 logger = logging.getLogger(__name__)
 
 
 class PredibaseError(Exception):
     def __init__(self, message: str):
         super().__init__(message)
         self.message = message
 
 
 class PredibaseResponseError(PredibaseError):
     def __init__(self, message: str, code: int):
         super().__init__(message)
         self.code = code
 
+
+class PredibaseServerError(PredibaseError):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
+class FinetuningError(PredibaseError):
+    def __init__(self, message: str):
+        super().__init__(message)
+
+
 is_ci = bool(os.getenv("PREDIBASE_CI", ""))
 
+
 @decorator
 def warn_outdated_sdk(fn, *args, **kwargs):
     resp = fn(*args, **kwargs)
     server_release_version = resp.headers.get("X-Predibase-Release-Version", None)
     if server_release_version is not None and not is_ci:
         if server_release_version == "" or server_release_version == "staging":
             if not __version__.startswith("0.1.1+dev") and not __version__.startswith("v2999"):
```

### Comparing `predibase-2024.4.8/predibase/cli.py` & `predibase-2024.5.1/predibase/cli.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/create.py` & `predibase-2024.5.1/predibase/cli_commands/create.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/delete.py` & `predibase-2024.5.1/predibase/cli_commands/delete.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/deploy.py` & `predibase-2024.5.1/predibase/cli_commands/deploy.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/download.py` & `predibase-2024.5.1/predibase/cli_commands/download.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/finetune.py` & `predibase-2024.5.1/predibase/cli_commands/finetune.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/list_resources.py` & `predibase-2024.5.1/predibase/cli_commands/list_resources.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/prompt.py` & `predibase-2024.5.1/predibase/cli_commands/prompt.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/settings.py` & `predibase-2024.5.1/predibase/cli_commands/settings.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/upload.py` & `predibase-2024.5.1/predibase/cli_commands/upload.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/cli_commands/utils.py` & `predibase-2024.5.1/predibase/cli_commands/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from rich.table import Table
 
 from predibase import PredibaseClient
 from predibase.pql.api import Session
 from predibase.resource.dataset import Dataset
 from predibase.resource.engine import Engine
 from predibase.resource.model import ModelRepo
-from predibase.util import DEFAULT_API_ENDPOINT, DEFAULT_SERVING_ENDPOINT
+from predibase.util import DEFAULT_API_ENDPOINT, get_serving_endpoint
 
 
 @dataclass
 class Defaults:
     repo: Optional[str] = None
     engine: Optional[str] = None
     session: Optional[Session] = None
@@ -69,16 +69,16 @@
     return get_client().get_dataset(dataset_name=dataset_name, connection_name=conn_name)
 
 
 def set_defaults_from_settings(settings: Dict[str, Any]):
     url = settings.get("endpoint")
     if url is None:
         url = os.environ.get("PREDIBASE_GATEWAY", DEFAULT_API_ENDPOINT)
-    
-    serving_endpoint = os.environ.get("PREDIBASE_SERVING_ENDPOINT", DEFAULT_SERVING_ENDPOINT)
+
+    serving_endpoint = get_serving_endpoint(url)
 
     global defaults
     defaults = Defaults(
         repo=settings.get("repo"),
         engine=settings.get("engine"),
         session=Session(token=settings.get("token"), url=url, serving_http_endpoint=serving_endpoint),
     )
```

### Comparing `predibase-2024.4.8/predibase/client.py` & `predibase-2024.5.1/predibase/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
             except NameError:
                 # We're not in a notebook; use standard tracebacklimit instead.
                 # IMPORTANT: setting this to a value <= 1 breaks colab horribly and has no effect in Jupyter.
                 sys.tracebacklimit = 0
 
             # https://stackoverflow.com/a/61077368
             if ipython:
+
                 def hide_traceback(
-                    exc_tuple=None, filename=None, tb_offset=None,
-                    exception_only=False, running_compiled_code=False
+                    exc_tuple=None, filename=None, tb_offset=None, exception_only=False, running_compiled_code=False
                 ):
                     etype, value, tb = sys.exc_info()
                     return ipython._showtraceback(etype, value, ipython.InteractiveTB.get_exception_only(etype, value))
 
                 ipython.showtraceback = hide_traceback
 
     @property
```

### Comparing `predibase-2024.4.8/predibase/connection.py` & `predibase-2024.5.1/predibase/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/connection_mixin.py` & `predibase-2024.5.1/predibase/connection_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/dataset_mixin.py` & `predibase-2024.5.1/predibase/dataset_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/deployment_mixin.py` & `predibase-2024.5.1/predibase/deployment_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/engine_mixin.py` & `predibase-2024.5.1/predibase/engine_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/llm_mixin.py` & `predibase-2024.5.1/predibase/llm_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/model_mixin.py` & `predibase-2024.5.1/predibase/model_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/permission_mixin.py` & `predibase-2024.5.1/predibase/permission_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/pql/__init__.py` & `predibase-2024.5.1/predibase/pql/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 from typing import Any, Dict, Optional
 
 import pandas as pd
 
 from predibase.pql.api import Session
 from predibase.pql.utils import remove_trailing_slash
-from predibase.util import DEFAULT_API_ENDPOINT, DEFAULT_SERVING_ENDPOINT, log_info
+from predibase.util import DEFAULT_API_ENDPOINT, get_serving_endpoint, log_info
 from predibase.util.settings import load_settings
 
 _session = Session()
 logger = logging.getLogger(__name__)
 
 
 def start_session(gateway: str = None, token: str = None, serving_endpoint: str = None) -> Session:
@@ -28,15 +28,16 @@
 
         if user is not None:
             log_info(f"Connected to Predibase as {user}")
 
     except Exception as e:
         raise ValueError(f"Unable to connect to Predibase: {e}")
 
-    return session
+    _session = session
+    return _session
 
 
 def connect_session(
     session: Session,
     url: Optional[str] = None,
     serving_endpoint: Optional[str] = None,
     token: Optional[str] = None,
@@ -46,15 +47,15 @@
     token = token or settings.get("token")
     url = url or settings.get("endpoint")
 
     if url is None:
         url = os.environ.get("PREDIBASE_GATEWAY", DEFAULT_API_ENDPOINT)
 
     if serving_endpoint is None:
-        serving_endpoint = os.environ.get("PREDIBASE_SERVING_ENDPOINT", DEFAULT_SERVING_ENDPOINT)
+        serving_endpoint = get_serving_endpoint(url)
 
     url = remove_trailing_slash(url)
     serving_endpoint = remove_trailing_slash(serving_endpoint)
 
     if token is None:
         token = os.environ.get("PREDIBASE_API_TOKEN")
         if token is None:
```

### Comparing `predibase-2024.4.8/predibase/pql/adapter.py` & `predibase-2024.5.1/predibase/pql/adapter.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/pql/api.py` & `predibase-2024.5.1/predibase/pql/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     metricsRegex,
     model_logs_directory,
 )
 from predibase.version import __version__
 
 is_ci = bool(os.getenv("PREDIBASE_CI", ""))
 
+
 @decorator
 def warn_outdated_sdk(fn, *args, **kwargs):
     resp = fn(*args, **kwargs)
     server_release_version = resp.headers.get("X-Predibase-Release-Version", None)
     if server_release_version is not None and not is_ci:
         if server_release_version == "" or server_release_version == "staging":
             if not __version__.startswith("0.1.1+dev") and not __version__.startswith("2999"):
@@ -86,14 +87,17 @@
     verbose: bool = False
     url: str = None
     serving_grpc_endpoint: str = None
     serving_http_endpoint: str = None
     tenant: str = "default"
     token: str = None
     timeout_in_seconds: int = 600  # 10 min timeout to allow for long requests to /generate endpoints
+    # Use separate requests object for HTTP vs Websocket requests
+    requests_session = requests.Session()
+    websockets_session = requests.Session()
 
     def __post_init__(self):
         self._token_user_cache: Optional[Tuple[str, User]] = None
 
     def execute(
         self,
         statement: str,
@@ -396,14 +400,15 @@
             )
             if resp["modelVersion"]["status"] in {"failed"}
             else None
         )
 
         last_status = None
 
+        pbar = None
         pbars = []
         training_pbar = None
         metrics_thread = None
         tensorboard_thread = None
         tensorboard_event = Event()
 
         def update_last_pbar(last_status: str, timeline_resp: Dict[str, Any]):
@@ -613,15 +618,15 @@
         # see: https://findwork.dev/blog/advanced-usage-python-requests-timeouts-retries-hooks/
         retry_strategy = Retry(
             total=4,
             backoff_factor=2,
             status_forcelist=[104, 429, 500, 502, 503, 504],  # Exclude bad request
             allowed_methods=["HEAD", "GET", "PUT", "PATCH", "POST", "OPTIONS"],
         )
-        http = requests.Session()
+        http = self.requests_session if self.requests_session else requests.Session()
         adapter = TimeoutHTTPAdapter(
             max_retries=retry_strategy,
             timeout=self.timeout_in_seconds,
         )
         http.mount("https://", adapter)
         http.mount("http://", adapter)
         return http
@@ -668,15 +673,16 @@
             params=params,
             timeout=(self.timeout_in_seconds, self.timeout_in_seconds),
         )
 
     @warn_outdated_sdk
     def _get_ws(self, endpoint: str):
         ws_url = self.url.replace("https://", "wss://").replace("http://", "ws://")
-        return requests.Session().get(ws_url + endpoint, headers=self.get_headers(), timeout=None, stream=True)
+        ws_session = self.websockets_session if self.websockets_session else requests.Session()
+        return ws_session.get(ws_url + endpoint, headers=self.get_headers(), timeout=None, stream=True)
 
     @warn_outdated_sdk
     def _delete(self, endpoint: str):
         return self._http().delete(
             self.url + endpoint,
             headers=self.get_headers(),
             timeout=(self.timeout_in_seconds, self.timeout_in_seconds),
```

### Comparing `predibase-2024.4.8/predibase/pql/utils.py` & `predibase-2024.5.1/predibase/pql/utils.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/predictor.py` & `predibase-2024.5.1/predibase/predictor.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/query_mixin.py` & `predibase-2024.5.1/predibase/query_mixin.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/config.py` & `predibase-2024.5.1/predibase/resource/config.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/connection.py` & `predibase-2024.5.1/predibase/resource/connection.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/connection_object.py` & `predibase-2024.5.1/predibase/resource/connection_object.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/connection_properties.py` & `predibase-2024.5.1/predibase/resource/connection_properties.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/dataset.py` & `predibase-2024.5.1/predibase/resource/dataset.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/dataset_info.py` & `predibase-2024.5.1/predibase/resource/dataset_info.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/deployment.py` & `predibase-2024.5.1/predibase/resource/deployment.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/engine.py` & `predibase-2024.5.1/predibase/resource/engine.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/llm/interface.py` & `predibase-2024.5.1/predibase/resource/llm/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,17 +272,17 @@
 
     def _override_adapter_options(self, options: Dict[str, Union[str, float]]) -> Dict[str, Union[str, float]]:
         if self._adapter:
             if isinstance(self._adapter, HuggingFaceLLM):
                 options["adapter_id"] = self._adapter.model_name
                 options["adapter_source"] = "hub"
             else:
-                options["adapter_id"] = (
-                    f"{self._adapter.uuid}/{self._adapter.best_run_id}/artifacts/model/model_weights/"
-                )
+                options[
+                    "adapter_id"
+                ] = f"{self._adapter.uuid}/{self._adapter.best_run_id}/artifacts/model/model_weights/"
                 options["adapter_source"] = "s3"
         return options
 
     def generate_stream(
         self,
         prompt: str,
         options: Optional[Dict[str, Union[str, float]]] = None,
```

### Comparing `predibase-2024.4.8/predibase/resource/llm/response.py` & `predibase-2024.5.1/predibase/resource/llm/response.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/llm/template.py` & `predibase-2024.5.1/predibase/resource/llm/template.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/llm/templates/lora_bf16.yaml` & `predibase-2024.5.1/predibase/resource/llm/templates/lora_bf16.yaml`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/llm/templates/qlora_4bit.yaml` & `predibase-2024.5.1/predibase/resource/llm/templates/qlora_4bit.yaml`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/llm/util.py` & `predibase-2024.5.1/predibase/resource/llm/util.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/model.py` & `predibase-2024.5.1/predibase/resource/model.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/query.py` & `predibase-2024.5.1/predibase/resource/query.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource/user.py` & `predibase-2024.5.1/predibase/resource/user.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resource_util.py` & `predibase-2024.5.1/predibase/resource_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/resources/datasets.py` & `predibase-2024.5.1/predibase/resources/datasets.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 from __future__ import annotations
 
 import mimetypes
 import os
+import pathlib
 from os import PathLike
 from typing import TYPE_CHECKING
 
 import requests
 from google.protobuf.json_format import MessageToJson
 from predibase_api.artifacts.v1.artifacts_pb2 import (
+    RegisterUploadedFileAsDatasetRequest,
     PresignedUrlForUploadRequest,
     ARTIFACT_TYPE_DATASET,
     PresignedUrlForUploadResponse,
-    RegisterUploadedFileAsDatasetRequest,
 )
 
-from predibase._errors import PredibaseError
-from predibase.resource.connection import get_dataset
-from predibase.resource.dataset import Dataset
+from predibase.resources.dataset import Dataset
+from predibase.resources.util import parse_connection_and_dataset_name
+
+# from predibase.resource.dataset import Dataset
 
 if TYPE_CHECKING:
-    from predibase.pql import Session
+    from predibase import Predibase
 
 
 class Datasets:
-    def __init__(self, session: Session):
-        self._session = session
+    def __init__(self, client: Predibase):
+        self._client = client
+        self._session = client._session
+
+    def get(self, dataset_ref: str | Dataset) -> Dataset:
+        if isinstance(dataset_ref, Dataset):
+            dataset_ref = f"{dataset_ref.connection_name}/{dataset_ref.name}"
 
-    def get(self, resource_id: str) -> Dataset:
-        if resource_id.startswith("pb://datasets/"):
-            resource_id = resource_id[len("pb://datasets/"):]
-
-        tokens = resource_id.split("/")
-        if len(tokens) == 1:
-            connection_name = None
-            dataset_name = tokens[0]
-        elif len(tokens) == 2:
-            connection_name, dataset_name = tokens
-        else:
-            raise PredibaseError(f"unable to parse resource ID {resource_id}")
+        connection, name = parse_connection_and_dataset_name(dataset_ref)
 
-        return get_dataset(self._session, connection_name=connection_name, dataset_name=dataset_name)
+        dataset_resp = self._client.http_get(f"/v1/datasets/name/{name}?connectionName={connection}")
+        return Dataset.model_validate(dataset_resp)
 
     def from_file(self, file_path: PathLike, *, name: str | None = None) -> Dataset:
+        if name is None:
+            name = pathlib.Path(file_path).stem
+
         with open(file_path, "rb") as f:
             file_name = os.path.basename(file_path)
             mime_type = mimetypes.guess_type(file_path)[0] or "text/plain"
 
             # Get presigned url for upload
             presigned_url_req = MessageToJson(
                 PresignedUrlForUploadRequest(
@@ -83,13 +83,10 @@
                     file_name=file_name,
                 ),
                 preserving_proto_field_name=True,
             )
             resp = self._session.post("/datasets/register_uploaded_file", data=register_dataset_req)
 
             dataset_id = resp["id"]
-            endpoint = f"/datasets/{dataset_id}"
+            endpoint = f"/datasets/{dataset_id}?withInfo=true"
             resp = self._session.wait_for_dataset(endpoint, until_fully_connected=True)
-
-            from predibase.resource_util import build_dataset
-
-            return build_dataset(resp, self._session)
+            return Dataset.model_validate(resp)
```

### Comparing `predibase-2024.4.8/predibase/triton_util.py` & `predibase-2024.5.1/predibase/triton_util.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/util/__init__.py` & `predibase-2024.5.1/predibase/util/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from decimal import Decimal
 
 import yaml
 from rich.console import Console
 from requests import Response
 
 DEFAULT_API_ENDPOINT = "https://api.app.predibase.com/v1"
-DEFAULT_SERVING_ENDPOINT = "serving.app.predibase.com"
 
 DEBUG = os.environ.get("PREDIBASE_DEBUG") is not None
 
 
 _console = Console()
 _error_console = Console(stderr=True, style="bold red")
 _info_console = Console(stderr=True, style="bold blue")
@@ -71,14 +70,24 @@
             url = url.replace("api.", "").replace("/v1", "")
         root_url = url
     from urllib.parse import urljoin
 
     return urljoin(root_url, endpoint)
 
 
+def get_serving_endpoint(gateway_endpoint: str) -> str:
+    # Repliace scheme and the rest of the endpoint
+    serving_endpoint = gateway_endpoint.replace("https://", "").replace("http://", "").replace("/v1", "")
+    # Replace the first part ("api") with "serving"
+    serving_endpoint_parts = serving_endpoint.split(".")
+    serving_endpoint_parts[0] = "serving"
+    serving_endpoint = ".".join(serving_endpoint_parts)
+    return serving_endpoint
+
+
 class JSONFloat(float):
     def __repr__(self):
         return format(Decimal(self), "f")
 
 
 class ConfigEncoder:
     def decimalize(self, val):
```

### Comparing `predibase-2024.4.8/predibase/util/metrics.py` & `predibase-2024.5.1/predibase/util/metrics.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/util/settings.py` & `predibase-2024.5.1/predibase/util/settings.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase/util/tensorboard.py` & `predibase-2024.5.1/predibase/util/tensorboard.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase.egg-info/SOURCES.txt` & `predibase-2024.5.1/predibase.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 requirements.txt
 setup.py
 predibase/__init__.py
 predibase/_client.py
 predibase/_errors.py
 predibase/cli.py
 predibase/client.py
+predibase/config.py
 predibase/connection.py
 predibase/connection_mixin.py
 predibase/dataset_mixin.py
 predibase/deployment_mixin.py
 predibase/engine_mixin.py
 predibase/llm_mixin.py
 predibase/model_mixin.py
@@ -61,22 +62,25 @@
 predibase/resource/llm/response.py
 predibase/resource/llm/template.py
 predibase/resource/llm/util.py
 predibase/resource/llm/templates/config.yaml
 predibase/resource/llm/templates/lora_bf16.yaml
 predibase/resource/llm/templates/qlora_4bit.yaml
 predibase/resources/__init__.py
+predibase/resources/adapter.py
 predibase/resources/adapters.py
-predibase/resources/completions.py
+predibase/resources/dataset.py
 predibase/resources/datasets.py
 predibase/resources/deployment.py
 predibase/resources/deployments.py
-predibase/resources/model.py
-predibase/resources/models.py
+predibase/resources/finetuning_job.py
+predibase/resources/finetuning_jobs.py
+predibase/resources/repo.py
 predibase/resources/repos.py
+predibase/resources/util.py
 predibase/util/__init__.py
 predibase/util/json.py
 predibase/util/metrics.py
 predibase/util/settings.py
 predibase/util/tensorboard.py
 predibase/util/url.py
 predibase/util/util.py
```

### Comparing `predibase-2024.4.8/predibase_notebook/__init__.py` & `predibase-2024.5.1/predibase_notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/predibase_notebook/env.py` & `predibase-2024.5.1/predibase_notebook/env.py`

 * *Files identical despite different names*

### Comparing `predibase-2024.4.8/setup.py` & `predibase-2024.5.1/setup.py`

 * *Files identical despite different names*

