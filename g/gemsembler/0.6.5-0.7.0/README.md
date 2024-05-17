# Comparing `tmp/gemsembler-0.6.5.tar.gz` & `tmp/gemsembler-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemsembler-0.6.5.tar", last modified: Tue Apr 30 11:34:24 2024, max compression
+gzip compressed data, was "gemsembler-0.7.0.tar", last modified: Fri May 17 09:11:59 2024, max compression
```

## Comparing `gemsembler-0.6.5.tar` & `gemsembler-0.7.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.572217 gemsembler-0.6.5/
--rw-rw-rw-   0 root         (0) root         (0)     1083 2024-04-30 11:34:12.000000 gemsembler-0.6.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-30 11:34:12.000000 gemsembler-0.6.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5466 2024-04-30 11:34:24.572217 gemsembler-0.6.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3046 2024-04-30 11:34:12.000000 gemsembler-0.6.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-30 11:34:12.000000 gemsembler-0.6.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-30 11:34:24.572217 gemsembler-0.6.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.561216 gemsembler-0.6.5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.565216 gemsembler-0.6.5/src/gemsembler/
--rw-rw-rw-   0 root         (0) root         (0)     1823 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     7949 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/anticreation.py
--rw-rw-rw-   0 root         (0) root         (0)    19906 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/comparison.py
--rw-rw-rw-   0 root         (0) root         (0)    14845 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/conversion.py
--rw-rw-rw-   0 root         (0) root         (0)    52270 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/creation.py
--rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/curation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.566216 gemsembler-0.6.5/src/gemsembler/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.567216 gemsembler-0.6.5/src/gemsembler/data/BU/
--rw-rw-rw-   0 root         (0) root         (0)   180894 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   303843 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   381510 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_gapseq.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    83221 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/BU/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.571216 gemsembler-0.6.5/src/gemsembler/data/LP/
--rw-rw-rw-   0 root         (0) root         (0)   153653 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA1.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   157673 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA2.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)    82710 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_MS2.sbml.gz
--rw-rw-rw-   0 root         (0) root         (0)   885760 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
--rw-rw-rw-   0 root         (0) root         (0)   151435 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   124883 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
--rw-rw-rw-   0 root         (0) root         (0)   547669 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/LP/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10388 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/dbs.py
--rw-rw-rw-   0 root         (0) root         (0)    18938 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/downstream.py
--rw-rw-rw-   0 root         (0) root         (0)    34325 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/drawing.py
--rw-rw-rw-   0 root         (0) root         (0)    24547 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/gathering.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/general.py
--rw-rw-rw-   0 root         (0) root         (0)    13452 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/genes.py
--rw-rw-rw-   0 root         (0) root         (0)    22859 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/pathsfinding.py
--rw-rw-rw-   0 root         (0) root         (0)     4557 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/periplasmic.py
--rw-rw-rw-   0 root         (0) root         (0)    10165 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    31443 2024-04-30 11:34:12.000000 gemsembler-0.6.5/src/gemsembler/structural.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.571216 gemsembler-0.6.5/src/gemsembler.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5466 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1435 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-30 11:34:24.000000 gemsembler-0.6.5/src/gemsembler.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-30 11:34:24.571216 gemsembler-0.6.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)    12691 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_conversion.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_curation.py
--rw-rw-rw-   0 root         (0) root         (0)     4293 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_dbs.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_gathering.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-30 11:34:12.000000 gemsembler-0.6.5/tests/test_selection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.019624 gemsembler-0.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2024-05-17 09:11:46.000000 gemsembler-0.7.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-05-17 09:11:46.000000 gemsembler-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5466 2024-05-17 09:11:59.018624 gemsembler-0.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-17 09:11:46.000000 gemsembler-0.7.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-17 09:11:46.000000 gemsembler-0.7.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 09:11:59.019624 gemsembler-0.7.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.006623 gemsembler-0.7.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.011623 gemsembler-0.7.0/src/gemsembler/
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10184 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/anticreation.py
+-rw-rw-rw-   0 root         (0) root         (0)    19906 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/comparison.py
+-rw-rw-rw-   0 root         (0) root         (0)    14845 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)    51980 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/curation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.012623 gemsembler-0.7.0/src/gemsembler/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.014623 gemsembler-0.7.0/src/gemsembler/data/BU/
+-rw-rw-rw-   0 root         (0) root         (0)   180894 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/BU/BU_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   303843 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/BU/BU_carveme_hom.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   381510 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/BU/BU_gapseq.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    83221 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/BU/BU_modelSEED.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/BU/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.017624 gemsembler-0.7.0/src/gemsembler/data/LP/
+-rw-rw-rw-   0 root         (0) root         (0)   153653 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/LP_CA1.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   157673 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/LP_CA2.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)    82710 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/LP_MS2.sbml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   885760 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/LP_WCFS1.fasta.gz
+-rw-rw-rw-   0 root         (0) root         (0)   151435 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   124883 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz
+-rw-rw-rw-   0 root         (0) root         (0)   547669 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/LP_protein_fasta.faa.gz
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/LP/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10388 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18993 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/downstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    34325 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/drawing.py
+-rw-rw-rw-   0 root         (0) root         (0)    24547 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    13452 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/genes.py
+-rw-rw-rw-   0 root         (0) root         (0)    22859 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/pathsfinding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4557 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/periplasmic.py
+-rw-rw-rw-   0 root         (0) root         (0)    10165 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    31443 2024-05-17 09:11:46.000000 gemsembler-0.7.0/src/gemsembler/structural.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.018624 gemsembler-0.7.0/src/gemsembler.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5466 2024-05-17 09:11:58.000000 gemsembler-0.7.0/src/gemsembler.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-05-17 09:11:59.000000 gemsembler-0.7.0/src/gemsembler.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 09:11:58.000000 gemsembler-0.7.0/src/gemsembler.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-17 09:11:58.000000 gemsembler-0.7.0/src/gemsembler.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2024-05-17 09:11:58.000000 gemsembler-0.7.0/src/gemsembler.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-17 09:11:58.000000 gemsembler-0.7.0/src/gemsembler.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 09:11:59.018624 gemsembler-0.7.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    12691 2024-05-17 09:11:46.000000 gemsembler-0.7.0/tests/test_conversion.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-17 09:11:46.000000 gemsembler-0.7.0/tests/test_curation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2024-05-17 09:11:46.000000 gemsembler-0.7.0/tests/test_dbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2024-05-17 09:11:46.000000 gemsembler-0.7.0/tests/test_gathering.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-05-17 09:11:46.000000 gemsembler-0.7.0/tests/test_selection.py
```

### Comparing `gemsembler-0.6.5/LICENSE` & `gemsembler-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/PKG-INFO` & `gemsembler-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.5
+Version: 0.7.0
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.6.5/README.md` & `gemsembler-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/pyproject.toml` & `gemsembler-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gemsembler"
-version = "0.6.5"
+version = "0.7.0"
 description = "A tool for assembling and comparing several types of Genome-Scale Metabolic Models."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     { name = "Elena Matveishina", email = "elena.matveishina@embl.de" },
     { name = "Bartosz Bartmanski", email = "bartosz.bartmanski@embl.de" }
 ]
