# Comparing `tmp/dbt_oracle-1.7.5.tar.gz` & `tmp/dbt_oracle-1.7.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_oracle-1.7.5.tar", last modified: Fri May 17 03:54:27 2024, max compression
+gzip compressed data, was "dbt_oracle-1.7.5rc1.tar", last modified: Thu Apr 25 22:00:39 2024, max compression
```

## Comparing `dbt_oracle-1.7.5.tar` & `dbt_oracle-1.7.5rc1.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.045492 dbt_oracle-1.7.5/
--rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt_oracle-1.7.5/HISTORY.md
--rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt_oracle-1.7.5/LICENSE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)       47 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/MANIFEST.in
--rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt_oracle-1.7.5/NOTICE.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)     3648 2024-05-17 03:54:27.045144 dbt_oracle-1.7.5/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     2359 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/README.md
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.912619 dbt_oracle-1.7.5/bin/
--rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt_oracle-1.7.5/bin/create-pem-from-p12
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.913743 dbt_oracle-1.7.5/dbt/
--rw-r--r--   0 abhisoms   (501) staff       (20)      712 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.915740 dbt_oracle-1.7.5/dbt/adapters/
--rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt_oracle-1.7.5/dbt/adapters/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.928245 dbt_oracle-1.7.5/dbt/adapters/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      655 2024-05-16 20:38:17.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/__version__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/column.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5156 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/connection_helper.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    12945 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/connections.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    17147 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/impl.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/keyword_catalog.py
--rw-r--r--   0 abhisoms   (501) staff       (20)    10945 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/python_submissions.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6310 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/relation.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.936416 dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1027 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2891 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/base.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     8309 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/materialized_view.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      978 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/policies.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.938827 dbt_oracle-1.7.5/dbt/include/
--rw-r--r--   0 abhisoms   (501) staff       (20)      712 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/include/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.941936 dbt_oracle-1.7.5/dbt/include/oracle/
--rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt_oracle-1.7.5/dbt/include/oracle/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      138 2023-12-05 00:49:54.000000 dbt_oracle-1.7.5/dbt/include/oracle/dbt_project.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.951347 dbt_oracle-1.7.5/dbt/include/oracle/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)    15223 2024-05-16 20:38:17.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/adapters.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/apply_grants.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     6788 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/catalog.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/columns.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1174 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/freshness.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.900001 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.954234 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/incremental/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4376 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     9452 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.955496 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/materialized_view/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4751 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/materialized_view/materialized_view.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.956957 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/python_model/
--rw-r--r--   0 abhisoms   (501) staff       (20)     4345 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/python_model/python.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.958121 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/seed/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2023-12-04 23:12:41.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.961723 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/snapshot/
--rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.963479 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/table/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5489 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/table/table.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.964782 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.965960 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/view/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-06-13 04:33:00.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/view/view.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.967467 dbt_oracle-1.7.5/dbt/include/oracle/macros/relations/
--rw-r--r--   0 abhisoms   (501) staff       (20)      838 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/relations/drop.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/schema_tests.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      757 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/show.sql
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.990377 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/data_types.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1367 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/date_spine.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/dateadd.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/datediff.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/datetrunc.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/except.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      157 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/generate_series.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/hash.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/last_day.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/position.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/right.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/timestamps.sql
--rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt_oracle-1.7.5/dbt/include/oracle/profile_template.yml
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.044109 dbt_oracle-1.7.5/dbt_oracle.egg-info/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3648 2024-05-17 03:54:26.000000 dbt_oracle-1.7.5/dbt_oracle.egg-info/PKG-INFO
--rw-r--r--   0 abhisoms   (501) staff       (20)     4420 2024-05-17 03:54:26.000000 dbt_oracle-1.7.5/dbt_oracle.egg-info/SOURCES.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2024-05-17 03:54:26.000000 dbt_oracle-1.7.5/dbt_oracle.egg-info/dependency_links.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt_oracle-1.7.5/dbt_oracle.egg-info/not-zip-safe
--rw-r--r--   0 abhisoms   (501) staff       (20)       35 2024-05-17 03:54:26.000000 dbt_oracle-1.7.5/dbt_oracle.egg-info/requires.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)        4 2024-05-17 03:54:26.000000 dbt_oracle-1.7.5/dbt_oracle.egg-info/top_level.txt
--rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt_oracle-1.7.5/pyproject.toml
--rw-r--r--   0 abhisoms   (501) staff       (20)     1338 2024-05-17 03:54:27.046666 dbt_oracle-1.7.5/setup.cfg
--rw-r--r--   0 abhisoms   (501) staff       (20)     3026 2024-05-16 20:38:17.000000 dbt_oracle-1.7.5/setup.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.000095 dbt_oracle-1.7.5/tests/
--rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/tests/README.md
--rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt_oracle-1.7.5/tests/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt_oracle-1.7.5/tests/conftest.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:26.902221 dbt_oracle-1.7.5/tests/functional/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.020616 dbt_oracle-1.7.5/tests/functional/adapter/
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.027737 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/__init__.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.031569 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.033018 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/sync_schema/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_unique_id.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.035945 dbt_oracle-1.7.5/tests/functional/adapter/macros/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt_oracle-1.7.5/tests/functional/adapter/macros/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/macros/test_alter_column_type.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.037632 dbt_oracle-1.7.5/tests/functional/adapter/snapshots/
--rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt_oracle-1.7.5/tests/functional/adapter/snapshots/__init__.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt_oracle-1.7.5/tests/functional/adapter/snapshots/test_invalidate_deletes.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_basic.py
--rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_concurrency.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4322 2024-05-16 20:29:49.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_config.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_data_types.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_docs_generate.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_docs_genreferences.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_ephemeral.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_generictests_where.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_grants.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5/tests/functional/adapter/test_quoted_relations.py
-drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-05-17 03:54:27.041381 dbt_oracle-1.7.5/tests/functional/adapter/utils/
--rw-r--r--   0 abhisoms   (501) staff       (20)     5714 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5/tests/functional/adapter/utils/test_common_utils.py
--rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5/tests/functional/adapter/utils/test_dateutils.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.594085 dbt_oracle-1.7.5rc1/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      398 2022-05-04 01:22:16.000000 dbt_oracle-1.7.5rc1/HISTORY.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)    11364 2022-03-16 18:13:02.000000 dbt_oracle-1.7.5rc1/LICENSE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)       47 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/MANIFEST.in
+-rw-r--r--   0 abhisoms   (501) staff       (20)      129 2022-04-26 13:32:00.000000 dbt_oracle-1.7.5rc1/NOTICE.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3651 2024-04-25 22:00:39.593776 dbt_oracle-1.7.5rc1/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2359 2024-03-18 15:24:30.000000 dbt_oracle-1.7.5rc1/README.md
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.486710 dbt_oracle-1.7.5rc1/bin/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2582 2022-07-07 19:56:20.000000 dbt_oracle-1.7.5rc1/bin/create-pem-from-p12
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.487885 dbt_oracle-1.7.5rc1/dbt/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      712 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.489012 dbt_oracle-1.7.5rc1/dbt/adapters/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      701 2022-03-30 23:04:45.000000 dbt_oracle-1.7.5rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.500271 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1040 2022-03-30 23:04:11.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      655 2024-04-25 20:43:40.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/__version__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2237 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/column.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5156 2024-04-19 01:05:08.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/connection_helper.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    12945 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/connections.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    17147 2024-03-18 15:24:30.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/impl.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6054 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/keyword_catalog.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)    10945 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/python_submissions.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6310 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.504310 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1027 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2891 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/base.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     8309 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/materialized_view.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      978 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/policies.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.505503 dbt_oracle-1.7.5rc1/dbt/include/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      712 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/include/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.508679 dbt_oracle-1.7.5rc1/dbt/include/oracle/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      687 2022-03-30 23:08:38.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      138 2023-12-05 00:49:54.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/dbt_project.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.516357 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)    15223 2024-04-25 20:47:48.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/adapters.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1332 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/apply_grants.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6788 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/catalog.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2177 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/columns.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1174 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/freshness.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.475197 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.518908 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/incremental/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4376 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     9452 2024-03-20 15:11:36.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.520949 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/materialized_view/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4751 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/materialized_view/materialized_view.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.522191 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/python_model/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4345 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/python_model/python.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.523323 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/seed/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1907 2023-12-04 23:12:41.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.526972 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/snapshot/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     9649 2022-11-15 22:09:50.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1444 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4922 2022-12-16 19:27:06.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.528404 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/table/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5489 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/table/table.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.529527 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1191 2022-03-30 23:06:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.530932 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/view/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3468 2023-06-13 04:33:00.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/view/view.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.532423 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/relations/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      838 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/relations/drop.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1906 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/schema_tests.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      757 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/show.sql
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.548263 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)      792 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      881 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/data_types.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1367 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/date_spine.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1457 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/dateadd.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2378 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/datediff.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1037 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/datetrunc.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      691 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/except.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      157 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/generate_series.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      807 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/hash.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      842 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/last_day.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      761 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/position.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      939 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/right.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      916 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/timestamps.sql
+-rw-r--r--   0 abhisoms   (501) staff       (20)      729 2022-05-24 00:59:25.000000 dbt_oracle-1.7.5rc1/dbt/include/oracle/profile_template.yml
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.592396 dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3651 2024-04-25 22:00:39.000000 dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/PKG-INFO
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4420 2024-04-25 22:00:39.000000 dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/SOURCES.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2024-04-25 22:00:39.000000 dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/dependency_links.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        1 2022-04-11 10:34:24.000000 dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/not-zip-safe
+-rw-r--r--   0 abhisoms   (501) staff       (20)       35 2024-04-25 22:00:39.000000 dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/requires.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)        4 2024-04-25 22:00:39.000000 dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/top_level.txt
+-rw-r--r--   0 abhisoms   (501) staff       (20)      100 2021-12-16 21:41:11.000000 dbt_oracle-1.7.5rc1/pyproject.toml
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1338 2024-04-25 22:00:39.595295 dbt_oracle-1.7.5rc1/setup.cfg
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3029 2024-04-25 22:00:15.000000 dbt_oracle-1.7.5rc1/setup.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.560028 dbt_oracle-1.7.5rc1/tests/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3339 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/tests/README.md
+-rw-r--r--   0 abhisoms   (501) staff       (20)      636 2022-08-08 20:50:48.000000 dbt_oracle-1.7.5rc1/tests/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1507 2022-06-27 15:21:32.000000 dbt_oracle-1.7.5rc1/tests/conftest.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.476753 dbt_oracle-1.7.5rc1/tests/functional/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.572094 dbt_oracle-1.7.5rc1/tests/functional/adapter/
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.578589 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/__init__.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.581877 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4919 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4558 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4765 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.583188 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/sync_schema/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/sync_schema/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5473 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2456 2023-02-10 17:55:45.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4652 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4882 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5907 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.584955 dbt_oracle-1.7.5rc1/tests/functional/adapter/macros/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-06-27 15:21:18.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/macros/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2441 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/macros/test_alter_column_type.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.586431 dbt_oracle-1.7.5rc1/tests/functional/adapter/snapshots/
+-rw-r--r--   0 abhisoms   (501) staff       (20)        0 2022-08-03 17:58:52.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/snapshots/__init__.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     3883 2022-08-03 17:58:52.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4629 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_basic.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)      783 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_concurrency.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4322 2024-02-23 01:59:10.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_config.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2979 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_data_types.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5413 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_docs_generate.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6587 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_docs_genreferences.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1201 2022-10-24 21:11:33.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_ephemeral.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     1993 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_generictests_where.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     2910 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_grants.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     4711 2022-07-25 16:13:20.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/test_quoted_relations.py
+drwxr-xr-x   0 abhisoms   (501) staff       (20)        0 2024-04-25 22:00:39.589541 dbt_oracle-1.7.5rc1/tests/functional/adapter/utils/
+-rw-r--r--   0 abhisoms   (501) staff       (20)     5714 2024-02-23 01:55:27.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/utils/test_common_utils.py
+-rw-r--r--   0 abhisoms   (501) staff       (20)     6830 2022-09-07 17:52:56.000000 dbt_oracle-1.7.5rc1/tests/functional/adapter/utils/test_dateutils.py
```

### Comparing `dbt_oracle-1.7.5/LICENSE.txt` & `dbt_oracle-1.7.5rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/PKG-INFO` & `dbt_oracle-1.7.5rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.7.5
+Version: 1.7.5rc1
 Summary: dbt (data build tool) adapter for Oracle Autonomous Database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Requires-Dist: dbt-core<1.8,~=1.7
