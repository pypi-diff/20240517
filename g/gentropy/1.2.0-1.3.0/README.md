# Comparing `tmp/gentropy-1.2.0.tar.gz` & `tmp/gentropy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentropy-1.2.0.tar", max compression
+gzip compressed data, was "gentropy-1.3.0.tar", max compression
```

## Comparing `gentropy-1.2.0.tar` & `gentropy-1.3.0.tar`

### file list

```diff
@@ -1,111 +1,115 @@
--rw-r--r--   0        0        0    10947 2024-03-07 16:25:14.349979 gentropy-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     2372 2024-03-07 16:25:14.349979 gentropy-1.2.0/README.md
--rw-r--r--   0        0        0     8597 2024-03-07 16:25:15.349968 gentropy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       87 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/__init__.py
--rw-r--r--   0        0        0       69 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/__init__.py
--rw-r--r--   0        0        0       59 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/data/__init__.py
--rw-r--r--   0        0        0    19674 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/data/gwas_pValueText_map.json
--rw-r--r--   0        0        0      555 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/data/gwas_population_2_LD_panel_map.json
--rw-r--r--   0        0        0       66 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/__init__.py
--rw-r--r--   0        0        0     1323 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/andersson2014.json
--rw-r--r--   0        0        0     1351 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/colocalisation.json
--rw-r--r--   0        0        0     1207 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/gene_index.json
--rw-r--r--   0        0        0     1125 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/intervals.json
--rw-r--r--   0        0        0      483 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/l2g_feature.json
--rw-r--r--   0        0        0     2553 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/l2g_feature_matrix.json
--rw-r--r--   0        0        0      788 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/l2g_gold_standard.json
--rw-r--r--   0        0        0      365 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/l2g_predictions.json
--rw-r--r--   0        0        0     1460 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/ld_index.json
--rw-r--r--   0        0        0     4765 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/study_index.json
--rw-r--r--   0        0        0     4487 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/study_locus.json
--rw-r--r--   0        0        0     2190 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/study_locus_overlap.json
--rw-r--r--   0        0        0     1169 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/summary_statistics.json
--rw-r--r--   0        0        0     1379 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/v2g.json
--rw-r--r--   0        0        0     5055 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/variant_annotation.json
--rw-r--r--   0        0        0     3471 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/assets/schemas/variant_index.json
--rw-r--r--   0        0        0      546 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/cli.py
--rw-r--r--   0        0        0     2875 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/clump.py
--rw-r--r--   0        0        0     1581 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/colocalisation.py
--rw-r--r--   0        0        0     6486 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/common/Liftover.py
--rw-r--r--   0        0        0       83 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/common/__init__.py
--rw-r--r--   0        0        0     2465 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/common/schemas.py
--rw-r--r--   0        0        0     6315 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/common/session.py
--rw-r--r--   0        0        0    14021 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/common/spark_helpers.py
--rw-r--r--   0        0        0    13310 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/common/utils.py
--rw-r--r--   0        0        0    12946 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/config.py
--rw-r--r--   0        0        0       72 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/__init__.py
--rw-r--r--   0        0        0      704 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/colocalisation.py
--rw-r--r--   0        0        0     6834 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/dataset.py
--rw-r--r--   0        0        0     2030 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/gene_index.py
--rw-r--r--   0        0        0     3595 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/intervals.py
--rw-r--r--   0        0        0      652 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/l2g_feature.py
--rw-r--r--   0        0        0     5970 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/l2g_feature_matrix.py
--rw-r--r--   0        0        0     7925 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/l2g_gold_standard.py
--rw-r--r--   0        0        0     3402 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/l2g_prediction.py
--rw-r--r--   0        0        0      674 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/ld_index.py
--rw-r--r--   0        0        0     6627 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/study_index.py
--rw-r--r--   0        0        0    19875 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/study_locus.py
--rw-r--r--   0        0        0     2354 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/study_locus_overlap.py
--rw-r--r--   0        0        0     4230 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/summary_statistics.py
--rw-r--r--   0        0        0     1605 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/v2g.py
--rw-r--r--   0        0        0     8184 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/variant_annotation.py
--rw-r--r--   0        0        0     2597 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/dataset/variant_index.py
--rw-r--r--   0        0        0       65 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/datasource/__init__.py
--rw-r--r--   0        0        0       77 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/datasource/eqtl_catalogue/__init__.py
--rw-r--r--   0        0        0    12453 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/datasource/eqtl_catalogue/finemapping.py
--rw-r--r--   0        0        0     5619 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/datasource/eqtl_catalogue/study_index.py
--rw-r--r--   0        0        0     3535 2024-03-07 16:25:14.365979 gentropy-1.2.0/src/gentropy/datasource/eqtl_catalogue/summary_stats.py
--rw-r--r--   0        0        0       70 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/finngen/__init__.py
--rw-r--r--   0        0        0    13789 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/finngen/finemapping.py
--rw-r--r--   0        0        0     3182 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/finngen/study_index.py
--rw-r--r--   0        0        0     3648 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/finngen/summary_stats.py
--rw-r--r--   0        0        0       68 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gnomad/__init__.py
--rw-r--r--   0        0        0    17560 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gnomad/ld.py
--rw-r--r--   0        0        0     7199 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gnomad/variants.py
--rw-r--r--   0        0        0       68 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/__init__.py
--rw-r--r--   0        0        0    48291 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/associations.py
--rw-r--r--   0        0        0    29805 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/study_index.py
--rw-r--r--   0        0        0     4931 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/study_splitter.py
--rw-r--r--   0        0        0     7037 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/summary_statistics.py
--rw-r--r--   0        0        0       62 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/intervals/__init__.py
--rw-r--r--   0        0        0     5103 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/intervals/andersson.py
--rw-r--r--   0        0        0     6341 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/intervals/javierre.py
--rw-r--r--   0        0        0     3558 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/intervals/jung.py
--rw-r--r--   0        0        0     3657 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/intervals/thurman.py
--rw-r--r--   0        0        0       78 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/open_targets/__init__.py
--rw-r--r--   0        0        0     5046 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/open_targets/l2g_gold_standard.py
--rw-r--r--   0        0        0     3166 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/open_targets/target.py
--rw-r--r--   0        0        0       68 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/ukbiobank/__init__.py
--rw-r--r--   0        0        0     4430 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/datasource/ukbiobank/study_index.py
--rw-r--r--   0        0        0     3055 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/eqtl_catalogue.py
--rw-r--r--   0        0        0     1696 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/finngen_finemapping_ingestion.py
--rw-r--r--   0        0        0      730 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/finngen_studies.py
--rw-r--r--   0        0        0      886 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/finngen_sumstat_preprocess.py
--rw-r--r--   0        0        0      968 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/gene_index.py
--rw-r--r--   0        0        0     3689 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/gwas_catalog_ingestion.py
--rw-r--r--   0        0        0     2379 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/gwas_catalog_study_curation.py
--rw-r--r--   0        0        0     7341 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/gwas_catalog_study_inclusion.py
--rw-r--r--   0        0        0     1098 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/gwas_catalog_sumstat_preprocess.py
--rw-r--r--   0        0        0     7457 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/l2g.py
--rw-r--r--   0        0        0     1836 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/ld_based_clumping.py
--rw-r--r--   0        0        0     1056 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/ld_index.py
--rw-r--r--   0        0        0       64 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/__init__.py
--rw-r--r--   0        0        0    34684 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/carma.py
--rw-r--r--   0        0        0     2784 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/clump.py
--rw-r--r--   0        0        0    10994 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/colocalisation.py
--rw-r--r--   0        0        0       76 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/l2g/__init__.py
--rw-r--r--   0        0        0     7289 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/l2g/evaluator.py
--rw-r--r--   0        0        0    15022 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/l2g/feature_factory.py
--rw-r--r--   0        0        0    11282 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/l2g/model.py
--rw-r--r--   0        0        0     4231 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/l2g/trainer.py
--rw-r--r--   0        0        0     7178 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/ld.py
--rw-r--r--   0        0        0    11051 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/pics.py
--rw-r--r--   0        0        0    17702 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/susie_inf.py
--rw-r--r--   0        0        0    13710 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/method/window_based_clumping.py
--rw-r--r--   0        0        0     1052 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/pics.py
--rw-r--r--   0        0        0        0 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/py.typed
--rw-r--r--   0        0        0     5357 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/v2g.py
--rw-r--r--   0        0        0     1188 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/variant_annotation.py
--rw-r--r--   0        0        0     1590 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/variant_index.py
--rw-r--r--   0        0        0     2112 2024-03-07 16:25:14.369979 gentropy-1.2.0/src/gentropy/window_based_clumping.py
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 gentropy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10947 2024-05-17 13:03:00.619229 gentropy-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     2372 2024-05-17 13:03:00.619229 gentropy-1.3.0/README.md
+-rw-r--r--   0        0        0     8607 2024-05-17 13:03:04.371263 gentropy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/__init__.py
+-rw-r--r--   0        0        0       69 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/data/__init__.py
+-rw-r--r--   0        0        0    19674 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/data/gwas_pValueText_map.json
+-rw-r--r--   0        0        0      555 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/data/gwas_population_2_LD_panel_map.json
+-rw-r--r--   0        0        0       66 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/andersson2014.json
+-rw-r--r--   0        0        0     1351 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/colocalisation.json
+-rw-r--r--   0        0        0     1207 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/gene_index.json
+-rw-r--r--   0        0        0     1125 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/intervals.json
+-rw-r--r--   0        0        0      483 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/l2g_feature.json
+-rw-r--r--   0        0        0     3055 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/l2g_feature_matrix.json
+-rw-r--r--   0        0        0      788 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/l2g_gold_standard.json
+-rw-r--r--   0        0        0      365 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/l2g_predictions.json
+-rw-r--r--   0        0        0     1460 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/ld_index.json
+-rw-r--r--   0        0        0      365 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/pairwise_ld.json
+-rw-r--r--   0        0        0     4765 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/study_index.json
+-rw-r--r--   0        0        0     4816 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/study_locus.json
+-rw-r--r--   0        0        0     2190 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/study_locus_overlap.json
+-rw-r--r--   0        0        0     1169 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/summary_statistics.json
+-rw-r--r--   0        0        0     1379 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/v2g.json
+-rw-r--r--   0        0        0     4939 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/variant_annotation.json
+-rw-r--r--   0        0        0     3471 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/assets/schemas/variant_index.json
+-rw-r--r--   0        0        0      546 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/cli.py
+-rw-r--r--   0        0        0     3222 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/colocalisation.py
+-rw-r--r--   0        0        0     6486 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/common/Liftover.py
+-rw-r--r--   0        0        0       83 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/common/__init__.py
+-rw-r--r--   0        0        0     2465 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/common/schemas.py
+-rw-r--r--   0        0        0     6315 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/common/session.py
+-rw-r--r--   0        0        0    14021 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/common/spark_helpers.py
+-rw-r--r--   0        0        0    11765 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/common/utils.py
+-rw-r--r--   0        0        0    14449 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/config.py
+-rw-r--r--   0        0        0       72 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/__init__.py
+-rw-r--r--   0        0        0      704 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/colocalisation.py
+-rw-r--r--   0        0        0     6834 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/dataset.py
+-rw-r--r--   0        0        0     2030 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/gene_index.py
+-rw-r--r--   0        0        0     3595 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/intervals.py
+-rw-r--r--   0        0        0      652 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/l2g_feature.py
+-rw-r--r--   0        0        0     5971 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/l2g_feature_matrix.py
+-rw-r--r--   0        0        0     7925 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/l2g_gold_standard.py
+-rw-r--r--   0        0        0     3408 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/l2g_prediction.py
+-rw-r--r--   0        0        0      674 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/ld_index.py
+-rw-r--r--   0        0        0     3250 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/pairwise_ld.py
+-rw-r--r--   0        0        0     6627 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/study_index.py
+-rw-r--r--   0        0        0    23650 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/study_locus.py
+-rw-r--r--   0        0        0     2354 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/study_locus_overlap.py
+-rw-r--r--   0        0        0     4545 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/summary_statistics.py
+-rw-r--r--   0        0        0     1605 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/v2g.py
+-rw-r--r--   0        0        0     8184 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/variant_annotation.py
+-rw-r--r--   0        0        0     2597 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/dataset/variant_index.py
+-rw-r--r--   0        0        0       65 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/eqtl_catalogue/__init__.py
+-rw-r--r--   0        0        0    12453 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/eqtl_catalogue/finemapping.py
+-rw-r--r--   0        0        0     5619 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/eqtl_catalogue/study_index.py
+-rw-r--r--   0        0        0     3535 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/eqtl_catalogue/summary_stats.py
+-rw-r--r--   0        0        0       70 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/finngen/__init__.py
+-rw-r--r--   0        0        0    13789 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/finngen/finemapping.py
+-rw-r--r--   0        0        0     3182 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/finngen/study_index.py
+-rw-r--r--   0        0        0     3735 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/finngen/summary_stats.py
+-rw-r--r--   0        0        0       68 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/gnomad/__init__.py
+-rw-r--r--   0        0        0    19606 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/gnomad/ld.py
+-rw-r--r--   0        0        0     5479 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/gnomad/variants.py
+-rw-r--r--   0        0        0       68 2024-05-17 13:03:00.639229 gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/__init__.py
+-rw-r--r--   0        0        0    50490 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/associations.py
+-rw-r--r--   0        0        0    29536 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/study_index.py
+-rw-r--r--   0        0        0     4931 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/study_splitter.py
+-rw-r--r--   0        0        0     7037 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/summary_statistics.py
+-rw-r--r--   0        0        0       62 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/intervals/__init__.py
+-rw-r--r--   0        0        0     5103 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/intervals/andersson.py
+-rw-r--r--   0        0        0     6341 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/intervals/javierre.py
+-rw-r--r--   0        0        0     3558 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/intervals/jung.py
+-rw-r--r--   0        0        0     3658 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/intervals/thurman.py
+-rw-r--r--   0        0        0       78 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/open_targets/__init__.py
+-rw-r--r--   0        0        0     5046 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/open_targets/l2g_gold_standard.py
+-rw-r--r--   0        0        0     3166 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/open_targets/target.py
+-rw-r--r--   0        0        0       68 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/ukbiobank/__init__.py
+-rw-r--r--   0        0        0     4430 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/datasource/ukbiobank/study_index.py
+-rw-r--r--   0        0        0     3055 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/eqtl_catalogue.py
+-rw-r--r--   0        0        0     1696 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/finngen_finemapping_ingestion.py
+-rw-r--r--   0        0        0      730 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/finngen_studies.py
+-rw-r--r--   0        0        0      886 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/finngen_sumstat_preprocess.py
+-rw-r--r--   0        0        0      968 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/gene_index.py
+-rw-r--r--   0        0        0     3689 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/gwas_catalog_ingestion.py
+-rw-r--r--   0        0        0     2379 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/gwas_catalog_study_curation.py
+-rw-r--r--   0        0        0     7341 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/gwas_catalog_study_inclusion.py
+-rw-r--r--   0        0        0     1098 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/gwas_catalog_sumstat_preprocess.py
+-rw-r--r--   0        0        0     7603 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/l2g.py
+-rw-r--r--   0        0        0     1836 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/ld_based_clumping.py
+-rw-r--r--   0        0        0     1056 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/ld_index.py
+-rw-r--r--   0        0        0       64 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/__init__.py
+-rw-r--r--   0        0        0    35347 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/carma.py
+-rw-r--r--   0        0        0     2784 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/clump.py
+-rw-r--r--   0        0        0    11098 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/colocalisation.py
+-rw-r--r--   0        0        0       76 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/l2g/__init__.py
+-rw-r--r--   0        0        0     7289 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/l2g/evaluator.py
+-rw-r--r--   0        0        0    13717 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/l2g/feature_factory.py
+-rw-r--r--   0        0        0    11387 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/l2g/model.py
+-rw-r--r--   0        0        0     4171 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/l2g/trainer.py
+-rw-r--r--   0        0        0     7178 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/ld.py
+-rw-r--r--   0        0        0    11051 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/pics.py
+-rw-r--r--   0        0        0     6850 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/sumstat_imputation.py
+-rw-r--r--   0        0        0    10541 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/sumstat_quality_controls.py
+-rw-r--r--   0        0        0    17704 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/susie_inf.py
+-rw-r--r--   0        0        0    10207 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/method/window_based_clumping.py
+-rw-r--r--   0        0        0     1181 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/pics.py
+-rw-r--r--   0        0        0        0 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/py.typed
+-rw-r--r--   0        0        0    47204 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/susie_finemapper.py
+-rw-r--r--   0        0        0     5357 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/v2g.py
+-rw-r--r--   0        0        0     1188 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/variant_annotation.py
+-rw-r--r--   0        0        0     1590 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/variant_index.py
+-rw-r--r--   0        0        0     2502 2024-05-17 13:03:00.643229 gentropy-1.3.0/src/gentropy/window_based_clumping.py
+-rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 gentropy-1.3.0/PKG-INFO
```

### Comparing `gentropy-1.2.0/LICENSE.md` & `gentropy-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/README.md` & `gentropy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/pyproject.toml` & `gentropy-1.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gentropy"
 # !! version is managed by semantic_release
