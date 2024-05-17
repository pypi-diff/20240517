# Comparing `tmp/acquiring-0.2.0.tar.gz` & `tmp/acquiring-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acquiring-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "acquiring-0.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `acquiring-0.2.0.tar` & `acquiring-0.3.0.tar`

### file list

```diff
@@ -1,86 +1,121 @@
--rw-r--r--   0        0        0       28 2024-04-08 09:12:12.325260 acquiring-0.2.0/.adr-dir
--rw-r--r--   0        0        0      108 2024-04-07 19:04:14.603829 acquiring-0.2.0/.env.example
--rw-r--r--   0        0        0     3104 2024-04-07 19:04:14.603927 acquiring-0.2.0/.gitignore
--rw-r--r--   0        0        0      176 2024-04-08 09:23:42.281005 acquiring-0.2.0/.markdownlint.json
--rw-r--r--   0        0        0     2835 2024-04-08 20:23:16.924084 acquiring-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      835 2024-04-07 19:04:14.604120 acquiring-0.2.0/Dockerfile
--rw-r--r--   0        0        0     1070 2024-04-07 19:04:14.604203 acquiring-0.2.0/LICENSE
--rw-r--r--   0        0        0      189 2024-04-07 19:04:14.604273 acquiring-0.2.0/MANIFEST.in
--rw-r--r--   0        0        0     1873 2024-04-08 18:23:16.298302 acquiring-0.2.0/README.md
--rw-r--r--   0        0        0       70 2024-04-08 20:30:46.801991 acquiring-0.2.0/acquiring/__init__.py
--rw-r--r--   0        0        0       29 2024-04-07 19:04:14.604503 acquiring-0.2.0/acquiring/admin.py
--rw-r--r--   0        0        0      181 2024-04-07 19:04:14.604568 acquiring-0.2.0/acquiring/apps.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.604637 acquiring-0.2.0/acquiring/contrib/__init__.py
--rw-r--r--   0        0        0      459 2024-04-07 19:04:14.604773 acquiring-0.2.0/acquiring/contrib/paypal/__init__.py
--rw-r--r--   0        0        0     9988 2024-04-07 19:04:14.604911 acquiring-0.2.0/acquiring/contrib/paypal/adapter.py
--rw-r--r--   0        0        0      178 2024-04-07 19:04:14.605022 acquiring-0.2.0/acquiring/contrib/paypal/blocks/__init__.py
--rw-r--r--   0        0        0     1290 2024-04-07 19:04:14.605098 acquiring-0.2.0/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py
--rw-r--r--   0        0        0     1936 2024-04-07 19:04:14.605175 acquiring-0.2.0/acquiring/contrib/paypal/blocks/paypal_create_order.py
--rw-r--r--   0        0        0     1572 2024-04-07 19:04:14.605255 acquiring-0.2.0/acquiring/contrib/paypal/domain.py
--rw-r--r--   0        0        0      719 2024-04-07 19:04:14.605370 acquiring-0.2.0/acquiring/domain/__init__.py
--rw-r--r--   0        0        0     1572 2024-04-07 19:04:14.605458 acquiring-0.2.0/acquiring/domain/blocks.py
--rw-r--r--   0        0        0    35649 2024-04-07 19:04:14.605584 acquiring-0.2.0/acquiring/domain/decision_logic.py
--rw-r--r--   0        0        0      481 2024-04-07 19:04:14.605678 acquiring-0.2.0/acquiring/domain/events.py
--rw-r--r--   0        0        0    18529 2024-04-07 19:04:14.605769 acquiring-0.2.0/acquiring/domain/flow.py
--rw-r--r--   0        0        0     2744 2024-04-07 19:04:14.605862 acquiring-0.2.0/acquiring/domain/payments.py
--rw-r--r--   0        0        0     1658 2024-04-07 19:04:14.605935 acquiring-0.2.0/acquiring/domain/providers.py
--rw-r--r--   0        0        0      504 2024-04-07 19:04:14.606013 acquiring-0.2.0/acquiring/enums.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.606096 acquiring-0.2.0/acquiring/migrations/__init__.py
--rw-r--r--   0        0        0     6658 2024-04-07 19:04:14.606394 acquiring-0.2.0/acquiring/migrations/django/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.606459 acquiring-0.2.0/acquiring/migrations/django/__init__.py
--rw-r--r--   0        0        0      491 2024-04-07 19:04:14.606638 acquiring-0.2.0/acquiring/models/__init__.py
--rw-r--r--   0        0        0     9250 2024-04-07 19:04:14.606754 acquiring-0.2.0/acquiring/models/django.py
--rw-r--r--   0        0        0     2199 2024-04-07 19:04:14.606881 acquiring-0.2.0/acquiring/protocols/__init__.py
--rw-r--r--   0        0        0      252 2024-04-07 19:04:14.606957 acquiring-0.2.0/acquiring/protocols/events.py
--rw-r--r--   0        0        0     2866 2024-04-07 19:04:14.607034 acquiring-0.2.0/acquiring/protocols/payments.py
--rw-r--r--   0        0        0      842 2024-04-07 19:04:14.607107 acquiring-0.2.0/acquiring/protocols/providers.py
--rw-r--r--   0        0        0      264 2024-04-07 19:04:14.607177 acquiring-0.2.0/acquiring/protocols/repositories.py
--rw-r--r--   0        0        0      193 2024-04-07 19:04:14.607301 acquiring-0.2.0/acquiring/repositories/__init__.py
--rw-r--r--   0        0        0     7589 2024-04-07 19:04:14.607396 acquiring-0.2.0/acquiring/repositories/django.py
--rw-r--r--   0        0        0     1144 2024-04-07 19:04:14.607482 acquiring-0.2.0/acquiring/settings.py
--rw-r--r--   0        0        0      111 2024-04-07 19:04:14.607558 acquiring-0.2.0/acquiring/utils.py
--rw-r--r--   0        0        0      458 2024-04-07 19:04:14.607634 acquiring-0.2.0/docker-compose.yaml
--rw-r--r--   0        0        0      483 2024-04-08 09:12:13.455703 acquiring-0.2.0/docs/architecture/decisions/0001-record-architecture-decisions.md
--rwxr-xr-x   0        0        0      666 2024-04-07 19:04:14.607704 acquiring-0.2.0/manage.py
--rw-r--r--   0        0        0     1477 2024-04-08 20:28:05.397546 acquiring-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       63 2024-04-07 19:04:14.607911 acquiring-0.2.0/requirements/base.txt
--rw-r--r--   0        0        0      136 2024-04-07 19:04:14.607992 acquiring-0.2.0/requirements/development-django.txt
--rw-r--r--   0        0        0      638 2024-04-07 19:04:14.608064 acquiring-0.2.0/requirements/development.txt
--rw-r--r--   0        0        0       74 2024-04-07 19:04:14.608127 acquiring-0.2.0/requirements/packaging.txt
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608351 acquiring-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     6057 2024-04-07 19:04:14.608500 acquiring-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0      152 2024-04-07 19:04:14.608641 acquiring-0.2.0/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608767 acquiring-0.2.0/tests/contrib/paypal/__init__.py
--rw-r--r--   0        0        0     5298 2024-04-07 19:04:14.609015 acquiring-0.2.0/tests/contrib/paypal/blocks/test_paypal_after_creating_order.py
--rw-r--r--   0        0        0     4171 2024-04-07 19:04:14.609119 acquiring-0.2.0/tests/contrib/paypal/blocks/test_paypal_create_order.py
--rw-r--r--   0        0        0     3513 2024-04-07 19:04:14.609198 acquiring-0.2.0/tests/contrib/paypal/test_live.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.609271 acquiring-0.2.0/tests/django/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-07 19:04:14.609364 acquiring-0.2.0/tests/django/factories.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.609437 acquiring-0.2.0/tests/django/repositories/__init__.py
--rw-r--r--   0        0        0     2653 2024-04-07 19:04:14.609550 acquiring-0.2.0/tests/django/repositories/test_block_event_repository.py
--rw-r--r--   0        0        0     5536 2024-04-07 19:04:14.609641 acquiring-0.2.0/tests/django/repositories/test_payment_attempt_repository.py
--rw-r--r--   0        0        0     6212 2024-04-07 19:04:14.609750 acquiring-0.2.0/tests/django/repositories/test_payment_method_repository.py
--rw-r--r--   0        0        0     2684 2024-04-07 19:04:14.609827 acquiring-0.2.0/tests/django/repositories/test_payment_operation_repository.py
--rw-r--r--   0        0        0     1249 2024-04-07 19:04:14.609909 acquiring-0.2.0/tests/django/repositories/test_transaction_repository.py
--rw-r--r--   0        0        0      517 2024-04-07 19:04:14.609998 acquiring-0.2.0/tests/django/test_migrations.py
--rw-r--r--   0        0        0      933 2024-04-07 19:04:14.610079 acquiring-0.2.0/tests/django/test_models.py
--rw-r--r--   0        0        0      174 2024-04-07 19:04:14.610144 acquiring-0.2.0/tests/django/utils.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610219 acquiring-0.2.0/tests/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610302 acquiring-0.2.0/tests/domain/blocks/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-07 19:04:14.610403 acquiring-0.2.0/tests/domain/blocks/test_wrapped_by_block_events.py
--rw-r--r--   0        0        0      739 2024-04-07 19:04:14.610475 acquiring-0.2.0/tests/domain/factories.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610549 acquiring-0.2.0/tests/domain/flows/__init__.py
--rw-r--r--   0        0        0     2177 2024-04-07 19:04:14.610626 acquiring-0.2.0/tests/domain/flows/conftest.py
--rw-r--r--   0        0        0     9427 2024-04-07 19:04:14.610753 acquiring-0.2.0/tests/domain/flows/test_after_confirm.py
--rw-r--r--   0        0        0     7953 2024-04-07 19:04:14.610850 acquiring-0.2.0/tests/domain/flows/test_after_pay.py
--rw-r--r--   0        0        0     8608 2024-04-07 19:04:14.610937 acquiring-0.2.0/tests/domain/flows/test_confirm.py
--rw-r--r--   0        0        0     1015 2024-04-07 19:04:14.611009 acquiring-0.2.0/tests/domain/flows/test_define_payment_flow.py
--rw-r--r--   0        0        0     9554 2024-04-07 19:04:14.611131 acquiring-0.2.0/tests/domain/flows/test_initialize.py
--rw-r--r--   0        0        0     6099 2024-04-07 19:04:14.611219 acquiring-0.2.0/tests/domain/flows/test_pay.py
--rw-r--r--   0        0        0    12896 2024-04-07 19:04:14.611351 acquiring-0.2.0/tests/domain/flows/test_process_actions.py
--rw-r--r--   0        0        0        0 2024-04-07 19:04:14.611424 acquiring-0.2.0/tests/domain/providers/__init__.py
--rw-r--r--   0        0        0     3443 2024-04-07 19:04:14.611516 acquiring-0.2.0/tests/domain/providers/test_wrapped_by_transaction.py
--rw-r--r--   0        0        0      416 2024-04-08 09:21:44.791998 acquiring-0.2.0/tests/tacit/README.md
--rw-r--r--   0        0        0     2526 2024-04-07 19:04:14.611710 acquiring-0.2.0/tests/tacit/test_files.py
--rw-r--r--   0        0        0      835 2024-04-07 19:04:14.611782 acquiring-0.2.0/tox.ini
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 acquiring-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2024-04-08 09:12:12.325260 acquiring-0.3.0/.adr-dir
+-rw-r--r--   0        0        0      135 2024-05-17 17:54:35.758196 acquiring-0.3.0/.env.example
+-rw-r--r--   0        0        0     3104 2024-04-29 15:06:04.143509 acquiring-0.3.0/.gitignore
+-rw-r--r--   0        0        0      176 2024-04-08 09:23:42.281005 acquiring-0.3.0/.markdownlint.json
+-rw-r--r--   0        0        0     3070 2024-05-17 17:11:58.976520 acquiring-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      438 2024-04-10 10:25:12.720112 acquiring-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1234 2024-04-12 07:54:52.741316 acquiring-0.3.0/Dockerfile
+-rw-r--r--   0        0        0     1070 2024-04-07 19:04:14.604203 acquiring-0.3.0/LICENSE
+-rw-r--r--   0        0        0      190 2024-04-09 20:23:33.063639 acquiring-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0     2071 2024-05-17 17:15:36.027748 acquiring-0.3.0/README.md
+-rw-r--r--   0        0        0      173 2024-05-17 17:20:00.067426 acquiring-0.3.0/acquiring/__init__.py
+-rw-r--r--   0        0        0      616 2024-04-23 21:15:41.949805 acquiring-0.3.0/acquiring/apps.py
+-rw-r--r--   0        0        0        0 2024-04-15 21:24:21.472983 acquiring-0.3.0/acquiring/contrib/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-12 14:53:46.923556 acquiring-0.3.0/acquiring/contrib/paypal/__init__.py
+-rw-r--r--   0        0        0     6331 2024-05-17 14:04:05.853025 acquiring-0.3.0/acquiring/contrib/paypal/adapter.py
+-rw-r--r--   0        0        0      178 2024-04-07 19:04:14.605022 acquiring-0.3.0/acquiring/contrib/paypal/blocks/__init__.py
+-rw-r--r--   0        0        0     1290 2024-05-17 14:00:23.251940 acquiring-0.3.0/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py
+-rw-r--r--   0        0        0     1973 2024-05-17 14:06:06.649977 acquiring-0.3.0/acquiring/contrib/paypal/blocks/paypal_create_order.py
+-rw-r--r--   0        0        0     1572 2024-04-07 19:04:14.605255 acquiring-0.3.0/acquiring/contrib/paypal/domain.py
+-rw-r--r--   0        0        0      700 2024-04-28 09:51:03.336728 acquiring-0.3.0/acquiring/domain/__init__.py
+-rw-r--r--   0        0        0     1685 2024-05-16 11:00:30.007935 acquiring-0.3.0/acquiring/domain/blocks.py
+-rw-r--r--   0        0        0     5936 2024-04-25 09:57:25.450086 acquiring-0.3.0/acquiring/domain/decision_logic.py
+-rw-r--r--   0        0        0      908 2024-05-16 11:00:30.009241 acquiring-0.3.0/acquiring/domain/events.py
+-rw-r--r--   0        0        0    19796 2024-05-16 11:00:30.011222 acquiring-0.3.0/acquiring/domain/flow.py
+-rw-r--r--   0        0        0     4098 2024-05-16 11:00:30.012302 acquiring-0.3.0/acquiring/domain/payments.py
+-rw-r--r--   0        0        0     1729 2024-05-17 13:51:18.159799 acquiring-0.3.0/acquiring/domain/providers.py
+-rw-r--r--   0        0        0     1265 2024-04-24 10:10:01.148240 acquiring-0.3.0/acquiring/enums.py
+-rw-r--r--   0        0        0     1632 2024-05-16 10:56:42.855367 acquiring-0.3.0/acquiring/protocols/__init__.py
+-rw-r--r--   0        0        0      245 2024-05-16 11:00:30.014551 acquiring-0.3.0/acquiring/protocols/events.py
+-rw-r--r--   0        0        0     2877 2024-05-16 11:00:30.015325 acquiring-0.3.0/acquiring/protocols/payments.py
+-rw-r--r--   0        0        0      800 2024-05-16 11:00:30.016237 acquiring-0.3.0/acquiring/protocols/providers.py
+-rw-r--r--   0        0        0     2132 2024-05-16 17:29:02.680549 acquiring-0.3.0/acquiring/protocols/storage.py
+-rw-r--r--   0        0        0      401 2024-04-23 17:52:13.537616 acquiring-0.3.0/acquiring/settings.py
+-rw-r--r--   0        0        0      211 2024-04-23 17:50:49.596526 acquiring-0.3.0/acquiring/storage/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-29 08:48:45.522667 acquiring-0.3.0/acquiring/storage/django/__init__.py
+-rw-r--r--   0        0        0     6654 2024-04-28 09:56:54.499633 acquiring-0.3.0/acquiring/storage/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:30:44.249631 acquiring-0.3.0/acquiring/storage/django/migrations/__init__.py
+-rw-r--r--   0        0        0     9179 2024-05-16 11:01:09.084686 acquiring-0.3.0/acquiring/storage/django/models.py
+-rw-r--r--   0        0        0     5131 2024-05-16 11:01:09.086009 acquiring-0.3.0/acquiring/storage/django/repositories.py
+-rw-r--r--   0        0        0     2399 2024-05-16 17:29:39.484911 acquiring-0.3.0/acquiring/storage/django/unit_of_work.py
+-rw-r--r--   0        0        0      191 2024-04-22 22:12:35.624075 acquiring-0.3.0/acquiring/storage/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2275 2024-04-22 21:40:07.708206 acquiring-0.3.0/acquiring/storage/sqlalchemy/migrations/env.py
+-rw-r--r--   0        0        0      635 2024-04-12 20:54:32.999638 acquiring-0.3.0/acquiring/storage/sqlalchemy/migrations/script.py.mako
+-rw-r--r--   0        0        0     1353 2024-04-29 13:18:37.993928 acquiring-0.3.0/acquiring/storage/sqlalchemy/migrations/versions/87b793f35b89_add_acquiring_models.py
+-rw-r--r--   0        0        0     2626 2024-05-16 11:01:09.088026 acquiring-0.3.0/acquiring/storage/sqlalchemy/models.py
+-rw-r--r--   0        0        0     1213 2024-05-16 11:01:09.088581 acquiring-0.3.0/acquiring/storage/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0     2148 2024-05-16 17:30:22.205942 acquiring-0.3.0/acquiring/storage/sqlalchemy/unit_of_work.py
+-rw-r--r--   0        0        0      358 2024-04-15 21:24:04.465544 acquiring-0.3.0/acquiring/utils.py
+-rw-r--r--   0        0        0     3683 2024-04-23 17:33:13.035493 acquiring-0.3.0/alembic.ini
+-rw-r--r--   0        0        0      712 2024-04-29 15:02:03.580627 acquiring-0.3.0/docker-compose.yaml
+-rw-r--r--   0        0        0      394 2024-04-10 10:23:35.861556 acquiring-0.3.0/docs/Dockerfile
+-rw-r--r--   0        0        0      483 2024-04-08 09:12:13.455703 acquiring-0.3.0/docs/architecture/decisions/0001-record-architecture-decisions.md
+-rw-r--r--   0        0        0     1395 2024-04-10 14:01:00.812132 acquiring-0.3.0/docs/architecture/decisions/0002-use-tacit-tests.md
+-rw-r--r--   0        0        0     1641 2024-04-10 18:18:42.875494 acquiring-0.3.0/docs/architecture/decisions/0003-documentation-is-code.md
+-rw-r--r--   0        0        0     1012 2024-04-10 21:28:47.193576 acquiring-0.3.0/docs/architecture/decisions/0004-reduce-doctests-to-a-minimum.md
+-rw-r--r--   0        0        0     3453 2024-04-13 18:02:53.958745 acquiring-0.3.0/docs/architecture/decisions/0005-maybe-functions-considered-harmful.md
+-rw-r--r--   0        0        0     2647 2024-04-14 21:02:55.401009 acquiring-0.3.0/docs/architecture/decisions/0006-use-import-module-more-often-than-from-module-import.md
+-rw-r--r--   0        0        0      647 2024-04-18 11:37:03.298067 acquiring-0.3.0/docs/architecture/decisions/0007-type-sparingly-but-with-confidence.md
+-rw-r--r--   0        0        0     2200 2024-04-24 10:56:33.838062 acquiring-0.3.0/docs/architecture/decisions/0008-domain-logic-happens-in-native-python.md
+-rw-r--r--   0        0        0     1345 2024-04-25 10:17:21.246825 acquiring-0.3.0/docs/architecture/decisions/0009-do-not-use-if-type-checking.md
+-rw-r--r--   0        0        0     1102 2024-04-28 21:12:22.951710 acquiring-0.3.0/docs/architecture/decisions/0010-exceptions-can-express-domain-concepts-too.md
+-rw-r--r--   0        0        0      988 2024-05-06 16:10:08.334738 acquiring-0.3.0/docs/architecture/decisions/0011-worse-is-better.md
+-rw-r--r--   0        0        0      416 2024-05-15 16:50:09.923734 acquiring-0.3.0/docs/architecture/decisions/0012-usage-driven-design.md
+-rw-r--r--   0        0        0     1590 2024-04-14 21:14:41.043915 acquiring-0.3.0/docs/architecture/index.md
+-rw-r--r--   0        0        0      751 2024-04-10 18:23:18.673594 acquiring-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      103 2024-04-10 18:23:18.673084 acquiring-0.3.0/docs/requirements.txt
+-rwxr-xr-x   0        0        0      666 2024-04-07 19:04:14.607704 acquiring-0.3.0/manage.py
+-rw-r--r--   0        0        0      164 2024-04-16 14:08:55.167288 acquiring-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0     1845 2024-05-17 17:54:22.507779 acquiring-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      158 2024-04-12 14:51:26.788691 acquiring-0.3.0/requirements/base.txt
+-rw-r--r--   0        0        0      136 2024-04-07 19:04:14.607992 acquiring-0.3.0/requirements/development-django.txt
+-rw-r--r--   0        0        0       69 2024-04-12 09:27:58.484325 acquiring-0.3.0/requirements/development-sqlalchemy.txt
+-rw-r--r--   0        0        0      634 2024-04-15 21:31:52.585788 acquiring-0.3.0/requirements/development.txt
+-rw-r--r--   0        0        0       74 2024-04-07 19:04:14.608127 acquiring-0.3.0/requirements/packaging.txt
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608351 acquiring-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     9516 2024-05-17 13:51:38.601641 acquiring-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      100 2024-04-12 14:53:46.923656 acquiring-0.3.0/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.608767 acquiring-0.3.0/tests/contrib/paypal/__init__.py
+-rw-r--r--   0        0        0     5882 2024-05-17 14:34:25.316375 acquiring-0.3.0/tests/contrib/paypal/blocks/test_paypal_after_creating_order.py
+-rw-r--r--   0        0        0     4834 2024-05-17 14:34:55.746504 acquiring-0.3.0/tests/contrib/paypal/blocks/test_paypal_create_order.py
+-rw-r--r--   0        0        0     2836 2024-05-17 14:06:52.895692 acquiring-0.3.0/tests/contrib/paypal/test_adapter.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610219 acquiring-0.3.0/tests/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610302 acquiring-0.3.0/tests/domain/blocks/__init__.py
+-rw-r--r--   0        0        0     2677 2024-05-17 14:07:50.348644 acquiring-0.3.0/tests/domain/blocks/test_wrapped_by_block_events.py
+-rw-r--r--   0        0        0      845 2024-05-16 11:01:09.096979 acquiring-0.3.0/tests/domain/factories.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.610549 acquiring-0.3.0/tests/domain/flows/__init__.py
+-rw-r--r--   0        0        0     1898 2024-05-16 11:01:09.097657 acquiring-0.3.0/tests/domain/flows/conftest.py
+-rw-r--r--   0        0        0    11098 2024-05-17 14:11:18.544860 acquiring-0.3.0/tests/domain/flows/test_after_confirm.py
+-rw-r--r--   0        0        0     9633 2024-05-17 14:11:48.145068 acquiring-0.3.0/tests/domain/flows/test_after_pay.py
+-rw-r--r--   0        0        0    10288 2024-05-17 14:12:39.949245 acquiring-0.3.0/tests/domain/flows/test_confirm.py
+-rw-r--r--   0        0        0     1753 2024-05-17 14:12:44.158593 acquiring-0.3.0/tests/domain/flows/test_define_payment_flow.py
+-rw-r--r--   0        0        0    11639 2024-05-17 14:22:06.486358 acquiring-0.3.0/tests/domain/flows/test_initialize.py
+-rw-r--r--   0        0        0     7217 2024-05-17 14:13:44.638667 acquiring-0.3.0/tests/domain/flows/test_pay.py
+-rw-r--r--   0        0        0    15642 2024-05-17 14:14:33.317947 acquiring-0.3.0/tests/domain/flows/test_process_actions.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:04:14.611424 acquiring-0.3.0/tests/domain/providers/__init__.py
+-rw-r--r--   0        0        0     3229 2024-05-17 14:34:04.886045 acquiring-0.3.0/tests/domain/providers/test_wrapped_by_transaction.py
+-rw-r--r--   0        0        0    41792 2024-05-16 11:01:09.106867 acquiring-0.3.0/tests/domain/test_decision_logic.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:19:52.684632 acquiring-0.3.0/tests/storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:20:06.748701 acquiring-0.3.0/tests/storage/django/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-16 11:01:09.108329 acquiring-0.3.0/tests/storage/django/factories.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:18:56.952489 acquiring-0.3.0/tests/storage/django/repositories/__init__.py
+-rw-r--r--   0        0        0     2589 2024-05-16 11:01:09.109784 acquiring-0.3.0/tests/storage/django/repositories/test_block_event_repository.py
+-rw-r--r--   0        0        0     3137 2024-05-16 11:01:09.110797 acquiring-0.3.0/tests/storage/django/repositories/test_payment_method_repository.py
+-rw-r--r--   0        0        0     2598 2024-05-16 11:01:09.111539 acquiring-0.3.0/tests/storage/django/repositories/test_payment_operation_repository.py
+-rw-r--r--   0        0        0     2430 2024-05-16 11:01:09.112252 acquiring-0.3.0/tests/storage/django/repositories/test_token_repository.py
+-rw-r--r--   0        0        0     1270 2024-05-16 11:01:09.112889 acquiring-0.3.0/tests/storage/django/repositories/test_transaction_repository.py
+-rw-r--r--   0        0        0     9705 2024-05-16 17:38:37.202961 acquiring-0.3.0/tests/storage/django/repositories/test_unit_of_work.py
+-rw-r--r--   0        0        0      518 2024-05-16 11:01:09.114699 acquiring-0.3.0/tests/storage/django/test_migrations.py
+-rw-r--r--   0        0        0      951 2024-04-22 22:12:35.473250 acquiring-0.3.0/tests/storage/django/test_models.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:27:27.777130 acquiring-0.3.0/tests/storage/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2049 2024-05-16 11:00:30.051582 acquiring-0.3.0/tests/storage/sqlalchemy/conftest.py
+-rw-r--r--   0        0        0      873 2024-05-16 11:01:09.117077 acquiring-0.3.0/tests/storage/sqlalchemy/factories.py
+-rw-r--r--   0        0        0        0 2024-04-12 13:27:36.895251 acquiring-0.3.0/tests/storage/sqlalchemy/repositories/__init__.py
+-rw-r--r--   0        0        0     2432 2024-05-16 11:01:09.118294 acquiring-0.3.0/tests/storage/sqlalchemy/repositories/test_payment_method_repository.py
+-rw-r--r--   0        0        0    10842 2024-05-16 17:26:43.644531 acquiring-0.3.0/tests/storage/sqlalchemy/repositories/test_unit_of_work.py
+-rw-r--r--   0        0        0       32 2024-04-13 21:49:54.429636 acquiring-0.3.0/tests/storage/sqlalchemy/test_migrations.py
+-rw-r--r--   0        0        0      634 2024-04-25 08:54:50.066518 acquiring-0.3.0/tests/storage/test_tacit.py
+-rw-r--r--   0        0        0      370 2024-05-16 11:01:09.120540 acquiring-0.3.0/tests/storage/utils.py
+-rw-r--r--   0        0        0     2511 2024-05-16 11:00:30.057049 acquiring-0.3.0/tests/tacit/test_files.py
+-rw-r--r--   0        0        0      835 2024-04-07 19:04:14.611782 acquiring-0.3.0/tox.ini
+-rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 acquiring-0.3.0/PKG-INFO
```

