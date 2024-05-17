# Comparing `tmp/resilient-51.0.1.1.824.tar.gz` & `tmp/resilient-51.0.2.0.974.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resilient-51.0.1.1.824.tar", last modified: Wed Apr  3 15:16:05 2024, max compression
+gzip compressed data, was "resilient-51.0.2.0.974.tar", last modified: Fri May 17 18:36:31 2024, max compression
```

## Comparing `resilient-51.0.1.1.824.tar` & `resilient-51.0.2.0.974.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11169 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/CHANGES
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.098412 resilient-51.0.1.1.824/co3/
--rw-rw-r--   0 travis    (2000) travis    (2000)      377 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/co3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/pyproject.toml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.102412 resilient-51.0.1.1.824/resilient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1029 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11944 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/app_config.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.102412 resilient-51.0.1.1.824/resilient/bin/
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/bin/res_keyring.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    37206 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12447 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3argparse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40264 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1966 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/definitions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17651 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2607 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/resilient/resilient_rest_mock.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.102412 resilient-51.0.1.1.824/resilient.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2024-04-03 15:16:05.000000 resilient-51.0.1.1.824/resilient.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      131 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      367 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-04-03 15:16:04.000000 resilient-51.0.1.1.824/resilient.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2037 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/helpers.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_paths.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      595 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/mock_plugins.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_responses/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_responses/session.JSON
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/.jwk/
--rw-rw-r--   0 travis    (2000) travis    (2000)       79 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)       87 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/API_KEY
--rw-rw-r--   0 travis    (2000) travis    (2000)      104 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/EMAIL
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/EMPTY
--rw-rw-r--   0 travis    (2000) travis    (2000)      120 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/PASSWORD
--rw-rw-r--   0 travis    (2000) travis    (2000)      125 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/shared_mock_data/mock_secrets/URL
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/template_test.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9531 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_app_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3_ii.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21843 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      318 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_co3sslutil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_finfo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11152 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/test_helpers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/xtest_gadget.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/xtest_patch.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      726 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tests/xtest_res_keyring.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 15:16:05.106412 resilient-51.0.1.1.824/tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tools/res_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1129 2024-04-03 15:15:23.000000 resilient-51.0.1.1.824/tox.ini
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.307164 resilient-51.0.2.0.974/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11242 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/CHANGES
+-rw-r--r--   0 travis    (2000) travis    (2000)     4091 2024-05-17 18:36:31.307164 resilient-51.0.2.0.974/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2217 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.299164 resilient-51.0.2.0.974/co3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      488 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/co3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      441 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/pyproject.toml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.299164 resilient-51.0.2.0.974/resilient/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1057 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1141 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11944 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/app_config.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.303164 resilient-51.0.2.0.974/resilient/bin/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/bin/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9088 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/bin/finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7221 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/bin/gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5093 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/bin/res_keyring.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    37206 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12447 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/co3argparse.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40264 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1236 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1966 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/constants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      854 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/definitions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17626 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10055 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2607 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/resilient/resilient_rest_mock.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.307164 resilient-51.0.2.0.974/resilient.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4091 2024-05-17 18:36:31.000000 resilient-51.0.2.0.974/resilient.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1574 2024-05-17 18:36:31.000000 resilient-51.0.2.0.974/resilient.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:31.000000 resilient-51.0.2.0.974/resilient.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      131 2024-05-17 18:36:31.000000 resilient-51.0.2.0.974/resilient.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      415 2024-05-17 18:36:31.000000 resilient-51.0.2.0.974/resilient.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2024-05-17 18:36:31.000000 resilient-51.0.2.0.974/resilient.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2177 2024-05-17 18:36:31.307164 resilient-51.0.2.0.974/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      183 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.303164 resilient-51.0.2.0.974/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4261 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1528 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/helpers.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.303164 resilient-51.0.2.0.974/tests/shared_mock_data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_paths.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.303164 resilient-51.0.2.0.974/tests/shared_mock_data/mock_plugins/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_plugins/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      595 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_plugins/mock_plugins.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.303164 resilient-51.0.2.0.974/tests/shared_mock_data/mock_responses/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3705 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_responses/session.JSON
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.307164 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.307164 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/.jwk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       79 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/.jwk/key.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)       87 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/.jwk/key_unused.jwk
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/API_KEY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      104 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/EMAIL
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/EMPTY
+-rw-rw-r--   0 travis    (2000) travis    (2000)      120 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/PASSWORD
+-rw-rw-r--   0 travis    (2000) travis    (2000)      125 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/PASSWORD_WITH_SPECIAL_CHARS
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/shared_mock_data/mock_secrets/URL
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/template_test.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9531 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/test_app_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9685 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/test_co3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20175 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/test_co3_ii.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21843 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/test_co3base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      318 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/test_co3sslutil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2383 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/test_finfo.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11152 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/test_helpers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2259 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/xtest_gadget.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6988 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/xtest_patch.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      726 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tests/xtest_res_keyring.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-05-17 18:36:31.307164 resilient-51.0.2.0.974/tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10657 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tools/res_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1136 2024-05-17 18:36:00.000000 resilient-51.0.2.0.974/tox.ini
```

### Comparing `resilient-51.0.1.1.824/CHANGES` & `resilient-51.0.2.0.974/CHANGES`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+**2024-05: version 51.0.2.0**
+
+* Added official support for Python 3.12
+
 **2024-04: version 51.0.1.1**
 
 * Updated ``jwcrypto`` dependency requirement to ``~= 1.5.6`` (for Python 3.9 and 3.11) to address CVE-2024-28102
   Note that Python 3.6 and Python 2.7 are no longer receiving security updates and should be moved away from immediately.
   See previous release below for details on our support for Python 3.11
 
 **2024-02: version 51.0.1.0**
```

