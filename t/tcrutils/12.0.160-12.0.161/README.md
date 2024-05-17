# Comparing `tmp/tcrutils-12.0.160.tar.gz` & `tmp/tcrutils-12.0.161.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcrutils-12.0.160.tar", max compression
+gzip compressed data, was "tcrutils-12.0.161.tar", max compression
```

## Comparing `tcrutils-12.0.160.tar` & `tcrutils-12.0.161.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.160/LICENSE
--rw-r--r--   0        0        0      586 2024-05-12 21:58:03.575884 tcrutils-12.0.160/pyproject.toml
--rw-r--r--   0        0        0     1942 2024-05-12 19:30:06.391823 tcrutils-12.0.160/README.md
--rw-r--r--   0        0        0     4756 2024-05-12 21:19:42.809708 tcrutils-12.0.160/tcrutils/__init__.py
--rw-r--r--   0        0        0      209 2024-05-12 21:58:06.111828 tcrutils-12.0.160/tcrutils/_version.py
--rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.160/tcrutils/discord/__init__.py
--rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.160/tcrutils/discord/tcrd_alias.py
--rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.160/tcrutils/discord/tcrd_constants.py
--rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.160/tcrutils/discord/tcrd_embeds.py
--rw-r--r--   0        0        0      378 2024-02-19 21:50:08.127201 tcrutils-12.0.160/tcrutils/discord/tcrd_limits.py
--rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.160/tcrutils/discord/tcrd_permissions.py
--rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.160/tcrutils/discord/tcrd_snowflake.py
--rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.160/tcrutils/discord/tcrd_string.py
--rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.160/tcrutils/discord/tcrd_types.py
--rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.160/tcrutils/dr/__init__.py
--rw-r--r--   0        0        0     8484 2024-05-12 21:53:37.237823 tcrutils-12.0.160/tcrutils/dr/core.py
--rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.160/tcrutils/dr/error.py
--rw-r--r--   0        0        0     2548 2024-05-12 21:22:47.566696 tcrutils-12.0.160/tcrutils/dr/placeholder_sets.py
--rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.160/tcrutils/dr/placeholders/__init__.py
--rw-r--r--   0        0        0     1574 2024-05-11 21:47:23.390141 tcrutils-12.0.160/tcrutils/dr/placeholders/p_discord.py
--rw-r--r--   0        0        0     4389 2024-05-12 19:28:10.182266 tcrutils-12.0.160/tcrutils/dr/placeholders/p_math.py
--rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.160/tcrutils/dr/placeholders/p_text.py
--rw-r--r--   0        0        0     4537 2024-05-12 18:55:58.211193 tcrutils-12.0.160/tcrutils/dr/util.py
--rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.160/tcrutils/imgui/__init__.py
--rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.160/tcrutils/imgui/tcri_dependencies.py
--rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.160/tcrutils/imgui/tcri_handler.py
--rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.160/tcrutils/imgui/types/tcri_types_imgui.py
--rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.160/tcrutils/src/tcr_b64.py
--rw-r--r--   0        0        0     1655 2024-05-02 14:13:55.166736 tcrutils-12.0.160/tcrutils/src/tcr_class.py
--rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.160/tcrutils/src/tcr_classfuncs.py
--rw-r--r--   0        0        0     4092 2024-05-11 21:11:34.733039 tcrutils-12.0.160/tcrutils/src/tcr_cloud_imports.py
--rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.160/tcrutils/src/tcr_compare.py
--rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.160/tcrutils/src/tcr_console.py
--rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.160/tcrutils/src/tcr_constants.py
--rw-r--r--   0        0        0     5892 2024-05-02 12:11:41.388680 tcrutils-12.0.160/tcrutils/src/tcr_decorator.py
--rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.160/tcrutils/src/tcr_dev.py
--rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.160/tcrutils/src/tcr_dict.py
--rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.160/tcrutils/src/tcr_dir.py
--rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.160/tcrutils/src/tcr_error.py
--rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.160/tcrutils/src/tcr_extract_error.py
--rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.160/tcrutils/src/tcr_F.py
--rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.160/tcrutils/src/tcr_getch.py
--rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.160/tcrutils/src/tcr_inject.py
--rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.160/tcrutils/src/tcr_input.py
--rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.160/tcrutils/src/tcr_inspect.py
--rw-r--r--   0        0        0     1080 2024-04-11 22:06:10.025542 tcrutils-12.0.160/tcrutils/src/tcr_int.py
--rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.160/tcrutils/src/tcr_iterable.py
--rw-r--r--   0        0        0     3264 2024-05-11 21:18:41.050978 tcrutils-12.0.160/tcrutils/src/tcr_joke.py
--rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.160/tcrutils/src/tcr_language.py
--rw-r--r--   0        0        0     1155 2024-03-09 23:40:24.608413 tcrutils-12.0.160/tcrutils/src/tcr_markdown.py
--rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.160/tcrutils/src/tcr_misspellings.py
--rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.160/tcrutils/src/tcr_null.py
--rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.160/tcrutils/src/tcr_other.py
--rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.160/tcrutils/src/tcr_overload.py
--rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.160/tcrutils/src/tcr_path.py
--rw-r--r--   0        0        0    29286 2024-04-19 22:20:25.582375 tcrutils-12.0.160/tcrutils/src/tcr_print.py
--rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.160/tcrutils/src/tcr_regex.py
--rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.160/tcrutils/src/tcr_run.py
--rw-r--r--   0        0        0     3888 2024-05-07 16:07:40.280190 tcrutils-12.0.160/tcrutils/src/tcr_sdb.py
--rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.160/tcrutils/src/tcr_string.py
--rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.160/tcrutils/src/tcr_terminal.py
--rw-r--r--   0        0        0     6951 2024-05-12 21:57:51.867345 tcrutils-12.0.160/tcrutils/src/tcr_test.py
--rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.160/tcrutils/src/tcr_timestr.py
--rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.160/tcrutils/src/tcr_types.py
--rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.160/tcrutils/src/tcr_uptime.py
--rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.160/tcrutils/src/tcr_void.py
--rw-r--r--   0        0        0     2557 1970-01-01 00:00:00.000000 tcrutils-12.0.160/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.161/LICENSE
+-rw-r--r--   0        0        0      609 2024-05-13 18:55:20.263766 tcrutils-12.0.161/pyproject.toml
+-rw-r--r--   0        0        0     2276 2024-05-13 14:24:56.384810 tcrutils-12.0.161/README.md
+-rw-r--r--   0        0        0     4756 2024-05-13 13:55:56.501211 tcrutils-12.0.161/tcrutils/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-13 18:55:22.659789 tcrutils-12.0.161/tcrutils/_version.py
+-rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.161/tcrutils/discord/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.161/tcrutils/discord/tcrd_alias.py
+-rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.161/tcrutils/discord/tcrd_constants.py
+-rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.161/tcrutils/discord/tcrd_embeds.py
+-rw-r--r--   0        0        0      378 2024-02-19 21:50:08.127201 tcrutils-12.0.161/tcrutils/discord/tcrd_limits.py
+-rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.161/tcrutils/discord/tcrd_permissions.py
+-rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.161/tcrutils/discord/tcrd_snowflake.py
+-rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.161/tcrutils/discord/tcrd_string.py
+-rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.161/tcrutils/discord/tcrd_types.py
+-rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.161/tcrutils/dr/__init__.py
+-rw-r--r--   0        0        0     9089 2024-05-13 14:29:20.133657 tcrutils-12.0.161/tcrutils/dr/core.py
+-rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.161/tcrutils/dr/error.py
+-rw-r--r--   0        0        0     3542 2024-05-13 14:44:23.672063 tcrutils-12.0.161/tcrutils/dr/placeholder_sets.py
+-rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.161/tcrutils/dr/placeholders/__init__.py
+-rw-r--r--   0        0        0     7389 2024-05-13 14:42:07.865297 tcrutils-12.0.161/tcrutils/dr/placeholders/p_discord.py
+-rw-r--r--   0        0        0     4387 2024-05-13 12:18:40.217769 tcrutils-12.0.161/tcrutils/dr/placeholders/p_math.py
+-rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.161/tcrutils/dr/placeholders/p_text.py
+-rw-r--r--   0        0        0     6167 2024-05-13 14:34:48.145563 tcrutils-12.0.161/tcrutils/dr/util.py
+-rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.161/tcrutils/imgui/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.161/tcrutils/imgui/tcri_dependencies.py
+-rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.161/tcrutils/imgui/tcri_handler.py
+-rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.161/tcrutils/imgui/types/tcri_types_imgui.py
+-rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.161/tcrutils/src/tcr_b64.py
+-rw-r--r--   0        0        0     1655 2024-05-02 14:13:55.166736 tcrutils-12.0.161/tcrutils/src/tcr_class.py
+-rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.161/tcrutils/src/tcr_classfuncs.py
+-rw-r--r--   0        0        0     4370 2024-05-13 18:53:12.432926 tcrutils-12.0.161/tcrutils/src/tcr_cloud_imports.py
+-rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.161/tcrutils/src/tcr_compare.py
+-rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.161/tcrutils/src/tcr_console.py
+-rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.161/tcrutils/src/tcr_constants.py
+-rw-r--r--   0        0        0     5892 2024-05-02 12:11:41.388680 tcrutils-12.0.161/tcrutils/src/tcr_decorator.py
+-rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.161/tcrutils/src/tcr_dev.py
+-rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.161/tcrutils/src/tcr_dict.py
+-rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.161/tcrutils/src/tcr_dir.py
+-rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.161/tcrutils/src/tcr_error.py
+-rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.161/tcrutils/src/tcr_extract_error.py
+-rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.161/tcrutils/src/tcr_F.py
+-rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.161/tcrutils/src/tcr_getch.py
+-rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.161/tcrutils/src/tcr_inject.py
+-rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.161/tcrutils/src/tcr_input.py
+-rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.161/tcrutils/src/tcr_inspect.py
+-rw-r--r--   0        0        0     1080 2024-04-11 22:06:10.025542 tcrutils-12.0.161/tcrutils/src/tcr_int.py
+-rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.161/tcrutils/src/tcr_iterable.py
+-rw-r--r--   0        0        0     3264 2024-05-11 21:18:41.050978 tcrutils-12.0.161/tcrutils/src/tcr_joke.py
+-rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.161/tcrutils/src/tcr_language.py
+-rw-r--r--   0        0        0     1155 2024-03-09 23:40:24.608413 tcrutils-12.0.161/tcrutils/src/tcr_markdown.py
+-rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.161/tcrutils/src/tcr_misspellings.py
+-rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.161/tcrutils/src/tcr_null.py
+-rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.161/tcrutils/src/tcr_other.py
+-rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.161/tcrutils/src/tcr_overload.py
+-rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.161/tcrutils/src/tcr_path.py
+-rw-r--r--   0        0        0    29286 2024-04-19 22:20:25.582375 tcrutils-12.0.161/tcrutils/src/tcr_print.py
+-rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.161/tcrutils/src/tcr_regex.py
+-rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.161/tcrutils/src/tcr_run.py
+-rw-r--r--   0        0        0     3888 2024-05-07 16:07:40.280190 tcrutils-12.0.161/tcrutils/src/tcr_sdb.py
+-rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.161/tcrutils/src/tcr_string.py
+-rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.161/tcrutils/src/tcr_terminal.py
+-rw-r--r--   0        0        0     6977 2024-05-13 11:41:52.760202 tcrutils-12.0.161/tcrutils/src/tcr_test.py
+-rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.161/tcrutils/src/tcr_timestr.py
+-rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.161/tcrutils/src/tcr_types.py
+-rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.161/tcrutils/src/tcr_uptime.py
+-rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.161/tcrutils/src/tcr_void.py
+-rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 tcrutils-12.0.161/PKG-INFO
```

### Comparing `tcrutils-12.0.160/LICENSE` & `tcrutils-12.0.161/LICENSE`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/pyproject.toml` & `tcrutils-12.0.161/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 extend = "C:/CUSTOM_ASSETS/pyproject.toml"
 [tool.ruff.format]
 quote-style = "single"
 indent-style = "space"
 
 [tool.poetry]
 name = "tcrutils"
-version = "12.0.160"
+version = "12.0.161"
 description = "Useful stuff for TCR projects!"
 authors = ["TheCreatorrrr"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11.0,<3.13"
 hikari = "^2.0.0.dev122"
 hikari-toolbox = "^0.1.6"
 hikari-miru = "^4.0.0"
 colored = "^2.2.4"
 colorama = "^0.4.6"
 attr = "^0.3.2"
+hikari-arc = "^1.3.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tcrutils-12.0.160/tcrutils/__init__.py` & `tcrutils-12.0.161/tcrutils/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/discord/__init__.py` & `tcrutils-12.0.161/tcrutils/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/discord/tcrd_embeds.py` & `tcrutils-12.0.161/tcrutils/discord/tcrd_embeds.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/discord/tcrd_permissions.py` & `tcrutils-12.0.161/tcrutils/discord/tcrd_permissions.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/discord/tcrd_snowflake.py` & `tcrutils-12.0.161/tcrutils/discord/tcrd_snowflake.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/discord/tcrd_string.py` & `tcrutils-12.0.161/tcrutils/discord/tcrd_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/discord/tcrd_types.py` & `tcrutils-12.0.161/tcrutils/discord/tcrd_types.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/dr/core.py` & `tcrutils-12.0.161/tcrutils/dr/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections.abc import Callable, Mapping
 from typing import Any
 
+from ..discord.tcrd_types import HikariDictMessage
 from ..src.tcr_console import breakpoint as bp
 from ..src.tcr_dict import merge_dicts
 from ..src.tcr_run import run_sac
 from .error import *
 from .util import _TT, _Token, build_placeholder_rich_return_value
 
 ### Lexer
@@ -151,16 +152,14 @@
     # except BaseException:
     #   ...
     except DynamicResponseError:
       raise
     except RecursionError as e:
       raise DynamicResponseRecursionError(f'{e}') from e
     except TypeError as e:
-      print(str(e))
-      input()
       if 'missing' in str(e) and 'required positional argument' in str(e):
         raise DynamicResponsePlaceholderTooFewArgumentsError(f'Placeholder {placeholder_text_tokens} requires more arguments than were provided.') from e
       raise DynamicResponsePythonErrorInPlaceholerError(f'An error occured within a placeholder {placeholder_text_tokens}.') from e
     except Exception as e:
       raise DynamicResponsePythonErrorInPlaceholerError(f'An error occured within a placeholder {placeholder_text_tokens}.') from e
 
     del tokens[first_open_index : first_close_index + 1]
@@ -174,54 +173,76 @@
 
     processed = await self.process_placeholders(self.tokens[:])
     return ''.join(x.value for x in processed), self.contexts
 
 
 ### Dynamic Response Builder
 
+RESP_CONTEXTS = (
+  'content',
+  'attachments',
+  'components',
+  'embed',
+  'stickers',
+  'tts',
+  'reply',
+  'reply_must_exist',
+  'mentions_everyone',
+  'mentions_reply',
+  'user_mentions',
+  'role_mentions',
+  'flags',
+)
+
 
 class DynamicResponseResult(str):
   contexts: dict[str, Any]
 
   def __new__(cls, string, contexts):
     instance = super().__new__(cls, string)
     instance.contexts = contexts
     return instance
 
+  @property
+  def resp(self) -> HikariDictMessage:
+    return merge_dicts({'content': self}, {x: y for x, y in self.contexts.items() if x in RESP_CONTEXTS})
+
 
 class DynamicResponseBuilder:
   placeholders: dict[str, Callable]
   parens: tuple[str, str]
   splitter: str
-  builtin_contexts: dict[str, Any]
+  instance_contexts: dict[str, Any]
 
   def __init__(
     self,
     *placeholders: dict[str, Callable] | None,
     parens: tuple[str, str] = ('{', '}'),
     splitter: str = '|',
     error_on_missing_placeholder: bool = True,
     error_on_invalid_placeholder_return: bool = True,
-    global_like_contexts: dict[str, Any] | None = None,
+    instance_contexts: dict[str, Any] | None = None,
+    context_constructors: dict[str, Callable[[], Any]] = {},  # noqa: B006
   ) -> None:
     if not all(isinstance(x, dict) for x in placeholders):
       raise TypeError('placeholders must be a dict or list of dicts')
     placeholders = merge_dicts(*placeholders)
 
     self.placeholders = placeholders
     self.parens = parens
     self.splitter = splitter
     self.error_on_missing_placeholder = error_on_missing_placeholder
     self.error_on_invalid_placeholder_return = error_on_invalid_placeholder_return
-    self.builtin_contexts = global_like_contexts or {}
+    self.instance_contexts = instance_contexts or {}
+    self.context_constructors = context_constructors
 
   async def __call__(self, text: str, **contexts: Any) -> DynamicResponseResult:
     tokens = _DRLexer(text, parens=self.parens)()
     parsed, contexts = await _DRParser(
-      contexts={**self.builtin_contexts, **contexts},
+      contexts={**self.instance_contexts, **{x: y() for x, y in self.context_constructors.items()}, **contexts},
       placeholders=self.placeholders,
       splitter=self.splitter,
       tokens=tokens,
       error_on_missing_placeholder=self.error_on_missing_placeholder,
       error_on_invalid_placeholder_return=self.error_on_invalid_placeholder_return,
       parens=self.parens,
     )()
```