### Comparing `acquiring-0.2.0/.gitignore` & `acquiring-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `acquiring-0.2.0/.pre-commit-config.yaml` & `acquiring-0.3.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-exclude: 'migrations/'
+exclude: '(migrations|decisions)/'
 repos:
 -   repo: https://github.com/hija/clean-dotenv
-    rev: v0.0.6
+    rev: v0.0.7
     hooks:
     -   id: clean-dotenv
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.6.0
     hooks:
     -   id: check-added-large-files
     -   id: check-ast
@@ -22,29 +22,29 @@
     -   id: trailing-whitespace
 -   repo: https://github.com/PyCQA/bandit
     rev: 1.7.8
     hooks:
     -   id: bandit
         args: ["-c", "pyproject.toml"]
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.4
     hooks:
     -   id: ruff
         args: [ --fix ]
 -   repo: https://github.com/jorisroovers/gitlint
     rev: v0.19.1
     hooks:
       - id: gitlint
 -   repo: https://github.com/adrienverge/yamllint
     rev: v1.35.1
     hooks:
       - id: yamllint
         args: [-d, "{extends: relaxed, rules: {line-length: {max: 120}}}"]
 -   repo: https://github.com/ambv/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
         args: [-l120]
 -   repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
       - id: isort
@@ -53,24 +53,29 @@
 -   repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
     hooks:
     -   id: python-check-blanket-noqa
     -   id: python-check-blanket-type-ignore
     -   id: python-no-eval
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-requests]
         args: ["--python-version", "3.12", --ignore-missing-imports, --disallow-any-explicit, --disallow-untyped-defs, --warn-redundant-casts, --warn-unused-ignores, --warn-unreachable, --strict-equality, --check-untyped-defs]
         exclude: "(manage.py)"
 -   repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
-    -  id: codespell
+    -   id: codespell
+-   repo: https://github.com/econchick/interrogate
+    rev: 1.7.0  # or master if you're bold
+    hooks:
+    -   id: interrogate
+        pass_filenames: false  # needed if excluding files with pyproject.toml or setup.cfg
 # -   repo: https://github.com/Yelp/detect-secrets
 #     rev: v1.4.0
 #     hooks:
 #     -   id: detect-secrets
 #         args: ['--baseline', '.secrets.baseline']
 # -   repo: https://github.com/mgedmin/check-manifest
 #     rev: "0.49"
@@ -85,10 +90,10 @@
     hooks:
     -   id: add-pre-commit-config-trailer
 -   repo: https://github.com/Mateusz-Grzelinski/actionlint-py
     rev: v1.6.27.13
     hooks:
     -   id: actionlint
 -   repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.39.0
+    rev: v0.40.0
     hooks:
     -   id: markdownlint
```

### Comparing `acquiring-0.2.0/Dockerfile` & `acquiring-0.3.0/Dockerfile`

 * *Files 25% similar despite different names*

```diff
@@ -9,16 +9,31 @@
 WORKDIR /code
 COPY requirements/ /code/requirements/
 
 # Check if DJANGO_VERSION is provided,
 # And install Django, the shared dependencies and requirements/$ENVIRONMENT-django.txt
 # Otherwise install just the shared dependencies
 ARG DJANGO_VERSION=""
+ARG SQLALCHEMY_VERSION=""
 ARG ENVIRONMENT
-RUN if [ ! -z "$DJANGO_VERSION" ]; then pip install Django==$DJANGO_VERSION && pip install -r requirements/${ENVIRONMENT}-django.txt; else pip install -r requirements/$ENVIRONMENT.txt; fi
+
+# Install Django, SQLAlchemy, and other dependencies
+RUN INSTALL_CMD=""; \
+    if [ ! -z "$DJANGO_VERSION" ]; then \
+        INSTALL_CMD="${INSTALL_CMD} Django==$DJANGO_VERSION -r requirements/${ENVIRONMENT}-django.txt "; \
+    fi; \
+    if [ ! -z "$SQLALCHEMY_VERSION" ]; then \
+        INSTALL_CMD="${INSTALL_CMD} SQLAlchemy==$SQLALCHEMY_VERSION -r requirements/${ENVIRONMENT}-sqlalchemy.txt "; \
+    fi; \
+    if [ ! -z "$INSTALL_CMD" ]; then \
+        pip install $INSTALL_CMD; \
+    else \
+        pip install -r requirements/$ENVIRONMENT.txt; \
+    fi;
+
 
 # Copy the acquiring package and the test project into the container
 COPY . /code/
 
 # Expose the port Django will run on
 EXPOSE 8000
```

### Comparing `acquiring-0.2.0/LICENSE` & `acquiring-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acquiring-0.2.0/README.md` & `acquiring-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # Acquiring
 
 Payment Orchestration Library for Python.
 
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+
+
 ## Overview
 
 Acquiring aspires to be a flexible and effective toolkit for building applications that handle money.
+The word "acquiring" is the industry term that means collecting and processing payments from customers.
 
 Some reasons you might want to check it out:
 
 - Stable interface via single PaymentFlow class.
 - Flexible internals that can be customized for any payment method, existing AND non-existing.
 - Platform agnostic (really!), meant to be plugged into your existing Django project easily.
 - Support for all database engines under the Django umbrella.
```

### Comparing `acquiring-0.2.0/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py` & `acquiring-0.3.0/acquiring/contrib/paypal/blocks/paypal_after_creating_order.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 
 from acquiring import domain, enums, protocols
 from acquiring.contrib import paypal
 
 
 @dataclass
 class PayPalAfterCreatingOrder:
-    block_event_repository: protocols.AbstractRepository
-    transaction_repository: protocols.AbstractRepository
 
     @domain.wrapped_by_block_events
     def run(
         self,
-        payment_method: "protocols.AbstractPaymentMethod",
+        unit_of_work: "protocols.UnitOfWork",
+        payment_method: "protocols.PaymentMethod",
         webhook_data: paypal.domain.PayPalWebhookData,
-    ) -> "protocols.AbstractBlockResponse":
-        self.transaction_repository.add(
-            domain.Transaction(
-                external_id=webhook_data.id,
-                timestamp=webhook_data.create_time,
-                raw_data=webhook_data.raw_data,
-                provider_name="paypal",
-                payment_method_id=payment_method.id,
+    ) -> "protocols.BlockResponse":
+        with unit_of_work as uow:
+            uow.transactions.add(
+                domain.Transaction(
+                    external_id=webhook_data.id,
+                    timestamp=webhook_data.create_time,
+                    raw_data=webhook_data.raw_data,
+                    provider_name="paypal",
+                    payment_method_id=payment_method.id,
+                )
             )
-        )
+            uow.commit()
 
         if webhook_data.event_type == "CHECKOUT.ORDER.APPROVED":
             return domain.BlockResponse(
                 status=enums.OperationStatusEnum.COMPLETED,
                 actions=[],
                 error_message=None,
             )
```

### Comparing `acquiring-0.2.0/acquiring/contrib/paypal/blocks/paypal_create_order.py` & `acquiring-0.3.0/acquiring/contrib/paypal/blocks/paypal_create_order.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 from ..adapter import PayPalAdapter
 from ..domain import Amount, Order, OrderIntentEnum, PayPalStatusEnum, PurchaseUnit
 
 
 @dataclass
 class PayPalCreateOrder:
     adapter: PayPalAdapter
