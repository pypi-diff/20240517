# Comparing `tmp/aurora_cli-2.6.0.0.tar.gz` & `tmp/aurora_cli-2.6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aurora_cli-2.6.0.0.tar", last modified: Thu May  2 18:27:35 2024, max compression
+gzip compressed data, was "aurora_cli-2.6.0.1.tar", last modified: Fri May 17 16:12:36 2024, max compression
```

## Comparing `aurora_cli-2.6.0.0.tar` & `aurora_cli-2.6.0.1.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/LICENSE
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1260 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/README.md
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2177 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/__main__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/src/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/src/features/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.509164 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3695 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_device.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3206 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     6158 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator_vm.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3478 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/common.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2900 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4015 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4846 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_build.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1013 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7772 2024-04-28 14:23:20.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4481 2024-05-02 18:22:53.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2039 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_icon.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5129 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_plugins.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    24329 2024-04-28 13:49:56.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1958 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1078 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_available.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1945 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_clear.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5457 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_install.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1165 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_installed.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4767 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_package.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1542 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_remove.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2994 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sign.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1977 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1351 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_targets.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2248 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_validate.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     8046 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4011 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/group_sdk.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.513164 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2597 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/utils.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/aurora_cli/src/support/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/__init__.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/__init__.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2413 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1499 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7080 2024-05-02 18:23:24.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/conf.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1291 2024-04-28 14:22:58.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/dependency.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1979 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/dependency_required.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3096 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/download.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7232 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/helper.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1965 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/output.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1531 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/sdk.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5097 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/ssh.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    17907 2024-04-28 14:20:11.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/texts.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2119 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/vbox.py
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2098 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.0/aurora_cli/src/support/versions.py
-drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/aurora_cli.egg-info/
--rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/PKG-INFO
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2623 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       56 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/entry_points.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      168 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/requires.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       18 2024-05-02 18:27:35.000000 aurora_cli-2.6.0.0/aurora_cli.egg-info/top_level.txt
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-05-02 18:27:35.517164 aurora_cli-2.6.0.0/setup.cfg
--rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1823 2024-05-02 18:23:17.000000 aurora_cli-2.6.0.0/setup.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    11358 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/LICENSE
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1260 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/README.md
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2177 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.1/aurora_cli/__main__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/features/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3695 2024-05-17 15:19:03.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/group_device.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3206 2024-05-17 15:19:10.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/group_emulator.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     6158 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/group_emulator_vm.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4177 2024-05-17 15:53:55.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/impl/common.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2900 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/devices/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4149 2024-05-17 05:16:20.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4846 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_build.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1013 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_debug.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7772 2024-04-28 14:23:20.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_debug_dart.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4481 2024-05-02 18:22:53.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4136 2024-05-17 08:51:27.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_format.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2039 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_icon.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5129 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_plugins.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    24329 2024-04-28 13:49:56.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1958 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1078 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_available.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1945 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_clear.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5457 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_install.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1165 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_installed.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4767 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_package.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1542 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_remove.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2994 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_sign.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1977 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_sudoers.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1351 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_targets.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2248 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_validate.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.566173 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     8046 2024-04-28 08:53:15.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     4011 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/group_sdk.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/impl/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/impl/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2597 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/impl/utils.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/aurora_cli/src/support/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/__init__.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/aurora_cli/src/support/alive_bar/
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        0 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/alive_bar/__init__.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2413 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1499 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/alive_bar/progress_alive_bar.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7325 2024-05-17 15:05:07.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/conf.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1291 2024-04-28 14:22:58.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/dependency.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2270 2024-05-17 04:52:58.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/dependency_required.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     3096 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/download.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     7317 2024-05-17 05:35:59.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/helper.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1965 2024-03-16 15:04:33.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/output.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1531 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/sdk.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     5097 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/ssh.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)    19030 2024-05-17 06:46:28.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/texts.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2119 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/vbox.py
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2098 2024-04-27 18:28:50.000000 aurora_cli-2.6.0.1/aurora_cli/src/support/versions.py
+drwxrwxr-x   0 keygenqt  (1000) keygenqt  (1000)        0 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/aurora_cli.egg-info/
+-rw-r--r--   0 keygenqt  (1000) keygenqt  (1000)     1474 2024-05-17 16:12:36.000000 aurora_cli-2.6.0.1/aurora_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     2679 2024-05-17 16:12:36.000000 aurora_cli-2.6.0.1/aurora_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)        1 2024-05-17 16:12:36.000000 aurora_cli-2.6.0.1/aurora_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       56 2024-05-17 16:12:36.000000 aurora_cli-2.6.0.1/aurora_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)      168 2024-05-17 16:12:36.000000 aurora_cli-2.6.0.1/aurora_cli.egg-info/requires.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       18 2024-05-17 16:12:36.000000 aurora_cli-2.6.0.1/aurora_cli.egg-info/top_level.txt
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)       38 2024-05-17 16:12:36.570173 aurora_cli-2.6.0.1/setup.cfg
+-rw-rw-r--   0 keygenqt  (1000) keygenqt  (1000)     1823 2024-05-17 16:12:11.000000 aurora_cli-2.6.0.1/setup.py
```

### Comparing `aurora_cli-2.6.0.0/LICENSE` & `aurora_cli-2.6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/PKG-INFO` & `aurora_cli-2.6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-cli
-Version: 2.6.0.0
+Version: 2.6.0.1
 Summary: An application that simplifies the life of an application developer for the Aurora OS.
 Home-page: https://github.com/keygenqt/aurora-cli
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aurora_cli-2.6.0.0/README.md` & `aurora_cli-2.6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/__main__.py` & `aurora_cli-2.6.0.1/aurora_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_device.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/devices/group_device.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/devices/group_emulator.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/group_emulator_vm.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/devices/group_emulator_vm.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/common.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/devices/impl/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,34 +65,50 @@
     if not paths:
         echo_stderr(AppTexts.file_no_one_not_found())
         exit(1)
 
     # Folder upload
     upload_path = '/home/defaultuser/Downloads'
 
