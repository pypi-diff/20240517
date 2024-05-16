# Comparing `tmp/cobramod-1.2.0.tar.gz` & `tmp/cobramod-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobramod-1.2.0.tar", last modified: Tue Feb 20 12:41:47 2024, max compression
+gzip compressed data, was "cobramod-1.3.0.tar", last modified: Thu May 16 22:31:46 2024, max compression
```

## Comparing `cobramod-1.2.0.tar` & `cobramod-1.3.0.tar`

### file list

```diff
@@ -1,61 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.907179 cobramod-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35095 2024-02-20 12:41:27.000000 cobramod-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    46364 2024-02-20 12:41:47.907179 cobramod-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-02-20 12:41:27.000000 cobramod-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-02-20 12:41:27.000000 cobramod-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 12:41:47.907179 cobramod-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.895180 cobramod-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.899180 cobramod-1.2.0/src/cobramod/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.899180 cobramod-1.2.0/src/cobramod/core/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33822 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/crossreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    30695 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/genes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11957 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/pathway.py
--rw-r--r--   0 runner    (1001) docker     (127)    13768 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/core/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.903180 cobramod-1.2.0/src/cobramod/data/
--rw-r--r--   0 runner    (1001) docker     (127)   379955 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/data/textbook_biocyc.sbml
--rw-r--r--   0 runner    (1001) docker     (127)   379144 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/data/textbook_kegg.sbml
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.903180 cobramod-1.2.0/src/cobramod/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/parsing/bigg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12110 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/parsing/biocyc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/parsing/db_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11683 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/parsing/kegg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/parsing/plantcyc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/parsing/solcyc.py
--rw-r--r--   0 runner    (1001) docker     (127)    26177 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11019 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.903180 cobramod-1.2.0/src/cobramod/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40417 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/visualization/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/visualization/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/visualization/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/visualization/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-20 12:41:27.000000 cobramod-1.2.0/src/cobramod/visualization/pair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.907179 cobramod-1.2.0/src/cobramod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    46364 2024-02-20 12:41:47.000000 cobramod-1.2.0/src/cobramod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-02-20 12:41:47.000000 cobramod-1.2.0/src/cobramod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 12:41:47.000000 cobramod-1.2.0/src/cobramod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-20 12:41:47.000000 cobramod-1.2.0/src/cobramod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-20 12:41:47.000000 cobramod-1.2.0/src/cobramod.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 12:41:47.907179 cobramod-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    34297 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_crossreferences.py
--rw-r--r--   0 runner    (1001) docker     (127)    22640 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_genes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11760 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    16105 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_pathway.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    41961 2024-02-20 12:41:27.000000 cobramod-1.2.0/tests/test_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.912980 cobramod-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35095 2024-05-16 22:31:09.000000 cobramod-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    47224 2024-05-16 22:31:46.912980 cobramod-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-05-16 22:31:09.000000 cobramod-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-16 22:31:10.000000 cobramod-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:31:46.912980 cobramod-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.892980 cobramod-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.896980 cobramod-1.3.0/src/cobramod/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.900980 cobramod-1.3.0/src/cobramod/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33873 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/crossreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/pathway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13769 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/core/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.900980 cobramod-1.3.0/src/cobramod/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   379955 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/data/textbook_biocyc.sbml
+-rw-r--r--   0 runner    (1001) docker     (127)   378623 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/data/textbook_biocyc_groups.sbml
+-rw-r--r--   0 runner    (1001) docker     (127)   379144 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/data/textbook_kegg.sbml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.904980 cobramod-1.3.0/src/cobramod/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/parsing/bigg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/parsing/biocyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/parsing/db_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/parsing/kegg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/parsing/plantcyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/parsing/solcyc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26631 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.904980 cobramod-1.3.0/src/cobramod/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    40937 2024-05-16 22:31:44.000000 cobramod-1.3.0/src/cobramod/static/LICENSES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   837758 2024-05-16 22:31:44.000000 cobramod-1.3.0/src/cobramod/static/escher.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)   880153 2024-05-16 22:31:44.000000 cobramod-1.3.0/src/cobramod/static/force_graph.mjs
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.908980 cobramod-1.3.0/src/cobramod/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41099 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/escher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/force_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-16 22:31:10.000000 cobramod-1.3.0/src/cobramod/visualization/pair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.908980 cobramod-1.3.0/src/cobramod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47224 2024-05-16 22:31:46.000000 cobramod-1.3.0/src/cobramod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-05-16 22:31:46.000000 cobramod-1.3.0/src/cobramod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:31:46.000000 cobramod-1.3.0/src/cobramod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 22:31:46.000000 cobramod-1.3.0/src/cobramod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 22:31:46.000000 cobramod-1.3.0/src/cobramod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:31:46.908980 cobramod-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    34323 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_crossreferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22760 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_genes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10766 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19737 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16192 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_pathway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34141 2024-05-16 22:31:10.000000 cobramod-1.3.0/tests/test_visualization.py
```

### Comparing `cobramod-1.2.0/LICENSE` & `cobramod-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cobramod-1.2.0/PKG-INFO` & `cobramod-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobramod
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for pathway-centric modification and extension of genome-scale metabolic networks
 Author-email: Stefano Camborda La Cruz <scambord@uni-koeln.de>, Jan-Niklas Weder <jweder@uni-koeln.de>, Nadine Töpfer <ntoepfer@uni-koeln.de>
 Maintainer-email: Nadine Töpfer <ntoepfer@uni-koeln.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -692,46 +692,53 @@
 Requires-Dist: colorlog
 Requires-Dist: cobra>=0.29.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: webcolors>=1.13
 Requires-Dist: pyarrow>=14.0.2
+Requires-Dist: anywidget>=0.9.9
 Provides-Extra: escher
 Requires-Dist: escher-legacy>=1.7.4; extra == "escher"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: jupyter-contrib-nbextensions; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinxcontrib-napoleon; extra == "dev"
 Requires-Dist: sphinxcontrib-bibtex; extra == "dev"
 
