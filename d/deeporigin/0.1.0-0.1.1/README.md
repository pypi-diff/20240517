# Comparing `tmp/deeporigin-0.1.0.tar.gz` & `tmp/deeporigin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeporigin-0.1.0.tar", last modified: Mon May 13 13:40:30 2024, max compression
+gzip compressed data, was "deeporigin-0.1.1.tar", last modified: Fri May 17 14:42:06 2024, max compression
```

## Comparing `deeporigin-0.1.0.tar` & `deeporigin-0.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.104365 deeporigin-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 13:40:22.000000 deeporigin-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 13:40:22.000000 deeporigin-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-13 13:40:30.104365 deeporigin-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-13 13:40:22.000000 deeporigin-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.104365 deeporigin-0.1.0/deeporigin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-13 13:40:30.000000 deeporigin-0.1.0/deeporigin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-13 13:40:30.000000 deeporigin-0.1.0/deeporigin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:40:30.000000 deeporigin-0.1.0/deeporigin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 13:40:30.000000 deeporigin-0.1.0/deeporigin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 13:40:30.000000 deeporigin-0.1.0/deeporigin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 13:40:30.000000 deeporigin-0.1.0/deeporigin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-13 13:40:22.000000 deeporigin-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:40:30.104365 deeporigin-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.096365 deeporigin-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 13:40:27.000000 deeporigin-0.1.0/src/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.096365 deeporigin-0.1.0/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.096365 deeporigin-0.1.0/src/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/config/default.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/context.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/feature_flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.100365 deeporigin-0.1.0/src/managed_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/managed_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/managed_data/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/managed_data/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/managed_data/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/managed_data/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.100365 deeporigin-0.1.0/src/variables/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/base_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    20222 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.100365 deeporigin-0.1.0/src/variables/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/anthropic_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/aws_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9728 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/git_http_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/gurobi_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/mosek_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/open_ai_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/private_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/private_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/secret_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/secret_env_var_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/secret_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/secret_file_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/variables/types/xpress_license_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-13 13:40:22.000000 deeporigin-0.1.0/src/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:40:30.104365 deeporigin-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-13 13:40:22.000000 deeporigin-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-13 13:40:22.000000 deeporigin-0.1.0/tests/test_cli_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-13 13:40:22.000000 deeporigin-0.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-13 13:40:22.000000 deeporigin-0.1.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-13 13:40:22.000000 deeporigin-0.1.0/tests/test_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-13 13:40:22.000000 deeporigin-0.1.0/tests/test_managed_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    89808 2024-05-13 13:40:22.000000 deeporigin-0.1.0/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.937538 deeporigin-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-17 14:42:03.000000 deeporigin-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 14:42:03.000000 deeporigin-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-17 14:42:06.937538 deeporigin-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-17 14:42:03.000000 deeporigin-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.933538 deeporigin-0.1.1/deeporigin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 14:42:06.000000 deeporigin-0.1.1/deeporigin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-17 14:42:03.000000 deeporigin-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:42:06.937538 deeporigin-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 14:42:04.000000 deeporigin-0.1.1/src/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/config/default.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/feature_flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/managed_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14175 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/managed_data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.929538 deeporigin-0.1.1/src/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/base_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20138 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.933538 deeporigin-0.1.1/src/variables/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/anthropic_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11608 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/aws_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9726 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/git_http_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/gurobi_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/mosek_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/open_ai_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/private_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/private_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_env_var_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/secret_file_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/variables/types/xpress_license_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 14:42:03.000000 deeporigin-0.1.1/src/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:42:06.933538 deeporigin-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_cli_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_managed_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89806 2024-05-17 14:42:03.000000 deeporigin-0.1.1/tests/test_variables.py
```

### Comparing `deeporigin-0.1.0/LICENSE.txt` & `deeporigin-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/PKG-INFO` & `deeporigin-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.1.0/README.md` & `deeporigin-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # deeporigin 
 
