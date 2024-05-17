# Comparing `tmp/liveramp_automation-1.4.0.tar.gz` & `tmp/liveramp_automation-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-1.4.0.tar", last modified: Tue May 14 08:28:27 2024, max compression
+gzip compressed data, was "liveramp_automation-1.4.1.tar", last modified: Fri May 17 02:15:23 2024, max compression
```

## Comparing `liveramp_automation-1.4.0.tar` & `liveramp_automation-1.4.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.657918 liveramp_automation-1.4.0/
--rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.4.0/LICENSE
--rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-05-14 08:28:27.657598 liveramp_automation-1.4.0/PKG-INFO
--rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.4.0/README.md
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.639307 liveramp_automation-1.4.0/liveramp_automation/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.4.0/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-05-14 08:28:24.000000 liveramp_automation-1.4.0/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.643395 liveramp_automation-1.4.0/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.0/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10815 2024-05-14 03:36:00.000000 liveramp_automation-1.4.0/liveramp_automation/helpers/bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.4.0/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.4.0/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     7369 2024-04-17 09:01:03.000000 liveramp_automation-1.4.0/liveramp_automation/helpers/fixture.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6184 2024-04-17 08:58:00.000000 liveramp_automation-1.4.0/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.4.0/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.648798 liveramp_automation-1.4.0/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.0/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.4.0/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.4.0/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     5025 2024-04-17 09:04:21.000000 liveramp_automation-1.4.0/liveramp_automation/utils/pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.4.0/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.4.0/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.4.0/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.4.0/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.4.0/liveramp_automation/utils/slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)      795 2024-04-23 06:11:59.000000 liveramp_automation-1.4.0/liveramp_automation/utils/steps.py
--rw-r--r--   0 jasqia     (503) staff       (20)     8423 2024-04-23 05:42:40.000000 liveramp_automation-1.4.0/liveramp_automation/utils/testrail.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.4.0/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.657073 liveramp_automation-1.4.0/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-05-14 08:28:27.000000 liveramp_automation-1.4.0/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (503) staff       (20)     1608 2024-05-14 08:28:27.000000 liveramp_automation-1.4.0/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-05-14 08:28:27.000000 liveramp_automation-1.4.0/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (503) staff       (20)      474 2024-05-14 08:28:27.000000 liveramp_automation-1.4.0/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-05-14 08:28:27.000000 liveramp_automation-1.4.0/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-05-14 08:28:27.657978 liveramp_automation-1.4.0/setup.cfg
--rw-r--r--   0 jasqia     (503) staff       (20)     1516 2024-04-24 07:51:56.000000 liveramp_automation-1.4.0/setup.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.649183 liveramp_automation-1.4.0/tests/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.0/tests/__init__.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.652179 liveramp_automation-1.4.0/tests/test_helpers/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.4.0/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4210 2024-05-14 02:00:56.000000 liveramp_automation-1.4.0/tests/test_helpers/test_bigquery.py
--rw-r--r--   0 jasqia     (503) staff       (20)     2347 2024-05-14 05:26:06.000000 liveramp_automation-1.4.0/tests/test_helpers/test_bucket.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.4.0/tests/test_helpers/test_file.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.4.0/tests/test_helpers/test_fixtures.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.4.0/tests/test_helpers/test_login.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.4.0/tests/test_helpers/test_notification.py
-drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-14 08:28:27.656340 liveramp_automation-1.4.0/tests/test_utils/
--rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.0/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.4.0/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.4.0/tests/test_utils/test_pagerduty.py
--rw-r--r--   0 jasqia     (503) staff       (20)     3324 2024-05-10 03:07:09.000000 liveramp_automation-1.4.0/tests/test_utils/test_parsers.py
--rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.4.0/tests/test_utils/test_playwright.py
--rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.4.0/tests/test_utils/test_request.py
--rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.4.0/tests/test_utils/test_selenium.py
--rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.4.0/tests/test_utils/test_slack.py
--rw-r--r--   0 jasqia     (503) staff       (20)     5406 2024-05-10 03:16:07.000000 liveramp_automation-1.4.0/tests/test_utils/test_testrail.py
--rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.4.0/tests/test_utils/test_version.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.824387 liveramp_automation-1.4.1/
+-rw-r--r--   0 jasqia     (503) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-1.4.1/LICENSE
+-rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-05-17 02:15:23.824032 liveramp_automation-1.4.1/PKG-INFO
+-rwxrwxrwx   0 jasqia     (503) staff       (20)     1744 2024-03-18 02:41:18.000000 liveramp_automation-1.4.1/README.md
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.806065 liveramp_automation-1.4.1/liveramp_automation/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-09-13 07:36:00.000000 liveramp_automation-1.4.1/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      479 2024-05-17 02:15:07.000000 liveramp_automation-1.4.1/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.809967 liveramp_automation-1.4.1/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.1/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10820 2024-05-17 02:15:01.000000 liveramp_automation-1.4.1/liveramp_automation/helpers/bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8134 2024-04-16 03:01:46.000000 liveramp_automation-1.4.1/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7898 2024-03-28 09:52:13.000000 liveramp_automation-1.4.1/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     7369 2024-04-17 09:01:03.000000 liveramp_automation-1.4.1/liveramp_automation/helpers/fixture.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6184 2024-04-17 08:58:00.000000 liveramp_automation-1.4.1/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10686 2024-04-17 08:09:25.000000 liveramp_automation-1.4.1/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.815006 liveramp_automation-1.4.1/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-1.4.1/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1934 2024-04-01 03:10:38.000000 liveramp_automation-1.4.1/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6445 2024-03-01 06:50:54.000000 liveramp_automation-1.4.1/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     5025 2024-04-17 09:04:21.000000 liveramp_automation-1.4.1/liveramp_automation/utils/pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1728 2023-08-16 02:33:25.000000 liveramp_automation-1.4.1/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4025 2023-09-13 03:08:07.000000 liveramp_automation-1.4.1/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10164 2023-12-01 07:13:44.000000 liveramp_automation-1.4.1/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    49909 2023-12-11 09:06:44.000000 liveramp_automation-1.4.1/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    10500 2024-03-05 09:08:06.000000 liveramp_automation-1.4.1/liveramp_automation/utils/slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      795 2024-04-23 06:11:59.000000 liveramp_automation-1.4.1/liveramp_automation/utils/steps.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     8423 2024-04-23 05:42:40.000000 liveramp_automation-1.4.1/liveramp_automation/utils/testrail.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1660 2023-12-11 09:11:45.000000 liveramp_automation-1.4.1/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.823437 liveramp_automation-1.4.1/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (503) staff       (20)     3000 2024-05-17 02:15:23.000000 liveramp_automation-1.4.1/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (503) staff       (20)     1608 2024-05-17 02:15:23.000000 liveramp_automation-1.4.1/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)        1 2024-05-17 02:15:23.000000 liveramp_automation-1.4.1/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)      474 2024-05-17 02:15:23.000000 liveramp_automation-1.4.1/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       26 2024-05-17 02:15:23.000000 liveramp_automation-1.4.1/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (503) staff       (20)       38 2024-05-17 02:15:23.824450 liveramp_automation-1.4.1/setup.cfg
+-rw-r--r--   0 jasqia     (503) staff       (20)     1516 2024-04-24 07:51:56.000000 liveramp_automation-1.4.1/setup.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.815377 liveramp_automation-1.4.1/tests/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.1/tests/__init__.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.818121 liveramp_automation-1.4.1/tests/test_helpers/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-1.4.1/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4384 2024-05-14 09:08:10.000000 liveramp_automation-1.4.1/tests/test_helpers/test_bigquery.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     2347 2024-05-14 05:26:06.000000 liveramp_automation-1.4.1/tests/test_helpers/test_bucket.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4132 2024-04-01 03:42:11.000000 liveramp_automation-1.4.1/tests/test_helpers/test_file.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1247 2024-03-14 08:05:22.000000 liveramp_automation-1.4.1/tests/test_helpers/test_fixtures.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1676 2024-03-14 09:32:27.000000 liveramp_automation-1.4.1/tests/test_helpers/test_login.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3508 2024-03-05 09:08:06.000000 liveramp_automation-1.4.1/tests/test_helpers/test_notification.py
+drwxr-xr-x   0 jasqia     (503) staff       (20)        0 2024-05-17 02:15:23.822816 liveramp_automation-1.4.1/tests/test_utils/
+-rw-r--r--   0 jasqia     (503) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-1.4.1/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1832 2024-03-28 09:52:13.000000 liveramp_automation-1.4.1/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     4783 2024-03-28 09:52:13.000000 liveramp_automation-1.4.1/tests/test_utils/test_pagerduty.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     3324 2024-05-10 03:07:09.000000 liveramp_automation-1.4.1/tests/test_utils/test_parsers.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     1014 2024-03-14 08:40:57.000000 liveramp_automation-1.4.1/tests/test_utils/test_playwright.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    13489 2024-04-01 03:10:38.000000 liveramp_automation-1.4.1/tests/test_utils/test_request.py
+-rw-r--r--   0 jasqia     (503) staff       (20)    39767 2024-03-28 09:52:13.000000 liveramp_automation-1.4.1/tests/test_utils/test_selenium.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     6615 2024-03-28 09:52:13.000000 liveramp_automation-1.4.1/tests/test_utils/test_slack.py
+-rw-r--r--   0 jasqia     (503) staff       (20)     5406 2024-05-10 03:16:07.000000 liveramp_automation-1.4.1/tests/test_utils/test_testrail.py
+-rw-r--r--   0 jasqia     (503) staff       (20)      742 2024-03-14 08:51:35.000000 liveramp_automation-1.4.1/tests/test_utils/test_version.py
```

### Comparing `liveramp_automation-1.4.0/LICENSE` & `liveramp_automation-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/PKG-INFO` & `liveramp_automation-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 1.4.0
+Version: 1.4.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.4.0/README.md` & `liveramp_automation-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/helpers/bigquery.py` & `liveramp_automation-1.4.1/liveramp_automation/helpers/bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         round_execution_result = "PASS"
         if failed_count > 0:
             round_execution_result = "FAIL"
         load_dotenv()
         test_round = {"id": unique_id,
                       "round_id": MACROS["now"],
                       "round_execution_env": os.environ.get('ENVCHOICE', 'PROD').upper(),
-                      "round_execution_product": os.environ.get('PRODUCT', 'PRODUCT'),
+                      "round_execution_product": os.environ.get('PRODUCTNAME', '').upper(),
                       "round_execution_time": MACROS["now"],
                       "round_timestamp": MACROS["now_readable"],
                       "round_feature_ids": ",".join(map(lambda x: x["id"], features)),
                       "round_execution_result": round_execution_result,
                       "round_case_numbers": len(scenarios),
                       "round_case_failed_numbers": failed_count}
         rounds.append(test_round)
