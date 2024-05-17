# Comparing `tmp/wgse_ng-1.0.0a2.tar.gz` & `tmp/wgse_ng-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wgse_ng-1.0.0a2.tar", last modified: Wed May 15 18:21:18 2024, max compression
+gzip compressed data, was "wgse_ng-1.0.0a3.tar", last modified: Fri May 17 20:10:04 2024, max compression
```

## Comparing `wgse_ng-1.0.0a2.tar` & `wgse_ng-1.0.0a3.tar`

### file list

```diff
@@ -1,133 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.874089 wgse_ng-1.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-15 18:21:18.874089 wgse_ng-1.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.874089 wgse_ng-1.0.0a2/WGSE_NG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-05-15 18:21:18.000000 wgse_ng-1.0.0a2/WGSE_NG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-15 18:21:18.000000 wgse_ng-1.0.0a2/WGSE_NG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:21:18.000000 wgse_ng-1.0.0a2/WGSE_NG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-15 18:21:18.000000 wgse_ng-1.0.0a2/WGSE_NG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-15 18:21:18.000000 wgse_ng-1.0.0a2/WGSE_NG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 18:21:18.000000 wgse_ng-1.0.0a2/WGSE_NG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:21:18.874089 wgse_ng-1.0.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.838088 wgse_ng-1.0.0a2/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/test/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/test/test_fasta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/test/test_fasta_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/test/test_microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/test/test_raw_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/test/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/test/test_unknown_bases_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.838088 wgse_ng-1.0.0a2/wgse/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/VERSION.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.842088 wgse_ng-1.0.0a2/wgse/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/adapters/alignment_map_file_info_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/adapters/alignment_stats_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/adapters/header_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/adapters/index_stats_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.842088 wgse_ng-1.0.0a2/wgse/alignment_map/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/alignment_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/alignment_map/alignment_map_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/alignment_map/alignment_map_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/alignment_map/alignment_map_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/alignment_map/alignment_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/alignment_map/depth_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/alignment_map/index_stats_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.846088 wgse_ng-1.0.0a2/wgse/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/alignment_map_file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/alignment_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/build.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/chromosome_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/file_type.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/mitochondrial_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/mitochondrial_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/mitochondrial_name_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/read_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/sequence_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/data/tabular_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.846088 wgse_ng-1.0.0a2/wgse/fasta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fasta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fasta/fasta_letter_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fasta/fasta_stats_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fasta/letter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fasta/letter_run_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fasta/letter_run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fasta/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.846088 wgse_ng-1.0.0a2/wgse/fastq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fastq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/fastq/fastq_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.846088 wgse_ng-1.0.0a2/wgse/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/gui/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    11756 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/gui/microarray_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/gui/table_dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/gui/ui_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/gui/ui_form.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.854088 wgse_ng-1.0.0a2/wgse/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.866088 wgse_ng-1.0.0a2/wgse/metadata/bed_templates/
--rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/bed_templates/19_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/bed_templates/19_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/bed_templates/38_wes.csv
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/bed_templates/38_y_mt.csv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/bed_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/builds.json
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/mtdna.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/ploidy.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4875881 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/references.json
--rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/references_template.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.866088 wgse_ng-1.0.0a2/wgse/metadata/report_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/report_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/report_templates/table_macro.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/report_templates/table_simple.html
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/report_templates/table_tab.html
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/sequencers.json
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/metadata/sources.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.870088 wgse_ng-1.0.0a2/wgse/microarray/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/microarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/microarray/microarray_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/microarray/microarray_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/microarray/raw_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.870088 wgse_ng-1.0.0a2/wgse/mtDNA/
--rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/mtDNA/CRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/mtDNA/RSRS.fasta
--rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/mtDNA/Yoruba.fasta
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/mtDNA/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/mtDNA/rCRS.fasta
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.870088 wgse_ng-1.0.0a2/wgse/reference_genome/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/reference_genome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/reference_genome/bgzip_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/reference_genome/decompressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/reference_genome/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/reference_genome/genome_metadata_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/reference_genome/repository_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.870088 wgse_ng-1.0.0a2/wgse/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/renderers/csv_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/renderers/html_aligned_file_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/renderers/html_simple_table_report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:18.874089 wgse_ng-1.0.0a2/wgse/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/check_prerequisites.py
--rw-r--r--   0 runner    (1001) docker     (127)     9747 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/file_type_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/installer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/mt_dna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/sequence_orderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/sequencers.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/unit_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/utility/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-15 18:21:14.000000 wgse_ng-1.0.0a2/wgse/variant_caller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/WGSE_NG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 20:10:04.000000 wgse_ng-1.0.0a3/WGSE_NG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_fasta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_fasta_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_raw_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/test/test_unknown_bases_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/wgse/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/VERSION.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/wgse/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/alignment_map_file_info_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/alignment_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/header_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/index_stats_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/adapters/reference_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.558822 wgse_ng-1.0.0a3/wgse/alignment_map/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/alignment_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/depth_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/alignment_map/index_stats_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.562822 wgse_ng-1.0.0a3/wgse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/alignment_map_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/alignment_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/chromosome_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/file_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/mitochondrial_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/mitochondrial_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/mitochondrial_name_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/read_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/sequence_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/data/tabular_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.562822 wgse_ng-1.0.0a3/wgse/fasta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/fasta_letter_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5319 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/fasta_stats_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/letter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/letter_run_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/letter_run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fasta/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.566823 wgse_ng-1.0.0a3/wgse/fastq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fastq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/fastq/fastq_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.566823 wgse_ng-1.0.0a3/wgse/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11882 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11884 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/microarray_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/table_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/ui_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9144 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/gui/ui_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.570823 wgse_ng-1.0.0a3/wgse/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.582823 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)  4482835 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/19_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/19_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  4687904 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_wes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_y_mt.csv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/bed_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:09:59.000000 wgse_ng-1.0.0a3/wgse/metadata/builds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/mtdna.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/ploidy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4213156 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/references.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/references_template.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/metadata/report_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_macro.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_simple.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_tab.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/sequencers.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/metadata/sources.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/microarray/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/microarray_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/microarray_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/microarray/raw_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/mtDNA/
+-rw-r--r--   0 runner    (1001) docker     (127)    16961 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/CRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/RSRS.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)    16863 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/Yoruba.fasta
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/mtDNA/rCRS.fasta
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/reference_genome/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/bgzip_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/decompressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7551 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/genome_metadata_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/reference_genome/repository_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.586823 wgse_ng-1.0.0a3/wgse/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/csv_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/html_aligned_file_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/renderers/html_simple_table_report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:04.590823 wgse_ng-1.0.0a3/wgse/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/check_prerequisites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/file_type_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/installer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/mt_dna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/sequence_orderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/sequencers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/unit_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/utility/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-17 20:10:00.000000 wgse_ng-1.0.0a3/wgse/variant_caller.py
```

### Comparing `wgse_ng-1.0.0a2/PKG-INFO` & `wgse_ng-1.0.0a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Whole Genome Sequencing data manipulation tool
-Home-page: https://github.com/chaplin89/WGSE-NG
+Home-page: https://github.com/WGSE-NG/WGSE-NG
 Author: Multiple
 Author-email: 
