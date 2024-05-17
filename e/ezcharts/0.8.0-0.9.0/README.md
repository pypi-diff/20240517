# Comparing `tmp/ezcharts-0.8.0.tar.gz` & `tmp/ezcharts-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcharts-0.8.0.tar", last modified: Fri Apr 12 12:15:41 2024, max compression
+gzip compressed data, was "ezcharts-0.9.0.tar", last modified: Fri May 17 12:14:07 2024, max compression
```

## Comparing `ezcharts-0.8.0.tar` & `ezcharts-0.9.0.tar`

### file list

```diff
@@ -1,289 +1,296 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-04-12 12:10:17.000000 ezcharts-0.8.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-12 12:10:17.000000 ezcharts-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8031 2024-04-12 12:15:41.480289 ezcharts-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7484 2024-04-12 12:10:17.000000 ezcharts-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.344287 ezcharts-0.8.0/ezcharts/
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.352287 ezcharts-0.8.0/ezcharts/components/
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9982 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/bcfstats.py
--rw-rw-rw-   0 root         (0) root         (0)    13432 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/clinvar.py
--rw-rw-rw-   0 root         (0) root         (0)     6395 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/common.py
--rw-rw-rw-   0 root         (0) root         (0)    14124 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/dss.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/ezchart.py
--rw-rw-rw-   0 root         (0) root         (0)    17755 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)    12869 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/modkit.py
--rw-rw-rw-   0 root         (0) root         (0)    13245 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/mosdepth.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/nextclade.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.356288 ezcharts-0.8.0/ezcharts/components/reports/
--rw-rw-rw-   0 root         (0) root         (0)     2952 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2939 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/comp.py
--rw-rw-rw-   0 root         (0) root         (0)     7435 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/labs.py
--rw-rw-rw-   0 root         (0) root         (0)     7797 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/ond.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     2327 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.356288 ezcharts-0.8.0/ezcharts/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-check-solid-sage.svg
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-check-solid-white.svg
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-exclamation-solid-red.svg
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-exclamation-solid-white.svg
--rw-rw-rw-   0 root         (0) root         (0)      402 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-minus-solid-neutral-cool.svg
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-minus-solid-white.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.360288 ezcharts-0.8.0/ezcharts/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/LAB_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/OND_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    33283 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/OND_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)    32771 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/ONT_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)   894078 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/dots.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.328287 ezcharts-0.8.0/ezcharts/data/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.360288 ezcharts-0.8.0/ezcharts/data/reference/hg19/
--rw-rw-rw-   0 root         (0) root         (0)     6297 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg19/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.364288 ezcharts-0.8.0/ezcharts/data/reference/hg38/
--rw-rw-rw-   0 root         (0) root         (0)    11449 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg38/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.364288 ezcharts-0.8.0/ezcharts/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1644 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/epi2melabs.js
--rw-rw-rw-   0 root         (0) root         (0)   394601 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey-util.js
--rw-rw-rw-   0 root         (0) root         (0)    22492 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey.js
--rw-rw-rw-   0 root         (0) root         (0)   249710 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/nextclade.html
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/ond.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.364288 ezcharts-0.8.0/ezcharts/data/styles/
--rw-rw-rw-   0 root         (0) root         (0)     6168 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/styles/epi2melabs.scss
--rw-rw-rw-   0 root         (0) root         (0)     2585 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/styles/metagenomics-sankey.css
--rw-rw-rw-   0 root         (0) root         (0)  1228637 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/styles/ond.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.380288 ezcharts-0.8.0/ezcharts/data/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/bamstats/
--rw-rw-rw-   0 root         (0) root         (0)     9394 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/bamstats/bamstats.readstats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/bamstats/empty.tsv
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/bamstats.flagstat.tsv
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/empty-no-header.tsv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/fastcat/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/empty-no-header.tsv
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/empty.tsv
--rw-rw-rw-   0 root         (0) root         (0)     5440 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/f1.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)     5426 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/f2.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    28549 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/hg38_cnv.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)     2420 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/hg38_some_bands.bed.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/empty_sample/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/empty_sample/length.hist
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/empty_sample/quality.hist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/
--rw-rw-rw-   0 root         (0) root         (0)    17008 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/length.hist
--rw-rw-rw-   0 root         (0) root         (0)     6469 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/quality.hist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.388288 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/
--rw-rw-rw-   0 root         (0) root         (0)    17008 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/length.hist
--rw-rw-rw-   0 root         (0) root         (0)     6469 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/quality.hist
--rw-rw-rw-   0 root         (0) root         (0)   427338 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/karyomap_vals.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    16943 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/nextclade.json
--rw-rw-rw-   0 root         (0) root         (0)      720 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/params.json
--rw-rw-rw-   0 root         (0) root         (0)     1649 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/plot-spec.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/real_data_test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.388288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/
--rw-rw-rw-   0 root         (0) root         (0)    27666 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/accuracy.hist
--rw-rw-rw-   0 root         (0) root         (0)     5619 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.flagstat.tsv
--rw-rw-rw-   0 root         (0) root         (0)   108079 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)     5796 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/coverage.hist
--rw-rw-rw-   0 root         (0) root         (0)     2985 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.hist
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.unmap.hist
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.hist
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.unmap.hist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.392288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/
--rw-rw-rw-   0 root         (0) root         (0)    15462 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/accuracy.hist
--rw-rw-rw-   0 root         (0) root         (0)     5591 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.flagstat.tsv
--rw-rw-rw-   0 root         (0) root         (0)    54744 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.readstats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)     4097 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/coverage.hist
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.hist
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.unmap.hist
--rw-rw-rw-   0 root         (0) root         (0)     4479 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.hist
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.unmap.hist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.396288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/
--rw-rw-rw-   0 root         (0) root         (0)     2985 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/length.hist
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/n_seqs
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-file-stats.tsv
--rw-rw-rw-   0 root         (0) root         (0)    67785 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-read-stats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/quality.hist
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/run_ids
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.396288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/
--rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/length.hist
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/n_seqs
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-file-stats.tsv
--rw-rw-rw-   0 root         (0) root         (0)    33847 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-read-stats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)     4479 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/quality.hist
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/run_ids
--rwxrwxrwx   0 root         (0) root         (0)      790 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/ref.fa.fai
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/sankey.json
--rw-rw-rw-   0 root         (0) root         (0)  1125122 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_dml.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    35285 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_dmr.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)  1458860 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_modkit.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_modkit_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)     7150 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_mosdepth.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_mosdepth_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/versions.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.396288 ezcharts-0.8.0/ezcharts/data/themes/
--rw-rw-rw-   0 root         (0) root         (0)     5624 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/themes/epi2melabs.json
--rw-rw-rw-   0 root         (0) root         (0)     5764 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/themes/ond.json
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/themes/walden.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.400288 ezcharts-0.8.0/ezcharts/data/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.336287 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.400288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/js/
--rw-rw-rw-   0 root         (0) root         (0)    80599 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.416288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/
--rw-rw-rw-   0 root         (0) root         (0)     5066 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
--rw-rw-rw-   0 root         (0) root         (0)     2055 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
--rw-rw-rw-   0 root         (0) root         (0)     1751 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
--rw-rw-rw-   0 root         (0) root         (0)     3195 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     6685 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     6941 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
--rw-rw-rw-   0 root         (0) root         (0)     5751 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1948 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
--rw-rw-rw-   0 root         (0) root         (0)     8093 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)    10554 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
--rw-rw-rw-   0 root         (0) root         (0)     6775 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     4043 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
--rw-rw-rw-   0 root         (0) root         (0)     4665 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
--rw-rw-rw-   0 root         (0) root         (0)     4725 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
--rw-rw-rw-   0 root         (0) root         (0)     3944 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      859 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
--rw-rw-rw-   0 root         (0) root         (0)     6907 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
--rw-rw-rw-   0 root         (0) root         (0)     2016 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
--rw-rw-rw-   0 root         (0) root         (0)    12404 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)     7371 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
--rw-rw-rw-   0 root         (0) root         (0)     4413 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
--rw-rw-rw-   0 root         (0) root         (0)     2490 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
--rw-rw-rw-   0 root         (0) root         (0)     3939 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
--rw-rw-rw-   0 root         (0) root         (0)    17886 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     3840 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
--rw-rw-rw-   0 root         (0) root         (0)    73610 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.420288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
--rw-rw-rw-   0 root         (0) root         (0)     2480 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
--rw-rw-rw-   0 root         (0) root         (0)     4833 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
--rw-rw-rw-   0 root         (0) root         (0)     5868 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
--rw-rw-rw-   0 root         (0) root         (0)     2796 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
--rw-rw-rw-   0 root         (0) root         (0)     2603 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
--rw-rw-rw-   0 root         (0) root         (0)     3896 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     1142 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.424288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
--rw-rw-rw-   0 root         (0) root         (0)      245 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      525 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0 root         (0) root         (0)     4580 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     1587 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
--rw-rw-rw-   0 root         (0) root         (0)     4164 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     1956 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
--rw-rw-rw-   0 root         (0) root         (0)     4726 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      395 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
--rw-rw-rw-   0 root         (0) root         (0)      582 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
--rw-rw-rw-   0 root         (0) root         (0)     1101 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
--rw-rw-rw-   0 root         (0) root         (0)     3380 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
--rw-rw-rw-   0 root         (0) root         (0)    10029 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
--rw-rw-rw-   0 root         (0) root         (0)  1017477 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/echarts.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css
--rw-rw-rw-   0 root         (0) root         (0)    38224 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js
--rw-rw-rw-   0 root         (0) root         (0)    16697 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/demo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/layout/
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.440289 ezcharts-0.8.0/ezcharts/layout/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2880 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/banner.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/cards.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/document.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2407 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/offcanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2758 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/section.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/stats.py
--rw-rw-rw-   0 root         (0) root         (0)     7694 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/table.py
--rw-rw-rw-   0 root         (0) root         (0)     5636 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     2893 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.476289 ezcharts-0.8.0/ezcharts/plots/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/_base.py
--rw-rw-rw-   0 root         (0) root         (0) 13970130 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/_model.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/axisgrid.py
--rw-rw-rw-   0 root         (0) root         (0)    11366 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/categorical.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/demo.py
--rw-rw-rw-   0 root         (0) root         (0)     5065 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)    12803 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/ideogram.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/karyomap.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/matrix.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/metagenomics_sankey.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     6619 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/relational.py
--rwxrwxrwx   0 root         (0) root         (0)     3463 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/sunburst.py
--rw-rw-rw-   0 root         (0) root         (0)     9950 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/ezcharts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8031 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11845 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 12:13:51.000000 ezcharts-0.8.0/ezcharts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      115 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-04-12 12:10:17.000000 ezcharts-0.8.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 12:15:41.480289 ezcharts-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2187 2024-04-12 12:10:17.000000 ezcharts-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/tests/components/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11053 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/components/test_fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/test_demo.py
--rw-rw-rw-   0 root         (0) root         (0)     1952 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.387613 ezcharts-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-05-17 11:16:13.000000 ezcharts-0.9.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-05-17 11:16:13.000000 ezcharts-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8031 2024-05-17 12:14:07.387613 ezcharts-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7484 2024-05-17 11:16:13.000000 ezcharts-0.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.295605 ezcharts-0.9.0/ezcharts/
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.299605 ezcharts-0.9.0/ezcharts/components/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10492 2024-05-17 12:08:51.000000 ezcharts-0.9.0/ezcharts/components/bcfstats.py
+-rw-rw-rw-   0 root         (0) root         (0)    13432 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/clinvar.py
+-rw-rw-rw-   0 root         (0) root         (0)     6395 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    14124 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/dss.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/ezchart.py
+-rw-rw-rw-   0 root         (0) root         (0)    32040 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)    12869 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/modkit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13245 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/mosdepth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/nextclade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.299605 ezcharts-0.9.0/ezcharts/components/reports/
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/reports/comp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7435 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/reports/labs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7797 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/reports/ond.py
+-rw-rw-rw-   0 root         (0) root         (0)     7797 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/reports/ont.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     2327 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/components/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.287604 ezcharts-0.9.0/ezcharts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.303606 ezcharts-0.9.0/ezcharts/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/icons/circle-check-solid-sage.svg
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/icons/circle-check-solid-white.svg
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/icons/circle-exclamation-solid-red.svg
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/icons/circle-exclamation-solid-white.svg
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/icons/circle-minus-solid-neutral-cool.svg
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/icons/circle-minus-solid-white.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.303606 ezcharts-0.9.0/ezcharts/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/images/LAB_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/images/OND_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33283 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/images/OND_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    32771 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/images/ONT_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)   894078 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/images/dots.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.287604 ezcharts-0.9.0/ezcharts/data/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.307606 ezcharts-0.9.0/ezcharts/data/reference/hg19/
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/reference/hg19/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.307606 ezcharts-0.9.0/ezcharts/data/reference/hg38/
+-rw-rw-rw-   0 root         (0) root         (0)    11449 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/reference/hg38/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.307606 ezcharts-0.9.0/ezcharts/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/scripts/epi2melabs.js
+-rw-rw-rw-   0 root         (0) root         (0)   394601 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/scripts/metagenomics-sankey-util.js
+-rw-rw-rw-   0 root         (0) root         (0)    22492 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/scripts/metagenomics-sankey.js
+-rw-rw-rw-   0 root         (0) root         (0)   249710 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/scripts/nextclade.html
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/scripts/ond.js
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/scripts/ont.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.311606 ezcharts-0.9.0/ezcharts/data/styles/
+-rw-rw-rw-   0 root         (0) root         (0)     6168 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/styles/epi2melabs.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/styles/metagenomics-sankey.css
+-rw-rw-rw-   0 root         (0) root         (0)  1228637 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/styles/ond.scss
+-rw-rw-rw-   0 root         (0) root         (0)  1228639 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/styles/ont.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.319607 ezcharts-0.9.0/ezcharts/data/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.323607 ezcharts-0.9.0/ezcharts/data/test/bamstats/
+-rw-rw-rw-   0 root         (0) root         (0)     9394 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/bamstats/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/bamstats/empty.tsv
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/bamstats.flagstat.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.323607 ezcharts-0.9.0/ezcharts/data/test/bcftools/
+-rw-rw-rw-   0 root         (0) root         (0)     8485 2024-05-17 12:08:51.000000 ezcharts-0.9.0/ezcharts/data/test/bcftools/cw-3767-variants.stats
+-rw-rw-rw-   0 root         (0) root         (0)     8876 2024-05-17 12:08:51.000000 ezcharts-0.9.0/ezcharts/data/test/bcftools/variants.stats
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/empty-no-header.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.323607 ezcharts-0.9.0/ezcharts/data/test/fastcat/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/fastcat/empty-no-header.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/fastcat/empty.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     5440 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/fastcat/f1.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     5426 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/fastcat/f2.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    28549 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/hg38_cnv.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/hg38_some_bands.bed.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.287604 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.323607 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/empty_sample/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/empty_sample/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/empty_sample/quality.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.323607 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_1/
+-rw-rw-rw-   0 root         (0) root         (0)    17008 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_1/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)     6469 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_1/quality.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.323607 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_2/
+-rw-rw-rw-   0 root         (0) root         (0)    17008 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_2/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)     6469 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_2/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)   427338 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/karyomap_vals.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    16943 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/nextclade.json
+-rw-rw-rw-   0 root         (0) root         (0)      720 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/plot-spec.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.287604 ezcharts-0.9.0/ezcharts/data/test/real_data_test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.287604 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.327608 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/
+-rw-rw-rw-   0 root         (0) root         (0)    27666 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/accuracy.hist
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)   108079 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     5796 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/coverage.hist
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.unmap.hist
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.unmap.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.331608 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/
+-rw-rw-rw-   0 root         (0) root         (0)    15462 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/accuracy.hist
+-rw-rw-rw-   0 root         (0) root         (0)     5591 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    54744 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/coverage.hist
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.unmap.hist
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-17 12:09:01.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.unmap.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.287604 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.331608 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/n_seqs
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-file-stats.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    67785 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-read-stats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/run_ids
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.331608 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/n_seqs
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-file-stats.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    33847 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-read-stats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/run_ids
+-rwxrwxrwx   0 root         (0) root         (0)      790 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/ref.fa.fai
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/sankey.json
+-rw-rw-rw-   0 root         (0) root         (0)  1125122 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/test_dml.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    35285 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/test_dmr.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)  1458860 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/test_modkit.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/test_modkit_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     7150 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/test_mosdepth.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/test_mosdepth_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/test/versions.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.335608 ezcharts-0.9.0/ezcharts/data/themes/
+-rw-rw-rw-   0 root         (0) root         (0)     5624 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/themes/epi2melabs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/themes/ond.json
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/themes/walden.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.335608 ezcharts-0.9.0/ezcharts/data/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.287604 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.335608 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/js/
+-rw-rw-rw-   0 root         (0) root         (0)    80599 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.347609 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3195 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     8093 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
+-rw-rw-rw-   0 root         (0) root         (0)    17886 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
+-rw-rw-rw-   0 root         (0) root         (0)    73610 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.347609 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.351610 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
+-rw-rw-rw-   0 root         (0) root         (0)      245 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.359610 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
+-rw-rw-rw-   0 root         (0) root         (0)      582 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3380 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.359610 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.359610 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
+-rw-rw-rw-   0 root         (0) root         (0)  1017477 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/echarts.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.359610 ezcharts-0.9.0/ezcharts/data/vendor/simple-datatables/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css
+-rw-rw-rw-   0 root         (0) root         (0)    38224 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js
+-rw-rw-rw-   0 root         (0) root         (0)    16697 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/demo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.359610 ezcharts-0.9.0/ezcharts/layout/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.363611 ezcharts-0.9.0/ezcharts/layout/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/banner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/offcanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     7694 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5636 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/snippets/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/layout/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.387613 ezcharts-0.9.0/ezcharts/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/_base.py
+-rw-rw-rw-   0 root         (0) root         (0) 13970130 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/axisgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    11366 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/categorical.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     5065 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12803 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/ideogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/karyomap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/metagenomics_sankey.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/relational.py
+-rwxrwxrwx   0 root         (0) root         (0)     3463 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/sunburst.py
+-rw-rw-rw-   0 root         (0) root         (0)     9853 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/plots/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-05-17 11:16:13.000000 ezcharts-0.9.0/ezcharts/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.387613 ezcharts-0.9.0/ezcharts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8031 2024-05-17 12:14:07.000000 ezcharts-0.9.0/ezcharts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12067 2024-05-17 12:14:07.000000 ezcharts-0.9.0/ezcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 12:14:07.000000 ezcharts-0.9.0/ezcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-17 12:14:07.000000 ezcharts-0.9.0/ezcharts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 12:12:27.000000 ezcharts-0.9.0/ezcharts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      115 2024-05-17 12:14:07.000000 ezcharts-0.9.0/ezcharts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-17 12:14:07.000000 ezcharts-0.9.0/ezcharts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-05-17 11:16:13.000000 ezcharts-0.9.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-17 12:14:07.387613 ezcharts-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-05-17 11:16:13.000000 ezcharts-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.387613 ezcharts-0.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-05-17 11:16:13.000000 ezcharts-0.9.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 12:14:07.387613 ezcharts-0.9.0/tests/components/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-17 11:16:13.000000 ezcharts-0.9.0/tests/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2024-05-17 12:08:51.000000 ezcharts-0.9.0/tests/components/test_bcftools.py
+-rw-rw-rw-   0 root         (0) root         (0)    12320 2024-05-17 11:16:13.000000 ezcharts-0.9.0/tests/components/test_fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-05-17 11:16:13.000000 ezcharts-0.9.0/tests/test_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2024-05-17 11:16:13.000000 ezcharts-0.9.0/tests/test_utils.py
```

### Comparing `ezcharts-0.8.0/LICENSE` & `ezcharts-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/PKG-INFO` & `ezcharts-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.8.0
+Version: 0.9.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bokeh~=3.1.0
```

### Comparing `ezcharts-0.8.0/README.md` & `ezcharts-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/__init__.py` & `ezcharts-0.9.0/ezcharts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Simple eCharts API."""
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 import argparse
 import importlib
 import logging
 
 from ezcharts import util
 from ezcharts.plots.axisgrid import *  # noqa: F401,F403
```

### Comparing `ezcharts-0.8.0/ezcharts/components/bcfstats.py` & `ezcharts-0.9.0/ezcharts/components/bcfstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,23 +149,31 @@
 
 
 def split_blocks(fname):
     """Split lines of a file into blocks based on comment lines."""
     comment = list()
     data = list()
     state = None
+    two_line_comments = ('IDD', 'TSTV', 'SiS', 'AF', 'QUAL', 'ST')
     with open(fname, 'r') as fh:
-        # TODO: handle empty tables
-        for line in fh.readlines():
+        lines = fh.readlines()
+        for line_num, line in enumerate(lines):
             if line.startswith('#'):
                 if state != 'comment' and state is not None:
                     yield comment, data
                     comment, data = list(), list()
                 state = 'comment'
                 comment.append(line.strip('# ').rstrip())
+                # if there are two comments appended and it's a special comment
+                # check the next line, if it's another comment, yield the comment
+                # and empty data
+                if len(comment) == 2 and comment[-1].startswith(two_line_comments):
+                    if lines[line_num + 1].startswith('#'):
+                        yield comment, []
+                        comment, data = list(), list()
             else:
                 state = 'data'
                 data.append(line.rstrip())
         yield comment, data
 
 
 def parse_bcftools_stats(fname, sample_name=None):
```

### Comparing `ezcharts-0.8.0/ezcharts/components/clinvar.py` & `ezcharts-0.9.0/ezcharts/components/clinvar.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/common.py` & `ezcharts-0.9.0/ezcharts/components/common.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/dss.py` & `ezcharts-0.9.0/ezcharts/components/dss.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/ezchart.py` & `ezcharts-0.9.0/ezcharts/components/ezchart.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/modkit.py` & `ezcharts-0.9.0/ezcharts/components/modkit.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/mosdepth.py` & `ezcharts-0.9.0/ezcharts/components/mosdepth.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/nextclade.py` & `ezcharts-0.9.0/ezcharts/components/nextclade.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/params.py` & `ezcharts-0.9.0/ezcharts/components/params.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/reports/__init__.py` & `ezcharts-0.9.0/ezcharts/components/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/reports/comp.py` & `ezcharts-0.9.0/ezcharts/components/reports/comp.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/reports/labs.py` & `ezcharts-0.9.0/ezcharts/components/reports/labs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/reports/ond.py` & `ezcharts-0.9.0/ezcharts/components/reports/ond.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/components/theme.py` & `ezcharts-0.9.0/ezcharts/components/theme.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Re-usable external resources."""
-from dominate.tags import div, img, script, style
+from dominate.tags import div, script, style
 
 from ezcharts.components.ezchart import EZChartTheme
 from ezcharts.layout.resource import (
     base_body_resources, base_head_resources,
     ImageResource, ScriptResource, StyleResource, ThemeResource)
 from ezcharts.layout.util import inline, load_json, transpile
 