-version = "1.2.0"
+version = "1.3.0"
 description = "Open Targets python framework for post-GWAS analysis"
 authors = ["Open Targets core team"]
 license = "Apache-2.0"
 readme = "README.md"
 documentation = "https://opentargets.github.io/gentropy/"
 repository = "https://github.com/opentargets/gentropy"
 packages = [{ include = "gentropy", from = "src" }]
@@ -31,21 +31,21 @@
 google = "^3.0.0"
 omegaconf = "^2.3.0"
 typing-extensions = "^4.9.0"
 scikit-learn = "^1.3.2"
 pandas = "^2.1.4"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^3.6.0"
-mypy = "^1.8"
+pre-commit = "^3.7.0"
+mypy = "^1.10"
 pep8-naming = "^0.13.2"
-interrogate = "^1.5.0"
+interrogate = "^1.7.0"
 isort = "^5.13.2"
 darglint = "^1.8.1"
-ruff = "^0.2.0"
+ruff = "^0.4.3"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocstrings-python = "^1.8.0"
 mkdocs-material = "*"
 mkdocs-section-index = "^0.3.4"
 mkdocs-git-revision-date-localized-plugin = "^1.2.2"
@@ -54,15 +54,15 @@
 mkdocs-exclude = "^1.0.2"
 mkdocs-git-committers-plugin-2 = "^2.2.3"
 lxml = "^5.1.0"
 pymdown-extensions = "^10.7"
 
 
 [tool.poetry.group.tests.dependencies]
-pytest-cov = "^4.1.0"
+pytest-cov = ">=4.1,<6.0"
 pytest-sugar = ">=0.9.5,<1.1.0"
 dbldatagen = "^0.3.1"
 pyparsing = "^3.1.1"
 pytest = ">=7.4.4,<9.0.0"
 pytest-xdist = "^3.5.0"
 
 
@@ -70,15 +70,15 @@
 ipython = "^8.19.0"
 ipykernel = "^6.28.0"
 google-cloud-dataproc = "^5.8.0"
 apache-airflow = "^2.8.0"
 apache-airflow-providers-google = "^10.13.1"
 pydoclint = ">=0.3.8,<0.5.0"
 prettier = "^0.0.7"
-deptry = "^0.12.0"
+deptry = ">=0.12,<0.17"
 python-semantic-release = ">=8.7,<10.0"
 yamllint = "^1.33.0"
 
 [tool.semantic_release]
 logging_use_named_masks = true
 build_command = "pip install poetry && poetry build"
 assets = []
