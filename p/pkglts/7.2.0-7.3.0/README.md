# Comparing `tmp/pkglts-7.2.0.tar.gz` & `tmp/pkglts-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkglts-7.2.0.tar", last modified: Wed Jan 10 10:43:07 2024, max compression
+gzip compressed data, was "pkglts-7.3.0.tar", last modified: Fri May 17 09:24:08 2024, max compression
```

## Comparing `pkglts-7.2.0.tar` & `pkglts-7.3.0.tar`

### file list

```diff
@@ -1,511 +1,511 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.848439 pkglts-7.2.0/
--rw-rw-rw-   0        0        0      538 2024-01-10 10:36:22.000000 pkglts-7.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3465 2024-01-10 10:36:22.000000 pkglts-7.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      167 2024-01-10 10:36:22.000000 pkglts-7.2.0/HISTORY.rst
--rw-rw-rw-   0        0        0    22406 2024-01-10 10:36:22.000000 pkglts-7.2.0/LICENSE
--rw-rw-rw-   0        0        0     6366 2024-01-10 10:43:07.847457 pkglts-7.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3741 2024-01-10 10:36:22.000000 pkglts-7.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.472962 pkglts-7.2.0/doc/
--rw-rw-rw-   0        0        0     6967 2024-01-10 10:36:23.000000 pkglts-7.2.0/doc/Makefile
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.474962 pkglts-7.2.0/doc/_notebook/
--rw-rw-rw-   0        0        0      754 2018-08-05 08:23:37.000000 pkglts-7.2.0/doc/_notebook/example.rst
--rw-rw-rw-   0        0        0       97 2018-08-05 07:42:43.000000 pkglts-7.2.0/doc/_notebook/index.rst
--rw-rw-rw-   0        0        0       29 2024-01-03 15:24:39.000000 pkglts-7.2.0/doc/authors.rst
--rw-rw-rw-   0        0        0     4272 2024-01-10 10:36:23.000000 pkglts-7.2.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2024-01-03 15:24:39.000000 pkglts-7.2.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-01-03 15:24:39.000000 pkglts-7.2.0/doc/history.rst
--rw-rw-rw-   0        0        0      420 2024-01-03 15:24:39.000000 pkglts-7.2.0/doc/index.rst
--rw-rw-rw-   0        0        0      694 2024-01-03 15:24:39.000000 pkglts-7.2.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2024-01-10 10:36:23.000000 pkglts-7.2.0/doc/make.bat
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.390587 pkglts-7.2.0/doc/option/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.474962 pkglts-7.2.0/doc/option/base/
--rw-rw-rw-   0        0        0     1778 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/base/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.475962 pkglts-7.2.0/doc/option/conda/
--rw-rw-rw-   0        0        0      621 2018-08-01 07:30:08.000000 pkglts-7.2.0/doc/option/conda/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.476962 pkglts-7.2.0/doc/option/coverage/
--rw-rw-rw-   0        0        0     2179 2024-01-03 14:05:39.000000 pkglts-7.2.0/doc/option/coverage/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.478962 pkglts-7.2.0/doc/option/coveralls/
--rw-rw-rw-   0        0        0     1766 2017-01-03 08:51:05.000000 pkglts-7.2.0/doc/option/coveralls/coveralls_tutorial.rst
--rw-rw-rw-   0        0        0      972 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/coveralls/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.480963 pkglts-7.2.0/doc/option/data/
--rw-rw-rw-   0        0        0     1150 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/data/data_tutorial.rst
--rw-rw-rw-   0        0        0      329 2017-01-03 08:51:05.000000 pkglts-7.2.0/doc/option/data/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.482964 pkglts-7.2.0/doc/option/doc/
--rw-rw-rw-   0        0        0      533 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/doc/history.rst
--rw-rw-rw-   0        0        0     2053 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/doc/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.483962 pkglts-7.2.0/doc/option/flake8/
--rw-rw-rw-   0        0        0      474 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/flake8/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.484962 pkglts-7.2.0/doc/option/git/
--rw-rw-rw-   0        0        0      400 2018-02-15 07:33:01.000000 pkglts-7.2.0/doc/option/git/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.486962 pkglts-7.2.0/doc/option/github/
--rw-rw-rw-   0        0        0     2785 2017-01-03 08:51:05.000000 pkglts-7.2.0/doc/option/github/github_tutorial.rst
--rw-rw-rw-   0        0        0      451 2018-02-15 07:33:01.000000 pkglts-7.2.0/doc/option/github/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.487962 pkglts-7.2.0/doc/option/gitlab/
--rw-rw-rw-   0        0        0     2627 2018-02-15 07:33:01.000000 pkglts-7.2.0/doc/option/gitlab/gitlab_tutorial.rst
--rw-rw-rw-   0        0        0      402 2018-02-15 07:33:01.000000 pkglts-7.2.0/doc/option/gitlab/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.489961 pkglts-7.2.0/doc/option/landscape/
--rw-rw-rw-   0        0        0     1207 2017-01-03 08:51:05.000000 pkglts-7.2.0/doc/option/landscape/landscape_tutorial.rst
--rw-rw-rw-   0        0        0     1006 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/landscape/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.490962 pkglts-7.2.0/doc/option/lgtm/
--rw-rw-rw-   0        0        0      557 2019-10-30 07:39:24.000000 pkglts-7.2.0/doc/option/lgtm/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.491961 pkglts-7.2.0/doc/option/license/
--rw-rw-rw-   0        0        0     7038 2019-10-29 19:00:47.000000 pkglts-7.2.0/doc/option/license/license_list.rst
--rw-rw-rw-   0        0        0      932 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/license/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.493962 pkglts-7.2.0/doc/option/notebook/
--rw-rw-rw-   0        0        0      913 2023-10-18 08:30:00.000000 pkglts-7.2.0/doc/option/notebook/main.rst
--rw-rw-rw-   0        0        0      861 2023-10-18 08:30:00.000000 pkglts-7.2.0/doc/option/notebook/nbcompile.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.494962 pkglts-7.2.0/doc/option/plugin_project/
--rw-rw-rw-   0        0        0     1080 2017-07-15 20:09:55.000000 pkglts-7.2.0/doc/option/plugin_project/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.496961 pkglts-7.2.0/doc/option/pypi/
--rw-rw-rw-   0        0        0      343 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/pypi/main.rst
--rw-rw-rw-   0        0        0     3642 2023-10-18 08:22:50.000000 pkglts-7.2.0/doc/option/pypi/pypi_tutorial.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.497965 pkglts-7.2.0/doc/option/pyproject/
--rw-rw-rw-   0        0        0      174 2024-01-03 14:05:39.000000 pkglts-7.2.0/doc/option/pyproject/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.499962 pkglts-7.2.0/doc/option/readthedocs/
--rw-rw-rw-   0        0        0      723 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/readthedocs/main.rst
--rw-rw-rw-   0        0        0     2223 2024-01-10 10:23:30.000000 pkglts-7.2.0/doc/option/readthedocs/readthedocs_tutorial.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.501963 pkglts-7.2.0/doc/option/reqs/
--rw-rw-rw-   0        0        0      887 2024-01-03 14:05:39.000000 pkglts-7.2.0/doc/option/reqs/main.rst
--rw-rw-rw-   0        0        0      365 2024-01-03 14:05:39.000000 pkglts-7.2.0/doc/option/reqs/reqs_tool.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.503963 pkglts-7.2.0/doc/option/requires/
--rw-rw-rw-   0        0        0      743 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/requires/main.rst
--rw-rw-rw-   0        0        0     1117 2018-02-15 07:33:01.000000 pkglts-7.2.0/doc/option/requires/requires_tutorial.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.504962 pkglts-7.2.0/doc/option/sphinx/
--rw-rw-rw-   0        0        0     1233 2023-10-18 08:33:06.000000 pkglts-7.2.0/doc/option/sphinx/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.504962 pkglts-7.2.0/doc/option/test/
--rw-rw-rw-   0        0        0     1056 2023-10-18 08:34:50.000000 pkglts-7.2.0/doc/option/test/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.505963 pkglts-7.2.0/doc/option/tox/
--rw-rw-rw-   0        0        0      700 2024-01-03 14:05:39.000000 pkglts-7.2.0/doc/option/tox/main.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.507962 pkglts-7.2.0/doc/option/travis/
--rw-rw-rw-   0        0        0      519 2021-05-27 13:53:46.000000 pkglts-7.2.0/doc/option/travis/main.rst
--rw-rw-rw-   0        0        0     2089 2021-05-27 13:53:46.000000 pkglts-7.2.0/doc/option/travis/travis_tutorial.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.508962 pkglts-7.2.0/doc/option/version/
--rw-rw-rw-   0        0        0      421 2018-08-05 08:23:37.000000 pkglts-7.2.0/doc/option/version/bump.rst
--rw-rw-rw-   0        0        0      556 2018-02-27 09:14:53.000000 pkglts-7.2.0/doc/option/version/main.rst
--rw-rw-rw-   0        0        0     2236 2024-01-03 14:05:39.000000 pkglts-7.2.0/doc/option_list.rst
--rw-rw-rw-   0        0        0     5884 2024-01-03 17:26:23.000000 pkglts-7.2.0/doc/readme.rst
--rw-rw-rw-   0        0        0      320 2024-01-03 14:05:39.000000 pkglts-7.2.0/doc/tool_list.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.513963 pkglts-7.2.0/doc/tutorial/
--rw-rw-rw-   0        0        0      668 2017-01-03 08:51:05.000000 pkglts-7.2.0/doc/tutorial/dvlpt_env.rst
--rw-rw-rw-   0        0        0      468 2017-01-03 08:51:05.000000 pkglts-7.2.0/doc/tutorial/migration.rst
--rw-rw-rw-   0        0        0     1147 2024-01-03 17:26:23.000000 pkglts-7.2.0/doc/tutorial/pypi.rst
--rw-rw-rw-   0        0        0      635 2017-01-03 08:51:05.000000 pkglts-7.2.0/doc/tutorial/web_tools.rst
--rw-rw-rw-   0        0        0      739 2023-10-18 08:17:17.000000 pkglts-7.2.0/doc/tutorials.rst
--rw-rw-rw-   0        0        0     1117 2024-01-03 15:24:39.000000 pkglts-7.2.0/doc/usage.rst
--rw-rw-rw-   0        0        0     4881 2024-01-10 10:36:23.000000 pkglts-7.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      338 2024-01-10 10:36:22.000000 pkglts-7.2.0/requirements.txt
--rw-rw-rw-   0        0        0       81 2024-01-10 10:36:22.000000 pkglts-7.2.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0       42 2024-01-10 10:43:07.848439 pkglts-7.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.391587 pkglts-7.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.531507 pkglts-7.2.0/src/pkglts/
--rw-rw-rw-   0        0        0      183 2024-01-10 10:36:23.000000 pkglts-7.2.0/src/pkglts/__init__.py
--rw-rw-rw-   0        0        0      202 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/config.py
--rw-rw-rw-   0        0        0    13039 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/config_management.py
--rw-rw-rw-   0        0        0     5526 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/dependency.py
--rw-rw-rw-   0        0        0      407 2019-08-27 13:00:03.000000 pkglts-7.2.0/src/pkglts/file_management.py
--rw-rw-rw-   0        0        0     2754 2019-11-13 12:35:41.000000 pkglts-7.2.0/src/pkglts/hash_management.py
--rw-rw-rw-   0        0        0     1427 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/local.py
--rw-rw-rw-   0        0        0     1634 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/logging_tools.py
--rw-rw-rw-   0        0        0     8162 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/manage.py
--rw-rw-rw-   0        0        0     7395 2020-10-22 13:45:14.000000 pkglts-7.2.0/src/pkglts/manage_script.py
--rw-rw-rw-   0        0        0     4113 2021-07-07 13:18:45.000000 pkglts-7.2.0/src/pkglts/manage_tools.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.540143 pkglts-7.2.0/src/pkglts/option/
--rw-rw-rw-   0        0        0       45 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.542143 pkglts-7.2.0/src/pkglts/option/appveyor/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/appveyor/__init__.py
--rw-rw-rw-   0        0        0     1169 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/appveyor/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.543147 pkglts-7.2.0/src/pkglts/option/appveyor/resource/
--rw-rw-rw-   0        0        0     1119 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/appveyor/resource/appveyor.yml
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.545143 pkglts-7.2.0/src/pkglts/option/base/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/base/__init__.py
--rw-rw-rw-   0        0        0     1310 2023-03-16 10:21:50.000000 pkglts-7.2.0/src/pkglts/option/base/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.547142 pkglts-7.2.0/src/pkglts/option/conda/
--rw-rw-rw-   0        0        0       20 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/conda/__init__.py
--rw-rw-rw-   0        0        0     1272 2024-01-03 19:05:21.000000 pkglts-7.2.0/src/pkglts/option/conda/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.394587 pkglts-7.2.0/src/pkglts/option/conda/resource/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.550142 pkglts-7.2.0/src/pkglts/option/conda/resource/conda/
--rw-rw-rw-   0        0        0     1087 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/conda/resource/conda/meta.yaml
--rw-rw-rw-   0        0        0      839 2024-01-10 08:19:45.000000 pkglts-7.2.0/src/pkglts/option/conda/resource/conda/requirements.yml
--rw-rw-rw-   0        0        0      681 2024-01-10 08:20:06.000000 pkglts-7.2.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.552143 pkglts-7.2.0/src/pkglts/option/coverage/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/coverage/__init__.py
--rw-rw-rw-   0        0        0      616 2023-03-16 10:29:48.000000 pkglts-7.2.0/src/pkglts/option/coverage/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.553143 pkglts-7.2.0/src/pkglts/option/coverage/resource/
--rw-rw-rw-   0        0        0      367 2018-06-06 09:43:05.000000 pkglts-7.2.0/src/pkglts/option/coverage/resource/.coveragerc
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.555142 pkglts-7.2.0/src/pkglts/option/coveralls/
--rw-rw-rw-   0        0        0       24 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/coveralls/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/coveralls/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.556142 pkglts-7.2.0/src/pkglts/option/data/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.399587 pkglts-7.2.0/src/pkglts/option/data/example/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.398586 pkglts-7.2.0/src/pkglts/option/data/example/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.561144 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png
--rw-rw-rw-   0        0        0       13 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.ui
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.564074 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.ui
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.568074 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.ui
--rw-rw-rw-   0        0        0      365 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/list_data.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.572074 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/
--rw-rw-rw-   0        0        0        0 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/__init__.py.tpl
--rw-rw-rw-   0        0        0   342163 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.txt
--rw-rw-rw-   0        0        0       11 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.ui
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.576075 pkglts-7.2.0/src/pkglts/option/data/example/test/
--rw-rw-rw-   0        0        0      538 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
--rw-rw-rw-   0        0        0      296 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/example/test/{% if not data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
--rw-rw-rw-   0        0        0      608 2023-03-16 10:29:48.000000 pkglts-7.2.0/src/pkglts/option/data/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.400587 pkglts-7.2.0/src/pkglts/option/data/resource/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.401588 pkglts-7.2.0/src/pkglts/option/data/resource/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.577074 pkglts-7.2.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
--rw-rw-rw-   0        0        0        0 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.578074 pkglts-7.2.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0     1500 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.581073 pkglts-7.2.0/src/pkglts/option/doc/
--rw-rw-rw-   0        0        0        0 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/doc/__init__.py
--rw-rw-rw-   0        0        0      987 2024-01-03 17:05:10.000000 pkglts-7.2.0/src/pkglts/option/doc/badge.py
--rw-rw-rw-   0        0        0     5564 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/doc/history.py
--rw-rw-rw-   0        0        0     1776 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/doc/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.590957 pkglts-7.2.0/src/pkglts/option/doc/resource/
--rw-rw-rw-   0        0        0      418 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}AUTHORS{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0     4509 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0       70 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}HISTORY{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0      175 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}README{% else %}_{% endif %}.md
--rw-rw-rw-   0        0        0      377 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}mkdocs{% else %}_{% endif %}.yml
--rw-rw-rw-   0        0        0      431 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}AUTHORS{% else %}_{% endif %}.rst
--rw-rw-rw-   0        0        0     4710 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst
--rw-rw-rw-   0        0        0      109 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}HISTORY{% else %}_{% endif %}.rst
--rw-rw-rw-   0        0        0      209 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}README{% else %}_{% endif %}.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.594006 pkglts-7.2.0/src/pkglts/option/flake8/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/flake8/__init__.py
--rw-rw-rw-   0        0        0      520 2023-03-16 10:29:48.000000 pkglts-7.2.0/src/pkglts/option/flake8/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.595003 pkglts-7.2.0/src/pkglts/option/flake8/resource/
--rw-rw-rw-   0        0        0      165 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/flake8/resource/.flake8
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.596003 pkglts-7.2.0/src/pkglts/option/git/
--rw-rw-rw-   0        0        0       18 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/git/__init__.py
--rw-rw-rw-   0        0        0     1492 2024-01-03 17:09:57.000000 pkglts-7.2.0/src/pkglts/option/git/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.597003 pkglts-7.2.0/src/pkglts/option/git/resource/
--rw-rw-rw-   0        0        0     1580 2021-03-03 16:14:09.000000 pkglts-7.2.0/src/pkglts/option/git/resource/.gitignore
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.599003 pkglts-7.2.0/src/pkglts/option/github/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/github/__init__.py
--rw-rw-rw-   0        0        0      905 2023-03-16 10:29:48.000000 pkglts-7.2.0/src/pkglts/option/github/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.601003 pkglts-7.2.0/src/pkglts/option/gitlab/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/gitlab/__init__.py
--rw-rw-rw-   0        0        0      950 2023-03-16 10:29:47.000000 pkglts-7.2.0/src/pkglts/option/gitlab/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.603409 pkglts-7.2.0/src/pkglts/option/landscape/
--rw-rw-rw-   0        0        0       24 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/landscape/__init__.py
--rw-rw-rw-   0        0        0      868 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/landscape/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.604076 pkglts-7.2.0/src/pkglts/option/landscape/resource/
--rw-rw-rw-   0        0        0      323 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/landscape/resource/.landscape.yml
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.605917 pkglts-7.2.0/src/pkglts/option/lgtm/
--rw-rw-rw-   0        0        0       19 2019-10-30 07:39:24.000000 pkglts-7.2.0/src/pkglts/option/lgtm/__init__.py
--rw-rw-rw-   0        0        0      938 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/lgtm/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.609116 pkglts-7.2.0/src/pkglts/option/license/
--rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/license/__init__.py
--rw-rw-rw-   0        0        0     1879 2023-03-16 10:29:48.000000 pkglts-7.2.0/src/pkglts/option/license/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.609417 pkglts-7.2.0/src/pkglts/option/license/resource/
--rw-rw-rw-   0        0        0       49 2020-03-17 18:25:54.000000 pkglts-7.2.0/src/pkglts/option/license/resource/LICENSE.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.657221 pkglts-7.2.0/src/pkglts/option/license/templates/
--rw-rw-rw-   0        0        0      741 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/agpl3-header.txt
--rw-rw-rw-   0        0        0    35211 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/agpl3.txt
--rw-rw-rw-   0        0        0      596 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/apache-header.txt
--rw-rw-rw-   0        0        0    11131 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/apache.txt
--rw-rw-rw-   0        0        0     1373 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/bsd2.txt
--rw-rw-rw-   0        0        0     1585 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/bsd3.txt
--rw-rw-rw-   0        0        0      389 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc0-header.txt
--rw-rw-rw-   0        0        0     7169 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc0.txt
--rw-rw-rw-   0        0        0      316 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by-header.txt
--rw-rw-rw-   0        0        0    19785 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by.txt
--rw-rw-rw-   0        0        0      333 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc-header.txt
--rw-rw-rw-   0        0        0    20812 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc.txt
--rw-rw-rw-   0        0        0      345 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc_nd-header.txt
--rw-rw-rw-   0        0        0    18957 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt
--rw-rw-rw-   0        0        0      347 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc_sa-header.txt
--rw-rw-rw-   0        0        0    22669 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt
--rw-rw-rw-   0        0        0      328 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nd-header.txt
--rw-rw-rw-   0        0        0    17942 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nd.txt
--rw-rw-rw-   0        0        0      330 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_sa-header.txt
--rw-rw-rw-   0        0        0    22597 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_sa.txt
--rw-rw-rw-   0        0        0    17650 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cddl.txt
--rw-rw-rw-   0        0        0     1527 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cecill-c-header.txt
--rw-rw-rw-   0        0        0    22380 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/cecill-c.txt
--rw-rw-rw-   0        0        0    11840 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/epl.txt
--rw-rw-rw-   0        0        0    18173 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/gpl2.txt
--rw-rw-rw-   0        0        0      720 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/gpl3-header.txt
--rw-rw-rw-   0        0        0    35864 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/gpl3.txt
--rw-rw-rw-   0        0        0     6426 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/inra_license_agreement.txt
--rw-rw-rw-   0        0        0      778 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/isc.txt
--rw-rw-rw-   0        0        0     7777 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/lgpl.txt
--rw-rw-rw-   0        0        0     1103 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/mit.txt
--rw-rw-rw-   0        0        0      196 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/mpl-header.txt
--rw-rw-rw-   0        0        0    16078 2017-05-18 09:15:38.000000 pkglts-7.2.0/src/pkglts/option/license/templates/mpl.txt
--rw-rw-rw-   0        0        0     9475 2020-04-14 06:55:23.000000 pkglts-7.2.0/src/pkglts/option/license/templates/private.txt
--rw-rw-rw-   0        0        0     1235 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/unlicense.txt
--rw-rw-rw-   0        0        0      301 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/wtfpl-header-warranty.txt
--rw-rw-rw-   0        0        0      301 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/wtfpl-header.txt
--rw-rw-rw-   0        0        0      515 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/wtfpl.txt
--rw-rw-rw-   0        0        0     1444 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/x11.txt
--rw-rw-rw-   0        0        0      919 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/license/templates/zlib.txt
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.661205 pkglts-7.2.0/src/pkglts/option/notebook/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/notebook/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.409587 pkglts-7.2.0/src/pkglts/option/notebook/example/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.662206 pkglts-7.2.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/
--rw-rw-rw-   0        0        0    17056 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb
--rw-rw-rw-   0        0        0     4449 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/notebook/nbcompile.py
--rw-rw-rw-   0        0        0      933 2023-03-16 10:29:47.000000 pkglts-7.2.0/src/pkglts/option/notebook/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.663793 pkglts-7.2.0/src/pkglts/option/plugin_project/
--rw-rw-rw-   0        0        0       49 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/plugin_project/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.411587 pkglts-7.2.0/src/pkglts/option/plugin_project/example/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.411587 pkglts-7.2.0/src/pkglts/option/plugin_project/example/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.411587 pkglts-7.2.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.665794 pkglts-7.2.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/
--rw-rw-rw-   0        0        0       83 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_file.txt
--rw-rw-rw-   0        0        0       92 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_script.py.tpl
--rw-rw-rw-   0        0        0     1093 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/plugin_project/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.666417 pkglts-7.2.0/src/pkglts/option/plugin_project/resource/
--rw-rw-rw-   0        0        0      208 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/plugin_project/resource/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.413586 pkglts-7.2.0/src/pkglts/option/plugin_project/resource/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.668467 pkglts-7.2.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0     1021 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.671500 pkglts-7.2.0/src/pkglts/option/pypi/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/pypi/__init__.py
--rw-rw-rw-   0        0        0     2902 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/pypi/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.672468 pkglts-7.2.0/src/pkglts/option/pypi/resource/
--rw-rw-rw-   0        0        0      290 2020-04-15 06:02:11.000000 pkglts-7.2.0/src/pkglts/option/pypi/resource/.pypirc
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.674466 pkglts-7.2.0/src/pkglts/option/pyproject/
--rw-rw-rw-   0        0        0       24 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/pyproject/__init__.py
--rw-rw-rw-   0        0        0     1978 2024-01-03 17:05:10.000000 pkglts-7.2.0/src/pkglts/option/pyproject/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.675466 pkglts-7.2.0/src/pkglts/option/pyproject/resource/
--rw-rw-rw-   0        0        0     2406 2024-01-05 13:51:55.000000 pkglts-7.2.0/src/pkglts/option/pyproject/resource/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.676466 pkglts-7.2.0/src/pkglts/option/readthedocs/
--rw-rw-rw-   0        0        0       26 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/readthedocs/__init__.py
--rw-rw-rw-   0        0        0     1809 2024-01-10 10:33:45.000000 pkglts-7.2.0/src/pkglts/option/readthedocs/option.py
--rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-7.2.0/src/pkglts/option/regenerate.no
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.680466 pkglts-7.2.0/src/pkglts/option/reqs/
--rw-rw-rw-   0        0        0       56 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/reqs/__init__.py
--rw-rw-rw-   0        0        0     2563 2023-04-26 14:57:35.000000 pkglts-7.2.0/src/pkglts/option/reqs/find_requirements.py
--rw-rw-rw-   0        0        0     3927 2024-01-03 18:59:32.000000 pkglts-7.2.0/src/pkglts/option/reqs/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.682467 pkglts-7.2.0/src/pkglts/option/reqs/resource/
--rw-rw-rw-   0        0        0      319 2020-04-15 06:18:47.000000 pkglts-7.2.0/src/pkglts/option/reqs/resource/requirements.txt
--rw-rw-rw-   0        0        0      136 2020-04-15 06:18:47.000000 pkglts-7.2.0/src/pkglts/option/reqs/resource/requirements_minimal.txt
--rw-rw-rw-   0        0        0     2100 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/reqs/stdpkgs.txt
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.684467 pkglts-7.2.0/src/pkglts/option/requires/
--rw-rw-rw-   0        0        0       23 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/requires/__init__.py
--rw-rw-rw-   0        0        0      928 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/requires/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.688467 pkglts-7.2.0/src/pkglts/option/sphinx/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/sphinx/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.421587 pkglts-7.2.0/src/pkglts/option/sphinx/example/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.689467 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.704408 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/
--rw-rw-rw-   0        0        0      312 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/autodoc.rst
--rw-rw-rw-   0        0        0      358 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/autosummary.rst
--rw-rw-rw-   0        0        0      385 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/graphviz.rst
--rw-rw-rw-   0        0        0      468 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/ifconfig.rst
--rw-rw-rw-   0        0        0      221 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/index.rst
--rw-rw-rw-   0        0        0      823 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst
--rw-rw-rw-   0        0        0      631 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst
--rw-rw-rw-   0        0        0      364 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/math.rst
--rw-rw-rw-   0        0        0      665 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst
--rw-rw-rw-   0        0        0      441 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/todo.rst
--rw-rw-rw-   0        0        0      344 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/viewcode.rst
--rw-rw-rw-   0        0        0      443 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/workflow.dot
--rw-rw-rw-   0        0        0      493 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/index.rst
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.421587 pkglts-7.2.0/src/pkglts/option/sphinx/example/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.707408 pkglts-7.2.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0      742 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl
--rw-rw-rw-   0        0        0      110 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance1.py.tpl
--rw-rw-rw-   0        0        0       82 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance2.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.708409 pkglts-7.2.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/
--rw-rw-rw-   0        0        0      109 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/README.rst
--rw-rw-rw-   0        0        0      297 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/plot_smth.py
--rw-rw-rw-   0        0        0     1568 2024-01-10 10:34:06.000000 pkglts-7.2.0/src/pkglts/option/sphinx/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.422587 pkglts-7.2.0/src/pkglts/option/sphinx/resource/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.712409 pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/
--rw-rw-rw-   0        0        0     6967 2021-03-01 14:25:42.000000 pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.713409 pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/
--rw-rw-rw-   0        0        0        0 2021-03-01 14:25:42.000000 pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/nonempty.txt
--rw-rw-rw-   0        0        0     5827 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl
--rwxrwxrwx   0        0        0     6731 2021-03-01 14:25:42.000000 pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.714409 pkglts-7.2.0/src/pkglts/option/src/
--rw-rw-rw-   0        0        0       58 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/src/__init__.py
--rw-rw-rw-   0        0        0      961 2023-03-16 10:29:48.000000 pkglts-7.2.0/src/pkglts/option/src/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.423587 pkglts-7.2.0/src/pkglts/option/src/resource/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.424587 pkglts-7.2.0/src/pkglts/option/src/resource/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.717425 pkglts-7.2.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0      109 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.720410 pkglts-7.2.0/src/pkglts/option/test/
--rw-rw-rw-   0        0        0       19 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.426587 pkglts-7.2.0/src/pkglts/option/test/example/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.425587 pkglts-7.2.0/src/pkglts/option/test/example/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.721410 pkglts-7.2.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0      497 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/example.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.723409 pkglts-7.2.0/src/pkglts/option/test/example/test/
--rw-rw-rw-   0        0        0      285 2018-04-08 21:39:40.000000 pkglts-7.2.0/src/pkglts/option/test/example/test/__init__.py.tpl
--rw-rw-rw-   0        0        0     1521 2018-02-15 07:33:01.000000 pkglts-7.2.0/src/pkglts/option/test/example/test/test_example.py.tpl
--rw-rw-rw-   0        0        0     1209 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/test/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.724409 pkglts-7.2.0/src/pkglts/option/test/resource/
--rw-rw-rw-   0        0        0      233 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/test/resource/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.725408 pkglts-7.2.0/src/pkglts/option/test/resource/test/
--rw-rw-rw-   0        0        0     1086 2023-04-17 13:15:22.000000 pkglts-7.2.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.726413 pkglts-7.2.0/src/pkglts/option/tox/
--rw-rw-rw-   0        0        0       18 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/tox/__init__.py
--rw-rw-rw-   0        0        0      541 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/tox/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.727409 pkglts-7.2.0/src/pkglts/option/tox/resource/
--rw-rw-rw-   0        0        0      463 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/tox/resource/tox.ini
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.729409 pkglts-7.2.0/src/pkglts/option/travis/
--rw-rw-rw-   0        0        0       21 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/travis/__init__.py
--rw-rw-rw-   0        0        0      890 2024-01-03 15:08:32.000000 pkglts-7.2.0/src/pkglts/option/travis/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.731409 pkglts-7.2.0/src/pkglts/option/travis/resource/
--rw-rw-rw-   0        0        0     1748 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/option/travis/resource/.travis.yml
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.734694 pkglts-7.2.0/src/pkglts/option/version/
--rw-rw-rw-   0        0        0       22 2018-02-27 09:14:53.000000 pkglts-7.2.0/src/pkglts/option/version/__init__.py
--rw-rw-rw-   0        0        0     1652 2021-07-07 13:18:45.000000 pkglts-7.2.0/src/pkglts/option/version/bump_version.py
--rw-rw-rw-   0        0        0     1179 2023-03-16 10:29:50.000000 pkglts-7.2.0/src/pkglts/option/version/option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.429587 pkglts-7.2.0/src/pkglts/option/version/resource/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.430593 pkglts-7.2.0/src/pkglts/option/version/resource/src/
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.737727 pkglts-7.2.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0       99 2019-10-29 06:16:57.000000 pkglts-7.2.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/__init__.py.tpl
--rw-rw-rw-   0        0        0      420 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/version.py.tpl
--rw-rw-rw-   0        0        0     2876 2021-07-07 13:18:45.000000 pkglts-7.2.0/src/pkglts/option_object.py
--rw-rw-rw-   0        0        0     1496 2024-01-03 17:19:46.000000 pkglts-7.2.0/src/pkglts/option_tools.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.738710 pkglts-7.2.0/src/pkglts/resource/
--rw-rw-rw-   0        0        0      395 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/resource/namespace__init__.py.tpl
--rw-rw-rw-   0        0        0     4731 2020-04-15 05:36:21.000000 pkglts-7.2.0/src/pkglts/small_tools.py
--rw-rw-rw-   0        0        0     7461 2024-01-03 14:05:39.000000 pkglts-7.2.0/src/pkglts/templating.py
--rw-rw-rw-   0        0        0     1710 2019-10-29 22:35:37.000000 pkglts-7.2.0/src/pkglts/tree_ascii_fmt.py
--rw-rw-rw-   0        0        0      367 2024-01-10 10:36:23.000000 pkglts-7.2.0/src/pkglts/version.py
--rw-rw-rw-   0        0        0     2169 2021-07-07 13:18:45.000000 pkglts-7.2.0/src/pkglts/version_management.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.846440 pkglts-7.2.0/src/pkglts.egg-info/
--rw-rw-rw-   0        0        0     6366 2024-01-10 10:43:07.000000 pkglts-7.2.0/src/pkglts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    16202 2024-01-10 10:43:07.000000 pkglts-7.2.0/src/pkglts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 10:43:07.000000 pkglts-7.2.0/src/pkglts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1430 2024-01-10 10:43:07.000000 pkglts-7.2.0/src/pkglts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      161 2024-01-10 10:43:07.000000 pkglts-7.2.0/src/pkglts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-01-10 10:43:07.000000 pkglts-7.2.0/src/pkglts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.761661 pkglts-7.2.0/test/
--rw-rw-rw-   0        0        0      982 2024-01-10 10:36:23.000000 pkglts-7.2.0/test/conftest.py
--rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-7.2.0/test/info.rst
--rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-7.2.0/test/regenerate.no
--rw-rw-rw-   0        0        0     3421 2020-04-15 05:45:06.000000 pkglts-7.2.0/test/test_config_management.py
--rw-rw-rw-   0        0        0     4791 2019-10-29 06:16:57.000000 pkglts-7.2.0/test/test_dependency.py
--rw-rw-rw-   0        0        0      340 2019-10-29 06:16:57.000000 pkglts-7.2.0/test/test_file_management.py
--rw-rw-rw-   0        0        0     1956 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_hash_management.py
--rw-rw-rw-   0        0        0      731 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_local.py
--rw-rw-rw-   0        0        0      315 2018-02-15 07:33:01.000000 pkglts-7.2.0/test/test_manage.py
--rw-rw-rw-   0        0        0     3051 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_manage_cfg.py
--rw-rw-rw-   0        0        0     1787 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_manage_clean.py
--rw-rw-rw-   0        0        0     2774 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_manage_example.py
--rw-rw-rw-   0        0        0     4454 2020-02-06 18:02:24.000000 pkglts-7.2.0/test/test_manage_regenerate.py
--rw-rw-rw-   0        0        0     1848 2020-10-22 13:45:14.000000 pkglts-7.2.0/test/test_manage_reset.py
--rw-rw-rw-   0        0        0      299 2019-10-29 06:16:57.000000 pkglts-7.2.0/test/test_manage_tools_check_option_parameters.py
--rw-rw-rw-   0        0        0     5217 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_manage_tools_regenerate.py
--rw-rw-rw-   0        0        0     2126 2020-02-06 18:02:24.000000 pkglts-7.2.0/test/test_manage_tools_update_option.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.764685 pkglts-7.2.0/test/test_option/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.767659 pkglts-7.2.0/test/test_option/test_appveyor/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_appveyor/__init__.py
--rw-rw-rw-   0        0        0      714 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_appveyor/test_config.py
--rw-rw-rw-   0        0        0      322 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_appveyor/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.770659 pkglts-7.2.0/test/test_option/test_base/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_base/__init__.py
--rw-rw-rw-   0        0        0     1338 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_base/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.772662 pkglts-7.2.0/test/test_option/test_conda/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_conda/__init__.py
--rw-rw-rw-   0        0        0     1074 2023-01-19 13:13:37.000000 pkglts-7.2.0/test/test_option/test_conda/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.775663 pkglts-7.2.0/test/test_option/test_coverage/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_coverage/__init__.py
--rw-rw-rw-   0        0        0      620 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_coverage/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.782680 pkglts-7.2.0/test/test_option/test_coveralls/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_coveralls/__init__.py
--rw-rw-rw-   0        0        0      458 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_coveralls/test_config.py
--rw-rw-rw-   0        0        0      309 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_coveralls/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.784662 pkglts-7.2.0/test/test_option/test_data/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_data/__init__.py
--rw-rw-rw-   0        0        0      547 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_data/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.788664 pkglts-7.2.0/test/test_option/test_doc/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_doc/__init__.py
--rw-rw-rw-   0        0        0      587 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_doc/test_badge.py
--rw-rw-rw-   0        0        0     1431 2024-01-03 15:00:39.000000 pkglts-7.2.0/test/test_option/test_doc/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.791622 pkglts-7.2.0/test/test_option/test_flake8/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_flake8/__init__.py
--rw-rw-rw-   0        0        0      446 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_flake8/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.795141 pkglts-7.2.0/test/test_option/test_git/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_git/__init__.py
--rw-rw-rw-   0        0        0      646 2022-03-25 13:56:41.000000 pkglts-7.2.0/test/test_option/test_git/test_config.py
--rw-rw-rw-   0        0        0      676 2024-01-03 14:05:39.000000 pkglts-7.2.0/test/test_option/test_git/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.797754 pkglts-7.2.0/test/test_option/test_github/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_github/__init__.py
--rw-rw-rw-   0        0        0      718 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_github/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.798769 pkglts-7.2.0/test/test_option/test_gitlab/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_gitlab/__init__.py
--rw-rw-rw-   0        0        0      732 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_gitlab/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.801769 pkglts-7.2.0/test/test_option/test_landscape/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_landscape/__init__.py
--rw-rw-rw-   0        0        0      458 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_landscape/test_config.py
--rw-rw-rw-   0        0        0      309 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_landscape/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.805534 pkglts-7.2.0/test/test_option/test_lgtm/
--rw-rw-rw-   0        0        0        0 2019-10-30 07:39:24.000000 pkglts-7.2.0/test/test_option/test_lgtm/__init__.py
--rw-rw-rw-   0        0        0      438 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_lgtm/test_config.py
--rw-rw-rw-   0        0        0      294 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_lgtm/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.808740 pkglts-7.2.0/test/test_option/test_license/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_license/__init__.py
--rw-rw-rw-   0        0        0      950 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_license/test_config.py
--rw-rw-rw-   0        0        0      590 2017-07-15 20:09:55.000000 pkglts-7.2.0/test/test_option/test_license/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.810753 pkglts-7.2.0/test/test_option/test_notebook/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_notebook/__init__.py
--rw-rw-rw-   0        0        0     1063 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_notebook/test_config.py
--rw-rw-rw-   0        0        0     2059 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_option_common.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.812754 pkglts-7.2.0/test/test_option/test_plugin_project/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_plugin_project/__init__.py
--rw-rw-rw-   0        0        0     1002 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_plugin_project/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.814753 pkglts-7.2.0/test/test_option/test_pypi/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_pypi/__init__.py
--rw-rw-rw-   0        0        0      692 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_pypi/test_config.py
--rw-rw-rw-   0        0        0     1143 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_pypi/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.817753 pkglts-7.2.0/test/test_option/test_pyproject/
--rw-rw-rw-   0        0        0        0 2024-01-03 14:05:39.000000 pkglts-7.2.0/test/test_option/test_pyproject/__init__.py
--rw-rw-rw-   0        0        0      744 2024-01-03 14:05:39.000000 pkglts-7.2.0/test/test_option/test_pyproject/test_config.py
--rw-rw-rw-   0        0        0     2485 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_pyproject/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.820872 pkglts-7.2.0/test/test_option/test_readthedocs/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_readthedocs/__init__.py
--rw-rw-rw-   0        0        0      744 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_readthedocs/test_config.py
--rw-rw-rw-   0        0        0      242 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_readthedocs/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.825433 pkglts-7.2.0/test/test_option/test_reqs/
--rw-rw-rw-   0        0        0        0 2019-10-29 06:16:57.000000 pkglts-7.2.0/test/test_option/test_reqs/__init__.py
--rw-rw-rw-   0        0        0     2231 2021-12-09 14:39:11.000000 pkglts-7.2.0/test/test_option/test_reqs/test_config.py
--rw-rw-rw-   0        0        0     1849 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_option/test_reqs/test_find_requirements.py
--rw-rw-rw-   0        0        0      529 2019-10-29 22:35:37.000000 pkglts-7.2.0/test/test_option/test_reqs/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.828442 pkglts-7.2.0/test/test_option/test_requires/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_requires/__init__.py
--rw-rw-rw-   0        0        0      454 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_requires/test_config.py
--rw-rw-rw-   0        0        0      306 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_requires/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.830441 pkglts-7.2.0/test/test_option/test_sphinx/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_sphinx/__init__.py
--rw-rw-rw-   0        0        0     1197 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_sphinx/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.833441 pkglts-7.2.0/test/test_option/test_src/
--rw-rw-rw-   0        0        0        0 2019-10-29 06:16:57.000000 pkglts-7.2.0/test/test_option/test_src/__init__.py
--rw-rw-rw-   0        0        0      690 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_src/test_config.py
--rw-rw-rw-   0        0        0      284 2019-10-29 06:16:57.000000 pkglts-7.2.0/test/test_option/test_src/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.835441 pkglts-7.2.0/test/test_option/test_test/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_test/__init__.py
--rw-rw-rw-   0        0        0      842 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_test/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.837464 pkglts-7.2.0/test/test_option/test_tox/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_tox/__init__.py
--rw-rw-rw-   0        0        0      434 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_tox/test_config.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.841454 pkglts-7.2.0/test/test_option/test_travis/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_travis/__init__.py
--rw-rw-rw-   0        0        0      446 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_travis/test_config.py
--rw-rw-rw-   0        0        0      300 2024-01-03 15:08:32.000000 pkglts-7.2.0/test/test_option/test_travis/test_handlers.py
-drwxrwxrwx   0        0        0        0 2024-01-10 10:43:07.844441 pkglts-7.2.0/test/test_option/test_version/
--rw-rw-rw-   0        0        0        0 2018-11-08 07:37:33.000000 pkglts-7.2.0/test/test_option/test_version/__init__.py
--rw-rw-rw-   0        0        0     1335 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_option/test_version/test_config.py
--rw-rw-rw-   0        0        0      527 2020-02-06 18:02:24.000000 pkglts-7.2.0/test/test_option/test_version/test_handlers.py
--rw-rw-rw-   0        0        0     2527 2020-02-06 18:02:24.000000 pkglts-7.2.0/test/test_option_tools.py
--rw-rw-rw-   0        0        0     2694 2018-06-09 22:55:54.000000 pkglts-7.2.0/test/test_templating.py
--rw-rw-rw-   0        0        0     2110 2021-07-07 13:18:45.000000 pkglts-7.2.0/test/test_version_management.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.402893 pkglts-7.3.0/
+-rw-rw-rw-   0        0        0      538 2024-05-17 08:57:52.000000 pkglts-7.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3465 2024-05-17 08:57:52.000000 pkglts-7.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      167 2024-05-17 08:57:52.000000 pkglts-7.3.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    22406 2024-05-17 08:57:52.000000 pkglts-7.3.0/LICENSE
+-rw-rw-rw-   0        0        0     6366 2024-05-17 09:24:08.402893 pkglts-7.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3741 2024-05-17 08:57:52.000000 pkglts-7.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.929646 pkglts-7.3.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-17 08:57:52.000000 pkglts-7.3.0/doc/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.931647 pkglts-7.3.0/doc/_notebook/
+-rw-rw-rw-   0        0        0      754 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/_notebook/example.rst
+-rw-rw-rw-   0        0        0       97 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/_notebook/index.rst
+-rw-rw-rw-   0        0        0       29 2024-01-03 15:24:39.000000 pkglts-7.3.0/doc/authors.rst
+-rw-rw-rw-   0        0        0     4272 2024-05-17 08:57:52.000000 pkglts-7.3.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-01-03 15:24:39.000000 pkglts-7.3.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-01-03 15:24:39.000000 pkglts-7.3.0/doc/history.rst
+-rw-rw-rw-   0        0        0      420 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/index.rst
+-rw-rw-rw-   0        0        0      694 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-17 08:57:52.000000 pkglts-7.3.0/doc/make.bat
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.836374 pkglts-7.3.0/doc/option/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.933647 pkglts-7.3.0/doc/option/base/
+-rw-rw-rw-   0        0        0     1778 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/base/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.933647 pkglts-7.3.0/doc/option/conda/
+-rw-rw-rw-   0        0        0      621 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/conda/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.935646 pkglts-7.3.0/doc/option/coverage/
+-rw-rw-rw-   0        0        0     2179 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/coverage/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.937661 pkglts-7.3.0/doc/option/coveralls/
+-rw-rw-rw-   0        0        0     1766 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/coveralls/coveralls_tutorial.rst
+-rw-rw-rw-   0        0        0      972 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/coveralls/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.941647 pkglts-7.3.0/doc/option/data/
+-rw-rw-rw-   0        0        0     1150 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/data/data_tutorial.rst
+-rw-rw-rw-   0        0        0      329 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/data/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.943647 pkglts-7.3.0/doc/option/doc/
+-rw-rw-rw-   0        0        0      533 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/doc/history.rst
+-rw-rw-rw-   0        0        0     2053 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/doc/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.943647 pkglts-7.3.0/doc/option/flake8/
+-rw-rw-rw-   0        0        0      474 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/flake8/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.943647 pkglts-7.3.0/doc/option/git/
+-rw-rw-rw-   0        0        0      400 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/git/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.947740 pkglts-7.3.0/doc/option/github/
+-rw-rw-rw-   0        0        0     2785 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/github/github_tutorial.rst
+-rw-rw-rw-   0        0        0      451 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/github/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.949682 pkglts-7.3.0/doc/option/gitlab/
+-rw-rw-rw-   0        0        0     2627 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/gitlab/gitlab_tutorial.rst
+-rw-rw-rw-   0        0        0      402 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/gitlab/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.951681 pkglts-7.3.0/doc/option/landscape/
+-rw-rw-rw-   0        0        0     1207 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/landscape/landscape_tutorial.rst
+-rw-rw-rw-   0        0        0     1006 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/landscape/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.954062 pkglts-7.3.0/doc/option/lgtm/
+-rw-rw-rw-   0        0        0      557 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/lgtm/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.958195 pkglts-7.3.0/doc/option/license/
+-rw-rw-rw-   0        0        0     7038 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/license/license_list.rst
+-rw-rw-rw-   0        0        0      932 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/license/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.960250 pkglts-7.3.0/doc/option/notebook/
+-rw-rw-rw-   0        0        0      913 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/notebook/main.rst
+-rw-rw-rw-   0        0        0      861 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/notebook/nbcompile.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.960250 pkglts-7.3.0/doc/option/plugin_project/
+-rw-rw-rw-   0        0        0     1080 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/plugin_project/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.964234 pkglts-7.3.0/doc/option/pypi/
+-rw-rw-rw-   0        0        0      343 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/pypi/main.rst
+-rw-rw-rw-   0        0        0     3642 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/pypi/pypi_tutorial.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.964234 pkglts-7.3.0/doc/option/pyproject/
+-rw-rw-rw-   0        0        0      174 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/pyproject/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.966251 pkglts-7.3.0/doc/option/readthedocs/
+-rw-rw-rw-   0        0        0      723 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/readthedocs/main.rst
+-rw-rw-rw-   0        0        0     2223 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/readthedocs/readthedocs_tutorial.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.970233 pkglts-7.3.0/doc/option/reqs/
+-rw-rw-rw-   0        0        0      887 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/reqs/main.rst
+-rw-rw-rw-   0        0        0      365 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/reqs/reqs_tool.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.972195 pkglts-7.3.0/doc/option/requires/
+-rw-rw-rw-   0        0        0      743 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/requires/main.rst
+-rw-rw-rw-   0        0        0     1117 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/requires/requires_tutorial.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.974195 pkglts-7.3.0/doc/option/sphinx/
+-rw-rw-rw-   0        0        0     1233 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/sphinx/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.974195 pkglts-7.3.0/doc/option/test/
+-rw-rw-rw-   0        0        0     1056 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/test/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.976194 pkglts-7.3.0/doc/option/tox/
+-rw-rw-rw-   0        0        0      700 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/tox/main.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.978195 pkglts-7.3.0/doc/option/travis/
+-rw-rw-rw-   0        0        0      519 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/travis/main.rst
+-rw-rw-rw-   0        0        0     2089 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/travis/travis_tutorial.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.980202 pkglts-7.3.0/doc/option/version/
+-rw-rw-rw-   0        0        0      421 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/version/bump.rst
+-rw-rw-rw-   0        0        0      556 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option/version/main.rst
+-rw-rw-rw-   0        0        0     2236 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/option_list.rst
+-rw-rw-rw-   0        0        0     5884 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/readme.rst
+-rw-rw-rw-   0        0        0      320 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/tool_list.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.986263 pkglts-7.3.0/doc/tutorial/
+-rw-rw-rw-   0        0        0      668 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/tutorial/dvlpt_env.rst
+-rw-rw-rw-   0        0        0      468 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/tutorial/migration.rst
+-rw-rw-rw-   0        0        0     1147 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/tutorial/pypi.rst
+-rw-rw-rw-   0        0        0      635 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/tutorial/web_tools.rst
+-rw-rw-rw-   0        0        0      739 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/tutorials.rst
+-rw-rw-rw-   0        0        0     1117 2024-05-13 13:01:16.000000 pkglts-7.3.0/doc/usage.rst
+-rw-rw-rw-   0        0        0     4881 2024-05-17 08:57:52.000000 pkglts-7.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      338 2024-05-17 08:57:52.000000 pkglts-7.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       81 2024-05-17 08:57:52.000000 pkglts-7.3.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:24:08.404896 pkglts-7.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.838358 pkglts-7.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.005958 pkglts-7.3.0/src/pkglts/
+-rw-rw-rw-   0        0        0      183 2024-05-17 08:57:52.000000 pkglts-7.3.0/src/pkglts/__init__.py
+-rw-rw-rw-   0        0        0      202 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/config.py
+-rw-rw-rw-   0        0        0    13039 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/config_management.py
+-rw-rw-rw-   0        0        0     5526 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/dependency.py
+-rw-rw-rw-   0        0        0      407 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/file_management.py
+-rw-rw-rw-   0        0        0     2754 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/hash_management.py
+-rw-rw-rw-   0        0        0     1427 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/local.py
+-rw-rw-rw-   0        0        0     1634 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/logging_tools.py
+-rw-rw-rw-   0        0        0     8162 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/manage.py
+-rw-rw-rw-   0        0        0     7395 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/manage_script.py
+-rw-rw-rw-   0        0        0     4113 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/manage_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.014892 pkglts-7.3.0/src/pkglts/option/
+-rw-rw-rw-   0        0        0       45 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.016891 pkglts-7.3.0/src/pkglts/option/appveyor/
+-rw-rw-rw-   0        0        0       23 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/appveyor/__init__.py
+-rw-rw-rw-   0        0        0     1169 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/appveyor/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.018897 pkglts-7.3.0/src/pkglts/option/appveyor/resource/
+-rw-rw-rw-   0        0        0     1119 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/appveyor/resource/appveyor.yml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.020897 pkglts-7.3.0/src/pkglts/option/base/
+-rw-rw-rw-   0        0        0       19 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/base/__init__.py
+-rw-rw-rw-   0        0        0     1310 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/base/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.022895 pkglts-7.3.0/src/pkglts/option/conda/
+-rw-rw-rw-   0        0        0       20 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/conda/__init__.py
+-rw-rw-rw-   0        0        0     1272 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/conda/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.840356 pkglts-7.3.0/src/pkglts/option/conda/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.026894 pkglts-7.3.0/src/pkglts/option/conda/resource/conda/
+-rw-rw-rw-   0        0        0     1087 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/conda/resource/conda/meta.yaml
+-rw-rw-rw-   0        0        0      839 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/conda/resource/conda/requirements.yml
+-rw-rw-rw-   0        0        0      681 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.028893 pkglts-7.3.0/src/pkglts/option/coverage/
+-rw-rw-rw-   0        0        0       23 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/coverage/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/coverage/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.028893 pkglts-7.3.0/src/pkglts/option/coverage/resource/
+-rw-rw-rw-   0        0        0      367 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/coverage/resource/.coveragerc
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.030895 pkglts-7.3.0/src/pkglts/option/coveralls/
+-rw-rw-rw-   0        0        0       24 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/coveralls/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/coveralls/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.035050 pkglts-7.3.0/src/pkglts/option/data/
+-rw-rw-rw-   0        0        0       19 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.848356 pkglts-7.3.0/src/pkglts/option/data/example/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.848356 pkglts-7.3.0/src/pkglts/option/data/example/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.039050 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
+-rw-rw-rw-   0        0        0   342163 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png
+-rw-rw-rw-   0        0        0       13 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.ui
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.041418 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/
+-rw-rw-rw-   0        0        0   342163 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.ui
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.047454 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/
+-rw-rw-rw-   0        0        0   342163 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.ui
+-rw-rw-rw-   0        0        0      365 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/list_data.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.053456 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/__init__.py.tpl
+-rw-rw-rw-   0        0        0   342163 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.ui
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.055478 pkglts-7.3.0/src/pkglts/option/data/example/test/
+-rw-rw-rw-   0        0        0      538 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
+-rw-rw-rw-   0        0        0      296 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/example/test/{% if not data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl
+-rw-rw-rw-   0        0        0      608 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.850378 pkglts-7.3.0/src/pkglts/option/data/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.850378 pkglts-7.3.0/src/pkglts/option/data/resource/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.055478 pkglts-7.3.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/resource/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.055478 pkglts-7.3.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0     1500 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.061455 pkglts-7.3.0/src/pkglts/option/doc/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/__init__.py
+-rw-rw-rw-   0        0        0      987 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/badge.py
+-rw-rw-rw-   0        0        0     5564 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/history.py
+-rw-rw-rw-   0        0        0     1776 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.071467 pkglts-7.3.0/src/pkglts/option/doc/resource/
+-rw-rw-rw-   0        0        0      418 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}AUTHORS{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0     4509 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0       70 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}HISTORY{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0      175 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}README{% else %}_{% endif %}.md
+-rw-rw-rw-   0        0        0      377 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}mkdocs{% else %}_{% endif %}.yml
+-rw-rw-rw-   0        0        0      431 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}AUTHORS{% else %}_{% endif %}.rst
+-rw-rw-rw-   0        0        0     4710 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst
+-rw-rw-rw-   0        0        0      109 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}HISTORY{% else %}_{% endif %}.rst
+-rw-rw-rw-   0        0        0      209 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}README{% else %}_{% endif %}.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.074363 pkglts-7.3.0/src/pkglts/option/flake8/
+-rw-rw-rw-   0        0        0       21 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/flake8/__init__.py
+-rw-rw-rw-   0        0        0      520 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/flake8/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.075052 pkglts-7.3.0/src/pkglts/option/flake8/resource/
+-rw-rw-rw-   0        0        0      165 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/flake8/resource/.flake8
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.077295 pkglts-7.3.0/src/pkglts/option/git/
+-rw-rw-rw-   0        0        0       18 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/git/__init__.py
+-rw-rw-rw-   0        0        0     1492 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/git/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.078013 pkglts-7.3.0/src/pkglts/option/git/resource/
+-rw-rw-rw-   0        0        0     1596 2024-05-17 08:55:23.000000 pkglts-7.3.0/src/pkglts/option/git/resource/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.080028 pkglts-7.3.0/src/pkglts/option/github/
+-rw-rw-rw-   0        0        0       21 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/github/__init__.py
+-rw-rw-rw-   0        0        0      905 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/github/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.084031 pkglts-7.3.0/src/pkglts/option/gitlab/
+-rw-rw-rw-   0        0        0       21 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/gitlab/__init__.py
+-rw-rw-rw-   0        0        0      950 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/gitlab/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.088028 pkglts-7.3.0/src/pkglts/option/landscape/
+-rw-rw-rw-   0        0        0       24 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/landscape/__init__.py
+-rw-rw-rw-   0        0        0      868 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/landscape/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.088028 pkglts-7.3.0/src/pkglts/option/landscape/resource/
+-rw-rw-rw-   0        0        0      323 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/landscape/resource/.landscape.yml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.090031 pkglts-7.3.0/src/pkglts/option/lgtm/
+-rw-rw-rw-   0        0        0       19 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/lgtm/__init__.py
+-rw-rw-rw-   0        0        0      938 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/lgtm/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.092031 pkglts-7.3.0/src/pkglts/option/license/
+-rw-rw-rw-   0        0        0       22 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/__init__.py
+-rw-rw-rw-   0        0        0     1879 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.094838 pkglts-7.3.0/src/pkglts/option/license/resource/
+-rw-rw-rw-   0        0        0       49 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/resource/LICENSE.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.144989 pkglts-7.3.0/src/pkglts/option/license/templates/
+-rw-rw-rw-   0        0        0      741 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/agpl3-header.txt
+-rw-rw-rw-   0        0        0    35211 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/agpl3.txt
+-rw-rw-rw-   0        0        0      596 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/apache-header.txt
+-rw-rw-rw-   0        0        0    11131 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/apache.txt
+-rw-rw-rw-   0        0        0     1373 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/bsd2.txt
+-rw-rw-rw-   0        0        0     1585 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/bsd3.txt
+-rw-rw-rw-   0        0        0      389 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc0-header.txt
+-rw-rw-rw-   0        0        0     7169 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc0.txt
+-rw-rw-rw-   0        0        0      316 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by-header.txt
+-rw-rw-rw-   0        0        0    19785 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by.txt
+-rw-rw-rw-   0        0        0      333 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc-header.txt
+-rw-rw-rw-   0        0        0    20812 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc.txt
+-rw-rw-rw-   0        0        0      345 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc_nd-header.txt
+-rw-rw-rw-   0        0        0    18957 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt
+-rw-rw-rw-   0        0        0      347 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc_sa-header.txt
+-rw-rw-rw-   0        0        0    22669 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt
+-rw-rw-rw-   0        0        0      328 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nd-header.txt
+-rw-rw-rw-   0        0        0    17942 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nd.txt
+-rw-rw-rw-   0        0        0      330 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_sa-header.txt
+-rw-rw-rw-   0        0        0    22597 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_sa.txt
+-rw-rw-rw-   0        0        0    17650 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cddl.txt
+-rw-rw-rw-   0        0        0     1527 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cecill-c-header.txt
+-rw-rw-rw-   0        0        0    22380 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/cecill-c.txt
+-rw-rw-rw-   0        0        0    11840 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/epl.txt
+-rw-rw-rw-   0        0        0    18173 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/gpl2.txt
+-rw-rw-rw-   0        0        0      720 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/gpl3-header.txt
+-rw-rw-rw-   0        0        0    35864 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/gpl3.txt
+-rw-rw-rw-   0        0        0     6426 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/inra_license_agreement.txt
+-rw-rw-rw-   0        0        0      778 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/isc.txt
+-rw-rw-rw-   0        0        0     7777 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/lgpl.txt
+-rw-rw-rw-   0        0        0     1103 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/mit.txt
+-rw-rw-rw-   0        0        0      196 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/mpl-header.txt
+-rw-rw-rw-   0        0        0    16078 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/mpl.txt
+-rw-rw-rw-   0        0        0     9475 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/private.txt
+-rw-rw-rw-   0        0        0     1235 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/unlicense.txt
+-rw-rw-rw-   0        0        0      301 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/wtfpl-header-warranty.txt
+-rw-rw-rw-   0        0        0      301 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/wtfpl-header.txt
+-rw-rw-rw-   0        0        0      515 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/wtfpl.txt
+-rw-rw-rw-   0        0        0     1444 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/x11.txt
+-rw-rw-rw-   0        0        0      919 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/license/templates/zlib.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.148977 pkglts-7.3.0/src/pkglts/option/notebook/
+-rw-rw-rw-   0        0        0       23 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/notebook/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.858356 pkglts-7.3.0/src/pkglts/option/notebook/example/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.148977 pkglts-7.3.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/
+-rw-rw-rw-   0        0        0    17056 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb
+-rw-rw-rw-   0        0        0     4449 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/notebook/nbcompile.py
+-rw-rw-rw-   0        0        0      933 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/notebook/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.151012 pkglts-7.3.0/src/pkglts/option/plugin_project/
+-rw-rw-rw-   0        0        0       49 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/plugin_project/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.862359 pkglts-7.3.0/src/pkglts/option/plugin_project/example/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.862359 pkglts-7.3.0/src/pkglts/option/plugin_project/example/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.862359 pkglts-7.3.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.153045 pkglts-7.3.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/
+-rw-rw-rw-   0        0        0       83 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_file.txt
+-rw-rw-rw-   0        0        0       92 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/plugin_project/example/src/{{ base.pkgname }}/resource/extra_script.py.tpl
+-rw-rw-rw-   0        0        0     1093 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/plugin_project/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.154946 pkglts-7.3.0/src/pkglts/option/plugin_project/resource/
+-rw-rw-rw-   0        0        0      208 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/plugin_project/resource/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.864356 pkglts-7.3.0/src/pkglts/option/plugin_project/resource/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.154946 pkglts-7.3.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0     1021 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.160983 pkglts-7.3.0/src/pkglts/option/pypi/
+-rw-rw-rw-   0        0        0       19 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/pypi/__init__.py
+-rw-rw-rw-   0        0        0     2902 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/pypi/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.160983 pkglts-7.3.0/src/pkglts/option/pypi/resource/
+-rw-rw-rw-   0        0        0      290 2020-04-15 06:02:11.000000 pkglts-7.3.0/src/pkglts/option/pypi/resource/.pypirc
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.164987 pkglts-7.3.0/src/pkglts/option/pyproject/
+-rw-rw-rw-   0        0        0       24 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/pyproject/__init__.py
+-rw-rw-rw-   0        0        0     1978 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/pyproject/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.166947 pkglts-7.3.0/src/pkglts/option/pyproject/resource/
+-rw-rw-rw-   0        0        0     2406 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/pyproject/resource/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.171002 pkglts-7.3.0/src/pkglts/option/readthedocs/
+-rw-rw-rw-   0        0        0       26 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/readthedocs/__init__.py
+-rw-rw-rw-   0        0        0     1809 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/readthedocs/option.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/regenerate.no
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.176187 pkglts-7.3.0/src/pkglts/option/reqs/
+-rw-rw-rw-   0        0        0       56 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/reqs/__init__.py
+-rw-rw-rw-   0        0        0     2563 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/reqs/find_requirements.py
+-rw-rw-rw-   0        0        0     3927 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/reqs/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.178220 pkglts-7.3.0/src/pkglts/option/reqs/resource/
+-rw-rw-rw-   0        0        0      319 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/reqs/resource/requirements.txt
+-rw-rw-rw-   0        0        0      136 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/reqs/resource/requirements_minimal.txt
+-rw-rw-rw-   0        0        0     2100 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/reqs/stdpkgs.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.180189 pkglts-7.3.0/src/pkglts/option/requires/
+-rw-rw-rw-   0        0        0       23 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/requires/__init__.py
+-rw-rw-rw-   0        0        0      928 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/requires/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.182231 pkglts-7.3.0/src/pkglts/option/sphinx/
+-rw-rw-rw-   0        0        0       21 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.872355 pkglts-7.3.0/src/pkglts/option/sphinx/example/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.184234 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.198189 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/
+-rw-rw-rw-   0        0        0      312 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/autodoc.rst
+-rw-rw-rw-   0        0        0      358 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/autosummary.rst
+-rw-rw-rw-   0        0        0      385 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/graphviz.rst
+-rw-rw-rw-   0        0        0      468 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/ifconfig.rst
+-rw-rw-rw-   0        0        0      221 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/index.rst
+-rw-rw-rw-   0        0        0      823 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst
+-rw-rw-rw-   0        0        0      631 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst
+-rw-rw-rw-   0        0        0      364 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/math.rst
+-rw-rw-rw-   0        0        0      665 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst
+-rw-rw-rw-   0        0        0      441 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/todo.rst
+-rw-rw-rw-   0        0        0      344 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/viewcode.rst
+-rw-rw-rw-   0        0        0      443 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/workflow.dot
+-rw-rw-rw-   0        0        0      493 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/index.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.870355 pkglts-7.3.0/src/pkglts/option/sphinx/example/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.200191 pkglts-7.3.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0      742 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl
+-rw-rw-rw-   0        0        0      110 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance1.py.tpl
+-rw-rw-rw-   0        0        0       82 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_inheritance2.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.202187 pkglts-7.3.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/
+-rw-rw-rw-   0        0        0      109 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/README.rst
+-rw-rw-rw-   0        0        0      297 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/example/{{ sphinx.gallery  }}/plot_smth.py
+-rw-rw-rw-   0        0        0     1568 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.872355 pkglts-7.3.0/src/pkglts/option/sphinx/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.206193 pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/
+-rw-rw-rw-   0        0        0     6967 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.208188 pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/_static/nonempty.txt
+-rw-rw-rw-   0        0        0     5827 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl
+-rwxrwxrwx   0        0        0     6731 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.210189 pkglts-7.3.0/src/pkglts/option/src/
+-rw-rw-rw-   0        0        0       58 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/src/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/src/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.878357 pkglts-7.3.0/src/pkglts/option/src/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.878357 pkglts-7.3.0/src/pkglts/option/src/resource/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.210189 pkglts-7.3.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0      109 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/src/resource/src/{{ base.pkgname }}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.214187 pkglts-7.3.0/src/pkglts/option/test/
+-rw-rw-rw-   0        0        0       19 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.880357 pkglts-7.3.0/src/pkglts/option/test/example/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.880357 pkglts-7.3.0/src/pkglts/option/test/example/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.216187 pkglts-7.3.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0      497 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/test/example/src/{{ base.pkgname }}/example.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.219687 pkglts-7.3.0/src/pkglts/option/test/example/test/
+-rw-rw-rw-   0        0        0      285 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/test/example/test/__init__.py.tpl
+-rw-rw-rw-   0        0        0     1521 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/test/example/test/test_example.py.tpl
+-rw-rw-rw-   0        0        0     1209 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/test/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.221700 pkglts-7.3.0/src/pkglts/option/test/resource/
+-rw-rw-rw-   0        0        0      233 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/test/resource/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.223700 pkglts-7.3.0/src/pkglts/option/test/resource/test/
+-rw-rw-rw-   0        0        0     1086 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.225698 pkglts-7.3.0/src/pkglts/option/tox/
+-rw-rw-rw-   0        0        0       18 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/tox/__init__.py
+-rw-rw-rw-   0        0        0      541 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/tox/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.227701 pkglts-7.3.0/src/pkglts/option/tox/resource/
+-rw-rw-rw-   0        0        0      463 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/tox/resource/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.229700 pkglts-7.3.0/src/pkglts/option/travis/
+-rw-rw-rw-   0        0        0       21 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/travis/__init__.py
+-rw-rw-rw-   0        0        0      890 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/travis/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.231699 pkglts-7.3.0/src/pkglts/option/travis/resource/
+-rw-rw-rw-   0        0        0     1748 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/travis/resource/.travis.yml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.237701 pkglts-7.3.0/src/pkglts/option/version/
+-rw-rw-rw-   0        0        0       22 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/version/__init__.py
+-rw-rw-rw-   0        0        0     1652 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/version/bump_version.py
+-rw-rw-rw-   0        0        0     1179 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/version/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.884365 pkglts-7.3.0/src/pkglts/option/version/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:07.884365 pkglts-7.3.0/src/pkglts/option/version/resource/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.241699 pkglts-7.3.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0       99 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/__init__.py.tpl
+-rw-rw-rw-   0        0        0      420 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option/version/resource/src/{{ base.pkgname }}/version.py.tpl
+-rw-rw-rw-   0        0        0     2876 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option_object.py
+-rw-rw-rw-   0        0        0     1496 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/option_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.243702 pkglts-7.3.0/src/pkglts/resource/
+-rw-rw-rw-   0        0        0      395 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/resource/namespace__init__.py.tpl
+-rw-rw-rw-   0        0        0     4731 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/small_tools.py
+-rw-rw-rw-   0        0        0     7461 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/templating.py
+-rw-rw-rw-   0        0        0     1710 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/tree_ascii_fmt.py
+-rw-rw-rw-   0        0        0      367 2024-05-17 08:57:52.000000 pkglts-7.3.0/src/pkglts/version.py
+-rw-rw-rw-   0        0        0     2169 2024-05-13 13:01:16.000000 pkglts-7.3.0/src/pkglts/version_management.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.400920 pkglts-7.3.0/src/pkglts.egg-info/
+-rw-rw-rw-   0        0        0     6366 2024-05-17 09:24:07.000000 pkglts-7.3.0/src/pkglts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    16202 2024-05-17 09:24:07.000000 pkglts-7.3.0/src/pkglts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:24:07.000000 pkglts-7.3.0/src/pkglts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1430 2024-05-17 09:24:07.000000 pkglts-7.3.0/src/pkglts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      161 2024-05-17 09:24:07.000000 pkglts-7.3.0/src/pkglts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-17 09:24:07.000000 pkglts-7.3.0/src/pkglts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.291579 pkglts-7.3.0/test/
+-rw-rw-rw-   0        0        0      982 2024-05-17 08:57:52.000000 pkglts-7.3.0/test/conftest.py
+-rw-rw-rw-   0        0        0        0 2017-01-03 08:51:05.000000 pkglts-7.3.0/test/info.rst
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/regenerate.no
+-rw-rw-rw-   0        0        0     3421 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_config_management.py
+-rw-rw-rw-   0        0        0     4791 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_dependency.py
+-rw-rw-rw-   0        0        0      340 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_file_management.py
+-rw-rw-rw-   0        0        0     1956 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_hash_management.py
+-rw-rw-rw-   0        0        0      731 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_local.py
+-rw-rw-rw-   0        0        0      315 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage.py
+-rw-rw-rw-   0        0        0     3051 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_cfg.py
+-rw-rw-rw-   0        0        0     1787 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_clean.py
+-rw-rw-rw-   0        0        0     2774 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_example.py
+-rw-rw-rw-   0        0        0     4454 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_regenerate.py
+-rw-rw-rw-   0        0        0     1848 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_reset.py
+-rw-rw-rw-   0        0        0      299 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_tools_check_option_parameters.py
+-rw-rw-rw-   0        0        0     5217 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_tools_regenerate.py
+-rw-rw-rw-   0        0        0     2126 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_manage_tools_update_option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.294074 pkglts-7.3.0/test/test_option/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.302395 pkglts-7.3.0/test/test_option/test_appveyor/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_appveyor/__init__.py
+-rw-rw-rw-   0        0        0      714 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_appveyor/test_config.py
+-rw-rw-rw-   0        0        0      322 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_appveyor/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.306179 pkglts-7.3.0/test/test_option/test_base/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_base/__init__.py
+-rw-rw-rw-   0        0        0     1338 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_base/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.309654 pkglts-7.3.0/test/test_option/test_conda/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_conda/__init__.py
+-rw-rw-rw-   0        0        0     1074 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_conda/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.312366 pkglts-7.3.0/test/test_option/test_coverage/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_coverage/__init__.py
+-rw-rw-rw-   0        0        0      620 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_coverage/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.318398 pkglts-7.3.0/test/test_option/test_coveralls/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_coveralls/__init__.py
+-rw-rw-rw-   0        0        0      458 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_coveralls/test_config.py
+-rw-rw-rw-   0        0        0      309 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_coveralls/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.321070 pkglts-7.3.0/test/test_option/test_data/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_data/__init__.py
+-rw-rw-rw-   0        0        0      547 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_data/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.329218 pkglts-7.3.0/test/test_option/test_doc/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_doc/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_doc/test_badge.py
+-rw-rw-rw-   0        0        0     1431 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_doc/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.331210 pkglts-7.3.0/test/test_option/test_flake8/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_flake8/__init__.py
+-rw-rw-rw-   0        0        0      446 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_flake8/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.337209 pkglts-7.3.0/test/test_option/test_git/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_git/__init__.py
+-rw-rw-rw-   0        0        0      646 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_git/test_config.py
+-rw-rw-rw-   0        0        0      676 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_git/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.339209 pkglts-7.3.0/test/test_option/test_github/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_github/__init__.py
+-rw-rw-rw-   0        0        0      718 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_github/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.339209 pkglts-7.3.0/test/test_option/test_gitlab/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_gitlab/__init__.py
+-rw-rw-rw-   0        0        0      732 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_gitlab/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.343209 pkglts-7.3.0/test/test_option/test_landscape/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_landscape/__init__.py
+-rw-rw-rw-   0        0        0      458 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_landscape/test_config.py
+-rw-rw-rw-   0        0        0      309 2024-05-13 13:01:16.000000 pkglts-7.3.0/test/test_option/test_landscape/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.347815 pkglts-7.3.0/test/test_option/test_lgtm/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_lgtm/__init__.py
+-rw-rw-rw-   0        0        0      438 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_lgtm/test_config.py
+-rw-rw-rw-   0        0        0      294 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_lgtm/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.350881 pkglts-7.3.0/test/test_option/test_license/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_license/__init__.py
+-rw-rw-rw-   0        0        0      950 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_license/test_config.py
+-rw-rw-rw-   0        0        0      590 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_license/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.352901 pkglts-7.3.0/test/test_option/test_notebook/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_notebook/__init__.py
+-rw-rw-rw-   0        0        0     1063 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_notebook/test_config.py
+-rw-rw-rw-   0        0        0     2059 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_option_common.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.356896 pkglts-7.3.0/test/test_option/test_plugin_project/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_plugin_project/__init__.py
+-rw-rw-rw-   0        0        0     1002 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_plugin_project/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.362896 pkglts-7.3.0/test/test_option/test_pypi/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_pypi/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_pypi/test_config.py
+-rw-rw-rw-   0        0        0     1143 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_pypi/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.366896 pkglts-7.3.0/test/test_option/test_pyproject/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_pyproject/__init__.py
+-rw-rw-rw-   0        0        0      744 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_pyproject/test_config.py
+-rw-rw-rw-   0        0        0     2485 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_pyproject/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.370895 pkglts-7.3.0/test/test_option/test_readthedocs/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_readthedocs/__init__.py
+-rw-rw-rw-   0        0        0      744 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_readthedocs/test_config.py
+-rw-rw-rw-   0        0        0      242 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_readthedocs/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.374895 pkglts-7.3.0/test/test_option/test_reqs/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_reqs/__init__.py
+-rw-rw-rw-   0        0        0     2231 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_reqs/test_config.py
+-rw-rw-rw-   0        0        0     1849 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_reqs/test_find_requirements.py
+-rw-rw-rw-   0        0        0      529 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_reqs/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.380933 pkglts-7.3.0/test/test_option/test_requires/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_requires/__init__.py
+-rw-rw-rw-   0        0        0      454 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_requires/test_config.py
+-rw-rw-rw-   0        0        0      306 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_requires/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.382894 pkglts-7.3.0/test/test_option/test_sphinx/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_sphinx/__init__.py
+-rw-rw-rw-   0        0        0     1197 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_sphinx/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.386896 pkglts-7.3.0/test/test_option/test_src/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_src/__init__.py
+-rw-rw-rw-   0        0        0      690 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_src/test_config.py
+-rw-rw-rw-   0        0        0      284 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_src/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.388895 pkglts-7.3.0/test/test_option/test_test/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_test/__init__.py
+-rw-rw-rw-   0        0        0      842 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_test/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.390914 pkglts-7.3.0/test/test_option/test_tox/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_tox/__init__.py
+-rw-rw-rw-   0        0        0      434 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_tox/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.396895 pkglts-7.3.0/test/test_option/test_travis/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_travis/__init__.py
+-rw-rw-rw-   0        0        0      446 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_travis/test_config.py
+-rw-rw-rw-   0        0        0      300 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_travis/test_handlers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:24:08.400920 pkglts-7.3.0/test/test_option/test_version/
+-rw-rw-rw-   0        0        0        0 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_version/__init__.py
+-rw-rw-rw-   0        0        0     1335 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_version/test_config.py
+-rw-rw-rw-   0        0        0      527 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option/test_version/test_handlers.py
+-rw-rw-rw-   0        0        0     2527 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_option_tools.py
+-rw-rw-rw-   0        0        0     2694 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_templating.py
+-rw-rw-rw-   0        0        0     2110 2024-05-13 13:01:17.000000 pkglts-7.3.0/test/test_version_management.py
```

### Comparing `pkglts-7.2.0/AUTHORS.rst` & `pkglts-7.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/CONTRIBUTING.rst` & `pkglts-7.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/LICENSE` & `pkglts-7.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/PKG-INFO` & `pkglts-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkglts
-Version: 7.2.0
+Version: 7.3.0
 Summary: Building packages with long term support
 Author-email: revesansparole <revesansparole@gmail.com>
 Maintainer-email: revesansparole <revesansparole@gmail.com>, ThT12 <ThT12@ThT12.fr>, pradal <christophe.pradal@inria.fr>, egarciaitk <emilien.garcia@itk.fr>, Simon Artzet <simon.artzet@gmail.com>, lquibel <lucie.quibel@itk.fr>, Christophe Pradal <christophe.pradal@inria.fr>, Samuel Andres <samuel.andres@itk.fr>
 License: CeCILL-C
 Project-URL: repository, https://github.com/revesansparole/pkglts
 Project-URL: appveyor, https://ci.appveyor.com/project/revesansparole/pkglts/branch/master
 Project-URL: coveralls, https://coveralls.io/github/revesansparole/pkglts?branch=master