### Comparing `tcrutils-12.0.160/tcrutils/dr/error.py` & `tcrutils-12.0.161/tcrutils/dr/error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/dr/placeholder_sets.py` & `tcrutils-12.0.161/tcrutils/dr/placeholder_sets.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,21 +13,52 @@
   '#':       __.comment,
   '//':      __.comment,
   'var':     __.var,
 }
 """Ctrl+click whatever you're hovering on to see aliases for all the text placeholders"""
 
 DISCORD = {
-  'username': __.username,
-  'mention':  __.mention,
-  '@':        __.mention,
-  '@@':       __partial(__.mention, 'noping'),
+  # Author
+  'username':      __.username,
+  'user_name':     __.username,
+  'user name':     __.username,
+  'globalname':    __.globalname,
+  'global_name':   __.globalname,
+  'global name':   __.globalname,
+  'nickname':      __.nickname,
+  'nick_name':     __.nickname,
+  'nick name':     __.nickname,
+  'mention':       __.mention,
+  '@':             __.mention,
+  '@@':  __partial(__.mention, 'noping'),
+  'discriminator': __.discriminator,
+  'discrim':       __.discriminator,
+  'tag':           __.tag,
+  'id':            __.id,
+  'bot':           __.bot,
+  'isbot':         __.bot,
+  'human':         __.human,
+  'ishuman':       __.human,
+  'roles':         __.roles,
+  'avatar':        __.avatar,
+
+  # Misc
+  'indms':         __.in_dms,
+  'in_dms':        __.in_dms,
+  'in dms':        __.in_dms,
 }
 """Ctrl+click whatever you're hovering on to see aliases for all the discord placeholders."""
 
