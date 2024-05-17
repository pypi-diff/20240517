# Comparing `tmp/mio-cli-1.3.6.tar.gz` & `tmp/mio_cli-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/homes/dpoulin/git/mio_cli_client/dist/tmphzu0tw27/mio-cli-1.3.6.tar", last modified: Thu Dec 21 01:52:57 2023, max compression
+gzip compressed data, was "mio_cli-1.3.7.tar", last modified: Thu May 16 17:37:06 2024, max compression
```

## Comparing `mio-cli-1.3.6.tar` & `mio_cli-1.3.7.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/data/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.3.6/src/data/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/doxygen-awesome-darkmode-toggle.js
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio-cli-1.3.6/src/data/doxygen-awesome.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio-cli-1.3.6/src/data/doxygen.awesome.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio-cli-1.3.6/src/data/doxygen.private.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio-cli-1.3.6/src/data/doxygen.public.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio-cli-1.3.6/src/data/doxygen_footer.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio-cli-1.3.6/src/data/doxygen_header.awesome.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio-cli-1.3.6/src/data/doxygen_header.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio-cli-1.3.6/src/data/doxygen_layout.xml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/doxygen_stylesheet.css
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/idv_doxyfilter_sv.pl
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio-cli-1.3.6/src/data/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/plantuml.jar
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio-cli-1.3.6/src/mio/__init__.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio-cli-1.3.6/src/mio/__main__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49802 2023-09-24 04:09:30.000000 mio-cli-1.3.6/src/mio/cache.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9149 2023-11-28 22:47:56.000000 mio-cli-1.3.6/src/mio/cfg.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio-cli-1.3.6/src/mio/clean.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    22072 2023-11-28 22:41:48.000000 mio-cli-1.3.6/src/mio/cli.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8094 2023-03-23 09:22:45.000000 mio-cli-1.3.6/src/mio/common.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio-cli-1.3.6/src/mio/cov.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio-cli-1.3.6/src/mio/doctor.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio-cli-1.3.6/src/mio/dox.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    92099 2023-12-20 00:50:19.000000 mio-cli-1.3.6/src/mio/eal.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12763 2023-12-19 00:54:08.000000 mio-cli-1.3.6/src/mio/help_text.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio-cli-1.3.6/src/mio/init.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio-cli-1.3.6/src/mio/install.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-09-23 23:12:22.000000 mio-cli-1.3.6/src/mio/main.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3278 2023-11-29 02:50:01.000000 mio-cli-1.3.6/src/mio/new.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16616 2023-12-12 03:28:19.000000 mio-cli-1.3.6/src/mio/publish.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35657 2023-11-21 19:42:20.000000 mio-cli-1.3.6/src/mio/regr.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio-cli-1.3.6/src/mio/results.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    27756 2023-12-20 00:50:33.000000 mio-cli-1.3.6/src/mio/sim.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio-cli-1.3.6/src/mio/user.py
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/PKG-INFO
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       34 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/entry_points.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio-cli-1.3.6/src/mio_cli.egg-info/not-zip-safe
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/requires.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/top_level.txt
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/templates/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio-cli-1.3.6/src/templates/LICENSE_solderpad_v2p1.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio-cli-1.3.6/src/templates/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio-cli-1.3.6/src/templates/dv_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio-cli-1.3.6/src/templates/interactive_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio-cli-1.3.6/src/templates/mdc.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio-cli-1.3.6/src/templates/mdc.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio-cli-1.3.6/src/templates/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio-cli-1.3.6/src/templates/project_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio-cli-1.3.6/src/templates/qst.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio-cli-1.3.6/src/templates/qst.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio-cli-1.3.6/src/templates/regression_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio-cli-1.3.6/src/templates/riv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio-cli-1.3.6/src/templates/riv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio-cli-1.3.6/src/templates/rtl_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio-cli-1.3.6/src/templates/sim_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio-cli-1.3.6/src/templates/ts.yml.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio-cli-1.3.6/src/templates/vcs.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio-cli-1.3.6/src/templates/vcs.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio-cli-1.3.6/src/templates/viv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio-cli-1.3.6/src/templates/viv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio-cli-1.3.6/src/templates/viv.prj.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio-cli-1.3.6/src/templates/vivado_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio-cli-1.3.6/src/templates/xcl.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio-cli-1.3.6/src/templates/xcl.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio-cli-1.3.6/LICENSE
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio-cli-1.3.6/README.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio-cli-1.3.6/pyproject.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2023-12-21 01:52:54.000000 mio-cli-1.3.6/setup.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-12-21 01:52:54.000000 mio-cli-1.3.6/PKG-INFO
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-16 17:37:05.890000 mio_cli-1.3.7/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio_cli-1.3.7/LICENSE
+-rw-r--r--   0 dpoulin   (1000) dpoulin   (1004)     4168 2024-05-16 17:37:05.890000 mio_cli-1.3.7/PKG-INFO
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio_cli-1.3.7/README.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio_cli-1.3.7/pyproject.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2024-05-16 17:37:05.890000 mio_cli-1.3.7/setup.cfg
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-16 17:37:05.530000 mio_cli-1.3.7/src/
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-16 17:37:05.580000 mio_cli-1.3.7/src/data/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio_cli-1.3.7/src/data/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio_cli-1.3.7/src/data/doxygen-awesome-darkmode-toggle.js
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio_cli-1.3.7/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio_cli-1.3.7/src/data/doxygen-awesome-sidebar-only.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio_cli-1.3.7/src/data/doxygen-awesome.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio_cli-1.3.7/src/data/doxygen.awesome.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio_cli-1.3.7/src/data/doxygen.private.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio_cli-1.3.7/src/data/doxygen.public.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio_cli-1.3.7/src/data/doxygen_footer.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio_cli-1.3.7/src/data/doxygen_header.awesome.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio_cli-1.3.7/src/data/doxygen_header.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio_cli-1.3.7/src/data/doxygen_layout.xml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio_cli-1.3.7/src/data/doxygen_stylesheet.css
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio_cli-1.3.7/src/data/idv_doxyfilter_sv.pl
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio_cli-1.3.7/src/data/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio_cli-1.3.7/src/data/plantuml.jar
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-16 17:37:05.820000 mio_cli-1.3.7/src/mio/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio_cli-1.3.7/src/mio/__init__.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio_cli-1.3.7/src/mio/__main__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49802 2023-09-24 04:09:30.000000 mio_cli-1.3.7/src/mio/cache.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9163 2024-05-10 00:04:12.000000 mio_cli-1.3.7/src/mio/cfg.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio_cli-1.3.7/src/mio/clean.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    22072 2023-11-28 22:41:48.000000 mio_cli-1.3.7/src/mio/cli.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8421 2024-05-11 20:06:43.000000 mio_cli-1.3.7/src/mio/common.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio_cli-1.3.7/src/mio/cov.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio_cli-1.3.7/src/mio/doctor.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio_cli-1.3.7/src/mio/dox.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    83098 2024-05-11 21:03:28.000000 mio_cli-1.3.7/src/mio/eal.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12763 2024-05-16 16:55:30.000000 mio_cli-1.3.7/src/mio/help_text.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio_cli-1.3.7/src/mio/init.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio_cli-1.3.7/src/mio/install.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-09-23 23:12:22.000000 mio_cli-1.3.7/src/mio/main.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3278 2024-05-01 23:17:34.000000 mio_cli-1.3.7/src/mio/new.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16616 2023-12-12 03:28:19.000000 mio_cli-1.3.7/src/mio/publish.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35836 2024-05-16 16:50:09.000000 mio_cli-1.3.7/src/mio/regr.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio_cli-1.3.7/src/mio/results.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    28188 2024-05-11 01:16:02.000000 mio_cli-1.3.7/src/mio/sim.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio_cli-1.3.7/src/mio/user.py
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-16 17:37:05.880000 mio_cli-1.3.7/src/mio_cli.egg-info/
+-rw-r--r--   0 dpoulin   (1000) dpoulin   (1004)     4168 2024-05-16 17:37:05.000000 mio_cli-1.3.7/src/mio_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2024-05-16 17:37:05.000000 mio_cli-1.3.7/src/mio_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2024-05-16 17:37:05.000000 mio_cli-1.3.7/src/mio_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       33 2024-05-16 17:37:05.000000 mio_cli-1.3.7/src/mio_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio_cli-1.3.7/src/mio_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2024-05-16 17:37:05.000000 mio_cli-1.3.7/src/mio_cli.egg-info/requires.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2024-05-16 17:37:05.000000 mio_cli-1.3.7/src/mio_cli.egg-info/top_level.txt
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-16 17:37:05.880000 mio_cli-1.3.7/src/templates/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio_cli-1.3.7/src/templates/LICENSE_solderpad_v2p1.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio_cli-1.3.7/src/templates/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio_cli-1.3.7/src/templates/dv_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio_cli-1.3.7/src/templates/interactive_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio_cli-1.3.7/src/templates/mdc.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio_cli-1.3.7/src/templates/mdc.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio_cli-1.3.7/src/templates/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio_cli-1.3.7/src/templates/project_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio_cli-1.3.7/src/templates/qst.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio_cli-1.3.7/src/templates/qst.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio_cli-1.3.7/src/templates/regression_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio_cli-1.3.7/src/templates/riv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio_cli-1.3.7/src/templates/riv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio_cli-1.3.7/src/templates/rtl_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio_cli-1.3.7/src/templates/sim_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio_cli-1.3.7/src/templates/ts.yml.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio_cli-1.3.7/src/templates/vcs.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio_cli-1.3.7/src/templates/vcs.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio_cli-1.3.7/src/templates/viv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio_cli-1.3.7/src/templates/viv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio_cli-1.3.7/src/templates/viv.prj.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio_cli-1.3.7/src/templates/vivado_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio_cli-1.3.7/src/templates/xcl.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio_cli-1.3.7/src/templates/xcl.mflist.j2
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mio-cli-1.3.6/src/data/doxygen-awesome-darkmode-toggle.js` & `mio_cli-1.3.7/src/data/doxygen-awesome-darkmode-toggle.js`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css` & `mio_cli-1.3.7/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only.css` & `mio_cli-1.3.7/src/data/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen-awesome.css` & `mio_cli-1.3.7/src/data/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen.awesome.cfg` & `mio_cli-1.3.7/src/data/doxygen.awesome.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen.private.cfg` & `mio_cli-1.3.7/src/data/doxygen.private.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen.public.cfg` & `mio_cli-1.3.7/src/data/doxygen.public.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen_footer.html` & `mio_cli-1.3.7/src/data/doxygen_footer.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen_header.awesome.html` & `mio_cli-1.3.7/src/data/doxygen_header.awesome.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen_header.html` & `mio_cli-1.3.7/src/data/doxygen_header.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen_layout.xml` & `mio_cli-1.3.7/src/data/doxygen_layout.xml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/doxygen_stylesheet.css` & `mio_cli-1.3.7/src/data/doxygen_stylesheet.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/idv_doxyfilter_sv.pl` & `mio_cli-1.3.7/src/data/idv_doxyfilter_sv.pl`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/mio.toml` & `mio_cli-1.3.7/src/data/mio.toml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/data/plantuml.jar` & `mio_cli-1.3.7/src/data/plantuml.jar`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/cache.py` & `mio_cli-1.3.7/src/mio/cache.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/cfg.py` & `mio_cli-1.3.7/src/mio/cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 glb_cfg  = {}
 
 #version_str = 'Moore.io Client Command Line Interface 1.2.0'
 mio_client_dir    = re.sub("cfg.py", "", os.path.realpath(__file__))
 mio_data_src_dir  = str(pathlib.Path(os.path.join(mio_client_dir, "../data")).resolve())
 mio_template_dir  = str(pathlib.Path(os.path.join(mio_client_dir, "../templates")).resolve())
 vivado_home       = os.getenv("MIO_VIVADO_HOME" , '/tools/vivado/2022.1/Vivado/2022.1/bin/')
-metrics_home      = os.getenv("MIO_METRICS_HOME", '/tools/metrics/')
+metrics_home      = os.getenv("MIO_METRICS_HOME", '~/metrics-c/dsim/20240129.4.0')
 vcs_home          = os.getenv("MIO_VCS_HOME"    , '/tools/vcs/'    )
 xcelium_home      = os.getenv("MIO_XCELIUM_HOME", '/tools/xcelium/')
 questa_home       = os.getenv("MIO_QUESTA_HOME" , '/tools/questa/' )
 riviera_home      = os.getenv("MIO_RIVIERA_HOME", '/tools/riviera/')
 uvm_dpi_so        = "uvm_dpi"
 user_dir          = os.path.expanduser("~")
 mio_user_dir      = user_dir + "/.mio"
```

