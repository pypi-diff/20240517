# Comparing `tmp/dajin2-0.4.5.zip` & `tmp/dajin2-0.4.6.zip`

## zipinfo {}

```diff
@@ -1,81 +1,81 @@
-Zip file size: 87135 bytes, number of entries: 79
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-24 02:13 dajin2-0.4.5/LICENSE
--rw-r--r--  2.0 unx     1189 b- defN 24-Apr-24 02:13 dajin2-0.4.5/setup.py
--rw-r--r--  2.0 unx    12234 b- defN 24-Apr-24 02:13 dajin2-0.4.5/README.md
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-24 02:13 dajin2-0.4.5/setup.cfg
--rw-r--r--  2.0 unx      270 b- defN 24-Apr-24 02:13 dajin2-0.4.5/requirements.txt
--rw-r--r--  2.0 unx    13318 b- defN 24-Apr-24 02:13 dajin2-0.4.5/PKG-INFO
--rw-r--r--  2.0 unx      139 b- defN 24-Apr-24 02:13 dajin2-0.4.5/MANIFEST.in
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     2272 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2.egg-info/top_level.txt
--rw-r--r--  2.0 unx    13318 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      236 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2.egg-info/requires.txt
--rw-r--r--  2.0 unx       47 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/
--rw-r--r--  2.0 unx     2947 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/gui.py
--rw-r--r--  2.0 unx     1901 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/template_igvjs.html
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/__init__.py
--rw-r--r--  2.0 unx     2860 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/view.py
--rw-r--r--  2.0 unx     9634 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/main.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/static/css/
--rw-r--r--  2.0 unx       27 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/static/css/style.css
--rw-r--r--  2.0 unx     1777 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/templates/index.html
--rw-r--r--  2.0 unx      245 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/dna_handler.py
--rw-r--r--  2.0 unx     2374 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/multiprocess.py
--rw-r--r--  2.0 unx     7420 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/sam_handler.py
--rw-r--r--  2.0 unx     7985 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/cssplits_handler.py
--rw-r--r--  2.0 unx     3184 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/fastx_handler.py
--rw-r--r--  2.0 unx     2112 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/config.py
--rw-r--r--  2.0 unx     5411 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/io.py
--rw-r--r--  2.0 unx     4775 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/report_generator.py
--rw-r--r--  2.0 unx     6579 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/utils/input_validator.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/classification/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/report/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/consensus/
--rw-r--r--  2.0 unx    10663 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/core.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/__init__.py
--rw-r--r--  2.0 unx     8891 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/midsv_caller.py
--rw-r--r--  2.0 unx    21347 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/insertions_to_fasta.py
--rw-r--r--  2.0 unx    13202 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/mutation_extractor.py
--rw-r--r--  2.0 unx     1032 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/directory_manager.py
--rw-r--r--  2.0 unx     1656 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/homopolymer_handler.py
--rw-r--r--  2.0 unx      699 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/__init__.py
--rw-r--r--  2.0 unx     3585 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/input_formatter.py
--rw-r--r--  2.0 unx     1931 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/genome_fetcher.py
--rw-r--r--  2.0 unx     1636 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/knockin_handler.py
--rw-r--r--  2.0 unx     4630 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/mapping.py
--rw-r--r--  2.0 unx      790 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/preprocess/cache_checker.py
--rw-r--r--  2.0 unx     3715 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/classification/allele_merger.py
--rw-r--r--  2.0 unx     1795 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/classification/classifier.py
--rw-r--r--  2.0 unx       67 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/classification/__init__.py
--rw-r--r--  2.0 unx     3215 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/label_extractor.py
--rw-r--r--  2.0 unx     6522 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/score_handler.py
--rw-r--r--  2.0 unx     2298 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/kmer_generator.py
--rw-r--r--  2.0 unx     3516 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/clustering.py
--rw-r--r--  2.0 unx      210 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/__init__.py
--rw-r--r--  2.0 unx     1460 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/appender.py
--rw-r--r--  2.0 unx     1193 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/label_updator.py
--rw-r--r--  2.0 unx     3708 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/label_merger.py
--rw-r--r--  2.0 unx     5000 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/clustering/strand_bias_handler.py
--rw-r--r--  2.0 unx     6248 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/report/bam_exporter.py
--rw-r--r--  2.0 unx     4801 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/report/mutation_exporter.py
--rw-r--r--  2.0 unx      142 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/report/__init__.py
--rw-r--r--  2.0 unx     2176 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/report/insertion_reflector.py
--rw-r--r--  2.0 unx     2859 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/report/sequence_exporter.py
--rw-r--r--  2.0 unx     4202 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/consensus/consensus.py
--rw-r--r--  2.0 unx     2847 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/consensus/name_handler.py
--rw-r--r--  2.0 unx     5690 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/consensus/mutation_extractor.py
--rw-r--r--  2.0 unx      402 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/consensus/__init__.py
--rw-r--r--  2.0 unx      374 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/consensus/clust_formatter.py
--rw-r--r--  2.0 unx     4120 b- defN 24-Apr-24 02:13 dajin2-0.4.5/src/DAJIN2/core/consensus/similarity_searcher.py
-79 files, 239991 bytes uncompressed, 74075 bytes compressed:  69.1%
+Zip file size: 89183 bytes, number of entries: 79
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/
+-rw-r--r--  2.0 unx    12407 b- defN 24-May-17 07:42 dajin2-0.4.6/README.md
+-rw-r--r--  2.0 unx     1069 b- defN 24-May-17 07:42 dajin2-0.4.6/LICENSE
+-rw-r--r--  2.0 unx    13514 b- defN 24-May-17 07:42 dajin2-0.4.6/PKG-INFO
+-rw-r--r--  2.0 unx      139 b- defN 24-May-17 07:42 dajin2-0.4.6/MANIFEST.in
+-rw-r--r--  2.0 unx       38 b- defN 24-May-17 07:42 dajin2-0.4.6/setup.cfg
+-rw-r--r--  2.0 unx      279 b- defN 24-May-17 07:42 dajin2-0.4.6/requirements.txt
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-17 07:42 dajin2-0.4.6/setup.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/__init__.py
+-rw-r--r--  2.0 unx     9613 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/main.py
+-rw-r--r--  2.0 unx     1901 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/template_igvjs.html
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/gui.py
+-rw-r--r--  2.0 unx     2860 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/view.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/static/css/
+-rw-r--r--  2.0 unx       27 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/static/css/style.css
+-rw-r--r--  2.0 unx     9033 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/cssplits_handler.py
+-rw-r--r--  2.0 unx     2139 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/config.py
+-rw-r--r--  2.0 unx     5749 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/io.py
+-rw-r--r--  2.0 unx     2374 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/multiprocess.py
+-rw-r--r--  2.0 unx      245 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/dna_handler.py
+-rw-r--r--  2.0 unx     3184 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/fastx_handler.py
+-rw-r--r--  2.0 unx     7210 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/input_validator.py
+-rw-r--r--  2.0 unx     4775 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/report_generator.py
+-rw-r--r--  2.0 unx     7420 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/utils/sam_handler.py
+-rw-r--r--  2.0 unx     1777 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/templates/index.html
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/consensus/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/classification/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/report/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/__init__.py
+-rw-r--r--  2.0 unx    10756 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/core.py
+-rw-r--r--  2.0 unx     4476 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/consensus/similarity_searcher.py
+-rw-r--r--  2.0 unx      402 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/consensus/__init__.py
+-rw-r--r--  2.0 unx     4202 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/consensus/consensus.py
+-rw-r--r--  2.0 unx      374 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/consensus/clust_formatter.py
+-rw-r--r--  2.0 unx     2847 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/consensus/name_handler.py
+-rw-r--r--  2.0 unx     5710 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/consensus/mutation_extractor.py
+-rw-r--r--  2.0 unx      699 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/__init__.py
+-rw-r--r--  2.0 unx    24211 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/insertions_to_fasta.py
+-rw-r--r--  2.0 unx    13931 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/mutation_extractor.py
+-rw-r--r--  2.0 unx     3585 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/input_formatter.py
+-rw-r--r--  2.0 unx      790 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/cache_checker.py
+-rw-r--r--  2.0 unx     1789 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/knockin_handler.py
+-rw-r--r--  2.0 unx     8905 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/midsv_caller.py
+-rw-r--r--  2.0 unx     2371 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/homopolymer_handler.py
+-rw-r--r--  2.0 unx     2214 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/genome_fetcher.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/directory_manager.py
+-rw-r--r--  2.0 unx     4630 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/preprocess/mapping.py
+-rw-r--r--  2.0 unx       67 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/classification/__init__.py
+-rw-r--r--  2.0 unx     1795 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/classification/classifier.py
+-rw-r--r--  2.0 unx     3715 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/classification/allele_merger.py
+-rw-r--r--  2.0 unx      210 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/__init__.py
+-rw-r--r--  2.0 unx     3215 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/label_extractor.py
+-rw-r--r--  2.0 unx     3708 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/label_merger.py
+-rw-r--r--  2.0 unx     6522 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/score_handler.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/label_updator.py
+-rw-r--r--  2.0 unx     1460 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/appender.py
+-rw-r--r--  2.0 unx     5418 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/strand_bias_handler.py
+-rw-r--r--  2.0 unx     2298 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/kmer_generator.py
+-rw-r--r--  2.0 unx     3516 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/clustering/clustering.py
+-rw-r--r--  2.0 unx     2176 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/report/insertion_reflector.py
+-rw-r--r--  2.0 unx     4801 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/report/mutation_exporter.py
+-rw-r--r--  2.0 unx      142 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/report/__init__.py
+-rw-r--r--  2.0 unx     6248 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/report/bam_exporter.py
+-rw-r--r--  2.0 unx     2859 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2/core/report/sequence_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx      244 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2.egg-info/requires.txt
+-rw-r--r--  2.0 unx    13514 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        7 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       47 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-17 07:42 dajin2-0.4.6/src/DAJIN2.egg-info/dependency_links.txt
+79 files, 248241 bytes uncompressed, 76123 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1,238 +1,238 @@
-Filename: dajin2-0.4.5/
+Filename: dajin2-0.4.6/
 Comment: 
 
-Filename: dajin2-0.4.5/src/
+Filename: dajin2-0.4.6/src/
 Comment: 
 
-Filename: dajin2-0.4.5/LICENSE
+Filename: dajin2-0.4.6/README.md
 Comment: 
 
-Filename: dajin2-0.4.5/setup.py
+Filename: dajin2-0.4.6/LICENSE
 Comment: 
 
-Filename: dajin2-0.4.5/README.md
+Filename: dajin2-0.4.6/PKG-INFO
 Comment: 
 
-Filename: dajin2-0.4.5/setup.cfg
+Filename: dajin2-0.4.6/MANIFEST.in
 Comment: 
 
-Filename: dajin2-0.4.5/requirements.txt
+Filename: dajin2-0.4.6/setup.cfg
 Comment: 
 
-Filename: dajin2-0.4.5/PKG-INFO
+Filename: dajin2-0.4.6/requirements.txt
 Comment: 
 
-Filename: dajin2-0.4.5/MANIFEST.in
+Filename: dajin2-0.4.6/setup.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2.egg-info/
+Filename: dajin2-0.4.6/src/DAJIN2/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/
+Filename: dajin2-0.4.6/src/DAJIN2.egg-info/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2.egg-info/dependency_links.txt
+Filename: dajin2-0.4.6/src/DAJIN2/static/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2.egg-info/SOURCES.txt
+Filename: dajin2-0.4.6/src/DAJIN2/utils/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2.egg-info/top_level.txt
+Filename: dajin2-0.4.6/src/DAJIN2/templates/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2.egg-info/PKG-INFO
+Filename: dajin2-0.4.6/src/DAJIN2/core/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2.egg-info/requires.txt
+Filename: dajin2-0.4.6/src/DAJIN2/__init__.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2.egg-info/entry_points.txt
+Filename: dajin2-0.4.6/src/DAJIN2/main.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/static/
+Filename: dajin2-0.4.6/src/DAJIN2/template_igvjs.html
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/templates/
+Filename: dajin2-0.4.6/src/DAJIN2/gui.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/
+Filename: dajin2-0.4.6/src/DAJIN2/view.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/
+Filename: dajin2-0.4.6/src/DAJIN2/static/css/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/gui.py
+Filename: dajin2-0.4.6/src/DAJIN2/static/css/style.css
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/template_igvjs.html
+Filename: dajin2-0.4.6/src/DAJIN2/utils/cssplits_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/__init__.py
+Filename: dajin2-0.4.6/src/DAJIN2/utils/config.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/view.py
+Filename: dajin2-0.4.6/src/DAJIN2/utils/io.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/main.py
+Filename: dajin2-0.4.6/src/DAJIN2/utils/multiprocess.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/static/css/
+Filename: dajin2-0.4.6/src/DAJIN2/utils/dna_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/static/css/style.css
+Filename: dajin2-0.4.6/src/DAJIN2/utils/fastx_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/templates/index.html
+Filename: dajin2-0.4.6/src/DAJIN2/utils/input_validator.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/dna_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/utils/report_generator.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/multiprocess.py
+Filename: dajin2-0.4.6/src/DAJIN2/utils/sam_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/sam_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/templates/index.html
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/cssplits_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/consensus/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/fastx_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/config.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/classification/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/io.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/report_generator.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/report/
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/utils/input_validator.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/__init__.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/
+Filename: dajin2-0.4.6/src/DAJIN2/core/core.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/classification/
+Filename: dajin2-0.4.6/src/DAJIN2/core/consensus/similarity_searcher.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/
+Filename: dajin2-0.4.6/src/DAJIN2/core/consensus/__init__.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/report/
+Filename: dajin2-0.4.6/src/DAJIN2/core/consensus/consensus.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/consensus/
+Filename: dajin2-0.4.6/src/DAJIN2/core/consensus/clust_formatter.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/core.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/consensus/name_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/__init__.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/consensus/mutation_extractor.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/midsv_caller.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/__init__.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/insertions_to_fasta.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/insertions_to_fasta.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/mutation_extractor.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/mutation_extractor.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/directory_manager.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/input_formatter.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/homopolymer_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/cache_checker.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/__init__.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/knockin_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/input_formatter.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/midsv_caller.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/genome_fetcher.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/homopolymer_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/knockin_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/genome_fetcher.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/mapping.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/directory_manager.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/preprocess/cache_checker.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/preprocess/mapping.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/classification/allele_merger.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/classification/__init__.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/classification/classifier.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/classification/classifier.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/classification/__init__.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/classification/allele_merger.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/label_extractor.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/__init__.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/score_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/label_extractor.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/kmer_generator.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/label_merger.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/clustering.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/score_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/__init__.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/label_updator.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/appender.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/appender.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/label_updator.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/strand_bias_handler.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/label_merger.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/kmer_generator.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/clustering/strand_bias_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/clustering/clustering.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/report/bam_exporter.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/report/insertion_reflector.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/report/mutation_exporter.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/report/mutation_exporter.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/report/__init__.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/report/__init__.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/report/insertion_reflector.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/report/bam_exporter.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/report/sequence_exporter.py
+Filename: dajin2-0.4.6/src/DAJIN2/core/report/sequence_exporter.py
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/consensus/consensus.py
+Filename: dajin2-0.4.6/src/DAJIN2.egg-info/SOURCES.txt
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/consensus/name_handler.py
+Filename: dajin2-0.4.6/src/DAJIN2.egg-info/requires.txt
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/consensus/mutation_extractor.py
+Filename: dajin2-0.4.6/src/DAJIN2.egg-info/PKG-INFO
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/consensus/__init__.py
+Filename: dajin2-0.4.6/src/DAJIN2.egg-info/top_level.txt
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/consensus/clust_formatter.py
+Filename: dajin2-0.4.6/src/DAJIN2.egg-info/entry_points.txt
 Comment: 
 
-Filename: dajin2-0.4.5/src/DAJIN2/core/consensus/similarity_searcher.py
+Filename: dajin2-0.4.6/src/DAJIN2.egg-info/dependency_links.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `dajin2-0.4.5/LICENSE` & `dajin2-0.4.6/LICENSE`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/setup.py` & `dajin2-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as requirements_file:
     install_requirements = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="DAJIN2",
-    version="0.4.5",
+    version="0.4.6",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
     description="One-step genotyping tools for targeted long-read sequencing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/DAJIN2",
     install_requires=install_requirements,
```