```

### Comparing `gentropy-1.2.0/src/gentropy/assets/data/gwas_pValueText_map.json` & `gentropy-1.3.0/src/gentropy/assets/data/gwas_pValueText_map.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/data/gwas_population_2_LD_panel_map.json` & `gentropy-1.3.0/src/gentropy/assets/data/gwas_population_2_LD_panel_map.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/andersson2014.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/andersson2014.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/colocalisation.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/colocalisation.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/gene_index.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/gene_index.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/intervals.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/intervals.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/l2g_feature_matrix.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/l2g_feature_matrix.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96%*

 * *Differences: {"'fields'": "{insert: [(21, OrderedDict([('metadata', OrderedDict()), ('name', "*

 * *             "'tuqtlColocClppMaximum'), ('nullable', True), ('type', 'float')])), (22, "*

 * *             "OrderedDict([('metadata', OrderedDict()), ('name', "*

 * *             "'tuqtlColocClppMaximumNeighborhood'), ('nullable', True), ('type', 'float')])), (23, "*

 * *             "OrderedDict([('metadata', OrderedDict()), ('name', 'tuqtlColocLlrMaximum'), "*

 * *             "('nullable', True), ('type', 'float')])), (24, OrderedDict([('metad […]*

```diff
@@ -121,11 +121,35 @@
             "type": "float"
         },
         {
             "metadata": {},
             "name": "sqtlColocLlrMaximumNeighborhood",
             "nullable": true,
             "type": "float"
+        },
+        {
+            "metadata": {},
+            "name": "tuqtlColocClppMaximum",
+            "nullable": true,
+            "type": "float"
+        },
+        {
+            "metadata": {},
+            "name": "tuqtlColocClppMaximumNeighborhood",
+            "nullable": true,
+            "type": "float"
+        },
+        {
+            "metadata": {},
+            "name": "tuqtlColocLlrMaximum",
+            "nullable": true,
+            "type": "float"
+        },
+        {
+            "metadata": {},
+            "name": "tuqtlColocLlrMaximumNeighborhood",
+            "nullable": true,
+            "type": "float"
         }
     ],
     "type": "struct"
 }
```

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/l2g_gold_standard.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/l2g_gold_standard.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/ld_index.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/ld_index.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/study_index.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/study_index.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/study_locus.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/study_locus.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659090909090909%*

 * *Differences: {"'fields'": "{insert: [(7, OrderedDict([('metadata', OrderedDict()), ('name', 'zScore'), "*

 * *             "('nullable', True), ('type', 'double')])), (17, OrderedDict([('metadata', "*

 * *             "OrderedDict()), ('name', 'purityMeanR2'), ('nullable', True), ('type', 'double')])), "*

 * *             "(18, OrderedDict([('metadata', OrderedDict()), ('name', 'purityMinR2'), ('nullable', "*

 * *             "True), ('type', 'double')]))]}"}*

```diff
@@ -40,14 +40,20 @@
             "metadata": {},
             "name": "beta",
             "nullable": true,
             "type": "double"
         },
         {
             "metadata": {},
+            "name": "zScore",
+            "nullable": true,
+            "type": "double"
+        },
+        {
+            "metadata": {},
             "name": "pValueMantissa",
             "nullable": true,
             "type": "float"
         },
         {
             "metadata": {},
             "name": "pValueExponent",
@@ -98,14 +104,26 @@
             "metadata": {},
             "name": "credibleSetlog10BF",
             "nullable": true,
             "type": "double"
         },
         {
             "metadata": {},
+            "name": "purityMeanR2",
+            "nullable": true,
+            "type": "double"
+        },
+        {
+            "metadata": {},
+            "name": "purityMinR2",
+            "nullable": true,
+            "type": "double"
+        },
+        {
+            "metadata": {},
             "name": "sampleSize",
             "nullable": true,
             "type": "integer"
         },
         {
             "metadata": {},
             "name": "ldSet",
```

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/study_locus_overlap.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/study_locus_overlap.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/summary_statistics.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/summary_statistics.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/v2g.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/v2g.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/variant_annotation.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/variant_annotation.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692308%*

 * *Differences: {"'fields'": '{delete: [3]}'}*

```diff
@@ -16,20 +16,14 @@
             "metadata": {},
             "name": "position",
             "nullable": false,
             "type": "integer"
         },
         {
             "metadata": {},
-            "name": "gnomadVariantId",
-            "nullable": false,
-            "type": "string"
-        },
-        {
-            "metadata": {},
             "name": "referenceAllele",
             "nullable": false,
             "type": "string"
         },
         {
             "metadata": {},
             "name": "alternateAllele",
```

### Comparing `gentropy-1.2.0/src/gentropy/assets/schemas/variant_index.json` & `gentropy-1.3.0/src/gentropy/assets/schemas/variant_index.json`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/cli.py` & `gentropy-1.3.0/src/gentropy/cli.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/clump.py` & `gentropy-1.3.0/src/gentropy/window_based_clumping.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,61 @@
-"""Step to run clump associations from summary statistics or study locus."""
-from __future__ import annotations
+"""Step to run window based clumping on summary statistics datasts."""
 
-from typing import Optional
+from __future__ import annotations
 
 from gentropy.common.session import Session
-from gentropy.dataset.ld_index import LDIndex
-from gentropy.dataset.study_index import StudyIndex
-from gentropy.dataset.study_locus import StudyLocus
 from gentropy.dataset.summary_statistics import SummaryStatistics
 
 
-class ClumpStep:
-    """Perform clumping of an association dataset to identify independent signals.
-
-    Two types of clumping are supported and are applied based on the input dataset:
-    - Clumping of summary statistics based on a window-based approach.
-    - Clumping of study locus based on LD.
-
-    Both approaches yield a StudyLocus dataset.
-    """
+class WindowBasedClumpingStep:
+    """Apply window based clumping on summary statistics datasets."""
 
     def __init__(
         self,
         session: Session,
-        input_path: str,
-        clumped_study_locus_path: str,
-        study_index_path: Optional[str] = None,
-        ld_index_path: Optional[str] = None,
-        locus_collect_distance: Optional[int] = None,
+        summary_statistics_input_path: str,
+        study_locus_output_path: str,
+        distance: int = 500_000,
+        collect_locus: bool = False,
+        collect_locus_distance: int = 500_000,
+        inclusion_list_path: str | None = None,
     ) -> None:
-        """Run the clumping step.
+        """Run window-based clumping step.
 
         Args:
             session (Session): Session object.
-            input_path (str): Input path for the study locus or summary statistics files.
-            clumped_study_locus_path (str): Output path for the clumped study locus dataset.
-            study_index_path (Optional[str]): Input path for the study index dataset.
-            ld_index_path (Optional[str]): Input path for the LD index dataset.
-            locus_collect_distance (Optional[int]): Distance in base pairs to collect variants around the study locus.
-
-        Raises:
-            ValueError: If study index and LD index paths are not provided for study locus.
+            summary_statistics_input_path (str): Path to the harmonized summary statistics dataset.
+            study_locus_output_path (str): Output path for the resulting study locus dataset.
+            distance (int): Distance, within which tagging variants are collected around the semi-index. Optional.
+            collect_locus (bool): Whether to collect locus around semi-indices. Optional.
+            collect_locus_distance (int): Distance, within which tagging variants are collected around the semi-index. Optional.
+            inclusion_list_path (str | None): Path to the inclusion list (list of white-listed study identifier). Optional.
         """
-        input_cols = session.spark.read.parquet(
-            input_path, recursiveFileLookup=True
-        ).columns
-        if "studyLocusId" in input_cols:
-            if study_index_path is None or ld_index_path is None:
-                raise ValueError(
-                    "Study index and LD index paths are required for clumping study locus."
-                )
-            study_locus = StudyLocus.from_parquet(session, input_path)
-            ld_index = LDIndex.from_parquet(session, ld_index_path)
-            study_index = StudyIndex.from_parquet(session, study_index_path)
-
-            clumped_study_locus = study_locus.annotate_ld(
-                study_index=study_index, ld_index=ld_index
-            ).clump()
+        # If inclusion list path is provided, only these studies will be read:
+        if inclusion_list_path:
+            study_ids_to_ingest = [
+                f'{summary_statistics_input_path}/{row["studyId"]}.parquet'
+                for row in session.spark.read.parquet(inclusion_list_path).collect()
+            ]
         else:
-            sumstats = SummaryStatistics.from_parquet(
-                session, input_path, recursiveFileLookup=True
-            ).coalesce(4000)
-            clumped_study_locus = sumstats.window_based_clumping(
-                locus_collect_distance=locus_collect_distance
-            )
+            # If no inclusion list is provided, read all summary stats in folder:
+            study_ids_to_ingest = [summary_statistics_input_path]
 
-        clumped_study_locus.df.write.mode(session.write_mode).parquet(
-            clumped_study_locus_path
+        ss = SummaryStatistics.from_parquet(
+            session,
+            study_ids_to_ingest,
+            recursiveFileLookup=True,
         )
+
+        # Clumping:
+        study_locus = ss.window_based_clumping(
+            distance=distance,
+        )
+
+        # Optional locus collection:
+        if collect_locus:
+            # Collecting locus around semi-indices:
+            study_locus = study_locus.annotate_locus_statistics(
+                ss, collect_locus_distance=collect_locus_distance
+            )
+
+        study_locus.df.write.mode(session.write_mode).parquet(study_locus_output_path)
```

### Comparing `gentropy-1.2.0/src/gentropy/colocalisation.py` & `gentropy-1.3.0/src/gentropy/variant_index.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,44 @@
-"""Step to generate colocalisation results."""
+"""Step to generate variant index dataset."""
 from __future__ import annotations
 
 from gentropy.common.session import Session
-from gentropy.dataset.study_index import StudyIndex
-from gentropy.dataset.study_locus import CredibleInterval, StudyLocus
-from gentropy.method.colocalisation import ECaviar
+from gentropy.dataset.study_locus import StudyLocus
+from gentropy.dataset.variant_annotation import VariantAnnotation
+from gentropy.dataset.variant_index import VariantIndex
 
 
-class ColocalisationStep:
-    """Colocalisation step.
+class VariantIndexStep:
+    """Run variant index step to only variants in study-locus sets.
 
-    This workflow runs colocalisation analyses that assess the degree to which independent signals of the association share the same causal variant in a region of the genome, typically limited by linkage disequilibrium (LD).
+    Using a `VariantAnnotation` dataset as a reference, this step creates and writes a dataset of the type `VariantIndex` that includes only variants that have disease-association data with a reduced set of annotations.
     """
 
     def __init__(
-        self,
+        self: VariantIndexStep,
         session: Session,
+        variant_annotation_path: str,
         credible_set_path: str,
-        study_index_path: str,
-        coloc_path: str,
+        variant_index_path: str,
     ) -> None:
-        """Run Colocalisation step.
+        """Run VariantIndex step.
 
         Args:
             session (Session): Session object.
-            credible_set_path (str): Input credible sets path.
-            study_index_path (str): Input study index path.
-            coloc_path (str): Output Colocalisation path.
+            variant_annotation_path (str): Variant annotation dataset path.
+            credible_set_path (str): Credible set dataset path.
+            variant_index_path (str): Variant index dataset path.
         """
         # Extract
+        va = VariantAnnotation.from_parquet(session, variant_annotation_path)
         credible_set = StudyLocus.from_parquet(
             session, credible_set_path, recursiveFileLookup=True
         )
-        si = StudyIndex.from_parquet(
-            session, study_index_path, recursiveFileLookup=True
-        )
 
         # Transform
-        overlaps = credible_set.filter_credible_set(
-            CredibleInterval.IS95
-        ).find_overlaps(si)
-        ecaviar_results = ECaviar.colocalise(overlaps)
+        vi = VariantIndex.from_variant_annotation(va, credible_set)
 
-        # Load
-        ecaviar_results.df.write.mode(session.write_mode).parquet(coloc_path)
+        (
+            vi.df.write.partitionBy("chromosome")
+            .mode(session.write_mode)
+            .parquet(variant_index_path)
+        )
```

### Comparing `gentropy-1.2.0/src/gentropy/common/Liftover.py` & `gentropy-1.3.0/src/gentropy/common/Liftover.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/common/schemas.py` & `gentropy-1.3.0/src/gentropy/common/schemas.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/common/session.py` & `gentropy-1.3.0/src/gentropy/common/session.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/common/spark_helpers.py` & `gentropy-1.3.0/src/gentropy/common/spark_helpers.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/common/utils.py` & `gentropy-1.3.0/src/gentropy/common/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Common functions in the Genetics datasets."""
+
 from __future__ import annotations
 
 import sys
 from math import floor, log10
 from typing import TYPE_CHECKING, Tuple
 
 import hail as hl
@@ -204,49 +205,14 @@
 
     return [
         mantissa.cast(t.FloatType()).alias("pValueMantissa"),
         exponent.cast(t.IntegerType()).alias("pValueExponent"),
     ]
 
 
-def convert_gnomad_position_to_ensembl(
-    position: Column, reference: Column, alternate: Column
-) -> Column:
-    """Convert GnomAD variant position to Ensembl variant position.
-
-    For indels (the reference or alternate allele is longer than 1), then adding 1 to the position, for SNPs,
-    the position is unchanged. More info about the problem: https://www.biostars.org/p/84686/
-
-    Args:
-        position (Column): Position of the variant in GnomAD's coordinates system.
-        reference (Column): The reference allele in GnomAD's coordinates system.
-        alternate (Column): The alternate allele in GnomAD's coordinates system.
-
-    Returns:
-        Column: The position of the variant in the Ensembl genome.
-
-    Examples:
-        >>> d = [(1, "A", "C"), (2, "AA", "C"), (3, "A", "AA")]
-        >>> df = spark.createDataFrame(d).toDF("position", "reference", "alternate")
-        >>> df.withColumn("new_position", convert_gnomad_position_to_ensembl(f.col("position"), f.col("reference"), f.col("alternate"))).show()
-        +--------+---------+---------+------------+
-        |position|reference|alternate|new_position|
-        +--------+---------+---------+------------+
-        |       1|        A|        C|           1|
-        |       2|       AA|        C|           3|
-        |       3|        A|       AA|           4|
-        +--------+---------+---------+------------+
-        <BLANKLINE>
-
-    """
-    return f.when(
-        (f.length(reference) > 1) | (f.length(alternate) > 1), position + 1
-    ).otherwise(position)
-
-
 def _liftover_loci(
     variant_index: Table, chain_path: str, dest_reference_genome: str
 ) -> Table:
     """Liftover a Hail table containing variant information from GRCh37 to GRCh38 or viceversa.
 
     Args:
         variant_index (Table): Variants to be lifted over
```

### Comparing `gentropy-1.2.0/src/gentropy/config.py` & `gentropy-1.3.0/src/gentropy/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 @dataclass
 class ColocalisationConfig(StepConfig):
     """Colocalisation step configuration."""
 
     credible_set_path: str = MISSING
     study_index_path: str = MISSING
     coloc_path: str = MISSING
+    colocalisation_method: str = MISSING
     _target_: str = "gentropy.colocalisation.ColocalisationStep"
 
 
 @dataclass
 class GeneIndexConfig(StepConfig):
     """Gene index step configuration."""
 
@@ -178,14 +179,15 @@
 
     session: Any = field(
         default_factory=lambda: {
             "extended_spark_conf": {
                 "spark.dynamicAllocation.enabled": "false",
                 "spark.driver.memory": "48g",
                 "spark.executor.memory": "48g",
+                "spark.sql.shuffle.partitions": "800",
             }
         }
     )
     run_mode: str = MISSING
     model_path: str = MISSING
     predictions_path: str = MISSING
     credible_set_path: str = MISSING
@@ -209,21 +211,25 @@
             # mean vep consequence score of the locus 95% credible set split by gene
             "vepMean",
             # max clpp for each (study, locus, gene) aggregating over all eQTLs
             "eqtlColocClppMaximum",
             # max clpp for each (study, locus) aggregating over all eQTLs
             "eqtlColocClppMaximumNeighborhood",
             # max clpp for each (study, locus, gene) aggregating over all pQTLs
-            # "pqtlColocClppMaximum",
+            "pqtlColocClppMaximum",
             # max clpp for each (study, locus) aggregating over all pQTLs
-            # "pqtlColocClppMaximumNeighborhood",
+            "pqtlColocClppMaximumNeighborhood",
             # max clpp for each (study, locus, gene) aggregating over all sQTLs
-            # "sqtlColocClppMaximum",
+            "sqtlColocClppMaximum",
             # max clpp for each (study, locus) aggregating over all sQTLs
-            # "sqtlColocClppMaximumNeighborhood",
+            "sqtlColocClppMaximumNeighborhood",
+            # max clpp for each (study, locus) aggregating over all tuQTLs
+            "tuqtlColocClppMaximum",
+            # max clpp for each (study, locus, gene) aggregating over all tuQTLs
+            "tuqtlColocClppMaximumNeighborhood",
             # # max log-likelihood ratio value for each (study, locus, gene) aggregating over all eQTLs
             # "eqtlColocLlrLocalMaximum",
             # # max log-likelihood ratio value for each (study, locus) aggregating over all eQTLs
             # "eqtlColocLlpMaximumNeighborhood",
             # # max log-likelihood ratio value for each (study, locus, gene) aggregating over all pQTLs
             # "pqtlColocLlrLocalMaximum",
             # # max log-likelihood ratio value for each (study, locus) aggregating over all pQTLs
@@ -312,21 +318,54 @@
 
 @dataclass
 class WindowBasedClumpingStep(StepConfig):
     """Window-based clumping step configuration."""
 
     summary_statistics_input_path: str = MISSING
     study_locus_output_path: str = MISSING
+    distance: int = 500_000
+    collect_locus: bool = False
+    collect_locus_distance: int = 500_000
     inclusion_list_path: str | None = None
-    locus_collect_distance: str | None = None
-
     _target_: str = "gentropy.window_based_clumping.WindowBasedClumpingStep"
 
 
 @dataclass
+class FinemapperConfig(StepConfig):
+    """SuSiE fine-mapper step configuration."""
+
+    session: Any = field(
+        default_factory=lambda: {
+            "start_hail": True,
+        }
+    )
+    study_locus_to_finemap: str = MISSING
+    study_locus_collected_path: str = MISSING
+    study_index_path: str = MISSING
+    output_path: str = MISSING
+    locus_radius: int = MISSING
+    max_causal_snps: int = MISSING
+    primary_signal_pval_threshold: float = MISSING
+    secondary_signal_pval_threshold: float = MISSING
+    purity_mean_r2_threshold: float = MISSING
+    purity_min_r2_threshold: float = MISSING
+    cs_lbf_th: float = MISSING
+    sum_pips: float = MISSING
+    logging: bool = MISSING
+    susie_est_tausq: bool = MISSING
+    run_carma: bool = MISSING
+    run_sumstat_imputation: bool = MISSING
+    carma_time_limit: int = MISSING
+    imputed_r2_threshold: float = MISSING
+    ld_score_threshold: float = MISSING
+    output_path_log: str = MISSING
+    _target_: str = "gentropy.susie_finemapper.SusieFineMapperStep"
+
+
+@dataclass
 class Config:
     """Application configuration."""
 
     # this is unfortunately verbose due to @dataclass limitations
     defaults: List[Any] = field(default_factory=lambda: ["_self_", {"step": MISSING}])
     step: StepConfig = MISSING
     datasets: dict[str, str] = field(default_factory=dict)
@@ -375,7 +414,8 @@
     )
 
     cs.store(group="step", name="pics", node=PICSConfig)
     cs.store(group="step", name="variant_annotation", node=VariantAnnotationConfig)
     cs.store(group="step", name="variant_index", node=VariantIndexConfig)
     cs.store(group="step", name="variant_to_gene", node=VariantToGeneConfig)
     cs.store(group="step", name="window_based_clumping", node=WindowBasedClumpingStep)
+    cs.store(group="step", name="susie_finemapping", node=FinemapperConfig)
```

### Comparing `gentropy-1.2.0/src/gentropy/dataset/colocalisation.py` & `gentropy-1.3.0/src/gentropy/dataset/colocalisation.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/dataset.py` & `gentropy-1.3.0/src/gentropy/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/gene_index.py` & `gentropy-1.3.0/src/gentropy/dataset/gene_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/intervals.py` & `gentropy-1.3.0/src/gentropy/dataset/intervals.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/l2g_feature.py` & `gentropy-1.3.0/src/gentropy/dataset/l2g_feature.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/l2g_feature_matrix.py` & `gentropy-1.3.0/src/gentropy/dataset/l2g_feature_matrix.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,41 +36,43 @@
             col for col in self._df.columns if col not in fixed_cols
         ]
 
     @classmethod
     def generate_features(
         cls: Type[L2GFeatureMatrix],
         features_list: list[str],
-        study_locus: StudyLocus,
+        credible_set: StudyLocus,
         study_index: StudyIndex,
         variant_gene: V2G,
         colocalisation: Colocalisation,
     ) -> L2GFeatureMatrix:
         """Generate features from the gentropy datasets.
 
         Args:
             features_list (list[str]): List of features to generate
-            study_locus (StudyLocus): Study locus dataset
+            credible_set (StudyLocus): Credible set dataset
             study_index (StudyIndex): Study index dataset
             variant_gene (V2G): Variant to gene dataset
             colocalisation (Colocalisation): Colocalisation dataset
 
         Returns:
             L2GFeatureMatrix: L2G feature matrix dataset
 
         Raises:
             ValueError: If the feature matrix is empty
         """
         if features_dfs := [
             # Extract features
-            ColocalisationFactory._get_coloc_features(
-                study_locus, study_index, colocalisation
+            ColocalisationFactory._get_max_coloc_per_credible_set(
+                colocalisation,
+                credible_set,
+                study_index,
             ).df,
-            StudyLocusFactory._get_tss_distance_features(study_locus, variant_gene).df,
-            StudyLocusFactory._get_vep_features(study_locus, variant_gene).df,
+            StudyLocusFactory._get_tss_distance_features(credible_set, variant_gene).df,
+            StudyLocusFactory._get_vep_features(credible_set, variant_gene).df,
         ]:
             fm = reduce(
                 lambda x, y: x.unionByName(y),
                 features_dfs,
             )
         else:
             raise ValueError("No features found")
@@ -158,12 +160,10 @@
             fraction (float): Fraction of the dataset to use for training
 
         Returns:
             tuple[L2GFeatureMatrix, L2GFeatureMatrix]: Training and test datasets
         """
         train, test = self._df.randomSplit([fraction, 1 - fraction], seed=42)
         return (
-            L2GFeatureMatrix(
-                _df=train, _schema=L2GFeatureMatrix.get_schema()
-            ).persist(),
-            L2GFeatureMatrix(_df=test, _schema=L2GFeatureMatrix.get_schema()).persist(),
+            L2GFeatureMatrix(_df=train, _schema=L2GFeatureMatrix.get_schema()),
+            L2GFeatureMatrix(_df=test, _schema=L2GFeatureMatrix.get_schema()),
         )
```

### Comparing `gentropy-1.2.0/src/gentropy/dataset/l2g_gold_standard.py` & `gentropy-1.3.0/src/gentropy/dataset/l2g_gold_standard.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/l2g_prediction.py` & `gentropy-1.3.0/src/gentropy/dataset/l2g_prediction.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,44 +40,44 @@
         return parse_spark_schema("l2g_predictions.json")
 
     @classmethod
     def from_credible_set(
         cls: Type[L2GPrediction],
         model_path: str,
         features_list: list[str],
-        study_locus: StudyLocus,
+        credible_set: StudyLocus,
         study_index: StudyIndex,
         v2g: V2G,
         coloc: Colocalisation,
     ) -> L2GPrediction:
         """Extract L2G predictions for a set of credible sets derived from GWAS.
 
         Args:
             model_path (str): Path to the fitted model
             features_list (list[str]): List of features to use for the model
-            study_locus (StudyLocus): Study locus dataset
+            credible_set (StudyLocus): Credible set dataset
             study_index (StudyIndex): Study index dataset
             v2g (V2G): Variant to gene dataset
             coloc (Colocalisation): Colocalisation dataset
 
         Returns:
             L2GPrediction: L2G dataset
         """
         fm = L2GFeatureMatrix.generate_features(
             features_list=features_list,
-            study_locus=study_locus,
+            credible_set=credible_set,
             study_index=study_index,
             variant_gene=v2g,
             colocalisation=coloc,
         ).fill_na()
 
         gwas_fm = L2GFeatureMatrix(
             _df=(
                 fm.df.join(
-                    study_locus.filter_by_study_type("gwas", study_index).df,
+                    credible_set.filter_by_study_type("gwas", study_index).df,
                     on="studyLocusId",
                 )
             ),
             _schema=cls.get_schema(),
         )
         return L2GPrediction(
             # Load and apply fitted model
```

### Comparing `gentropy-1.2.0/src/gentropy/dataset/ld_index.py` & `gentropy-1.3.0/src/gentropy/dataset/ld_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/study_index.py` & `gentropy-1.3.0/src/gentropy/dataset/study_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/study_locus.py` & `gentropy-1.3.0/src/gentropy/dataset/study_locus.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Study locus dataset."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import TYPE_CHECKING
 
 import pyspark.sql.functions as f
@@ -20,14 +21,15 @@
 
 if TYPE_CHECKING:
     from pyspark.sql import Column, DataFrame
     from pyspark.sql.types import StructType
 
     from gentropy.dataset.ld_index import LDIndex
     from gentropy.dataset.study_index import StudyIndex
+    from gentropy.dataset.summary_statistics import SummaryStatistics
 
 
 class StudyLocusQualityCheck(Enum):
     """Study-Locus quality control options listing concerns on the quality of the association.
 
     Attributes:
         SUBSIGNIFICANT_FLAG (str): p-value below significance threshold
@@ -76,39 +78,60 @@
 class StudyLocus(Dataset):
     """Study-Locus dataset.
 
     This dataset captures associations between study/traits and a genetic loci as provided by finemapping methods.
     """
 
     @staticmethod
-    def _overlapping_peaks(credset_to_overlap: DataFrame) -> DataFrame:
+    def _overlapping_peaks(
+        credset_to_overlap: DataFrame, intra_study_overlap: bool = False
+    ) -> DataFrame:
         """Calculate overlapping signals (study-locus) between GWAS-GWAS and GWAS-Molecular trait.
 
         Args:
             credset_to_overlap (DataFrame): DataFrame containing at least `studyLocusId`, `studyType`, `chromosome` and `tagVariantId` columns.
+            intra_study_overlap (bool): When True, finds intra-study overlaps for credible set deduplication. Default is False.
 
         Returns:
             DataFrame: containing `leftStudyLocusId`, `rightStudyLocusId` and `chromosome` columns.
         """
         # Reduce columns to the minimum to reduce the size of the dataframe
         credset_to_overlap = credset_to_overlap.select(
-            "studyLocusId", "studyType", "chromosome", "tagVariantId"
+            "studyLocusId",
+            "studyId",
+            "studyType",
+            "chromosome",
+            "region",
+            "tagVariantId",
         )
+        # Define join condition - if intra_study_overlap is True, finds overlaps within the same study. Otherwise finds gwas vs everything overlaps for coloc.
+        join_condition = (
+            [
+                f.col("left.studyId") == f.col("right.studyId"),
+                f.col("left.chromosome") == f.col("right.chromosome"),
+                f.col("left.tagVariantId") == f.col("right.tagVariantId"),
+                f.col("left.studyLocusId") > f.col("right.studyLocusId"),
+                f.col("left.region") != f.col("right.region"),
+            ]
+            if intra_study_overlap
+            else [
+                f.col("left.chromosome") == f.col("right.chromosome"),
+                f.col("left.tagVariantId") == f.col("right.tagVariantId"),
+                (f.col("right.studyType") != "gwas")
+                | (f.col("left.studyLocusId") > f.col("right.studyLocusId")),
+                f.col("left.studyType") == f.lit("gwas"),
+            ]
+        )
+
         return (
             credset_to_overlap.alias("left")
-            .filter(f.col("studyType") == "gwas")
-            # Self join with complex condition. Left it's all gwas and right can be gwas or molecular trait
+            # Self join with complex condition.
             .join(
                 credset_to_overlap.alias("right"),
-                on=[
-                    f.col("left.chromosome") == f.col("right.chromosome"),
-                    f.col("left.tagVariantId") == f.col("right.tagVariantId"),
-                    (f.col("right.studyType") != "gwas")
-                    | (f.col("left.studyLocusId") > f.col("right.studyLocusId")),
-                ],
+                on=join_condition,
                 how="inner",
             )
             .select(
                 f.col("left.studyLocusId").alias("leftStudyLocusId"),
                 f.col("right.studyLocusId").alias("rightStudyLocusId"),
                 f.col("left.chromosome").alias("chromosome"),
             )
@@ -299,45 +322,50 @@
             f.filter(
                 f.col("locus"),
                 lambda tag: (tag[credible_interval.value]),
             ),
         )
         return self
 
-    def find_overlaps(self: StudyLocus, study_index: StudyIndex) -> StudyLocusOverlap:
+    def find_overlaps(
+        self: StudyLocus, study_index: StudyIndex, intra_study_overlap: bool = False
+    ) -> StudyLocusOverlap:
         """Calculate overlapping study-locus.
 
         Find overlapping study-locus that share at least one tagging variant. All GWAS-GWAS and all GWAS-Molecular traits are computed with the Molecular traits always
         appearing on the right side.
 
         Args:
             study_index (StudyIndex): Study index to resolve study types.
+            intra_study_overlap (bool): If True, finds intra-study overlaps for credible set deduplication. Default is False.
 
         Returns:
             StudyLocusOverlap: Pairs of overlapping study-locus with aligned tags.
         """
         loci_to_overlap = (
             self.df.join(study_index.study_type_lut(), on="studyId", how="inner")
             .withColumn("locus", f.explode("locus"))
             .select(
                 "studyLocusId",
+                "studyId",
                 "studyType",
                 "chromosome",
+                "region",
                 f.col("locus.variantId").alias("tagVariantId"),
                 f.col("locus.logBF").alias("logBF"),
                 f.col("locus.posteriorProbability").alias("posteriorProbability"),
                 f.col("locus.pValueMantissa").alias("pValueMantissa"),
                 f.col("locus.pValueExponent").alias("pValueExponent"),
                 f.col("locus.beta").alias("beta"),
             )
             .persist()
         )
 
         # overlapping study-locus
-        peak_overlaps = self._overlapping_peaks(loci_to_overlap)
+        peak_overlaps = self._overlapping_peaks(loci_to_overlap, intra_study_overlap)
 
         # study-locus overlap by aligning overlapping variants
         return self._align_overlapping_tags(loci_to_overlap, peak_overlaps)
 
     def unique_variants_in_locus(self: StudyLocus) -> DataFrame:
         """All unique variants collected in a `StudyLocus` dataframe.
 
@@ -423,14 +451,82 @@
                         CredibleInterval.IS99.value, (acc < 0.99) & acc.isNotNull()
                     ),
                 ),
             ),
         )
         return self
 