+    # Check version Aurora OS
+    is_apm = False
+    _, ssh_stdout, _ = client.exec_command('version')
+    for value in iter(ssh_stdout.readline, ""):
+        print(str(value).strip())
+        is_apm = 'Aurora 5.0' in str(value).strip()
+
     for path in paths:
         echo_line()
         echo_stdout(AppTexts.start_upload(path))
         if upload_file_sftp(client, upload_path, path):
             # Get file name
             file_name = os.path.basename(path)
             # Exec command
-            if data:
-                execute = 'echo {} | {} {upload_path}/{file_name}'.format(
-                    data['devel-su'],
-                    'devel-su pkcon -y install-local',
-                    upload_path=upload_path,
-                    file_name=file_name
-                )
+            if is_apm:
+                prompt = "{'ShowPrompt': <false>}"
+                execute = (f'gdbus call --system '
+                           f'--dest ru.omp.APM '
+                           f'--object-path /ru/omp/APM '
+                           f'--method ru.omp.APM.Install '
+                           f'"{upload_path}/{file_name}" '
+                           f'"{prompt}"')
             else:
-                execute = '{} {upload_path}/{file_name}'.format(
-                    'pkcon -y install-local',
-                    upload_path=upload_path,
-                    file_name=file_name
-                )
+                if data:
+                    execute = 'echo {} | {} {upload_path}/{file_name}'.format(
+                        data['devel-su'],
+                        'devel-su pkcon -y install-local',
+                        upload_path=upload_path,
+                        file_name=file_name
+                    )
+                else:
+                    execute = '{} {upload_path}/{file_name}'.format(
+                        'pkcon -y install-local',
+                        upload_path=upload_path,
+                        file_name=file_name
+                    )
             echo_line()
             if verbose != VerboseType.verbose:
                 echo_stdout(AppTexts.package_install_loading())
             # Execute command
             ssh_client_exec_command(client, execute, verbose, ['^error.+', '.+error.+'])
 
     # Close ssh client
```

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/devices/impl/utils.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/devices/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pathlib import Path
 
 import click
 from git import Repo
 
 from aurora_cli.src.features.flutter.group_flutter_build import group_flutter_build
 from aurora_cli.src.features.flutter.group_flutter_debug import group_flutter_debug
+from aurora_cli.src.features.flutter.group_flutter_format import group_flutter_format
 from aurora_cli.src.features.flutter.group_flutter_icon import group_flutter_icons
 from aurora_cli.src.features.flutter.group_flutter_plugins import group_flutter_plugins
 from aurora_cli.src.features.flutter.impl.utils import get_list_flutter_installed
 from aurora_cli.src.support.alive_bar.git_progress_alive_bar import GitProgressAliveBar
 from aurora_cli.src.support.helper import prompt_index, clear_file_line
 from aurora_cli.src.support.output import echo_stdout, echo_stderr
 from aurora_cli.src.support.texts import AppTexts
@@ -39,14 +40,15 @@
 
 
 # Add subgroup
 group_flutter.add_command(group_flutter_debug)
 group_flutter.add_command(group_flutter_build)
 group_flutter.add_command(group_flutter_plugins)
 group_flutter.add_command(group_flutter_icons)
+group_flutter.add_command(group_flutter_format)
 
 
 @group_flutter.command()
 def available():
     """Get available versions Flutter SDK."""
 
     versions = get_versions_flutter()
```

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_build.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_build.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_debug.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_dart.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_debug_dart.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_debug_gdb.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_icon.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_icon.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/group_flutter_plugins.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/group_flutter_plugins.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/flutter/impl/utils.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/flutter/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_available.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_available.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_clear.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_clear.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_install.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_install.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_installed.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_installed.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_package.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_package.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_remove.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_remove.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sign.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_sign.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_sudoers.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_sudoers.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_targets.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_targets.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/group_psdk_validate.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/group_psdk_validate.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/psdk/impl/utils.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/psdk/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/group_sdk.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/group_sdk.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/features/sdk/impl/utils.py` & `aurora_cli-2.6.0.1/aurora_cli/src/features/sdk/impl/utils.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/alive_bar/git_progress_alive_bar.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/alive_bar/progress_alive_bar.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/alive_bar/progress_alive_bar.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/conf.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 # Temp folder
 PATH_TEMP = '~/.aurora-cli/temp'
 
 # Public key pairs
 URL_KEY = 'https://developer.auroraos.ru/static/regular_key.pem'
 URL_CERT = 'https://developer.auroraos.ru/static/regular_cert.pem'
 