-    block_event_repository: protocols.AbstractRepository
 
     @domain.wrapped_by_block_events
     def run(
-        self, payment_method: "protocols.AbstractPaymentMethod", *args: Sequence, **kwargs: dict
-    ) -> "protocols.AbstractBlockResponse":
+        self,
+        unit_of_work: "protocols.UnitOfWork",
+        payment_method: "protocols.PaymentMethod",
+        *args: Sequence,
+        **kwargs: dict,
+    ) -> "protocols.BlockResponse":
         external_id = uuid.uuid4()
 
         items = payment_method.payment_attempt.items
         order = Order(
             intent=OrderIntentEnum.CAPTURE,
             purchase_units=[
                 PurchaseUnit(
@@ -30,14 +33,15 @@
                         value=str(item.quantity),
                     ),
                 )
                 for item in items
             ],
         )
         response = self.adapter.create_order(
+            unit_of_work=unit_of_work,
             payment_method=payment_method,
             request_id=external_id,
             order=order,
         )
 
         if response.status == PayPalStatusEnum.FAILED:
             return domain.BlockResponse(
```

### Comparing `acquiring-0.2.0/acquiring/contrib/paypal/domain.py` & `acquiring-0.3.0/acquiring/contrib/paypal/domain.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.2.0/acquiring/domain/__init__.py` & `acquiring-0.3.0/acquiring/domain/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 from .blocks import BlockResponse, wrapped_by_block_events
 from .events import BlockEvent
 from .flow import PaymentFlow
 from .payments import (
     DraftItem,
     DraftPaymentAttempt,
     DraftPaymentMethod,
+    DraftToken,
     Item,
     PaymentAttempt,
     PaymentMethod,
     PaymentOperation,
     Token,
 )
 from .providers import Transaction, wrapped_by_transaction
 
 __all__ = [
     "BlockEvent",
     "BlockResponse",
     "DraftItem",
     "DraftPaymentAttempt",
     "DraftPaymentMethod",
+    "DraftToken",
     "Item",
     "PaymentAttempt",
     "PaymentFlow",
     "PaymentMethod",
     "PaymentOperation",
     "Token",
     "Transaction",
     "wrapped_by_block_events",
     "wrapped_by_transaction",
 ]
-
-
-assert __all__ == sorted(__all__), sorted(__all__)
```

### Comparing `acquiring-0.2.0/acquiring/domain/flow.py` & `acquiring-0.3.0/acquiring/domain/flow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import functools
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Callable, Optional, Sequence
+from typing import Callable, Optional, Sequence
 
 import acquiring.domain.decision_logic as dl
-from acquiring import domain
+from acquiring import domain, protocols
 from acquiring.enums import OperationStatusEnum, OperationTypeEnum
 
-if TYPE_CHECKING:
-    from acquiring import protocols
-
 
 def payment_operation_type(  # type:ignore[misc]
-    function: Callable[..., "protocols.AbstractOperationResponse"]
-) -> Callable[..., "protocols.AbstractOperationResponse"]:
+    function: Callable[..., "protocols.OperationResponse"]
+) -> Callable[..., "protocols.OperationResponse"]:
     """
     This decorator verifies that the name of this function belongs to one of the OperationTypeEnums
 
     >>> def initialize(): pass
     >>> payment_operation_type(initialize)()
     >>> def bad_name(): pass
     >>> payment_operation_type(bad_name)()
@@ -36,146 +33,159 @@
     >>> payment_operation_type(__pay)()
     """
 
     @functools.wraps(function)
     def wrapper(
         *args: Sequence,
         **kwargs: dict,
-    ) -> "protocols.AbstractOperationResponse":
+    ) -> "protocols.OperationResponse":
         if function.__name__ not in OperationTypeEnum:
 
             # Private methods that start with double _ and have a name that belongs to enum are also allowed
             if function.__name__.startswith("__") and function.__name__[2:] in OperationTypeEnum:
                 return function(*args, **kwargs)
 
             raise TypeError("This function cannot be a payment type")
 
         return function(*args, **kwargs)
 
     return wrapper
 
 
 def refresh_payment_method(  # type:ignore[misc]
-    function: Callable[..., "protocols.AbstractOperationResponse"]
-) -> Callable[..., "protocols.AbstractOperationResponse"]:
+    function: Callable[..., "protocols.OperationResponse"]
+) -> Callable[..., "protocols.OperationResponse"]:
     """
     Refresh the payment from the database, or force an early failed OperationResponse otherwise.
     """
 
     @functools.wraps(function)
     def wrapper(
-        self: "protocols.AbstractPaymentFlow",
-        payment_method: "protocols.AbstractPaymentMethod",
+        self: "protocols.PaymentFlow",
+        payment_method: "protocols.PaymentMethod",
         *args: Sequence,
         **kwargs: dict,
-    ) -> "protocols.AbstractOperationResponse":
+    ) -> "protocols.OperationResponse":
         try:
-            payment_method = self.payment_method_repository.get(id=payment_method.id)
+            with self.unit_of_work as uow:
+                payment_method = uow.payment_methods.get(id=payment_method.id)
         except domain.PaymentMethod.DoesNotExist:
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=None,
                 error_message="PaymentMethod not found",
                 type=OperationTypeEnum(function.__name__),  # already valid thanks to @payment_operation_type
             )
         return function(self, payment_method, *args, **kwargs)
 
     return wrapper
 
 
 @dataclass
 class OperationResponse:
+    """Represents the outcome of a PaymentFlow operation type method execution"""
+
     status: OperationStatusEnum
-    payment_method: Optional["protocols.AbstractPaymentMethod"]
+    payment_method: Optional["protocols.PaymentMethod"]
     type: OperationTypeEnum
     error_message: Optional[str] = None
     actions: list[dict] = field(default_factory=list)
 
 
 # TODO Decorate this class to ensure that all payment_operation_types are implemented as methods
 @dataclass
 class PaymentFlow:
-    payment_method_repository: "protocols.AbstractRepository"
-    payment_operation_repository: "protocols.AbstractRepository"
+    """
+    Context class that defines what's common across all Payment Methods and their execution.
+
+    What's specific to each payment method is implemented inside each one of the block(s).
+    """
+
+    unit_of_work: "protocols.UnitOfWork"
 
-    initialize_block: Optional["protocols.AbstractBlock"]
-    process_action_block: Optional["protocols.AbstractBlock"]
+    initialize_block: Optional["protocols.Block"]
+    process_action_block: Optional["protocols.Block"]
 
-    pay_blocks: list["protocols.AbstractBlock"]
-    after_pay_blocks: list["protocols.AbstractBlock"]
+    pay_blocks: list["protocols.Block"]
+    after_pay_blocks: list["protocols.Block"]
 
-    confirm_block: Optional["protocols.AbstractBlock"]
-    after_confirm_blocks: list["protocols.AbstractBlock"]
+    confirm_block: Optional["protocols.Block"]
+    after_confirm_blocks: list["protocols.Block"]
 
     @payment_operation_type
     @refresh_payment_method
-    def initialize(self, payment_method: "protocols.AbstractPaymentMethod") -> "protocols.AbstractOperationResponse":
+    def initialize(self, payment_method: "protocols.PaymentMethod") -> "protocols.OperationResponse":
         # Verify that the payment can go through this operation type
         if not dl.can_initialize(payment_method):
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=None,
                 error_message="PaymentMethod cannot go through this operation",
                 type=OperationTypeEnum.INITIALIZE,
             )
 
         # Create Started PaymentOperation
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.INITIALIZE,
-            status=OperationStatusEnum.STARTED,
-        )
-
-        # Run Operation Block if it exists
-        if self.initialize_block is None:
-            self.payment_operation_repository.add(
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
                 payment_method=payment_method,
                 type=OperationTypeEnum.INITIALIZE,
-                status=OperationStatusEnum.NOT_PERFORMED,
+                status=OperationStatusEnum.STARTED,
             )
+
+        # Run Operation Block if it exists
+        if self.initialize_block is None:
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.INITIALIZE,
+                    status=OperationStatusEnum.NOT_PERFORMED,
+                )
             return self.__pay(payment_method)
 
-        block_response = self.initialize_block.run(payment_method=payment_method)
+        block_response = self.initialize_block.run(unit_of_work=self.unit_of_work, payment_method=payment_method)
 
         # Validate that status is one of the expected ones
         if block_response.status not in [
             OperationStatusEnum.COMPLETED,
             OperationStatusEnum.FAILED,
             OperationStatusEnum.REQUIRES_ACTION,
         ]:
-            self.payment_operation_repository.add(
-                payment_method=payment_method,
-                type=OperationTypeEnum.INITIALIZE,  # TODO Refer to function name rather than explicit input in all cases
-                status=OperationStatusEnum.FAILED,
-            )
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.INITIALIZE,  # TODO Refer to function name rather than explicit input in all cases
+                    status=OperationStatusEnum.FAILED,
+                )
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=payment_method,
                 type=OperationTypeEnum.INITIALIZE,  # TODO Refer to function name rather than explicit input in all cases
                 error_message=f"Invalid status {block_response.status}",
             )
         if block_response.status == OperationStatusEnum.REQUIRES_ACTION and not block_response.actions:
-            self.payment_operation_repository.add(
-                payment_method=payment_method,
-                type=OperationTypeEnum.INITIALIZE,
-                status=OperationStatusEnum.FAILED,
-            )
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.INITIALIZE,
+                    status=OperationStatusEnum.FAILED,
+                )
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=payment_method,
                 type=OperationTypeEnum.INITIALIZE,
                 error_message="Status is require actions, but no actions were provided",
             )
 
         # Create PaymentOperation with the outcome
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.INITIALIZE,
-            status=block_response.status,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.INITIALIZE,
+                status=block_response.status,
+            )
 
         # Return Response
         if block_response.status == OperationStatusEnum.COMPLETED:
             return self.__pay(payment_method)
 
         return OperationResponse(
             status=block_response.status,
@@ -183,102 +193,109 @@
             payment_method=payment_method,
             type=OperationTypeEnum.INITIALIZE,
         )
 
     @payment_operation_type
     @refresh_payment_method
     def process_action(
-        self, payment_method: "protocols.AbstractPaymentMethod", action_data: dict
-    ) -> "protocols.AbstractOperationResponse":
+        self, payment_method: "protocols.PaymentMethod", action_data: dict
+    ) -> "protocols.OperationResponse":
         # Verify that the payment can go through this operation type
 
         if not dl.can_process_action(payment_method):
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=None,
                 error_message="PaymentMethod cannot go through this operation",
                 type=OperationTypeEnum.PROCESS_ACTION,
             )
 
         # Create Started PaymentOperation
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.PROCESS_ACTION,
-            status=OperationStatusEnum.STARTED,
-        )
-
-        if self.process_action_block is None:
-            self.payment_operation_repository.add(
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
                 payment_method=payment_method,
                 type=OperationTypeEnum.PROCESS_ACTION,
-                status=OperationStatusEnum.NOT_PERFORMED,
+                status=OperationStatusEnum.STARTED,
             )
+
+        if self.process_action_block is None:
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.PROCESS_ACTION,
+                    status=OperationStatusEnum.NOT_PERFORMED,
+                )
             return OperationResponse(
                 status=OperationStatusEnum.NOT_PERFORMED,
                 payment_method=payment_method,
                 type=OperationTypeEnum.PROCESS_ACTION,
                 error_message="PaymentFlow does not include a block for this operation type",
             )
 
         # Run Operation Block
-        block_response = self.process_action_block.run(payment_method=payment_method, action_data=action_data)
+        block_response = self.process_action_block.run(
+            unit_of_work=self.unit_of_work, payment_method=payment_method, action_data=action_data
+        )
 
         # Validate that status is one of the expected ones
         if block_response.status not in [
             OperationStatusEnum.COMPLETED,
             OperationStatusEnum.FAILED,
         ]:
-            self.payment_operation_repository.add(
-                payment_method=payment_method,
-                type=OperationTypeEnum.PROCESS_ACTION,
-                status=OperationStatusEnum.FAILED,
-            )
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.PROCESS_ACTION,
+                    status=OperationStatusEnum.FAILED,
+                )
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=payment_method,
                 type=OperationTypeEnum.PROCESS_ACTION,
                 error_message=f"Invalid status {block_response.status}",
             )
 
         # Create PaymentOperation with the outcome
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.PROCESS_ACTION,
-            status=block_response.status,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.PROCESS_ACTION,
+                status=block_response.status,
+            )
 
         # Return Response
         if block_response.status == OperationStatusEnum.COMPLETED:
             return self.__pay(payment_method)
 
         return OperationResponse(
             status=block_response.status,
             actions=block_response.actions,
             payment_method=payment_method,
             type=OperationTypeEnum.PROCESS_ACTION,
         )
 
     @payment_operation_type
-    def __pay(self, payment_method: "protocols.AbstractPaymentMethod") -> "protocols.AbstractOperationResponse":
+    def __pay(self, payment_method: "protocols.PaymentMethod") -> "protocols.OperationResponse":
         # No need to refresh from DB
 
         # No need to verify if payment can go through a private method
 
         # Create Started PaymentOperation
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.PAY,
-            status=OperationStatusEnum.STARTED,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.PAY,
+                status=OperationStatusEnum.STARTED,
+            )
 
         # Run Operation Blocks
         responses = []
         actions = []
         for block in self.pay_blocks:
-            response = block.run(payment_method)
+            response = block.run(unit_of_work=self.unit_of_work, payment_method=payment_method)
             responses.append(response)
             actions += response.actions
 
         has_completed = all([response.status == OperationStatusEnum.COMPLETED for response in responses])
 
         is_pending = any([response.status == OperationStatusEnum.PENDING for response in responses])
 
@@ -287,192 +304,207 @@
         elif not has_completed and is_pending:
             status = OperationStatusEnum.PENDING
         else:
             # TODO Allow for the possibility of any block forcing the response to be failed
             status = OperationStatusEnum.FAILED
 
         # Create PaymentOperation with the outcome
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.PAY,
-            status=status,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.PAY,
+                status=status,
+            )
 
         # Return Response
         return OperationResponse(
             status=status,
             payment_method=payment_method,
             actions=actions,
             type=OperationTypeEnum.PAY,
             error_message=", ".join(
                 [response.error_message for response in responses if response.error_message is not None]
             ),
         )
 
     @payment_operation_type
     @refresh_payment_method
-    def after_pay(self, payment_method: "protocols.AbstractPaymentMethod") -> "protocols.AbstractOperationResponse":
+    def after_pay(self, payment_method: "protocols.PaymentMethod") -> "protocols.OperationResponse":
         # Verify that the payment can go through this operation type
         if not dl.can_after_pay(payment_method):
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=None,
                 error_message="PaymentMethod cannot go through this operation",
                 type=OperationTypeEnum.AFTER_PAY,
             )
 
         # Create Started PaymentOperation
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.AFTER_PAY,
-            status=OperationStatusEnum.STARTED,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.AFTER_PAY,
+                status=OperationStatusEnum.STARTED,
+            )
 
         # Run Operation Blocks
-        responses = [block.run(payment_method) for block in self.after_pay_blocks]
+        responses = [
+            block.run(unit_of_work=self.unit_of_work, payment_method=payment_method) for block in self.after_pay_blocks
+        ]
 
         has_completed = all([response.status == OperationStatusEnum.COMPLETED for response in responses])
 
         if not has_completed:
-            self.payment_operation_repository.add(
-                payment_method=payment_method,
-                type=OperationTypeEnum.AFTER_PAY,
-                status=OperationStatusEnum.FAILED,
-            )
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.AFTER_PAY,
+                    status=OperationStatusEnum.FAILED,
+                )
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=payment_method,
                 type=OperationTypeEnum.AFTER_PAY,
             )
 
         status = OperationStatusEnum.COMPLETED if has_completed else OperationStatusEnum.FAILED
 
         # Create PaymentOperation with the outcome
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.AFTER_PAY,
-            status=status,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.AFTER_PAY,
+                status=status,
+            )
 
         # Return Response
         return OperationResponse(
             status=status,
             payment_method=payment_method,
             type=OperationTypeEnum.AFTER_PAY,
         )
 
     @payment_operation_type
     @refresh_payment_method
-    def confirm(self, payment_method: "protocols.AbstractPaymentMethod") -> "protocols.AbstractOperationResponse":
+    def confirm(self, payment_method: "protocols.PaymentMethod") -> "protocols.OperationResponse":
         # Verify that the payment can go through this operation type
         if not dl.can_confirm(payment_method):
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=None,
                 error_message="PaymentMethod cannot go through this operation",
                 type=OperationTypeEnum.CONFIRM,
             )
 
         # Create Started PaymentOperation
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.CONFIRM,
-            status=OperationStatusEnum.STARTED,
-        )
-
-        # Run Operation Blocks
-        if self.confirm_block is None:
-            self.payment_operation_repository.add(
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
                 payment_method=payment_method,
                 type=OperationTypeEnum.CONFIRM,
-                status=OperationStatusEnum.NOT_PERFORMED,
+                status=OperationStatusEnum.STARTED,
             )
+
+        # Run Operation Blocks
+        if self.confirm_block is None:
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.CONFIRM,
+                    status=OperationStatusEnum.NOT_PERFORMED,
+                )
             return OperationResponse(
                 status=OperationStatusEnum.NOT_PERFORMED,
                 payment_method=payment_method,
                 type=OperationTypeEnum.CONFIRM,
                 error_message="PaymentFlow does not include a block for this operation type",
             )
 
         # Run Operation Block
