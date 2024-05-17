# Comparing `tmp/resilient_lib-51.0.1.1.824.tar.gz` & `tmp/resilient_lib-51.0.2.0.974.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient_lib-51.0.1.1.824.tar", last modified: Wed Apr  3 15:16:24 2024, max compression
+gzip compressed data, was "resilient_lib-51.0.2.0.974.tar", last modified: Fri May 17 18:36:58 2024, max compression
```

## Comparing `resilient_lib-51.0.1.1.824.tar` & `resilient_lib-51.0.2.0.974.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7635 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.198412 resilient_lib-51.0.1.1.824/resilient_lib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      871 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib/components/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/function_result.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      795 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/integration_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30035 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/poller_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24854 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/requests_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24321 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/resilient_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/templates_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/components/workflow_status.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)      293 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12644 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4491 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7207 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/elements.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/ui/tab.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib/util/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/util/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/util/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      410 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/resilient_lib/util/constants.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2648 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2899 2024-04-03 15:16:24.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      188 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-04-03 15:16:23.000000 resilient_lib-51.0.1.1.824/resilient_lib.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1455 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3114 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/conftest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/tests/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)      119 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/data/default_template.jinja
--rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/data/override_template.jinja
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.202412 resilient_lib-51.0.1.1.824/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.206412 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/cert.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/key.open.pem
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.206412 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__orgs_[0-9]+$.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json
--rw-rw-r--   0 travis    (2000) travis    (2000)  1618280 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      775 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    16122 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__attachment.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      359 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__table_data.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9051 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    17000 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_function_metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_html2markdown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_oauth2_client_credentials_session.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_payload.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13935 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_poller.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38969 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_requests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/test_templates.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:24.210412 resilient_lib-51.0.1.1.824/tests/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2974 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1986 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_conditions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_permissions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tests/ui/test_tab.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1074 2024-04-03 15:15:23.000000 resilient_lib-51.0.1.1.824/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.227164 resilient_lib-51.0.2.0.974/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7708 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/CHANGES
+-rw-r--r--   0 travis    (2000) travis    (2000)     2977 2024-05-17 18:36:58.227164 resilient_lib-51.0.2.0.974/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1727 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.211164 resilient_lib-51.0.2.0.974/resilient_lib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      939 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.215164 resilient_lib-51.0.2.0.974/resilient_lib/components/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1400 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2341 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/function_result.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10468 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      795 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/integration_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8828 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    30035 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/poller_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24854 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/requests_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24321 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/resilient_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23208 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/templates_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1530 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/components/workflow_status.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.215164 resilient_lib-51.0.2.0.974/resilient_lib/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      293 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12644 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/ui/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4491 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/ui/conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7761 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/ui/elements.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3848 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/ui/tab.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.215164 resilient_lib-51.0.2.0.974/resilient_lib/util/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/util/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/util/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      410 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/resilient_lib/util/constants.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.227164 resilient_lib-51.0.2.0.974/resilient_lib.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     2977 2024-05-17 18:36:58.000000 resilient_lib-51.0.2.0.974/resilient_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2899 2024-05-17 18:36:58.000000 resilient_lib-51.0.2.0.974/resilient_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:58.000000 resilient_lib-51.0.2.0.974/resilient_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2024-05-17 18:36:58.000000 resilient_lib-51.0.2.0.974/resilient_lib.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      188 2024-05-17 18:36:58.000000 resilient_lib-51.0.2.0.974/resilient_lib.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-05-17 18:36:58.000000 resilient_lib-51.0.2.0.974/resilient_lib.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1489 2024-05-17 18:36:58.231164 resilient_lib-51.0.2.0.974/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.215164 resilient_lib-51.0.2.0.974/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3114 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/conftest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.219164 resilient_lib-51.0.2.0.974/tests/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      119 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/data/default_template.jinja
+-rw-rw-r--   0 travis    (2000) travis    (2000)      171 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/data/override_template.jinja
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.219164 resilient_lib-51.0.2.0.974/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.219164 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_certs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1996 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_certs/cert.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3247 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_certs/key.open.pem
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.227164 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      604 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1025 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   282455 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      798 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3087 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9043 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       36 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__orgs_[0-9]+$.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1459 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)  1618280 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      775 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3527 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16122 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   180619 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      428 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_POST__attachment.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1974 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      359 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_POST__table_data.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9051 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16990 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1093 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_function_metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11263 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_html2markdown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6802 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_oauth2_client_credentials_session.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1193 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_payload.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13935 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_poller.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38969 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_requests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10291 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/test_templates.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:58.227164 resilient_lib-51.0.2.0.974/tests/ui/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/ui/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3404 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/ui/test_common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1986 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/ui/test_conditions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2197 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/ui/test_permissions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3634 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tests/ui/test_tab.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1081 2024-05-17 18:36:00.000000 resilient_lib-51.0.2.0.974/tox.ini
```

### Comparing `resilient_lib-51.0.1.1.824/CHANGES` & `resilient_lib-51.0.2.0.974/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2024-05: version 51.0.2.0**
+
+* Added official support for Python 3.12
+
 **2024-04: version 51.0.1.1**
 
 * No major changes. Just bumping build number to coincide with other builds
 
 **2024-02: version 51.0.1.0**
 
 * All SOAR Python libraries now officially support Python 3.11
