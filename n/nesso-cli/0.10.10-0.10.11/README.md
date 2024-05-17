# Comparing `tmp/nesso_cli-0.10.10.tar.gz` & `tmp/nesso_cli-0.10.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nesso_cli-0.10.10.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nesso_cli-0.10.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nesso_cli-0.10.10.tar` & `nesso_cli-0.10.11.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1742 2024-05-08 14:05:33.612801 nesso_cli-0.10.10/README.md
--rw-r--r--   0        0        0     2721 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/pyproject.toml
--rw-r--r--   0        0        0      548 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/jobs/.gitkeep
--rw-r--r--   0        0        0       34 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/jobs/main.py
--rw-r--r--   0        0        0        0 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/__init__.py
--rw-r--r--   0        0        0      114 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/__init__.py
--rw-r--r--   0        0        0     1214 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/LICENSE.md
--rw-r--r--   0        0        0      786 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/__init__.py
--rw-r--r--   0        0        0     9078 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/templater.py
--rw-r--r--   0        0        0   230402 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/project.py
--rw-r--r--   0        0        0     4580 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/sqlfluff_util.py
--rw-r--r--   0        0        0       29 2024-05-08 14:05:33.620801 nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/state.py
--rw-r--r--   0        0        0    10770 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/base_model.py
--rw-r--r--   0        0        0    16174 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/common.py
--rw-r--r--   0        0        0     1352 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/config.py
--rw-r--r--   0        0        0      403 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/context.py
--rw-r--r--   0        0        0    20703 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/init.py
--rw-r--r--   0        0        0     3804 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/main.py
--rw-r--r--   0        0        0      607 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/metadata.py
--rw-r--r--   0        0        0     3838 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/model.py
--rw-r--r--   0        0        0    33788 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/models.py
--rw-r--r--   0        0        0       56 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/dbt_project.yml
--rw-r--r--   0        0        0     9825 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/codegen_helpers.sql
--rw-r--r--   0        0        0      641 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/create_description_markdown.sql
--rw-r--r--   0        0        0    14152 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/dbt_profiler.sql
--rw-r--r--   0        0        0     1506 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_base_model.sql
--rw-r--r--   0        0        0    14728 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_model_yaml_boilerplate.sql
--rw-r--r--   0        0        0     2420 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_seed_yaml_boilerplate.sql
--rw-r--r--   0        0        0     5514 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_source_yaml_boilerplate.sql
--rw-r--r--   0        0        0      445 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/get_custom_schema.sql
--rw-r--r--   0        0        0      551 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/get_source_pii_columns.sql
--rw-r--r--   0        0        0      677 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/get_table_columns.sql
--rw-r--r--   0        0        0      559 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/hash_column.sql
--rw-r--r--   0        0        0      481 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/hash_source_pii_columns.sql
--rw-r--r--   0        0        0     1101 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/redshift_external_tables_fix.sql
--rw-r--r--   0        0        0     7862 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/seed.py
--rw-r--r--   0        0        0    15312 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/source.py
--rw-r--r--   0        0        0     2111 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/.gitignore
--rw-r--r--   0        0        0      809 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/.vscode/extensions.list
--rw-r--r--   0        0        0       57 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/.vscode/install_extensions.sh
--rw-r--r--   0        0        0      774 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/.vscode/settings.json
--rw-r--r--   0        0        0      136 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/CONTRIBUTING.md
--rw-r--r--   0        0        0     1249 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/README.md
--rw-r--r--   0        0        0      362 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/config.yml
--rw-r--r--   0        0        0     1465 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/dbt_project.yml
--rw-r--r--   0        0        0      585 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/packages.yml
--rw-r--r--   0        0        0     1505 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/prepare.sh
--rw-r--r--   0        0        0      126 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/requirements.txt
--rw-r--r--   0        0        0      148 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/templates/{{ bronze_schema }}.yml
--rw-r--r--   0        0        0       23 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/.env.example
--rw-r--r--   0        0        0      321 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/compose.yml
--rw-r--r--   0        0        0    17585 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/conftest.py
--rw-r--r--   0        0        0      265 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/.nesso/config.yml
--rw-r--r--   0        0        0      772 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/dbt_project.yml
--rw-r--r--   0        0        0      205 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/packages.yml
--rw-r--r--   0        0        0      412 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/profiles.yml
--rw-r--r--   0        0        0    14415 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/seeds/average salary test.xlsx
--rw-r--r--   0        0        0      130 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/seeds/countries_example.csv
--rw-r--r--   0        0        0      784 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/trino/dbt_project.yml
--rw-r--r--   0        0        0      170 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/trino/packages.yml
--rw-r--r--   0        0        0      251 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/trino/profiles.yml
--rw-r--r--   0        0        0     6796 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/functional/test_da_workflow.py
--rw-r--r--   0        0        0      162 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/pytest.ini
--rw-r--r--   0        0        0    15884 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_base_model.py
--rw-r--r--   0        0        0     7194 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_common.py
--rw-r--r--   0        0        0     2029 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_dbt_macros.py
--rw-r--r--   0        0        0    12980 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_init.py
--rw-r--r--   0        0        0      923 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_main.py
--rw-r--r--   0        0        0      234 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_metadata.py
--rw-r--r--   0        0        0     4210 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_model.py
--rw-r--r--   0        0        0     7862 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_models.py
--rw-r--r--   0        0        0     8828 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_seed.py
--rw-r--r--   0        0        0    15331 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_source.py
--rw-r--r--   0        0        0    16207 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_update.py
--rw-r--r--   0        0        0     1042 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/test_yaml_generators.py
--rw-r--r--   0        0        0    11267 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/tests/validate_tables.py
--rw-r--r--   0        0        0     3470 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/update.py
--rw-r--r--   0        0        0     1664 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/models/yaml_generators.py
--rw-r--r--   0        0        0      880 2024-05-08 14:05:33.624801 nesso_cli-0.10.10/src/nesso_cli/nesso_cli.py
--rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 nesso_cli-0.10.10/PKG-INFO
+-rw-r--r--   0        0        0     1742 2024-05-17 08:20:29.414827 nesso_cli-0.10.11/README.md
+-rw-r--r--   0        0        0     2721 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/pyproject.toml
+-rw-r--r--   0        0        0      548 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/jobs/.gitkeep
+-rw-r--r--   0        0        0       34 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/jobs/main.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/__init__.py
+-rw-r--r--   0        0        0      114 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/__init__.py
+-rw-r--r--   0        0        0     1214 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/LICENSE.md
+-rw-r--r--   0        0        0      786 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/__init__.py
+-rw-r--r--   0        0        0     9078 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/templater.py
+-rw-r--r--   0        0        0   230402 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/project.py
+-rw-r--r--   0        0        0     4580 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/sqlfluff_util.py
+-rw-r--r--   0        0        0       29 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/state.py
+-rw-r--r--   0        0        0    10770 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/base_model.py
+-rw-r--r--   0        0        0    16174 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/common.py
+-rw-r--r--   0        0        0     1352 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/config.py
+-rw-r--r--   0        0        0      403 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/context.py
+-rw-r--r--   0        0        0    20703 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/init.py
+-rw-r--r--   0        0        0     3804 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/main.py
+-rw-r--r--   0        0        0      607 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/metadata.py
+-rw-r--r--   0        0        0     3838 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/model.py
+-rw-r--r--   0        0        0    33903 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/models.py
+-rw-r--r--   0        0        0       56 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/dbt_project.yml
+-rw-r--r--   0        0        0     9825 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/codegen_helpers.sql
+-rw-r--r--   0        0        0      641 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/create_description_markdown.sql
+-rw-r--r--   0        0        0    14152 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/dbt_profiler.sql
+-rw-r--r--   0        0        0     1506 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_base_model.sql
+-rw-r--r--   0        0        0    14728 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_model_yaml_boilerplate.sql
+-rw-r--r--   0        0        0     2420 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_seed_yaml_boilerplate.sql
+-rw-r--r--   0        0        0     5514 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_source_yaml_boilerplate.sql
+-rw-r--r--   0        0        0      445 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/get_custom_schema.sql
+-rw-r--r--   0        0        0      551 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/get_source_pii_columns.sql
+-rw-r--r--   0        0        0      677 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/get_table_columns.sql
+-rw-r--r--   0        0        0      559 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/hash_column.sql
+-rw-r--r--   0        0        0      481 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/hash_source_pii_columns.sql
+-rw-r--r--   0        0        0     1101 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/redshift_external_tables_fix.sql
+-rw-r--r--   0        0        0     7862 2024-05-17 08:20:29.422827 nesso_cli-0.10.11/src/nesso_cli/models/seed.py
+-rw-r--r--   0        0        0    15288 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/source.py
+-rw-r--r--   0        0        0     2111 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/.gitignore
+-rw-r--r--   0        0        0      809 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/.vscode/extensions.list
+-rw-r--r--   0        0        0       57 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/.vscode/install_extensions.sh
+-rw-r--r--   0        0        0      774 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/.vscode/settings.json
+-rw-r--r--   0        0        0      136 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1249 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/README.md
+-rw-r--r--   0        0        0      362 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/config.yml
+-rw-r--r--   0        0        0     1465 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/dbt_project.yml
+-rw-r--r--   0        0        0      585 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/packages.yml
+-rw-r--r--   0        0        0     1505 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/prepare.sh
+-rw-r--r--   0        0        0       50 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/requirements.txt
+-rw-r--r--   0        0        0      148 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/templates/{{ bronze_schema }}.yml
+-rw-r--r--   0        0        0       23 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/.env.example
+-rw-r--r--   0        0        0      321 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/compose.yml
+-rw-r--r--   0        0        0    17585 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/conftest.py
+-rw-r--r--   0        0        0      265 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/.nesso/config.yml
+-rw-r--r--   0        0        0      772 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/dbt_project.yml
+-rw-r--r--   0        0        0      205 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/packages.yml
+-rw-r--r--   0        0        0      412 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/profiles.yml
+-rw-r--r--   0        0        0    14415 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/seeds/average salary test.xlsx
+-rw-r--r--   0        0        0      130 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/seeds/countries_example.csv
+-rw-r--r--   0        0        0      784 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/trino/dbt_project.yml
+-rw-r--r--   0        0        0      170 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/trino/packages.yml
+-rw-r--r--   0        0        0      251 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/trino/profiles.yml
+-rw-r--r--   0        0        0     6796 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/functional/test_da_workflow.py
+-rw-r--r--   0        0        0      162 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/pytest.ini
+-rw-r--r--   0        0        0    15884 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_base_model.py
+-rw-r--r--   0        0        0     7194 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_common.py
+-rw-r--r--   0        0        0     2029 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_dbt_macros.py
+-rw-r--r--   0        0        0    12980 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_init.py
+-rw-r--r--   0        0        0      923 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_main.py
+-rw-r--r--   0        0        0      234 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_metadata.py
+-rw-r--r--   0        0        0     4210 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_model.py
+-rw-r--r--   0        0        0     7862 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_models.py
+-rw-r--r--   0        0        0     8828 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_seed.py
+-rw-r--r--   0        0        0    15331 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_source.py
+-rw-r--r--   0        0        0    16207 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_update.py
+-rw-r--r--   0        0        0     1042 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/test_yaml_generators.py
+-rw-r--r--   0        0        0    11267 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/tests/validate_tables.py
+-rw-r--r--   0        0        0     3470 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/update.py
+-rw-r--r--   0        0        0     1664 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/models/yaml_generators.py
+-rw-r--r--   0        0        0      880 2024-05-17 08:20:29.426827 nesso_cli-0.10.11/src/nesso_cli/nesso_cli.py
+-rw-r--r--   0        0        0     4922 1970-01-01 00:00:00.000000 nesso_cli-0.10.11/PKG-INFO
```

### Comparing `nesso_cli-0.10.10/README.md` & `nesso_cli-0.10.11/README.md`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/pyproject.toml` & `nesso_cli-0.10.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "nesso_cli"
 description = "A CLI tool for managing data models."
 readme = "README.md"
-version = "0.10.10"
+version = "0.10.11"
 authors = [{ name = "Michał Zawadzki", email = "mzawadzki@dyvenia.com" }]
 classifiers = []
 keywords = ["cli", "dbt", "dyvenia", "data", "nesso", "models"]
 requires-python = ">=3.10, <3.13"
 dependencies = [
   "loguru == 0.7.2",
   "python-dotenv == 1.0.0",
```