-        block_response = self.confirm_block.run(payment_method=payment_method)
+        block_response = self.confirm_block.run(unit_of_work=self.unit_of_work, payment_method=payment_method)
 
         # Validate that status is one of the expected ones
         if block_response.status not in [
             OperationStatusEnum.COMPLETED,
             OperationStatusEnum.FAILED,
             OperationStatusEnum.PENDING,
         ]:
-            self.payment_operation_repository.add(
-                payment_method=payment_method,
-                type=OperationTypeEnum.CONFIRM,
-                status=OperationStatusEnum.FAILED,
-            )
+            with self.unit_of_work as uow:
+                uow.payment_operations.add(
+                    payment_method=payment_method,
+                    type=OperationTypeEnum.CONFIRM,
+                    status=OperationStatusEnum.FAILED,
+                )
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=payment_method,
                 type=OperationTypeEnum.CONFIRM,
                 error_message=f"Invalid status {block_response.status}",
             )
 
         # Create PaymentOperation with the outcome
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.CONFIRM,
-            status=block_response.status,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.CONFIRM,
+                status=block_response.status,
+            )
 
         # Return Response
         return OperationResponse(
             status=block_response.status,
             payment_method=payment_method,
             type=OperationTypeEnum.CONFIRM,
             error_message=block_response.error_message,
         )
 
     @payment_operation_type
     @refresh_payment_method
-    def after_confirm(self, payment_method: "protocols.AbstractPaymentMethod") -> "protocols.AbstractOperationResponse":
+    def after_confirm(self, payment_method: "protocols.PaymentMethod") -> "protocols.OperationResponse":
         # Verify that the payment can go through this operation type
         if not dl.can_after_confirm(payment_method):
             return OperationResponse(
                 status=OperationStatusEnum.FAILED,
                 payment_method=None,
                 error_message="PaymentMethod cannot go through this operation",
                 type=OperationTypeEnum.AFTER_CONFIRM,
             )
 
         # Create Started PaymentOperation
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.AFTER_CONFIRM,
-            status=OperationStatusEnum.STARTED,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.AFTER_CONFIRM,
+                status=OperationStatusEnum.STARTED,
+            )
 
         # Run Operation Blocks
-        responses = [block.run(payment_method) for block in self.after_confirm_blocks]
+        responses = [
+            block.run(unit_of_work=self.unit_of_work, payment_method=payment_method)
+            for block in self.after_confirm_blocks
+        ]
 
         has_completed = all([response.status == OperationStatusEnum.COMPLETED for response in responses])
 
         is_pending = any([response.status == OperationStatusEnum.PENDING for response in responses])
 
         if has_completed:
             status = OperationStatusEnum.COMPLETED
         elif not has_completed and is_pending:
             status = OperationStatusEnum.PENDING
         else:
             # TODO Allow for the possibility of any block forcing the response to be failed
             status = OperationStatusEnum.FAILED
 
         # Create PaymentOperation with the outcome
-        self.payment_operation_repository.add(
-            payment_method=payment_method,
-            type=OperationTypeEnum.AFTER_CONFIRM,
-            status=status,
-        )
+        with self.unit_of_work as uow:
+            uow.payment_operations.add(
+                payment_method=payment_method,
+                type=OperationTypeEnum.AFTER_CONFIRM,
+                status=status,
+            )
 
         # Return Response
         return OperationResponse(
             status=status,
             payment_method=payment_method,
             type=OperationTypeEnum.AFTER_CONFIRM,
             error_message=", ".join(
```

### Comparing `acquiring-0.2.0/acquiring/domain/payments.py` & `acquiring-0.3.0/acquiring/protocols/payments.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,125 @@
-from dataclasses import dataclass, field
+"""
+The term protocols is used for types supporting structural subtyping.
+
+Check this link for more info.
+https://typing.readthedocs.io/en/latest/spec/protocol.html#protocols
+"""
+
+from dataclasses import field
 from datetime import datetime
-from typing import TYPE_CHECKING, Optional, Sequence
+from typing import Optional, Protocol, Sequence, runtime_checkable
 from uuid import UUID
 
-if TYPE_CHECKING:
-    from acquiring import enums, protocols
+from acquiring.enums import OperationStatusEnum, OperationTypeEnum
 
+from .storage import UnitOfWork
 
-# TODO frozen=True compatible with protocols.AbstractPaymentOperation (expected settable variable, got read-only attribute)
-@dataclass
-class PaymentOperation:
-    type: "enums.OperationTypeEnum"
-    status: "enums.OperationStatusEnum"
-    payment_method_id: UUID
 
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}:{self.type}|{self.status}"
+class PaymentOperation(Protocol):
+    payment_method_id: UUID
+    type: OperationTypeEnum
+    status: OperationStatusEnum
 
-    class DuplicateError(Exception):
-        pass
+    def __repr__(self) -> str: ...
 
 
-@dataclass
-class PaymentMethod:
-    id: UUID
+class DraftToken(Protocol):
     created_at: datetime
-    payment_attempt: "protocols.AbstractPaymentAttempt"
-    confirmable: bool
-    token: Optional["protocols.AbstractToken"] = None
-    payment_operations: list["protocols.AbstractPaymentOperation"] = field(default_factory=list, repr=True)
+    token: str
+    metadata: Optional[dict[str, str | int]]
+    expires_at: Optional[datetime]
+    fingerprint: Optional[str]
 
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}:{self.id}"
 
-    def has_payment_operation(self, type: "enums.OperationTypeEnum", status: "enums.OperationStatusEnum") -> bool:
-        return any(operation.type == type and operation.status == status for operation in self.payment_operations)
+class Token(Protocol):
+    created_at: datetime
+    token: str
+    payment_method_id: UUID
+    metadata: Optional[dict[str, str | int]]
+    expires_at: Optional[datetime]
+    fingerprint: Optional[str]
 
-    class DoesNotExist(Exception):
-        pass
+    def __repr__(self) -> str: ...
 
 
-@dataclass
-class DraftPaymentMethod:
-    payment_attempt: "protocols.AbstractPaymentAttempt"
-    confirmable: bool
-    token: Optional["protocols.AbstractToken"] = None
+class DraftItem(Protocol):
+    reference: str
+    name: str
+    quantity: int
+    unit_price: int
+    quantity_unit: Optional[str]
 
 
-@dataclass
-class Item:
+class Item(Protocol):
     id: UUID
     created_at: datetime
     payment_attempt_id: UUID
     reference: str
     name: str
     quantity: int
     quantity_unit: Optional[str]
     unit_price: int
 
-    class InvalidTotalAmount(Exception):
-        pass
 
+# TODO Have this class the DoesNotExist internal class
+class PaymentAttempt(Protocol):
+    id: UUID
+    created_at: datetime
+    amount: int
+    currency: str
+    payment_method_ids: list[UUID]
+    items: Sequence[Item] = field(default_factory=list)
 
-@dataclass
-class DraftItem:
-    reference: str
-    name: str
-    quantity: int
-    unit_price: int
-    quantity_unit: Optional[str] = None
+    def __repr__(self) -> str: ...
 
 
-@dataclass
-class PaymentAttempt:
+# TODO Have this class the DoesNotExist internal class
+class PaymentMethod(Protocol):
     id: UUID
     created_at: datetime
-    amount: int
-    currency: str
-    payment_method_ids: list[UUID] = field(default_factory=list)
-    items: Sequence["protocols.AbstractItem"] = field(default_factory=list)
+    tokens: list[Token]
+    payment_attempt: PaymentAttempt
+    confirmable: bool
+    payment_operations: list[PaymentOperation]
 
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}:{self.id}|{self.amount}{self.currency}"
+    def __repr__(self) -> str: ...
 
-    class DoesNotExist(Exception):
-        pass
+    def has_payment_operation(
+        self: "PaymentMethod",
+        type: OperationTypeEnum,
+        status: OperationStatusEnum,
+    ) -> bool: ...
 
 
-@dataclass
-class DraftPaymentAttempt:
+class DraftPaymentMethod(Protocol):
+    payment_attempt: PaymentAttempt
+    confirmable: bool
+    tokens: list[DraftToken]
+
+
+class DraftPaymentAttempt(Protocol):
     amount: int
     currency: str
-    items: Sequence["protocols.AbstractDraftItem"] = field(default_factory=list)
+    items: Sequence[DraftItem] = field(default_factory=list)
 
 
-@dataclass
-class Token:
-    created_at: datetime
-    token: str
-    metadata: Optional[dict[str, str | int]] = field(default_factory=dict)
-    expires_at: Optional[datetime] = None
-    fingerprint: Optional[str] = None
+class OperationResponse(Protocol):
+    status: OperationStatusEnum
+    payment_method: Optional["PaymentMethod"]
+    type: OperationTypeEnum
+    error_message: Optional[str]
+    actions: list[dict]
+
+
+class BlockResponse(Protocol):
+    status: OperationStatusEnum
+    actions: list[dict] = field(default_factory=list)
+    error_message: Optional[str] = None
+
+
+@runtime_checkable
+class Block(Protocol):
 
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}:{self.token}"
+    def run(
+        self, unit_of_work: UnitOfWork, payment_method: PaymentMethod, *args: Sequence, **kwargs: dict
+    ) -> BlockResponse: ...
```

### Comparing `acquiring-0.2.0/acquiring/domain/providers.py` & `acquiring-0.3.0/acquiring/domain/providers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import functools
 from dataclasses import dataclass
 from datetime import datetime
-from typing import TYPE_CHECKING, Callable, Sequence
+from typing import Callable, Sequence
 from uuid import UUID
-from acquiring import domain
 
-if TYPE_CHECKING:
-    from acquiring import protocols
+from acquiring import domain, protocols
 
 
 @dataclass
 class Transaction:
     external_id: str
     timestamp: datetime
     raw_data: dict
     provider_name: str
     payment_method_id: UUID
 
     def __repr__(self) -> str:
+        """String representation of the class"""
         return f"{self.__class__.__name__}:{self.provider_name}|{self.external_id}"
 
 
 def wrapped_by_transaction(  # type:ignore[misc]
-    function: Callable[..., "protocols.AbstractAdapterResponse"]
-) -> Callable[..., "protocols.AbstractAdapterResponse"]:
+    function: Callable[..., "protocols.AdapterResponse"]
+) -> Callable[..., "protocols.AdapterResponse"]:
     """This decorator ensures that a Transaction gets created after interacting with the Provider via its adapter"""
 
     @functools.wraps(function)
     def wrapper(
-        self: "protocols.AbstractAdapter",
-        payment_method: "protocols.AbstractPaymentMethod",
+        self: "protocols.Adapter",
+        unit_of_work: "protocols.UnitOfWork",
+        payment_method: "protocols.PaymentMethod",
         *args: Sequence,
         **kwargs: dict,
-    ) -> "protocols.AbstractAdapterResponse":
-        result = function(self, payment_method, *args, **kwargs)
+    ) -> "protocols.AdapterResponse":
+        result = function(self, unit_of_work, payment_method, *args, **kwargs)
 
         # A transaction is created only when the Adapter Response is successful
         if result.timestamp is not None and result.external_id is not None:
             transaction = domain.Transaction(
                 external_id=result.external_id,
                 timestamp=result.timestamp,
                 raw_data=result.raw_data,
                 provider_name=self.provider_name,
                 payment_method_id=payment_method.id,
             )
-            self.transaction_repository.add(transaction)
+            with unit_of_work as uow:
+                uow.transactions.add(transaction)
+                uow.commit()
 
         return result
 
     return wrapper
```

### Comparing `acquiring-0.2.0/acquiring/migrations/django/0001_initial.py` & `acquiring-0.3.0/acquiring/storage/django/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Generated by Django 5.0.2 on 2024-04-04 12:42
+# Generated by Django 4.2 on 2024-04-28 04:56
 
 import django.core.validators
+from django.db import migrations, models
 import django.db.models.deletion
 import uuid
-from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
@@ -23,22 +23,46 @@
                 ('currency', models.CharField(max_length=3, validators=[django.core.validators.MinLengthValidator(3)])),
             ],
             options={
                 'abstract': False,
             },
         ),
         migrations.CreateModel(
+            name='PaymentMethod',
+            fields=[
+                ('created_at', models.DateTimeField(auto_now_add=True)),
+                ('id', models.UUIDField(default=uuid.uuid4, editable=False, primary_key=True, serialize=False)),
+                ('confirmable', models.BooleanField(editable=False, help_text='Whether this PaymentMethod can at some point run inside PaymentFlow.confirm')),
+                ('payment_attempt', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='payment_methods', to='acquiring.paymentattempt')),
+            ],
+            options={
+                'abstract': False,
+            },
+        ),
+        migrations.CreateModel(
+            name='Transaction',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('external_id', models.TextField()),
+                ('timestamp', models.DateTimeField()),
+                ('raw_data', models.JSONField()),
+                ('provider_name', models.TextField()),
+                ('payment_method', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='transaction', to='acquiring.paymentmethod')),
+            ],
+        ),
+        migrations.CreateModel(
             name='Token',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_at', models.DateTimeField()),
                 ('expires_at', models.DateTimeField(blank=True, null=True)),
                 ('token', models.TextField()),
                 ('fingerprint', models.TextField(blank=True, help_text='Fingerprinting provides a way to correlate multiple tokens together that contain the same data without needing access to the underlying data.', null=True)),
                 ('metadata', models.JSONField(blank=True, help_text='tag your tokens with custom key-value attributes (i.e., to reference a record in your own database, tag records that fall into certain compliance requirements like GDPR, etc)', null=True)),
+                ('payment_method', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='tokens', to='acquiring.paymentmethod')),
             ],
         ),
         migrations.CreateModel(
             name='Item',
             fields=[
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('id', models.UUIDField(default=uuid.uuid4, editable=False, primary_key=True, serialize=False)),
@@ -50,57 +74,33 @@
                 ('payment_attempt', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='items', to='acquiring.paymentattempt')),
             ],
             options={
                 'abstract': False,
             },
         ),
         migrations.CreateModel(
-            name='PaymentMethod',
+            name='PaymentOperation',
             fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
-                ('id', models.UUIDField(default=uuid.uuid4, editable=False, primary_key=True, serialize=False)),
-                ('confirmable', models.BooleanField(editable=False, help_text='Whether this PaymentMethod can at some point run inside PaymentFlow.confirm')),
-                ('payment_attempt', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='payment_methods', to='acquiring.paymentattempt')),
-                ('token', models.OneToOneField(blank=True, null=True, on_delete=django.db.models.deletion.PROTECT, related_name='payment_method', to='acquiring.token')),
+                ('type', models.CharField(choices=[('initialize', 'Initialize'), ('process_action', 'Process Action'), ('pay', 'Pay'), ('confirm', 'Confirm'), ('refund', 'Refund'), ('after_pay', 'After Pay'), ('after_confirm', 'After Confirm'), ('after_refund', 'After Refund')], max_length=16)),
+                ('status', models.CharField(choices=[('started', 'Started'), ('failed', 'Failed'), ('completed', 'Completed'), ('requires_action', 'Requires Action'), ('pending', 'Pending'), ('not_performed', 'Not Performed')], db_index=True, max_length=15)),
+                ('payment_method', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='payment_operations', to='acquiring.paymentmethod')),
             ],
             options={
-                'abstract': False,
+                'unique_together': {('status', 'payment_method', 'type')},
             },
         ),
         migrations.CreateModel(
-            name='Transaction',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('external_id', models.TextField()),
-                ('timestamp', models.DateTimeField()),
-                ('raw_data', models.JSONField()),
-                ('provider_name', models.TextField()),
-                ('payment_method', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='transaction', to='acquiring.paymentmethod')),
-            ],
-        ),
-        migrations.CreateModel(
             name='BlockEvent',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('status', models.CharField(choices=[('started', 'Started'), ('failed', 'Failed'), ('completed', 'Completed'), ('requires_action', 'Requires Action'), ('pending', 'Pending'), ('not_performed', 'Not Performed')], max_length=15)),
                 ('block_name', models.CharField(max_length=20)),
                 ('payment_method', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='acquiring.paymentmethod')),
             ],
             options={
                 'unique_together': {('status', 'payment_method', 'block_name')},
             },
         ),
-        migrations.CreateModel(
-            name='PaymentOperation',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('created_at', models.DateTimeField(auto_now_add=True)),
-                ('type', models.CharField(choices=[('initialize', 'Initialize'), ('process_action', 'Process Action'), ('pay', 'Pay'), ('confirm', 'Confirm'), ('refund', 'Refund'), ('after_pay', 'After Pay'), ('after_confirm', 'After Confirm'), ('after_refund', 'After Refund')], max_length=16)),
-                ('status', models.CharField(choices=[('started', 'Started'), ('failed', 'Failed'), ('completed', 'Completed'), ('requires_action', 'Requires Action'), ('pending', 'Pending'), ('not_performed', 'Not Performed')], max_length=15)),
-                ('payment_method', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='payment_operations', to='acquiring.paymentmethod')),
-            ],
-            options={
-                'unique_together': {('status', 'payment_method', 'type')},
-            },
-        ),
     ]
```

### Comparing `acquiring-0.2.0/acquiring/models/django.py` & `acquiring-0.3.0/acquiring/storage/django/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
-from typing import TYPE_CHECKING
 from uuid import uuid4
 
 import django.db.models
 from django.core import validators as django_validators
 
-from acquiring import domain
-
-if TYPE_CHECKING:
-    from acquiring import protocols
-
+from acquiring import domain, protocols
 
 CURRENCY_CODE_MAX_LENGTH = 3
 
 
 class Identifiable(django.db.models.Model):
     """Mixin for models that can be identified"""
 
