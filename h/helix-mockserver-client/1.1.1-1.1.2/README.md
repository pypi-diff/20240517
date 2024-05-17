# Comparing `tmp/helix_mockserver_client-1.1.1.tar.gz` & `tmp/helix_mockserver_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helix_mockserver_client-1.1.1.tar", last modified: Sat Dec  2 19:12:30 2023, max compression
+gzip compressed data, was "helix_mockserver_client-1.1.2.tar", last modified: Mon May  6 19:58:05 2024, max compression
```

## Comparing `helix_mockserver_client-1.1.1.tar` & `helix_mockserver_client-1.1.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.116181 helix_mockserver_client-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-12-02 19:12:30.116181 helix_mockserver_client-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-02 19:12:29.000000 helix_mockserver_client-1.1.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.116181 helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-12-02 19:12:30.000000 helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2023-12-02 19:12:30.000000 helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 19:12:30.000000 helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 19:12:30.000000 helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-02 19:12:30.000000 helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-02 19:12:30.000000 helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/mockserver_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/_timing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/mockserver_client/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/exceptions/mock_server_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/exceptions/mock_server_request_not_found_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/match_request_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mock_expectation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mock_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mock_request_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mock_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17730 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mock_requests_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mock_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    45761 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mockserver_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/mockserver_verify_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/mockserver_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-12-02 19:12:30.116181 helix_mockserver_client-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-12-02 19:12:29.000000 helix_mockserver_client-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/from_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file/test_mock_server_from_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/from_file_content_type_form_urlencoded/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_content_type_form_urlencoded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_content_type_form_urlencoded/test_mock_server_content_type_url_formencoded.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_mismatch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_mismatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_expectation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_expectation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:30.112181 helix_mockserver_client-1.1.1/tests/json_unit_ignore_elements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/json_unit_ignore_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5842 2023-12-02 19:12:02.000000 helix_mockserver_client-1.1.1/tests/json_unit_ignore_elements/test_mock_server_json_unit_ignore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.959894 helix_mockserver_client-1.1.2/mockserver_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/_timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.959894 helix_mockserver_client-1.1.2/mockserver_client/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/exceptions/mock_server_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/exceptions/mock_server_request_not_found_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/match_request_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mock_expectation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mock_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mock_request_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mock_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18655 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mock_requests_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mock_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45761 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mockserver_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/mockserver_verify_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/mockserver_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-06 19:58:05.000000 helix_mockserver_client-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.959894 helix_mockserver_client-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/tests/from_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file/test_mock_server_from_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/tests/from_file_content_type_form_urlencoded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_content_type_form_urlencoded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_content_type_form_urlencoded/test_mock_server_content_type_url_formencoded.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_mismatch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_mismatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_expectation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_expectation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 19:58:05.963894 helix_mockserver_client-1.1.2/tests/json_unit_ignore_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/json_unit_ignore_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-05-06 19:57:36.000000 helix_mockserver_client-1.1.2/tests/json_unit_ignore_elements/test_mock_server_json_unit_ignore.py
```

### Comparing `helix_mockserver_client-1.1.1/LICENSE` & `helix_mockserver_client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/Makefile` & `helix_mockserver_client-1.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/PKG-INFO` & `helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: helix_mockserver_client
-Version: 1.1.1
+Name: helix-mockserver-client
+Version: 1.1.2
 Summary: mockserver_client
 Home-page: https://github.com/icanbwell/mockserver_client
 Author: Imran Qureshi
 Author-email: imran.qureshi@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `helix_mockserver_client-1.1.1/README.md` & `helix_mockserver_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/PKG-INFO` & `helix_mockserver_client-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: helix-mockserver-client
-Version: 1.1.1
+Name: helix_mockserver_client
+Version: 1.1.2
 Summary: mockserver_client
 Home-page: https://github.com/icanbwell/mockserver_client
 Author: Imran Qureshi
 Author-email: imran.qureshi@icanbwell.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `helix_mockserver_client-1.1.1/helix_mockserver_client.egg-info/SOURCES.txt` & `helix_mockserver_client-1.1.2/helix_mockserver_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py` & `helix_mockserver_client-1.1.2/mockserver_client/exceptions/mock_server_expectation_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py` & `helix_mockserver_client-1.1.2/mockserver_client/exceptions/mock_server_json_content_mismatch_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/exceptions/mock_server_request_not_found_exception.py` & `helix_mockserver_client-1.1.2/mockserver_client/exceptions/mock_server_request_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mock_expectation.py` & `helix_mockserver_client-1.1.2/mockserver_client/mock_expectation.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mock_request.py` & `helix_mockserver_client-1.1.2/mockserver_client/mock_request.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mock_request_logger.py` & `helix_mockserver_client-1.1.2/mockserver_client/mock_request_logger.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mock_request_response.py` & `helix_mockserver_client-1.1.2/mockserver_client/mock_request_response.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mock_requests_loader.py` & `helix_mockserver_client-1.1.2/mockserver_client/mock_requests_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,14 +168,45 @@
                 path=path,
                 body=json_equals(fhir_request),
             ),
             response=mock_response(body=payload),
             timing=times(1),
             file_path=file_path,
         )