```

### Comparing `pkglts-7.2.0/README.rst` & `pkglts-7.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/Makefile` & `pkglts-7.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/_notebook/example.rst` & `pkglts-7.3.0/doc/_notebook/example.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/conf.py` & `pkglts-7.3.0/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "7.2.0"
+version = "7.3.0"
 # The full version, including alpha/beta/rc tags.
-release = "7.2.0"
+release = "7.3.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `pkglts-7.2.0/doc/installation.rst` & `pkglts-7.3.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/make.bat` & `pkglts-7.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/base/main.rst` & `pkglts-7.3.0/doc/option/base/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/conda/main.rst` & `pkglts-7.3.0/doc/option/conda/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/coverage/main.rst` & `pkglts-7.3.0/doc/option/coverage/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/coveralls/coveralls_tutorial.rst` & `pkglts-7.3.0/doc/option/coveralls/coveralls_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/coveralls/main.rst` & `pkglts-7.3.0/doc/option/coveralls/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/data/data_tutorial.rst` & `pkglts-7.3.0/doc/option/data/data_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/doc/history.rst` & `pkglts-7.3.0/doc/option/doc/history.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/doc/main.rst` & `pkglts-7.3.0/doc/option/doc/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/github/github_tutorial.rst` & `pkglts-7.3.0/doc/option/github/github_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/gitlab/gitlab_tutorial.rst` & `pkglts-7.3.0/doc/option/gitlab/gitlab_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/landscape/landscape_tutorial.rst` & `pkglts-7.3.0/doc/option/landscape/landscape_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/landscape/main.rst` & `pkglts-7.3.0/doc/option/landscape/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/lgtm/main.rst` & `pkglts-7.3.0/doc/option/lgtm/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/license/license_list.rst` & `pkglts-7.3.0/doc/option/license/license_list.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/license/main.rst` & `pkglts-7.3.0/doc/option/license/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/notebook/main.rst` & `pkglts-7.3.0/doc/option/notebook/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/notebook/nbcompile.rst` & `pkglts-7.3.0/doc/option/notebook/nbcompile.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/plugin_project/main.rst` & `pkglts-7.3.0/doc/option/plugin_project/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/pypi/pypi_tutorial.rst` & `pkglts-7.3.0/doc/option/pypi/pypi_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/readthedocs/main.rst` & `pkglts-7.3.0/doc/option/readthedocs/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/readthedocs/readthedocs_tutorial.rst` & `pkglts-7.3.0/doc/option/readthedocs/readthedocs_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/reqs/main.rst` & `pkglts-7.3.0/doc/option/reqs/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/requires/main.rst` & `pkglts-7.3.0/doc/option/requires/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/requires/requires_tutorial.rst` & `pkglts-7.3.0/doc/option/requires/requires_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/sphinx/main.rst` & `pkglts-7.3.0/doc/option/sphinx/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/test/main.rst` & `pkglts-7.3.0/doc/option/test/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/tox/main.rst` & `pkglts-7.3.0/doc/option/tox/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/travis/main.rst` & `pkglts-7.3.0/doc/option/travis/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/travis/travis_tutorial.rst` & `pkglts-7.3.0/doc/option/travis/travis_tutorial.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option/version/main.rst` & `pkglts-7.3.0/doc/option/version/main.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/option_list.rst` & `pkglts-7.3.0/doc/option_list.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/readme.rst` & `pkglts-7.3.0/doc/readme.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/tutorial/dvlpt_env.rst` & `pkglts-7.3.0/doc/tutorial/dvlpt_env.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/tutorial/pypi.rst` & `pkglts-7.3.0/doc/tutorial/pypi.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/tutorial/web_tools.rst` & `pkglts-7.3.0/doc/tutorial/web_tools.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/tutorials.rst` & `pkglts-7.3.0/doc/tutorials.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/doc/usage.rst` & `pkglts-7.3.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/pyproject.toml` & `pkglts-7.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 requires = ["setuptools", "wheel"]  # , "setuptools-scm"]  # PEP 508 specifications.
 build-backend = "setuptools.build_meta"  # we don't know if we need it
 # #}
 
 # {# pkglts, pyproject.project
 [project]  # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 name = "pkglts"
