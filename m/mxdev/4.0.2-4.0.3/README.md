# Comparing `tmp/mxdev-4.0.2.tar.gz` & `tmp/mxdev-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxdev-4.0.2.tar", last modified: Tue Mar 12 23:45:46 2024, max compression
+gzip compressed data, was "mxdev-4.0.3.tar", last modified: Fri May 17 11:51:35 2024, max compression
```

## Comparing `mxdev-4.0.2.tar` & `mxdev-4.0.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.323175 mxdev-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-03-12 23:45:41.000000 mxdev-4.0.2/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-03-12 23:45:41.000000 mxdev-4.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-12 23:45:41.000000 mxdev-4.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-12 23:45:41.000000 mxdev-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-03-12 23:45:46.323175 mxdev-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11470 2024-03-12 23:45:41.000000 mxdev-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.315175 mxdev-4.0.2/example/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-12 23:45:41.000000 mxdev-4.0.2/example/constraints-infile.txt
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-12 23:45:41.000000 mxdev-4.0.2/example/example.ini
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-12 23:45:41.000000 mxdev-4.0.2/example/requirements-infile.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-12 23:45:41.000000 mxdev-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 23:45:46.323175 mxdev-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.311175 mxdev-4.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.315175 mxdev-4.0.2/src/mxdev/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/including.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.319175 mxdev-4.0.2/src/mxdev/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.323175 mxdev-4.0.2/src/mxdev/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file01.ini
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file02.ini
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file03.ini
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file04.ini
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file_with_http_include01.ini
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file_with_http_include02.ini
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file_with_http_include03.ini
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/data/file_with_http_include04.ini
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    17769 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/test_git_submodules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/test_including.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/test_mercurial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/test_svn.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/test_vcs_filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.323175 mxdev-4.0.2/src/mxdev/vcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/bazaar.py
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/common.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4991 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/darcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/gitsvn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/mercurial.py
--rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-03-12 23:45:41.000000 mxdev-4.0.2/src/mxdev/vcs/svn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 23:45:46.323175 mxdev-4.0.2/src/mxdev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20311 2024-03-12 23:45:46.000000 mxdev-4.0.2/src/mxdev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-12 23:45:46.000000 mxdev-4.0.2/src/mxdev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 23:45:46.000000 mxdev-4.0.2/src/mxdev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-12 23:45:46.000000 mxdev-4.0.2/src/mxdev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 23:45:46.000000 mxdev-4.0.2/src/mxdev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-12 23:45:46.000000 mxdev-4.0.2/src/mxdev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 23:45:46.000000 mxdev-4.0.2/src/mxdev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.754864 mxdev-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-17 11:51:31.000000 mxdev-4.0.3/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-17 11:51:31.000000 mxdev-4.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-17 11:51:31.000000 mxdev-4.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-17 11:51:31.000000 mxdev-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20814 2024-05-17 11:51:35.754864 mxdev-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-05-17 11:51:31.000000 mxdev-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.746864 mxdev-4.0.3/example/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-17 11:51:31.000000 mxdev-4.0.3/example/constraints-infile.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-17 11:51:31.000000 mxdev-4.0.3/example/example.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 11:51:31.000000 mxdev-4.0.3/example/requirements-infile.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-17 11:51:31.000000 mxdev-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 11:51:35.754864 mxdev-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.742864 mxdev-4.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.746864 mxdev-4.0.3/src/mxdev/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/including.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9077 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.750864 mxdev-4.0.3/src/mxdev/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.750864 mxdev-4.0.3/src/mxdev/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file01.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file02.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file03.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file04.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file_with_http_include01.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file_with_http_include02.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file_with_http_include03.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/data/file_with_http_include04.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18043 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/test_git_submodules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/test_including.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/test_mercurial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/test_svn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/test_vcs_filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.754864 mxdev-4.0.3/src/mxdev/vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/bazaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4991 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/darcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/gitsvn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/mercurial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-05-17 11:51:31.000000 mxdev-4.0.3/src/mxdev/vcs/svn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 11:51:35.754864 mxdev-4.0.3/src/mxdev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20814 2024-05-17 11:51:35.000000 mxdev-4.0.3/src/mxdev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-17 11:51:35.000000 mxdev-4.0.3/src/mxdev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:51:35.000000 mxdev-4.0.3/src/mxdev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 11:51:35.000000 mxdev-4.0.3/src/mxdev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 11:51:35.000000 mxdev-4.0.3/src/mxdev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 11:51:35.000000 mxdev-4.0.3/src/mxdev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 11:51:35.000000 mxdev-4.0.3/src/mxdev.egg-info/top_level.txt
```

### Comparing `mxdev-4.0.2/CHANGES.md` & `mxdev-4.0.3/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 ## Changes
 
