# Comparing `tmp/linktest-2.8.2.tar.gz` & `tmp/linktest-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.8.2.tar", last modified: Wed May 15 06:44:02 2024, max compression
+gzip compressed data, was "linktest-2.8.3.tar", last modified: Fri May 17 06:34:38 2024, max compression
```

## Comparing `linktest-2.8.2.tar` & `linktest-2.8.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-15 06:44:02.695959 linktest-2.8.2/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-15 06:44:02.695634 linktest-2.8.2/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-15 06:44:02.692582 linktest-2.8.2/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-15 06:35:55.000000 linktest-2.8.2/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/auto_generate_testcase_list-backup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    28841 2024-05-15 06:37:29.000000 linktest-2.8.2/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-14 06:39:54.000000 linktest-2.8.2/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8676 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102436 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-15 06:35:59.000000 linktest-2.8.2/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-14 06:39:55.000000 linktest-2.8.2/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-15 06:44:02.695225 linktest-2.8.2/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-15 06:44:02.000000 linktest-2.8.2/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-15 06:44:02.696015 linktest-2.8.2/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-15 06:43:57.000000 linktest-2.8.2/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-17 06:34:38.444645 linktest-2.8.3/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-17 06:34:38.444367 linktest-2.8.3/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-17 06:34:38.442035 linktest-2.8.3/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-17 06:28:08.000000 linktest-2.8.3/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/auto_generate_testcase_list-backup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    28841 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10326 2024-05-17 06:28:03.000000 linktest-2.8.3/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-17 06:31:46.000000 linktest-2.8.3/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8899 2024-05-17 06:30:10.000000 linktest-2.8.3/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102436 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4811 2024-05-17 06:31:14.000000 linktest-2.8.3/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-17 06:28:14.000000 linktest-2.8.3/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-15 06:44:46.000000 linktest-2.8.3/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-17 06:34:38.444009 linktest-2.8.3/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-17 06:34:38.000000 linktest-2.8.3/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-17 06:34:38.444695 linktest-2.8.3/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-17 06:34:33.000000 linktest-2.8.3/setup.py
```

### Comparing `linktest-2.8.2/linktest/appium_utils.py` & `linktest-2.8.3/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/auto_generate_testcase_list-backup.py` & `linktest-2.8.3/linktest/auto_generate_testcase_list-backup.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/auto_generate_testcase_list.py` & `linktest-2.8.3/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.8.3/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                         continue
 
                     if not has_run_test_flag:
                         message = (
                             f"\n--- {PROJECT_INFO.project_path + os.sep + file_full_name} 文件中没有找到合法的 `run_test(self, ...)` 方法 ---\n"
                             f" LinkTest 的 DataSet 功能的标准要求: \n"
                             f"  1. CSV 文件及其对应的 Python 文件的文件名必须保持一致\n"
-                            f"  2. Python 文件中必须定义 `run_test(self, ...)` 方法, 并且参数列表中除了 `self` 之外, 必须至少还有一个其他参数\n"
+                            f"  2. Python 文件中必须定义 `run_test(self, ...)` 方法, 并且参数列表中除了 `self` 或 `self: APITestCase` 之外, 必须至少还有一个其他参数\n"
                             f"  3. Python 文件中定义的 `run_test()` 方法的所有参数名（除 `self` 参数外), 都必须存在于对应的 CSV 文件的表头（header）中\n"
                             f"--- 测试用例文件将不会自动生成。如需更多帮助信息，请运行以下命令：python3 run.py --help csv ---\n"
                         )
                         print(message)
 
                         continue
```

### Comparing `linktest-2.8.2/linktest/base_testcase.py` & `linktest-2.8.3/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/clean_data.py` & `linktest-2.8.3/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/conver_xml_into_db.py` & `linktest-2.8.3/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/database_helper.py` & `linktest-2.8.3/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/date_utilities.py` & `linktest-2.8.3/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/doctor.py` & `linktest-2.8.3/linktest/doctor.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/framework_log.py` & `linktest-2.8.3/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/generate_html_log.py` & `linktest-2.8.3/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/get_adb_devices.py` & `linktest-2.8.3/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/get_ios_devices_list.py` & `linktest-2.8.3/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/get_platform_info.py` & `linktest-2.8.3/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/get_project_info.py` & `linktest-2.8.3/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/html_report.py` & `linktest-2.8.3/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/logged_requests.py` & `linktest-2.8.3/linktest/logged_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,40 +52,41 @@
                 if res.status_code == 200:
                     return res
 
             instance.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> cURL Start >>>>>>>>>>>>>>>>>>>>>>>>>")
             instance.logger.info(os.linesep + curlify.to_curl(res.request) + os.linesep)
             instance.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< cURL End <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