## Comparing `dajin2-0.4.5/README.md` & `dajin2-0.4.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,28 @@
 + **Multi-Sample Compatibility**: Enabling parallel processing of multiple samples. This facilitates efficient progression of large-scale experiments and comparative studies.
 
 
 ## 🛠 Installation
 
 ### Prerequisites
 
-- Python 3.8 or later
+- Python 3.8 to 3.10
 - Unix-like environment (Linux, macOS, WSL2, etc.)
 
 ### From [Bioconda](https://anaconda.org/bioconda/DAJIN2) (Recommended)
 
 ```bash
 conda create -n env-dajin2 -c conda-forge -c bioconda python=3.10 DAJIN2 -y
 conda activate env-dajin2
 ```
 
+> [!IMPORTANT]
+> DAJIN2 supports Python versions 3.8 to 3.10, but not Python 3.11 yet due to a [Bioconda issue](https://github.com/bioconda/bioconda-recipes/issues/37805).
+
+
 > [!NOTE]
 > To Apple Silicon (ARM64) users:  
 > [Since the Bioconda channel does not yet support Apple Silicon](https://github.com/bioconda/bioconda-recipes/issues/37068#issuecomment-1257790919), please use the following command to install `DAJIN2` through Rosetta.
 > ```bash
 > CONDA_SUBDIR=osx-64 conda create -n env-dajin2 -c conda-forge -c bioconda python=3.10 DAJIN2 -y
 > conda activate env-dajin2
 > conda config --env --set subdir osx-64
```

## Comparing `dajin2-0.4.5/PKG-INFO` & `dajin2-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.4.5
+Version: 0.4.6
 Summary: One-step genotyping tools for targeted long-read sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: openpyxl>=3.1.0
 Requires-Dist: rapidfuzz>=3.6.0
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: mappy>=2.24
@@ -57,24 +58,28 @@
 + **Multi-Sample Compatibility**: Enabling parallel processing of multiple samples. This facilitates efficient progression of large-scale experiments and comparative studies.
 
 
 ## 🛠 Installation
 
 ### Prerequisites
 
-- Python 3.8 or later
+- Python 3.8 to 3.10
 - Unix-like environment (Linux, macOS, WSL2, etc.)
 
 ### From [Bioconda](https://anaconda.org/bioconda/DAJIN2) (Recommended)
 
 ```bash
 conda create -n env-dajin2 -c conda-forge -c bioconda python=3.10 DAJIN2 -y
 conda activate env-dajin2
 ```
 
+> [!IMPORTANT]
+> DAJIN2 supports Python versions 3.8 to 3.10, but not Python 3.11 yet due to a [Bioconda issue](https://github.com/bioconda/bioconda-recipes/issues/37805).
+
+
 > [!NOTE]
 > To Apple Silicon (ARM64) users:  
 > [Since the Bioconda channel does not yet support Apple Silicon](https://github.com/bioconda/bioconda-recipes/issues/37068#issuecomment-1257790919), please use the following command to install `DAJIN2` through Rosetta.
 > ```bash
 > CONDA_SUBDIR=osx-64 conda create -n env-dajin2 -c conda-forge -c bioconda python=3.10 DAJIN2 -y
 > conda activate env-dajin2
 > conda config --env --set subdir osx-64
```

## Comparing `dajin2-0.4.5/src/DAJIN2.egg-info/SOURCES.txt` & `dajin2-0.4.6/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2.egg-info/PKG-INFO` & `dajin2-0.4.6/src/DAJIN2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.4.5
+Version: 0.4.6
 Summary: One-step genotyping tools for targeted long-read sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: certifi
 Requires-Dist: numpy>=1.24.0
 Requires-Dist: scipy>=1.10.0
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: openpyxl>=3.1.0
 Requires-Dist: rapidfuzz>=3.6.0
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: mappy>=2.24
@@ -57,24 +58,28 @@
 + **Multi-Sample Compatibility**: Enabling parallel processing of multiple samples. This facilitates efficient progression of large-scale experiments and comparative studies.
 
 
 ## 🛠 Installation
 
 ### Prerequisites
 
-- Python 3.8 or later
+- Python 3.8 to 3.10
 - Unix-like environment (Linux, macOS, WSL2, etc.)
 
 ### From [Bioconda](https://anaconda.org/bioconda/DAJIN2) (Recommended)
 
 ```bash
 conda create -n env-dajin2 -c conda-forge -c bioconda python=3.10 DAJIN2 -y
 conda activate env-dajin2
 ```
 
+> [!IMPORTANT]
+> DAJIN2 supports Python versions 3.8 to 3.10, but not Python 3.11 yet due to a [Bioconda issue](https://github.com/bioconda/bioconda-recipes/issues/37805).
+
+
 > [!NOTE]
 > To Apple Silicon (ARM64) users:  
 > [Since the Bioconda channel does not yet support Apple Silicon](https://github.com/bioconda/bioconda-recipes/issues/37068#issuecomment-1257790919), please use the following command to install `DAJIN2` through Rosetta.
 > ```bash
 > CONDA_SUBDIR=osx-64 conda create -n env-dajin2 -c conda-forge -c bioconda python=3.10 DAJIN2 -y
 > conda activate env-dajin2
 > conda config --env --set subdir osx-64
```

## Comparing `dajin2-0.4.5/src/DAJIN2/gui.py` & `dajin2-0.4.6/src/DAJIN2/gui.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/template_igvjs.html` & `dajin2-0.4.6/src/DAJIN2/template_igvjs.html`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/view.py` & `dajin2-0.4.6/src/DAJIN2/view.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/main.py` & `dajin2-0.4.6/src/DAJIN2/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,24 +9,22 @@
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
 
 
 import sys
 import shutil
 import argparse
 from pathlib import Path
+from copy import deepcopy
 from itertools import groupby
 
 from DAJIN2 import gui, view
 from DAJIN2.core import core
 from DAJIN2.utils import io, config, report_generator, input_validator, multiprocess
 
 
-DAJIN_VERSION = "0.4.5"
-
-
 def generate_report(name: str) -> None:
     report_generator.report(name)
     print(
         f"\N{party popper} Finished! Open {config.DAJIN_RESULTS_DIR}/{name} to see the report.",
         file=sys.stderr,
     )
 
@@ -54,50 +52,51 @@
 
 
 ################################################################################
 # Batch mode
 ################################################################################
 
 
-def validate_headers_of_batch_file(headers: list, filepath: str) -> None:
+def validate_headers_of_batch_file(headers: set[str], filepath: str) -> None:
     """Validate the headers of a batch file."""
-    required_headers = ["sample", "control", "allele", "name"]
-    accepted_headers = ["sample", "control", "allele", "name", "genome"]
+    required_headers = {"sample", "control", "allele", "name"}
+    accepted_headers = {"sample", "control", "allele", "name", "genome"}
 
-    if not set(required_headers).issubset(set(headers)):
-        raise ValueError(f"{filepath} must contain {', '.join(required_headers)} in the header")
+    if not required_headers.issubset(headers):
+        raise ValueError(f'{filepath} must contain "sample", "control", "allele" and "name" in the header')
 
-    if not set(headers).issubset(accepted_headers):
-        raise ValueError(f"Accepted header names of {filepath} are {', '.join(accepted_headers)}.")
+    if not headers.issubset(accepted_headers):
+        raise ValueError(f'Accepted header names of {filepath} are "sample", "control", "allele", "name", or "genome".')
 
 
-def create_argument_dict(headers: list, group: list, cache_urls_genome: dict, is_control: bool) -> dict:
+def create_argument_dict(args: dict, cache_urls_genome: dict, is_control: bool) -> dict[str, str]:
     """Create a dictionary of arguments from the given headers and group."""
-    args = dict(zip(headers, group))
-    args["threads"] = 1  # Set the number of threads to 1 for batch mode
+    args_update = deepcopy(args)
+
+    args_update["threads"] = 1  # Set the number of threads to 1 for batch mode
 
     # Assign the "sample" field depending on whether it's a control or not
     if is_control:
-        args["sample"] = args["control"]
+        args_update["sample"] = args_update["control"]
     else:
-        if args["sample"] == args["control"]:
+        if args_update["sample"] == args_update["control"]:
             return {}  # Return an empty dict to indicate a skipped group
 
-    if args.get("genome"):
-        args.update(cache_urls_genome[args["genome"]])
+    if args_update.get("genome"):
+        args_update.update(cache_urls_genome[args_update["genome"]])
 
-    return args
+    return args_update
 
 
 def run_DAJIN2(
-    groups: list, headers: list, cache_urls_genome: dict, is_control: bool = True, num_workers: int = 1
+    groups: list[dict[str, str]], cache_urls_genome: dict, is_control: bool = True, num_workers: int = 1
 ) -> None:
     contents = []
-    for group in groups:
-        args = create_argument_dict(headers, group, cache_urls_genome, is_control)
+    for args in groups:
+        args = create_argument_dict(args, cache_urls_genome, is_control)
         if args:  # Add args to contents only if it's not an empty dict
             contents.append(args)
 
     # Return a list of unique dictionaries
     contents_unique = [dict(item) for item in set(frozenset(d.items()) for d in contents)]
 
     contents_unique.sort(key=lambda x: x["sample"])
@@ -110,44 +109,45 @@
 
 def execute_batch_mode(arguments: dict[str]):
     path_batchfile = io.convert_to_posix(arguments["file"])
 
     if not Path(path_batchfile).exists():
         raise FileNotFoundError(f"'{path_batchfile}' does not exist.")
 
-    inputs = io.load_batchfile(path_batchfile)
+    records = io.load_batchfile(path_batchfile)
 
     # Validate Column of the batch file
-    headers = inputs[0]
+    headers = set(records[0].keys())
     validate_headers_of_batch_file(headers, path_batchfile)
 
     # Validate contents and fetch genome urls
-    contents = inputs[1:]
     cache_urls_genome = dict()
-    index_of_name = headers.index("name")
-    contents.sort(key=lambda x: x[index_of_name])
-    for _, groups in groupby(contents, key=lambda x: x[index_of_name]):
-        for group in groups:
-            args = dict(zip(headers, group))
-            # validate contents in the batch file
+    records.sort(key=lambda x: x["name"])
+    for _, groups in groupby(records, key=lambda x: x["name"]):
+        for args in groups:
+            # Validate contents in the batch file
             input_validator.validate_files(args["sample"], args["control"], args["allele"])
-            # validate genome and fetch urls
+            # Validate genome and fetch urls
             if args.get("genome") and args["genome"] not in cache_urls_genome:
                 urls_genome = input_validator.validate_genome_and_fetch_urls(args["genome"])
                 cache_urls_genome[args["genome"]] = urls_genome
-    for name, groups in groupby(contents, key=lambda x: x[index_of_name]):
-        # set logging to export log to stderr and file
+
+    # Run DAJIN2
+    for name, groups in groupby(records, key=lambda x: x["name"]):
+        groups: list[dict[str, str]] = list(groups)
+        # Set logging to export log to stderr and file
         config.reset_logging()
         path_logfile = config.get_logfile()
         config.set_logging(path_logfile)
-        groups = list(groups)
-        # Run DAJIN2
-        run_DAJIN2(groups, headers, cache_urls_genome, is_control=True, num_workers=arguments["threads"])
-        run_DAJIN2(groups, headers, cache_urls_genome, is_control=False, num_workers=arguments["threads"])
-        # Finish
+
+        # Start DAJIN2
+        run_DAJIN2(groups, cache_urls_genome, is_control=True, num_workers=arguments["threads"])
+        run_DAJIN2(groups, cache_urls_genome, is_control=False, num_workers=arguments["threads"])
+
+        # Finish call
         generate_report(name)
         shutil.move(path_logfile, Path("DAJIN_Results", name))
         if not arguments["debug"]:
             shutil.rmtree(Path("DAJIN_Results", ".tempdir", name))
 
 
 def execute():
@@ -161,15 +161,15 @@
     parser.add_argument("-c", "--control", type=str, help="Path to a control directory including FASTQ file")
     parser.add_argument("-a", "--allele", type=str, help="Path to a FASTA file")
     parser.add_argument("-n", "--name", type=str, help="Output directory name", default="Results")
     parser.add_argument(
         "-g", "--genome", type=str, default="", help="Reference genome ID (e.g hg38, mm39) [default: '']"
     )
     parser.add_argument("-t", "--threads", type=int, default=1, help="Number of threads [default: 1]")
-    parser.add_argument("-v", "--version", action="version", version=f"DAJIN2 version {DAJIN_VERSION}")
+    parser.add_argument("-v", "--version", action="version", version=f"DAJIN2 version {config.DAJIN_VERSION}")
     parser.add_argument("-d", "--debug", action="store_true", help=argparse.SUPPRESS)
 
     ###############################################################################
     # Batch mode
     ###############################################################################
 
     def batchmode(args):
```

## Comparing `dajin2-0.4.5/src/DAJIN2/templates/index.html` & `dajin2-0.4.6/src/DAJIN2/templates/index.html`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/multiprocess.py` & `dajin2-0.4.6/src/DAJIN2/utils/multiprocess.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/sam_handler.py` & `dajin2-0.4.6/src/DAJIN2/utils/sam_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             break
         # Increment mutation count for non-match operations
         if op != "M":
             count_mutation += num
     return count_mutation
 
 
-def trim_cigar_on_microhomology(cigar_split: list, len_microhomology: int) -> tuple(str, int):
+def trim_cigar_on_microhomology(cigar_split: list, len_microhomology: int) -> tuple[str, int]:
     """Trim CIGAR based on the length of the microhomology."""
     cigar_trimmed = cigar_split[::-1]
     total_num = 0
     num_deleletion = 0
     while total_num < len_microhomology:
         cigar = cigar_trimmed.pop()
         num, op = int(cigar[:-1]), cigar[-1]
```

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/cssplits_handler.py` & `dajin2-0.4.6/src/DAJIN2/utils/cssplits_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -156,77 +156,103 @@
 
 
 ###########################################################
 # detect_insertion_within_deletion
 ###########################################################
 
 
-def is_start_of_deletion(i: int, cssplits: list[str], start_del_count: int = 3) -> bool:
-    """
-    Determine if the current index is the start of a deletion.
-    If there are consecutive deletions from the beginning, it is determined that there is a cluster of deletions.
-    """
-    if i + start_del_count > len(cssplits):
+def is_start_of_consecutive_deletions(cssplits: list[str], i: int, del_range: int = 3) -> bool:
+    """Determine if the current index is the start of a consective deletion."""
+    if i + del_range > len(cssplits):
         return False
-    return all([cs.startswith("-") for cs in cssplits[i : i + start_del_count]])
 
+    for j in range(del_range):
+        if not cssplits[i + j].startswith("-"):
+            return False
+
+    return True
+
+
+def get_range_of_inclusive_deletions(cssplits: list[str], del_range: int = 3, distance: int = 10) -> set[int]:
+    inclusive_deletion_range: set[int] = set()
+    n: int = len(cssplits)
+    i: int = 0
+    while i < n:
+        # Check for start of deletion
+        if cssplits[i].startswith("-"):
+            start: int = i
+            while i < n and cssplits[i].startswith("-"):
+                i += 1
+            # We have found the end of a deletion range
+            end: int = i
+            # Check if deletion length is enough to be considered
+
+            if end - start >= del_range:
+                # Now check for matching sequence within 'distance'
+                match_count: int = 0
+                while i < n and match_count <= distance:
+                    if cssplits[i].startswith("="):
+                        match_count += 1
+                    elif cssplits[i].startswith("-"):
+                        # If another deletion is found, reset match count and update range
+                        next_start: int = i
+                        while i < n and cssplits[i].startswith("-"):
+                            i += 1
+                            next_end: int = i
+                        if next_end - next_start >= del_range:
+                            inclusive_deletion_range.update(range(start, next_end))
+
+                            start = next_start
+                            end = next_end
+                            match_count = 0
+                            break
+                    i += 1
 
-def is_within_deletion(i: int, cssplits: list[str], distance: int = 10) -> bool:
-    """Count matches that are continuous for `distance` bases, and if there is a deletion in between, it is determined to be inside a cluster of deletions."""
-    exist_deletion = False
-    total_num_match = 0
-    j = 1
-    while True:
-        if i + j >= len(cssplits) or total_num_match > distance:
-            exist_deletion = False
-            break
-        current = cssplits[i + j]
-        if current.startswith("="):
-            total_num_match += 1
-        else:
-            total_num_match = 0
-            if current.startswith("-"):
-                exist_deletion = True
-                break
-        j += 1
-    return exist_deletion
+        i += 1
+
+    return inclusive_deletion_range
 
 
 def adjust_cs_insertion(cs: str) -> str:
     if cs.startswith("-"):
         return None
     elif cs.startswith("+"):
         ins = "|".join(cs.split("|")[:-1])
         end_cs = cs.split("|")[-1][-1]
         cs_insertion = f"{ins}|+{end_cs}|"
     else:
         cs_insertion = f"+{cs[-1]}|"
     return cs_insertion
 
 
-def detect_insertion_within_deletion(cssplits: str, start_del_count: int = 3, distance: int = 10) -> str:
-    cssplits = cssplits.split(",")
+def reallocate_insertion_within_deletion(cssplit: str, del_range: int = 3, distance: int = 10) -> str:
+    """
+    Since the mapping in minimap2 is local alignment, insertion bases within large deletions may be partially mapped to the reference genome and not detected as insertion bases. Therefore, update cssplits to detect insertions within large deletions as insertions.
+    """
+    cssplits = cssplit.split(",")
     cssplits_updated = cssplits.copy()
 
-    insertion = []
-    within_deletion = False
+    range_of_inclusive_deletion: set[int] = get_range_of_inclusive_deletions(cssplits, del_range, distance)
+
+    insertion_within_deletion = []
     for i, cs in enumerate(cssplits):
-        if cs.startswith("-"):
-            if within_deletion is False and is_start_of_deletion(i, cssplits, start_del_count) is False:
+        if i in range_of_inclusive_deletion:
+            if cs.startswith("-"):
                 continue
-            within_deletion = is_within_deletion(i, cssplits, distance)
-            if within_deletion is False:
-                cssplits_updated[i + 1] = "".join(insertion) + cssplits_updated[i + 1]
-                insertion = []
-        if within_deletion is False:
-            continue
-        if not cs.startswith("-"):
-            if cs.startswith("*"):
-                cssplits_updated[i] = f"-{cs[1]}"
+            if cs.startswith("N") or cs.startswith("n"):
+                cs_new = cs
+            elif cs.startswith("*"):
+                cs_new = f"-{cs[1]}"
             elif cs.startswith("+") and cs.split("|")[-1].startswith("*"):
-                cssplits_updated[i] = f'-{cs.split("|")[-1][1]}'
+                cs_new = f'-{cs.split("|")[-1][1]}'
             else:
-                cssplits_updated[i] = f"-{cs[-1]}"
-            adjusted_cs = adjust_cs_insertion(cs)
-            insertion.append(adjusted_cs)
+                cs_new = f"-{cs[-1]}"
+            cssplits_updated[i] = cs_new
+
+            insertion_within_deletion.append(adjust_cs_insertion(cs))
+        else:
+            if not insertion_within_deletion:
+                continue
+            cssplits_updated[i] = "".join(insertion_within_deletion) + cs
+            insertion_within_deletion = []
 
     return ",".join(cssplits_updated)
```

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/fastx_handler.py` & `dajin2-0.4.6/src/DAJIN2/utils/fastx_handler.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/config.py` & `dajin2-0.4.6/src/DAJIN2/utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import warnings
 import datetime
 
 from pathlib import Path
 
 from sklearn.exceptions import ConvergenceWarning
 
-
+DAJIN_VERSION = "0.4.6"
 DAJIN_RESULTS_DIR = Path("DAJIN_Results")
 TEMP_ROOT_DIR = Path(DAJIN_RESULTS_DIR, ".tempdir")
 
 
 class DeferredFileHandler(logging.FileHandler):
     def __init__(self, filename, mode="a", encoding=None, delay=True):
         # Setting delay to True to defer the file opening
@@ -24,15 +24,15 @@
         if self.stream is None:
             self.stream = self._open()
         super().emit(record)
 
 
 def get_logfile() -> Path:
     current_time = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    return Path(f"{current_time}_DAJIN2.log")
+    return Path(f"DAJIN2_log_{current_time}.txt")
 
 
 def set_logging(path_logfile: Path) -> None:
     log_format = "%(asctime)s, %(levelname)s, %(message)s"
     date_format = "%Y-%m-%d %H:%M:%S"
 
     stderr_handler = logging.StreamHandler()
```

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/io.py` & `dajin2-0.4.6/src/DAJIN2/utils/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -91,38 +91,47 @@
     elif file_extension == ".csv":
         return "csv"
     else:
         raise ValueError("The provided file must be either an Excel or CSV file.")
 
 
 def read_xlsx(file_path: str | Path) -> list[dict[str, str]]:
-    """Load data from an Excel file and return as a list."""
+    """Load data from an Excel file."""
     wb = load_workbook(filename=file_path)
     ws = wb.active
 
     headers = [cell for cell in next(ws.iter_rows(min_row=1, max_row=1, values_only=True))]
 
-    data = []
+    records = []
     for row in ws.iter_rows(min_row=2, values_only=True):
+        if all(element is None for element in row):  # Skip rows with all None values
+            continue
         row_data = {headers[i]: (row[i] if i < len(row) else None) for i in range(len(headers))}
-        data.append(row_data)
+        records.append(row_data)
 
-    return data
+    return records
 
 
-def read_csv(file_path: str) -> list[dict[str, str]]:
-    """Load data from a CSV file and return as a list."""
+def read_csv(file_path: str | Path) -> list[dict[str, str]]:
+    """Load data from a CSV file."""
     with open(file_path, "r") as csvfile:
-        inputs = []
+
+        header = [field.strip() for field in next(csv.reader(csvfile))]
+
+        records = []
         for row in csv.reader(csvfile):
             if not row:  # Skip empty rows
                 continue
-            trimmed_row = [field.strip() for field in row]
-            inputs.append(trimmed_row)
-        return inputs
+            if all(element is None for element in row):  # Skip rows with all None values
+                continue
+            row_trimmed = [field.strip() for field in row]
+            row_data = {h: v for h, v in zip(header, row_trimmed)}
+            records.append(row_data)
+
+        return records
 
 
 def load_batchfile(batchfile_path: str) -> list[dict[str, str]]:
     """Load data from either an Excel or CSV file."""
     file_type = determine_file_type(batchfile_path)
     if file_type == "excel":
         return read_xlsx(batchfile_path)
```

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/report_generator.py` & `dajin2-0.4.6/src/DAJIN2/utils/report_generator.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/utils/input_validator.py` & `dajin2-0.4.6/src/DAJIN2/utils/input_validator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from __future__ import annotations
 
 import os
 import re
+import ssl
 import hashlib
 
 from pathlib import Path
 from urllib.error import URLError
 from urllib.request import urlopen
 import xml.etree.ElementTree as ET
 
 import mappy
 
+########################################################################
+# To accommodate cases where a user might input negative values or
+# excessively large values, update the number of threads
+# from "1" to "max cpu threads - 1".
+########################################################################
+
 
 def update_threads(threads: int) -> int:
     available_threads = os.cpu_count() - 1
     threads_updated = max(1, min(threads, available_threads))
     return threads_updated
 
 
@@ -103,51 +110,51 @@
 
 
 ########################################################################
 # Check genome and UCSC server
 ########################################################################
 
 
-def get_html(url: str) -> str:
-    try:
-        with urlopen(url, timeout=10) as response:
-            html = response.read().decode("utf-8")
-        return html
-    except URLError:
-        return ""
+def fetch_html_without_verification(url: str) -> str:
+    context = ssl._create_unverified_context()  # Create an SSL context that temporarily disables verification
+    with urlopen(url, context=context, timeout=10) as response:
+        return response.read().decode("utf-8")
 
 
 def format_url(key: str, url: str) -> str:
     return url + "/hg38" if key == "goldenpath" else url
 
 
 def get_first_available_url(key: str, urls: list[str]) -> str | None:
     search_keys = {"blat": "BLAT Search Genome", "das": "GRCh38/hg38", "goldenpath": "bigZips"}
-    return next((url for url in urls if search_keys[key] in get_html(format_url(key, url))), None)
+    return next(
+        (url for url in urls if search_keys[key] in fetch_html_without_verification(format_url(key, url))), None
+    )
 
 
-def fetch_xml_data(url: str) -> bytes:
+def fetch_xml_without_verification(url: str) -> bytes:
     """Fetch XML data from a given URL."""
-    with urlopen(url) as response:
+    context = ssl._create_unverified_context()  # Create an SSL context that temporarily disables verification
+    with urlopen(url, context=context, timeout=10) as response:
         return response.read()
 
 
-def extract_genome_ids_from_xml(xml_data: bytes) -> set:
+def extract_genome_ids_from_xml(xml_data: bytes) -> set[str]:
     """Extract genome IDs from XML data."""
     root = ET.fromstring(xml_data)
     return {cc.attrib["id"] for child in root for cc in child if cc.tag == "SOURCE"}
 
 
-def get_genome_ids_in_ucsc(url_das: str) -> set:
+def get_genome_ids_in_ucsc(url_das: str) -> set[str]:
     """Get available genome IDs in UCSC."""
-    xml_data = fetch_xml_data(url_das)
+    xml_data = fetch_xml_without_verification(url_das)
     return extract_genome_ids_from_xml(xml_data)
 
 
-def is_genome_in_ucsc_ids(genome: str, url_das: str) -> bool:
+def is_genome_id_available_in_ucsc(genome: str, url_das: str) -> bool:
     genome_ids = get_genome_ids_in_ucsc(url_das)
     return genome in genome_ids
 
 
 def validate_genome_and_fetch_urls(genome: str) -> dict[str, str]:
     server_lists = {
         "blat": [
@@ -174,13 +181,13 @@
         "goldenpath": "All UCSC GoldenPath servers are currently down. Please wait for a while and try again.",
     }
 
     for key, message in error_messages.items():
         if available_servers[key] is None:
             raise URLError(message)
 
-    if not is_genome_in_ucsc_ids(genome, available_servers["das"]):
+    if not is_genome_id_available_in_ucsc(genome, available_servers["das"]):
         raise ValueError(f"{genome} is not listed. Available genomes are in {available_servers['das']}")
 
     del available_servers["das"]
 
     return available_servers
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/core.py` & `dajin2-0.4.6/src/DAJIN2/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
 import shutil
 import logging
 
 from pathlib import Path
 
-from DAJIN2.utils import io, fastx_handler
+from DAJIN2.utils import io, config, fastx_handler
 from DAJIN2.core import classification, clustering, consensus, preprocess, report
 from DAJIN2.core.preprocess.input_formatter import FormattedInputs
 
 logger = logging.getLogger(__name__)
 
 
 ###########################################################
 # main
 ###########################################################
 
 
 def execute_control(arguments: dict):
+
+    logger.info(f"\N{runner} Start running DAJIN2 version {config.DAJIN_VERSION}")
+
     logger.info(f"{arguments['control']} is now processing...")
 
     ###########################################################
     # Preprocess
     ###########################################################
     ARGS: FormattedInputs = preprocess.format_inputs(arguments)
     preprocess.create_temporal_directories(ARGS.tempdir, ARGS.control_name, is_control=True)
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/midsv_caller.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/midsv_caller.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,17 @@
 
 def convert_consecutive_indels(midsv_sample: Generator) -> Generator[list[dict]]:
     for m in midsv_sample:
         m["CSSPLIT"] = convert_consecutive_indels_to_match(m["CSSPLIT"])
         yield m
 
 
-def detect_insertion_within_deletion(midsv_sample: Generator) -> Generator[list[dict]]:
+def reallocate_insertions_within_deletion(midsv_sample: Generator) -> Generator[list[dict]]:
     for m in midsv_sample:
-        m["CSSPLIT"] = cssplits_handler.detect_insertion_within_deletion(m["CSSPLIT"])
+        m["CSSPLIT"] = cssplits_handler.reallocate_insertion_within_deletion(m["CSSPLIT"])
         yield m
 
 
 ###########################################################
 # main
 ###########################################################
 
@@ -220,9 +220,9 @@
         sam_of_map_ont = filter_sam_by_preset(sam_ont, qname_of_map_ont, preset="map-ont")
         sam_of_splice = filter_sam_by_preset(sam_splice, qname_of_map_ont, preset="splice")
         midsv_chaind = transform_to_midsv_format(chain(sam_of_map_ont, sam_of_splice))
         midsv_sample = replace_internal_n_to_d(midsv_chaind, sequence)
         midsv_sample = convert_flag_to_strand(midsv_sample)
         midsv_sample = filter_samples_by_n_proportion(midsv_sample)
         midsv_sample = convert_consecutive_indels(midsv_sample)
-        midsv_sample = detect_insertion_within_deletion(midsv_sample)
+        midsv_sample = reallocate_insertions_within_deletion(midsv_sample)
         midsv.write_jsonl(midsv_sample, path_output_midsv)
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/insertions_to_fasta.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/insertions_to_fasta.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,46 +6,48 @@
 from itertools import groupby
 from collections import defaultdict, Counter
 from typing import Generator
 
 import numpy as np
 from rapidfuzz import process
 from rapidfuzz.distance import DamerauLevenshtein
+
 from sklearn.cluster import MeanShift
 
 from DAJIN2.core.preprocess.mapping import to_sam
 from DAJIN2.utils import io, config
 from DAJIN2.utils.cssplits_handler import convert_cssplits_to_cstag
 
 config.set_warnings_ignore()
 
 import cstag
 
 
-def remove_non_alphabets(s: str) -> str:
+def remove_non_alphabets(cssplits: str) -> str:
     """Convert a cssplits to a plain DNA sequence."""
-    return "".join([char for char in s if char.isalpha()])
+    return "".join([char for char in cssplits if char.isalpha()])
 
 
 ###########################################################
 # Cluster insertion alleles
 ###########################################################
 
 
-def clustering_insertions(insertions_cssplit: list[str]) -> list[int]:
-    seq_all = [remove_non_alphabets(seq) for seq in insertions_cssplit]
+def clustering_insertions(cssplits_insertion: list[str], n_decoy: int = 1000) -> list[int]:
+    seq_all = [remove_non_alphabets(seq) for seq in cssplits_insertion]
     query = seq_all[0]
     _, distances, _ = zip(*process.extract_iter(query, seq_all, scorer=DamerauLevenshtein.normalized_distance))
 
-    # Add random values from 0 to 1
-    distances = list(distances)
-    rng = np.random.default_rng(1)
-    distances.extend(rng.random(max(100, len(seq_all))))
+    # By adding upper (1) and lower (0) limits, we prevent errors where minor differences are clustered (e.g., 0.1 and 0.2 becoming separate clusters).
+
+    insertion_lengths = [[len(c) for c in cs.split(",")] for cs in cssplits_insertion]
+
+    scores = [s + [d] for s, d in zip(insertion_lengths, distances)]
 
-    return MeanShift().fit(np.array(distances).reshape(-1, 1)).labels_.tolist()[: len(seq_all)]
+    return MeanShift(bin_seeding=True).fit_predict(np.array(scores)).tolist()
 
 
 ###########################################################
 # Detect insertion sequences
 ###########################################################
 
 
@@ -64,16 +66,16 @@
 
 def extract_enriched_insertions(
     insertions_sample: dict, insertions_control: dict, coverage_sample: int
 ) -> dict[int, dict[str, int]]:
     enriched_insertions = dict()
     threshold_sample = max(5, int(coverage_sample * 0.5 / 100))
     for i in insertions_sample:
-        ins_sample = insertions_sample[i]
-        ins_control = insertions_control.get(i, [])
+        ins_sample: list[str] = insertions_sample[i]
+        ins_control: list[str] = insertions_control.get(i, [])
 
         labels_all = clustering_insertions(ins_sample + ins_control)
         labels_sample = labels_all[: len(ins_sample)]
         labels_control = labels_all[len(ins_sample) : len(ins_sample) + len(ins_control)]
 
         labels_count_sample = dict(Counter(labels_sample))
         labels_count_control = dict(Counter(labels_control))
@@ -116,14 +118,15 @@
 
 ###########################################################
 # Merge similar insertion sequences
 ###########################################################
 
 
 def group_index_by_consecutive_insertions(mutation_loci: list[set[str]]) -> list[tuple[int]]:
+    """Groups indices of consecutive locations containing "+" mutations in the input list."""
     index = sorted(i for i, m in enumerate(mutation_loci) if "+" in m)
     index_grouped = []
     for _, group in groupby(enumerate(index), lambda i_x: i_x[0] - i_x[1]):
         items = [value for _, value in group]
         index_grouped.append(tuple(items))
     return index_grouped
 
@@ -157,29 +160,44 @@
             sequences.add(seq)
             counts += count
         insertion_merged[tuple(sorted(sequences))] = counts
 
     return insertion_merged
 
 
+def remove_minor_groups(insertions_merged: dict[tuple[int], dict[tuple[str], int]], coverage: int, threshold: float = 0.5) -> dict[tuple[int], dict[tuple[str], int]]:
+    for _, ins in insertions_merged.items():
+        # Create a list of elements to delete
+        to_delete = []
+        for seq, count in ins.items():
+            if count < coverage * threshold // 100:
+                to_delete.append(seq)
+
+        # Delete the collected elements
+        for seq in to_delete:
+            del ins[seq]
+
+    return insertions_merged
+
+
 def merge_similar_insertions(
-    insertions: dict[int, dict[str, int]], mutation_loci: list[set[str]]
-) -> dict[tuple(int), dict[tuple[str], int]]:
+    insertions: dict[int, dict[str, int]], mutation_loci: list[set[str]], coverage: int, threshold: float = 0.5
+) -> dict[tuple[int], dict[tuple[str], int]]:
     index_grouped = group_index_by_consecutive_insertions(mutation_loci)
     insertions_grouped = group_insertions(insertions, index_grouped)
     insertions_merged = dict()
     for idx, insertion in insertions_grouped.items():
         if len(insertion) == 1:
             seq, count = next(iter(insertion.items()))
             insertions_merged[idx] = {tuple([seq]): count}
             continue
-        labels = clustering_insertions(insertion)
+        labels = clustering_insertions(insertion, n_decoy=1000)
         insertions_merged[idx] = get_merged_insertion(insertion, labels)
 
-    return insertions_merged
+    return remove_minor_groups(insertions_merged, coverage, threshold)
 
 
 ###########################################################
 # Pre- and post-process of clustering insertion alleles
 ###########################################################
 
 
@@ -188,16 +206,16 @@
     for key_tuple in dict_keys:
         for num in key_tuple:
             flattened_nums.add(num)
     return flattened_nums
 
 
 def subset_insertions(
-    insertions_merged: dict[tuple(int), dict[tuple[str], int]], num_subset: int = 100
-) -> dict[tuple(int), dict[tuple[str], int]]:
+    insertions_merged: dict[tuple[int], dict[tuple[str], int]], num_subset: int = 100
+) -> dict[tuple[int], dict[tuple[str], int]]:
     """
     If the number of seqs exceeds `num_subset`, limit it to only the `num_subset` elements with fiexd random sampling.
     """
     random.seed(1)
     insertions_merged_subset = defaultdict(dict)
     for idx_grouped, insertions in insertions_merged.items():
         for cs_insertion, counts in insertions.items():
@@ -208,76 +226,82 @@
             sequences = tuple(remove_non_alphabets(seq) for seq in sequences)
             insertions_merged_subset[idx_grouped][sequences] = counts
 
     return dict(insertions_merged_subset)
 
 
 def extract_score_and_sequence(
-    path_sample, insertions_merged: dict[tuple(int), dict[tuple[str], int]]
+    path_sample, insertions_merged: dict[tuple[int], dict[tuple[str], int]]
 ) -> list[tuple[list[int], str]]:
     scores = []
     sequences = []
 
     insertions_merged_subset = subset_insertions(insertions_merged, num_subset=100)
     set_keys = flatten_keys_to_set(insertions_merged.keys())
 
     cache_score = defaultdict(int)
     for m in io.read_jsonl(path_sample):
         cssplits = m["CSSPLIT"].split(",")
-        if not any(True for i in set_keys if cssplits[i].startswith("+")):
+
+        # Skip if there is no insertion
+        if all(not cssplits[i].startswith("+") for i in set_keys):
             continue
 
         score = [0] * len(insertions_merged)
         sequence = ["N"] * len(insertions_merged)
         for i, (idx_grouped, insertions) in enumerate(insertions_merged.items()):
             for idx in idx_grouped:
                 if not cssplits[idx].startswith("+"):
                     continue
 
+                # Use the cache if there is already a precomputed value
+                if (idx, cssplits[idx]) in cache_score:
+                    score[i] = cache_score[(idx, cssplits[idx])]
+                    sequence[i] = cssplits[idx]
+                    continue
+
+                # Record the insertion sequence and count if the sample and insertion sequences are the same
                 for seqs, count in insertions.items():
                     if cssplits[idx] in seqs:
                         score[i] = count
                         sequence[i] = cssplits[idx]
+                        cache_score[(idx, cssplits[idx])] = count
                         continue
 
-                if (idx, cssplits[idx]) in cache_score:
-                    score[i] = cache_score[(idx, cssplits[idx])]
-                    sequence[i] = cssplits[idx]
-                    continue
-
                 flag_break = False
                 for seqs, count in insertions_merged_subset[idx_grouped].items():
                     for _, distance, _ in process.extract_iter(
                         remove_non_alphabets(cssplits[idx]), seqs, scorer=DamerauLevenshtein.normalized_distance
                     ):
+                        # Record the insertion sequence and count if the sample and insertion sequences are similar
                         if distance < 0.1:
                             score[i] = count
                             sequence[i] = cssplits[idx]
                             flag_break = True
                             break
+
                     if flag_break:
                         cache_score[(idx, cssplits[idx])] = count
                         break
 
         if any(score):
             scores.append(score)
             sequences.append(",".join(sequence))
 
     return [(score, sequence) for score, sequence in zip(scores, sequences)]
 
 
 def filter_minor_label(
-    path_sample: str,
     labels: list[int],
     insertions_scores_sequences: list[tuple[list[int], str]],
+    coverage: int,
     threshold: float = 0.5,
-) -> tuple(list[int], list[str]):
-    coverage = io.count_newlines(path_sample)
-    _, counts = np.unique(labels, return_counts=True)
-    minor_labels = {label for label, count in enumerate(counts) if count / coverage * 100 < threshold}
+) -> tuple[list[int], list[str]]:
+    labels_, counts_ = np.unique(labels, return_counts=True)
+    minor_labels = {label for label, count in zip(labels_, counts_) if count < coverage * threshold // 100}
     index_minor_labels = {i for i, label in enumerate(labels) if label in minor_labels}
     labels_filtered = [label for i, label in enumerate(labels) if i not in index_minor_labels]
     score_seq_filterd = [
         score_seq for i, score_seq in enumerate(insertions_scores_sequences) if i not in index_minor_labels
     ]
     return labels_filtered, score_seq_filterd
 
@@ -314,25 +338,25 @@
             continue
         cs_tags.append(sam.split("\t")[-1])
         positions.append(int(sam.split("\t")[3]))
     return cs_tags, positions
 
 
 def mapping_insertion(
-    TEMPDIR: Path, SAMPLE_NAME: str, cs_transposed: list[str], consensus_length: int
+    TEMPDIR: Path, SAMPLE_NAME: str, cs_transposed: list[str], consensus_length: int, uuid4: str
 ) -> Generator[str]:
     # Temporarily cache the reference sequence
     cs_insertion = next(cs for cs in cs_transposed if cs != "N" and len(cs) == consensus_length)
     ref_seq = cstag.to_sequence(convert_cssplits_to_cstag([cs_insertion]))
 
-    path_reference = Path(TEMPDIR, SAMPLE_NAME, "fasta", f"reference-{str(uuid.uuid4())}.fasta")
+    path_reference = Path(TEMPDIR, SAMPLE_NAME, "fasta", f"reference-{uuid4}.fasta")
     Path(path_reference).write_text(f">reference_insertion\n{ref_seq}\n")
 
     # Temporarily cache the query sequences
-    path_query = Path(TEMPDIR, SAMPLE_NAME, "fasta", f"query-{str(uuid.uuid4())}.fasta")
+    path_query = Path(TEMPDIR, SAMPLE_NAME, "fasta", f"query-{uuid4}.fasta")
     with Path(path_query).open("w") as file:
         for i, cs_insertion in enumerate(cs_transposed):
             que_seq = cstag.to_sequence(convert_cssplits_to_cstag([cs_insertion]))
             file.write(f">query_insertion_{i}\n{que_seq}\n")
 
     # Switch the mappy settings to either long-read or short-read, depending on the length of the reference sequence
     if len(ref_seq) > 500:
@@ -363,15 +387,15 @@
         consensus_length = max(count_cs, key=count_cs.get)
         count_consensus = sum(1 for cs in cs_transposed if len(cs) == consensus_length)
 
         if count_N > count_consensus:
             consensus_insertion.append("N")
             continue
 
-        sam_insertions = mapping_insertion(TEMPDIR, SAMPLE_NAME, cs_transposed, consensus_length)
+        sam_insertions = mapping_insertion(TEMPDIR, SAMPLE_NAME, cs_transposed, consensus_length, str(uuid.uuid4()))
 
         cs_tags, positions = get_cstag_position(sam_insertions)
         if cs_tags == []:  # When not mapped at all, append `N`.
             consensus_insertion.append("N")
         else:
             cs_insertion_consensus = cstag.to_sequence(cstag.consensus(cs_tags, positions))
             cs_last = Counter(cs.split("|")[-1] for cs in cs_transposed if len(cs) == consensus_length).most_common()[
@@ -380,72 +404,55 @@
             cssplits_insertion_consensus = "|".join("+" + cs for cs in cs_insertion_consensus[:-1]) + "|" + cs_last
             consensus_insertion.append(cssplits_insertion_consensus)
 
     return ",".join(consensus_insertion)
 
 
 def remove_all_n(cons_sequence: dict[int, str]) -> dict[int, str]:
+    """Remove all `N` sequences."""
     cons_sequence_removed = dict()
     for label, seq in cons_sequence.items():
         if all(True if s == "N" else False for s in seq.split(",")):
             continue
         cons_sequence_removed[label] = seq
     return cons_sequence_removed
 
 
-def update_labels(d: dict, FASTA_ALLELES: dict) -> dict:
-    """
-    Update labels to avoid duplicating user-specified alleles
-    (insertion1 -> insertion01 -> insertion001...)
-    """
-    user_defined_alleles = set(FASTA_ALLELES)
-    d_values = list(d.values())
-    len_d = len(d_values)
-    digits_up = 0
-    while True:
-        digits = len(str(len_d)) + digits_up
-        d_updated = {f"insertion{i+1:0{digits}}": seq for i, seq in enumerate(d_values)}
-        if user_defined_alleles.isdisjoint(set(d_updated)):
-            break
-        digits_up += 1
-    return d_updated
-
-
-def call_consensus_of_insertion(
-    TEMPDIR: Path, SAMPLE_NAME: str, FASTA_ALLELES: dict, insertion_sequences_subset: list[dict]
-) -> dict[int, str]:
+def call_consensus_of_insertion(TEMPDIR: Path, SAMPLE_NAME: str, insertion_sequences_subset: list[dict]) -> dict[int, str]:
     """Generate consensus cssplits."""
     consensus_insertion_cssplits = dict()
     insertion_sequences_subset.sort(key=lambda x: x["LABEL"])
     for label, group in groupby(insertion_sequences_subset, key=lambda x: x["LABEL"]):
         cssplits = [cs["CSSPLIT"].split(",") for cs in group]
         consensus_insertion_cssplits[label] = generate_consensus_insertions(TEMPDIR, SAMPLE_NAME, cssplits)
 
-    return update_labels(remove_all_n(consensus_insertion_cssplits), FASTA_ALLELES)
+    return remove_all_n(consensus_insertion_cssplits)
 
 
 ###########################################################
 # Generate cstag and FASTA
 ###########################################################
 
 
 def extract_index_of_insertions(
-    insertions: dict[int, dict[str, int]], insertions_merged: dict[tuple(int), dict[tuple[str], int]]
+    insertions: dict[int, dict[str, int]], insertions_merged: dict[tuple[int], dict[tuple[str], int]]
 ) -> list[int]:
     """`insertions_merged` contains multiple surrounding indices for a single insertion allele. Among them, select the one index where the insertion allele is most frequent."""
     index_of_insertions = []
+    max_idx = -1
     for idx_group in insertions_merged:
         max_val = -1
         for idx in idx_group:
             if idx not in insertions:
                 continue
             if max_val < sum(insertions[idx].values()):
                 max_val = sum(insertions[idx].values())
                 max_idx = idx
-        index_of_insertions.append(max_idx)
+        if max_idx != -1:
+            index_of_insertions.append(max_idx)
     return index_of_insertions
 
 
 def generate_cstag(
     consensus_of_insertions: dict[str, str], index_of_insertions: list[int], sequence: str
 ) -> dict[str, str]:
     cstag_insertions = dict()
@@ -463,70 +470,121 @@
 def generate_fasta(cstag_insertions: dict[str, str]) -> dict[str, str]:
     fasta_insertions = dict()
     for label, cs_tag in cstag_insertions.items():
         fasta_insertions[label] = cstag.to_sequence(cs_tag)
     return fasta_insertions
 
 
+def extract_unique_insertions(FASTA_ALLELES: dict[str, str], fasta_insertions: dict[str, str]) -> dict[str, str]:
+    """
+    Extract unique insertion alleles if they are dissimilar to the FASTA_ALLELES input by the user.
+    "Unique insertion alleles" are defined as sequences that have a difference of more than 10 bases compared to the sequences in FASTA_ALLELES
+    """
+    to_keep = []
+    for query_key, query_seq in fasta_insertions.items():
+        _, distances, _ = zip(*process.extract_iter(query_seq, FASTA_ALLELES.values(), scorer=DamerauLevenshtein.distance))
+        if all(d > 10 for d in distances):
+            to_keep.append(query_key)
+
+    return {key: fasta_insertions[key] for key in to_keep if key in fasta_insertions}
+
+
+def update_labels(d: dict, FASTA_ALLELES: dict) -> dict:
+    """
+    Update labels to avoid duplicating user-specified alleles.
+    If the allele 'insertion1' exists in FASTA_ALLELES, increment the digits.
+    (insertion1 -> insertion01 -> insertion001...)
+    """
+    user_defined_alleles = set(FASTA_ALLELES)
+    d_values = list(d.values())
+    len_d = len(d_values)
+    digits_up = 0
+    while True:
+        digits = len(str(len_d)) + digits_up
+        d_updated = {f"insertion{i+1:0{digits}}": seq for i, seq in enumerate(d_values)}
+        if user_defined_alleles.isdisjoint(set(d_updated)):
+            break
+        digits_up += 1
+    return d_updated
+
+
 ###########################################################
-# Save cstag (HTML) and fasta
+# Save cstag and fasta
 ###########################################################
 
 
 def save_fasta(TEMPDIR: Path | str, SAMPLE_NAME: str, fasta_insertions: dict[str, str]) -> None:
     for header, seq in fasta_insertions.items():
         Path(TEMPDIR, SAMPLE_NAME, "fasta", f"{header}.fasta").write_text(f">{header}\n{seq}\n")
 
 
 def save_cstag(TEMPDIR: Path | str, SAMPLE_NAME: str, cstag_insertions: dict[str, str]) -> None:
     for header, cs_tag in cstag_insertions.items():
         Path(TEMPDIR, SAMPLE_NAME, "cstag", f"{header}.txt").write_text(cs_tag + "\n")
 
-
-# def save_html(TEMPDIR: Path, SAMPLE_NAME: str, cstag_insertions: dict[int, str]) -> None:
-#     for header, cs_tag in cstag_insertions.items():
-#         html = cstag.to_html(cs_tag, f"{SAMPLE_NAME} {header}")
-#         Path(TEMPDIR, "report", "HTML", SAMPLE_NAME, f"{header}.html").write_text(html)
-
-
 ###########################################################
 # main
 ###########################################################
 
 
+def remove_temporal_files(TEMPDIR: Path, SAMPLE_NAME: str) -> None:
+    _ = [path.unlink() for path in Path(TEMPDIR, SAMPLE_NAME, "fasta").glob("reference-*.fasta")]
+    _ = [path.unlink() for path in Path(TEMPDIR, SAMPLE_NAME, "fasta").glob("query-*.fasta")]
+
+
 def generate_insertion_fasta(TEMPDIR, SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES) -> None:
     PATH_SAMPLE = Path(TEMPDIR, SAMPLE_NAME, "midsv", "control.json")
     PATH_CONTROL = Path(TEMPDIR, CONTROL_NAME, "midsv", "control.json")
-    SEQUENCE = FASTA_ALLELES["control"]
     MUTATION_LOCI = io.load_pickle(Path(TEMPDIR, SAMPLE_NAME, "mutation_loci", "control.pickle"))
 
     insertions = extract_insertions(PATH_SAMPLE, PATH_CONTROL, MUTATION_LOCI)
     if insertions == dict():
+        """If there is no insertion, return None"""
+        return None
+
+    coverage: int = io.count_newlines(PATH_SAMPLE)
+
+    insertions_merged = merge_similar_insertions(insertions, MUTATION_LOCI, coverage, threshold=0.5)
+    if all(True if v == {} else False for v in insertions_merged.values()):
+        """"If all the insertion alleles were minor, return None"""
         return None
-    insertions_merged = merge_similar_insertions(insertions, MUTATION_LOCI)
+
+    # Clustering similar insertion alleles
     insertions_scores_sequences = extract_score_and_sequence(PATH_SAMPLE, insertions_merged)
-    labels = clustering_insertions([cssplit for _, cssplit in insertions_scores_sequences])
+    cssplits_insertion = [cssplit for _, cssplit in insertions_scores_sequences]
+    labels = clustering_insertions(cssplits_insertion, n_decoy=1000)
     labels_filtered, insertion_scores_sequences_filtered = filter_minor_label(
-        PATH_SAMPLE, labels, insertions_scores_sequences, threshold=0.5
+        labels, insertions_scores_sequences, coverage, threshold=0.5
     )
+
+    # Consensus calling
     insertion_sequences_subset = subset_sequences(
         [seq for _, seq in insertion_scores_sequences_filtered], labels_filtered, num=1000
     )
-    consensus_of_insertions = call_consensus_of_insertion(
-        TEMPDIR, SAMPLE_NAME, FASTA_ALLELES, insertion_sequences_subset
-    )
+    consensus_of_insertions = call_consensus_of_insertion(TEMPDIR, SAMPLE_NAME, insertion_sequences_subset)
     if consensus_of_insertions == dict():
         """
         If there is no insertion sequence, return None
         It is possible when all insertion sequence annotated as `N` that is filtered out
         """
+        remove_temporal_files(TEMPDIR, SAMPLE_NAME)
         return None
+
+    # Format the insertion sequences as cstag and fasta
     index_of_insertions = extract_index_of_insertions(insertions, insertions_merged)
-    cstag_insertions = generate_cstag(consensus_of_insertions, index_of_insertions, SEQUENCE)
+    cstag_insertions = generate_cstag(consensus_of_insertions, index_of_insertions, FASTA_ALLELES["control"])
     fasta_insertions = generate_fasta(cstag_insertions)
+    fasta_insertions_unique = extract_unique_insertions(FASTA_ALLELES, fasta_insertions)
 
-    save_fasta(TEMPDIR, SAMPLE_NAME, fasta_insertions)
-    save_cstag(TEMPDIR, SAMPLE_NAME, cstag_insertions)
-    # save_html(TEMPDIR, SAMPLE_NAME, cstag_insertions)
+    if fasta_insertions_unique == dict():
+        remove_temporal_files(TEMPDIR, SAMPLE_NAME)
+        return None
 
-    _ = [path.unlink() for path in Path(TEMPDIR, SAMPLE_NAME, "fasta").glob("reference-*.fasta")]
-    _ = [path.unlink() for path in Path(TEMPDIR, SAMPLE_NAME, "fasta").glob("query-*.fasta")]
+    # Update labels
+    cstag_insertions_update = {key: cstag_insertions[key] for key in fasta_insertions_unique.keys()}
+    cstag_insertions_update = update_labels(cstag_insertions_update, FASTA_ALLELES)
+    fasta_insertions_update = update_labels(fasta_insertions_unique, FASTA_ALLELES)
+
+    save_cstag(TEMPDIR, SAMPLE_NAME, cstag_insertions_update)
+    save_fasta(TEMPDIR, SAMPLE_NAME, fasta_insertions_update)
+
+    remove_temporal_files(TEMPDIR, SAMPLE_NAME)
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/mutation_extractor.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/mutation_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 config.set_warnings_ignore()
 
 
 import numpy as np
 from sklearn.cluster import MiniBatchKMeans
 
 from DAJIN2.utils import io
-from DAJIN2.core.preprocess import homopolymer_handler
+from DAJIN2.core.preprocess.homopolymer_handler import extract_sequence_errors_in_homopolymer_loci
 
 
 def count_indels(midsv_sample: Generator[dict], sequence: str) -> dict[str, list[int]]:
     len_sequence = len(sequence)
     count = {"=": [0] * len_sequence, "+": [0] * len_sequence, "-": [0] * len_sequence, "*": [0] * len_sequence}
     for samp in midsv_sample:
         for i, cs in enumerate(samp["CSSPLIT"].split(",")):
@@ -80,58 +80,73 @@
 
 
 ###########################################################
 # Extract Anomalous Loci
 ###########################################################
 
 
-def cosine_similarity(x, y):
-    return np.dot(x, y) / (np.linalg.norm(x) * np.linalg.norm(y))
+def cosine_distance(x: list[float], y: list[float]) -> float:
+    # Add 1e-6 to avoid division by zero when calculating cosine similarity
+    x = np.array(x) + 1e-6
+    y = np.array(y) + 1e-6
+    return 1 - float(np.dot(x, y) / (np.linalg.norm(x) * np.linalg.norm(y)))
 
 
-def identify_dissimilar_loci(values_sample, values_control, index: int, is_consensus: bool = False) -> int:
+def is_dissimilar_loci(values_sample, values_control, index: int, is_consensus: bool = False) -> bool:
     # If 'sample' has more than 20% variation compared to 'control' in consensus mode, unconditionally set it to 'dissimilar loci'. This is set to counteract cases where, when evaluating cosine similarity during significant deletions, values exceedingly close to 1 can occur even if not observed in the control (e.g., control = [1,1,1,1,1], sample = [100,100,100,100,100] -> cosine similarity = 1).
-    if is_consensus and values_sample[index] - values_control[index] > 20:
-        return True
+    if values_sample[index] - values_control[index] > 20:
+        if is_consensus:
+            if values_sample[index] > 75:
+                return True
+        else:
+            return True
+
+    # Subset 10 bases around index.
+    x = values_sample[index : index + 10]
+    y = values_control[index : index + 10]
 
-    # Subset 10 bases around index and add 1e-6 to avoid division by zero when calculating cosine similarity.
-    x = np.array(values_sample[index - 5 : index + 6]) + 1e-6
-    y = np.array(values_control[index - 5 : index + 6]) + 1e-6
+    x_slice = values_sample[index + 1 : index + 11]
+    y_slice = values_control[index + 1 : index + 11]
 
-    return cosine_similarity(x, y) < 0.95
+    distance = cosine_distance(x, y)
+    distance_slice = cosine_distance(x_slice, y_slice)
+
+    return distance > 0.05 and distance / (distance + distance_slice) > 0.9
 
 
 def detect_anomalies(values_sample, values_control, threshold: float, is_consensus: bool = False) -> set[int]:
     """
     Detect anomalies and return indices of outliers.
     """
     values_subtract = values_sample - values_control
     values_subtract = np.where(values_subtract <= threshold, 0, values_subtract)
 
     values_subtract_reshaped = values_subtract.reshape(-1, 1)
     kmeans = MiniBatchKMeans(n_clusters=2, random_state=0, n_init="auto").fit(values_subtract_reshaped)
-    threshold_kmeans = kmeans.cluster_centers_.mean()
+    # Set the maximum threshold to 10 to prevent missing relatively minor mutations due to the k-means centers being overly influenced by obvious mutations.
+    threshold_kmeans = min(20, kmeans.cluster_centers_.mean())
     candidate_loci = {i for i, v in enumerate(values_subtract_reshaped) if v > threshold_kmeans}
 
-    return {i for i in candidate_loci if identify_dissimilar_loci(values_sample, values_control, i, is_consensus)}
+    return {i for i in candidate_loci if is_dissimilar_loci(values_sample, values_control, i, is_consensus)}
 
 
 def extract_anomal_loci(
     indels_normalized_sample,
     indels_normalized_control,
     thresholds: dict[str, float],
     is_consensus: bool = False,
 ) -> dict[str, set[int]]:
-    results = dict()
+    """Extract outlier loci compareing indel counts between sample and control."""
+    anomal_loci = dict()
     for mut in {"+", "-", "*"}:
         values_sample = indels_normalized_sample[mut]
         values_control = indels_normalized_control[mut]
         idx_outliers = detect_anomalies(values_sample, values_control, thresholds[mut], is_consensus)
-        results[mut] = idx_outliers
-    return results
+        anomal_loci[mut] = idx_outliers
+    return anomal_loci
 
 
 ###########################################################
 # Homolopolymer region
 ###########################################################
 
 
@@ -273,20 +288,20 @@
     is_consensus: bool = False,
 ) -> list[set[str]]:
     indels_normalized_sample = io.load_pickle(path_indels_normalized_sample)
     indels_normalized_control = io.load_pickle(path_indels_normalized_control)
 
     """Extract candidate mutation loci"""
     indels_normalized_minimize_control = minimize_mutation_counts(indels_normalized_control, indels_normalized_sample)
-    anomal_loci = extract_anomal_loci(
+    anomal_loci: dict[str, set[int]] = extract_anomal_loci(
         indels_normalized_sample, indels_normalized_minimize_control, thresholds, is_consensus
     )
 
     """Extract error loci in homopolymer regions"""
-    errors_in_homopolymer = homopolymer_handler.extract_errors(
+    errors_in_homopolymer = extract_sequence_errors_in_homopolymer_loci(
         sequence, indels_normalized_sample, indels_normalized_control, anomal_loci
     )
     mutation_loci = discard_errors_in_homopolymer(anomal_loci, errors_in_homopolymer)
 
     """Merge all mutations and knockin loci"""
     if path_knockin.exists():
         knockin_loci = io.load_pickle(path_knockin)
@@ -315,12 +330,12 @@
         if not Path(path_mutation_control, file_name).exists():
             file_name = f"{allele}_normalized.pickle"
         path_indels_normalized_control = Path(path_mutation_control, file_name)
 
         path_indels_normalized_sample = Path(path_mutation_sample, f"{allele}_normalized.pickle")
         path_knockin = Path(ARGS.tempdir, ARGS.sample_name, "knockin_loci", f"{allele}.pickle")
 
-        mutation_loci = extract_mutation_loci(
+        mutation_loci: list[set[str]] = extract_mutation_loci(
             sequence, path_indels_normalized_sample, path_indels_normalized_control, path_knockin
         )
 
         io.save_pickle(mutation_loci, path_output)
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/directory_manager.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/directory_manager.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/__init__.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/__init__.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/input_formatter.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/input_formatter.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/genome_fetcher.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/genome_fetcher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 from __future__ import annotations
 
+import ssl
 from urllib.request import urlopen
 
 
+def fetch_html_without_verification(url: str) -> str:
+    context = ssl._create_unverified_context()  # Create an SSL context that temporarily disables verification
+    with urlopen(url, context=context, timeout=10) as response:
+        return response.read().decode("utf-8").split("\n")
+
+
 def fetch_seq_coordinates(genome: str, blat_url: str, seq: str) -> dict:
     url = f"{blat_url}?db={genome}&type=BLAT&userSeq={seq}"
-    records = urlopen(url).read().decode("utf8").split("\n")
+    records = fetch_html_without_verification(url)
     matches = []
     for record in records:
         if "100.0%" not in record:
             continue
         record_trim = [r for r in record.split(" ") if r]
         if record_trim[-1] == str(len(seq)):
             matches = record_trim
@@ -39,13 +46,13 @@
 
 
 def fetch_chromosome_size(genome_coordinates: dict, genome_urls: dict) -> int:
     chrom = genome_coordinates["chrom"]
     genome = genome_coordinates["genome"]
     url = f"{genome_urls['goldenpath']}/{genome}/bigZips/{genome}.chrom.sizes"
 
-    response = urlopen(url).read().decode("utf8").split("\n")
-    for line in response:
-        chrom_name, size = line.split("\t")
+    records = fetch_html_without_verification(url)
+    for record in records:
+        chrom_name, size = record.split("\t")
         if chrom == chrom_name:
             return int(size)
     raise ValueError(f"Chromosome {chrom} size not found.")
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/mapping.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/mapping.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/preprocess/cache_checker.py` & `dajin2-0.4.6/src/DAJIN2/core/preprocess/cache_checker.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/classification/allele_merger.py` & `dajin2-0.4.6/src/DAJIN2/core/classification/allele_merger.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/classification/classifier.py` & `dajin2-0.4.6/src/DAJIN2/core/classification/classifier.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/label_extractor.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/label_extractor.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/score_handler.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/score_handler.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/kmer_generator.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/kmer_generator.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/clustering.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/clustering.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/appender.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/appender.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/label_updator.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/label_updator.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/label_merger.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/label_merger.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/clustering/strand_bias_handler.py` & `dajin2-0.4.6/src/DAJIN2/core/clustering/strand_bias_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 This module provides functions to determine whether each allele obtained after clustering is formed due to sequencing errors caused by strand bias.
 
 Re-allocates reads belonging to clusters with strand bias to clusters without strand bias.
 """
 
 from pathlib import Path
+from typing import Generator
 from collections import defaultdict
 from sklearn.tree import DecisionTreeClassifier
 
 from DAJIN2.utils import io
 
 # Constants
 STRAND_BIAS_LOWER_LIMIT = 0.1
@@ -36,40 +37,47 @@
 
 ###############################################################################
 # Handle Strand bias
 # # Clusters of reads with mutations with strand bias are merged into similar clusters without strand bias
 ###############################################################################
 
 
-def count_strand(labels: list[int], samples: list[dict[str, str]]) -> tuple[dict[str, int], dict[str, int]]:
+def count_strand(labels: list[int], samples: Generator[dict[str, str]]) -> tuple[dict[str, int], dict[str, int]]:
     """Count the occurrences of each strand type by label."""
     positive_strand_counts_by_labels = defaultdict(int)
     total_counts_by_labels = defaultdict(int)
 
     for label, sample in zip(labels, samples):
         total_counts_by_labels[label] += 1
         if sample["STRAND"] == "+":
             positive_strand_counts_by_labels[label] += 1
 
     return dict(positive_strand_counts_by_labels), dict(total_counts_by_labels)
 
 
 def determine_strand_biases(
-    positive_strand_counts_by_labels: defaultdict, total_counts_by_labels: defaultdict
+    positive_strand_counts_by_labels: dict[str, int], total_counts_by_labels: dict[str, int]
 ) -> dict[int, bool]:
     """Determine strand biases based on positive strand counts."""
     strand_biases = {}
     for label, total in total_counts_by_labels.items():
-        positive_strand_count = positive_strand_counts_by_labels[label]
+        positive_strand_count = positive_strand_counts_by_labels.get(label, 0)
         strand_ratio = positive_strand_count / total
         strand_biases[label] = not (STRAND_BIAS_LOWER_LIMIT < strand_ratio < STRAND_BIAS_UPPER_LIMIT)
 
     return strand_biases
 
 
+def annotate_strand_bias_by_labels(path_sample: Path, labels: list[int]) -> bool:
+    """Determine whether there is strand bias in the samples based on the provided labels."""
+    samples = io.read_jsonl(path_sample)
+    positive_strand_counts_by_labels, total_counts_by_labels = count_strand(labels, samples)
+    return determine_strand_biases(positive_strand_counts_by_labels, total_counts_by_labels)
+
+
 def prepare_training_testing_sets(labels, scores, strand_biases) -> tuple[list, list, list]:
     """Prepare training and testing datasets based on strand biases."""
     train_data, train_labels, test_data = [], [], []
     for label, score in zip(labels, scores):
         if strand_biases[label]:
             test_data.append(score)
         else:
@@ -92,24 +100,27 @@
         if strand_biases[label]:
             labels[i] = next(label_predictions)
     return labels
 
 
 def remove_biased_clusters(path_sample: Path, path_score_sample: Path, labels: list[int]) -> list[int]:
     """Remove clusters with strand bias by re-labeling based on decision tree predictions.
-    Continue until at least one of the samples exhibits strand bias (i.e., do not calculate if all samples exhibit strand bias, or conversely, if none of the samples exhibit strand bias) or
+    Continue until at least one of the samples exhibits strand bias (i.e., do not calculate if all samples exhibit strand bias or, if none of the samples exhibit strand bias) and
     1000 iterations are reached, which serves as a safeguard to prevent infinite loops.
     """
-    samples = io.read_jsonl(path_sample)
-    positive_strand_counts_by_labels, total_counts_by_labels = count_strand(labels, samples)
-    strand_biases = determine_strand_biases(positive_strand_counts_by_labels, total_counts_by_labels)
+    strand_biases = annotate_strand_bias_by_labels(path_sample, labels)
 
     iteration_count = 0
     labels_corrected = labels
     while len(set(strand_biases.values())) > 1 and iteration_count < 1000:
+        # Re-allocation of labels of biased clusters to unbiased clusters
         scores = io.read_jsonl(path_score_sample)
         train_data, train_labels, test_data = prepare_training_testing_sets(labels, scores, strand_biases)
         dtree = train_decision_tree(train_data, train_labels)
         labels_corrected = allocate_labels(labels, strand_biases, dtree, test_data)
-        strand_biases = determine_strand_biases(labels_corrected, path_sample)
+
+        # Re-calculate strand biases based on the corrected labels
+        strand_biases = annotate_strand_bias_by_labels(path_sample, labels)
+
         iteration_count += 1
+
     return labels_corrected
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/report/bam_exporter.py` & `dajin2-0.4.6/src/DAJIN2/core/report/bam_exporter.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/report/mutation_exporter.py` & `dajin2-0.4.6/src/DAJIN2/core/report/mutation_exporter.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/report/insertion_reflector.py` & `dajin2-0.4.6/src/DAJIN2/core/report/insertion_reflector.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/report/sequence_exporter.py` & `dajin2-0.4.6/src/DAJIN2/core/report/sequence_exporter.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/consensus/consensus.py` & `dajin2-0.4.6/src/DAJIN2/core/consensus/consensus.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/consensus/name_handler.py` & `dajin2-0.4.6/src/DAJIN2/core/consensus/name_handler.py`

 * *Files identical despite different names*

## Comparing `dajin2-0.4.5/src/DAJIN2/core/consensus/mutation_extractor.py` & `dajin2-0.4.6/src/DAJIN2/core/consensus/mutation_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,17 @@
 def cache_normalized_indels(ARGS, path_midsv_sample: Path) -> None:
     allele, label, *_ = path_midsv_sample.stem.split("_")
     sequence = ARGS.fasta_alleles[allele]
 
     path_midsv_control = extract_path_control(ARGS, allele)
     path_midsv_n_filtered_control = extract_path_n_filtered_control(ARGS, path_midsv_control)
 
-    cache_selected_control_by_similarity(path_midsv_n_filtered_control, path_midsv_sample, path_midsv_sample.parent)
+    cache_selected_control_by_similarity(
+        ARGS, path_midsv_n_filtered_control, path_midsv_sample, path_midsv_sample.parent
+    )
 
     path_midsv_similar_control = Path(path_midsv_sample.parent, f"{allele}_{label}_control.jsonl")
 
     _, indels_normalized_sample = summarize_indels(path_midsv_sample, sequence)
     _, indels_normalized_control = summarize_indels(path_midsv_similar_control, sequence)
 
     path_consensus = Path(ARGS.tempdir, ARGS.sample_name, "consensus")
```

## Comparing `dajin2-0.4.5/src/DAJIN2/core/consensus/similarity_searcher.py` & `dajin2-0.4.6/src/DAJIN2/core/consensus/similarity_searcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,32 +68,42 @@
 
 
 ###########################################################
 # main
 ###########################################################
 
 
-def filter_control(path_midsv_control: Path, path_midsv_sample: Path) -> list[bool]:
+def filter_control(ARGS, path_midsv_control: Path, path_midsv_sample: Path) -> list[bool]:
     """
     find similar control reads compared to sample reads
     """
     cssplits = (m["CSSPLIT"].split(",") for m in io.read_jsonl(path_midsv_sample))
     coverage_match = np.array([sum(1 for cs in cssplit if cs.startswith("=")) for cssplit in zip(*cssplits)])
     mut_onehot_sample = onehot_by_mutations(io.read_jsonl(path_midsv_sample))
-    mut_onehot_control = onehot_by_mutations(io.read_jsonl(path_midsv_control))
+
+    path_mut_onehot_control = Path(
+        ARGS.tempdir, ARGS.control_name, "consensus", f"{path_midsv_control.stem}_onehot.pickle"
+    )
+    if path_mut_onehot_control.exists():
+        mut_onehot_control = io.load_pickle(path_mut_onehot_control)
+    else:
+        mut_onehot_control = onehot_by_mutations(io.read_jsonl(path_midsv_control))
+        io.save_pickle(mut_onehot_control, path_mut_onehot_control)
 
     mut_percentage_sample = calculate_percentage(mut_onehot_sample, coverage_match)
     values_mask = get_values_to_mask(mut_percentage_sample)
 
     mut_onehot_sample_masked = apply_mask(mut_onehot_sample, values_mask)
     mut_onehot_control_masked = apply_mask(mut_onehot_control, values_mask)
 
     return identify_normal_reads(mut_onehot_sample_masked, mut_onehot_control_masked)
 
 
-def cache_selected_control_by_similarity(path_midsv_control: Path, path_midsv_sample: Path, path_output: Path) -> None:
-    normal_reads_flags = filter_control(path_midsv_control, path_midsv_sample)
+def cache_selected_control_by_similarity(
+    ARGS, path_midsv_control: Path, path_midsv_sample: Path, path_output: Path
+) -> None:
+    normal_reads_flags = filter_control(ARGS, path_midsv_control, path_midsv_sample)
     midsv_control = io.read_jsonl(path_midsv_control)
     midsv_filtered = (m for m, flag in zip(midsv_control, normal_reads_flags) if flag is True)
 
     allele, label, *_ = Path(path_midsv_sample).stem.split("_")
     io.write_jsonl(midsv_filtered, Path(path_output, f"{allele}_{label}_control.jsonl"))
```