@@ -43,15 +38,15 @@
             django_validators.MinLengthValidator(CURRENCY_CODE_MAX_LENGTH),
         ],
     )
 
     def __str__(self) -> str:
         return f"[id={self.id}, {self.currency}{self.amount}]"
 
-    def to_domain(self) -> "protocols.AbstractPaymentAttempt":
+    def to_domain(self) -> "protocols.PaymentAttempt":
         return domain.PaymentAttempt(
             id=self.id,
             created_at=self.created_at,
             amount=self.amount,
             currency=self.currency,
             items=[item.to_domain() for item in self.items.all()],
             payment_method_ids=[payment_method.id for payment_method in self.payment_methods.all()],
@@ -91,15 +86,15 @@
             "Currency is assumed to be the one provided in PaymentAttempt."
         )
     )
 
     def __str__(self) -> str:
         return f"[reference={self.reference}, quantity={self.quantity}{str(' ' + self.quantity_unit) if self.quantity_unit else ''}]"
 
-    def to_domain(self) -> "protocols.AbstractItem":
+    def to_domain(self) -> "protocols.Item":
         return domain.Item(
             id=self.id,
             created_at=self.created_at,
             payment_attempt_id=self.payment_attempt_id,
             name=self.name,
             quantity=self.quantity,
             quantity_unit=self.quantity_unit,
@@ -112,35 +107,27 @@
 
     payment_attempt = django.db.models.ForeignKey(
         PaymentAttempt,
         on_delete=django.db.models.CASCADE,
         related_name="payment_methods",
     )
 
-    token = django.db.models.OneToOneField(
-        "Token",
-        on_delete=django.db.models.PROTECT,
-        null=True,
-        blank=True,
-        related_name="payment_method",
-    )
-
     confirmable = django.db.models.BooleanField(
         editable=False,
         help_text="Whether this PaymentMethod can at some point run inside PaymentFlow.confirm",
     )
 
     def __str__(self) -> str:
         return f"[id={self.id}]"
 
-    def to_domain(self) -> "protocols.AbstractPaymentMethod":
+    def to_domain(self) -> "protocols.PaymentMethod":
         return domain.PaymentMethod(
             id=self.id,
             created_at=self.created_at,
-            token=self.token.to_domain() if self.token else None,
+            tokens=[token.to_domain() for token in self.tokens.all()],
             payment_attempt=self.payment_attempt.to_domain(),
             payment_operations=[payment_operation.to_domain() for payment_operation in self.payment_operations.all()],
             confirmable=self.confirmable,
         )
 
 
 class Token(django.db.models.Model):
@@ -158,24 +145,31 @@
 
     metadata = django.db.models.JSONField(
         null=True,
         blank=True,
         help_text="tag your tokens with custom key-value attributes (i.e., to reference a record in your own database, tag records that fall into certain compliance requirements like GDPR, etc)",
     )
 
+    payment_method = django.db.models.ForeignKey(
+        PaymentMethod,
+        on_delete=django.db.models.CASCADE,
+        related_name="tokens",
+    )
+
     def __str__(self) -> str:
         return f"[{self.token}]"
 
-    def to_domain(self) -> "protocols.AbstractToken":
+    def to_domain(self) -> "protocols.Token":
         return domain.Token(
             created_at=self.created_at,
             expires_at=self.expires_at,
             token=self.token,
             fingerprint=self.fingerprint,
             metadata=self.metadata,
+            payment_method_id=self.payment_method_id,
         )
 
 
 class PaymentOperationTypeChoices(django.db.models.TextChoices):
     INITIALIZE = "initialize"
     PROCESS_ACTION = "process_action"
     PAY = "pay"
@@ -195,49 +189,49 @@
     NOT_PERFORMED = "not_performed"
 
 
 # TODO Add failure reason to Payment Operation as an optional string
 class PaymentOperation(django.db.models.Model):
     created_at = django.db.models.DateTimeField(auto_now_add=True)
 
-    type = django.db.models.CharField(max_length=16, choices=PaymentOperationTypeChoices)
-    status = django.db.models.CharField(max_length=15, choices=StatusChoices)
+    type = django.db.models.CharField(max_length=16, choices=PaymentOperationTypeChoices.choices)
+    status = django.db.models.CharField(max_length=15, choices=StatusChoices.choices, db_index=True)
     payment_method = django.db.models.ForeignKey(
         PaymentMethod,
         on_delete=django.db.models.CASCADE,
         related_name="payment_operations",
     )
 
     class Meta:
         unique_together = ("status", "payment_method", "type")
 
     def __str__(self) -> str:
         return f"[type={self.type}, status={self.status}]"
 
-    def to_domain(self) -> "protocols.AbstractPaymentOperation":
+    def to_domain(self) -> "protocols.PaymentOperation":
         return domain.PaymentOperation(
             type=self.type,
             status=self.status,
             payment_method_id=self.payment_method_id,
         )
 
 
 class BlockEvent(django.db.models.Model):
     created_at = django.db.models.DateTimeField(auto_now_add=True)
-    status = django.db.models.CharField(max_length=15, choices=StatusChoices)
+    status = django.db.models.CharField(max_length=15, choices=StatusChoices.choices)
     payment_method = django.db.models.ForeignKey(PaymentMethod, on_delete=django.db.models.CASCADE)
     block_name = django.db.models.CharField(max_length=20)
 
     class Meta:
         unique_together = ("status", "payment_method", "block_name")
 
     def __str__(self) -> str:
         return f"[{self.block_name}|status={self.status}]"
 
-    def to_domain(self) -> "protocols.AbstractBlockEvent":
+    def to_domain(self) -> "protocols.BlockEvent":
         return domain.BlockEvent(
             status=self.status,
             payment_method_id=self.payment_method.id,
             block_name=self.block_name,
         )
 
 
@@ -257,15 +251,15 @@
         on_delete=django.db.models.CASCADE,
         related_name="transaction",
     )
 
     def __str__(self) -> str:
         return f"[provider={self.provider_name}|payment_method={self.payment_method_id}|{self.external_id}]"
 
-    def to_domain(self) -> "protocols.AbstractTransaction":
+    def to_domain(self) -> "protocols.Transaction":
         return domain.Transaction(
             external_id=self.external_id,
             timestamp=self.timestamp,
             raw_data=self.raw_data,
             provider_name=self.provider_name,
             payment_method_id=self.payment_method_id,
         )
```

### Comparing `acquiring-0.2.0/acquiring/protocols/providers.py` & `acquiring-0.3.0/acquiring/protocols/providers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from dataclasses import dataclass
 from datetime import datetime
 from enum import StrEnum
 from typing import Generic, Optional, Protocol, TypeVar
 from uuid import UUID
 
-from acquiring.protocols import repositories
+from acquiring.protocols import storage
 
 Status = TypeVar("Status", bound=StrEnum)
 
 
 @dataclass(match_args=False)
-class AbstractAdapterResponse(Generic[Status], Protocol):
+class AdapterResponse(Generic[Status], Protocol):
     external_id: Optional[str]  # UUID cannot be imposed across all adapters
     timestamp: Optional[datetime]
     raw_data: dict
     status: Status
 
 
 @dataclass
-class AbstractAdapter(Protocol):
+class Adapter(Protocol):
     base_url: str
     provider_name: str
-    transaction_repository: repositories.AbstractRepository
+    transaction_repository: storage.Repository
 
 
 @dataclass
-class AbstractTransaction(Protocol):
+class Transaction(Protocol):
     external_id: str
     timestamp: datetime
     raw_data: dict
     provider_name: str
     payment_method_id: UUID
 
     def __repr__(self) -> str: ...
```

### Comparing `acquiring-0.2.0/acquiring/repositories/django.py` & `acquiring-0.3.0/acquiring/storage/django/repositories.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,194 +1,139 @@
-from typing import TYPE_CHECKING
 from uuid import UUID
 
 import deal
 import django.db.transaction
 
-from acquiring import domain, models
+from acquiring import domain, protocols
 from acquiring.enums import OperationStatusEnum, OperationTypeEnum
-
-if TYPE_CHECKING:
-    from acquiring import protocols
-
-
-class PaymentAttemptRepository:
-
-    @deal.reason(
-        domain.Item.InvalidTotalAmount,
-        lambda _, data: sum(i.quantity * i.unit_price for i in data.items) != data.amount,
-    )
-    def add(self, data: "protocols.AbstractDraftPaymentAttempt") -> "protocols.AbstractPaymentAttempt":
-        with django.db.transaction.atomic():
-
-            payment_attempt = models.PaymentAttempt(
-                amount=data.amount,
-                currency=data.currency,
-            )
-            payment_attempt.save()
-            if data.items:
-                items = [
-                    models.Item(
-                        name=item.name,
-                        quantity=item.quantity,
-                        quantity_unit=item.quantity_unit,
-                        reference=item.reference,
-                        unit_price=item.unit_price,
-                        payment_attempt=payment_attempt,
-                    )
-                    for item in data.items
-                ]
-                # TODO Embed this validation into Item somehow?
-                if sum(item.quantity * item.unit_price for item in items) != payment_attempt.amount:
-                    raise domain.Item.InvalidTotalAmount
-                models.Item.objects.bulk_create(items)
-
-        return payment_attempt.to_domain()
-
-    @deal.reason(
-        domain.PaymentAttempt.DoesNotExist,
-        lambda _, id: models.PaymentAttempt.objects.filter(id=id).count() == 0,
-    )
-    def get(self, id: UUID) -> "protocols.AbstractPaymentAttempt":
-        try:
-            payment_attempt = models.PaymentAttempt.objects.prefetch_related(
-                "payment_methods",
-                "payment_methods__payment_operations",
-            ).get(id=id)
-            return payment_attempt.to_domain()
-        except models.PaymentAttempt.DoesNotExist:
-            raise domain.PaymentAttempt.DoesNotExist
+from acquiring.storage.django import models
 
 
 class PaymentMethodRepository:
 
     @deal.safe()
-    def add(self, data: "protocols.AbstractDraftPaymentMethod") -> "protocols.AbstractPaymentMethod":
-        with django.db.transaction.atomic():
-            db_payment_method = models.PaymentMethod(
-                payment_attempt_id=data.payment_attempt.id,
-                confirmable=data.confirmable,
-            )
-
-            if data.token:
-                db_token = models.Token(
-                    payment_method=db_payment_method,
-                    created_at=data.token.created_at,  # TODO Ensure via type that datetime is timezone aware
-                    token=data.token.token,
-                    expires_at=data.token.expires_at,  # TODO Ensure via type that datetime is timezone aware
-                    fingerprint=data.token.fingerprint,
-                    metadata=data.token.metadata,
-                )
-                db_token.save()
-                db_payment_method.token = db_token
-            db_payment_method.save()
+    def add(self, data: "protocols.DraftPaymentMethod") -> "protocols.PaymentMethod":
+        db_payment_method = models.PaymentMethod(
+            payment_attempt_id=data.payment_attempt.id,
+            confirmable=data.confirmable,
+        )
+        db_payment_method.save()
         return db_payment_method.to_domain()
 
     @deal.reason(
         domain.PaymentMethod.DoesNotExist,
         lambda _, id: models.PaymentMethod.objects.filter(id=id).count() == 0,
     )
-    def get(self, id: UUID) -> "protocols.AbstractPaymentMethod":
+    def get(self, id: UUID) -> "protocols.PaymentMethod":
         try:
             payment_method = (
-                models.PaymentMethod.objects.prefetch_related("payment_operations")
-                .select_related("token", "payment_attempt")
+                models.PaymentMethod.objects.prefetch_related("payment_operations", "tokens")
+                .select_related("payment_attempt")
                 .get(id=id)
             )
             return payment_method.to_domain()
         except models.PaymentMethod.DoesNotExist:
             raise domain.PaymentMethod.DoesNotExist
 
-    @deal.reason(
-        domain.PaymentMethod.DoesNotExist,
-        lambda _, payment_method, token: models.PaymentMethod.objects.filter(id=payment_method.id).count() == 0,
-    )
-    def add_token(
-        self, payment_method: "protocols.AbstractPaymentMethod", token: "protocols.AbstractToken"
-    ) -> "protocols.AbstractPaymentMethod":
-        try:
-            db_payment_method = models.PaymentMethod.objects.get(id=payment_method.id)
-        except models.PaymentMethod.DoesNotExist:
-            raise domain.PaymentMethod.DoesNotExist
-
-        with django.db.transaction.atomic():
-            db_token = models.Token(
-                payment_method=db_payment_method,
-                created_at=token.created_at,  # TODO Ensure via type that datetime is timezone aware
-                token=token.token,
-                expires_at=token.expires_at,  # TODO Ensure via type that datetime is timezone aware
-                fingerprint=token.fingerprint,
-                metadata=token.metadata,
-            )
-            db_token.save()
-            db_payment_method.token = db_token
-            db_payment_method.save()
-
-            payment_method.token = db_token.to_domain()
-            return payment_method
-
 
 class PaymentOperationRepository:
 
-    @deal.raises(domain.PaymentOperation.DuplicateError)  # TODO Turn this into deal.reason
+    @deal.raises(domain.PaymentOperation.Duplicated)  # TODO Turn this into deal.reason
     def add(
         self,
-        payment_method: "protocols.AbstractPaymentMethod",
+        payment_method: "protocols.PaymentMethod",
         type: OperationTypeEnum,
         status: OperationStatusEnum,
-    ) -> "protocols.AbstractPaymentOperation":
+    ) -> "protocols.PaymentOperation":
         db_payment_operation = models.PaymentOperation(
             payment_method_id=payment_method.id,
             type=type,
             status=status,
         )
         try:
             db_payment_operation.save()
             payment_operation = db_payment_operation.to_domain()
             payment_method.payment_operations.append(payment_operation)
             return payment_operation
         except django.db.utils.IntegrityError:
-            raise domain.PaymentOperation.DuplicateError
+            raise domain.PaymentOperation.Duplicated
 
-    def get(self, id: UUID) -> "protocols.AbstractPaymentOperation": ...  # type: ignore[empty-body]
+    def get(self, id: UUID) -> "protocols.PaymentOperation": ...  # type: ignore[empty-body]
 
 
 # TODO Append block event to payment_method.block_events?
 # TODO Test when payment method id does not correspond to any existing payment method
 class BlockEventRepository:
 
-    @deal.raises(domain.BlockEvent.DuplicateError)  # TODO Turn this into deal.reason
-    def add(self, block_event: "protocols.AbstractBlockEvent") -> "protocols.AbstractBlockEvent":
+    @deal.raises(domain.BlockEvent.Duplicated)  # TODO Turn this into deal.reason
+    def add(self, block_event: "protocols.BlockEvent") -> "protocols.BlockEvent":
         try:
             db_block_event = models.BlockEvent(
                 status=block_event.status,
                 payment_method_id=block_event.payment_method_id,
                 block_name=block_event.block_name,
             )
             db_block_event.save()
             return db_block_event.to_domain()
         except django.db.utils.IntegrityError:
-            raise domain.BlockEvent.DuplicateError
+            raise domain.BlockEvent.Duplicated
 
-    def get(self, id: UUID) -> "protocols.AbstractBlockEvent": ...  # type: ignore[empty-body]
+    def get(self, id: UUID) -> "protocols.BlockEvent": ...  # type: ignore[empty-body]
 
 
 # TODO Append transaction to payment_method.transactions?
 # TODO Test when payment method id does not correspond to any existing payment method
 class TransactionRepository:
 
     @deal.safe()
     def add(
         self,
-        transaction: "protocols.AbstractTransaction",
-    ) -> "protocols.AbstractTransaction":
+        transaction: "protocols.Transaction",
+    ) -> "protocols.Transaction":
         db_transaction = models.Transaction(
             external_id=transaction.external_id,
             timestamp=transaction.timestamp,
             raw_data=transaction.raw_data,
             provider_name=transaction.provider_name,
             payment_method_id=transaction.payment_method_id,
         )
         db_transaction.save()
         return db_transaction.to_domain()
 
-    def get(self, id: UUID) -> "protocols.AbstractTransaction": ...  # type: ignore[empty-body]
+    def get(self, id: UUID) -> "protocols.Transaction": ...  # type: ignore[empty-body]
+
+
+class TokenRepository:
+
+    @deal.reason(
+        domain.Token.DoesNotExist,
+        lambda _, token: models.Token.objects.filter(token=token).count() == 0,
+    )
+    def get(self, token: str) -> "protocols.PaymentMethod":
+        try:
+            instance = models.Token.objects.select_related("token").get(token=token)
+            return instance.to_domain()
+        except models.Token.DoesNotExist:
+            raise domain.Token.DoesNotExist
+
+    @deal.reason(
+        domain.PaymentMethod.DoesNotExist,
+        lambda _, payment_method, token: models.PaymentMethod.objects.filter(id=payment_method.id).count() == 0,
+    )
+    def add(self, payment_method: "protocols.PaymentMethod", token: "protocols.Token") -> "protocols.PaymentMethod":
+        try:
+            db_payment_method = models.PaymentMethod.objects.get(id=payment_method.id)
+        except models.PaymentMethod.DoesNotExist:
+            raise domain.PaymentMethod.DoesNotExist
+
+        db_token = models.Token(
+            payment_method=db_payment_method,
+            created_at=token.created_at,  # TODO Ensure via type that datetime is timezone aware
+            token=token.token,
+            expires_at=token.expires_at,  # TODO Ensure via type that datetime is timezone aware
+            fingerprint=token.fingerprint,
+            metadata=token.metadata,
+        )
+        db_token.save()
+
+        payment_method.tokens.append(db_token.to_domain())
+        return payment_method
```

### Comparing `acquiring-0.2.0/manage.py` & `acquiring-0.3.0/manage.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.2.0/requirements/development.txt` & `acquiring-0.3.0/requirements/development.txt`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 # Flit to simplify package management
 flit
 
 # Hypothesis to find edge cases
 hypothesis[pytz]
 
+# interrogate to check for missing docstrings
+interrogate
+
 # ipdb to access the IPython debugger as if it were the pdb module
 ipdb
 
 
 # Mutatest to check if small modifications (mutations) in the code are detectable by tests
 mutatest
 
@@ -22,15 +25,12 @@
 
 # Pytest to run the tests
 pytest
 
 # pytest-cov to measure code coverage
 pytest-cov
 
-# python-dotenv to manage environment variables
-python-dotenv
-
 # Responses to mock requests
 responses
 
 # Tox to automate and standardize testing in Python
 tox
```