-Keywords: bioinformatics
-Classifier: Development Status :: 1 - Planning
+Keywords: bioinformatics,genetics,wgs,microarray,science
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `wgse_ng-1.0.0a2/README.md` & `wgse_ng-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/WGSE_NG.egg-info/PKG-INFO` & `wgse_ng-1.0.0a3/WGSE_NG.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: WGSE-NG
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Whole Genome Sequencing data manipulation tool
-Home-page: https://github.com/chaplin89/WGSE-NG
+Home-page: https://github.com/WGSE-NG/WGSE-NG
 Author: Multiple
 Author-email: 
-Keywords: bioinformatics
-Classifier: Development Status :: 1 - Planning
+Keywords: bioinformatics,genetics,wgs,microarray,science
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Environment :: X11 Applications :: Qt
+Classifier: Environment :: Win32 (MS Windows)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `wgse_ng-1.0.0a2/WGSE_NG.egg-info/SOURCES.txt` & `wgse_ng-1.0.0a3/WGSE_NG.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,34 +19,35 @@
 wgse/main.py
 wgse/variant_caller.py
 wgse/adapters/__init__.py
 wgse/adapters/alignment_map_file_info_adapter.py
 wgse/adapters/alignment_stats_adapter.py
 wgse/adapters/header_adapter.py
 wgse/adapters/index_stats_adapter.py
+wgse/adapters/reference_adapter.py
 wgse/alignment_map/__init__.py
 wgse/alignment_map/alignment_map_file.py
 wgse/alignment_map/alignment_map_header.py
 wgse/alignment_map/alignment_map_row.py
 wgse/alignment_map/alignment_stats_calculator.py
 wgse/alignment_map/depth_analyzer.py
 wgse/alignment_map/index_stats_calculator.py
 wgse/data/__init__.py
 wgse/data/alignment_map_file_info.py
 wgse/data/alignment_stats.py
 wgse/data/build.py
 wgse/data/chromosome_name_type.py
 wgse/data/file_type.py
 wgse/data/gender.py
+wgse/data/genome.py
 wgse/data/microarray_converter.py
 wgse/data/mitochondrial_model.py
 wgse/data/mitochondrial_model_type.py
 wgse/data/mitochondrial_name_type.py
 wgse/data/read_type.py
-wgse/data/reference.py
 wgse/data/sequence.py
 wgse/data/sequence_type.py
 wgse/data/sorting.py
 wgse/data/source.py
 wgse/data/tabular_data.py
 wgse/fasta/__init__.py
 wgse/fasta/fasta_letter_counter.py
