# Comparing `tmp/rc3-0.0.5.tar.gz` & `tmp/rc3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rc3-0.0.5.tar", last modified: Wed May 15 20:05:03 2024, max compression
+gzip compressed data, was "rc3-0.0.6.tar", last modified: Fri May 17 16:45:44 2024, max compression
```

## Comparing `rc3-0.0.5.tar` & `rc3-0.0.6.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.944085 rc3-0.0.5/
--rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.5/.gitignore
--rw-rw-rw-   0        0        0     1087 2024-05-06 20:36:33.000000 rc3-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    11488 2024-05-15 20:05:03.942087 rc3-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     9437 2024-05-15 20:01:38.000000 rc3-0.0.5/README.md
--rw-rw-rw-   0        0        0     1044 2024-05-07 23:16:04.000000 rc3-0.0.5/WINDOWS_SETUP.md
--rw-rw-rw-   0        0        0      823 2024-05-15 20:04:21.000000 rc3-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.5/rc3.iml
--rw-rw-rw-   0        0        0       42 2024-05-15 20:05:03.945086 rc3-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.749005 rc3-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.772041 rc3-0.0.5/src/rc3/
--rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.793028 rc3-0.0.5/src/rc3/archive/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/archive/__init__.py
--rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/archive/cmd_home.py
--rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/archive/cmd_root.py
--rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/archive/cmd_subs.py
--rw-rw-rw-   0        0        0     1924 2024-05-07 23:36:03.000000 rc3-0.0.5/src/rc3/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.815156 rc3-0.0.5/src/rc3/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/commands/__init__.py
--rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.5/src/rc3/commands/cmd_collection.py
--rw-rw-rw-   0        0        0     5467 2024-05-07 23:33:42.000000 rc3-0.0.5/src/rc3/commands/cmd_environment.py
--rw-rw-rw-   0        0        0     1454 2024-05-07 23:35:00.000000 rc3-0.0.5/src/rc3/commands/cmd_global.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:38.000000 rc3-0.0.5/src/rc3/commands/cmd_hello.py
--rw-rw-rw-   0        0        0     3414 2024-05-15 20:01:43.000000 rc3-0.0.5/src/rc3/commands/cmd_init.py
--rw-rw-rw-   0        0        0     2136 2024-05-08 19:24:17.000000 rc3-0.0.5/src/rc3/commands/cmd_list.py
--rw-rw-rw-   0        0        0     4322 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/commands/cmd_request.py
--rw-rw-rw-   0        0        0     9478 2024-05-08 18:59:18.000000 rc3-0.0.5/src/rc3/commands/cmd_send.py
--rw-rw-rw-   0        0        0     1368 2024-05-08 18:10:08.000000 rc3-0.0.5/src/rc3/commands/cmd_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.828203 rc3-0.0.5/src/rc3/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/__init__.py
--rw-rw-rw-   0        0        0      524 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/config_helper.py
--rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.5/src/rc3/common/data_helper.py
--rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/decorators.py
--rw-rw-rw-   0        0        0     2670 2024-05-06 20:00:31.000000 rc3-0.0.5/src/rc3/common/env_helper.py
--rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.5/src/rc3/common/inherit_helper.py
--rw-rw-rw-   0        0        0    10723 2024-05-08 18:47:05.000000 rc3-0.0.5/src/rc3/common/json_helper.py
--rw-rw-rw-   0        0        0     2503 2024-05-08 19:08:29.000000 rc3-0.0.5/src/rc3/common/print_helper.py
--rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/common/rc_globals.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.829202 rc3-0.0.5/src/rc3/data/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/src/rc3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.830201 rc3-0.0.5/src/rc3/data/collection/
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.834936 rc3-0.0.5/src/rc3/data/collection/environments/
--rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.5/src/rc3/data/collection/environments/.gitignore
--rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/environments/dev.defaults
--rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/environments/localhost.defaults
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.850927 rc3-0.0.5/src/rc3/data/collection/examples/
--rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.858548 rc3-0.0.5/src/rc3/data/collection/greetings-basic/
--rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-basic/update-greeting.request
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.861546 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.5/src/rc3/data/collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.864543 rc3-0.0.5/src/rc3/data/home/
--rw-rw-rw-   0        0        0      130 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/rc-global.json
--rw-rw-rw-   0        0        0      354 2024-05-07 23:02:39.000000 rc3-0.0.5/src/rc3/data/home/rc-settings.json
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.873014 rc3-0.0.5/src/rc3/data/home/schemas/
--rw-rw-rw-   0        0        0     1151 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
--rw-rw-rw-   0        0        0      918 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
--rw-rw-rw-   0        0        0      473 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
--rw-rw-rw-   0        0        0      605 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
--rw-rw-rw-   0        0        0     3241 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-request-0.0.3.json
--rw-rw-rw-   0        0        0     2259 2024-05-07 23:02:08.000000 rc3-0.0.5/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.939088 rc3-0.0.5/src/rc3.egg-info/
--rw-rw-rw-   0        0        0    11488 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5186 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      100 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-15 20:05:03.000000 rc3-0.0.5/src/rc3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.874013 rc3-0.0.5/temp-collection/
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.878014 rc3-0.0.5/temp-collection/environments/
--rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.5/temp-collection/environments/.gitignore
--rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/environments/dev.defaults
--rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/environments/localhost.defaults
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.893486 rc3-0.0.5/temp-collection/examples/
--rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Auth_Basic.request
--rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Auth_Bearer.request
--rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Auth_Token.request
--rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Extract_JsonPath.request
--rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_Extract_Regex.request
--rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_GET.request
--rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_KitchenSink.request
--rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_MintOauth2Token.request
--rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_POST_json.request
--rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_POST_text-plain.request
--rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_QueryParams.request
--rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/example_UseOauth2Token.request
--rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/examples/folder.json
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.900482 rc3-0.0.5/temp-collection/greetings-basic/
--rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/greeting.request
--rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/greetings.request
--rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/new-greeting.request
--rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/rc-folder.json
--rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/remove-greeting.request
--rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-basic/update-greeting.request
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.904479 rc3-0.0.5/temp-collection/greetings-oauth2/
--rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-oauth2/greeting.request
--rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-oauth2/mint-admin-token.request
--rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.5/temp-collection/greetings-oauth2/mint-token.request
--rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.5/temp-collection/rc-collection.json
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.907480 rc3-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.918470 rc3-0.0.5/tests/commands/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/__init__.py
--rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_collection.py
--rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_environment.py
--rw-rw-rw-   0        0        0     1856 2024-05-08 19:17:23.000000 rc3-0.0.5/tests/commands/test_init.py
--rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_list.py
--rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_request.py
--rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/commands/test_send.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.930460 rc3-0.0.5/tests/commands/test_send_files/
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_is_verbose.yaml
--rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_mint_extract_use_token.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_not_verbose.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_request_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_send_1.yaml
--rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_send_2.yaml
--rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_send_basics.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_settings_no_responses.yaml
--rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/commands/test_send_files/test_settings_with_responses.yaml
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.932972 rc3-0.0.5/tests/common/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/common/__init__.py
--rw-rw-rw-   0        0        0     5211 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/common/test_env_helper.py
--rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.5/tests/common/test_inherit_helper.py
--rw-rw-rw-   0        0        0     1124 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.935091 rc3-0.0.5/tests/learning/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/learning/__init__.py
--rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/learning/test_sample.py
--rw-rw-rw-   0        0        0     1665 2024-05-06 20:00:31.000000 rc3-0.0.5/tests/test_cli.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:05:03.937090 rc3-0.0.5/tests/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/util/__init__.py
--rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.5/tests/util/decorators.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.238582 rc3-0.0.6/
+-rw-rw-rw-   0        0        0     3141 2024-05-06 19:59:38.000000 rc3-0.0.6/.gitignore
+-rw-rw-rw-   0        0        0     1087 2024-05-06 20:36:33.000000 rc3-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    11541 2024-05-17 16:45:44.237582 rc3-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9437 2024-05-15 20:01:38.000000 rc3-0.0.6/README.md
+-rw-rw-rw-   0        0        0     1044 2024-05-07 23:16:04.000000 rc3-0.0.6/WINDOWS_SETUP.md
+-rw-rw-rw-   0        0        0      828 2024-05-17 16:41:36.000000 rc3-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      475 2024-05-06 20:07:47.000000 rc3-0.0.6/rc3.iml
+-rw-rw-rw-   0        0        0       97 2024-05-17 16:45:44.239582 rc3-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.054067 rc3-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.078325 rc3-0.0.6/src/rc3/
+-rw-rw-rw-   0        0        0      246 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.091677 rc3-0.0.6/src/rc3/archive/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/archive/__init__.py
+-rw-rw-rw-   0        0        0      406 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/archive/cmd_home.py
+-rw-rw-rw-   0        0        0      637 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/archive/cmd_root.py
+-rw-rw-rw-   0        0        0     1125 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/archive/cmd_subs.py
+-rw-rw-rw-   0        0        0     1924 2024-05-07 23:36:03.000000 rc3-0.0.6/src/rc3/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.106666 rc3-0.0.6/src/rc3/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/commands/__init__.py
+-rw-rw-rw-   0        0        0     3415 2024-05-06 22:52:43.000000 rc3-0.0.6/src/rc3/commands/cmd_collection.py
+-rw-rw-rw-   0        0        0     5467 2024-05-07 23:33:42.000000 rc3-0.0.6/src/rc3/commands/cmd_environment.py
+-rw-rw-rw-   0        0        0     1454 2024-05-07 23:35:00.000000 rc3-0.0.6/src/rc3/commands/cmd_global.py
+-rw-rw-rw-   0        0        0      524 2024-05-06 19:59:38.000000 rc3-0.0.6/src/rc3/commands/cmd_hello.py
+-rw-rw-rw-   0        0        0     3414 2024-05-15 20:01:43.000000 rc3-0.0.6/src/rc3/commands/cmd_init.py
+-rw-rw-rw-   0        0        0     2136 2024-05-08 19:24:17.000000 rc3-0.0.6/src/rc3/commands/cmd_list.py
+-rw-rw-rw-   0        0        0     4322 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/commands/cmd_request.py
+-rw-rw-rw-   0        0        0     9478 2024-05-08 18:59:18.000000 rc3-0.0.6/src/rc3/commands/cmd_send.py
+-rw-rw-rw-   0        0        0     1368 2024-05-08 18:10:08.000000 rc3-0.0.6/src/rc3/commands/cmd_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.118656 rc3-0.0.6/src/rc3/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/__init__.py
+-rw-rw-rw-   0        0        0      524 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/config_helper.py
+-rw-rw-rw-   0        0        0      869 2024-05-06 22:59:13.000000 rc3-0.0.6/src/rc3/common/data_helper.py
+-rw-rw-rw-   0        0        0      936 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/decorators.py
+-rw-rw-rw-   0        0        0     2670 2024-05-06 20:00:31.000000 rc3-0.0.6/src/rc3/common/env_helper.py
+-rw-rw-rw-   0        0        0     1364 2024-05-06 22:52:57.000000 rc3-0.0.6/src/rc3/common/inherit_helper.py
+-rw-rw-rw-   0        0        0    10723 2024-05-08 18:47:05.000000 rc3-0.0.6/src/rc3/common/json_helper.py
+-rw-rw-rw-   0        0        0     2503 2024-05-08 19:08:29.000000 rc3-0.0.6/src/rc3/common/print_helper.py
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/common/rc_globals.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.119655 rc3-0.0.6/src/rc3/data/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/src/rc3/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.120655 rc3-0.0.6/src/rc3/data/collection/
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.126651 rc3-0.0.6/src/rc3/data/collection/environments/
+-rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.6/src/rc3/data/collection/environments/.gitignore
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/environments/dev.defaults
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/environments/localhost.defaults
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.143640 rc3-0.0.6/src/rc3/data/collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.150636 rc3-0.0.6/src/rc3/data/collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.154635 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.6/src/rc3/data/collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.158631 rc3-0.0.6/src/rc3/data/home/
+-rw-rw-rw-   0        0        0      130 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/rc-global.json
+-rw-rw-rw-   0        0        0      354 2024-05-07 23:02:39.000000 rc3-0.0.6/src/rc3/data/home/rc-settings.json
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.166626 rc3-0.0.6/src/rc3/data/home/schemas/
+-rw-rw-rw-   0        0        0     1151 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-auth-0.0.3.json
+-rw-rw-rw-   0        0        0      918 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-collection-0.0.3.json
+-rw-rw-rw-   0        0        0      473 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-environment-0.0.3.json
+-rw-rw-rw-   0        0        0      605 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-folder-0.0.3.json
+-rw-rw-rw-   0        0        0     3241 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-request-0.0.3.json
+-rw-rw-rw-   0        0        0     2259 2024-05-07 23:02:08.000000 rc3-0.0.6/src/rc3/data/home/schemas/rc3-settings-0.0.3.json
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.235592 rc3-0.0.6/src/rc3.egg-info/
+-rw-rw-rw-   0        0        0    11541 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5196 2024-05-17 16:45:44.000000 rc3-0.0.6/src/rc3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      100 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-17 16:45:43.000000 rc3-0.0.6/src/rc3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.167629 rc3-0.0.6/temp-collection/
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.172622 rc3-0.0.6/temp-collection/environments/
+-rw-rw-rw-   0        0        0        6 2024-05-15 19:30:06.000000 rc3-0.0.6/temp-collection/environments/.gitignore
+-rw-rw-rw-   0        0        0      277 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/environments/dev.defaults
+-rw-rw-rw-   0        0        0      307 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/environments/localhost.defaults
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.189612 rc3-0.0.6/temp-collection/examples/
+-rw-rw-rw-   0        0        0      247 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Auth_Basic.request
+-rw-rw-rw-   0        0        0      914 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Auth_Bearer.request
+-rw-rw-rw-   0        0        0      960 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Auth_Token.request
+-rw-rw-rw-   0        0        0      436 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Extract_JsonPath.request
+-rw-rw-rw-   0        0        0      455 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_Extract_Regex.request
+-rw-rw-rw-   0        0        0      190 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_GET.request
+-rw-rw-rw-   0        0        0      799 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_KitchenSink.request
+-rw-rw-rw-   0        0        0      401 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_MintOauth2Token.request
+-rw-rw-rw-   0        0        0      275 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_POST_json.request
+-rw-rw-rw-   0        0        0      231 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_POST_text-plain.request
+-rw-rw-rw-   0        0        0      240 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_QueryParams.request
+-rw-rw-rw-   0        0        0      227 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/example_UseOauth2Token.request
+-rw-rw-rw-   0        0        0      272 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/examples/folder.json
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.197607 rc3-0.0.6/temp-collection/greetings-basic/
+-rw-rw-rw-   0        0        0      384 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/greeting.request
+-rw-rw-rw-   0        0        0      180 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/greetings.request
+-rw-rw-rw-   0        0        0      291 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/new-greeting.request
+-rw-rw-rw-   0        0        0      297 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/rc-folder.json
+-rw-rw-rw-   0        0        0      185 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/remove-greeting.request
+-rw-rw-rw-   0        0        0      313 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-basic/update-greeting.request
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.200605 rc3-0.0.6/temp-collection/greetings-oauth2/
+-rw-rw-rw-   0        0        0      218 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-oauth2/greeting.request
+-rw-rw-rw-   0        0        0      466 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-oauth2/mint-admin-token.request
+-rw-rw-rw-   0        0        0      465 2024-05-07 23:02:08.000000 rc3-0.0.6/temp-collection/greetings-oauth2/mint-token.request
+-rw-rw-rw-   0        0        0      247 2024-05-08 14:58:01.000000 rc3-0.0.6/temp-collection/rc-collection.json
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.204602 rc3-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.213596 rc3-0.0.6/tests/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/__init__.py
+-rw-rw-rw-   0        0        0      599 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_collection.py
+-rw-rw-rw-   0        0        0     5698 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_environment.py
+-rw-rw-rw-   0        0        0     1856 2024-05-08 19:17:23.000000 rc3-0.0.6/tests/commands/test_init.py
+-rw-rw-rw-   0        0        0      427 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_list.py
+-rw-rw-rw-   0        0        0     5923 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_request.py
+-rw-rw-rw-   0        0        0     6322 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/commands/test_send.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.226590 rc3-0.0.6/tests/commands/test_send_files/
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_is_verbose.yaml
+-rw-rw-rw-   0        0        0     1178 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_mint_extract_use_token.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_not_verbose.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_request_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_send_1.yaml
+-rw-rw-rw-   0        0        0      663 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_send_2.yaml
+-rw-rw-rw-   0        0        0     1098 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_send_basics.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_settings_no_responses.yaml
+-rw-rw-rw-   0        0        0      263 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/commands/test_send_files/test_settings_with_responses.yaml
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.230587 rc3-0.0.6/tests/common/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/common/__init__.py
+-rw-rw-rw-   0        0        0     5211 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/common/test_env_helper.py
+-rw-rw-rw-   0        0        0     3345 2024-05-06 22:51:48.000000 rc3-0.0.6/tests/common/test_inherit_helper.py
+-rw-rw-rw-   0        0        0     1124 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.232586 rc3-0.0.6/tests/learning/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/learning/__init__.py
+-rw-rw-rw-   0        0        0      518 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/learning/test_sample.py
+-rw-rw-rw-   0        0        0     1665 2024-05-06 20:00:31.000000 rc3-0.0.6/tests/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-05-17 16:45:44.234585 rc3-0.0.6/tests/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/util/__init__.py
+-rw-rw-rw-   0        0        0     1407 2024-05-06 19:59:39.000000 rc3-0.0.6/tests/util/decorators.py
```

### Comparing `rc3-0.0.5/.gitignore` & `rc3-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/LICENSE` & `rc3-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/PKG-INFO` & `rc3-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: rc3
-Version: 0.0.5
+Version: 0.0.6
 Summary: Rest CLI (rc)