-version = "7.2.0"
+version = "7.3.0"
 description = "Building packages with long term support"
 readme = "README.rst"
 requires-python = ">= 3.6"
 license = {text = "CeCILL-C"}
 authors = [
     {name = "revesansparole", email = "revesansparole@gmail.com"},
 ]
```

### Comparing `pkglts-7.2.0/src/pkglts/config_management.py` & `pkglts-7.3.0/src/pkglts/config_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/dependency.py` & `pkglts-7.3.0/src/pkglts/dependency.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/hash_management.py` & `pkglts-7.3.0/src/pkglts/hash_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/local.py` & `pkglts-7.3.0/src/pkglts/local.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/logging_tools.py` & `pkglts-7.3.0/src/pkglts/logging_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/manage.py` & `pkglts-7.3.0/src/pkglts/manage.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/manage_script.py` & `pkglts-7.3.0/src/pkglts/manage_script.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/manage_tools.py` & `pkglts-7.3.0/src/pkglts/manage_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/appveyor/option.py` & `pkglts-7.3.0/src/pkglts/option/appveyor/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/appveyor/resource/appveyor.yml` & `pkglts-7.3.0/src/pkglts/option/appveyor/resource/appveyor.yml`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/base/option.py` & `pkglts-7.3.0/src/pkglts/option/base/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/conda/option.py` & `pkglts-7.3.0/src/pkglts/option/conda/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/conda/resource/conda/meta.yaml` & `pkglts-7.3.0/src/pkglts/option/conda/resource/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/conda/resource/conda/requirements.yml` & `pkglts-7.3.0/src/pkglts/option/conda/resource/conda/requirements.yml`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml` & `pkglts-7.3.0/src/pkglts/option/conda/resource/conda/requirements_minimal.yml`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/coverage/option.py` & `pkglts-7.3.0/src/pkglts/option/coverage/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/coveralls/option.py` & `pkglts-7.3.0/src/pkglts/option/coveralls/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png` & `pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/ext_data.png`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png` & `pkglts-7.3.0/src/pkglts/option/data/example/src/{% if data.use_ext_dir %}{{ base.pkgname }}_data{% endif %}/sub/sub_ext_data.png`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png` & `pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/data.png`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png` & `pkglts-7.3.0/src/pkglts/option/data/example/src/{% if not data.use_ext_dir %}{{ base.pkgname }}{% endif %}/sub/sub_data.png`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl` & `pkglts-7.3.0/src/pkglts/option/data/example/test/{% if data.use_ext_dir %}test_data{% else %}_{% endif %}.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/data/option.py` & `pkglts-7.3.0/src/pkglts/option/data/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl` & `pkglts-7.3.0/src/pkglts/option/data/resource/src/{{ base.pkgname }}/{% if data.use_ext_dir %}data_access{% else %}_{% endif %}.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/doc/badge.py` & `pkglts-7.3.0/src/pkglts/option/doc/badge.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/doc/history.py` & `pkglts-7.3.0/src/pkglts/option/doc/history.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/doc/option.py` & `pkglts-7.3.0/src/pkglts/option/doc/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md` & `pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'md' %}CONTRIBUTING{% else %}_{% endif %}.md`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst` & `pkglts-7.3.0/src/pkglts/option/doc/resource/{% if doc.fmt == 'rst' %}CONTRIBUTING{% else %}_{% endif %}.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/flake8/option.py` & `pkglts-7.3.0/src/pkglts/option/flake8/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/git/option.py` & `pkglts-7.3.0/src/pkglts/option/git/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/git/resource/.gitignore` & `pkglts-7.3.0/src/pkglts/option/git/resource/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,16 @@
 
 {%- if 'sphinx' is available %}
 # sphinx autogen file
 {{ sphinx.doc_dir }}/build/
 {{ sphinx.doc_dir }}/_dvlpt/
 {% if sphinx.gallery != "" -%}
 doc/_gallery/