+## 4.0.3 (2024-05-17)
+
+
+- Fix #45: Packages with capital names do not get ignored when checked out.
+  [jensens]
+
+
 ## 4.0.2 (2024-03-13)
 
 - Fix #42: deprecated use of `pkg_resoures` to load entry points and parse requirements.
   This enables mxdev to work on Python 3.12, where `pkg_resources` is no longer installed by default in virtual_envs.
   [jensens]
 
 ## 4.0.1 (2024-03-01)
```

### Comparing `mxdev-4.0.2/CONTRIBUTING.md` & `mxdev-4.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/LICENSE.md` & `mxdev-4.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/PKG-INFO` & `mxdev-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxdev
-Version: 4.0.2
+Version: 4.0.3
 Summary: Enable to work with Python projects containing lots of packages, of which you only want to develop some.
 Author-email: MX Stack Developers <dev@bluedynamics.com>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://github.com/mxstack/mxdev
 Project-URL: Bug Reports, https://github.com/mxstack/mxdev/issues
 Project-URL: Source, https://github.com/mxstack/mxdev/
 Keywords: pip,vcs,git,development
@@ -148,14 +148,18 @@
     otherpackage==33.12.1
 ```
 
 It is possible to add as many overrides as needed.
 When writing the *constraints-out*, the new version will be taken into account.
 If there is a source section defined for the same package, the source will be used and entries here are ignored.
 
+Note: When using [uv](https://pypi.org/project/uv/) pip install the version overrides here are not needed, since it [supports overrides nativly](https://github.com/astral-sh/uv?tab=readme-ov-file#dependency-overrides).
+With uv it is recommended to create an `overrides.txt` file with the version overrides and use `uv pip install --overrides overrides.txt [..]` to install the packages.
+
+
 #### `ignores`
 
 Ignore packages that are already defined in a dependent constraints file.
 No new version will be provided.
 This is specifically handy if a package is going to be installed editable from local file system (like `-e .`), but was already pinned in an upstream constraints file.
 
 This can be defined as:
@@ -437,14 +441,21 @@
 
 Maintainers are Jens Klein and the [BlueDynamics Alliance](https://bluedynamics.com) developer team.
 
 We appreciate any contribution! If you have an idea, found a bug, want to drop us a question, or a release is needed, please just file an issue at the [mxdev issue tracker](https://github.com/bluedynamics/mxdev/issues).
 
 ## Changes
 
+## 4.0.3 (2024-05-17)
+
+
+- Fix #45: Packages with capital names do not get ignored when checked out.
+  [jensens]
+
+
 ## 4.0.2 (2024-03-13)
 
 - Fix #42: deprecated use of `pkg_resoures` to load entry points and parse requirements.
   This enables mxdev to work on Python 3.12, where `pkg_resources` is no longer installed by default in virtual_envs.
   [jensens]
 
 ## 4.0.1 (2024-03-01)
```

### Comparing `mxdev-4.0.2/README.md` & `mxdev-4.0.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,18 @@
     otherpackage==33.12.1
 ```
 
 It is possible to add as many overrides as needed.
 When writing the *constraints-out*, the new version will be taken into account.
 If there is a source section defined for the same package, the source will be used and entries here are ignored.
 
+Note: When using [uv](https://pypi.org/project/uv/) pip install the version overrides here are not needed, since it [supports overrides nativly](https://github.com/astral-sh/uv?tab=readme-ov-file#dependency-overrides).
+With uv it is recommended to create an `overrides.txt` file with the version overrides and use `uv pip install --overrides overrides.txt [..]` to install the packages.
+
+
 #### `ignores`
 
 Ignore packages that are already defined in a dependent constraints file.
 No new version will be provided.
 This is specifically handy if a package is going to be installed editable from local file system (like `-e .`), but was already pinned in an upstream constraints file.
 
 This can be defined as:
```