@@ -71,33 +71,33 @@
     tag=EZChartTheme,
     loader=load_json)
 
 OND_head_resources = [OND_CSS, *base_head_resources, OND_CHART_THEME]
 OND_body_resources = [OND_JS, *base_body_resources]
 
 
-class ONTLogo(img):
+class ONTLogo(div):
     """ONT logo element."""
 
     def __init__(self) -> None:
         """Create an img with the data URI logo."""
         super().__init__(
-            inline(ImageResource('ONT_logo.txt').data_file),
-            tagname='img',
-            style="height: 35px;",
+            inline(ImageResource('OND_logo.svg').data_file),
+            tagname='div',
+            style="width: 35px; height: 35px;",
             className="d-flex",
             alt="ONT Logo")
 
 
 # TODO: Create
 ONT_CSS = StyleResource(
-    path='epi2melabs.scss',
+    path='ont.scss',
     tag=style,
     loader=transpile)
 
 ONT_JS = ScriptResource(
-    path='epi2melabs.js',
+    path='ont.js',
     tag=script,
     loader=inline)
 
 ONT_head_resources = [ONT_CSS, *base_head_resources]
 ONT_body_resources = [ONT_JS, *base_body_resources]
```

### Comparing `ezcharts-0.8.0/ezcharts/components/versions.py` & `ezcharts-0.9.0/ezcharts/components/versions.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/images/LAB_logo.svg` & `ezcharts-0.9.0/ezcharts/data/images/LAB_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/images/OND_logo.svg` & `ezcharts-0.9.0/ezcharts/data/images/OND_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/images/OND_logo.txt` & `ezcharts-0.9.0/ezcharts/data/images/OND_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/images/ONT_logo.txt` & `ezcharts-0.9.0/ezcharts/data/images/ONT_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/images/dots.svg` & `ezcharts-0.9.0/ezcharts/data/images/dots.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/reference/hg19/cytoBand.txt.gz` & `ezcharts-0.9.0/ezcharts/data/reference/hg19/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/reference/hg38/cytoBand.txt.gz` & `ezcharts-0.9.0/ezcharts/data/reference/hg38/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/scripts/epi2melabs.js` & `ezcharts-0.9.0/ezcharts/data/scripts/epi2melabs.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey-util.js` & `ezcharts-0.9.0/ezcharts/data/scripts/metagenomics-sankey-util.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey.js` & `ezcharts-0.9.0/ezcharts/data/scripts/metagenomics-sankey.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/scripts/nextclade.html` & `ezcharts-0.9.0/ezcharts/data/scripts/nextclade.html`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/scripts/ond.js` & `ezcharts-0.9.0/ezcharts/data/scripts/ond.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/styles/epi2melabs.scss` & `ezcharts-0.9.0/ezcharts/data/styles/epi2melabs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/styles/metagenomics-sankey.css` & `ezcharts-0.9.0/ezcharts/data/styles/metagenomics-sankey.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/styles/ond.scss` & `ezcharts-0.9.0/ezcharts/data/styles/ond.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/bamstats/bamstats.readstats.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/bamstats/bamstats.readstats.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/fastcat/f1.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/fastcat/f1.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/fastcat/f2.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/fastcat/f2.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/hg38_cnv.bed.gz` & `ezcharts-0.9.0/ezcharts/data/test/hg38_cnv.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/hg38_some_bands.bed.gz` & `ezcharts-0.9.0/ezcharts/data/test/hg38_some_bands.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/length.hist` & `ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_1/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/quality.hist` & `ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_1/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/length.hist` & `ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_2/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/quality.hist` & `ezcharts-0.9.0/ezcharts/data/test/histogram_stats/sample_2/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/karyomap_vals.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/karyomap_vals.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/nextclade.json` & `ezcharts-0.9.0/ezcharts/data/test/nextclade.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/params.json` & `ezcharts-0.9.0/ezcharts/data/test/params.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/plot-spec.json` & `ezcharts-0.9.0/ezcharts/data/test/plot-spec.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/accuracy.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/accuracy.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.flagstat.tsv` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.flagstat.tsv`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/coverage.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/coverage.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/accuracy.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/accuracy.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.flagstat.tsv` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.flagstat.tsv`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.readstats.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.readstats.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/coverage.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/coverage.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/length.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-read-stats.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-read-stats.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/quality.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode01/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/length.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-read-stats.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-read-stats.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/quality.hist` & `ezcharts-0.9.0/ezcharts/data/test/real_data_test/fastcat/barcode02/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/ref.fa.fai` & `ezcharts-0.9.0/ezcharts/data/test/ref.fa.fai`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/sankey.json` & `ezcharts-0.9.0/ezcharts/data/test/sankey.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/test_dml.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/test_dml.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/test_dmr.tsv.gz` & `ezcharts-0.9.0/ezcharts/data/test/test_dmr.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/test_modkit.bed.gz` & `ezcharts-0.9.0/ezcharts/data/test/test_modkit.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/test/test_mosdepth.bed.gz` & `ezcharts-0.9.0/ezcharts/data/test/test_mosdepth.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/themes/epi2melabs.json` & `ezcharts-0.9.0/ezcharts/data/themes/epi2melabs.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/themes/ond.json` & `ezcharts-0.9.0/ezcharts/data/themes/ond.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/themes/walden.json` & `ezcharts-0.9.0/ezcharts/data/themes/walden.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss` & `ezcharts-0.9.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/echarts.min.js` & `ezcharts-0.9.0/ezcharts/data/vendor/echarts.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css` & `ezcharts-0.9.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js` & `ezcharts-0.9.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/demo.py` & `ezcharts-0.9.0/ezcharts/demo.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/base.py` & `ezcharts-0.9.0/ezcharts/layout/base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/resource.py` & `ezcharts-0.9.0/ezcharts/layout/resource.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/__init__.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/banner.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/banner.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/cards.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/cards.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/document.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/document.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/grid.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/grid.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/offcanvas.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/offcanvas.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/progress.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/progress.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/section.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/section.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/stats.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/stats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/table.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/table.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/snippets/tabs.py` & `ezcharts-0.9.0/ezcharts/layout/snippets/tabs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/layout/util.py` & `ezcharts-0.9.0/ezcharts/layout/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/__init__.py` & `ezcharts-0.9.0/ezcharts/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/_base.py` & `ezcharts-0.9.0/ezcharts/plots/_base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/_model.py` & `ezcharts-0.9.0/ezcharts/plots/_model.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/categorical.py` & `ezcharts-0.9.0/ezcharts/plots/categorical.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/demo.py` & `ezcharts-0.9.0/ezcharts/plots/demo.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/distribution.py` & `ezcharts-0.9.0/ezcharts/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/ideogram.py` & `ezcharts-0.9.0/ezcharts/plots/ideogram.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/karyomap.py` & `ezcharts-0.9.0/ezcharts/plots/karyomap.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/matrix.py` & `ezcharts-0.9.0/ezcharts/plots/matrix.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/metagenomics_sankey.py` & `ezcharts-0.9.0/ezcharts/plots/metagenomics_sankey.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/relational.py` & `ezcharts-0.9.0/ezcharts/plots/relational.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/sunburst.py` & `ezcharts-0.9.0/ezcharts/plots/sunburst.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts/plots/util.py` & `ezcharts-0.9.0/ezcharts/plots/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,24 +261,24 @@
 
 
 def empty_plot(**kwargs):
     """Empty plot for when all else fails.
 
     :param kwargs: kwargs for bokeh figure.
 
-    :returns: a eChart empty plot.
+    :returns: an eChart empty plot.
 
     """
     plt = plots._NoAxisFixPlot()
     plt.title = {
         "text": "Plotting Failed",
         "subtext": "Oops! Something went wrong in plotting your data.",
         "subtextStyle": {
             "fontStyle": "italic",
-            "color": "#0084A9",
+            "color": Colors.cerulean,
         },
         "itemGap": 30,
     }
     return plt
 
 
 def plot_wrapper(func):