+# Configuration file clang-format
+URL_CLANG_FORMAT_CONF = 'https://gitlab.com/omprussia/flutter/flutter/-/raw/stable/.clang-format'
+
 
 # Loader configuration yaml
 class Conf:
 
     @staticmethod
     def get_temp_folder() -> str:
         temp_folder = Path(get_path_file(PATH_TEMP, check_exist=False))
@@ -150,14 +153,18 @@
         # Check and download key pairs
         Conf._check_key_pairs(self.conf_path)
 
         # Load config
         with open(self.conf_path, 'rb') as file:
             self.conf = load(file.read(), Loader=Loader)
 
+    # Get config folder
+    def get_folder(self) -> Path:
+        return Path(os.path.dirname(self.conf_path))
+
     # Get config path
     def get_path(self) -> Path:
         return self.conf_path
 
     # Get config keys
     def get_workdir(self) -> Path:
         if 'workdir' not in self.conf.keys():
```

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/dependency.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/dependency.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/dependency_required.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/dependency_required.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,7 +54,16 @@
 # Check dependency gdb-multiarch
 def check_dependency_gdb_multiarch():
     try:
         subprocess.run(['gdb-multiarch', '--version'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
     except (Exception,):
         echo_stderr(AppTexts.error_dependency_gdb_multiarch())
         exit(1)
+
+
+# Check dependency clang-format
+def check_dependency_clang_format():
+    try:
+        subprocess.run(['clang-format', '--version'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    except (Exception,):
+        echo_stderr(AppTexts.error_dependency_clang_format())
+        exit(1)
```

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/download.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/download.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/helper.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,29 +103,33 @@
 def find_path_file(extension: str, path: Path) -> Path | None:
     files = glob.glob(f'{path}/*.{extension}')
     if files:
         return Path(files[0])
     return None
 
 
-# Get full path file
-def get_path_file(path: str, check_exist=True) -> str | None:
-    if not path:
-        return None
-
+# Get path
+def get_format_path(path: str) -> Path:
     # Format path
     if path.startswith('~/'):
         path = os.path.expanduser(path)
     if path.startswith('./'):
         path = '{}{}'.format(os.getcwd(), path[1:])
     if path.startswith('../'):
         path = '{}/{}'.format(os.getcwd(), path)
+    return Path(path)
+
+
+# Get full path file
+def get_path_file(path: str, check_exist=True) -> str | None:
+    if not path:
+        return None
 
     # Read path
-    path = Path(path)
+    path = get_format_path(path)
 
     if not check_exist:
         return str(path.absolute())
 
     # Check exist
     if path.is_file():
         return str(path.absolute())