+DISCORD_TROUBLEMAKERS = {
+  'attach':     __.attach,
+  'attachment': __.attach, # May cause a BadRequestError when a technically valid link is supplied but one that doesn't point to any valid file to attach.
+}
+
+ALL_DISCORD = {**DISCORD, **DISCORD_TROUBLEMAKERS}
+
 UNSAFE_MATH = {
   'add':         __.add,
   'subtract':    __.subtract,
   'sub':         __.subtract,
   'multiply':    __.multiply,
   'mul':         __.multiply,
   'divide':      __.divide,
@@ -36,15 +67,15 @@
   'fdiv':        __.floordivide,
   'floordiv':    __.floordivide,
   'power':       __.power,
   'pow':         __.power,
   'modulo':      __.modulo,
   'mod':         __.modulo,
 }
-"""Unsafe math operations are those which may stall the main python thread forever if certain arguments are supplied.
+"""WARNING: Unsafe math operations are those which may stall the main python thread forever if certain arguments are supplied.
 
 I tried searching far and wide for a time-based termination solution but i couldn't find any that worked or worked not only on unix.
 
 Ctrl+click whatever you're hovering on to see aliases for all the unsafe math placeholders.
 """
 
 SAFE_MATH = {
@@ -54,22 +85,22 @@
   'ceiling': __.ceil,
 }
 """Read unsafe math operations doc string to find out what are safe ones.
 
 Ctrl+click whatever you're hovering on to see aliases for all the safe math placeholders.
 """
 
+# fmt: on
+
 SAFE_AND_UNSAFE_MATH = {**UNSAFE_MATH, **SAFE_MATH}
 """WARNING: This contains both UNSAFE and safe sides of the math module. To see more see .UNSAFE_MATH docstring.
 
 Ctrl+click whatever you're hovering on to see aliases for all the math placeholders.
 """
 
-# fmt: on
-
 ALL = merge_dicts(
   *[y for x, y in vars().items() if x.upper() == x and x.lower() != x],
-  {x: y for x, y in vars(__).items() if not x.startswith('_') and not x.startswith('p_')},
+  # {x: y for x, y in vars(__).items() if not x.startswith('_') and not x.startswith('p_')},
 )
-ALL_NON_DISCORD = {x: y for x, y in ALL.items() if x not in DISCORD}
+ALL_NON_DISCORD = {x: y for x, y in ALL.items() if x not in ALL_DISCORD}
 ALL_NON_UNSAFEMATH = {x: y for x, y in ALL.items() if x not in UNSAFE_MATH}
-ALL_NON_UNSAFEMATH_NON_DISCORD = {x: y for x, y in ALL.items() if x not in UNSAFE_MATH and x not in DISCORD}
+ALL_NON_UNSAFEMATH_NON_DISCORD = {x: y for x, y in ALL.items() if x not in UNSAFE_MATH and x not in ALL_DISCORD}
```

### Comparing `tcrutils-12.0.160/tcrutils/dr/placeholders/p_math.py` & `tcrutils-12.0.161/tcrutils/dr/placeholders/p_math.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
   ```txt
   6
   ```
   """
   args = [__.number(x, flatten_to_int_when_possible=True) for x in args]
   return sum(args)
 