+    def annotate_locus_statistics(
+        self: StudyLocus,
+        summary_statistics: SummaryStatistics,
+        collect_locus_distance: int,
+    ) -> StudyLocus:
+        """Annotates study locus with summary statistics in the specified distance around the position.
+
+        Args:
+            summary_statistics (SummaryStatistics): Summary statistics to be used for annotation.
+            collect_locus_distance (int): distance from variant defining window for inclusion of variants in locus.
+
+        Returns:
+            StudyLocus: Study locus annotated with summary statistics in `locus` column. If no statistics are found, the `locus` column will be empty.
+        """
+        # The clumps will be used several times (persisting)
+        self.df.persist()
+        # Renaming columns:
+        sumstats_renamed = summary_statistics.df.selectExpr(
+            *[f"{col} as tag_{col}" for col in summary_statistics.df.columns]
+        ).alias("sumstat")
+
+        locus_df = (
+            sumstats_renamed
+            # Joining the two datasets together:
+            .join(
+                f.broadcast(
+                    self.df.alias("clumped").select(
+                        "position", "chromosome", "studyId", "studyLocusId"
+                    )
+                ),
+                on=[
+                    (f.col("sumstat.tag_studyId") == f.col("clumped.studyId"))
+                    & (f.col("sumstat.tag_chromosome") == f.col("clumped.chromosome"))
+                    & (
+                        f.col("sumstat.tag_position")
+                        >= (f.col("clumped.position") - collect_locus_distance)
+                    )
+                    & (
+                        f.col("sumstat.tag_position")
+                        <= (f.col("clumped.position") + collect_locus_distance)
+                    )
+                ],
+                how="inner",
+            )
+            .withColumn(
+                "locus",
+                f.struct(
+                    f.col("tag_variantId").alias("variantId"),
+                    f.col("tag_beta").alias("beta"),
+                    f.col("tag_pValueMantissa").alias("pValueMantissa"),
+                    f.col("tag_pValueExponent").alias("pValueExponent"),
+                    f.col("tag_standardError").alias("standardError"),
+                ),
+            )
+            .groupBy("studyLocusId")
+            .agg(
+                f.collect_list(f.col("locus")).alias("locus"),
+            )
+        )
+
+        self.df = self.df.drop("locus").join(
+            locus_df,
+            on="studyLocusId",
+            how="left",
+        )
+
+        return self
+
     def annotate_ld(
         self: StudyLocus, study_index: StudyIndex, ld_index: LDIndex
     ) -> StudyLocus:
         """Annotate LD information to study-locus.
 
         Args:
             study_index (StudyIndex): Study index to resolve ancestries.
```

### Comparing `gentropy-1.2.0/src/gentropy/dataset/study_locus_overlap.py` & `gentropy-1.3.0/src/gentropy/dataset/study_locus_overlap.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/summary_statistics.py` & `gentropy-1.3.0/src/gentropy/dataset/summary_statistics.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from typing import TYPE_CHECKING
 
 import pyspark.sql.functions as f
 
 from gentropy.common.schemas import parse_spark_schema
 from gentropy.common.utils import parse_region, split_pvalue
 from gentropy.dataset.dataset import Dataset
-from gentropy.method.window_based_clumping import WindowBasedClumping
 
 if TYPE_CHECKING:
     from pyspark.sql.types import StructType
 
     from gentropy.dataset.study_locus import StudyLocus
 
 
@@ -55,42 +54,32 @@
         )
         return SummaryStatistics(_df=df, _schema=self._schema)
 
     def window_based_clumping(
         self: SummaryStatistics,
         distance: int = 500_000,
         gwas_significance: float = 5e-8,
-        baseline_significance: float = 0.05,
-        locus_collect_distance: int | None = None,
     ) -> StudyLocus:
-        """Generate study-locus from summary statistics by distance based clumping + collect locus.
+        """Generate study-locus from summary statistics using window-based clumping.
+
+        For more info, see [`WindowBasedClumping`][gentropy.method.window_based_clumping.WindowBasedClumping]
 
         Args:
             distance (int): Distance in base pairs to be used for clumping. Defaults to 500_000.
             gwas_significance (float, optional): GWAS significance threshold. Defaults to 5e-8.
-            baseline_significance (float, optional): Baseline significance threshold for inclusion in the locus. Defaults to 0.05.
-            locus_collect_distance (int | None): The distance to collect locus around semi-indices. If not provided, locus is not collected.
 
         Returns:
-            StudyLocus: Clumped study-locus containing variants based on window.
+            StudyLocus: Clumped study-locus optionally containing variants based on window.
         """
