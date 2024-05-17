# Comparing `tmp/mio_cli-1.3.8.tar.gz` & `tmp/mio_cli-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mio_cli-1.3.8.tar", last modified: Fri May 17 12:13:33 2024, max compression
+gzip compressed data, was "mio_cli-1.3.9.tar", last modified: Fri May 17 13:08:16 2024, max compression
```

## Comparing `mio_cli-1.3.8.tar` & `mio_cli-1.3.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 12:13:31.330000 mio_cli-1.3.8/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio_cli-1.3.8/LICENSE
--rw-r--r--   0 dpoulin   (1000) dpoulin   (1004)     4168 2024-05-17 12:13:31.320000 mio_cli-1.3.8/PKG-INFO
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio_cli-1.3.8/README.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio_cli-1.3.8/pyproject.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2024-05-17 12:13:31.330000 mio_cli-1.3.8/setup.cfg
-drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 12:13:30.990000 mio_cli-1.3.8/src/
-drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 12:13:31.030000 mio_cli-1.3.8/src/data/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio_cli-1.3.8/src/data/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio_cli-1.3.8/src/data/doxygen-awesome-darkmode-toggle.js
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio_cli-1.3.8/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio_cli-1.3.8/src/data/doxygen-awesome-sidebar-only.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio_cli-1.3.8/src/data/doxygen-awesome.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio_cli-1.3.8/src/data/doxygen.awesome.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio_cli-1.3.8/src/data/doxygen.private.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio_cli-1.3.8/src/data/doxygen.public.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio_cli-1.3.8/src/data/doxygen_footer.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio_cli-1.3.8/src/data/doxygen_header.awesome.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio_cli-1.3.8/src/data/doxygen_header.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio_cli-1.3.8/src/data/doxygen_layout.xml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio_cli-1.3.8/src/data/doxygen_stylesheet.css
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio_cli-1.3.8/src/data/idv_doxyfilter_sv.pl
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio_cli-1.3.8/src/data/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio_cli-1.3.8/src/data/plantuml.jar
-drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 12:13:31.270000 mio_cli-1.3.8/src/mio/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio_cli-1.3.8/src/mio/__init__.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio_cli-1.3.8/src/mio/__main__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49802 2023-09-24 04:09:30.000000 mio_cli-1.3.8/src/mio/cache.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9163 2024-05-10 00:04:12.000000 mio_cli-1.3.8/src/mio/cfg.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio_cli-1.3.8/src/mio/clean.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    22072 2023-11-28 22:41:48.000000 mio_cli-1.3.8/src/mio/cli.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8421 2024-05-11 20:06:43.000000 mio_cli-1.3.8/src/mio/common.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio_cli-1.3.8/src/mio/cov.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio_cli-1.3.8/src/mio/doctor.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio_cli-1.3.8/src/mio/dox.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    83095 2024-05-17 12:02:52.000000 mio_cli-1.3.8/src/mio/eal.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12763 2024-05-17 12:06:36.000000 mio_cli-1.3.8/src/mio/help_text.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio_cli-1.3.8/src/mio/init.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio_cli-1.3.8/src/mio/install.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-09-23 23:12:22.000000 mio_cli-1.3.8/src/mio/main.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3278 2024-05-01 23:17:34.000000 mio_cli-1.3.8/src/mio/new.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16616 2023-12-12 03:28:19.000000 mio_cli-1.3.8/src/mio/publish.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35835 2024-05-17 12:04:27.000000 mio_cli-1.3.8/src/mio/regr.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio_cli-1.3.8/src/mio/results.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    28182 2024-05-17 12:09:56.000000 mio_cli-1.3.8/src/mio/sim.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio_cli-1.3.8/src/mio/user.py
-drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 12:13:31.320000 mio_cli-1.3.8/src/mio_cli.egg-info/
--rw-r--r--   0 dpoulin   (1000) dpoulin   (1004)     4168 2024-05-17 12:13:30.000000 mio_cli-1.3.8/src/mio_cli.egg-info/PKG-INFO
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2024-05-17 12:13:30.000000 mio_cli-1.3.8/src/mio_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2024-05-17 12:13:30.000000 mio_cli-1.3.8/src/mio_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       33 2024-05-17 12:13:30.000000 mio_cli-1.3.8/src/mio_cli.egg-info/entry_points.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio_cli-1.3.8/src/mio_cli.egg-info/not-zip-safe
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2024-05-17 12:13:30.000000 mio_cli-1.3.8/src/mio_cli.egg-info/requires.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2024-05-17 12:13:30.000000 mio_cli-1.3.8/src/mio_cli.egg-info/top_level.txt
-drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 12:13:31.320000 mio_cli-1.3.8/src/templates/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio_cli-1.3.8/src/templates/LICENSE_solderpad_v2p1.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio_cli-1.3.8/src/templates/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio_cli-1.3.8/src/templates/dv_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio_cli-1.3.8/src/templates/interactive_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio_cli-1.3.8/src/templates/mdc.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio_cli-1.3.8/src/templates/mdc.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio_cli-1.3.8/src/templates/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio_cli-1.3.8/src/templates/project_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio_cli-1.3.8/src/templates/qst.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio_cli-1.3.8/src/templates/qst.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio_cli-1.3.8/src/templates/regression_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio_cli-1.3.8/src/templates/riv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio_cli-1.3.8/src/templates/riv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio_cli-1.3.8/src/templates/rtl_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio_cli-1.3.8/src/templates/sim_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio_cli-1.3.8/src/templates/ts.yml.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio_cli-1.3.8/src/templates/vcs.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio_cli-1.3.8/src/templates/vcs.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio_cli-1.3.8/src/templates/viv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio_cli-1.3.8/src/templates/viv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio_cli-1.3.8/src/templates/viv.prj.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio_cli-1.3.8/src/templates/vivado_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio_cli-1.3.8/src/templates/xcl.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio_cli-1.3.8/src/templates/xcl.mflist.j2
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 13:08:14.460000 mio_cli-1.3.9/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio_cli-1.3.9/LICENSE
+-rw-r--r--   0 dpoulin   (1000) dpoulin   (1004)     4168 2024-05-17 13:08:14.450000 mio_cli-1.3.9/PKG-INFO
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio_cli-1.3.9/README.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio_cli-1.3.9/pyproject.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2024-05-17 13:08:14.460000 mio_cli-1.3.9/setup.cfg
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 13:08:14.090000 mio_cli-1.3.9/src/
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 13:08:14.140000 mio_cli-1.3.9/src/data/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio_cli-1.3.9/src/data/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio_cli-1.3.9/src/data/doxygen-awesome-darkmode-toggle.js
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio_cli-1.3.9/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio_cli-1.3.9/src/data/doxygen-awesome-sidebar-only.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio_cli-1.3.9/src/data/doxygen-awesome.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio_cli-1.3.9/src/data/doxygen.awesome.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio_cli-1.3.9/src/data/doxygen.private.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio_cli-1.3.9/src/data/doxygen.public.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio_cli-1.3.9/src/data/doxygen_footer.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio_cli-1.3.9/src/data/doxygen_header.awesome.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio_cli-1.3.9/src/data/doxygen_header.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio_cli-1.3.9/src/data/doxygen_layout.xml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio_cli-1.3.9/src/data/doxygen_stylesheet.css
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio_cli-1.3.9/src/data/idv_doxyfilter_sv.pl
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio_cli-1.3.9/src/data/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio_cli-1.3.9/src/data/plantuml.jar
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 13:08:14.380000 mio_cli-1.3.9/src/mio/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio_cli-1.3.9/src/mio/__init__.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio_cli-1.3.9/src/mio/__main__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49802 2023-09-24 04:09:30.000000 mio_cli-1.3.9/src/mio/cache.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9163 2024-05-10 00:04:12.000000 mio_cli-1.3.9/src/mio/cfg.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio_cli-1.3.9/src/mio/clean.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    22072 2023-11-28 22:41:48.000000 mio_cli-1.3.9/src/mio/cli.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8421 2024-05-11 20:06:43.000000 mio_cli-1.3.9/src/mio/common.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio_cli-1.3.9/src/mio/cov.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio_cli-1.3.9/src/mio/doctor.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio_cli-1.3.9/src/mio/dox.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    83098 2024-05-17 13:07:48.000000 mio_cli-1.3.9/src/mio/eal.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12763 2024-05-17 13:07:57.000000 mio_cli-1.3.9/src/mio/help_text.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio_cli-1.3.9/src/mio/init.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio_cli-1.3.9/src/mio/install.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-09-23 23:12:22.000000 mio_cli-1.3.9/src/mio/main.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3278 2024-05-01 23:17:34.000000 mio_cli-1.3.9/src/mio/new.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16616 2023-12-12 03:28:19.000000 mio_cli-1.3.9/src/mio/publish.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35835 2024-05-17 12:04:27.000000 mio_cli-1.3.9/src/mio/regr.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio_cli-1.3.9/src/mio/results.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    28182 2024-05-17 12:09:56.000000 mio_cli-1.3.9/src/mio/sim.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio_cli-1.3.9/src/mio/user.py
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 13:08:14.450000 mio_cli-1.3.9/src/mio_cli.egg-info/
+-rw-r--r--   0 dpoulin   (1000) dpoulin   (1004)     4168 2024-05-17 13:08:13.000000 mio_cli-1.3.9/src/mio_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2024-05-17 13:08:14.000000 mio_cli-1.3.9/src/mio_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2024-05-17 13:08:13.000000 mio_cli-1.3.9/src/mio_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       33 2024-05-17 13:08:13.000000 mio_cli-1.3.9/src/mio_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio_cli-1.3.9/src/mio_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2024-05-17 13:08:13.000000 mio_cli-1.3.9/src/mio_cli.egg-info/requires.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2024-05-17 13:08:13.000000 mio_cli-1.3.9/src/mio_cli.egg-info/top_level.txt
+drwxr-xr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2024-05-17 13:08:14.450000 mio_cli-1.3.9/src/templates/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio_cli-1.3.9/src/templates/LICENSE_solderpad_v2p1.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio_cli-1.3.9/src/templates/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio_cli-1.3.9/src/templates/dv_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio_cli-1.3.9/src/templates/interactive_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio_cli-1.3.9/src/templates/mdc.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio_cli-1.3.9/src/templates/mdc.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio_cli-1.3.9/src/templates/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio_cli-1.3.9/src/templates/project_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio_cli-1.3.9/src/templates/qst.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio_cli-1.3.9/src/templates/qst.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio_cli-1.3.9/src/templates/regression_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio_cli-1.3.9/src/templates/riv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio_cli-1.3.9/src/templates/riv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio_cli-1.3.9/src/templates/rtl_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio_cli-1.3.9/src/templates/sim_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio_cli-1.3.9/src/templates/ts.yml.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio_cli-1.3.9/src/templates/vcs.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio_cli-1.3.9/src/templates/vcs.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio_cli-1.3.9/src/templates/viv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio_cli-1.3.9/src/templates/viv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio_cli-1.3.9/src/templates/viv.prj.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio_cli-1.3.9/src/templates/vivado_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio_cli-1.3.9/src/templates/xcl.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio_cli-1.3.9/src/templates/xcl.mflist.j2
```

### Comparing `mio_cli-1.3.8/LICENSE` & `mio_cli-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/PKG-INFO` & `mio_cli-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.8
+Version: 1.3.9
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mio_cli-1.3.8/README.md` & `mio_cli-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/setup.cfg` & `mio_cli-1.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mio-cli
-version = 1.3.8
+version = 1.3.9
 author = Datum Technology Corporation
 author_email = mio@datumtc.ca
 description = The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = SystemVerilog, UVM, DV, verilog, VHDL, hdl, rtl, synthesis, FPGA, simulation, Xilinx, Altera
 url = https://datum-technology-corporation.github.io/mio_cli_client/
