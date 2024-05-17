# Comparing `tmp/ezcharts-0.7.9.tar.gz` & `tmp/ezcharts-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcharts-0.7.9.tar", last modified: Mon Mar 11 16:00:32 2024, max compression
+gzip compressed data, was "ezcharts-0.8.0.tar", last modified: Fri Apr 12 12:15:41 2024, max compression
```

## Comparing `ezcharts-0.7.9.tar` & `ezcharts-0.8.0.tar`

### file list

```diff
@@ -1,241 +1,289 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.626702 ezcharts-0.7.9/
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-03-11 15:48:21.000000 ezcharts-0.7.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-03-11 15:48:21.000000 ezcharts-0.7.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7901 2024-03-11 16:00:32.626702 ezcharts-0.7.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7354 2024-03-11 15:48:21.000000 ezcharts-0.7.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.514692 ezcharts-0.7.9/ezcharts/
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.518693 ezcharts-0.7.9/ezcharts/components/
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9982 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/bcfstats.py
--rw-rw-rw-   0 root         (0) root         (0)    13432 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/clinvar.py
--rw-rw-rw-   0 root         (0) root         (0)     6395 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/common.py
--rw-rw-rw-   0 root         (0) root         (0)    14124 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/dss.py
--rw-rw-rw-   0 root         (0) root         (0)     3635 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/ezchart.py
--rw-rw-rw-   0 root         (0) root         (0)    25081 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/fastcat.py
--rw-rw-rw-   0 root         (0) root         (0)    12869 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/modkit.py
--rw-rw-rw-   0 root         (0) root         (0)    13245 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/mosdepth.py
--rw-rw-rw-   0 root         (0) root         (0)     1945 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/nextclade.py
--rw-rw-rw-   0 root         (0) root         (0)     1634 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.518693 ezcharts-0.7.9/ezcharts/components/reports/
--rw-rw-rw-   0 root         (0) root         (0)     2952 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2939 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/reports/comp.py
--rw-rw-rw-   0 root         (0) root         (0)     7295 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/reports/labs.py
--rw-rw-rw-   0 root         (0) root         (0)     7667 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/reports/ond.py
--rw-rw-rw-   0 root         (0) root         (0)     2538 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/theme.py
--rw-rw-rw-   0 root         (0) root         (0)     2327 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/components/versions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.498691 ezcharts-0.7.9/ezcharts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.522693 ezcharts-0.7.9/ezcharts/data/icons/
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/icons/circle-check-solid-sage.svg
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/icons/circle-check-solid-white.svg
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/icons/circle-exclamation-solid-red.svg
--rw-rw-rw-   0 root         (0) root         (0)      449 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/icons/circle-exclamation-solid-white.svg
--rw-rw-rw-   0 root         (0) root         (0)      402 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/icons/circle-minus-solid-neutral-cool.svg
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/icons/circle-minus-solid-white.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.522693 ezcharts-0.7.9/ezcharts/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1978 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/images/LAB_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)     2529 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/images/OND_logo.svg
--rw-rw-rw-   0 root         (0) root         (0)    33283 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/images/OND_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)    32771 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/images/ONT_logo.txt
--rw-rw-rw-   0 root         (0) root         (0)   894078 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/images/dots.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.498691 ezcharts-0.7.9/ezcharts/data/reference/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.530694 ezcharts-0.7.9/ezcharts/data/reference/hg19/
--rw-rw-rw-   0 root         (0) root         (0)     6297 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/reference/hg19/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.530694 ezcharts-0.7.9/ezcharts/data/reference/hg38/
--rw-rw-rw-   0 root         (0) root         (0)    11449 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/reference/hg38/cytoBand.txt.gz
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.534694 ezcharts-0.7.9/ezcharts/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1644 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/scripts/epi2melabs.js
--rw-rw-rw-   0 root         (0) root         (0)   394601 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/scripts/metagenomics-sankey-util.js
--rw-rw-rw-   0 root         (0) root         (0)    22492 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/scripts/metagenomics-sankey.js
--rw-rw-rw-   0 root         (0) root         (0)   249710 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/scripts/nextclade.html
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/scripts/ond.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.534694 ezcharts-0.7.9/ezcharts/data/styles/
--rw-rw-rw-   0 root         (0) root         (0)     6168 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/styles/epi2melabs.scss
--rw-rw-rw-   0 root         (0) root         (0)     2585 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/styles/metagenomics-sankey.css
--rw-rw-rw-   0 root         (0) root         (0)  1228637 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/styles/ond.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.550696 ezcharts-0.7.9/ezcharts/data/test/
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/bamstats.flagstat.tsv
--rw-rw-rw-   0 root         (0) root         (0)  1916228 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/bamstats.readstats.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    11320 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/fastcat.stats.gz
--rw-rw-rw-   0 root         (0) root         (0)    28549 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/hg38_cnv.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)     2420 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/hg38_some_bands.bed.gz
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.498691 ezcharts-0.7.9/ezcharts/data/test/histogram_stats/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.550696 ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_1/
--rw-rw-rw-   0 root         (0) root         (0)    17008 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_1/length.hist
--rw-rw-rw-   0 root         (0) root         (0)     6469 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_1/quality.hist
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.554696 ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_2/
--rw-rw-rw-   0 root         (0) root         (0)    17008 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_2/length.hist
--rw-rw-rw-   0 root         (0) root         (0)     6469 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_2/quality.hist
--rw-rw-rw-   0 root         (0) root         (0)   427338 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/karyomap_vals.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    16943 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/nextclade.json
--rw-rw-rw-   0 root         (0) root         (0)      720 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/params.json
--rw-rw-rw-   0 root         (0) root         (0)     1649 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/plot-spec.json
--rwxrwxrwx   0 root         (0) root         (0)      790 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/ref.fa.fai
--rw-rw-rw-   0 root         (0) root         (0)     1797 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/sankey.json
--rw-rw-rw-   0 root         (0) root         (0)  1125122 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/test_dml.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)    35285 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/test_dmr.tsv.gz
--rw-rw-rw-   0 root         (0) root         (0)  1458860 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/test_modkit.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/test_modkit_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)     7150 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/test_mosdepth.bed.gz
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/test_mosdepth_summary.tsv
--rw-rw-rw-   0 root         (0) root         (0)       91 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/test/versions.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.554696 ezcharts-0.7.9/ezcharts/data/themes/
--rw-rw-rw-   0 root         (0) root         (0)     5624 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/themes/epi2melabs.json
--rw-rw-rw-   0 root         (0) root         (0)     5764 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/themes/ond.json
--rw-rw-rw-   0 root         (0) root         (0)     5536 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/themes/walden.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.554696 ezcharts-0.7.9/ezcharts/data/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.498691 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.554696 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/js/
--rw-rw-rw-   0 root         (0) root         (0)    80599 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.570697 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/
--rw-rw-rw-   0 root         (0) root         (0)     5066 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
--rw-rw-rw-   0 root         (0) root         (0)     2055 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
--rw-rw-rw-   0 root         (0) root         (0)     1751 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
--rw-rw-rw-   0 root         (0) root         (0)     3195 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     6685 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     6941 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
--rw-rw-rw-   0 root         (0) root         (0)     5751 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
--rw-rw-rw-   0 root         (0) root         (0)     1948 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
--rw-rw-rw-   0 root         (0) root         (0)     1201 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
--rw-rw-rw-   0 root         (0) root         (0)     8093 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)    10554 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
--rw-rw-rw-   0 root         (0) root         (0)      575 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      294 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
--rw-rw-rw-   0 root         (0) root         (0)     1158 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
--rw-rw-rw-   0 root         (0) root         (0)     6775 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     4043 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
--rw-rw-rw-   0 root         (0) root         (0)     7762 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
--rw-rw-rw-   0 root         (0) root         (0)     4665 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
--rw-rw-rw-   0 root         (0) root         (0)     9104 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
--rw-rw-rw-   0 root         (0) root         (0)     4725 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
--rw-rw-rw-   0 root         (0) root         (0)     3944 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      859 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
--rw-rw-rw-   0 root         (0) root         (0)     6907 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
--rw-rw-rw-   0 root         (0) root         (0)     2016 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
--rw-rw-rw-   0 root         (0) root         (0)    12404 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)     7371 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
--rw-rw-rw-   0 root         (0) root         (0)     4413 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
--rw-rw-rw-   0 root         (0) root         (0)     2490 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
--rw-rw-rw-   0 root         (0) root         (0)     3939 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
--rw-rw-rw-   0 root         (0) root         (0)    17886 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     3840 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
--rw-rw-rw-   0 root         (0) root         (0)    73610 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
--rw-rw-rw-   0 root         (0) root         (0)     1253 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)      938 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.574698 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
--rw-rw-rw-   0 root         (0) root         (0)     2480 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
--rw-rw-rw-   0 root         (0) root         (0)     4833 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
--rw-rw-rw-   0 root         (0) root         (0)     5868 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
--rw-rw-rw-   0 root         (0) root         (0)     2796 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
--rw-rw-rw-   0 root         (0) root         (0)     2603 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
--rw-rw-rw-   0 root         (0) root         (0)     3896 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
--rw-rw-rw-   0 root         (0) root         (0)     1142 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.574698 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
--rw-rw-rw-   0 root         (0) root         (0)      399 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
--rw-rw-rw-   0 root         (0) root         (0)      245 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.582698 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      525 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
--rw-rw-rw-   0 root         (0) root         (0)      230 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
--rw-rw-rw-   0 root         (0) root         (0)     4580 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
--rw-rw-rw-   0 root         (0) root         (0)     1587 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
--rw-rw-rw-   0 root         (0) root         (0)     4164 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
--rw-rw-rw-   0 root         (0) root         (0)     1956 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
--rw-rw-rw-   0 root         (0) root         (0)     4726 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
--rw-rw-rw-   0 root         (0) root         (0)      395 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
--rw-rw-rw-   0 root         (0) root         (0)      582 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
--rw-rw-rw-   0 root         (0) root         (0)     1101 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
--rw-rw-rw-   0 root         (0) root         (0)      661 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
--rw-rw-rw-   0 root         (0) root         (0)     3380 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.582698 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
--rw-rw-rw-   0 root         (0) root         (0)     1737 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.582698 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
--rw-rw-rw-   0 root         (0) root         (0)    10029 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
--rw-rw-rw-   0 root         (0) root         (0)  1017477 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/echarts.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.590699 ezcharts-0.7.9/ezcharts/data/vendor/simple-datatables/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/simple-datatables/simple-datatables.css
--rw-rw-rw-   0 root         (0) root         (0)    38224 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/data/vendor/simple-datatables/simple-datatables.js
--rw-rw-rw-   0 root         (0) root         (0)    15206 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/demo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.590699 ezcharts-0.7.9/ezcharts/layout/
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4086 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.594699 ezcharts-0.7.9/ezcharts/layout/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2880 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/banner.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/cards.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/document.py
--rw-rw-rw-   0 root         (0) root         (0)     2126 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/grid.py
--rw-rw-rw-   0 root         (0) root         (0)     2407 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/offcanvas.py
--rw-rw-rw-   0 root         (0) root         (0)     2758 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/section.py
--rw-rw-rw-   0 root         (0) root         (0)     1550 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/stats.py
--rw-rw-rw-   0 root         (0) root         (0)     7694 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/table.py
--rw-rw-rw-   0 root         (0) root         (0)     5636 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/snippets/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     2893 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/layout/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.622702 ezcharts-0.7.9/ezcharts/plots/
--rw-rw-rw-   0 root         (0) root         (0)     8564 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/_base.py
--rw-rw-rw-   0 root         (0) root         (0) 13970130 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/_model.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/axisgrid.py
--rw-rw-rw-   0 root         (0) root         (0)     7702 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/categorical.py
--rw-rw-rw-   0 root         (0) root         (0)      935 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/demo.py
--rw-rw-rw-   0 root         (0) root         (0)     5065 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)    12803 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/ideogram.py
--rw-rw-rw-   0 root         (0) root         (0)     5066 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/karyomap.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/matrix.py
--rw-rw-rw-   0 root         (0) root         (0)     2720 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/metagenomics_sankey.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/regression.py
--rw-rw-rw-   0 root         (0) root         (0)     6619 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/relational.py
--rwxrwxrwx   0 root         (0) root         (0)     3444 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/sunburst.py
--rw-rw-rw-   0 root         (0) root         (0)     7208 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/plots/util.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-03-11 15:48:21.000000 ezcharts-0.7.9/ezcharts/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.626702 ezcharts-0.7.9/ezcharts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7901 2024-03-11 16:00:32.000000 ezcharts-0.7.9/ezcharts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9544 2024-03-11 16:00:32.000000 ezcharts-0.7.9/ezcharts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 16:00:32.000000 ezcharts-0.7.9/ezcharts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-03-11 16:00:32.000000 ezcharts-0.7.9/ezcharts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-11 15:58:26.000000 ezcharts-0.7.9/ezcharts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      115 2024-03-11 16:00:32.000000 ezcharts-0.7.9/ezcharts.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-11 16:00:32.000000 ezcharts-0.7.9/ezcharts.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      209 2024-03-11 15:48:21.000000 ezcharts-0.7.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-11 16:00:32.626702 ezcharts-0.7.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2187 2024-03-11 15:48:21.000000 ezcharts-0.7.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-11 16:00:32.626702 ezcharts-0.7.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-03-11 15:48:21.000000 ezcharts-0.7.9/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      216 2024-03-11 15:48:21.000000 ezcharts-0.7.9/tests/test_demo.py
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-03-11 15:48:21.000000 ezcharts-0.7.9/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-04-12 12:10:17.000000 ezcharts-0.8.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-04-12 12:10:17.000000 ezcharts-0.8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8031 2024-04-12 12:15:41.480289 ezcharts-0.8.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7484 2024-04-12 12:10:17.000000 ezcharts-0.8.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.344287 ezcharts-0.8.0/ezcharts/
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.352287 ezcharts-0.8.0/ezcharts/components/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9982 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/bcfstats.py
+-rw-rw-rw-   0 root         (0) root         (0)    13432 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/clinvar.py
+-rw-rw-rw-   0 root         (0) root         (0)     6395 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/common.py
+-rw-rw-rw-   0 root         (0) root         (0)    14124 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/dss.py
+-rw-rw-rw-   0 root         (0) root         (0)     3635 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/ezchart.py
+-rw-rw-rw-   0 root         (0) root         (0)    17755 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)    12869 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/modkit.py
+-rw-rw-rw-   0 root         (0) root         (0)    13245 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/mosdepth.py
+-rw-rw-rw-   0 root         (0) root         (0)     1945 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/nextclade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1634 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.356288 ezcharts-0.8.0/ezcharts/components/reports/
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/comp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7435 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/labs.py
+-rw-rw-rw-   0 root         (0) root         (0)     7797 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/reports/ond.py
+-rw-rw-rw-   0 root         (0) root         (0)     2538 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/theme.py
+-rw-rw-rw-   0 root         (0) root         (0)     2327 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/components/versions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.356288 ezcharts-0.8.0/ezcharts/data/icons/
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-check-solid-sage.svg
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-check-solid-white.svg
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-exclamation-solid-red.svg
+-rw-rw-rw-   0 root         (0) root         (0)      449 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-exclamation-solid-white.svg
+-rw-rw-rw-   0 root         (0) root         (0)      402 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-minus-solid-neutral-cool.svg
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/icons/circle-minus-solid-white.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.360288 ezcharts-0.8.0/ezcharts/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1978 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/LAB_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/OND_logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33283 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/OND_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    32771 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/ONT_logo.txt
+-rw-rw-rw-   0 root         (0) root         (0)   894078 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/images/dots.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.328287 ezcharts-0.8.0/ezcharts/data/reference/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.360288 ezcharts-0.8.0/ezcharts/data/reference/hg19/
+-rw-rw-rw-   0 root         (0) root         (0)     6297 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg19/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg19/hg19.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.364288 ezcharts-0.8.0/ezcharts/data/reference/hg38/
+-rw-rw-rw-   0 root         (0) root         (0)    11449 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg38/cytoBand.txt.gz
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/reference/hg38/hg38.chrom.sizes.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.364288 ezcharts-0.8.0/ezcharts/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/epi2melabs.js
+-rw-rw-rw-   0 root         (0) root         (0)   394601 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey-util.js
+-rw-rw-rw-   0 root         (0) root         (0)    22492 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey.js
+-rw-rw-rw-   0 root         (0) root         (0)   249710 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/nextclade.html
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/scripts/ond.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.364288 ezcharts-0.8.0/ezcharts/data/styles/
+-rw-rw-rw-   0 root         (0) root         (0)     6168 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/styles/epi2melabs.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2585 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/styles/metagenomics-sankey.css
+-rw-rw-rw-   0 root         (0) root         (0)  1228637 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/styles/ond.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.380288 ezcharts-0.8.0/ezcharts/data/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/bamstats/
+-rw-rw-rw-   0 root         (0) root         (0)     9394 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/bamstats/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/bamstats/empty.tsv
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/empty-no-header.tsv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/fastcat/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/empty-no-header.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/empty.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     5440 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/f1.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     5426 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/fastcat/f2.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    28549 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/hg38_cnv.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)     2420 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/hg38_some_bands.bed.gz
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/empty_sample/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/empty_sample/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/empty_sample/quality.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.384288 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/
+-rw-rw-rw-   0 root         (0) root         (0)    17008 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)     6469 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/quality.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.388288 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/
+-rw-rw-rw-   0 root         (0) root         (0)    17008 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)     6469 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)   427338 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/karyomap_vals.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    16943 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/nextclade.json
+-rw-rw-rw-   0 root         (0) root         (0)      720 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/params.json
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/plot-spec.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/real_data_test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.388288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/
+-rw-rw-rw-   0 root         (0) root         (0)    27666 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/accuracy.hist
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)   108079 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     5796 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/coverage.hist
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/length.unmap.hist
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode01/quality.unmap.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.392288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/
+-rw-rw-rw-   0 root         (0) root         (0)    15462 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/accuracy.hist
+-rw-rw-rw-   0 root         (0) root         (0)     5591 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.flagstat.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    54744 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/bamstats.readstats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/coverage.hist
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/length.unmap.hist
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-12 12:10:18.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/bamstats/barcode02/quality.unmap.hist
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.332287 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.396288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/
+-rw-rw-rw-   0 root         (0) root         (0)     2985 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/n_seqs
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-file-stats.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    67785 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/per-read-stats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     5502 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode01/run_ids
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.396288 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/length.hist
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/n_seqs
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-file-stats.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    33847 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/per-read-stats.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/quality.hist
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/real_data_test/fastcat/barcode02/run_ids
+-rwxrwxrwx   0 root         (0) root         (0)      790 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/ref.fa.fai
+-rw-rw-rw-   0 root         (0) root         (0)     1797 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/sankey.json
+-rw-rw-rw-   0 root         (0) root         (0)  1125122 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_dml.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    35285 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_dmr.tsv.gz
+-rw-rw-rw-   0 root         (0) root         (0)  1458860 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_modkit.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_modkit_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     7150 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_mosdepth.bed.gz
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/test_mosdepth_summary.tsv
+-rw-rw-rw-   0 root         (0) root         (0)       91 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/test/versions.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.396288 ezcharts-0.8.0/ezcharts/data/themes/
+-rw-rw-rw-   0 root         (0) root         (0)     5624 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/themes/epi2melabs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5764 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/themes/ond.json
+-rw-rw-rw-   0 root         (0) root         (0)     5536 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/themes/walden.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.400288 ezcharts-0.8.0/ezcharts/data/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.336287 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.400288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/js/
+-rw-rw-rw-   0 root         (0) root         (0)    80599 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.416288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2055 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1751 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3195 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6685 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6941 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1948 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     8093 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      294 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_helpers.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6775 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss
+-rw-rw-rw-   0 root         (0) root         (0)      875 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7762 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss
+-rw-rw-rw-   0 root         (0) root         (0)     9104 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4725 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3944 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      859 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss
+-rw-rw-rw-   0 root         (0) root         (0)     6907 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss
+-rw-rw-rw-   0 root         (0) root         (0)    12404 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4413 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2490 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss
+-rw-rw-rw-   0 root         (0) root         (0)      425 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_transitions.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss
+-rw-rw-rw-   0 root         (0) root         (0)    17886 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3840 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss
+-rw-rw-rw-   0 root         (0) root         (0)    73610 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1253 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-reboot.scss
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)      938 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.420288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/
+-rw-rw-rw-   0 root         (0) root         (0)     2480 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4833 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3896 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_validation.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.424288 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_color-bg.scss
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_colored-links.scss
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_ratio.scss
+-rw-rw-rw-   0 root         (0) root         (0)      245 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stacks.scss
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_stretched-link.scss
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_text-truncation.scss
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_visually-hidden.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_vr.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_backdrop.scss
+-rw-rw-rw-   0 root         (0) root         (0)      230 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_banner.scss
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_box-shadow.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_clearfix.scss
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-mode.scss
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_color-scheme.scss
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_container.scss
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4164 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss
+-rw-rw-rw-   0 root         (0) root         (0)     4726 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_image.scss
+-rw-rw-rw-   0 root         (0) root         (0)      582 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_lists.scss
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_pagination.scss
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_reset-text.scss
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_resize.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1101 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss
+-rw-rw-rw-   0 root         (0) root         (0)      168 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_text-truncate.scss
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss
+-rw-rw-rw-   0 root         (0) root         (0)     3380 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)     1737 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/
+-rw-rw-rw-   0 root         (0) root         (0)    10029 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss
+-rw-rw-rw-   0 root         (0) root         (0)  1017477 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/echarts.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css
+-rw-rw-rw-   0 root         (0) root         (0)    38224 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js
+-rw-rw-rw-   0 root         (0) root         (0)    16697 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/demo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.436289 ezcharts-0.8.0/ezcharts/layout/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4086 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.440289 ezcharts-0.8.0/ezcharts/layout/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2880 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/banner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/cards.py
+-rw-rw-rw-   0 root         (0) root         (0)      981 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/document.py
+-rw-rw-rw-   0 root         (0) root         (0)     2126 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     2407 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/offcanvas.py
+-rw-rw-rw-   0 root         (0) root         (0)     2758 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/section.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     7694 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/table.py
+-rw-rw-rw-   0 root         (0) root         (0)     5636 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/snippets/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/layout/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.476289 ezcharts-0.8.0/ezcharts/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/_base.py
+-rw-rw-rw-   0 root         (0) root         (0) 13970130 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/_model.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/axisgrid.py
+-rw-rw-rw-   0 root         (0) root         (0)    11366 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/categorical.py
+-rw-rw-rw-   0 root         (0) root         (0)      935 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     5065 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)    12803 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/ideogram.py
+-rw-rw-rw-   0 root         (0) root         (0)     5066 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/karyomap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/matrix.py
+-rw-rw-rw-   0 root         (0) root         (0)     2720 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/metagenomics_sankey.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/regression.py
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/relational.py
+-rwxrwxrwx   0 root         (0) root         (0)     3463 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/sunburst.py
+-rw-rw-rw-   0 root         (0) root         (0)     9950 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/plots/util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-12 12:10:17.000000 ezcharts-0.8.0/ezcharts/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/ezcharts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8031 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11845 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 12:13:51.000000 ezcharts-0.8.0/ezcharts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      115 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-12 12:15:41.000000 ezcharts-0.8.0/ezcharts.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      209 2024-04-12 12:10:17.000000 ezcharts-0.8.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 12:15:41.480289 ezcharts-0.8.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-04-12 12:10:17.000000 ezcharts-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 12:15:41.480289 ezcharts-0.8.0/tests/components/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11053 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/components/test_fastcat.py
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/test_demo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2024-04-12 12:10:17.000000 ezcharts-0.8.0/tests/test_utils.py
```

### Comparing `ezcharts-0.7.9/LICENSE` & `ezcharts-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/PKG-INFO` & `ezcharts-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.7.9
+Version: 0.8.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bokeh~=3.1.0
@@ -218,14 +218,17 @@
 
 report.write("tmp.html")
 ```
 
 Note that `EZChart()` is required to add the plot to the enclosing `dominate`
 context.
 
+### Debug mode
+Decorator for plotting a message when the plot fails can be skipped by setting the env variable EZCHARTS_DEBUG=1.
+
 **Components**
 
 Components provide higher level application-specific layouts (a table for
 [Nextclade](https://clades.nextstrain.org/) results, for instance) that may also
 include charts and light data processing capabilities (e.g. to parse and
 visualise [fastcat](https://github.com/epi2me-labs/fastcat) output).
```