```

### Comparing `wgse_ng-1.0.0a2/setup.py` & `wgse_ng-1.0.0a3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,14 @@
     "pyinstaller",
     "PySide6",
     "jinja2",
     "vcf_parser",
     "WGSE-NG-3rd-party",
 ]
 
-DOC = ""
-
 setup(
     name="WGSE-NG",
     packages=find_packages(include=["wgse", "wgse.*"]),
     author="Multiple",
     author_email="",
     include_package_data=True,
     package_data={
@@ -33,26 +31,29 @@
         "wgse.metadata.bed_templates": ["*.*"],
         "wgse.metadata.report_templates": ["*.*"],
     },
     description="Whole Genome Sequencing data manipulation tool",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     install_requires=DEPENDENCIES,
-    url="https://github.com/chaplin89/WGSE-NG",
+    url="https://github.com/WGSE-NG/WGSE-NG",
     version=VERSION,
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
+        "Environment :: Console",
+        "Environment :: X11 Applications :: Qt",
+        "Environment :: Win32 (MS Windows)",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
     entry_points={
         "gui_scripts": [
             "wgse = wgse.main:main",
         ]
     },
-    keywords="bioinformatics",
+    keywords=["bioinformatics", "genetics", "wgs", "microarray", "science"],
 )
```

### Comparing `wgse_ng-1.0.0a2/test/test_buckets.py` & `wgse_ng-1.0.0a3/test/test_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/test/test_fasta.py` & `wgse_ng-1.0.0a3/test/test_fasta.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/test/test_fasta_dictionary.py` & `wgse_ng-1.0.0a3/test/test_fasta_dictionary.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/test/test_microarray_converter.py` & `wgse_ng-1.0.0a3/test/test_microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/test/test_raw_file.py` & `wgse_ng-1.0.0a3/test/test_raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/test/test_sequence.py` & `wgse_ng-1.0.0a3/test/test_sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/test/test_unknown_bases_stats.py` & `wgse_ng-1.0.0a3/test/test_unknown_bases_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/__init__.py` & `wgse_ng-1.0.0a3/wgse/__init__.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/adapters/alignment_map_file_info_adapter.py` & `wgse_ng-1.0.0a3/wgse/adapters/alignment_map_file_info_adapter.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
             "sorted": "Sorted",
             "indexed": "Indexed",
             "file_type": "File type",
             "reference_genome": "Reference genome",
             "content": "Content",
             "primary": "Primary",
             "mitochondrial_dna_type": "Mitochondrial DNA type",
-            "build": "Build",
             "name_type_chromosomes": "Name type chromosomes",
             "name_type_mtdna": "Name type mtDNA",
             "sequence_count": "Sequence count",
             "gender": "Gender",
         }
         size = stats.path.stat().st_size
         size /= 1024**3
```

### Comparing `wgse_ng-1.0.0a2/wgse/adapters/alignment_stats_adapter.py` & `wgse_ng-1.0.0a3/wgse/adapters/alignment_stats_adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import enum
 from wgse.data.alignment_stats import AlignmentStats
 from wgse.data.tabular_data import TabularData, TabularDataRow
 
 
 class AlignmentStatsAdapter:
     def adapt(input_data: AlignmentStats):
         name_map = {
@@ -20,9 +21,11 @@
             "standard_dev_quality": "Standard deviation quality",
             "read_type": "Read type",
         }
 
         rows = []
         for key, value in name_map.items():
             data = input_data.__dict__[key]
+            if isinstance(data, enum.Enum):
+                data = str(data.name)
             rows.append(TabularDataRow(value, [str(data)]))
         return TabularData(None, rows)