-            api_version = ""
-            # 检查响应头部中的各种可能的版本信息
-            api_version_keys = ["version", "Version", "VERSION",
-                                "API-Version", "API-VERSION", "api-version",
-                                "API-Version-Header", "api-version-header", "API-VERSION-HEADER"]
-
-            # ===== log api's version =====
-            for key in api_version_keys:
-                if key in res.headers:
-                    api_version = f"API version found in headers: {res.headers[key]}"
-                    break
-
-            if not api_version:
-                # 如果未在响应头部中找到版本信息，请检查响应体中的各种可能的版本信息
-                try:
-                    response_body = res.json()
-
-                    for key in api_version_keys:
-                        if key in response_body:
-                            api_version = f"API version found in response body: {response_body[key]}"
-                            break
-                except json_func.JSONDecodeError:
-                    instance.logger.warning(os.linesep +  traceback.format_exc() + os.linesep)
-
-            if api_version:
-                instance.logger.info(os.linesep + "- API Version: %s" % api_version)
+            # todo 此处应该做成配置项，是否记录API版本信息，并且 API的version字段应该是可配置的
+            # api_version = ""
+            # # 检查响应头部中的各种可能的版本信息
+            # api_version_keys = ["version", "Version", "VERSION",
+            #                     "API-Version", "API-VERSION", "api-version",
+            #                     "API-Version-Header", "api-version-header", "API-VERSION-HEADER"]
+            #
+            # # ===== log api's version =====
+            # for key in api_version_keys:
+            #     if key in res.headers:
+            #         api_version = f"API version found in headers: {res.headers[key]}"
+            #         break
+            #
+            # if not api_version:
+            #     # 如果未在响应头部中找到版本信息，请检查响应体中的各种可能的版本信息
+            #     try:
+            #         response_body = res.json()
+            #
+            #         for key in api_version_keys:
+            #             if key in response_body:
+            #                 api_version = f"API version found in response body: {response_body[key]}"
+            #                 break
+            #     except json_func.JSONDecodeError:
+            #         instance.logger.warning(os.linesep +  traceback.format_exc() + os.linesep)
+            #
+            # if api_version:
+            #     instance.logger.info(os.linesep + "- API Version: %s" % api_version)
 
             return res
 
         return wrapper
 
     @log_curl
     def get(self, url, params=None, **kwargs):
```

### Comparing `linktest-2.8.2/linktest/main.py` & `linktest-2.8.3/linktest/main.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/memory_usage.py` & `linktest-2.8.3/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/re_func.py` & `linktest-2.8.3/linktest/re_func.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,34 +17,37 @@
     # 1. The string begins with `def` followed by a space.
     # 2. Then comes a valid Python method name, starting with a letter or underscore, followed by any number of letters, numbers, or underscores.
     # 3. Then comes zero or more spaces, followed by a left parenthesis.
     # 4. Then comes zero or more spaces, followed by `self`, then a comma and at least one character (representing at least one argument).
     # 5. Then any number of characters (including zero), followed by a right parenthesis.
     # 6. Finally, zero or more spaces, followed by a colon.
 
-    pattern = r'^def\s+run_test\s*\(\s*self\s*,.+?\):.*$'
+    pattern = r'^def\s+run_test\s*\(\s*self(?:\s*:\s*APITestCase)?\s*,.+?\):.*$'
     match = re.match(pattern, method_string)
 
     file_base_name = os.path.splitext(csv_file_full_path)[0]
 
     if match:
-        arugments_in_method_string = method_string.replace(" ", "").split("self,")[1].split(")")[0].split(",")
+        if method_string.__contains__("self,"):
+            arugments_in_method_string = method_string.replace(" ", "").split("self,")[1].split(")")[0].split(",")
+        if method_string.__contains__("self: APITestCase,"):
+            arugments_in_method_string = method_string.replace(" ", "").split("self:APITestCase,")[1].split(")")[0].split(",")
 
         with open(csv_file_full_path, 'r') as csv_file:
             reader = csv.reader(csv_file, delimiter=detect_delimiter.detect_delimiter(csv_file_full_path))
             headers = next(reader)  # 读取第一行
 
             if set(arugments_in_method_string).issubset(set(headers)):
                 return arugments_in_method_string
             else:
                 miss_arguments_message = (
                     f"\n--- `run_test()` 方法的格式并未满足LinkTest框架的标准要求: ---\n"
                     f" LinkTest 的 DataSet 功能的标准要求: \n"
                     f"  1. CSV 文件及其对应的 Python 文件的文件名必须保持一致\n"
-                    f"  2. Python 文件中必须定义 `run_test(self, ...)` 方法, 并且参数列表中除了 `self` 之外, 必须至少还有一个其他参数\n"
+                    f"  2. Python 文件中必须定义 `run_test(self, ...)` 方法, 并且参数列表中除了 `self`或`self: APITestCase` 之外, 必须至少还有一个其他参数\n"
                     f"  3. Python 文件中定义的 `run_test()` 方法的所有参数名（除 `self` 参数外), 都必须存在于对应的 CSV 文件的表头（header）中\n\n"
                     f" - {file_base_name}.csv 文件的表头内容为: {headers}\n"
                     f" - {file_base_name}.py 文件中定义的 `run_test()` 方法的参数为: {arugments_in_method_string}\n"
                     f"--- 测试用例文件将不会自动生成。如需更多帮助信息，请运行以下命令：python3 run.py --help csv ---\n"
                 )
                 print(miss_arguments_message)
                 return "miss_arguments"
```

### Comparing `linktest-2.8.2/linktest/run.py` & `linktest-2.8.3/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/run_testcase_thread.py` & `linktest-2.8.3/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/scp_report_to_specified_path.py` & `linktest-2.8.3/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/selenium_helper.py` & `linktest-2.8.3/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/timeout_thread.py` & `linktest-2.8.3/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/ui_testcase.py` & `linktest-2.8.3/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/update_config.py` & `linktest-2.8.3/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/webdriver_wrapper.py` & `linktest-2.8.3/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/webdriver_wrapper_chrome.py` & `linktest-2.8.3/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/webdriver_wrapper_edge.py` & `linktest-2.8.3/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/webdriver_wrapper_firefox.py` & `linktest-2.8.3/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/webdriver_wrapper_ie.py` & `linktest-2.8.3/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/webdriver_wrapper_safari.py` & `linktest-2.8.3/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest/xml_report.py` & `linktest-2.8.3/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.2/linktest.egg-info/SOURCES.txt` & `linktest-2.8.3/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

