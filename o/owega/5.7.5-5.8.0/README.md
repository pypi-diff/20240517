# Comparing `tmp/owega-5.7.5.tar.gz` & `tmp/owega-5.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.7.5.tar", last modified: Tue May 14 11:40:57 2024, max compression
+gzip compressed data, was "owega-5.8.0.tar", last modified: Fri May 17 21:54:38 2024, max compression
```

## Comparing `owega-5.7.5.tar` & `owega-5.8.0.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:57.000029 owega-5.7.5/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-14 10:31:00.000000 owega-5.7.5/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16703 2024-05-14 11:40:57.000029 owega-5.7.5/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5183 2024-05-14 10:31:00.000000 owega-5.7.5/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.990029 owega-5.7.5/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.996029 owega-5.7.5/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-07 09:02:58.000000 owega-5.7.5/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-14 10:31:00.000000 owega-5.7.5/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-14 10:30:45.000000 owega-5.7.5/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2407 2024-05-07 09:02:58.000000 owega-5.7.5/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.997029 owega-5.7.5/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-05-07 09:02:58.000000 owega-5.7.5/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-02-19 10:01:29.000000 owega-5.7.5/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-05-07 09:02:58.000000 owega-5.7.5/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-05-07 09:02:58.000000 owega-5.7.5/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.998029 owega-5.7.5/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-02-19 10:01:29.000000 owega-5.7.5/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3460 2024-05-14 11:20:30.000000 owega-5.7.5/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-05-07 09:02:58.000000 owega-5.7.5/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-14 10:30:45.000000 owega-5.7.5/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-02-19 10:01:29.000000 owega-5.7.5/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-14 10:31:00.000000 owega-5.7.5/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.998029 owega-5.7.5/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-05-07 09:02:58.000000 owega-5.7.5/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    25209 2024-05-14 11:35:10.000000 owega-5.7.5/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-05-07 09:02:58.000000 owega-5.7.5/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-02-19 10:01:29.000000 owega-5.7.5/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.999029 owega-5.7.5/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-02-19 10:01:29.000000 owega-5.7.5/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1850 2024-05-14 11:26:56.000000 owega-5.7.5/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.999029 owega-5.7.5/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-02-19 10:01:29.000000 owega-5.7.5/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-07 09:02:58.000000 owega-5.7.5/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-14 10:31:00.000000 owega-5.7.5/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-02-19 10:01:29.000000 owega-5.7.5/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-14 10:31:00.000000 owega-5.7.5/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11604 2024-05-14 10:31:00.000000 owega-5.7.5/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-14 10:31:00.000000 owega-5.7.5/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-14 11:40:56.999029 owega-5.7.5/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16703 2024-05-14 11:40:56.000000 owega-5.7.5/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1656 2024-05-14 11:40:56.000000 owega-5.7.5/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-14 11:40:56.000000 owega-5.7.5/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-14 11:40:56.000000 owega-5.7.5/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-14 11:40:56.000000 owega-5.7.5/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-14 11:40:56.000000 owega-5.7.5/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-01-18 13:10:34.000000 owega-5.7.5/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-14 11:40:57.000029 owega-5.7.5/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2109 2024-05-14 10:31:00.000000 owega-5.7.5/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-17 21:44:57.000000 owega-5.8.0/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16737 2024-05-17 21:54:38.146937 owega-5.8.0/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5183 2024-05-17 21:44:57.000000 owega-5.8.0/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.144938 owega-5.8.0/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.145938 owega-5.8.0/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1302 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_time.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2470 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.145938 owega-5.8.0/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.145938 owega-5.8.0/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3628 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-05-17 21:44:57.000000 owega-5.8.0/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-17 21:44:57.000000 owega-5.8.0/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-05-17 21:44:57.000000 owega-5.8.0/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10338 2024-05-17 21:44:57.000000 owega-5.8.0/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    25331 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-05-17 21:44:57.000000 owega-5.8.0/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-05-17 21:44:57.000000 owega-5.8.0/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2655 2024-05-17 21:44:57.000000 owega-5.8.0/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-05-17 21:44:57.000000 owega-5.8.0/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-17 21:44:57.000000 owega-5.8.0/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-17 21:44:57.000000 owega-5.8.0/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-05-17 21:44:57.000000 owega-5.8.0/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-17 21:44:57.000000 owega-5.8.0/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11780 2024-05-17 21:44:57.000000 owega-5.8.0/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-17 21:44:57.000000 owega-5.8.0/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 21:54:38.146937 owega-5.8.0/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16737 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-17 21:54:38.000000 owega-5.8.0/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-05-17 21:44:57.000000 owega-5.8.0/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-17 21:54:38.146937 owega-5.8.0/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2093 2024-05-17 21:44:57.000000 owega-5.8.0/setup.py
```

### Comparing `owega-5.7.5/LICENSE` & `owega-5.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/PKG-INFO` & `owega-5.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.7.5
+Version: 5.8.0
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -142,15 +142,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.7.5 CHANGELOG:
+OWEGA v5.8.0 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -379,8 +379,11 @@
        (added support for all GPT model as of 2024-05-14)
        (added support for all mistral API models as of today)
        (all other models return a cost of 0)
 5.7.4: Added pretty print if the rich module is installed.
 5.7.5: Fixed the bottom toolbar being cut short when terminal
        doesn't have enough columns.
        (also, added gpt-4o and mixtral-8x22b to default list)