### Comparing `ezcharts-0.7.9/README.md` & `ezcharts-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,17 @@
 
 report.write("tmp.html")
 ```
 
 Note that `EZChart()` is required to add the plot to the enclosing `dominate`
 context.
 
+### Debug mode
+Decorator for plotting a message when the plot fails can be skipped by setting the env variable EZCHARTS_DEBUG=1.
+
 **Components**
 
 Components provide higher level application-specific layouts (a table for
 [Nextclade](https://clades.nextstrain.org/) results, for instance) that may also
 include charts and light data processing capabilities (e.g. to parse and
 visualise [fastcat](https://github.com/epi2me-labs/fastcat) output).
```

### Comparing `ezcharts-0.7.9/ezcharts/__init__.py` & `ezcharts-0.8.0/ezcharts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Simple eCharts API."""
 
-__version__ = "0.7.9"
+__version__ = "0.8.0"
 
 import argparse
 import importlib
 import logging
 
 from ezcharts import util
 from ezcharts.plots.axisgrid import *  # noqa: F401,F403
```

### Comparing `ezcharts-0.7.9/ezcharts/components/bcfstats.py` & `ezcharts-0.8.0/ezcharts/components/bcfstats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/clinvar.py` & `ezcharts-0.8.0/ezcharts/components/clinvar.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/common.py` & `ezcharts-0.8.0/ezcharts/components/common.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/dss.py` & `ezcharts-0.8.0/ezcharts/components/dss.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/ezchart.py` & `ezcharts-0.8.0/ezcharts/components/ezchart.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/fastcat.py` & `ezcharts-0.8.0/ezcharts/components/fastcat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,666 +1,541 @@
 """An ezcharts component for plotting sequence summaries."""
 import argparse