+    elif method == "PUT":
+        id_ = fhir_request["id"]
+        # noinspection PyPep8Naming
+        resourceType = fhir_request["resourceType"]
+        path = f"{('/' + url_prefix) if url_prefix else ''}/4_0_0/{resourceType}/{id_}"
+
+        payload = (
+            json.dumps(
+                [
+                    {
+                        "id": id_,
+                        "updated": True,
+                        "created": False,
+                        "resourceType": resourceType,
+                    }
+                ]
+            )
+            if not response_body
+            else response_body
+        )
+
+        mock_client.expect(
+            request=mock_request(
+                method="PUT",
+                path=path,
+                body=json_equals(fhir_request),
+            ),
+            response=mock_response(body=payload),
+            timing=times(1),
+            file_path=file_path,
+        )
     else:
         if not relative_path:
             id_ = fhir_request["id"]
             # noinspection PyPep8Naming
             resourceType = fhir_request["resourceType"]
             path = (
                 f"{('/' + url_prefix) if url_prefix else ''}/4_0_0/{resourceType}/{id_}"
```

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mock_response.py` & `helix_mockserver_client-1.1.2/mockserver_client/mock_response.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mockserver_client.py` & `helix_mockserver_client-1.1.2/mockserver_client/mockserver_client.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/mockserver_client/mockserver_verify_exception.py` & `helix_mockserver_client-1.1.2/mockserver_client/mockserver_verify_exception.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/setup.py` & `helix_mockserver_client-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/tests/from_file/test_mock_server_from_file.py` & `helix_mockserver_client-1.1.2/tests/from_file/test_mock_server_from_file.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/tests/from_file_content_type_form_urlencoded/test_mock_server_content_type_url_formencoded.py` & `helix_mockserver_client-1.1.2/tests/from_file_content_type_form_urlencoded/test_mock_server_content_type_url_formencoded.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py` & `helix_mockserver_client-1.1.2/tests/from_file_multiple_calls/test_mock_server_from_file_multiple_calls.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py` & `helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_mismatch/test_mock_server_from_file_multiple_calls_mismatch.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py` & `helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_expectation/test_mock_server_from_file_multiple_calls_missing_expectation.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py` & `helix_mockserver_client-1.1.2/tests/from_file_multiple_calls_missing_request/test_mock_server_from_file_multiple_calls_missing_request.py`

 * *Files identical despite different names*

### Comparing `helix_mockserver_client-1.1.1/tests/json_unit_ignore_elements/test_mock_server_json_unit_ignore.py` & `helix_mockserver_client-1.1.2/tests/json_unit_ignore_elements/test_mock_server_json_unit_ignore.py`

 * *Files identical despite different names*