+
+5.8.0: Added time-aware mode...
+
 ```
```

### Comparing `owega-5.7.5/README.md` & `owega-5.8.0/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.8.0/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_commands.py` & `owega-5.8.0/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_context.py` & `owega-5.8.0/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.8.0/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_dinput.py` & `owega-5.8.0/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_edit.py` & `owega-5.8.0/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_estimation.py` & `owega-5.8.0/owega/OweHandlers/handle_estimation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Handle /estimation."""
 from ..config import baseConf
 from ..OwegaSession import OwegaSession as ps
 from ..utils import info_print
 
 
-# enables/disables command execution
 def handle_estimation(
     temp_file,
     messages,
     given="",
     temp_is_temp=False,
     silent=False
 ):
```

### Comparing `owega-5.7.5/owega/OweHandlers/handle_finput.py` & `owega-5.8.0/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_frequency.py` & `owega-5.8.0/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_genconf.py` & `owega-5.8.0/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_history.py` & `owega-5.8.0/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_image.py` & `owega-5.8.0/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_load.py` & `owega-5.8.0/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_model.py` & `owega-5.8.0/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_presence.py` & `owega-5.8.0/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_quit.py` & `owega-5.8.0/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_save.py` & `owega-5.8.0/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_system.py` & `owega-5.8.0/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_temperature.py` & `owega-5.8.0/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_tokens.py` & `owega-5.8.0/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_top_p.py` & `owega-5.8.0/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handle_tts.py` & `owega-5.8.0/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OweHandlers/handlers.py` & `owega-5.8.0/owega/OweHandlers/handlers.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .handle_load import item_load
 from .handle_model import item_model
 from .handle_presence import item_presence
 from .handle_quit import item_quit
 from .handle_save import item_save
 from .handle_system import item_system
 from .handle_temperature import item_temperature
+from .handle_time import item_time
 from .handle_tokens import item_tokens
 from .handle_top_p import item_top_p
 from .handle_tts import item_tts
 
 
 # prints help
 def handle_help(temp_file, messages, given="", temp_is_temp=False):
@@ -71,14 +72,15 @@
     items.append(item_presence)
     items.append(item_edit)
     items.append(item_system)
     items.append(item_add_sysmem)
     items.append(item_del_sysmem)
     items.append(item_tts)
     items.append(item_image)
+    items.append(item_time)
 
     for item in items:
         for command in item.get('commands', []):
             handler_helps[command] = item.get('help', '')
             handlers[command] = item.get('fun', void_func)
```

### Comparing `owega-5.7.5/owega/OwegaFun/__init__.py` & `owega-5.8.0/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OwegaFun/functions.py` & `owega-5.8.0/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.8.0/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OwegaFun/utility.py` & `owega-5.8.0/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.8.0/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,28 +70,33 @@
             for e in to_add:
                 self.table.append(e)
 
             self.count += 1
             self.wpos += to_add_count
 
         def newline(self):