+import copy
 import os
-from pathlib import Path
 
 import numpy as np
 import pandas as pd
-from pandas.api import types as pd_types
 from pkg_resources import resource_filename
 import sigfig
 
 import ezcharts as ezc
 from ezcharts.components.ezchart import EZChart
 from ezcharts.components.reports.comp import ComponentReport
 from ezcharts.layout.base import Snippet
 from ezcharts.layout.snippets import DataTable, Grid, Tabs
-from ezcharts.plots import util
 
-# Categorical types
-CATEGORICAL = pd_types.CategoricalDtype(ordered=True)
+
+FASTCAT_COLS_DTYPES = {
+    "read_id": str,
+    "filename": "category",
+    "sample_name": "category",
+    "read_length": int,
+    "mean_quality": float,
+    "channel": int,
+    "read_number": int,
+    "start_time": str,
+}
+
+BAMSTATS_COLS_DTYPES = {
+    "name": str,
+    "sample_name": "category",
+    "ref": "category",
+    "coverage": float,
+    "ref_coverage": float,
+    "qstart": "Int64",
+    "qend": "Int64",
+    "rstart": "Int64",
+    "rend": "Int64",
+    "aligned_ref_len": "Int64",
+    "direction": "category",
+    "length": int,
+    "read_length": int,
+    "mean_quality": float,
+    "start_time": str,
+    "match": int,
+    "ins": int,
+    "del": int,
+    "sub": int,
+    "iden": float,
+    "acc": float,
+    "duplex": int,
+}
+
+BAMSTATS_FLAGSTAT_COLS_DTYPES = {
+    "ref": "category",
+    "sample_name": "category",
+    "total": int,
+    "primary": int,
+    "secondary": int,
+    "supplementary": int,
+    "unmapped": int,
+    "qcfail": int,
+    "duplicate": int,
+    "duplex": int,
+    "duplex_forming": int,
+}
+
+TIMES = ["start_time"]
+
+
+def _intersect_columns(base, requested=None):
+    # Take one of the dtype dictionaries and intersect with a list
+    cols = base
+    if requested is not None:
+        if invalid_cols := set(requested) - set(base.keys()):
+            raise ValueError(f"Found unexpected columns {invalid_cols}.")
+        cols = {col: base[col] for col in requested}
+    times = [t for t in TIMES if t in cols]
+    if len(times) == 0:
+        times = None
+    return cols, times
+
+
+def _localize_time(df):
+    # ensure we have datetime format, convert to utc
+    for t in TIMES:
+        if t in df.columns:
+            df[t] = pd.to_datetime(df.start_time, utc=True).dt.tz_localize(None)
+    return df
 
 
 class SeqSummary(Snippet):
     """Generate sequence summary plots."""
 
     def __init__(
-            self,
-            seq_summary=None,
-            histogram_stats_dir=None,
-            theme='epi2melabs',
-            **kwargs):
+        self,
+        seq_summary,
+        flagstat=None,
+        sample_names=None,
+        theme="epi2melabs",
+    ):
         """Create sequence summary component.
 
-        If seq_summary contains results from multiple samples, each will be
-        plotted in its own tab.
-
-        :param seq_summary: A path to a fastcat read stats output file or
-            DataFrame.
-        :param histogram_stats_dir: A path to a directory with fastcat stats histograms
-            in per-sample subdirectories.
-        :param theme: EPI2ME theme.
-        :param kwargs:  options are 'flagstat' and 'bam_summary'.
+        :param seq_summary: a path to a fastcat/bamstats read stats output file
+            or dataframe (or a tuple of such).
+        :param flagstat: a path to a bamstats flagstat output file or dataframe
+            (or tuple of such).
+        :sample_names: tuple of sample names. Required when other input arguments
+            are tuples.
+        :param theme: String defining the visual theme for the plots.
         """
         super().__init__(styles=None, classes=None)
+        self.theme = theme
+
+        # we need at least seq_summary or histograms
+        if not (
+                isinstance(seq_summary, pd.DataFrame)
+                or isinstance(seq_summary, str)
+                or isinstance(seq_summary, tuple)):
+            raise ValueError(
+                "`seq_summary` must be a path to a fastcat/bamstats read stats output "
+                "file or dataframe, or histogram directories (or a tuple of such).")
+
+        # check sample_names is a tuple if files are provided in tuples.
+        if (isinstance(seq_summary, tuple)) and not isinstance(sample_names, tuple):
+            raise ValueError(
+                "`sample_names` must be provided as a tuple "
+                "when more than one input provided.")
+
+        # check tuples are all the same length
+        if isinstance(sample_names, tuple) and (len(sample_names) != len(seq_summary)):
+            raise ValueError(
+                "`sample_names` must have the same length as `seq_summary`.")
+        if (
+                (flagstat is not None)
+                and isinstance(flagstat, tuple)
+                and (len(sample_names) != len(flagstat))):
+            raise ValueError(
+                "`sample_names` must have the same length as `flagstat`.")
 
         with self:
-            if seq_summary is not None:
-                # Assume the input is in fastcat format. If not, try to import as
-                # bamstats format.
-                if isinstance(seq_summary, pd.DataFrame):
-                    df_all = seq_summary
-                else:
-                    try:
-                        df_all = load_stats(seq_summary, format='fastcat')
-                    except ValueError:
-                        df_all = load_stats(seq_summary, format='bamstats')
-                # Check that the file is not empty
-                if df_all.empty:
-                    raise pd.errors.EmptyDataError('seq_summary is empty')
-                # Out of the intersection of columns between `fastcat` and
-                # `bamstats` output, only the column with the read IDs has a
-                # different name (`read_id` in `fastcat` and `name` in `bamstats`).
-                # Rename to ensure the dataframes produced from either `fastcat` or
-                # `bamstats` are consistent.
-                if df_all.columns[0] == "name":
-                    df_all.rename(columns={"name": "read_id"}, inplace=True)
-                # the following assumes that `fastcat` / `bamstats` has been run
-                # with `-s` which is not necessarily the case (if there was only
-                # one sample) --> create a dummy 'sample_name' column if missing
-                if 'sample_name' not in df_all.columns:
-                    df_all['sample_name'] = 'sample'
-                if len(df_all['sample_name'].unique()) == 1:
-                    # we only got a single sample --> no dropdown
-                    draw_all_plots(df_all, theme)
-                else:
-                    # several samples --> use a dropdown menu
-                    tabs = Tabs()
-                    with tabs.add_dropdown_menu():
-                        for sample_id, df_sample in df_all.groupby('sample_name'):
-                            with tabs.add_dropdown_tab(sample_id):
-                                draw_all_plots(df_sample, theme)
-            else:
-                if not histogram_stats_dir:
-                    raise ValueError(
-                        "If seq_summary is not provided, a histogram stats directory"
-                        " path must be provided")
+            if isinstance(seq_summary, tuple):
+                # several samples => use a dropdown
                 tabs = Tabs()
                 with tabs.add_dropdown_menu():
-                    for hist_sample_dir in Path(histogram_stats_dir).iterdir():
-                        if not hist_sample_dir.is_dir():
-                            continue
-                        with tabs.add_dropdown_tab(hist_sample_dir.name):
-                            draw_all_plots_precomputed(hist_sample_dir, theme)
-
-            # Create flagstat tables
-            if "flagstat" in kwargs:
-                if isinstance(kwargs["flagstat"], pd.DataFrame):
-                    flagstat = kwargs["flagstat"]
-                else:
-                    flagstat = load_bamstats_flagstat(kwargs["flagstat"])
-                # Check that the file is not empty
-                if flagstat.empty:
-                    raise pd.errors.EmptyDataError('flagstat is empty')
-                # the following assumes that `fastcat` / `bamstats` has been run
-                # with `-s` which is not necessarily the case (if there was only
-                # one sample) --> create a dummy 'sample_name' column if missing
-                if 'sample_name' not in df_all.columns:
-                    flagstat['sample_name'] = 'sample'
-                if len(flagstat['sample_name'].unique()) == 1:
-                    # we only got a single sample --> no dropdown
-                    DataTable.from_pandas(flagstat, use_index=False)
-                else:
-                    # several samples --> use a dropdown menu
+                    for sample_name, data in zip(sample_names, seq_summary):
+                        with tabs.add_dropdown_tab(sample_name):
+                            self._draw_summary_plots(data)
+            else:
+                # single sample
+                self._draw_summary_plots(seq_summary)
+
+            # same again for flagstat
+            if flagstat is not None:
+                if isinstance(flagstat, tuple):
                     tabs = Tabs()
                     with tabs.add_dropdown_menu():