### Comparing `mxdev-4.0.2/pyproject.toml` & `mxdev-4.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "mxdev"
 description = "Enable to work with Python projects containing lots of packages, of which you only want to develop some."
-version = "4.0.2"
+version = "4.0.3"
 keywords = ["pip", "vcs", "git", "development"]
 authors = [
   {name = "MX Stack Developers", email = "dev@bluedynamics.com" }
 ]
 requires-python = ">=3.8"
 license = { text = "BSD 2-Clause License" }
 classifiers = [
```

### Comparing `mxdev-4.0.2/src/mxdev/config.py` & `mxdev-4.0.3/src/mxdev/config.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/entry_points.py` & `mxdev-4.0.3/src/mxdev/entry_points.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/hooks.py` & `mxdev-4.0.3/src/mxdev/hooks.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/including.py` & `mxdev-4.0.3/src/mxdev/including.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/main.py` & `mxdev-4.0.3/src/mxdev/main.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/processing.py` & `mxdev-4.0.3/src/mxdev/processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .logging import logger
 from .state import State
 from .vcs.common import WorkingCopies
 from packaging.requirements import Requirement
 from pathlib import Path
 from urllib import parse
 from urllib import request
+from urllib.error import URLError
 
 import typing
 
 
 def process_line(
     line: str,
     package_keys: typing.List[str],
@@ -49,19 +50,20 @@
             variety="r",
         )
     try:
         parsed = Requirement(line)
     except Exception:
         pass
     else:
-        if parsed.name in package_keys:
+        parsed_name_lower = parsed.name.lower()
+        if parsed_name_lower in [k.lower() for k in package_keys]:
             line = f"# {line.strip()} -> mxdev disabled (source)\n"
-        if variety == "c" and parsed.name in override_keys:
+        if variety == "c" and parsed_name_lower in [k.lower() for k in override_keys]:
             line = f"# {line.strip()} -> mxdev disabled (override)\n"
-        if variety == "c" and parsed.name in ignore_keys:
+        if variety == "c" and parsed_name_lower in [k.lower() for k in ignore_keys]:
             line = f"# {line.strip()} -> mxdev disabled (ignore)\n"
     if variety == "c":
         return [], [line]
     return [line], []
 
 
 def process_io(
@@ -121,24 +123,27 @@
                 )
         else:
             logger.info(
                 f"Can not read {variety_verbose} file '{file_or_url}', "
                 "it does not exist. Empty file assumed."
             )
     else:
-        with request.urlopen(file_or_url) as fio:
-            process_io(
-                fio,
-                requirements,
-                constraints,
-                package_keys,
-                override_keys,
-                ignore_keys,
-                variety,
-            )
+        try:
+            with request.urlopen(file_or_url) as fio:
+                process_io(
+                    fio,
+                    requirements,
+                    constraints,
+                    package_keys,
+                    override_keys,
+                    ignore_keys,
+                    variety,
+                )
+        except URLError as e:
+            raise Exception(f"Failed to fetch '{file_or_url}': {e}")
 
     if requirements and variety == "r":
         requirements = (
             [
                 "#" * 79 + "\n",
                 f"# begin requirements from: {file_or_url}\n\n",
             ]
```

### Comparing `mxdev-4.0.2/src/mxdev/tests/test_common.py` & `mxdev-4.0.3/src/mxdev/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/tests/test_git.py` & `mxdev-4.0.3/src/mxdev/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/tests/test_git_submodules.py` & `mxdev-4.0.3/src/mxdev/tests/test_git_submodules.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import pytest
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_checkout_with_submodule(mkgitrepo, src, caplog):
+def test_checkout_with_submodule(mkgitrepo, src, caplog, git_allow_file_protocol):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in itith
     """
 
     submodule_name = "submodule_a"
     submodule_a = mkgitrepo(submodule_name)
     submodule_a.add_file("foo")
@@ -46,15 +46,15 @@
             ]
         )
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_checkout_with_two_submodules(mkgitrepo, src):
+def test_checkout_with_two_submodules(mkgitrepo, src, git_allow_file_protocol):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a'
     and a submodule 'submodule_b' in it.
     """
 
     submodule_name = "submodule_a"
     submodule = mkgitrepo(submodule_name)
@@ -98,15 +98,17 @@
             ),
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_checkout_with_two_submodules_recursive(mkgitrepo, src):
+def test_checkout_with_two_submodules_recursive(
+    mkgitrepo, src, git_allow_file_protocol
+):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a'
     and a submodule 'submodule_b' in it.
     but this time we test it with the "recursive" option
     """
 
     submodule_name = "submodule_a"
@@ -141,15 +143,15 @@
             ("info", ("Cloned 'egg' with git from '%s'." % egg.url,), {}),
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_update_with_submodule(mkgitrepo, src):
+def test_update_with_submodule(mkgitrepo, src, git_allow_file_protocol):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it.
     Add a new 'submodule_b' to 'egg' and check it succesfully initializes.
     """
     submodule_name = "submodule_a"
     submodule = mkgitrepo(submodule_name)
     submodule.add_file("foo")
@@ -204,15 +206,15 @@
             ),
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_update_with_submodule_recursive(mkgitrepo, src):
+def test_update_with_submodule_recursive(mkgitrepo, src, git_allow_file_protocol):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it.
     Add a new 'submodule_b' to 'egg' and check it succesfully initializes.
     """
     submodule_name = "submodule_a"
     submodule = mkgitrepo(submodule_name)
     submodule.add_file("foo")
@@ -261,15 +263,15 @@
             ),
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_checkout_with_submodules_option_never(mkgitrepo, src):
+def test_checkout_with_submodules_option_never(mkgitrepo, src, git_allow_file_protocol):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it
     without initializing the submodule, restricted by global 'never'
     """
 
     submodule_name = "submodule_a"
     submodule_a = mkgitrepo(submodule_name)
