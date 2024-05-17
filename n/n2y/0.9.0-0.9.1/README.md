# Comparing `tmp/n2y-0.9.0.tar.gz` & `tmp/n2y-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "n2y-0.9.0.tar", last modified: Thu Feb  1 19:11:36 2024, max compression
+gzip compressed data, was "n2y-0.9.1.tar", last modified: Thu Feb  1 19:35:13 2024, max compression
```

## Comparing `n2y-0.9.0.tar` & `n2y-0.9.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:36.531002 n2y-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-01 19:11:36.531002 n2y-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29337 2024-02-01 19:11:20.000000 n2y-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:36.523002 n2y-0.9.0/n2y/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    30953 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:36.523002 n2y-0.9.0/n2y/data/
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/data/mermaid_err.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/emoji.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26088 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/notion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/notion_mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:36.527002 n2y-0.9.0/n2y/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/dbfootnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/deepheaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/downloadfileproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/expandbluetoggles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/expandlinktopages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)    19367 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/jinjarenderpage.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/linkedheaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/rawcodeblocks.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/plugins/removecallouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/properties.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/property_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/rich_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-02-01 19:11:20.000000 n2y-0.9.0/n2y/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:36.531002 n2y-0.9.0/n2y.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-01 19:11:36.000000 n2y-0.9.0/n2y.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-01 19:11:36.000000 n2y-0.9.0/n2y.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 19:11:36.000000 n2y-0.9.0/n2y.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-01 19:11:36.000000 n2y-0.9.0/n2y.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-01 19:11:36.000000 n2y-0.9.0/n2y.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-01 19:11:36.000000 n2y-0.9.0/n2y.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-01 19:11:36.531002 n2y-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-01 19:11:20.000000 n2y-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:11:36.531002 n2y-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_append_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_audit_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16123 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_expandbluetoggles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_first_pass_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_jinjarenderpage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_linkedheaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_plain_text_to_pandoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_plugin_dbfootnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_property_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_rich_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-01 19:11:20.000000 n2y-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:35:13.016121 n2y-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-01 19:35:13.016121 n2y-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29392 2024-02-01 19:34:57.000000 n2y-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:35:13.012121 n2y-0.9.1/n2y/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30953 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:35:13.012121 n2y-0.9.1/n2y/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/data/mermaid_err.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26088 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/notion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/notion_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:35:13.012121 n2y-0.9.1/n2y/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/dbfootnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/deepheaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/downloadfileproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/expandbluetoggles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/expandlinktopages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19367 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/jinjarenderpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/linkedheaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/rawcodeblocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/plugins/removecallouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/property_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8076 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-02-01 19:34:57.000000 n2y-0.9.1/n2y/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:35:13.016121 n2y-0.9.1/n2y.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-01 19:35:12.000000 n2y-0.9.1/n2y.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-01 19:35:13.000000 n2y-0.9.1/n2y.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 19:35:12.000000 n2y-0.9.1/n2y.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-01 19:35:13.000000 n2y-0.9.1/n2y.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-01 19:35:13.000000 n2y-0.9.1/n2y.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-01 19:35:13.000000 n2y-0.9.1/n2y.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-01 19:35:13.016121 n2y-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-01 19:34:57.000000 n2y-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 19:35:13.016121 n2y-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_append_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_audit_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25872 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16123 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_expandbluetoggles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_first_pass_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11976 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_jinjarenderpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_linkedheaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_plain_text_to_pandoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_plugin_dbfootnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_property_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-01 19:34:57.000000 n2y-0.9.1/tests/test_utils.py
```

### Comparing `n2y-0.9.0/PKG-INFO` & `n2y-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n2y
-Version: 0.9.0
+Version: 0.9.1
 Summary: Notion to YAML
 Home-page: https://github.com/innolitics/n2y
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: notion documentation yaml markdown
 Classifier: Development Status :: 4 - Beta
```

### Comparing `n2y-0.9.0/README.md` & `n2y-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,17 @@
 - Make the plugin system more fully featured and easier to use
 - Add support for recursively dumping sets of pages and preserving links between them
 - Add some sort of Notion API caching mechanism
 - Add more examples to the documentation
 
 ## Changelog
 
+### v0.9.1
+- Delete print statement in `rich_text.py`
+
 ### v0.9.0
 - pass the `pandoc_options` setting to wherever `pandoc.write` is called for consistency. Also,
   this should reasonably be the expected behavior.
 
 ### v0.8.2
 
 - stop filtering linebreaks from table cells
