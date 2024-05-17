# Comparing `tmp/glabpkg-4.0.1.tar.gz` & `tmp/glabpkg-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glabpkg-4.0.1.tar", last modified: Fri May 17 07:55:20 2024, max compression
+gzip compressed data, was "glabpkg-4.1.0.tar", last modified: Fri May 17 09:34:20 2024, max compression
```

## Comparing `glabpkg-4.0.1.tar` & `glabpkg-4.1.0.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.069487 glabpkg-4.0.1/
--rw-rw-rw-   0        0        0      352 2024-05-17 07:49:45.000000 glabpkg-4.0.1/AUTHORS.rst
--rw-rw-rw-   0        0        0     3313 2024-05-17 07:49:45.000000 glabpkg-4.0.1/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2024-05-17 07:49:45.000000 glabpkg-4.0.1/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2024-05-17 07:49:45.000000 glabpkg-4.0.1/LICENSE
--rw-rw-rw-   0        0        0     3293 2024-05-17 07:55:20.066413 glabpkg-4.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2024-05-17 07:49:45.000000 glabpkg-4.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.979544 glabpkg-4.0.1/doc/
--rw-rw-rw-   0        0        0     6967 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/Makefile
--rw-rw-rw-   0        0        0       29 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.989382 glabpkg-4.0.1/doc/badges/
--rw-rw-rw-   0        0        0      282 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.989382 glabpkg-4.0.1/doc/biblio/
--rw-rw-rw-   0        0        0      513 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     4287 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/conf.py
--rw-rw-rw-   0        0        0       34 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/history.rst
--rw-rw-rw-   0        0        0      579 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/index.rst
--rw-rw-rw-   0        0        0      217 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/make.bat
--rw-rw-rw-   0        0        0      133 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/management.rst
--rw-rw-rw-   0        0        0     1491 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.989382 glabpkg-4.0.1/doc/user/
--rw-rw-rw-   0        0        0       86 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2024-05-17 07:49:45.000000 glabpkg-4.0.1/doc/user/overview.rst
--rw-rw-rw-   0        0        0     2788 2024-05-17 07:49:45.000000 glabpkg-4.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      277 2024-05-17 07:49:45.000000 glabpkg-4.0.1/requirements.txt
--rw-rw-rw-   0        0        0       44 2024-05-17 07:49:45.000000 glabpkg-4.0.1/requirements_minimal.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 07:55:20.069487 glabpkg-4.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.929626 glabpkg-4.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.989382 glabpkg-4.0.1/src/glabpkg/
--rw-rw-rw-   0        0        0      188 2024-05-17 07:49:45.000000 glabpkg-4.0.1/src/glabpkg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.999177 glabpkg-4.0.1/src/glabpkg/base/
--rw-rw-rw-   0        0        0        0 2020-02-06 17:37:05.000000 glabpkg-4.0.1/src/glabpkg/base/__init__.py
--rw-rw-rw-   0        0        0      853 2021-06-25 18:38:58.000000 glabpkg-4.0.1/src/glabpkg/base/option.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.007015 glabpkg-4.0.1/src/glabpkg/base/resource/
--rw-rw-rw-   0        0        0      434 2020-02-06 17:37:05.000000 glabpkg-4.0.1/src/glabpkg/base/resource/.gitattributes.tpl
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.939431 glabpkg-4.0.1/src/glabpkg/base/resource/.gitlab/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.009599 glabpkg-4.0.1/src/glabpkg/base/resource/.gitlab/issue_templates/
--rw-rw-rw-   0        0        0      160 2020-02-21 10:42:42.000000 glabpkg-4.0.1/src/glabpkg/base/resource/.gitlab/issue_templates/bug.md
--rw-rw-rw-   0        0        0      102 2020-02-21 10:42:42.000000 glabpkg-4.0.1/src/glabpkg/base/resource/.gitlab/issue_templates/feature.md
--rw-rw-rw-   0        0        0       53 2020-02-21 10:42:42.000000 glabpkg-4.0.1/src/glabpkg/base/resource/.gitlab/issue_templates/technical_task.md
--rw-rw-rw-   0        0        0      363 2021-08-26 14:10:46.000000 glabpkg-4.0.1/src/glabpkg/base/resource/.gitlab-ci.yml
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.009599 glabpkg-4.0.1/src/glabpkg/data/
--rw-rw-rw-   0        0        0        0 2021-07-06 09:14:59.000000 glabpkg-4.0.1/src/glabpkg/data/__init__.py
--rw-rw-rw-   0        0        0      332 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/data/option.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.939431 glabpkg-4.0.1/src/glabpkg/data/resource/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.009599 glabpkg-4.0.1/src/glabpkg/data/resource/raw/
--rw-rw-rw-   0        0        0      117 2021-07-06 09:14:59.000000 glabpkg-4.0.1/src/glabpkg/data/resource/raw/readme.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.009599 glabpkg-4.0.1/src/glabpkg/data/resource/script/
--rw-rw-rw-   0        0        0      122 2021-07-06 09:14:59.000000 glabpkg-4.0.1/src/glabpkg/data/resource/script/readme.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.939431 glabpkg-4.0.1/src/glabpkg/data/resource/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.009599 glabpkg-4.0.1/src/glabpkg/data/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0       65 2024-05-17 07:34:39.000000 glabpkg-4.0.1/src/glabpkg/data/resource/src/{{ base.pkgname }}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.009599 glabpkg-4.0.1/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/
--rw-rw-rw-   0        0        0      134 2021-07-06 09:14:59.000000 glabpkg-4.0.1/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/readme.rst
--rw-rw-rw-   0        0        0      379 2024-05-17 07:34:39.000000 glabpkg-4.0.1/src/glabpkg/data/resource/src/{{ base.pkgname }}/info.py.tpl
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.019462 glabpkg-4.0.1/src/glabpkg/data/resource/test/
--rw-rw-rw-   0        0        0      289 2024-05-17 07:29:47.000000 glabpkg-4.0.1/src/glabpkg/data/resource/test/test_packaging.py.tpl
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.019462 glabpkg-4.0.1/src/glabpkg/pkg/
--rw-rw-rw-   0        0        0        0 2021-06-25 14:18:59.000000 glabpkg-4.0.1/src/glabpkg/pkg/__init__.py
--rw-rw-rw-   0        0        0     1828 2024-01-03 18:35:00.000000 glabpkg-4.0.1/src/glabpkg/pkg/option.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:19.939431 glabpkg-4.0.1/src/glabpkg/pkg/resource/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.019462 glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.019462 glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/badges/
--rw-rw-rw-   0        0        0     1094 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg
--rw-rw-rw-   0        0        0     1090 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg
--rw-rw-rw-   0        0        0      172 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/badges/listing.rst
--rw-rw-rw-   0        0        0      184 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/installation.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.019462 glabpkg-4.0.1/src/glabpkg/pkg_dev/
--rw-rw-rw-   0        0        0        0 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-01-03 18:35:00.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/option.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.032404 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/
--rw-rw-rw-   0        0        0     1665 2024-03-14 15:29:53.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      444 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.040807 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/
--rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.040807 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/badges/
--rw-rw-rw-   0        0        0     1002 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg
--rw-rw-rw-   0        0        0      110 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.040807 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0       34 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/history.rst
--rw-rw-rw-   0        0        0      634 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/index.rst
--rw-rw-rw-   0        0        0      209 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/installation.rst
--rw-rw-rw-   0        0        0      133 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/management.rst
--rw-rw-rw-   0        0        0      557 2024-01-03 18:35:00.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.040807 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/user/
--rw-rw-rw-   0        0        0       86 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/user/overview.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.040807 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/example/
--rw-rw-rw-   0        0        0      254 2022-12-04 11:33:38.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/example/readme.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.049404 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/test/
--rw-rw-rw-   0        0        0      148 2024-05-17 06:30:12.000000 glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/test/test_packaging.py.tpl
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.049404 glabpkg-4.0.1/src/glabpkg/report/
--rw-rw-rw-   0        0        0        0 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/__init__.py
--rw-rw-rw-   0        0        0     1559 2024-01-03 18:35:00.000000 glabpkg-4.0.1/src/glabpkg/report/option.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.049404 glabpkg-4.0.1/src/glabpkg/report/resource/
--rw-rw-rw-   0        0        0      949 2023-03-09 14:37:10.000000 glabpkg-4.0.1/src/glabpkg/report/resource/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      923 2022-03-28 12:29:45.000000 glabpkg-4.0.1/src/glabpkg/report/resource/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.049404 glabpkg-4.0.1/src/glabpkg/report/resource/report/
--rw-rw-rw-   0        0        0       51 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/report/authors.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.059229 glabpkg-4.0.1/src/glabpkg/report/resource/report/badges/
--rw-rw-rw-   0        0        0     1001 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/report/badges/badge_doc.svg
--rw-rw-rw-   0        0        0      109 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/report/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.062901 glabpkg-4.0.1/src/glabpkg/report/resource/report/biblio/
--rw-rw-rw-   0        0        0      513 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/report/biblio/biblio.rst
--rw-rw-rw-   0        0        0      130 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/report/conf.py.tpl
--rw-rw-rw-   0        0        0      376 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/report/index.rst
--rw-rw-rw-   0        0        0       89 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/report/introduction.rst
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.062901 glabpkg-4.0.1/src/glabpkg/report/resource/script/
--rw-rw-rw-   0        0        0       56 2021-07-06 09:29:24.000000 glabpkg-4.0.1/src/glabpkg/report/resource/script/readme.rst
--rw-rw-rw-   0        0        0      367 2024-05-17 07:49:45.000000 glabpkg-4.0.1/src/glabpkg/version.py
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.066413 glabpkg-4.0.1/src/glabpkg.egg-info/
--rw-rw-rw-   0        0        0     3293 2024-05-17 07:55:19.000000 glabpkg-4.0.1/src/glabpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3069 2024-05-17 07:55:19.000000 glabpkg-4.0.1/src/glabpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 07:55:19.000000 glabpkg-4.0.1/src/glabpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      250 2024-05-17 07:55:19.000000 glabpkg-4.0.1/src/glabpkg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2024-05-17 07:55:19.000000 glabpkg-4.0.1/src/glabpkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-17 07:55:19.000000 glabpkg-4.0.1/src/glabpkg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-17 07:55:20.066413 glabpkg-4.0.1/test/
--rw-rw-rw-   0        0        0      983 2024-05-17 07:49:45.000000 glabpkg-4.0.1/test/conftest.py
--rw-rw-rw-   0        0        0      114 2024-05-17 07:49:45.000000 glabpkg-4.0.1/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.473752 glabpkg-4.1.0/
+-rw-rw-rw-   0        0        0      352 2024-05-17 09:28:49.000000 glabpkg-4.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3313 2024-05-17 09:28:49.000000 glabpkg-4.1.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-17 09:28:49.000000 glabpkg-4.1.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-17 09:28:49.000000 glabpkg-4.1.0/LICENSE
+-rw-rw-rw-   0        0        0     3293 2024-05-17 09:34:20.472751 glabpkg-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2024-05-17 09:28:49.000000 glabpkg-4.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.389491 glabpkg-4.1.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.390491 glabpkg-4.1.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.391491 glabpkg-4.1.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     4287 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/history.rst
+-rw-rw-rw-   0        0        0      579 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/index.rst
+-rw-rw-rw-   0        0        0      217 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1491 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.394523 glabpkg-4.1.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-17 09:28:49.000000 glabpkg-4.1.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2788 2024-05-17 09:28:49.000000 glabpkg-4.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      277 2024-05-17 09:28:49.000000 glabpkg-4.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       44 2024-05-17 09:28:49.000000 glabpkg-4.1.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 09:34:20.473752 glabpkg-4.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.339492 glabpkg-4.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.397491 glabpkg-4.1.0/src/glabpkg/
+-rw-rw-rw-   0        0        0      188 2024-05-17 09:28:49.000000 glabpkg-4.1.0/src/glabpkg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.405491 glabpkg-4.1.0/src/glabpkg/base/
+-rw-rw-rw-   0        0        0        0 2020-02-06 17:37:05.000000 glabpkg-4.1.0/src/glabpkg/base/__init__.py
+-rw-rw-rw-   0        0        0      853 2021-06-25 18:38:58.000000 glabpkg-4.1.0/src/glabpkg/base/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.408053 glabpkg-4.1.0/src/glabpkg/base/resource/
+-rw-rw-rw-   0        0        0      434 2020-02-06 17:37:05.000000 glabpkg-4.1.0/src/glabpkg/base/resource/.gitattributes.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.341491 glabpkg-4.1.0/src/glabpkg/base/resource/.gitlab/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.412262 glabpkg-4.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/
+-rw-rw-rw-   0        0        0      160 2020-02-21 10:42:42.000000 glabpkg-4.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/bug.md
+-rw-rw-rw-   0        0        0      102 2020-02-21 10:42:42.000000 glabpkg-4.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/feature.md
+-rw-rw-rw-   0        0        0       53 2020-02-21 10:42:42.000000 glabpkg-4.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/technical_task.md
+-rw-rw-rw-   0        0        0      363 2021-08-26 14:10:46.000000 glabpkg-4.1.0/src/glabpkg/base/resource/.gitlab-ci.yml
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.416258 glabpkg-4.1.0/src/glabpkg/data/
+-rw-rw-rw-   0        0        0        0 2021-07-06 09:14:59.000000 glabpkg-4.1.0/src/glabpkg/data/__init__.py
+-rw-rw-rw-   0        0        0      332 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/data/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.349491 glabpkg-4.1.0/src/glabpkg/data/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.417258 glabpkg-4.1.0/src/glabpkg/data/resource/raw/
+-rw-rw-rw-   0        0        0      117 2021-07-06 09:14:59.000000 glabpkg-4.1.0/src/glabpkg/data/resource/raw/readme.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.418259 glabpkg-4.1.0/src/glabpkg/data/resource/script/
+-rw-rw-rw-   0        0        0      122 2021-07-06 09:14:59.000000 glabpkg-4.1.0/src/glabpkg/data/resource/script/readme.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.348518 glabpkg-4.1.0/src/glabpkg/data/resource/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.421461 glabpkg-4.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0       65 2024-05-17 07:34:39.000000 glabpkg-4.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.422386 glabpkg-4.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/
+-rw-rw-rw-   0        0        0      134 2021-07-06 09:14:59.000000 glabpkg-4.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/readme.rst
+-rw-rw-rw-   0        0        0      379 2024-05-17 07:34:39.000000 glabpkg-4.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/info.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.424078 glabpkg-4.1.0/src/glabpkg/data/resource/test/
+-rw-rw-rw-   0        0        0      289 2024-05-17 07:29:47.000000 glabpkg-4.1.0/src/glabpkg/data/resource/test/test_packaging.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.426157 glabpkg-4.1.0/src/glabpkg/pkg/
+-rw-rw-rw-   0        0        0        0 2021-06-25 14:18:59.000000 glabpkg-4.1.0/src/glabpkg/pkg/__init__.py
+-rw-rw-rw-   0        0        0     1828 2024-01-03 18:35:00.000000 glabpkg-4.1.0/src/glabpkg/pkg/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.350490 glabpkg-4.1.0/src/glabpkg/pkg/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.428158 glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.432160 glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/badges/
+-rw-rw-rw-   0        0        0     1094 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg
+-rw-rw-rw-   0        0        0     1090 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg
+-rw-rw-rw-   0        0        0      172 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/badges/listing.rst
+-rw-rw-rw-   0        0        0      184 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/installation.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.434157 glabpkg-4.1.0/src/glabpkg/pkg_dev/
+-rw-rw-rw-   0        0        0        0 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-01-03 18:35:00.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.436939 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/
+-rw-rw-rw-   0        0        0     1665 2024-03-14 15:29:53.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      444 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.447982 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/
+-rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.449983 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/badges/
+-rw-rw-rw-   0        0        0      984 2024-05-17 09:27:13.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg
+-rw-rw-rw-   0        0        0      110 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.450522 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0       34 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/history.rst
+-rw-rw-rw-   0        0        0      634 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/index.rst
+-rw-rw-rw-   0        0        0      209 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/installation.rst
+-rw-rw-rw-   0        0        0      133 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/management.rst
+-rw-rw-rw-   0        0        0      557 2024-01-03 18:35:00.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.452436 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/user/
+-rw-rw-rw-   0        0        0       86 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/user/overview.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.453435 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/example/
+-rw-rw-rw-   0        0        0      254 2022-12-04 11:33:38.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/example/readme.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.454732 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/test/
+-rw-rw-rw-   0        0        0      148 2024-05-17 06:30:12.000000 glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/test/test_packaging.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.456750 glabpkg-4.1.0/src/glabpkg/report/
+-rw-rw-rw-   0        0        0        0 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/__init__.py
+-rw-rw-rw-   0        0        0     1559 2024-01-03 18:35:00.000000 glabpkg-4.1.0/src/glabpkg/report/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.459751 glabpkg-4.1.0/src/glabpkg/report/resource/
+-rw-rw-rw-   0        0        0      949 2023-03-09 14:37:10.000000 glabpkg-4.1.0/src/glabpkg/report/resource/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      923 2022-03-28 12:29:45.000000 glabpkg-4.1.0/src/glabpkg/report/resource/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.464751 glabpkg-4.1.0/src/glabpkg/report/resource/report/
+-rw-rw-rw-   0        0        0       51 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/report/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.466751 glabpkg-4.1.0/src/glabpkg/report/resource/report/badges/
+-rw-rw-rw-   0        0        0     1001 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/report/badges/badge_doc.svg
+-rw-rw-rw-   0        0        0      109 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/report/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.467751 glabpkg-4.1.0/src/glabpkg/report/resource/report/biblio/
+-rw-rw-rw-   0        0        0      513 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/report/biblio/biblio.rst
+-rw-rw-rw-   0        0        0      130 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/report/conf.py.tpl
+-rw-rw-rw-   0        0        0      376 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/report/index.rst
+-rw-rw-rw-   0        0        0       89 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/report/introduction.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.468750 glabpkg-4.1.0/src/glabpkg/report/resource/script/
+-rw-rw-rw-   0        0        0       56 2021-07-06 09:29:24.000000 glabpkg-4.1.0/src/glabpkg/report/resource/script/readme.rst
+-rw-rw-rw-   0        0        0      367 2024-05-17 09:28:49.000000 glabpkg-4.1.0/src/glabpkg/version.py
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.471751 glabpkg-4.1.0/src/glabpkg.egg-info/
+-rw-rw-rw-   0        0        0     3293 2024-05-17 09:34:20.000000 glabpkg-4.1.0/src/glabpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3069 2024-05-17 09:34:20.000000 glabpkg-4.1.0/src/glabpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 09:34:20.000000 glabpkg-4.1.0/src/glabpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      250 2024-05-17 09:34:20.000000 glabpkg-4.1.0/src/glabpkg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-05-17 09:34:20.000000 glabpkg-4.1.0/src/glabpkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 09:34:20.000000 glabpkg-4.1.0/src/glabpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 09:34:20.470752 glabpkg-4.1.0/test/
+-rw-rw-rw-   0        0        0      983 2024-05-17 09:28:49.000000 glabpkg-4.1.0/test/conftest.py
+-rw-rw-rw-   0        0        0      114 2024-05-17 09:28:49.000000 glabpkg-4.1.0/test/test_packaging.py
```

### Comparing `glabpkg-4.0.1/CONTRIBUTING.rst` & `glabpkg-4.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/LICENSE` & `glabpkg-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/PKG-INFO` & `glabpkg-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: glabpkg
-Version: 4.0.1
+Version: 4.1.0
 Summary: template for python packages hosted on gitlab
 Author-email: revesansparole <revesansparole@gmail.com>
 Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>, jchopard <jerome.chopard@itk.fr>
 License: cc_by_nc
 Project-URL: repository, https://gitlab.com/revesansparole/glabpkg
