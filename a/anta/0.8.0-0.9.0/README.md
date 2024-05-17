# Comparing `tmp/anta-0.8.0.tar.gz` & `tmp/anta-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anta-0.8.0.tar", last modified: Fri Sep 22 12:57:23 2023, max compression
+gzip compressed data, was "anta-0.9.0.tar", last modified: Thu Sep 28 19:12:39 2023, max compression
```

## Comparing `anta-0.8.0.tar` & `anta-0.9.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.945142 anta-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2023-09-22 12:57:11.000000 anta-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21613 2023-09-22 12:57:23.941142 anta-0.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.929141 anta-0.8.0/anta/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-09-22 12:57:11.000000 anta-0.8.0/anta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/cli/debug/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/debug/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/cli/exec/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/exec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/exec/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/exec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/cli/get/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/get/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/get/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/get/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/cli/nrfu/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/nrfu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/nrfu/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/nrfu/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2023-09-22 12:57:11.000000 anta-0.8.0/anta/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-22 12:57:11.000000 anta-0.8.0/anta/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6796 2023-09-22 12:57:11.000000 anta-0.8.0/anta/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13186 2023-09-22 12:57:11.000000 anta-0.8.0/anta/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/inventory/
--rw-r--r--   0 runner    (1001) docker     (127)    10361 2023-09-22 12:57:11.000000 anta-0.8.0/anta/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-09-22 12:57:11.000000 anta-0.8.0/anta/inventory/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2023-09-22 12:57:11.000000 anta-0.8.0/anta/inventory/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6279 2023-09-22 12:57:11.000000 anta-0.8.0/anta/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    21263 2023-09-22 12:57:11.000000 anta-0.8.0/anta/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/reporter/
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2023-09-22 12:57:11.000000 anta-0.8.0/anta/reporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-09-22 12:57:11.000000 anta-0.8.0/anta/reporter/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta/result_manager/
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2023-09-22 12:57:11.000000 anta-0.8.0/anta/result_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2023-09-22 12:57:11.000000 anta-0.8.0/anta/result_manager/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-09-22 12:57:11.000000 anta-0.8.0/anta/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.937142 anta-0.8.0/anta/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12851 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/aaa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4952 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/field_notices.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)    19943 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    10647 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9086 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/mlag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/multicast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.937142 anta-0.8.0/anta/tests/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28899 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/routing/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6249 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/routing/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/routing/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/software.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/stp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8605 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tests/vxlan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.937142 anta-0.8.0/anta/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tools/get_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tools/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-09-22 12:57:11.000000 anta-0.8.0/anta/tools/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.933141 anta-0.8.0/anta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21613 2023-09-22 12:57:23.000000 anta-0.8.0/anta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-09-22 12:57:23.000000 anta-0.8.0/anta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 12:57:23.000000 anta-0.8.0/anta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 12:57:23.000000 anta-0.8.0/anta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-09-22 12:57:23.000000 anta-0.8.0/anta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-22 12:57:23.000000 anta-0.8.0/anta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 12:57:23.937142 anta-0.8.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5209 2023-09-22 12:57:11.000000 anta-0.8.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8471 2023-09-22 12:57:11.000000 anta-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-22 12:57:23.945142 anta-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.644892 anta-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2023-09-28 19:12:27.000000 anta-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21766 2023-09-28 19:12:39.640892 anta-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-09-28 19:12:27.000000 anta-0.9.0/anta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/cli/debug/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/debug/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/cli/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/exec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/exec/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/exec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/get/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/get/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/get/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/cli/nrfu/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/nrfu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/nrfu/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/nrfu/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2023-09-28 19:12:27.000000 anta-0.9.0/anta/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-09-28 19:12:27.000000 anta-0.9.0/anta/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6796 2023-09-28 19:12:27.000000 anta-0.9.0/anta/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16590 2023-09-28 19:12:27.000000 anta-0.9.0/anta/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/inventory/
+-rw-r--r--   0 runner    (1001) docker     (127)    11582 2023-09-28 19:12:27.000000 anta-0.9.0/anta/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2023-09-28 19:12:27.000000 anta-0.9.0/anta/inventory/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-09-28 19:12:27.000000 anta-0.9.0/anta/inventory/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2023-09-28 19:12:27.000000 anta-0.9.0/anta/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22241 2023-09-28 19:12:27.000000 anta-0.9.0/anta/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2023-09-28 19:12:27.000000 anta-0.9.0/anta/reporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2023-09-28 19:12:27.000000 anta-0.9.0/anta/reporter/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta/result_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2023-09-28 19:12:27.000000 anta-0.9.0/anta/result_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2023-09-28 19:12:27.000000 anta-0.9.0/anta/result_manager/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2023-09-28 19:12:27.000000 anta-0.9.0/anta/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.636891 anta-0.9.0/anta/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/aaa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4952 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/field_notices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19943 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9086 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/mlag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/multicast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.636891 anta-0.9.0/anta/tests/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28899 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/routing/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6249 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/routing/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/routing/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/software.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8743 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/stp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8605 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tests/vxlan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.636891 anta-0.9.0/anta/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tools/get_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2023-09-28 19:12:27.000000 anta-0.9.0/anta/tools/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.632891 anta-0.9.0/anta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21766 2023-09-28 19:12:39.000000 anta-0.9.0/anta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-09-28 19:12:39.000000 anta-0.9.0/anta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 19:12:39.000000 anta-0.9.0/anta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 19:12:39.000000 anta-0.9.0/anta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2023-09-28 19:12:39.000000 anta-0.9.0/anta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-09-28 19:12:39.000000 anta-0.9.0/anta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 19:12:39.636891 anta-0.9.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5330 2023-09-28 19:12:27.000000 anta-0.9.0/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2023-09-28 19:12:27.000000 anta-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-28 19:12:39.644892 anta-0.9.0/setup.cfg
```

### Comparing `anta-0.8.0/LICENSE` & `anta-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/PKG-INFO` & `anta-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.8.0
+Version: 0.9.0
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Thomas Grimonet <tgrimonet@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,19 +224,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiocache~=0.12.2
 Requires-Dist: aio-eapi==0.6.3
 Requires-Dist: click~=8.1.6
 Requires-Dist: click-help-colors~=0.9
 Requires-Dist: cvprac~=1.3.1