### Comparing `nesso_cli-0.10.10/src/nesso_cli/__init__.py` & `nesso_cli-0.10.11/src/nesso_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/LICENSE.md` & `nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/__init__.py` & `nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/__init__.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/templater.py` & `nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/dbt_templater/templater.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/project.py` & `nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/project.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/_vendored/dbt_core_interface/sqlfluff_util.py` & `nesso_cli-0.10.11/src/nesso_cli/models/_vendored/dbt_core_interface/sqlfluff_util.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/base_model.py` & `nesso_cli-0.10.11/src/nesso_cli/models/base_model.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/common.py` & `nesso_cli-0.10.11/src/nesso_cli/models/common.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/config.py` & `nesso_cli-0.10.11/src/nesso_cli/models/config.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/init.py` & `nesso_cli-0.10.11/src/nesso_cli/models/init.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/main.py` & `nesso_cli-0.10.11/src/nesso_cli/models/main.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/metadata.py` & `nesso_cli-0.10.11/src/nesso_cli/models/metadata.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/model.py` & `nesso_cli-0.10.11/src/nesso_cli/models/model.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/models.py` & `nesso_cli-0.10.11/src/nesso_cli/models/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import copy
 from enum import Enum
 from pathlib import Path
 from typing import Any, Literal, Optional, Tuple, Union
 