```

### Comparing `resilient_lib-51.0.1.1.824/PKG-INFO` & `resilient_lib-51.0.2.0.974/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: resilient_lib
-Version: 51.0.1.1.824
+Version: 51.0.2.0.974
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-lib-changes
 Keywords: ibm,soar,resilient,resilient-circuits,circuits,resilient-lib,common
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12,>=2.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
 Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: resilient>=51.0.2.0
+Requires-Dist: pytz~=2024.1
+Requires-Dist: deprecated~=1.2
+Requires-Dist: beautifulsoup4~=4.9
+Requires-Dist: jinja2~=3.1; python_version > "3.6"
+Requires-Dist: jinja2~=3.0; python_version == "3.6"
+Requires-Dist: jinja2~=2.0; python_version == "2.7"
 
 ![IBM Security](https://raw.githubusercontent.com/ibmresilient/resilient-python-api/master/resilient-sdk/assets/IBM_Security_lockup_pos_RGB.png)
 
 # IBM SOAR Common Library
 
 
 ## Overview
```

### Comparing `resilient_lib-51.0.1.1.824/README.md` & `resilient_lib-51.0.2.0.974/README.md`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/__init__.py` & `resilient_lib-51.0.2.0.974/resilient_lib/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 
-import pkg_resources
-
 try:
-    __version__ = pkg_resources.get_distribution(__name__).version
-except pkg_resources.DistributionNotFound:
+    from importlib.metadata import distribution, PackageNotFoundError
+except ImportError:
+    from importlib_metadata import distribution, PackageNotFoundError
+try:
+    __version__ = distribution(__name__).version
+except PackageNotFoundError:
     __version__ = None
 
-pkg_resources.declare_namespace(__name__)
-
 from resilient_lib.components.function_result import ResultPayload
 from resilient_lib.components.html2markdown import MarkdownParser
 from resilient_lib.components.requests_common import RequestsCommon, RequestsCommonWithoutSession
 from resilient_lib.components.resilient_common import *
 from resilient_lib.components.workflow_status import get_workflow_status
 from resilient_lib.components.oauth2_client_credentials_session import OAuth2ClientCredentialsSession
 from resilient_lib.components.integration_errors import IntegrationError
```

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/function_metrics.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/function_result.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/function_result.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/html2markdown.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/integration_errors.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/integration_errors.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/oauth2_client_credentials_session.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/poller_common.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/poller_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/requests_common.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/requests_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/resilient_common.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/resilient_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/templates_common.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/templates_common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/components/workflow_status.py` & `resilient_lib-51.0.2.0.974/resilient_lib/components/workflow_status.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/ui/common.py` & `resilient_lib-51.0.2.0.974/resilient_lib/ui/common.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/ui/conditions.py` & `resilient_lib-51.0.2.0.974/resilient_lib/ui/conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/ui/elements.py` & `resilient_lib-51.0.2.0.974/resilient_lib/ui/elements.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,31 +70,34 @@
             "element": self.ELEMENT_TYPE,
             "content": self.api_name
         }
 
 class Header(UIElementBase):
     ELEMENT_TYPE = "header"
 
