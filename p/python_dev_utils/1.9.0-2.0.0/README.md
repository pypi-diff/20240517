# Comparing `tmp/python_dev_utils-1.9.0.tar.gz` & `tmp/python_dev_utils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-1.9.0.tar", last modified: Mon May 13 09:18:56 2024, max compression
+gzip compressed data, was "python_dev_utils-2.0.0.tar", last modified: Fri May 17 10:36:24 2024, max compression
```

## Comparing `python_dev_utils-1.9.0.tar` & `python_dev_utils-2.0.0.tar`

### file list

```diff
@@ -1,98 +1,99 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.9.0/LICENCE
--rw-r--r--   0        0        0     5202 2024-05-03 14:00:43.373038 python_dev_utils-1.9.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.9.0/dev_utils/__init__.py
--rw-r--r--   0        0        0      407 2024-04-27 11:38:00.638361 python_dev_utils-1.9.0/dev_utils/alembic/__init__.py
--rw-r--r--   0        0        0     1688 2024-04-27 11:26:29.918706 python_dev_utils-1.9.0/dev_utils/alembic/ignore_table.py
--rw-r--r--   0        0        0      921 2024-04-25 13:19:12.947590 python_dev_utils-1.9.0/dev_utils/alembic/migration_numbering.py
--rw-r--r--   0        0        0      892 2024-04-27 09:22:42.892410 python_dev_utils-1.9.0/dev_utils/alembic/utils.py
--rw-r--r--   0        0        0        0 2024-05-01 13:16:34.515756 python_dev_utils-1.9.0/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.9.0/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.9.0/dev_utils/core/exc.py
--rw-r--r--   0        0        0      571 2024-05-13 07:44:56.451508 python_dev_utils-1.9.0/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.9.0/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.9.0/dev_utils/core/results.py
--rw-r--r--   0        0        0      662 2024-05-01 13:15:58.588972 python_dev_utils-1.9.0/dev_utils/core/utils/__init__.py
--rw-r--r--   0        0        0      265 2024-04-26 08:51:43.164520 python_dev_utils-1.9.0/dev_utils/core/utils/datetime.py
--rw-r--r--   0        0        0     1040 2024-04-27 11:36:17.853859 python_dev_utils-1.9.0/dev_utils/core/utils/envs.py
--rw-r--r--   0        0        0      766 2024-04-27 11:36:37.669763 python_dev_utils-1.9.0/dev_utils/core/utils/humanize.py
--rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-1.9.0/dev_utils/core/utils/inspect.py
--rw-r--r--   0        0        0     1578 2024-04-27 11:36:52.604691 python_dev_utils-1.9.0/dev_utils/core/utils/strings.py
--rw-r--r--   0        0        0      328 2024-05-03 13:54:07.264813 python_dev_utils-1.9.0/dev_utils/fastapi/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.9.0/dev_utils/fastapi/middlewares/__init__.py
--rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.9.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
--rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-1.9.0/dev_utils/fastapi/openapi/__init__.py
--rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-1.9.0/dev_utils/fastapi/openapi/exporter.py
--rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-1.9.0/dev_utils/py.typed
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.9.0/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16338 2024-05-13 06:46:01.972166 python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0        0 2024-05-08 10:00:10.227785 python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/ext/__init__.py
--rw-r--r--   0        0        0    10333 2024-05-13 09:17:00.325336 python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/ext/fastapi.py
--rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     4138 2024-05-02 07:47:31.057832 python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/audit.py
--rw-r--r--   0        0        0     1261 2024-04-30 19:40:08.223220 python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/base.py
--rw-r--r--   0        0        0     8121 2024-05-06 10:12:09.604547 python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/general.py
--rw-r--r--   0        0        0     1229 2024-04-30 19:48:16.754203 python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/ids.py
--rw-r--r--   0        0        0     1005 2024-04-25 11:36:06.219628 python_dev_utils-1.9.0/dev_utils/sqlalchemy/naming_conventions.py
--rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.9.0/dev_utils/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.9.0/dev_utils/sqlalchemy/profiling/containers.py
--rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.9.0/dev_utils/sqlalchemy/profiling/profilers.py
--rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.9.0/dev_utils/sqlalchemy/profiling/utils.py
--rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.9.0/dev_utils/sqlalchemy/types/__init__.py
--rw-r--r--   0        0        0     2457 2024-05-01 11:31:16.251129 python_dev_utils-1.9.0/dev_utils/sqlalchemy/types/datetime.py
--rw-r--r--   0        0        0     3348 2024-05-02 06:36:14.437004 python_dev_utils-1.9.0/dev_utils/sqlalchemy/types/pydantic.py
--rw-r--r--   0        0        0    14281 2024-04-25 13:17:22.836564 python_dev_utils-1.9.0/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0      863 2024-05-03 13:55:40.190397 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/__init__.py
--rw-r--r--   0        0        0     3474 2024-05-03 13:51:00.856651 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/constants.py
--rw-r--r--   0        0        0    12313 2024-05-03 13:51:58.674390 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/exc.py
--rw-r--r--   0        0        0        0 2024-05-08 10:01:14.439027 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/__init__.py
--rw-r--r--   0        0        0      309 2024-05-06 06:55:08.545628 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/__init__.py
--rw-r--r--   0        0        0     3692 2024-05-08 10:02:34.539731 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/handlers.py
--rw-r--r--   0        0        0     2176 2024-05-03 13:49:22.085103 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/openapi_override.py
--rw-r--r--   0        0        0     2536 2024-05-06 06:57:09.609863 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/schemas.py
--rw-r--r--   0        0        0     1257 2024-05-03 13:49:14.900136 python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/utils.py
--rw-r--r--   0        0        0     3250 2024-05-13 09:18:56.058748 python_dev_utils-1.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.9.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 06:25:13.597435 python_dev_utils-1.9.0/tests/alembic/__init__.py
--rw-r--r--   0        0        0     1256 2024-04-27 11:29:42.045776 python_dev_utils-1.9.0/tests/alembic/test_ignore_table.py
--rw-r--r--   0        0        0      772 2024-04-26 09:16:01.643863 python_dev_utils-1.9.0/tests/alembic/test_migration_numbering.py
--rw-r--r--   0        0        0      746 2024-04-27 11:15:08.238156 python_dev_utils-1.9.0/tests/alembic/test_utils.py
--rw-r--r--   0        0        0     9331 2024-05-02 06:38:31.027987 python_dev_utils-1.9.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.9.0/tests/core/__init__.py
--rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.9.0/tests/core/test_abstract.py
--rw-r--r--   0        0        0      393 2024-04-27 09:47:42.911786 python_dev_utils-1.9.0/tests/core/test_datetime_utils.py
--rw-r--r--   0        0        0     3152 2024-04-27 10:11:57.366723 python_dev_utils-1.9.0/tests/core/test_env_utils.py
--rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-1.9.0/tests/core/test_guards.py
--rw-r--r--   0        0        0     1485 2024-04-27 10:11:40.278820 python_dev_utils-1.9.0/tests/core/test_humanize_utils.py
--rw-r--r--   0        0        0      487 2024-04-27 09:48:27.358654 python_dev_utils-1.9.0/tests/core/test_inspect_utils.py
--rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.9.0/tests/core/test_results.py
--rw-r--r--   0        0        0     1258 2024-04-27 11:01:55.517321 python_dev_utils-1.9.0/tests/core/test_strings_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.9.0/tests/fastapi/__init__.py
--rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.9.0/tests/fastapi/test_middlewares.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.9.0/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.9.0/tests/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0    10025 2024-05-13 08:53:44.578433 python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_fastapi_ext.py
--rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.9.0/tests/sqlalchemy/mixins/__init__.py
--rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.9.0/tests/sqlalchemy/mixins/test_audit.py
--rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.9.0/tests/sqlalchemy/mixins/test_base.py
--rw-r--r--   0        0        0     8632 2024-05-06 10:12:41.636497 python_dev_utils-1.9.0/tests/sqlalchemy/mixins/test_general.py
--rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.9.0/tests/sqlalchemy/mixins/test_ids.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.9.0/tests/sqlalchemy/profiling/__init__.py
--rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.9.0/tests/sqlalchemy/profiling/test_profilers.py
--rw-r--r--   0        0        0      394 2024-04-26 09:26:06.714312 python_dev_utils-1.9.0/tests/sqlalchemy/test_naming_conventions.py
--rw-r--r--   0        0        0     4407 2024-05-02 06:53:17.265549 python_dev_utils-1.9.0/tests/sqlalchemy/test_types.py
--rw-r--r--   0        0        0     9789 2024-04-25 13:18:24.229021 python_dev_utils-1.9.0/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.9.0/tests/types.py
--rw-r--r--   0        0        0     8044 2024-05-13 06:48:08.244532 python_dev_utils-1.9.0/tests/utils.py
--rw-r--r--   0        0        0        0 2024-05-03 13:53:03.076101 python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/__init__.py
--rw-r--r--   0        0        0     1467 2024-05-08 10:02:15.524852 python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/conftest.py
--rw-r--r--   0        0        0     6060 2024-05-03 13:56:41.003124 python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py
--rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py
--rw-r--r--   0        0        0     1605 2024-05-08 10:01:38.593958 python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py
--rw-r--r--   0        0        0     5907 1970-01-01 00:00:00.000000 python_dev_utils-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-2.0.0/LICENCE
+-rw-r--r--   0        0        0     5202 2024-05-03 14:00:43.373038 python_dev_utils-2.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-2.0.0/dev_utils/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-27 11:38:00.638361 python_dev_utils-2.0.0/dev_utils/alembic/__init__.py
+-rw-r--r--   0        0        0     1688 2024-04-27 11:26:29.918706 python_dev_utils-2.0.0/dev_utils/alembic/ignore_table.py
+-rw-r--r--   0        0        0      921 2024-04-25 13:19:12.947590 python_dev_utils-2.0.0/dev_utils/alembic/migration_numbering.py
+-rw-r--r--   0        0        0      892 2024-04-27 09:22:42.892410 python_dev_utils-2.0.0/dev_utils/alembic/utils.py
+-rw-r--r--   0        0        0        0 2024-05-01 13:16:34.515756 python_dev_utils-2.0.0/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-2.0.0/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-2.0.0/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-05-14 06:51:06.437977 python_dev_utils-2.0.0/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-2.0.0/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-2.0.0/dev_utils/core/results.py
+-rw-r--r--   0        0        0      662 2024-05-01 13:15:58.588972 python_dev_utils-2.0.0/dev_utils/core/utils/__init__.py
+-rw-r--r--   0        0        0      265 2024-04-26 08:51:43.164520 python_dev_utils-2.0.0/dev_utils/core/utils/datetime.py
+-rw-r--r--   0        0        0     1040 2024-04-27 11:36:17.853859 python_dev_utils-2.0.0/dev_utils/core/utils/envs.py
+-rw-r--r--   0        0        0      766 2024-04-27 11:36:37.669763 python_dev_utils-2.0.0/dev_utils/core/utils/humanize.py
+-rw-r--r--   0        0        0      677 2024-04-16 09:16:22.025777 python_dev_utils-2.0.0/dev_utils/core/utils/inspect.py
+-rw-r--r--   0        0        0     1578 2024-04-27 11:36:52.604691 python_dev_utils-2.0.0/dev_utils/core/utils/strings.py
+-rw-r--r--   0        0        0      328 2024-05-03 13:54:07.264813 python_dev_utils-2.0.0/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-2.0.0/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-2.0.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0        0 2024-04-22 08:05:13.247824 python_dev_utils-2.0.0/dev_utils/fastapi/openapi/__init__.py
+-rw-r--r--   0        0        0     1901 2024-04-23 07:13:12.131657 python_dev_utils-2.0.0/dev_utils/fastapi/openapi/exporter.py
+-rw-r--r--   0        0        0        0 2024-04-16 07:40:41.209053 python_dev_utils-2.0.0/dev_utils/py.typed
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-2.0.0/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16338 2024-05-13 06:46:01.972166 python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:00:10.227785 python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/ext/__init__.py
+-rw-r--r--   0        0        0     7831 2024-05-14 12:53:52.075437 python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/ext/fastapi.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     4152 2024-05-17 09:40:34.381018 python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1261 2024-04-30 19:40:08.223220 python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     8113 2024-05-14 11:20:13.960368 python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0     1229 2024-04-30 19:48:16.754203 python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0     1005 2024-04-25 11:36:06.219628 python_dev_utils-2.0.0/dev_utils/sqlalchemy/naming_conventions.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-2.0.0/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-2.0.0/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-2.0.0/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-2.0.0/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-2.0.0/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2475 2024-05-14 06:40:49.535172 python_dev_utils-2.0.0/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0     3386 2024-05-14 08:57:11.526339 python_dev_utils-2.0.0/dev_utils/sqlalchemy/types/pydantic.py
+-rw-r--r--   0        0        0     3777 2024-05-14 08:46:10.141999 python_dev_utils-2.0.0/dev_utils/sqlalchemy/types/relativedelta.py
+-rw-r--r--   0        0        0    14281 2024-04-25 13:17:22.836564 python_dev_utils-2.0.0/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0      863 2024-05-03 13:55:40.190397 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0     3474 2024-05-03 13:51:00.856651 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/constants.py
+-rw-r--r--   0        0        0    12148 2024-05-14 11:22:34.773674 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:01:14.439027 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-06 06:55:08.545628 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/__init__.py
+-rw-r--r--   0        0        0     3692 2024-05-08 10:02:34.539731 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/handlers.py
+-rw-r--r--   0        0        0     2176 2024-05-03 13:49:22.085103 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/openapi_override.py
+-rw-r--r--   0        0        0     2536 2024-05-06 06:57:09.609863 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/schemas.py
+-rw-r--r--   0        0        0     1257 2024-05-03 13:49:14.900136 python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/utils.py
+-rw-r--r--   0        0        0     3315 2024-05-17 10:36:24.025613 python_dev_utils-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:25:13.597435 python_dev_utils-2.0.0/tests/alembic/__init__.py
+-rw-r--r--   0        0        0     1256 2024-04-27 11:29:42.045776 python_dev_utils-2.0.0/tests/alembic/test_ignore_table.py
+-rw-r--r--   0        0        0      772 2024-04-26 09:16:01.643863 python_dev_utils-2.0.0/tests/alembic/test_migration_numbering.py
+-rw-r--r--   0        0        0      746 2024-04-27 11:15:08.238156 python_dev_utils-2.0.0/tests/alembic/test_utils.py
+-rw-r--r--   0        0        0     9331 2024-05-02 06:38:31.027987 python_dev_utils-2.0.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-2.0.0/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-2.0.0/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      393 2024-04-27 09:47:42.911786 python_dev_utils-2.0.0/tests/core/test_datetime_utils.py
+-rw-r--r--   0        0        0     3152 2024-04-27 10:11:57.366723 python_dev_utils-2.0.0/tests/core/test_env_utils.py
+-rw-r--r--   0        0        0      876 2024-04-16 09:26:13.267072 python_dev_utils-2.0.0/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1485 2024-04-27 10:11:40.278820 python_dev_utils-2.0.0/tests/core/test_humanize_utils.py
+-rw-r--r--   0        0        0      487 2024-04-27 09:48:27.358654 python_dev_utils-2.0.0/tests/core/test_inspect_utils.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-2.0.0/tests/core/test_results.py
+-rw-r--r--   0        0        0     1258 2024-04-27 11:01:55.517321 python_dev_utils-2.0.0/tests/core/test_strings_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-2.0.0/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-2.0.0/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-2.0.0/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-2.0.0/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0    10025 2024-05-13 08:53:44.578433 python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_fastapi_ext.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-2.0.0/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-05-17 10:34:06.541762 python_dev_utils-2.0.0/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-2.0.0/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     8632 2024-05-06 10:12:41.636497 python_dev_utils-2.0.0/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-2.0.0/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-2.0.0/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-2.0.0/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0      394 2024-04-26 09:26:06.714312 python_dev_utils-2.0.0/tests/sqlalchemy/test_naming_conventions.py
+-rw-r--r--   0        0        0     6740 2024-05-14 08:48:39.966849 python_dev_utils-2.0.0/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     9789 2024-04-25 13:18:24.229021 python_dev_utils-2.0.0/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-2.0.0/tests/types.py
+-rw-r--r--   0        0        0     8318 2024-05-17 07:13:52.003812 python_dev_utils-2.0.0/tests/utils.py
+-rw-r--r--   0        0        0        0 2024-05-03 13:53:03.076101 python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/__init__.py
+-rw-r--r--   0        0        0     1467 2024-05-08 10:02:15.524852 python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/conftest.py
+-rw-r--r--   0        0        0     6060 2024-05-03 13:56:41.003124 python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2074 2024-04-22 12:16:38.058690 python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py
+-rw-r--r--   0        0        0     1605 2024-05-08 10:01:38.593958 python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py
+-rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 python_dev_utils-2.0.0/PKG-INFO
```

### Comparing `python_dev_utils-1.9.0/LICENCE` & `python_dev_utils-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/README.md` & `python_dev_utils-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/alembic/ignore_table.py` & `python_dev_utils-2.0.0/dev_utils/alembic/ignore_table.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/alembic/migration_numbering.py` & `python_dev_utils-2.0.0/dev_utils/alembic/migration_numbering.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/alembic/utils.py` & `python_dev_utils-2.0.0/dev_utils/alembic/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/abstract.py` & `python_dev_utils-2.0.0/dev_utils/core/abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/exc.py` & `python_dev_utils-2.0.0/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/guards.py` & `python_dev_utils-2.0.0/dev_utils/core/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/logging.py` & `python_dev_utils-2.0.0/dev_utils/core/logging.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/results.py` & `python_dev_utils-2.0.0/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/utils/__init__.py` & `python_dev_utils-2.0.0/dev_utils/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/utils/envs.py` & `python_dev_utils-2.0.0/dev_utils/core/utils/envs.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/utils/humanize.py` & `python_dev_utils-2.0.0/dev_utils/core/utils/humanize.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/utils/inspect.py` & `python_dev_utils-2.0.0/dev_utils/core/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/core/utils/strings.py` & `python_dev_utils-2.0.0/dev_utils/core/utils/strings.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py` & `python_dev_utils-2.0.0/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/fastapi/openapi/exporter.py` & `python_dev_utils-2.0.0/dev_utils/fastapi/openapi/exporter.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/filters/types.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/filters/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/base.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/general.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
             exclude = set()
         if isinstance(item, dict):
             return self._is_dict_different_from(item, exclude)
         elif self.__class__ == item.__class__:  # type: ignore
             return self._is_model_different_from(item, exclude)
         if self.__safe_difference__:
             return True
