# Comparing `tmp/glabpkg-3.1.0.tar.gz` & `tmp/glabpkg-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glabpkg-3.1.0.tar", last modified: Thu Mar 14 15:35:39 2024, max compression
+gzip compressed data, was "glabpkg-4.0.0.tar", last modified: Fri May 17 07:05:45 2024, max compression
```

## Comparing `glabpkg-3.1.0.tar` & `glabpkg-4.0.0.tar`

### file list

```diff
@@ -1,138 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.942362 glabpkg-3.1.0/
--rw-rw-rw-   0        0        0      352 2024-03-14 15:30:21.000000 glabpkg-3.1.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     3313 2024-03-14 15:30:21.000000 glabpkg-3.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      106 2024-03-14 15:30:21.000000 glabpkg-3.1.0/HISTORY.rst
--rw-rw-rw-   0        0        0    20838 2024-03-14 15:30:21.000000 glabpkg-3.1.0/LICENSE
--rw-rw-rw-   0        0        0     3293 2024-03-14 15:35:39.941318 glabpkg-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2024-03-14 15:30:21.000000 glabpkg-3.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.835076 glabpkg-3.1.0/doc/
--rw-rw-rw-   0        0        0     6967 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/Makefile
--rw-rw-rw-   0        0        0       29 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.836035 glabpkg-3.1.0/doc/badges/
--rw-rw-rw-   0        0        0      282 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.838035 glabpkg-3.1.0/doc/biblio/
--rw-rw-rw-   0        0        0      513 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0     4287 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/conf.py
--rw-rw-rw-   0        0        0       34 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/history.rst
--rw-rw-rw-   0        0        0      579 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/index.rst
--rw-rw-rw-   0        0        0      217 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/installation.rst
--rwxrwxrwx   0        0        0     6731 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/make.bat
--rw-rw-rw-   0        0        0      133 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/management.rst
--rw-rw-rw-   0        0        0     1491 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.840657 glabpkg-3.1.0/doc/user/
--rw-rw-rw-   0        0        0       86 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2024-03-14 15:30:21.000000 glabpkg-3.1.0/doc/user/overview.rst
--rw-rw-rw-   0        0        0     2848 2024-03-14 15:30:21.000000 glabpkg-3.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      277 2024-03-14 15:30:21.000000 glabpkg-3.1.0/requirements.txt
--rw-rw-rw-   0        0        0       44 2024-03-14 15:30:21.000000 glabpkg-3.1.0/requirements_minimal.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 15:35:39.942362 glabpkg-3.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.780325 glabpkg-3.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.843784 glabpkg-3.1.0/src/glabpkg/
--rw-rw-rw-   0        0        0      188 2024-03-14 15:30:21.000000 glabpkg-3.1.0/src/glabpkg/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.856181 glabpkg-3.1.0/src/glabpkg/base/
--rw-rw-rw-   0        0        0        0 2020-02-06 17:37:05.000000 glabpkg-3.1.0/src/glabpkg/base/__init__.py
--rw-rw-rw-   0        0        0      853 2021-06-25 18:38:58.000000 glabpkg-3.1.0/src/glabpkg/base/option.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.858776 glabpkg-3.1.0/src/glabpkg/base/resource/
--rw-rw-rw-   0        0        0      434 2020-02-06 17:37:05.000000 glabpkg-3.1.0/src/glabpkg/base/resource/.gitattributes.tpl
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.782471 glabpkg-3.1.0/src/glabpkg/base/resource/.gitlab/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.864006 glabpkg-3.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/
--rw-rw-rw-   0        0        0      160 2020-02-21 10:42:42.000000 glabpkg-3.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/bug.md
--rw-rw-rw-   0        0        0      102 2020-02-21 10:42:42.000000 glabpkg-3.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/feature.md
--rw-rw-rw-   0        0        0       53 2020-02-21 10:42:42.000000 glabpkg-3.1.0/src/glabpkg/base/resource/.gitlab/issue_templates/technical_task.md
--rw-rw-rw-   0        0        0      363 2021-08-26 14:10:46.000000 glabpkg-3.1.0/src/glabpkg/base/resource/.gitlab-ci.yml
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.866071 glabpkg-3.1.0/src/glabpkg/data/
--rw-rw-rw-   0        0        0        0 2021-07-06 09:14:59.000000 glabpkg-3.1.0/src/glabpkg/data/__init__.py
--rw-rw-rw-   0        0        0      332 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/data/option.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.784023 glabpkg-3.1.0/src/glabpkg/data/resource/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.867115 glabpkg-3.1.0/src/glabpkg/data/resource/script/
--rw-rw-rw-   0        0        0      122 2021-07-06 09:14:59.000000 glabpkg-3.1.0/src/glabpkg/data/resource/script/readme.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.784985 glabpkg-3.1.0/src/glabpkg/data/resource/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.871275 glabpkg-3.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0       82 2021-07-06 09:14:59.000000 glabpkg-3.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.872319 glabpkg-3.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/
--rw-rw-rw-   0        0        0      134 2021-07-06 09:14:59.000000 glabpkg-3.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/readme.rst
--rw-rw-rw-   0        0        0      193 2021-07-06 09:14:59.000000 glabpkg-3.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/info.py.tpl
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.873877 glabpkg-3.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/raw/
--rw-rw-rw-   0        0        0      117 2021-07-06 09:14:59.000000 glabpkg-3.1.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/raw/readme.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.875877 glabpkg-3.1.0/src/glabpkg/data_alt/
--rw-rw-rw-   0        0        0        0 2022-01-13 14:44:45.000000 glabpkg-3.1.0/src/glabpkg/data_alt/__init__.py
--rw-rw-rw-   0        0        0      331 2022-01-13 14:44:45.000000 glabpkg-3.1.0/src/glabpkg/data_alt/option.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.788047 glabpkg-3.1.0/src/glabpkg/data_alt/resource/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.876912 glabpkg-3.1.0/src/glabpkg/data_alt/resource/script/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.877876 glabpkg-3.1.0/src/glabpkg/data_alt/resource/script/raw/
--rw-rw-rw-   0        0        0      117 2022-01-13 14:44:45.000000 glabpkg-3.1.0/src/glabpkg/data_alt/resource/script/raw/readme.rst
--rw-rw-rw-   0        0        0      122 2022-01-13 14:44:45.000000 glabpkg-3.1.0/src/glabpkg/data_alt/resource/script/readme.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.789149 glabpkg-3.1.0/src/glabpkg/data_alt/resource/src/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.881564 glabpkg-3.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/
--rw-rw-rw-   0        0        0       73 2022-01-13 14:44:45.000000 glabpkg-3.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/__init__.py.tpl
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.882602 glabpkg-3.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/clean/
--rw-rw-rw-   0        0        0      134 2022-01-13 14:44:45.000000 glabpkg-3.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/clean/readme.rst
--rw-rw-rw-   0        0        0      152 2022-01-13 14:44:45.000000 glabpkg-3.1.0/src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/info.py.tpl
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.885222 glabpkg-3.1.0/src/glabpkg/pkg/
--rw-rw-rw-   0        0        0        0 2021-06-25 14:18:59.000000 glabpkg-3.1.0/src/glabpkg/pkg/__init__.py
--rw-rw-rw-   0        0        0     1828 2024-01-03 18:35:00.000000 glabpkg-3.1.0/src/glabpkg/pkg/option.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.793063 glabpkg-3.1.0/src/glabpkg/pkg/resource/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.887238 glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.890982 glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/badges/
--rw-rw-rw-   0        0        0     1094 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg
--rw-rw-rw-   0        0        0     1090 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg
--rw-rw-rw-   0        0        0      172 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/badges/listing.rst
--rw-rw-rw-   0        0        0      184 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/installation.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.893067 glabpkg-3.1.0/src/glabpkg/pkg_dev/
--rw-rw-rw-   0        0        0        0 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-01-03 18:35:00.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/option.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.896257 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/
--rw-rw-rw-   0        0        0     1665 2024-03-14 15:29:53.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      444 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.908778 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/
--rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/authors.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.910867 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/badges/
--rw-rw-rw-   0        0        0     1002 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg
--rw-rw-rw-   0        0        0      110 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.912979 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/
--rw-rw-rw-   0        0        0      513 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst
--rw-rw-rw-   0        0        0       34 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/contributing.rst
--rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/history.rst
--rw-rw-rw-   0        0        0      634 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/index.rst
--rw-rw-rw-   0        0        0      209 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/installation.rst
--rw-rw-rw-   0        0        0      133 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/management.rst
--rw-rw-rw-   0        0        0      557 2024-01-03 18:35:00.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/readme.rst
--rw-rw-rw-   0        0        0       21 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/usage.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.916171 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/user/
--rw-rw-rw-   0        0        0       86 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/user/index.rst
--rw-rw-rw-   0        0        0       66 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/user/overview.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.917231 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/example/
--rw-rw-rw-   0        0        0      254 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/example/readme.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.918175 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/test/
--rw-rw-rw-   0        0        0      114 2022-12-04 11:33:38.000000 glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/test/test_packaging.py.tpl
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.921323 glabpkg-3.1.0/src/glabpkg/report/
--rw-rw-rw-   0        0        0        0 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/__init__.py
--rw-rw-rw-   0        0        0     1559 2024-01-03 18:35:00.000000 glabpkg-3.1.0/src/glabpkg/report/option.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.923406 glabpkg-3.1.0/src/glabpkg/report/resource/
--rw-rw-rw-   0        0        0      949 2023-03-09 14:37:10.000000 glabpkg-3.1.0/src/glabpkg/report/resource/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      923 2022-03-28 12:29:45.000000 glabpkg-3.1.0/src/glabpkg/report/resource/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.928178 glabpkg-3.1.0/src/glabpkg/report/resource/report/
--rw-rw-rw-   0        0        0       51 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/report/authors.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.932715 glabpkg-3.1.0/src/glabpkg/report/resource/report/badges/
--rw-rw-rw-   0        0        0     1001 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/report/badges/badge_doc.svg
--rw-rw-rw-   0        0        0      109 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/report/badges/listing.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.933915 glabpkg-3.1.0/src/glabpkg/report/resource/report/biblio/
--rw-rw-rw-   0        0        0      513 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/report/biblio/biblio.rst
--rw-rw-rw-   0        0        0      130 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/report/conf.py.tpl
--rw-rw-rw-   0        0        0      376 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/report/index.rst
--rw-rw-rw-   0        0        0       89 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/report/introduction.rst
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.935005 glabpkg-3.1.0/src/glabpkg/report/resource/script/
--rw-rw-rw-   0        0        0       56 2021-07-06 09:29:24.000000 glabpkg-3.1.0/src/glabpkg/report/resource/script/readme.rst
--rw-rw-rw-   0        0        0      367 2024-03-14 15:30:21.000000 glabpkg-3.1.0/src/glabpkg/version.py
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.939222 glabpkg-3.1.0/src/glabpkg.egg-info/
--rw-rw-rw-   0        0        0     3293 2024-03-14 15:35:39.000000 glabpkg-3.1.0/src/glabpkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3407 2024-03-14 15:35:39.000000 glabpkg-3.1.0/src/glabpkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 15:35:39.000000 glabpkg-3.1.0/src/glabpkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      307 2024-03-14 15:35:39.000000 glabpkg-3.1.0/src/glabpkg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      106 2024-03-14 15:35:39.000000 glabpkg-3.1.0/src/glabpkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-14 15:35:39.000000 glabpkg-3.1.0/src/glabpkg.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 15:35:39.938167 glabpkg-3.1.0/test/
--rw-rw-rw-   0        0        0      983 2024-03-14 15:30:21.000000 glabpkg-3.1.0/test/conftest.py
--rw-rw-rw-   0        0        0       80 2024-03-14 15:30:21.000000 glabpkg-3.1.0/test/test_packaging.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.163276 glabpkg-4.0.0/
+-rw-rw-rw-   0        0        0      352 2024-05-17 07:04:14.000000 glabpkg-4.0.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3313 2024-05-17 07:04:14.000000 glabpkg-4.0.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      106 2024-05-17 07:04:14.000000 glabpkg-4.0.0/HISTORY.rst
+-rw-rw-rw-   0        0        0    20838 2024-05-17 07:04:14.000000 glabpkg-4.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3293 2024-05-17 07:05:45.160912 glabpkg-4.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2024-05-17 07:04:56.000000 glabpkg-4.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.078353 glabpkg-4.0.0/doc/
+-rw-rw-rw-   0        0        0     6967 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/Makefile
+-rw-rw-rw-   0        0        0       29 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.080406 glabpkg-4.0.0/doc/badges/
+-rw-rw-rw-   0        0        0      282 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.080406 glabpkg-4.0.0/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0     4287 2024-05-17 07:04:56.000000 glabpkg-4.0.0/doc/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/history.rst
+-rw-rw-rw-   0        0        0      579 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/index.rst
+-rw-rw-rw-   0        0        0      217 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/installation.rst
+-rwxrwxrwx   0        0        0     6731 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/make.bat
+-rw-rw-rw-   0        0        0      133 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/management.rst
+-rw-rw-rw-   0        0        0     1491 2024-05-17 07:04:56.000000 glabpkg-4.0.0/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.080406 glabpkg-4.0.0/doc/user/
+-rw-rw-rw-   0        0        0       86 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2024-05-17 07:04:14.000000 glabpkg-4.0.0/doc/user/overview.rst
+-rw-rw-rw-   0        0        0     2788 2024-05-17 07:04:56.000000 glabpkg-4.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      277 2024-05-17 07:04:14.000000 glabpkg-4.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       44 2024-05-17 07:04:14.000000 glabpkg-4.0.0/requirements_minimal.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 07:05:45.163276 glabpkg-4.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.029922 glabpkg-4.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.080406 glabpkg-4.0.0/src/glabpkg/
+-rw-rw-rw-   0        0        0      188 2024-05-17 07:04:14.000000 glabpkg-4.0.0/src/glabpkg/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.090475 glabpkg-4.0.0/src/glabpkg/base/
+-rw-rw-rw-   0        0        0        0 2020-02-06 17:37:05.000000 glabpkg-4.0.0/src/glabpkg/base/__init__.py
+-rw-rw-rw-   0        0        0      853 2021-06-25 18:38:58.000000 glabpkg-4.0.0/src/glabpkg/base/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.098518 glabpkg-4.0.0/src/glabpkg/base/resource/
+-rw-rw-rw-   0        0        0      434 2020-02-06 17:37:05.000000 glabpkg-4.0.0/src/glabpkg/base/resource/.gitattributes.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.029922 glabpkg-4.0.0/src/glabpkg/base/resource/.gitlab/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.100538 glabpkg-4.0.0/src/glabpkg/base/resource/.gitlab/issue_templates/
+-rw-rw-rw-   0        0        0      160 2020-02-21 10:42:42.000000 glabpkg-4.0.0/src/glabpkg/base/resource/.gitlab/issue_templates/bug.md
+-rw-rw-rw-   0        0        0      102 2020-02-21 10:42:42.000000 glabpkg-4.0.0/src/glabpkg/base/resource/.gitlab/issue_templates/feature.md
+-rw-rw-rw-   0        0        0       53 2020-02-21 10:42:42.000000 glabpkg-4.0.0/src/glabpkg/base/resource/.gitlab/issue_templates/technical_task.md
+-rw-rw-rw-   0        0        0      363 2021-08-26 14:10:46.000000 glabpkg-4.0.0/src/glabpkg/base/resource/.gitlab-ci.yml
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.103366 glabpkg-4.0.0/src/glabpkg/data/
+-rw-rw-rw-   0        0        0        0 2021-07-06 09:14:59.000000 glabpkg-4.0.0/src/glabpkg/data/__init__.py
+-rw-rw-rw-   0        0        0      332 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/data/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.040040 glabpkg-4.0.0/src/glabpkg/data/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.103366 glabpkg-4.0.0/src/glabpkg/data/resource/raw/
+-rw-rw-rw-   0        0        0      117 2021-07-06 09:14:59.000000 glabpkg-4.0.0/src/glabpkg/data/resource/raw/readme.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.103366 glabpkg-4.0.0/src/glabpkg/data/resource/script/
+-rw-rw-rw-   0        0        0      122 2021-07-06 09:14:59.000000 glabpkg-4.0.0/src/glabpkg/data/resource/script/readme.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.040040 glabpkg-4.0.0/src/glabpkg/data/resource/src/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.108491 glabpkg-4.0.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/
+-rw-rw-rw-   0        0        0       82 2021-07-06 09:14:59.000000 glabpkg-4.0.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/__init__.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.108491 glabpkg-4.0.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/
+-rw-rw-rw-   0        0        0      134 2021-07-06 09:14:59.000000 glabpkg-4.0.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/readme.rst
+-rw-rw-rw-   0        0        0      207 2024-05-17 06:27:09.000000 glabpkg-4.0.0/src/glabpkg/data/resource/src/{{ base.pkgname }}/info.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.108491 glabpkg-4.0.0/src/glabpkg/data/resource/test/
+-rw-rw-rw-   0        0        0      191 2024-05-17 06:30:12.000000 glabpkg-4.0.0/src/glabpkg/data/resource/test/test_packaging.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.113498 glabpkg-4.0.0/src/glabpkg/pkg/
+-rw-rw-rw-   0        0        0        0 2021-06-25 14:18:59.000000 glabpkg-4.0.0/src/glabpkg/pkg/__init__.py
+-rw-rw-rw-   0        0        0     1828 2024-01-03 18:35:00.000000 glabpkg-4.0.0/src/glabpkg/pkg/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.040040 glabpkg-4.0.0/src/glabpkg/pkg/resource/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.113498 glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.118556 glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/badges/
+-rw-rw-rw-   0        0        0     1094 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg
+-rw-rw-rw-   0        0        0     1090 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg
+-rw-rw-rw-   0        0        0      172 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/badges/listing.rst
+-rw-rw-rw-   0        0        0      184 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/installation.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.120583 glabpkg-4.0.0/src/glabpkg/pkg_dev/
+-rw-rw-rw-   0        0        0        0 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-01-03 18:35:00.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.120583 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/
+-rw-rw-rw-   0        0        0     1665 2024-03-14 15:29:53.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      444 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.133195 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/
+-rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.135936 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/badges/
+-rw-rw-rw-   0        0        0     1002 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg
+-rw-rw-rw-   0        0        0      110 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.137030 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/biblio/
+-rw-rw-rw-   0        0        0      513 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst
+-rw-rw-rw-   0        0        0       34 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/contributing.rst
+-rw-rw-rw-   0        0        0       29 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/history.rst
+-rw-rw-rw-   0        0        0      634 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/index.rst
+-rw-rw-rw-   0        0        0      209 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/installation.rst
+-rw-rw-rw-   0        0        0      133 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/management.rst
+-rw-rw-rw-   0        0        0      557 2024-01-03 18:35:00.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/readme.rst
+-rw-rw-rw-   0        0        0       21 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/usage.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.138921 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/user/
+-rw-rw-rw-   0        0        0       86 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/user/index.rst
+-rw-rw-rw-   0        0        0       66 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/user/overview.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.140604 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/example/
+-rw-rw-rw-   0        0        0      254 2022-12-04 11:33:38.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/example/readme.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.141165 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/test/
+-rw-rw-rw-   0        0        0      148 2024-05-17 06:30:12.000000 glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/test/test_packaging.py.tpl
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.141165 glabpkg-4.0.0/src/glabpkg/report/
+-rw-rw-rw-   0        0        0        0 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/__init__.py
+-rw-rw-rw-   0        0        0     1559 2024-01-03 18:35:00.000000 glabpkg-4.0.0/src/glabpkg/report/option.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.145632 glabpkg-4.0.0/src/glabpkg/report/resource/
+-rw-rw-rw-   0        0        0      949 2023-03-09 14:37:10.000000 glabpkg-4.0.0/src/glabpkg/report/resource/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      923 2022-03-28 12:29:45.000000 glabpkg-4.0.0/src/glabpkg/report/resource/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.151791 glabpkg-4.0.0/src/glabpkg/report/resource/report/
+-rw-rw-rw-   0        0        0       51 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/report/authors.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.151791 glabpkg-4.0.0/src/glabpkg/report/resource/report/badges/
+-rw-rw-rw-   0        0        0     1001 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/report/badges/badge_doc.svg
+-rw-rw-rw-   0        0        0      109 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/report/badges/listing.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.151791 glabpkg-4.0.0/src/glabpkg/report/resource/report/biblio/
+-rw-rw-rw-   0        0        0      513 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/report/biblio/biblio.rst
+-rw-rw-rw-   0        0        0      130 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/report/conf.py.tpl
+-rw-rw-rw-   0        0        0      376 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/report/index.rst
+-rw-rw-rw-   0        0        0       89 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/report/introduction.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.151791 glabpkg-4.0.0/src/glabpkg/report/resource/script/
+-rw-rw-rw-   0        0        0       56 2021-07-06 09:29:24.000000 glabpkg-4.0.0/src/glabpkg/report/resource/script/readme.rst
+-rw-rw-rw-   0        0        0      367 2024-05-17 07:04:56.000000 glabpkg-4.0.0/src/glabpkg/version.py
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.160912 glabpkg-4.0.0/src/glabpkg.egg-info/
+-rw-rw-rw-   0        0        0     3293 2024-05-17 07:05:44.000000 glabpkg-4.0.0/src/glabpkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3069 2024-05-17 07:05:45.000000 glabpkg-4.0.0/src/glabpkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 07:05:44.000000 glabpkg-4.0.0/src/glabpkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      250 2024-05-17 07:05:44.000000 glabpkg-4.0.0/src/glabpkg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2024-05-17 07:05:44.000000 glabpkg-4.0.0/src/glabpkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-17 07:05:44.000000 glabpkg-4.0.0/src/glabpkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 07:05:45.158884 glabpkg-4.0.0/test/
+-rw-rw-rw-   0        0        0      983 2024-05-17 07:04:14.000000 glabpkg-4.0.0/test/conftest.py
+-rw-rw-rw-   0        0        0      114 2024-05-17 07:04:14.000000 glabpkg-4.0.0/test/test_packaging.py
```

### Comparing `glabpkg-3.1.0/CONTRIBUTING.rst` & `glabpkg-4.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/LICENSE` & `glabpkg-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/PKG-INFO` & `glabpkg-4.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: glabpkg
-Version: 3.1.0
+Version: 4.0.0
 Summary: template for python packages hosted on gitlab
 Author-email: revesansparole <revesansparole@gmail.com>
 Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>, jchopard <jerome.chopard@itk.fr>
 License: cc_by_nc
 Project-URL: repository, https://gitlab.com/revesansparole/glabpkg