@@ -294,20 +294,17 @@
     def wrapper_accepting_arguments(*args, **kwargs):
         """Argument wrapper for decorator."""
         logger = util.get_named_logger("PlotWrap")
         try:
             p = func(*args, **kwargs)
             return p
         except Exception as e:
-            # check is debug mode is enabled:
-            if (
-                "EZCHARTS_DEBUG" in os.environ
-                and os.environ.get("EZCHARTS_DEBUG") == "1"
-            ):
-                return func(*args, **kwargs)
+            # check if debug mode is enabled:
+            if os.environ.get("EZCHARTS_DEBUG") == "1":
+                raise e
             else:
                 # plot empty
                 try:
                     p = empty_plot(**kwargs)
                     logger.exception("Plotting user plot failed with: " + str(e))
                     return p
                 # if empty plot fails
```

### Comparing `ezcharts-0.8.0/ezcharts/util.py` & `ezcharts-0.9.0/ezcharts/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/ezcharts.egg-info/PKG-INFO` & `ezcharts-0.9.0/ezcharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.8.0
+Version: 0.9.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bokeh~=3.1.0
```

### Comparing `ezcharts-0.8.0/ezcharts.egg-info/SOURCES.txt` & `ezcharts-0.9.0/ezcharts.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ezcharts/components/params.py
 ezcharts/components/theme.py
 ezcharts/components/versions.py
 ezcharts/components/reports/__init__.py
 ezcharts/components/reports/comp.py
 ezcharts/components/reports/labs.py
 ezcharts/components/reports/ond.py