-        msg = f"Incorrect item. Ожидались: Dict, {self.__class__.__name__}. Got: {type(item)}."
+        msg = f"Incorrect item. Expected: Dict or {self.__class__.__name__}. Got: {type(item)}."
         raise TypeError(msg)
 
 
 @declarative_mixin
 class BetterReprMixin(BaseModelMixin):
     """Mixin with better __repr__ method for SQLAlchemy model instances."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/mixins/ids.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/mixins/ids.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/naming_conventions.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/profiling/containers.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/profiling/profilers.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/profiling/utils.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/types/datetime.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/types/datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, Any
 
 from sqlalchemy import DateTime, TypeDecorator
 from sqlalchemy.ext.compiler import compiles  # type: ignore
 from sqlalchemy.sql import expression
 
 if TYPE_CHECKING:
-    from sqlalchemy import Dialect
+    from sqlalchemy.engine.interfaces import Dialect
 
 
 UTC = zoneinfo.ZoneInfo("UTC")
 
 
 class Utcnow(expression.FunctionElement[datetime.datetime]):
     """Alias for DateTime type for new mapping.
```

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/types/pydantic.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/types/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pydantic.version import version_short
 from sqlalchemy import JSON as JSON_COLUMN
 from sqlalchemy.dialects.postgresql import JSONB
 from sqlalchemy.types import JSON as JSON_TYPE
 from sqlalchemy.types import TypeDecorator
 
 if TYPE_CHECKING:
-    from sqlalchemy import Dialect
+    from sqlalchemy.engine.interfaces import Dialect
 
 pydantic_version = tuple(map(int, version_short().split(".")))
 T = TypeVar("T", BaseModel, list[BaseModel], tuple[BaseModel, ...])
 
 is_pydantic_v2 = pydantic_version >= (2, 0)
 
 if is_pydantic_v2:
@@ -37,14 +37,15 @@
     return json.dumps(obj, default=pydantic_encoder, **kwargs)
 
 
 class PydanticType(TypeDecorator[T]):
     """Type decorator for JSON field as pydantic model."""
 
     impl = JSON_TYPE
+    cache_ok = True
 
     def __init__(self, pydantic_type: type[T]) -> None:
         super().__init__()
         self.pydantic_type = pydantic_type
 
     @staticmethod
     def _is_valid_pydantic_model(
```