-                        for sample_id, df_sample in flagstat.groupby('sample_name'):
-                            with tabs.add_dropdown_tab(sample_id):
-                                DataTable.from_pandas(df_sample, use_index=False)
-            # Create bamstats metrics
-            if "bam_summary" in kwargs:
-                if isinstance(kwargs["bam_summary"], pd.DataFrame):
-                    df_all = kwargs["bam_summary"]
-                else:
-                    df_all = load_stats(kwargs["bam_summary"], format='bamstats')
-                # Check that the file is not empty
-                if df_all.empty:
-                    raise pd.errors.EmptyDataError('seq_summary is empty')
-                # Out of the intersection of columns between `fastcat` and
-                # `bamstats` output, only the column with the read IDs has a
-                # different name (`read_id` in `fastcat` and `name` in `bamstats`).
-                # Rename to ensure the dataframes produced from either `fastcat` or
-                # `bamstats` are consistent.
-                if df_all.columns[0] == "name":
-                    df_all.rename(columns={"name": "read_id"}, inplace=True)
-                # the following assumes that `fastcat` / `bamstats` has been run
-                # with `-s` which is not necessarily the case (if there was only
-                # one sample) --> create a dummy 'sample_name' column if missing
-                if 'sample_name' not in df_all.columns:
-                    df_all['sample_name'] = 'sample'
-                if len(df_all['sample_name'].unique()) == 1:
-                    # we only got a single sample --> no dropdown
-                    draw_all_plots(df_all, theme)
+                        for sample_name, data in zip(sample_names, flagstat):
+                            with tabs.add_dropdown_tab(sample_name):
+                                self._draw_flagstat_table(data)
                 else:
-                    # several samples --> use a dropdown menu
-                    tabs = Tabs()
-                    with tabs.add_dropdown_menu():
-                        for sample_id, df_sample in df_all.groupby('sample_name'):
-                            with tabs.add_dropdown_tab(sample_id):
-                                draw_all_plots(df_sample, theme)
+                    self._draw_flagstat_table(flagstat)
 
+    def _draw_summary_plots(self, data):
+        """Draw quality, read_length, yield plots using raw data.
 
-def draw_all_plots(seq_summary, theme):
-    """Draw all three plots using raw data.
-
-    :param seq_summary: pd.DataFrame containing per-sequence summary information.
-    :param theme: EPI2ME theme.
-    """
-    with Grid(columns=3):
-        EZChart(read_quality_plot(seq_summary), theme)
-        EZChart(read_length_plot(seq_summary), theme)
-        EZChart(base_yield_plot(seq_summary), theme)
-
-
-def draw_all_plots_precomputed(hist_dir, theme):
-    """Draw all three plots using pre-computed histograms.
-
-    :param hist_dir: path to fastcat sample histogram directory.
-    :param theme: EPI2ME theme.
-    """
-    length_hist = pd.read_csv(
-        hist_dir / 'length.hist', sep='\t',
-        dtype=np.uint64, names=['start', 'end', 'count'])
-    quality_hist = pd.read_csv(
-        hist_dir / 'quality.hist', sep='\t',
-        dtype=np.float64, names=['start', 'end', 'count'])
-    with Grid(columns=3):
-        EZChart(precomputed_read_quality_plot(quality_hist), theme)
-        EZChart(precomputed_read_length_plot(length_hist), theme)
-        EZChart(precomputed_base_yield_plot(length_hist), theme)
+        :param seq_summary: pd.DataFrame containing per-sequence summary information.
+        :param theme: EPI2ME theme.
+        """
+        # data is either a summary file, a dataframe (of a summary file),
+        # or a directory (of histogram files).
+        qdata, ldata = None, None
+        if isinstance(data, pd.DataFrame):
+            qdata, ldata = data, data
+        else:
+            try:
+                df = load_stats(data)
+                qdata, ldata = df, df
+            except Exception:
+                try:
+                    qdata = load_histogram(data, "quality")
+                    ldata = load_histogram(data, "length")
+                except Exception:
+                    raise ValueError("Could not load input data.")
+
+        with Grid(columns=3):
+            EZChart(read_quality_plot(qdata), self.theme)
+            EZChart(read_length_plot(ldata), self.theme)
+            EZChart(base_yield_plot(ldata), self.theme)
+
+    def _draw_bamstat_table(self, data):
+        if not isinstance(data, pd.DataFrame):
+            data = load_bamstats_flagstat(data)
+        DataTable.from_pandas(data, use_index=False)
 
 
-def base_yield_plot(
-        seq_summary,
-        title='Base yield above read length'):
+@ezc.plots.util.plot_wrapper
+def base_yield_plot(data):
     """Create yield plot by plotting total yield above read length.
 
-    :param seq_summary: pd.DataFrame containing per-sequence summary information.
-    :param title: Plot title.
+    :param data: fastcat/bamstats summary data or read-length histogram data.
     """
-    if not isinstance(seq_summary, pd.DataFrame):
-        df = util.read_files(seq_summary)[['read_length']]
+    xlab = "Read length / kb"
+    ylab = "Yield above length / Gbases"
+    thinning = None  # don't really know why this is different
+    # note: we want an anticumulative sum, hence all the [::-1]
+    if "read_length" in data.columns:
+        # need to create the data
+        thinning = 1000
+        length = np.concatenate(([0], np.sort(data["read_length"])), dtype="int")
+        cumsum = np.cumsum(length[::-1])[::-1]
     else:
-        df = seq_summary
-    df = df.sort_values('read_length', ascending=True)
-    df = pd.concat(
-        (pd.DataFrame.from_dict({'read_length': 0}, orient='index').T, df))
-
-    ylab = 'Yield above length / Gbases'
-    xlab = 'Read length / kb'
-
-    # If we have u/int8 or u/int16 cast to float to prevent overflow
-    df.read_length = df.read_length.astype('uint64')
-    df[ylab] = \
-        df.read_length.cumsum()[::-1].values / 1e+9
-    df[xlab] = df['read_length'] / 1000
-
-    # No need plot all the points
-    if len(df) > 1000:
-        step = len(df) // 1000
-        # thin the data while keeping the last data point
-        df = pd.concat((df.loc[::step, :], df.iloc[[-1]]), axis=0)
-
-    plt = ezc.lineplot(data=df, x=xlab, y=ylab, hue=None)
-    plt.series[0].showSymbol = False
-    plt.title = dict(
-        text=title,
-        subtext=f"Total yield: {sigfig.round(df.iloc[0][ylab], sigfigs=3)} Gb"
-    )
-    return plt
-
+        # assume histogram
+        # TODO: this assumes even bins
+        thinning = 100
+        length = data["start"]
+        cumsum = np.cumsum(
+            data["start"][::-1].to_numpy() * data["count"][::-1].to_numpy()
+        )[::-1]
 
-def histogram_median(hist, x='start', y='count'):
-    """Calculate the median value from histogram data.
-
-    :param hist: pd.DataFrame with columns [start, end, count].
-    :param x: the x-axis variable.
-    :param y: the y-axis variable.
-    """
-    cumsum = np.cumsum(hist[y]).to_numpy()
     mid = cumsum[-1] / 2
-    pos = np.searchsorted(cumsum, mid)
-    return hist[x][pos]
-
-
-def precomputed_base_yield_plot(
-        hist,
-        title='Base yield above read length'):
-    """
-    Create yield above read length plot from pre-computed histogram data.
-
-    :param hist: pd.DataFrame with columns [start, end, count].
-    :param title: plot title.
-    """
-    # reverse the histogram to so that the longest reads come first
-    hist = hist[::-1]
+    n50_index = np.searchsorted(cumsum, mid)
+    n50 = length[n50_index]
 
-    xlab = 'Read length / kb'
-    ylab = 'Yield above length / Gbases'
+    # TODO: we needn't create this only to thin it immediately
+    df = pd.DataFrame({xlab: length / 1000, ylab: cumsum / 1e9}, copy=False)
 
-    # Get read length cumulative sum
-    cs = np.cumsum(hist['start'] * hist['count']).to_numpy()
-    hist[ylab] = cs / 1e+9
-    hist = hist.rename(columns={'start': xlab})
-    hist[xlab] = hist[xlab] / 1000
-
-    mid = cs[-1] / 2
-    n50_index = np.searchsorted(cs, mid)
-    n50 = hist.iat[n50_index, hist.columns.get_loc(xlab)]
-
-    # no need to plot all the points
-    if len(hist) > 100:
-        step = len(hist) // 100
-        # thin the data while keeping the last data point
-        subsampled = hist[::step]
-        if subsampled.iloc[-1][xlab] != hist.iloc[-1][xlab]:
-            subsampled = subsampled.append(hist.iloc[-1])
-        hist = subsampled
+    # thin the data while keeping last
+    if len(df) > thinning:
+        step = len(df) // thinning
+        df = pd.concat((df.loc[::step, :], df.iloc[[-1]]), axis=0)
 
-    plt = ezc.lineplot(x=hist[xlab], y=hist[ylab], hue=None)
+    plt = ezc.lineplot(data=df, x=xlab, y=ylab, hue=None)
     plt.series[0].showSymbol = False
     plt.title = dict(
-        text=title,
+        text="Base yield above read length",
         subtext=(
-            f"Total yield: {sigfig.round(hist[ylab].iloc[0])} "
-            f"Gb. N50: {sigfig.round(n50, 3)}kb")
+            f"Total yield: {sigfig.round(df.iloc[0][ylab], sigfigs=3)} Gb "
+            f"Gb. N50: {sigfig.round(n50, 3)}kb"
+        ),
     )
     return plt
 
 
-def read_quality_plot(
-        seq_summary, binwidth=0.2,
-        min_qual=4, max_qual=30, title='Read quality'):
+@ezc.plots.util.plot_wrapper
+def read_quality_plot(data, binwidth=0.2, min_qual=4, max_qual=30):
     """Create read quality summary plot.
 
-    :param seq_summary: pd.DataFrame containing per-sequence summary information.
+    :param data: fastcat/bamstats summary data or read-length histogram data.
     :param binwidth: width of each bin.
     :param min_qual: the minimum quality value to plot.
     :param max_qual: the maximum quality value to plot.
     :param title: title of the plot.
     """
-    if not isinstance(seq_summary, pd.DataFrame):
-        df = util.read_files(seq_summary)[['mean_quality']]
+    plt, mean_q, median_q = None, None, None
+    if "read_length" in data.columns:
+        # fastcat/bamstats
+        mean_q = np.round(data.mean_quality.mean(), 1)
+        median_q = int(data.mean_quality.median())
+        plt = ezc.histplot(
+            data=data.mean_quality, binwidth=binwidth, binrange=(min_qual, max_qual)
+        )
     else:
-        df = seq_summary
-    mean_q = np.round(df.mean_quality.mean(), 1)
-    median_q = int(df.mean_quality.median())
-
-    plt = ezc.histplot(
-        data=df.mean_quality, binwidth=binwidth, binrange=(min_qual, max_qual))
-    plt.title = dict(
-        text=title,
-        subtext=f"Mean: {mean_q}. Median: {median_q}")
-    plt.xAxis.name = 'Quality score'
-    plt.xAxis.min, plt.xAxis.max = min_qual, max_qual
-    plt.yAxis.name = 'Number of reads'
-    return plt
-
-
-def precomputed_read_quality_plot(
-        hist, binwidth=0.2,
-        min_qual=4, max_qual=30, title='Read quality'):
-    """Create read quality summary plot from pre-computed histograms.
+        # histogram
+        mean_q = np.round(
+            np.average(0.5 * (data["start"] + data["end"]), weights=data["count"]), 1
+        )
+        median_q = int(histogram_median(data))
+        plt = ezc.histplot(
+            data=data["start"],
+            weights=data["count"],
+            binwidth=binwidth,
+            binrange=(min_qual, max_qual),
+        )
 
-    :param hist: pd.DataFrame with columns [start, end, count].
-    :param binwidth: width of each bin.
-    :param min_qual: the minimum quality value to plot.
-    :param max_qual: the maximum quality value to plot.
-    :param title: title of the plot.
-    """
-    median = histogram_median(hist)
-    mean_q = np.average(0.5*(hist["start"] + hist["end"]), weights=hist['count'])
-    plt = ezc.histplot(
-        data=hist['start'], weights=hist['count'],
-        binwidth=binwidth, binrange=(min_qual, max_qual))
     plt.title = dict(
-        text=title,
-        subtext=f"Mean: {mean_q:.1f}. Median: {median:.1f}")
-    plt.xAxis.name = 'Quality score'
+        text="Read quality", subtext=f"Mean: {mean_q:.1f}. Median: {median_q:.1f}"
+    )
+    plt.xAxis.name = "Quality score"
     plt.xAxis.min, plt.xAxis.max = min_qual, max_qual