+ezcharts/components/reports/ont.py
 ezcharts/data/icons/circle-check-solid-sage.svg
 ezcharts/data/icons/circle-check-solid-white.svg
 ezcharts/data/icons/circle-exclamation-solid-red.svg
 ezcharts/data/icons/circle-exclamation-solid-white.svg
 ezcharts/data/icons/circle-minus-solid-neutral-cool.svg
 ezcharts/data/icons/circle-minus-solid-white.svg
 ezcharts/data/images/LAB_logo.svg
@@ -46,17 +47,19 @@
 ezcharts/data/reference/hg38/cytoBand.txt.gz
 ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
 ezcharts/data/scripts/epi2melabs.js
 ezcharts/data/scripts/metagenomics-sankey-util.js
 ezcharts/data/scripts/metagenomics-sankey.js
 ezcharts/data/scripts/nextclade.html
 ezcharts/data/scripts/ond.js
+ezcharts/data/scripts/ont.js
 ezcharts/data/styles/epi2melabs.scss
 ezcharts/data/styles/metagenomics-sankey.css
 ezcharts/data/styles/ond.scss
+ezcharts/data/styles/ont.scss
 ezcharts/data/test/bamstats.flagstat.tsv
 ezcharts/data/test/empty-no-header.tsv
 ezcharts/data/test/hg38_cnv.bed.gz
 ezcharts/data/test/hg38_some_bands.bed.gz
 ezcharts/data/test/karyomap_vals.tsv.gz
 ezcharts/data/test/nextclade.json
 ezcharts/data/test/params.json