-            self.table.append((f"class:blue", '\n'))
+            self.table.append(("class:blue", '\n'))
             self.count = 0
             self.wpos = 0
 
     to_ret = tr()
     to_ret.add(f"v{OwegaChangelog.version}")
     to_ret.add("model", baseConf.get("model", "unknown"))
     to_ret.add(
         "cmds",
         "ON" if baseConf.get("commands") else "OFF",
         "bottom-on" if baseConf.get("commands") else "bottom-off"
     )
     to_ret.add("tokens", baseConf.get("max_tokens", "unknown"))
     to_ret.add(
+        "time",
+        "ON" if baseConf.get("time_awareness") else "OFF",
+        "bottom-on" if baseConf.get("time_awareness") else "bottom-off"
+    )
+    to_ret.add(
         "estm",
         "ON" if baseConf.get("estimation") else "OFF",
         "bottom-on" if baseConf.get("estimation") else "bottom-off"
     )
     to_ret.add(
         "TTS",
         "ON" if baseConf.get("tts_enabled") else "OFF",
```

### Comparing `owega-5.7.5/owega/OwegaSession/promptsession.py` & `owega-5.8.0/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/ask.py` & `owega-5.8.0/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/changelog/changelog.py` & `owega-5.8.0/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,19 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 8, 0)
+            .addLine("Added time-aware mode...")
+        )
+
+        self.logs.append(
             ChangelogEntry(5, 7, 5)
             .addLine("Fixed the bottom toolbar being cut short when terminal")
             .addLine("doesn't have enough columns.")
             .addLine("(also, added gpt-4o and mixtral-8x22b to default list)")
         )
         self.logs.append(
             ChangelogEntry(5, 7, 4)
```

### Comparing `owega-5.7.5/owega/changelog/changelogEntry.py` & `owega-5.8.0/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/changelog/version.py` & `owega-5.8.0/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/conversation/conversation.py` & `owega-5.8.0/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/getLogger.py` & `owega-5.8.0/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/license.py` & `owega-5.8.0/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega/owega.py` & `owega-5.8.0/owega/owega.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,17 @@
                 messages = current_handler(
                     temp_file,
                     messages,
                     given,
                     temp_is_temp
                 )
         if not command_found:
+            if baseConf.get("time_awareness", False):
+                date_str = time.strftime("[%Y-%m-%d %H:%M:%S]")
+                user_input = f"{date_str}\n" + user_input
             if baseConf.get("estimation", False):
                 etkn, cost = estimated_tokens_and_cost(
                     user_input,
                     messages,
                     functionlist_to_toollist(existingFunctions.getEnabled()),
                     baseConf.get('model', ''),
                     baseConf.get("max_tokens", 4096)
```

### Comparing `owega-5.7.5/owega/utils.py` & `owega-5.8.0/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.7.5/owega.egg-info/PKG-INFO` & `owega-5.8.0/owega.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.7.5
+Version: 5.8.0
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -142,15 +142,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.7.5 CHANGELOG:
+OWEGA v5.8.0 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -379,8 +379,11 @@
        (added support for all GPT model as of 2024-05-14)
        (added support for all mistral API models as of today)
        (all other models return a cost of 0)
 5.7.4: Added pretty print if the rich module is installed.
 5.7.5: Fixed the bottom toolbar being cut short when terminal
        doesn't have enough columns.
        (also, added gpt-4o and mixtral-8x22b to default list)
+
+5.8.0: Added time-aware mode...
+
 ```
```

### Comparing `owega-5.7.5/owega.egg-info/SOURCES.txt` & `owega-5.8.0/owega.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 owega/OweHandlers/handle_load.py
 owega/OweHandlers/handle_model.py
 owega/OweHandlers/handle_presence.py
 owega/OweHandlers/handle_quit.py
 owega/OweHandlers/handle_save.py
 owega/OweHandlers/handle_system.py
 owega/OweHandlers/handle_temperature.py
+owega/OweHandlers/handle_time.py
 owega/OweHandlers/handle_tokens.py
 owega/OweHandlers/handle_top_p.py
 owega/OweHandlers/handle_tts.py
 owega/OweHandlers/handlers.py
 owega/OwegaFun/__init__.py
 owega/OwegaFun/functions.py
 owega/OwegaFun/longTermSouvenirs.py
```

### Comparing `owega-5.7.5/setup.py` & `owega-5.8.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """Setup config for installing the package."""
 
 from setuptools import setup
 
-from owega.changelog import OwegaChangelog as oc
-
 desc = open('README.md').read()
 desc += '\n\n'
 desc += "## CHANGELOG: "
 desc += '\n```\n'
-desc += oc.log
+desc += open('CHANGELOG').read()
 desc += '\n```\n'
 
 requirements = [
     'openai>=1.1.1',
     'prompt_toolkit>=3.0',
     'requests>=2.0',
     'beautifulsoup4>=4.0',
@@ -26,15 +24,15 @@
     'python-editor>=1.0',
     'markdownify>=0.11',
     'setuptools>=60.0',
 ]
 
 setup(
     name='owega',
-    version=oc.version_str,
+    version=open('VERSION').read().strip(),
     description="A command-line interface for conversing with GPT models (from OpenAI)",
     long_description=desc,
     long_description_content_type='text/markdown',
     author="darkgeem",
     author_email="darkgeem@pyrokinesis.fr",
     url="https://git.pyrokinesis.fr/darkgeem/owega",
     classifiers=[
```