-    plt.yAxis.name = 'Number of reads'
+    plt.yAxis.name = "Number of reads"
     return plt
 
 
+@ezc.plots.util.plot_wrapper
 def read_length_plot(
-    seq_summary,
-    xlim=(0, None),
-    quantile_limits=False,
-    bins=100,
-    bin_width=None,
-    title="Read length",
+    data, xlim=(0, None), quantile_limits=False, bins=100, binwidth=None
 ):
     """Create a read length plot.
 
     :param seq_summary: pd.DataFrame containing per-sequence summary information.
     :param xlim: viewable read length limits.
     :param quantile_limits: if True, xlim is interpreted as quantiles of the data rather
         than absolute values.
     :param bins: number of bins.
-    :param bin_width: bin width.
+    :param binwidth: bin width.
     :param title: plot title.
 
     The reads will be filtered with `min_len` and `max_len` before calculating the
     histogram. The subtext of the plot title will still show the mean / median / maximum
     of the full data.
     """
-    if not isinstance(seq_summary, pd.DataFrame):
-        df = util.read_files(seq_summary)[['read_length']]
-    else:
-        df = seq_summary
-
-    mean_length = int(df['read_length'].mean())
-    median_length = int(np.median(df['read_length']))
-    max_ = int(np.max(df['read_length']))
-    min_ = int(np.min(df['read_length']))
-
-    read_lengths = df['read_length'].values
-
+    plt, mean_length, median_length = None, None, None
     min_len, max_len = xlim
-
     if min_len is None:
         min_len = 0
-    if max_len is None:
-        max_len = 1 if quantile_limits else read_lengths.max()
-
-    if quantile_limits:
-        min_len, max_len = np.quantile(read_lengths, [min_len, max_len])
-        # set `xlim` so that we can use it to set the x-axis limits below
-        xlim = (min_len, max_len)
-
-    read_lengths = read_lengths[
-        (read_lengths >= min_len) & (read_lengths <= max_len)
-    ]
-
-    read_lengths = read_lengths / 1000
-    if bin_width is not None:
-        bin_width /= 1000
+    # create data to plot depending on input type.
+    if "read_length" in data.columns:
+        # fastcat/bamstats
+        mean_length = np.round(data.read_length.mean(), 1)
+        median_length = int(data.read_length.median())
+        max_ = int(np.max(data["read_length"]))
+        min_ = int(np.min(data["read_length"]))
+        read_lengths = data["read_length"].values
+
+        if max_len is None:
+            max_len = 1 if quantile_limits else read_lengths.max()
+
+        if quantile_limits:
+            min_len, max_len = np.quantile(read_lengths, [min_len, max_len])
+            # set `xlim` so that we can use it to set the x-axis limits below
+            xlim = (min_len, max_len)
+
+        read_lengths = read_lengths[
+            (read_lengths >= min_len) & (read_lengths <= max_len)
+        ]
+
+        read_lengths = read_lengths / 1000
+        if binwidth is not None:
+            binwidth /= 1000
+        plt = ezc.histplot(data=read_lengths, bins=bins, binwidth=binwidth)
+    else:
+        # histogram
+        if max_len is None:
+            max_len = 1 if quantile_limits else data.iloc[-1]["end"]
+        if quantile_limits:
+            cs = np.cumsum(data["count"])
+            lower_idx, upper_idx = np.searchsorted(cs, np.quantile(cs, quantile_limits))
+            min_len, max_len = (data["start"][lower_idx], data["end"][upper_idx])
+            xlim = (min_len, max_len)
+
+        median_length = histogram_median(data)
+        mean_length = np.average(data["start"], weights=data["count"])
+        max_ = data.iloc[-1]["end"]
+        min_ = data.iloc[0]["start"]
+        data = data[(data["start"] >= min_len) & (data["end"] <= max_len)]
+        plt = ezc.histplot(
+            data=data["start"] / 1000,
+            bins=bins,
+            binwidth=binwidth,
+            weights=data["count"],
+        )
 
-    plt = ezc.histplot(data=read_lengths, bins=bins, binwidth=bin_width)
+    # customize the plot
     plt.title = dict(
-        text=title,
+        text="Read Length",
         subtext=(
-            f"Mean: {mean_length:,d}. Median: {median_length:,d}. "
+            f"Mean: {mean_length:.1f}. Median: {median_length:.1f}. "
             f"Min: {min_:,d}. Max: {max_:,d}"
-        )
+        ),
     )
-    plt.xAxis.name = 'Read length / kb'
-    plt.yAxis.name = 'Number of reads'
+    plt.xAxis.name = "Read length / kb"
+    plt.yAxis.name = "Number of reads"
 
     if xlim[0] is not None:
         plt.xAxis.min = xlim[0] / 1000
     if xlim[1] is not None:
         plt.xAxis.max = xlim[1] / 1000
     return plt
 
 
-def precomputed_read_length_plot(
-        hist,
-        xlim=(0, None),
-        quantile_limits=False,
-        bins=100,
-        bin_width=None,
-        title="Read length"):
-    """Create a read length plot from pre-computed histogram data.
+def load_fastcat(fpath, target_cols=None):
+    """Load and prepare fastcat per-read stats.
 
-    :param hist: pd.DataFrame with columns [start, end, count].
-    :param xlim: viewable read length limits.
-    :param quantile_limits: if True, xlim is interpreted as quantiles of the data
-        rather than absolute values.
-    :param bins: number of bins.
-    :param bin_width: bin width.
-    :param title: plot title.
+    :param fpath: path to a fastcat stats file.
+    :target_cols: columns to be loaded in the dataframe.
 
-    The reads will be filtered with `min_len` and `max_len` before calculating the
-    histogram. The subtext of the plot title will still show the mean / median / maximum
-    of the full data.
+    :returns: a dataframe
     """
-    min_len, max_len = xlim
+    cols, time_cols = _intersect_columns(copy.copy(FASTCAT_COLS_DTYPES), target_cols)
+    try:
+        df = pd.read_csv(
+            fpath, sep="\t", usecols=cols.keys(), dtype=cols, parse_dates=time_cols
+        )
+    except pd.errors.EmptyDataError:
+        raise Exception(f"Empty input: {fpath}")
+    df = _localize_time(df)
+    return df
 
-    if min_len is None:
-        min_len = 0
-    if max_len is None:
-        max_len = 1 if quantile_limits else hist.iloc[-1]['end']
 
-    if quantile_limits:
-        cs = np.cumsum(hist['count'])
-        lower_idx, upper_idx = np.searchsorted(
-            cs, np.quantile(cs, quantile_limits))
-        min_len, max_len = (hist['start'][lower_idx], hist['end'][upper_idx])
-        xlim = (min_len, max_len)
-
-    median_length = histogram_median(hist)
-    mean_length = np.average(hist['start'], weights=hist['count'])
-    max_ = hist.iloc[-1]['end']
-    min_ = hist.iloc[0]['start']
+def load_bamstats(fpath, target_cols=None):
+    """Load and prepare bamstats per-read stats.
 
-    hist = hist[(hist['start'] >= min_len) & (hist['end'] <= max_len)]
+    :param fpath: path to a bamstats stats file.
+    :target_cols: columns to be loaded in the dataframe.
 