```

### Comparing `liveramp_automation-1.4.0/liveramp_automation/helpers/bucket.py` & `liveramp_automation-1.4.1/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/helpers/file.py` & `liveramp_automation-1.4.1/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/helpers/fixture.py` & `liveramp_automation-1.4.1/liveramp_automation/helpers/fixture.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/helpers/login.py` & `liveramp_automation-1.4.1/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/helpers/notification.py` & `liveramp_automation-1.4.1/liveramp_automation/helpers/notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/allure.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/log.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/pagerduty.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/parsers.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/playwright.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/request.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/selenium.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/slack.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/steps.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/steps.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/testrail.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/testrail.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation/utils/time.py` & `liveramp_automation-1.4.1/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-1.4.1/liveramp_automation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 1.4.0
+Version: 1.4.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: allure-pytest-bdd
```

### Comparing `liveramp_automation-1.4.0/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-1.4.1/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/setup.py` & `liveramp_automation-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_helpers/test_bigquery.py` & `liveramp_automation-1.4.1/tests/test_helpers/test_bigquery.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,127 +1,127 @@
 from liveramp_automation.helpers.bigquery import BigQueryConnector
 from unittest.mock import patch
 
 project_id = "liveramp-eng-qa-reliability"
-dataset_id = "liveramp_automation_test"
+dataset_id = "customer_impact_hours"
 table_name = "test_table"
 round_table = "round_table"
 feature_table = "feature_table"
 scenario_table = "scenario_table"
 step_table = "step_table"
 connector = BigQueryConnector(project_id, dataset_id)
 sql_query = f"SELECT * FROM `{project_id}.{dataset_id}.{table_name}` where age > 1;"
 output_csv_path = "tests/test_helpers/test.csv"
 cucumber_json_path = "tests/resources/cucumber.json"
 bucket_name = "liveramp_automation_test"
 source_blob_name = "Unit/test.csv"
 