-    def __init__(self, content):
+    def __init__(self, content, show_link_header=False):
         """
         Headers aren't api_name based, they're "content" based.
         So we use the super class to use its validations but we overwrite
         the Conditions and add a ``content`` variable
 
         :param content: header content to display
+        :param show_link_header: boolean to enable "show link header" in UI for header element; defaults to False
         :type content: str
         """
         super(Header, self).__init__(content)
         self.content = content
+        self.show_link_header = show_link_header if show_link_header else False
         self.conditions = Conditions(self.content)
 
     def as_dto(self):
         return {
             "element": self.ELEMENT_TYPE,
-            "content": self.content
+            "content": self.content,
+            "show_link_header": self.show_link_header
         }
 
 class HTMLBlock(UIElementBase):
     ELEMENT_TYPE = "html"
 
     def __init__(self, content):
         """
@@ -162,38 +165,41 @@
             SHOW_IF = [
                 SelectField("my_select").conditions.has_one_of(["a", "b"])
             ]
 
     """
     ELEMENT_TYPE = "section"
 
-    def __init__(self, element_list, show_if=None):
+    def __init__(self, element_list, show_if=None, show_link_header=False):
         """
         We call super init to validate required fields but otherwise we
         implement all our own methods.
 
         :param element_list: list of fields, datatables, etc.. to include in the section
         :type element_list: list[UIElementBase]
         :param show_if: list of condition DTOs, defaults to None (i.e. show always)
         :type show_if: list[dict], optional
+        :param show_link_header: boolean to enable "show link header" in UI for header element; defaults to False
+        :type show_link_header: bool, optional
         """
         super(Section, self).__init__(None)
         self.fields = element_list if element_list else []
         self.show_if = show_if if show_if else []
+        self.show_link_header = show_link_header if show_link_header else False
 
         assert isinstance(self.fields, list), "'element_list' must be a list"
         assert isinstance(self.show_if, list), "'show_if' must be a list"
         assert all([element.ELEMENT_TYPE != self.ELEMENT_TYPE for element in self.fields]), "Cannot create nested Sections"
 
     def as_dto(self):
         return {
             "element": self.ELEMENT_TYPE,
             "fields": [element.as_dto() for element in self.fields] if self.fields else [],
             "show_if": self.show_if,
-            "show_link_header": False
+            "show_link_header": self.show_link_header
         }
 
     def exists_in(self, fields):
         """
         Given a list of fields of a tab, find if this section (exactly!) already exists.
         """
         full_matches = []
```

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/ui/tab.py` & `resilient_lib-51.0.2.0.974/resilient_lib/ui/tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib/util/config.py` & `resilient_lib-51.0.2.0.974/resilient_lib/util/config.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib.egg-info/PKG-INFO` & `resilient_lib-51.0.2.0.974/resilient_lib.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
-Name: resilient-lib
-Version: 51.0.1.1.824
+Name: resilient_lib
+Version: 51.0.2.0.974
 Summary: Python module with library calls which facilitate the development of Apps for IBM SOAR
 Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient-lib
 Author: IBM SOAR
 License: MIT
 Project-URL: Documentation, https://ibm.biz/soar-docs
 Project-URL: API Docs, https://ibm.biz/soar-python-docs
 Project-URL: IBM Community, https://ibm.biz/soarcommunity
 Project-URL: Change Log, https://ibm.biz/resilient-lib-changes
 Keywords: ibm,soar,resilient,resilient-circuits,circuits,resilient-lib,common
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12,>=2.7
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,>=2.7
 Description-Content-Type: text/markdown; charset=UTF-8
+Requires-Dist: resilient>=51.0.2.0
+Requires-Dist: pytz~=2024.1
+Requires-Dist: deprecated~=1.2
+Requires-Dist: beautifulsoup4~=4.9
+Requires-Dist: jinja2~=3.1; python_version > "3.6"
+Requires-Dist: jinja2~=3.0; python_version == "3.6"
+Requires-Dist: jinja2~=2.0; python_version == "2.7"
 
 ![IBM Security](https://raw.githubusercontent.com/ibmresilient/resilient-python-api/master/resilient-sdk/assets/IBM_Security_lockup_pos_RGB.png)
 
 # IBM SOAR Common Library
 
 
 ## Overview
```