+doc/sg_*.rst
+
 {% endif -%}
 {% endif %}
 
 # #}
 
 # user custom filters
```

### Comparing `pkglts-7.2.0/src/pkglts/option/github/option.py` & `pkglts-7.3.0/src/pkglts/option/github/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/gitlab/option.py` & `pkglts-7.3.0/src/pkglts/option/gitlab/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/landscape/option.py` & `pkglts-7.3.0/src/pkglts/option/landscape/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/lgtm/option.py` & `pkglts-7.3.0/src/pkglts/option/lgtm/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/option.py` & `pkglts-7.3.0/src/pkglts/option/license/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/agpl3-header.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/agpl3-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/agpl3.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/agpl3.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/apache-header.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/apache-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/apache.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/apache.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/bsd2.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/bsd2.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/bsd3.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/bsd3.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cc0.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cc0.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cc_by.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cc_by.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc_nd.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nc_sa.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_nd.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_nd.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cc_by_sa.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cc_by_sa.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cddl.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cddl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cecill-c-header.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cecill-c-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/cecill-c.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/cecill-c.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/epl.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/epl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/gpl2.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/gpl2.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/gpl3-header.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/gpl3-header.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/gpl3.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/gpl3.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/inra_license_agreement.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/inra_license_agreement.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/isc.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/isc.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/lgpl.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/lgpl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/mit.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/mit.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/mpl.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/mpl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/private.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/private.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/unlicense.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/unlicense.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/wtfpl.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/x11.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/x11.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/license/templates/zlib.txt` & `pkglts-7.3.0/src/pkglts/option/license/templates/zlib.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb` & `pkglts-7.3.0/src/pkglts/option/notebook/example/{{ notebook.src_directory }}/example.ipynb`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/notebook/nbcompile.py` & `pkglts-7.3.0/src/pkglts/option/notebook/nbcompile.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/notebook/option.py` & `pkglts-7.3.0/src/pkglts/option/notebook/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/plugin_project/option.py` & `pkglts-7.3.0/src/pkglts/option/plugin_project/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl` & `pkglts-7.3.0/src/pkglts/option/plugin_project/resource/src/{{ base.pkgname }}/option.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/pypi/option.py` & `pkglts-7.3.0/src/pkglts/option/pypi/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/pyproject/option.py` & `pkglts-7.3.0/src/pkglts/option/pyproject/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/pyproject/resource/pyproject.toml` & `pkglts-7.3.0/src/pkglts/option/pyproject/resource/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/readthedocs/option.py` & `pkglts-7.3.0/src/pkglts/option/readthedocs/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/reqs/find_requirements.py` & `pkglts-7.3.0/src/pkglts/option/reqs/find_requirements.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/reqs/option.py` & `pkglts-7.3.0/src/pkglts/option/reqs/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/reqs/stdpkgs.txt` & `pkglts-7.3.0/src/pkglts/option/reqs/stdpkgs.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/requires/option.py` & `pkglts-7.3.0/src/pkglts/option/requires/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst` & `pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/inheritance.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst` & `pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/intersphinx.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst` & `pkglts-7.3.0/src/pkglts/option/sphinx/example/doc/docexamples/matplotlib.rst`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl` & `pkglts-7.3.0/src/pkglts/option/sphinx/example/src/{{ base.pkgname }}/example_doc.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/option.py` & `pkglts-7.3.0/src/pkglts/option/sphinx/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile` & `pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/Makefile`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl` & `pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat` & `pkglts-7.3.0/src/pkglts/option/sphinx/resource/{{sphinx.doc_dir}}/make.bat`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/src/option.py` & `pkglts-7.3.0/src/pkglts/option/src/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/test/example/test/test_example.py.tpl` & `pkglts-7.3.0/src/pkglts/option/test/example/test/test_example.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/test/option.py` & `pkglts-7.3.0/src/pkglts/option/test/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl` & `pkglts-7.3.0/src/pkglts/option/test/resource/test/{% if test.suite_name == 'pytest' %}conftest{% else %}_{% endif %}.py.tpl`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/tox/option.py` & `pkglts-7.3.0/src/pkglts/option/tox/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/travis/option.py` & `pkglts-7.3.0/src/pkglts/option/travis/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/travis/resource/.travis.yml` & `pkglts-7.3.0/src/pkglts/option/travis/resource/.travis.yml`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/version/bump_version.py` & `pkglts-7.3.0/src/pkglts/option/version/bump_version.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option/version/option.py` & `pkglts-7.3.0/src/pkglts/option/version/option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option_object.py` & `pkglts-7.3.0/src/pkglts/option_object.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/option_tools.py` & `pkglts-7.3.0/src/pkglts/option_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/small_tools.py` & `pkglts-7.3.0/src/pkglts/small_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/templating.py` & `pkglts-7.3.0/src/pkglts/templating.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/tree_ascii_fmt.py` & `pkglts-7.3.0/src/pkglts/tree_ascii_fmt.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts/version_management.py` & `pkglts-7.3.0/src/pkglts/version_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts.egg-info/PKG-INFO` & `pkglts-7.3.0/src/pkglts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkglts
-Version: 7.2.0
+Version: 7.3.0
 Summary: Building packages with long term support
 Author-email: revesansparole <revesansparole@gmail.com>
 Maintainer-email: revesansparole <revesansparole@gmail.com>, ThT12 <ThT12@ThT12.fr>, pradal <christophe.pradal@inria.fr>, egarciaitk <emilien.garcia@itk.fr>, Simon Artzet <simon.artzet@gmail.com>, lquibel <lucie.quibel@itk.fr>, Christophe Pradal <christophe.pradal@inria.fr>, Samuel Andres <samuel.andres@itk.fr>
 License: CeCILL-C
 Project-URL: repository, https://github.com/revesansparole/pkglts
 Project-URL: appveyor, https://ci.appveyor.com/project/revesansparole/pkglts/branch/master
 Project-URL: coveralls, https://coveralls.io/github/revesansparole/pkglts?branch=master