-        return (
-            WindowBasedClumping.clump_with_locus(
-                self,
-                window_length=distance,
-                p_value_significance=gwas_significance,
-                p_value_baseline=baseline_significance,
-                locus_window_length=locus_collect_distance,
-            )
-            if locus_collect_distance
-            else WindowBasedClumping.clump(
-                self,
-                window_length=distance,
-                p_value_significance=gwas_significance,
-            )
+        from gentropy.method.window_based_clumping import WindowBasedClumping
+
+        return WindowBasedClumping.clump(
+            self,
+            distance=distance,
+            gwas_significance=gwas_significance,
         )
 
     def exclude_region(self: SummaryStatistics, region: str) -> SummaryStatistics:
         """Exclude a region from the summary stats dataset.
 
         Args:
             region (str): region given in "chr##:#####-####" format
@@ -110,7 +99,33 @@
                             & (f.col("position") <= end_position)
                         )
                     )
                 )
             ),
             _schema=SummaryStatistics.get_schema(),
         )
+
+    def sanity_filter(self: SummaryStatistics) -> SummaryStatistics:
+        """The function filters the summary statistics by sanity filters.
+
+        The function filters the summary statistics by the following filters:
+            - The p-value should not be eqaul 1.
+            - The beta and se should not be equal 0.
+            - The p-value, beta and se should not be NaN.
+
+        Returns:
+            SummaryStatistics: The filtered summary statistics.
+        """
+        gwas_df = self._df
+        gwas_df = gwas_df.dropna(
+            subset=["beta", "standardError", "pValueMantissa", "pValueExponent"]
+        )
+
+        gwas_df = gwas_df.filter((f.col("beta") != 0) & (f.col("standardError") != 0))
+        gwas_df = gwas_df.filter(
+            f.col("pValueMantissa") * 10 ** f.col("pValueExponent") != 1
+        )
+
+        return SummaryStatistics(
+            _df=gwas_df,
+            _schema=SummaryStatistics.get_schema(),
+        )
```

### Comparing `gentropy-1.2.0/src/gentropy/dataset/v2g.py` & `gentropy-1.3.0/src/gentropy/dataset/v2g.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/variant_annotation.py` & `gentropy-1.3.0/src/gentropy/dataset/variant_annotation.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/dataset/variant_index.py` & `gentropy-1.3.0/src/gentropy/dataset/variant_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/eqtl_catalogue/finemapping.py` & `gentropy-1.3.0/src/gentropy/datasource/eqtl_catalogue/finemapping.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/eqtl_catalogue/study_index.py` & `gentropy-1.3.0/src/gentropy/datasource/eqtl_catalogue/study_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/eqtl_catalogue/summary_stats.py` & `gentropy-1.3.0/src/gentropy/datasource/eqtl_catalogue/summary_stats.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/finngen/finemapping.py` & `gentropy-1.3.0/src/gentropy/datasource/finngen/finemapping.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/finngen/study_index.py` & `gentropy-1.3.0/src/gentropy/datasource/finngen/study_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/finngen/summary_stats.py` & `gentropy-1.3.0/src/gentropy/datasource/finngen/summary_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,24 +46,27 @@
         Args:
             spark (SparkSession): Spark session object.
             raw_file (str): Path to raw summary statistics .gz files.
 
         Returns:
             SummaryStatistics: Processed summary statistics dataset
         """
-        study_id = raw_file.split("/")[-1].split(".")[0].upper()
         processed_summary_stats_df = (
             spark.read.schema(cls.raw_schema)
             .option("delimiter", "\t")
             .csv(raw_file, header=True)
             # Drop rows which don't have proper position.
             .filter(f.col("pos").cast(t.IntegerType()).isNotNull())
             .select(
                 # From the full path, extracts just the filename, and converts to upper case to get the study ID.
-                f.lit(study_id).alias("studyId"),
+                f.upper(
+                    f.regexp_extract(
+                        f.input_file_name(), r"([^/]+)(\.tsv\.gz|\.gz|\.tsv)", 1
+                    )
+                ).alias("studyId"),
                 # Add variant information.
                 f.concat_ws(
                     "_",
                     f.col("#chrom"),
                     f.col("pos"),
                     f.col("ref"),
                     f.col("alt"),
```

### Comparing `gentropy-1.2.0/src/gentropy/datasource/gnomad/ld.py` & `gentropy-1.3.0/src/gentropy/datasource/gnomad/ld.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Step to import filtered version of a LD matrix (block matrix)."""
+
 from __future__ import annotations
 
 import sys
 from dataclasses import dataclass, field
 from functools import reduce
 from typing import TYPE_CHECKING
 
 import hail as hl
+import numpy as np
 import pyspark.sql.functions as f
 from hail.linalg import BlockMatrix
 from pyspark.sql import Window
 
 from gentropy.common.spark_helpers import get_top_ranked_in_window, get_value_from_row
-from gentropy.common.utils import _liftover_loci, convert_gnomad_position_to_ensembl
+from gentropy.common.utils import _liftover_loci
 from gentropy.dataset.ld_index import LDIndex
 
 if TYPE_CHECKING:
-    from pyspark.sql import DataFrame
+    from pyspark.sql import DataFrame, Row
 
 
 @dataclass
 class GnomADLDMatrix:
     """Toolset ot interact with GnomAD LD dataset (version: r2.1.1).
 
     Datasets are accessed in Hail's native format, as provided by the [GnomAD consortium](https://gnomad.broadinstitute.org/downloads/#v2-linkage-disequilibrium).
@@ -30,14 +32,15 @@
         ld_index_raw_template (str): Template for the LD index path. Defaults to "gs://gcp-public-data--gnomad/release/2.1.1/ld/gnomad.genomes.r2.1.1.{POP}.common.ld.variant_indices.ht".
         grch37_to_grch38_chain_path (str): Path to the chain file used to lift over the coordinates. Defaults to "gs://hail-common/references/grch37_to_grch38.over.chain.gz".
         ld_populations (list[str]): List of populations to use to build the LDIndex. Defaults to ["afr", "amr", "asj", "eas", "fin", "nfe", "nwe", "seu"].
     """
 
     ld_matrix_template: str = "gs://gcp-public-data--gnomad/release/2.1.1/ld/gnomad.genomes.r2.1.1.{POP}.common.adj.ld.bm"
     ld_index_raw_template: str = "gs://gcp-public-data--gnomad/release/2.1.1/ld/gnomad.genomes.r2.1.1.{POP}.common.ld.variant_indices.ht"
+    liftover_ht_path: str = "gs://gcp-public-data--gnomad/release/2.1.1/liftover_grch38/ht/genomes/gnomad.genomes.r2.1.1.sites.liftover_grch38.ht"
     grch37_to_grch38_chain_path: str = (
         "gs://hail-common/references/grch37_to_grch38.over.chain.gz"
     )
     ld_populations: list[str] = field(
         default_factory=lambda: [
             "afr",  # African-American
             "amr",  # American Admixed/Latino
@@ -171,32 +174,23 @@
             ld_index_raw, grch37_to_grch38_chain_path, "GRCh38"
         )
 
         return (
             ld_index_38.to_spark()
             # Filter out variants where the liftover failed
             .filter(f.col("`locus_GRCh38.position`").isNotNull())
-            .withColumn(
-                "chromosome", f.regexp_replace("`locus_GRCh38.contig`", "chr", "")
-            )
-            .withColumn(
-                "position",
-                convert_gnomad_position_to_ensembl(
-                    f.col("`locus_GRCh38.position`"),
-                    f.col("`alleles`").getItem(0),
-                    f.col("`alleles`").getItem(1),
-                ),
-            )
             .select(
-                "chromosome",
-                "position",
+                f.regexp_replace("`locus_GRCh38.contig`", "chr", "").alias(
+                    "chromosome"
+                ),
+                f.col("`locus_GRCh38.position`").alias("position"),
                 f.concat_ws(
                     "_",
-                    f.col("chromosome"),
-                    f.col("position"),
+                    f.regexp_replace("`locus_GRCh38.contig`", "chr", ""),
+                    f.col("`locus_GRCh38.position`"),
                     f.col("`alleles`").getItem(0),
                     f.col("`alleles`").getItem(1),
                 ).alias("variantId"),
                 f.col("idx"),
             )
             # Filter out ambiguous liftover results: multiple indices for the same variant
             .withColumn("count", f.count("*").over(Window.partitionBy(["variantId"])))
@@ -214,17 +208,17 @@
             ld_index (DataFrame): Dataframe with resolved variant indices
             ld_matrix (DataFrame): Dataframe with the filtered LD matrix
 
         Returns:
             DataFrame: Dataframe with variant IDs instead of `i` and `j` indices
         """
         ld_index_i = ld_index.selectExpr(
-            "idx as i", "variantId as variantId_i", "chromosome"
+            "idx as i", "variantId as variantIdI", "chromosome"
         )
-        ld_index_j = ld_index.selectExpr("idx as j", "variantId as variantId_j")
+        ld_index_j = ld_index.selectExpr("idx as j", "variantId as variantIdJ")
         return (
             ld_matrix.join(ld_index_i, on="i", how="inner")
             .join(ld_index_j, on="j", how="inner")
             .drop("i", "j")
         )
 
     @staticmethod
@@ -234,43 +228,43 @@
         Args:
             ld_matrix (DataFrame): Triangular LD matrix converted to a Spark DataFrame
 
         Returns:
             DataFrame: Square LD matrix without diagonal duplicates
 
         Examples:
-            >>> df = spark.createDataFrame(
-            ...     [
-            ...         (1, 1, 1.0, "1", "AFR"),
-            ...         (1, 2, 0.5, "1", "AFR"),
-            ...         (2, 2, 1.0, "1", "AFR"),
-            ...     ],
-            ...     ["variantId_i", "variantId_j", "r", "chromosome", "population"],
-            ... )
-            >>> GnomADLDMatrix._transpose_ld_matrix(df).show()
-            +-----------+-----------+---+----------+----------+
-            |variantId_i|variantId_j|  r|chromosome|population|
-            +-----------+-----------+---+----------+----------+
-            |          1|          2|0.5|         1|       AFR|
-            |          1|          1|1.0|         1|       AFR|
-            |          2|          1|0.5|         1|       AFR|
-            |          2|          2|1.0|         1|       AFR|
-            +-----------+-----------+---+----------+----------+
-            <BLANKLINE>
+        >>> df = spark.createDataFrame(
+        ...     [
+        ...         (1, 1, 1.0, "1", "AFR"),
+        ...         (1, 2, 0.5, "1", "AFR"),
+        ...         (2, 2, 1.0, "1", "AFR"),
+        ...     ],
+        ...     ["variantIdI", "variantIdJ", "r", "chromosome", "population"],
+        ... )
+        >>> GnomADLDMatrix._transpose_ld_matrix(df).show()
+        +----------+----------+---+----------+----------+
+        |variantIdI|variantIdJ|  r|chromosome|population|
+        +----------+----------+---+----------+----------+
+        |         1|         2|0.5|         1|       AFR|
+        |         1|         1|1.0|         1|       AFR|
+        |         2|         1|0.5|         1|       AFR|
+        |         2|         2|1.0|         1|       AFR|
+        +----------+----------+---+----------+----------+
+        <BLANKLINE>
         """
         ld_matrix_transposed = ld_matrix.selectExpr(
-            "variantId_i as variantId_j",
-            "variantId_j as variantId_i",
+            "variantIdI as variantIdJ",
+            "variantIdJ as variantIdI",
             "r",
             "chromosome",
             "population",
         )
-        return ld_matrix.filter(
-            f.col("variantId_i") != f.col("variantId_j")
-        ).unionByName(ld_matrix_transposed)
+        return ld_matrix.filter(f.col("variantIdI") != f.col("variantIdJ")).unionByName(
+            ld_matrix_transposed
+        )
 
     def as_ld_index(
         self: GnomADLDMatrix,
         min_r2: float,
     ) -> LDIndex:
         """Create LDIndex dataset aggregating the LD information across a set of populations.
 
@@ -303,16 +297,16 @@
                 print(f"Failed to create LDIndex for population {pop}: {e}")  # noqa: T201
                 sys.exit(1)
 
         ld_index_unaggregated = (
             GnomADLDMatrix._transpose_ld_matrix(
                 reduce(lambda df1, df2: df1.unionByName(df2), ld_indices_unaggregated)
             )
-            .withColumnRenamed("variantId_i", "variantId")
-            .withColumnRenamed("variantId_j", "tagVariantId")
+            .withColumnRenamed("variantIdI", "variantId")
+            .withColumnRenamed("variantIdJ", "tagVariantId")
         )
         return LDIndex(
             _df=self._aggregate_ld_index_across_populations(ld_index_unaggregated),
             _schema=LDIndex.get_schema(),
         )
 
     def get_ld_variants(
@@ -341,15 +335,14 @@
             )
             .filter(
                 (f.col("chromosome") == chromosome)
                 & (f.col("position") >= start)
                 & (f.col("position") <= end)
             )
             .select("chromosome", "position", "variantId", "idx")
-            .persist()
         )
 
         if ld_index_df.limit(1).count() == 0:
             # If the returned slice from the ld index is empty, return None
             return None
 
         # Compute start and end indices
@@ -391,28 +384,28 @@
         return (
             self.get_ld_matrix_slice(
                 gnomad_ancestry, start_index=start_index, end_index=end_index
             )
             .join(
                 ld_index_df.select(
                     f.col("idx").alias("idx_i"),
-                    f.col("variantId").alias("variantId_i"),
+                    f.col("variantId").alias("variantIdI"),
                 ),
                 on="idx_i",
                 how="inner",
             )
             .join(
                 ld_index_df.select(
                     f.col("idx").alias("idx_j"),
-                    f.col("variantId").alias("variantId_j"),
+                    f.col("variantId").alias("variantIdJ"),
                 ),
                 on="idx_j",
                 how="inner",
             )
-            .select("variantId_i", "variantId_j", "r")
+            .select("variantIdI", "variantIdJ", "r")
         )
 
     def get_ld_matrix_slice(
         self: GnomADLDMatrix,
         gnomad_ancestry: str,
         start_index: int,
         end_index: int,
@@ -444,7 +437,77 @@
                 (f.col("i") + start_index).alias("idx_i"),
                 (f.col("j") + start_index).alias("idx_j"),
                 f.when(f.col("i") == f.col("j"), f.col("entry") / 2)
                 .otherwise(f.col("entry"))
                 .alias("r"),
             )
         )
+
+    def get_locus_index(
+        self: GnomADLDMatrix,
+        study_locus_row: Row,
+        radius: int = 500_000,
+        major_population: str = "nfe",
+    ) -> DataFrame:
+        """Extract hail matrix index from StudyLocus rows.
+
+        Args:
+            study_locus_row (Row): Study-locus row
+            radius (int): Locus radius to extract from gnomad matrix
+            major_population (str): Major population to extract from gnomad matrix, default is "nfe"
+
+        Returns:
+            DataFrame: Returns the index of the gnomad matrix for the locus
+
+        """
+        chromosome = str("chr" + study_locus_row["chromosome"])
+        start = study_locus_row["position"] - radius
+        end = study_locus_row["position"] + radius
+
+        liftover_ht = hl.read_table(self.liftover_ht_path)
+        liftover_ht = (
+            liftover_ht.filter(
+                (liftover_ht.locus.contig == chromosome)
+                & (liftover_ht.locus.position >= start)
+                & (liftover_ht.locus.position <= end)
+            )
+            .key_by()
+            .select("locus", "alleles", "original_locus")
+            .key_by("original_locus", "alleles")
+            .naive_coalesce(20)
+        )
+
+        hail_index = hl.read_table(
+            self.ld_index_raw_template.format(POP=major_population)
+        )
+
+        joined_index = (
+            liftover_ht.join(hail_index, how="inner").order_by("idx").to_spark()
+        )
+
+        return joined_index
+
+    @staticmethod
+    def get_numpy_matrix(
+        locus_index: DataFrame,
+        gnomad_ancestry: str = "nfe",
+    ) -> np.ndarray:
+        """Extract the LD block matrix for a locus.
+
+        Args:
+            locus_index (DataFrame): hail matrix variant index table
+            gnomad_ancestry (str): GnomAD major ancestry label eg. `nfe`
+
+        Returns:
+            np.ndarray: LD block matrix for the locus
+        """
+        idx = [row["idx"] for row in locus_index.select("idx").collect()]
+
+        half_matrix = (
+            BlockMatrix.read(
+                GnomADLDMatrix.ld_matrix_template.format(POP=gnomad_ancestry)
+            )
+            .filter(idx, idx)
+            .to_numpy()
+        )
+
+        return (half_matrix + half_matrix.T) - np.diag(np.diag(half_matrix))
```

### Comparing `gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/associations.py` & `gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/associations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Study Locus for GWAS Catalog data source."""
+
 from __future__ import annotations
 
 import importlib.resources as pkg_resources
 import json
 from dataclasses import dataclass
 from itertools import chain
 from typing import TYPE_CHECKING
@@ -28,14 +29,48 @@
 
 
 @dataclass
 class GWASCatalogCuratedAssociationsParser:
     """GWAS Catalog curated associations parser."""
 
     @staticmethod
+    def convert_gnomad_position_to_ensembl(
+        position: Column, reference: Column, alternate: Column
+    ) -> Column:
+        """Convert GnomAD variant position to Ensembl variant position.
+
+        For indels (the reference or alternate allele is longer than 1), then adding 1 to the position, for SNPs,
+        the position is unchanged. More info about the problem: https://www.biostars.org/p/84686/
+
+        Args:
+            position (Column): Position of the variant in GnomAD's coordinates system.
+            reference (Column): The reference allele in GnomAD's coordinates system.
+            alternate (Column): The alternate allele in GnomAD's coordinates system.
+
+        Returns:
+            Column: The position of the variant in the Ensembl genome.
+
+        Examples:
+            >>> d = [(1, "A", "C"), (2, "AA", "C"), (3, "A", "AA")]
+            >>> df = spark.createDataFrame(d).toDF("position", "reference", "alternate")
+            >>> df.withColumn("new_position", GWASCatalogCuratedAssociationsParser.convert_gnomad_position_to_ensembl(f.col("position"), f.col("reference"), f.col("alternate"))).show()
+            +--------+---------+---------+------------+
+            |position|reference|alternate|new_position|
+            +--------+---------+---------+------------+
+            |       1|        A|        C|           1|
+            |       2|       AA|        C|           3|
+            |       3|        A|       AA|           4|
+            +--------+---------+---------+------------+
+            <BLANKLINE>
+        """
+        return f.when(
+            (f.length(reference) > 1) | (f.length(alternate) > 1), position + 1
+        ).otherwise(position)
+
+    @staticmethod
     def _parse_pvalue(pvalue: Column) -> tuple[Column, Column]:
         """Parse p-value column.
 
         Args:
             pvalue (Column): p-value [string]
 
         Returns:
@@ -174,15 +209,16 @@
             DataFrame: GWAS Catalog associations data including `variantId`, `referenceAllele`,
             `alternateAllele`, `chromosome`, `position` with variant metadata
         """
         # Subset of GWAS Catalog associations required for resolving variant IDs:
         gwas_associations_subset = gwas_associations.select(
             "studyLocusId",
             f.col("CHR_ID").alias("chromosome"),
-            f.col("CHR_POS").cast(IntegerType()).alias("position"),
+            # The positions from GWAS Catalog are from ensembl that causes discrepancy for indels:
+            f.col("CHR_POS").cast(IntegerType()).alias("ensemblPosition"),
             # List of all SNPs associated with the variant
             GWASCatalogCuratedAssociationsParser._collect_rsids(
                 f.split(f.col("SNPS"), "; ").getItem(0),
                 f.col("SNP_ID_CURRENT"),
                 f.split(f.col("STRONGEST SNP-RISK ALLELE"), "; ").getItem(0),
             ).alias("rsIdsGwasCatalog"),
             GWASCatalogCuratedAssociationsParser._normalise_risk_allele(
@@ -190,34 +226,41 @@
             ).alias("riskAllele"),
         )
 
         # Subset of variant annotation required for GWAS Catalog annotations:
         va_subset = variant_annotation.df.select(
             "variantId",
             "chromosome",
+            # Calculate the position in Ensembl coordinates for indels:
+            GWASCatalogCuratedAssociationsParser.convert_gnomad_position_to_ensembl(
+                f.col("position"), f.col("referenceAllele"), f.col("alternateAllele")
+            ).alias("ensemblPosition"),
+            # Keeping GnomAD position:
             "position",
             f.col("rsIds").alias("rsIdsGnomad"),
             "referenceAllele",
             "alternateAllele",
             "alleleFrequencies",
             variant_annotation.max_maf().alias("maxMaf"),
         ).join(
             f.broadcast(
-                gwas_associations_subset.select("chromosome", "position").distinct()
+                gwas_associations_subset.select(
+                    "chromosome", "ensemblPosition"
+                ).distinct()
             ),
-            on=["chromosome", "position"],
+            on=["chromosome", "ensemblPosition"],
             how="inner",
         )
 
         # Semi-resolved ids (still contains duplicates when conclusion was not possible to make
         # based on rsIds or allele concordance)
         filtered_associations = (
             gwas_associations_subset.join(
                 f.broadcast(va_subset),
-                on=["chromosome", "position"],
+                on=["chromosome", "ensemblPosition"],
                 how="left",
             )
             .withColumn(
                 "rsIdFilter",
                 GWASCatalogCuratedAssociationsParser._flag_mappings_to_retain(
                     f.col("studyLocusId"),
                     GWASCatalogCuratedAssociationsParser._compare_rsids(
```

### Comparing `gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/study_index.py` & `gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/study_index.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,15 @@
                     "traitFromSource"
                 ),
                 f.col("INITIAL SAMPLE SIZE").alias("initialSampleSize"),
                 parse_efos(f.col("MAPPED_TRAIT_URI")).alias("traitFromSourceMappedIds"),
                 parse_efos(f.col("MAPPED BACKGROUND TRAIT URI")).alias(
                     "backgroundTraitFromSourceMappedIds"
                 ),
+                cls.parse_cohorts(f.col("COHORT")).alias("cohorts"),
             ),
             _schema=StudyIndexGWASCatalog.get_schema(),
         )
 
     @classmethod
     def from_source(
         cls: type[StudyIndexGWASCatalogParser],
@@ -544,22 +545,14 @@
                     *[f.expr(column2camel_case(x)) for x in df.columns]
                 )
             ).withColumnRenamed(
                 "studyAccession", "studyId"
             )  # studyId has not been split yet
         )
 
-        # Parsing cohort information:
-        cohorts = ancestry_lut.select(
-            f.col("STUDY ACCESSION").alias("studyId"),
-            GWASCatalogStudyIndexParser.parse_cohorts(f.col("COHORT(S)")).alias(
-                "cohorts"
-            ),
-        ).distinct()
-
         # Get a high resolution dataset on experimental stage:
         ancestry_stages = (
             ancestry.groupBy("studyId")
             .pivot("stage")
             .agg(
                 f.collect_set(
                     f.struct(
@@ -640,17 +633,15 @@
         )
 
         parsed_ancestry_lut = ancestry_stages.join(
             europeans_deconvoluted, on="studyId", how="outer"
         ).select(
             "studyId", "discoverySamples", "ldPopulationStructure", "replicationSamples"
         )
-        self.df = self.df.join(parsed_ancestry_lut, on="studyId", how="left").join(
-            cohorts, on="studyId", how="left"
-        )
+        self.df = self.df.join(parsed_ancestry_lut, on="studyId", how="left")
         return self
 
     def annotate_sumstats_info(
         self: StudyIndexGWASCatalog, sumstats_lut: DataFrame
     ) -> StudyIndexGWASCatalog:
         """Annotate summary stat locations.
```

### Comparing `gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/study_splitter.py` & `gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/study_splitter.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/gwas_catalog/summary_statistics.py` & `gentropy-1.3.0/src/gentropy/datasource/gwas_catalog/summary_statistics.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/intervals/andersson.py` & `gentropy-1.3.0/src/gentropy/datasource/intervals/andersson.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/intervals/javierre.py` & `gentropy-1.3.0/src/gentropy/datasource/intervals/javierre.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/intervals/jung.py` & `gentropy-1.3.0/src/gentropy/datasource/intervals/jung.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/intervals/thurman.py` & `gentropy-1.3.0/src/gentropy/datasource/intervals/thurman.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                 t.StructField("gene_name", t.StringType(), False),
                 t.StructField("chrom", t.StringType(), False),
                 t.StructField("start", t.IntegerType(), False),
                 t.StructField("end", t.IntegerType(), False),
                 t.StructField("score", t.FloatType(), False),
             ]
         )