+![PyPI](https://img.shields.io/pypi/v/deeporigin)
+
 This repository contains the `deeporigin` CLI and 
 python client, which allows you to interact with 
 Deep Origin from the command line. 
 
 > [!WARNING]  
 > The `deeporigin` client is under active development. Features
 > may change, or be removed.
```

### Comparing `deeporigin-0.1.0/deeporigin.egg-info/PKG-INFO` & `deeporigin-0.1.1/deeporigin.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeporigin
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line tool and Python client for working with Deep Origin
 Author-email: Deep Origin <support@deeporigin.com>
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
```

### Comparing `deeporigin-0.1.0/deeporigin.egg-info/SOURCES.txt` & `deeporigin-0.1.1/deeporigin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/pyproject.toml` & `deeporigin-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/__init__.py` & `deeporigin-0.1.1/src/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/auth.py` & `deeporigin-0.1.1/src/auth.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/cli/__init__.py` & `deeporigin-0.1.1/src/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/cli/context.py` & `deeporigin-0.1.1/src/cli/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/cli/data.py` & `deeporigin-0.1.1/src/cli/data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/cli/variables.py` & `deeporigin-0.1.1/src/cli/variables.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/config/__init__.py` & `deeporigin-0.1.1/src/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/config/default.yml` & `deeporigin-0.1.1/src/config/default.yml`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/context.py` & `deeporigin-0.1.1/src/context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/feature_flags.py` & `deeporigin-0.1.1/src/feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/managed_data/_api.py` & `deeporigin-0.1.1/src/managed_data/_api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/managed_data/api.py` & `deeporigin-0.1.1/src/managed_data/api.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/managed_data/client.py` & `deeporigin-0.1.1/src/managed_data/client.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/managed_data/schema.py` & `deeporigin-0.1.1/src/managed_data/schema.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/utils.py` & `deeporigin-0.1.1/src/utils.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/base_type.py` & `deeporigin-0.1.1/src/variables/base_type.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/core.py` & `deeporigin-0.1.1/src/variables/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -372,17 +372,14 @@
     """
     # login
     if not get_feature_flags().variables:
         msg = "Updating variables is not yet available. For beta access, please contact support at support@deeporigin.com."
         warnings.warn(msg, FeatureNotAvailableWarning)
         return []
 
-    # Get an access token for the Deep Origin API
-    tokens = auth.get_tokens()
-
     # load the CronTab configuration
     with crontab.CronTab(user=True) as cron_tab:
         # get the id of the cron job
         cron_job_id = get_auto_install_variables_cronjob_id()
 
         # remove previous job
         for job in cron_tab.find_comment(comment=cron_job_id):
@@ -458,15 +455,15 @@
         )
         commands.append(
             f"export DEEP_ORIGIN_AUTO_INSTALL_VARIABLES_FILENAME='{escaped_auto_install_variables_filename}'"
         )
 
         if not cli:
             cli = sys.argv[0]
-            if not cli.endswith("/deep-origin") and not cli.endswith(
+            if not cli.endswith("/deeporigin") and not cli.endswith(
                 "pytest/__main__.py"
             ):
                 raise DeepOriginException(
                     "Auto installation must be run from the Deep Origin CLI"
                 )
 
         cli_command = [cli, "variables", "install"]
@@ -480,15 +477,15 @@
         cli_command.append("--type")
         cli_command.extend([type.name for type in types])
 
         if overwrite:
             cli_command.append("--overwrite")
 
         log_filename = os.path.expanduser(
-            os.path.join("~", ".log", "deep-origin", "variables-auto-install.log")
+            os.path.join("~", ".log", "deeporigin", "variables-auto-install.log")
         )
         os.makedirs(os.path.dirname(log_filename), exist_ok=True)
 
         cli_command = " ".join(cli_command)
         commands.append(f"{cli_command} >> {log_filename} 2>&1")
 
         job_filename = config.auto_install_variables_filename
```

### Comparing `deeporigin-0.1.0/src/variables/types/__init__.py` & `deeporigin-0.1.1/src/variables/types/__init__.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/aws_profile.py` & `deeporigin-0.1.1/src/variables/types/aws_profile.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/env_var.py` & `deeporigin-0.1.1/src/variables/types/env_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,12 +265,12 @@
             is_user_variable (:obj:`bool`, optional): whether the variable is a user or system variable
             user_home_dirname (:obj:`str`, optional): user's home directory
 
         Returns:
             :obj:`str`: Environment variable filename
         """
         if is_user_variable:
-            return os.path.join(user_home_dirname, ".deep-origin", "user-variables.env")
+            return os.path.join(user_home_dirname, ".deeporigin", "user-variables.env")
         else:
             return os.path.join(
-                user_home_dirname, ".deep-origin", "system-variables.env"
+                user_home_dirname, ".deeporigin", "system-variables.env"
             )
```

### Comparing `deeporigin-0.1.0/src/variables/types/file.py` & `deeporigin-0.1.1/src/variables/types/file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/git_http_credentials.py` & `deeporigin-0.1.1/src/variables/types/git_http_credentials.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/private_gpg_key.py` & `deeporigin-0.1.1/src/variables/types/private_gpg_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/private_ssh_key.py` & `deeporigin-0.1.1/src/variables/types/private_ssh_key.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/secret_env_var_value.py` & `deeporigin-0.1.1/src/variables/types/secret_env_var_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/secret_file_value.py` & `deeporigin-0.1.1/src/variables/types/secret_file_value.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/src/variables/types/xpress_license_file.py` & `deeporigin-0.1.1/src/variables/types/xpress_license_file.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/tests/test_cli.py` & `deeporigin-0.1.1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
 
 class TestCase(unittest.TestCase):
     def test_raw_help(self):
         with unittest.mock.patch("sys.argv", ["", "--help"]):
             with self.assertRaises(SystemExit) as context:
                 cli.main()
-                self.assertRegex(context.Exception, "usage: deep-origin")
+                self.assertRegex(context.Exception, "usage: deeporigin")
 
     def test_help(self):
         with cli.App(argv=["--help"]) as app:
             with self.assertRaises(SystemExit) as context:
                 app.run()
-                self.assertRegex(context.Exception, "usage: deep-origin")
+                self.assertRegex(context.Exception, "usage: deeporigin")
 
         with cli.App(argv=[]) as app:
             with self.assertRaises(SystemExit) as context:
                 app.run()
-                self.assertRegex(context.Exception, "usage: deep-origin")
+                self.assertRegex(context.Exception, "usage: deeporigin")
 
     def test_version(self):
         stdout_capture = io.StringIO()
         stderr_capture = io.StringIO()
 
         with redirect_stdout(stdout_capture), redirect_stderr(stderr_capture):
             with cli.App(argv=["--version"]) as app:
```

### Comparing `deeporigin-0.1.0/tests/test_cli_data.py` & `deeporigin-0.1.1/tests/test_cli_data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/tests/test_config.py` & `deeporigin-0.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/tests/test_context.py` & `deeporigin-0.1.1/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/tests/test_feature_flags.py` & `deeporigin-0.1.1/tests/test_feature_flags.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/tests/test_managed_data.py` & `deeporigin-0.1.1/tests/test_managed_data.py`

 * *Files identical despite different names*

### Comparing `deeporigin-0.1.0/tests/test_variables.py` & `deeporigin-0.1.1/tests/test_variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1626,15 +1626,15 @@
                     "access_token": "xxx",
                     "refresh_token": "xxx",
                 },
             ),
         ]
         with unittest.mock.patch("requests.post", side_effect=responses):
             variables.enable_variable_auto_updating(
-                user=False, org=False, cli="deep-origin"
+                user=False, org=False, cli="deeporigin"
             )
 
         with crontab.CronTab(user=True) as cron_tab:
             self.assertIn(
                 True,
                 set(job.is_enabled() for job in cron_tab.find_comment(cron_job_id)),
             )
@@ -2478,15 +2478,15 @@
             drn="drn:1",
             name="var-1",
             value="z",
         )
         var_xpress.install(None, user_home_dirname)
         expected_filenames.append(var_xpress.FILENAME.replace("~/", ""))
         expected_filenames.append(".bashrc")
-        expected_filenames.append(".deep-origin")
+        expected_filenames.append(".deeporigin")
         self.assertEqual(
             sorted(expected_filenames), sorted(os.listdir(user_home_dirname))
         )
         with open(
             utils.expand_user(var_xpress.FILENAME, user_home_dirname), "r"
         ) as file:
             self.assertEqual(var_xpress.value, file.read())
```