@@ -68,14 +71,16 @@
 ezcharts/data/test/test_modkit.bed.gz
 ezcharts/data/test/test_modkit_summary.tsv
 ezcharts/data/test/test_mosdepth.bed.gz
 ezcharts/data/test/test_mosdepth_summary.tsv
 ezcharts/data/test/versions.txt
 ezcharts/data/test/bamstats/bamstats.readstats.tsv.gz
 ezcharts/data/test/bamstats/empty.tsv
+ezcharts/data/test/bcftools/cw-3767-variants.stats
+ezcharts/data/test/bcftools/variants.stats
 ezcharts/data/test/fastcat/empty-no-header.tsv
 ezcharts/data/test/fastcat/empty.tsv
 ezcharts/data/test/fastcat/f1.tsv.gz
 ezcharts/data/test/fastcat/f2.tsv.gz
 ezcharts/data/test/histogram_stats/empty_sample/length.hist
 ezcharts/data/test/histogram_stats/empty_sample/quality.hist
 ezcharts/data/test/histogram_stats/sample_1/length.hist
@@ -237,8 +242,9 @@
 ezcharts/plots/relational.py
 ezcharts/plots/sunburst.py
 ezcharts/plots/util.py
 tests/__init__.py
 tests/test_demo.py
 tests/test_utils.py
 tests/components/__init__.py