```

### Comparing `wgse_ng-1.0.0a2/wgse/adapters/header_adapter.py` & `wgse_ng-1.0.0a3/wgse/adapters/header_adapter.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,16 +6,44 @@
 )
 from wgse.data.tabular_data import TabularData, TabularDataRow
 
 
 class HeaderSequenceAdapter:
     def adapt(input_data: list[AlignmentMapHeaderSequence]):
         return TabularData(
-            ["Name", "Length", "MD5"],
-            [TabularDataRow(None, [x.name, str(x.length), x.md5]) for x in input_data],
+            [
+                "Name",
+                "Length",
+                "MD5",
+                "Alternate locus",
+                "Alternative names",
+                "Description",
+                "Genome",
+                "Molecule topology",
+                "Species",
+                "URI",
+            ],
+            [
+                TabularDataRow(
+                    None,
+                    [
+                        x.name,
+                        str(x.length),
+                        x.md5,
+                        x.alternate_locus,
+                        x.alternative_names,
+                        x.description,
+                        x.genome_assembly_identifier,
+                        x.molecule_topology,
+                        x.species,
+                        x.uri,
+                    ],
+                )
+                for x in input_data
+            ],
         )
 
 
 class HeaderProgramsAdapter:
     def adapt(input_data: list[AlignmentMapHeaderProgram]):
         return TabularData(
             ["ID", "Description", "Command line", "Previous", "Program version"],
```

### Comparing `wgse_ng-1.0.0a2/wgse/adapters/index_stats_adapter.py` & `wgse_ng-1.0.0a3/wgse/adapters/index_stats_adapter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/alignment_map/alignment_map_file.py` & `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,16 +172,19 @@
             indexed_stats = IndexStatsCalculator(self.path)
             file_info.index_stats = indexed_stats.get_stats()
             file_info.gender = self.get_gender(file_info.index_stats)
 
         # If file is not sorted computing AlignmentStats is expensive.
         # Let the caller request them.
         if file_info.sorted == Sorting.Coordinate:
-            calculator = AlignmentStatsCalculator(file_info)
-            file_info.alignment_stats = calculator.get_stats()
+            is_cram = file_info.file_type == FileType.CRAM 
+            has_reference = file_info.reference_genome.ready_reference is not None
+            if is_cram and has_reference or not is_cram:
+                calculator = AlignmentStatsCalculator(file_info)
+                file_info.alignment_stats = calculator.get_stats()
         return file_info
 
     def get_mitochondrial_dna_type(self, reference: Reference):
         if self.header.sequences is None:
             return MitochondrialModelType.Unknown
         sequences = {
             SequenceOrderer.canonicalize(x.name): x
```

### Comparing `wgse_ng-1.0.0a2/wgse/alignment_map/alignment_map_header.py` & `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_header.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/alignment_map/alignment_map_row.py` & `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_map_row.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/alignment_map/alignment_stats_calculator.py` & `wgse_ng-1.0.0a3/wgse/alignment_map/alignment_stats_calculator.py`

 * *Files 5% similar despite different names*

```diff
@@ -132,36 +132,38 @@
             new_delta_quality = sample.mapping_quality - average_quality
             squared_deviation_quality += delta_quality * new_delta_quality
 
         # Establish the read type based on the majority of samples
         majority = considered_samples * 0.5
         read_type = ReadType.Unknown
         if read_type_count > majority:
-            read_type = ReadType.PairedEnd
+            read_type = ReadType.Paired
         elif read_type_count < -majority:
-            read_type = ReadType.SingleEnd
+            read_type = ReadType.Single
 
         if count_length <= 2:
             raise RuntimeError(
                 "Unable to compute read length stats as the number of valid samples is less than 2."
             )
-        if count_insert_size <= 2 and read_type == ReadType.PairedEnd:
+        if count_insert_size <= 2 and read_type == ReadType.Paired:
             raise RuntimeError(
                 "Unable to compute insert size stats as the number of valid samples is less than 2."
             )
         if count_quality <= 2:
             raise RuntimeError(
                 "Unable to compute alignment quality stats as the number of valid samples is less than 2."
             )
         if read_type == ReadType.Unknown:
             raise RuntimeError(
                 "Unable to determine read type as there's a similar number of single vs paired reads."
             )
 
         stats = AlignmentStats()
+        stats.samples_count = self._config.samples
+        stats.skipped_samples = self._config.skip
         stats.read_type = read_type
         stats.duplicate = duplicate_count
         stats.sequencer = sequencer
 
         stats.count_length = count_length
         stats.count_insert_size = count_insert_size
         stats.count_quality = count_quality
```

### Comparing `wgse_ng-1.0.0a2/wgse/alignment_map/depth_analyzer.py` & `wgse_ng-1.0.0a3/wgse/alignment_map/depth_analyzer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/alignment_map/index_stats_calculator.py` & `wgse_ng-1.0.0a3/wgse/alignment_map/index_stats_calculator.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/configuration.py` & `wgse_ng-1.0.0a3/wgse/configuration.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/data/alignment_map_file_info.py` & `wgse_ng-1.0.0a3/wgse/data/alignment_map_file_info.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/data/alignment_stats.py` & `wgse_ng-1.0.0a3/wgse/data/alignment_stats.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/data/microarray_converter.py` & `wgse_ng-1.0.0a3/wgse/data/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/data/mitochondrial_model.py` & `wgse_ng-1.0.0a3/wgse/data/mitochondrial_model.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/data/reference.py` & `wgse_ng-1.0.0a3/wgse/data/genome.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/data/sequence.py` & `wgse_ng-1.0.0a3/wgse/data/sequence.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/fasta/fasta_letter_counter.py` & `wgse_ng-1.0.0a3/wgse/fasta/fasta_letter_counter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/fasta/fasta_stats_files.py` & `wgse_ng-1.0.0a3/wgse/fasta/fasta_stats_files.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/fasta/letter_run_buckets.py` & `wgse_ng-1.0.0a3/wgse/fasta/letter_run_buckets.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/fasta/letter_run_collection.py` & `wgse_ng-1.0.0a3/wgse/fasta/letter_run_collection.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/fastq/fastq_file.py` & `wgse_ng-1.0.0a3/wgse/fastq/fastq_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/gui/extract.py` & `wgse_ng-1.0.0a3/wgse/gui/extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/gui/main.py` & `wgse_ng-1.0.0a3/wgse/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from wgse.adapters.header_adapter import (
     HeaderCommentsAdapter,
     HeaderProgramsAdapter,
     HeaderReadGroupAdapter,
     HeaderSequenceAdapter,
 )
 from wgse.adapters.index_stats_adapter import IndexStatsAdapter
+from wgse.adapters.reference_adapter import ReferenceAdapter
 from wgse.alignment_map.alignment_map_file import AlignmentMapFile
 from wgse.configuration import MANAGER_CFG
 from wgse.data.gender import Gender
 from wgse.data.sorting import Sorting
 from wgse.gui.extract import ExtractDialog
 from wgse.gui.table_dialog import ListTableDialog, TableDialog
 from wgse.gui.ui_form import Ui_MainWindow
@@ -175,15 +176,15 @@
         size = f"{size:.1f} GB"
 
         rows = [
             ("Directory", str(self.current_file.path.parent)),
             ("Filename", str(self.current_file.path.name)),
             ("Size", size),
             ("File Type", info.file_type.name),
-            ("Reference", info.reference_genome.build),
+            ("Reference", f"{info.reference_genome.build} ({info.reference_genome.status.name})"),
             ("Gender", gender_string),
             ("Sorted", sorted_string),
             ("Indexed", indexed_string),
             ("Mitochondrial DNA Model", info.mitochondrial_dna_model.name),
             ("Header", click_to_open),
             ("Alignment stats", click_to_open),
             ("Index stats", click_to_open),
@@ -301,15 +302,18 @@
         )
         dialog.exec()
 
     def _show_coverage_stats(self):
         return
 
     def _show_reference(self):
-        pass
+        adapted = ReferenceAdapter.adapt(self.current_file.file_info.reference_genome)
+        dialog = TableDialog("Reference genome", self)
+        dialog.set_data(adapted)
+        dialog.exec()
 
     def _show_alignment_stats(self):
         if self.current_file is None:
             return
         dialog = TableDialog("Alignment statistics", self)
         dialog.set_data(
             AlignmentStatsAdapter.adapt(self.current_file.file_info.alignment_stats)
```

### Comparing `wgse_ng-1.0.0a2/wgse/gui/microarray_format.py` & `wgse_ng-1.0.0a3/wgse/gui/microarray_format.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/gui/table_dialog.py` & `wgse_ng-1.0.0a3/wgse/gui/table_dialog.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/gui/ui_extract.py` & `wgse_ng-1.0.0a3/wgse/gui/ui_extract.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/gui/ui_form.py` & `wgse_ng-1.0.0a3/wgse/gui/ui_form.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/main.py` & `wgse_ng-1.0.0a3/wgse/main.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/bed_templates/19_wes.csv` & `wgse_ng-1.0.0a3/wgse/metadata/bed_templates/19_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/bed_templates/38_wes.csv` & `wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_wes.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/bed_templates/38_y_mt.csv` & `wgse_ng-1.0.0a3/wgse/metadata/bed_templates/38_y_mt.csv`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/mtdna.json` & `wgse_ng-1.0.0a3/wgse/metadata/mtdna.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/references_template.json` & `wgse_ng-1.0.0a3/wgse/metadata/references_template.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/report_templates/table_macro.html` & `wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_macro.html`

 * *Files 22% similar despite different names*

```diff
@@ -6,21 +6,21 @@
                 {% for column in tabular_data.horizontal_header %}
                 <th scope="col">{{ column }}</th>
                 {% endfor %}
             </tr>
         </thead>
         {% endif %}
         <tbody>
-            {% for index in range(0, tabular_data.rows|length) %}
+            {% for row in tabular_data.rows %}
             <tr>
-                {% if tabular_data.rows[index].header %}
-                <th scope="row">{{ tabular_data.rows[index].header }}</th>
+                {% if row.vertical_header %}
+                <th scope="row">{{ row.vertical_header }}</th>
                 {% endif %}
 
-                {% for column in tabular_data.rows[index].value %}
+                {% for column in row.columns %}
                 <td>{{ column }}</td>
                 {% endfor %}
             </tr>
             {% endfor %}
         </tbody>
     </table>
 {% endmacro %}
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
 {% macro build_table(tabular_data) %}
 {{{{ ccoolluummnn }}}}
-{{{{ ttaabbuullaarr__ddaattaa..rroowwss[[iinnddeexx]]..hheeaaddeerr }}}} {{ column }}
+{{{{ rrooww..vveerrttiiccaall__hheeaaddeerr }}}} {{ column }}
 {% endmacro %}
```

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/report_templates/table_simple.html` & `wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_simple.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/report_templates/table_tab.html` & `wgse_ng-1.0.0a3/wgse/metadata/report_templates/table_tab.html`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/sequencers.json` & `wgse_ng-1.0.0a3/wgse/metadata/sequencers.json`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/metadata/sources.json` & `wgse_ng-1.0.0a3/wgse/metadata/sources.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {'insert': "[(5, OrderedDict([('name', 'NIH'), ('description', 'File distributed by the National "*

 * *           "Library of Medicine (https://ncbi.nlm.nih.gov/)'), ('urls', "*

 * *           "['https://ftp.ncbi.nlm.nih.gov/genomes'])]))]"}*

```diff
@@ -57,9 +57,16 @@
     },
     {
         "description": "File distributed by the Ensembl project (https://www.ensembl.org/info/about/index.html)",
         "name": "Ensembl",
         "urls": [
             "https://ftp.ensembl.org/pub/"
         ]
+    },
+    {
+        "description": "File distributed by the National Library of Medicine (https://ncbi.nlm.nih.gov/)",
+        "name": "NIH",
+        "urls": [
+            "https://ftp.ncbi.nlm.nih.gov/genomes"
+        ]
     }
 ]
```

### Comparing `wgse_ng-1.0.0a2/wgse/microarray/microarray_converter.py` & `wgse_ng-1.0.0a3/wgse/microarray/microarray_converter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/microarray/microarray_line_formatter.py` & `wgse_ng-1.0.0a3/wgse/microarray/microarray_line_formatter.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/microarray/raw_file.py` & `wgse_ng-1.0.0a3/wgse/microarray/raw_file.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/mtDNA/CRS.fasta` & `wgse_ng-1.0.0a3/wgse/mtDNA/CRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/mtDNA/RSRS.fasta` & `wgse_ng-1.0.0a3/wgse/mtDNA/RSRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/mtDNA/Yoruba.fasta` & `wgse_ng-1.0.0a3/wgse/mtDNA/Yoruba.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/mtDNA/rCRS.fasta` & `wgse_ng-1.0.0a3/wgse/mtDNA/rCRS.fasta`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/reference_genome/decompressor.py` & `wgse_ng-1.0.0a3/wgse/reference_genome/decompressor.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,32 +4,32 @@
 import shutil
 import typing
 import zipfile
 from pathlib import Path
 
 from wgse.utility.external import BgzipAction, External
 from wgse.reference_genome.genome_metadata_loader import Genome
-from wgse.utility.file_type_checker import FileTypeChecker, Type
+from wgse.utility.file_type_checker import FileTypeChecker, FileType
 
 
 class Decompressor:
     def __init__(
         self,
         type_checker: FileTypeChecker = FileTypeChecker(),
         external: External = External(),
     ) -> None:
         self._external = external
         self._type_checker = type_checker
 
-        self._handlers: typing.Dict[Type, typing.Callable[[Path, Path], None]] = {
-            Type.GZIP: Decompressor.razf_gzip,
-            Type.RAZF_GZIP: Decompressor.razf_gzip,
-            Type.ZIP: Decompressor.zip,
-            Type.SEVENZIP: Decompressor.sevenzip,
-            Type.BZIP: Decompressor.bzip,
+        self._handlers: typing.Dict[FileType, typing.Callable[[Path, Path], None]] = {
+            FileType.GZIP: Decompressor.razf_gzip,
+            FileType.RAZF_GZIP: Decompressor.razf_gzip,
+            FileType.ZIP: Decompressor.zip,
+            FileType.SEVENZIP: Decompressor.sevenzip,
+            FileType.BZIP: Decompressor.bzip,
         }
 
     def gz(self, input_file: Path, output_file: Path):
         # Not reliable with RAZF and currently not used.
         with gzip.open(str(input_file), "rb") as f_in:
             with open(output_file, "wb") as f_out:
                 shutil.copyfileobj(f_in, f_out)
@@ -66,33 +66,34 @@
 
     def decompression_needed(self, genome: Genome, file: Path):
         if not file.exists():
             return True
 
         type = self._type_checker.get_type(file)
         # Shortcut in case we're dealing with a BGZIP file
-        if type == Type.BGZIP:
+        if type == FileType.BGZIP:
             if genome.bgzip_size is None:
-                return True
+                genome.bgzip_size = file.stat().st_size
+                return False
             if file.stat().st_size == genome.bgzip_size:
                 return False
         # Shortcut in case we're dealing with a FASTA file
-        elif type == Type.DECOMPRESSED:
+        elif type == FileType.DECOMPRESSED:
             if genome.decompressed_size is None:
                 return True
             if file.stat().st_size == genome.decompressed_size:
                 return False
         return True
 
     def perform(self, genome: Genome, downloaded: Path = None):
-        if self.decompression_needed(genome, downloaded):
+        if not self.decompression_needed(genome, downloaded):
             return downloaded
         
         target = downloaded.with_suffix(".fa")
-        if self.decompression_needed(genome, target):
+        if not self.decompression_needed(genome, target):
             return target
 
         if not downloaded.exists():
             raise FileNotFoundError(f"Unable to find file {downloaded.name}")
 
         type = self._type_checker.get_type(downloaded)
         if type not in self._handlers:
```

### Comparing `wgse_ng-1.0.0a2/wgse/reference_genome/downloader.py` & `wgse_ng-1.0.0a3/wgse/reference_genome/downloader.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/reference_genome/genome_metadata_loader.py` & `wgse_ng-1.0.0a3/wgse/reference_genome/genome_metadata_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import typing
 
 from wgse.configuration import MANAGER_CFG
 from wgse.data.build import Build
-from wgse.data.reference import Genome
+from wgse.data.genome import Genome
 from wgse.data.sequence import Sequence
 from wgse.data.source import Source
 
 
 class GenomeMetadataLoader:
     """Manage metadata related to reference genomes.
 
@@ -54,15 +54,15 @@
         self.genome_root = self._config.genomes
         self.references_path = self._config.metadata.joinpath("references.json")
         self.sources_path = self._config.metadata.joinpath("sources.json")
         
         if not self.genome_root.is_dir():
             raise FileNotFoundError(
                 f"Unable to find {str(self.genome_root)} or is not a directory."
-            )        
+            )
         if not self.references_path.is_file():
             raise FileNotFoundError(
                 f"Unable to find {str(self.references_path)} or is not a file."
             )
         if not self.sources_path.is_file():
             raise FileNotFoundError(
                 f"Unable to find {str(self.sources_path)} or is not a file."
```

### Comparing `wgse_ng-1.0.0a2/wgse/renderers/html_aligned_file_report.py` & `wgse_ng-1.0.0a3/wgse/renderers/html_aligned_file_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/renderers/html_simple_table_report.py` & `wgse_ng-1.0.0a3/wgse/renderers/html_simple_table_report.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/utility/check_prerequisites.py` & `wgse_ng-1.0.0a3/wgse/utility/check_prerequisites.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import enum
 import inspect
+import logging
 import subprocess
+import wgse.utility.external
 from subprocess import Popen
 
 from wgse.configuration import MANAGER_CFG
 from wgse.utility.external import External
 
+logger = logging.getLogger(__name__)
 
 class PrerequisiteIssueSeverity(enum.Enum):
     INFO = enum.auto()
     WARNING = enum.auto()
     ERROR = enum.auto()
 
 
@@ -43,14 +46,16 @@
         self._ext = MANAGER_CFG.EXTERNAL
         self._gen = MANAGER_CFG.GENERAL
         self.failed = self.check_prerequisites()
 
     def check_prerequisites(self) -> list[PrerequisiteIssue]:
         # TODO: this sucks
         # TODO: empty config var should fallback on defaults with an INFO msg
+        old_level = logging.getLogger(wgse.utility.external.__name__).level
+        logging.getLogger(wgse.utility.external.__name__).setLevel(logging.INFO)
         missing = []
         if self._repo.metadata is None:
             missing.append(
                 PrerequisiteIssue(
                     PrerequisiteIssueSeverity.ERROR,
                     PrerequisiteIssueType.CONFIG_ISSUE,
                     "Metadata field is empty in repository config",
@@ -141,14 +146,15 @@
             except Exception as e:
                 m = PrerequisiteIssue(
                     PrerequisiteIssueSeverity.ERROR,
                     PrerequisiteIssueType.BINARY_ERROR,
                     f"{f.__name__} : {e!s}",
                 )
                 missing.append(m)
+        logging.getLogger(wgse.utility.external.__name__).setLevel(old_level)
         return missing
 
 
 if __name__ == "__main__":
     failing = CheckPrerequisites().check_prerequisites()
     if len(failing) == 0:
         print("All requirements are satisfied")
```

### Comparing `wgse_ng-1.0.0a2/wgse/utility/external.py` & `wgse_ng-1.0.0a3/wgse/utility/external.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import shutil
 import subprocess
 import sys
 from pathlib import Path
 
 from wgse.configuration import MANAGER_CFG
 
+logger = logging.getLogger(__name__)
+
 if "win" in sys.platform:
     third_party = str(MANAGER_CFG.EXTERNAL.root)
     if third_party not in os.environ["PATH"]:
         os.environ["PATH"] += ";" + third_party
     if ".JAR" not in os.environ["PATHEXT"]:
         os.environ["PATHEXT"] += ";.JAR"
 
@@ -37,15 +39,15 @@
         args = [*interpreter, shutil.which(f.__name__), *[str(x) for x in args]]
 
         if wait:
             # Force stdout/stderr to be PIPE as we
             # need to collect the output
             stdout = subprocess.PIPE
             stderr = subprocess.PIPE
-        logging.debug(f"Calling: {shlex.join(args)}")
+        logger.debug(f"Calling: {shlex.join(args)}")
 
         output = subprocess.Popen(args, stdout=stdout, stdin=stdin, stderr=stderr)
         if wait == True:
             out, err = output.communicate()
             if output.returncode != 0:
                 raise RuntimeError(f"Call to {f.__name__} failed: {err.decode()}")
             return out
@@ -199,16 +201,22 @@
         out = self.bgzip(
             [action_flags[action], str(input), "-@", str(self._config.threads)],
             wait=True,
         )
         if inferred_filename != output:
             inferred_filename.rename(output)
             if action == BgzipAction.Compress:
+                target = Path(str(output) + ".gzi")
                 inferred_gzi_filename = Path(str(inferred_filename) + ".gzi")
-                inferred_gzi_filename.rename(str(output) + ".gzi")
+                if target.exists():
+                    target.unlink()
+                if not inferred_gzi_filename.exists():
+                    raise FileNotFoundError(f"BGZIP index not found for {inferred_gzi_filename.name}")
+                inferred_gzi_filename.rename(target)
+        return output
 
     def idxstats(self, input: Path):
         """Generate BAM index statistics"""
         arguments = [self._samtools, "idxstat", input]
         process = subprocess.run(arguments)
         return process.stdout.decode("utf-8")
```

### Comparing `wgse_ng-1.0.0a2/wgse/utility/file_type_checker.py` & `wgse_ng-1.0.0a3/wgse/utility/file_type_checker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
 import enum
 from pathlib import Path
 
 from wgse.utility.external import External
 
 
-class Type(enum.Enum):
+class FileType(enum.Enum):
     ZIP = 0
     BZIP = 1
     SEVENZIP = 2
     # GZIP is not used ATM as it's not reliable.
     GZIP = 3
     BGZIP = 4
     RAZF_GZIP = 5
     DECOMPRESSED = 6
 
 
 class FileTypeChecker:
 
     _EXT_TO_TYPE = {
-        ".7z": Type.SEVENZIP,
-        ".zip": Type.ZIP,
-        ".bz2": Type.BZIP,
-        ".bz": Type.BZIP,
-        ".gz": Type.RAZF_GZIP,
-        ".fa": Type.DECOMPRESSED,
-        ".fasta": Type.DECOMPRESSED,
-        ".fna": Type.DECOMPRESSED
+        ".7z": FileType.SEVENZIP,
+        ".zip": FileType.ZIP,
+        ".bz2": FileType.BZIP,
+        ".bz": FileType.BZIP,
+        ".gz": FileType.RAZF_GZIP,
+        ".fa": FileType.DECOMPRESSED,
+        ".fasta": FileType.DECOMPRESSED,
+        ".fna": FileType.DECOMPRESSED
     }
     
     _TYPE_TO_EXT = {
-        Type.SEVENZIP: ".7z",
-        Type.ZIP : ".zip",
-        Type.BZIP: ".bz2",
-        Type.RAZF_GZIP:".fa.gz",
-        Type.GZIP:".fa.gz",
-        Type.DECOMPRESSED: ".fa"
+        FileType.SEVENZIP: ".7z",
+        FileType.ZIP : ".zip",
+        FileType.BZIP: ".bz2",
+        FileType.RAZF_GZIP:".fa.gz",
+        FileType.GZIP:".fa.gz",
+        FileType.DECOMPRESSED: ".fa"
     }
 
     _HTSFILE_TO_TYPE = {
-        "BGZF": Type.BGZIP,
-        "gzip": Type.RAZF_GZIP,
-        "RAZF": Type.RAZF_GZIP,
-        "FASTA": Type.DECOMPRESSED,
+        "BGZF": FileType.BGZIP,
+        "gzip": FileType.RAZF_GZIP,
+        "RAZF": FileType.RAZF_GZIP,
+        "FASTA": FileType.DECOMPRESSED,
     }
 
     def __init__(self, external: External=External()) -> None:
         self._external = external
 
-    def get_type(self, file: Path) -> Type:
+    def get_type(self, file: Path) -> FileType:
         """Get a Type starting from a file path.
 
         Args:
             file (Path): Path of the file to analyze.
 
         Returns:
             Type | None: Type or None if the type is unknown.
```

### Comparing `wgse_ng-1.0.0a2/wgse/utility/mt_dna.py` & `wgse_ng-1.0.0a3/wgse/utility/mt_dna.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/utility/regions.py` & `wgse_ng-1.0.0a3/wgse/utility/regions.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/utility/sequence_orderer.py` & `wgse_ng-1.0.0a3/wgse/utility/sequence_orderer.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/utility/sequencers.py` & `wgse_ng-1.0.0a3/wgse/utility/sequencers.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/utility/updater.py` & `wgse_ng-1.0.0a3/wgse/utility/updater.py`

 * *Files identical despite different names*

### Comparing `wgse_ng-1.0.0a2/wgse/variant_caller.py` & `wgse_ng-1.0.0a3/wgse/variant_caller.py`

 * *Files identical despite different names*

