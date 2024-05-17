# Comparing `tmp/datalad_next-1.3.0.tar.gz` & `tmp/datalad_next-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_next-1.3.0.tar", last modified: Tue Mar 19 12:43:03 2024, max compression
+gzip compressed data, was "datalad_next-1.4.0.tar", last modified: Fri May 17 19:27:07 2024, max compression
```

## Comparing `datalad_next-1.3.0.tar` & `datalad_next-1.4.0.tar`

### file list

```diff
@@ -1,326 +1,354 @@
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.911132 datalad_next-1.3.0/
--rw-rw-r--   0 mih       (1000) mih       (1000)     4809 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.all-contributorsrc
--rw-rw-r--   0 mih       (1000) mih       (1000)    16333 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.appveyor.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      265 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.codeclimate.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)       79 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.codespellrc
--rw-rw-r--   0 mih       (1000) mih       (1000)      241 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.coveragerc
--rw-rw-r--   0 mih       (1000) mih       (1000)       38 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.gitattributes
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.891130 datalad_next-1.3.0/.github/
--rw-rw-r--   0 mih       (1000) mih       (1000)      657 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.github/PULL_REQUEST_TEMPLATE.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/.github/workflows/
--rw-rw-r--   0 mih       (1000) mih       (1000)      320 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.github/workflows/codespell.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      613 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.github/workflows/docbuild.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.github/workflows/mypy.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     2830 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.github/workflows/update-contributors.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      123 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.gitignore
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.noannex
--rw-rw-r--   0 mih       (1000) mih       (1000)     2394 2024-03-19 12:42:43.000000 datalad_next-1.3.0/.zenodo.json
--rw-rw-r--   0 mih       (1000) mih       (1000)    53198 2024-03-19 12:42:43.000000 datalad_next-1.3.0/CHANGELOG.md
--rw-rw-r--   0 mih       (1000) mih       (1000)     2451 2024-03-19 12:42:43.000000 datalad_next-1.3.0/CITATION.cff
--rw-rw-r--   0 mih       (1000) mih       (1000)     7954 2024-03-19 12:42:43.000000 datalad_next-1.3.0/CONTRIBUTING.md
--rw-rw-r--   0 mih       (1000) mih       (1000)       55 2024-03-19 12:42:43.000000 datalad_next-1.3.0/CONTRIBUTORS
--rw-rw-r--   0 mih       (1000) mih       (1000)     1609 2024-03-19 12:42:43.000000 datalad_next-1.3.0/LICENSE
--rw-rw-r--   0 mih       (1000) mih       (1000)      124 2024-03-19 12:42:43.000000 datalad_next-1.3.0/MANIFEST.in
--rw-rw-r--   0 mih       (1000) mih       (1000)      506 2024-03-19 12:42:43.000000 datalad_next-1.3.0/Makefile
--rw-r--r--   0 mih       (1000) mih       (1000)    20140 2024-03-19 12:43:03.911132 datalad_next-1.3.0/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)    19109 2024-03-19 12:42:43.000000 datalad_next-1.3.0/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/_datalad_buildsupport/
--rw-rw-r--   0 mih       (1000) mih       (1000)      529 2024-03-19 12:42:43.000000 datalad_next-1.3.0/_datalad_buildsupport/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10699 2024-03-19 12:42:43.000000 datalad_next-1.3.0/_datalad_buildsupport/formatters.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8520 2024-03-19 12:42:43.000000 datalad_next-1.3.0/_datalad_buildsupport/setup.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/changelog.d/
--rw-rw-r--   0 mih       (1000) mih       (1000)      234 2024-03-19 12:42:43.000000 datalad_next-1.3.0/changelog.d/README
--rw-rw-r--   0 mih       (1000) mih       (1000)      312 2024-03-19 12:42:43.000000 datalad_next-1.3.0/changelog.d/scriv.ini
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/changelog.d/templates/
--rw-rw-r--   0 mih       (1000) mih       (1000)       74 2024-03-19 12:42:43.000000 datalad_next-1.3.0/changelog.d/templates/entry_title.md.j2
--rw-rw-r--   0 mih       (1000) mih       (1000)      349 2024-03-19 12:42:43.000000 datalad_next-1.3.0/changelog.d/templates/new_fragment.md.j2
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/
--rw-rw-r--   0 mih       (1000) mih       (1000)     4028 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-03-19 12:43:03.911132 datalad_next-1.3.0/datalad_next/_version.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/annexbackends/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexbackends/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10375 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexbackends/base.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/annexbackends/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexbackends/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1978 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexbackends/tests/test_base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2429 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexbackends/xdlra.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/annexremotes/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3639 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexremotes/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    23285 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexremotes/archivist.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/annexremotes/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexremotes/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9576 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexremotes/tests/test_archivist.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16906 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexremotes/tests/test_uncurl.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    22959 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/annexremotes/uncurl.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/archive_operations/
--rw-rw-r--   0 mih       (1000) mih       (1000)      870 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/archive_operations/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3181 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/archive_operations/base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3828 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/archive_operations/tarfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/archive_operations/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/archive_operations/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2670 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/archive_operations/tests/test_tarfile.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3111 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/archive_operations/tests/test_zipfile.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4315 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/archive_operations/zipfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/commands/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3702 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    26365 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/create_sibling_webdav.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    19186 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/credentials.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14081 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/download.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16851 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/ls_file_collection.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4426 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/results.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14518 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/status.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/commands/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    15000 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/test_create_sibling_webdav.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6160 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/test_credentials.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9133 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/test_download.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8333 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/test_ls_file_collection.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1766 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/test_results.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1819 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/test_status.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    31754 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tests/test_tree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    46335 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/commands/tree.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/config/
--rw-rw-r--   0 mih       (1000) mih       (1000)      244 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/config/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next/config/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/config/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      325 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/config/tests/test_core.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5747 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/config/tests/test_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3355 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/config/utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2197 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/conftest.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/constraints/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3490 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8724 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16694 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/basic.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18795 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/compound.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4774 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    12974 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3881 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/formats.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5669 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/git.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    18669 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/parameter.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     7361 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/parameter_legacy.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/constraints/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4416 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/test_base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9875 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/test_basic.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11946 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/test_cmdarg_validation.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9523 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/test_compound.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1807 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/test_exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14738 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/test_special_purpose.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2072 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/tests/test_tutorial.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1047 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/constraints/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/consts/
--rw-rw-r--   0 mih       (1000) mih       (1000)      775 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/consts/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/credman/
--rw-rw-r--   0 mih       (1000) mih       (1000)      232 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/credman/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    43876 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/credman/manager.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/credman/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/credman/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    15102 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/credman/tests/test_credman.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/datasets/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1788 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/datasets/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1805 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/datasets/annexrepo.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/exceptions/
--rw-rw-r--   0 mih       (1000) mih       (1000)      779 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/exceptions/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/gitremotes/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/gitremotes/__init__.py
--rwxrwxr-x   0 mih       (1000) mih       (1000)    52669 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/gitremotes/datalad_annex.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/gitremotes/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/gitremotes/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14941 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/gitremotes/tests/test_datalad_annex.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/iter_collections/
--rw-rw-r--   0 mih       (1000) mih       (1000)     2182 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14174 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/annexworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2183 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/directory.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    17804 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/gitdiff.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    19402 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/gitstatus.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4529 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/gittree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    13158 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/gitworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3475 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tarfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/iter_collections/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4461 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_iterannexworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2844 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_iterdir.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    12436 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergitdiff.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10107 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergitstatus.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3353 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergittree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8321 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergitworktree.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3357 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itertar.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2454 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_iterzip.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      994 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/tests/test_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3663 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2812 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iter_collections/zipfile.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/iterable_subprocess/
--rw-rw-r--   0 mih       (1000) mih       (1000)       20 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/.coveragerc
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.891130 datalad_next-1.3.0/datalad_next/iterable_subprocess/.github/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.899131 datalad_next-1.3.0/datalad_next/iterable_subprocess/.github/workflows/
--rw-rw-r--   0 mih       (1000) mih       (1000)      993 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      819 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/.github/workflows/test.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     1799 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/.gitignore
--rw-rw-r--   0 mih       (1000) mih       (1000)     1091 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/LICENSE
--rw-rw-r--   0 mih       (1000) mih       (1000)     3710 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/README.md
--rw-rw-r--   0 mih       (1000) mih       (1000)      859 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)       15 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/codecov.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)     6803 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/iterable_subprocess.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      736 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/pyproject.toml
--rw-rw-r--   0 mih       (1000) mih       (1000)    11706 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/iterable_subprocess/test_iterable_subprocess.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/itertools/
--rw-rw-r--   0 mih       (1000) mih       (1000)      523 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4265 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/align_pattern.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5286 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/decode_bytes.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5703 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/itemize.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4065 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/load_json.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8378 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/reroute.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/itertools/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1141 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/tests/test_align_pattern.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1078 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/tests/test_decode_bytes.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1225 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/tests/test_itemize.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1381 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/tests/test_load_json.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1588 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/itertools/tests/test_reroute.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/patches/
--rw-rw-r--   0 mih       (1000) mih       (1000)     2009 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4173 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/annexrepo.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2075 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/cli_configoverrides.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1326 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/commanderror.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      491 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/common_cfg.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6849 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/configuration.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5443 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/create_sibling_ghlike.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    16127 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/create_sibling_gitlab.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5037 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/customremotes_main.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1173 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/distribution_dataset.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      309 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/enabled.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11068 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/interface_utils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    17041 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/push_optimize.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    10128 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/push_to_export_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3067 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/run.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2424 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/siblings.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      827 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/test_keyring.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/patches/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2347 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_annex_progress_logging.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      615 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_cli_configoverrides.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      721 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_commanderror.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1798 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_configuration.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1465 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_create_sibling_ghlike.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    17167 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_create_sibling_gitlab.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1421 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_push.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     7798 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_push_to_export_remote.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      839 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/tests/test_run.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2129 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/patches/update.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/repo_utils/
--rw-rw-r--   0 mih       (1000) mih       (1000)      192 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/repo_utils/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/repo_utils/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/repo_utils/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1098 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/repo_utils/tests/test_head.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1555 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/repo_utils/worktree.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/runners/
--rw-rw-r--   0 mih       (1000) mih       (1000)     2234 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/runners/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     6366 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/runners/git.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3918 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/runners/iter_subproc.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      887 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/runners/protocols.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/runners/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/runners/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1190 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/runners/tests/test_git.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      946 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/runners/tests/test_iter_subproc.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1081 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    24303 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/tests/fixtures.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      156 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/tests/marker.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/tests/test_common_cfg.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      120 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/tests/test_register.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      486 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/tests/test_testutils.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9315 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/tests/utils.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/types/
--rw-rw-r--   0 mih       (1000) mih       (1000)      267 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/types/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/types/annexkey.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5417 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/types/archivist.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      266 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/types/enums.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/types/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/types/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      905 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/types/tests/test_annexkey.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2020 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/types/tests/test_archivist.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.903131 datalad_next-1.3.0/datalad_next/uis/
--rw-rw-r--   0 mih       (1000) mih       (1000)      337 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/uis/__init__.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/datalad_next/url_operations/
--rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     8076 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/any.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14899 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/base.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2091 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/exceptions.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     9046 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/file.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    11849 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/http.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    14741 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/ssh.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/datalad_next/url_operations/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2041 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/tests/test_any.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3443 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/tests/test_file.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5066 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/tests/test_http.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     4598 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/url_operations/tests/test_ssh.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/datalad_next/utils/
--rw-rw-r--   0 mih       (1000) mih       (1000)     2778 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      134 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/consts.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      326 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/credman.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     3927 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/deprecate.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     2667 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/http_helpers.py
--rw-rw-r--   0 mih       (1000) mih       (1000)       37 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/log.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1737 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/multihash.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      857 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/patch.py
--rw-rw-r--   0 mih       (1000) mih       (1000)    15257 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/requests_auth.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5859 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/specialremote.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/datalad_next/utils/tests/
--rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/tests/__init__.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     5673 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/tests/test_deprecated.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      543 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/tests/test_multihash.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      240 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/tests/test_paramdictator.py
--rw-rw-r--   0 mih       (1000) mih       (1000)     1486 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/tests/test_parse_www_authenticate.py
--rw-rw-r--   0 mih       (1000) mih       (1000)      483 2024-03-19 12:42:43.000000 datalad_next-1.3.0/datalad_next/utils/tests/test_patch.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.895130 datalad_next-1.3.0/datalad_next.egg-info/
--rw-r--r--   0 mih       (1000) mih       (1000)    20140 2024-03-19 12:43:03.000000 datalad_next-1.3.0/datalad_next.egg-info/PKG-INFO
--rw-rw-r--   0 mih       (1000) mih       (1000)     9946 2024-03-19 12:43:03.000000 datalad_next-1.3.0/datalad_next.egg-info/SOURCES.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)        1 2024-03-19 12:43:03.000000 datalad_next-1.3.0/datalad_next.egg-info/dependency_links.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      342 2024-03-19 12:43:03.000000 datalad_next-1.3.0/datalad_next.egg-info/entry_points.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)      167 2024-03-19 12:43:03.000000 datalad_next-1.3.0/datalad_next.egg-info/requires.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)       13 2024-03-19 12:43:03.000000 datalad_next-1.3.0/datalad_next.egg-info/top_level.txt
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/docs/
--rw-rw-r--   0 mih       (1000) mih       (1000)      546 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/CODEOWNERS
--rw-rw-r--   0 mih       (1000) mih       (1000)     7496 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/Makefile
--rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/README.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/docs/policy/
--rw-rw-r--   0 mih       (1000) mih       (1000)      826 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/policy/release-management.md
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/docs/source/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/docs/source/_static/
--rw-rw-r--   0 mih       (1000) mih       (1000)      958 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/_static/datalad_logo.png
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.891130 datalad_next-1.3.0/docs/source/_templates/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/docs/source/_templates/autosummary/
--rw-rw-r--   0 mih       (1000) mih       (1000)      116 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/_templates/autosummary/class.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      436 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/_templates/autosummary/module.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/annex-backends.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      179 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/annex-specialremotes.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      218 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/api.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      306 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/cmd.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     4698 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/conf.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/docs/source/developer_guide/
--rw-rw-r--   0 mih       (1000) mih       (1000)     3431 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/developer_guide/constraints.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/developer_guide/contributing.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      314 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/developer_guide/index.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      140 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/git-remote-helpers.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)     3476 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/index.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      503 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/patches.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)      735 2024-03-19 12:42:43.000000 datalad_next-1.3.0/docs/source/pyutils.rst
--rw-rw-r--   0 mih       (1000) mih       (1000)       60 2024-03-19 12:42:43.000000 datalad_next-1.3.0/pyproject.toml
--rw-rw-r--   0 mih       (1000) mih       (1000)      554 2024-03-19 12:42:43.000000 datalad_next-1.3.0/readthedocs.yml
--rw-rw-r--   0 mih       (1000) mih       (1000)      128 2024-03-19 12:42:43.000000 datalad_next-1.3.0/requirements-devel.txt
--rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-03-19 12:43:03.911132 datalad_next-1.3.0/setup.cfg
--rwxrwxr-x   0 mih       (1000) mih       (1000)      364 2024-03-19 12:42:43.000000 datalad_next-1.3.0/setup.py
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.891130 datalad_next-1.3.0/tools/
-drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-03-19 12:43:03.907132 datalad_next-1.3.0/tools/appveyor/
--rw-rw-r--   0 mih       (1000) mih       (1000)      291 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/chmod600.bat
--rwxrwxr-x   0 mih       (1000) mih       (1000)      311 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/docker-load-httpbin
--rwxrwxr-x   0 mih       (1000) mih       (1000)      124 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/enable-ssh-login
--rw-rw-r--   0 mih       (1000) mih       (1000)      101 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/env_setup.bat
--rwxrwxr-x   0 mih       (1000) mih       (1000)      399 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/install-git-annex
--rwxrwxr-x   0 mih       (1000) mih       (1000)      331 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/install-syspkgs
--rwxrwxr-x   0 mih       (1000) mih       (1000)     1464 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/setup-sshd
--rw-rw-r--   0 mih       (1000) mih       (1000)     1054 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/setup-sshd.bat
--rwxrwxr-x   0 mih       (1000) mih       (1000)      330 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/verify-ssh-access
--rw-rw-r--   0 mih       (1000) mih       (1000)      343 2024-03-19 12:42:43.000000 datalad_next-1.3.0/tools/appveyor/verify-ssh-access.bat
--rw-rw-r--   0 mih       (1000) mih       (1000)    86677 2024-03-19 12:42:43.000000 datalad_next-1.3.0/versioneer.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4809 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.all-contributorsrc
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16333 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.appveyor.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      265 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.codeclimate.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)       46 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.codespell-exclude
+-rw-rw-r--   0 mih       (1000) mih       (1000)       79 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.codespellrc
+-rw-rw-r--   0 mih       (1000) mih       (1000)      286 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.coveragerc
+-rw-rw-r--   0 mih       (1000) mih       (1000)       38 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.gitattributes
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/.github/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      657 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/.github/workflows/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      377 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/codespell.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      613 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/docbuild.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/mypy.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2830 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.github/workflows/update-contributors.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      123 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.gitignore
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.noannex
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2394 2024-05-17 19:26:55.000000 datalad_next-1.4.0/.zenodo.json
+-rw-rw-r--   0 mih       (1000) mih       (1000)    58894 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CHANGELOG.md
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2451 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CITATION.cff
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8180 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CONTRIBUTING.md
+-rw-rw-r--   0 mih       (1000) mih       (1000)       55 2024-05-17 19:26:55.000000 datalad_next-1.4.0/CONTRIBUTORS
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1609 2024-05-17 19:26:55.000000 datalad_next-1.4.0/LICENSE
+-rw-rw-r--   0 mih       (1000) mih       (1000)      124 2024-05-17 19:26:55.000000 datalad_next-1.4.0/MANIFEST.in
+-rw-rw-r--   0 mih       (1000) mih       (1000)      506 2024-05-17 19:26:55.000000 datalad_next-1.4.0/Makefile
+-rw-r--r--   0 mih       (1000) mih       (1000)    19945 2024-05-17 19:27:07.642464 datalad_next-1.4.0/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18914 2024-05-17 19:26:55.000000 datalad_next-1.4.0/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/_datalad_buildsupport/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      529 2024-05-17 19:26:55.000000 datalad_next-1.4.0/_datalad_buildsupport/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10699 2024-05-17 19:26:55.000000 datalad_next-1.4.0/_datalad_buildsupport/formatters.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8520 2024-05-17 19:26:55.000000 datalad_next-1.4.0/_datalad_buildsupport/setup.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/changelog.d/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      234 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/README
+-rw-rw-r--   0 mih       (1000) mih       (1000)      312 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/scriv.ini
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/changelog.d/templates/
+-rw-rw-r--   0 mih       (1000) mih       (1000)       74 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/templates/entry_title.md.j2
+-rw-rw-r--   0 mih       (1000) mih       (1000)      349 2024-05-17 19:26:55.000000 datalad_next-1.4.0/changelog.d/templates/new_fragment.md.j2
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4028 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-05-17 19:27:07.642464 datalad_next-1.4.0/datalad_next/_version.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexbackends/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10375 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/base.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexbackends/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1978 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/tests/test_base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2429 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexbackends/xdlra.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexremotes/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3639 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    23285 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/archivist.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/annexremotes/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9576 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/tests/test_archivist.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16906 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/tests/test_uncurl.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    22959 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/annexremotes/uncurl.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/archive_operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      870 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3181 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3828 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tarfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/archive_operations/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2670 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tests/test_tarfile.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3111 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/tests/test_zipfile.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4315 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/archive_operations/zipfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/commands/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3702 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    26365 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/create_sibling_webdav.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    19186 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/credentials.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14081 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/download.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    17496 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/ls_file_collection.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4426 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/results.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14601 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/status.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/commands/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    15000 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_create_sibling_webdav.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6160 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_credentials.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9133 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_download.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8333 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_ls_file_collection.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1766 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_results.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1819 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_status.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    31754 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tests/test_tree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    46335 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/commands/tree.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next/config/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      244 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/config/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      325 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/tests/test_core.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5747 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/tests/test_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3904 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/config/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2197 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/conftest.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/constraints/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3490 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8724 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16694 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/basic.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18795 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/compound.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4774 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12974 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3881 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/formats.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5669 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/git.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18669 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/parameter.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7361 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/parameter_legacy.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/constraints/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4416 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9875 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_basic.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11946 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_cmdarg_validation.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_compound.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1807 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14738 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_special_purpose.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2072 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/tests/test_tutorial.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1047 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/constraints/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/consts/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      775 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/consts/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/credman/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      232 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    43876 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/manager.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/credman/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    15102 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/credman/tests/test_credman.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/datasets/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1788 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/datasets/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1805 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/datasets/annexrepo.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/exceptions/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      779 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/exceptions/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/gitremotes/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/__init__.py
+-rwxrwxr-x   0 mih       (1000) mih       (1000)    52669 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/datalad_annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/gitremotes/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14941 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/gitremotes/tests/test_datalad_annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iter_collections/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2182 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14857 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/annexworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2183 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/directory.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18526 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gitdiff.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    20038 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gitstatus.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4529 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gittree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13158 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/gitworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3475 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tarfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iter_collections/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4939 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterannexworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2844 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterdir.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    12436 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitdiff.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10920 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitstatus.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3353 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergittree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8321 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitworktree.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3357 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itertar.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2454 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterzip.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      994 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/tests/test_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3663 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2812 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iter_collections/zipfile.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iterable_subprocess/
+-rw-rw-r--   0 mih       (1000) mih       (1000)       20 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.coveragerc
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.622464 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.630464 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      993 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      819 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/test.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1799 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/.gitignore
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1091 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/LICENSE
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3710 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/README.md
+-rw-rw-r--   0 mih       (1000) mih       (1000)      859 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)       15 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/codecov.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7086 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/iterable_subprocess.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      736 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/pyproject.toml
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11706 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/iterable_subprocess/test_iterable_subprocess.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/itertools/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4520 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/align_pattern.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5286 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/decode_bytes.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5703 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/itemize.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4065 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/load_json.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8378 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/reroute.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/itertools/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2048 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_align_pattern.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1078 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_decode_bytes.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1225 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_itemize.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1381 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_load_json.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1588 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/itertools/tests/test_reroute.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/patches/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2009 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2252 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/add_method_url2transport_path.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4173 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/annexrepo.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2075 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/cli_configoverrides.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1326 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/commanderror.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      491 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/common_cfg.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6849 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/configuration.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5443 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/create_sibling_ghlike.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    16127 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/create_sibling_gitlab.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6224 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/customremotes_main.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1173 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/distribution_dataset.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      434 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/enabled.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    37392 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/fix_ria_ora_tests.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11068 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/interface_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      646 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/patch_ria_ora.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    17041 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/push_optimize.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10128 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/push_to_export_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    35692 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/replace_create_sibling_ria.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    41308 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/replace_ora_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    13580 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/replace_sshremoteio.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8093 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/ria_utils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3067 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/run.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2424 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/siblings.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2525 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/ssh_exec.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4330 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/sshconnector.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      827 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/test_keyring.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/patches/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1607 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_add_method_url2transport_path.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2347 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_annex_progress_logging.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      615 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_cli_configoverrides.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      721 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_commanderror.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1798 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_configuration.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1465 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_ghlike.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    17167 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_gitlab.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1421 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_push.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7798 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_push_to_export_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1436 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_replace_ora_remote.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      977 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_ria.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      839 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_run.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3393 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/tests/test_sshremoteio.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2129 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/patches/update.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/repo_utils/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      267 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1240 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/annex.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/repo_utils/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      610 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/tests/test_annex.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1098 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/tests/test_head.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1909 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/repo_utils/worktree.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.634464 datalad_next-1.4.0/datalad_next/runners/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3001 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     6380 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/git.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4167 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/iter_subproc.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      887 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/protocols.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/runners/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1190 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/tests/test_git.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      946 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/runners/tests/test_iter_subproc.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/shell/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7843 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/shell/operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3070 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/operations/common.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11452 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/operations/posix.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10989 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/response_generators.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    27832 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/shell.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/shell/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3835 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/tests/test_response_generators.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    18189 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/shell/tests/test_shell.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1081 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    24864 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/fixtures.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      156 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/marker.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/test_common_cfg.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      120 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/test_register.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      486 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/test_testutils.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9422 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/tests/utils.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/types/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      267 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1523 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/annexkey.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5417 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/archivist.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      266 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/enums.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/types/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      905 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/tests/test_annexkey.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2020 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/types/tests/test_archivist.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/uis/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      337 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/uis/__init__.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/url_operations/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     8076 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/any.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14899 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/base.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2091 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/exceptions.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     9046 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/file.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    11849 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/http.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    14741 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/ssh.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/url_operations/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2041 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_any.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3443 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_file.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5066 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_http.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4598 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/url_operations/tests/test_ssh.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/utils/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2778 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      134 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/consts.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      326 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/credman.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3927 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/deprecate.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     2667 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/http_helpers.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)       37 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/log.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1737 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/multihash.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      857 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/patch.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)    15257 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/requests_auth.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5859 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/specialremote.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/datalad_next/utils/tests/
+-rw-rw-r--   0 mih       (1000) mih       (1000)        0 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/__init__.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     5673 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_deprecated.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      543 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_multihash.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      240 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_paramdictator.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1486 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_parse_www_authenticate.py
+-rw-rw-r--   0 mih       (1000) mih       (1000)      483 2024-05-17 19:26:55.000000 datalad_next-1.4.0/datalad_next/utils/tests/test_patch.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.626464 datalad_next-1.4.0/datalad_next.egg-info/
+-rw-r--r--   0 mih       (1000) mih       (1000)    19945 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/PKG-INFO
+-rw-rw-r--   0 mih       (1000) mih       (1000)    10974 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/SOURCES.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)        1 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/dependency_links.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      342 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/entry_points.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)      167 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/requires.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)       13 2024-05-17 19:27:07.000000 datalad_next-1.4.0/datalad_next.egg-info/top_level.txt
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/docs/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      658 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/CODEOWNERS
+-rw-rw-r--   0 mih       (1000) mih       (1000)     7496 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/Makefile
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1755 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/README.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.638464 datalad_next-1.4.0/docs/policy/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      826 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/policy/release-management.md
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/_static/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      958 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/_static/datalad_logo.png
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.622464 datalad_next-1.4.0/docs/source/_templates/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/_templates/autosummary/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      116 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/_templates/autosummary/class.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      436 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      142 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/annex-backends.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      179 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/annex-specialremotes.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      218 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/api.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      306 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/cmd.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     4843 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/conf.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/docs/source/developer_guide/
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3431 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/developer_guide/constraints.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      497 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/developer_guide/contributing.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      314 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/developer_guide/index.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      140 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/git-remote-helpers.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)     3476 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/index.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      690 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/patches.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)      744 2024-05-17 19:26:55.000000 datalad_next-1.4.0/docs/source/pyutils.rst
+-rw-rw-r--   0 mih       (1000) mih       (1000)       60 2024-05-17 19:26:55.000000 datalad_next-1.4.0/pyproject.toml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      554 2024-05-17 19:26:55.000000 datalad_next-1.4.0/readthedocs.yml
+-rw-rw-r--   0 mih       (1000) mih       (1000)      128 2024-05-17 19:26:55.000000 datalad_next-1.4.0/requirements-devel.txt
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1419 2024-05-17 19:27:07.642464 datalad_next-1.4.0/setup.cfg
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      364 2024-05-17 19:26:55.000000 datalad_next-1.4.0/setup.py
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.622464 datalad_next-1.4.0/tools/
+drwxrwxr-x   0 mih       (1000) mih       (1000)        0 2024-05-17 19:27:07.642464 datalad_next-1.4.0/tools/appveyor/
+-rw-rw-r--   0 mih       (1000) mih       (1000)      291 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/chmod600.bat
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      311 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/docker-load-httpbin
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      124 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/enable-ssh-login
+-rw-rw-r--   0 mih       (1000) mih       (1000)      101 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/env_setup.bat
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      399 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/install-git-annex
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      331 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/install-syspkgs
+-rwxrwxr-x   0 mih       (1000) mih       (1000)     1464 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/setup-sshd
+-rw-rw-r--   0 mih       (1000) mih       (1000)     1054 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/setup-sshd.bat
+-rwxrwxr-x   0 mih       (1000) mih       (1000)      330 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/verify-ssh-access
+-rw-rw-r--   0 mih       (1000) mih       (1000)      343 2024-05-17 19:26:55.000000 datalad_next-1.4.0/tools/appveyor/verify-ssh-access.bat
+-rw-rw-r--   0 mih       (1000) mih       (1000)    86677 2024-05-17 19:26:55.000000 datalad_next-1.4.0/versioneer.py
```

### Comparing `datalad_next-1.3.0/.all-contributorsrc` & `datalad_next-1.4.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/.appveyor.yml` & `datalad_next-1.4.0/.appveyor.yml`

 * *Files 1% similar despite different names*

```diff
@@ -283,16 +283,16 @@
       # store original TMPDIR setting to limit modification to test execution
       - export PREV_TMPDIR=$TMPDIR
       # make TMPDIR a "crippled filesystem" to test wrong assumptions of POSIX-ness
       # on POSIX OSes. The test fixtures will create all test datasets under TMPDIR
       - |
         set -e
         if [ "$APPVEYOR_JOB_NAME" = "test-linux-crippled" ]; then