-Requires-Dist: pydantic<2.4.0,>=2.1.1
+Requires-Dist: pydantic<2.5.0,>=2.1.1
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rich~=13.5.2
 Requires-Dist: asyncssh~=2.13.2
 Requires-Dist: Jinja2~=3.1.2
 Provides-Extra: dev
 Requires-Dist: bumpver==2023.1126; extra == "dev"
@@ -340,23 +341,24 @@
   --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
                                   ANTA logging level  [env var:
                                   ANTA_LOG_LEVEL; default: INFO]
   --ignore-status                 Always exit with success  [env var:
                                   ANTA_IGNORE_STATUS]
   --ignore-error                  Only report failures and not errors  [env
                                   var: ANTA_IGNORE_ERROR]
+  --disable-cache                 Disable cache globally  [env var:
+                                  ANTA_DISABLE_CACHE]
   --help                          Show this message and exit.
 
 Commands:
   debug  Debug commands for building ANTA
   exec   Execute commands to inventory devices
   get    Get data from/to ANTA
   nrfu   Run NRFU against inventory devices
 ```
-
 > `username`, `password`, `enable-password`, `enable`, `timeout` and `insecure` values are the same for all devices
 
 
 ## Documentation
 
 The documentation is published on [ANTA package website](https://www.anta.ninja). Also, a [demo repository](https://github.com/titom73/atd-anta-demo) is available to facilitate your journey with ANTA.
```

### Comparing `anta-0.8.0/anta/__init__.py` & `anta-0.9.0/anta/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/__init__.py` & `anta-0.9.0/anta/cli/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             logging.getLevelName(logging.DEBUG),
         ],
         case_sensitive=False,
     ),
 )
 @click.option("--ignore-status", help="Always exit with success", show_envvar=True, is_flag=True, default=False)
 @click.option("--ignore-error", help="Only report failures and not errors", show_envvar=True, is_flag=True, default=False)
+@click.option("--disable-cache", help="Disable cache globally", show_envvar=True, show_default=True, is_flag=True, default=False)
 def anta(
     ctx: click.Context, inventory: pathlib.Path, log_level: Literal["CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG"], log_file: pathlib.Path, **kwargs: Any
 ) -> None:
     # pylint: disable=unused-argument
     """Arista Network Test Automation (ANTA) CLI"""
     setup_logging(log_level, log_file)
```

### Comparing `anta-0.8.0/anta/cli/debug/commands.py` & `anta-0.9.0/anta/cli/debug/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/exec/commands.py` & `anta-0.9.0/anta/cli/exec/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/exec/utils.py` & `anta-0.9.0/anta/cli/exec/utils.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/get/commands.py` & `anta-0.9.0/anta/cli/get/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/get/utils.py` & `anta-0.9.0/anta/cli/get/utils.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/nrfu/commands.py` & `anta-0.9.0/anta/cli/nrfu/commands.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/nrfu/utils.py` & `anta-0.9.0/anta/cli/nrfu/utils.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/cli/utils.py` & `anta-0.9.0/anta/cli/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
             inventory_file=str(path),
             username=ctx.params["username"],
             password=ctx.params["password"],
             enable=ctx.params["enable"],
             enable_password=ctx.params["enable_password"],
             timeout=ctx.params["timeout"],
             insecure=ctx.params["insecure"],
+            disable_cache=ctx.params["disable_cache"],
         )
     except Exception as e:  # pylint: disable=broad-exception-caught
         message = f"Unable to parse ANTA Inventory file '{path}'"
         anta_log_exception(e, message, logger)
         ctx.fail(message)
     return inventory
```

### Comparing `anta-0.8.0/anta/custom_types.py` & `anta-0.9.0/anta/custom_types.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/decorators.py` & `anta-0.9.0/anta/decorators.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/device.py` & `anta-0.9.0/anta/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,97 +5,159 @@
 ANTA Device Abstraction Module
 """
 from __future__ import annotations
 
 import asyncio
 import logging
 from abc import ABC, abstractmethod
+from collections import defaultdict
 from collections.abc import Iterator
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 import asyncssh
+from aiocache import Cache
+from aiocache.plugins import HitMissRatioPlugin
 from aioeapi import Device, EapiCommandError
 from asyncssh import SSHClientConnection, SSHClientConnectionOptions
 from httpx import ConnectError, HTTPError
 
 from anta import __DEBUG__
 from anta.models import DEFAULT_TAG, AntaCommand
 from anta.tools.misc import anta_log_exception, exc_to_str
 
 logger = logging.getLogger(__name__)
 
 
 class AntaDevice(ABC):
     """
     Abstract class representing a device in ANTA.
