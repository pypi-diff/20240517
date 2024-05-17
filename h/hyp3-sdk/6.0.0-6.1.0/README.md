# Comparing `tmp/hyp3_sdk-6.0.0.tar.gz` & `tmp/hyp3_sdk-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyp3_sdk-6.0.0.tar", last modified: Fri Feb  2 20:46:40 2024, max compression
+gzip compressed data, was "hyp3_sdk-6.1.0.tar", last modified: Wed Feb 28 20:13:44 2024, max compression
```

## Comparing `hyp3_sdk-6.0.0.tar` & `hyp3_sdk-6.1.0.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.075387 hyp3_sdk-6.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.067387 hyp3_sdk-6.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.067387 hyp3_sdk-6.0.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.071387 hyp3_sdk-6.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/changelog.yml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/create-jira-issue.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/distribute.yml
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/labeled-pr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/notify-downstream.yml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/release-template-comment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/static-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/tag-version.yml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.gitleaks.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/.trufflehog.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14521 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-02 20:46:40.075387 hyp3_sdk-6.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.071387 hyp3_sdk-6.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/docs/sdk_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/docs/search_other_user_jobs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-02 20:46:40.075387 hyp3_sdk-6.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.067387 hyp3_sdk-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.071387 hyp3_sdk-6.0.0/src/hyp3_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/src/hyp3_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/src/hyp3_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22496 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/src/hyp3_sdk/hyp3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/src/hyp3_sdk/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/src/hyp3_sdk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.075387 hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-02 20:46:40.000000 hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-02-02 20:46:40.000000 hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 20:46:40.000000 hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 20:46:39.000000 hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-02 20:46:40.000000 hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-02 20:46:40.000000 hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.071387 hyp3_sdk-6.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:46:40.075387 hyp3_sdk-6.0.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/tests/data/product.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/tests/test_hyp3.py
--rw-r--r--   0 runner    (1001) docker     (127)    15425 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-02 20:46:16.000000 hyp3_sdk-6.0.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.156214 hyp3_sdk-6.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.152214 hyp3_sdk-6.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.152214 hyp3_sdk-6.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.152214 hyp3_sdk-6.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/create-jira-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/distribute.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/labeled-pr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/notify-downstream.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/release-template-comment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/static-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/tag-version.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/.gitleaks.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-28 20:13:44.156214 hyp3_sdk-6.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.152214 hyp3_sdk-6.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/docs/sdk_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/docs/search_other_user_jobs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 20:13:44.156214 hyp3_sdk-6.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.148214 hyp3_sdk-6.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.152214 hyp3_sdk-6.1.0/src/hyp3_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/src/hyp3_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/src/hyp3_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22735 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/src/hyp3_sdk/hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/src/hyp3_sdk/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/src/hyp3_sdk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.156214 hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-28 20:13:44.000000 hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-28 20:13:44.000000 hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 20:13:44.000000 hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 20:13:43.000000 hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-28 20:13:44.000000 hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-28 20:13:44.000000 hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.156214 hyp3_sdk-6.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:13:44.156214 hyp3_sdk-6.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/tests/data/product.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/tests/test_hyp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-02-28 20:13:20.000000 hyp3_sdk-6.1.0/tests/test_util.py
```

### Comparing `hyp3_sdk-6.0.0/.github/ISSUE_TEMPLATE/feature_request.md` & `hyp3_sdk-6.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/.github/workflows/distribute.yml` & `hyp3_sdk-6.1.0/.github/workflows/distribute.yml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on:
   push:
     tags:
       - v*
 
 jobs:
   call-version-info-workflow:
-    uses: ASFHyP3/actions/.github/workflows/reusable-version-info.yml@v0.9.0
+    uses: ASFHyP3/actions/.github/workflows/reusable-version-info.yml@v0.11.0
 
   distribute:
     runs-on: ubuntu-latest
     defaults:
       run:
         shell: bash -l {0}
     steps:
```

### Comparing `hyp3_sdk-6.0.0/.gitignore` & `hyp3_sdk-6.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/.gitleaks.toml` & `hyp3_sdk-6.1.0/.gitleaks.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/CHANGELOG.md` & `hyp3_sdk-6.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [PEP 440](https://www.python.org/dev/peps/pep-0440/) 
 and uses [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [6.1.0]
+
+### Added
+* `HyP3.costs` method to retrieve the job cost lookup table, following the addition of the `/costs` API endpoint in HyP3 v6.2.0
+* `Batch.total_credit_cost` method to calculate the total credit cost for a batch of jobs
+
 ## [6.0.0]
 This release accommodates changes to the HyP3 API schema introduced in HyP3 v6.0.0
 
 ### Added
 * `credit_cost` attribute to the `Job` class
 * `HyP3.check_credits` method to determine your remaining processing credits
```

### Comparing `hyp3_sdk-6.0.0/CODE_OF_CONDUCT.md` & `hyp3_sdk-6.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/LICENSE` & `hyp3_sdk-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/PKG-INFO` & `hyp3_sdk-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3_sdk
-Version: 6.0.0
+Version: 6.1.0
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-6.0.0/README.md` & `hyp3_sdk-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/docs/sdk_example.ipynb` & `hyp3_sdk-6.1.0/docs/sdk_example.ipynb`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/docs/search_other_user_jobs.ipynb` & `hyp3_sdk-6.1.0/docs/search_other_user_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/pyproject.toml` & `hyp3_sdk-6.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/src/hyp3_sdk/exceptions.py` & `hyp3_sdk-6.1.0/src/hyp3_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/src/hyp3_sdk/hyp3.py` & `hyp3_sdk-6.1.0/src/hyp3_sdk/hyp3.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,7 +501,16 @@
 
         Returns:
             Your remaining processing credits, or None if you have no processing limit
         """
         warn('This method is deprecated and will be removed in a future release.\n'
              'Please use `HyP3.check_credits` instead.', DeprecationWarning, stacklevel=2)
         return self.check_credits()
+
+    def costs(self) -> dict:
+        """
+        Returns:
+            Table of job costs
+        """
+        response = self.session.get(urljoin(self.url, '/costs'))
+        _raise_for_hyp3_status(response)
+        return response.json()
```

### Comparing `hyp3_sdk-6.0.0/src/hyp3_sdk/jobs.py` & `hyp3_sdk-6.1.0/src/hyp3_sdk/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,7 +287,10 @@
             elif job.pending() and pending:
                 filtered_jobs.append(job)
 
             elif job.failed() and failed:
                 filtered_jobs.append(job)
 
         return Batch(filtered_jobs)
+
+    def total_credit_cost(self):
+        return sum(job.credit_cost for job in self.jobs if job.credit_cost is not None)
```

### Comparing `hyp3_sdk-6.0.0/src/hyp3_sdk/util.py` & `hyp3_sdk-6.1.0/src/hyp3_sdk/util.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/PKG-INFO` & `hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyp3_sdk
-Version: 6.0.0
+Version: 6.1.0
 Summary: A python wrapper around the HyP3 API
 Author-email: ASF APD/Tools Team <uaf-asf-apd@alaska.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/ASFHyP3/hyp3-sdk
 Project-URL: Bug Tracker, https://github.com/ASFHyP3/hyp3-sdk/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `hyp3_sdk-6.0.0/src/hyp3_sdk.egg-info/SOURCES.txt` & `hyp3_sdk-6.1.0/src/hyp3_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .gitignore
 .gitleaks.toml
-.trufflehog.txt
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 LICENSE
 MANIFEST.in
 README.md
 environment.yml
 postBuild
```

### Comparing `hyp3_sdk-6.0.0/tests/conftest.py` & `hyp3_sdk-6.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/tests/data/product.zip` & `hyp3_sdk-6.1.0/tests/data/product.zip`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/tests/test_exceptions.py` & `hyp3_sdk-6.1.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hyp3_sdk-6.0.0/tests/test_hyp3.py` & `hyp3_sdk-6.1.0/tests/test_hyp3.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,7 +433,17 @@
         'user_id': 'someUser'
     }
     with patch('hyp3_sdk.util.get_authenticated_session', mock_get_authenticated_session):
         api = HyP3()
     responses.add(responses.GET, urljoin(api.url, '/user'), json=api_response)
 
     assert math.isclose(api.check_credits(), 25.)
+
+
+@responses.activate
+def test_costs():
+    api_response = {'foo': 5}
+    with patch('hyp3_sdk.util.get_authenticated_session', mock_get_authenticated_session):
+        api = HyP3()
+    responses.add(responses.GET, urljoin(api.url, '/costs'), json=api_response)
+
+    assert api.costs() == {'foo': 5}
```

### Comparing `hyp3_sdk-6.0.0/tests/test_jobs.py` & `hyp3_sdk-6.1.0/tests/test_jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -436,7 +436,70 @@
 
     everything = batch.filter_jobs(failed=True)
     assert len(everything) == len(batch)
     for ii, job in enumerate(everything.jobs):
         assert job.status_code == batch.jobs[ii].status_code
         if job.succeeded():
             assert job.expired() == batch.jobs[ii].expired()
+
+
+def test_batch_total_credit_cost():
+    batch = Batch()
+    assert batch.total_credit_cost() == 0
+
+    batch = Batch([
+        Job.from_dict({
+            'job_type': 'foo',
+            'job_id': 'foo',
+            'request_time': '2024-01-01T00:00:00Z',
+            'status_code': 'foo',
+            'user_id': 'foo',
+        }),
+    ])
+    assert batch.total_credit_cost() == 0
+
+    batch = Batch([
+        Job.from_dict({
+            'job_type': 'foo',
+            'job_id': 'foo',
+            'request_time': '2024-01-01T00:00:00Z',
+            'status_code': 'foo',
+            'user_id': 'foo',
+            'credit_cost': 4
+        }),
+        Job.from_dict({
+            'job_type': 'foo',
+            'job_id': 'foo',
+            'request_time': '2024-01-01T00:00:00Z',
+            'status_code': 'foo',
+            'user_id': 'foo',
+        }),
+    ])
+    assert batch.total_credit_cost() == 4
+
+    batch = Batch([
+        Job.from_dict({
+            'job_type': 'foo',
+            'job_id': 'foo',
+            'request_time': '2024-01-01T00:00:00Z',
+            'status_code': 'foo',
+            'user_id': 'foo',
+            'credit_cost': 1
+        }),
+        Job.from_dict({
+            'job_type': 'foo',
+            'job_id': 'foo',
+            'request_time': '2024-01-01T00:00:00Z',
+            'status_code': 'foo',
+            'user_id': 'foo',
+            'credit_cost': 2
+        }),
+        Job.from_dict({
+            'job_type': 'foo',
+            'job_id': 'foo',
+            'request_time': '2024-01-01T00:00:00Z',
+            'status_code': 'foo',
+            'user_id': 'foo',
+            'credit_cost': 5
+        }),
+    ])
+    assert batch.total_credit_cost() == 8
```

### Comparing `hyp3_sdk-6.0.0/tests/test_util.py` & `hyp3_sdk-6.1.0/tests/test_util.py`

 * *Files identical despite different names*