-    plt = ezc.histplot(
-        data=hist['start'] / 1000, bins=bins, binwidth=bin_width, weights=hist['count'])
-    plt.title = dict(
-        text=title,
-        subtext=(
-            f"Mean: {mean_length:.1f}. Median: {median_length:.1f}. "
-            f"Min: {min_:,d}. Max: {max_:,d}"
+    :returns: a dataframe
+    """
+    cols, time_cols = _intersect_columns(copy.copy(BAMSTATS_COLS_DTYPES), target_cols)
+    try:
+        df = pd.read_csv(
+            fpath, sep="\t", usecols=cols.keys(), dtype=cols, parse_dates=time_cols
         )
-    )
-    plt.xAxis.name = 'Read length / kb'
-    plt.yAxis.name = 'Number of reads'
-
-    if xlim[0] is not None:
-        plt.xAxis.min = xlim[0] / 1000
-    if xlim[1] is not None:
-        plt.xAxis.max = xlim[1] / 1000
-    return plt
+    except pd.errors.EmptyDataError:
+        raise Exception(f"Empty input: {fpath}")
+    df = _localize_time(df)
+    # to be consistent with fastcat
+    df.rename(columns={"name": "read_id"}, inplace=True)
+    return df
 
 
-def load_bamstats_flagstat(flagstat):
+def load_bamstats_flagstat(fpath):
     """Load and prepare bamstats flagstat output.
 
-    :param flagstat: path to file(s) containing bamstats flagstat output. Either a
-        path to a single file or a path to a directory containing stats files.
+    :param fpath: path to a bamstats flagstat file.
+
+    :returns: a dataframe
     """
-    relevant_stats_cols_dtypes = {
-        "ref": CATEGORICAL,
-        "sample_name": CATEGORICAL,
-        "total": int,
-        "primary": int,
-        "secondary": int,
-        "supplementary": int,
-        "unmapped": int,
-        "qcfail": int,
-        "duplicate": int,
+    try:
+        df = pd.read_csv(
+            fpath,
+            sep="\t",
+            usecols=BAMSTATS_FLAGSTAT_COLS_DTYPES.keys(),
+            dtype=BAMSTATS_FLAGSTAT_COLS_DTYPES,
+        )
+    except pd.errors.EmptyDataError:
+        raise Exception(f"Empty input: {fpath}")
+    df["status"] = df["ref"].apply(lambda x: "Unmapped" if x == "*" else "Mapped")
+    return df
+
+
+def load_histogram(hist_dir, dtype="quality"):
+    """Load fastcat/bamstats histograms.
+
+    :param hist_dir: pathname to input directory.
+    :param dtype: histogram datatype to load.
+    """
+    allowed = {
+        "quality",
+        "length",
+        "quality.unmap",
+        "length.unmap",
+        "accuracy",
+        "coverage",
     }
-    # Prepare input files
-    dfs = []
-    if os.path.isdir(flagstat):
-        input_files = [(flagstat, i) for i in os.listdir(flagstat)]
-    elif os.path.isfile(flagstat):
-        input_files = [(None, flagstat)]
-    else:
-        raise Exception(f'No valid input: {flagstat}')
-    # If no files, throw error
-    if len(input_files) == 0:
-        raise FileNotFoundError(f'No valid input found in {flagstat}')
-    # Start processing file
-    for inpath, fname in input_files:
-        try:
-            flagstat_file = fname if inpath is None else f'{inpath}/{fname}'
-            df = pd.read_csv(
-                flagstat_file, sep="\t",
-                usecols=relevant_stats_cols_dtypes.keys(),
-                dtype=relevant_stats_cols_dtypes)
-            # If it's empty, add an empty DF
-            if df.empty:
-                cols = relevant_stats_cols_dtypes.update(
-                    {'Status': str, 'filename': str})
-                dfs.append(pd.DataFrame(columns=cols))
-                continue
-            # Add mapped/unmapped status
-            df["Status"] = df["ref"].apply(
-                lambda x: "Unmapped" if x == "*" else "Mapped"
-            )
-            # Add file name
-            df['filename'] = fname.split('/')[-1]
-            # Append processed DF
-            dfs.append(df)
-        except pd.errors.EmptyDataError:
-            cols = relevant_stats_cols_dtypes.update({'filename': str})
-            dfs.append(pd.DataFrame(columns=cols.keys()).astype(cols))
-    return pd.concat(dfs).reset_index(drop=True)
-
-
-def load_stats(stat, format=None):
-    """Load and prepare bamstats flagstat.
-
-    :param stat: flagstat file paths. Either a single path to a file, a list/tuple of
-        paths, or a path to a directory containing files.
-    :param format: stats source: bamstats/fastcat.
+    if dtype not in allowed:
+        raise ValueError(f"`dtype` must be one of {allowed}.")
+    dt = float
+    if "length" in dtype:
+        dt = int
+
+    hist = pd.read_csv(
+        os.path.join(hist_dir, f"{dtype}.hist"),
+        sep="\t",
+        names=["start", "end", "count"],
+        dtype={"start": dt, "end": dt, "count": int},
+    )
+    return hist
+
+
+def load_stats(fpath, target_cols=None):
+    """Load and prepare fastcat or bamstats per-read stats.
+
+    This function is intended to be used when the caller does not know (and care)
+    the origin of the input file, but wishes to load the common columns.
 
+    :params fpath: path to a fastcat or bamstats stats file.
+    :param target_cols: list of columns to read from file.
+
+    :returns: a dataframe
     """
-    # Input columns for bamstats
-    bamstats_cols_dtypes = {
-        "name": str,
-        "sample_name": CATEGORICAL,
-        "ref": CATEGORICAL,
-        "coverage": float,
-        "ref_coverage": float,
-        "read_length": int,
-        "mean_quality": float,
-        "acc": float,
-    }
-    # Input columns for fastcat
-    fastcat_cols_dtypes = {
-        "read_id": str,
-        "filename": CATEGORICAL,
-        "sample_name": CATEGORICAL,
-        "read_length": int,
-        "mean_quality": float,
-        "channel": int,
-        "read_number": int,
-        "start_time": str,
-    }
-    # Infer format
-    if format == 'bamstats':
-        relevant_stats_cols_dtypes = bamstats_cols_dtypes
-        time_cols = None
-    elif format == 'fastcat':
-        relevant_stats_cols_dtypes = fastcat_cols_dtypes
-        time_cols = ['start_time']
-    else:
-        raise ValueError(f"{format} not valid file type")
-    # Prepare input files
-    dfs = []
-    if isinstance(stat, (list, tuple)) and all([os.path.isfile(path) for path in stat]):
-        # got a list of files
-        input_files = [(None, file) for file in stat]
-    elif os.path.isdir(stat):
-        input_files = [(stat, i) for i in os.listdir(stat)]
-    elif os.path.isfile(stat):
-        input_files = [(None, stat)]
-    else:
-        raise Exception(f'No valid input: {stat}')
-    # If no files, throw error
-    if len(input_files) == 0:
-        raise FileNotFoundError(f'No valid input found in {stat}')
-    # Start processing
-    for (inpath, fname) in input_files:
-        try:
-            fastcat_file = fname if not inpath else f'{inpath}/{fname}'
-            df = pd.read_csv(
-                fastcat_file,
-                sep="\t",
-                header=0,
-                usecols=relevant_stats_cols_dtypes.keys(),
-                dtype=relevant_stats_cols_dtypes,
-                parse_dates=time_cols
-                )
-            # If it's empty, add an empty DF
-            if df.empty:
-                cols = relevant_stats_cols_dtypes.update(
-                    {'filename': str})
-                dfs.append(
-                    pd.DataFrame(columns=cols).rename(columns={'name': 'read_id'}))
-                continue
-            # Add file name if missing
-            if 'filename' not in df.columns:
-                df['filename'] = fname.split('/')[-1]
-            # Rename "name" to "read_id"
-            if 'read_id' not in df.columns and 'name' in df.columns:
-                df.rename(columns={'name': 'read_id'}, inplace=True)
-            if format == 'fastcat':
-                # Ensure we have datetime format
-                # Use utc=true to account for mixed time offsets.
-                # This converts dates to UTC.
-                # https://pandas.pydata.org/docs/reference/api/pandas.to_datetime.html
-                df['start_time'] = pd.to_datetime(
-                    df.start_time, utc=True).dt.tz_localize(None)
-            # Append processed DF
-            dfs.append(df)
-        except pd.errors.EmptyDataError:
-            cols = relevant_stats_cols_dtypes.update({'filename': str})
-            dfs.append(
-                pd.DataFrame(columns=cols.keys()).astype(cols))
-    # concatenate and emit
-    return pd.concat(dfs).reset_index(drop=True)
+    if target_cols is None:
+        target_cols = ["sample_name", "read_length", "mean_quality"]
+    df = None
+    try:
+        df = load_fastcat(fpath, target_cols=target_cols)
+    except ValueError:
+        df = load_bamstats(fpath, target_cols=target_cols)
+    return df
+
+
+def histogram_median(hist, x="start", y="count"):
+    """Calculate the median value from histogram data.
+
+    :param hist: pd.DataFrame with columns [start, end, count].
+    :param x: the x-axis variable.
+    :param y: the y-axis variable.
+    """
+    # TODO: start and end may not be end = start + 1
+    cumsum = np.cumsum(hist[y]).to_numpy()
+    mid = cumsum[-1] / 2
+    pos = np.searchsorted(cumsum, mid)
+    return hist[x][pos]
 
 
 def main(args):
     """Entry point to demonstrate a sequence summary component."""
-    comp_title = 'Sequence Summary'
+    comp_title = "Sequence Summary"
     # Define inputs.
     # If seq_summary is not passed, then use bam_readstats
     if args.seq_summary:
         seq_summary = args.seq_summary
     elif args.seq_summary is None and args.bam_readstats is not None:
         seq_summary = args.bam_readstats
     else:
-        raise ValueError('No valid input for seq_summary/bam_readstats.')
-    if args.seq_summary is not None and args.bam_readstats is not None:
-        bam_summary = args.bam_readstats
-    else:
-        bam_summary = None
+        raise ValueError("No valid input for seq_summary/bam_readstats.")
     # Create summary
-    seq_sum = SeqSummary(
-        seq_summary,
-        bam_summary=bam_summary,
-        flagstat=args.bam_flagstat
-        )
+    seq_sum = SeqSummary(seq_summary, flagstat=args.bam_flagstat)
     # Write report
     report = ComponentReport(comp_title, seq_sum)
     report.write(args.output)
 
 
 def argparser():
     """Argument parser for entrypoint."""
     parser = argparse.ArgumentParser(
-        'Sequence summary',
+        "Sequence summary",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        add_help=False)
+        add_help=False,
+    )
     parser.add_argument(
         "--seq_summary",
-        default=resource_filename('ezcharts', "data/test/fastcat.stats.gz"),
-        help="Sequence summary TSV from fastcat.")
+        default=resource_filename("ezcharts", "data/test/fastcat"),
+        help="Sequence summary TSV from fastcat.",
+    )
     parser.add_argument(
         "--bam_flagstat",
-        default=resource_filename('ezcharts', "data/test/bamstats.flagstat.tsv"),
-        help="Bam flagstats TSV from bamstats.")
+        default=resource_filename(
+            "ezcharts", "data/test/bamstats/bamstats.flagstat.tsv"
+        ),
+        help="Bam flagstats TSV from bamstats.",
+    )
     parser.add_argument(
         "--bam_readstats",
-        default=resource_filename('ezcharts', "data/test/bamstats.readstats.tsv.gz"),
-        help="Read statistics TSV from bamstats.")
+        default=resource_filename("ezcharts", "data/test/bamstats/"),
+        help="Read statistics TSV from bamstats.",
+    )
     parser.add_argument(
-        "--output",
-        default="seq_summary_report.html",
-        help="Output HTML file.")
+        "--output", default="seq_summary_report.html", help="Output HTML file."
+    )
     return parser
```

### Comparing `ezcharts-0.7.9/ezcharts/components/modkit.py` & `ezcharts-0.8.0/ezcharts/components/modkit.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/mosdepth.py` & `ezcharts-0.8.0/ezcharts/components/mosdepth.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/nextclade.py` & `ezcharts-0.8.0/ezcharts/components/nextclade.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/params.py` & `ezcharts-0.8.0/ezcharts/components/params.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/reports/__init__.py` & `ezcharts-0.8.0/ezcharts/components/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/reports/comp.py` & `ezcharts-0.8.0/ezcharts/components/reports/comp.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/reports/labs.py` & `ezcharts-0.8.0/ezcharts/components/reports/labs.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """A styled footer component for use in a Report."""
 
     TAG = 'div'
 
     def __init__(
         self,
         workflow_name: str,
+        workflow_version: str,
         classes: ILabsAddendumClasses = ILabsAddendumClasses(),
         use_defaults: bool = True
     ) -> None:
         """Create tag."""
         super().__init__(
             styles=None,
             classes=classes,
@@ -43,20 +44,19 @@
 
         with self:
             self.container = div(className=classes.inner)
 
         if use_defaults:
             with self.container:
                 h4('About this report', className="pb-3")
-                with p(
-                    "This report was produced using the "
-                    f"epi2me-labs/{workflow_name}. The workflow "
-                    "can be run using"
-                ):
-                    code(f"nextflow run epi2me-labs/{workflow_name} --help")
+                p(
+                    "This report was produced using the ",
+                    code(f"epi2me-labs/{workflow_name}"),
+                    f" nextflow workflow ({workflow_version})."
+                )
                 p(
                     "Oxford Nanopore Technologies products are not "
                     "intended for use for health assessment or to "
                     "diagnose, treat, mitigate, cure or prevent any "
                     "disease or condition.")
 
 
@@ -100,15 +100,15 @@
             classes=classes,
             style=f"min-height: {header_height}px;",
             className=classes.container)
 
         spacer.add(self)
         with self:
             with div(className=self.classes.inner):