```

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/output.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/output.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/sdk.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/sdk.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/ssh.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/ssh.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/texts.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/texts.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,19 @@
 
     @staticmethod
     def error_dependency_gdb_multiarch():
         return ('<red>Application</red> "gdb-multiarch" <red>not found, install it.</red>'
                 + ('\nTry: sudo apt install gdb-multiarch' if check_dependency_apt() else ''))
 
     @staticmethod
+    def error_dependency_clang_format():
+        return ('<red>Application</red> "clang-format" <red>not found, install it.</red>'
+                + ('\nTry: sudo apt install clang-format' if check_dependency_apt() else ''))
+
+    @staticmethod
     def error_connect_internet():
         return '<red>Internet connection error. Check the connection.</red>'
 
     @staticmethod
     def error_find_ssh_key(path_key: str):
         return ('<red>Public-key authentication is required to connect to the debug</red>.\n'
                 '<red>Key not found:</red> {path}').format(path=path_key)
@@ -134,14 +139,18 @@
                  '\n<cyan>For detailed reporting, use the</cyan> --verbose (-v) <cyan>flag.</cyan>'))
 
     @staticmethod
     def file_not_found(path: str):
         return '<red>File path not found:</red> {}'.format(path)
 
     @staticmethod
+    def dir_not_found(path: str):
+        return '<red>Directory path not found:</red> {}'.format(path)
+
+    @staticmethod
     def already_exists(name: str):
         return '<blue>Already exists:</blue> {}'.format(name)
 
     @staticmethod
     def download(name: str):
         return '<blue>Download:</blue> {}'.format(name)
 
@@ -206,14 +215,18 @@
         return '<red>Virtual machine not found.</red>'
 
     @staticmethod
     def flutter_not_found():
         return '<red>Flutter installed not found.</red>'
 
     @staticmethod
+    def configuration_clang_format_not_found():
+        return '<red>The clang-format configuration file is required.</red>'
+
+    @staticmethod
     def flutter_error_read_json():
         return '<red>Error read json file.</red>'
 
     @staticmethod
     def flutter_platform_specific_plugins(plugins: []):
         if not plugins or len(plugins) == 1:
             return None
@@ -256,14 +269,18 @@
         return '<green>Configuration file created successfully:</green> {}'.format(path)
 
     @staticmethod
     def conf_download_keys_confirm():
         return 'Download public keys for sign RPM packages?'
 
     @staticmethod
+    def conf_download_clang_format_conf_confirm():
+        return 'Download clang-format configuration file?'
+
+    @staticmethod
     def conf_download_keys_success(path: str):
         return '<green>Public key pairs download successfully:</green> {}'.format(path)
 
     @staticmethod
     def flutter_versions(versions: []):
         return 'Available versions Flutter SDK:\n{}'.format('\n'.join(versions))
 
@@ -526,7 +543,19 @@
     @staticmethod
     def flutter_icons_create_success(path: str):
         return '<green>Create icons successfully:</green> {}'.format(path)
 
     @staticmethod
     def confirm_image_size():
         return 'The image\'s width and height are not equal, continue?'
+
+    @staticmethod
+    def end_format(count_files: int, time_end: str):
+        return 'Formatted {count_f} files in {time} seconds.'.format(count_f=count_files, time=time_end)
+
+    @staticmethod
+    def run_clang_format(path: str):
+        return '<blue>Format</blue> <red>C++</red> <blue>files folder:</blue> {}'.format(path)
+
+    @staticmethod
+    def run_dart_format(path: str):
+        return '<blue>Format</blue> <green>Dart</green> <blue>files folder:</blue> {}'.format(path)
```

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/vbox.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/vbox.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli/src/support/versions.py` & `aurora_cli-2.6.0.1/aurora_cli/src/support/versions.py`

 * *Files identical despite different names*

### Comparing `aurora_cli-2.6.0.0/aurora_cli.egg-info/PKG-INFO` & `aurora_cli-2.6.0.1/aurora_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aurora-cli
-Version: 2.6.0.0
+Version: 2.6.0.1
 Summary: An application that simplifies the life of an application developer for the Aurora OS.
 Home-page: https://github.com/keygenqt/aurora-cli
 Author: Vitaliy Zarubin
 Author-email: keygenqt@gmail.com
 Requires-Python: >=3.8.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aurora_cli-2.6.0.0/aurora_cli.egg-info/SOURCES.txt` & `aurora_cli-2.6.0.1/aurora_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 aurora_cli/src/features/devices/impl/utils.py
 aurora_cli/src/features/flutter/__init__.py
 aurora_cli/src/features/flutter/group_flutter.py
 aurora_cli/src/features/flutter/group_flutter_build.py
 aurora_cli/src/features/flutter/group_flutter_debug.py
 aurora_cli/src/features/flutter/group_flutter_debug_dart.py
 aurora_cli/src/features/flutter/group_flutter_debug_gdb.py
+aurora_cli/src/features/flutter/group_flutter_format.py
 aurora_cli/src/features/flutter/group_flutter_icon.py
 aurora_cli/src/features/flutter/group_flutter_plugins.py
 aurora_cli/src/features/flutter/impl/__init__.py
 aurora_cli/src/features/flutter/impl/utils.py
 aurora_cli/src/features/psdk/__init__.py
 aurora_cli/src/features/psdk/group_psdk.py
 aurora_cli/src/features/psdk/group_psdk_available.py
```

### Comparing `aurora_cli-2.6.0.0/setup.py` & `aurora_cli-2.6.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 See the License for the specific language governing permissions and
 limitations under the License.
 ```
 """
 
 setuptools.setup(
     name='aurora-cli',
-    version='2.6.0.0',
+    version='2.6.0.1',
     author='Vitaliy Zarubin',
     author_email='keygenqt@gmail.com',
     description='An application that simplifies the life of an application developer for the Aurora OS.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/keygenqt/aurora-cli",
     packages=setuptools.find_packages(exclude=['*tests.*', '*tests']),
```