-          # 500 MB VFAT FS in a box
-          sudo dd if=/dev/zero of=/crippledfs.img count=500 bs=1M
+          # 750 MB VFAT FS in a box
+          sudo dd if=/dev/zero of=/crippledfs.img count=750 bs=1M
           sudo mkfs.vfat /crippledfs.img
           sudo mkdir /crippledfs
           sudo mount -o "uid=$(id -u),gid=$(id -g)" /crippledfs.img /crippledfs
           echo "== mount >>"
           mount | grep crippled
           echo "<< mount =="
           export TMPDIR=/crippledfs
```

### Comparing `datalad_next-1.3.0/.github/PULL_REQUEST_TEMPLATE.md` & `datalad_next-1.4.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/.github/workflows/docbuild.yml` & `datalad_next-1.4.0/.github/workflows/docbuild.yml`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     runs-on: ubuntu-latest
 
     steps:
     - name: Set up environment
       run: |
         git config --global user.email "test@github.land"
         git config --global user.name "GitHub Almighty"
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python 3.10
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: '3.10'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements-devel.txt
         pip install .
```

### Comparing `datalad_next-1.3.0/.github/workflows/mypy.yml` & `datalad_next-1.4.0/.github/workflows/mypy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,25 @@
       - '!**/tests/**.py'
 
 jobs:
   static-type-check:
     runs-on: ubuntu-latest
     steps:
       - name: Setup Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: 3.11
           architecture: x64
       - name: Checkout
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
       - name: Install mypy
         run: python -m pip install mypy  # you can pin your preferred version
       - name: Get Python changed files
         id: changed-py-files