+<div align="center">
+
 ![Static Badge](https://img.shields.io/badge/python-3.10%7C3.11%7C3.12-%20blue)
 ![GitHub](https://img.shields.io/github/license/Toepfer-Lab/cobramod)
-![Read the Docs (version)](https://img.shields.io/readthedocs/cobramod/latest)
-![Tests](https://img.shields.io/github/workflow/status/Toepfer-Lab/cobramod/Test%20build%20and%20publish%20Cobramod%20to%20PyPI?label=tests)
-![Version](https://img.shields.io/pypi/v/cobramod?label=version)
-[![Downloads](https://pepy.tech/badge/cobramod)](https://pepy.tech/project/cobramod)
+[![Downloads](https://img.shields.io/pepy/dt/cobramod
+)](https://pepy.tech/project/cobramod)
 
+![Version](https://img.shields.io/pypi/v/cobramod?label=version)
+![Read the Docs (version)](https://img.shields.io/readthedocs/cobramod/latest)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Toepfer-lab/cobramod/test-build-and-publish.yml)
+![Coverage Status](./docs/source/img/coverage.svg)
 
 CobraMod: A pathway-centric curation tool for constraint-based metabolic models
 ===============================================================================
 
+
 ![image](https://raw.githubusercontent.com/Toepfer-Lab/cobramod/master/docs/source/img/logo.png)
+</div>
 
 CobraMod is a Python 3 open-source package for pathway-centric curation of
-genome-scale metabolic models (GEMs). It builds upon the [COBRApy toolbox]
-(https://opencobra.github.io/cobrapy/) and offers a comprehensible set of
-functions for semi-automated network extension, curation and visualization.
-CobraMod supports all databases from the [BioCyc collection](https://
-biocyc.org/), the [KEGG database](https://www.genome.jp/kegg/), and the [BiGG
+genome-scale metabolic models (GEMs). It builds upon the 
+[COBRApy toolbox](https://opencobra.github.io/cobrapy/) and offers a 
+comprehensible set of functions for semi-automated network extension, curation and visualization.
+CobraMod supports all databases from the [BioCyc collection](https://biocyc.org/), 
+the [KEGG database](https://www.genome.jp/kegg/), and the [BiGG
 Models repository](http://bigg.ucsd.edu/). It optionally can interact with
 Escher for pathway and flux visualization.
 
 This package converts pathway information into native COBRApy objects and
 quality-checks them while adding them to the model. This includes testing for:
 
 -   duplicate elements
@@ -801,14 +808,33 @@
 CobraMod is licensed under the GPL-3 License. Read the
 [LICENSE](https://github.com/Toepfer-Lab/cobramod/blob/master/LICENSE)
 for more information.
 
 
 Development
 -----------
+CobraMod consists of a Python and JavaScript/TypeScript part. 
+The following briefly describes all the commands to build a local 
+version from the source files.
+
+### JavaScript
+
+Since we need Node modules to build the Jupyter integrations con CobraMod, 
+a package.json is included in the project. All dependencies contained 
+in it can be made available locally using [yarn](https://yarnpkg.com/). The foiling command can be used for this:
+
+    yarn install
+
+We use [Vite](https://vitejs.dev/) to build the Javascript part of the Jupyter integrations. So, we can use the following command to build a bundled version of the integrations.
+
+    yarn run vite build
+
+This creates bundled JavaScript files under '/src/cobramod/static'.
+
+### Python
 
 You can contribute to CobraMod by cloning the repository and installing it in
 developer mode and using the `dev` dependency group via pip:
 
     pip install -e ".[dev]"
 
 Optionally, a conda environment file is supplied (*environment.yml*). This
```

### Comparing `cobramod-1.2.0/README.md` & `cobramod-1.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+<div align="center">
+
 ![Static Badge](https://img.shields.io/badge/python-3.10%7C3.11%7C3.12-%20blue)
 ![GitHub](https://img.shields.io/github/license/Toepfer-Lab/cobramod)
-![Read the Docs (version)](https://img.shields.io/readthedocs/cobramod/latest)
-![Tests](https://img.shields.io/github/workflow/status/Toepfer-Lab/cobramod/Test%20build%20and%20publish%20Cobramod%20to%20PyPI?label=tests)
-![Version](https://img.shields.io/pypi/v/cobramod?label=version)
-[![Downloads](https://pepy.tech/badge/cobramod)](https://pepy.tech/project/cobramod)
+[![Downloads](https://img.shields.io/pepy/dt/cobramod
+)](https://pepy.tech/project/cobramod)
 
+![Version](https://img.shields.io/pypi/v/cobramod?label=version)
+![Read the Docs (version)](https://img.shields.io/readthedocs/cobramod/latest)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Toepfer-lab/cobramod/test-build-and-publish.yml)
+![Coverage Status](./docs/source/img/coverage.svg)
 
 CobraMod: A pathway-centric curation tool for constraint-based metabolic models
 ===============================================================================
 
+
 ![image](https://raw.githubusercontent.com/Toepfer-Lab/cobramod/master/docs/source/img/logo.png)
+</div>
 
 CobraMod is a Python 3 open-source package for pathway-centric curation of
-genome-scale metabolic models (GEMs). It builds upon the [COBRApy toolbox]
-(https://opencobra.github.io/cobrapy/) and offers a comprehensible set of
-functions for semi-automated network extension, curation and visualization.
-CobraMod supports all databases from the [BioCyc collection](https://
-biocyc.org/), the [KEGG database](https://www.genome.jp/kegg/), and the [BiGG
+genome-scale metabolic models (GEMs). It builds upon the 
+[COBRApy toolbox](https://opencobra.github.io/cobrapy/) and offers a 
+comprehensible set of functions for semi-automated network extension, curation and visualization.
+CobraMod supports all databases from the [BioCyc collection](https://biocyc.org/), 
+the [KEGG database](https://www.genome.jp/kegg/), and the [BiGG
 Models repository](http://bigg.ucsd.edu/). It optionally can interact with
 Escher for pathway and flux visualization.
 
 This package converts pathway information into native COBRApy objects and
 quality-checks them while adding them to the model. This includes testing for:
 
 -   duplicate elements
@@ -90,14 +96,33 @@
 CobraMod is licensed under the GPL-3 License. Read the
 [LICENSE](https://github.com/Toepfer-Lab/cobramod/blob/master/LICENSE)
 for more information.
 
 
 Development
 -----------
+CobraMod consists of a Python and JavaScript/TypeScript part. 
+The following briefly describes all the commands to build a local 
+version from the source files.
+
+### JavaScript
+
+Since we need Node modules to build the Jupyter integrations con CobraMod, 
+a package.json is included in the project. All dependencies contained 
+in it can be made available locally using [yarn](https://yarnpkg.com/). The foiling command can be used for this:
+
+    yarn install
+
+We use [Vite](https://vitejs.dev/) to build the Javascript part of the Jupyter integrations. So, we can use the following command to build a bundled version of the integrations.
+
+    yarn run vite build
+
+This creates bundled JavaScript files under '/src/cobramod/static'.
+
+### Python
 
 You can contribute to CobraMod by cloning the repository and installing it in
 developer mode and using the `dev` dependency group via pip:
 
     pip install -e ".[dev]"
 
 Optionally, a conda environment file is supplied (*environment.yml*). This
```

### Comparing `cobramod-1.2.0/pyproject.toml` & `cobramod-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -21,38 +21,44 @@
 dependencies = [
     "colorlog",
     "cobra>=0.29.0",
     "requests>=2.31.0",
     "tqdm>=4.62.3",
     "openpyxl>=3.1.2",
     "webcolors>=1.13",
-    "pyarrow>=14.0.2"
+    "pyarrow>=14.0.2",
+    "anywidget>=0.9.9"
 ]
 
 [project.optional-dependencies]
 escher = ["escher-legacy>=1.7.4"]
 dev = [
-	"ruff",
-	"tox",
-  "sphinx",
-  "nbsphinx",
-  "sphinx-autoapi",
-  "jupyter-contrib-nbextensions",
-  "sphinx-rtd-theme",
-  "sphinxcontrib-napoleon",
-  "sphinxcontrib-bibtex"
+    "ruff",
+    "tox",
+    "sphinx",
+    "nbsphinx",
+    "sphinx-autoapi",
+    "jupyter-contrib-nbextensions",
+    "sphinx-rtd-theme",
+    "sphinxcontrib-napoleon",
+    "sphinxcontrib-bibtex",
 ]
 
 [project.urls]
 homepage = "https://github.com/Toepfer-Lab/cobramod"
 Documentation = "https://cobramod.readthedocs.io/"
 bugtracker = "https://github.com/Toepfer-Lab/cobramod/issues"
 
+[build-system]
+requires = ["setuptools >= 61.0"]
+build-backend = "setuptools.build_meta"
+
 [tool.setuptools.package-data]
 "cobramod.data" = ["*.sbml"]
+"cobramod.static" = ["*"]
 
 [tool.setuptools.dynamic]
 version = {attr = "cobramod.__version__"}
 readme = {file = "README.md", content-type = "text/markdown"}
 
 [tool.ruff]
 line-length = 80
```

### Comparing `cobramod-1.2.0/src/cobramod/__init__.py` & `cobramod-1.3.0/src/cobramod/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 By default, CobraMod creates the file "debug.log", which displays the changes,
 which occurred when running a script. In order to modify the logging, import
 "debug_log" from "cobramod.debug". The default logging level is defined as
 INFO. Read the documentation of logging for more information.
 
 For a list of databases, load variable :obj:`cobramod.available_databases`
 """
+
 from cobramod.core.creation import (
     add_metabolites,
     add_reactions,
     create_object,
 )
 from cobramod.core.crossreferences import add_crossreferences
 from cobramod.core.extension import test_non_zero_flux, add_pathway
@@ -49,8 +50,8 @@
     "add_pathway",
     "test_non_zero_flux",
     "Pathway",
     "model_convert",
     "add_crossreferences",
 ]
 
-__version__ = "1.2.0"
+__version__ = "1.3.0"
```

### Comparing `cobramod-1.2.0/src/cobramod/core/__init__.py` & `cobramod-1.3.0/src/cobramod/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cobramod-1.2.0/src/cobramod/core/creation.py` & `cobramod-1.3.0/src/cobramod/core/creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Object creation
 
 This module handles the creation of COBRApy's objects
 :class:`cobra.core.metabolite.Metabolite` and
 :class:`cobra.core.reaction.Reaction`. Dictionaries containing the data of a
 given database are used.
 """
+
 from __future__ import annotations
 
 from contextlib import suppress
 from pathlib import Path
 from typing import Optional, Union
 
 import cobra.core as cobra_core
@@ -612,15 +613,15 @@
             )
     return new_reactions
 
 
 def create_object(
     identifier: str,
     directory: Union[Path, str],
-    database: str,
+    database: Optional[str],
     compartment: str,
     replacement: dict[str, str] = {},
     show_imbalance: bool = True,
     stop_imbalance: bool = False,
     model: cobra_core.Model = cobra_core.Model(),
     model_id: Optional[str] = None,
     genome: Optional[str] = None,
@@ -630,15 +631,15 @@
     database. Identifier names will be formatted.
 
     .. hint:: Hyphens will become underscores.
 
     Args:
         identifier (str): Original identifier of the database.
         directory (Path): Path to directory where data is stored.
-        database (str): Name of database. Check
+        database (Optional[str]): Name of database. Check
             :obj:`cobramod.retrieval.available_databases` for a list of names.
         compartment (str): Location of the object. In case of reaction, all
             metabolites will be included in the same location.
         replacement (dict[str, str]): Dictionary with either the new identifier
             and/or the identifier of an object inside the model.
 
     Arguments for reactions:
@@ -766,21 +767,22 @@
     # Kwargs
     replacement: dict[str, str] = kwargs.pop("replacement", {})
     model_id: str = kwargs.pop("model_id", {})
 
     if isinstance(obj, str):
         obj = Path(obj).absolute()
 
+    metabolites: list[cobra_core.Metabolite]
     if isinstance(obj, Path):
         metabolites = get_file_metabolites(
             model, obj, replacement, directory, database, model_id
         )
 
     elif isinstance(obj, list):
-        metabolites: list[cobra_core.Metabolite] = []
+        metabolites = []
 
         for item in obj:
             if isinstance(item, cobra_core.Metabolite):
                 metabolites.append(item)
 
             elif isinstance(item, str):
                 metabolites.append(
@@ -934,29 +936,30 @@
     if isinstance(directory, str):
         directory = Path(directory).absolute()
 
     if isinstance(obj, str):
         obj = Path(obj).absolute()
 
     # In case of a Path
+    reactions: list[cobra_core.Reaction]
     if isinstance(obj, Path):
         reactions = get_file_reactions(
             model=model,
             filename=obj,
             directory=directory,
             database=database,
             replacement=replacement,
             stop_imbalance=stop_imbalance,
             show_imbalance=show_imbalance,
             genome=genome,
             model_id=model_id,
         )
 
     elif isinstance(obj, list):
-        reactions: list[cobra_core.Reaction] = []
+        reactions = []
 
         for item in obj:
             if isinstance(item, str):
                 reactions.append(
                     string_to_reaction(
                         line=item,
                         model=model,
```

### Comparing `cobramod-1.2.0/src/cobramod/core/crossreferences.py` & `cobramod-1.3.0/src/cobramod/core/crossreferences.py`

 * *Files identical despite different names*

### Comparing `cobramod-1.2.0/src/cobramod/core/extension.py` & `cobramod-1.3.0/src/cobramod/core/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 a model and the corresponding test that comes with it.
 
 Most important functions:
 - add_pathway: Adds a pathway or multiple reactions into a model.
 - test_non_zero_flux: Checks that the given reaction in a model is active and
     gives a non-zero flux.
 """
+
 from __future__ import annotations
 
 from contextlib import suppress
 from pathlib import Path
 from typing import Generator, Optional, Union
 
 import cobra.core as cobra_core
@@ -30,15 +31,15 @@
 cobra_tolerance: float = cobra_core.Configuration().tolerance
 
 
 def yield_reaction_from_list(
     sequence: list[str],
     compartment: str,
     directory: Path,
-    database: str,
+    database: Optional[str],
     show_imbalance: bool,
     stop_imbalance: bool,
     replacement: dict,
     model: cobra_core.Model,
     model_id: str,
     genome: Optional[str],
 ) -> Generator[cobra_core.Reaction, None, None]:
@@ -47,15 +48,15 @@
 
     .. hint:: Hyphens will become underscores. Double hyphens become single\
     underscores.
 
     Args:
         sequence (list): Identifiers for the reactions.
         directory (Path): Path to directory where data is located.
-        database (str): Name of the database. Check
+        database (Optional[str]): Name of the database. Check
             :obj:`cobramod.available_databases` for a list of names.
         compartment (str): Location of the reaction.
         replacement (dict): Original identifiers to be replaced.
             Values are the new identifiers. This applies to metabolites.
         stop_imbalance (bool): If unbalanced reaction is found, stop process.
         show_imbalance (bool): If unbalanced reaction is found, show output.
         model_id (str): Exclusive for BIGG. Retrieve object from specified
@@ -582,29 +583,29 @@
                 model_id=model_id,
                 genome=genome,
             )
         )
         previous: str = ""
         for i, reaction in enumerate(sequence):
             if i == len(sequence) - 1:
-                graph[reaction.id] = None
+                graph[reaction.id] = None  # type: ignore
 
             if previous:
                 value = graph.get(previous)
 
                 if not value:
-                    value = reaction.id
+                    value = reaction.id  # type: ignore
 
                 elif isinstance(value, tuple):
-                    a = list(value) + [reaction.id]
-                    value = tuple(a)
+                    a = list(value) + [reaction.id]  # type: ignore
+                    value = tuple(a)  # type: ignore
 
                 graph[previous] = value
 
-            previous = reaction.id
+            previous = reaction.id  # type: ignore
 
         # Add to model
         add_reactions_to_Pathway(
             model=model,
             pathway=pathway,
             sequence=sequence,
             ignore_list=ignore_list,
@@ -621,15 +622,15 @@
     pathway.notes["ORDER"] = pathway.graph
 
 
 def add_pathway_from_strings(
     model: cobra_core.Model,
     identifier: str,
     sequence: list[str],
-    database: str,
+    database: Optional[str],
     compartment: str,
     directory: Path,
     avoid_list: list[str],
     replacement: dict[str, str],
     ignore_list: list[str],
     stop_imbalance: bool,
     show_imbalance: bool,
@@ -640,15 +641,15 @@
     Adds a sequence of identifiers to given model. It will automatically test
     for valid optimized values.
 
     Args:
         model (Model): Model to expand.
         identifier (str): Common :class:`cobramod.pathway.Pathway` identifier.
         sequence (list): List reaction identifiers.
-        database (str): Name of the database.
+        database (Optional[str]): Name of the database.
             Check :obj:`cobramod.available_databases` for a list of names.
         compartment: Location of the reactions.
         directory (Path): Path for directory to store and retrieve data.
 
     Arguments for complex pathways:
         avoid_list (list, optional): A sequence of reactions identifiers to
             avoid adding to the model.
```

### Comparing `cobramod-1.2.0/src/cobramod/core/genes.py` & `cobramod-1.3.0/src/cobramod/core/genes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Modules genes
 
 This module is responsible for the creation of COBRApy Genes from the parsed
 data of the specific parsers.
 """
+
 from typing import Any
 
 import cobra.core as cobra_core
 
 from cobramod.debug import debug_log
```

### Comparing `cobramod-1.2.0/src/cobramod/core/graph.py` & `cobramod-1.3.0/src/cobramod/core/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 order of the reactions. I.e. the relationship between reactions. The main
 function of this module:
 
 build_graph: From given dictionary with Parent-reaction:children-reaction,
 return the corresponding non-cyclic directed graph.
 
 """
+
 from __future__ import annotations
 
 from collections import Counter
 from contextlib import suppress
 from itertools import chain
 from typing import Any, Dict, Union
 
@@ -310,15 +311,15 @@
         cut_parents(graph=graph)
         # Fix cycles if found
         cycles = return_cycles(graph=graph)
         # Check until no cycles are found.
         while cycles:
             # This is modify graph
             # TODO: check whether tuples are affected
-            cut_cycle(graph=graph, key=cycles[0][0])
+            cut_cycle(graph=graph, key=cycles[0][0])  # type: ignore
             cycles = return_cycles(graph=graph)
     # This would modify the graph. Use copy
     mapping = get_mapping(graph=graph.copy(), stop_list=[], new=[])
     mapping.sort(key=len, reverse=True)
     return mapping
```

### Comparing `cobramod-1.2.0/src/cobramod/core/pathway.py` & `cobramod-1.3.0/src/cobramod/core/pathway.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """COBRApy Group-child class extension
 
-The new class :class:`cobramod.pathway.Pathway" is child derived from
+The new class :class:`cobramod.pathway.Pathway` is child derived from
 :class:`cobra.core.group.Group`. It extends some functionalities such as:
 
 - solution: Obtain the solution for the specific members.
 - visualize: get a :class:`escher.Builder` for that specific Pathway.
 """
+
 from __future__ import annotations
 
 import warnings
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, Literal
 
 import cobra.core as cobra_core
 
+from cobramod.visualization.escher import EscherIntegration
+from cobramod.visualization.force_graph import ForceGraphIntegration
+
 try:
     import escher
 
     _has_escher = True
 except ImportError:
     _has_escher = False
 
@@ -95,15 +99,15 @@
         super().__init__(
             id=id,
             name=name,
             kind=kind,
         )
 
         # Loop has to be after __init__, otherwise, behavior of class changes.
-        self.graph = dict()
+        self.graph = dict()  # type: ignore
         self.notes: dict[str, Any] = {"ORDER": dict()}
 
         if members:
             for member in members:
                 # Remove no Reactions
                 if not isinstance(member, cobra_core.Reaction):
                     debug_log.debug(
@@ -268,26 +272,54 @@
 
     def visualize(
         self,
         solution_fluxes: Optional[
             Union[cobra_core.Solution, dict[str, float]]
         ] = None,
         filename: Optional[Union[str, Path]] = None,
-    ) -> Optional[escher.Builder]:
+        vis: Literal["escher", "escher-custom", "3d-force"] = "escher",
+        never_ask_before_quit: bool = False,
+    ) -> Union[escher.Builder, EscherIntegration, ForceGraphIntegration, None]:
         """
+        .. versionchanged:: 1.3.0
+            The 'vis' parameter has been added. This allows one to choose between different visualization tools.
+
         Returns a :class:`escher.Builder`, which can be used to create visual
         representations of the pathway.
 
-        Args:
-            solution_fluxes (Solution, dict): Series or Dictionary with fluxes.
-                The values will be then showed in the Builder.
-                Defaults to None.
-            filename (str, Path): Path for the HTML. Defaults to
-                "pathway.html" in the current working directory.
+        :param solution_fluxes: Series or Dictionary with fluxes. The values will be then showed in the Builder. Defaults to None.
+
+        :param filename: Path for the HTML. Defaults to "pathway.html" in the current working directory.
+
+        :param vis:
+            .. versionadded:: 1.3.0
+            Parameter that determines the visualization tool used. It is possible to choose between the original
+            Escher integration [escher], the one embedded in CobraMod [escher-custom] and a 3-dimensional
+            force directed graph visualization [3d-force].
+
+            .. deprecated:: 1.3.0
+                The original python integration of Escher will be removed in a future version due to dependency
+                conflicts with Jupyter. The integration embedded in CobraMod will take its place in the future.
+                This can already be used by setting 'vis' to "escher-custom".
+
+        :param never_ask_before_quit:
+            .. versionadded:: 1.3.0
+
+            Option to control whether a warning dialog is displayed when the Escher Builder window is closed.
+            Only has an effect when using Escher for visualization.
+
         """
+
+        if vis == "3d-force":
+            widget = ForceGraphIntegration()
+            widget.model = self
+            widget.solution = solution_fluxes
+
+            return widget
+
         json_dict = JsonDictionary()
         if filename is None:
             filename = "pathway.html"
 
         # Define solution. If None, nothing will be added. Either dict or
         # regular solution
         if solution_fluxes is not None:
@@ -296,33 +328,57 @@
             json_dict.flux_solution = solution_fluxes
 
         # Get graph and add to json_dict
         json_dict.graph = self.graph.copy()
         reactions: dict[str, str] = {m.id: m.reaction for m in self.members}
         json_dict.reaction_strings = reactions
 
+        if vis == "escher-custom":
+            builder = json_dict.visualize(
+                filepath=filename,
+                vertical=self.vertical,
+                color=[self.color_positive, self.color_negative],
+                min_max=self.color_min_max,
+                quantile=self.color_quantile,
+                max_steps=self.color_max_steps,
+                n_steps=self.color_n_steps,
+                custom_integration=True,
+                never_ask_before_quit=never_ask_before_quit,
+            )
+            return builder
+
         if _has_escher:
             builder = json_dict.visualize(
                 filepath=filename,
                 vertical=self.vertical,
                 color=[self.color_positive, self.color_negative],
                 min_max=self.color_min_max,
                 quantile=self.color_quantile,
                 max_steps=self.color_max_steps,
                 n_steps=self.color_n_steps,
             )
             debug_log.info(f'Visualization saved in "{filename}"')
+            warnings.warn(
+                "The use of Escher's own Python integration will be removed in a future CobraMod version to "
+                "avoid installation problems due to dependency incompatibilities. Instead, you can use "
+                "CobraMod's built-in Escher integration. To use it, simply pass 'escher-custom' as an "
+                "argument to 'vis'.",
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+
             return builder
         else:
             warnings.warn(
                 "Package Escher was not found. No visualization in available. "
                 "You can install this extra-dependency running "
-                "'pip install cobramod[escher]'"
+                "'pip install cobramod[escher]'. Alternatively, you can use CobraMod's own integration of Escher. "
+                "To use it, just specify 'escher-custom' for the 'vis' argument."
             )
-            return
+            return None
 
     def _repr_html_(self):
         """
         Returns a HTML string with the attributes of the Pathway
         """
         return f"""
 <table> <tbody> <tr> <td><strong>Pathway identifier</strong></td>
```

### Comparing `cobramod-1.2.0/src/cobramod/core/summary.py` & `cobramod-1.3.0/src/cobramod/core/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Summary
 
 This module is responsible for the short summary in the command
 line and for other summaries in different formats.
 """
+
 from __future__ import annotations
 from pathlib import Path
 from typing import Union, Optional
 
 import pandas
 from cobra import Model
```

### Comparing `cobramod-1.2.0/src/cobramod/data/textbook_biocyc.sbml` & `cobramod-1.3.0/src/cobramod/data/textbook_biocyc.sbml`

 * *Files identical despite different names*

### Comparing `cobramod-1.2.0/src/cobramod/data/textbook_kegg.sbml` & `cobramod-1.3.0/src/cobramod/data/textbook_kegg.sbml`

 * *Files identical despite different names*

### Comparing `cobramod-1.2.0/src/cobramod/debug.py` & `cobramod-1.3.0/src/cobramod/debug.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 The logs are saved in the directory 'logs' created in the working directory.
 Cobramod saves the logs by date, i.e, running the commands in different days
 will results in different files. The default level is set to INFO.
 
 The name of logger variable is `debug_log`
 """
+
 import datetime as dt
 import logging
 from pathlib import Path
 
 import colorlog
 
 debug_log = logging.getLogger("debug_log")
@@ -31,24 +32,24 @@
 # In direct stream
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(formatter)
 debug_log.addHandler(stream_handler)
 
 # File logs
 format_str = "[%(asctime)s] %(levelname)s %(message)s"
-formatter = logging.Formatter(format_str, TIME_STR)
+formatter_file = logging.Formatter(format_str, TIME_STR)
 
 log_dir = Path("logs").absolute()
 log_dir.mkdir(exist_ok=True)
 log_path = log_dir.joinpath(
     f"cobramod_{dt.date.today().strftime('%Y%m%d')}.log"
 )
 
 debug_handler = logging.FileHandler(log_path, mode="a+")
-debug_handler.setFormatter(formatter)
+debug_handler.setFormatter(formatter_file)
 
 debug_log.addHandler(debug_handler)
 
 
 def change_to_debug() -> None:
     """
     Changes the logging level to DEBUG and changes the formatting of it.
```

### Comparing `cobramod-1.2.0/src/cobramod/error.py` & `cobramod-1.3.0/src/cobramod/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Errors for CobraMod
 
 This module creates special errors for CobraMod. Read each error for their
 explanation.
 """
+
 from cobramod.debug import debug_log
 
 
 class UserInterruption(Exception):
     """
     Exception that is used if the input of a user interrupts the program flow.
     """
```

### Comparing `cobramod-1.2.0/src/cobramod/parsing/bigg.py` & `cobramod-1.3.0/src/cobramod/parsing/bigg.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - Metabolites: Normally, simple names.
 - Reactions: Mostly abbreviations.
 - Genes: It is included in the Reactions. Names and gene-reaction-rule is also
 acquired
 
 They change identifiers depending on the model given. BiGG have multiple models
 """
+
 from __future__ import annotations
 
 from contextlib import suppress
 from typing import Any
 
 import requests
```

### Comparing `cobramod-1.2.0/src/cobramod/parsing/biocyc.py` & `cobramod-1.3.0/src/cobramod/parsing/biocyc.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This module handles the retrieval of data from BioCyc into a local directory.
 The possible type of data that can be downloaded:
 
 - Metabolites: Normally have an abbreviation or short name.
 - Reactions: Can have the words "RXN" in the identifier. Enzymes can sometimes
 be used instead. The gene information for the reactions is included if found.
 """
+
 from __future__ import annotations
 
 import urllib.parse
 import xml.etree.ElementTree as et
 from contextlib import suppress
 from pathlib import Path
 from typing import Any
@@ -110,17 +111,17 @@
     }
     return reversibility[text]
 
 
 def parse_reaction_attributes(
     root: et.Element, entry: str, gene_directory: Path
 ) -> dict[str, Any]:
-    name = root.find("*[@ID]/enzymatic-reaction/*/common-name")
-    if name is not None and name.text:
-        name = name.text
+    name_element = root.find("*[@ID]/enzymatic-reaction/*/common-name")
+    if name_element is not None and name_element.text:
+        name = name_element.text
     else:
         name = entry
     equation = reaction_str_from_xml(root)
 
     attributes = {
         "name": name,
         "equation": equation,
```

### Comparing `cobramod-1.2.0/src/cobramod/parsing/db_version.py` & `cobramod-1.3.0/src/cobramod/parsing/db_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Database versioning configurator
 
 This modules includes the class DataVersionConfigurator which is in charge of
 obtaining and comparing the version from the obtained metabolic data.
 It uses the same structure of using a Singleton for the configuration in
 COBRApy
 """
+
 from pathlib import Path
 from typing import Optional, Union
 
 import pandas as pd
 from cobra.core.singleton import Singleton
 
 import cobramod.error as cmod_error
```

### Comparing `cobramod-1.2.0/src/cobramod/parsing/kegg.py` & `cobramod-1.3.0/src/cobramod/parsing/kegg.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 The possible type of data that can be downloaded:
 
 - Metabolite: Identifiers that start with the letter C, e.g C00001
 - Reactions: Identifiers that start with the letter R, e.g R00001. The
 gene information for reactions is also included if the specie is specified
 - Module Pathways: Identifiers that start with the letter M, e.g M00001
 """
+
 from __future__ import annotations
 
 from contextlib import suppress
 from itertools import chain
 from pathlib import Path
 from typing import Any, Generator, Optional
```

### Comparing `cobramod-1.2.0/src/cobramod/parsing/plantcyc.py` & `cobramod-1.3.0/src/cobramod/parsing/plantcyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Gene parsing for Plantcyc
 
 The main functions to parse Metabolites and Reactions are found in the module
 Biocyc
 """
+
 import urllib.parse
 import xml.etree.ElementTree as et
 from pathlib import Path
 from typing import Any
 
 import requests
```

### Comparing `cobramod-1.2.0/src/cobramod/parsing/solcyc.py` & `cobramod-1.3.0/src/cobramod/parsing/solcyc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Gene parsing for SolanaCyc
 
 The main functions to parse Metabolites and Reactions are found in the module
 Biocyc
 """
+
 import urllib.parse
 import xml.etree.ElementTree as et
 from pathlib import Path
 from typing import Any
 
 import requests
```

### Comparing `cobramod-1.2.0/src/cobramod/retrieval.py` & `cobramod-1.3.0/src/cobramod/retrieval.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 data representation for this package. The class Data includes methods for
 parsing itself into a Reaction, Metabolite or Pathway.
 
 Additionally, this package includes high level functions such as `get_data`,
 `file_to_Data_class` or `get_response` that handles the data retrieval or
 convertion
 """
+
 from __future__ import annotations
 
 import json
 import urllib.parse
 import warnings
 import xml.etree.ElementTree as et
 from pathlib import Path
@@ -147,15 +148,15 @@
     database: str
     attributes: dict[str, Any]
     path: Path
     model_id: str
     genome: str
     version: str
     """
-    CobraMod's Data object. This class is responsable for converting
+    CobraMod's Data object. This class is responsible for converting
     information into COBRApy objects
     """
 
     def __init__(
         self,
         identifier: str,
         attributes: dict[str, str],
@@ -192,27 +193,30 @@
                 version = json.load(f).get("bigg_models_version")
         else:
             info_response = requests.get(
                 "http://bigg.ucsd.edu/api/v2/database_version"
             )
             info_response.raise_for_status()
 
-            with path.parents[1].joinpath("database_version").open(
-                mode="w+"
-            ) as f:
+            with (
+                path.parents[1]
+                .joinpath("database_version")
+                .open(mode="w+") as f
+            ):
                 f.write(info_response.text)
             version = info_response.json().get("bigg_models_version")
 
         if version is None:
             raise Exception("Version of the BIGG JSON cannot be empty!")
 
         # Non universal models includes suffices
         if model_id != "universal":
             entry = entry[: entry.find("_")]
 
+        mode: Literal["Pathway", "Reaction", "Metabolite"]
         if is_compound:
             mode = "Metabolite"
             attributes = bigg.parse_metabolite_attributes(data)
         else:
             mode = "Reaction"
             attributes = bigg.parse_reaction_attributes(data, entry)
 
@@ -222,15 +226,15 @@
     def from_text(
         cls, entry: str, text: str, database: str, path: Path, genome: str
     ):
         """
         Creates an instance from plain text. Database: KEGG
         """
         data: dict[str, list[str]] = kegg.data_from_string(text)
-        mode = data["ENTRY"][0].split()[-1]
+        entry_mode = data["ENTRY"][0].split()[-1]
         gene_path = path.parent.joinpath("GENES")
 
         if path.parent.joinpath("database_version").exists():
             with open(path.parent.joinpath("database_version"), "r") as f:
                 version = cmod_utils.kegg_info_to_version(f.read())
         else:
             info_response = requests.get("http://rest.kegg.jp/info/kegg")
@@ -239,47 +243,50 @@
             with path.parent.joinpath("database_version").open(mode="w+") as f:
                 f.write(info_response.text)
             version = cmod_utils.kegg_info_to_version(info_response.text)
 
         if version is None:
             raise Exception("Version of the BIGG JSON cannot be empty!")
 
-        if mode == "Compound":
+        mode: Literal["Pathway", "Reaction", "Metabolite"]
+        if entry_mode == "Compound":
             mode = "Metabolite"
             attributes = kegg.parse_metabolite_attributes(data, entry)
 
-        elif mode == "Reaction":
+        elif entry_mode == "Reaction":
+            mode = "Reaction"
             attributes = kegg.parse_reaction_attributes(
                 data, entry, genome, gene_path
             )
 
-        elif mode == "Module":
+        elif entry_mode == "Module":
             mode = "Pathway"
             attributes = kegg.parse_pathway_attributes(data, entry)
         else:
-            raise AttributeError(f"Cannot parse type '{mode}'")
+            raise AttributeError(f"Cannot parse type '{entry_mode}'")
 
         obj = cls(entry, attributes, mode, database, path, "", version)
         obj.genome = genome
         return obj
 
     @classmethod
     def from_xml(cls, entry: str, root: et.Element, database: str, path: Path):
         """
         Creates an instance from an XML file. Database: Biocyc families
         """
-        version = root.find("metadata/PGDB")
-        if version is not None:
-            version = version.attrib.get("version")
-
-        if version is None:
+        version_element = root.find("metadata/PGDB")
+        if version_element is not None:
+            version: Optional[str] = version_element.attrib.get("version")
+            assert version is not None
+        else:
             raise Exception("Version for the XML cannot be empty!")
 
         gene_path = path.parent.joinpath("GENES")
 
+        mode: Literal["Pathway", "Reaction", "Metabolite"]
         if (
             root.findall("Compound")
             or root.findall("Protein")
             or root.findall("RNA")
         ):
             mode = "Metabolite"
             attributes = biocyc.parse_metabolite_attributes(root, entry)
@@ -599,25 +606,26 @@
         family = family.upper()
 
         directory = directory.joinpath(family)
 
     if not directory.exists():
         directory.mkdir()
 
+    extra: Path
     # Try first locally and the query databases
     if not database:
         try:
             filename = next(directory.rglob(identifier + "*"))
             response_database = filename.parent.name.upper()
 
         except StopIteration:
             response_database, response = get_response(identifier)
 
             if response_database == "bigg":
-                extra: Path = getattr(response, "extra")
+                extra = getattr(response, "extra")
 
                 if not extra:
                     raise AttributeError(
                         "The 'extra' attribute was not found in the response"
                     )
                 directory = directory.joinpath(extra)
 
@@ -674,15 +682,15 @@
                         DeprecationWarning,
                     )
                     solcyc.retrieve_gene_information(
                         directory, identifier, database
                     )
 
             if response_database == "BIGG":
-                extra: Path = getattr(response, "extra")
+                extra = getattr(response, "extra")
 
                 if not extra:
                     raise AttributeError(
                         "The 'extra' attribute was not found in the response"
                     )
                 directory = directory.joinpath("BIGG", extra)
 
@@ -736,50 +744,52 @@
     position = cmod_utils.get_arrow_position(reaction_str)
     arrow = reaction_str[position : position + 3]
     reaction.bounds = cmod_utils.ARROWS[arrow]
 
     compounds: dict[str, float] = {}
     # Reactants
     for pair in reaction_str[:position].rstrip().strip().split("+"):
+        coefficient: Union[str, float]
         try:
-            coefficient, metabolite = pair.rstrip().strip().split(" ")
+            coefficient, metabolite_str = pair.rstrip().strip().split(" ")
         except ValueError:
             coefficient = 1
-            metabolite = pair.rstrip().strip()
+            metabolite_str = pair.rstrip().strip()
 
             # Empty part
-            if metabolite == "":
+            if metabolite_str == "":
                 break
 
-        compounds[metabolite] = -1.0 * float(coefficient)
+        compounds[metabolite_str] = -1.0 * float(coefficient)
 
     # products
     for pair in reaction_str[position + 3 :].rstrip().strip().split("+"):
         try:
-            coefficient, metabolite = pair.rstrip().strip().split(" ")
+            coefficient, metabolite_str = pair.rstrip().strip().split(" ")
         except ValueError:
             coefficient = 1
-            metabolite = pair.rstrip().strip()
+            metabolite_str = pair.rstrip().strip()
 
             # Empty part
-            if metabolite == "":
+            if metabolite_str == "":
                 break
 
-        compounds[metabolite] = float(coefficient)
+        compounds[metabolite_str] = float(coefficient)
 
     # It must be a biocyc family
     # if database is not None and database.find(":") != -1:
     #     directory = directory.parent
 
     for identifier, coefficient in compounds.items():
         compartment = identifier[-1]
 
         identifier = replacement.get(identifier[:-2], identifier[:-2])
         identifier = f"{identifier}_{compartment}"
 
+        metabolite: cobra_core.Metabolite
         try:
             data = get_data(identifier[:-2], directory, database, model_id)
             metabolite = creation.metabolite_from_data(data, compartment, model)
 
         except (requests.HTTPError, ValueError):
             metabolite = cobra_core.Metabolite(
                 identifier, name=identifier, compartment=compartment
```

### Comparing `cobramod-1.2.0/src/cobramod/utils.py` & `cobramod-1.3.0/src/cobramod/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This module is intended to stored multiple functions, which cannot be grouped
 to any module. In other words, these functions are general functions. An
 example:
 
  - check_imbalance: Check for unbalanced reactions.
 """
+
 import io
 from pathlib import Path
 from re import match
 from typing import Any, Generator, Iterable, Iterator, Optional, TextIO
 
 import cobra.core as cobra_core
 from cobra import DictList, Reaction
```

### Comparing `cobramod-1.2.0/src/cobramod/visualization/__init__.py` & `cobramod-1.3.0/src/cobramod/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `cobramod-1.2.0/src/cobramod/visualization/converter.py` & `cobramod-1.3.0/src/cobramod/visualization/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,29 @@
 - add_reaction: Parses a reaction string and add the information into the
 JsonDictionary.
 - add_blank: Adds a empty reaction. This is useful for the extra space in the
 visualizations.
 - visualize: Saves Escher visualization as a HTML and return the Escher
 Builder.
 """
+
 import fileinput
 import math
 from collections import UserDict, namedtuple
 from contextlib import suppress
 from itertools import cycle
 from json import dumps
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import webcolors
 
+from cobramod.visualization.escher import EscherIntegration
+
 try:
     import escher
 except ImportError:
     # NOTE: there might be a better way
     pass
 
 from cobramod.visualization.debug import debug_log
@@ -257,15 +260,15 @@
         return {
             "x": self.X,
             "y": self.Y,
             "width": self.CANVAS_WIDTH,
             "height": self.CANVAS_HEIGHT,
         }
 
-    def json_dump(self, indent: int = None) -> str:
+    def json_dump(self, indent: Optional[int] = None) -> str:
         """
         Returns a string that is the JSON representation of this class.
 
         Args:
             indent (int): Defines the indentation for the JSON.
                 Defaults to None.
         """
@@ -774,18 +777,18 @@
         self.data["reactions"] = {}
         self.data["nodes"] = {}
         self.reaction_scale = dict()
 
     def color_grading(
         self,
         color: List[Union[str, List[int], None]],
-        min_max: List[float] = None,
+        min_max: Optional[List[float]] = None,
         quantile: bool = False,
         max_steps: int = 100,
-        n_steps: int = None,
+        n_steps: Optional[int] = None,
     ):
         """
         Function that creates a color scale between two predefined colors. The
         number of color gradations corresponds to the number of fluxes.
 
         Parameters:
             color (list of str or list of list of int):
@@ -939,14 +942,16 @@
         filepath: Union[str, Path],
         vertical: bool = False,
         color: Optional[List[Union[str, List[int], None]]] = None,
         min_max: Optional[List[float]] = None,
         quantile: bool = False,
         max_steps: int = 100,
         n_steps: Optional[int] = None,
+        custom_integration: bool = False,
+        never_ask_before_quit: bool = False,
     ):
         """
         Saves the visualization of the JsonDictionary in given path as a HTML.
         Returns the builder for the JsonDictionary. If method is called in
         Jupyter or Qtconsole, it will show the embedded builder of the escher
         visualization. Else, it will open the default browser of the operating
         system and will load the previously saved HTML.
@@ -1024,34 +1029,48 @@
                 color=color,
                 min_max=min_max,
                 quantile=quantile,
                 max_steps=max_steps,
                 n_steps=n_steps,
             )
 
-        builder = escher.Builder(
-            # Check how reaction_styles behaves
-            reaction_styles=["color", "text"],
-            map_name=self.data["head"]["map_name"],
-            map_json=self.json_dump(),
-            reaction_scale=self.reaction_scale,
-        )
+        if not custom_integration:
+            builder = escher.Builder(
+                # Check how reaction_styles behaves
+                reaction_styles=["color", "text"],
+                map_name=self.data["head"]["map_name"],
+                map_json=self.json_dump(),
+                reaction_scale=self.reaction_scale,
+            )
+
+            if self.flux_solution:
+                builder.reaction_data = self.flux_solution
+            builder.save_html(filepath=filepath)
+
+            f = fileinput.FileInput(filepath, inplace=True)
+            for line in f:
+                if f.lineno() == 6:
+                    print(line.replace("1.7.4", "1.7.3"), end="")
+                else:
+                    print(line, end="")
+            f.close()
+            debug_log.info(f'Visualization saved in "{filepath}"')
+
+        else:
+            builder = EscherIntegration(
+                # Check how reaction_styles behaves
+                reaction_styles=["color", "text"],
+                map_name=self.data["head"]["map_name"],
+                map_json=self.json_dump(),
+                reaction_scale=self.reaction_scale,
+                reaction_data=self.flux_solution,
+                never_ask_before_quit=never_ask_before_quit,
+            )
+
+            builder.save_html(filepath=filepath)
+
         # This statement is needed, otherwise, all reactions labels will
         # appear with "(nd)".
-        if self.flux_solution:
-            builder.reaction_data = self.flux_solution
-        builder.save_html(filepath=filepath)
-
-        # FIXME: temporal solution to https://github.com/Toepfer-Lab/escher-legacy/pull/6
-        f = fileinput.FileInput(filepath, inplace=True)
-        for line in f:
-            if f.lineno() == 6:
-                print(line.replace("1.7.4", "1.7.3"), end="")
-            else:
-                print(line, end="")
-        f.close()
-
-        debug_log.info(f'Visualization saved in "{filepath}"')
 
         # Cleaning Up
         self._reset()
         return builder
```

### Comparing `cobramod-1.2.0/src/cobramod/visualization/debug.py` & `cobramod-1.3.0/src/cobramod/visualization/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Configures the debug logging tool. The format follows the syntax: `(asctime)
 (levelname) (message)`. The logs are saved in the logs directory and includes
 'visualization' in the file and its date. The default level is set to DEBUG.
 
 The name of logger variable is `visualization`
 """
+
 import datetime as dt
 import logging
 from pathlib import Path
 
 
 debug_log = logging.getLogger("visualization")
 debug_log.setLevel(logging.DEBUG)
```

### Comparing `cobramod-1.2.0/src/cobramod/visualization/items.py` & `cobramod-1.3.0/src/cobramod/visualization/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 The classes retain their original JSON names and attributes.
 - Node: Represents the nodes. They can be a metabolite or markers. They give
 the position of all dots in the canvas.
 - Segment: Represents the connections between nodes.
 - Reaction: Represents a reaction. They contain the needed segments for the
 visualization of the pathway.
 """
+
 from contextlib import suppress
 from collections import UserDict
-from typing import Any
+from typing import Any, Optional
 
 from cobramod.error import NodeAttributeError
 from cobramod.visualization.pair import PairDictionary
 from cobramod.visualization.debug import debug_log
 
 
 class Node(UserDict):
@@ -29,16 +30,16 @@
     """
 
     def __init__(
         self: Any,
         node_type: str,
         x: float,
         y: float,
-        label_x: float = None,
-        label_y: float = None,
+        label_x: Optional[float] = None,
+        label_y: Optional[float] = None,
         bigg_id: str = "",
         name: str = "",
         node_is_primary: bool = False,
     ):
         """
         Build a node for JsonCobramod, which can be parsed later into a proper
         JSON for Escher. A node can be a metabolite, midmarker or multimarker.
```

### Comparing `cobramod-1.2.0/src/cobramod/visualization/mapping.py` & `cobramod-1.3.0/src/cobramod/visualization/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This modules handles the mapping of a directed graph into a matrix that can be
 used in Escher. The main function is
 :func:`cobramod.visualization.mapping.get_mapping`, which checks if the graph
 is lineal and creates the representation in a matrix. In case of cyclic path,
 it will cut it.
 """
+
 from itertools import chain
 from typing import Dict, List
 
 from cobramod.core.graph import get_graph_dict
 
 
 def get_all_values(dictionary: dict, keys: list) -> set:
@@ -117,15 +118,15 @@
     longest = mapping[0]
     # TODO: change defaults of height
     relation = child_map(mapping=mapping, dictionary=graph)
     # If path is completely unrelated
     if not relation:
         return mapping
     matrix = [[0] * len(longest)]
-    matrix[0] = longest
+    matrix[0] = longest  # type: ignore
     # dictionary for start positions
     start_position = {"0": 0}
     for index, keys in relation.items():
         # child = item, parent = index
         item: str
         for item in keys:
             # Should not raised an error since we have the relation
@@ -139,22 +140,22 @@
             try:
                 start = start_position[str(index)]
             except KeyError:
                 start = 0
             # add 0's and extend
             start_position[item] = start + position_j + 1
             row = [0] * start_position[item]
-            row.extend(mapping[int(item)])
+            row.extend(mapping[int(item)])  # type: ignore
             matrix.append(row)
     # Add unrelated paths
     for index, line in enumerate(mapping):
         if str(index) not in relation.keys() and str(index) not in list(
             chain.from_iterable(relation.values())
         ):
-            matrix.append(line)
+            matrix.append(line)  # type: ignore
     return matrix
 
 
 def fill_matrix(matrix: List[list], length: int):
     """
     Fills each row of the matrix with 0 until it reaches given length
```

### Comparing `cobramod-1.2.0/src/cobramod/visualization/pair.py` & `cobramod-1.3.0/src/cobramod/visualization/pair.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from collections import UserDict
 from contextlib import suppress
+from typing import Optional
 
 from cobramod.error import FoundInPairError
 
 
 class PairDictionary(UserDict):
     """
     Dictionary that can include a pair (linked) dictionary. Both dictionaries
     cannot have the same keys. It is posible that only a dictionary is a
     PairDictionary, while the other a regular dictionary. The method
     :func:`cobramod.visualization.PairDictionary.set_pair' sets the pair
     for the dictionary.
     """
 
-    def __init__(self, pair: UserDict = None, **kwargs):
+    def __init__(self, pair: Optional[UserDict] = None, **kwargs):
         """
         Creates the regular dictionary and can set a pair dictionary if given.
         All keyword-arguments from a regular dictionary can be passed to this
         method.
         """
         self.pair = pair
         super().__init__(**kwargs)
```

### Comparing `cobramod-1.2.0/src/cobramod.egg-info/PKG-INFO` & `cobramod-1.3.0/src/cobramod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobramod
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python package for pathway-centric modification and extension of genome-scale metabolic networks
 Author-email: Stefano Camborda La Cruz <scambord@uni-koeln.de>, Jan-Niklas Weder <jweder@uni-koeln.de>, Nadine Töpfer <ntoepfer@uni-koeln.de>
 Maintainer-email: Nadine Töpfer <ntoepfer@uni-koeln.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -692,46 +692,53 @@
 Requires-Dist: colorlog
 Requires-Dist: cobra>=0.29.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: webcolors>=1.13
 Requires-Dist: pyarrow>=14.0.2
+Requires-Dist: anywidget>=0.9.9
 Provides-Extra: escher
 Requires-Dist: escher-legacy>=1.7.4; extra == "escher"
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
 Requires-Dist: sphinx; extra == "dev"
 Requires-Dist: nbsphinx; extra == "dev"
 Requires-Dist: sphinx-autoapi; extra == "dev"
 Requires-Dist: jupyter-contrib-nbextensions; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: sphinxcontrib-napoleon; extra == "dev"
 Requires-Dist: sphinxcontrib-bibtex; extra == "dev"
 
+<div align="center">
+
 ![Static Badge](https://img.shields.io/badge/python-3.10%7C3.11%7C3.12-%20blue)
 ![GitHub](https://img.shields.io/github/license/Toepfer-Lab/cobramod)
-![Read the Docs (version)](https://img.shields.io/readthedocs/cobramod/latest)
-![Tests](https://img.shields.io/github/workflow/status/Toepfer-Lab/cobramod/Test%20build%20and%20publish%20Cobramod%20to%20PyPI?label=tests)
-![Version](https://img.shields.io/pypi/v/cobramod?label=version)
-[![Downloads](https://pepy.tech/badge/cobramod)](https://pepy.tech/project/cobramod)
+[![Downloads](https://img.shields.io/pepy/dt/cobramod
+)](https://pepy.tech/project/cobramod)
 
+![Version](https://img.shields.io/pypi/v/cobramod?label=version)
+![Read the Docs (version)](https://img.shields.io/readthedocs/cobramod/latest)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/Toepfer-lab/cobramod/test-build-and-publish.yml)
+![Coverage Status](./docs/source/img/coverage.svg)
 
 CobraMod: A pathway-centric curation tool for constraint-based metabolic models
 ===============================================================================
 
+
 ![image](https://raw.githubusercontent.com/Toepfer-Lab/cobramod/master/docs/source/img/logo.png)
+</div>
 
 CobraMod is a Python 3 open-source package for pathway-centric curation of
-genome-scale metabolic models (GEMs). It builds upon the [COBRApy toolbox]
-(https://opencobra.github.io/cobrapy/) and offers a comprehensible set of
-functions for semi-automated network extension, curation and visualization.
-CobraMod supports all databases from the [BioCyc collection](https://
-biocyc.org/), the [KEGG database](https://www.genome.jp/kegg/), and the [BiGG
+genome-scale metabolic models (GEMs). It builds upon the 
+[COBRApy toolbox](https://opencobra.github.io/cobrapy/) and offers a 
+comprehensible set of functions for semi-automated network extension, curation and visualization.
+CobraMod supports all databases from the [BioCyc collection](https://biocyc.org/), 
+the [KEGG database](https://www.genome.jp/kegg/), and the [BiGG
 Models repository](http://bigg.ucsd.edu/). It optionally can interact with
 Escher for pathway and flux visualization.
 
 This package converts pathway information into native COBRApy objects and
 quality-checks them while adding them to the model. This includes testing for:
 
 -   duplicate elements
@@ -801,14 +808,33 @@
 CobraMod is licensed under the GPL-3 License. Read the
 [LICENSE](https://github.com/Toepfer-Lab/cobramod/blob/master/LICENSE)
 for more information.
 
 
 Development
 -----------
+CobraMod consists of a Python and JavaScript/TypeScript part. 
+The following briefly describes all the commands to build a local 
+version from the source files.
+
+### JavaScript
+
+Since we need Node modules to build the Jupyter integrations con CobraMod, 
+a package.json is included in the project. All dependencies contained 
+in it can be made available locally using [yarn](https://yarnpkg.com/). The foiling command can be used for this:
+
+    yarn install
+
+We use [Vite](https://vitejs.dev/) to build the Javascript part of the Jupyter integrations. So, we can use the following command to build a bundled version of the integrations.
+
+    yarn run vite build
+
+This creates bundled JavaScript files under '/src/cobramod/static'.
+
+### Python
 
 You can contribute to CobraMod by cloning the repository and installing it in
 developer mode and using the `dev` dependency group via pip:
 
     pip install -e ".[dev]"
 
 Optionally, a conda environment file is supplied (*environment.yml*). This
```

### Comparing `cobramod-1.2.0/src/cobramod.egg-info/SOURCES.txt` & `cobramod-1.3.0/src/cobramod.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -16,26 +16,33 @@
 src/cobramod/core/creation.py
 src/cobramod/core/crossreferences.py
 src/cobramod/core/extension.py
 src/cobramod/core/genes.py
 src/cobramod/core/graph.py
 src/cobramod/core/pathway.py
 src/cobramod/core/summary.py
+src/cobramod/data/__init__.py
 src/cobramod/data/textbook_biocyc.sbml
+src/cobramod/data/textbook_biocyc_groups.sbml
 src/cobramod/data/textbook_kegg.sbml
 src/cobramod/parsing/__init__.py
 src/cobramod/parsing/bigg.py
 src/cobramod/parsing/biocyc.py
 src/cobramod/parsing/db_version.py
 src/cobramod/parsing/kegg.py
 src/cobramod/parsing/plantcyc.py
 src/cobramod/parsing/solcyc.py
+src/cobramod/static/LICENSES.txt
+src/cobramod/static/escher.mjs
+src/cobramod/static/force_graph.mjs
 src/cobramod/visualization/__init__.py
 src/cobramod/visualization/converter.py
 src/cobramod/visualization/debug.py
+src/cobramod/visualization/escher.py
+src/cobramod/visualization/force_graph.py
 src/cobramod/visualization/items.py
 src/cobramod/visualization/mapping.py
 src/cobramod/visualization/pair.py
 tests/test_creation.py
 tests/test_crossreferences.py
 tests/test_extension.py
 tests/test_genes.py
```

### Comparing `cobramod-1.2.0/tests/test_creation.py` & `cobramod-1.3.0/tests/test_creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 metabolites are tested. Important is the independency of the functions, unless
 they are part of the API such as add_metabolites. Therefore the modules is
 separated in:
 
 - SimpleFunctions: Creation of objects
 - ComplexFunctions: Functions, that uses multiple simple functions.
 """
+
 import unittest
 from logging import DEBUG
 from pathlib import Path
 
 import cobra.core as cobra_core
 import cobramod.retrieval as cmod_retrieval
 import requests
@@ -23,16 +24,14 @@
 from cobramod.error import NoDelimiter, WrongSyntax
 from cobramod.parsing.db_version import DataVersionConfigurator
 from cobramod.test import textbook_kegg
 
 NAME = "test_model"
 
 debug_log.setLevel(DEBUG)
-data_conf = DataVersionConfigurator()
-data_conf.force_same_version = True
 
 dir_data = Path(__file__).resolve().parent.joinpath("data")
 dir_input = Path(__file__).resolve().parent.joinpath("input")
 
 # If data is missing, then do not test. Data should always be the same
 if not dir_data.exists():
     raise NotADirectoryError("Data for the test is missing")
@@ -40,14 +39,20 @@
 
 class SimpleFunctions(unittest.TestCase):
     """
     Test for simple test such as creating metabolites from string or from
     files.
     """
 
+    @classmethod
+    def setUp(cls):
+        # ToDo Versioning should be tested in its own test class
+        data_conf = DataVersionConfigurator()
+        data_conf.ignore_db_versions = True
+
     def test_find_replacements(self):
         replace_dict = {
             "ACETALD-DEHYDROG-RXN": "R00228_c",
             "WATER_c": "C00001_c",
             "WATER_d": "C00001_d",
         }
         # CASE 1: Reaction
@@ -561,18 +566,14 @@
         test_names = ["GLC_cb", "RXN_14462_p"]
         self.assertListEqual(
             list1=test_names, list2=[reaction.id for reaction in test_list]
         )
 
 
 class ComplexFunctions(unittest.TestCase):
-    # @classmethod
-    # def setUpClass(cls):
-    #     BaseParser.ignore_db_versions = True
-
     def test_create_object(self):
         # CASE: metabolite from MetaCyc
         test_object = cr.create_object(
             identifier="GLC",
             directory=dir_data,
             compartment="c",
             database="META",
```

### Comparing `cobramod-1.2.0/tests/test_crossreferences.py` & `cobramod-1.3.0/tests/test_crossreferences.py`

 * *Files identical despite different names*

### Comparing `cobramod-1.2.0/tests/test_extension.py` & `cobramod-1.3.0/tests/test_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 divided in to parts:
 
 - CreatingSequences: Functions, that create the corresponding reactions as
 sequences and their corresponding flux test.
 - AddingPathways: Functions, that manage the addition of Pathways into the
 metabolic models.
 """
+
 import logging
 import unittest
 from pathlib import Path
 
 import cobra.core as cobra_core
 import cobramod.error as cmod_error
 import cobramod.retrieval as cmod_retrieval
@@ -26,26 +27,30 @@
 from cobramod.debug import change_to_debug
 from cobramod.parsing.db_version import DataVersionConfigurator
 from cobramod.test import textbook, textbook_biocyc, textbook_kegg
 
 NAME = "test_model"
 
 change_to_debug()
-data_conf = DataVersionConfigurator()
-data_conf.force_same_version = True
 
 dir_data = Path(__file__).resolve().parent.joinpath("data")
 dir_input = Path(__file__).resolve().parent.joinpath("input")
 
 # If data is missing, then do not test. Data should always be the same
 if not dir_data.exists():
     raise NotADirectoryError("Data for the test is missing")
 
 
 class CreatingSequences(unittest.TestCase):
+    @classmethod
+    def setUp(cls):
+        # ToDo Versioning should be tested in its own test class
+        data_conf = DataVersionConfigurator()
+        data_conf.ignore_db_versions = True
+
     def test_create_reactions(self):
         # CASE: Simple Case Biocyc
         generator = ex.yield_reaction_from_list(
             sequence=[
                 "OXALODECARB-RXN",
                 "AROMATIC-L-AMINO-ACID-DECARBOXYLASE-RXN",
             ],
```

### Comparing `cobramod-1.2.0/tests/test_genes.py` & `cobramod-1.3.0/tests/test_genes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 """Unittest for genes verification
 
 In this module, the creation of genes for multiple function and their behavior
 are checked
 """
+
 import logging
 import unittest
 from pathlib import Path
 
 import cobra.core as cobra_core
 from cobra import __version__ as cobra_version
 from cobramod import __version__ as cmod_version
```

### Comparing `cobramod-1.2.0/tests/test_graph.py` & `cobramod-1.3.0/tests/test_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 """Unittest for module graph
 
 In this modules, the new algorithm is tested. The TestCase GraphTesting checks
 that the behavior of all important functions works as intended
 """
+
 import unittest
 from pathlib import Path
 from typing import Any
 
 import cobramod.core.graph as gr
 from cobra import __version__ as cobra_version
 from cobramod import __version__ as cmod_version
```

### Comparing `cobramod-1.2.0/tests/test_models.py` & `cobramod-1.3.0/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 This module checks if a large and a small model behaves as intended. This
 examples should simulate real cases. There are two test:
 
 - ShortModel: This should utilize the textbook_biocyc model from cobramod.
 - LargeModel: Uses a real GEM
 """
+
 import unittest
 from pathlib import Path
 
 import cobra.core as cobra_core
 import cobra.io as cobra_io
 import cobramod.error as cmod_error
 from cobra import __version__ as cobra_version
@@ -20,29 +21,32 @@
 from cobramod.debug import change_to_debug
 from cobramod.parsing.db_version import DataVersionConfigurator
 from cobramod.test import textbook_biocyc
 
 change_to_debug()
 dir_data = Path(__file__).resolve().parent.joinpath("data")
 
-data_conf = DataVersionConfigurator()
-
 # If data is missing, then do not test. Data should always be the same
 if not dir_data.exists():
     raise NotADirectoryError("Data for the test is missing")
 
 dir_input = Path(__file__).resolve().parent.joinpath("input")
 
 # Large Model
 main_model = cobra_io.read_sbml_model(
     str(dir_input.joinpath("test_model.sbml"))
 )
 
 
 class ShortModel(unittest.TestCase):
+    @classmethod
+    def setUp(cls):
+        data_conf = DataVersionConfigurator()
+        data_conf.ignore_db_versions = True
+
     def test_lineal_pathways(self):
         # For this test, Gluconeogenesis; L-aspartate and L-asparagine
         # biosynthesis, and Nicotine biosynthesis added to test for feasible
         # results.
         test_model = textbook_biocyc.copy()
 
         # Adding Gluconeogenesis
```

### Comparing `cobramod-1.2.0/tests/test_parsing.py` & `cobramod-1.3.0/tests/test_parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 - TestBiocyc: For Biocyc-related databases
 - TestBigg: For BiGG database
 - TestKegg: For Kegg
 - TestPlantCyc: For PlantCyc
 - TestSolcyc: For SolCyc
 """
+
 import unittest
 from pathlib import Path
 
 import cobra.core as cobra_core
 import cobramod.error as cmod_error
 import cobramod.retrieval as cmod_retrieval
 import requests
@@ -24,14 +25,15 @@
 from cobramod.parsing.db_version import DataVersionConfigurator
 
 dir_data = Path(__file__).resolve().parent.joinpath("data")
 
 change_to_debug()
 data_conf = DataVersionConfigurator()
 
+
 # If data is missing, then do not test. Data should always be the same
 if not dir_data.exists():
     raise NotADirectoryError("Data for the test is missing")
 
 
 class TestKegg(unittest.TestCase):
     """
```

### Comparing `cobramod-1.2.0/tests/test_pathway.py` & `cobramod-1.3.0/tests/test_pathway.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python3
 """Unittest for module pathway
 
 This module includes the TestCase TestGroup. This checks the behavior of the
 new child of :obj:`cobra.core.group.Group` "Pathway". This new class is able
 to use Escher for its visualizations.
 """
+
 import unittest
 from json import loads
 from pathlib import Path
 from random import randint
 from tempfile import TemporaryDirectory
 from time import sleep
 from webbrowser import open as web_open
 
 import cobra.core as cobra_core
 import cobra.io as cobra_io
 import cobramod.error as cmod_error
 import cobramod.test as cmod_test
-import escher
 import pandas as pd
 from cobra import __version__ as cobra_version
 from cobramod import __version__ as cmod_version
 from cobramod.core import pathway as pt
 from cobramod.core.extension import add_pathway
 from cobramod.debug import change_to_debug
 
@@ -190,22 +190,20 @@
         test_group.graph = {
             "EX_glc__D_e": "GLCpts",
             "GLCpts": "G6PDH2r",
             "G6PDH2r": "PGL",
             "PGL": "GND",
             "GND": None,
         }
-        test_builder = test_group.visualize()
+        test_builder = test_group.visualize(vis="escher-custom")
 
         web_open("pathway.html")
         sleep(1)
         test_group.vertical = True
-        test_builder = test_group.visualize()
-        if not isinstance(test_builder, escher.Builder):
-            raise TypeError("Escher was not loaded")
+        test_builder = test_group.visualize(vis="escher-custom")
 
         self.assertEqual(
             first=len(loads(test_builder.map_json)[1]["reactions"]),  # type: ignore
             second=5,
         )
         # CASE: Members after initialization.
         test_model = cmod_test.textbook.copy()
@@ -246,20 +244,24 @@
 
         self.assertEqual(first=len(test_pathway.members), second=5)
         test_solution = {
             reaction.id: randint(-4, 4) for reaction in test_pathway.members
         }
         test_pathway.color_negative = "red"
         test_pathway.color_positive = "green"
-        test_pathway.visualize(solution_fluxes=test_solution)
+        test_pathway.visualize(
+            solution_fluxes=test_solution, vis="escher-custom"
+        )
         web_open("pathway.html")
         sleep(1)
 
         test_pathway.vertical = True
-        test_pathway.visualize(solution_fluxes=test_solution)
+        test_pathway.visualize(
+            solution_fluxes=test_solution, vis="escher-custom"
+        )
         web_open("pathway.html")
         sleep(1)
 
         # CASE: Regular Biocyc
         add_pathway(
             model=test_model,
             pathway="PWY-1187",
@@ -277,19 +279,23 @@
         self.assertEqual(first=len(test_pathway.members), second=14)
         self.assertTrue(expr=test_pathway.notes["ORDER"])
         test_solution: dict[str, float] = {
             reaction.id: randint(-4, 4) for reaction in test_pathway.members
         }
         test_pathway.color_negative = "purple"
         test_pathway.color_positive = "blue"
-        test_pathway.visualize(solution_fluxes=test_solution)
+        test_pathway.visualize(
+            solution_fluxes=test_solution, vis="escher-custom"
+        )
         web_open("pathway.html")
         sleep(1)
         test_pathway.vertical = True
-        test_pathway.visualize(solution_fluxes=test_solution)
+        test_pathway.visualize(
+            solution_fluxes=test_solution, vis="escher-custom"
+        )
 
     def test_model_convert(self):
         # CASE: regular conversion of Groups
         test_model = cmod_test.textbook.copy()
         test_list = [
             test_model.reactions[0],
             test_model.reactions[1],
```

### Comparing `cobramod-1.2.0/tests/test_summary.py` & `cobramod-1.3.0/tests/test_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 """Unitest for build of summary
 
 This modules checks functions responsable for the creation of txt, csv and xlsx
 files.
 """
+
 import tempfile
 from pathlib import Path
 from unittest import TestCase, main
 
 import numpy
 import pandas
 from cobra import Model
```

### Comparing `cobramod-1.2.0/tests/test_test.py` & `cobramod-1.3.0/tests/test_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 """
 Check if models are available
 """
+
 import unittest
-from pathlib import Path
+from importlib import resources
+
+import cobra
 
-import pkg_resources
+import cobramod
 
 
 class ModuleTest(unittest.TestCase):
     def test_directory(self):
         self.assertTrue(
-            Path(
-                pkg_resources.resource_filename("cobra", "data/textbook.xml.gz")
-            ).exists()
+            resources.files(cobra).joinpath("data/textbook.xml.gz").is_file()
         )
         self.assertTrue(
-            Path(
-                pkg_resources.resource_filename(
-                    "cobramod", "data/textbook_biocyc.sbml"
-                )
-            ).exists()
+            resources.files(cobramod)
+            .joinpath("data/textbook_biocyc.sbml")
+            .is_file()
         )
         self.assertTrue(
-            Path(
-                pkg_resources.resource_filename(
-                    "cobramod", "data/textbook_kegg.sbml"
-                )
-            ).exists()
+            resources.files(cobramod)
+            .joinpath("data/textbook_kegg.sbml")
+            .is_file()
         )
 
 
 if __name__ == "__main__":
     unittest.main(verbosity=2, failfast=True)
```

### Comparing `cobramod-1.2.0/tests/test_utils.py` & `cobramod-1.3.0/tests/test_utils.py`

 * *Files identical despite different names*