### Comparing `resilient_lib-51.0.1.1.824/resilient_lib.egg-info/SOURCES.txt` & `resilient_lib-51.0.2.0.974/resilient_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/setup.cfg` & `resilient_lib-51.0.2.0.974/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -12,24 +12,25 @@
 	IBM Community = https://ibm.biz/soarcommunity
 	Change Log = https://ibm.biz/resilient-lib-changes
 classifiers = 
 	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 keywords = ibm, soar, resilient, resilient-circuits, circuits, resilient-lib, common
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12
+python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
-	resilient      >= 51.0.1.1
+	resilient      >= 51.0.2.0
 	
 	pytz           ~= 2024.1
 	deprecated     ~= 1.2
 	beautifulsoup4 ~= 4.9
 	
 	jinja2         ~= 3.1; python_version > "3.6"
```

### Comparing `resilient_lib-51.0.1.1.824/tests/conftest.py` & `resilient_lib-51.0.2.0.974/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/cert.pem` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_certs/cert.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_certs/key.open.pem` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_certs/key.open.pem`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__actions.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__attachments.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__const.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__functions.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__incidents_.*.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__layouts.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__rest_session.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__task.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types[\w]*$.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_artifact.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_function_fields.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_GET__types_incident_fields.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_POST__rest_session.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json` & `resilient_lib-51.0.2.0.974/tests/shared_mock_data/mock_responses/200_JSON_PUT__layouts_[0-9]+.json`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/test_common.py` & `resilient_lib-51.0.2.0.974/tests/test_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,47 +104,47 @@
 
         # Test mandatory field is empty string
         with self.assertRaisesRegex(ValueError,
                                     "'empty_input' is mandatory and is not set. You must set this value to run this function"):
             validate_fields(("empty_input"), inputs)
 
         # Test no mandatory fields
-        self.assertEquals(validate_fields([], inputs), expected_output)
+        self.assertEqual(validate_fields([], inputs), expected_output)
 
         # Test getting single input from returned dict
-        self.assertEquals(validate_fields(("bool_input_true"), inputs).get("bool_input_true"), True)
-        self.assertEquals(validate_fields([], inputs).get("bool_input_true"), True)
+        self.assertEqual(validate_fields(("bool_input_true"), inputs).get("bool_input_true"), True)
+        self.assertEqual(validate_fields([], inputs).get("bool_input_true"), True)
 
         # Test getting value defined as False
-        self.assertEquals(validate_fields(["bool_input_false"], inputs).get("bool_input_false"), False)
+        self.assertEqual(validate_fields(["bool_input_false"], inputs).get("bool_input_false"), False)
 
         # Test select + multi-select type fields