-Author-email: Gary Wilcox <gary@dugan-wilcox.com>
+Home-page: https://github.com/gswilcox01/rc3
+Author: Gary Wilcox
+Author-email: gary@dugan-wilcox.com
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `rc3-0.0.5/README.md` & `rc3-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/WINDOWS_SETUP.md` & `rc3-0.0.6/WINDOWS_SETUP.md`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/pyproject.toml` & `rc3-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0","setuptools-scm","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rc3"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
-  { name="Gary Wilcox", email="gary@dugan-wilcox.com" },
+  { name="Gary Wilcox" },
+  { email="gary@dugan-wilcox.com" }
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 description = "Rest CLI (rc)"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `rc3-0.0.5/src/rc3/archive/cmd_root.py` & `rc3-0.0.6/src/rc3/archive/cmd_root.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/archive/cmd_subs.py` & `rc3-0.0.6/src/rc3/archive/cmd_subs.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/cli.py` & `rc3-0.0.6/src/rc3/cli.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_collection.py` & `rc3-0.0.6/src/rc3/commands/cmd_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_environment.py` & `rc3-0.0.6/src/rc3/commands/cmd_environment.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_global.py` & `rc3-0.0.6/src/rc3/commands/cmd_global.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_hello.py` & `rc3-0.0.6/src/rc3/commands/cmd_hello.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_init.py` & `rc3-0.0.6/src/rc3/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_list.py` & `rc3-0.0.6/src/rc3/commands/cmd_list.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_request.py` & `rc3-0.0.6/src/rc3/commands/cmd_request.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_send.py` & `rc3-0.0.6/src/rc3/commands/cmd_send.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/commands/cmd_settings.py` & `rc3-0.0.6/src/rc3/commands/cmd_settings.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/common/config_helper.py` & `rc3-0.0.6/src/rc3/common/config_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/common/data_helper.py` & `rc3-0.0.6/src/rc3/common/data_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/common/decorators.py` & `rc3-0.0.6/src/rc3/common/decorators.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/common/env_helper.py` & `rc3-0.0.6/src/rc3/common/env_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/common/inherit_helper.py` & `rc3-0.0.6/src/rc3/common/inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/common/json_helper.py` & `rc3-0.0.6/src/rc3/common/json_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/common/print_helper.py` & `rc3-0.0.6/src/rc3/common/print_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Bearer.request` & `rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Bearer.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/collection/examples/example_Auth_Token.request` & `rc3-0.0.6/src/rc3/data/collection/examples/example_Auth_Token.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/collection/examples/example_KitchenSink.request` & `rc3-0.0.6/src/rc3/data/collection/examples/example_KitchenSink.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/home/schemas/rc3-auth-0.0.3.json` & `rc3-0.0.6/src/rc3/data/home/schemas/rc3-auth-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/home/schemas/rc3-collection-0.0.3.json` & `rc3-0.0.6/src/rc3/data/home/schemas/rc3-collection-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/home/schemas/rc3-folder-0.0.3.json` & `rc3-0.0.6/src/rc3/data/home/schemas/rc3-folder-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/home/schemas/rc3-request-0.0.3.json` & `rc3-0.0.6/src/rc3/data/home/schemas/rc3-request-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3/data/home/schemas/rc3-settings-0.0.3.json` & `rc3-0.0.6/src/rc3/data/home/schemas/rc3-settings-0.0.3.json`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/src/rc3.egg-info/PKG-INFO` & `rc3-0.0.6/src/rc3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: rc3
-Version: 0.0.5
+Version: 0.0.6
 Summary: Rest CLI (rc)