+
 @__.STRINGIFY
 @__.REQUIRE_POSITIONAL(1, 0)
 @__.FLATTEN_IF_POSSIBLE
 def subtract(_, *args: str, **ctxs) -> int | float:
   """### Subtract numbers (supports any number of args).
 
   Example:
@@ -117,15 +118,15 @@
 
 @__.STRINGIFY
 @__.REQUIRE_POSITIONAL(1, None)
 @__.FLATTEN_IF_POSSIBLE
 def power(_, base: str, exponent: str = '2', *args: str, **ctxs) -> int | float:
   args = [__.number(x, flatten_to_int_when_possible=True) for x in (base, exponent, *args)]
 
-  return __.functools.reduce(lambda x, y: x ** y, args)
+  return __.functools.reduce(lambda x, y: x**y, args)
 
 
 @__.STRINGIFY
 @__.REQUIRE_POSITIONAL(1, None)
 @__.FLATTEN_IF_POSSIBLE
 def modulo(_, *args: str, **ctxs) -> int | float:
   """### Modulo numbers (supports any number of args).
@@ -210,8 +211,7 @@
   Result:
   ```txt
   10
   10
   ```
   """
   return __.math.ceil(__.number(n))
-
```

### Comparing `tcrutils-12.0.160/tcrutils/dr/placeholders/p_text.py` & `tcrutils-12.0.161/tcrutils/dr/placeholders/p_text.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/dr/util.py` & `tcrutils-12.0.161/tcrutils/dr/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 import functools
 import math
 import typing as t
+
+if t.TYPE_CHECKING:
+  import arc
+import re as regex
 from collections.abc import Callable
 from enum import Enum, auto
 from functools import wraps
 
+import hikari
+
 from ..src.tcr_compare import able
+from ..src.tcr_console import console as c
+from ..src.tcr_regex import RegexPreset
 from ..src.tcr_run import run_sac
 from .error import *
 
 
 class _TT(Enum):
   TEXT = auto()
   PAREN_OPEN = auto()
@@ -62,44 +70,42 @@
       raise DynamicResponsePlaceholderMissingContextError(f'One of {ctxs!r} must be present')
 
     return wrapper
 
   return decorator
 
 
+def REQUIRE_AUTHOR(func):
+  @REQUIRE('event', 'ctx')
+  @wraps(func)
+  async def wrapper(*args, event, ctx, **kwargs):
+    return await run_sac(func, *args, author=(ctx.author if ctx else event.author), event=event, ctx=ctx, **kwargs)
+
+  return wrapper
+
+
 def SWITCH(switch_name: str, *, remove: bool = True):
   """Append a bool context depending on whether or not the passed phrase is in args. Optionally remove it."""
 
   def decorator(func):
     @wraps(func)
     async def wrapper(*args, **kwargs):
       if switch_name in args:
+        if remove:
+          args = tuple(x for x in args if x != switch_name)
         kwargs[switch_name] = True
       else:
         kwargs[switch_name] = False
       return await run_sac(func, *args, **kwargs)
 
     return wrapper
 
   return decorator
 
 
-def rebuild_yourself(*args: str, __parens: tuple[str, str], __splitter: str, **_):
-  """# Rebuild Yourself (RYS).
-
-  Return the placeholder as text, as if it wasnt evaluated at all.
-  For example {dummy} -> returns the str '{dummy}'. Therefore it looks like the placeholder wasnt evaluated.
-
-  This requires at least __parens and __splitter built-in contexts but can take entire **contexts and void others.
-
-  This also supports argumented placeholders for example: {div|1|0} # Division by 0 is invalid so your implementation may be to return the str '{div|1|0}' - although that's not a very good example (it'd be better to return some numeric value for consistency) it's one that ilustrates the point.
-  """
-  return f'{__parens[0]}{(__splitter.join(args))}{__parens[1]}'
-
-
 def DEBUG_CATCH_ERRORS(func):
   @wraps(func)
   async def wrapper(*args, **kwargs):
     try:
       return await run_sac(func, *args, **kwargs)
     except Exception as e:
       print(e)
@@ -125,29 +131,86 @@
 def STRINGIFY(func: Callable):
   @wraps(func)
   async def wrapper(*args, **kwargs):
     return str(await run_sac(func, *args, **kwargs))
 
   return wrapper
 
+
 def FLATTEN_IF_POSSIBLE(func: Callable):
   @wraps(func)
   async def wrapper(*args, **kwargs):
     return flatten_if_possible(await run_sac(func, *args, **kwargs))
 
   return wrapper
 
+
+def REQUIRE_GUILD(default: Callable[..., str] | str = ''):
+  def decorator(func):
+    @REQUIRE('event', 'ctx')
+    @wraps(func)
+    async def wrapper(*args, ctx, event, **kwargs):
+      if ctx:
+        guild = ctx.get_guild()
+      elif hasattr(event, 'get_guild'):
+        guild = event.get_guild()
+      else:
+        guild = None
+
+      if guild is None:
+        return default(func, args, ctx=ctx, event=event, **kwargs) if callable(default) else default
+
+      return await run_sac(func, *args, guild=guild, ctx=ctx, event=event, **kwargs)
+
+    return wrapper
+
+  return decorator
+
+
+def REQUIRE_MEMBER_AUTHOR(default: Callable[..., str] | str = ''):
+  def decorator(func):
+    @REQUIRE_AUTHOR
+    @REQUIRE_GUILD(default)
+    @wraps(func)
+    async def wrapper(*args, guild, author, **kwargs):
+      return await run_sac(func, *args, member=guild.get_member(author), guild=guild, author=author, **kwargs)
+
+    return wrapper
+
+  return decorator
+
+def rebuild_yourself(*args: str, __parens: tuple[str, str], __splitter: str, **_):
+  """# Rebuild Yourself (RYS).
+
+  Return the placeholder as text, as if it wasnt evaluated at all.
+  For example {dummy} -> returns the str '{dummy}'. Therefore it looks like the placeholder wasnt evaluated.
+
+  This requires at least __parens and __splitter built-in contexts but can take entire **contexts and void others.
+
+  This also supports argumented placeholders for example: {div|1|0} # Division by 0 is invalid so your implementation may be to return the str '{div|1|0}' - although that's not a very good example (it'd be better to return some numeric value for consistency) it's one that ilustrates the point.
+  """
+  return f'{__parens[0]}{(__splitter.join(args))}{__parens[1]}'
+
+
 def flatten_if_possible(n: float | int) -> float | int:
-  if n == int(n):
+  if n.is_integer():
     return int(n)
   return n
 
+
 def number(
   s: str,
   *,
   flatten_to_int_when_possible: bool = False,
   default: int | float = 0,
 ) -> float | int:
   if r := able(float, s):
     a = float(r.result)
-    return flatten_if_possible(a)
+    if flatten_to_int_when_possible:
+      return flatten_if_possible(a)
+    else:
+      return a
   return default
+
+
+def jsbool(b: bool) -> str:
+  return 'true' if b else 'false'
```

### Comparing `tcrutils-12.0.160/tcrutils/imgui/tcri_dependencies.py` & `tcrutils-12.0.161/tcrutils/imgui/tcri_dependencies.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/imgui/tcri_handler.py` & `tcrutils-12.0.161/tcrutils/imgui/tcri_handler.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/imgui/types/tcri_types_imgui.py` & `tcrutils-12.0.161/tcrutils/imgui/types/tcri_types_imgui.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_class.py` & `tcrutils-12.0.161/tcrutils/src/tcr_class.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_classfuncs.py` & `tcrutils-12.0.161/tcrutils/src/tcr_classfuncs.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_cloud_imports.py` & `tcrutils-12.0.161/tcrutils/src/tcr_cloud_imports.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 """
 import ast
 import importlib.abc
 import importlib.machinery
 import sys
 import types
 