+tests/components/test_bcftools.py
 tests/components/test_fastcat.py
```

### Comparing `ezcharts-0.8.0/setup.py` & `ezcharts-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.8.0/tests/components/test_fastcat.py` & `ezcharts-0.9.0/tests/components/test_fastcat.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,41 +156,44 @@
     per_read_stats_fastcat = resource_filename(
         "ezcharts", "data/test/real_data_test/fastcat/barcode01/per-read-stats.tsv.gz"
     )
     per_read_stats_bamstats = resource_filename(
         "ezcharts",
         "data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz",
     )
-    target_cols = ["sample_name", "read_length", "mean_quality"]
+    target_cols_fastcat = ["sample_name", "read_length", "mean_quality"]
+    target_cols_bamstats = [
+        "sample_name", "coverage", "read_length", "mean_quality", "acc"]
     to_test = (
-        (per_read_stats_fastcat, fastcat.FASTCAT_COLS_DTYPES),
-        (per_read_stats_bamstats, fastcat.BAMSTATS_COLS_DTYPES),
+        (per_read_stats_fastcat, fastcat.FASTCAT_COLS_DTYPES, target_cols_fastcat),
+        (per_read_stats_bamstats, fastcat.BAMSTATS_COLS_DTYPES, target_cols_bamstats),
     )