-    An implementation of this class needs must override the abstract coroutines `collect()` and
+    An implementation of this class must override the abstract coroutines `_collect()` and
     `refresh()`.
 
     Attributes:
         name: Device name
         is_online: True if the device IP is reachable and a port can be open
         established: True if remote command execution succeeds
         hw_model: Hardware model of the device
         tags: List of tags for this device
+        cache: In-memory cache from aiocache library for this device (None if cache is disabled)
+        cache_locks: Dictionary mapping keys to asyncio locks to guarantee exclusive access to the cache if not disabled
     """
 
-    def __init__(self, name: str, tags: Optional[list[str]] = None) -> None:
+    def __init__(self, name: str, tags: Optional[list[str]] = None, disable_cache: bool = False) -> None:
         """
         Constructor of AntaDevice
 
         Args:
             name: Device name
-            tags: list of tags for this device
+            tags: List of tags for this device
+            disable_cache: Disable caching for all commands for this device. Defaults to False.
         """
         self.name: str = name
         self.hw_model: Optional[str] = None
         self.tags: list[str] = tags if tags is not None else []
         self.is_online: bool = False
         self.established: bool = False
+        self.cache: Optional[Cache] = None
+        self.cache_locks: Optional[defaultdict[str, asyncio.Lock]] = None
+
+        # Initialize cache if not disabled
+        if not disable_cache:
+            self._init_cache()
 
         # Ensure tag 'all' is always set
         if DEFAULT_TAG not in self.tags:
             self.tags.append(DEFAULT_TAG)
 
+    def _init_cache(self) -> None:
+        """
+        Initialize cache for the device, can be overriden by subclasses to manipulate how it works
+        """
+        self.cache = Cache(cache_class=Cache.MEMORY, ttl=60, namespace=self.name, plugins=[HitMissRatioPlugin()])
+        self.cache_locks = defaultdict(asyncio.Lock)
+
+    @property
+    def cache_statistics(self) -> dict[str, Any] | None:
+        """
+        Returns the device cache statistics for logging purposes
+        """
+        # Need to ignore pylint no-member as Cache is a proxy class and pylint is not smart enough
+        # https://github.com/pylint-dev/pylint/issues/7258
+        if self.cache is not None:
+            stats = self.cache.hit_miss_ratio  # pylint: disable=no-member
+            return {"total_commands_sent": stats["total"], "cache_hits": stats["hits"], "cache_hit_ratio": f"{stats['hit_ratio'] * 100:.2f}%"}
+        return None
+
     def __rich_repr__(self) -> Iterator[tuple[str, Any]]:
         """
         Implements Rich Repr Protocol
         https://rich.readthedocs.io/en/stable/pretty.html#rich-repr-protocol
         """
         yield "name", self.name
         yield "tags", self.tags
         yield "hw_model", self.hw_model
         yield "is_online", self.is_online
         yield "established", self.established
+        yield "disable_cache", self.cache is None
 
     @abstractmethod
     def __eq__(self, other: object) -> bool:
         """
         AntaDevice equality depends on the class implementation.
         """
 
     @abstractmethod
-    async def collect(self, command: AntaCommand) -> None:
+    async def _collect(self, command: AntaCommand) -> None:
         """
         Collect device command output.
         This abstract coroutine can be used to implement any command collection method
         for a device in ANTA.
 
-        The `collect()` implementation needs to populate the `output` attribute
+        The `_collect()` implementation needs to populate the `output` attribute
         of the `AntaCommand` object passed as argument.
 
-        If a failure occurs, the `collect()` implementation is expected to catch the
+        If a failure occurs, the `_collect()` implementation is expected to catch the
         exception and implement proper logging, the `output` attribute of the
         `AntaCommand` object passed as argument would be `None` in this case.
 
         Args:
             command: the command to collect
         """
 
+    async def collect(self, command: AntaCommand) -> None:
+        """
+        Collects the output for a specified command.
+
+        When caching is activated on both the device and the command,
+        this method prioritizes retrieving the output from the cache. In cases where the output isn't cached yet,
+        it will be freshly collected and then stored in the cache for future access.
+        The method employs asynchronous locks based on the command's UID to guarantee exclusive access to the cache.
+
+        When caching is NOT enabled, either at the device or command level, the method directly collects the output
+        via the private `_collect` method without interacting with the cache.
+
+        Args:
+            command (AntaCommand): The command to process.
+        """
+        # Need to ignore pylint no-member as Cache is a proxy class and pylint is not smart enough
+        # https://github.com/pylint-dev/pylint/issues/7258
+        if self.cache is not None and self.cache_locks is not None and command.use_cache:
+            async with self.cache_locks[command.uid]:
+                cached_output = await self.cache.get(command.uid)  # pylint: disable=no-member
+
+                if cached_output is not None:
+                    logger.debug(f"Cache hit for {command.command} on {self.name}")
+                    command.output = cached_output
+                else:
+                    await self._collect(command=command)
+                    await self.cache.set(command.uid, command.output)  # pylint: disable=no-member
+        else:
+            await self._collect(command=command)
+
     async def collect_commands(self, commands: list[AntaCommand]) -> None:
         """
         Collect multiple commands.
 
         Args:
             commands: the commands to collect
         """
@@ -147,14 +209,15 @@
         enable_password: Optional[str] = None,
         port: Optional[int] = None,
         ssh_port: Optional[int] = 22,
         tags: Optional[list[str]] = None,
         timeout: Optional[float] = None,
         insecure: bool = False,
         proto: Literal["http", "https"] = "https",
+        disable_cache: bool = False,
     ) -> None:
         """
         Constructor of AsyncEOSDevice
 
         Args:
             host: Device FQDN or IP
             username: Username to connect to eAPI and SSH