-        return spark.read.csv(path, sep="\t", header=True, schema=thurman_schema)
+        return spark.read.csv(path, sep="\t", header=False, schema=thurman_schema)
 
     @classmethod
     def parse(
         cls: type[IntervalsThurman],
         thurman_raw: DataFrame,
         gene_index: GeneIndex,
         lift: LiftOverSpark,
```

### Comparing `gentropy-1.2.0/src/gentropy/datasource/open_targets/l2g_gold_standard.py` & `gentropy-1.3.0/src/gentropy/datasource/open_targets/l2g_gold_standard.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/open_targets/target.py` & `gentropy-1.3.0/src/gentropy/datasource/open_targets/target.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/datasource/ukbiobank/study_index.py` & `gentropy-1.3.0/src/gentropy/datasource/ukbiobank/study_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/eqtl_catalogue.py` & `gentropy-1.3.0/src/gentropy/eqtl_catalogue.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/finngen_finemapping_ingestion.py` & `gentropy-1.3.0/src/gentropy/finngen_finemapping_ingestion.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/finngen_studies.py` & `gentropy-1.3.0/src/gentropy/finngen_studies.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/finngen_sumstat_preprocess.py` & `gentropy-1.3.0/src/gentropy/finngen_sumstat_preprocess.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/gene_index.py` & `gentropy-1.3.0/src/gentropy/gene_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/gwas_catalog_ingestion.py` & `gentropy-1.3.0/src/gentropy/gwas_catalog_ingestion.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/gwas_catalog_study_curation.py` & `gentropy-1.3.0/src/gentropy/gwas_catalog_study_curation.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/gwas_catalog_study_inclusion.py` & `gentropy-1.3.0/src/gentropy/gwas_catalog_study_inclusion.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/gwas_catalog_sumstat_preprocess.py` & `gentropy-1.3.0/src/gentropy/gwas_catalog_sumstat_preprocess.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/l2g.py` & `gentropy-1.3.0/src/gentropy/l2g.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,17 @@
         credible_set = StudyLocus.from_parquet(
             session, credible_set_path, recursiveFileLookup=True
         )
         studies = StudyIndex.from_parquet(
             session, study_index_path, recursiveFileLookup=True
         )
         v2g = V2G.from_parquet(session, variant_gene_path)
-        coloc = Colocalisation.from_parquet(session, colocalisation_path)
+        coloc = Colocalisation.from_parquet(
+            session, colocalisation_path, recursiveFileLookup=True
+        )
 
         if run_mode == "predict":
             if not model_path or not predictions_path:
                 raise ValueError(
                     "model_path and predictions_path must be set for predict mode."
                 )
             predictions = L2GPrediction.from_credible_set(
@@ -87,15 +89,15 @@
             session.logger.info(predictions_path)
         elif (
             run_mode == "train"
             and gold_standard_curation_path
             and gene_interactions_path
         ):
             # Process gold standard and L2G features
-            gs_curation = session.spark.read.json(gold_standard_curation_path).persist()
+            gs_curation = session.spark.read.json(gold_standard_curation_path)
             interactions = session.spark.read.parquet(gene_interactions_path)
             study_locus_overlap = StudyLocus(
                 # We just extract overlaps of associations in the gold standard. This parsing is a duplication of the one in the gold standard curation,
                 # but we need to do it here to be able to parse gold standards later
                 _df=credible_set.df.join(
                     f.broadcast(
                         gs_curation.select(
@@ -122,31 +124,35 @@
                 v2g=v2g,
                 study_locus_overlap=study_locus_overlap,
                 interactions=interactions,
             )
 
             fm = L2GFeatureMatrix.generate_features(
                 features_list=features_list,
-                study_locus=credible_set,
+                credible_set=credible_set,
                 study_index=studies,
                 variant_gene=v2g,
                 colocalisation=coloc,
             )
 
-            # Join and fill null values with 0
-            data = L2GFeatureMatrix(
-                _df=fm.df.join(
-                    f.broadcast(
-                        gold_standards.df.drop("variantId", "studyId", "sources")
+            data = (
+                # Annotate gold standards with features
+                L2GFeatureMatrix(
+                    _df=fm.df.join(
+                        f.broadcast(
+                            gold_standards.df.drop("variantId", "studyId", "sources")
+                        ),
+                        on=["studyLocusId", "geneId"],
+                        how="inner",
                     ),
-                    on=["studyLocusId", "geneId"],
-                    how="inner",
-                ),
-                _schema=L2GFeatureMatrix.get_schema(),
-            ).fill_na()
+                    _schema=L2GFeatureMatrix.get_schema(),
+                )
+                .fill_na()
+                .select_features(list(features_list))
+            )
 
             # Instantiate classifier
             estimator = SparkXGBClassifier(
                 eval_metric="logloss",
                 features_col="features",
                 label_col="label",
                 max_depth=5,
@@ -161,16 +167,15 @@
                     l2g_model=l2g_model,
                     data=data,
                     num_folds=cv_folds,
                 )
             else:
                 # Train model
                 LocusToGeneTrainer.train(
-                    data=data,
+                    gold_standard_data=data,
                     l2g_model=l2g_model,
-                    features_list=list(features_list),
                     model_path=model_path,
                     evaluate=True,
                     wandb_run_name=wandb_run_name,
                     **hyperparameters,
                 )
                 session.logger.info(model_path)
```

### Comparing `gentropy-1.2.0/src/gentropy/ld_based_clumping.py` & `gentropy-1.3.0/src/gentropy/ld_based_clumping.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/ld_index.py` & `gentropy-1.3.0/src/gentropy/ld_index.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/method/carma.py` & `gentropy-1.3.0/src/gentropy/method/carma.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """CARMA outlier detection method."""
 from __future__ import annotations
 
 import concurrent.futures
+import warnings
 from itertools import combinations
 from math import floor, lgamma
 from typing import Any
 
 import numpy as np
 import pandas as pd
 from scipy.linalg import det, inv, pinv
@@ -28,14 +29,16 @@
 
         Returns:
             dict[str, Any]: A dictionary containing the following results:
                 - PIPs: A numeric vector of posterior inclusion probabilities (PIPs) for all SNPs or None.
                 - B_list: A dataframe containing the marginal likelihoods and the corresponding model space or None.
                 - Outliers: A list of outlier SNPs or None.
         """
+        # Ignore pandas future warnings
+        warnings.simplefilter(action="ignore", category=FutureWarning)
         try:
             # Execute CARMA.CARMA_spike_slab_noEM with a timeout
             with concurrent.futures.ThreadPoolExecutor(max_workers=1) as executor:
                 future = executor.submit(CARMA.CARMA_spike_slab_noEM, z=z, ld=ld)
                 result = future.result(timeout=sec_threshold)
         except concurrent.futures.TimeoutError:
             # If execution exceeds the timeout, return None
@@ -850,17 +853,27 @@
                         )
                         S = set_gamma[sec_sample[0]][ind_sec].tolist()
                     else:
                         aa = set_star["margin"] - max(set_star["margin"])
                         sec_sample = np.random.choice(
                             range(0, 3), 1, p=np.exp(aa) / np.sum(np.exp(aa))
                         )
-                        S = set_gamma[sec_sample[0]][
-                            int(set_star["gamma_set_index"][sec_sample[0]])
-                        ].tolist()
+                        if set_gamma[sec_sample[0]] is not None:
+                            S = set_gamma[sec_sample[0]][
+                                int(set_star["gamma_set_index"][sec_sample[0]])
+                            ].tolist()
+                        else:
+                            sec_sample = np.random.choice(
+                                range(1, 3),
+                                1,
+                                p=np.exp(aa)[[1, 2]] / np.sum(np.exp(aa)[[1, 2]]),
+                            )
+                            S = set_gamma[sec_sample[0]][
+                                int(set_star["gamma_set_index"][sec_sample[0]])
+                            ].tolist()
 
                 for item in conditional_S:
                     if item not in S:
                         S.append(item)
             # END h_ind loop
             #
             if conditional_S is not None:
```

### Comparing `gentropy-1.2.0/src/gentropy/method/clump.py` & `gentropy-1.3.0/src/gentropy/method/clump.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/method/colocalisation.py` & `gentropy-1.3.0/src/gentropy/method/colocalisation.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 class ECaviar:
     """ECaviar-based colocalisation analysis.
 
     It extends [CAVIAR](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5142122/#bib18) framework to explicitly estimate the posterior probability that the same variant is causal in 2 studies while accounting for the uncertainty of LD. eCAVIAR computes the colocalization posterior probability (**CLPP**) by utilizing the marginal posterior probabilities. This framework allows for **multiple variants to be causal** in a single locus.
     """
 
+    METHOD_NAME: str = "eCAVIAR"
+    METHOD_METRIC: str = "clpp"
+
     @staticmethod
     def _get_clpp(left_pp: Column, right_pp: Column) -> Column:
         """Calculate the colocalisation posterior probability (CLPP).
 
         If the fact that the same variant is found causal for two studies are independent events,
         CLPP is defined as the product of posterior porbabilities that a variant is causal in both studies.
 
@@ -77,15 +80,15 @@
                     ),
                 )
                 .groupBy("leftStudyLocusId", "rightStudyLocusId", "chromosome")
                 .agg(
                     f.count("*").alias("numberColocalisingVariants"),
                     f.sum(f.col("clpp")).alias("clpp"),
                 )
-                .withColumn("colocalisationMethod", f.lit("eCAVIAR"))
+                .withColumn("colocalisationMethod", f.lit(cls.METHOD_NAME))
             ),
             _schema=Colocalisation.get_schema(),
         )
 
 
 class Coloc:
     """Calculate bayesian colocalisation based on overlapping signals from credible sets.
@@ -104,14 +107,16 @@
 
         Coloc requires the availability of Bayes factors (BF) for each variant in the credible set (`logBF` column).
 
     Attributes:
         PSEUDOCOUNT (float): Pseudocount to avoid log(0). Defaults to 1e-10.
     """
 
+    METHOD_NAME: str = "COLOC"
+    METHOD_METRIC: str = "llr"
     PSEUDOCOUNT: float = 1e-10
 
     @staticmethod
     def _get_posteriors(all_bfs: NDArray[np.float64]) -> DenseVector:
         """Calculate posterior probabilities for each hypothesis.
 
         Args:
@@ -150,32 +155,32 @@
             Colocalisation: Colocalisation results
         """
         # register udfs
         logsum = f.udf(get_logsum, DoubleType())
         posteriors = f.udf(Coloc._get_posteriors, VectorUDT())
         return Colocalisation(
             _df=(
-                overlapping_signals.df
+                overlapping_signals.df.select("*", "statistics.*")
                 # Before summing log_BF columns nulls need to be filled with 0:
-                .fillna(0, subset=["statistics.left_logBF", "statistics.right_logBF"])
+                .fillna(0, subset=["left_logBF", "right_logBF"])
                 # Sum of log_BFs for each pair of signals
                 .withColumn(
                     "sum_log_bf",
-                    f.col("statistics.left_logBF") + f.col("statistics.right_logBF"),
+                    f.col("left_logBF") + f.col("right_logBF"),
                 )
                 # Group by overlapping peak and generating dense vectors of log_BF:
                 .groupBy("chromosome", "leftStudyLocusId", "rightStudyLocusId")
                 .agg(
                     f.count("*").alias("numberColocalisingVariants"),
-                    fml.array_to_vector(
-                        f.collect_list(f.col("statistics.left_logBF"))
-                    ).alias("left_logBF"),
-                    fml.array_to_vector(
-                        f.collect_list(f.col("statistics.right_logBF"))
-                    ).alias("right_logBF"),
+                    fml.array_to_vector(f.collect_list(f.col("left_logBF"))).alias(
+                        "left_logBF"
+                    ),
+                    fml.array_to_vector(f.collect_list(f.col("right_logBF"))).alias(
+                        "right_logBF"
+                    ),
                     fml.array_to_vector(f.collect_list(f.col("sum_log_bf"))).alias(
                         "sum_log_bf"
                     ),
                 )
                 .withColumn("logsum1", logsum(f.col("left_logBF")))
                 .withColumn("logsum2", logsum(f.col("right_logBF")))
                 .withColumn("logsum12", logsum(f.col("sum_log_bf")))
@@ -249,11 +254,11 @@
                     "h4h3",
                     "lH0bf",
                     "lH1bf",
                     "lH2bf",
                     "lH3bf",
                     "lH4bf",
                 )
-                .withColumn("colocalisationMethod", f.lit("COLOC"))
+                .withColumn("colocalisationMethod", f.lit(cls.METHOD_NAME))
             ),
             _schema=Colocalisation.get_schema(),
         )
```

### Comparing `gentropy-1.2.0/src/gentropy/method/l2g/evaluator.py` & `gentropy-1.3.0/src/gentropy/method/l2g/evaluator.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/method/l2g/feature_factory.py` & `gentropy-1.3.0/src/gentropy/method/l2g/feature_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,263 +1,210 @@
 """Collection of methods that extract features from the gentropy datasets to be fed in L2G."""
 from __future__ import annotations
 
 from functools import reduce
+from itertools import chain
 from typing import TYPE_CHECKING
 
 import pyspark.sql.functions as f
 
 from gentropy.common.spark_helpers import (
     convert_from_wide_to_long,
     get_record_with_maximum_value,
 )
 from gentropy.dataset.l2g_feature import L2GFeature
 from gentropy.dataset.study_locus import CredibleInterval, StudyLocus
+from gentropy.method.colocalisation import Coloc, ECaviar
 
 if TYPE_CHECKING:
     from pyspark.sql import Column, DataFrame
 
     from gentropy.dataset.colocalisation import Colocalisation
     from gentropy.dataset.study_index import StudyIndex
     from gentropy.dataset.v2g import V2G
 
 
 class ColocalisationFactory:
     """Feature extraction in colocalisation."""
 
+    @classmethod
+    def _add_colocalisation_metric(cls: type[ColocalisationFactory]) -> Column:
+        """Expression that adds a `colocalisationMetric` column to the colocalisation dataframe in preparation for feature extraction.
+
+        Returns:
+            Column: The expression that adds a `colocalisationMetric` column with the derived metric
+        """
+        method_metric_map = {
+            ECaviar.METHOD_NAME: ECaviar.METHOD_METRIC,
+            Coloc.METHOD_NAME: Coloc.METHOD_METRIC,
+        }
+        map_expr = f.create_map(*[f.lit(x) for x in chain(*method_metric_map.items())])
+        return map_expr[f.col("colocalisationMethod")].alias("colocalisationMetric")
+
     @staticmethod
-    def _get_max_coloc_per_study_locus(
-        study_locus: StudyLocus,
-        studies: StudyIndex,
+    def _get_max_coloc_per_credible_set(
         colocalisation: Colocalisation,
-        colocalisation_method: str,
+        credible_set: StudyLocus,
+        studies: StudyIndex,
     ) -> L2GFeature:
         """Get the maximum colocalisation posterior probability for each pair of overlapping study-locus per type of colocalisation method and QTL type.
 
         Args:
-            study_locus (StudyLocus): Study locus dataset
-            studies (StudyIndex): Study index dataset
             colocalisation (Colocalisation): Colocalisation dataset
-            colocalisation_method (str): Colocalisation method to extract the max from
+            credible_set (StudyLocus): Study locus dataset
+            studies (StudyIndex): Study index dataset
 
         Returns:
             L2GFeature: Stores the features with the max coloc probabilities for each pair of study-locus
-
-        Raises:
-            ValueError: If the colocalisation method is not supported
         """
-        if colocalisation_method not in ["COLOC", "eCAVIAR"]:
-            raise ValueError(
-                f"Colocalisation method {colocalisation_method} not supported"
-            )
-        if colocalisation_method == "COLOC":
-            coloc_score_col_name = "log2h4h3"
-            coloc_feature_col_template = "ColocLlrMaximum"
-
-        elif colocalisation_method == "eCAVIAR":
-            coloc_score_col_name = "clpp"
-            coloc_feature_col_template = "ColocClppMaximum"
+        colocalisation_df = colocalisation.df.select(
+            f.col("leftStudyLocusId").alias("studyLocusId"),
+            "rightStudyLocusId",
+            f.coalesce("log2h4h3", "clpp").alias("score"),
+            ColocalisationFactory._add_colocalisation_metric(),
+        )
 
-        colocalising_study_locus = (
-            study_locus.df.select("studyLocusId", "studyId")
+        colocalising_credible_sets = (
+            credible_set.df.select("studyLocusId", "studyId")
             # annotate studyLoci with overlapping IDs on the left - to just keep GWAS associations
             .join(
-                colocalisation.df.selectExpr(
-                    "leftStudyLocusId as studyLocusId",
-                    "rightStudyLocusId",
-                    "colocalisationMethod",
-                    f"{coloc_score_col_name} as coloc_score",
-                ),
+                colocalisation_df,
                 on="studyLocusId",
                 how="inner",
             )
             # bring study metadata to just keep QTL studies on the right
             .join(
-                study_locus.df.selectExpr(
-                    "studyLocusId as rightStudyLocusId", "studyId as right_studyId"
+                credible_set.df.join(
+                    studies.df.select("studyId", "studyType", "geneId"), "studyId"
+                ).selectExpr(
+                    "studyLocusId as rightStudyLocusId",
+                    "studyType as right_studyType",
+                    "geneId",
                 ),
                 on="rightStudyLocusId",
                 how="inner",
             )
-            .join(
-                f.broadcast(
-                    studies.df.selectExpr(
-                        "studyId as right_studyId",
-                        "studyType as right_studyType",
-                        "geneId",
-                    )
-                ),
-                on="right_studyId",
-                how="inner",
-            )
-            .filter(
-                (f.col("colocalisationMethod") == colocalisation_method)
-                & (f.col("right_studyType") != "gwas")
+            .filter(f.col("right_studyType") != "gwas")
+            .select(
+                "studyLocusId",
+                "right_studyType",
+                "geneId",
+                "score",
+                "colocalisationMetric",
             )
-            .select("studyLocusId", "right_studyType", "geneId", "coloc_score")
         )
 
-        # Max PP calculation per studyLocus AND type of QTL
-        local_max = get_record_with_maximum_value(
-            colocalising_study_locus,
-            ["studyLocusId", "right_studyType", "geneId"],
-            "coloc_score",
-        ).persist()
-
-        intercept = 0.0001
-        neighbourhood_max = (
-            (
-                local_max.selectExpr(
-                    "studyLocusId", "coloc_score as coloc_local_max", "geneId"
-                )
-                .join(
-                    # Add maximum in the neighborhood
-                    get_record_with_maximum_value(
-                        colocalising_study_locus.withColumnRenamed(
-                            "coloc_score", "coloc_neighborhood_max"
-                        ),
-                        ["studyLocusId", "right_studyType"],
-                        "coloc_neighborhood_max",
-                    ).drop("geneId"),
-                    on="studyLocusId",
-                )
-                .withColumn(
-                    f"{coloc_feature_col_template}Neighborhood",
-                    f.log10(
-                        f.abs(
-                            f.col("coloc_local_max")
-                            - f.col("coloc_neighborhood_max")
-                            + f.lit(intercept)
-                        )
-                    ),
-                )
+        # Max PP calculation per credible set AND type of QTL AND colocalisation method
+        local_max = (
+            get_record_with_maximum_value(
+                colocalising_credible_sets,
+                ["studyLocusId", "right_studyType", "geneId", "colocalisationMetric"],
+                "score",
+            )
+            .select(
+                "*",
+                f.col("score").alias("max_score"),
+                f.lit("Local").alias("score_type"),
             )
-            .drop("coloc_neighborhood_max", "coloc_local_max")
-            .persist()
+            .drop("score")
         )
 
-        # Split feature per molQTL
-        local_dfs = []
-        nbh_dfs = []
-        qtl_types: list[str] = (
-            colocalising_study_locus.select("right_studyType")
-            .distinct()
-            .toPandas()["right_studyType"]
-            .tolist()
-        ) or ["eqtl", "pqtl", "sqtl"]
-        for qtl_type in qtl_types:
-            filtered_local_max = (
-                local_max.filter(f.col("right_studyType") == qtl_type)
-                .withColumnRenamed(
-                    "coloc_score",
-                    f"{qtl_type}{coloc_feature_col_template}",
-                )
-                .drop("right_studyType")
+        neighbourhood_max = (
+            local_max.selectExpr(
+                "studyLocusId", "max_score as local_max_score", "geneId"
             )
-            local_dfs.append(filtered_local_max)
-
-            filtered_neighbourhood_max = (
-                neighbourhood_max.filter(f.col("right_studyType") == qtl_type)
-                .withColumnRenamed(
-                    f"{coloc_feature_col_template}Neighborhood",
-                    f"{qtl_type}{coloc_feature_col_template}Neighborhood",
-                )
-                .drop("right_studyType")
+            .join(
+                # Add maximum in the neighborhood
+                get_record_with_maximum_value(
+                    colocalising_credible_sets.withColumnRenamed(
+                        "score", "tmp_nbh_max_score"
+                    ),
+                    ["studyLocusId", "right_studyType", "colocalisationMetric"],
+                    "tmp_nbh_max_score",
+                ).drop("geneId"),
+                on="studyLocusId",
             )
-            nbh_dfs.append(filtered_neighbourhood_max)
-
-        wide_dfs = reduce(
-            lambda x, y: x.unionByName(y, allowMissingColumns=True),
-            local_dfs + nbh_dfs,
-        )
-
-        return L2GFeature(
-            _df=convert_from_wide_to_long(
-                wide_dfs.groupBy("studyLocusId", "geneId").agg(
-                    *(
-                        f.first(f.col(c), ignorenulls=True).alias(c)
-                        for c in wide_dfs.columns
-                        if c
-                        not in [
-                            "studyLocusId",
-                            "geneId",
-                        ]
+            .withColumn("score_type", f.lit("Neighborhood"))
+            .withColumn(
+                "max_score",
+                f.log10(
+                    f.abs(
+                        f.col("local_max_score")
+                        - f.col("tmp_nbh_max_score")
+                        + f.lit(0.0001)  # intercept
                     )
                 ),
-                id_vars=("studyLocusId", "geneId"),
-                var_name="featureName",
-                value_name="featureValue",
-            ),
-            _schema=L2GFeature.get_schema(),
-        )
-
-    @staticmethod
-    def _get_coloc_features(
-        study_locus: StudyLocus, studies: StudyIndex, colocalisation: Colocalisation
-    ) -> L2GFeature:
-        """Calls _get_max_coloc_per_study_locus for both methods and concatenates the results.
-
-        !!! note "Colocalisation features are only available for the eCAVIAR results for now."
-
-        Args:
-            study_locus (StudyLocus): Study locus dataset
-            studies (StudyIndex): Study index dataset
-            colocalisation (Colocalisation): Colocalisation dataset
-
-        Returns:
-            L2GFeature: Stores the features with the max coloc probabilities for each pair of study-locus
-        """
-        coloc_clpp = ColocalisationFactory._get_max_coloc_per_study_locus(
-            study_locus,
-            studies,
-            colocalisation,
-            "eCAVIAR",
-        )
+            )
+        ).drop("tmp_nbh_max_score", "local_max_score")
 
         return L2GFeature(
-            _df=coloc_clpp.df,
+            _df=(
+                # Combine local and neighborhood metrics
+                local_max.unionByName(
+                    neighbourhood_max, allowMissingColumns=True
+                ).select(
+                    "studyLocusId",
+                    "geneId",
+                    # Feature name is a concatenation of the QTL type, colocalisation metric and if it's local or in the vicinity
+                    f.concat_ws(
+                        "",
+                        f.col("right_studyType"),
+                        f.lit("Coloc"),
+                        f.initcap(f.col("colocalisationMetric")),
+                        f.lit("Maximum"),
+                        f.regexp_replace(f.col("score_type"), "Local", ""),
+                    ).alias("featureName"),
+                    f.col("max_score").cast("float").alias("featureValue"),
+                )
+            ),
             _schema=L2GFeature.get_schema(),
         )
 
 
 class StudyLocusFactory(StudyLocus):
     """Feature extraction in study locus."""
 
     @staticmethod
-    def _get_tss_distance_features(
-        study_locus: StudyLocus, distances: V2G
-    ) -> L2GFeature:
-        """Joins StudyLocus with the V2G to extract the minimum distance to a gene TSS of all variants in a StudyLocus credible set.
+    def _get_tss_distance_features(credible_set: StudyLocus, v2g: V2G) -> L2GFeature:
+        """Joins StudyLocus with the V2G to extract a score that is based on the distance to a gene TSS of any variant weighted by its posterior probability in a credible set.
 
         Args:
-            study_locus (StudyLocus): Study locus dataset
-            distances (V2G): Dataframe containing the distances of all variants to all genes TSS within a region
+            credible_set (StudyLocus): Credible set dataset
+            v2g (V2G): Dataframe containing the distances of all variants to all genes TSS within a region
 
         Returns:
-            L2GFeature: Stores the features with the minimum distance among all variants in the credible set and a gene TSS.
+            L2GFeature: Stores the features with the score of weighting the distance to the TSS by the posterior probability of the variant
 
         """
         wide_df = (
-            study_locus.filter_credible_set(CredibleInterval.IS95)
-            .df.select(
+            credible_set.filter_credible_set(CredibleInterval.IS95)
+            .df.withColumn("variantInLocus", f.explode_outer("locus"))
+            .select(
                 "studyLocusId",
                 "variantId",
-                f.explode("locus.variantId").alias("tagVariantId"),
+                f.col("variantInLocus.variantId").alias("variantInLocusId"),
+                f.col("variantInLocus.posteriorProbability").alias(
+                    "variantInLocusPosteriorProbability"
+                ),
             )
             .join(
-                distances.df.selectExpr(
-                    "variantId as tagVariantId", "geneId", "distance"
+                v2g.df.filter(f.col("datasourceId") == "canonical_tss").selectExpr(
+                    "variantId as variantInLocusId", "geneId", "score"
                 ),
-                on="tagVariantId",
+                on="variantInLocusId",
                 how="inner",
             )
+            .withColumn(
+                "weightedScore",
+                f.col("score") * f.col("variantInLocusPosteriorProbability"),
+            )
             .groupBy("studyLocusId", "geneId")
             .agg(
-                f.min("distance").alias("distanceTssMinimum"),
-                f.mean("distance").alias("distanceTssMean"),
+                f.min("weightedScore").alias("distanceTssMinimum"),
+                f.mean("weightedScore").alias("distanceTssMean"),
             )
         )
 
         return L2GFeature(
             _df=convert_from_wide_to_long(
                 wide_df,
                 id_vars=("studyLocusId", "geneId"),
@@ -317,58 +264,59 @@
                     f.collect_set("geneId").alias("geneId"),
                 )
                 .withColumn("geneId", f.explode("geneId"))
             )
 
         credible_set_w_variant_consequences = (
             credible_set.filter_credible_set(CredibleInterval.IS95)
-            .df.withColumn("variantInLocusId", f.explode(f.col("locus.variantId")))
-            .withColumn(
-                "variantInLocusPosteriorProbability",
-                f.explode(f.col("locus.posteriorProbability")),
+            .df.withColumn("variantInLocus", f.explode_outer("locus"))
+            .select(
+                f.col("studyLocusId"),
+                f.col("variantId"),
+                f.col("studyId"),
+                f.col("variantInLocus.variantId").alias("variantInLocusId"),
+                f.col("variantInLocus.posteriorProbability").alias(
+                    "variantInLocusPosteriorProbability"
+                ),
             )
             .join(
                 # Join with V2G to get variant consequences
-                v2g.df.filter(
-                    f.col("datasourceId") == "variantConsequence"
-                ).withColumnRenamed("variantId", "variantInLocusId"),
+                v2g.df.filter(f.col("datasourceId") == "variantConsequence").selectExpr(
+                    "variantId as variantInLocusId", "geneId", "score"
+                ),
                 on="variantInLocusId",
             )
-            .withColumn(
-                "weightedScore",
-                f.col("score") * f.col("variantInLocusPosteriorProbability"),
-            )
             .select(
                 "studyLocusId",
                 "variantId",
                 "studyId",
                 "geneId",
-                "score",
-                "weightedScore",
+                (f.col("score") * f.col("variantInLocusPosteriorProbability")).alias(
+                    "weightedScore"
+                ),
             )
             .distinct()
-            .persist()
         )
 
         return L2GFeature(
             _df=convert_from_wide_to_long(
                 reduce(
                     lambda x, y: x.unionByName(y, allowMissingColumns=True),
                     [
                         # Calculate overall max VEP score for all genes in the vicinity
                         credible_set_w_variant_consequences.transform(
                             _aggregate_vep_feature,
-                            f.max("score"),
+                            f.max("weightedScore"),
                             ["studyLocusId"],
                             "vepMaximumNeighborhood",
                         ),
                         # Calculate overall max VEP score per gene
                         credible_set_w_variant_consequences.transform(
                             _aggregate_vep_feature,
-                            f.max("score"),
+                            f.max("weightedScore"),
                             ["studyLocusId", "geneId"],
                             "vepMaximum",
                         ),
                         # Calculate mean VEP score for all genes in the vicinity
                         credible_set_w_variant_consequences.transform(
                             _aggregate_vep_feature,
                             f.mean("weightedScore"),
```

### Comparing `gentropy-1.2.0/src/gentropy/method/l2g/model.py` & `gentropy-1.3.0/src/gentropy/method/l2g/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -203,40 +203,43 @@
         return self
 
     def evaluate(
         self: LocusToGeneModel,
         results: DataFrame,
         hyperparameters: dict[str, Any],
         wandb_run_name: str | None,
-        training_data: L2GFeatureMatrix | None = None,
+        gold_standard_data: L2GFeatureMatrix | None = None,
     ) -> None:
         """Perform evaluation of the model predictions for the test set and track the results with W&B.
 
         Args:
             results (DataFrame): Dataframe containing the predictions
             hyperparameters (dict[str, Any]): Hyperparameters used for the model
             wandb_run_name (str | None): Descriptive name for the run to be tracked with W&B
-            training_data (L2GFeatureMatrix | None): Training data used for the model. If provided, the ratio of positive to negative labels will be logged to W&B
+            gold_standard_data (L2GFeatureMatrix | None): Feature matrix for the associations in the gold standard. If provided, the ratio of positive to negative labels will be logged to W&B
         """
         binary_evaluator = BinaryClassificationEvaluator(
             rawPredictionCol="rawPrediction", labelCol="label"
         )
         multi_evaluator = MulticlassClassificationEvaluator(
             labelCol="label", predictionCol="prediction"
         )
 
-        if wandb_run_name and training_data:
+        if wandb_run_name and gold_standard_data:
             run = wandb_init(
                 project=self.wandb_l2g_project_name,
                 config=hyperparameters,
                 name=wandb_run_name,
             )
             if isinstance(run, Run):
                 self.log_to_wandb(
-                    results, training_data, [binary_evaluator, multi_evaluator], run
+                    results,
+                    gold_standard_data,
+                    [binary_evaluator, multi_evaluator],
+                    run,
                 )
                 run.finish()
 
     @property
     def feature_name_map(self: LocusToGeneModel) -> dict[str, str]:
         """Return a dictionary mapping encoded feature names to the original names.
```

### Comparing `gentropy-1.2.0/src/gentropy/method/l2g/trainer.py` & `gentropy-1.3.0/src/gentropy/method/l2g/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,46 +18,44 @@
 
     _model: LocusToGeneModel
     train_set: L2GFeatureMatrix
 
     @classmethod
     def train(
         cls: type[LocusToGeneTrainer],
-        data: L2GFeatureMatrix,
+        gold_standard_data: L2GFeatureMatrix,
         l2g_model: LocusToGeneModel,
-        features_list: list[str],
         evaluate: bool,
         wandb_run_name: str | None = None,
         model_path: str | None = None,
         **hyperparams: dict[str, Any],
     ) -> LocusToGeneModel:
         """Train the Locus to Gene model.
 
         Args:
-            data (L2GFeatureMatrix): Feature matrix containing the data
+            gold_standard_data (L2GFeatureMatrix): Feature matrix for the associations in the gold standard
             l2g_model (LocusToGeneModel): Model to fit to the data on
-            features_list (list[str]): List of features to use for the model
             evaluate (bool): Whether to evaluate the model on a test set
             wandb_run_name (str | None): Descriptive name for the run to be tracked with W&B
             model_path (str | None): Path to save the model to
             **hyperparams (dict[str, Any]): Hyperparameters to use for the model
 
         Returns:
             LocusToGeneModel: Trained model
         """
-        train, test = data.select_features(features_list).train_test_split(fraction=0.8)
+        train, test = gold_standard_data.train_test_split(fraction=0.8)
 
         model = l2g_model.add_pipeline_stage(l2g_model.estimator).fit(train)
 
         if evaluate:
             l2g_model.evaluate(
                 results=model.predict(test),
                 hyperparameters=hyperparams,
                 wandb_run_name=wandb_run_name,
-                training_data=train,
+                gold_standard_data=gold_standard_data,
             )
         if model_path:
             l2g_model.save(model_path)
         return l2g_model
 
     @classmethod
     def cross_validate(
```

### Comparing `gentropy-1.2.0/src/gentropy/method/ld.py` & `gentropy-1.3.0/src/gentropy/method/ld.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/method/pics.py` & `gentropy-1.3.0/src/gentropy/method/pics.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/method/susie_inf.py` & `gentropy-1.3.0/src/gentropy/method/susie_inf.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         V: np.ndarray | None = None,
         Dsq: np.ndarray | None = None,
         est_ssq: bool = True,
         ssq: np.ndarray | None = None,
         ssq_range: tuple[float, float] = (0, 1),
         pi0: np.ndarray | None = None,
         est_sigmasq: bool = True,
-        est_tausq: bool = True,
+        est_tausq: bool = False,
         sigmasq: float = 1,
         tausq: float = 0,
         sigmasq_range: tuple[float, float] | None = None,
         tausq_range: tuple[float, float] | None = None,
         PIP: np.ndarray | None = None,
         mu: np.ndarray | None = None,
         method: str = "moments",
@@ -395,15 +395,15 @@
                 sigmasq = res.x
         return sigmasq, tausq
 
     @staticmethod
     def cred_inf(
         PIP: np.ndarray,
         n: int = 100_000,
-        coverage: float = 0.9,
+        coverage: float = 0.99,
         purity: float = 0.5,
         LD: np.ndarray | None = None,
         V: np.ndarray | None = None,
         Dsq: np.ndarray | None = None,
         dedup: bool = True,
     ) -> list[Any]:
         """Compute credible sets from single-effect PIPs.
```

### Comparing `gentropy-1.2.0/src/gentropy/method/window_based_clumping.py` & `gentropy-1.3.0/src/gentropy/method/window_based_clumping.py`

 * *Files 23% similar despite different names*

```diff
@@ -147,52 +147,51 @@
             else:
                 # None of the leads were within the window:
                 lead_indices.append(index)
                 is_lead[index] = 1
 
         return DenseVector(is_lead)
 
-    @classmethod
+    @staticmethod
     def clump(
-        cls: type[WindowBasedClumping],
-        summary_stats: SummaryStatistics,
-        window_length: int,
-        p_value_significance: float = 5e-8,
+        summary_statistics: SummaryStatistics,
+        distance: int = 500_000,
+        gwas_significance: float = 5e-8,
     ) -> StudyLocus:
-        """Clump summary statistics by distance.
+        """Clump significant signals from summary statistics based on window.
 
         Args:
-            summary_stats (SummaryStatistics): summary statistics to clump
-            window_length (int): window length in basepair
-            p_value_significance (float): only more significant variants are considered
+            summary_statistics (SummaryStatistics): Summary statistics to be used for clumping.
+            distance (int): Distance in base pairs to be used for clumping. Defaults to 500_000.
+            gwas_significance (float): GWAS significance threshold. Defaults to 5e-8.
 
         Returns:
-            StudyLocus: clumped summary statistics
+            StudyLocus: clumped summary statistics (without locus collection)
         """
         # Create window for locus clusters
         # - variants where the distance between subsequent variants is below the defined threshold.
         # - Variants are sorted by descending significance
         cluster_window = Window.partitionBy(
             "studyId", "chromosome", "cluster_id"
         ).orderBy(f.col("pValueExponent").asc(), f.col("pValueMantissa").asc())
 
         return StudyLocus(
             _df=(
-                summary_stats
+                summary_statistics
                 # Dropping snps below significance - all subsequent steps are done on significant variants:
-                .pvalue_filter(p_value_significance)
+                .pvalue_filter(gwas_significance)
                 .df
                 # Clustering summary variants for efficient windowing (complexity reduction):
                 .withColumn(
                     "cluster_id",
                     WindowBasedClumping._cluster_peaks(
                         f.col("studyId"),
                         f.col("chromosome"),
                         f.col("position"),
-                        window_length,
+                        distance,
                     ),
                 )
                 # Within each cluster variants are ranked by significance:
                 .withColumn("pvRank", f.row_number().over(cluster_window))
                 # Collect positions in cluster for the most significant variant (complexity reduction):
                 .withColumn(
                     "collectedPositions",
@@ -209,15 +208,15 @@
                 .withColumn(
                     "semiIndices",
                     f.when(
                         f.size(f.col("collectedPositions")) > 0,
                         fml.vector_to_array(
                             f.udf(WindowBasedClumping._prune_peak, VectorUDT())(
                                 fml.array_to_vector(f.col("collectedPositions")),
-                                f.lit(window_length),
+                                f.lit(distance),
                             )
                         ),
                     ),
                 )
                 # Propagating the result of the above calculation for all rows:
                 .withColumn(
                     "semiIndices",
@@ -241,95 +240,7 @@
                 # Initialize QC column as array of strings:
                 .withColumn(
                     "qualityControls", f.array().cast(t.ArrayType(t.StringType()))
                 )
             ),
             _schema=StudyLocus.get_schema(),
         )
-
-    @classmethod
-    def clump_with_locus(
-        cls: type[WindowBasedClumping],
-        summary_stats: SummaryStatistics,
-        window_length: int,
-        p_value_significance: float = 5e-8,
-        p_value_baseline: float = 0.05,
-        locus_window_length: int | None = None,
-    ) -> StudyLocus:
-        """Clump significant associations while collecting locus around them.
-
-        Args:
-            summary_stats (SummaryStatistics): Input summary statistics dataset
-            window_length (int): Window size in  bp, used for distance based clumping.
-            p_value_significance (float): GWAS significance threshold used to filter peaks. Defaults to 5e-8.
-            p_value_baseline (float): Least significant threshold. Below this, all snps are dropped. Defaults to 0.05.
-            locus_window_length (int | None): The distance for collecting locus around the semi indices. Defaults to None.
-
-        Returns:
-            StudyLocus: StudyLocus after clumping with information about the `locus`
-        """
-        # If no locus window provided, using the same value:
-        if locus_window_length is None:
-            locus_window_length = window_length
-
-        # Run distance based clumping on the summary stats:
-        clumped_dataframe = WindowBasedClumping.clump(
-            summary_stats,
-            window_length=window_length,
-            p_value_significance=p_value_significance,
-        ).df.alias("clumped")
-
-        # Get list of columns from clumped dataset for further propagation:
-        clumped_columns = clumped_dataframe.columns
-
-        # Dropping variants not meeting the baseline criteria:
-        sumstats_baseline = summary_stats.pvalue_filter(p_value_baseline).df
-
-        # Renaming columns:
-        sumstats_baseline_renamed = sumstats_baseline.selectExpr(
-            *[f"{col} as tag_{col}" for col in sumstats_baseline.columns]
-        ).alias("sumstat")
-
-        study_locus_df = (
-            sumstats_baseline_renamed
-            # Joining the two datasets together:
-            .join(
-                f.broadcast(clumped_dataframe),
-                on=[
-                    (f.col("sumstat.tag_studyId") == f.col("clumped.studyId"))
-                    & (f.col("sumstat.tag_chromosome") == f.col("clumped.chromosome"))
-                    & (
-                        f.col("sumstat.tag_position")
-                        >= (f.col("clumped.position") - locus_window_length)
-                    )
-                    & (
-                        f.col("sumstat.tag_position")
-                        <= (f.col("clumped.position") + locus_window_length)
-                    )
-                ],
-                how="right",
-            )
-            .withColumn(
-                "locus",
-                f.struct(
-                    f.col("tag_variantId").alias("variantId"),
-                    f.col("tag_beta").alias("beta"),
-                    f.col("tag_pValueMantissa").alias("pValueMantissa"),
-                    f.col("tag_pValueExponent").alias("pValueExponent"),
-                    f.col("tag_standardError").alias("standardError"),
-                ),
-            )
-            .groupby("studyLocusId")
-            .agg(
-                *[
-                    f.first(col).alias(col)
-                    for col in clumped_columns
-                    if col != "studyLocusId"
-                ],
-                f.collect_list(f.col("locus")).alias("locus"),
-            )
-        )
-
-        return StudyLocus(
-            _df=study_locus_df,
-            _schema=StudyLocus.get_schema(),
-        )
```

### Comparing `gentropy-1.2.0/src/gentropy/pics.py` & `gentropy-1.3.0/src/gentropy/pics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Step to apply PICS finemapping."""
 
 from __future__ import annotations
 
 from gentropy.common.session import Session
-from gentropy.dataset.study_locus import StudyLocus
+from gentropy.dataset.study_locus import CredibleInterval, StudyLocus
 from gentropy.method.pics import PICS
 
 
 class PICSStep:
     """PICS finemapping of LD-annotated StudyLocus."""
 
     def __init__(
@@ -24,10 +24,14 @@
             picsed_study_locus_out (str): Output PICSed study-locus path.
         """
         # Extract
         study_locus_ld_annotated = StudyLocus.from_parquet(
             session, study_locus_ld_annotated_in
         )
         # PICS
-        picsed_sl = PICS.finemap(study_locus_ld_annotated).annotate_credible_sets()
+        picsed_sl = (
+            PICS.finemap(study_locus_ld_annotated)
+            .annotate_credible_sets()
+            .filter_credible_set(credible_interval=CredibleInterval.IS99)
+        )
         # Write
         picsed_sl.df.write.mode(session.write_mode).parquet(picsed_study_locus_out)
```

### Comparing `gentropy-1.2.0/src/gentropy/v2g.py` & `gentropy-1.3.0/src/gentropy/v2g.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/src/gentropy/variant_annotation.py` & `gentropy-1.3.0/src/gentropy/variant_annotation.py`

 * *Files identical despite different names*

### Comparing `gentropy-1.2.0/PKG-INFO` & `gentropy-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gentropy
-Version: 1.2.0
+Version: 1.3.0
 Summary: Open Targets python framework for post-GWAS analysis
 Home-page: https://github.com/opentargets/gentropy
 License: Apache-2.0
 Author: Open Targets core team
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gentropy Version: 1.2.0 Summary: Open Targets
+Metadata-Version: 2.1 Name: gentropy Version: 1.3.0 Summary: Open Targets
 python framework for post-GWAS analysis Home-page: https://github.com/
 opentargets/gentropy License: Apache-2.0 Author: Open Targets core team
 Requires-Python: >=3.10,<3.11 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Requires-Dist: google (>=3.0.0,<4.0.0)
 Requires-Dist: hail (==0.2.127) Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0) Requires-Dist: omegaconf
```