-                with a(href="/", className=self.classes.logo):
+                with a(href="https://labs.epi2me.io/", className=self.classes.logo):
                     logo()
                 for group in groups:
                     setattr(
                         self, group,
                         ul(className=self.classes.nav_list, __pretty=False))
 
     def add_link(
@@ -167,14 +167,15 @@
 
     def __init__(
         self,
         report_title,
         workflow_name,
         workflow_params_path: str,
         workflow_versions_path: str,
+        workflow_version: str,
         logo: Type[html_tag] = EPI2MELabsLogo,
         head_resources: List[Resource] = LAB_head_resources,
         body_resources: List[Resource] = LAB_body_resources,
         created_date: Optional[str] = None
     ) -> None:
         """Create tag."""
         super().__init__(
@@ -188,14 +189,15 @@
             self.intro_content = section(id="intro-content", role="region")
             with self.intro_content:
                 self.banner = Banner(report_title, workflow_name)
                 self.banner.add_badge("Research use only")
                 if not created_date:
                     created_date = datetime.today().strftime('%Y-%m-%d')
                 self.banner.add_badge(created_date, bg_class="bg-secondary")
+                self.banner.add_badge(workflow_version)
 
         with self.main:
             self.meta_content = section(id="meta-content", role="region")
             with self.meta_content:
                 with Section(
                     "versions",
                     'Software versions',
@@ -207,15 +209,17 @@
                     "parameters",
                     'Workflow parameters',
                     overflow=True
                 ):
                     ParamsTable(workflow_params_path)
 
         with self.footer:
-            self.addendum = LabsAddendum(workflow_name=workflow_name)
+            self.addendum = LabsAddendum(
+                workflow_name=workflow_name, workflow_version=workflow_version
+            )
 
     def add_badge(
         self,
         title: str,
         bg_class=None
     ) -> None:
         """Add a badge to the banner."""
```

### Comparing `ezcharts-0.7.9/ezcharts/components/reports/ond.py` & `ezcharts-0.8.0/ezcharts/components/reports/ond.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """A styled footer component for use in a Report."""
 
     TAG = 'div'
 
     def __init__(
         self,
         workflow_name: str,
+        workflow_version: str,
         classes: ILabsAddendumClasses = ILabsAddendumClasses(),
         use_defaults: bool = True
     ) -> None:
         """Create tag."""
         super().__init__(
             styles=None,
             classes=classes,
@@ -43,20 +44,19 @@
 
         with self:
             self.container = div(className=classes.inner)
 
         if use_defaults:
             with self.container:
                 h4('About this report', className="pb-3")
-                with p(
-                    "This report was produced using the "
-                    f"epi2me-labs/{workflow_name}. The workflow "
-                    "can be run using"
-                ):
-                    code(f"nextflow run epi2me-labs/{workflow_name} --help")
+                p(
+                    "This report was produced using the ",
+                    code(f"epi2me-labs/{workflow_name}"),
+                    f" nextflow workflow ({workflow_version})."
+                )
                 p(
                     "Oxford Nanopore Technologies products are not "
                     "intended for use for health assessment or to "
                     "diagnose, treat, mitigate, cure or prevent any "
                     "disease or condition.")
 
 
@@ -172,14 +172,15 @@
 
     def __init__(
         self,
         report_title,
         workflow_name,
         workflow_params_path: str,
         workflow_versions_path: str,
+        workflow_version: str,
         logo: Type[html_tag] = ONDLogo,
         head_resources: List[Resource] = OND_head_resources,
         body_resources: List[Resource] = OND_body_resources,
         created_date: Optional[str] = None,
         default_content: bool = True
     ) -> None:
         """Create tag."""
@@ -195,14 +196,15 @@
                 self.intro_content = section(id="intro-content", role="region")
                 with self.intro_content:
                     self.banner = Banner(report_title, workflow_name)
                     self.banner.add_badge("Research use only", bg_class='bg-danger')
                     if not created_date:
                         created_date = datetime.today().strftime('%Y-%m-%d')
                         self.banner.add_badge(created_date, bg_class="bg-secondary")
+                    self.banner.add_badge(workflow_version)
 
             with self.main:
                 self.meta_content = section(id="meta-content", role="region")
                 with self.meta_content:
                     with Section(
                         "versions",
                         'Software versions',
@@ -214,15 +216,17 @@
                         "parameters",
                         'Workflow parameters',
                         overflow=True
                     ):
                         ParamsTable(workflow_params_path)
 
             with self.footer:
-                self.addendum = LabsAddendum(workflow_name=workflow_name)
+                self.addendum = LabsAddendum(
+                    workflow_name=workflow_name, workflow_version=workflow_version
+                )
 
     def add_badge(
         self,
         title: str,
         bg_class=None
     ) -> None:
         """Add a badge to the banner."""
```

### Comparing `ezcharts-0.7.9/ezcharts/components/theme.py` & `ezcharts-0.8.0/ezcharts/components/theme.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/components/versions.py` & `ezcharts-0.8.0/ezcharts/components/versions.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/images/LAB_logo.svg` & `ezcharts-0.8.0/ezcharts/data/images/LAB_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/images/OND_logo.svg` & `ezcharts-0.8.0/ezcharts/data/images/OND_logo.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/images/OND_logo.txt` & `ezcharts-0.8.0/ezcharts/data/images/OND_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/images/ONT_logo.txt` & `ezcharts-0.8.0/ezcharts/data/images/ONT_logo.txt`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/images/dots.svg` & `ezcharts-0.8.0/ezcharts/data/images/dots.svg`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/reference/hg19/cytoBand.txt.gz` & `ezcharts-0.8.0/ezcharts/data/reference/hg19/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/reference/hg38/cytoBand.txt.gz` & `ezcharts-0.8.0/ezcharts/data/reference/hg38/cytoBand.txt.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/scripts/epi2melabs.js` & `ezcharts-0.8.0/ezcharts/data/scripts/epi2melabs.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/scripts/metagenomics-sankey-util.js` & `ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey-util.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/scripts/metagenomics-sankey.js` & `ezcharts-0.8.0/ezcharts/data/scripts/metagenomics-sankey.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/scripts/nextclade.html` & `ezcharts-0.8.0/ezcharts/data/scripts/nextclade.html`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/scripts/ond.js` & `ezcharts-0.8.0/ezcharts/data/scripts/ond.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/styles/epi2melabs.scss` & `ezcharts-0.8.0/ezcharts/data/styles/epi2melabs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/styles/metagenomics-sankey.css` & `ezcharts-0.8.0/ezcharts/data/styles/metagenomics-sankey.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/styles/ond.scss` & `ezcharts-0.8.0/ezcharts/data/styles/ond.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/hg38_cnv.bed.gz` & `ezcharts-0.8.0/ezcharts/data/test/hg38_cnv.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/hg38_some_bands.bed.gz` & `ezcharts-0.8.0/ezcharts/data/test/hg38_some_bands.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_1/length.hist` & `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_1/quality.hist` & `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_1/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_2/length.hist` & `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/length.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/histogram_stats/sample_2/quality.hist` & `ezcharts-0.8.0/ezcharts/data/test/histogram_stats/sample_2/quality.hist`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/karyomap_vals.tsv.gz` & `ezcharts-0.8.0/ezcharts/data/test/karyomap_vals.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/nextclade.json` & `ezcharts-0.8.0/ezcharts/data/test/nextclade.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/params.json` & `ezcharts-0.8.0/ezcharts/data/test/params.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/plot-spec.json` & `ezcharts-0.8.0/ezcharts/data/test/plot-spec.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/ref.fa.fai` & `ezcharts-0.8.0/ezcharts/data/test/ref.fa.fai`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/sankey.json` & `ezcharts-0.8.0/ezcharts/data/test/sankey.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/test_dml.tsv.gz` & `ezcharts-0.8.0/ezcharts/data/test/test_dml.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/test_dmr.tsv.gz` & `ezcharts-0.8.0/ezcharts/data/test/test_dmr.tsv.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/test_modkit.bed.gz` & `ezcharts-0.8.0/ezcharts/data/test/test_modkit.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/test/test_mosdepth.bed.gz` & `ezcharts-0.8.0/ezcharts/data/test/test_mosdepth.bed.gz`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/themes/epi2melabs.json` & `ezcharts-0.8.0/ezcharts/data/themes/epi2melabs.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/themes/ond.json` & `ezcharts-0.8.0/ezcharts/data/themes/ond.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/themes/walden.json` & `ezcharts-0.8.0/ezcharts/data/themes/walden.json`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables-dark.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_alert.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss` & `ezcharts-0.8.0/ezcharts/data/vendor/bootstrap-5.3.0/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/echarts.min.js` & `ezcharts-0.8.0/ezcharts/data/vendor/echarts.min.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/simple-datatables/simple-datatables.css` & `ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.css`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/data/vendor/simple-datatables/simple-datatables.js` & `ezcharts-0.8.0/ezcharts/data/vendor/simple-datatables/simple-datatables.js`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/demo.py` & `ezcharts-0.8.0/ezcharts/demo.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 from ezcharts.layout.snippets.offcanvas import IOffCanvasClasses, OffCanvas
 from ezcharts.plots import BokehPlot, Plot
 from ezcharts.plots.ideogram import ideogram
 from ezcharts.plots.karyomap import karyomap
 
 
 # Setup simple globals
-WORKFLOW_NAME = 'wf-template2'
+WORKFLOW_NAME = 'wf-template'
+WORKFLOW_VERSION = "v1.0.0"
 REPORT_TITLE = f'{WORKFLOW_NAME}-report'
 
 
 def main(args):
     """Demo for ezCharts functionality."""
     logger = util.get_named_logger("ezChrtDemo")
 
@@ -79,33 +80,53 @@
         elif style == "heatmap":
             # make data a matrix like you would expect for a heatmap
             df = raw_df.set_index([raw_df.columns[0]])
             # set the names of the axes
             df = df.rename_axis("Product")
             df = df.rename_axis("Year", axis=1)
             plot = ezc.heatmap(data=df)
+        elif style == "boxplot":
+            # lets add some data to show off outliers
+            raw_df['2024'] = [10.1, 100.0, 101.1, 99.8]
+            df = pd.melt(raw_df, value_vars=['2015', '2016', '2017', '2024'])
+            plot = ezc.boxplot(
+                df, x="variable", y="value", order=['2024', '2017', '2015', '2016'])
         else:
             raise ValueError("Unknown plot style")
-        plot.title = {"text": f"Example {style} chart"}
+
+        title_text = f"Example {style} chart"
+
+        # adding a title is different for echarts and bokeh
+        if isinstance(plot, BokehPlot):
+            plot._fig.title.text = title_text
+        else:
+            plot.title = {"text": title_text}
+
         return plot
 
     # Then, time to construct a report
     logger.info('Building report')
 
     # Example data
     params = resource_filename('ezcharts', "data/test/params.json")
     versions = resource_filename('ezcharts', "data/test/versions.txt")
     nxt_json = resource_filename('ezcharts', "data/test/nextclade.json")
-    histogram_stats_dir = resource_filename(
-        'ezcharts', "data/test/histogram_stats")
+    histogram_stats_dir = tuple(
+        [
+            resource_filename("ezcharts", "data/test/histogram_stats/sample_1"),
+            resource_filename("ezcharts", "data/test/histogram_stats/sample_2"),
+            resource_filename("ezcharts", "data/test/histogram_stats/empty_sample/"),
+        ]
+    )
 
     # Create report
     # Note we need to add nextclade as a resource
     report = LabsReport(
         REPORT_TITLE, WORKFLOW_NAME, params, versions,
+        workflow_version=WORKFLOW_VERSION,
         head_resources=[*LAB_head_resources, NXTComponent])
 
     # Add a header badge via a method on the report element.
     report.add_badge('Test badge', bg_class="bg-primary")
 
     # Make a progress bar for the median accuracy box
     median_accuracy = Progress(
@@ -128,15 +149,17 @@
                 ('1213986', 'Read count'),
                 (median_accuracy, 'Median accuracy'),
                 ('10213 bp', 'Some other stat')
             ])
 
     # Add sequence summary component
     with report.add_section('Sequence summaries', 'Summaries'):
-        SeqSummary(histogram_stats_dir=histogram_stats_dir)
+        SeqSummary(
+            seq_summary=histogram_stats_dir,
+            sample_names=tuple(['sample_1', 'sample_2', 'sample_3']))
 
     # This also adds to main_content, but provides a nice
     # container snippet as a starting context.
 
     with report.add_section('Controls', 'Controls'):
         # This is an example of how to use bootstrap cards
         Cards(
@@ -213,14 +236,15 @@
             # Grids are snippets that provide responsive
             # layouts via css grid
             with Grid():
                 EZChart(example_plot("line"))
                 EZChart(example_plot("scatter"))
                 EZChart(example_plot("bar"))
                 EZChart(example_plot("histogram"))
+                EZChart(example_plot("boxplot"))
         with tabs.add_tab('Accuracy'):
             p("This is a mixed tab!")
             EZChart(example_plot())
         with tabs.add_tab('Depth'):
             p('Testing, testing, 1 2 3')
 
         # Dropdowns are nested one more level
@@ -233,14 +257,21 @@
                 EZChart(plot)
             with tabs.add_dropdown_tab('Simple - single colour'):
                 # set color=grey for a uniform colouring
                 plot = ezc.barplot(
                     data=example_df, x='year', y='sales', color='grey'
                 )
                 EZChart(plot)
+            with tabs.add_dropdown_tab('Simple - single colour, ignore stacking'):
+                # set color=grey for a uniform colouring
+                # try setting also dodge=False, to check it doesn't break
+                plot = ezc.barplot(
+                    data=example_df, x='year', y='sales', color='grey', dodge=False
+                )
+                EZChart(plot)
             with tabs.add_dropdown_tab('Grouped'):
                 # set dodge=True for a grouped barplot
                 plot = ezc.barplot(
                     data=example_df, x='year', y='sales', hue='product', dodge=True
                 )
                 EZChart(plot)
             with tabs.add_dropdown_tab('Stacked'):
@@ -251,14 +282,17 @@
                 EZChart(plot)
             with tabs.add_dropdown_tab('Nested'):
                 # set nested_x=True for a nested barplot
                 plot = ezc.barplot(
                     data=example_df, x='year', y='sales', hue='product', nested_x=True
                 )
                 EZChart(plot)
+        with tabs.add_tab('Plotting Failed'):
+            # Force fail in plotting
+            EZChart(ezc.sunburst([], label_rotate="tangential", label_minAngle=100))
 
     with report.add_section('Nextclade results', 'Nextclade', True):
         NextClade(nxt_json)
 
     with report.add_section('Heatmap', 'Heatmap'):
         EZChart(example_plot("heatmap"))
 
@@ -311,17 +345,19 @@
         sankey_json = resource_filename('ezcharts', "data/test/sankey.json")
         with open(sankey_json, 'r') as sfh:
             sankey_dict = json.load(sfh)
             ezc.metagenomics_sankey(sankey_dict)
 
     dataset_examples = {
         'fastcat': load_stats(resource_filename(
-            'ezcharts', "data/test/fastcat.stats.gz"), format='fastcat'),
+            'ezcharts',
+            "data/test/fastcat/f1.tsv.gz")),
         'bamstats': load_stats(resource_filename(
-            'ezcharts', "data/test/bamstats.readstats.tsv.gz"), format='bamstats'),
+            'ezcharts',
+            "data/test/bamstats/bamstats.readstats.tsv.gz")),
         'flagstat': load_bamstats_flagstat(resource_filename(
             'ezcharts', "data/test/bamstats.flagstat.tsv")),
         'modkit summary': load_modkit_summary(resource_filename(
             'ezcharts', "data/test/test_modkit_summary.tsv")),
         'modkit bedMethyl': load_bedmethyl(resource_filename(
             'ezcharts', "data/test/test_modkit.bed.gz")),
         'DSS DML': load_dml(resource_filename(
```

### Comparing `ezcharts-0.7.9/ezcharts/layout/base.py` & `ezcharts-0.8.0/ezcharts/layout/base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/resource.py` & `ezcharts-0.8.0/ezcharts/layout/resource.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/__init__.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/__init__.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/banner.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/banner.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/cards.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/cards.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/document.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/document.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/grid.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/grid.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/offcanvas.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/offcanvas.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/progress.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/progress.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/section.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/section.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/stats.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/stats.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/table.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/table.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/snippets/tabs.py` & `ezcharts-0.8.0/ezcharts/layout/snippets/tabs.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/layout/util.py` & `ezcharts-0.8.0/ezcharts/layout/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/__init__.py` & `ezcharts-0.8.0/ezcharts/plots/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -229,14 +229,29 @@
             height=300,
             width=600,
         )
         defaults.update(kwargs)
         self._fig = figure(*args, **defaults)
         # remove Bokeh logo
         self._fig.toolbar.logo = None
+        # axis lines
+        axis_color = "#677884"
+        axis_width = 1.2
+        axis_font = "normal"
+        self._fig.yaxis.axis_line_color = axis_color
+        self._fig.yaxis.axis_line_width = axis_width
+        self._fig.yaxis.axis_label_text_font_style = axis_font
+        self._fig.xaxis.axis_line_color = axis_color
+        self._fig.xaxis.axis_line_width = axis_width
+        self._fig.xaxis.axis_label_text_font_style = axis_font
+
+        self._fig.yaxis.minor_tick_line_color = None
+        self._fig.xaxis.major_tick_line_color = axis_color
+        self._fig.yaxis.major_tick_line_color = axis_color
+        self._fig.title.text_font_size = "18px"
 
     @property
     def logger(self):
         """Return logger for class."""
         return self._logger
```

### Comparing `ezcharts-0.7.9/ezcharts/plots/_base.py` & `ezcharts-0.8.0/ezcharts/plots/_base.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/_model.py` & `ezcharts-0.8.0/ezcharts/plots/_model.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/categorical.py` & `ezcharts-0.8.0/ezcharts/plots/categorical.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Categorical plots."""
+from collections import Counter
 
-from bokeh.models import ColumnDataSource, FactorRange
+from bokeh.models import ColumnDataSource, FactorRange, Whisker
 import bokeh.transform as bkt
 import numpy as np
+import pandas as pd
 from seaborn.categorical import _BarPlotter
 
 from ezcharts.plots import BokehPlot
 
 
 __all__ = [
     "catplot", "stripplot", "swarmplot", "boxplot", "violinplot",
@@ -24,17 +26,118 @@
 
 
 def swarmplot(*args, **kwargs):
     """Draw a categorical scatterplot with non-overlapping points."""
     raise NotImplementedError
 
 
-def boxplot(*args, **kwargs):
+def boxplot(
+        data=None, *, x=None, y=None, hue=None, order=None, hue_order=None,
+        orient=None, color=None, palette=None, saturation=1, fill=True,
+        dodge=None, width=None, gap=None, whis=1.5, linecolor='auto', linewidth=1,
+        fliersize=6, hue_norm=None, native_scale=None, log_scale=None,
+        formatter=None, legend=None, ax=None, **kwargs):
     """Draw a box plot to show distributions with respect to categories."""
-    raise NotImplementedError
+    # deal with stuff we haven't implemented, yet
+    not_implemented = [
+        hue, hue_order, orient, dodge, width, ax, formatter, legend,
+        gap, hue_norm, native_scale, log_scale]
+    for i in not_implemented:
+        if i is not None:
+            raise NotImplementedError(
+                f"The parameter with the value {i} is not yet implemented.")
+
+    # use our default palette if no colour options were provided
+    if palette is None and color is None:
+        palette = BokehPlot.colors
+
+    # we are going to group by our x
+    groups = data[x].unique()
+
+    # compute quantiles
+    qs = data.groupby(x)[y].quantile([0.25, 0.5, 0.75])
+    qs = qs.unstack().reset_index()
+    qs.columns = [x, "q1", "q2", "q3"]
+    df = pd.merge(data, qs, on=x, how="left")
+
+    # if the user specifies an order for their categorical variables
+    if isinstance(order, list):
+        # check to make sure user has included all categorical variables
+        check = Counter(order) == Counter(groups)
+        if check:
+            groups = order
+        else:
+            raise ValueError(
+                f"all categories ({groups}) not present in order ({order})")
+
+    # compute IQR outlier bounds
+    iqr = df.q3 - df.q1
+
+    # whiskers
+    if isinstance(whis, float):
+        df["upper"] = df.q3 + whis * iqr
+        df["lower"] = df.q1 - whis * iqr
+    else:
+        raise NotImplementedError(
+            f"'whis' must be float, {type(whis)} is not supported or implemented")
+
+    source = ColumnDataSource(df)
+
+    # quantile boxes color
+    if not color:
+        color = bkt.factor_cmap(x, palette, groups)
+
+    # use seaborn bits and bobs for color
+    if not fill:
+        color = None
+        linecolor = "black"
+    else:
+        if linecolor == 'auto':
+            linecolor = "black"
+
+    # outlier range
+    whisker = Whisker(
+        base=x, upper="upper", lower="lower", source=source,
+        line_width=linewidth, line_color=linecolor)
+
+    whisker.upper_head.size = whisker.lower_head.size = 20
+
+    # outliers
+    outliers = df[~df[y].between(df.lower, df.upper)]
+
+    # we need to accpount for whskers and outliers in the y-range
+    y_min = df["lower"].min()
+    y_max = df["upper"].max()
+
+    # if there are outliers then we need to take those into account
+    if not outliers.empty:
+        y_min = np.min([outliers[y].min(), df["lower"].min()])
+        y_max = np.max([outliers[y].max(), df["upper"].max()])
+
+    y_range = (1.1 * y_min, 1.1 * y_max)
+
+    plt = BokehPlot(x_range=groups, y_range=y_range)
+    p = plt._fig
+    p.add_layout(whisker)
+
+    p.vbar(
+        x, 0.7, "q2", "q3", source=source, fill_color=color, line_color=linecolor,
+        line_width=linewidth, fill_alpha=saturation)
+
+    p.vbar(
+        x, 0.7, "q1", "q2", source=source, fill_color=color, line_color=linecolor,
+        line_width=linewidth, fill_alpha=saturation)
+
+    p.scatter(x, y, source=outliers, size=fliersize, color="black", alpha=0.5)
+
+    p.xgrid.grid_line_color = None
+    p.xaxis.axis_label = x.capitalize()
+    p.yaxis.axis_label = y.capitalize()
+
+    return plt
 
 
 def violinplot(*args, **kwargs):
     """Draw a combination of boxplot and kernel density estimate."""
     raise NotImplementedError
 
 
@@ -123,18 +226,19 @@
         plt = BokehPlot(x_range=group_names)
     else:
         plt = BokehPlot(y_range=group_names)
 
     p = plt._fig
 
     # Define plot orientation
+    # If both hue and dodge=False are provided, make a stacked bar chart
     if plotter.orient == "v":
-        plot_bars_func = p.vbar if dodge else p.vbar_stack
+        plot_bars_func = p.vbar_stack if not dodge and hue else p.vbar
     else:
-        plot_bars_func = p.hbar if dodge else p.hbar_stack
+        plot_bars_func = p.hbar_stack if not dodge and hue else p.hbar
 
     if plotter.plot_hues is None:
         # simple barplot (i.e. only a single group of bars)
         if plotter.orient == "v":
             plot_bars_func(
                 x=group_names,
                 top=plotter.statistic,
@@ -233,13 +337,17 @@
     if plotter.orient == "v":
         p.xgrid.grid_line_color = None
         p.y_range.start = 0
     else:
         p.ygrid.grid_line_color = None
         p.x_range.start = 0
 
+    if not nested_x:
+        p.xaxis.axis_label = x.capitalize()
+        p.yaxis.axis_label = y.capitalize()
+
     return plt
 
 
 def countplot(*args, **kwargs):
     """Show the counts of observations in each categorical bin using bars."""
     raise NotImplementedError
```

### Comparing `ezcharts-0.7.9/ezcharts/plots/demo.py` & `ezcharts-0.8.0/ezcharts/plots/demo.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/distribution.py` & `ezcharts-0.8.0/ezcharts/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/ideogram.py` & `ezcharts-0.8.0/ezcharts/plots/ideogram.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/karyomap.py` & `ezcharts-0.8.0/ezcharts/plots/karyomap.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/matrix.py` & `ezcharts-0.8.0/ezcharts/plots/matrix.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/metagenomics_sankey.py` & `ezcharts-0.8.0/ezcharts/plots/metagenomics_sankey.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/relational.py` & `ezcharts-0.8.0/ezcharts/plots/relational.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts/plots/sunburst.py` & `ezcharts-0.8.0/ezcharts/plots/sunburst.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from ezcharts.plots import _NoAxisFixPlot, util
 
 
 __all__ = ["sunburst"]
 
 
+@util.plot_wrapper
 def sunburst(
     data, tooltip=True, visualMap=True, min_value=0, max_value=None,
     color_scale=None, label_rotate="radial", label_minAngle=0, show_label=True
 ):
     """Create sunburst plot.
 
     :param data (list): List of nested dictionaries of the following structure:
```

### Comparing `ezcharts-0.7.9/ezcharts/util.py` & `ezcharts-0.8.0/ezcharts/util.py`

 * *Files identical despite different names*

### Comparing `ezcharts-0.7.9/ezcharts.egg-info/PKG-INFO` & `ezcharts-0.8.0/ezcharts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezcharts
-Version: 0.7.9
+Version: 0.8.0
 Summary: eCharts plotting API.
 Home-page: https://github.com/epi2me-labs/ezcharts
 Author: cwright
 Author-email: cwright@nanoporetech.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bokeh~=3.1.0
@@ -218,14 +218,17 @@
 
 report.write("tmp.html")
 ```
 
 Note that `EZChart()` is required to add the plot to the enclosing `dominate`
 context.
 
+### Debug mode
+Decorator for plotting a message when the plot fails can be skipped by setting the env variable EZCHARTS_DEBUG=1.
+
 **Components**
 
 Components provide higher level application-specific layouts (a table for
 [Nextclade](https://clades.nextstrain.org/) results, for instance) that may also
 include charts and light data processing capabilities (e.g. to parse and
 visualise [fastcat](https://github.com/epi2me-labs/fastcat) output).
```

### Comparing `ezcharts-0.7.9/setup.py` & `ezcharts-0.8.0/setup.py`

 * *Files identical despite different names*