-        self.assertEquals(validate_fields(["select_input"], inputs).get("select_input"), "select choice")
-        self.assertEquals(validate_fields([], inputs).get("multi_select_input"),
+        self.assertEqual(validate_fields(["select_input"], inputs).get("select_input"), "select choice")
+        self.assertEqual(validate_fields([], inputs).get("multi_select_input"),
                           ["select choice one", "select choice two"])
 
         # Test 'Text with value string Input' type
-        self.assertEquals(validate_fields(["text_with_value_string"], inputs).get("text_with_value_string"),
+        self.assertEqual(validate_fields(["text_with_value_string"], inputs).get("text_with_value_string"),
                           "mock text")
 
         # Test placeholder
         with self.assertRaisesRegex(ValueError,
                                     "'str_input' is mandatory and still has its placeholder value of 'some text'. You must set this value correctly to run this function"):
             validate_fields(mandatory_fields, inputs)
 
         # Test works with a namedtuple
         inputs_as_named_tuple = namedtuple("fn_inputs", inputs.keys())(*inputs.values())
-        self.assertEquals(validate_fields(("bool_input_true"), inputs_as_named_tuple).get("bool_input_true"), True)
+        self.assertEqual(validate_fields(("bool_input_true"), inputs_as_named_tuple).get("bool_input_true"), True)
 
         validated_named_tuple_inputs_i = validate_fields([], inputs_as_named_tuple)
-        self.assertEquals(validated_named_tuple_inputs_i, expected_output)
+        self.assertEqual(validated_named_tuple_inputs_i, expected_output)
 
         # Test called again on a normalized dict
         validated_named_tuple_inputs_ii = validate_fields([], validated_named_tuple_inputs_i)
-        self.assertEquals(validated_named_tuple_inputs_ii, expected_output)
+        self.assertEqual(validated_named_tuple_inputs_ii, expected_output)
 
     def test_unescape(self):
         # unescape(data)
         test_data = "&lt;-&gt;"
         self.assertEqual(unescape(test_data), '<->')
 
         self.assertEqual(unescape("&ab;xx"), '&ab;xx')
```

### Comparing `resilient_lib-51.0.1.1.824/tests/test_function_metrics.py` & `resilient_lib-51.0.2.0.974/tests/test_function_metrics.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/test_html2markdown.py` & `resilient_lib-51.0.2.0.974/tests/test_html2markdown.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/test_oauth2_client_credentials_session.py` & `resilient_lib-51.0.2.0.974/tests/test_oauth2_client_credentials_session.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/test_payload.py` & `resilient_lib-51.0.2.0.974/tests/test_payload.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/test_poller.py` & `resilient_lib-51.0.2.0.974/tests/test_poller.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/test_requests.py` & `resilient_lib-51.0.2.0.974/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/test_templates.py` & `resilient_lib-51.0.2.0.974/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/ui/test_common.py` & `resilient_lib-51.0.2.0.974/tests/ui/test_common.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     NAME = "test"
     UUID = "test"
     SECTION = "test"
     CONTAINS = [
         Datatable('test'),
         Field('test'),
         Section(
-            element_list=[HTMLBlock("<h1>HTML Header</h1>"), Header("Built-in Header")],
+            element_list=[HTMLBlock("<h1>HTML Header</h1>"), Header("Built-in Header"), Header("Header show link True", show_link_header=True)],
             show_if=[Field("id").conditions.has_value()]
         )
     ]
 
     SHOW_IF = [Field('test').conditions.has_value()]
 
 class TestSubmittedData(object):
@@ -34,17 +34,22 @@
     Tests that payload submitted to the server contains proper tab information.
     """
 
     def test_create_tab(self, fx_soar_adapter):
         create_tab(MockTab, OPTS)
 
         payload = json.loads(fx_soar_adapter.request_history[-1].text)
-        assert MockTab.exists_in(payload.get('content'))
+        assert MockTab.exists_in(payload.get("content"))
         for field in MockTab.CONTAINS:
-            assert field.exists_in(MockTab.get_from_tabs(payload.get('content')).get("fields"))
+            assert field.exists_in(MockTab.get_from_tabs(payload.get("content")).get("fields"))
+
+        # check for header 'show_link_header' settings properly applied.
+        # NOTE: this could be finicky if anything changes in the MockTab, beware
+        assert payload.get("content")[21].get("fields")[-1].get("fields")[1].get("show_link_header") is False
+        assert payload.get("content")[21].get("fields")[-1].get("fields")[2].get("show_link_header") is True
 
     def test_update_tab_disabled(self, fx_soar_adapter):
         create_tab(MockTab, OPTS)
 
         # assert that PUT was called and correct payload present
         assert fx_soar_adapter.call_count == 5
```

### Comparing `resilient_lib-51.0.1.1.824/tests/ui/test_conditions.py` & `resilient_lib-51.0.2.0.974/tests/ui/test_conditions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/ui/test_permissions.py` & `resilient_lib-51.0.2.0.974/tests/ui/test_permissions.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tests/ui/test_tab.py` & `resilient_lib-51.0.2.0.974/tests/ui/test_tab.py`

 * *Files identical despite different names*

### Comparing `resilient_lib-51.0.1.1.824/tox.ini` & `resilient_lib-51.0.2.0.974/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py27, py36, py39, py311
+envlist = py27, py36, py39, py311, py312
 skip_install=true
 skipsdist=true
 skip_missing_interpreters=true
 
 [testenv]
 passenv=TEST_RESILIENT_*
 deps =
```