@@ -293,15 +295,17 @@
             ("info", ("Cloned 'egg' with git from '%s'." % egg.url,), {})
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_checkout_with_submodules_option_never_source_always(mkgitrepo, src):
+def test_checkout_with_submodules_option_never_source_always(
+    mkgitrepo, src, git_allow_file_protocol
+):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it
     and a module 'egg2' with the same submodule, initializing only the submodule
     on egg that has the 'always' option
     """
 
     submodule_name = "submodule_a"
@@ -354,15 +358,17 @@
             ("info", ("Cloned 'egg2' with git from '%s'." % egg2.url,), {}),
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_checkout_with_submodules_option_always_source_never(mkgitrepo, src):
+def test_checkout_with_submodules_option_always_source_never(
+    mkgitrepo, src, git_allow_file_protocol
+):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it
     and a module 'egg2' with the same submodule, not initializing the submodule
     on egg2 that has the 'never' option
 
     """
 
@@ -414,15 +420,15 @@
             ("info", ("Cloned 'egg2' with git from '%s'." % egg2.url,), {}),
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_update_with_submodule_checkout(mkgitrepo, src):
+def test_update_with_submodule_checkout(mkgitrepo, src, git_allow_file_protocol):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it.
     Add a new 'submodule_b' to 'egg' and check it doesn't get initialized.
     """
 
     submodule_name = "submodule_a"
     submodule = mkgitrepo(submodule_name)
@@ -478,15 +484,17 @@
             ("info", ("Switching to branch 'master'.",), {}),
         ]
 
 
 @pytest.mark.skipif(
     condition=os.name == "nt", reason="submodules seem not to work on windows"
 )
-def test_update_with_submodule_dont_update_previous_submodules(mkgitrepo, src):
+def test_update_with_submodule_dont_update_previous_submodules(
+    mkgitrepo, src, git_allow_file_protocol
+):
     """
     Tests the checkout of a module 'egg' with a submodule 'submodule_a' in it.
     Commits changes in the detached submodule, and checks update didn't break
     the changes.
     """
 
     submodule_name = "submodule_a"
```

### Comparing `mxdev-4.0.2/src/mxdev/tests/test_including.py` & `mxdev-4.0.3/src/mxdev/tests/test_including.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/tests/test_mercurial.py` & `mxdev-4.0.3/src/mxdev/tests/test_mercurial.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/tests/test_svn.py` & `mxdev-4.0.3/src/mxdev/tests/test_svn.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/tests/utils.py` & `mxdev-4.0.3/src/mxdev/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
         if msg is None:
             msg = fname
         self(f"git commit {repo_file} -m {msg}", echo=False)
 
     def add_submodule(self, submodule: "GitRepo", submodule_name: str):
         assert isinstance(submodule, GitRepo)
         assert isinstance(submodule_name, str)
+
         self(f"git submodule add {submodule.url}")
         self("git add .gitmodules")
         self(f"git add {submodule_name}")
         self(f"git commit -m 'Add submodule {submodule_name}'")
 
     def add_branch(self, bname: str, msg: Union[str, None] = None):
         self(f"git checkout -b {bname}")
```

### Comparing `mxdev-4.0.2/src/mxdev/vcs/bazaar.py` & `mxdev-4.0.3/src/mxdev/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/vcs/common.py` & `mxdev-4.0.3/src/mxdev/vcs/common.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/vcs/darcs.py` & `mxdev-4.0.3/src/mxdev/vcs/darcs.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/vcs/filesystem.py` & `mxdev-4.0.3/src/mxdev/vcs/filesystem.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/vcs/git.py` & `mxdev-4.0.3/src/mxdev/vcs/git.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/vcs/gitsvn.py` & `mxdev-4.0.3/src/mxdev/vcs/gitsvn.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/vcs/mercurial.py` & `mxdev-4.0.3/src/mxdev/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev/vcs/svn.py` & `mxdev-4.0.3/src/mxdev/vcs/svn.py`

 * *Files identical despite different names*

### Comparing `mxdev-4.0.2/src/mxdev.egg-info/PKG-INFO` & `mxdev-4.0.3/src/mxdev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxdev
-Version: 4.0.2
+Version: 4.0.3
 Summary: Enable to work with Python projects containing lots of packages, of which you only want to develop some.
 Author-email: MX Stack Developers <dev@bluedynamics.com>
 License: BSD 2-Clause License
 Project-URL: Homepage, https://github.com/mxstack/mxdev
 Project-URL: Bug Reports, https://github.com/mxstack/mxdev/issues
 Project-URL: Source, https://github.com/mxstack/mxdev/
 Keywords: pip,vcs,git,development
@@ -148,14 +148,18 @@
     otherpackage==33.12.1
 ```
 
 It is possible to add as many overrides as needed.
 When writing the *constraints-out*, the new version will be taken into account.
 If there is a source section defined for the same package, the source will be used and entries here are ignored.
 
+Note: When using [uv](https://pypi.org/project/uv/) pip install the version overrides here are not needed, since it [supports overrides nativly](https://github.com/astral-sh/uv?tab=readme-ov-file#dependency-overrides).
+With uv it is recommended to create an `overrides.txt` file with the version overrides and use `uv pip install --overrides overrides.txt [..]` to install the packages.
+
+
 #### `ignores`
 
 Ignore packages that are already defined in a dependent constraints file.
 No new version will be provided.
 This is specifically handy if a package is going to be installed editable from local file system (like `-e .`), but was already pinned in an upstream constraints file.
 
 This can be defined as:
@@ -437,14 +441,21 @@
 
 Maintainers are Jens Klein and the [BlueDynamics Alliance](https://bluedynamics.com) developer team.
 
 We appreciate any contribution! If you have an idea, found a bug, want to drop us a question, or a release is needed, please just file an issue at the [mxdev issue tracker](https://github.com/bluedynamics/mxdev/issues).
 
 ## Changes
 
+## 4.0.3 (2024-05-17)
+
+
+- Fix #45: Packages with capital names do not get ignored when checked out.
+  [jensens]
+
+
 ## 4.0.2 (2024-03-13)
 
 - Fix #42: deprecated use of `pkg_resoures` to load entry points and parse requirements.
   This enables mxdev to work on Python 3.12, where `pkg_resources` is no longer installed by default in virtual_envs.
   [jensens]
 
 ## 4.0.1 (2024-03-01)
```

### Comparing `mxdev-4.0.2/src/mxdev.egg-info/SOURCES.txt` & `mxdev-4.0.3/src/mxdev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