-import requests
+from ..src.tcr_console import console as c
 
 
 def is_valid_python_source(code: str) -> bool:
   try:
     ast.parse(code)
   except SyntaxError:
     return False
@@ -84,14 +84,20 @@
       loader,
       origin=url,
       is_package=True,
     )
 
   def _get_remote_python_source(self, url):
     try:
+      import requests
+    except ImportError:
+      c.error('You need to install requests to use tcr.cloud_imports: pip install requests')
+      c.error('I am not adding this as dependency because this is a joke module...')
+      raise
+    try:
       response = requests.get(url)
       response.raise_for_status()
     except requests.HTTPError:
       return None
 
     source = response.text
```

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_compare.py` & `tcrutils-12.0.161/tcrutils/src/tcr_compare.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_console.py` & `tcrutils-12.0.161/tcrutils/src/tcr_console.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_decorator.py` & `tcrutils-12.0.161/tcrutils/src/tcr_decorator.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_dev.py` & `tcrutils-12.0.161/tcrutils/src/tcr_dev.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_dict.py` & `tcrutils-12.0.161/tcrutils/src/tcr_dict.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_error.py` & `tcrutils-12.0.161/tcrutils/src/tcr_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_extract_error.py` & `tcrutils-12.0.161/tcrutils/src/tcr_extract_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_getch.py` & `tcrutils-12.0.161/tcrutils/src/tcr_getch.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_inject.py` & `tcrutils-12.0.161/tcrutils/src/tcr_inject.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_input.py` & `tcrutils-12.0.161/tcrutils/src/tcr_input.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_inspect.py` & `tcrutils-12.0.161/tcrutils/src/tcr_inspect.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_int.py` & `tcrutils-12.0.161/tcrutils/src/tcr_int.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_iterable.py` & `tcrutils-12.0.161/tcrutils/src/tcr_iterable.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_joke.py` & `tcrutils-12.0.161/tcrutils/src/tcr_joke.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_language.py` & `tcrutils-12.0.161/tcrutils/src/tcr_language.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_markdown.py` & `tcrutils-12.0.161/tcrutils/src/tcr_markdown.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_misspellings.py` & `tcrutils-12.0.161/tcrutils/src/tcr_misspellings.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_null.py` & `tcrutils-12.0.161/tcrutils/src/tcr_null.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_overload.py` & `tcrutils-12.0.161/tcrutils/src/tcr_overload.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_path.py` & `tcrutils-12.0.161/tcrutils/src/tcr_path.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_print.py` & `tcrutils-12.0.161/tcrutils/src/tcr_print.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_regex.py` & `tcrutils-12.0.161/tcrutils/src/tcr_regex.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_run.py` & `tcrutils-12.0.161/tcrutils/src/tcr_run.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_sdb.py` & `tcrutils-12.0.161/tcrutils/src/tcr_sdb.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_string.py` & `tcrutils-12.0.161/tcrutils/src/tcr_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_terminal.py` & `tcrutils-12.0.161/tcrutils/src/tcr_terminal.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_test.py` & `tcrutils-12.0.161/tcrutils/src/tcr_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,20 @@
     obj,
     padding=f" {(ASSERTION_ASS if randint(1, 1000) != 69 else ASSERTION_ASS.replace('PASS', ' ASS')) if result else ASSERTION_FAIL} ",
     printhook=lambda x, **kwargs: print(x + comment, **kwargs),
   )
 
 
 def total_default_printhook(s: str, failures: int, total: int, *args, **kwargs):
-  console(f'{s}{" " if total else f"{Fore.RED}{Style.bold}< no tests registered > "}{Fore.RED if failures else Fore.GREEN}{Style.bold}{failures}{FMTC.DECIMAL}/{FMTC.NUMBER}{total}{FMTC._}', *args, fmt_iterable=lambda a, *_, **__: str(a), **kwargs)
+  console(
+    f'{s}{" " if total else f"{Fore.RED}{Style.bold}< no tests registered > "}{Fore.RED if failures else Fore.GREEN}{Style.bold}{failures}{FMTC.DECIMAL}/{FMTC.NUMBER}{total}{FMTC._}',
+    *args,
+    fmt_iterable=lambda a, *_, **__: str(a),
+    **kwargs,
+  )
 
 
 @dataclass
 class _TestResult:
   result: bool
```

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_timestr.py` & `tcrutils-12.0.161/tcrutils/src/tcr_timestr.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_uptime.py` & `tcrutils-12.0.161/tcrutils/src/tcr_uptime.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/tcrutils/src/tcr_void.py` & `tcrutils-12.0.161/tcrutils/src/tcr_void.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.160/PKG-INFO` & `tcrutils-12.0.161/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tcrutils
-Version: 12.0.160
+Version: 12.0.161
 Summary: Useful stuff for TCR projects!
 License: GPL-3.0
 Author: TheCreatorrrr
 Requires-Python: >=3.11.0,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: attr (>=0.3.2,<0.4.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: colored (>=2.2.4,<3.0.0)
 Requires-Dist: hikari (>=2.0.0.dev122,<3.0.0)
+Requires-Dist: hikari-arc (>=1.3.0,<2.0.0)
 Requires-Dist: hikari-miru (>=4.0.0,<5.0.0)
 Requires-Dist: hikari-toolbox (>=0.1.6,<0.2.0)
 Description-Content-Type: text/markdown
 
 # TCRUtils
 
 Useful stuff for tcr projects.
@@ -26,16 +27,29 @@
     - [ ] add docstrings
   - [ ] finish execute
     - [ ] remove old execute
     - [ ] add docstrings
     - [ ] Placeholders
       - [ ] How to make your own placeholders template
       - Discord
-        - [ ] mention / @ / @@
-        - [ ] username
+        - Author
+          - [x] mention / @ / @@
+          - [x] username
+          - [x] global name
+          - [x] nickname
+          - [x] discrim
+          - [x] tag
+          - [x] id
+          - [x] isbot
+          - [x] ishuman
+          - [x] indms
+          - [x] avatar
+          - [x] roles
+          - [ ] color
+        - [ ] attach (convert url to attachment)
       - Text
         - [ ] args
         - [x] var
         - [ ] Args
         - [ ] Variable with Arguments
         - [ ] Prefix
         - [ ] Alias
```

#### html2text {}

```diff
@@ -1,26 +1,29 @@
-Metadata-Version: 2.1 Name: tcrutils Version: 12.0.160 Summary: Useful stuff
+Metadata-Version: 2.1 Name: tcrutils Version: 12.0.161 Summary: Useful stuff
 for TCR projects! License: GPL-3.0 Author: TheCreatorrrr Requires-Python:
 >=3.11.0,<3.13 Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: attr (>=0.3.2,<0.4.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: colored (>=2.2.4,<3.0.0) Requires-Dist: hikari
-(>=2.0.0.dev122,<3.0.0) Requires-Dist: hikari-miru (>=4.0.0,<5.0.0) Requires-
-Dist: hikari-toolbox (>=0.1.6,<0.2.0) Description-Content-Type: text/markdown #
-TCRUtils Useful stuff for tcr projects. ## Todo - [ ] finish imgui - [ ] add
-docstrings - [ ] finish execute - [ ] remove old execute - [ ] add docstrings -
-[ ] Placeholders - [ ] How to make your own placeholders template - Discord -
-[ ] mention / @ / @@ - [ ] username - Text - [ ] args - [x] var - [ ] Args -
-[ ] Variable with Arguments - [ ] Prefix - [ ] Alias - [ ] Test - [ ] Switch -
-[ ] Length - [ ] Lower - [ ] Upper - [ ] Capitalize - [ ] Apostrophe - [ ]
-Unmark - [ ] Reverse - [ ] Repeat - [ ] Limit - [ ] Slice - [ ] Split - [ ]
-Contains - [ ] URL - [ ] Spoiler - [ ] Replace - [ ] Regex - [ ] Regex Replace
-- [ ] Trim - [ ] Hex Color - [ ] Char - [ ] Char Code - [ ] Newline - [ ]
-comment - Math - [ ] RNG - [x] Add - [x] Subtract - [x] Multiply - [x] Divide -
-[x] Power - [x] Modulo - [x] Round - [x] Floor - [x] Ceil - [ ] Fixed - [ ]
-Precise - [ ] Highest - [ ] Lowest - [ ] Absolute - [ ] Clamp - [ ] Commafy -
-[ ] Nth - [ ] Bit - [ ] BBit - [ ] Base ~~
+(>=2.0.0.dev122,<3.0.0) Requires-Dist: hikari-arc (>=1.3.0,<2.0.0) Requires-
+Dist: hikari-miru (>=4.0.0,<5.0.0) Requires-Dist: hikari-toolbox
+(>=0.1.6,<0.2.0) Description-Content-Type: text/markdown # TCRUtils Useful
+stuff for tcr projects. ## Todo - [ ] finish imgui - [ ] add docstrings - [ ]
+finish execute - [ ] remove old execute - [ ] add docstrings - [ ] Placeholders
+- [ ] How to make your own placeholders template - Discord - Author - [x]
+mention / @ / @@ - [x] username - [x] global name - [x] nickname - [x] discrim
+- [x] tag - [x] id - [x] isbot - [x] ishuman - [x] indms - [x] avatar - [x]
+roles - [ ] color - [ ] attach (convert url to attachment) - Text - [ ] args -
+[x] var - [ ] Args - [ ] Variable with Arguments - [ ] Prefix - [ ] Alias - [ ]
+Test - [ ] Switch - [ ] Length - [ ] Lower - [ ] Upper - [ ] Capitalize - [ ]
+Apostrophe - [ ] Unmark - [ ] Reverse - [ ] Repeat - [ ] Limit - [ ] Slice -
+[ ] Split - [ ] Contains - [ ] URL - [ ] Spoiler - [ ] Replace - [ ] Regex -
+[ ] Regex Replace - [ ] Trim - [ ] Hex Color - [ ] Char - [ ] Char Code - [ ]
+Newline - [ ] comment - Math - [ ] RNG - [x] Add - [x] Subtract - [x] Multiply
+- [x] Divide - [x] Power - [x] Modulo - [x] Round - [x] Floor - [x] Ceil - [ ]
+Fixed - [ ] Precise - [ ] Highest - [ ] Lowest - [ ] Absolute - [ ] Clamp - [ ]
+Commafy - [ ] Nth - [ ] Bit - [ ] BBit - [ ] Base ~~
 ~~ ~~
 ~~ ~~
 ~~ ~~
 ~~
```