-Requires-Dist: oracledb==2.2.0
+Requires-Dist: oracledb==2.1.2
 
 # dbt-oracle
 
 [![PyPI version](https://badge.fury.io/py/dbt-oracle.svg)](https://pypi.python.org/pypi/dbt-oracle)
 [![dbt-tests-adapter](https://github.com/oracle/dbt-oracle/actions/workflows/oracle-xe-adapter-tests.yml/badge.svg)](https://github.com/oracle/dbt-oracle/actions/workflows/oracle-xe-adapter-tests.yml)
 [![dbt-oracle docs](https://img.shields.io/badge/docs-read-blue)](https://docs.getdbt.com/reference/warehouse-setups/oracle-setup)
 [![dbt-oracle license](https://img.shields.io/badge/license-Apache%202.0-blue)][4]
```

### Comparing `dbt_oracle-1.7.5/README.md` & `dbt_oracle-1.7.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/bin/create-pem-from-p12` & `dbt_oracle-1.7.5rc1/bin/create-pem-from-p12`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/__init__.py` & `dbt_oracle-1.7.5rc1/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/__init__.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/__init__.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/__version__.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 
   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
 """
-version = "1.7.14"
+version = "1.7.13"
```

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/column.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/column.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/connection_helper.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/connection_helper.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/connections.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/impl.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/keyword_catalog.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/keyword_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/python_submissions.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/relation.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/__init__.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/base.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/materialized_view.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/adapters/oracle/relation_configs/policies.py` & `dbt_oracle-1.7.5rc1/dbt/adapters/oracle/relation_configs/policies.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/__init__.py` & `dbt_oracle-1.7.5rc1/dbt/include/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/__init__.py` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/adapters.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/apply_grants.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/catalog.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/columns.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/freshness.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/incremental/incremental.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/incremental/strategies.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/materialized_view/materialized_view.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/materialized_view/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/python_model/python.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/seed/seed.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/snapshot/strategies.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/snapshot/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/table/table.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/tests/helpers.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/materializations/view/view.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/materializations/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/relations/drop.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/relations/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/schema_tests.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/schema_tests.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/show.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/show.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/cast_bool_to_text.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/cast_bool_to_text.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/data_types.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/date_spine.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/dateadd.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/datediff.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/datetrunc.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/datetrunc.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/except.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/except.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/hash.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/hash.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/last_day.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/last_day.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/position.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/position.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/right.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/right.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/macros/utils/timestamps.sql` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt/include/oracle/profile_template.yml` & `dbt_oracle-1.7.5rc1/dbt/include/oracle/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/dbt_oracle.egg-info/PKG-INFO` & `dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-oracle
-Version: 1.7.5
+Version: 1.7.5rc1
 Summary: dbt (data build tool) adapter for Oracle Autonomous Database
 Home-page: https://github.com/oracle/dbt-oracle
 Author: Oracle
 License: Apache Software License 2.0
 Project-URL: Documentation, https://docs.getdbt.com/reference/warehouse-profiles/oracle-profile
 Project-URL: Source, https://github.com/oracle/dbt-oracle
 Project-URL: Bug Tracker, https://github.com/oracle/dbt-oracle/issues
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 Requires-Dist: dbt-core<1.8,~=1.7
-Requires-Dist: oracledb==2.2.0
+Requires-Dist: oracledb==2.1.2
 
 # dbt-oracle
 
 [![PyPI version](https://badge.fury.io/py/dbt-oracle.svg)](https://pypi.python.org/pypi/dbt-oracle)
 [![dbt-tests-adapter](https://github.com/oracle/dbt-oracle/actions/workflows/oracle-xe-adapter-tests.yml/badge.svg)](https://github.com/oracle/dbt-oracle/actions/workflows/oracle-xe-adapter-tests.yml)
 [![dbt-oracle docs](https://img.shields.io/badge/docs-read-blue)](https://docs.getdbt.com/reference/warehouse-setups/oracle-setup)
 [![dbt-oracle license](https://img.shields.io/badge/license-Apache%202.0-blue)][4]
```

### Comparing `dbt_oracle-1.7.5/dbt_oracle.egg-info/SOURCES.txt` & `dbt_oracle-1.7.5rc1/dbt_oracle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/setup.cfg` & `dbt_oracle-1.7.5rc1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 [options]
 python_requires = >=3.8
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 install_requires = 
 	dbt-core~=1.7,<1.8
-	oracledb==2.2.0
+	oracledb==2.1.2
 test_suite = tests
 test_requires = 
 	dbt-tests-adapter~=1.7,<1.8
 	pytest
 scripts = 
 	bin/create-pem-from-p12
```

### Comparing `dbt_oracle-1.7.5/setup.py` & `dbt_oracle-1.7.5rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 
 requirements = [
         "dbt-core~=1.7,<1.8",
-        "oracledb==2.2.0"
+        "oracledb==2.1.2"
 ]
 
 test_requirements = [
     "dbt-tests-adapter~=1.7,<1.8",
     "pytest"
 ]
 
@@ -55,15 +55,15 @@
     'Bug Tracker': 'https://github.com/oracle/dbt-oracle/issues',
     'CI': 'https://github.com/oracle/dbt-oracle/actions',
     "Release Notes": "https://github.com/oracle/dbt-oracle/releases"
 }
 
 url = 'https://github.com/oracle/dbt-oracle'
 
-VERSION = '1.7.5'
+VERSION = '1.7.5rc1'
 setup(
     author="Oracle",
     python_requires='>=3.8',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `dbt_oracle-1.7.5/tests/README.md` & `dbt_oracle-1.7.5rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/__init__.py` & `dbt_oracle-1.7.5rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/conftest.py` & `dbt_oracle-1.7.5rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/test_quoted_columns_incremental_insert.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/quotes/test_quotes_enabled_in_model.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/sync_schema/test_quote_special_characters_and_keywords.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_quotes_with_merge_update_columns.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/incremental_materialization/test_unique_id.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/incremental_materialization/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/macros/test_alter_column_type.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/macros/test_alter_column_type.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/snapshots/test_invalidate_deletes.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/snapshots/test_invalidate_deletes.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_basic.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_concurrency.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_config.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_config.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_data_types.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_data_types.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_docs_generate.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_docs_genreferences.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_docs_genreferences.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_ephemeral.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_generictests_where.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_generictests_where.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_grants.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_grants.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/test_quoted_relations.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/test_quoted_relations.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/utils/test_common_utils.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/utils/test_common_utils.py`

 * *Files identical despite different names*

### Comparing `dbt_oracle-1.7.5/tests/functional/adapter/utils/test_dateutils.py` & `dbt_oracle-1.7.5rc1/tests/functional/adapter/utils/test_dateutils.py`

 * *Files identical despite different names*