-Project-URL: pip, https://pypi.org/project/glabpkg/3.1.0/
+Project-URL: pip, https://pypi.org/project/glabpkg/4.0.0/
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
-    :target: https://pypi.org/project/glabpkg/3.1.0/
+    :target: https://pypi.org/project/glabpkg/4.0.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-3.1.0/README.rst` & `glabpkg-4.0.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 glabpkg
 ========================
 
 .. {# pkglts, doc
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/3.1.0/
+    :target: https://pypi.org/project/glabpkg/4.0.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-3.1.0/doc/Makefile` & `glabpkg-4.0.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/doc/biblio/biblio.rst` & `glabpkg-4.0.0/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/doc/conf.py` & `glabpkg-4.0.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 
 # The short X.Y version.
-version = "3.1.0"
+version = "4.0.0"
 # The full version, including alpha/beta/rc tags.
-release = "3.1.0"
+release = "4.0.0"
 
 
 exclude_patterns = ['build', 'dist']
 
 pygments_style = 'sphinx'
 
 # -- Options for HTML output -------------------------------------------
```

### Comparing `glabpkg-3.1.0/doc/index.rst` & `glabpkg-4.0.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/doc/make.bat` & `glabpkg-4.0.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/doc/readme.rst` & `glabpkg-4.0.0/doc/readme.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Overview
 ========
 
 .. {# pkglts, glabpkg_dev
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_pip.svg
     :alt: PyPI version
-    :target: https://pypi.org/project/glabpkg/3.1.0/
+    :target: https://pypi.org/project/glabpkg/4.0.0/
 
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
```

### Comparing `glabpkg-3.1.0/pyproject.toml` & `glabpkg-4.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 requires = ["setuptools", "wheel"]  # , "setuptools-scm"]  # PEP 508 specifications.
 build-backend = "setuptools.build_meta"  # we don't know if we need it
 # #}
 
 # {# pkglts, pyproject.project
 [project]  # https://packaging.python.org/en/latest/specifications/pyproject-toml/
 name = "glabpkg"
-version = "3.1.0"
+version = "4.0.0"
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
-pip = "https://pypi.org/project/glabpkg/3.1.0/"
+pip = "https://pypi.org/project/glabpkg/4.0.0/"
 conda = "https://anaconda.org/revesansparole/glabpkg"
 doc = "https://revesansparole.gitlab.io/glabpkg/"
 pypi = "https://badge.fury.io/py/glabpkg"
 
 
 [tool.setuptools]
 include-package-data = true
@@ -89,9 +89,8 @@
 # #}
 
 [project.entry-points."pkglts"]
 glabbase = "glabpkg.base.option:OptionGlabBase"
 glabpkg_dev = "glabpkg.pkg_dev.option:OptionGlabPkgDev"
 glabpkg = "glabpkg.pkg.option:OptionGlabPkg"
 glabdata = "glabpkg.data.option:OptionGlabData"
-glabdata_alt = "glabpkg.data_alt.option:OptionGlabDataAlt"
 glabreport = "glabpkg.report.option:OptionGlabReport"
```

### Comparing `glabpkg-3.1.0/src/glabpkg/base/option.py` & `glabpkg-4.0.0/src/glabpkg/base/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg/option.py` & `glabpkg-4.0.0/src/glabpkg/pkg/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg` & `glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg` & `glabpkg-4.0.0/src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg_dev/option.py` & `glabpkg-4.0.0/src/glabpkg/pkg_dev/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml` & `glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg` & `glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/badges/badge_doc.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst` & `glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/index.rst` & `glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/index.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/pkg_dev/resource/doc/readme.rst` & `glabpkg-4.0.0/src/glabpkg/pkg_dev/resource/doc/readme.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/report/option.py` & `glabpkg-4.0.0/src/glabpkg/report/option.py`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/report/resource/.gitlab-ci.yml` & `glabpkg-4.0.0/src/glabpkg/report/resource/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/report/resource/README.rst` & `glabpkg-4.0.0/src/glabpkg/report/resource/README.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/report/resource/report/badges/badge_doc.svg` & `glabpkg-4.0.0/src/glabpkg/report/resource/report/badges/badge_doc.svg`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg/report/resource/report/biblio/biblio.rst` & `glabpkg-4.0.0/src/glabpkg/report/resource/report/biblio/biblio.rst`

 * *Files identical despite different names*

### Comparing `glabpkg-3.1.0/src/glabpkg.egg-info/PKG-INFO` & `glabpkg-4.0.0/src/glabpkg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: glabpkg
-Version: 3.1.0
+Version: 4.0.0
 Summary: template for python packages hosted on gitlab
 Author-email: revesansparole <revesansparole@gmail.com>
 Maintainer-email: revesansparole <revesansparole@gmail.com>, Jerome Chopard <revesansparole@gmail.com>, jchopard <jerome.chopard@itk.fr>
 License: cc_by_nc
 Project-URL: repository, https://gitlab.com/revesansparole/glabpkg
-Project-URL: pip, https://pypi.org/project/glabpkg/3.1.0/
+Project-URL: pip, https://pypi.org/project/glabpkg/4.0.0/
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
-    :target: https://pypi.org/project/glabpkg/3.1.0/
+    :target: https://pypi.org/project/glabpkg/4.0.0/
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_pkging_conda.svg
     :alt: Conda version
     :target: https://anaconda.org/revesansparole/glabpkg
 
 .. image:: https://revesansparole.gitlab.io/glabpkg/_images/badge_doc.svg
     :alt: Documentation status
```

### Comparing `glabpkg-3.1.0/src/glabpkg.egg-info/SOURCES.txt` & `glabpkg-4.0.0/src/glabpkg.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -34,26 +34,20 @@
 src/glabpkg/base/resource/.gitattributes.tpl
 src/glabpkg/base/resource/.gitlab-ci.yml
 src/glabpkg/base/resource/.gitlab/issue_templates/bug.md
 src/glabpkg/base/resource/.gitlab/issue_templates/feature.md
 src/glabpkg/base/resource/.gitlab/issue_templates/technical_task.md
 src/glabpkg/data/__init__.py
 src/glabpkg/data/option.py
+src/glabpkg/data/resource/raw/readme.rst
 src/glabpkg/data/resource/script/readme.rst
 src/glabpkg/data/resource/src/{{ base.pkgname }}/__init__.py.tpl
 src/glabpkg/data/resource/src/{{ base.pkgname }}/info.py.tpl
 src/glabpkg/data/resource/src/{{ base.pkgname }}/clean/readme.rst
-src/glabpkg/data/resource/src/{{ base.pkgname }}/raw/readme.rst
-src/glabpkg/data_alt/__init__.py
-src/glabpkg/data_alt/option.py
-src/glabpkg/data_alt/resource/script/readme.rst
-src/glabpkg/data_alt/resource/script/raw/readme.rst
-src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/__init__.py.tpl
-src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/info.py.tpl
-src/glabpkg/data_alt/resource/src/{{ base.pkgname }}/clean/readme.rst
+src/glabpkg/data/resource/test/test_packaging.py.tpl
 src/glabpkg/pkg/__init__.py
 src/glabpkg/pkg/option.py
 src/glabpkg/pkg/resource/doc/installation.rst
 src/glabpkg/pkg/resource/doc/badges/badge_pkging_conda.svg
 src/glabpkg/pkg/resource/doc/badges/badge_pkging_pip.svg
 src/glabpkg/pkg/resource/doc/badges/listing.rst
 src/glabpkg/pkg_dev/__init__.py
```

### Comparing `glabpkg-3.1.0/test/conftest.py` & `glabpkg-4.0.0/test/conftest.py`

 * *Files identical despite different names*
