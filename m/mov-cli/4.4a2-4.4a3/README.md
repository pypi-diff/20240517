# Comparing `tmp/mov_cli-4.4a2.tar.gz` & `tmp/mov_cli-4.4a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-4.4a2.tar", last modified: Fri May 10 02:34:55 2024, max compression
+gzip compressed data, was "mov_cli-4.4a3.tar", last modified: Fri May 17 20:50:00 2024, max compression
```

## Comparing `mov_cli-4.4a2.tar` & `mov_cli-4.4a3.tar`

### file list

```diff
@@ -1,76 +1,75 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.500015 mov_cli-4.4a2/.github/
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.503348 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      185 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/addprovider.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      925 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      319 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/dependabot.yml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.503348 mov_cli-4.4a2/.github/workflows/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.github/workflows/pypi.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.4a2/.github/workflows/ruff.yml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.4a2/.gitignore
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.4a2/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.4a2/Makefile
--rw-r--r--   0 goldy     (1000) goldy     (1000)     8049 2024-05-10 02:34:55.513348 mov_cli-4.4a2/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     5336 2024-05-03 21:25:09.000000 mov_cli-4.4a2/README.md
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1549 2024-04-19 20:31:56.000000 mov_cli-4.4a2/disclaimer.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.506681 mov_cli-4.4a2/mov_cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      135 2024-05-10 01:48:21.000000 mov_cli-4.4a2/mov_cli/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/cli/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.4a2/mov_cli/cli/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6033 2024-05-10 02:23:24.000000 mov_cli-4.4a2/mov_cli/cli/__main__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/cli/auto_select.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2265 2024-05-10 02:23:30.000000 mov_cli-4.4a2/mov_cli/cli/configuration.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2063 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/cli/episode.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3640 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/cli/play.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1533 2024-04-29 18:49:16.000000 mov_cli-4.4a2/mov_cli/cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      159 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/cli/random_tips.json
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6217 2024-05-03 22:20:27.000000 mov_cli-4.4a2/mov_cli/cli/scraper.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1105 2024-05-10 01:47:20.000000 mov_cli-4.4a2/mov_cli/cli/search.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     6946 2024-04-25 20:43:50.000000 mov_cli-4.4a2/mov_cli/cli/ui.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1320 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/cli/watch_options.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     8406 2024-05-10 02:04:37.000000 mov_cli-4.4a2/mov_cli/config.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      621 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/config.template.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2245 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/download.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/errors.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3434 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/http_client.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/iterfzf/
--rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.4a2/mov_cli/iterfzf/LICENSE.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.4a2/mov_cli/iterfzf/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.4a2/mov_cli/logger.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/media/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       44 2023-12-08 21:51:24.000000 mov_cli-4.4a2/mov_cli/media/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2953 2024-04-29 18:49:16.000000 mov_cli-4.4a2/mov_cli/media/media.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2134 2024-05-10 01:51:12.000000 mov_cli-4.4a2/mov_cli/media/metadata.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.510015 mov_cli-4.4a2/mov_cli/players/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      134 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      972 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/custom_player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1599 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/iina.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1885 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/mpv.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      715 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/player.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2305 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/syncplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3632 2024-05-03 21:25:09.000000 mov_cli-4.4a2/mov_cli/players/vlc.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2047 2024-04-29 18:49:16.000000 mov_cli-4.4a2/mov_cli/plugins.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1776 2024-05-03 22:17:47.000000 mov_cli-4.4a2/mov_cli/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/mov_cli/utils/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.4a2/mov_cli/utils/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      620 2024-04-04 00:43:21.000000 mov_cli-4.4a2/mov_cli/utils/episode_selector.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.4a2/mov_cli/utils/paths.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)      652 2024-03-13 15:29:53.000000 mov_cli-4.4a2/mov_cli/utils/platform.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/mov_cli/utils/scraper/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/utils/scraper/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4751 2024-04-19 20:31:56.000000 mov_cli-4.4a2/mov_cli/utils/scraper/the_movie_db.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2824 2024-05-01 08:46:47.000000 mov_cli-4.4a2/mov_cli/utils/version.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/mov_cli.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     8049 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1510 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/entry_points.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)      244 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-05-10 02:34:55.000000 mov_cli-4.4a2/mov_cli.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1801 2024-05-10 02:03:17.000000 mov_cli-4.4a2/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.4a2/ruff.toml
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-10 02:34:55.513348 mov_cli-4.4a2/scripts/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.4a2/scripts/test_cli.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-10 02:34:55.513348 mov_cli-4.4a2/setup.cfg
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.135967 mov_cli-4.4a3/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.122634 mov_cli-4.4a3/.github/
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.125967 mov_cli-4.4a3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      469 2024-05-16 17:10:47.000000 mov_cli-4.4a3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      300 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      500 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.github/dependabot.yml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.125967 mov_cli-4.4a3/.github/workflows/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1047 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.github/workflows/pypi.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      704 2024-03-20 02:02:17.000000 mov_cli-4.4a3/.github/workflows/ruff.yml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       78 2023-12-08 21:51:24.000000 mov_cli-4.4a3/.gitignore
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 00:50:47.000000 mov_cli-4.4a3/LICENSE
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      296 2024-04-25 20:43:50.000000 mov_cli-4.4a3/Makefile
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8683 2024-05-17 20:50:00.135967 mov_cli-4.4a3/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     5970 2024-05-16 17:10:47.000000 mov_cli-4.4a3/README.md
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1545 2024-05-16 17:10:47.000000 mov_cli-4.4a3/disclaimer.md
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.125967 mov_cli-4.4a3/mov_cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      135 2024-05-16 17:10:56.000000 mov_cli-4.4a3/mov_cli/__init__.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.129301 mov_cli-4.4a3/mov_cli/cli/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       17 2023-12-08 21:51:24.000000 mov_cli-4.4a3/mov_cli/cli/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6199 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/cli/__main__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      416 2024-04-19 20:31:56.000000 mov_cli-4.4a3/mov_cli/cli/auto_select.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2455 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/configuration.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2099 2024-05-16 21:27:57.000000 mov_cli-4.4a3/mov_cli/cli/episode.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3640 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/play.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1533 2024-04-29 18:49:16.000000 mov_cli-4.4a3/mov_cli/cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      225 2024-05-16 17:09:32.000000 mov_cli-4.4a3/mov_cli/cli/random_tips.json
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     6217 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/scraper.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1096 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/cli/search.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     7063 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/ui.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1318 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/cli/watch_options.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     9115 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/config.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      640 2024-05-17 20:46:10.000000 mov_cli-4.4a3/mov_cli/config.template.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2245 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/download.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      563 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/errors.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3434 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/http_client.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.129301 mov_cli-4.4a3/mov_cli/iterfzf/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)    35147 2024-03-10 14:47:07.000000 mov_cli-4.4a3/mov_cli/iterfzf/LICENSE.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4123 2024-04-04 00:43:21.000000 mov_cli-4.4a3/mov_cli/iterfzf/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      229 2023-12-08 21:51:24.000000 mov_cli-4.4a3/mov_cli/logger.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/media/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       67 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/media/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3010 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/media/media.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1972 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/media/metadata.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      355 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/media/quality.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/players/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      134 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      972 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/custom_player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1599 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/iina.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1891 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/players/mpv.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      715 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/player.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2305 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/players/syncplay.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3638 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/players/vlc.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2047 2024-04-29 18:49:16.000000 mov_cli-4.4a3/mov_cli/plugins.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1776 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/scraper.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/utils/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       99 2024-04-22 21:39:57.000000 mov_cli-4.4a3/mov_cli/utils/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      707 2024-05-16 17:10:43.000000 mov_cli-4.4a3/mov_cli/utils/episode_selector.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     2018 2024-04-22 23:14:10.000000 mov_cli-4.4a3/mov_cli/utils/paths.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1133 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/utils/platform.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli/utils/scraper/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       69 2024-04-19 20:31:56.000000 mov_cli-4.4a3/mov_cli/utils/scraper/__init__.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     4752 2024-05-16 21:28:20.000000 mov_cli-4.4a3/mov_cli/utils/scraper/the_movie_db.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     3576 2024-05-17 20:45:21.000000 mov_cli-4.4a3/mov_cli/utils/version.py
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/mov_cli.egg-info/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     8683 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/PKG-INFO
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1460 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       53 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/entry_points.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      244 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/requires.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)        8 2024-05-17 20:50:00.000000 mov_cli-4.4a3/mov_cli.egg-info/top_level.txt
+-rw-r--r--   0 goldy     (1000) goldy     (1000)     1801 2024-05-16 17:10:43.000000 mov_cli-4.4a3/pyproject.toml
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      243 2024-04-04 00:43:21.000000 mov_cli-4.4a3/ruff.toml
+drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-05-17 20:50:00.132634 mov_cli-4.4a3/scripts/
+-rw-r--r--   0 goldy     (1000) goldy     (1000)      285 2023-12-08 21:51:24.000000 mov_cli-4.4a3/scripts/test_cli.py
+-rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-05-17 20:50:00.135967 mov_cli-4.4a3/setup.cfg
```

### Comparing `mov_cli-4.4a2/.github/workflows/pypi.yml` & `mov_cli-4.4a3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/.github/workflows/ruff.yml` & `mov_cli-4.4a3/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/LICENSE` & `mov_cli-4.4a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/PKG-INFO` & `mov_cli-4.4a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.4a2
+Version: 4.4a3
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -87,15 +87,20 @@
     <img src="https://invidget.switchblade.xyz/BMzC7ePsBV" alt="Logo" width="400">
   </a>
 
 </div>
 <br>
 
 > [!Note]
-> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also I would advise not using it as a library yet as the API still has many breaking changes.
+> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also, I would advise not using it as a library yet as the API still has many breaking changes.
+
+## What is mov-cli? 💫
+mov-cli is a command line tool that streamlines the process of streaming media from the comfort of your terminal; ~~*so you can show off to your friends the superiority of the command line.*~~ 💪 The tool is sort of a framework that handles metadata and configuration, then simply invokes your media player.
+
+mov-cli [is **not** a piracy tool](./disclaimer.md); in fact, we encourage the opposite through the existence of our plugins [mov-cli-fs](https://github.com/mov-cli/mov-cli-files) and [mov-cli-media-server](https://github.com/mov-cli/mov-cli-ms). 🫵 You obtain the media. You pick the plugins.
 
 ## Installation 🛠️
 
 > [!TIP]
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.4a2 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a3 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -40,59 +40,68 @@
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
-plugins up to date**. Also I would advise not using it as a library yet as the
-API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
-cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
-Windows - Android (via [Termux](https://termux.dev/en/)) - *iOS (via [iSH
-Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/
-issues/256) - MacOS - **[python](https://www.python.org/downloads/)**
-(**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
-(optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
-fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
-**[mpv](https://mpv.io/installation/)** (recommended & default media player) To
-get running these are all the prerequisites you'll need. With the prerequisites
-installed, mov-cli can be installed via the pip command on all platforms with
-Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
-[wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation)
-for more in-depth guidance on installing mov-cli. ## Usage ð±ï¸ mov-cli
-comes packaged with a CLI interface via the `mov-cli` command you can use in
-your respective terminal. > [!NOTE] > You may notice mov-cli doesn't ship with
-any scrapers (or previously known as providers) by default, this is because v4
-is plugin-based and scrapers are now part of plugins that must be chosen to be
-installed. > Find out how to do so at the [wiki](https://github.com/mov-cli/
-mov-cli/wiki#plugins). 1. Install the scraper plugin of your choice. Visit this
-[wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so
-and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a
-list of **third-party** mov-cli plugins. ```sh mov-cli -e ``` Alternatively,
-you may also edit by manually opening the config file. See this [Wiki page]
-(https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
-```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
-mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
-132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
-`flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
-plugin, **however once again mov-cli is plugin based and there are many of them
-[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Star Graph
-â­ [![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-
-cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing
-â¨ Pull requests are welcome and *appreciated*. For major changes, please open
-an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
-_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
-justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
-animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
-cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
-cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
-forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
-mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
+plugins up to date**. Also, I would advise not using it as a library yet as the
+API still has many breaking changes. ## What is mov-cli? ð« mov-cli is a
+command line tool that streamlines the process of streaming media from the
+comfort of your terminal; ~~*so you can show off to your friends the
+superiority of the command line.*~~ ðª The tool is sort of a framework that
+handles metadata and configuration, then simply invokes your media player. mov-
+cli [is **not** a piracy tool](./disclaimer.md); in fact, we encourage the
+opposite through the existence of our plugins [mov-cli-fs](https://github.com/
+mov-cli/mov-cli-files) and [mov-cli-media-server](https://github.com/mov-cli/
+mov-cli-ms). ð«µ You obtain the media. You pick the plugins. ## Installation
+ð ï¸ > [!TIP] > For in-depth installation instructions hit the [wiki](https:
+//github.com/mov-cli/mov-cli/wiki/Installation). ### Prerequisites - **A
+supported platform:** - Linux - Windows - Android (via [Termux](https://
+termux.dev/en/)) - *iOS (via [iSH Shell](https://ish.app/))* (unstable, https:/
+/github.com/mov-cli/mov-cli/issues/256) - MacOS - **[python](https://
+www.python.org/downloads/)** (**required**, with pip) - **[lxml](https://
+pypi.org/project/lxml/)** (optional, â¡ faster scraping) - **[fzf](https://
+github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but
+**highly recommended**) - **[mpv](https://mpv.io/installation/)** (recommended
+& default media player) To get running these are all the prerequisites you'll
+need. With the prerequisites installed, mov-cli can be installed via the pip
+command on all platforms with Python version 3.8 or above. ```sh pip install
+mov-cli -U ``` > Check out the [wiki on installation](https://github.com/mov-
+cli/mov-cli/wiki/Installation) for more in-depth guidance on installing mov-
+cli. ## Usage ð±ï¸ mov-cli comes packaged with a CLI interface via the `mov-
+cli` command you can use in your respective terminal. > [!NOTE] > You may
+notice mov-cli doesn't ship with any scrapers (or previously known as
+providers) by default, this is because v4 is plugin-based and scrapers are now
+part of plugins that must be chosen to be installed. > Find out how to do so at
+the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins). 1. Install the
+scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-
+cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://
+github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli
+plugins. ```sh mov-cli -e ``` Alternatively, you may also edit by manually
+opening the config file. See this [Wiki page](https://github.com/mov-cli/mov-
+cli/wiki/Configuration#introduction) on that. ```toml [mov-cli.plugins] youtube
+= "mov-cli-youtube" ``` 2. Scrape away! ```sh mov-cli -s youtube flight 370 ```
+[https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-
+f788da1d5118]> The command above searches for `flight 370` with our [youtube]
+(https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-
+cli is plugin based and there are many of them [in the wild](https://
+github.com/topics/mov-cli-plugin). ð** ## Star Graph â­ [![Star Graph
+Chart](https://api.star-history.com/svg?repos=mov-cli/mov-cli&type=Date)]
+(https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing â¨ Pull
+requests are welcome and *appreciated*. For major changes, please open an issue
+first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-cli](https://
+github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/
+lobster) and [animdl](https://github.com/justfoolingaround/animdl)
+[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-
+cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/mov-
+cli/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
+mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/mov-
+cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/ [pypi-stats-url]: https://
 pypistats.org/packages/mov-cli [python-shield]: https://img.shields.io/pypi/
 pyversions/mov-cli?style=flat [issues-shield]: https://img.shields.io/github/
 issues/mov-cli/mov-cli?style=flat [issues-url]: https://github.com/mov-cli/mov-
 cli/issues [license-shield]: https://img.shields.io/github/license/mov-cli/mov-
```

### Comparing `mov_cli-4.4a2/README.md` & `mov_cli-4.4a3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,20 @@
     <img src="https://invidget.switchblade.xyz/BMzC7ePsBV" alt="Logo" width="400">
   </a>
 
 </div>
 <br>
 
 > [!Note]
-> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also I would advise not using it as a library yet as the API still has many breaking changes.
+> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also, I would advise not using it as a library yet as the API still has many breaking changes.
+
+## What is mov-cli? 💫
+mov-cli is a command line tool that streamlines the process of streaming media from the comfort of your terminal; ~~*so you can show off to your friends the superiority of the command line.*~~ 💪 The tool is sort of a framework that handles metadata and configuration, then simply invokes your media player.
+
+mov-cli [is **not** a piracy tool](./disclaimer.md); in fact, we encourage the opposite through the existence of our plugins [mov-cli-fs](https://github.com/mov-cli/mov-cli-files) and [mov-cli-media-server](https://github.com/mov-cli/mov-cli-ms). 🫵 You obtain the media. You pick the plugins.
 
 ## Installation 🛠️
 
 > [!TIP]
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
```

#### html2text {}

```diff
@@ -5,59 +5,68 @@
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
-plugins up to date**. Also I would advise not using it as a library yet as the
-API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
-cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
-Windows - Android (via [Termux](https://termux.dev/en/)) - *iOS (via [iSH
-Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/
-issues/256) - MacOS - **[python](https://www.python.org/downloads/)**
-(**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
-(optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
-fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
-**[mpv](https://mpv.io/installation/)** (recommended & default media player) To
-get running these are all the prerequisites you'll need. With the prerequisites
-installed, mov-cli can be installed via the pip command on all platforms with
-Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
-[wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation)
-for more in-depth guidance on installing mov-cli. ## Usage ð±ï¸ mov-cli
-comes packaged with a CLI interface via the `mov-cli` command you can use in
-your respective terminal. > [!NOTE] > You may notice mov-cli doesn't ship with
-any scrapers (or previously known as providers) by default, this is because v4
-is plugin-based and scrapers are now part of plugins that must be chosen to be
-installed. > Find out how to do so at the [wiki](https://github.com/mov-cli/
-mov-cli/wiki#plugins). 1. Install the scraper plugin of your choice. Visit this
-[wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so
-and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a
-list of **third-party** mov-cli plugins. ```sh mov-cli -e ``` Alternatively,
-you may also edit by manually opening the config file. See this [Wiki page]
-(https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
-```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
-mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
-132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
-`flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
-plugin, **however once again mov-cli is plugin based and there are many of them
-[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Star Graph
-â­ [![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-
-cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing
-â¨ Pull requests are welcome and *appreciated*. For major changes, please open
-an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
-_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
-justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
-animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
-cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
-cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
-forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
-mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
+plugins up to date**. Also, I would advise not using it as a library yet as the
+API still has many breaking changes. ## What is mov-cli? ð« mov-cli is a
+command line tool that streamlines the process of streaming media from the
+comfort of your terminal; ~~*so you can show off to your friends the
+superiority of the command line.*~~ ðª The tool is sort of a framework that
+handles metadata and configuration, then simply invokes your media player. mov-
+cli [is **not** a piracy tool](./disclaimer.md); in fact, we encourage the
+opposite through the existence of our plugins [mov-cli-fs](https://github.com/
+mov-cli/mov-cli-files) and [mov-cli-media-server](https://github.com/mov-cli/
+mov-cli-ms). ð«µ You obtain the media. You pick the plugins. ## Installation
+ð ï¸ > [!TIP] > For in-depth installation instructions hit the [wiki](https:
+//github.com/mov-cli/mov-cli/wiki/Installation). ### Prerequisites - **A
+supported platform:** - Linux - Windows - Android (via [Termux](https://
+termux.dev/en/)) - *iOS (via [iSH Shell](https://ish.app/))* (unstable, https:/
+/github.com/mov-cli/mov-cli/issues/256) - MacOS - **[python](https://
+www.python.org/downloads/)** (**required**, with pip) - **[lxml](https://
+pypi.org/project/lxml/)** (optional, â¡ faster scraping) - **[fzf](https://
+github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but
+**highly recommended**) - **[mpv](https://mpv.io/installation/)** (recommended
+& default media player) To get running these are all the prerequisites you'll
+need. With the prerequisites installed, mov-cli can be installed via the pip
+command on all platforms with Python version 3.8 or above. ```sh pip install
+mov-cli -U ``` > Check out the [wiki on installation](https://github.com/mov-
+cli/mov-cli/wiki/Installation) for more in-depth guidance on installing mov-
+cli. ## Usage ð±ï¸ mov-cli comes packaged with a CLI interface via the `mov-
+cli` command you can use in your respective terminal. > [!NOTE] > You may
+notice mov-cli doesn't ship with any scrapers (or previously known as
+providers) by default, this is because v4 is plugin-based and scrapers are now
+part of plugins that must be chosen to be installed. > Find out how to do so at
+the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins). 1. Install the
+scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-
+cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://
+github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli
+plugins. ```sh mov-cli -e ``` Alternatively, you may also edit by manually
+opening the config file. See this [Wiki page](https://github.com/mov-cli/mov-
+cli/wiki/Configuration#introduction) on that. ```toml [mov-cli.plugins] youtube
+= "mov-cli-youtube" ``` 2. Scrape away! ```sh mov-cli -s youtube flight 370 ```
+[https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-
+f788da1d5118]> The command above searches for `flight 370` with our [youtube]
+(https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-
+cli is plugin based and there are many of them [in the wild](https://
+github.com/topics/mov-cli-plugin). ð** ## Star Graph â­ [![Star Graph
+Chart](https://api.star-history.com/svg?repos=mov-cli/mov-cli&type=Date)]
+(https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing â¨ Pull
+requests are welcome and *appreciated*. For major changes, please open an issue
+first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-cli](https://
+github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/
+lobster) and [animdl](https://github.com/justfoolingaround/animdl)
+[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-
+cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/mov-
+cli/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
+mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/mov-
+cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/ [pypi-stats-url]: https://
 pypistats.org/packages/mov-cli [python-shield]: https://img.shields.io/pypi/
 pyversions/mov-cli?style=flat [issues-shield]: https://img.shields.io/github/
 issues/mov-cli/mov-cli?style=flat [issues-url]: https://github.com/mov-cli/mov-
 cli/issues [license-shield]: https://img.shields.io/github/license/mov-cli/mov-
```

### Comparing `mov_cli-4.4a2/disclaimer.md` & `mov_cli-4.4a3/disclaimer.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 <div align="center">
 
   # Disclaimer
 
 </div>
 
 ## This project: mov-cli
-
 The core aim of this project is to correlate automation and efficiency to extract what is provided to a user on the internet.
 
 Think of this project as your browser, which can visit sites like https://youtube.com, making multiple useless/tracking requests. This project is made for easier access to content without its tracking.
 
 **This project has no control over the content it is serving; using copyrighted content from user-made plugins is not accounted for by the developers. It is at the user's own risk.**
 
 ## DMCA and Copyright Infringements
-
 **This tool works like a browser, and the maliciousness of the tool is directly based on the user.**
 
 This project uses client-side content access mechanisms. Hence, the copyright infringements or DMCA regarding this project should be forwarded to the associated site by the associated notifier of any such claims.
 
 **Do not harass the developers. Any personal information about the developers is intentionally not made public. Exploiting such information without consent regarding this topic will lead to legal actions by the developers themselves.**
 
 ## Third-Party Plugins
-
 Please note that plugins used with this project are developed by third-parties, and anyone can create them. The developers of this project do not endorse or take responsibility for the actions or content provided by these plugins.
 
 ## Contacting the developers
-
 Begin by creating a GitHub issue or joining the Discord: https://discord.gg/BMzC7ePsBV
```

### Comparing `mov_cli-4.4a2/mov_cli/cli/__main__.py` & `mov_cli-4.4a3/mov_cli/cli/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,29 +32,30 @@
     debug: Optional[bool] = typer.Option(None, help = "Enable extra logging details. Useful for bug reporting."), 
     player: Optional[str] = typer.Option(None, "--player", "-p", help = "Player you would like to stream with. E.g. mpv, vlc"), 
     scraper: Optional[str] = typer.Option(None, "--scraper", "-s", help = "Scraper you would like to scrape with. E.g. remote_stream, sflix"), 
     fzf: Optional[bool] = typer.Option(None, help = "Toggle fzf on/off for all user selection prompts."), 
     episode: Optional[str] = typer.Option(None, "--episode", "-ep", help = "Episode and season you wanna scrape. E.g. {episode}:{season} like -> 26:3"), 
     auto_select: Optional[int] = typer.Option(None, "--choice", "-c", help = "Auto select the search results. E.g. Setting it to 1 with query 'nyan cat' will pick " \
         "the first nyan cat video to show up in search results."
-    ), 
+    ),
+    limit: Optional[int] = typer.Option(None, "--limit", "-l", help = "Specify the maximum number of results"),
 
     version: bool = typer.Option(False, "--version", help = "Display what version mov-cli is currently on."), 
     edit: bool = typer.Option(False, "--edit", "-e", help = "Opens the mov-cli config with your respective editor."), 
     download: bool = typer.Option(False, "--download", "-d", help = "Downloads the media instead of playing."),
     list_plugins: bool = typer.Option(False, "--list-plugins", "-lp", help = "Prints all configured plugins and their scrapers."),
 ):
     config = Config()
 
     config = set_cli_config(
-        config,
-        debug = debug,
-        player = player,
-        scraper = scraper,
-        fzf = fzf
+        config, 
+        debug = debug, 
+        player = player, 
+        scraper = (scraper, ["scrapers", "default"]), 
+        fzf = (fzf, ["ui", "fzf"])
     )
 
     if config.debug:
         mov_cli_logger.setLevel(logging.DEBUG)
 
     mov_cli_logger.debug(f"Config -> {config.data}")
 
@@ -96,15 +97,15 @@
             )
             return False
 
         selected_scraper[2].update(scrape_options)
 
         chosen_scraper = use_scraper(selected_scraper, config, http_client)
 
-        choice = search(query, auto_select, chosen_scraper, config.fzf_enabled)
+        choice = search(query, auto_select, chosen_scraper, config.fzf_enabled, limit)
 
         if choice is None:
             mov_cli_logger.error("There was no results or you didn't select anything.")
             return False
 
         chosen_episode = handle_episode(
             episode_string = episode,
```

### Comparing `mov_cli-4.4a2/mov_cli/cli/configuration.py` & `mov_cli-4.4a3/mov_cli/scraper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,71 +1,55 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from pathlib import Path
-    from typing import Optional, Any
-    from ..config import Config
-
-import os
-from subprocess import check_call, CalledProcessError
-
-from .. import utils
-from ..logger import mov_cli_logger
-
-def set_cli_config(config: Config, **kwargs: Optional[Any]) -> Config:
-    debug = kwargs.get("debug")
-    player = kwargs.get("player")
-    scraper = kwargs.get("scraper")
-    fzf = kwargs.get("fzf")
-
-    if debug is not None:
-        config.data["debug"] = debug
-
-    if player is not None:
-        config.data["player"] = player
-
-    if scraper is not None:
-        if config.data.get("scrapers") is None:
-            config.data["scrapers"] = {}
-
-        config.data["scrapers"]["default"] = scraper
-
-    if fzf is not None:
-        if config.data.get("ui") is None:
-            config.data["ui"] = {}
-
-        config.data["ui"]["fzf"] = fzf
-
-    return config
-
-def open_config_file(config: Config, file_path: Optional[Path] = None):
-    """Opens the config file in the respectable editor for that platform."""
-    editor = config.editor
-    platform = utils.what_platform()
-
-    if editor is None: 
-        env_editor = os.environ.get("EDITOR")        
-
-        if env_editor is not None:
-            editor = env_editor
-        else:
-            if platform == "Windows":
-                editor = "notepad"
-            elif platform == "Darwin":
-                editor = "nano" # NOTE: https://support.apple.com/guide/terminal/use-command-line-text-editors-apdb02f1133-25af-4c65-8976-159609f99817/mac
-            elif platform == "iOS":
-                editor = "vi"
-            elif platform == "Linux" or platform == "Android":
-                editor = "nano"
-
-    mov_cli_logger.debug("Opening config file...")
-
-    appdata_path = utils.get_appdata_directory(platform)
-
-    try:
-        check_call([editor, config.config_path if file_path is None else appdata_path.joinpath(file_path)])
-    except (FileNotFoundError, CalledProcessError) as e:
-        mov_cli_logger.error(
-            f"Failed to open config file with the editor '{editor}'! Error: {e}" \
-                f"\nYou can manually edit it over here: '{config.config_path}'."
-        )
+    from typing import Dict, Literal, Iterable, Optional
+
+    from .config import Config
+    from .utils import EpisodeSelector
+    from .http_client import HTTPClient
+    from .media import Metadata, Multi, Single
+
+    ScraperOptionsT = Dict[str, str | bool]
+
+from bs4 import BeautifulSoup
+from abc import ABC, abstractmethod
+from devgoldyutils import LoggerAdapter
+
+from .logger import mov_cli_logger
+
+__all__ = (
+    "Scraper",
+)
+
+class Scraper(ABC):
+    """A base class for building scrapers from."""
+    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
+        self.config = config
+        self.http_client = http_client
+        self.options = options or {}
+
+        self.logger = LoggerAdapter(mov_cli_logger, prefix = self.__class__.__name__)
+
+        super().__init__()
+
+    def soup(self, html: str, **kwargs) -> BeautifulSoup:
+        """A ready to use beautiful soup instance."""
+        return BeautifulSoup(html, self.config.parser, **kwargs)
+
+    @abstractmethod
+    def search(self, query: str, limit: int = 20) -> Iterable[Metadata]:
+        """Where your searching for media should be done. Should return or yield Metadata."""
+        ...
+
+    @abstractmethod
+    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Optional[Multi | Single]:
+        """
+        Where your scraping for the media should be performed. 
+        Should return or yield an instance of Media.
+        """
+        ...
+
+    @abstractmethod
+    def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
+        """Returns episode count for each season in that Movie/Series."""
+        ...
```

### Comparing `mov_cli-4.4a2/mov_cli/cli/episode.py` & `mov_cli-4.4a3/mov_cli/cli/episode.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 from .ui import prompt
 
 from ..media import MetadataType
 from ..utils import EpisodeSelector
 from ..logger import mov_cli_logger
 
 def handle_episode(episode_string: Optional[str], scraper: Scraper, choice: Metadata, fzf_enabled: bool) -> Optional[EpisodeSelector]:
-    if choice.type == MetadataType.MOVIE:
+    if choice.type == MetadataType.SINGLE:
         return EpisodeSelector()
 
+    metadata_episodes = scraper.scrape_episodes(choice)
+
     if episode_string is None:
         mov_cli_logger.info(f"Scrapping episodes for '{Colours.CLAY.apply(choice.title)}'...")
-        metadata_episodes = scraper.scrape_episodes(choice)
 
         if metadata_episodes.get(None) == 1:
             return EpisodeSelector()
 
         season = prompt(
             "Select Season", 
             choices = [season for season in metadata_episodes], 
@@ -41,15 +42,15 @@
             display = lambda x: f"Episode {x}",
             fzf_enabled = fzf_enabled
         )
 
         if episode is None:
             return None
 
-        return EpisodeSelector(episode, season)
+        return EpisodeSelector(episode, season, metadata_episodes)
 
     try:
         episode_season = episode_string.split(":")
 
         episode = 1
         season = 1
 
@@ -64,8 +65,8 @@
         mov_cli_logger.error(
             "Incorrect episode format! This is how it's done --> '5:1' (5 being episode and 1 being season)\n" \
                 f"Error: {e}"
         )
 
         return None
 
-    return EpisodeSelector(episode, season)
+    return EpisodeSelector(episode, season, metadata_episodes)
```

### Comparing `mov_cli-4.4a2/mov_cli/cli/play.py` & `mov_cli-4.4a3/mov_cli/cli/play.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/cli/plugins.py` & `mov_cli-4.4a3/mov_cli/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/cli/scraper.py` & `mov_cli-4.4a3/mov_cli/cli/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/cli/search.py` & `mov_cli-4.4a3/mov_cli/cli/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 from devgoldyutils import Colours
 
 from .ui import prompt
 from .auto_select import auto_select_choice
 from .plugins import handle_internal_plugin_error
 
-from ..media import MetadataType
 from ..logger import mov_cli_logger
 
-def search(query: str, auto_select: Optional[int], scraper: Scraper, fzf_enabled: bool) -> Optional[Metadata]:
+def search(query: str, auto_select: Optional[int], scraper: Scraper, fzf_enabled: bool, limit: int = 20) -> Optional[Metadata]:
     choice = None
 
     mov_cli_logger.info(f"Searching for '{Colours.ORANGE.apply(query)}'...")
 
     try:
-        search_results = scraper.search(query)
+        search_results = scraper.search(query, limit)
     except Exception as e:
         handle_internal_plugin_error(e)
 
     if auto_select is not None:
         choice = auto_select_choice((choice for choice in search_results), auto_select)
     else:
         choice = prompt(
```

### Comparing `mov_cli-4.4a2/mov_cli/cli/ui.py` & `mov_cli-4.4a3/mov_cli/cli/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from inquirer.themes import Default
 from devgoldyutils import Colours, LoggerAdapter
 
 import mov_cli
 
 from ..iterfzf import iterfzf
 from ..logger import mov_cli_logger
-from ..utils import  what_platform, update_available, plugin_update_available
+from ..utils import  what_platform, update_available, plugin_update_available, update_command
 
 __all__ = (
     "prompt", 
 )
 
 logger = LoggerAdapter(mov_cli_logger, prefix = Colours.PURPLE.apply("prompt"))
 
@@ -160,19 +160,20 @@
     plugins: Dict[str, str], 
     check_for_updates: bool = False, 
     display_tip: bool = False, 
     display_version: bool = False
 ) -> str:
     """Returns cli welcome message."""
     now = datetime.now()
+    mov_cli_path = Path(os.path.split(__file__)[0])
     adjective = random.choice(
         ("gorgeous", "wonderful", "beautiful", "magnificent")
     )
 
-    random_tips_path = Path(os.path.split(__file__)[0]).joinpath("random_tips.json")
+    random_tips_path = mov_cli_path.joinpath("random_tips.json")
 
     greeting, user_name = greetings()
 
     text = f"\n{greeting}, {Colours.ORANGE.apply(user_name)}."
     text += now.strftime(
         f"\n    It's {Colours.BLUE}%I:%M %p {Colours.RESET}on a {Colours.PURPLE}{adjective} {Colours.PINK_GREY}%A! {Colours.RESET}"
     )
@@ -191,15 +192,17 @@
 
     if display_version is True:
         text += f"\n\n{Colours.CLAY}-> {Colours.RESET}Version: {Colours.BLUE}{mov_cli.__version__}{Colours.RESET}"
 
     if check_for_updates:
 
         if update_available():
-            text += f"\n\n {Colours.PURPLE}ツ {Colours.ORANGE}An update is available! --> {Colours.RESET}pip install mov-cli -U"
+            update = update_command(mov_cli_path)
+            text += f"\n\n {Colours.PURPLE}ツ {Colours.ORANGE}An update is available! --> {Colours.RESET}{update}"
 
         plugin_needs_updating, plugins_to_update = plugin_update_available(plugins)
 
         if plugin_needs_updating:
-            text += f"\n\n {Colours.ORANGE}|˶˙ᵕ˙ )ﾉﾞ {Colours.GREEN}Some plugins need updating! --> {Colours.RESET}pip install {' '.join(plugins_to_update)} -U"
+            update = update_command(mov_cli_path, plugins_to_update)
+            text += f"\n\n {Colours.ORANGE}|˶˙ᵕ˙ )ﾉﾞ {Colours.GREEN}Some plugins need updating! --> {Colours.RESET}{update}"
 
     return text + "\n"
```

### Comparing `mov_cli-4.4a2/mov_cli/cli/watch_options.py` & `mov_cli-4.4a3/mov_cli/cli/watch_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     from ..players import Player
     from ..utils.platform import SUPPORTED_PLATFORMS
 
 import time
 from subprocess import Popen
 
 from .ui import prompt
-from ..media import Series
+from ..media import Multi
 
 def watch_options(
     popen: Popen, 
     player: Player, 
     platform: SUPPORTED_PLATFORMS, 
     media: Media, 
     fzf_enabled: bool
 ) -> Optional[Literal["search", "next", "previous", "select"]]:
     options = [
         "search",
         "replay",
         "quit"
     ]
 
-    if isinstance(media, Series):
+    if isinstance(media, Multi):
         options.insert(0, "next")
         options.insert(1, "previous")
         options.insert(2, "select")
 
     if platform == "iOS":
         time.sleep(3) # so iOS mfs have time to read the "pasted to clipboard" prompt. (untested 👍) lmao
```

### Comparing `mov_cli-4.4a2/mov_cli/config.py` & `mov_cli-4.4a3/mov_cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from decouple import AutoConfig
 from importlib.util import find_spec
 from devgoldyutils import LoggerAdapter
 
 from . import players, utils
 from .logger import mov_cli_logger
 from .utils import get_appdata_directory
+from .media import Quality
 
 __all__ = ("Config",)
 
 @final
 class ConfigUIData(TypedDict):
     fzf: bool
 
@@ -39,26 +40,30 @@
 
 @final
 class ConfigDownloadsData(TypedDict):
     save_path: str
     yt_dlp: bool
 
 @final
+class ConfigQualityData(TypedDict):
+    resolution: int
+
+@final
 class ConfigData(TypedDict):
     version: int
     debug: bool
     player: str
     editor: str
     parser: SupportedParsersT
     ui: ConfigUIData
     http: ConfigHTTPData
     downloads: ConfigDownloadsData
     scrapers: ScrapersConfigT | Dict[str, str]
     plugins: Dict[str, str]
-    resolution: int
+    quality: ConfigQualityData | str
 
 HttpHeadersData = TypedDict(
     "HttpHeadersData", 
     {
         "User-Agent": NotRequired[str],
         "Accept-Language": NotRequired[str],
         "Accept": NotRequired[str]
@@ -210,16 +215,36 @@
             "Accept-Language": "en-US,en;q=0.5",
             "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
         }
 
         return self.data.get("http", {}).get("headers", default_headers)
 
     @property
-    def resolution(self) -> Optional[int]:
-        return self.data.get("quality", {}).get("resolution")
+    def resolution(self) -> Quality:
+        resolution_pixel = None
+        quality_config = self.data.get("quality", {})
+
+        if isinstance(quality_config, str):
+
+            for quality_format, quality in Quality.__members__.items():
+
+                if quality_format.startswith("_"):
+                    quality_format = quality_format[1:]
+
+                if quality_config.upper() == quality_format:
+                    return quality
+
+            return Quality.AUTO
+
+        resolution_pixel = quality_config.get("resolution")
+
+        if resolution_pixel is None or resolution_pixel not in Quality._value2member_map_:
+            return Quality.AUTO
+
+        return Quality(resolution_pixel)
 
     def get_env_config(self) -> AutoConfig:
         """Returns python decouple config object for mov-cli's appdata .env file."""
         return AutoConfig(self._env_path)
 
     def __get_config_file(self) -> Path:
         """Function that returns the path to the config file with multi platform support."""
```

### Comparing `mov_cli-4.4a2/mov_cli/config.template.toml` & `mov_cli-4.4a3/mov_cli/config.template.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [mov-cli]
 version = 1
-player = "mpv"
 debug = false
+player = "mpv"
+quality = "auto"
 # parser = "lxml"
 # editor = "nano"
 skip_update_checker = false
 
+# [mov-cli.quality]
+# resolution = 720
+
 # [mov-cli.ui]
 # fzf = true
 
 [mov-cli.plugins] # E.g: namespace = "package-name"
 test = "mov-cli-test"
 
 [mov-cli.scrapers]
-# default = "films"
+# default = "youtube"
 test = "test.DEFAULT"
 
 # [mov-cli.http] # Don't mess with it if you don't know what you are doing!
 # headers = { User-Agent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/117.0" }
 
 # [mov-cli.downloads] # Do not use backslashes use forward slashes
 # save_path = "~/Downloads"
-# yt_dlp = true
-
-# [mov-cli.quality]
-# resolution = 720
+# yt_dlp = true
```

### Comparing `mov_cli-4.4a2/mov_cli/download.py` & `mov_cli-4.4a3/mov_cli/download.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/errors.py` & `mov_cli-4.4a3/mov_cli/errors.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/http_client.py` & `mov_cli-4.4a3/mov_cli/http_client.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/iterfzf/LICENSE.txt` & `mov_cli-4.4a3/mov_cli/iterfzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/iterfzf/__init__.py` & `mov_cli-4.4a3/mov_cli/iterfzf/__init__.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/media/media.py` & `mov_cli-4.4a3/mov_cli/media/media.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if TYPE_CHECKING:
     from typing import Optional
     from ..utils import EpisodeSelector
 
 from abc import abstractmethod
 
 __all__ = (
-    "Media",
+    "Media", 
     "Multi", 
     "Single", 
     "Movie", 
     "Series"
 )
 
 class Media():
@@ -92,10 +92,10 @@
 
     @property
     def display_name(self) -> str:
         return f"{self.title} ({self.year})" if self.year is not None else self.title
 
 # Backwards compatibility for post v4.3 extensions.
 Series = Multi
-"""DEPRECATED!!! USE 'Multi' INSTEAD! This will be removed after v4.4."""
+"""DEPRECATED!!! USE 'Multi' INSTEAD! This will be removed after v4.4 and WILL cause hard crashes."""
 Movie = Single
-"""DEPRECATED!!! USE 'Single' INSTEAD! This will be removed after v4.4."""
+"""DEPRECATED!!! USE 'Single' INSTEAD! This will be removed after v4.4 and WILL cause hard crashes."""
```

### Comparing `mov_cli-4.4a2/mov_cli/media/metadata.py` & `mov_cli-4.4a3/mov_cli/media/metadata.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 if TYPE_CHECKING:
     from typing import List, Callable, Optional, Tuple
 
 from enum import Enum
 from devgoldyutils import Colours
 from dataclasses import dataclass, field
 
-__all__ = ("MetadataType", "Metadata", "ExtraMetadata", "AiringType")
+__all__ = (
+    "MetadataType", 
+    "Metadata", 
+    "ExtraMetadata", 
+    "AiringType"
+)
 
 class MetadataType(Enum):
     MULTI = 0
     """Media with multiple seasons and episodes."""
     SINGLE = 1
     """Media with no seasons and episodes. Like a film or short animation."""
 
-    SERIES = 0
-    """DEPRECATED!!! USE 'MetadataType.MULTI' INSTEAD! This will be removed after v4.4."""
-    MOVIE = 1
-    """DEPRECATED!!! USE 'MetadataType.SINGLE' INSTEAD!. This will be removed after v4.4."""
-
 class AiringType(Enum):
     DONE = 0
     ONGOING = 1
     PRODUCTION = 2
     RELEASED = 3
     CANCELED = 4
 
@@ -54,13 +54,13 @@
 @dataclass
 class ExtraMetadata():
     """More in-depth metadata about media."""
     description: Optional[str]
     """Description of Series, Film or TV Station."""
     image_url: Optional[str]
     """Url to high res image cover of Series, Film or TV Station."""
-    alternate_titles: List[str] | Tuple[str, str]
+    alternate_titles: List[str] | Tuple[str, str] | None = field(default = None)
 
     cast: List[str] | None = field(default = None)
     genres: List[str] | None = field(default = None)
 
     airing: AiringType | None = field(default = None)
```

### Comparing `mov_cli-4.4a2/mov_cli/players/custom_player.py` & `mov_cli-4.4a3/mov_cli/players/custom_player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/players/iina.py` & `mov_cli-4.4a3/mov_cli/players/iina.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/players/mpv.py` & `mov_cli-4.4a3/mov_cli/players/mpv.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,12 +51,12 @@
             if media.audio_url is not None:
                 args.append(f"--audio-file={media.audio_url}")
 
             if media.subtitles is not None:
                 args.append(f"--sub-file={media.subtitles}")
 
             if self.config.resolution is not None:
-                args.append(f"--hls-bitrate={self.config.resolution}") # NOTE: This only works when the file is a m3u8
+                args.append(f"--hls-bitrate={self.config.resolution.value}") # NOTE: This only works when the file is a m3u8
 
             return subprocess.Popen(args)
 
         return None
```

### Comparing `mov_cli-4.4a2/mov_cli/players/player.py` & `mov_cli-4.4a3/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/players/syncplay.py` & `mov_cli-4.4a3/mov_cli/players/syncplay.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/players/vlc.py` & `mov_cli-4.4a3/mov_cli/players/vlc.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 if subtitles.startswith("https://"):
                     logger.debug("Subtitles detected as a url.")
                     subtitles = str(self.__url_subtitles_to_file(media, subtitles))
 
                 args.append(f"--sub-file={subtitles}")
 
             if self.config.resolution is not None:
-                args.append(f"--adaptive-maxwidth={self.config.resolution}") # NOTE: I don't really know if that works ~ Ananas
+                args.append(f"--adaptive-maxwidth={self.config.resolution.value}") # NOTE: I don't really know if that works ~ Ananas
 
             return subprocess.Popen(args)
 
         return None
 
     def __url_subtitles_to_file(self, media: Media, subtitles_url: str) -> Path:
         sub_file_exists_already = False
```

### Comparing `mov_cli-4.4a2/mov_cli/plugins.py` & `mov_cli-4.4a3/mov_cli/plugins.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/utils/episode_selector.py` & `mov_cli-4.4a3/mov_cli/utils/episode_selector.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 __all__ = ("EpisodeSelector",)
 
 @dataclass
 class EpisodeSelector:
     """Swift util to use when asking the scraper which episode of a show to scrape."""
     episode: int = field(default = 1)
     season: int = field(default = 1)
+    media_episodes: dict = field(default = dict)
 
     # NOTE: I made it private as I don't want library devs using 
     # this method yet because it may drastically change in the future.
     def _next_season(self) -> None:
         self.episode = 1
         self.season += 1
 
     def _previous_season(self) -> None:
         self.season -= 1
-        self.episode = 1
+        self.episode = self.media_episodes.get(self.season, 1)
```

### Comparing `mov_cli-4.4a2/mov_cli/utils/paths.py` & `mov_cli-4.4a3/mov_cli/utils/paths.py`

 * *Files identical despite different names*

### Comparing `mov_cli-4.4a2/mov_cli/utils/scraper/the_movie_db.py` & `mov_cli-4.4a3/mov_cli/utils/scraper/the_movie_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,23 @@
     def search(self, query: str, limit: int = 10) -> Generator[Metadata, Any, None]:
         serial_list: List[TMDbSerial] = []
 
         movie = self.http_client.get(self.search_url.format("movie", query, self.api_key)).json()["results"]
         tv = self.http_client.get(self.search_url.format("tv", query, self.api_key)).json()["results"]
 
         for item in movie:
-            item = TMDbSerial(item, MetadataType.MOVIE)
+            item = TMDbSerial(item, MetadataType.SINGLE)
 
             if not item.release_date:
                 continue
 
             serial_list.append(item)
 
         for item in tv:
-            item = TMDbSerial(item, MetadataType.SERIES)
+            item = TMDbSerial(item, MetadataType.MULTI)
 
             if not item.release_date:
                 continue
 
             serial_list.append(item)
 
         for item in serial_list:
@@ -80,15 +80,15 @@
                 continue
 
             scraped_seasons[season["season_number"]] = season["episode_count"]
 
         return scraped_seasons
 
     def __extra_metadata(self, serial: TMDbSerial) -> ExtraMetadata: # This API is dawgshit
-        type = "movie" if serial.type == MetadataType.MOVIE else "tv"
+        type = "movie" if serial.type == MetadataType.SINGLE else "tv"
         metadata = self.http_client.get(self.metadata.format(type, serial.id, self.api_key)).json()
 
         description = None
         image_url = None
         cast = None
         alternate_titles = None
         genres = None
```

### Comparing `mov_cli-4.4a2/mov_cli/utils/version.py` & `mov_cli-4.4a3/mov_cli/utils/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Tuple, List, Dict
+    from pathlib import Path
 
 import httpx
 from packaging import version
 from devgoldyutils import LoggerAdapter, Colours
 
 import mov_cli
 from ..plugins import load_plugin
 from ..logger import mov_cli_logger
+from .platform import what_distro
 
 __all__ = (
     "update_available", 
-    "plugin_update_available"
+    "plugin_update_available",
+    "update_command",
 )
 
 logger = LoggerAdapter(mov_cli_logger, prefix = Colours.GREEN.apply("version"))
 
 def update_available() -> bool:
     logger.debug("Checking if mov-cli needs updating...")
 
@@ -84,8 +87,27 @@
 
         if version.parse(pypi_version) > version.parse(plugin_version):
             plugins_with_updates.append(pypi_package_name)
 
     if not plugins_with_updates == []:
         return True, plugins_with_updates
 
-    return False, []
+    return False, []
+
+def update_command(mov_cli_path: Path, package: str | list = "mov-cli"):
+    path = str(mov_cli_path)
+
+    if "pipx" in path:
+        return "pipx upgrade mov-cli --include-injected"
+    elif "/usr/bin" in path:
+        if what_distro() == "arch":
+            return "yay"
+        else:
+            if isinstance(package, list):
+                return f"Use your package manager. Packages to update: {' '.join(package)}"
+            else:
+                return f"Use your package manager. Package to update: {package}"
+    
+    if isinstance(package, list):
+        return f"pip install {' '.join(package)} -U"
+    else:
+        return f"pip install {package} -U"
```

### Comparing `mov_cli-4.4a2/mov_cli.egg-info/PKG-INFO` & `mov_cli-4.4a3/mov_cli.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 4.4a2
+Version: 4.4a3
 Summary: Watch everything from your terminal.
 Author-email: Pain <painedposeidon444@gmail.com>, Ananas <ananas@r3tr0ananas.pro>, Goldy <goldy@devgoldy.xyz>
 License: MIT License
         
         Copyright (c) 2024 mov-cli
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -87,15 +87,20 @@
     <img src="https://invidget.switchblade.xyz/BMzC7ePsBV" alt="Logo" width="400">
   </a>
 
 </div>
 <br>
 
 > [!Note]
-> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also I would advise not using it as a library yet as the API still has many breaking changes.
+> v4 is constantly changing so be sure to **keep the tool and your plugins up to date**. Also, I would advise not using it as a library yet as the API still has many breaking changes.
+
+## What is mov-cli? 💫
+mov-cli is a command line tool that streamlines the process of streaming media from the comfort of your terminal; ~~*so you can show off to your friends the superiority of the command line.*~~ 💪 The tool is sort of a framework that handles metadata and configuration, then simply invokes your media player.
+
+mov-cli [is **not** a piracy tool](./disclaimer.md); in fact, we encourage the opposite through the existence of our plugins [mov-cli-fs](https://github.com/mov-cli/mov-cli-files) and [mov-cli-media-server](https://github.com/mov-cli/mov-cli-ms). 🫵 You obtain the media. You pick the plugins.
 
 ## Installation 🛠️
 
 > [!TIP]
 > For in-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-cli/wiki/Installation).
 
 ### Prerequisites
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 4.4a2 Summary: Watch everything
+Metadata-Version: 2.1 Name: mov-cli Version: 4.4a3 Summary: Watch everything
 from your terminal. Author-email: Pain
 gmail.com>, Ananas
 r3tr0ananas.pro>, Goldy
 devgoldy.xyz> License: MIT License Copyright (c) 2024 mov-cli Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
@@ -40,59 +40,68 @@
                   _[_L_o_g_o_]Watch everything from your terminal.
 
                          _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 
                                     _[_L_o_g_o_]
 
 > [!Note] > v4 is constantly changing so be sure to **keep the tool and your
-plugins up to date**. Also I would advise not using it as a library yet as the
-API still has many breaking changes. ## Installation ð ï¸ > [!TIP] > For in-
-depth installation instructions hit the [wiki](https://github.com/mov-cli/mov-
-cli/wiki/Installation). ### Prerequisites - **A supported platform:** - Linux -
-Windows - Android (via [Termux](https://termux.dev/en/)) - *iOS (via [iSH
-Shell](https://ish.app/))* (unstable, https://github.com/mov-cli/mov-cli/
-issues/256) - MacOS - **[python](https://www.python.org/downloads/)**
-(**required**, with pip) - **[lxml](https://pypi.org/project/lxml/)**
-(optional, â¡ faster scraping) - **[fzf](https://github.com/junegunn/
-fzf?tab=readme-ov-file#installation)** (optional but **highly recommended**) -
-**[mpv](https://mpv.io/installation/)** (recommended & default media player) To
-get running these are all the prerequisites you'll need. With the prerequisites
-installed, mov-cli can be installed via the pip command on all platforms with
-Python version 3.8 or above. ```sh pip install mov-cli -U ``` > Check out the
-[wiki on installation](https://github.com/mov-cli/mov-cli/wiki/Installation)
-for more in-depth guidance on installing mov-cli. ## Usage ð±ï¸ mov-cli
-comes packaged with a CLI interface via the `mov-cli` command you can use in
-your respective terminal. > [!NOTE] > You may notice mov-cli doesn't ship with
-any scrapers (or previously known as providers) by default, this is because v4
-is plugin-based and scrapers are now part of plugins that must be chosen to be
-installed. > Find out how to do so at the [wiki](https://github.com/mov-cli/
-mov-cli/wiki#plugins). 1. Install the scraper plugin of your choice. Visit this
-[wiki page](https://github.com/mov-cli/mov-cli/wiki/Plugins) on how to do so
-and the [mov-cli-plugin](https://github.com/topics/mov-cli-plugin) topic for a
-list of **third-party** mov-cli plugins. ```sh mov-cli -e ``` Alternatively,
-you may also edit by manually opening the config file. See this [Wiki page]
-(https://github.com/mov-cli/mov-cli/wiki/Configuration#introduction) on that.
-```toml [mov-cli.plugins] youtube = "mov-cli-youtube" ``` 2. Scrape away! ```sh
-mov-cli -s youtube flight 370 ``` [https://github.com/mov-cli/mov-cli/assets/
-132799819/8ccbd4b9-16d7-44cd-af8c-f788da1d5118]> The command above searches for
-`flight 370` with our [youtube](https://github.com/mov-cli/mov-cli-youtube)
-plugin, **however once again mov-cli is plugin based and there are many of them
-[in the wild](https://github.com/topics/mov-cli-plugin). ð** ## Star Graph
-â­ [![Star Graph Chart](https://api.star-history.com/svg?repos=mov-cli/mov-
-cli&type=Date)](https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing
-â¨ Pull requests are welcome and *appreciated*. For major changes, please open
-an issue first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/
-_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-
-cli](https://github.com/pystardust/ani-cli), [lobster](https://github.com/
-justchokingaround/lobster) and [animdl](https://github.com/justfoolingaround/
-animdl) [contributors-shield]: https://img.shields.io/github/contributors/mov-
-cli/mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-
-cli/mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
-forks/mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/
-mov-cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
+plugins up to date**. Also, I would advise not using it as a library yet as the
+API still has many breaking changes. ## What is mov-cli? ð« mov-cli is a
+command line tool that streamlines the process of streaming media from the
+comfort of your terminal; ~~*so you can show off to your friends the
+superiority of the command line.*~~ ðª The tool is sort of a framework that
+handles metadata and configuration, then simply invokes your media player. mov-
+cli [is **not** a piracy tool](./disclaimer.md); in fact, we encourage the
+opposite through the existence of our plugins [mov-cli-fs](https://github.com/
+mov-cli/mov-cli-files) and [mov-cli-media-server](https://github.com/mov-cli/
+mov-cli-ms). ð«µ You obtain the media. You pick the plugins. ## Installation
+ð ï¸ > [!TIP] > For in-depth installation instructions hit the [wiki](https:
+//github.com/mov-cli/mov-cli/wiki/Installation). ### Prerequisites - **A
+supported platform:** - Linux - Windows - Android (via [Termux](https://
+termux.dev/en/)) - *iOS (via [iSH Shell](https://ish.app/))* (unstable, https:/
+/github.com/mov-cli/mov-cli/issues/256) - MacOS - **[python](https://
+www.python.org/downloads/)** (**required**, with pip) - **[lxml](https://
+pypi.org/project/lxml/)** (optional, â¡ faster scraping) - **[fzf](https://
+github.com/junegunn/fzf?tab=readme-ov-file#installation)** (optional but
+**highly recommended**) - **[mpv](https://mpv.io/installation/)** (recommended
+& default media player) To get running these are all the prerequisites you'll
+need. With the prerequisites installed, mov-cli can be installed via the pip
+command on all platforms with Python version 3.8 or above. ```sh pip install
+mov-cli -U ``` > Check out the [wiki on installation](https://github.com/mov-
+cli/mov-cli/wiki/Installation) for more in-depth guidance on installing mov-
+cli. ## Usage ð±ï¸ mov-cli comes packaged with a CLI interface via the `mov-
+cli` command you can use in your respective terminal. > [!NOTE] > You may
+notice mov-cli doesn't ship with any scrapers (or previously known as
+providers) by default, this is because v4 is plugin-based and scrapers are now
+part of plugins that must be chosen to be installed. > Find out how to do so at
+the [wiki](https://github.com/mov-cli/mov-cli/wiki#plugins). 1. Install the
+scraper plugin of your choice. Visit this [wiki page](https://github.com/mov-
+cli/mov-cli/wiki/Plugins) on how to do so and the [mov-cli-plugin](https://
+github.com/topics/mov-cli-plugin) topic for a list of **third-party** mov-cli
+plugins. ```sh mov-cli -e ``` Alternatively, you may also edit by manually
+opening the config file. See this [Wiki page](https://github.com/mov-cli/mov-
+cli/wiki/Configuration#introduction) on that. ```toml [mov-cli.plugins] youtube
+= "mov-cli-youtube" ``` 2. Scrape away! ```sh mov-cli -s youtube flight 370 ```
+[https://github.com/mov-cli/mov-cli/assets/132799819/8ccbd4b9-16d7-44cd-af8c-
+f788da1d5118]> The command above searches for `flight 370` with our [youtube]
+(https://github.com/mov-cli/mov-cli-youtube) plugin, **however once again mov-
+cli is plugin based and there are many of them [in the wild](https://
+github.com/topics/mov-cli-plugin). ð** ## Star Graph â­ [![Star Graph
+Chart](https://api.star-history.com/svg?repos=mov-cli/mov-cli&type=Date)]
+(https://star-history.com/#mov-cli/mov-cli&Date) ## Contributing â¨ Pull
+requests are welcome and *appreciated*. For major changes, please open an issue
+first to discuss what you would like to change. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/
+_i_m_a_g_e_?_r_e_p_o_=_m_o_v_-_c_l_i_/_m_o_v_-_c_l_i_]## Inspiration ð Inspired by [ani-cli](https://
+github.com/pystardust/ani-cli), [lobster](https://github.com/justchokingaround/
+lobster) and [animdl](https://github.com/justfoolingaround/animdl)
+[contributors-shield]: https://img.shields.io/github/contributors/mov-cli/mov-
+cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/mov-
+cli/graphs/contributors [forks-shield]: https://img.shields.io/github/forks/
+mov-cli/mov-cli.svg?style=for-the-badge [forks-url]: https://github.com/mov-
+cli/mov-cli/network/members [stars-shield]: https://img.shields.io/github/
 stars/mov-cli/mov-cli?style=flat [stars-url]: https://github.com/mov-cli/mov-
 cli/stargazers [pypi-shield]: https://img.shields.io/pypi/v/mov-cli?style=flat
 [pypi-url]: https://pypi.org/project/mov-cli/ [pypi-stats-url]: https://
 pypistats.org/packages/mov-cli [python-shield]: https://img.shields.io/pypi/
 pyversions/mov-cli?style=flat [issues-shield]: https://img.shields.io/github/
 issues/mov-cli/mov-cli?style=flat [issues-url]: https://github.com/mov-cli/mov-
 cli/issues [license-shield]: https://img.shields.io/github/license/mov-cli/mov-
```

### Comparing `mov_cli-4.4a2/mov_cli.egg-info/SOURCES.txt` & `mov_cli-4.4a3/mov_cli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 LICENSE
 Makefile
 README.md
 disclaimer.md
 pyproject.toml
 ruff.toml
 .github/dependabot.yml
-.github/ISSUE_TEMPLATE/addprovider.md
-.github/ISSUE_TEMPLATE/bug-report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
 .github/workflows/pypi.yml
 .github/workflows/ruff.yml
 mov_cli/__init__.py
 mov_cli/config.py
 mov_cli/config.template.toml
@@ -40,14 +38,15 @@
 mov_cli/cli/ui.py
 mov_cli/cli/watch_options.py
 mov_cli/iterfzf/LICENSE.txt
 mov_cli/iterfzf/__init__.py
 mov_cli/media/__init__.py
 mov_cli/media/media.py
 mov_cli/media/metadata.py
+mov_cli/media/quality.py
 mov_cli/players/__init__.py
 mov_cli/players/custom_player.py
 mov_cli/players/iina.py
 mov_cli/players/mpv.py
 mov_cli/players/player.py
 mov_cli/players/syncplay.py
 mov_cli/players/vlc.py
```

### Comparing `mov_cli-4.4a2/pyproject.toml` & `mov_cli-4.4a3/pyproject.toml`

 * *Files identical despite different names*

