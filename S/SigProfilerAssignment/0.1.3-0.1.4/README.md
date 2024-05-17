# Comparing `tmp/SigProfilerAssignment-0.1.3.tar.gz` & `tmp/SigProfilerAssignment-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SigProfilerAssignment-0.1.3.tar", last modified: Fri Feb 16 21:21:45 2024, max compression
+gzip compressed data, was "SigProfilerAssignment-0.1.4.tar", last modified: Thu Mar  7 20:09:54 2024, max compression
```

## Comparing `SigProfilerAssignment-0.1.3.tar` & `SigProfilerAssignment-0.1.4.tar`

### file list

```diff
@@ -1,202 +1,203 @@
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.968467 SigProfilerAssignment-0.1.3/
--rw-r--r--   0 mbarnes    (501) staff       (20)     1342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/LICENSE.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)      719 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/MANIFEST.in
--rw-r--r--   0 mbarnes    (501) staff       (20)    12700 2024-02-16 21:21:45.967912 SigProfilerAssignment-0.1.3/PKG-INFO
--rw-r--r--   0 mbarnes    (501) staff       (20)    11906 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/README.md
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.799848 SigProfilerAssignment-0.1.3/SigProfilerAssignment/
--rw-r--r--   0 mbarnes    (501) staff       (20)     4610 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/Analyzer.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.809192 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/
--rw-r--r--   0 mbarnes    (501) staff       (20)    30371 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    17348 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16417 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16601 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16771 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    16851 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    17285 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.812645 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/
--rw-r--r--   0 mbarnes    (501) staff       (20)    12535 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png
--rw-r--r--   0 mbarnes    (501) staff       (20)      165 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/CREDIT.md
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.813499 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/
--rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf
--rw-r--r--   0 mbarnes    (501) staff       (20)   267633 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py
--rw-r--r--   0 mbarnes    (501) staff       (20)       50 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/__init__.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.822314 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     3342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
--rw-r--r--   0 mbarnes    (501) staff       (20)      803 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/CNV_features.tsv
--rw-r--r--   0 mbarnes    (501) staff       (20)    15995 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/CNV_signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     1641 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/CN_classes_dictionary.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   128402 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.792935 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.853366 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/
--rw-r--r--   0 mbarnes    (501) staff       (20)    14328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39321 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt
--rwxr-xr-x   0 mbarnes    (501) staff       (20)    36586 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53285 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   137506 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138652 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   109467 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   148966 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    18940 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17759 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17844 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    29808 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   151235 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153270 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    13831 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    18328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    22118 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    96398 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166615 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17757 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17857 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    28686 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt
--rwxr-xr-x   0 mbarnes    (501) staff       (20)   128501 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129752 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.875910 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39244 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39286 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53205 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53265 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138534 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138665 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150027 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150132 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17825 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17827 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153188 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153263 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    33984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31738 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178722 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166497 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     4375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17829 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129685 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129793 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.901393 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39299 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53208 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53279 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138625 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138642 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150107 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150127 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17819 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153243 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    33977 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31764 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178725 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166529 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17818 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129718 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129754 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.926272 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39310 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53293 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138548 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138590 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150036 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150053 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153159 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153192 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    34014 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31766 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178728 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166558 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129655 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129717 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.953001 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/
--rw-r--r--   0 mbarnes    (501) staff       (20)    39230 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    39249 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53187 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138524 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   138634 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150001 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   150098 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   153225 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    33996 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    31745 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   178687 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   166478 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17840 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    17851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129663 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   129739 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)   380152 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx
--rw-r--r--   0 mbarnes    (501) staff       (20)     7124 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Samples.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     3851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/csvexample.csv
--rwxr-xr-x   0 mbarnes    (501) staff       (20)     8338 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv
--rw-r--r--   0 mbarnes    (501) staff       (20)    16970 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv
--rwxr-xr-x   0 mbarnes    (501) staff       (20)    57422 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.794463 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.953705 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/cnv_input/
--rw-r--r--   0 mbarnes    (501) staff       (20)   381521 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.962051 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/
--rw-r--r--   0 mbarnes    (501) staff       (20)     2375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     5496 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     6019 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     6848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     1837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)    12790 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     3937 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     2085 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     2359 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)     1163 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.966275 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/
--rw-r--r--   0 mbarnes    (501) staff       (20)    42134 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   144692 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   132516 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   243267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)   144314 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf
--rw-r--r--   0 mbarnes    (501) staff       (20)    63575 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/decompose_subroutines.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    40644 2024-02-16 21:21:13.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/decomposition.py
--rw-r--r--   0 mbarnes    (501) staff       (20)    36157 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/single_sample.py
--rw-r--r--   0 mbarnes    (501) staff       (20)      167 2024-02-16 21:21:45.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment/version.py
-drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-02-16 21:21:45.966999 SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/
--rw-r--r--   0 mbarnes    (501) staff       (20)    12700 2024-02-16 21:21:45.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/PKG-INFO
--rw-r--r--   0 mbarnes    (501) staff       (20)    13369 2024-02-16 21:21:45.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/SOURCES.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-02-16 21:21:45.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/dependency_links.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-01-24 20:17:52.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/not-zip-safe
--rw-r--r--   0 mbarnes    (501) staff       (20)      253 2024-02-16 21:21:45.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/requires.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)       22 2024-02-16 21:21:45.000000 SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/top_level.txt
--rw-r--r--   0 mbarnes    (501) staff       (20)       38 2024-02-16 21:21:45.968587 SigProfilerAssignment-0.1.3/setup.cfg
--rw-r--r--   0 mbarnes    (501) staff       (20)     1586 2024-02-16 21:21:13.000000 SigProfilerAssignment-0.1.3/setup.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.572787 SigProfilerAssignment-0.1.4/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/LICENSE.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)      719 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/MANIFEST.in
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12252 2024-03-07 20:09:54.572382 SigProfilerAssignment-0.1.4/PKG-INFO
+-rw-r--r--   0 mbarnes    (501) staff       (20)    11906 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/README.md
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.735602 SigProfilerAssignment-0.1.4/SigProfilerAssignment/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     4610 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/Analyzer.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.766089 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    32944 2024-03-07 20:09:36.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17348 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16417 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16601 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16771 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16851 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17285 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17349 2024-03-07 20:09:36.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SV32.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.770161 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12535 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png
+-rw-r--r--   0 mbarnes    (501) staff       (20)      165 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/CREDIT.md
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.773676 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/
+-rw-r--r--   0 mbarnes    (501) staff       (20)   750984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   267633 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)       50 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/__init__.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.920953 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)     3342 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
+-rw-r--r--   0 mbarnes    (501) staff       (20)      803 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/CNV_features.tsv
+-rw-r--r--   0 mbarnes    (501) staff       (20)    15995 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/CNV_signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1641 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/CN_classes_dictionary.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   128402 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.720314 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.050047 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    14328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39321 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)    36586 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53285 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   137506 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138652 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    29489 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   109467 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   148966 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    18940 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17759 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17844 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    29808 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   151235 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153270 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    13831 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    18328 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31758 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    22118 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    96398 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166615 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17757 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17857 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    28686 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)   128501 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129752 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.175799 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39244 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39286 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53205 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53265 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138534 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138665 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17833 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17826 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150027 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150132 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17825 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17827 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153188 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153263 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    33984 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31738 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178722 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166497 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     4375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17829 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129685 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129793 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.293168 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39299 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53208 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53279 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138625 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138642 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17834 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17816 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150107 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150127 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17819 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153243 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    33977 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31764 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178725 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166529 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17836 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17818 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129718 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129754 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.401508 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39213 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39310 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53293 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138548 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138590 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17839 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150036 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150053 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17843 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153159 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153192 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    34014 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31766 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178728 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166558 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17842 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129655 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129717 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.514091 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39230 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    39249 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53187 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    53199 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138524 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   138634 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17837 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17847 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150001 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   150098 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17838 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153133 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   153225 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    33996 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    31745 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   178687 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   166478 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17840 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    17851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129663 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   129739 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)   380152 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx
+-rw-r--r--   0 mbarnes    (501) staff       (20)     7124 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Samples.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3851 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/csvexample.csv
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)     8338 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv
+-rw-r--r--   0 mbarnes    (501) staff       (20)    16970 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv
+-rwxr-xr-x   0 mbarnes    (501) staff       (20)    57422 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.721818 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.526642 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/cnv_input/
+-rw-r--r--   0 mbarnes    (501) staff       (20)   381521 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.537702 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/
+-rw-r--r--   0 mbarnes    (501) staff       (20)     2375 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     5496 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6019 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     6848 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1864 2024-03-07 20:09:36.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12790 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     3937 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     2085 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     2359 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1163 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:54.571610 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    42134 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   144692 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   132516 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   243267 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)   144314 2024-01-24 17:38:12.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf
+-rw-r--r--   0 mbarnes    (501) staff       (20)    63678 2024-03-07 20:09:36.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/decompose_subroutines.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    40644 2024-02-16 21:21:13.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/decomposition.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)    36157 2024-01-25 18:13:15.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/single_sample.py
+-rw-r--r--   0 mbarnes    (501) staff       (20)      164 2024-03-07 20:09:53.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment/version.py
+drwxr-xr-x   0 mbarnes    (501) staff       (20)        0 2024-03-07 20:09:53.739983 SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/
+-rw-r--r--   0 mbarnes    (501) staff       (20)    12252 2024-03-07 20:09:53.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/PKG-INFO
+-rw-r--r--   0 mbarnes    (501) staff       (20)    13436 2024-03-07 20:09:53.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/SOURCES.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-03-07 20:09:53.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/dependency_links.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)        1 2024-01-24 20:17:52.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/not-zip-safe
+-rw-r--r--   0 mbarnes    (501) staff       (20)      253 2024-03-07 20:09:53.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/requires.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)       22 2024-03-07 20:09:53.000000 SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/top_level.txt
+-rw-r--r--   0 mbarnes    (501) staff       (20)       38 2024-03-07 20:09:54.572878 SigProfilerAssignment-0.1.4/setup.cfg
+-rw-r--r--   0 mbarnes    (501) staff       (20)     1583 2024-03-07 20:09:36.000000 SigProfilerAssignment-0.1.4/setup.py
```

### Comparing `SigProfilerAssignment-0.1.3/LICENSE.txt` & `SigProfilerAssignment-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/MANIFEST.in` & `SigProfilerAssignment-0.1.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/PKG-INFO` & `SigProfilerAssignment-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 Metadata-Version: 2.1
 Name: SigProfilerAssignment