@@ -164,18 +227,19 @@
             enable_password: Password used to gain privileged access on EOS
             port: eAPI port. Defaults to 80 is proto is 'http' or 443 if proto is 'https'.
             ssh_port: SSH port
             tags: List of tags for this device
             timeout: Timeout value in seconds for outgoing connections. Default to 10 secs.
             insecure: Disable SSH Host Key validation
             proto: eAPI protocol. Value can be 'http' or 'https'
+            disable_cache: Disable caching for all commands for this device. Defaults to False.
         """
         if name is None:
             name = f"{host}{f':{port}' if port else ''}"
-        super().__init__(name, tags)
+        super().__init__(name, tags, disable_cache)
         self.enable = enable
         self._enable_password = enable_password
         self._session: Device = Device(host=host, port=port, username=username, password=password, proto=proto, timeout=timeout)
         ssh_params: dict[str, Any] = {}
         if insecure:
             ssh_params.update({"known_hosts": None})
         self._ssh_opts: SSHClientConnectionOptions = SSHClientConnectionOptions(host=host, port=ssh_port, username=username, password=password, **ssh_params)
@@ -206,15 +270,15 @@
         Two AsyncEOSDevice objects are equal if the hostname and the port are the same.
         This covers the use case of port forwarding when the host is localhost and the devices have different ports.
         """
         if not isinstance(other, AsyncEOSDevice):
             return False
         return self._session.host == other._session.host and self._session.port == other._session.port
 
-    async def collect(self, command: AntaCommand) -> None:
+    async def _collect(self, command: AntaCommand) -> None:
         """
         Collect device command output from EOS using aio-eapi.
 
         Supports outformat `json` and `text` as output structure.
         Gain privileged access using the `enable_password` attribute
         of the `AntaDevice` instance if populated.
```

### Comparing `anta-0.8.0/anta/inventory/__init__.py` & `anta-0.9.0/anta/inventory/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,27 +41,42 @@
             if (dev_type := dev.__class__.__name__) not in devs:
                 devs[dev_type] = 1
             else:
                 devs[dev_type] += 1
         return f"ANTA Inventory contains {' '.join([f'{n} devices ({t})' for t, n in devs.items()])}"
 
     @staticmethod
+    def _update_disable_cache(inventory_disable_cache: bool, kwargs: dict[str, Any]) -> dict[str, Any]:
+        """
+        Return new dictionary, replacing kwargs with added disable_cache value from inventory_value
+        if disable_cache has not been set by CLI.
+
+        Args:
+            inventory_disable_cache (bool): The value of disable_cache in the inventory
+            kwargs: The kwargs to instantiate the device
+        """
+        updated_kwargs = kwargs.copy()
+        updated_kwargs["disable_cache"] = inventory_disable_cache or kwargs.get("disable_cache")
+        return updated_kwargs
+
+    @staticmethod
     def _parse_hosts(inventory_input: AntaInventoryInput, inventory: AntaInventory, **kwargs: Any) -> None:
         """
         Parses the host section of an AntaInventoryInput and add the devices to the inventory
 
         Args:
             inventory_input (AntaInventoryInput): AntaInventoryInput used to parse the devices
             inventory (AntaInventory): AntaInventory to add the parsed devices to
         """
         if inventory_input.hosts is None:
             return
 
         for host in inventory_input.hosts:
-            device = AsyncEOSDevice(name=host.name, host=str(host.host), port=host.port, tags=host.tags, **kwargs)
+            updated_kwargs = AntaInventory._update_disable_cache(host.disable_cache, kwargs)
+            device = AsyncEOSDevice(name=host.name, host=str(host.host), port=host.port, tags=host.tags, **updated_kwargs)
             inventory.add_device(device)
 
     @staticmethod
     def _parse_networks(inventory_input: AntaInventoryInput, inventory: AntaInventory, **kwargs: Any) -> None:
         """
         Parses the network section of an AntaInventoryInput and add the devices to the inventory.
 