@@ -49,15 +49,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 namespaces = true
 where = ["src"]
 
 [tool.bumpver]
-current_version = "0.6.5"
+current_version = "0.7.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `gemsembler-0.6.5/src/gemsembler/__init__.py` & `gemsembler-0.7.0/src/gemsembler/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from importlib.resources import files
 from .anticreation import get_model_of_interest, get_models_with_all_confidence_levels
 from .creation import read_supermodel_from_pkl
 from .data import BU, LP
 from .gathering import GatheredModels, load_sbml_model
 
-__version__ = "0.6.5"
+__version__ = "0.7.0"
 
 lp_example = [
     dict(
         model_id="curated_LP",
         path_to_model=files(LP) / "LP_iLP728_revision_data_met_C_c.xml.gz",
         model_type="carveme",
         path_to_genome=files(LP) / "LP_protein_fasta.faa.gz",
```

### Comparing `gemsembler-0.6.5/src/gemsembler/__main__.py` & `gemsembler-0.7.0/src/gemsembler/__main__.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/anticreation.py` & `gemsembler-0.7.0/src/gemsembler/anticreation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from copy import deepcopy
 from pathlib import Path
 from pprint import pprint
 
 from cobra import Metabolite, Model, Reaction
 from cobra.io import validate_sbml_model, write_sbml_model
 
@@ -60,14 +61,15 @@
 
 def get_model_of_interest(
     supermodel: SuperModel,
     interest_level: str,
     output_name=None,
     gene_interest_level=None,
     biomass_interest_level=None,
+    simple_biomass_products=True,
     extend_zero_bounds=True,
     gapfill_transport=True,
     reactions_include: [NewElement] = None,
     reactions_exclude: [NewElement] = None,
 ):
     """ Creating COBRA model from supermodel based on specific level of interest for example core or union.
     Additionaly, some reactions"""
@@ -81,29 +83,27 @@
     elif interest_level in supermodel.reactions.comparison.keys():
         in_reactions = supermodel.reactions.comparison[interest_level].values()
     else:
         raise ValueError(
             f"Interest level {interest_level} is not determined yet. "
             f"Please run corresponding supermodel comparison first."
         )
-    if supermodel.reactions.assembly.get("Biomass") not in in_reactions:
-        in_reactions = list(in_reactions) + [
-            supermodel.reactions.assembly.get("Biomass")
-        ]
     if reactions_include:
         in_reactions = list(set(in_reactions) | set(reactions_include))
     else:
         reactions_include = []
     if reactions_exclude:
         in_reactions = list(set(in_reactions) - set(reactions_exclude))
+    if supermodel.reactions.assembly.get("Biomass") in in_reactions:
+        in_reactions = list(
+            set(list(in_reactions)) - {supermodel.reactions.assembly.get("Biomass")}
+        )
     for r in in_reactions:
         if r in reactions_include:
             interest_level_r = "assembly"
-        elif r.id == "Biomass":
-            interest_level_r = biomass_interest_level
         else:
             interest_level_r = interest_level
         if interest_level_r in supermodel.sources + ["assembly"]:
             r_upper_bound = r.upper_bound
             r_lower_bound = r.lower_bound
             r_metabolites = r.metabolites
         else:
@@ -143,14 +143,62 @@
         if r_gene_reaction_rule.get(gene_interest_level):
             out_reaction.gene_reaction_rule = r_gene_reaction_rule.get(
                 gene_interest_level
             )[0]
         else:
             out_reaction.gene_reaction_rule = ""
         outmodel.add_reactions([out_reaction])
+    biomass_reaction = Reaction("Biomass")
+    if biomass_interest_level in supermodel.sources + ["assembly"]:
+        biomass_reaction.upper_bound = supermodel.reactions.assembly[
+            "Biomass"
+        ].upper_bound.get(biomass_interest_level)[0]
+        biomass_reaction.lower_bound = supermodel.reactions.assembly[
+            "Biomass"
+        ].lower_bound.get(biomass_interest_level)[0]
+        bio_r_metabolites = supermodel.reactions.assembly["Biomass"].metabolites
+    else:
+        biomass_reaction.upper_bound = (
+            supermodel.reactions.assembly["Biomass"]
+            .upper_bound["comparison"]
+            .get(biomass_interest_level)[0]
+        )
+        biomass_reaction.lower_bound = (
+            supermodel.reactions.assembly["Biomass"]
+            .lower_bound["comparison"]
+            .get(biomass_interest_level)[0]
+        )
+        bio_r_metabolites = supermodel.reactions.assembly["Biomass"].metabolites[
+            "comparison"
+        ]
+    if simple_biomass_products:
+        biomass_prod_id = ["adp_c", "h_c", "pi_c", "ppi_c"]
+        for met, k in bio_r_metabolites.get(biomass_interest_level).items():
+            if met.id in biomass_prod_id:
+                biomass_prod_id.remove(met.id)
+                bio_met = Metabolite(
+                    met.id, name=met.name, compartment=met.compartments["assembly"][0]
+                )
+                biomass_reaction.add_metabolites({bio_met: k})
+            if k < 0:
+                bio_met = Metabolite(
+                    met.id, name=met.name, compartment=met.compartments["assembly"][0]
+                )
+                biomass_reaction.add_metabolites({bio_met: k})
+        if biomass_prod_id:
+            warnings.warn(
+                f"Some expected biomass products are not found: {' '.join(biomass_prod_id)}"
+            )
+    else:
+        for met, k in bio_r_metabolites.get(biomass_interest_level).items():
+            bio_met = Metabolite(
+                met.id, name=met.name, compartment=met.compartments["assembly"][0]
+            )
+            biomass_reaction.add_metabolites({bio_met: k})
+    outmodel.add_reactions([biomass_reaction])
     outmodel.objective = "Biomass"
     if gapfill_transport:
         gapfill_transport_r(outmodel, supermodel)
     if output_name is not None:
         write_sbml_model(outmodel, output_name)
         report = validate_sbml_model(filename=output_name)
         pprint(report)
@@ -158,14 +206,15 @@
 
 
 def get_models_with_all_confidence_levels(
     supermodel: SuperModel,
     output_dir=None,
     gene_interest_level=None,
     biomass_interest_level=None,
+    simple_biomass_products=True,
     extend_zero_bounds=True,
     gapfill_transport=True,
     reactions_include: [NewElement] = None,
     reactions_exclude: [NewElement] = None,
 ):
     output_models = {}
     confidence_levels = deepcopy(supermodel.sources)
@@ -181,14 +230,15 @@
             {
                 level: get_model_of_interest(
                     supermodel,
                     level,
                     output_name=output_dir_lev,
                     gene_interest_level=gene_interest_level,
                     biomass_interest_level=biomass_interest_level,
+                    simple_biomass_products=simple_biomass_products,
                     extend_zero_bounds=extend_zero_bounds,
                     gapfill_transport=gapfill_transport,
                     reactions_include=reactions_include,
                     reactions_exclude=reactions_exclude,
                 )
             }
         )
```

### Comparing `gemsembler-0.6.5/src/gemsembler/comparison.py` & `gemsembler-0.7.0/src/gemsembler/comparison.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/conversion.py` & `gemsembler-0.7.0/src/gemsembler/conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/creation.py` & `gemsembler-0.7.0/src/gemsembler/creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,33 +448,26 @@
                             )
 
     def _find_gene_and_gpr(
         self, connections: KnowledgeConnectingOldNew, gene_folder, do_notconv=False
     ):
         genes_to_add = defaultdict(list)
         for model_id in self.in_models["models_list"]:
-            genes_not_to_add = ["not_found"]
             old_rs = connections.get_old_rs(model_id, self.id, do_notconv)
             if not old_rs:
                 continue
             new_gpr_unite_r = []
             for oldr in old_rs:
                 if not oldr.genes:
                     continue
                 gene_convert = {}
                 for oldrg in oldr.genes:
                     pot_new_g_id = connections.get_new_gene_id(model_id, oldrg.id)
                     gene_convert.update({oldrg.id: pot_new_g_id})
-                    if (not do_notconv) & (
-                        connections.g_conversion_tables[model_id] is not None
-                    ):
-                        genes_not_to_add.append(oldrg.id)
-                    if pot_new_g_id not in genes_not_to_add:
-                        genes_to_add[model_id].append(pot_new_g_id)
-                        genes_not_to_add.append(pot_new_g_id)
+                    genes_to_add[model_id].append(pot_new_g_id)
                 old_gpr = oldr.gene_reaction_rule
                 new_gpr, mix_gpr = makeNewGPR(old_gpr, gene_convert)
                 if new_gpr:
                     new_gpr_unite_r.append(new_gpr)
                 self.gene_reaction_rule.get(model_id + "_mixed").append(mix_gpr)
             if len(new_gpr_unite_r) == 1:
                 self.gene_reaction_rule.get(model_id).append(new_gpr_unite_r[0])