-    for fname, TYPE in to_test:
+    for fname, TYPE, target_cols in to_test:
         actual = fastcat.load_stats(fname)
         expected = _read_pandas(fname, TYPE, target_cols=target_cols)
         _compare_frames(actual, expected)
 
 
 def test_025_equality_of_result():
     """Return a consistent data structure."""
     per_read_stats_fastcat = resource_filename(
         "ezcharts", "data/test/real_data_test/fastcat/barcode01/per-read-stats.tsv.gz"
     )
     per_read_stats_bamstats = resource_filename(
         "ezcharts",
         "data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz",
     )
+    target_cols = ["sample_name", "read_length", "mean_quality"]
     actual_fastcat = (
-        fastcat.load_stats(per_read_stats_fastcat)
+        fastcat.load_stats(per_read_stats_fastcat, target_cols=target_cols)
         .sort_values(["read_length", "mean_quality"])
         .reset_index(drop=True)
     )
     actual_bamstats = (
-        fastcat.load_stats(per_read_stats_bamstats)
+        fastcat.load_stats(per_read_stats_bamstats, target_cols=target_cols)
         .sort_values(["read_length", "mean_quality"])
         .reset_index(drop=True)
     )
     _compare_frames(actual_fastcat, actual_bamstats)
 
 
 def test_031_read_flagstat():