-Author-email: Gary Wilcox <gary@dugan-wilcox.com>
+Home-page: https://github.com/gswilcox01/rc3
+Author: Gary Wilcox
+Author-email: gary@dugan-wilcox.com
 License: MIT License
         
         Copyright (c) 2018 Real Python
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `rc3-0.0.5/src/rc3.egg-info/SOURCES.txt` & `rc3-0.0.6/src/rc3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 LICENSE
 README.md
 WINDOWS_SETUP.md
 pyproject.toml
 rc3.iml
+setup.cfg
 src/rc3/__init__.py
 src/rc3/cli.py
 src/rc3.egg-info/PKG-INFO
 src/rc3.egg-info/SOURCES.txt
 src/rc3.egg-info/dependency_links.txt
 src/rc3.egg-info/entry_points.txt
 src/rc3.egg-info/requires.txt
```

### Comparing `rc3-0.0.5/temp-collection/examples/example_Auth_Bearer.request` & `rc3-0.0.6/temp-collection/examples/example_Auth_Bearer.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/temp-collection/examples/example_Auth_Token.request` & `rc3-0.0.6/temp-collection/examples/example_Auth_Token.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/temp-collection/examples/example_KitchenSink.request` & `rc3-0.0.6/temp-collection/examples/example_KitchenSink.request`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_collection.py` & `rc3-0.0.6/tests/commands/test_collection.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_environment.py` & `rc3-0.0.6/tests/commands/test_environment.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_init.py` & `rc3-0.0.6/tests/commands/test_init.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_request.py` & `rc3-0.0.6/tests/commands/test_request.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_send.py` & `rc3-0.0.6/tests/commands/test_send.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_send_files/test_mint_extract_use_token.yaml` & `rc3-0.0.6/tests/commands/test_send_files/test_mint_extract_use_token.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_send_files/test_send_2.yaml` & `rc3-0.0.6/tests/commands/test_send_files/test_send_2.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/commands/test_send_files/test_send_basics.yaml` & `rc3-0.0.6/tests/commands/test_send_files/test_send_basics.yaml`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/common/test_env_helper.py` & `rc3-0.0.6/tests/common/test_env_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/common/test_inherit_helper.py` & `rc3-0.0.6/tests/common/test_inherit_helper.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/conftest.py` & `rc3-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/learning/test_sample.py` & `rc3-0.0.6/tests/learning/test_sample.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/test_cli.py` & `rc3-0.0.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rc3-0.0.5/tests/util/decorators.py` & `rc3-0.0.6/tests/util/decorators.py`

 * *Files identical despite different names*

