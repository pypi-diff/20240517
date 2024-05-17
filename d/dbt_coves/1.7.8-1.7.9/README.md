# Comparing `tmp/dbt_coves-1.7.8.tar.gz` & `tmp/dbt_coves-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.7.8.tar", max compression
+gzip compressed data, was "dbt_coves-1.7.9.tar", max compression
```

## Comparing `dbt_coves-1.7.8.tar` & `dbt_coves-1.7.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0    11357 2024-04-29 21:27:24.353636 dbt_coves-1.7.8/LICENSE
--rw-r--r--   0        0        0    28693 2024-04-29 21:27:24.353636 dbt_coves-1.7.8/README.md
--rw-r--r--   0        0        0       22 2024-04-29 21:27:46.685749 dbt_coves-1.7.8/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.353636 dbt_coves-1.7.8/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0    12670 2024-04-29 21:27:24.353636 dbt_coves-1.7.8/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.353636 dbt_coves-1.7.8/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0     1364 2024-04-29 21:27:24.353636 dbt_coves-1.7.8/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     8982 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     3008 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/data_sync/__init__.py
--rw-r--r--   0        0        0      864 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/data_sync/main.py
--rw-r--r--   0        0        0     3369 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/data_sync/snowflake.py
--rw-r--r--   0        0        0     2833 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/README.md
--rw-r--r--   0        0        0     7165 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/__init__.py
--rw-r--r--   0        0        0     5174 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/helpers.py
--rw-r--r--   0        0        0     2459 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/schema_types.py
--rw-r--r--   0        0        0     5397 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    12275 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4555 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    16975 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_dags.py
--rw-r--r--   0        0        0      226 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_generators/__init__.py
--rw-r--r--   0        0        0     6997 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_generators/airbyte.py
--rw-r--r--   0        0        0     6320 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_generators/base.py
--rw-r--r--   0        0        0     6593 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_generators/fivetran.py
--rw-r--r--   0        0        0    18628 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     5897 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/docs.py
--rw-r--r--   0        0        0     1473 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10624 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8736 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    15161 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2682 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    25832 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0      640 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    18462 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0      494 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/base.py
--rw-r--r--   0        0        0     4287 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6751 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1214 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0     1667 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/pre_commit.py
--rw-r--r--   0        0        0    10262 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      845 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
--rw-r--r--   0        0        0     2110 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
--rw-r--r--   0        0        0       75 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
--rw-r--r--   0        0        0     2743 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
--rw-r--r--   0        0        0      668 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
--rw-r--r--   0        0        0      102 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
--rw-r--r--   0        0        0     1371 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0    11451 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    18547 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1131 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/log.py
--rw-r--r--   0        0        0     1749 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/secrets.py
--rw-r--r--   0        0        0     1342 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     2205 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/tracking.py
--rw-r--r--   0        0        0     1575 2024-04-29 21:27:24.357636 dbt_coves-1.7.8/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3914 2024-04-29 21:27:46.685749 dbt_coves-1.7.8/pyproject.toml
--rw-r--r--   0        0        0    30968 1970-01-01 00:00:00.000000 dbt_coves-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-30 20:16:48.725865 dbt_coves-1.7.9/LICENSE
+-rw-r--r--   0        0        0    28693 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/README.md
+-rw-r--r--   0        0        0       22 2024-04-30 20:17:12.901960 dbt_coves-1.7.9/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0    12670 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0     1364 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     8982 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     3008 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/data_sync/__init__.py
+-rw-r--r--   0        0        0      864 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/data_sync/main.py
+-rw-r--r--   0        0        0     3369 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/data_sync/snowflake.py
+-rw-r--r--   0        0        0     2833 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/README.md
+-rw-r--r--   0        0        0     7165 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/__init__.py
+-rw-r--r--   0        0        0     5174 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/helpers.py
+-rw-r--r--   0        0        0     2459 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/schema_types.py
+-rw-r--r--   0        0        0     5397 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    12275 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4555 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    16975 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_dags.py
+-rw-r--r--   0        0        0      226 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_generators/__init__.py
+-rw-r--r--   0        0        0     6997 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_generators/airbyte.py
+-rw-r--r--   0        0        0     6320 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_generators/base.py
+-rw-r--r--   0        0        0     6593 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_generators/fivetran.py
+-rw-r--r--   0        0        0    18628 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     5897 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/docs.py
+-rw-r--r--   0        0        0     1473 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10624 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8736 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    15161 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2682 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    25832 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0      640 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    18462 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/base.py
+-rw-r--r--   0        0        0     4287 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6751 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1214 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0     1667 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/pre_commit.py
+-rw-r--r--   0        0        0    10262 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      845 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
+-rw-r--r--   0        0        0     2110 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
+-rw-r--r--   0        0        0       75 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
+-rw-r--r--   0        0        0     2743 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
+-rw-r--r--   0        0        0      668 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
+-rw-r--r--   0        0        0      102 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
+-rw-r--r--   0        0        0     1371 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0    11451 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    18547 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1131 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0     1749 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/secrets.py
+-rw-r--r--   0        0        0     1342 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     2205 2024-04-30 20:16:48.729865 dbt_coves-1.7.9/dbt_coves/utils/tracking.py
+-rw-r--r--   0        0        0     1575 2024-04-30 20:16:48.733865 dbt_coves-1.7.9/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3909 2024-04-30 20:17:12.901960 dbt_coves-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0    30959 1970-01-01 00:00:00.000000 dbt_coves-1.7.9/PKG-INFO
```

### Comparing `dbt_coves-1.7.8/LICENSE` & `dbt_coves-1.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/README.md` & `dbt_coves-1.7.9/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/config/config.py` & `dbt_coves-1.7.9/dbt_coves/config/config.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/core/exceptions.py` & `dbt_coves-1.7.9/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/core/main.py` & `dbt_coves-1.7.9/dbt_coves/core/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/base.py` & `dbt_coves-1.7.9/dbt_coves/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/data_sync/main.py` & `dbt_coves-1.7.9/dbt_coves/tasks/data_sync/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/data_sync/snowflake.py` & `dbt_coves-1.7.9/dbt_coves/tasks/data_sync/snowflake.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/README.md` & `dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/README.md`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/__init__.py` & `dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/helpers.py` & `dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/data_sync/sql_database/schema_types.py` & `dbt_coves-1.7.9/dbt_coves/tasks/data_sync/sql_database/schema_types.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.7.9/dbt_coves/tasks/dbt/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.7.9/dbt_coves/tasks/extract/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.7.9/dbt_coves/tasks/extract/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.7.9/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_dags.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_dags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_generators/airbyte.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_generators/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_generators/base.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_generators/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/airflow_generators/fivetran.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/airflow_generators/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/docs.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/docs.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/sources.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.7.9/dbt_coves/tasks/generate/templates.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.7.9/dbt_coves/tasks/load/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/load/base.py` & `dbt_coves-1.7.9/dbt_coves/tasks/load/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.7.9/dbt_coves/tasks/load/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/load/main.py` & `dbt_coves-1.7.9/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/git.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/main.py` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/pre_commit.py` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/pre_commit.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/ssh.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/copier.yml` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/copier.yml`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/tasks/setup/utils.py` & `dbt_coves-1.7.9/dbt_coves/tasks/setup/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.7.9/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/ui/traceback.py` & `dbt_coves-1.7.9/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/api_caller.py` & `dbt_coves-1.7.9/dbt_coves/utils/api_caller.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/flags.py` & `dbt_coves-1.7.9/dbt_coves/utils/flags.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/jinja.py` & `dbt_coves-1.7.9/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/log.py` & `dbt_coves-1.7.9/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/secrets.py` & `dbt_coves-1.7.9/dbt_coves/utils/secrets.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/shell.py` & `dbt_coves-1.7.9/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/tracking.py` & `dbt_coves-1.7.9/dbt_coves/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/dbt_coves/utils/yaml.py` & `dbt_coves-1.7.9/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.7.8/pyproject.toml` & `dbt_coves-1.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.7.8"
+version = "1.7.9"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Information Technology",
@@ -41,15 +41,15 @@
 bumpversion = "^0.6.0"
 typing_extensions = { version = "^4.0", python = "^3.7" }
 ruamel-yaml = "^0.17.21"
 db-dtypes = "^1.0.5"
 copier = "6.0.0"
 gitpython = "^3.1.31"
 mixpanel = "^4.10.0"
-black = "^23.11.0"
+black = "^23"
 isort = "^5.12.0"
 dlt = {extras = ["postgres"], version = "^0.4.8"}
 psycopg2-binary = "^2.9.9"
 sqlalchemy = "^1.4"
 pyyaml-include = "<2.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `dbt_coves-1.7.8/PKG-INFO` & `dbt_coves-1.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt_coves
-Version: 1.7.8
+Version: 1.7.9
 Summary: CLI tool for dbt users adopting analytics engineering best practices.
 Home-page: https://datacoves.com
 License: Apache 2.0
 Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
 Author: Datacoves
 Author-email: hello@datacoves.com
 Requires-Python: >=3.8.1,<3.12
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Requires-Dist: Jinja2 (>2.11.2)
 Requires-Dist: PyYAML (>=5.4.1)
-Requires-Dist: black (>=23.11.0,<24.0.0)
+Requires-Dist: black (>=23,<24)
 Requires-Dist: bumpversion (>=0.6.0,<0.7.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
 Requires-Dist: copier (==6.0.0)
 Requires-Dist: db-dtypes (>=1.0.5,<2.0.0)
 Requires-Dist: dbt-core (>=1.1,<1.8)
 Requires-Dist: dlt[postgres] (>=0.4.8,<0.5.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
```