### Comparing `acquiring-0.2.0/tests/conftest.py` & `acquiring-0.3.0/tests/contrib/paypal/blocks/test_paypal_after_creating_order.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,184 +1,172 @@
-import os
 import uuid
-from dataclasses import dataclass
-from datetime import datetime
-from typing import Callable, Generator, List, Optional
-from unittest import mock
+from datetime import datetime, timezone
+from typing import Callable, Optional
 
-import pytest
+from faker import Faker
 
 from acquiring import domain, enums, protocols
+from acquiring.contrib import paypal
 
+fake = Faker()
 
-# https://docs.pytest.org/en/7.1.x/reference/reference.html?highlight=pytest_config#pytest.hookspec.pytest_configure
-def pytest_configure(config: Callable) -> None:
-    try:
-        import django
-        from django.conf import settings
-
-        from acquiring import settings as project_settings
-
-        settings.configure(
-            DATABASES={
-                "default": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"},
-                "secondary": {"ENGINE": "django.db.backends.sqlite3", "NAME": ":memory:"},
+
+# TODO implement hypothesis
+def test_givenACorrectPaymentMethod_whenRunningPayPalAfterCreatingOrder_thenItCompletesPayment(
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
+    ],
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
+    ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_unit_of_work: type[protocols.UnitOfWork],
+) -> None:
+
+    payment_method = domain.PaymentMethod(
+        id=uuid.uuid4(),
+        created_at=datetime.now(),
+        payment_attempt=domain.PaymentAttempt(
+            id=uuid.uuid4(),
+            created_at=datetime.now(),
+            amount=30,
+            currency="USD",
+        ),
+        confirmable=False,
+    )
+
+    unit_of_work = fake_unit_of_work(
+        payment_method_repository_class=fake_payment_method_repository_class([]),
+        payment_operation_repository_class=fake_payment_operation_repository_class([]),
+        block_event_repository_class=fake_block_event_repository_class([]),
+        transaction_repository_class=fake_transaction_repository_class([]),
+    )
+
+    block = paypal.blocks.PayPalAfterCreatingOrder()
+
+    external_id = "WH-684457241H310260F-0FC94184GF055315P"
+    fake_create_time = datetime.now(timezone.utc).isoformat()
+    fake_merchant_id = fake.md5()
+    fake_currency = fake.currency_code()
+    payee_email = fake.email()
+    payer_email = fake.email()
+    payer_first_name = fake.first_name()
+    payer_last_name = fake.last_name()
+    payer_country = fake.country_code()
+    payer_id = fake.md5()
+
+    raw_data = {
+        "id": external_id,
+        "event_version": "1.0",
+        "create_time": fake_create_time,
+        "resource_type": "checkout-order",
+        "resource_version": "2.0",
+        "event_type": "CHECKOUT.ORDER.APPROVED",
+        "summary": fake.sentence(),
+        "resource": {
+            "create_time": datetime.now(timezone.utc).isoformat(),
+            "purchase_units": [
+                {
+                    "reference_id": fake.uuid4(),
+                    "amount": {"currency_code": fake_currency, "value": "10.00"},
+                    "payee": {
+                        "email_address": payee_email,
+                        "merchant_id": fake_merchant_id,
+                    },
+                },
+                {
+                    "reference_id": fake.uuid4(),
+                    "amount": {"currency_code": fake_currency, "value": "20.00"},
+                    "payee": {
+                        "email_address": payee_email,
+                        "merchant_id": fake_merchant_id,
+                    },
+                },
+            ],
+            "links": [
+                {
+                    "href": fake.url(),
+                    "rel": fake.word(),
+                    "method": fake.http_method(),
+                }
+                for _ in range(3)
+            ],
+            "id": "55855893X5198173A",
+            "payment_source": {
+                "paypal": {
+                    "email_address": payer_email,
+                    "account_id": payer_id,
+                    "account_status": "VERIFIED",
+                    "name": {
+                        "given_name": payer_first_name,
+                        "surname": payer_last_name,
+                    },
+                    "address": {"country_code": payer_country},
+                }
+            },
+            "intent": "CAPTURE",
+            "payer": {
+                "name": {"given_name": payer_first_name, "surname": payer_last_name},
+                "email_address": payer_email,
+                "payer_id": payer_id,
+                "address": {"country_code": payer_country},
             },
-            INSTALLED_APPS=project_settings.INSTALLED_APPS,
-            MIGRATION_MODULES={"acquiring": "acquiring.migrations.django"},
-        )
-
-        django.setup()
-    except ImportError:
-        # django isn't installed, skip
-        return
-
-
-@pytest.fixture()
-def fake_os_environ() -> Generator:
-    with mock.patch.dict(
-        os.environ,
-        {
-            "PAYPAL_CLIENT_ID": "long-client-id",
-            "PAYPAL_CLIENT_SECRET": "long-client-secret",
-            "PAYPAL_BASE_URL": "https://api-m.sandbox.paypal.com/",
+            "status": "APPROVED",
         },
-    ):
-        yield
-
-
-@pytest.fixture(scope="module")
-def fake_payment_method_repository() -> Callable[
-    [Optional[List[protocols.AbstractPaymentMethod]]],
-    protocols.AbstractRepository,
-]:
-
-    @dataclass
-    class FakePaymentMethodRepository:
-        units: List[protocols.AbstractPaymentMethod]
-
-        def add(self, data: protocols.AbstractDraftPaymentMethod) -> protocols.AbstractPaymentMethod:
-            payment_method = domain.PaymentMethod(
-                id=uuid.uuid4(),
-                created_at=datetime.now(),
-                payment_attempt=data.payment_attempt,
-                confirmable=data.confirmable,
-                token=data.token,
-                payment_operations=[],
-            )
-            self.units.append(payment_method)
-            return payment_method
-
-        def get(self, id: uuid.UUID) -> protocols.AbstractPaymentMethod:
-            for unit in self.units:
-                if unit.id == id:
-                    return unit
-            raise domain.PaymentMethod.DoesNotExist
-
-    def build_repository(
-        units: Optional[list[protocols.AbstractPaymentMethod]] = None,
-    ) -> protocols.AbstractRepository:
-        return FakePaymentMethodRepository(units=units if units else [])
-
-    return build_repository
-
-
-@pytest.fixture(scope="module")
-def fake_payment_operation_repository() -> Callable[
-    [Optional[list[protocols.AbstractPaymentOperation]]],
-    protocols.AbstractRepository,
-]:
-
-    @dataclass
-    class FakePaymentOperationRepository:
-        units: list[protocols.AbstractPaymentOperation]
-
-        def add(
-            self,
-            payment_method: protocols.AbstractPaymentMethod,
-            type: enums.OperationTypeEnum,
-            status: enums.OperationStatusEnum,
-        ) -> protocols.AbstractPaymentOperation:
-            payment_operation = domain.PaymentOperation(
-                type=type,
-                status=status,
-                payment_method_id=payment_method.id,
-            )
-            payment_method.payment_operations.append(payment_operation)
-            return payment_operation
-
-        def get(  # type:ignore[empty-body]
-            self, id: uuid.UUID
-        ) -> protocols.AbstractPaymentOperation: ...
-
-    def build_repository(
-        units: Optional[list[protocols.AbstractPaymentOperation]] = None,
-    ) -> protocols.AbstractRepository:
-        return FakePaymentOperationRepository(units=units if units else [])
-
-    return build_repository
-
-
-@pytest.fixture(scope="module")
-def fake_transaction_repository() -> Callable[
-    [Optional[List[protocols.AbstractTransaction]]],
-    protocols.AbstractRepository,
-]:
-
-    @dataclass
-    class FakeAbstractTransactionRepository:
-        units: List[protocols.AbstractTransaction]
-
-        def add(self, transaction: protocols.AbstractTransaction) -> protocols.AbstractTransaction:
-            transaction = domain.Transaction(
-                external_id=transaction.external_id,
-                timestamp=transaction.timestamp,
-                raw_data=transaction.raw_data,
-                provider_name=transaction.provider_name,
-                payment_method_id=transaction.payment_method_id,
-            )
-            self.units.append(transaction)
-            return transaction
-
-        def get(  # type:ignore[empty-body]
-            self,
-            id: uuid.UUID,
-        ) -> protocols.AbstractTransaction: ...
-
-    def build_repository(
-        units: Optional[list[protocols.AbstractTransaction]] = None,
-    ) -> protocols.AbstractRepository:
-        return FakeAbstractTransactionRepository(units=units if units else [])
-
-    return build_repository
-
-
-@pytest.fixture(scope="module")
-def fake_block_event_repository() -> (
-    Callable[[Optional[list[protocols.AbstractBlockEvent]]], protocols.AbstractRepository]
-):
-
-    @dataclass
-    class FakeBlockEventRepository:
-        units: list[protocols.AbstractBlockEvent]
-
-        def add(self, block_event: protocols.AbstractBlockEvent) -> protocols.AbstractBlockEvent:
-            block_event = domain.BlockEvent(
-                status=block_event.status,
-                payment_method_id=block_event.payment_method_id,
-                block_name=block_event.block_name,
-            )
-            self.units.append(block_event)
-            return block_event
-
-        def get(  # type:ignore[empty-body]
-            self, id: uuid.UUID
-        ) -> protocols.AbstractBlockEvent: ...
-
-    assert issubclass(FakeBlockEventRepository, protocols.AbstractRepository)
-
-    def build_repository(
-        units: Optional[list[protocols.AbstractBlockEvent]] = None,
-    ) -> protocols.AbstractRepository:
-        return FakeBlockEventRepository(units=units if units else [])
-
-    return build_repository
+        "links": [
+            {
+                "href": fake.url(),
+                "rel": fake.word(),
+                "method": fake.http_method(),
+            }
+            for _ in range(2)
+        ],
+    }
+
+    response = block.run(
+        unit_of_work,
+        payment_method,
+        webhook_data=paypal.domain.PayPalWebhookData(
+            id=raw_data["id"],
+            event_version=raw_data["event_version"],
+            create_time=datetime.fromisoformat(raw_data["create_time"]),
+            resource_type=raw_data["resource_type"],
+            resource_version=raw_data["resource_version"],
+            event_type=raw_data["event_type"],
+            summary=raw_data["summary"],
+            raw_data=raw_data,
+        ),
+    )
+
+    assert response == domain.BlockResponse(
+        status=enums.OperationStatusEnum.COMPLETED,
+        actions=[],
+        error_message=None,
+    )
+
+    block_events: list[domain.BlockEvent] = unit_of_work.block_event_units  # type:ignore[attr-defined]
+    assert len(block_events) == 2
+    assert [block.status for block in block_events] == [
+        enums.OperationStatusEnum.STARTED,
+        enums.OperationStatusEnum.COMPLETED,
+    ]
+
+    transactions: list[domain.Transaction] = unit_of_work.transaction_units  # type:ignore[attr-defined]
+
+    assert len(transactions) == 1
+
+    assert transactions[0] == domain.Transaction(
+        external_id=external_id,
+        timestamp=datetime.fromisoformat(fake_create_time),
+        raw_data=raw_data,
+        provider_name="paypal",
+        payment_method_id=payment_method.id,
+    )
```

### Comparing `acquiring-0.2.0/tests/contrib/paypal/blocks/test_paypal_create_order.py` & `acquiring-0.3.0/tests/contrib/paypal/blocks/test_paypal_create_order.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 import os
 import uuid
 from datetime import datetime, timezone
-from typing import Callable, Generator
+from typing import Callable, Generator, Optional
 
 import responses
 from faker import Faker
 
 from acquiring import domain, enums, protocols
 from acquiring.contrib import paypal
 
 fake = Faker()
 
 
 @responses.activate
-def test_givenACorrectPaymentMethod_whenRunningPayPalCreateOrder_thenItReturnsRedirectAction(  # type:ignore[misc]
+def test_givenACorrectPaymentMethod_whenRunningPayPalCreateOrder_thenItReturnsRedirectAction(
     fake_os_environ: Generator,
-    fake_transaction_repository: Callable[
-        ...,
-        protocols.AbstractRepository,
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
     ],
-    fake_block_event_repository: Callable[
-        ...,
-        protocols.AbstractRepository,
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
     ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_unit_of_work: type[protocols.UnitOfWork],
 ) -> None:
     payment_method = domain.PaymentMethod(
         id=uuid.uuid4(),
         created_at=datetime.now(),
         payment_attempt=domain.PaymentAttempt(
             id=uuid.uuid4(),
             created_at=datetime.now(),
@@ -47,23 +56,26 @@
             "expires_in": 31668,
             "nonce": f"{datetime.now(timezone.utc).isoformat()}-{fake.password(length=40, special_chars=False, upper_case=False)}",
         },
         status=201,
         content_type="application/json",
     )
 
-    repository = fake_block_event_repository()
+    unit_of_work = fake_unit_of_work(
+        payment_method_repository_class=fake_payment_method_repository_class([]),
+        payment_operation_repository_class=fake_payment_operation_repository_class([]),
+        block_event_repository_class=fake_block_event_repository_class([]),
+        transaction_repository_class=fake_transaction_repository_class([]),
+    )
 
     block = paypal.blocks.PayPalCreateOrder(
-        block_event_repository=repository,
         adapter=paypal.adapter.PayPalAdapter(
             base_url=os.environ["PAYPAL_BASE_URL"],
             client_id=os.environ["PAYPAL_CLIENT_ID"],
             client_secret=os.environ["PAYPAL_CLIENT_SECRET"],
-            transaction_repository=fake_transaction_repository(),
             callback_url=fake.url(),
             webhook_id=fake.isbn10(),
         ),
     )
 
     fake_create_time = datetime.now(timezone.utc).isoformat()
     fake_id = fake.password(length=10, special_chars=False, upper_case=False).upper()
@@ -96,23 +108,23 @@
         responses.Response(
             responses.POST,
             f"{os.environ['PAYPAL_BASE_URL']}v2/checkout/orders",
             json=raw_response,
         )
     )
 
-    response = block.run(payment_method)
+    response = block.run(unit_of_work, payment_method)
 
     assert response == domain.BlockResponse(
         status=enums.OperationStatusEnum.COMPLETED,
         actions=[{"redirect_url": approve_url}],
         error_message=None,
     )
 
-    block_events: list[domain.BlockEvent] = repository.units  # type:ignore[attr-defined]
+    block_events: list[domain.BlockEvent] = unit_of_work.block_event_units  # type:ignore[attr-defined]
     assert len(block_events) == 2
     assert [block.status for block in block_events] == [
         enums.OperationStatusEnum.STARTED,
         enums.OperationStatusEnum.COMPLETED,
     ]
 
     # assert models.Transaction.objects.count() == 1
```

### Comparing `acquiring-0.2.0/tests/django/factories.py` & `acquiring-0.3.0/tests/storage/django/factories.py`

 * *Files identical despite different names*

### Comparing `acquiring-0.2.0/tests/django/repositories/test_block_event_repository.py` & `acquiring-0.3.0/tests/storage/django/repositories/test_block_event_repository.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pytest
-from hypothesis import given, settings
-from hypothesis import strategies as st
+from faker import Faker
 
 from acquiring.enums import OperationStatusEnum
 from acquiring.utils import is_django_installed
-from tests.django.utils import skip_if_django_not_installed
+from tests.storage.utils import skip_if_django_not_installed
 
 if is_django_installed():
-    from acquiring import domain, models, repositories
-    from tests.django.factories import BlockEventFactory, PaymentAttemptFactory, PaymentMethodFactory
+    from acquiring import domain, storage
+    from tests.storage.django.factories import BlockEventFactory, PaymentAttemptFactory, PaymentMethodFactory
+
+fake = Faker()
 
 
 @skip_if_django_not_installed
 @pytest.mark.django_db
 @pytest.mark.parametrize("status", OperationStatusEnum)
 def test_givenCorrectData_whenCallingRepositoryAdd_thenBlockEventGetsCreated(
     status: OperationStatusEnum,
@@ -21,57 +22,57 @@
     db_payment_method = PaymentMethodFactory(payment_attempt=PaymentAttemptFactory())
     block_event = domain.BlockEvent(
         status=status,
         payment_method_id=db_payment_method.id,
         block_name="test",
     )
 
-    result = repositories.django.BlockEventRepository().add(block_event)
+    result = storage.django.BlockEventRepository().add(block_event)
 
-    db_block_events = models.BlockEvent.objects.all()
+    db_block_events = storage.django.models.BlockEvent.objects.all()
     assert len(db_block_events) == 1
     db_block_event = db_block_events[0]
 
     assert db_block_event.to_domain() == result
 
 
 @skip_if_django_not_installed
 @pytest.mark.django_db
-@given(block_name=st.text(), status=st.sampled_from(OperationStatusEnum))
-@settings(max_examples=100)
+@pytest.mark.parametrize("status", OperationStatusEnum)
 def test_givenAllData_whenCallingRepositoryAdd_thenBlockEventGetsCreated(
-    block_name: str, status: OperationStatusEnum
+    status: OperationStatusEnum,
 ) -> None:
+    block_name = fake.name()
 
     db_payment_method = PaymentMethodFactory(payment_attempt=PaymentAttemptFactory())
     block_event = domain.BlockEvent(
         status=status,
         payment_method_id=db_payment_method.id,
         block_name=block_name,
     )
 
-    result = repositories.django.BlockEventRepository().add(block_event)
+    result = storage.django.BlockEventRepository().add(block_event)
 
-    db_block_event = models.BlockEvent.objects.get(
+    db_block_event = storage.django.models.BlockEvent.objects.get(
         block_name=block_name, payment_method_id=db_payment_method.id, status=status
     )
     assert db_block_event.to_domain() == result
 
 
 @skip_if_django_not_installed
 @pytest.mark.django_db
-def test_givenExistingBlockEventRow_whenCallingRepositoryAdd_thenthenDuplicateErrorGetsRaised() -> None:
+def test_givenExistingBlockEventRow_whenCallingRepositoryAdd_thenthenDuplicatedErrorGetsRaised() -> None:
 
     db_payment_method = PaymentMethodFactory(payment_attempt=PaymentAttemptFactory())
     db_block_event = BlockEventFactory(
         status=OperationStatusEnum.PENDING,
         payment_method_id=db_payment_method.id,
         block_name="test",
     )
     block_event = domain.BlockEvent(
         status=db_block_event.status,
         payment_method_id=db_payment_method.id,
         block_name=db_block_event.block_name,
     )
 
-    with pytest.raises(domain.BlockEvent.DuplicateError):
-        repositories.django.BlockEventRepository().add(block_event)
+    with pytest.raises(domain.BlockEvent.Duplicated):
+        storage.django.BlockEventRepository().add(block_event)
```

### Comparing `acquiring-0.2.0/tests/django/repositories/test_payment_method_repository.py` & `acquiring-0.3.0/tests/domain/flows/test_pay.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,194 +1,181 @@
 import uuid
-from datetime import datetime, timedelta
-from typing import Callable
+from typing import Callable, Optional
 
 import pytest
-from faker import Faker
 
-from acquiring import enums
-from acquiring.utils import is_django_installed
-from tests.django.utils import skip_if_django_not_installed
-
-fake = Faker()
-
-if is_django_installed():
-    from django.utils import timezone  # TODO replace with native aware Python datetime object
-
-    from acquiring import domain, models, repositories
-    from tests.django.factories import (
-        PaymentAttemptFactory,
-        PaymentMethodFactory,
-        PaymentOperationFactory,
-        TokenFactory,
-    )
-
-
-@skip_if_django_not_installed
-@pytest.mark.django_db
-def test_givenCorrectData_whenCallingRepositoryAdd_thenPaymentMethodGetsCreated(
-    django_assert_num_queries: Callable,
-) -> None:
-
-    payment_attempt = PaymentAttemptFactory()
-    data = domain.DraftPaymentMethod(
-        payment_attempt=payment_attempt.to_domain(),
-        confirmable=True,
-    )
-
-    with django_assert_num_queries(7):
-        result = repositories.django.PaymentMethodRepository().add(data)
-
-    db_payment_methods = models.PaymentMethod.objects.all()
-    assert len(db_payment_methods) == 1
-    db_payment_method = db_payment_methods[0]
-
-    assert db_payment_method.id == result.id
-    assert db_payment_method.created_at == result.created_at
-    assert db_payment_method.to_domain() == result
-
-
-@skip_if_django_not_installed
-@pytest.mark.django_db
-@pytest.mark.parametrize("confirmable", [True, False])
-def test_givenTokenData_whenCallingRepositoryAdd_thenTokenGetsCreated(
-    django_assert_num_queries: Callable, confirmable: bool
-) -> None:
-
-    payment_attempt = PaymentAttemptFactory()
-    data = domain.DraftPaymentMethod(
-        payment_attempt=payment_attempt.to_domain(),
-        confirmable=confirmable,
-        token=domain.Token(
-            created_at=timezone.now(),
-            token=fake.sha256(raw_output=False),
-            expires_at=timezone.now() + timedelta(days=365),
-            fingerprint=fake.sha256(),
-            metadata={"customer_id": str(uuid.uuid4())},
-        ),
-    )
-
-    with django_assert_num_queries(8):
-        result = repositories.django.PaymentMethodRepository().add(data)
-
-    db_tokens = models.Token.objects.all()
-    assert len(db_tokens) == 1
-    db_token = db_tokens[0]
-
-    db_payment_methods = models.PaymentMethod.objects.all()
-    assert len(db_payment_methods) == 1
-    db_payment_method = db_payment_methods[0]
-
-    assert db_token.payment_method == db_payment_method
-
-    assert result.token == db_token.to_domain()
-
-
-@skip_if_django_not_installed
-@pytest.mark.django_db
-def test_givenExistingPaymentMethodRow_whenCallingRepositoryGet_thenPaymentGetsRetrieved(
-    django_assert_num_queries: Callable,
-) -> None:
-    db_payment_attempt = PaymentAttemptFactory()
-    db_payment_method = PaymentMethodFactory(payment_attempt=db_payment_attempt)
-    db_token = TokenFactory(
-        token=fake.sha256(),
-        created_at=timezone.now(),
-    )
-    db_payment_method.token = db_token
-    db_payment_method.save()
-    PaymentOperationFactory.create(
-        payment_method_id=db_payment_method.id,
-        status=enums.OperationStatusEnum.STARTED,
-        type=enums.OperationTypeEnum.INITIALIZE,
-    )
-    PaymentOperationFactory.create(
-        payment_method_id=db_payment_method.id,
-        status=enums.OperationStatusEnum.COMPLETED,
-        type=enums.OperationTypeEnum.INITIALIZE,
-    )
-
-    with django_assert_num_queries(4):
-        result = repositories.django.PaymentMethodRepository().get(id=db_payment_method.id)
-
-    assert result == db_payment_method.to_domain()
-
-
-@skip_if_django_not_installed
-@pytest.mark.django_db
-def test_givenNonExistingPaymentMethodRow_whenCallingRepositoryGet_thenDoesNotExistGetsRaise(
-    django_assert_num_queries: Callable,
-) -> None:
-    payment_attempt = domain.PaymentAttempt(
-        id=uuid.uuid4(),
-        created_at=datetime.now(),
-        amount=10,
-        currency="USD",
-        payment_method_ids=[],
-    )
-
-    payment_method = domain.PaymentMethod(
-        id=uuid.uuid4(),
+from acquiring import domain, protocols
+from acquiring.enums import OperationStatusEnum, OperationTypeEnum
+from tests.domain import factories
+
+COMPLETED_STATUS = [OperationStatusEnum.COMPLETED]
+
+PENDING_STATUS = [OperationStatusEnum.PENDING]
+
+FAILED_STATUS = [
+    OperationStatusEnum.STARTED,
+    OperationStatusEnum.REQUIRES_ACTION,
+    OperationStatusEnum.FAILED,
+    OperationStatusEnum.NOT_PERFORMED,
+]
+
+
+def test_statusListsAreComplete() -> None:
+    assert set(COMPLETED_STATUS + PENDING_STATUS + FAILED_STATUS) == set(OperationStatusEnum)
+
+
+@pytest.mark.parametrize(
+    "result_status, payment_operation_status",
+    [(OperationStatusEnum.COMPLETED, status) for status in COMPLETED_STATUS]
+    + [(OperationStatusEnum.PENDING, status) for status in PENDING_STATUS]
+    + [(OperationStatusEnum.FAILED, status) for status in FAILED_STATUS],
+)
+def test_givenAValidPaymentMethod_whenInitializeCompletes_thenPaymentFlowCallsPayAndReturnsTheCorrectOperationResponse(
+    fake_block: type[protocols.Block],
+    fake_process_action_block: type[protocols.Block],
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
+    ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_unit_of_work: type[protocols.UnitOfWork],
+    result_status: OperationStatusEnum,
+    payment_operation_status: OperationStatusEnum,
+) -> None:
+    # given a valid payment attempt
+    payment_attempt = factories.PaymentAttemptFactory()
+    payment_method_id = uuid.uuid4()
+    payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
-        created_at=datetime.now(),
-        confirmable=False,
+        id=payment_method_id,
     )
 
-    with django_assert_num_queries(2), pytest.raises(domain.PaymentMethod.DoesNotExist):
-        repositories.django.PaymentMethodRepository().get(id=payment_method.id)
-
-
-@skip_if_django_not_installed
-@pytest.mark.django_db
-def test_givenCorrectTokenDataAndExistingPaymentMethod_whenCallingRepositoryAddToken_thenTokenGetsCreated(
-    django_assert_num_queries: Callable,
-) -> None:
-
-    db_payment_attempt = PaymentAttemptFactory()
-    db_payment_method = PaymentMethodFactory(payment_attempt_id=db_payment_attempt.id)
-    payment_method = db_payment_method.to_domain()
-    token = domain.Token(created_at=timezone.now(), token=fake.sha256())
-
-    with django_assert_num_queries(5):
-        result = repositories.django.PaymentMethodRepository().add_token(
-            payment_method=payment_method,
-            token=token,
-        )
-
-    db_tokens = models.Token.objects.all()
-    assert len(db_tokens) == 1
-    db_token = db_tokens[0]
-
-    assert db_token.to_domain() == token
-    assert payment_method.token == token
-
-    assert result == payment_method
-
-
-# TODO Turn pytest.mark.django_db into skip if when pytest-django is not installed
-@skip_if_django_not_installed
-@pytest.mark.django_db
-def test_givenNonExistingPaymentMethodRow_whenCallingRepositoryAddToken_thenDoesNotExistGetsRaise(
-    django_assert_num_queries: Callable,
-) -> None:
-
-    payment_attempt = domain.PaymentAttempt(
-        id=uuid.uuid4(),
-        created_at=datetime.now(),
-        amount=10,
-        currency="USD",
-        payment_method_ids=[],
-    )
-
-    payment_method = domain.PaymentMethod(
-        id=uuid.uuid4(),
+    # when Initializing
+    result = domain.PaymentFlow(
+        unit_of_work=fake_unit_of_work(
+            payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
+            payment_operation_repository_class=fake_payment_operation_repository_class([]),
+            block_event_repository_class=fake_block_event_repository_class([]),
+            transaction_repository_class=fake_transaction_repository_class([]),
+        ),
+        initialize_block=fake_block(  # type:ignore[call-arg]
+            fake_response_status=OperationStatusEnum.COMPLETED,
+            fake_response_actions=[],
+        ),
+        process_action_block=fake_process_action_block(),
+        pay_blocks=[
+            fake_block(fake_response_status=payment_operation_status)  # type:ignore[call-arg]
+        ],
+        after_pay_blocks=[],
+        confirm_block=None,
+        after_confirm_blocks=[],
+    ).initialize(payment_method)
+
+    # then the payment flow returns the correct Operation Response
+    db_payment_operations = payment_method.payment_operations
+    assert len(db_payment_operations) == 4
+
+    assert db_payment_operations[0].type == OperationTypeEnum.INITIALIZE
+    assert db_payment_operations[0].status == OperationStatusEnum.STARTED
+
+    assert db_payment_operations[1].type == OperationTypeEnum.INITIALIZE
+    assert db_payment_operations[1].status == OperationStatusEnum.COMPLETED
+
+    assert db_payment_operations[2].type == OperationTypeEnum.PAY
+    assert db_payment_operations[2].status == OperationStatusEnum.STARTED
+
+    assert db_payment_operations[3].type == OperationTypeEnum.PAY
+    assert db_payment_operations[3].status == result_status
+
+    assert result.type == OperationTypeEnum.PAY
+    assert result.status == result_status
+    assert result.actions == []
+    assert result.payment_method is not None
+    assert result.payment_method.id == payment_method.id
+
+
+def test_givenAValidPaymentMethod_whenPayCompletesWithActions_thenPaymentFlowReturnsAnOperationResponseWithActions(
+    fake_block: type[protocols.Block],
+    fake_process_action_block: type[protocols.Block],
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
+    ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_unit_of_work: type[protocols.UnitOfWork],
+) -> None:
+    # given a valid payment attempt
+    payment_attempt = factories.PaymentAttemptFactory()
+    payment_method_id = uuid.uuid4()
+    payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
-        created_at=datetime.now(),
-        confirmable=False,
+        id=payment_method_id,
     )
-    token = domain.Token(created_at=timezone.now(), token=fake.sha256())
+    action = {"test": "action"}
 
-    with django_assert_num_queries(2), pytest.raises(domain.PaymentMethod.DoesNotExist):
-        repositories.django.PaymentMethodRepository().add_token(
-            payment_method=payment_method,
-            token=token,
-        )
+    # when Initializing
+    result = domain.PaymentFlow(
+        unit_of_work=fake_unit_of_work(
+            payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
+            payment_operation_repository_class=fake_payment_operation_repository_class([]),
+            block_event_repository_class=fake_block_event_repository_class([]),
+            transaction_repository_class=fake_transaction_repository_class([]),
+        ),
+        initialize_block=fake_block(  # type:ignore[call-arg]
+            fake_response_status=OperationStatusEnum.COMPLETED,
+            fake_response_actions=[],
+        ),
+        process_action_block=fake_process_action_block(),
+        pay_blocks=[
+            fake_block(  # type:ignore[call-arg]
+                fake_response_status=OperationStatusEnum.PENDING,
+                fake_response_actions=[action],
+            )
+        ],
+        after_pay_blocks=[],
+        confirm_block=None,
+        after_confirm_blocks=[],
+    ).initialize(payment_method)
+
+    # then the payment flow returns the correct Operation Response
+    db_payment_operations = payment_method.payment_operations
+    assert len(db_payment_operations) == 4
+
+    assert db_payment_operations[0].type == OperationTypeEnum.INITIALIZE
+    assert db_payment_operations[0].status == OperationStatusEnum.STARTED
+
+    assert db_payment_operations[1].type == OperationTypeEnum.INITIALIZE
+    assert db_payment_operations[1].status == OperationStatusEnum.COMPLETED
+
+    assert db_payment_operations[2].type == OperationTypeEnum.PAY
+    assert db_payment_operations[2].status == OperationStatusEnum.STARTED
+
+    assert db_payment_operations[3].type == OperationTypeEnum.PAY
+    assert db_payment_operations[3].status == OperationStatusEnum.PENDING
+
+    assert result.type == OperationTypeEnum.PAY
+    assert result.status == OperationStatusEnum.PENDING
+    assert result.actions == [action]
+    assert result.payment_method is not None
+    assert result.payment_method.id == payment_method.id
```

### Comparing `acquiring-0.2.0/tests/django/repositories/test_payment_operation_repository.py` & `acquiring-0.3.0/tests/storage/django/repositories/test_payment_operation_repository.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,67 @@
+from itertools import product
+
 import pytest
-from hypothesis import given, settings
-from hypothesis import strategies as st
 
 from acquiring.enums import OperationStatusEnum, OperationTypeEnum
 from acquiring.utils import is_django_installed
-from tests.django.utils import skip_if_django_not_installed
+from tests.storage.utils import skip_if_django_not_installed
 
 if is_django_installed():
-    from acquiring import domain, models, repositories
-    from tests.django.factories import PaymentAttemptFactory, PaymentMethodFactory, PaymentOperationFactory
+    from acquiring import domain, storage
+    from tests.storage.django.factories import PaymentAttemptFactory, PaymentMethodFactory, PaymentOperationFactory
 
 
 @skip_if_django_not_installed
 @pytest.mark.django_db
-@given(
-    payment_operation_type=st.sampled_from(OperationTypeEnum),
-    payment_operation_status=st.sampled_from(OperationStatusEnum),
+@pytest.mark.parametrize(
+    "payment_operation_type, payment_operation_status", product(OperationTypeEnum, OperationStatusEnum)
 )
-@settings(max_examples=100)
 def test_givenExistingPaymentMethodRow_whenCallingRepositoryAdd_thenPaymentOperationGetsCreated(
     payment_operation_type: OperationTypeEnum,
     payment_operation_status: OperationStatusEnum,
 ) -> None:
     # Given existing payment method row in payment methods table
     db_payment_attempt = PaymentAttemptFactory()
     db_payment_method = PaymentMethodFactory(payment_attempt_id=db_payment_attempt.id)
     payment_method = db_payment_method.to_domain()
 
     # When calling PaymentOperationRepository.add_payment_operation
-    repositories.django.PaymentOperationRepository().add(
+    storage.django.PaymentOperationRepository().add(
         payment_method=payment_method,
         type=payment_operation_type,
         status=payment_operation_status,
     )
 
     # Then PaymentOperation gets created
-    payment_operation = models.PaymentOperation.objects.get(
+    payment_operation = storage.django.models.PaymentOperation.objects.get(
         payment_method_id=db_payment_method.id,
         status=payment_operation_status,
         type=payment_operation_type,
     )
 
     # And payment method gets the payment operation added after add_payment_operation
     assert len(payment_method.payment_operations) == 1
     assert payment_method.payment_operations[0] == payment_operation.to_domain()
 
 
 @skip_if_django_not_installed
 @pytest.mark.django_db
-def test_givenExistingPaymentOperationRow_whenCallingRepositoryAdd_thenthenDuplicateErrorGetsRaised() -> None:
+def test_givenExistingPaymentOperationRow_whenCallingRepositoryAdd_thenthenDuplicatedErrorGetsRaised() -> None:
 
     db_payment_attempt = PaymentAttemptFactory()
     db_payment_method = PaymentMethodFactory(payment_attempt_id=db_payment_attempt.id)
     payment_method = db_payment_method.to_domain()
 
     # given existing payment operation
     PaymentOperationFactory(
         payment_method_id=payment_method.id,
         type=OperationTypeEnum.INITIALIZE,
         status=OperationStatusEnum.STARTED,
     )
 
-    with pytest.raises(domain.PaymentOperation.DuplicateError):
-        repositories.django.PaymentOperationRepository().add(
+    with pytest.raises(domain.PaymentOperation.Duplicated):
+        storage.django.PaymentOperationRepository().add(
             payment_method=payment_method,
             type=OperationTypeEnum.INITIALIZE,
             status=OperationStatusEnum.STARTED,
         )
```

### Comparing `acquiring-0.2.0/tests/django/repositories/test_transaction_repository.py` & `acquiring-0.3.0/tests/storage/django/repositories/test_transaction_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Callable
 
 import pytest
 from faker import Faker
 
 from acquiring.utils import is_django_installed
-from tests.django.utils import skip_if_django_not_installed
+from tests.storage.utils import skip_if_django_not_installed
 
 fake = Faker()
 
 
 if is_django_installed():
     from django.utils import timezone
 
-    from acquiring import domain, models, repositories
-    from tests.django.factories import PaymentAttemptFactory, PaymentMethodFactory
+    from acquiring import domain, storage
+    from tests.storage.django.factories import PaymentAttemptFactory, PaymentMethodFactory
 
 
 @skip_if_django_not_installed
 @pytest.mark.django_db
 def test_givenCorrectData_whenCallingRepositoryAdd_thenPaymentOperationGetsCreated(
     django_assert_num_queries: Callable,
 ) -> None:
@@ -28,15 +28,15 @@
         timestamp=timezone.now(),
         provider_name=fake.company(),
         payment_method_id=db_payment_method.id,
         raw_data={},
     )
 
     with django_assert_num_queries(1):
-        repositories.django.TransactionRepository().add(
+        storage.django.TransactionRepository().add(
             transaction=transaction,
         )
 
-    assert models.Transaction.objects.count() == 1
-    db_transaction = models.Transaction.objects.first()
+    assert storage.django.models.Transaction.objects.count() == 1
+    db_transaction = storage.django.models.Transaction.objects.first()
 
     assert transaction == db_transaction.to_domain()
```

### Comparing `acquiring-0.2.0/tests/django/test_migrations.py` & `acquiring-0.3.0/tests/storage/django/test_migrations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from acquiring.utils import is_django_installed
-from tests.django.utils import skip_if_django_not_installed
+from tests.storage.utils import skip_if_django_not_installed
 
 if is_django_installed():
     from django_test_migrations.plan import all_migrations, nodes_to_tuples
 
 
 @skip_if_django_not_installed
 @pytest.mark.django_db
```

### Comparing `acquiring-0.2.0/tests/domain/factories.py` & `acquiring-0.3.0/tests/domain/factories.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,7 +22,12 @@
 class PaymentMethodFactory(factory.Factory):
     id = factory.LazyAttribute(lambda _: fake.uuid4())
     created_at = factory.LazyAttribute(lambda _: datetime.now())
     confirmable = False
 
     class Meta:
         model = domain.PaymentMethod
+
+
+class PaymentOperationFactory(factory.Factory):
+    class Meta:
+        model = domain.PaymentOperation
```

### Comparing `acquiring-0.2.0/tests/domain/flows/test_after_confirm.py` & `acquiring-0.3.0/tests/domain/flows/test_after_confirm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 from datetime import datetime
-from typing import Callable, Optional, Type
+from typing import Callable, Optional
 
 import pytest
 
 from acquiring import domain, protocols
 from acquiring.domain import decision_logic as dl
 from acquiring.enums import OperationStatusEnum, OperationTypeEnum
 from tests.domain import factories
@@ -28,23 +28,31 @@
 @pytest.mark.parametrize(
     "result_status, payment_operation_status",
     [(OperationStatusEnum.COMPLETED, status) for status in COMPLETED_STATUS]
     + [(OperationStatusEnum.PENDING, status) for status in PENDING_STATUS]
     + [(OperationStatusEnum.FAILED, status) for status in FAILED_STATUS],
 )
 def test_givenAValidPaymentMethod_whenAfterConfirmingCompletes_thenPaymentFlowReturnsTheCorrectOperationResponse(
-    fake_block: Type[protocols.AbstractBlock],
-    fake_process_action_block: Type[protocols.AbstractBlock],
-    fake_payment_method_repository: Callable[
-        [Optional[list[protocols.AbstractPaymentMethod]]],
-        protocols.AbstractRepository,
-    ],
-    fake_payment_operation_repository: Callable[
-        [Optional[list[protocols.AbstractPaymentOperation]]],
-        protocols.AbstractRepository,
+    fake_unit_of_work: type[protocols.UnitOfWork],
+    fake_block: type[protocols.Block],
+    fake_process_action_block: type[protocols.Block],
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]], type[protocols.Repository]
+    ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
     ],
     result_status: OperationStatusEnum,
     payment_operation_status: OperationStatusEnum,
 ) -> None:
 
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
@@ -94,16 +102,20 @@
                 payment_method_id=payment_method_id,
             ),
         ],
     )
 
     # when Confirming
     result = domain.PaymentFlow(
-        payment_method_repository=fake_payment_method_repository([payment_method]),
-        payment_operation_repository=fake_payment_operation_repository([]),
+        unit_of_work=fake_unit_of_work(
+            payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
+            payment_operation_repository_class=fake_payment_operation_repository_class([]),
+            block_event_repository_class=fake_block_event_repository_class([]),
+            transaction_repository_class=fake_transaction_repository_class([]),
+        ),
         initialize_block=fake_block(  # type:ignore[call-arg]
             fake_response_status=OperationStatusEnum.COMPLETED,
             fake_response_actions=[],
         ),
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
@@ -153,39 +165,52 @@
     assert result.status == result_status
     assert result.actions == []
     assert result.payment_method is not None
     assert result.payment_method.id == payment_method_id
 
 
 def test_givenAPaymentMethodThatCannotAfterConfirm_whenAfterConfirming_thenPaymentFlowReturnsAFailedStatusOperationResponse(
-    fake_block: Type[protocols.AbstractBlock],
-    fake_process_action_block: Type[protocols.AbstractBlock],
-    fake_payment_method_repository: Callable[
-        [Optional[list[protocols.AbstractPaymentMethod]]],
-        protocols.AbstractRepository,
-    ],
-    fake_payment_operation_repository: Callable[
-        [Optional[list[protocols.AbstractPaymentOperation]]],
-        protocols.AbstractRepository,
+    fake_block: type[protocols.Block],
+    fake_process_action_block: type[protocols.Block],
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
+    ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
     ],
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_unit_of_work: type[protocols.UnitOfWork],
 ) -> None:
     # Given a payment method that cannot initialize
     payment_attempt = factories.PaymentAttemptFactory()
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=False,
     )
     assert dl.can_after_confirm(payment_method) is False
 
     # When Initializing
     result = domain.PaymentFlow(
-        payment_method_repository=fake_payment_method_repository([payment_method]),
-        payment_operation_repository=fake_payment_operation_repository([]),
+        unit_of_work=fake_unit_of_work(
+            payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
+            payment_operation_repository_class=fake_payment_operation_repository_class([]),
+            block_event_repository_class=fake_block_event_repository_class([]),
+            transaction_repository_class=fake_transaction_repository_class([]),
+        ),
         initialize_block=fake_block(),
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=fake_block(),
         after_confirm_blocks=[],
     ).after_confirm(payment_method)
@@ -193,24 +218,33 @@
     # then the payment flow returns a failed status operation response
     assert result.type == OperationTypeEnum.AFTER_CONFIRM
     assert result.status == OperationStatusEnum.FAILED
     result.error_message == "PaymentMethod cannot go through this operation"
 
 
 def test_givenANonExistingPaymentMethod_whenAfterConfirming_thenPaymentFlowReturnsAFailedStatusOperationResponse(
-    fake_block: Type[protocols.AbstractBlock],
-    fake_process_action_block: Type[protocols.AbstractBlock],
-    fake_payment_method_repository: Callable[
-        [Optional[list[protocols.AbstractPaymentMethod]]],
-        protocols.AbstractRepository,
-    ],
-    fake_payment_operation_repository: Callable[
-        [Optional[list[protocols.AbstractPaymentOperation]]],
-        protocols.AbstractRepository,
+    fake_block: type[protocols.Block],
+    fake_process_action_block: type[protocols.Block],
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
+    ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
     ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_unit_of_work: type[protocols.UnitOfWork],
 ) -> None:
 
     payment_attempt = domain.PaymentAttempt(
         id=uuid.uuid4(),
         created_at=datetime.now(),
         amount=10,
         currency="USD",
@@ -222,16 +256,20 @@
         payment_attempt=payment_attempt,
         created_at=datetime.now(),
         confirmable=False,
     )
 
     # When Confirming
     result = domain.PaymentFlow(
-        payment_method_repository=fake_payment_method_repository([payment_method]),
-        payment_operation_repository=fake_payment_operation_repository([]),
+        unit_of_work=fake_unit_of_work(
+            payment_method_repository_class=fake_payment_method_repository_class([payment_method]),
+            payment_operation_repository_class=fake_payment_operation_repository_class([]),
+            block_event_repository_class=fake_block_event_repository_class([]),
+            transaction_repository_class=fake_transaction_repository_class([]),
+        ),
         initialize_block=fake_block(),
         process_action_block=fake_process_action_block(),
         pay_blocks=[],
         after_pay_blocks=[],
         confirm_block=None,
         after_confirm_blocks=[],
     ).after_confirm(payment_method)
```

### Comparing `acquiring-0.2.0/tests/domain/providers/test_wrapped_by_transaction.py` & `acquiring-0.3.0/tests/domain/providers/test_wrapped_by_transaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,19 +7,32 @@
 
 from acquiring import domain, enums, protocols
 from tests.domain import factories
 
 fake = Faker()
 
 
-def test_givenValidFunction_whenDecoratedWithwrapped_by_transaction_thenTransactionGetsCorrectlyCreated(  # type:ignore[misc]
-    fake_transaction_repository: Callable[
-        ...,
-        protocols.AbstractRepository,
+def test_givenValidFunction_whenDecoratedWithwrapped_by_transaction_thenTransactionGetsCorrectlyCreated(
+    fake_payment_method_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
     ],
+    fake_transaction_repository_class: Callable[
+        [Optional[list[protocols.PaymentMethod]]],
+        type[protocols.Repository],
+    ],
+    fake_payment_operation_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_block_event_repository_class: Callable[
+        [Optional[list[protocols.PaymentOperation]]],
+        type[protocols.Repository],
+    ],
+    fake_unit_of_work: type[protocols.UnitOfWork],
 ) -> None:
 
     external_id = "external"
     timestamp = datetime.now()
     raw_data = fake.pydict()
     provider_name = fake.company()
 
@@ -30,23 +43,24 @@
         raw_data: dict
         status: str
 
     @dataclass
     class FakeAdapter:
         base_url: str
         provider_name: str
-        transaction_repository: protocols.AbstractRepository
 
         @domain.wrapped_by_transaction
         def do_something(
-            self: protocols.AbstractAdapter,
-            payment_method: protocols.AbstractPaymentMethod,
+            self: protocols.Adapter,
+            unit_of_work: protocols.UnitOfWork,
+            payment_method: protocols.PaymentMethod,
             *args: Sequence,
             **kwargs: dict,
-        ) -> protocols.AbstractAdapterResponse:
+        ) -> protocols.AdapterResponse:
+            """This is the expected doc"""
 
             return FakeAdapterResponse(
                 external_id=external_id,
                 timestamp=timestamp,
                 raw_data=raw_data,
                 status=enums.OperationStatusEnum.COMPLETED,
             )
@@ -55,60 +69,32 @@
     payment_method_id = uuid.uuid4()
     payment_method = factories.PaymentMethodFactory(
         payment_attempt=payment_attempt,
         id=payment_method_id,
         confirmable=True,
     )
 
-    transaction_repository = fake_transaction_repository()
+    unit_of_work = fake_unit_of_work(
+        payment_method_repository_class=fake_payment_method_repository_class([]),
+        payment_operation_repository_class=fake_payment_operation_repository_class([]),
+        block_event_repository_class=fake_block_event_repository_class([]),
+        transaction_repository_class=fake_transaction_repository_class([]),
+    )
 
     FakeAdapter(
         base_url=fake.url(),
         provider_name=provider_name,
-        transaction_repository=transaction_repository,
-    ).do_something(payment_method)
+    ).do_something(unit_of_work, payment_method)
 
-    transactions: list[protocols.AbstractTransaction] = transaction_repository.units  # type:ignore[attr-defined]
+    transactions: list[protocols.Transaction] = unit_of_work.transaction_units  # type:ignore[attr-defined]
     assert len(transactions) == 1
 
     assert transactions[0] == domain.Transaction(
         external_id=external_id,
         timestamp=timestamp,
         raw_data=raw_data,
         provider_name=provider_name,
         payment_method_id=payment_method.id,
     )
 
-
-def test_givenValidFunction_whenDecoratedWithwrapped_by_transaction_thenNameAndDocsArePreserved() -> None:
-
-    @dataclass(match_args=False)
-    class FakeAdapterResponse:
-        external_id: Optional[str]
-        timestamp: Optional[datetime]
-        raw_data: dict
-        status: str
-
-    @dataclass
-    class FakeAdapter:
-        base_url: str
-        provider_name: str
-        transaction_repository: protocols.AbstractRepository
-
-        @domain.wrapped_by_transaction
-        def do_something(
-            self: protocols.AbstractAdapter,
-            payment_method: protocols.AbstractPaymentMethod,
-            *args: Sequence,
-            **kwargs: dict,
-        ) -> protocols.AbstractAdapterResponse:
-            """This is the expected doc"""
-
-            return FakeAdapterResponse(
-                external_id="external",
-                timestamp=datetime.now(),
-                raw_data=fake.pydict(),
-                status=enums.OperationStatusEnum.COMPLETED,
-            )
-
     assert FakeAdapter.do_something.__name__ == "do_something"
     assert FakeAdapter.do_something.__doc__ == "This is the expected doc"
```

### Comparing `acquiring-0.2.0/tests/tacit/test_files.py` & `acquiring-0.3.0/tests/tacit/test_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import enum
 import importlib.util
 import inspect
 import os
 from typing import Protocol
+
 from acquiring import protocols
 
 
 def test_allProtocolFilesContainSubclassesOfDecoratorProtocolOrEnum() -> None:
     project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
     acquiring_dir = os.path.join(project_dir, "acquiring")
     for root, dirs, files in os.walk(acquiring_dir):
@@ -24,21 +25,21 @@
                         ) or issubclass(
                             obj, enum.Enum
                         ), f"class {name} is neither a Protocol nor an Enum"
                     elif inspect.isfunction(obj) and obj.__module__ == module_name:  # A non-imported function
                         assert hasattr(obj, "__call__"), f"function {name} is not a decorator"
 
 
-def test_allRepositoryFilesContainSubclassesOfAbstractRepository() -> None:
+def test_allRepositoryFilesContainSubclassesOfRepository() -> None:
     project_dir = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
     acquiring_dir = os.path.join(project_dir, "acquiring")
     for root, dirs, files in os.walk(acquiring_dir):
         for file in files:
             if file.endswith("repositories.py"):
                 file_path = os.path.join(root, file)
                 module_name = os.path.splitext(os.path.basename(file_path))[0]
                 spec = importlib.util.spec_from_file_location(module_name, file_path)
                 module = importlib.util.module_from_spec(spec)  # type:ignore[arg-type]
                 spec.loader.exec_module(module)  # type:ignore[union-attr]
                 for name, obj in inspect.getmembers(module):
                     if inspect.isclass(obj) and obj.__module__ == module_name:  # A non-imported class
-                        assert issubclass(obj, protocols.AbstractRepository), f"class {name} is not a repository"
+                        assert issubclass(obj, protocols.Repository), f"class {name} is not a repository"
```

### Comparing `acquiring-0.2.0/tox.ini` & `acquiring-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `acquiring-0.2.0/PKG-INFO` & `acquiring-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 Metadata-Version: 2.1
 Name: acquiring
-Version: 0.2.0
+Version: 0.3.0
 Summary: Payment Orchestration Library for Python
 Author-email: Alvaro Duran <alvaro.duranb@hotmail.com>
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Office/Business :: Financial :: Point-Of-Sale
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires-Dist: django>=4.2 ; extra == "django"
+Requires-Dist: sqlalchemy>=1.4 ; extra == "sqlalchemy"
 Project-URL: Home, https://github.com/acquiringlabs/acquiring
+Provides-Extra: django
+Provides-Extra: sqlalchemy
 
 # Acquiring
 
 Payment Orchestration Library for Python.
 
+[![Common Changelog](https://common-changelog.org/badge.svg)](https://common-changelog.org)
+
+
 ## Overview
 
 Acquiring aspires to be a flexible and effective toolkit for building applications that handle money.
+The word "acquiring" is the industry term that means collecting and processing payments from customers.
 
 Some reasons you might want to check it out:
 
 - Stable interface via single PaymentFlow class.
 - Flexible internals that can be customized for any payment method, existing AND non-existing.
 - Platform agnostic (really!), meant to be plugged into your existing Django project easily.
 - Support for all database engines under the Django umbrella.
```