-        uses: tj-actions/changed-files@v23
+        uses: tj-actions/changed-files@v44
         with:
           files: |
             *.py
             **/*.py
       - name: Type check changed files
         if: steps.changed-py-files.outputs.any_changed == 'true'
         run: |
```

### Comparing `datalad_next-1.3.0/.github/workflows/update-contributors.yml` & `datalad_next-1.4.0/.github/workflows/update-contributors.yml`

 * *Files 0% similar despite different names*

```diff
@@ -75,12 +75,12 @@
           fi
           echo "OPEN_PULL_REQUEST=${OPEN_PULL_REQUEST}" >> $GITHUB_ENV
           echo "PULL_REQUEST_FROM_BRANCH=${BRANCH_FROM}" >> $GITHUB_ENV
           echo "PULL_REQUEST_TITLE=[tributors] ${BRANCH_FROM}" >> $GITHUB_ENV
           echo "PULL_REQUEST_BODY='Tributors update automated pull request.\n\n[skip ci]'" >> $GITHUB_ENV
 
       - name: Open Pull Request
-        uses: vsoch/pull-request-action@1.0.24
+        uses: vsoch/pull-request-action@1.1.1
         if: ${{ env.OPEN_PULL_REQUEST == '1' }}
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          PULL_REQUEST_BRANCH: "main"
+          PULL_REQUEST_BRANCH: "main"
```

### Comparing `datalad_next-1.3.0/.zenodo.json` & `datalad_next-1.4.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/CHANGELOG.md` & `datalad_next-1.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,120 @@
+# 1.4.0 (2024-05-17)
+
+## 🐛 Bug Fixes
+
+- RIA over SSH access from Mac clients to Linux server was broken
+  due to an inappropriate platform check that assumed that local and
+  remote platform are identical.
+  Fixes https://github.com/datalad/datalad/issues/7536 via
+  https://github.com/datalad/datalad-next/pull/653 (by @mih)
+
+- `next-status` has received a number of fixes:
+
+  - It no longer issues undesirable modification reports
+    that are based on `mtime` changes alone (i.e., no content change).
+    Fixes https://github.com/datalad/datalad-next/issues/639 via
+    https://github.com/datalad/datalad-next/pull/650 (by @mih)
+  - It now detects staged changes in repositories with no
+    commit.
+    Fixes https://github.com/datalad/datalad-next/issues/680 via
+    https://github.com/datalad/datalad-next/pull/681 (by @mih)
+  - `next-status -r mono` now reports on new commits in submodules.
+    Previously this was ignored, leading to the impression of
+    clean datasets despite unsaved changes.
+    Fixes https://github.com/datalad/datalad-next/issues/645 via
+    https://github.com/datalad/datalad-next/pull/679 (by @mih)
+
+- `iter_annexworktree()` can now also be used on plain Git repos,
+  and would behave exactly as if reporting on non-annexed files
+  in a git-annex repo. Previously, a cryptic `iterable did not yield
+  matching item for route-in item, cardinality mismatch?` error was
+  issued in this case.
+  Fixes https://github.com/datalad/datalad-next/issues/670 via
+  https://github.com/datalad/datalad-next/pull/673 (by @mih)
+
+## 💫 Enhancements and new features
+
+- `datalad_next.shell` provides a context manager for (long-running)
+  shell or interpreter subprocesses. Within the context any number of
+  commands can be executed in such a shell, and each command can
+  process input (iterables), and yield output (iterables). This feature
+  is suitable for running and controlling "remote shells" like a login
+  shell on a server via SSH. A range of utilities is provided to
+  employ this functionality for special purpose implementations
+  (e.g., accept fixed-length or variable-length process output).
+  A suite of operations like download/upload file to a remote shell is
+  provided for POSIX-compliant shells `datalad_next.shell.operations.posix`.
+  https://github.com/datalad/datalad-next/pull/596 (by @christian-monch)
+
+- A rewrite of `SSHRemoteIO`, the RIA SSH-operations implementation from
+  datalad-core is provided as a patch. It is based on the new `shell`
+  feature, and provides more robust operations. It's IO performance is
+  at the same level as `scp`-based down/uploads. In contrast to the
+  original implementation, it support fine-grained progress reporting
+  for uploads and downloads.
+  Via https://github.com/datalad/datalad-next/pull/655 (by @mih)
+
+- The `SpecialRemote` base class in datalad-core is patched to support
+  a standard `close()` method for implementing resource release and cleanup
+  operations. The main special remote entry point has been altered to
+  run implementations within a `closing()` context manager to guarantee
+  execution of such handlers.
+  Via https://github.com/datalad/datalad-next/pull/655 (by @mih)
+
+- A new `has_initialized_annex()` helper function is provided to
+  test for a locally initialized annex in a repo.
+  Via https://github.com/datalad/datalad-next/pull/673 (by @mih)
+
+- `iter_annexworktree()` can now also be used on plain Git repositories,
+  and it yields the same output and behavior as running on a git-annex
+  repository with no annex'ed content (just tracked with Git).
+  Fixes https://github.com/datalad/datalad-next/issues/670 via
+  https://github.com/datalad/datalad-next/pull/673 (by @mih)
+
+- `next-status` and `iter_gitstatus()` have been improved to
+  report on further modifications after a file addition has been
+  originally staged.
+  Fixes https://github.com/datalad/datalad-next/issues/637 via
+  https://github.com/datalad/datalad-next/pull/679 (by @mih)
+
+- `next-status` result rendering has been updated to be more markedly
+  different than git-status's. Coloring is now exclusively
+  determined by the nature of a change, rather than being partially
+  similar to git-status's index-updated annotation. This reduces
+  the chance for misinterpretations, and does not create an undesirable
+  focus on the Git index (which is largely ignored by DataLad).
+  Fixes https://github.com/datalad/datalad-next/issues/640 via
+  https://github.com/datalad/datalad-next/pull/679 (by @mih)
+
+- A large 3k-line patch set replaces almost the entire RIA implementation,
+  including the ORA special remote, and the `create-sibling-ria` command.
+  The new implementation brings uniform support for Windows clients, progress
+  reporting for uploads and downloads via SSH, and a faster and more
+  robust behavior for SSH-based operations (based on the new remote
+  shell feature).
+  Fixes https://github.com/datalad/datalad-next/issues/654 via
+  https://github.com/datalad/datalad-next/pull/669 (by @christian-monch)
+
+## 📝 Documentation
+
+- Git-related subprocess execution helpers are now accessible in the
+  rendered documentation, and all supported file collections are now
+  mentioned in the `ls-file-collection` command help.
+  Fixes https://github.com/datalad/datalad-next/issues/668 via
+  https://github.com/datalad/datalad-next/pull/671 (by @mih)
+
+## 🛡 Tests
+
+- Test setup has been improved to support a uniform, datalad-next
+  enabled environment for subprocesses too. This extends the scope
+  of testing to special remote implementations and other code that
+  is executed in subprocesses, and relies on runtime patches.
+  See https://github.com/datalad/datalad-next/pull/i665 (by @mih)
+
 # 1.3.0 (2024-03-19)
 
 ## 💫 Enhancements and new features
 
 - Code organization is adjusted to clearly indicate what is part of the
   package's public Python API. Anything that can be imported directly from
   the top-level of any sub-package is part of the public API.
```

### Comparing `datalad_next-1.3.0/CITATION.cff` & `datalad_next-1.4.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/CONTRIBUTING.md` & `datalad_next-1.4.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 A sub-package contains any number of code files, and a `tests` directory with all test implementations for that particular sub-package, and only for that sub-package. Other, deeper directory hierarchies are not to be expected.
 
 There is no limit to the number of files. Contributors should strive for files with less than 500 lines of code.
 
 Within a sub-package, code should generally use relative imports. The corresponding tests should also import the tested code via relative imports.
 
-Code users should be able to import the most relevant functionality from the sub-package's `__init__.py`. Only items importable from the sub-package's top-level are considered to be part of its "public" API.
+Code users should be able to import the most relevant functionality from the sub-package's `__init__.py`. Only items importable from the sub-package's top-level are considered to be part of its "public" API. If a sub-module is imported in the sub-package's `__init__.py`, consider adding `__all__` to the sub-module to restrict wildcard imports from the sub-module, and to document what is considered to be part of the "public" API. 
 
 Sub-packages should be as self-contained as possible. Individual components in `datalad-next` should strive to be easily migratable to the DataLad core package. This means that any organization principles like *all-exceptions-go-into-a-single-location-in-datalad-next* do not apply. For example, each sub-package should define its exceptions separately from others. When functionality is shared between sub-packages, absolute imports should be made.
 
 There is one special sub-package in `datalad-next`: `patches`. All runtime patches to be applied to the DataLad core package must be placed here.
 
 
 ### Runtime patches
```

### Comparing `datalad_next-1.3.0/LICENSE` & `datalad_next-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/PKG-INFO` & `datalad_next-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_next
-Version: 1.3.0
+Version: 1.4.0
 Summary: What is next in DataLad
 Home-page: https://github.com/datalad/datalad-next
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -29,15 +29,14 @@
 Requires-Dist: requests_toolbelt; extra == "httpsupport"
 
 # DataLad NEXT extension
 
 [![All Contributors](https://img.shields.io/github/all-contributors/datalad/datalad-next?color=ee8449&style=flat-square)](#contributors)
 [![Build status](https://ci.appveyor.com/api/projects/status/dxomp8wysjb7x2os/branch/main?svg=true)](https://ci.appveyor.com/project/mih/datalad-next/branch/main)
 [![codecov](https://codecov.io/gh/datalad/datalad-next/branch/main/graph/badge.svg?token=2P8rak7lSX)](https://codecov.io/gh/datalad/datalad-next)
-[![crippled-filesystems](https://github.com/datalad/datalad-next/workflows/crippled-filesystems/badge.svg)](https://github.com/datalad/datalad-next/actions?query=workflow%3Acrippled-filesystems)
 [![docs](https://github.com/datalad/datalad-next/workflows/docs/badge.svg)](https://github.com/datalad/datalad-next/actions?query=workflow%3Adocs)
 [![Documentation Status](https://readthedocs.org/projects/datalad-next/badge/?version=latest)](http://docs.datalad.org/projects/next/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![GitHub release](https://img.shields.io/github/release/datalad/datalad-next.svg)](https://GitHub.com/datalad/datalad-next/releases/)
 [![PyPI version fury.io](https://badge.fury.io/py/datalad-next.svg)](https://pypi.python.org/pypi/datalad-next/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6833099.svg)](https://doi.org/10.5281/zenodo.6833099)
```

### Comparing `datalad_next-1.3.0/README.md` & `datalad_next-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # DataLad NEXT extension
 
 [![All Contributors](https://img.shields.io/github/all-contributors/datalad/datalad-next?color=ee8449&style=flat-square)](#contributors)
 [![Build status](https://ci.appveyor.com/api/projects/status/dxomp8wysjb7x2os/branch/main?svg=true)](https://ci.appveyor.com/project/mih/datalad-next/branch/main)
 [![codecov](https://codecov.io/gh/datalad/datalad-next/branch/main/graph/badge.svg?token=2P8rak7lSX)](https://codecov.io/gh/datalad/datalad-next)
-[![crippled-filesystems](https://github.com/datalad/datalad-next/workflows/crippled-filesystems/badge.svg)](https://github.com/datalad/datalad-next/actions?query=workflow%3Acrippled-filesystems)
 [![docs](https://github.com/datalad/datalad-next/workflows/docs/badge.svg)](https://github.com/datalad/datalad-next/actions?query=workflow%3Adocs)
 [![Documentation Status](https://readthedocs.org/projects/datalad-next/badge/?version=latest)](http://docs.datalad.org/projects/next/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![GitHub release](https://img.shields.io/github/release/datalad/datalad-next.svg)](https://GitHub.com/datalad/datalad-next/releases/)
 [![PyPI version fury.io](https://badge.fury.io/py/datalad-next.svg)](https://pypi.python.org/pypi/datalad-next/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6833099.svg)](https://doi.org/10.5281/zenodo.6833099)
```

### Comparing `datalad_next-1.3.0/_datalad_buildsupport/__init__.py` & `datalad_next-1.4.0/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/_datalad_buildsupport/formatters.py` & `datalad_next-1.4.0/_datalad_buildsupport/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/_datalad_buildsupport/setup.py` & `datalad_next-1.4.0/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/__init__.py` & `datalad_next-1.4.0/datalad_next/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexbackends/base.py` & `datalad_next-1.4.0/datalad_next/annexbackends/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexbackends/tests/test_base.py` & `datalad_next-1.4.0/datalad_next/annexbackends/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexbackends/xdlra.py` & `datalad_next-1.4.0/datalad_next/annexbackends/xdlra.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexremotes/__init__.py` & `datalad_next-1.4.0/datalad_next/annexremotes/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexremotes/archivist.py` & `datalad_next-1.4.0/datalad_next/annexremotes/archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexremotes/tests/test_archivist.py` & `datalad_next-1.4.0/datalad_next/annexremotes/tests/test_archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexremotes/tests/test_uncurl.py` & `datalad_next-1.4.0/datalad_next/annexremotes/tests/test_uncurl.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/annexremotes/uncurl.py` & `datalad_next-1.4.0/datalad_next/annexremotes/uncurl.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/archive_operations/__init__.py` & `datalad_next-1.4.0/datalad_next/archive_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/archive_operations/base.py` & `datalad_next-1.4.0/datalad_next/archive_operations/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/archive_operations/tarfile.py` & `datalad_next-1.4.0/datalad_next/archive_operations/tarfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/archive_operations/tests/test_tarfile.py` & `datalad_next-1.4.0/datalad_next/archive_operations/tests/test_tarfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/archive_operations/tests/test_zipfile.py` & `datalad_next-1.4.0/datalad_next/archive_operations/tests/test_zipfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/archive_operations/zipfile.py` & `datalad_next-1.4.0/datalad_next/archive_operations/zipfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/__init__.py` & `datalad_next-1.4.0/datalad_next/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/create_sibling_webdav.py` & `datalad_next-1.4.0/datalad_next/commands/create_sibling_webdav.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/credentials.py` & `datalad_next-1.4.0/datalad_next/commands/credentials.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/download.py` & `datalad_next-1.4.0/datalad_next/commands/download.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/ls_file_collection.py` & `datalad_next-1.4.0/datalad_next/commands/ls_file_collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -315,24 +315,31 @@
       is the SHA-type blob identifier as reported and used by Git.
       [PY: When hashes are computed, an ``fp`` property with a file-like is
       provided. Reading file data from it requires a ``seek(0)`` in most
       cases. This file handle is only open when items are yielded directly
       by this command (``return_type='generator``) and only until the next
       result is yielded. PY]
 
+    ``annexworktree``
+      Like ``gitworktree``, but amends the reported items with git-annex
+      information, such as ``annexkey``, ``annexsize``, and ``annnexobjpath``.
+
     ``tarfile``
       Reports on members of a TAR archive. The collection identifier is the
       path of the TAR file. Item identifiers are the relative paths
       of archive members within the archive. Reported properties are similar
       to the ``directory`` collection type.
       [PY: When hashes are computed, an ``fp`` property with a file-like
       is provided. Reading file data from it requires a ``seek(0)`` in most
       cases. This file handle is only open when items are yielded directly
       by this command (``return_type='generator``) and only until the next
       result is yielded. PY]
+
+    ``zipfile``
+      Like ``tarfile`` for reporting on ZIP archives.
     """
     _validator_ = LsFileCollectionParamValidator()
 
     # this is largely here for documentation and CLI parser building
     _params_ = dict(
         type=Parameter(
             args=("type",),
@@ -382,14 +389,21 @@
                  " data, but can retrieve the files after confirming"
                  " their availability (i.e., via `git annex fsck`)",
          'code_cmd':
          'datalad -f json ls-file-collection directory wwwdir --hash md5 \\\n'
          ' | jq \'. | select(.type == "file")\' \\\n'
          ' | jq --slurp . \\\n'
          " | datalad addurls --key 'et:MD5-s{size}--{hash-md5}' - 'https://example.com/{item}'"},
+        {'text': 'List annex keys of all files in the working tree of a dataset',
+         'code_py': "[r['annexkey'] \\\n"
+                    "for r in ls_file_collection('annexworktree', '.') \\\n"
+                    "if 'annexkey' in r]",
+         'code_cmd': "datalad -f json ls-file-collection annexworktree . \\\n"
+                     "| jq '. | select(.annexkey) | .annexkey'",
+        },
     ]
 
     @staticmethod
     @eval_results
     def __call__(
             type: str,
             collection: CollectionSpec,
```

### Comparing `datalad_next-1.3.0/datalad_next/commands/results.py` & `datalad_next-1.4.0/datalad_next/commands/results.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/status.py` & `datalad_next-1.4.0/datalad_next/commands/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,23 +52,14 @@
     added = 'added'
     modified = 'modified'
     deleted = 'deleted'
     untracked = 'untracked'
     unknown = 'unknown'
 
 
-STATE_COLOR_MAP = {
-    StatusState.added: ac.GREEN,
-    StatusState.modified: ac.RED,
-    StatusState.deleted: ac.RED,
-    StatusState.untracked: ac.RED,
-    StatusState.unknown: ac.YELLOW,
-}
-
-
 diffstatus2resultstate_map = {
     GitDiffStatus.addition: StatusState.added,
     GitDiffStatus.copy: StatusState.added,
     GitDiffStatus.deletion: StatusState.deleted,
     GitDiffStatus.modification: StatusState.modified,
     GitDiffStatus.rename: StatusState.added,
     GitDiffStatus.typechange: StatusState.modified,
@@ -354,20 +345,31 @@
         max_len = len('untracked')
         state = res.state.value
         # message format is same as for previous command implementation
         ui.message(u'{fill}{state}: {path}{type_}{annot}'.format(
             fill=' ' * max(0, max_len - len(state)),
             state=ac.color_word(
                 res.state.value,
-                STATE_COLOR_MAP.get(res.state)),
+                _get_result_status_render_color(res)),
             path=path,
             type_=' ({})'.format(ac.color_word(type_, ac.MAGENTA))
             if type_ else '',
             annot=f' [{", ".join(q.value for q in res.modification_types)}]'
             if res.modification_types else '',
         ))
 
     @staticmethod
     def custom_result_summary_renderer(results):
         # no reports, no changes
         if len(results) == 0:
             ui.message("nothing to save, working tree clean")
+
+
+def _get_result_status_render_color(res):
+    if res.state == StatusState.deleted:
+        return ac.RED
+    elif res.state == StatusState.modified:
+        return ac.CYAN
+    elif res.state == StatusState.added:
+        return ac.GREEN
+    else:
+        return ac.BOLD
```

### Comparing `datalad_next-1.3.0/datalad_next/commands/tests/test_create_sibling_webdav.py` & `datalad_next-1.4.0/datalad_next/commands/tests/test_create_sibling_webdav.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/tests/test_credentials.py` & `datalad_next-1.4.0/datalad_next/commands/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/tests/test_download.py` & `datalad_next-1.4.0/datalad_next/commands/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/tests/test_ls_file_collection.py` & `datalad_next-1.4.0/datalad_next/commands/tests/test_ls_file_collection.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/tests/test_results.py` & `datalad_next-1.4.0/datalad_next/commands/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/tests/test_status.py` & `datalad_next-1.4.0/datalad_next/commands/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/tests/test_tree.py` & `datalad_next-1.4.0/datalad_next/commands/tests/test_tree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/commands/tree.py` & `datalad_next-1.4.0/datalad_next/commands/tree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/config/tests/test_utils.py` & `datalad_next-1.4.0/datalad_next/config/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/config/utils.py` & `datalad_next-1.4.0/datalad_next/config/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -69,25 +69,34 @@
 
     Any existing declaration of configuration items in the environment is
     replaced. Any ENV variable of a *valid* existing declaration is removed,
     before the set configuration items are posted in the ENV.
 
     Multi-value configuration keys are supported (values provided as a tuple).
 
+    Any item with a value of ``None`` will be posted into the ENV with an
+    empty string as value, i.e. the corresponding ``GIT_CONFIG_VALUE_{count}``
+    variable will be an empty string. ``None`` item values indicate that the
+    configuration key was unset on the command line, via the global option
+    ``-c``.
+
     No verification (e.g., of syntax compliance) is performed.
     """
     _clean_env_from_gitconfig_items()
 
     count = 0
     for key, value in items.items():
         # homogeneous processing of multiple value items, and single values
         values = value if isinstance(value, tuple) else (value,)
         for v in values:
             environ[f'GIT_CONFIG_KEY_{count}'] = key
-            environ[f'GIT_CONFIG_VALUE_{count}'] = v
+            # we support None even though not an allowed input type, because
+            # of https://github.com/datalad/datalad/issues/7589
+            # this can be removed, when that issue is resolved.
+            environ[f'GIT_CONFIG_VALUE_{count}'] = '' if v is None else str(v)
             count += 1
     if count:
         environ['GIT_CONFIG_COUNT'] = str(count)
 
 
 def _clean_env_from_gitconfig_items():
     # we only care about intact specifications here, if there was cruft
```

### Comparing `datalad_next-1.3.0/datalad_next/conftest.py` & `datalad_next-1.4.0/datalad_next/conftest.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/__init__.py` & `datalad_next-1.4.0/datalad_next/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/base.py` & `datalad_next-1.4.0/datalad_next/constraints/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/basic.py` & `datalad_next-1.4.0/datalad_next/constraints/basic.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/compound.py` & `datalad_next-1.4.0/datalad_next/constraints/compound.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/dataset.py` & `datalad_next-1.4.0/datalad_next/constraints/dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/exceptions.py` & `datalad_next-1.4.0/datalad_next/constraints/exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/formats.py` & `datalad_next-1.4.0/datalad_next/constraints/formats.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/git.py` & `datalad_next-1.4.0/datalad_next/constraints/git.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/parameter.py` & `datalad_next-1.4.0/datalad_next/constraints/parameter.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/parameter_legacy.py` & `datalad_next-1.4.0/datalad_next/constraints/parameter_legacy.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/tests/test_base.py` & `datalad_next-1.4.0/datalad_next/constraints/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/tests/test_basic.py` & `datalad_next-1.4.0/datalad_next/constraints/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/tests/test_cmdarg_validation.py` & `datalad_next-1.4.0/datalad_next/constraints/tests/test_cmdarg_validation.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/tests/test_compound.py` & `datalad_next-1.4.0/datalad_next/constraints/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/tests/test_exceptions.py` & `datalad_next-1.4.0/datalad_next/constraints/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/tests/test_special_purpose.py` & `datalad_next-1.4.0/datalad_next/constraints/tests/test_special_purpose.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/tests/test_tutorial.py` & `datalad_next-1.4.0/datalad_next/constraints/tests/test_tutorial.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/constraints/utils.py` & `datalad_next-1.4.0/datalad_next/constraints/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/consts/__init__.py` & `datalad_next-1.4.0/datalad_next/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/credman/manager.py` & `datalad_next-1.4.0/datalad_next/credman/manager.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/credman/tests/test_credman.py` & `datalad_next-1.4.0/datalad_next/credman/tests/test_credman.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/datasets/__init__.py` & `datalad_next-1.4.0/datalad_next/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/datasets/annexrepo.py` & `datalad_next-1.4.0/datalad_next/datasets/annexrepo.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/exceptions/__init__.py` & `datalad_next-1.4.0/datalad_next/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/gitremotes/datalad_annex.py` & `datalad_next-1.4.0/datalad_next/gitremotes/datalad_annex.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/gitremotes/tests/test_datalad_annex.py` & `datalad_next-1.4.0/datalad_next/gitremotes/tests/test_datalad_annex.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/__init__.py` & `datalad_next-1.4.0/datalad_next/iter_collections/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/annexworktree.py` & `datalad_next-1.4.0/datalad_next/iter_collections/annexworktree.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from datalad_next.itertools import (
     itemize,
     load_json,
     route_in,
     route_out,
     StoreOnly,
 )
+from datalad_next.repo_utils import has_initialized_annex
 from datalad_next.runners import iter_git_subproc
 
 from .gitworktree import (
     GitWorktreeItem,
     GitWorktreeFileSystemItem,
     iter_gitworktree
 )
@@ -142,14 +143,28 @@
         path,
         untracked=untracked,
         link_target=False,
         fp=False,
         recursive=recursive,
     )
 
+    if not has_initialized_annex(path):
+        # this is not an annex repo.
+        # we just yield the items from the gitworktree iterator.
+        # we funnel them through the standard result item prep
+        # function for type equality.
+        # when a recursive-mode other than 'repository' will be
+        # implemented, this implementation needs to be double-checked
+        # to avoid decision making on submodules just based on
+        # the nature of the toplevel repo.
+        for item in glsf:
+            yield _get_worktree_item(
+                path, get_fs_info=link_target, git_item=item)
+        return
+
     git_fileinfo_store: list[Any] = list()
     # this is a technical helper that will just store a bunch of `None`s
     # for aligning item-results between git-ls-files and git-annex-find
     _annex_git_align: list[Any] = list()
 
     with \
             iter_git_subproc(
```

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/directory.py` & `datalad_next-1.4.0/datalad_next/iter_collections/directory.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/gitdiff.py` & `datalad_next-1.4.0/datalad_next/iter_collections/gitdiff.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     CommandError,
     iter_git_subproc,
 )
 from datalad_next.itertools import (
     decode_bytes,
     itemize,
 )
-from datalad_next.runners import call_git_oneline
+from datalad_next.runners import (
+    call_git,
+    call_git_oneline,
+)
 
 from .gittree import (
     GitTreeItem,
     GitTreeItemType,
     _mode_type_map,
 )
 
@@ -80,18 +83,22 @@
     prev_gittype: GitTreeItemType | None = None
 
     status: GitDiffStatus | None = None
     percentage: int | None = None
     """This is the percentage of similarity for copy-status and
     rename-status diff items, and the percentage of dissimilarity
     for modifications."""
-    modification_types: tuple[GitContainerModificationType] | None = None
+    modification_types: tuple[GitContainerModificationType, ...] | None = None
     """Qualifiers for modification types of container-type
     items (directories, submodules)."""
 
+    def __post_init__(self):
+        if self.status == GitDiffStatus.addition and self.gitsha is None:
+            self.add_modification_type(GitContainerModificationType.modified_content)
+
     @cached_property
     def prev_path(self) -> PurePosixPath | None:
         """Returns the item ``prev_name`` as a ``PurePosixPath``
         instance"""
         if self.prev_name is None:
             return None
         return PurePosixPath(self.prev_name)
@@ -206,14 +213,27 @@
         find_copies=find_copies,
         yield_tree_items=yield_tree_items,
         eval_submodule_state=eval_submodule_state,
     )
 
     cmd = _build_cmd(**kwargs)
 
+    if cmd[0] == 'diff-index':
+        # when we compare to the index, we need a refresh run to not have
+        # something like plain mtime changes trigger modification reports
+        # https://github.com/datalad/datalad-next/issues/639
+        call_git([
+            'update-index',
+            # must come first, we recurse ourselves
+            '--ignore-submodules',
+            # we want to continue the refresh when the index need updating
+            '-q',
+            '--refresh',
+        ])
+
     # when do we need to condense subdir reports into a single dir-report
     reported_dirs: set[str] = set()
     _single_dir = (cmd[0] == 'diff-index') and recursive == 'no'
     # diff-tree reports the compared tree when no from is given, we need
     # to skip that output below
     skip_first = (cmd[0] == 'diff-tree') and from_treeish is None
     pending_props = None
```

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/gitstatus.py` & `datalad_next-1.4.0/datalad_next/iter_collections/gitstatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging
 from pathlib import (
     Path,
     PurePath,
 )
 from typing import Generator
 
+from datalad_next.consts import PRE_INIT_COMMIT_SHA
 from datalad_next.runners import (
     CommandError,
     call_git_lines,
     iter_git_subproc,
 )
 from datalad_next.itertools import (
     decode_bytes,
@@ -95,14 +96,18 @@
       The ``name`` and ``prev_name`` attributes of an item are a ``str`` with
       the corresponding (relative) path, as reported by Git
       (in POSIX conventions).
     """
     path = Path(path)
 
     head, corresponding_head = get_worktree_head(path)
+    if head is None:
+        # no commit at all -> compare to an empty repo.
+        head = PRE_INIT_COMMIT_SHA
+
     # TODO it would make sense to always (or optionally) compare against any
     # existing corresponding_head. This would make the status communicate
     # anything that has not made it into the corresponding branch yet
 
     common_args = dict(
         head=head,
         path=path,
@@ -158,23 +163,23 @@
             for item in iter_gitworktree(
                 path,
                 untracked=untracked,
                 recursive='no',
             )
         }
     # diff constrained to direct children
-    for item in ([] if head is None else iter_gitdiff(
+    for item in iter_gitdiff(
         path,
-        from_treeish='HEAD',
+        from_treeish=head,
         # to the worktree
         to_treeish=None,
         recursive='no',
         # TODO trim scope like in repo_items
         eval_submodule_state=eval_submodule_state,
-    )):
+    ):
         if item.status != GitDiffStatus.deletion \
                 and item.gittype in container_types:
             if item.gittype == GitTreeItemType.submodule:
                 # issue standard submodule container report
                 _eval_submodule(path, item, eval_submodule_state)
             else:
                 dir_path = path / item.path
@@ -247,25 +252,25 @@
     present_submodules = {
         # stringify name for speedy comparison
         # TODO double-check that comparisons are primarily with
         # GitDiffItem.name which is str
         str(item.name): item for item in iter_submodules(path)
     }
     # start with a repository-contrained diff against the worktree
-    for item in ([] if head is None else iter_gitdiff(
+    for item in iter_gitdiff(
         path,
-        from_treeish='HEAD',
+        from_treeish=head,
         # to the worktree
         to_treeish=None,
         recursive='repository',
         # we should be able to go cheaper with the submodule evaluation here.
         # We need to redo some check for adjusted mode, and other cases anyways
         eval_submodule_state='commit'
         if eval_submodule_state == 'full' else eval_submodule_state,
-    )):
+    ):
         # immediately investigate any submodules that are already
         # reported modified by Git
         if item.gittype == GitTreeItemType.submodule:
             _eval_submodule(path, item, eval_submodule_state)
             # we dealt with this submodule
             present_submodules.pop(item.name, None)
         if item.status:
@@ -312,20 +317,22 @@
     for item in _yield_repo_items(
         head=head,
         path=path,
         untracked=untracked,
         # TODO do we need to adjust the eval mode here for the diff recmodes?
         eval_submodule_state=eval_submodule_state,
     ):
-        # we get to see any submodule item passing through here, and can simply
-        # call this function again for a subpath
+        # there is nothing else to do for any non-submodule item
         if item.gittype != GitTreeItemType.submodule:
             yield item
             continue
 
+        # we get to see any submodule item passing through here, and can simply
+        # call this function again for a subpath
+
         # submodule recursion
         # the .path of a GitTreeItem is always POSIX
         sm_path = path / item.path
         if recursion_mode == 'submodules':
             # in this mode, we run the submodule status against it own
             # worktree head
             sm_head, _ = get_worktree_head(sm_path)
@@ -338,14 +345,22 @@
             # respect to the recorded state in the parent. This is either
             # the current gitsha, or (if git detected a committed
             # modification) the previous sha. This way, any further report
             # on changes a comprehensive from the point of view of the parent
             # repository, hence no submodule item is emitted
             sm_head = item.gitsha or item.prev_gitsha
 
+            if GitContainerModificationType.new_commits in item.modification_types:
+                # this is a submodule that has new commits compared to
+                # its state in the parent dataset. We need to yield this
+                # item, even if nothing else is modified, because otherwise
+                # this (unsafed) changed would go unnoticed
+                # https://github.com/datalad/datalad-next/issues/645
+                yield item
+
         for i in _yield_hierarchy_items(
             head=sm_head,
             path=sm_path,
             untracked=untracked,
             # TODO here we could implement handling for a recursion-depth limit
             recursion_mode=recursion_mode,
             eval_submodule_state=eval_submodule_state,
```

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/gittree.py` & `datalad_next-1.4.0/datalad_next/iter_collections/gittree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/gitworktree.py` & `datalad_next-1.4.0/datalad_next/iter_collections/gitworktree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tarfile.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tarfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_iterannexworktree.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterannexworktree.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 )
 
 from datalad import cfg as dlcfg
 
 from datalad_next.datasets import Dataset
 from datalad_next.utils import check_symlink_capability
 
-from ..gitworktree import GitTreeItemType
+from ..gitworktree import (
+    GitTreeItemType,
+    iter_gitworktree,
+)
 from ..annexworktree import iter_annexworktree
 
 from .test_itergitworktree import prep_fp_tester
 
 
 def _mkds(tmp_path_factory, monkeypatch, cfg_overrides):
     with monkeypatch.context() as m:
@@ -113,7 +116,17 @@
     all_items = list(iter_annexworktree(
         existing_dataset.pathobj, recursive='no'))
     # we get a .datalad directory-tyoe item, rather than the file item from
     # inside the dir
     dirs = [i for i in all_items if i.gittype == GitTreeItemType.directory]
     assert len(dirs) == 1
     dirs[0].name == PurePath('.datalad')
+
+
+def test_iter_annexworktree_noannex(existing_noannex_dataset):
+    # plain smoke test to ensure this can run on a dataset without an annex
+    all_annex_items = list(
+        iter_annexworktree(existing_noannex_dataset.pathobj))
+    all_git_items = list(iter_gitworktree(existing_noannex_dataset.pathobj))
+    assert len(all_annex_items) == len(all_git_items)
+    for a, g in zip(all_annex_items, all_git_items):
+        assert a.name == g.name
```

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_iterdir.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterdir.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergitdiff.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitdiff.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergitstatus.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitstatus.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,20 @@
             or GitContainerModificationType.untracked_content in i.modification_types
             for i in st.values()
             if 'u' in i.path.name.split('_')[1]
         )
 
         # anything modified is labeled as such
         assert all(
+            # either directly
             i.status == GitDiffStatus.modification
+            # or as an addition with a modification on top
+            or (i.status == GitDiffStatus.addition
+                and GitContainerModificationType.modified_content
+                    in i.modification_types)
             for i in st.values()
             if 'm' in i.path.name.split('_')[1]
         )
 
         # anything deleted is labeled as such
         assert all(
             i.status == GitDiffStatus.deletion
@@ -209,26 +214,42 @@
         )
     }
     # in this mode we expect ALL results of a 'repository' mode recursion,
     # including the submodule-type items, plus additional ones from within
     # the submodules
     _assert_testcases(
         st,
-        # repository and recursive test cases, minus any direct submodule
-        # items
+        # repository and recursive test cases
         [c for c in chain(test_cases_repository_recursion,
                           test_cases_submodule_recursion)
-         if not c['name'].split('/')[-1].split('_')[0] == 'sm'])
+         # minus any submodule that have no new commits
+         # (this only thing that is not attributable to individual
+         # content changes)
+         if not c['name'].split('/')[-1] in (
+             'sm_m', 'sm_mu', 'sm_u',
+         )])
 
 
 def test_status_gitinit(tmp_path):
     # initialize a fresh git repo, but make no commits
     assert call_git_success(['init'], cwd=tmp_path)
     for recmode in ('no', 'repository', 'submodules'):
         assert [] == list(iter_gitstatus(tmp_path, recursive=recmode))
     # untracked reporting must be working normal
     (tmp_path / 'untracked').touch()
     for recmode in ('no', 'repository', 'submodules'):
         res = list(iter_gitstatus(tmp_path, recursive=recmode))
         assert len(res) == 1
         assert res[0].name == 'untracked'
         assert res[0].status == GitDiffStatus.other
+
+
+def test_status_nohead_staged(tmp_path):
+    # initialize a fresh git repo, but make no commits
+    assert call_git_success(['init'], cwd=tmp_path)
+    # stage a file
+    (tmp_path / 'probe').write_text('tostage')
+    assert call_git_success(['add', 'probe'], cwd=tmp_path)
+    _assert_testcases(
+        {i.name: i for i in iter_gitstatus(tmp_path)},
+        [{'name': 'probe', 'status': GitDiffStatus.addition}],
+    )
```

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergittree.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergittree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itergitworktree.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itergitworktree.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_itertar.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_itertar.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_iterzip.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_iterzip.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/tests/test_utils.py` & `datalad_next-1.4.0/datalad_next/iter_collections/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/utils.py` & `datalad_next-1.4.0/datalad_next/iter_collections/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iter_collections/zipfile.py` & `datalad_next-1.4.0/datalad_next/iter_collections/zipfile.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/deploy-package-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/.github/workflows/test.yml` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/.gitignore` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/.gitignore`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/LICENSE` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/README.md` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/README.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/__init__.py` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/iterable_subprocess.py` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/iterable_subprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,38 @@
 from subprocess import PIPE, Popen
 from threading import Thread
 
 # Importing from datalad-core to prevent circular imports
 from datalad_next.exceptions import CommandError
 
 
+class OutputFrom(Generator):
+    def __init__(self, stdout, stderr_deque, chunk_size=65536):
+        self.stdout = stdout
+        self.stderr_deque = stderr_deque
+        self.chunk_size = chunk_size
+        self.returncode = None
+
+    def send(self, _):
+        chunk = self.stdout.read(self.chunk_size)
+        if not chunk:
+            raise StopIteration
+        return chunk
+
+    def throw(self, typ, value=None, traceback=None):
+        return super().throw(typ, value, traceback)
+
+
 @contextmanager
 def iterable_subprocess(
     program,
     input_chunks,
     chunk_size=65536,
     cwd=None,
+    bufsize=-1,
 ):
     # This context starts a thread that populates the subprocess's standard input. It
     # also starts a threads that reads the process's standard error. Otherwise we risk
     # a deadlock - there is no output because the process is waiting for more input.
     #
     # This itself introduces its own complications and risks, but hopefully mitigated
     # by having a well defined start and stop mechanism that also avoid sending data
@@ -101,28 +119,14 @@
             except OSError as e:
                 # silently ignore Errno22, which happens on
                 # windows when trying to interacted with file descriptors
                 # associated with a process that exited already
                 if e.errno != 22:
                     raise
 
-    class OutputFrom(Generator):
-        def __init__(self, stdout):
-            self.stdout = stdout
-            self.returncode = None
-
-        def send(self, _):
-            chunk = self.stdout.read(chunk_size)
-            if not chunk:
-                raise StopIteration
-            return chunk
-
-        def throw(self, typ, value=None, traceback=None):
-            return super().throw(typ, value, traceback)
-
     def keep_only_most_recent(stderr, stderr_deque):
         total_length = 0
         while True:
             chunk = stderr.read(chunk_size)
             total_length += len(chunk)
             if not chunk:
                 break
@@ -140,35 +144,40 @@
     chunk_generator = None
     exception_stdin = None
     exception_stderr = None
 
     try:
 
         with \
-                Popen(
+                Popen(  # nosec - all arguments are controlled by the caller
                     program,
                     stdin=PIPE,
                     stdout=PIPE,
                     stderr=PIPE,
                     cwd=cwd,
+                    bufsize=bufsize,
                 ) as proc, \
                 thread(
                     keep_only_most_recent,
                     proc.stderr,
                     stderr_deque,
                 ) as (start_t_stderr, join_t_stderr), \
                 thread(
                     input_to,
                     proc.stdin,
                 ) as (start_t_stdin, join_t_stdin):
 
             try:
                 start_t_stderr()
                 start_t_stdin()
-                chunk_generator = OutputFrom(proc.stdout)
+                chunk_generator = OutputFrom(
+                    proc.stdout,
+                    stderr_deque,
+                    chunk_size
+                )
                 yield chunk_generator
             except BaseException:
                 proc.terminate()
                 raise
             finally:
                 proc.stdout.close()
                 exception_stdin = join_t_stdin()
```

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/pyproject.toml` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/iterable_subprocess/test_iterable_subprocess.py` & `datalad_next-1.4.0/datalad_next/iterable_subprocess/test_iterable_subprocess.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/__init__.py` & `datalad_next-1.4.0/datalad_next/itertools/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/align_pattern.py` & `datalad_next-1.4.0/datalad_next/itertools/align_pattern.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ Function to ensure that a pattern is completely contained in single chunks
 """
 
 from __future__ import annotations
 
+import re
 from typing import (
     Generator,
     Iterable,
 )
 
 
 def align_pattern(iterable: Iterable[str | bytes | bytearray],
@@ -70,33 +71,39 @@
     -------
     str | bytes | bytearray
         data chunks that have at least the size of the pattern and do not end
         with a prefix of the pattern. Note that a data chunk might contain the
         pattern multiple times.
     """
 
-    def ends_with_pattern_prefix(data: str | bytes | bytearray,
-                                 pattern: str | bytes | bytearray,
-                                 ) -> bool:
-        """ Check whether the chunk ends with a prefix of the pattern """
-        for index in range(len(pattern) - 1, 0, -1):
-            if data[-index:] == pattern[:index]:
-                return True
-        return False
-
+    # Create pattern matcher for all
+    if isinstance(pattern, str):
+        regex: str | bytes | bytearray = '(' + '|'.join(
+            '.' * (len(pattern) - index - 1) + re.escape(pattern[:index]) + '$'
+            for index in range(1, len(pattern))
+        ) + ')'
+    else:
+        regex = b'(' + b'|'.join(
+            b'.' * (len(pattern) - index - 1) + re.escape(pattern[:index]) + b'$'
+            for index in range(1, len(pattern))
+        ) + b')'
+    pattern_matcher = re.compile(regex, re.DOTALL)
+    pattern_sub = len(pattern) - 1
     # Join data chunks until they are sufficiently long to contain the pattern,
     # i.e. have at least size: `len(pattern)`. Continue joining, if the chunk
     # ends with a prefix of the pattern.
     current_chunk = None
     for data_chunk in iterable:
         # get the type of current_chunk from the type of this data_chunk
         if current_chunk is None:
             current_chunk = data_chunk
         else:
             current_chunk += data_chunk
         if len(current_chunk) >= len(pattern) \
-                and not ends_with_pattern_prefix(current_chunk, pattern):
+                and not (
+                    current_chunk[-1] in pattern
+                    and pattern_matcher.match(current_chunk, len(current_chunk) - pattern_sub)):
             yield current_chunk
             current_chunk = None
 
     if current_chunk is not None:
         yield current_chunk
```

### Comparing `datalad_next-1.3.0/datalad_next/itertools/decode_bytes.py` & `datalad_next-1.4.0/datalad_next/itertools/decode_bytes.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/itemize.py` & `datalad_next-1.4.0/datalad_next/itertools/itemize.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/load_json.py` & `datalad_next-1.4.0/datalad_next/itertools/load_json.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/reroute.py` & `datalad_next-1.4.0/datalad_next/itertools/reroute.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/tests/test_decode_bytes.py` & `datalad_next-1.4.0/datalad_next/itertools/tests/test_decode_bytes.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/tests/test_itemize.py` & `datalad_next-1.4.0/datalad_next/itertools/tests/test_itemize.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/tests/test_load_json.py` & `datalad_next-1.4.0/datalad_next/itertools/tests/test_load_json.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/itertools/tests/test_reroute.py` & `datalad_next-1.4.0/datalad_next/itertools/tests/test_reroute.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/__init__.py` & `datalad_next-1.4.0/datalad_next/patches/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/annexrepo.py` & `datalad_next-1.4.0/datalad_next/patches/annexrepo.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/cli_configoverrides.py` & `datalad_next-1.4.0/datalad_next/patches/cli_configoverrides.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/commanderror.py` & `datalad_next-1.4.0/datalad_next/patches/commanderror.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/configuration.py` & `datalad_next-1.4.0/datalad_next/patches/configuration.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/create_sibling_ghlike.py` & `datalad_next-1.4.0/datalad_next/patches/create_sibling_ghlike.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/create_sibling_gitlab.py` & `datalad_next-1.4.0/datalad_next/patches/create_sibling_gitlab.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/customremotes_main.py` & `datalad_next-1.4.0/datalad_next/patches/customremotes_main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,24 @@
-"""Connect ``log_progress``-style progress reporting to git-annex
+"""Connect ``log_progress``-style progress reporting to git-annex, add `close()`
 
 This patch introduces a dedicated progress log handler as a proxy between
 standard datalad progress logging and a git-annex special remote as
 an approach to report (data transfer) progress to a git-annex parent process.
 
 This functionality is only (to be) used in dedicated special remote processes.
+
+This patch also adds a standard `close()` handler to special remotes, and calls
+that handler in a context manager to ensure releasing any resources. This
+replaces the custom `stop()` method, which is undocumented and only used by the
+`datalad-archive` special remote.
+
+This patch also adds code that allows to patch a class that is already loaded
 """
 
+from contextlib import closing
 import logging
 from typing import (
     Dict,
     Type,
 )
 
 from . import apply_patch
@@ -107,30 +115,50 @@
 
     .. seealso::
 
        :class:`AnnexProgressLogHandler`
     """
     assert cls is not None
     from annexremote import Master
-    master = Master()
-    remote = cls(master)
-    master.LinkRemote(remote)
 
-    # we add an additional handler to the logger to deal with
-    # progress reports
-    dlroot_lgr = logging.getLogger('datalad')
-    phandler = AnnexProgressLogHandler(remote)
-    phandler.addFilter(only_progress_logrecords)
-    dlroot_lgr.addHandler(phandler)
-
-    # run the remote
-    master.Listen()
-    # cleanup
-    if hasattr(remote, 'stop'):
-        remote.stop()
+    # Reload the class, to allow `cls` itself to be patched.
+    new_module = __import__(cls.__module__, fromlist=[cls.__name__])
+    cls = getattr(new_module, cls.__name__)
 
+    master = Master()
+    # this context manager use relies on patching in a close() below
+    with closing(cls(master)) as remote:
+        master.LinkRemote(remote)
+
+        # we add an additional handler to the logger to deal with
+        # progress reports
+        dlroot_lgr = logging.getLogger('datalad')
+        phandler = AnnexProgressLogHandler(remote)
+        phandler.addFilter(only_progress_logrecords)
+        dlroot_lgr.addHandler(phandler)
+
+        # run the remote
+        master.Listen()
+        # cleanup special case datalad-core `archive` remote
+        # nobody should do this, use `close()`
+        if hasattr(remote, 'stop'):
+            remote.stop()
+
+
+# a default cleanup handler for CoreBaseSpecialRemote
+# this enables us to use a standard `closing()` context manager with
+# special remotes
+def specialremote_defaultclose_noop(self):
+    pass
 
+
+apply_patch(
+    'datalad.customremotes', 'SpecialRemote', 'close',
+    specialremote_defaultclose_noop,
+    msg='Retrofit `SpecialRemote` with a `close()` handler',
+    expect_attr_present=False,
+)
 apply_patch(
     'datalad.customremotes.main', None, '_main',
     patched_underscore_main,
     msg='Replace special remote _main() '
     "with datalad-next's progress logging enabled variant")
```

### Comparing `datalad_next-1.3.0/datalad_next/patches/distribution_dataset.py` & `datalad_next-1.4.0/datalad_next/patches/distribution_dataset.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/interface_utils.py` & `datalad_next-1.4.0/datalad_next/patches/interface_utils.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/push_optimize.py` & `datalad_next-1.4.0/datalad_next/patches/push_optimize.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/push_to_export_remote.py` & `datalad_next-1.4.0/datalad_next/patches/push_to_export_remote.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/run.py` & `datalad_next-1.4.0/datalad_next/patches/run.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/siblings.py` & `datalad_next-1.4.0/datalad_next/patches/siblings.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/test_keyring.py` & `datalad_next-1.4.0/datalad_next/patches/test_keyring.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_annex_progress_logging.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_annex_progress_logging.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_cli_configoverrides.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_cli_configoverrides.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_commanderror.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_commanderror.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_configuration.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_create_sibling_ghlike.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_ghlike.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_create_sibling_gitlab.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_create_sibling_gitlab.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_push.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_push.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_push_to_export_remote.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_push_to_export_remote.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/tests/test_run.py` & `datalad_next-1.4.0/datalad_next/patches/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/patches/update.py` & `datalad_next-1.4.0/datalad_next/patches/update.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/repo_utils/tests/test_head.py` & `datalad_next-1.4.0/datalad_next/repo_utils/tests/test_head.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/repo_utils/worktree.py` & `datalad_next-1.4.0/datalad_next/repo_utils/worktree.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,24 @@
     call_git_lines,
 )
 
 
 def get_worktree_head(
     path: Path,
 ) -> tuple[str | None, str | None]:
+    """Returns the symbolic name of the worktree `HEAD` at the given path
+
+    Returns
+    -------
+    tuple
+      The first item is the symbolic name of the worktree `HEAD`, or `None`
+      if there is no commit.
+      The second item is the symbolic name of the "corresponding branch" in
+      an adjusted-mode git-annex repository, or `None`.
+    """
     try:
         HEAD = call_git_lines(
             # we add the pathspec disambiguator to get cleaner error messages
             # (and we only report the first item below, to take it off again)
             ['rev-parse', '-q', '--symbolic-full-name', 'HEAD', '--'],
             cwd=path,
             # we are doing error message parsing below, fix the language
```

### Comparing `datalad_next-1.3.0/datalad_next/runners/git.py` & `datalad_next-1.4.0/datalad_next/runners/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
 def call_git(
     args: list[str],
     *,
     cwd: Path | None = None,
     force_c_locale: bool = False,
 ) -> None:
-    """Call git with no output capture, raises on non-zero exit.
+    """Call Git with no output capture, raises on non-zero exit.
 
     If ``cwd`` is not None, the function changes the working directory to
     ``cwd`` before executing the command.
 
     If ``force_c_locale`` is ``True`` the environment of the Git process
     is altered to ensure output according to the C locale. This is useful
     when output has to be processed in a locale invariant fashion.
@@ -92,15 +92,15 @@
 
 def call_git_success(
     args: list[str],
     *,
     cwd: Path | None = None,
     capture_output: bool = False,
 ) -> bool:
-    """Call Git for a single line of output.
+    """Call Git and report success or failure of the command
 
     ``args`` is a list of arguments for the Git command. This list must not
     contain the Git executable itself. It will be prepended (unconditionally)
     to the arguments before passing them on.
 
     If ``cwd`` is not None, the function changes the working directory to
     ``cwd`` before executing the command.
@@ -124,15 +124,15 @@
 def call_git_lines(
     args: list[str],
     *,
     cwd: Path | None = None,
     input: str | None = None,
     force_c_locale: bool = False,
 ) -> list[str]:
-    """Call Git for any (small) number of lines of output.
+    """Call Git for any (small) number of lines of output
 
     ``args`` is a list of arguments for the Git command. This list must not
     contain the Git executable itself. It will be prepended (unconditionally)
     to the arguments before passing them on.
 
     If ``cwd`` is not None, the function changes the working directory to
     ``cwd`` before executing the command.
@@ -164,15 +164,15 @@
 def call_git_oneline(
     args: list[str],
     *,
     cwd: Path | None = None,
     input: str | None = None,
     force_c_locale: bool = False,
 ) -> str:
-    """Call git for a single line of output.
+    """Call Git for a single line of output
 
     If ``cwd`` is not None, the function changes the working directory to
     ``cwd`` before executing the command.
 
     If ``input`` is not None, the argument becomes the subprocess’s stdin.
     This is intended for small-scale inputs. For call that require processing
     large inputs, ``iter_git_subproc()`` is to be preferred.
```

### Comparing `datalad_next-1.3.0/datalad_next/runners/iter_subproc.py` & `datalad_next-1.4.0/datalad_next/runners/iter_subproc.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 
 from pathlib import Path
 from typing import (
     Iterable,
     List,
 )
 
-from datalad_next.iterable_subprocess import iterable_subprocess
+from datalad_next.iterable_subprocess.iterable_subprocess import (
+    iterable_subprocess,
+    OutputFrom,
+)
 from datalad_next.exceptions import CommandError
 from datalad_next.consts import COPY_BUFSIZE
 
 __all__ = ['iter_subproc']
 
 
 def iter_subproc(
     args: List[str],
     *,
     input: Iterable[bytes] | None = None,
     chunk_size: int = COPY_BUFSIZE,
     cwd: Path | None = None,
+    bufsize: int = -1,
 ):
     """Context manager to communicate with a subprocess using iterables
 
     This offers a higher level interface to subprocesses than Python's
     built-in ``subprocess`` module. It allows a subprocess to be naturally
     placed in a chain of iterables as part of a data processing pipeline.
     It is also helpful when data won't fit in memory and has to be streamed.
@@ -84,18 +88,22 @@
     input: iterable, optional
       If given, chunks of ``bytes`` to be written, iteratively, to the
       subprocess's ``stdin``.
     chunk_size: int, optional
       Size of chunks to read from the subprocess's stdout/stderr in bytes.
     cwd: Path
       Working directory for the subprocess, passed to ``subprocess.Popen``.
+    bufsize: int, optional
+      Buffer size to use for the subprocess's ``stdin``, ``stdout``, and
+      ``stderr``. See ``subprocess.Popen`` for details.
 
     Returns
     -------
     contextmanager
     """
     return iterable_subprocess(
         args,
         tuple() if input is None else input,
         chunk_size=chunk_size,
         cwd=cwd,
+        bufsize=bufsize,
     )
```

### Comparing `datalad_next-1.3.0/datalad_next/runners/protocols.py` & `datalad_next-1.4.0/datalad_next/runners/protocols.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/runners/tests/test_git.py` & `datalad_next-1.4.0/datalad_next/runners/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/runners/tests/test_iter_subproc.py` & `datalad_next-1.4.0/datalad_next/runners/tests/test_iter_subproc.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/tests/__init__.py` & `datalad_next-1.4.0/datalad_next/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/tests/fixtures.py` & `datalad_next-1.4.0/datalad_next/tests/fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -127,25 +127,29 @@
     backend.file_path = prev_fpath
 
 
 # the following is taken from datalad/conftest.py
 # sadly, this is defined inline and cannot be reused directly
 standard_gitconfig = """\
 [user]
-        name = DataLad Tester
-        email = test@example.com
+    name = DataLad Tester
+    email = test@example.com
 [core]
-	askPass =
+    askPass =
 [datalad "log"]
-        exc = 1
+    exc = 1
+[datalad "extensions"]
+    # load the next extension to be able to test patches of annex remotes
+    # that run in subprocesses
+    load = next
 [annex "security"]
-	# from annex 6.20180626 file:/// and http://localhost access isn't
-	# allowed by default
-	allowed-url-schemes = http https file
-	allowed-http-addresses = all
+    # from annex 6.20180626 file:/// and http://localhost access isn't
+    # allowed by default
+    allowed-url-schemes = http https file
+    allowed-http-addresses = all
 [protocol "file"]
     # since git 2.38.1 cannot by default use local clones for submodules
     # https://github.blog/2022-10-18-git-security-vulnerabilities-announced/#cve-2022-39253
     allow = always
 """ + os.environ.get('DATALAD_TESTS_GITCONFIG', '').replace('\\n', os.linesep)
 
 
@@ -301,14 +305,15 @@
 
         ❯ git status -uall
         On branch dl-test-branch
         Changes to be committed:
           (use "git restore --staged <file>..." to unstage)
                 new file:   dir_m/file_a
                 new file:   file_a
+                new file:   file_am
 
         Changes not staged for commit:
           (use "git add/rm <file>..." to update what will be committed)
           (use "git restore <file>..." to discard changes in working directory)
           (commit or discard the untracked or modified content in submodules)
                 deleted:    dir_d/file_d
                 deleted:    dir_m/file_d
@@ -316,24 +321,26 @@
                 deleted:    dir_sm/sm_d
                 modified:   dir_sm/sm_m (modified content)
                 modified:   dir_sm/sm_mu (modified content, untracked content)
                 modified:   dir_sm/sm_n (new commits)
                 modified:   dir_sm/sm_nm (new commits, modified content)
                 modified:   dir_sm/sm_nmu (new commits, modified content, untracked content)
                 modified:   dir_sm/sm_u (untracked content)
+                modified:   file_am
                 deleted:    file_d
                 modified:   file_m
 
         Untracked files:
           (use "git add <file>..." to include in what will be committed)
                 dir_m/dir_u/file_u
                 dir_m/file_u
                 dir_u/file_u
                 file_u
 
+
     Suffix indicates the ought-to state (multiple possible):
 
     a - added
     c - clean
     d - deleted
     n - new commits
     m - modified
@@ -398,14 +405,19 @@
     (ds.pathobj / 'file_d').unlink()
     # added items
     for smname in ('.', 'dir', 'sm_m', 'sm_nm', 'sm_mu', 'sm_nmu'):
         obj = dss[smname]
         pobj = obj.pathobj if isinstance(obj, Dataset) else obj
         (pobj / 'file_a').write_text('added')
         assert call_git_success(['add', 'file_a'], cwd=pobj)
+    # added and then modified file
+    file_am_obj = ds.pathobj / 'file_am'
+    file_am_obj.write_text('added')
+    assert call_git_success(['add', 'file_am'], cwd=ds.pathobj)
+    file_am_obj.write_text('modified')
 
     # record git-status output as a reference
     status_start = call_git_lines(['status'], cwd=ds.pathobj)
     yield ds
     # compare with initial git-status output, if there are any
     # differences the assumptions of any consuming test could be
     # invalidated. The modifying code must be found and fixed
@@ -660,17 +672,20 @@
         info[e] = v
 
     yield info
 
 
 @pytest.fixture(autouse=False, scope="function")
 def sshserver(sshserver_setup, datalad_cfg, monkeypatch):
+    # strip any leading / from the path, we add one, and
+    # only one below
+    sshserver_path = sshserver_setup['SSH_PATH'].lstrip('/')
     baseurl = f"ssh://{sshserver_setup['SSH_LOGIN']}" \
         f"@{sshserver_setup['HOST']}" \
         f":{sshserver_setup['SSH_PORT']}" \
-        f"/{sshserver_setup['SSH_PATH']}"
+        f"/{sshserver_path}"
     with monkeypatch.context() as m:
         m.setenv("DATALAD_SSH_IDENTITYFILE", sshserver_setup['SSH_SECKEY'])
         # force reload the config manager, to ensure the private key setting
         # makes it into the active config
         datalad_cfg.reload(force=True)
         yield baseurl, Path(sshserver_setup['LOCALPATH'])
```

### Comparing `datalad_next-1.3.0/datalad_next/tests/utils.py` & `datalad_next-1.4.0/datalad_next/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 from datalad.tests.test_utils_testrepos import BasicGitTestRepo
 from datalad.cli.tests.test_main import run_main
 from datalad.ui.progressbars import SilentProgressBar
 from datalad.utils import (
     create_tree,
     md5sum,
 )
+from datalad_next.shell import shell
 from datalad_next.utils import (
     CredentialManager,
 )
 
 lgr = logging.getLogger("datalad.tests.utils")
 
 
@@ -273,31 +274,31 @@
     given, it must be a representation of that server-side path on the local
     file system (e.g., a bindmount), and the helper tests whether the created
     content is also reflected in this directory.
     """
     # we can only handle openssh
     ssh_bin = os.environ.get('DATALAD_SSH_EXECUTABLE', 'ssh')
 
-    ssh_call = [
+    ssh_bash_call = [
         ssh_bin,
         '-i', seckey,
         '-p', port,
         f'{login}@{host}',
+        'bash',
     ]
     # now try if this is a viable configuration
     # verify execute and write permissions (implicitly also POSIX path handling
-    subprocess.run(
-        ssh_call + [
-            f"bash -c 'mkdir -p {path} && touch {path}/datalad-tests-probe'"],
-        stdin=subprocess.PIPE,
-        check=True,
-    )
-    if localpath:
-        # check if a given
-        assert (Path(localpath) / 'datalad-tests-probe').exists()
-    subprocess.run(
-        ssh_call + [f"bash -c 'rm {path}/datalad-tests-probe'"],
-        stdin=subprocess.PIPE,
-        check=True,
-    )
+    from more_itertools import consume
+    with shell(ssh_bash_call) as ssh:
+        # each call here will crash with CommandError, if it does not work
+        ssh(f'mkdir -p {path}', check=True)
+        ssh(f'touch {path}/datalad-tests-probe', check=True)
+
+        if localpath:
+            # we should see the probe file locally
+            assert (Path(localpath) / 'datalad-tests-probe').exists()
+
+        # cleanup
+        ssh(f'rm {path}/datalad-tests-probe', check=True)
+
     if localpath:
         assert not (Path(localpath) / 'datalad-tests-probe').exists()
```

### Comparing `datalad_next-1.3.0/datalad_next/types/annexkey.py` & `datalad_next-1.4.0/datalad_next/types/annexkey.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/types/archivist.py` & `datalad_next-1.4.0/datalad_next/types/archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/types/tests/test_annexkey.py` & `datalad_next-1.4.0/datalad_next/types/tests/test_annexkey.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/types/tests/test_archivist.py` & `datalad_next-1.4.0/datalad_next/types/tests/test_archivist.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/__init__.py` & `datalad_next-1.4.0/datalad_next/url_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/any.py` & `datalad_next-1.4.0/datalad_next/url_operations/any.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/base.py` & `datalad_next-1.4.0/datalad_next/url_operations/base.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/exceptions.py` & `datalad_next-1.4.0/datalad_next/url_operations/exceptions.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/file.py` & `datalad_next-1.4.0/datalad_next/url_operations/file.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/http.py` & `datalad_next-1.4.0/datalad_next/url_operations/http.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/ssh.py` & `datalad_next-1.4.0/datalad_next/url_operations/ssh.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/tests/test_any.py` & `datalad_next-1.4.0/datalad_next/url_operations/tests/test_any.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/tests/test_file.py` & `datalad_next-1.4.0/datalad_next/url_operations/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/tests/test_http.py` & `datalad_next-1.4.0/datalad_next/url_operations/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/url_operations/tests/test_ssh.py` & `datalad_next-1.4.0/datalad_next/url_operations/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/__init__.py` & `datalad_next-1.4.0/datalad_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/deprecate.py` & `datalad_next-1.4.0/datalad_next/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/http_helpers.py` & `datalad_next-1.4.0/datalad_next/utils/http_helpers.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/multihash.py` & `datalad_next-1.4.0/datalad_next/utils/multihash.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/patch.py` & `datalad_next-1.4.0/datalad_next/utils/patch.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/requests_auth.py` & `datalad_next-1.4.0/datalad_next/utils/requests_auth.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/specialremote.py` & `datalad_next-1.4.0/datalad_next/utils/specialremote.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/tests/test_deprecated.py` & `datalad_next-1.4.0/datalad_next/utils/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/tests/test_multihash.py` & `datalad_next-1.4.0/datalad_next/utils/tests/test_multihash.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next/utils/tests/test_parse_www_authenticate.py` & `datalad_next-1.4.0/datalad_next/utils/tests/test_parse_www_authenticate.py`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/datalad_next.egg-info/PKG-INFO` & `datalad_next-1.4.0/datalad_next.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-next
-Version: 1.3.0
+Version: 1.4.0
 Summary: What is next in DataLad
 Home-page: https://github.com/datalad/datalad-next
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
@@ -29,15 +29,14 @@
 Requires-Dist: requests_toolbelt; extra == "httpsupport"
 
 # DataLad NEXT extension
 
 [![All Contributors](https://img.shields.io/github/all-contributors/datalad/datalad-next?color=ee8449&style=flat-square)](#contributors)
 [![Build status](https://ci.appveyor.com/api/projects/status/dxomp8wysjb7x2os/branch/main?svg=true)](https://ci.appveyor.com/project/mih/datalad-next/branch/main)
 [![codecov](https://codecov.io/gh/datalad/datalad-next/branch/main/graph/badge.svg?token=2P8rak7lSX)](https://codecov.io/gh/datalad/datalad-next)
-[![crippled-filesystems](https://github.com/datalad/datalad-next/workflows/crippled-filesystems/badge.svg)](https://github.com/datalad/datalad-next/actions?query=workflow%3Acrippled-filesystems)
 [![docs](https://github.com/datalad/datalad-next/workflows/docs/badge.svg)](https://github.com/datalad/datalad-next/actions?query=workflow%3Adocs)
 [![Documentation Status](https://readthedocs.org/projects/datalad-next/badge/?version=latest)](http://docs.datalad.org/projects/next/en/latest/?badge=latest)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![GitHub release](https://img.shields.io/github/release/datalad/datalad-next.svg)](https://GitHub.com/datalad/datalad-next/releases/)
 [![PyPI version fury.io](https://badge.fury.io/py/datalad-next.svg)](https://pypi.python.org/pypi/datalad-next/)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6833099.svg)](https://doi.org/10.5281/zenodo.6833099)
```

### Comparing `datalad_next-1.3.0/datalad_next.egg-info/SOURCES.txt` & `datalad_next-1.4.0/datalad_next.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .all-contributorsrc
 .appveyor.yml
 .codeclimate.yml
+.codespell-exclude
 .codespellrc
 .coveragerc
 .gitattributes
 .gitignore
 .noannex
 .zenodo.json
 CHANGELOG.md
@@ -152,52 +153,76 @@
 datalad_next/itertools/tests/__init__.py
 datalad_next/itertools/tests/test_align_pattern.py
 datalad_next/itertools/tests/test_decode_bytes.py
 datalad_next/itertools/tests/test_itemize.py
 datalad_next/itertools/tests/test_load_json.py
 datalad_next/itertools/tests/test_reroute.py
 datalad_next/patches/__init__.py
+datalad_next/patches/add_method_url2transport_path.py
 datalad_next/patches/annexrepo.py
 datalad_next/patches/cli_configoverrides.py
 datalad_next/patches/commanderror.py
 datalad_next/patches/common_cfg.py
 datalad_next/patches/configuration.py
 datalad_next/patches/create_sibling_ghlike.py
 datalad_next/patches/create_sibling_gitlab.py
 datalad_next/patches/customremotes_main.py
 datalad_next/patches/distribution_dataset.py
 datalad_next/patches/enabled.py
+datalad_next/patches/fix_ria_ora_tests.py
 datalad_next/patches/interface_utils.py
+datalad_next/patches/patch_ria_ora.py
 datalad_next/patches/push_optimize.py
 datalad_next/patches/push_to_export_remote.py
+datalad_next/patches/replace_create_sibling_ria.py
+datalad_next/patches/replace_ora_remote.py
+datalad_next/patches/replace_sshremoteio.py
+datalad_next/patches/ria_utils.py
 datalad_next/patches/run.py
 datalad_next/patches/siblings.py
+datalad_next/patches/ssh_exec.py
+datalad_next/patches/sshconnector.py
 datalad_next/patches/test_keyring.py
 datalad_next/patches/update.py
 datalad_next/patches/tests/__init__.py
+datalad_next/patches/tests/test_add_method_url2transport_path.py
 datalad_next/patches/tests/test_annex_progress_logging.py
 datalad_next/patches/tests/test_cli_configoverrides.py
 datalad_next/patches/tests/test_commanderror.py
 datalad_next/patches/tests/test_configuration.py
 datalad_next/patches/tests/test_create_sibling_ghlike.py
 datalad_next/patches/tests/test_create_sibling_gitlab.py
 datalad_next/patches/tests/test_push.py
 datalad_next/patches/tests/test_push_to_export_remote.py
+datalad_next/patches/tests/test_replace_ora_remote.py
+datalad_next/patches/tests/test_ria.py
 datalad_next/patches/tests/test_run.py
+datalad_next/patches/tests/test_sshremoteio.py
 datalad_next/repo_utils/__init__.py
+datalad_next/repo_utils/annex.py
 datalad_next/repo_utils/worktree.py
 datalad_next/repo_utils/tests/__init__.py
+datalad_next/repo_utils/tests/test_annex.py
 datalad_next/repo_utils/tests/test_head.py
 datalad_next/runners/__init__.py
 datalad_next/runners/git.py
 datalad_next/runners/iter_subproc.py
 datalad_next/runners/protocols.py
 datalad_next/runners/tests/__init__.py
 datalad_next/runners/tests/test_git.py
 datalad_next/runners/tests/test_iter_subproc.py
+datalad_next/shell/__init__.py
+datalad_next/shell/response_generators.py
+datalad_next/shell/shell.py
+datalad_next/shell/operations/__init__.py
+datalad_next/shell/operations/common.py
+datalad_next/shell/operations/posix.py
+datalad_next/shell/tests/__init__.py
+datalad_next/shell/tests/test_response_generators.py
+datalad_next/shell/tests/test_shell.py
 datalad_next/tests/__init__.py
 datalad_next/tests/fixtures.py
 datalad_next/tests/marker.py
 datalad_next/tests/test_common_cfg.py
 datalad_next/tests/test_register.py
 datalad_next/tests/test_testutils.py
 datalad_next/tests/utils.py
```

### Comparing `datalad_next-1.3.0/docs/CODEOWNERS` & `datalad_next-1.4.0/docs/CODEOWNERS`

 * *Files 19% similar despite different names*

```diff
@@ -7,8 +7,11 @@
 #
 # RT member approval is required for any merge request.
 #
 # Merge requests are accepted (automatically) when all (relevant)
 # status checks have passed, and RT approval was given.
 *   michael.hanke@gmail.com
 /iter_collections/ christian.moench@web.de
+/iterable_subprocess/ christian.moench@web.de
+/patches/ christian.moench@web.de
 /runners/ christian.moench@web.de
+/shell/ christian.moench@web.de
```

### Comparing `datalad_next-1.3.0/docs/Makefile` & `datalad_next-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/docs/README.md` & `datalad_next-1.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/docs/policy/release-management.md` & `datalad_next-1.4.0/docs/policy/release-management.md`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/docs/source/_static/datalad_logo.png` & `datalad_next-1.4.0/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/docs/source/conf.py` & `datalad_next-1.4.0/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
+from __future__ import annotations
 
 import sys
 import subprocess
 
 import datetime
 from os.path import (
     abspath,
@@ -103,15 +104,15 @@
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'en'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = []
+exclude_patterns: list[str] = []
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = 'sphinx'
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
@@ -136,7 +137,10 @@
 # If true, links to the reST sources are added to the pages.
 html_show_sourcelink = False
 
 # smart quotes are incompatible with the RST flavor of the generated manpages
 # but see `smartquotes_action` for more fine-grained control, in case
 # some of this functionality is needed
 smartquotes = False
+
+# render docstrings for dunder-methods, e.g. `__call__`.
+napoleon_include_special_with_doc = True
```

### Comparing `datalad_next-1.3.0/docs/source/developer_guide/constraints.rst` & `datalad_next-1.4.0/docs/source/developer_guide/constraints.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/docs/source/index.rst` & `datalad_next-1.4.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/docs/source/pyutils.rst` & `datalad_next-1.4.0/docs/source/pyutils.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,13 +24,14 @@
    datasets
    exceptions
    iterable_subprocess
    itertools
    iter_collections
    repo_utils
    runners
+   shell
    tests
    tests.fixtures
    types
    uis
    url_operations
    utils
```

### Comparing `datalad_next-1.3.0/readthedocs.yml` & `datalad_next-1.4.0/readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/setup.cfg` & `datalad_next-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/tools/appveyor/setup-sshd` & `datalad_next-1.4.0/tools/appveyor/setup-sshd`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/tools/appveyor/setup-sshd.bat` & `datalad_next-1.4.0/tools/appveyor/setup-sshd.bat`

 * *Files identical despite different names*

### Comparing `datalad_next-1.3.0/versioneer.py` & `datalad_next-1.4.0/versioneer.py`

 * *Files identical despite different names*