### Comparing `python_dev_utils-1.9.0/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-2.0.0/dev_utils/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/__init__.py` & `python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/constants.py` & `python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/constants.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/exc.py` & `python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/exc.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     message: str = abstract_class_property(str)
     location: str | None = None
     template: Template | str | None = None
     attr: str | None = None
     nested_errors: list["BaseVerboseHTTPException"] | None = None
 
     def __init__(  # noqa: D105
-        self: Self,
+        self,
         *nested_errors: "BaseVerboseHTTPException",
         status_code: int | None = None,
         code: str | None = None,
         type_: str | None = None,
         message: str | None = None,
         location: str | None = None,
         template: Template | str | None = None,
@@ -119,38 +119,38 @@
             self.message = self.template.format(**mapping)
         if status_code is not None:
             self.status_code = status_code
         if nested_errors:
             self.nested_errors = list(nested_errors)
         self.headers = headers
 
-    def _get_attribute(self: Self, name: str) -> Any:  # noqa: ANN401  # pragma: no coverage
+    def _get_attribute(self, name: str) -> Any:  # noqa: ANN401  # pragma: no coverage
         """Safe getattr for verbose http exceptions."""
         try:
             return repr(getattr(self, name))
         except (AttributeError, TypeError):
             return ABSTRACT_PROPERTY_DEFAULT_VALUE
 
-    def __repr__(self: Self) -> str:  # noqa: D105
+    def __repr__(self) -> str:  # noqa: D105
         cls_path = get_object_class_absolute_name(self.__class__)
         attrs = (
             f'status_code={self.status_code}, code={self._get_attribute("code")}, '
             f'type={self._get_attribute("type_")}, message={self._get_attribute("message")}, '
             f'location={self.location}, template={self.template}, attr={self.attr}'
         )
         return f"{cls_path}({attrs})"
 
-    def __str__(self: Self) -> str:  # noqa: D105  # pragma: no coverage
+    def __str__(self) -> str:  # noqa: D105  # pragma: no coverage
         try:
             return self.message
         except (AttributeError, TypeError):
             return ABSTRACT_CLS_DEFAULT_VALUE
 
     def from_template(
-        self: Self,
+        self,
         **mapping: object,
     ) -> Self:
         """Fill message with template and return self.
 
         Usage:
         ```
         class SomeClass(BaseVerboseHTTPException):
@@ -172,16 +172,16 @@
             return self
         if isinstance(self.template, Template):
             self.message = self.template.safe_substitute(**mapping)
         else:
             self.message = self.template.format(**mapping)
         return self
 
-    def with_attr(self: Self, attr_name: str) -> Self:
-        """Добавляет поле атрибута в класс исключения.
+    def with_attr(self, attr_name: str) -> Self:
+        """Add attribute of the error.
 
         Usage:
         ```
         class SomeClass(BaseVerboseHTTPException):
             status_code = status.HTTP_400_BAD_REQUEST
             code = 'abc'
             type_ = 'abc'
@@ -194,16 +194,16 @@
 
         >>> SomeClass().with_attr('attr').attr
         'attr'
         """
         self.attr = attr_name
         return self
 
-    def with_location(self: Self, location: str) -> Self:
-        """Добавляет поле расположения в класс исключения.
+    def with_location(self, location: str) -> Self:
+        """Add location of the error.
 
         Usage:
         ```
         class SomeClass(BaseVerboseHTTPException):
             status_code = status.HTTP_400_BAD_REQUEST
             code = 'abc'
             type_ = 'abc'
@@ -217,18 +217,18 @@
         >>> SomeClass().with_location('loc').location
         'loc'
         """
         self.location = location
         return self
 
     def with_nested_errors(
-        self: Self,
+        self,
         nested_errors: Sequence["BaseVerboseHTTPException"],
     ) -> Self:
-        """Convert Exception instance into dict.
+        """Add nested errors to parent (self) error.
 
         Usage:
         ```
         class SomeClass(BaseVerboseHTTPException):
             code = 'abc'
             type_ = 'abc'
             message = 'abc'
@@ -247,15 +247,15 @@
         else:
             self.nested_errors = (
                 nested_errors.copy() if isinstance(nested_errors, list) else list(nested_errors)
             )
         return self
 
     def as_dict(
-        self: Self,
+        self,
         attr_name: str | None = None,
         location: str | None = None,
         nested_errors: Sequence["BaseVerboseHTTPException"] | None = None,
         **mapping: object,
     ) -> VerboseHTTPExceptionDict:
         """Convert Exception instance into dict.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/handlers.py` & `python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/openapi_override.py` & `python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/openapi_override.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/schemas.py` & `python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/schemas.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/dev_utils/verbose_http_exceptions/ext/fastapi/utils.py` & `python_dev_utils-2.0.0/dev_utils/verbose_http_exceptions/ext/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/pyproject.toml` & `python_dev_utils-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -172,40 +172,44 @@
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
     "pytest-mock>=3.14.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "1.9.0"
+version = "2.0.0"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 profiling = [
     "fastapi",
-    "sqlalchemy>=2.0.28",
+    "sqlalchemy>=2.0",
 ]
 sqlalchemy_filters = [
-    "sqlalchemy>=2.0.28",
+    "sqlalchemy>=2.0",
 ]
 extract_openapi = [
     "fastapi",
     "uvicorn",
 ]
 migration_numbering = [
     "alembic",
 ]
+relativedelta_type = [
+    "python-dateutil",
+    "sqlalchemy>=2.0",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `python_dev_utils-1.9.0/tests/alembic/test_ignore_table.py` & `python_dev_utils-2.0.0/tests/alembic/test_ignore_table.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/alembic/test_migration_numbering.py` & `python_dev_utils-2.0.0/tests/alembic/test_migration_numbering.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/alembic/test_utils.py` & `python_dev_utils-2.0.0/tests/alembic/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/conftest.py` & `python_dev_utils-2.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/core/test_abstract.py` & `python_dev_utils-2.0.0/tests/core/test_abstract.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/core/test_env_utils.py` & `python_dev_utils-2.0.0/tests/core/test_env_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/core/test_guards.py` & `python_dev_utils-2.0.0/tests/core/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/core/test_humanize_utils.py` & `python_dev_utils-2.0.0/tests/core/test_humanize_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/core/test_results.py` & `python_dev_utils-2.0.0/tests/core/test_results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/core/test_strings_utils.py` & `python_dev_utils-2.0.0/tests/core/test_strings_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_converters.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_fastapi_ext.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_fastapi_ext.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_guards.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_guards.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/filters/test_operators.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/mixins/test_audit.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/mixins/test_audit.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/mixins/test_base.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/mixins/test_base.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/mixins/test_general.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/mixins/test_general.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/profiling/test_profilers.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/sqlalchemy/test_utils.py` & `python_dev_utils-2.0.0/tests/sqlalchemy/test_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/types.py` & `python_dev_utils-2.0.0/tests/types.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/utils.py` & `python_dev_utils-2.0.0/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import datetime
 import random
 from typing import TYPE_CHECKING, Any, TypeVar
 
+from dateutil.relativedelta import relativedelta
 from pydantic import BaseModel
 from sqlalchemy import ForeignKey, inspect
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.hybrid import hybrid_method, hybrid_property
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
+from dev_utils.sqlalchemy.mixins.audit import AuditMixin
 from dev_utils.sqlalchemy.mixins.general import BetterReprMixin, DictConverterMixin, DifferenceMixin
 from dev_utils.sqlalchemy.types.datetime import UTCDateTime
 from dev_utils.sqlalchemy.types.pydantic import PydanticType
+from dev_utils.sqlalchemy.types.relativedelta import RelativeInterval
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
@@ -232,18 +235,19 @@
         return self.name + "" + self.other_name
 
     @hybrid_method
     def get_full_name(self):  # noqa
         return self.name + "" + self.other_name
 
 
-class TableWithUTCDT(Base):  # noqa: D101
+class TableWithUTCDT(AuditMixin, Base):  # noqa: D101
     __tablename__ = "table_with_UTC_dt"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     dt_field: Mapped[datetime.datetime | None] = mapped_column(UTCDateTime)
     pydantic_type: Mapped[PydanticTestSchema | None] = mapped_column(
         PydanticType(PydanticTestSchema),
     )
     pydantic_list_type: Mapped[list[PydanticTestSchema] | None] = mapped_column(
         PydanticType(list[PydanticTestSchema]),
     )
+    relative_interval: Mapped[relativedelta | None] = mapped_column(RelativeInterval)
```

### Comparing `python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/conftest.py` & `python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/conftest.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py` & `python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py` & `python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_handlers.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py` & `python_dev_utils-2.0.0/tests/verbose_http_exceptions.py/test_verbose_http_exceptions_fastapi_utils.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-1.9.0/PKG-INFO` & `python_dev_utils-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 1.9.0
+Version: 2.0.0
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: profiling
 Provides-Extra: sqlalchemy-filters
 Provides-Extra: extract-openapi
 Provides-Extra: migration-numbering
+Provides-Extra: relativedelta-type
 Requires-Dist: fastapi; extra == "profiling"
-Requires-Dist: sqlalchemy>=2.0.28; extra == "profiling"
-Requires-Dist: sqlalchemy>=2.0.28; extra == "sqlalchemy-filters"
+Requires-Dist: sqlalchemy>=2.0; extra == "profiling"
+Requires-Dist: sqlalchemy>=2.0; extra == "sqlalchemy-filters"
 Requires-Dist: fastapi; extra == "extract-openapi"
 Requires-Dist: uvicorn; extra == "extract-openapi"
 Requires-Dist: alembic; extra == "migration-numbering"
+Requires-Dist: python-dateutil; extra == "relativedelta-type"
+Requires-Dist: sqlalchemy>=2.0; extra == "relativedelta-type"
 Description-Content-Type: text/markdown
 
 
 # Dev utils
 
 ![coverage](./coverage.svg)
```