@@ -73,16 +88,17 @@
             InventoryIncorrectSchema: Inventory file is not following AntaInventory Schema.
         """
         if inventory_input.networks is None:
             return
 
         for network in inventory_input.networks:
             try:
+                updated_kwargs = AntaInventory._update_disable_cache(network.disable_cache, kwargs)
                 for host_ip in ip_network(str(network.network)):
-                    device = AsyncEOSDevice(host=str(host_ip), tags=network.tags, **kwargs)
+                    device = AsyncEOSDevice(host=str(host_ip), tags=network.tags, **updated_kwargs)
                     inventory.add_device(device)
             except ValueError as e:
                 message = "Could not parse network {network.network} in the inventory"
                 anta_log_exception(e, message, logger)
                 raise InventoryIncorrectSchema(message) from e
 
     @staticmethod
@@ -98,20 +114,21 @@
             InventoryIncorrectSchema: Inventory file is not following AntaInventory Schema.
         """
         if inventory_input.ranges is None:
             return
 
         for range_def in inventory_input.ranges:
             try:
+                updated_kwargs = AntaInventory._update_disable_cache(range_def.disable_cache, kwargs)
                 range_increment = ip_address(str(range_def.start))
                 range_stop = ip_address(str(range_def.end))
                 while range_increment <= range_stop:  # type: ignore[operator]
                     # mypy raise an issue about comparing IPv4Address and IPv6Address
                     # but this is handled by the ipaddress module natively by raising a TypeError
-                    device = AsyncEOSDevice(host=str(range_increment), tags=range_def.tags, **kwargs)
+                    device = AsyncEOSDevice(host=str(range_increment), tags=range_def.tags, **updated_kwargs)
                     inventory.add_device(device)
                     range_increment += 1
             except ValueError as e:
                 message = f"Could not parse the following range in the inventory: {range_def.start} - {range_def.end}"
                 anta_log_exception(e, message, logger)
                 raise InventoryIncorrectSchema(message) from e
             except TypeError as e:
@@ -124,26 +141,30 @@
         inventory_file: str,
         username: str,
         password: str,
         enable: bool = False,
         enable_password: Optional[str] = None,
         timeout: Optional[float] = None,
         insecure: bool = False,
+        disable_cache: bool = False,
     ) -> AntaInventory:
         # pylint: disable=too-many-arguments
         """
         Create an AntaInventory instance from an inventory file.
         The inventory devices are AsyncEOSDevice instances.
 
         Args:
             inventory_file (str): Path to inventory YAML file where user has described his inputs
             username (str): Username to use to connect to devices
             password (str): Password to use to connect to devices
             enable (bool): Whether or not the commands need to be run in enable mode towards the devices
+            enable_password (str, optional): Enable password to use if required
             timeout (float, optional): timeout in seconds for every API call.
+            insecure (bool): Disable SSH Host Key validation
+            disable_cache (bool): Disable cache globally
 
         Raises:
             InventoryRootKeyError: Root key of inventory is missing.
             InventoryIncorrectSchema: Inventory file is not following AntaInventory Schema.
             InventoryUnknownFormat: Output format is not supported.
         """
 
@@ -151,14 +172,15 @@
         kwargs: dict[str, Any] = {
             "username": username,
             "password": password,
             "enable": enable,
             "enable_password": enable_password,
             "timeout": timeout,
             "insecure": insecure,
+            "disable_cache": disable_cache,
         }
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
         with open(inventory_file, "r", encoding="UTF-8") as file:
             data = safe_load(file)
 
         # Load data using Pydantic
```

### Comparing `anta-0.8.0/anta/loader.py` & `anta-0.9.0/anta/loader.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/models.py` & `anta-0.9.0/anta/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Use of this source code is governed by the Apache License 2.0
 # that can be found in the LICENSE file.
 """
 Models to define a TestStructure
 """
 from __future__ import annotations
 
+import hashlib
 import logging
 import time
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from datetime import timedelta
 from functools import wraps
 
@@ -59,35 +60,45 @@
     Can render a command from parameters.
 
     Attributes:
         template: Python f-string. Example: 'show vlan {vlan_id}'
         version: eAPI version - valid values are 1 or "latest" - default is "latest"
         revision: Revision of the command. Valid values are 1 to 99. Revision has precedence over version.
         ofmt: eAPI output - json or text - default is json
+        use_cache: Enable or disable caching for this AntaTemplate if the AntaDevice supports it - default is True
     """
 
     template: str
     version: Literal[1, "latest"] = "latest"
     revision: Optional[conint(ge=1, le=99)] = None  # type: ignore
     ofmt: Literal["json", "text"] = "json"
+    use_cache: bool = True
 
     def render(self, **params: dict[str, Any]) -> AntaCommand:
         """Render an AntaCommand from an AntaTemplate instance.
         Keep the parameters used in the AntaTemplate instance.
 
         Args:
             params: dictionary of variables with string values to render the Python f-string
 
         Returns:
             command: The rendered AntaCommand.
                      This AntaCommand instance have a template attribute that references this
                      AntaTemplate instance.
         """
         try:
-            return AntaCommand(command=self.template.format(**params), ofmt=self.ofmt, version=self.version, revision=self.revision, template=self, params=params)
+            return AntaCommand(
+                command=self.template.format(**params),
+                ofmt=self.ofmt,
+                version=self.version,
+                revision=self.revision,
+                template=self,
+                params=params,
+                use_cache=self.use_cache,
+            )
         except KeyError as e:
             raise AntaTemplateRenderError(self, e.args[0]) from e
 
 
 class AntaCommand(BaseModel):
     """Class to define a command.
 