### Comparing `mio-cli-1.3.6/src/mio/clean.py` & `mio_cli-1.3.7/src/mio/clean.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/cli.py` & `mio_cli-1.3.7/src/mio/cli.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/common.py` & `mio_cli-1.3.7/src/mio/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -266,7 +266,19 @@
         vendor, ip = clean_str.split("/")
     else:
         ip = clean_str
         vendor = ""
     return [vendor, ip]
 
 
+def set_env_var(key, val):
+    dbg(f"Setting env var '{key}' to '{val}'")
+    os.environ[key] = val
+
+def append_env_path(val):
+    path_val = os.environ["PATH"]
+    path_val = f"{val}:{path_val}"
+    os.environ["PATH"] = path_val
+    new_path = os.environ["PATH"]
+    dbg(f"Appended '{val}' to PATH.  New PATH='{new_path}'")
+
+
```

### Comparing `mio-cli-1.3.6/src/mio/cov.py` & `mio_cli-1.3.7/src/mio/cov.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/doctor.py` & `mio_cli-1.3.7/src/mio/doctor.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/dox.py` & `mio_cli-1.3.7/src/mio/dox.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/eal.py` & `mio_cli-1.3.7/src/mio/eal.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,26 +106,30 @@
 
 
 
 
 
 
 def init_workspace(sim_job):