@@ -310,20 +313,52 @@
     else:
         fastcat.SeqSummary(
             seq_summary=tuple([resource_filename("ezcharts", i) for i in input]),
             sample_names=tuple(["S" + i for i in input]),
         )
 
 
-def test_105_SeqSummary_empty_file():
+def test_105_bamstats_inputs():
+    """Test if SeqSummary works with bam_flagstat inputs."""
+    # Create a couple of samples
+    seq_summary = resource_filename(
+        "ezcharts",
+        "data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz"
+    )
+    flagstats = resource_filename(
+        "ezcharts",
+        "data/test/real_data_test/bamstats/barcode01/bamstats.flagstat.tsv"
+    )
+    # pass just first sample
+    fastcat.SeqSummary(
+        seq_summary=seq_summary,
+        sample_names="barcode01",
+        flagstat=flagstats)
+
+
+def test_106_multi_sample_by_metric():
+    """Test if SeqCompare works."""
+    # Create a couple of samples
+    samples, files = _multisamples()
+    with pytest.raises(
+        ValueError,
+        match="`sample_names` must be provided as a tuple "
+        + "when more than one input provided.",
+    ):
+        # pass just first sample
+        fastcat.SeqCompare(
+            seq_summary=tuple(files), sample_names=samples[0])
+
+
+def test_107_SeqSummary_empty_file():
     """Create the SeqSummary component with an empty file (summaries)."""
     with _empty_file(dtype=fastcat.FASTCAT_COLS_DTYPES) as fname:
         fastcat.SeqSummary(seq_summary=fname)
 
 
-def test_106_SeqSummary_empty_histogram_files():
+def test_108_SeqSummary_empty_histogram_files():
     """Create the SeqSummary component with an histograms dir with empty files."""
     fastcat.SeqSummary(
         seq_summary=resource_filename(
             "ezcharts", "data/test/histogram_stats/empty_sample/"
         )
     )
```

### Comparing `ezcharts-0.8.0/tests/test_utils.py` & `ezcharts-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