-Project-URL: pip, https://pypi.org/project/glabpkg/4.0.1/
+Project-URL: pip, https://pypi.org/project/glabpkg/4.1.0/
 Project-URL: conda, https://anaconda.org/revesansparole/glabpkg
 Project-URL: doc, https://revesansparole.gitlab.io/glabpkg/
 Project-URL: pypi, https://badge.fury.io/py/glabpkg
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -42,15 +42,15 @@
 glabpkg
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/4.0.1/
+    :target: https://pypi.org/project/glabpkg/4.1.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-4.0.1/README.rst` & `glabpkg-4.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 glabpkg
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/4.0.1/
+    :target: https://pypi.org/project/glabpkg/4.1.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-4.0.1/doc/Makefile` & `glabpkg-4.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/doc/biblio/biblio.rst` & `glabpkg-4.1.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/doc/conf.py` & `glabpkg-4.1.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "4.0.1"
+version = "4.1.0"
 # The full version, including alpha/beta/rc tags.
-release = "4.0.1"
+release = "4.1.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `glabpkg-4.0.1/doc/index.rst` & `glabpkg-4.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/doc/make.bat` & `glabpkg-4.1.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/doc/readme.rst` & `glabpkg-4.1.0/doc/readme.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Overview
 ========
 
 .. {# pkglts, glabpkg_dev
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/4.0.1/
+    :target: https://pypi.org/project/glabpkg/4.1.0/
 
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
```

### Comparing `glabpkg-4.0.1/pyproject.toml` & `glabpkg-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 requires = ["setuptools", "wheel"]  # , "setuptools-scm"]  # PEP 508 specifications.
 build-backend = "setuptools.build_meta"  # we don't know if we need it
 # #}
 
 # {# pkglts, pyproject.project
 [project]  # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 name = "glabpkg"
-version = "4.0.1"
+version = "4.1.0"
 description = "template for python packages hosted on gitlab"
 readme = "README.rst"
 requires-python = ">= 3.7"
 license = {text = "cc_by_nc"}
 authors = [
     {name = "revesansparole", email = "revesansparole@gmail.com"},
 ]
@@ -55,15 +55,15 @@
     "pytest-cov",
     "pytest-mock",
 ]
 
 
 [project.urls]
 repository = "https://gitlab.com/revesansparole/glabpkg"