```

### Comparing `pkglts-7.2.0/src/pkglts.egg-info/SOURCES.txt` & `pkglts-7.3.0/src/pkglts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/src/pkglts.egg-info/entry_points.txt` & `pkglts-7.3.0/src/pkglts.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/conftest.py` & `pkglts-7.3.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_config_management.py` & `pkglts-7.3.0/test/test_config_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_dependency.py` & `pkglts-7.3.0/test/test_dependency.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_hash_management.py` & `pkglts-7.3.0/test/test_hash_management.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_local.py` & `pkglts-7.3.0/test/test_local.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_manage_cfg.py` & `pkglts-7.3.0/test/test_manage_cfg.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_manage_clean.py` & `pkglts-7.3.0/test/test_manage_clean.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_manage_example.py` & `pkglts-7.3.0/test/test_manage_example.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_manage_regenerate.py` & `pkglts-7.3.0/test/test_manage_regenerate.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_manage_reset.py` & `pkglts-7.3.0/test/test_manage_reset.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_manage_tools_regenerate.py` & `pkglts-7.3.0/test/test_manage_tools_regenerate.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_manage_tools_update_option.py` & `pkglts-7.3.0/test/test_manage_tools_update_option.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_appveyor/test_config.py` & `pkglts-7.3.0/test/test_option/test_appveyor/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_base/test_config.py` & `pkglts-7.3.0/test/test_option/test_base/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_conda/test_config.py` & `pkglts-7.3.0/test/test_option/test_conda/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_coverage/test_config.py` & `pkglts-7.3.0/test/test_option/test_coverage/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_data/test_config.py` & `pkglts-7.3.0/test/test_option/test_data/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_doc/test_badge.py` & `pkglts-7.3.0/test/test_option/test_doc/test_badge.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_doc/test_config.py` & `pkglts-7.3.0/test/test_option/test_doc/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_git/test_config.py` & `pkglts-7.3.0/test/test_option/test_git/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_git/test_handlers.py` & `pkglts-7.3.0/test/test_option/test_git/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_github/test_config.py` & `pkglts-7.3.0/test/test_option/test_github/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_gitlab/test_config.py` & `pkglts-7.3.0/test/test_option/test_gitlab/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_license/test_config.py` & `pkglts-7.3.0/test/test_option/test_license/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_license/test_handlers.py` & `pkglts-7.3.0/test/test_option/test_license/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_notebook/test_config.py` & `pkglts-7.3.0/test/test_option/test_notebook/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_option_common.py` & `pkglts-7.3.0/test/test_option/test_option_common.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_plugin_project/test_config.py` & `pkglts-7.3.0/test/test_option/test_plugin_project/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_pypi/test_config.py` & `pkglts-7.3.0/test/test_option/test_pypi/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_pypi/test_handlers.py` & `pkglts-7.3.0/test/test_option/test_pypi/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_pyproject/test_config.py` & `pkglts-7.3.0/test/test_option/test_pyproject/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_pyproject/test_handlers.py` & `pkglts-7.3.0/test/test_option/test_pyproject/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_readthedocs/test_config.py` & `pkglts-7.3.0/test/test_option/test_readthedocs/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_reqs/test_config.py` & `pkglts-7.3.0/test/test_option/test_reqs/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_reqs/test_find_requirements.py` & `pkglts-7.3.0/test/test_option/test_reqs/test_find_requirements.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_reqs/test_handlers.py` & `pkglts-7.3.0/test/test_option/test_reqs/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_sphinx/test_config.py` & `pkglts-7.3.0/test/test_option/test_sphinx/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_src/test_config.py` & `pkglts-7.3.0/test/test_option/test_src/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_test/test_config.py` & `pkglts-7.3.0/test/test_option/test_test/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_version/test_config.py` & `pkglts-7.3.0/test/test_option/test_version/test_config.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option/test_version/test_handlers.py` & `pkglts-7.3.0/test/test_option/test_version/test_handlers.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_option_tools.py` & `pkglts-7.3.0/test/test_option_tools.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_templating.py` & `pkglts-7.3.0/test/test_templating.py`

 * *Files identical despite different names*

### Comparing `pkglts-7.2.0/test/test_version_management.py` & `pkglts-7.3.0/test/test_version_management.py`

 * *Files identical despite different names*