-from dbt.contracts.graph.nodes import ColumnInfo
+try:
+    # dbt <= 1.3
+    from dbt.contracts.graph.parsed import ColumnInfo
+except Exception:
+    # dbt > 1.3
+    from dbt.contracts.graph.nodes import ColumnInfo
+
 from pydantic import BaseModel, Field, create_model
 
 from nesso_cli.models.common import (
     DbtProject,
     get_current_dbt_project_obj,
     get_db_table_columns,
     snakecase,
```

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/codegen_helpers.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/codegen_helpers.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/create_description_markdown.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/create_description_markdown.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/dbt_profiler.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/dbt_profiler.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_base_model.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_base_model.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_model_yaml_boilerplate.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_model_yaml_boilerplate.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_seed_yaml_boilerplate.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_seed_yaml_boilerplate.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/generate_source_yaml_boilerplate.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/generate_source_yaml_boilerplate.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/get_source_pii_columns.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/get_source_pii_columns.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/get_table_columns.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/get_table_columns.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/hash_column.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/hash_column.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/nesso_macros/macros/redshift_external_tables_fix.sql` & `nesso_cli-0.10.11/src/nesso_cli/models/nesso_macros/macros/redshift_external_tables_fix.sql`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/seed.py` & `nesso_cli-0.10.11/src/nesso_cli/models/seed.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/source.py` & `nesso_cli-0.10.11/src/nesso_cli/models/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,29 +48,18 @@
 def check_if_source_table_exists(
     source: str, table_name: str, schema_path: Optional[Union[str, Path]] = None
 ) -> bool:
     if schema_path is None:
         schema_path = _get_default_schema_path(source)
 
     if check_if_source_exists(source, schema_path=schema_path):
-        with open(schema_path) as f:
-            schema = yaml.load(f)
-
-            if schema is None:
-                return False
-
-            source_definitions = schema["sources"]
-            source_definition = [
-                sd for sd in source_definitions if sd["name"] == source
-            ][0]
-            source_tables = source_definition.get("tables")
-            if not source_tables:
-                return False
-            else:
-                return any([table["name"] == table_name for table in source_tables])
+        with open(schema_path, "r") as f:
+            for line in f.readlines():
+                if f"- name: {table_name}" in line or f'-name: "{table_name}"' in line:
+                    return True
     return False
 
 
 def _create_table_docs(
     base_dir: Path,
     schema: str,
     table: str,
@@ -368,22 +357,29 @@
     )
     generate_source_text_command = (
         f"""dbt -q run-operation generate_source --args '{args}' --target {env}"""
     )
 
     source_str = call_shell(generate_source_text_command, print_logs=False)
 
+    # Special case when adding the first table.
+    has_tables = False
     with open(schema_path, "r") as file:
-        cfg = yaml.load(file)
+        for line_number, line in enumerate(file):
+            if "tables" in line:
+                has_tables = True
+                break
+            elif line_number > 100:
+                # The "tables" key is at the top of the props file, so need to scan the
+                # entire file (it could have millions of rows).
+                break
+    if not has_tables:
+        source_str = "\n" + indent("tables:", " " * 4) + source_str
 
     with open(schema_path, "a") as file:
-        # Special case when adding the first table.
-        if not cfg["sources"][0].get("tables"):
-            source_str = "\n" + indent("tables:", " " * 4) + source_str
-
         file.write(source_str)
 
     print(f"Source table {fqn_fmt} has been added successfully.")
 
     schema_path_trimmed = schema_path.relative_to(
         schema_path.parent.parent.parent.parent
     )
```

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/templates/.gitignore` & `nesso_cli-0.10.11/src/nesso_cli/models/templates/.gitignore`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/templates/.vscode/extensions.list` & `nesso_cli-0.10.11/src/nesso_cli/models/templates/.vscode/extensions.list`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/templates/.vscode/settings.json` & `nesso_cli-0.10.11/src/nesso_cli/models/templates/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/templates/README.md` & `nesso_cli-0.10.11/src/nesso_cli/models/templates/README.md`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/templates/dbt_project.yml` & `nesso_cli-0.10.11/src/nesso_cli/models/templates/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/templates/packages.yml` & `nesso_cli-0.10.11/src/nesso_cli/models/templates/packages.yml`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/templates/prepare.sh` & `nesso_cli-0.10.11/src/nesso_cli/models/templates/prepare.sh`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/conftest.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/dbt_project.yml` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/postgres/seeds/average salary test.xlsx` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/postgres/seeds/average salary test.xlsx`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/dbt_projects/trino/dbt_project.yml` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/dbt_projects/trino/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/functional/test_da_workflow.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/functional/test_da_workflow.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_base_model.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_common.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_dbt_macros.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_dbt_macros.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_init.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_main.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_model.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_models.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_seed.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_seed.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_source.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_update.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/test_yaml_generators.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/test_yaml_generators.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/tests/validate_tables.py` & `nesso_cli-0.10.11/src/nesso_cli/models/tests/validate_tables.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/update.py` & `nesso_cli-0.10.11/src/nesso_cli/models/update.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/models/yaml_generators.py` & `nesso_cli-0.10.11/src/nesso_cli/models/yaml_generators.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/src/nesso_cli/nesso_cli.py` & `nesso_cli-0.10.11/src/nesso_cli/nesso_cli.py`

 * *Files identical despite different names*

### Comparing `nesso_cli-0.10.10/PKG-INFO` & `nesso_cli-0.10.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nesso_cli
-Version: 0.10.10
+Version: 0.10.11
 Summary: A CLI tool for managing data models.
 Keywords: cli,dbt,dyvenia,data,nesso,models
 Author-email: Michał Zawadzki <mzawadzki@dyvenia.com>
 Requires-Python: >=3.10, <3.13
 Description-Content-Type: text/markdown
 Requires-Dist: loguru == 0.7.2
 Requires-Dist: python-dotenv == 1.0.0
```