```

### Comparing `n2y-0.9.0/n2y/audit.py` & `n2y-0.9.1/n2y/audit.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/blocks.py` & `n2y-0.9.1/n2y/blocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/comment.py` & `n2y-0.9.1/n2y/comment.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/config.py` & `n2y-0.9.1/n2y/config.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/data/mermaid_err.png` & `n2y-0.9.1/n2y/data/mermaid_err.png`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/database.py` & `n2y-0.9.1/n2y/database.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/errors.py` & `n2y-0.9.1/n2y/errors.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/export.py` & `n2y-0.9.1/n2y/export.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/file.py` & `n2y-0.9.1/n2y/file.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/main.py` & `n2y-0.9.1/n2y/main.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/mentions.py` & `n2y-0.9.1/n2y/mentions.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/notion.py` & `n2y-0.9.1/n2y/notion.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/notion_mocks.py` & `n2y-0.9.1/n2y/notion_mocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/page.py` & `n2y-0.9.1/n2y/page.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/dbfootnotes.py` & `n2y-0.9.1/n2y/plugins/dbfootnotes.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/deepheaders.py` & `n2y-0.9.1/n2y/plugins/deepheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/downloadfileproperty.py` & `n2y-0.9.1/n2y/plugins/downloadfileproperty.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/expandbluetoggles.py` & `n2y-0.9.1/n2y/plugins/expandbluetoggles.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/expandlinktopages.py` & `n2y-0.9.1/n2y/plugins/expandlinktopages.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/footnotes.py` & `n2y-0.9.1/n2y/plugins/footnotes.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/jinjarenderpage.py` & `n2y-0.9.1/n2y/plugins/jinjarenderpage.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/linkedheaders.py` & `n2y-0.9.1/n2y/plugins/linkedheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/mermaid.py` & `n2y-0.9.1/n2y/plugins/mermaid.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/plugins/rawcodeblocks.py` & `n2y-0.9.1/n2y/plugins/rawcodeblocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/properties.py` & `n2y-0.9.1/n2y/properties.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/property_values.py` & `n2y-0.9.1/n2y/property_values.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/rich_text.py` & `n2y-0.9.1/n2y/rich_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,14 @@
     def __getitem__(self, index):
         return self.items[index]
 
     def to_pandoc(self):
         return sum([item.to_pandoc() for item in self.items], [])
 
     def to_value(self, pandoc_format, pandoc_options):
-        print(self.client.export_defaults)
         return pandoc_write_or_log_errors(
             self.to_pandoc(),
             format=pandoc_format,
             options=pandoc_options,
         )
 
     def to_plain_text(self):
```

### Comparing `n2y-0.9.0/n2y/user.py` & `n2y-0.9.1/n2y/user.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y/utils.py` & `n2y-0.9.1/n2y/utils.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/n2y.egg-info/PKG-INFO` & `n2y-0.9.1/n2y.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: n2y
-Version: 0.9.0
+Version: 0.9.1
 Summary: Notion to YAML
 Home-page: https://github.com/innolitics/n2y
 Author: Innolitics, LLC
 Author-email: info@innolitics.com
 License: MIT
 Keywords: notion documentation yaml markdown
 Classifier: Development Status :: 4 - Beta
```

### Comparing `n2y-0.9.0/n2y.egg-info/SOURCES.txt` & `n2y-0.9.1/n2y.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/setup.py` & `n2y-0.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 description = "Notion to YAML"
 
 setup(
     name="n2y",
-    version="0.9.0",
+    version="0.9.1",
     description=description,
     long_description=description,
     long_description_content_type="text/x-rst",
     url="https://github.com/innolitics/n2y",
     author="Innolitics, LLC",
     author_email="info@innolitics.com",
     license="MIT",
```

### Comparing `n2y-0.9.0/tests/test_append_end_to_end.py` & `n2y-0.9.1/tests/test_append_end_to_end.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_audit_end_to_end.py` & `n2y-0.9.1/tests/test_audit_end_to_end.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_blocks.py` & `n2y-0.9.1/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_config.py` & `n2y-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_end_to_end.py` & `n2y-0.9.1/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_expandbluetoggles.py` & `n2y-0.9.1/tests/test_expandbluetoggles.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_export.py` & `n2y-0.9.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_first_pass_output.py` & `n2y-0.9.1/tests/test_first_pass_output.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_jinjarenderpage.py` & `n2y-0.9.1/tests/test_jinjarenderpage.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_linkedheaders.py` & `n2y-0.9.1/tests/test_linkedheaders.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_plain_text_to_pandoc.py` & `n2y-0.9.1/tests/test_plain_text_to_pandoc.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_plugin_dbfootnotes.py` & `n2y-0.9.1/tests/test_plugin_dbfootnotes.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_plugins.py` & `n2y-0.9.1/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_property_values.py` & `n2y-0.9.1/tests/test_property_values.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_rich_text.py` & `n2y-0.9.1/tests/test_rich_text.py`

 * *Files identical despite different names*

### Comparing `n2y-0.9.0/tests/test_utils.py` & `n2y-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