-Version: 0.1.3
+Version: 0.1.4
 Summary: Mutational signatures attribution and decomposition tool
 Home-page: https://github.com/AlexandrovLab/SigProfilerAssignment.git
 Author: Raviteja Vangara
 Author-email: rvangara@health.ucsd.edu
 License: UCSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: scipy>=1.6.3
-Requires-Dist: numpy>=1.21.2
-Requires-Dist: pandas<2.0.0,>=1.2.4
-Requires-Dist: SigProfilerMatrixGenerator>=1.2.17
-Requires-Dist: sigProfilerPlotting>=1.3.20
-Requires-Dist: statsmodels>=0.9.0
-Requires-Dist: scikit-learn>=0.24.2
-Requires-Dist: psutil>=5.6.1
-Requires-Dist: reportlab>=3.5.42
-Requires-Dist: PyPDF2>=3.0.0
-Requires-Dist: alive_progress>=2.4.1
-Requires-Dist: pdf2image>=1.16.0
-Requires-Dist: PyMuPDF>=1.21.0
 
 [![Docs](https://img.shields.io/badge/docs-latest-blue.svg)](https://osf.io/mz79v/wiki/home/) 
 [![License](https://img.shields.io/badge/License-BSD\%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Build Status](https://api.travis-ci.com/AlexandrovLab/SigProfilerAssignment.svg?branch=main)](https://app.travis-ci.com/AlexandrovLab/SigProfilerAssignment)
 
 <img src="SigProfilerAssignment/figures/SigProfilerAssignment.png" alt="drawing" width="1000"/>
```

### Comparing `SigProfilerAssignment-0.1.3/README.md` & `SigProfilerAssignment-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/Analyzer.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/Analyzer.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,90 +22,97 @@
 import numpy as np
 import scipy.stats
 import sigProfilerPlotting as sigPlt
 import shutil
 import SigProfilerAssignment
 import SigProfilerAssignment.DecompositionPlots
 from SigProfilerAssignment.DecompositionPlots import SigProfilerPlottingMatrix as mPlt
-from SigProfilerAssignment.DecompositionPlots import PlotDecomposition_SBS96 as spd_96
-from SigProfilerAssignment.DecompositionPlots import PlotDecomposition_SBS288 as spd_288
 from SigProfilerAssignment.DecompositionPlots import (
+    PlotDecomposition_SBS96 as spd_96,
+    PlotDecomposition_SBS288 as spd_288,
     PlotDecomposition_SBS1536 as spd_1536,
+    PlotDecomposition_DBS78 as spd_78,
+    PlotDecomposition_ID83 as spd_83,
+    PlotDecomposition_CNV48 as cnv_48,
+    PlotDecomposition_SV32 as sv_32,
 )
-from SigProfilerAssignment.DecompositionPlots import PlotDecomposition_DBS78 as spd_78
-from SigProfilerAssignment.DecompositionPlots import PlotDecomposition_ID83 as spd_83
-from SigProfilerAssignment.DecompositionPlots import PlotDecomposition_CNV48 as cnv_48
 from SigProfilerAssignment import decompose_subroutines as sub
 
 # imports for working with plots in memory
 import io
 from PIL import Image
 from reportlab.lib.utils import ImageReader
 import json
 import base64
 
+
 # Global Variables
 SBS_CONTEXTS = ["6", "24", "96", "288", "384", "1536", "6144"]
 DBS_CONTEXTS = ["78", "186", "1248", "2976"]
 ID_CONTEXTS = ["28", "83", "415"]
 CNV_CONTEXTS = ["48"]
+SV_CONTEXTS = ["32"]
 MTYPE_OPTIONS = [
     "6",
     "24",
     "96",
     "384",
     "1536",
     "6144",
     "28",
     "83",
     "415",
     "78",
     "186",
     "1248",
     "2976",
+    "32",
 ]
 DECOMPOSITION_PATH = SigProfilerAssignment.DecompositionPlots.__path__[0]
 REFSIG_PATH = os.path.join(
     SigProfilerAssignment.__path__[0], "data/Reference_Signatures"
 )
 TEMPLATE_PATH = os.path.join(DECOMPOSITION_PATH, "CosmicTemplates")
 
-
 # Remove templates so that they can be rebuilt
 def remove_cosmic_templates():
     if not os.path.exists(TEMPLATE_PATH):
         print("No files are installed at: ", TEMPLATE_PATH)
     try:
         shutil.rmtree(TEMPLATE_PATH)
     except OSError as e:
         print("Error: %s : %s" % (TEMPLATE_PATH, e.strerror))
 
 
 # Create a set of serialized JSON reference signature plots for fast loading
 def install_cosmic_plots(
     context_type="96", genome_build="GRCh37", cosmic_version="3.4", exome=False
 ):
+
     if not os.path.exists(TEMPLATE_PATH):
         os.mkdir(TEMPLATE_PATH)
 
-    # determine if context is from SBS, ID, DBS, or CNV
+    # determine if context is from SBS, ID, DBS, CNV or SV
     context_type_str = ""
     if context_type in SBS_CONTEXTS:
         context_type_str = "SBS"
         # the mtype of the cosmic reference signatures to be plotted
         cosmic_mtype = "96"
     elif context_type in DBS_CONTEXTS:
         context_type_str = "DBS"
         cosmic_mtype = "78"
     elif context_type in ID_CONTEXTS:
         context_type_str = "ID"
         cosmic_mtype = "83"
     elif context_type in CNV_CONTEXTS:
         context_type_str = "CNV"
         cosmic_mtype = "48"
+    elif context_type in SV_CONTEXTS:
+        context_type_str = "SV"
+        cosmic_mtype = "32"
     else:
         raise ValueError("ERROR: context", context_type, "not in context lists.")
 
     # if exome is true, append _exome to end of file name
     exome_str = ""
     if exome:
         exome_str = "_exome"
@@ -134,14 +141,28 @@
     # ID signatures exome=False, genome_build=GRCh37
     if context_type in ID_CONTEXTS:
         cosmic_file_name = "COSMIC_v" + str(cosmic_version) + "_ID_GRCh37.txt"
         json_file_name = "COSMIC_v" + str(cosmic_version) + "_ID_GRCh37.json"
         genome_build = "GRCh37"
         exome_str = ""
 
+    # CNV signatures exome=False, genome_build=GRCh37
+    if context_type in CNV_CONTEXTS:
+        cosmic_file_name = "COSMIC_v" + str(cosmic_version) + "_CN_GRCh37.txt"
+        json_file_name = "COSMIC_v" + str(cosmic_version) + "_CN_GRCh37.json"
+        genome_build = "GRCh37"
+        exome_str = ""
+
+    # SV signatures exome=False, genome_build=GRCh37
+    if context_type in SV_CONTEXTS:
+        cosmic_file_name = "COSMIC_v" + str(cosmic_version) + "_SV_GRCh38.txt"
+        json_file_name = "COSMIC_v" + str(cosmic_version) + "_SV_GRCh38.json"
+        genome_build = "GRCh38"
+        exome_str = ""
+
     # Load cosmic plots if they exist
     filename = os.path.join(TEMPLATE_PATH, json_file_name)
     if os.path.exists(filename):
         cosmic_buff_bytes = json.load(open(filename))
         cosmic_buff_plots = {}
         # Read from JSON, decode, and convert to bytesIO
         for tmp_plots in cosmic_buff_bytes.keys():
@@ -161,15 +182,14 @@
             + "_"
             + context_type_str
             + "_"
             + genome_build
             + exome_str,
             "now...",
         )
-
         # Create the respective plots
         if context_type_str == "SBS":
             cosmic_buff_plots = sigPlt.plotSBS(
                 cosmic_file_path,
                 "buffer",
                 "buffer",
                 cosmic_mtype,
@@ -191,14 +211,33 @@
                 cosmic_file_path,
                 "buffer",
                 "buffer",
                 cosmic_mtype,
                 percentage=True,
                 savefig_format="PIL_Image",
             )
+        elif context_type_str == "CNV":
+            cosmic_buff_plots = sigPlt.plotCNV(
+                cosmic_file_path,
+                "buffer",
+                "buffer",
+                percentage=True,
+                aggregate=False,
+                read_from_file=False,
+                savefig_format="PIL_Image",
+            )
+        elif context_type_str == "SV":
+            cosmic_buff_plots = sigPlt.plotSV(
+                cosmic_file_path,
+                "buffer",
+                "buffer",
+                percentage=True,
+                aggregate=False,
+                savefig_format="PIL_Image",
+            )
 
         # Process the plots to be stored in JSON file
         cosmic_img_dict = {}
         for tmp_plot in cosmic_buff_plots.keys():
             # Convert to bytesIO and encode to base64
             plot_bytes = io.BytesIO()
             seek_start = cosmic_buff_plots[tmp_plot].seek(0)
@@ -409,16 +448,41 @@
             aggregate=False,
             read_from_file=False,
             savefig_format="PIL_Image",
         )
     return denovo_plots, basis_plots
 
 
+def genSV_pngs(denovo_mtx, basis_mtx, output_path, project, mtype):
+    denovo_plots = dict()
+    basis_plots = dict()
+    denovo_plots = sigPlt.plotSV(
+        denovo_mtx,
+        output_path,
+        project,
+        percentage=True,
+        aggregate=False,
+        savefig_format="PIL_Image",
+    )
+
+    if basis_mtx is not None:
+        basis_plots = sigPlt.plotSV(
+            basis_mtx,
+            output_path,
+            project,
+            percentage=True,
+            aggregate=False,
+            savefig_format="PIL_Image",
+        )
+    return denovo_plots, basis_plots
+
+
 # signames, weights
 def gen_sub_plots(denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp):
+
     # Make output directory
     if not os.path.exists(output_path):
         os.makedirs(output_path)
 
     if mtype in SBS_CONTEXTS:
         denovo_plots, basis_plots = genSBS_pngs(
             denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp
@@ -438,14 +502,19 @@
         return denovo_plots, basis_plots
 
     elif mtype in CNV_CONTEXTS:
         denovo_plots, basis_plots = genCNV_pngs(
             denovo_mtx, basis_mtx, output_path, project, mtype
         )
         return denovo_plots, basis_plots
+    elif mtype in SV_CONTEXTS:
+        denovo_plots, basis_plots = genSV_pngs(
+            denovo_mtx, basis_mtx, output_path, project, mtype
+        )
+        return denovo_plots, basis_plots
 
     else:
         print("ERROR: mtype is " + mtype + " and is not yet supported.")
 
 
 # generate the plot for the reconstruction
 def gen_reconstructed_png_percent(
@@ -506,14 +575,23 @@
             output_path,
             "reconstruction_" + project,
             percentage=True,
             aggregate=False,
             read_from_file=False,
             savefig_format="PIL_Image",
         )
+    elif mtype in SV_CONTEXTS:
+        reconstruction_plot = sigPlt.plotSV(
+            reconstruction_mtx,
+            output_path,
+            "reconstruction_" + project,
+            percentage=True,
+            aggregate=False,
+            savefig_format="PIL_Image",
+        )
     else:
         print("ERROR: mtype is " + mtype + " and is not yet supported.")
 
     return reconstruction_mtx, reconstruction_plot
 
 
 # generate the plot for the reconstruction
@@ -587,14 +665,24 @@
             output_path,
             "reconstruction_" + project,
             percentage=True,
             aggregate=False,
             read_from_file=False,
             savefig_format="PIL_Image",
         )
+    elif mtype in SV_CONTEXTS:
+        reconstruction_plot = sigPlt.plotSV(
+            reconstruction_mtx,
+            output_path,
+            "reconstruction_" + project,
+            percentage=True,
+            aggregate=False,
+            read_from_file=False,
+            savefig_format="PIL_Image",
+        )
     else:
         print("ERROR: mtype is " + mtype + " and is not yet supported.")
 
     return reconstruction_mtx, reconstruction_plot
 
 
 def gen_decomposition(
@@ -608,14 +696,15 @@
     basis_plots_dict,
     reconstruction_plot_dict,
     reconstruction=False,
     statistics=None,
     cosmic_version=None,
     custom_text=None,
 ):
+
     """
     Generate the correct plot based on mtype.
 
     Parameters:
     ----------
     denovo_name: 				(String) 			Name of denovo signature
     basis_names: 				(List of Strings) 	Names of basis signatures
@@ -740,14 +829,30 @@
             reconstruction_plot_dict,
             reconstruction,
             statistics,
             cosmic_version,
             custom_text,
         )
         return byte_plot
+    elif mtype == "32":
+        byte_plot = sv_32.gen_decomposition(
+            denovo_name,
+            basis_names,
+            weights,
+            output_path,
+            project,
+            denovo_plots_dict,
+            basis_plots_dict,
+            reconstruction_plot_dict,
+            reconstruction,
+            statistics,
+            cosmic_version,
+            custom_text,
+        )
+        return byte_plot
 
 
 def run_PlotDecomposition(
     denovo_mtx,
     denovo_name,
     basis_mtx,
     basis_names,
@@ -769,16 +874,15 @@
 
     denovo_mtx: Pandas Dataframe. This format represents the catalog of mutations seperated by tab.
 
     denovo_name: String. The name of the one sample in denovo_mtx to decompose.
 
     basis_mtx: Pandas Dataframe. This format represents the catalog of mutations seperated by tab.
 
-    basis_names: List of Strings. The names of the samples in denovo_mtx that
-    the denovo_name sample from denovo_mtx is decomposed into.
+    basis_names: List of Strings. The names of the samples in denovo_mtx that the denovo_name sample from denovo_mtx is decomposed into.
     ie. basis_names=["SBS1", "SBS5", "SBS15", "SBS20"]
 
     weights: List of Strings. The percentile weight corresponding to each basis
     in basis_names. Refer to example function call below for more detail.
     ie. weights=["11.58%", "42.38%", "16.46%", "29.58%"]
 
     output_path: String. Path to where to store the output.
@@ -792,42 +896,33 @@
     custom_text: String. A custom message displayed on decomposition plot.
 
     Returns:
     -------
     None.
     """
     # Create the denovo plots and load basis plots
-    if mtype != "48":
-        denovo_plots_dict = gen_sub_plots(
-            denovo_mtx, None, output_path, project, mtype, ss_decomp=False
-        )
-        denovo_plots_dict = denovo_plots_dict[0]
-    else:
-        # cnv basis plots need to be generated and not loaded
-        denovo_plots_dict, basis_plots_dict = gen_sub_plots(
-            denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp=False
-        )
-    # Create the matrix and plot for the reconstructed matrix
+    denovo_plots_dict, basis_plots_dict = gen_sub_plots(
+        denovo_mtx, basis_mtx, output_path, project, mtype, ss_decomp=False
+    )
     reconstructed_mtx, reconstruction_plot_dict = gen_reconstructed_png_percent(
         denovo_name, basis_mtx, basis_names, weights, output_path, project, mtype
     )
     # Create a subset matrix with the present signatures
     present_sigs = np.array(basis_mtx[basis_names])
     reconstructed_mtx = np.dot(present_sigs, nonzero_exposures)
     # Convert dictionary of bytes to dictionary of images
     denovo_plots_dict = convert_to_imgReaderDict(denovo_plots_dict)
     # Load in the COSMIC plots
-    if mtype != "48":
-        basis_plots_dict = install_cosmic_plots(
-            context_type=mtype,
-            genome_build=genome_build,
-            cosmic_version=cosmic_version,
-            exome=exome,
-        )
-        basis_plots_dict = {key: basis_plots_dict[key] for key in basis_names}
+    basis_plots_dict = install_cosmic_plots(
+        context_type=mtype,
+        genome_build=genome_build,
+        cosmic_version=cosmic_version,
+        exome=exome,
+    )
+    basis_plots_dict = {key: basis_plots_dict[key] for key in basis_names}
     basis_plots_dict = convert_to_imgReaderDict(basis_plots_dict)
     # Generate the reconstruction plot
     reconstruction_plot_dict = convert_to_imgReaderDict(reconstruction_plot_dict)
     # Get the reconstruction statistics
     statistics = calculate_similarities(denovo_mtx, denovo_name, reconstructed_mtx)
     # Return the decomposition plot as a byte array
     byte_plot = gen_decomposition(
```

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/21_breast_WGS_substitutions.mat`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/CNV_features.tsv` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/CNV_features.tsv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/CNV_signatures.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/CNV_signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/CN_classes_dictionary.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/CN_classes_dictionary.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/DBS_signatures_genome_builds.xlsx`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v1_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v2_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.1_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS288_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.2_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_CN_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.3_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_CN_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3.4_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_DBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_ID_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh37/COSMIC_v3_SBS_GRCh37_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v1_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v2_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.1_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.2_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.3_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3.4_SV_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_DBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/GRCh38/COSMIC_v3_SBS_GRCh38_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v1_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v2_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.1_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.2_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.3_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3.4_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_DBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm10/COSMIC_v3_SBS_mm10_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v1_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v2_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.1_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.2_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.3_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3.4_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_DBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/mm9/COSMIC_v3_SBS_mm9_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v1_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v2_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.1_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.2_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.3_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3.4_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_DBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Reference_Signatures/rn6/COSMIC_v3_SBS_rn6_exome.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/SBS_signatures_genome_builds.xlsx`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/Samples.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/Samples.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/csvexample.csv` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/csvexample.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/sigProfiler_DBS_signatures.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/sigProfiler_ID_signatures.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/sigProfiler_SBS_signatures_2018_03_28.csv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/cnv_input/all.breast.ascat.summary.sample.tsv`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/CNV48_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/DBS78_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/ID83_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/SBS96_S3_Signatures.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/SV32_S3_Signatures.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-MutationType	0	1	2
-clustered_del_1-10Kb	0.00591623	0.00000119	0.00003543
-clustered_del_10-100Kb	0.00754999	0.00000101	0.00599576
-clustered_del_100Kb-1Mb	0.01723822	0.00000066	0.02294156
-clustered_del_1Mb-10Mb	0.02895137	0.00000094	0.03714988
-clustered_del_>10Mb	0.02151931	0.00000096	0.00003624
-clustered_tds_1-10Kb	0.00138182	0.00000152	0.00000141
-clustered_tds_10-100Kb	0.00363530	0.00277485	0.00528629
-clustered_tds_100Kb-1Mb	0.00751767	0.00000075	0.03179513
-clustered_tds_1Mb-10Mb	0.02024984	0.00000084	0.00387149
-clustered_tds_>10Mb	0.01728936	0.00000073	0.01635656
-clustered_inv_1-10Kb	0.01599352	0.00000107	0.06660425
-clustered_inv_10-100Kb	0.01473596	0.00000077	0.04657534
-clustered_inv_100Kb-1Mb	0.02195676	0.00000093	0.07297037
-clustered_inv_1Mb-10Mb	0.05721262	0.00000059	0.02610903
-clustered_inv_>10Mb	0.03575116	0.00000068	0.01932889
-clustered_trans	0.31742983	0.00000000	0.11931097
-non-clustered_del_1-10Kb	0.01235744	0.10028469	0.03929744
-non-clustered_del_10-100Kb	0.01642868	0.08869502	0.06827200
-non-clustered_del_100Kb-1Mb	0.04314541	0.02361266	0.01049556
-non-clustered_del_1Mb-10Mb	0.02307427	0.02360570	0.02154467
-non-clustered_del_>10Mb	0.01346200	0.02884193	0.02113914
-non-clustered_tds_1-10Kb	0.00098514	0.00559656	0.00000127
-non-clustered_tds_10-100Kb	0.00011906	0.01948073	0.02651685
-non-clustered_tds_100Kb-1Mb	0.01252569	0.03134159	0.00405312
-non-clustered_tds_1Mb-10Mb	0.02074378	0.00844506	0.01205615
-non-clustered_tds_>10Mb	0.01391367	0.02407620	0.01162608
-non-clustered_inv_1-10Kb	0.01775605	0.04985384	0.05993695
-non-clustered_inv_10-100Kb	0.00886354	0.01882036	0.02325057
-non-clustered_inv_100Kb-1Mb	0.02501168	0.04010485	0.02112356
-non-clustered_inv_1Mb-10Mb	0.03438851	0.04624524	0.01434552
-non-clustered_inv_>10Mb	0.04593804	0.10010973	0.00383835
-non-clustered_trans	0.11695809	0.38809832	0.18813424
+MutationType	SV32A	SV32B	SV32C
+clustered_del_1-10Kb	0.00591623	0.00000119	0.00003543
+clustered_del_10-100Kb	0.00754999	0.00000101	0.00599576
+clustered_del_100Kb-1Mb	0.01723822	0.00000066	0.02294156
+clustered_del_1Mb-10Mb	0.02895137	0.00000094	0.03714988
+clustered_del_>10Mb	0.02151931	0.00000096	0.00003624
+clustered_tds_1-10Kb	0.00138182	0.00000152	0.00000141
+clustered_tds_10-100Kb	0.0036353	0.00277485	0.00528629
+clustered_tds_100Kb-1Mb	0.00751767	0.00000075	0.03179513
+clustered_tds_1Mb-10Mb	0.02024984	0.00000084	0.00387149
+clustered_tds_>10Mb	0.01728936	0.00000073	0.01635656
+clustered_inv_1-10Kb	0.01599352	0.00000107	0.06660425
+clustered_inv_10-100Kb	0.01473596	0.00000077	0.04657534
+clustered_inv_100Kb-1Mb	0.02195676	0.00000093	0.07297037
+clustered_inv_1Mb-10Mb	0.05721262	0.00000059	0.02610903
+clustered_inv_>10Mb	0.03575116	0.00000068	0.01932889
+clustered_trans	0.31742983	0	0.11931097
+non-clustered_del_1-10Kb	0.01235744	0.10028469	0.03929744
+non-clustered_del_10-100Kb	0.01642868	0.08869502	0.068272
+non-clustered_del_100Kb-1Mb	0.04314541	0.02361266	0.01049556
+non-clustered_del_1Mb-10Mb	0.02307427	0.0236057	0.02154467
+non-clustered_del_>10Mb	0.013462	0.02884193	0.02113914
+non-clustered_tds_1-10Kb	0.00098514	0.00559656	0.00000127
+non-clustered_tds_10-100Kb	0.00011906	0.01948073	0.02651685
+non-clustered_tds_100Kb-1Mb	0.01252569	0.03134159	0.00405312
+non-clustered_tds_1Mb-10Mb	0.02074378	0.00844506	0.01205615
+non-clustered_tds_>10Mb	0.01391367	0.0240762	0.01162608
+non-clustered_inv_1-10Kb	0.01775605	0.04985384	0.05993695
+non-clustered_inv_10-100Kb	0.00886354	0.01882036	0.02325057
+non-clustered_inv_100Kb-1Mb	0.02501168	0.04010485	0.02112356
+non-clustered_inv_1Mb-10Mb	0.03438851	0.04624524	0.01434552
+non-clustered_inv_>10Mb	0.04593804	0.10010973	0.00383835
+non-clustered_trans	0.11695809	0.38809832	0.18813424
```

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_CNV48.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_DBS.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_ID.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SBS.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/txt_input/sample_matrix_SV32.txt`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3851a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3890a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3904a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD3945a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/data/tests/vcf_input/PD4005a.vcf`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/decompose_subroutines.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/decompose_subroutines.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     else:
         print(
             "The selected genome build is "
             + str(genome_build)
             + ". COSMIC signatures are available only for GRCh37/38, mm9/10 and rn6 genomes. So, the genome build is reset to GRCh37."
         )
         genome_build = "GRCh37"
-
     if samples.shape[0] == 96:
         if exome == False:
             sigDatabase = pd.read_csv(
                 paths
                 + "/data/Reference_Signatures/"
                 + genome_build
                 + "/COSMIC_v"
@@ -177,14 +176,15 @@
             + str(cosmic_version)
             + "_CN_GRCh37.txt",
             sep="\t",
             index_col=0,
         )
         signames = sigDatabase.columns
         connected_sigs = False
+
     elif samples.shape[0] == 32:
         if cosmic_version < 3.4:
             print(
                 f"The selected cosmic version is {cosmic_version}. However, SV signatures are "
                 "available only for version 3.4 and newer. Therefore, the cosmic version has "
                 "been reset to 3.4."
             )
@@ -201,14 +201,15 @@
         connected_sigs = False
     else:
         sigDatabase = pd.DataFrame(samples)
         sigDatabase.columns = sigDatabase.columns.astype(str)
         sigDatabase.index = sigDatabase.index.astype(str)
         signames = sigDatabase.columns
         connected_sigs = False
+
     return sigDatabase, signames, connected_sigs, genome_build
 
     if signature_database != None:  # pd.core.frame.DataFrame:
         print("################## USING CUSTOM SIGNATURE DATBASE ##################")
         signature_database = pd.read_csv(signature_database, sep="\t", index_col=0)
         if samples.shape[0] == signature_database.shape[0]:
             sigDatabase = signature_database
@@ -568,14 +569,16 @@
             mtype_par = "96"
         elif mtype == "DINUC" or mtype == "78":
             mtype_par = "78"
         elif mtype == "INDEL" or mtype == "83":
             mtype_par = "83"
         elif mtype == "CNV" or mtype == "48":
             mtype_par = "48"
+        elif mtype == "SV" or mtype == "32":
+            mtype_par = "32"
         else:
             mtype_par = "none"
         # only create decomposition plots for COSMIC signatures
         if (
             mtype_par != "none"
             and make_decomposition_plots == True
             and signature_database is None
@@ -663,14 +666,15 @@
             contexts = {
                 "96": "SBS96",
                 "288": "SBS288",
                 "1536": "SBS1536",
                 "78": "DBS78",
                 "83": "ID83",
                 "48": "CNV",
+                "32": "SV",
             }
             merger.write(
                 directory + "/" + contexts[mtype_par] + "_Decomposition_Plots.pdf"
             )
     except:
         print(
             "The context-"
```

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/decomposition.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/decomposition.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment/single_sample.py` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment/single_sample.py`

 * *Files identical despite different names*

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/PKG-INFO` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,17 @@
 Metadata-Version: 2.1
 Name: SigProfilerAssignment
-Version: 0.1.3
+Version: 0.1.4
 Summary: Mutational signatures attribution and decomposition tool
 Home-page: https://github.com/AlexandrovLab/SigProfilerAssignment.git
 Author: Raviteja Vangara
 Author-email: rvangara@health.ucsd.edu
 License: UCSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: scipy>=1.6.3
-Requires-Dist: numpy>=1.21.2
-Requires-Dist: pandas<2.0.0,>=1.2.4
-Requires-Dist: SigProfilerMatrixGenerator>=1.2.17
-Requires-Dist: sigProfilerPlotting>=1.3.20
-Requires-Dist: statsmodels>=0.9.0
-Requires-Dist: scikit-learn>=0.24.2
-Requires-Dist: psutil>=5.6.1
-Requires-Dist: reportlab>=3.5.42
-Requires-Dist: PyPDF2>=3.0.0
-Requires-Dist: alive_progress>=2.4.1
-Requires-Dist: pdf2image>=1.16.0
-Requires-Dist: PyMuPDF>=1.21.0
 
 [![Docs](https://img.shields.io/badge/docs-latest-blue.svg)](https://osf.io/mz79v/wiki/home/) 
 [![License](https://img.shields.io/badge/License-BSD\%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 [![Build Status](https://api.travis-ci.com/AlexandrovLab/SigProfilerAssignment.svg?branch=main)](https://app.travis-ci.com/AlexandrovLab/SigProfilerAssignment)
 
 <img src="SigProfilerAssignment/figures/SigProfilerAssignment.png" alt="drawing" width="1000"/>
```

### Comparing `SigProfilerAssignment-0.1.3/SigProfilerAssignment.egg-info/SOURCES.txt` & `SigProfilerAssignment-0.1.4/SigProfilerAssignment.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_CNV48.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_DBS78.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_ID83.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS1536.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS288.py
 SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SBS96.py
+SigProfilerAssignment/DecompositionPlots/PlotDecomposition_SV32.py
 SigProfilerAssignment/DecompositionPlots/SigProfilerPlottingMatrix.py
 SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Accolade_fermante.png
 SigProfilerAssignment/DecompositionPlots/ReferenceFiles/CREDIT.md
 SigProfilerAssignment/DecompositionPlots/ReferenceFiles/Fonts/Arial Bold.ttf
 SigProfilerAssignment/data/21_breast_WGS_substitutions.mat
 SigProfilerAssignment/data/CNV_features.tsv
 SigProfilerAssignment/data/CNV_signatures.txt
```

### Comparing `SigProfilerAssignment-0.1.3/setup.py` & `SigProfilerAssignment-0.1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import shutil
 import os
 
 # remove the dist folder first if exists
 if os.path.exists("dist"):
     shutil.rmtree("dist")
 
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 
 
 def write_version_py(filename="SigProfilerAssignment/version.py"):
     # Copied from numpy setup.py
     cnt = """
 # THIS FILE IS GENERATED FROM SigProfilerAssignment SETUP.PY
 short_version = '%(version)s'
 version = '%(version)s'
-Update = 'v0.1.3: Modify how ndarrays are processed'
+Update = 'v0.1.4: Add SV decomposition plotting.'
 
     
     """
     fh = open(filename, "w")
     fh.write(
         cnt
         % {
```