### Comparing `resilient-51.0.1.1.824/PKG-INFO` & `resilient-51.0.2.0.974/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: resilient
-Version: 51.0.1.1.824
-Summary: Python client module for the IBM SOAR REST API
-Home-page: https://github.com/ibmresilient/resilient-python-api/tree/main/resilient
-Author: IBM SOAR
-License: MIT
-Project-URL: Documentation, https://ibm.biz/soar-docs
-Project-URL: API Docs, https://ibm.biz/soar-python-docs
-Project-URL: IBM Community, https://ibm.biz/soarcommunity
-Project-URL: Change Log, https://ibm.biz/resilient-changes
-Keywords: ibm,soar,resilient,resilient-circuits,circuits,resilient-sdk,sdk
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12,>=2.7
-Description-Content-Type: text/markdown; charset=UTF-8
-
 ![IBM Security](https://raw.githubusercontent.com/ibmresilient/resilient-python-api/master/resilient-sdk/assets/IBM_Security_lockup_pos_RGB.png)
 
 # IBM SOAR Python Library
 
 ## Overview
 This package is a Python client module for the IBM SOAR REST API.
```

### Comparing `resilient-51.0.1.1.824/resilient/LICENSE` & `resilient-51.0.2.0.974/resilient/LICENSE`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/__init__.py` & `resilient-51.0.2.0.974/resilient/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 #!/usr/bin/env python
-# (c) Copyright IBM Corp. 2010, 2017. All Rights Reserved.
+# (c) Copyright IBM Corp. 2010, 2024. All Rights Reserved.
 
-import pkg_resources
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
 
 from .co3 import SimpleClient, \
     SimpleHTTPException, \
     PatchConflictException, \
     get_client, \
     get_config_file, \
```

### Comparing `resilient-51.0.1.1.824/resilient/app_config.py` & `resilient-51.0.2.0.974/resilient/app_config.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/bin/finfo.py` & `resilient-51.0.2.0.974/resilient/bin/finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/bin/gadget.py` & `resilient-51.0.2.0.974/resilient/bin/gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/bin/res_keyring.py` & `resilient-51.0.2.0.974/resilient/bin/res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/co3.py` & `resilient-51.0.2.0.974/resilient/co3.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/co3argparse.py` & `resilient-51.0.2.0.974/resilient/co3argparse.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/co3base.py` & `resilient-51.0.2.0.974/resilient/co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/co3sslutil.py` & `resilient-51.0.2.0.974/resilient/co3sslutil.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/constants.py` & `resilient-51.0.2.0.974/resilient/constants.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/definitions.py` & `resilient-51.0.2.0.974/resilient/definitions.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/helpers.py` & `resilient-51.0.2.0.974/resilient/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,24 +153,22 @@
     """
 
     var = os.getenv(var_to_get)
 
     if not var:
         return {}
 
-    var = mask_special_chars(var)
-    var = unquote_str(var)
     parsed_var = urlparse(var)
 
     return {
         "scheme": parsed_var.scheme,
         "hostname": parsed_var.hostname,
         "port": parsed_var.port,
-        "username": unmask_special_chars(parsed_var.username),
-        "password": unmask_special_chars(parsed_var.password)
+        "username": unquote(parsed_var.username) if parsed_var.username else "",
+        "password": unquote(parsed_var.password) if parsed_var.password else ""
     }
 
 
 def is_in_no_proxy(host, no_proxy_var=constants.ENV_NO_PROXY):
     """
     Return True if `host` is found in `no_proxy_var`
     else returns False
```

### Comparing `resilient-51.0.1.1.824/resilient/patch.py` & `resilient-51.0.2.0.974/resilient/patch.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient/resilient_rest_mock.py` & `resilient-51.0.2.0.974/resilient/resilient_rest_mock.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/resilient.egg-info/SOURCES.txt` & `resilient-51.0.2.0.974/resilient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/setup.cfg` & `resilient-51.0.2.0.974/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -12,44 +12,48 @@
 	IBM Community = https://ibm.biz/soarcommunity
 	Change Log = https://ibm.biz/resilient-changes
 classifiers = 
 	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 keywords = ibm, soar, resilient, resilient-circuits, circuits, resilient-sdk, sdk
 
 [options]
 packages = find:
 include_package_data = True
-python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,<3.12
+python_requires = >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
 setup_requires = setuptools_scm
 platforms = any
 install_requires = 
 	resilient-app-config-plugins
 	
 	retry2            ~= 0.9
 	requests          ~= 2.27
 	requests-toolbelt ~= 1.0
 	six               ~= 1.16
 	
 	keyring           ~= 23.5;   python_version  > "3.6"
 	cachetools        ~= 5.0;    python_version  > "3.6"
-	setuptools        ~= 65.5.1; python_version  > "3.6"
+	setuptools        ~= 69.2.0; python_version  > "3.6"
 	jwcrypto          ~= 1.5.6;  python_version  > "3.6"
 	
 	keyring           ~= 23.4;   python_version == "3.6"
 	cachetools        ~= 2.1;    python_version == "3.6"
 	setuptools        ~= 59.6;   python_version == "3.6"
 	jwcrypto          == 1.5.1;  python_version == "3.6" # see https://github.com/latchset/jwcrypto/pull/340
 	
 	configparser      ~= 4.0;    python_version == "2.7"
 	cachetools        ~= 2.1;    python_version == "2.7"
 	keyring           == 18.0.1; python_version == "2.7"
 	setuptools        ~= 44.0;   python_version == "2.7"
+	
+	importlib_metadata ~= 4.8; python_version == "3.6"
+	importlib_metadata ~= 2.1; python_version == "2.7"
 
 [options.entry_points]
 console_scripts = 
 	finfo = resilient.bin.finfo:main
 	gadget = resilient.bin.gadget:main
 	res-keyring = resilient.bin.res_keyring:main
```

### Comparing `resilient-51.0.1.1.824/tests/conftest.py` & `resilient-51.0.2.0.974/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/helpers.py` & `resilient-51.0.2.0.974/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/shared_mock_data/mock_paths.py` & `resilient-51.0.2.0.974/tests/shared_mock_data/mock_paths.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/shared_mock_data/mock_plugins/mock_plugins.py` & `resilient-51.0.2.0.974/tests/shared_mock_data/mock_plugins/mock_plugins.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/shared_mock_data/mock_responses/session.JSON` & `resilient-51.0.2.0.974/tests/shared_mock_data/mock_responses/session.JSON`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/test_app_config.py` & `resilient-51.0.2.0.974/tests/test_app_config.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/test_co3.py` & `resilient-51.0.2.0.974/tests/test_co3.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 def test_client_put(fx_simple_client):
 
     base_client = fx_simple_client[0]
     requests_adapter = fx_simple_client[1]
 
     test_headers = {"content-type": "application/octet-stream"}
 
-    mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)    
+    mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)
 
     requests_adapter.register_uri('PUT',
                                   mock_uri,
                                   status_code=200,
                                   request_headers=test_headers,
                                   text=json.dumps(test_headers))
 
@@ -69,15 +69,15 @@
 def test_client_put_with_error(fx_simple_client):
 
     base_client = fx_simple_client[0]
     requests_adapter = fx_simple_client[1]
 
     test_headers = {"content-type": "application/octet-stream"}
 
-    mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)    
+    mock_uri = '{0}/rest/orgs/{1}/playbooks/imports'.format(base_client.base_url, base_client.org_id)
 
     requests_adapter.register_uri('PUT',
                                   mock_uri,
                                   status_code=403)
 
     uri = "/playbooks/imports"
```

### Comparing `resilient-51.0.1.1.824/tests/test_co3_ii.py` & `resilient-51.0.2.0.974/tests/test_co3_ii.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/test_co3base.py` & `resilient-51.0.2.0.974/tests/test_co3base.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/test_finfo.py` & `resilient-51.0.2.0.974/tests/test_finfo.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/test_helpers.py` & `resilient-51.0.2.0.974/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/xtest_gadget.py` & `resilient-51.0.2.0.974/tests/xtest_gadget.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/xtest_patch.py` & `resilient-51.0.2.0.974/tests/xtest_patch.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tests/xtest_res_keyring.py` & `resilient-51.0.2.0.974/tests/xtest_res_keyring.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tools/res_utils.py` & `resilient-51.0.2.0.974/tools/res_utils.py`

 * *Files identical despite different names*

### Comparing `resilient-51.0.1.1.824/tox.ini` & `resilient-51.0.2.0.974/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = py27, py36, py39, py311
+envlist = py27, py36, py39, py311, py312
 skip_missing_interpreters=True
 skip_install=true
 skipsdist=true
 
 [testenv]
 passenv=TEST_RESILIENT_*
 deps =
```