@@ -103,30 +114,39 @@
         __Revision has precedence over version.__
 
     Attributes:
         command: Device command
         version: eAPI version - valid values are 1 or "latest" - default is "latest"
         revision: eAPI revision of the command. Valid values are 1 to 99. Revision has precedence over version.
         ofmt: eAPI output - json or text - default is json
+        output: Output of the command populated by the collect() function
         template: AntaTemplate object used to render this command
-        params: dictionary of variables with string values to render the template
+        params: Dictionary of variables with string values to render the template
         failed: If the command execution fails, the Exception object is stored in this field
+        use_cache: Enable or disable caching for this AntaCommand if the AntaDevice supports it - default is True
     """
 
     # This is required if we want to keep an Exception object in the failed field
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     command: str
     version: Literal[1, "latest"] = "latest"
     revision: Optional[conint(ge=1, le=99)] = None  # type: ignore
     ofmt: Literal["json", "text"] = "json"
     output: Optional[Union[Dict[str, Any], str]] = None
     template: Optional[AntaTemplate] = None
     failed: Optional[Exception] = None
     params: Dict[str, Any] = {}
+    use_cache: bool = True
+
+    @property
+    def uid(self) -> str:
+        """Generate a unique identifier for this command"""
+        uid_str = f"{self.command}_{self.version}_{self.revision or 'NA'}_{self.ofmt}"
+        return hashlib.sha1(uid_str.encode()).hexdigest()
 
     @property
     def json_output(self) -> dict[str, Any]:
         """Get the command output as JSON"""
         if self.output is None:
             raise RuntimeError(f"There is no output for command {self.command}")
         if self.ofmt != "json" or not isinstance(self.output, dict):
@@ -354,17 +374,20 @@
 
         if eos_data is not None:
             self.logger.debug(f"Test {self.name} initialized with input data")
             self.save_commands_data(eos_data)
 
     def save_commands_data(self, eos_data: list[dict[str, Any] | str]) -> None:
         """Populate output of all AntaCommand instances in `instance_commands`"""
-        if len(eos_data) != len(self.instance_commands):
+        if len(eos_data) > len(self.instance_commands):
             self.result.is_error(message="Test initialization error: Trying to save more data than there are commands for the test")
             return
+        if len(eos_data) < len(self.instance_commands):
+            self.result.is_error(message="Test initialization error: Trying to save less data than there are commands for the test")
+            return
         for index, data in enumerate(eos_data or []):
             self.instance_commands[index].output = data
 
     def __init_subclass__(cls) -> None:
         """Verify that the mandatory class attributes are defined"""
         mandatory_attributes = ["name", "description", "categories", "commands"]
         for attr in mandatory_attributes:
```

### Comparing `anta-0.8.0/anta/reporter/__init__.py` & `anta-0.9.0/anta/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/reporter/models.py` & `anta-0.9.0/anta/reporter/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/result_manager/__init__.py` & `anta-0.9.0/anta/result_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/result_manager/models.py` & `anta-0.9.0/anta/result_manager/models.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/runner.py` & `anta-0.9.0/anta/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,17 +41,18 @@
         any: ResultManager object gets updated with the test results.
     """
 
     await inventory.connect_inventory()
 
     # asyncio.gather takes an iterator of the function to run concurrently.
     # we get the cross product of the devices and tests to build that iterator.
-
+    devices = inventory.get_inventory(established_only=established_only, tags=tags).values()
     coros = []
-    for device, test in itertools.product(inventory.get_inventory(established_only=established_only, tags=tags).values(), tests):
+
+    for device, test in itertools.product(devices, tests):
         test_class = test[0]
         test_inputs = test[1]
         try:
             # Instantiate AntaTest object
             test_instance = test_class(device=device, inputs=test_inputs)
             coros.append(test_instance.test(eos_data=None))
         except Exception as e:  # pylint: disable=broad-exception-caught
@@ -66,7 +67,14 @@
     logger.debug(res)
     for r in res:
         if isinstance(r, Exception):
             message = "Error in main ANTA Runner"
             anta_log_exception(r, message, logger)
         else:
             manager.add_test_result(r)