-pip = "https://pypi.org/project/glabpkg/4.0.1/"
+pip = "https://pypi.org/project/glabpkg/4.1.0/"
 conda = "https://anaconda.org/revesansparole/glabpkg"
 doc = "https://revesansparole.gitlab.io/glabpkg/"
 pypi = "https://badge.fury.io/py/glabpkg"
 
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `glabpkg-4.0.1/src/glabpkg/base/option.py` & `glabpkg-4.1.0/src/glabpkg/base/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg/option.py` & `glabpkg-4.1.0/src/glabpkg/pkg/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg` & `glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg` & `glabpkg-4.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg_dev/option.py` & `glabpkg-4.1.0/src/glabpkg/pkg_dev/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml` & `glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg` & `glabpkg-4.1.0/src/glabpkg/report/resource/report/badges/badge_doc.svg`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<!-- {# pkglts, glabpkg_dev -->
+<!-- {# pkglts, glabreport -->
 <svg xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink" width="86" height="20">
     <linearGradient id="b" x2="0" y2="100%">
         <stop offset="0" stop-color="#bbb" stop-opacity=".1"/>
         <stop offset="1" stop-opacity=".1"/>
     </linearGradient>
     <clipPath id="a">
```

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst` & `glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/index.rst` & `glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/index.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/pkg_dev/resource/doc/readme.rst` & `glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/readme.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/report/option.py` & `glabpkg-4.1.0/src/glabpkg/report/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/report/resource/.gitlab-ci.yml` & `glabpkg-4.1.0/src/glabpkg/report/resource/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/report/resource/README.rst` & `glabpkg-4.1.0/src/glabpkg/report/resource/README.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg/report/resource/report/badges/badge_doc.svg` & `glabpkg-4.1.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-<!-- {# pkglts, glabreport -->
+<!-- {# pkglts, glabpkg_dev -->
 <svg xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink" width="86" height="20">
     <linearGradient id="b" x2="0" y2="100%">
         <stop offset="0" stop-color="#bbb" stop-opacity=".1"/>
         <stop offset="1" stop-opacity=".1"/>
     </linearGradient>
     <clipPath id="a">
-        <rect width="86" height="20" rx="3" fill="#fff"/>
+        <rect width="56" height="20" rx="3" fill="#fff"/>
     </clipPath>
     <g clip-path="url(#a)">
-        <path fill="#555" d="M0 0h35v20H0z"/>
-        <path fill="#4c1" d="M35 0h51v20H35z"/>
-        <path fill="url(#b)" d="M0 0h86v20H0z"/>
+        <path fill="#555" d="M0 0h36v20H0z"/>
+        <path fill="#4c1" d="M36 0h20v20H36z"/>
+        <path fill="url(#b)" d="M0 0h56v20H0z"/>
     </g>
     <g fill="#fff" text-anchor="middle"
        font-family="DejaVu Sans,Verdana,Geneva,sans-serif" font-size="11">
-        <text x="17.5" y="15" fill="#010101" fill-opacity=".3">docs</text>
-        <text x="17.5" y="14">docs</text>
-        <text x="59.5" y="15" fill="#010101" fill-opacity=".3">passing</text>
-        <text x="59.5" y="14">passing</text>
+        <text x="18" y="15" fill="#010101" fill-opacity=".3">docs</text>
+        <text x="18" y="14">docs</text>
+        <text x="46" y="15" fill="#010101" fill-opacity=".3">go</text>
+        <text x="46" y="14">go</text>
     </g>
 </svg>
 <!-- #} -->
```

### Comparing `glabpkg-4.0.1/src/glabpkg/report/resource/report/biblio/biblio.rst` & `glabpkg-4.1.0/src/glabpkg/report/resource/report/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/src/glabpkg.egg-info/PKG-INFO` & `glabpkg-4.1.0/src/glabpkg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: glabpkg
-Version: 4.0.1
+Version: 4.1.0
 Summary: template for python packages hosted on gitlab
 Author-email: revesansparole <revesansparole@gmail.com>
 Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>, jchopard <jerome.chopard@itk.fr>
 License: cc_by_nc
 Project-URL: repository, https://gitlab.com/revesansparole/glabpkg
-Project-URL: pip, https://pypi.org/project/glabpkg/4.0.1/
+Project-URL: pip, https://pypi.org/project/glabpkg/4.1.0/
 Project-URL: conda, https://anaconda.org/revesansparole/glabpkg
 Project-URL: doc, https://revesansparole.gitlab.io/glabpkg/
 Project-URL: pypi, https://badge.fury.io/py/glabpkg
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
@@ -42,15 +42,15 @@
 glabpkg
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/4.0.1/
+    :target: https://pypi.org/project/glabpkg/4.1.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-4.0.1/src/glabpkg.egg-info/SOURCES.txt` & `glabpkg-4.1.0/src/glabpkg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glabpkg-4.0.1/test/conftest.py` & `glabpkg-4.1.0/test/conftest.py`

 * *Files identical despite different names*