-    if (not sim_job.bwrap) and sim_job.simulator == common.simulators_enum.METRICS:
-        mdc_status = get_process_output(cfg.metrics_home + "/mdc", ["status"], wd=cfg.project_dir)
-        if "This is not a DSim Cloud workspace" in mdc_status:
-            common.info("Initializing mdc workspace ...")
-            mdc_init = get_process_output(cfg.metrics_home + "/mdc", ["init"], wd=cfg.project_dir)
-            if "ERROR" in mdc_init:
-                common.fatal(f"Failed to initialize mdc workspace")
-        elif "Status: Paused" in mdc_status:
-            common.info("Resuming Metrics workspace, this will take a few minutes ...")
-            mdc_resume = get_process_output(cfg.metrics_home + "/mdc", ["workspace", "resume"], wd=cfg.project_dir)
-            if "ERROR" in mdc_resume:
-                common.fatal(f"Failed to resume mdc workspace")
+    if sim_job.simulator == common.simulators_enum.METRICS:
+        if (not sim_job.bwrap) and sim_job.is_regression:
+            mdc_status = get_process_output(cfg.metrics_home + "/mdc", ["status"], wd=cfg.project_dir)
+            if "This is not a DSim Cloud workspace" in mdc_status:
+                common.info("Initializing mdc workspace ...")
+                mdc_init = get_process_output(cfg.metrics_home + "/mdc", ["init"], wd=cfg.project_dir)
+                if "ERROR" in mdc_init:
+                    common.fatal(f"Failed to initialize mdc workspace")
+            elif "Status: Paused" in mdc_status:
+                common.info("Resuming Metrics workspace, this will take a few minutes ...")
+                mdc_resume = get_process_output(cfg.metrics_home + "/mdc", ["workspace", "resume"], wd=cfg.project_dir)
+                if "ERROR" in mdc_resume:
+                    common.fatal(f"Failed to resume mdc workspace")
+        else:
+            pass
+            #set_mtr_env_vars()
 
 
 def invoke_fsoc(ip, core, sim_job):
     sim_str = common.get_simulator_short_name(sim_job.simulator)
     fsc_args = argparse.Namespace()
     fsc_args.setup       = True
     fsc_args.build       = False
@@ -152,18 +156,15 @@
     sys.stdout = sys.__stdout__
     
     try:
         file_path_partial_name = re.sub(r':', '_', core.name)
         eda_file_dir = cfg.fsoc_dir + "/" + core.sname + "/sim-xsim"
         eda_file_path = eda_file_dir + "/" + file_path_partial_name + "_0.eda.yml"
         core_rel_path = os.path.relpath(core.dir, eda_file_dir)
-        if sim_job.simulator == common.simulators_enum.METRICS:
-            core_base_path = os.path.relpath(core.dir, cfg.temp_path)
-        else:
-            core_base_path = "$MIO_" + core.sname.replace("-", "_").upper() + "_SRC_PATH"
+        core_base_path = "$MIO_" + core.sname.replace("-", "_").upper() + "_SRC_PATH"
         if not os.path.exists(eda_file_path):
             common.fatal("Could not find FuseSoC output file " + eda_file_path)
         else:
             with open(eda_file_path, 'r') as edafile:
                 eda_yaml = yaml.load(edafile, Loader=SafeLoader)
                 if not eda_yaml:
                     common.fatal("Could not parse FuseSoC output file " + eda_file_path)
@@ -217,17 +218,14 @@
                 flist_template = cfg.templateEnv.get_template(f"{sim_str}.flist.j2")
                 outputText = flist_template.render(defines=defines, files=files, dirs=dirs)
                 flist_file_path = str(pathlib.Path(cfg.temp_path + "/" + file_path_partial_name + "_0.flist").resolve())
                 with open(flist_file_path,'w') as flist_file:
                     flist_file.write(outputText)
                 flist_file.close()
                 
-                if sim_job.simulator == common.simulators_enum.METRICS:
-                    flist_file_path = os.path.relpath(flist_file_path, cfg.project_dir)
-                
                 return flist_file_path
     except Exception as e:
         common.fatal("Failed to convert FuseSoC output data for core '" + core.name + "': "+ str(e))
 
 
 
 def gen_image_ip(ip, sim_job, fsoc_core_name, fsoc_core_flist_path):
@@ -304,21 +302,14 @@
                 common.copy_directory(ip.path + "/" + ip.src_path, f"{cfg.temp_path}/{ip_dir}")
             path = "${PROJECT_ROOT_DIR}/.mio/temp/" + ip_dir
         else:
             if ip.is_encrypted:
                 path = "${PROJECT_ROOT_DIR}/" + os.path.relpath(ip.path + "/" + ip.src_path + "." + sim_str, cfg.project_dir)
             else:
                 path = "${PROJECT_ROOT_DIR}/" + os.path.relpath(ip.path + "/" + ip.src_path, cfg.project_dir)
-    elif ip.is_global and (sim_job.simulator == common.simulators_enum.METRICS):
-        if ip.is_encrypted:
-            common.copy_directory(ip.path + "/" + ip.src_path + "." + sim_str, f"{cfg.temp_path}/{ip_dir}")
-            path = ".mio/temp/" + ip_dir
-        else:
-            common.copy_directory(ip.path + "/" + ip.src_path, f"{cfg.temp_path}/{ip_dir}")
-            path = ".mio/temp/" + ip_dir
     else:
         if ip.is_encrypted:
             path = ip.path + "/" + ip.src_path + "." + sim_str
         else:
             path = ip.path + "/" + ip.src_path
     
     flist_env_var_name = 'MIO_' + ip.name.upper() + '_SRC_PATH'
@@ -361,22 +352,20 @@
 def elab_ip(ip, sim_job):
     ip_str = f"{ip.vendor}/{ip.name}"
     ip_dir_name = f"{ip.vendor}__{ip.name}"
     sim_str = common.get_simulator_short_name(sim_job.simulator)
     defines = sim_job.cmp_args
     if sim_job.is_regression:
         ip_dir_name = f"{ip.vendor}__{ip.name}__{sim_job.regression_name}__{sim_job.regression_timestamp}"
-        if sim_job.simulator != common.simulators_enum.METRICS:
-            common.create_dir(cfg.sim_output_dir + "/" + sim_str + "/regr_wd/" + ip_dir_name)
-        elab_out =            cfg.sim_output_dir + "/" + sim_str + "/regr_wd/" + ip_dir_name
+        common.create_dir(cfg.sim_output_dir + "/" + sim_str + "/regr_wd/" + ip_dir_name)
+        elab_out =        cfg.sim_output_dir + "/" + sim_str + "/regr_wd/" + ip_dir_name
     else:
         ip_dir_name = f"{ip.vendor}__{ip.name}"
         elab_out = cfg.sim_output_dir + "/" + sim_str + "/sim_wd/" + ip_dir_name
-    if sim_job.simulator != common.simulators_enum.METRICS:
-        common.create_dir(elab_out)
+    common.create_dir(elab_out)
     timestamp_start = common.timestamp()
     log_file_path = do_elab(ip, sim_job, elab_out)
     if not sim_job.dry_run:
         timestamp_end = common.timestamp()
         errors = scan_elab_log_file_for_errors(log_file_path, sim_job)
         if len(errors):
             common.error("Errors during Elaboration of IP '" + ip_str + "':")
@@ -427,15 +416,15 @@
         cmp_out = ip_regr_root_path
     else:
         cmp_out = cfg.sim_output_dir + "/" + sim_str + "/sim_wd/" + ip_dir_name
     
     if sim_job.simulator != common.simulators_enum.METRICS:
         if sim_job.is_regression:
             common.create_dir(ip_regr_root_path)
-        common.create_dir(cmp_out)
+    common.create_dir(cmp_out)
     
     compilation_log_path = cfg.sim_dir + "/cmp/" + name + "." + sim_str + ".log"
     compilation_command_file = f"{ip_dir_name}.{sim_str}.gen_image.cmd.txt"
     
     if sim_job.simulator == common.simulators_enum.VIVADO:
         common.fatal(f"Vivado cannot Compile and Elaborate in one step.")
     elif sim_job.simulator == common.simulators_enum.VCS:
@@ -447,45 +436,31 @@
         arg_list.append("-l "  + compilation_log_path)
         write_cmd_to_disk(sim_job, "vcs", arg_list, compilation_command_file)
         sim_job.bwrap_commands += launch_eda_bin(cfg.vcs_home + "/vcs", arg_list, wd=cmp_out, output=cfg.dbg, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.METRICS:
         arg_list += metrics_default_gen_image_args
         arg_list.append("-F " + flist_path)
-        mtr_compilation_log_path = ip_dir_name + "." + sim_str + ".log"
-        arg_list.append("-l " + mtr_compilation_log_path)
+        arg_list.append("-l " + compilation_log_path)
         arg_list.append(f"-timescale {cfg.sim_timescale}")
         
-        if ip.vendor == "@global":
-            arg_list.append(f"-genimage global__{ip.name}")
-        elif ip.vendor == "@fsoc":
-            arg_list.append(f"-genimage fsoc__{ip.name}")
-        else:
-            arg_list.append(f"-genimage {ip.vendor}__{ip.name}")
+        arg_list.append(f"-genimage {ip.vendor}__{ip.name}")
         
         for construct in ip.hdl_src_top_constructs:
             if "." in construct:
                 lib,name = construct.split(".")
                 arg_list.append(f"-top {name}")
             else:
                 arg_list.append(f"-top {construct}")
         
-        arg_list_str = ""
-        for arg in arg_list:
-            arg_list_str = arg_list_str + f" {arg}"
         if cfg.dbg:
-            arg_list_str += " -g"
-            arg_list = [f"dsim -v -a '{arg_list_str}'"]
-        else:
-            arg_list = [f"dsim -a '{arg_list_str}'"]
-        write_cmd_to_disk(sim_job, "mdc", arg_list, compilation_command_file)
-        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", arg_list, wd=cfg.project_dir, output=cfg.dbg, dry_run=sim_job.dry_run)
-        launch_eda_bin(cfg.metrics_home + "/mdc", ["download", mtr_compilation_log_path], wd=cfg.project_dir, output=cfg.dbg, dry_run=sim_job.dry_run)
-        if not sim_job.dry_run:
-            common.move_file(f"{cfg.project_dir}/_downloaded_{mtr_compilation_log_path}", compilation_log_path)
+            pass
+            #arg_list.append("-g")
+        write_cmd_to_disk(sim_job, "dsim", arg_list, compilation_command_file)
+        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/bin/dsim", arg_list, wd=cmp_out, output=cfg.dbg, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.XCELIUM:
         arg_list += xcelium_default_gen_image_args
         arg_list.append(license_macros_file_path);
         arg_list.append("-f " + flist_path)
         # TODO Add compilation output argument for nc
         write_cmd_to_disk(sim_job, "xrun", arg_list, compilation_command_file)
@@ -530,23 +505,21 @@
     
     ip_dir_name = f"{vendor}__{name}"
     cmp_out_dir = cfg.sim_output_dir + "/" + sim_str + "/cmp_out/"
     cmp_out = cmp_out_dir + ip_dir_name
     
     if sim_job.is_regression:
         ip_dir_name = f"{sim_job.vendor}__{sim_job.ip}__{sim_job.regression_name}__{sim_job.regression_timestamp}"
-        if sim_job.simulator != common.simulators_enum.METRICS:
-            common.create_dir(cfg.sim_output_dir + "/" + sim_str + "/regr_wd/" + ip_dir_name)
+        common.create_dir(cfg.sim_output_dir + "/" + sim_str + "/regr_wd/" + ip_dir_name)
         sim_out = cfg.sim_output_dir + "/" + sim_str + "/regr_wd/" + ip_dir_name
     else:
         sim_out = cfg.sim_output_dir + "/" + sim_str + "/sim_wd/" + ip_dir_name
     
-    if sim_job.simulator != common.simulators_enum.METRICS:
-        common.create_dir(cmp_out)
-        common.create_dir(sim_out)
+    common.create_dir(cmp_out)
+    common.create_dir(sim_out)
     
     compilation_log_path = cfg.sim_dir + "/cmp/" + name + "." + sim_str + ".cmp.log"
     compilation_command_file = f"{ip_dir_name}.{sim_str}.cmp.cmd.txt"
     
     if sim_job.simulator == common.simulators_enum.VIVADO:
         arg_list += vivado_default_compilation_args
         arg_list += incdir_list
@@ -570,40 +543,22 @@
         arg_list.append("-l "  + compilation_log_path)
         write_cmd_to_disk(sim_job, "vcs", arg_list, compilation_command_file)
         sim_job.bwrap_commands += launch_eda_bin(cfg.vcs_home + "/vcs", arg_list, wd=sim_out, output=cfg.dbg, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.METRICS:
         arg_list += metrics_default_compilation_args
         arg_list += incdir_list
-        if vendor == "@global":
-            arg_list.append(f"-lib global__{name}")
-        elif vendor == "@fsoc":
-            arg_list.append(f"-lib fsoc__{name}")
-        else:
-            arg_list.append(f"-lib {vendor}__{name}")
-        #common.copy_file(license_macros_file_path, f"{cfg.temp_path}/uvml_mio_lic_macros.svh")
-        #arg_list.append(f".mio/temp/uvml_mio_lic_macros.svh") # HACK compute that path
         arg_list.append("-F " + flist_path)
-        mtr_compilation_log_path = ip_dir_name + "." + sim_str + ".cmp.log"
-        arg_list.append("-l " + mtr_compilation_log_path)
+        arg_list.append("-l " + compilation_log_path)
         
-        arg_list_str = ""
-        for arg in arg_list:
-            arg_list_str = arg_list_str + f" {arg}"
         if cfg.dbg:
-            arg_list_str += " -g"
-            arg_list = [f"dvlcom -v -a '{arg_list_str}'"]
-        else:
-            arg_list = [f"dvlcom -a '{arg_list_str}'"]
-        #launch_eda_bin(cfg.metrics_home + "/mdc", ["initialize"], wd=cfg.project_dir, output=True) # TODO Add project.yml and store this in there
-        write_cmd_to_disk(sim_job, "mdc", arg_list, compilation_command_file)
-        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", arg_list, wd=cfg.project_dir, output=cfg.dbg, dry_run=sim_job.dry_run)
-        launch_eda_bin(cfg.metrics_home + "/mdc", ["download", mtr_compilation_log_path], wd=cfg.project_dir, output=cfg.dbg, dry_run=sim_job.dry_run)
-        if not sim_job.dry_run:
-            common.move_file(f"{cfg.project_dir}/_downloaded_{mtr_compilation_log_path}", compilation_log_path)
+            pass
+            #arg_list.append("-g")
+        write_cmd_to_disk(sim_job, "dvlcom", arg_list, compilation_command_file)
+        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/bin/dvlcom", arg_list, wd=cmp_out, output=cfg.dbg, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.XCELIUM:
         arg_list += xcelium_default_compilation_args
         arg_list.append(license_macros_file_path);
         arg_list.append("-f " + flist_path)
         # TODO Add compilation output argument for nc
         write_cmd_to_disk(sim_job, "xrun", arg_list, compilation_command_file)
@@ -737,56 +692,39 @@
         if ip.has_dut:
             arg_list += dut_elab_to_arg_list(ip, sim_job)
         # TODO Add elaboration output argument for vcs
         write_cmd_to_disk(sim_job, "vcs", arg_list, elaboration_command_file)
         sim_job.bwrap_commands += launch_eda_bin(cfg.vcs_home + "/vcs", arg_list, wd, output=cfg.dbg, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.METRICS:
-        arg_list += metrics_default_elaboration_args
-        mtr_elaboration_log_path = ip_dir_name + "." + sim_str + ".elab.log"
-        arg_list.append(f"-l {mtr_elaboration_log_path}")
+        arg_list.append(f"-l {elaboration_log_path}")
         arg_list.append(f"-timescale {cfg.sim_timescale}")
         arg_list += def_list
         arg_list += elab_list
         arg_list += deps_list
         if ip.has_dut:
             arg_list += dut_elab_to_arg_list(ip, sim_job)
-        #arg_list.append(f"+incdir+%UVM_HOME%/src")
-        #arg_list.append(f"%UVM_HOME%/src/uvm_pkg.sv")
         
-        if ip.vendor == "@global":
-            arg_list.append(f"-genimage global__{ip.name}")
-            arg_list.append(f"-L global__{ip.name}")
-        elif ip.vendor == "@fsoc":
-            arg_list.append(f"-genimage fsoc__{ip.name}")
-            arg_list.append(f"-L fsoc__{ip.name}")
-        else:
-            arg_list.append(f"-genimage {ip.vendor}__{ip.name}")
-            arg_list.append(f"-L {ip.vendor}__{ip.name}")
+        arg_list.append(f"-genimage {ip.vendor}__{ip.name}")
+        arg_list.append(f"-L {ip.vendor}__{ip.name}={ip_cmp_path}")
         
         for construct in ip.hdl_src_top_constructs:
             if "." in construct:
                 lib,name = construct.split(".")
                 arg_list.append(f"-top {name}")
             else:
                 arg_list.append(f"-top {construct}")
         
-        arg_list_str = ""
-        for arg in arg_list:
-            arg_list_str = arg_list_str + f" {arg}"
+        common.create_dir(wd)
+        
         if cfg.dbg:
-            arg_list_str += " -g"
-            arg_list = [f"dsim -v -a '{arg_list_str}'"]
-        else:
-            arg_list = [f"dsim -a '{arg_list_str}'"]
+            pass
+            #arg_list.append(f"-g")
         write_cmd_to_disk(sim_job, "mdc", arg_list, elaboration_command_file)
-        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", arg_list, wd=cfg.project_dir, output=cfg.dbg, dry_run=sim_job.dry_run)
-        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", mtr_elaboration_log_path], wd=cfg.project_dir, output=cfg.dbg, dry_run=sim_job.dry_run)
-        if not sim_job.dry_run:
-            common.move_file(f"{cfg.project_dir}/_downloaded_{mtr_elaboration_log_path}", elaboration_log_path)
+        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/bin/dsim", arg_list, wd, output=cfg.dbg, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.XCELIUM:
         arg_list += xcelium_default_elaboration_args
         if ip.has_dut:
             arg_list += dut_elab_to_arg_list(ip, sim_job)
         # TODO Add elaboration output argument for nc
         write_cmd_to_disk(sim_job, "xrun", arg_list, elaboration_command_file)
@@ -846,40 +784,26 @@
     
     plus_args["__MIO_TOKEN"] = user.login()
     
     if sim_job.target_name != "default":
         target_str = f"_{sim_job.target_name}"
     else:
         target_str = f""
-    if sim_job.simulator == common.simulators_enum.METRICS:
-        mdc_regr_results_dir = cfg.temp_path + "/mdc_regr"
-        mdc_sim_results_dir  = cfg.temp_path + "/mdc_results"
-        common.create_dir(mdc_regr_results_dir)
-        common.create_dir(mdc_sim_results_dir )
-        if sim_job.is_regression:
-            common.create_dir       (mdc_regr_results_dir + "/" + ip.name + target_str + "_" + sim_job.regression_name + "_" + sim_job.regression_timestamp)
-            mdc_tests_results_path = ".mio/temp/mdc_regr/"      + ip.name + target_str + "_" + sim_job.regression_name + "_" + sim_job.regression_timestamp + "/" + test_result_dir
-        else:
-            common.create_dir       (mdc_sim_results_dir + "/" + test_result_dir)
-            mdc_tests_results_path = ".mio/temp/mdc_results/"  + test_result_dir
     if sim_job.is_regression:
         common.create_dir   (cfg.regr_results_dir + "/" + ip.name + target_str + "_" + sim_job.regression_name + "_" + sim_job.regression_timestamp)
         tests_results_path = cfg.regr_results_dir + "/" + ip.name + target_str + "_" + sim_job.regression_name + "_" + sim_job.regression_timestamp + "/" + test_result_dir
     else:
         tests_results_path = cfg.sim_results_dir + "/" + test_result_dir
     
     output = not sim_job.is_regression
     
     simulation_log_path = tests_results_path + "/sim.log"
     cov_path = tests_results_path + "/cov"
     common.create_dir(tests_results_path)
     common.create_dir(tests_results_path + "/uvmx")
-    if sim_job.simulator == common.simulators_enum.METRICS:
-        common.create_dir(cfg.project_dir + "/" + mdc_tests_results_path)
-        common.create_dir(cfg.project_dir + "/" + mdc_tests_results_path + "/uvmx")
     sim_job.results_path = tests_results_path
     sim_job.results_dir_name = test_result_dir
     if sim_job.waves:
         if sim_job.simulator == common.simulators_enum.VIVADO:
             wave_capture_script_path = tests_results_path + "/waves.viv.tcl"
             waves_path = tests_results_path + "/waves.wdb"
             arg_list.append("--wdb "      + waves_path              )
@@ -929,27 +853,19 @@
         elif sim_job.simulator == common.simulators_enum.RIVIERA:
             # TODO Implement coverage for riviera
             pass
     
     plus_args["UVM_NO_RELNOTES"                ] = ""
     plus_args["UVM_VERBOSITY"                  ] = "UVM_" + sim_job.verbosity.upper()
     plus_args["UVM_MAX_QUIT_COUNT"             ] = str(sim_job.max_errors)
-    
-    if sim_job.simulator == common.simulators_enum.METRICS:
-        plus_args["SIM_DIR_RESULTS"                ] = f"{mdc_tests_results_path}/.."
-        plus_args["UVMX_FILE_BASE_DIR_SIM"         ] = os.path.relpath(cfg.sim_dir, cfg.project_dir)
-        plus_args["UVMX_FILE_BASE_DIR_TEST_RESULTS"] = f"{mdc_tests_results_path}"
-        plus_args["UVMX_FILE_BASE_DIR_TB"          ] = os.path.relpath(ip.path + "/" + ip.src_path, cfg.project_dir)
-        plus_args["UVMX_FILE_BASE_DIR_TESTS"       ] = os.path.relpath(ip.path + "/" + ip.src_path + "/" + ip.hdl_src_tests_path, cfg.project_dir)
-    else:
-        plus_args["SIM_DIR_RESULTS"                ] = f"{cfg.sim_results_dir}"
-        plus_args["UVMX_FILE_BASE_DIR_SIM"         ] = cfg.sim_dir
-        plus_args["UVMX_FILE_BASE_DIR_TEST_RESULTS"] = tests_results_path
-        plus_args["UVMX_FILE_BASE_DIR_TB"          ] = ip.path + "/" + ip.src_path
-        plus_args["UVMX_FILE_BASE_DIR_TESTS"       ] = ip.path + "/" + ip.src_path + "/" + ip.hdl_src_tests_path
+    plus_args["SIM_DIR_RESULTS"                ] = f"{cfg.sim_results_dir}"
+    plus_args["UVMX_FILE_BASE_DIR_SIM"         ] = cfg.sim_dir
+    plus_args["UVMX_FILE_BASE_DIR_TEST_RESULTS"] = tests_results_path
+    plus_args["UVMX_FILE_BASE_DIR_TB"          ] = ip.path + "/" + ip.src_path
+    plus_args["UVMX_FILE_BASE_DIR_TESTS"       ] = ip.path + "/" + ip.src_path + "/" + ip.hdl_src_tests_path
     
     if ip.has_targets:
         if not sim_job.target_name in ip.targets:
             common.fatal(f"IP '{ip.vendor}/{ip.name}' does not have specified target '{sim_job.target_name}'")
         sim_args = ip.targets[sim_job.target_name].sim_args
         for arg in sim_args:
             plus_args[arg] = sim_args[arg]
@@ -979,57 +895,35 @@
         write_cmd_to_disk(sim_job, "simv", arg_list, simulation_command_file)
         sem.release()
         sim_job.bwrap_commands += launch_eda_bin(cfg.vcs_home + "/simv", arg_list, wd, output=output, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.METRICS:
         arg_list += metrics_default_simulation_args
         arg_list += plus_args_list
-        mtr_simulation_log_path = f"{test_result_dir}.log"
-        prism_data_path = f"{mdc_tests_results_path}/prism.data"
+        prism_data_path = f"{tests_results_path}/prism.data"
         prism_data_downloaded_path = f"{cfg.project_dir}/_downloaded_prism.data"
-        arg_list.append("-l " + mtr_simulation_log_path)
+        arg_list.append("-l " + simulation_log_path)
         arg_list.append("-sv_seed " + str(sim_job.seed))
         arg_list.append(f"-image {ip.vendor}__{ip.name}")
         arg_list.append(f"-timescale {cfg.sim_timescale}")
-        arg_list.append(f"-sv_lib %UVM_HOME%/src/dpi/libuvm_dpi.so")
+        arg_list.append( "-sv_lib ${UVM_HOME}/src/dpi/libuvm_dpi.so")
         arg_list.append(f"-sv_lib libcurl.so")
         #arg_list.append(f"-work {ip.vendor}__{ip.name}")
         
         so_libs = get_all_so_libs(ip, sim_job)
         for so_lib in so_libs:
-            so_lib_temp_path = f"{cfg.temp_path}/{so_lib}"
-            common.copy_file(so_libs[so_lib], so_lib_temp_path)
-            so_lib_path = os.path.relpath(so_lib_temp_path, cfg.project_dir)
-            arg_list.append(f"-sv_lib {so_lib_path}")
-        
-        arg_list_str = ""
-        for arg in arg_list:
-            arg_list_str = arg_list_str + f" {arg}"
+            common.copy_file(so_libs[so_lib], f"{wd}/{so_lib}")
+            arg_list.append(f"-sv_lib {so_lib}")
+        
         if cfg.dbg:
-            arg_list = [f"dsim -v -a '{arg_list_str}'"]
-        else:
-            arg_list = [f"dsim -a '{arg_list_str}'"]
-        write_cmd_to_disk(sim_job, "mdc", arg_list, simulation_command_file)
+            pass
+            #arg_list.append("-g")
+        write_cmd_to_disk(sim_job, "dsim", arg_list, simulation_command_file)
         sem.release()
-        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", arg_list, wd=cfg.project_dir, output=output, dry_run=sim_job.dry_run)
-        common.remove_file(f"{cfg.project_dir}/_downloaded_{mtr_simulation_log_path}")
-        common.info("Downloading simulation log ...")
-        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", mtr_simulation_log_path], wd=cfg.project_dir, dry_run=sim_job.dry_run)
-        if not sim_job.dry_run:
-            common.move_file(f"{cfg.project_dir}/_downloaded_{mtr_simulation_log_path}", simulation_log_path)
-            if sim_job.waves:
-                common.remove_file(f"{cfg.project_dir}/_downloaded_{test_result_dir}.vcd.gz")
-                common.info("Downloading simulation waveforms ...")
-                sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", f"{test_result_dir}.vcd.gz"], wd=cfg.project_dir, dry_run=sim_job.dry_run)
-                common.move_file(f"{cfg.project_dir}/_downloaded_{test_result_dir}.vcd.gz", f"{tests_results_path}/waves.vcd.gz")
-            common.remove_file(f"{cfg.project_dir}/_downloaded_prism.data")
-            common.info("Downloading simulation data ...")
-            sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", prism_data_path], wd=cfg.project_dir, dry_run=sim_job.dry_run)
-            common.move_file(prism_data_downloaded_path, f"{tests_results_path}/prism.data")
-            download_uvmx_logs_mdc(sim_job, mdc_tests_results_path, tests_results_path)
+        sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/bin/dsim", arg_list, wd, output=output, dry_run=sim_job.dry_run)
         
     elif sim_job.simulator == common.simulators_enum.XCELIUM:
         arg_list += xcelium_default_simulation_args
         # TODO Add simulation output argument for nc
         write_cmd_to_disk(sim_job, "xrun", arg_list, simulation_command_file)
         sem.release()
         sim_job.bwrap_commands += launch_eda_bin(cfg.nc_home + "/xrun", arg_list, wd, output=output, dry_run=sim_job.dry_run)
@@ -1169,43 +1063,31 @@
     ip_dir = f"{ip.vendor}__{ip.name}"
     sim_str = common.get_simulator_short_name(sim_job.simulator)
     found_flist = False
     flist_path = ""
     
     if ip.hdl_src_flists[sim_job.simulator] != "":
         found_flist = True
-        if ip.is_global and (sim_job.simulator == common.simulators_enum.METRICS):
-            flist_path = f".mio/temp/{ip_dir}/{ip.hdl_src_flists[sim_job.simulator]}"
+        if ip.is_encrypted:
+            flist_path = f"{ip.path}/{ip.src_path}.{sim_str}/{ip.hdl_src_flists[sim_job.simulator]}"
         else:
-            if ip.is_encrypted:
-                flist_path = f"{ip.path}/{ip.src_path}.{sim_str}/{ip.hdl_src_flists[sim_job.simulator]}"
-            else:
-                flist_path = f"{ip.path}/{ip.src_path}/{ip.hdl_src_flists[sim_job.simulator]}"
+            flist_path = f"{ip.path}/{ip.src_path}/{ip.hdl_src_flists[sim_job.simulator]}"
     if not found_flist:
         flist_path = gen_flist(ip, sim_job, include_uvm)
     return flist_path
 
 
 
 def gen_master_flist(ip, sim_job, deps, fsoc_core_name, fsoc_core_flist_path):
     sim_str = common.get_simulator_short_name(sim_job.simulator)
     
     flists = gen_flists(ip, deps, sim_job, False)
     flist_path = cfg.temp_path + "/" + ip.vendor + "__" + ip.name + ".top." + sim_str + ".flist"
-    if sim_job.simulator == common.simulators_enum.METRICS:
-        final_flists = []
-        if fsoc_core_flist_path != "":
-            final_flists.append(fsoc_core_flist_path.replace(".mio/temp/", ""))
-        for flist in flists:
-            final_flist = os.path.relpath(flist, cfg.temp_path)
-            final_flists.append(final_flist)
-        flists = final_flists
-    else:
-        if fsoc_core_flist_path != "":
-            flists.insert(0, fsoc_core_flist_path)
+    if fsoc_core_flist_path != "":
+        flists.insert(0, fsoc_core_flist_path)
     
     defines = []
     if ip.has_targets:
         cmp_args = {}
         if not sim_job.target_name in ip.targets:
             common.fatal(f"IP '{ip.vendor}/{ip.name}' does not have specified target '{sim_job.target_name}'")
         cmp_args = ip.targets[sim_job.target_name].cmp_args
@@ -1217,17 +1099,14 @@
                 define['value'] = ""
             else:
                 define['boolean'] = False
                 define['value'] = cmp_args[arg]
             defines.append(define)
     
     gen_mflist_file(sim_job.simulator, ip.vendor, ip.name, flist_path, defines, flists)
-    if sim_job.simulator == common.simulators_enum.METRICS:
-        flist_path = os.path.relpath(flist_path, cfg.project_dir)
-        #flist_path = flist_path.replace(cfg.project_dir, "")
     
     return flist_path
 
 
 
 def gen_prj_file(sim_job, ip, flist_path):
     ip_str = f"{ip.vendor}/{ip.name}"
@@ -1284,48 +1163,21 @@
     
     rel_ip_path = os.path.relpath(ip.path, cfg.temp_path)
     simulator = sim_str
     flist_template = cfg.templateEnv.get_template(f"{simulator}.flist.j2")
     directories = []
     for dir in ip.hdl_src_directories:
         if dir == ".":
-            if sim_job.simulator == common.simulators_enum.METRICS:
-                if ip.is_global:
-                    directories.append(f"{ip_dir}")
-                else:
-                    if ip.is_encrypted:
-                        directories.append(f"{rel_ip_path}/{ip.src_path}.{sim_str}")
-                    else:
-                        directories.append(f"{rel_ip_path}/{ip.src_path}")
-            else:
-                directories.append("${MIO_" + ip.name.upper() + "_SRC_PATH}")
+            directories.append("${MIO_" + ip.name.upper() + "_SRC_PATH}")
         else:
-            if sim_job.simulator == common.simulators_enum.METRICS:
-                if ip.is_global:
-                    directories.append(f"{ip_dir}/{dir}")
-                else:
-                    if ip.is_encrypted:
-                        directories.append(f"{rel_ip_path}/{ip.src_path}.{sim_str}/{dir}")
-                    else:
-                        directories.append(f"{rel_ip_path}/{ip.src_path}/{dir}")
-            else:
-                directories.append("${MIO_" + ip.name.upper() + "_SRC_PATH}/" + dir)
+            directories.append("${MIO_" + ip.name.upper() + "_SRC_PATH}/" + dir)
     
     top_files = []
     for file in ip.hdl_src_top_files:
-        if sim_job.simulator == common.simulators_enum.METRICS:
-            if ip.is_global:
-                top_files.append(f"{ip_dir}/{file}")
-            else:
-                if ip.is_encrypted:
-                    top_files.append(f"{rel_ip_path}/{ip.src_path}.{sim_str}/{file}")
-                else:
-                    top_files.append(f"{rel_ip_path}/{ip.src_path}/{file}")
-        else:
-            top_files.append("${MIO_" + ip.name.upper() + "_SRC_PATH}/" + file)
+        top_files.append("${MIO_" + ip.name.upper() + "_SRC_PATH}/" + file)
     
     flist_path = cfg.temp_path + "/" + ip.vendor + "__" + ip.name + "." + simulator + ".flist"
     if include_uvm:
         if ip.type == "dv":
             include_uvm = True
         else:
             include_uvm = False
@@ -1894,14 +1746,25 @@
                     common.remove_file(path_downloaded_file)
                     common.remove_file(path_final_file     )
                     sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", f"{file}"], wd=wd, output=cfg.dbg)
                     common.move_file(path_downloaded_file, path_final_file)
 
 
 
+def set_mtr_env_vars():
+    common.set_env_var("DSIM_HOME"           , f"{cfg.metrics_home}")
+    common.set_env_var("LLVM_HOME"           , f"{cfg.metrics_home}/llvm_small")
+    common.set_env_var("STD_LIBS"            , f"{cfg.metrics_home}/std_pkgs/lib")
+    common.set_env_var("UVM_HOME"            , f"{cfg.metrics_home}/uvm/{cfg.uvm_version}")
+    common.set_env_var("DSIM_LD_LIBRARY_PATH", f"{cfg.metrics_home}/lib:{cfg.metrics_home}/llvm_small/lib")
+    common.set_env_var("LD_LIBRARY_PATH"     , "${DSIM_LD_LIBRARY_PATH}")
+    common.append_env_path(f"{cfg.metrics_home}/bin")
+    common.append_env_path(f"{cfg.metrics_home}/uvm-1.2/bin")
+    common.append_env_path(f"{cfg.metrics_home}/llvm_small/bin")
+
 
 
 
 
 
 
 
@@ -2010,20 +1873,15 @@
 
 def convert_deps_to_args(deps, sim_job):
     sim_str = common.get_simulator_short_name(sim_job.simulator)
     args = []
     for dep in deps:
         if dep.name != "uvm":
             if sim_job.simulator == common.simulators_enum.METRICS:
-                if dep.vendor == "@global":
-                    dep_dir_name = f"global__{dep.name}"
-                elif dep.vendor == "@fsoc":
-                    dep_dir_name = f"fsoc__{dep.name}"
-                else:
-                    dep_dir_name = f"{dep.vendor}__{dep.name}"
+                dep_dir_name = f"{dep.vendor}__{dep.name}"
                 lib_str = f"-L {dep_dir_name}"
             elif sim_job.simulator == common.simulators_enum.QUESTA:
                 dep_dir_name = f"{dep.vendor}__{dep.name}"
                 lib_str = f"-L {dep_dir_name}"
             else:
                 dep_dir_name = f"{dep.vendor}__{dep.name}"
                 lib_str = "-L " + dep.name + "=" + cfg.sim_output_dir + "/" + sim_str + "/cmp_out/" + dep_dir_name
@@ -2045,23 +1903,23 @@
 
 
 def get_incdir_list(deps, sim_job):
     sim_str = common.get_simulator_short_name(sim_job.simulator)
     incdir_list = []
     for dep in deps:
         for dir in dep.hdl_src_directories:
-            if dep.is_global and (sim_job.bwrap or sim_job.simulator == common.simulators_enum.METRICS):
+            if dep.is_global and (sim_job.bwrap):
                 src_path = f"{cfg.temp_path}/{dep.vendor}__{dep.name}/{dir}"
             else:
                 if dep.is_encrypted:
                     src_path = f"{dep.path}/{dep.src_path}.{sim_str}/{dir}"
                 else:
                     src_path = f"{dep.path}/{dep.src_path}/{dir}"
             if sim_job.simulator == common.simulators_enum.VIVADO:
                 incdir_list.append("-i " + src_path)
             else:
-                if (sim_job.bwrap or sim_job.simulator == common.simulators_enum.METRICS):
+                if (sim_job.bwrap):
                     src_path = os.path.relpath(src_path, cfg.project_dir)
                 incdir_list.append("+incdir+" + src_path)
     return incdir_list
```

### Comparing `mio-cli-1.3.6/src/mio/help_text.py` & `mio_cli-1.3.7/src/mio/help_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2021-2023 Datum Technology Corporation
 # SPDX-License-Identifier: GPL-3.0
 ########################################################################################################################
 
 
-version = "1.3.6"
+version = "1.3.7"
 version_text = f"Moore.io CLI Client v{version}"
 
 
 
 main_help_text = f"""
                                  Moore.io (`mio`) Command Line Interface (CLI) - v{version}
                                       User Manual: https://mio-cli.readthedocs.io/
```

### Comparing `mio-cli-1.3.6/src/mio/init.py` & `mio_cli-1.3.7/src/mio/init.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/install.py` & `mio_cli-1.3.7/src/mio/install.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/new.py` & `mio_cli-1.3.7/src/mio/new.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/publish.py` & `mio_cli-1.3.7/src/mio/publish.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/regr.py` & `mio_cli-1.3.7/src/mio/regr.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,14 +518,18 @@
     deps_to_install = len(ip.get_deps_to_install())
     if deps_to_install > 0:
         common.fatal(f"You must first install this IP's dependencies ({deps_to_install}): `mio install {name}`")
     
     if simulator == None:
         simulator = cfg.default_simulator
     
+    # Temporary until Metrics Cloud sim jobs are working
+    if simulator == common.simulators_enum.METRICS::
+        common.fatal(f"Regressions not supported for DSim yet")
+    
     common.create_dir(cfg.regr_results_dir)
     test_suite = scan_target_ip_for_test_suite(ip, simulator)
     if test_suite.target_name != "*":
         if test_suite.target_name != target_name:
             common.fatal(f"Specified target '{target_name}' does not match test suite's {test_suite.target_name}")
     regression = test_suite.get_regression(cfg.cli_args.regr)
     regression.reduce()
```

### Comparing `mio-cli-1.3.6/src/mio/results.py` & `mio_cli-1.3.7/src/mio/results.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio/sim.py` & `mio_cli-1.3.7/src/mio/sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,20 @@
 
 
 def create_sim_directories(sim_job):
     common.dbg("Creating sim directories")
     common.create_dir(cfg.sim_dir)
     common.create_dir(cfg.sim_output_dir)
     common.create_dir(cfg.regr_results_dir)
+    common.create_dir(cfg.sim_output_dir + "/mdc"                     )
+    common.create_dir(cfg.sim_output_dir + "/mdc/cov_wd"              )
+    common.create_dir(cfg.sim_output_dir + "/mdc/cmp_out"             )
+    common.create_dir(cfg.sim_output_dir + "/mdc/sim_wd"              )
+    common.create_dir(cfg.sim_output_dir + "/mdc/regr_wd"             )
+    common.create_dir(cfg.sim_output_dir + "/mdc/so_libs"             )
     common.create_dir(cfg.sim_output_dir + "/viv"                     )
     common.create_dir(cfg.sim_output_dir + "/viv/cov_wd"              )
     common.create_dir(cfg.sim_output_dir + "/viv/cmp_out"             )
     common.create_dir(cfg.sim_output_dir + "/viv/sim_wd"              )
     common.create_dir(cfg.sim_output_dir + "/viv/regr_wd"             )
     common.create_dir(cfg.sim_output_dir + "/viv/so_libs"             )
     common.create_dir(cfg.sim_output_dir + "/vcs"                     )
```

### Comparing `mio-cli-1.3.6/src/mio/user.py` & `mio_cli-1.3.7/src/mio/user.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/mio_cli.egg-info/PKG-INFO` & `mio_cli-1.3.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.6
+Version: 1.3.7
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sphinx_book_theme>=0.2.0
+Requires-Dist: zipfile2>=0.0.12
+Requires-Dist: tqdm>=4.63.0
+Requires-Dist: Jinja2>=3.0.3
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: toml>=0.10.2
+Requires-Dist: fusesoc==1.12.0
+Requires-Dist: requests>=2.27.1
+Requires-Dist: semver>=2.13.0
+Requires-Dist: ezodf>=0.3.2
 
 [![License](https://img.shields.io/badge/License-GPL%203.0-blue.svg)](https://opensource.org/licenses/GPL-3.0)
 [![Documentation Status](https://readthedocs.org/projects/mio-cli/badge/?version=latest)](https://mio-cli.readthedocs.io/en/latest/index.html)
 
 # [Moore.io](https://www.mooreio.com/) [Command Line Interface Client](https://datum-technology-corporation.github.io/mio_cli_client/)
 
 
@@ -86,9 +94,7 @@
       
    Manage Results and other EDA Tool Outputs
       clean          Manages outputs from tools (other than job results)
       cov            Manages coverage data from EDA tools
       dox            HDL source code documentation generation via Doxygen
       results        Manages results from EDA tools
 ````
-
-
```

### Comparing `mio-cli-1.3.6/src/mio_cli.egg-info/SOURCES.txt` & `mio_cli-1.3.7/src/mio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/templates/LICENSE_solderpad_v2p1.md` & `mio_cli-1.3.7/src/templates/LICENSE_solderpad_v2p1.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/templates/dv_ip.yml` & `mio_cli-1.3.7/src/templates/dv_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/templates/interactive_results.html.j2` & `mio_cli-1.3.7/src/templates/interactive_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/templates/regression_results.html.j2` & `mio_cli-1.3.7/src/templates/regression_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/templates/rtl_ip.yml` & `mio_cli-1.3.7/src/templates/rtl_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/templates/ts.yml.j2` & `mio_cli-1.3.7/src/templates/ts.yml.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/src/templates/vivado_ip.yml` & `mio_cli-1.3.7/src/templates/vivado_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/LICENSE` & `mio_cli-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/README.md` & `mio_cli-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.6/setup.cfg` & `mio_cli-1.3.7/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mio-cli
-version = 1.3.6
+version = 1.3.7
 author = Datum Technology Corporation
 author_email = mio@datumtc.ca
 description = The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = SystemVerilog, UVM, DV, verilog, VHDL, hdl, rtl, synthesis, FPGA, simulation, Xilinx, Altera
 url = https://datum-technology-corporation.github.io/mio_cli_client/
```

### Comparing `mio-cli-1.3.6/PKG-INFO` & `mio_cli-1.3.7/src/mio_cli.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.6
+Version: 1.3.7
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.6.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: sphinx_book_theme>=0.2.0
+Requires-Dist: zipfile2>=0.0.12
+Requires-Dist: tqdm>=4.63.0
+Requires-Dist: Jinja2>=3.0.3
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: toml>=0.10.2
+Requires-Dist: fusesoc==1.12.0
+Requires-Dist: requests>=2.27.1
+Requires-Dist: semver>=2.13.0
+Requires-Dist: ezodf>=0.3.2
 
 [![License](https://img.shields.io/badge/License-GPL%203.0-blue.svg)](https://opensource.org/licenses/GPL-3.0)
 [![Documentation Status](https://readthedocs.org/projects/mio-cli/badge/?version=latest)](https://mio-cli.readthedocs.io/en/latest/index.html)
 
 # [Moore.io](https://www.mooreio.com/) [Command Line Interface Client](https://datum-technology-corporation.github.io/mio_cli_client/)
 
 
@@ -86,9 +94,7 @@
       
    Manage Results and other EDA Tool Outputs
       clean          Manages outputs from tools (other than job results)
       cov            Manages coverage data from EDA tools
       dox            HDL source code documentation generation via Doxygen
       results        Manages results from EDA tools
 ````
-
-
```