@@ -817,16 +810,17 @@
             met._find_reactions(connection_knowledge)
         for r in self.reactions.assembly.values():
             r._find_reactants_products(connection_knowledge, "reactants")
             r._find_reactants_products(connection_knowledge, "products")
             r._find_metabolites(connection_knowledge)
             g_to_add = r._find_gene_and_gpr(connection_knowledge, gene_folder)
             for model_id, gene_ids in g_to_add.items():
-                for g_id in gene_ids:
-                    r.genes[model_id].append(self.genes.assembly[g_id])
+                for g_id in list(set(gene_ids)):
+                    if g_id in self.genes.assembly.keys():
+                        r.genes[model_id].append(self.genes.assembly[g_id])
         for gene in self.genes.assembly.values():
             gene._find_reactions(all_models_data, connection_knowledge)
         if not do_mix:
             for met in self.metabolites.notconverted.values():
                 met._find_reactions(connection_knowledge, do_notconv=True)
             for r in self.reactions.notconverted.values():
                 r._find_reactants_products(
@@ -836,15 +830,15 @@
                     connection_knowledge, "products", do_notconv=True
                 )
                 r._find_metabolites(connection_knowledge, do_notconv=True)
                 g_to_add = r._find_gene_and_gpr(
                     connection_knowledge, gene_folder, do_notconv=True
                 )
                 for model_id, gene_ids in g_to_add.items():