```

### Comparing `mio_cli-1.3.8/src/data/doxygen-awesome-darkmode-toggle.js` & `mio_cli-1.3.9/src/data/doxygen-awesome-darkmode-toggle.js`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css` & `mio_cli-1.3.9/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen-awesome-sidebar-only.css` & `mio_cli-1.3.9/src/data/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen-awesome.css` & `mio_cli-1.3.9/src/data/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen.awesome.cfg` & `mio_cli-1.3.9/src/data/doxygen.awesome.cfg`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen.private.cfg` & `mio_cli-1.3.9/src/data/doxygen.private.cfg`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen.public.cfg` & `mio_cli-1.3.9/src/data/doxygen.public.cfg`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen_footer.html` & `mio_cli-1.3.9/src/data/doxygen_footer.html`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen_header.awesome.html` & `mio_cli-1.3.9/src/data/doxygen_header.awesome.html`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen_header.html` & `mio_cli-1.3.9/src/data/doxygen_header.html`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen_layout.xml` & `mio_cli-1.3.9/src/data/doxygen_layout.xml`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/doxygen_stylesheet.css` & `mio_cli-1.3.9/src/data/doxygen_stylesheet.css`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/idv_doxyfilter_sv.pl` & `mio_cli-1.3.9/src/data/idv_doxyfilter_sv.pl`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/mio.toml` & `mio_cli-1.3.9/src/data/mio.toml`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/data/plantuml.jar` & `mio_cli-1.3.9/src/data/plantuml.jar`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/cache.py` & `mio_cli-1.3.9/src/mio/cache.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/cfg.py` & `mio_cli-1.3.9/src/mio/cfg.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/clean.py` & `mio_cli-1.3.9/src/mio/clean.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/cli.py` & `mio_cli-1.3.9/src/mio/cli.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/common.py` & `mio_cli-1.3.9/src/mio/common.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/cov.py` & `mio_cli-1.3.9/src/mio/cov.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/doctor.py` & `mio_cli-1.3.9/src/mio/doctor.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/dox.py` & `mio_cli-1.3.9/src/mio/dox.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/eal.py` & `mio_cli-1.3.9/src/mio/eal.py`

 * *Files 0% similar despite different names*

```diff
@@ -818,15 +818,15 @@
                     f.close()
                 except Exception as e:
                     common.fatal("Could not create wave capture script at " + wave_capture_script_path + ": " + str(e))
         elif sim_job.simulator == common.simulators_enum.VCS:
             # TODO Implement waves file for vcs
             pass
         elif sim_job.simulator == common.simulators_enum.METRICS:
-            arg_list.append(f"-waves {test_result_dir}.mxd")
+            arg_list.append(f"-waves {tests_results_path}.mxd")
         elif sim_job.simulator == common.simulators_enum.XCELIUM:
             # TODO Implement waves file for xcelium
             pass
         elif sim_job.simulator == common.simulators_enum.QUESTA:
             # TODO Implement waves file for questa
             pass
         elif sim_job.simulator == common.simulators_enum.RIVIERA:
```

### Comparing `mio_cli-1.3.8/src/mio/help_text.py` & `mio_cli-1.3.9/src/mio/help_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2021-2023 Datum Technology Corporation
 # SPDX-License-Identifier: GPL-3.0
 ########################################################################################################################
 
 
-version = "1.3.8"
+version = "1.3.9"
 version_text = f"Moore.io CLI Client v{version}"
 
 
 
 main_help_text = f"""
                                  Moore.io (`mio`) Command Line Interface (CLI) - v{version}
                                       User Manual: https://mio-cli.readthedocs.io/
```

### Comparing `mio_cli-1.3.8/src/mio/init.py` & `mio_cli-1.3.9/src/mio/init.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/install.py` & `mio_cli-1.3.9/src/mio/install.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/new.py` & `mio_cli-1.3.9/src/mio/new.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/publish.py` & `mio_cli-1.3.9/src/mio/publish.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/regr.py` & `mio_cli-1.3.9/src/mio/regr.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/results.py` & `mio_cli-1.3.9/src/mio/results.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/sim.py` & `mio_cli-1.3.9/src/mio/sim.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio/user.py` & `mio_cli-1.3.9/src/mio/user.py`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/mio_cli.egg-info/PKG-INFO` & `mio_cli-1.3.9/src/mio_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.8
+Version: 1.3.9
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mio_cli-1.3.8/src/mio_cli.egg-info/SOURCES.txt` & `mio_cli-1.3.9/src/mio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/templates/LICENSE_solderpad_v2p1.md` & `mio_cli-1.3.9/src/templates/LICENSE_solderpad_v2p1.md`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/templates/dv_ip.yml` & `mio_cli-1.3.9/src/templates/dv_ip.yml`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/templates/interactive_results.html.j2` & `mio_cli-1.3.9/src/templates/interactive_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/templates/regression_results.html.j2` & `mio_cli-1.3.9/src/templates/regression_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/templates/rtl_ip.yml` & `mio_cli-1.3.9/src/templates/rtl_ip.yml`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/templates/ts.yml.j2` & `mio_cli-1.3.9/src/templates/ts.yml.j2`

 * *Files identical despite different names*

### Comparing `mio_cli-1.3.8/src/templates/vivado_ip.yml` & `mio_cli-1.3.9/src/templates/vivado_ip.yml`

 * *Files identical despite different names*