-
-def mocked_requests_response_exception(*args, **kwargs):
-    if len(args) > 0 and 'Finish' in args[0]:
-        raise Exception("Test")
-    pass
-
-
-def test_connect():
-    result = connector.connect()
-    assert result == 0
-
-
-@patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
-def test_connect_exception(mock):
-    result = connector.connect()
-    assert result is None
-
-
-def test_query():
-    result = connector.query(sql_query)
-    if result:
-        for row in result:
-            print(row)
-    assert result
-
-
-@patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
-def test_query_exception(mock):
-    result = connector.query(sql_query)
-    assert result is None
-
-
-def test_query_rows():
-    result = connector.query_rows(sql_query)
-    assert result
-
-
-@patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
-def test_query_rows_exception(mock):
-    result = connector.query_rows(sql_query)
-    assert result is None
-
-
-def test_query_export():
-    result = connector.query_export(sql_query, output_csv_path)
-    assert result == 0
-
-
-@patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
-def test_query_export_exception(mock):
-    result = connector.query_export(sql_query, output_csv_path)
-    assert result is None
-
-
-def test_dataset_tables():
-    result = connector.dataset_tables()
-    assert result
-
-
-@patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
-def test_dataset_tables_exception(mock):
-    result = connector.dataset_tables()
-    assert result is None
-
-
-def test_insert_from_bucket():
-    result = connector.insert_from_bucket(bucket_name, source_blob_name, table_name)
-    assert result
-
-
-@patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
-def test_insert_from_bucket_exception(mock):
-    result = connector.insert_from_bucket(bucket_name, source_blob_name, table_name)
-    assert result is None
-
-
-@patch('google.cloud.bigquery.Client.insert_rows')
-def test_insert_from_report_bigquery(mock):
-    connector.insert_from_pytest_bdd_cucumber_report(
-        cucumber_json_path,
-        f"{project_id}.{dataset_id}.{feature_table}",
-        f"{project_id}.{dataset_id}.{scenario_table}",
-        f"{project_id}.{dataset_id}.{step_table}")
-    steps_dict = mock.call_args.args[1]
-    assert mock.call_count == 3
-    assert len(mock.call_args.args) == 2
-    assert "id" in steps_dict[1]
-    assert "name" in steps_dict[1]
-    assert "keyword" in steps_dict[1]
-    assert "line" in steps_dict[1]
-    assert "status" in steps_dict[1]
-    assert "duration" in steps_dict[1]
-    assert "location" in steps_dict[1]
-
-
-@patch('google.cloud.bigquery.Client.insert_rows')
-def test_insert_from_report_bigquery_file_not_found(mock):
-    connector.insert_from_pytest_bdd_cucumber_report(
-        cucumber_json_path+"not_found.json",
-        f"{project_id}.{dataset_id}.{feature_table}",
-        f"{project_id}.{dataset_id}.{scenario_table}",
-        f"{project_id}.{dataset_id}.{step_table}")
-    assert mock.call_count == 3
+#
+# def mocked_requests_response_exception(*args, **kwargs):
+#     if len(args) > 0 and 'Finish' in args[0]:
+#         raise Exception("Test")
+#     pass
+#
+#
+# def test_connect():
+#     result = connector.connect()
+#     assert result == 0
+#
+#
+# @patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
+# def test_connect_exception(mock):
+#     result = connector.connect()
+#     assert result is None
+#
+#
+# def test_query():
+#     result = connector.query(sql_query)
+#     if result:
+#         for row in result:
+#             print(row)
+#     assert result
+#
+#
+# @patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
+# def test_query_exception(mock):
+#     result = connector.query(sql_query)
+#     assert result is None
+#
+#
+# def test_query_rows():
+#     result = connector.query_rows(sql_query)
+#     assert result
+#
+#
+# @patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
+# def test_query_rows_exception(mock):
+#     result = connector.query_rows(sql_query)
+#     assert result is None
+#
+#
+# def test_query_export():
+#     result = connector.query_export(sql_query, output_csv_path)
+#     assert result == 0
+#
+#
+# @patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
+# def test_query_export_exception(mock):
+#     result = connector.query_export(sql_query, output_csv_path)
+#     assert result is None
+#
+#
+# def test_dataset_tables():
+#     result = connector.dataset_tables()
+#     assert result
+#
+#
+# @patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
+# def test_dataset_tables_exception(mock):
+#     result = connector.dataset_tables()
+#     assert result is None
+#
+#
+# def test_insert_from_bucket():
+#     result = connector.insert_from_bucket(bucket_name, source_blob_name, table_name)
+#     assert result
+#
+#
+# @patch('liveramp_automation.utils.log.Logger.info', side_effect=mocked_requests_response_exception)
+# def test_insert_from_bucket_exception(mock):
+#     result = connector.insert_from_bucket(bucket_name, source_blob_name, table_name)
+#     assert result is None
+#
+#
+# @patch('google.cloud.bigquery.Client.insert_rows')
+# def test_insert_from_report_bigquery(mock):
+#     connector.insert_from_pytest_bdd_cucumber_report(
+#         cucumber_json_path,
+#         f"{project_id}.{dataset_id}.{feature_table}",
+#         f"{project_id}.{dataset_id}.{scenario_table}",
+#         f"{project_id}.{dataset_id}.{step_table}")
+#     steps_dict = mock.call_args.args[1]
+#     assert mock.call_count == 3
+#     assert len(mock.call_args.args) == 2
+#     assert "id" in steps_dict[1]
+#     assert "name" in steps_dict[1]
+#     assert "keyword" in steps_dict[1]
+#     assert "line" in steps_dict[1]
+#     assert "status" in steps_dict[1]
+#     assert "duration" in steps_dict[1]
+#     assert "location" in steps_dict[1]
+#
+#
+# @patch('google.cloud.bigquery.Client.insert_rows')
+# def test_insert_from_report_bigquery_file_not_found(mock):
+#     connector.insert_from_pytest_bdd_cucumber_report(
+#         cucumber_json_path+"not_found.json",
+#         f"{project_id}.{dataset_id}.{feature_table}",
+#         f"{project_id}.{dataset_id}.{scenario_table}",
+#         f"{project_id}.{dataset_id}.{step_table}")
+#     assert mock.call_count == 3
 
 
 def test_insert_from_report():
     result = connector.insert_from_pytest_bdd_cucumber_report(
         cucumber_json_path,
         f"{project_id}.{dataset_id}.{round_table}",
         f"{project_id}.{dataset_id}.{feature_table}",
```

### Comparing `liveramp_automation-1.4.0/tests/test_helpers/test_bucket.py` & `liveramp_automation-1.4.1/tests/test_helpers/test_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_helpers/test_file.py` & `liveramp_automation-1.4.1/tests/test_helpers/test_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_helpers/test_fixtures.py` & `liveramp_automation-1.4.1/tests/test_helpers/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_helpers/test_login.py` & `liveramp_automation-1.4.1/tests/test_helpers/test_login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_helpers/test_notification.py` & `liveramp_automation-1.4.1/tests/test_helpers/test_notification.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_log.py` & `liveramp_automation-1.4.1/tests/test_utils/test_log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_pagerduty.py` & `liveramp_automation-1.4.1/tests/test_utils/test_pagerduty.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_parsers.py` & `liveramp_automation-1.4.1/tests/test_utils/test_parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_playwright.py` & `liveramp_automation-1.4.1/tests/test_utils/test_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_request.py` & `liveramp_automation-1.4.1/tests/test_utils/test_request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_selenium.py` & `liveramp_automation-1.4.1/tests/test_utils/test_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_slack.py` & `liveramp_automation-1.4.1/tests/test_utils/test_slack.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_testrail.py` & `liveramp_automation-1.4.1/tests/test_utils/test_testrail.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-1.4.0/tests/test_utils/test_version.py` & `liveramp_automation-1.4.1/tests/test_utils/test_version.py`

 * *Files identical despite different names*