+
+    # Get each device statistics
+    for device in devices:
+        if device.cache_statistics is not None:
+            logger.info(f"Cache statistics for {device.name}: {device.cache_statistics}")
+        else:
+            logger.info(f"Caching is not enabled on {device.name}")
```

### Comparing `anta-0.8.0/anta/tests/aaa.py` & `anta-0.9.0/anta/tests/aaa.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/configuration.py` & `anta-0.9.0/anta/tests/configuration.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/connectivity.py` & `anta-0.9.0/anta/tests/connectivity.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/field_notices.py` & `anta-0.9.0/anta/tests/field_notices.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/hardware.py` & `anta-0.9.0/anta/tests/hardware.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/interfaces.py` & `anta-0.9.0/anta/tests/interfaces.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/logging.py` & `anta-0.9.0/anta/tests/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     """
 
     name = "VerifyLoggingLogsGeneration"
     description = "Verifies if logs are generated."
     categories = ["logging"]
     commands = [
         AntaCommand(command="send log level informational message ANTA VerifyLoggingLogsGeneration validation"),
-        AntaCommand(command="show logging informational last 30 seconds | grep ANTA", ofmt="text"),
+        AntaCommand(command="show logging informational last 30 seconds | grep ANTA", ofmt="text", use_cache=False),
     ]
 
     @AntaTest.anta_test
     def test(self) -> None:
         log_pattern = r"ANTA VerifyLoggingLogsGeneration validation"
         output = self.instance_commands[1].text_output
         lines = output.strip().split("\n")[::-1]
@@ -169,15 +169,15 @@
 
     name = "VerifyLoggingHostname"
     description = "Verifies if logs are generated with the device FQDN."
     categories = ["logging"]
     commands = [
         AntaCommand(command="show hostname"),
         AntaCommand(command="send log level informational message ANTA VerifyLoggingHostname validation"),
-        AntaCommand(command="show logging informational last 30 seconds | grep ANTA", ofmt="text"),
+        AntaCommand(command="show logging informational last 30 seconds | grep ANTA", ofmt="text", use_cache=False),
     ]
 
     @AntaTest.anta_test
     def test(self) -> None:
         output_hostname = self.instance_commands[0].json_output
         output_logging = self.instance_commands[2].text_output
         fqdn = output_hostname["fqdn"]
@@ -204,15 +204,15 @@
     """
 
     name = "VerifyLoggingTimestamp"
     description = "Verifies if logs are generated with the appropriate timestamp."
     categories = ["logging"]
     commands = [
         AntaCommand(command="send log level informational message ANTA VerifyLoggingTimestamp validation"),
-        AntaCommand(command="show logging informational last 30 seconds | grep ANTA", ofmt="text"),
+        AntaCommand(command="show logging informational last 30 seconds | grep ANTA", ofmt="text", use_cache=False),
     ]
 
     @AntaTest.anta_test
     def test(self) -> None:
         log_pattern = r"ANTA VerifyLoggingTimestamp validation"
         timestamp_pattern = r"\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}\.\d{6}-\d{2}:\d{2}"
         output = self.instance_commands[1].text_output
```

### Comparing `anta-0.8.0/anta/tests/mlag.py` & `anta-0.9.0/anta/tests/mlag.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/multicast.py` & `anta-0.9.0/anta/tests/multicast.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/profiles.py` & `anta-0.9.0/anta/tests/profiles.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/routing/bgp.py` & `anta-0.9.0/anta/tests/routing/bgp.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/routing/generic.py` & `anta-0.9.0/anta/tests/routing/generic.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/routing/ospf.py` & `anta-0.9.0/anta/tests/routing/ospf.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/security.py` & `anta-0.9.0/anta/tests/security.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/snmp.py` & `anta-0.9.0/anta/tests/snmp.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/software.py` & `anta-0.9.0/anta/tests/software.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/stp.py` & `anta-0.9.0/anta/tests/stp.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,21 +175,23 @@
 
     @AntaTest.anta_test
     def test(self) -> None:
         command_output = self.instance_commands[0].json_output
         if not (stp_instances := command_output["instances"]):
             self.result.is_failure("No STP instances configured")
             return
-        for instance in stp_instances:
-            if instance.startswith("MST"):
-                prefix = "MST"
-                break
-            if instance.startswith("VL"):
-                prefix = "VL"
-                break
+        # Checking the type of instances based on first instance
+        first_name = list(stp_instances)[0]
+        if first_name.startswith("MST"):
+            prefix = "MST"
+        elif first_name.startswith("VL"):
+            prefix = "VL"
+        else:
+            self.result.is_failure(f"Unsupported STP instance type: {first_name}")
+            return
         check_instances = [f"{prefix}{instance_id}" for instance_id in self.inputs.instances] if self.inputs.instances else command_output["instances"].keys()
         wrong_priority_instances = [
             instance for instance in check_instances if get_value(command_output, f"instances.{instance}.rootBridge.priority") != self.inputs.priority
         ]
         if wrong_priority_instances:
             self.result.is_failure(f"The following instance(s) have the wrong STP root priority configured: {wrong_priority_instances}")
         else:
```

### Comparing `anta-0.8.0/anta/tests/system.py` & `anta-0.9.0/anta/tests/system.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tests/vxlan.py` & `anta-0.9.0/anta/tests/vxlan.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tools/get_value.py` & `anta-0.9.0/anta/tools/get_value.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tools/misc.py` & `anta-0.9.0/anta/tools/misc.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta/tools/pydantic.py` & `anta-0.9.0/anta/tools/pydantic.py`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta.egg-info/PKG-INFO` & `anta-0.9.0/anta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anta
-Version: 0.8.0
+Version: 0.9.0
 Summary: Arista Network Test Automation (ANTA) Framework
 Author-email: Khelil Sator <ksator@arista.com>
 Maintainer-email: Khelil Sator <ksator@arista.com>, Matthieu Tâche <mtache@arista.com>, Thomas Grimonet <tgrimonet@arista.com>, Guillaume Mulocher <gmulocher@arista.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -224,19 +224,20 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Networking
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiocache~=0.12.2
 Requires-Dist: aio-eapi==0.6.3
 Requires-Dist: click~=8.1.6
 Requires-Dist: click-help-colors~=0.9
 Requires-Dist: cvprac~=1.3.1
-Requires-Dist: pydantic<2.4.0,>=2.1.1
+Requires-Dist: pydantic<2.5.0,>=2.1.1
 Requires-Dist: PyYAML~=6.0
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rich~=13.5.2
 Requires-Dist: asyncssh~=2.13.2
 Requires-Dist: Jinja2~=3.1.2
 Provides-Extra: dev
 Requires-Dist: bumpver==2023.1126; extra == "dev"
@@ -340,23 +341,24 @@
   --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
                                   ANTA logging level  [env var:
                                   ANTA_LOG_LEVEL; default: INFO]
   --ignore-status                 Always exit with success  [env var:
                                   ANTA_IGNORE_STATUS]
   --ignore-error                  Only report failures and not errors  [env
                                   var: ANTA_IGNORE_ERROR]
+  --disable-cache                 Disable cache globally  [env var:
+                                  ANTA_DISABLE_CACHE]
   --help                          Show this message and exit.
 
 Commands:
   debug  Debug commands for building ANTA
   exec   Execute commands to inventory devices
   get    Get data from/to ANTA
   nrfu   Run NRFU against inventory devices
 ```
-
 > `username`, `password`, `enable-password`, `enable`, `timeout` and `insecure` values are the same for all devices
 
 
 ## Documentation
 
 The documentation is published on [ANTA package website](https://www.anta.ninja). Also, a [demo repository](https://github.com/titom73/atd-anta-demo) is available to facilitate your journey with ANTA.
```

### Comparing `anta-0.8.0/anta.egg-info/SOURCES.txt` & `anta-0.9.0/anta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anta-0.8.0/anta.egg-info/requires.txt` & `anta-0.9.0/anta.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+aiocache~=0.12.2
 aio-eapi==0.6.3
 click~=8.1.6
 click-help-colors~=0.9
 cvprac~=1.3.1
-pydantic<2.4.0,>=2.1.1
+pydantic<2.5.0,>=2.1.1
 PyYAML~=6.0
 requests~=2.31.0
 rich~=13.5.2
 asyncssh~=2.13.2
 Jinja2~=3.1.2
 
 [dev]
```

### Comparing `anta-0.8.0/docs/README.md` & `anta-0.9.0/docs/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -65,23 +65,24 @@
   --log-level, --log [CRITICAL|ERROR|WARNING|INFO|DEBUG]
                                   ANTA logging level  [env var:
                                   ANTA_LOG_LEVEL; default: INFO]
   --ignore-status                 Always exit with success  [env var:
                                   ANTA_IGNORE_STATUS]
   --ignore-error                  Only report failures and not errors  [env
                                   var: ANTA_IGNORE_ERROR]
+  --disable-cache                 Disable cache globally  [env var:
+                                  ANTA_DISABLE_CACHE]
   --help                          Show this message and exit.
 
 Commands:
   debug  Debug commands for building ANTA
   exec   Execute commands to inventory devices
   get    Get data from/to ANTA
   nrfu   Run NRFU against inventory devices
 ```
-
 > `username`, `password`, `enable-password`, `enable`, `timeout` and `insecure` values are the same for all devices
 
 
 ## Documentation
 
 The documentation is published on [ANTA package website](https://www.anta.ninja). Also, a [demo repository](https://github.com/titom73/atd-anta-demo) is available to facilitate your journey with ANTA.
```

### Comparing `anta-0.8.0/pyproject.toml` & `anta-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # content of pyproject.toml
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anta"
-version = "v0.8.0"
+version = "v0.9.0"
 readme = "docs/README.md"
 authors = [{ name = "Khelil Sator", email = "ksator@arista.com" }]
 maintainers = [
   { name = "Khelil Sator", email = "ksator@arista.com" },
   { name = "Matthieu Tâche", email = "mtache@arista.com" },
   { name = "Thomas Grimonet", email = "tgrimonet@arista.com" },
   { name = "Guillaume Mulocher", email = "gmulocher@arista.com" },
 ]
 description = "Arista Network Test Automation (ANTA) Framework"
 license = { file = "LICENSE" }
 dependencies = [
+  "aiocache~=0.12.2",
   "aio-eapi==0.6.3",
   "click~=8.1.6",
   "click-help-colors~=0.9",
   "cvprac~=1.3.1",
-  "pydantic>=2.1.1,<2.4.0",
+  "pydantic>=2.1.1,<2.5.0",
   "PyYAML~=6.0",
   "requests~=2.31.0",
   "rich~=13.5.2",
   "asyncssh~=2.13.2",
   "Jinja2~=3.1.2",
 ]
 keywords = ["test", "anta", "Arista", "network", "automation", "networking", "devops", "netdevops"]
@@ -102,15 +103,15 @@
 include = ["anta*"]
 namespaces = false
 
 ################################
 # Version
 ################################
 [tool.bumpver]
-current_version = "0.8.0"
+current_version = "0.9.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "bump: Version {old_version} -> {new_version}"
 commit = true
 # No tag
 tag = false
 push = false
```