-                    for g_id in gene_ids:
+                    for g_id in list(set(gene_ids)):
                         if g_id in self.genes.notconverted.keys():
                             r.genes[model_id].append(self.genes.notconverted[g_id])
             for gene in self.genes.notconverted.values():
                 gene._find_reactions(all_models_data, connection_knowledge, True)
 
     def __get_additional_attributes(
         self,
```

### Comparing `gemsembler-0.6.5/src/gemsembler/curation.py` & `gemsembler-0.7.0/src/gemsembler/curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/BU/BU_agora.xml.gz` & `gemsembler-0.7.0/src/gemsembler/data/BU/BU_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/BU/BU_carveme_hom.xml.gz` & `gemsembler-0.7.0/src/gemsembler/data/BU/BU_carveme_hom.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/BU/BU_gapseq.xml.gz` & `gemsembler-0.7.0/src/gemsembler/data/BU/BU_gapseq.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/BU/BU_modelSEED.sbml.gz` & `gemsembler-0.7.0/src/gemsembler/data/BU/BU_modelSEED.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA1.xml.gz` & `gemsembler-0.7.0/src/gemsembler/data/LP/LP_CA1.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/LP/LP_CA2.xml.gz` & `gemsembler-0.7.0/src/gemsembler/data/LP/LP_CA2.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/LP/LP_MS2.sbml.gz` & `gemsembler-0.7.0/src/gemsembler/data/LP/LP_MS2.sbml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1.fasta.gz` & `gemsembler-0.7.0/src/gemsembler/data/LP/LP_WCFS1.fasta.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz` & `gemsembler-0.7.0/src/gemsembler/data/LP/LP_WCFS1_agora.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz` & `gemsembler-0.7.0/src/gemsembler/data/LP/LP_iLP728_revision_data_met_C_c.xml.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/data/LP/LP_protein_fasta.faa.gz` & `gemsembler-0.7.0/src/gemsembler/data/LP/LP_protein_fasta.faa.gz`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/dbs.py` & `gemsembler-0.7.0/src/gemsembler/dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/downstream.py` & `gemsembler-0.7.0/src/gemsembler/downstream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import operator
 import re
 import warnings
 from collections import defaultdict
-from copy import deepcopy
 from pathlib import Path
 
 import dill
 import pandas as pd
 from cobra.flux_analysis import pfba
 from .creation import SuperModel
 from .comparison import getCoreGPR
@@ -127,16 +126,17 @@
     output_name: str,
     additional_met=False,
     genes=True,
     and_as_solid=False,
     directed=True,
     met_not_int=None,
     n_letter=None,
-    wid=None,
-    hei=None,
+    wid=1920,
+    hei=1080,
+    size=25,
     write_table=True,
     yes_range=1,
     no_range=1,
 ):
     glycolysis = {
         "HEX1": [("glc__D_c", "g6p_c")],
         "PGI": [("g6p_c", "f6p_c")],
@@ -156,14 +156,15 @@
         genes,
         and_as_solid,
         directed,
         met_not_int,
         n_letter,
         wid,
         hei,
+        size,
     )
     if write_table:
         t_name = re.sub(".html$", ".tsv", output_name)
         t = table_reactions_confidence(
             supermodel,
             t_name,
             list(glycolysis.keys()),
@@ -182,16 +183,17 @@
     output_name: str,
     additional_met=False,
     genes=True,
     and_as_solid=False,
     directed=True,
     met_not_int=None,
     n_letter=None,
-    wid=None,
-    hei=None,
+    wid=1920,
+    hei=1080,
+    size=25,
     write_table=True,
     yes_range=1,
     no_range=1,
 ):
     tca = {
         "PYK": [("pep_c", "pyr_c")],
         "PPC": [("pep_c", "oaa_c")],
@@ -231,14 +233,15 @@
         genes,
         and_as_solid,
         directed,
         met_not_int,
         n_letter,
         wid,
         hei,
+        size,
     )
     if write_table:
         t_name = re.sub(".html$", ".tsv", output_name)
         t = table_reactions_confidence(
             supermodel,
             t_name,
             list(tca.keys()),
@@ -257,16 +260,17 @@
     output_name: str,
     additional_met=False,
     genes=True,
     and_as_solid=False,
     directed=True,
     met_not_int=None,
     n_letter=None,
-    wid=None,
-    hei=None,
+    wid=1920,
+    hei=1080,
+    size=25,
     write_table=True,
     yes_range=1,
     no_range=1,
 ):
     pentose_phosphate_pathway = {
         "G6PBDH": [("g6p_B_c", "6pgl_c")],
         "G6PDH2r": [("g6p_c", "6pgl_c")],
@@ -288,14 +292,15 @@
         genes,
         and_as_solid,
         directed,
         met_not_int,
         n_letter,
         wid,
         hei,
+        size,
     )
     if write_table:
         t_name = re.sub(".html$", ".tsv", output_name)
         t = table_reactions_confidence(
             supermodel,
             t_name,
             list(pentose_phosphate_pathway.keys()),
```

### Comparing `gemsembler-0.6.5/src/gemsembler/drawing.py` & `gemsembler-0.7.0/src/gemsembler/drawing.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/gathering.py` & `gemsembler-0.7.0/src/gemsembler/gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/genes.py` & `gemsembler-0.7.0/src/gemsembler/genes.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/pathsfinding.py` & `gemsembler-0.7.0/src/gemsembler/pathsfinding.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/periplasmic.py` & `gemsembler-0.7.0/src/gemsembler/periplasmic.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/selection.py` & `gemsembler-0.7.0/src/gemsembler/selection.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler/structural.py` & `gemsembler-0.7.0/src/gemsembler/structural.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/src/gemsembler.egg-info/PKG-INFO` & `gemsembler-0.7.0/src/gemsembler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemsembler
-Version: 0.6.5
+Version: 0.7.0
 Summary: A tool for assembling and comparing several types of Genome-Scale Metabolic Models.
 Author-email: Elena Matveishina <elena.matveishina@embl.de>, Bartosz Bartmanski <bartosz.bartmanski@embl.de>
 License: MIT License
         
         Copyright (c) 2024 Zimmermann-Kogadeeva Group
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `gemsembler-0.6.5/src/gemsembler.egg-info/SOURCES.txt` & `gemsembler-0.7.0/src/gemsembler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/tests/test_conversion.py` & `gemsembler-0.7.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/tests/test_curation.py` & `gemsembler-0.7.0/tests/test_curation.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/tests/test_dbs.py` & `gemsembler-0.7.0/tests/test_dbs.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/tests/test_gathering.py` & `gemsembler-0.7.0/tests/test_gathering.py`

 * *Files identical despite different names*

### Comparing `gemsembler-0.6.5/tests/test_selection.py` & `gemsembler-0.7.0/tests/test_selection.py`

 * *Files identical despite different names*

