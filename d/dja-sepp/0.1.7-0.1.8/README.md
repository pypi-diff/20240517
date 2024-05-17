# Comparing `tmp/dja_sepp-0.1.7.tar.gz` & `tmp/dja_sepp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dja_sepp-0.1.7.tar", last modified: Fri May 17 09:42:03 2024, max compression
+gzip compressed data, was "dja_sepp-0.1.8.tar", last modified: Fri May 17 11:49:01 2024, max compression
```

## Comparing `dja_sepp-0.1.7.tar` & `dja_sepp-0.1.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:42:03.077803 dja_sepp-0.1.7/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.7/LICENSE
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:42:03.075255 dja_sepp-0.1.7/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1640 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/README.md
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      809 2024-05-17 09:41:49.000000 dja_sepp-0.1.7/pyproject.toml
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 09:42:03.078823 dja_sepp-0.1.7/setup.cfg
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:42:02.739157 dja_sepp-0.1.7/src/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:42:02.758192 dja_sepp-0.1.7/src/dja_sepp/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.7/src/dja_sepp/__init__.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:42:02.739733 dja_sepp-0.1.7/src/dja_sepp/data/
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:42:03.071456 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12002 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12704 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14806 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11987 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    49028 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18124 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18921 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8303 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13861 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    10113 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    23209 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15354 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8036 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11604 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    34304 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    17928 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    47252 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5323 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    24254 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    31613 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    25376 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5181 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22508 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13854 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    37987 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    19362 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6616 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6628 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15109 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4076 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4778 2024-05-16 12:32:24.000000 dja_sepp-0.1.7/src/dja_sepp/psfex.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.7/src/dja_sepp/s3.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9073 2024-05-17 08:36:10.000000 dja_sepp-0.1.7/src/dja_sepp/sepp.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22764 2024-05-17 07:41:45.000000 dja_sepp-0.1.7/src/dja_sepp/sextractor.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.7/src/dja_sepp/tiles.py
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.7/src/dja_sepp/utils.py
-drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 09:42:03.073744 dja_sepp-0.1.7/src/dja_sepp.egg-info/
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2306 2024-05-17 09:42:02.000000 dja_sepp-0.1.7/src/dja_sepp.egg-info/PKG-INFO
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2680 2024-05-17 09:42:02.000000 dja_sepp-0.1.7/src/dja_sepp.egg-info/SOURCES.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 09:42:02.000000 dja_sepp-0.1.7/src/dja_sepp.egg-info/dependency_links.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 09:42:02.000000 dja_sepp-0.1.7/src/dja_sepp.egg-info/requires.txt
--rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 09:42:02.000000 dja_sepp-0.1.7/src/dja_sepp.egg-info/top_level.txt
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.275007 dja_sepp-0.1.8/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1071 2024-05-16 12:43:35.000000 dja_sepp-0.1.8/LICENSE
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2546 2024-05-17 11:49:01.272786 dja_sepp-0.1.8/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     1880 2024-05-17 10:56:47.000000 dja_sepp-0.1.8/README.md
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      809 2024-05-17 11:48:29.000000 dja_sepp-0.1.8/pyproject.toml
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       38 2024-05-17 11:49:01.275667 dja_sepp-0.1.8/setup.cfg
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.114853 dja_sepp-0.1.8/src/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.144599 dja_sepp-0.1.8/src/dja_sepp/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)      656 2024-05-17 08:37:29.000000 dja_sepp-0.1.8/src/dja_sepp/__init__.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.118365 dja_sepp-0.1.8/src/dja_sepp/data/
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.267103 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12002 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    12704 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14806 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11987 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    49028 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18124 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    18921 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8303 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13861 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    10113 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    23209 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15354 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     8036 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    11604 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    34304 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    17928 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    47252 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5323 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    24254 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    31613 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    25376 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     5181 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    22508 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    13854 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    37987 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    19362 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6616 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6628 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    15109 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4076 2024-05-16 12:32:24.000000 dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     4856 2024-05-17 11:48:01.000000 dja_sepp-0.1.8/src/dja_sepp/psfex.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     3563 2024-05-17 08:10:03.000000 dja_sepp-0.1.8/src/dja_sepp/s3.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     9372 2024-05-17 11:47:30.000000 dja_sepp-0.1.8/src/dja_sepp/sepp.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    23244 2024-05-17 11:46:36.000000 dja_sepp-0.1.8/src/dja_sepp/sextractor.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     6936 2024-05-17 08:36:35.000000 dja_sepp-0.1.8/src/dja_sepp/tiles.py
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)    14100 2024-05-17 09:21:37.000000 dja_sepp-0.1.8/src/dja_sepp/utils.py
+drwxr-xr-x   0 aurelien  (1000) aurelien  (1000)        0 2024-05-17 11:49:01.269774 dja_sepp-0.1.8/src/dja_sepp.egg-info/
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2546 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/PKG-INFO
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)     2680 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/SOURCES.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        1 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/dependency_links.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)       51 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/requires.txt
+-rw-r--r--   0 aurelien  (1000) aurelien  (1000)        9 2024-05-17 11:49:01.000000 dja_sepp-0.1.8/src/dja_sepp.egg-info/top_level.txt
```

### Comparing `dja_sepp-0.1.7/LICENSE` & `dja_sepp-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/PKG-INFO` & `dja_sepp-0.1.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,35 @@
-Metadata-Version: 2.1
-Name: dja_sepp
-Version: 0.1.7
-Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
-Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
-Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
-Project-URL: DJA, https://dawn-cph.github.io/dja/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: awscli
-Requires-Dist: boto3
-Requires-Dist: numpy
-Requires-Dist: matplotlib
-Requires-Dist: astropy
-Requires-Dist: scikit-learn
-
 # DJA x SourceXtractor++
 
 ## Introduction
 
 This project looks into implementing SourceXtractor++ on the [DAWN JWST Archive](https://dawn-cph.github.io/dja/) (DJA). The DJA is a repository of public JWST galaxy data reduced and ready for science. This project aims at expanding the DJA with model fitting and more precise measurements on the different sets of photometric images.
 
+[![PyPI - Version](https://img.shields.io/pypi/v/dja_sepp)](https://pypi.org/project/dja-sepp/)
+
+
+## Installation
+
+This code can be installed via PyPI: ```pip install dja_sepp --upgrade```
+
 ## Usage
 
-0. *(optional)* Cutouts in the image : [`00.2_Cutout.ipynb`](00.2_Cutout.ipynb)
-1. Detect point-like sources with the F200W band + create the PSF for every band : [`03.1_SingleBand-PSF.ipynb`](03.1_SingleBand-PSF.ipynb)
-2. Run SourceXtractor++ in detection mode : [`04_SE++.ipynb`](04_SE++.ipynb)
-3. Compare the results to the DJA : [`06_Validation.ipynb`](06_Validation.ipynb)
-4. View and analyse the results : [`05_Analysis.ipynb`](05_Analysis.ipynb)
+0. *(optional)* Cutouts in the image : [`00.2_Cutout.ipynb`](notebooks/00.2_Cutout.ipynb)
+1. Detect point-like sources with the F200W band + create the PSF for every band : [`03.1_SingleBand-PSF.ipynb`](notebooks/03.1_SingleBand-PSF.ipynb)
+2. Run SourceXtractor++ in detection mode : [`04_SE++.ipynb`](notebooks/04_SE++.ipynb)
+3. Compare the results to the DJA : [`06_Validation.ipynb`](notebooks/06_Validation.ipynb)
+4. View and analyse the results : [`05_Analysis.ipynb`](notebooks/05_Analysis.ipynb)
 
 ## Dependencies
 
 * [SExtractor](https://www.astromatic.net/software/sextractor/)
 * [PSFEx](https://www.astromatic.net/software/psfex/)
 * [SourceXtractor++](https://github.com/astrorama/SourceXtractorPlusPlus)
 * [Astropy](https://www.astropy.org/index.html)
 
 ## Utilization with AWS EC2
 
 One of the goal of this project is also to run SourceXtractor++ on [AWS EC2](https://aws.amazon.com/ec2/) to make it run in the background and faster than on your personal computer. 
 
 A benchmark is currently being run to find how to set the parameters in SE++ and AWS EC2 to minimize runtime depending on the size of your images and the number of bands wanted.
 
-To know how to use easily AWS EC2 in combination with Jupyter, please refer to [this series of tutorial](https://github.com/AstroAure/VSJupytEC2).
+To know how to use easily AWS EC2 in combination with Jupyter, please refer to [this series of tutorial](https://github.com/AstroAure/VSJupytEC2).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dja_sepp-0.1.7/pyproject.toml` & `dja_sepp-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dja_sepp"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
     {name="Aurélien Genin", email="aurelien.genin@polytechnique.org"}
 ]
 description = "Package to run SourceXtractor++ on the DAWN JWST Archive"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dja_sepp-0.1.7/src/dja_sepp/__init__.py` & `dja_sepp-0.1.8/src/dja_sepp/__init__.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F070W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F090W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F115W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F140M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W2_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F150W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F162M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F164N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F182M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F187N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F200W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F210M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F212N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F250M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F277W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F300M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F322W2_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F323N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F335M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F356W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F360M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F405N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F410M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F430M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F444W_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F460M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F466N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F470N_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/F480M_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt` & `dja_sepp-0.1.8/src/dja_sepp/data/NIRCam_Filters-Throughput/WLP4_mean_system_throughput.txt`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/psfex.py` & `dja_sepp-0.1.8/src/dja_sepp/psfex.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import subprocess
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib.colors import SymLogNorm
 from astropy.io import fits
 
 # To work, this file requires you to have PSFEx installed on your machine.
 
@@ -27,23 +28,24 @@
     verbose : verbose parameter
     """
     os.makedirs(dir_chckimg, exist_ok=True)
     os.makedirs(dir_psfex, exist_ok=True)
     study_name = ".".join(cat_name.split("/")[-1].split(".")[:-1])
     output_chk = f"{dir_chckimg}/{study_name}"
     verbose_type = 'NORMAL' if verbose else 'QUIET'
-    os.system(f'psfex {cat_name} -c {config_file} \
-                -CHECKIMAGE_NAME {dir_chckimg}/chi2.fits,{dir_chckimg}/samp.fits,{dir_chckimg}/res.fits,{dir_chckimg}/snap.fits \
-                -CHECKPLOT_NAME {output_chk}_selfwhm,{output_chk}_chi2,{output_chk}_counts \
-                -XML_NAME {output_chk}_xml.xml \
-                -OUTCAT_NAME {output_cat}_psf_cat.fits \
-                -PSF_DIR {dir_psfex} \
-                -SAMPLE_FWHMRANGE "{fwhm_range}" \
-                -SAMPLE_MINSN {min_snr} \
-                -VERBOSE_TYPE {verbose_type}')
+    subprocess.run(f'psfex {cat_name} -c {config_file} \
+                   -CHECKIMAGE_NAME {dir_chckimg}/chi2.fits,{dir_chckimg}/samp.fits,{dir_chckimg}/res.fits,{dir_chckimg}/snap.fits \
+                   -CHECKPLOT_NAME {output_chk}_selfwhm,{output_chk}_chi2,{output_chk}_counts \
+                   -XML_NAME {output_chk}_xml.xml \
+                   -OUTCAT_NAME {output_cat}_psf_cat.fits \
+                   -PSF_DIR {dir_psfex} \
+                   -SAMPLE_FWHMRANGE "{fwhm_range}" \
+                   -SAMPLE_MINSN {min_snr} \
+                   -VERBOSE_TYPE {verbose_type}',
+                   shell=True)
     filename = f"{dir_psfex}/{study_name}_psf.psf"
     if save_psf_png:
         image = fits.open(filename)
         psf = image[1].data[0][0][0]
         image.close()
         fig, ax = plt.subplots(figsize=(6,6))
         ax.set_axis_off()
```

### Comparing `dja_sepp-0.1.7/src/dja_sepp/s3.py` & `dja_sepp-0.1.8/src/dja_sepp/s3.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/sepp.py` & `dja_sepp-0.1.8/src/dja_sepp/sepp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import subprocess
 import glob
 import re
 import sys
 import boto3
 from astropy.io import fits
 import numpy as np
 from . import utils
@@ -81,50 +82,51 @@
             'list_of_PSF_names' : psfs
             }
     os.makedirs(checkimg_path, exist_ok=True)
     os.environ['MKL_NUM_THREADS'] = '1'
     os.environ['MKL_DYNAMIC'] = 'FALSE'
     os.environ['OMP_NUM_THREADS'] = '1'
     os.environ['OMP_DYNAMIC'] = 'FALSE'
-    os.system(f"sourcextractor++ \
-            --python-config-file {python_config} \
-            --python-arg '{args}' \
-            --output-catalog-filename {output_catname} \
-            --output-properties {properties} \
-            --output-flush-size 10 \
-            --detection-image {detect_img} \
-            --weight-type WEIGHT \
-            --weight-absolute 0 \
-            --segmentation-filter {filt} \
-            --background-cell-size 128 \
-            --segmentation-algorithm LUTZ \
-            --smoothing-box-size 5 \
-            --detection-threshold 0.80 \
-            --detection-minimum-area 7 \
-            --partition-corethreshold yes \
-            --core-threshold-value 1.5 \
-            --core-minimum-area 9 \
-            --grouping-algorithm split \
-            --partition-multithreshold yes \
-            --partition-minimum-area 18 \
-            --grouping-hard-limit 0 \
-            --partition-minimum-contrast 0.0001 \
-            --partition-threshold-count 42 \
-            --use-cleaning yes \
-            --cleaning-minimum-area 15 \
-            --model-fitting-iterations 550 \
-            --sampling-scale-factor 1 \
-            --check-image-model-fitting {checkimg_path}/model.fits \
-            --check-image-residual {checkimg_path}/resid.fits \
-            --log-file {output_catname.replace('.fits', '.log')} \
-            --log-level DEBUG \
-            --thread-count {thread_count} \
-            --tile-memory-limit {tile_memory_limit} \
-            --tile-size {tile_size} \
-            ")
+    subprocess.run(f"sourcextractor++ \
+                   --python-config-file {python_config} \
+                   --python-arg '{args}' \
+                   --output-catalog-filename {output_catname} \
+                   --output-properties {properties} \
+                   --output-flush-size 10 \
+                   --detection-image {detect_img} \
+                   --weight-type WEIGHT \
+                   --weight-absolute 0 \
+                   --segmentation-filter {filt} \
+                   --background-cell-size 128 \
+                   --segmentation-algorithm LUTZ \
+                   --smoothing-box-size 5 \
+                   --detection-threshold 0.80 \
+                   --detection-minimum-area 7 \
+                   --partition-corethreshold yes \
+                   --core-threshold-value 1.5 \
+                   --core-minimum-area 9 \
+                   --grouping-algorithm split \
+                   --partition-multithreshold yes \
+                   --partition-minimum-area 18 \
+                   --grouping-hard-limit 0 \
+                   --partition-minimum-contrast 0.0001 \
+                   --partition-threshold-count 42 \
+                   --use-cleaning yes \
+                   --cleaning-minimum-area 15 \
+                   --model-fitting-iterations 550 \
+                   --sampling-scale-factor 1 \
+                   --check-image-model-fitting {checkimg_path}/model.fits \
+                   --check-image-residual {checkimg_path}/resid.fits \
+                   --log-file {output_catname.replace('.fits', '.log')} \
+                   --log-level DEBUG \
+                   --thread-count {thread_count} \
+                   --tile-memory-limit {tile_memory_limit} \
+                   --tile-size {tile_size} \
+                   ",
+                   shell=True)
 
 def main_tile(tile, img_dir, sepp_dir, psf_dir, config_dir):
     # Python configuration file for SE++
     python_config=f'{config_dir}/sepp-config.py'
     # Detection image
     detect_img=glob.glob(f'{img_dir}/*ir*sci*-{tile}.fits')[0]
     # Filter to use on the detection image
```

### Comparing `dja_sepp-0.1.7/src/dja_sepp/sextractor.py` & `dja_sepp-0.1.8/src/dja_sepp/sextractor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
+import subprocess
 import glob
 from astropy.io import fits
 from astropy.coordinates import SkyCoord
 import astropy.units as u
 from astropy.table import Table
 import numpy as np
 import matplotlib.pyplot as plt
 from matplotlib import colormaps
 from matplotlib.colors import SymLogNorm
 from matplotlib.patches import Rectangle
 import random as rd
 from sklearn.cluster import DBSCAN
 from sklearn.linear_model import RANSACRegressor
 
-
 # To work, this file requires you to have SExtractor installed on your machine.
 
 def run_sextractor(detect_img      : str, weight_img   : str, 
                    output_cat      : str, 
                    config_file     : str, params_file  : str,
                    dir_chckimg     : str,
                    detect_thresh   : float = 12.0,
@@ -32,28 +32,36 @@
     config_file : filename of the SExtractor configuration file
     params_file : filename of the SExtarctor parameters file
     dir_chckimg : path to folder to save checkimages (will be created if non-existing)
     detect_thresh : value of the DETECT_THRESH to use
     analysis_thresh : value of the ANALYSIS_THRESH to use
     verbose : verbose parameter
     """
+    # Find SExtractor installed version
+    cmd = ""
+    if subprocess.run('sex --version', shell=True, capture_output=True).returncode==0: cmd = "sex"
+    elif subprocess.run('source-extractor --version', shell=True, capture_output=True).returncode==0: cmd = "source-extractor"
+    else:
+        print("SExtractor not found ! Make sure it is installed.")
+        return None
     os.makedirs("/".join(output_cat.split("/")[:-1]), exist_ok=True)
     os.makedirs(dir_chckimg, exist_ok=True)
     study_name = '.'.join(detect_img.split('/')[-1].split('.')[:-1])
     seg_img = f'{dir_chckimg}/{study_name}_seg.fits'
     verbose_type = 'NORMAL' if verbose else 'QUIET'
     os.environ['LD_LIBRARY_PATH'] = '/usr/lib' # Link 'libcfitsio.so.10'
-    os.system(f'sex {detect_img} -c {config_file} \
-            -CATALOG_NAME {output_cat} \
-            -WEIGHT_IMAGE {weight_img} -WEIGHT_TYPE MAP_WEIGHT \
-            -PARAMETERS_NAME {params_file} \
-            -CHECKIMAGE_NAME {seg_img} \
-            -DETECT_THRESH {detect_thresh} \
-            -ANALYSIS_THRESH {analysis_thresh} \
-            -VERBOSE_TYPE {verbose_type}')
+    subprocess.run(f'{cmd} {detect_img} -c {config_file} \
+                   -CATALOG_NAME {output_cat} \
+                   -WEIGHT_IMAGE {weight_img} -WEIGHT_TYPE MAP_WEIGHT \
+                   -PARAMETERS_NAME {params_file} \
+                   -CHECKIMAGE_NAME {seg_img} \
+                   -DETECT_THRESH {detect_thresh} \
+                   -ANALYSIS_THRESH {analysis_thresh} \
+                   -VERBOSE_TYPE {verbose_type}',
+                   shell=True)
     return output_cat
     
 def show_vignets(data, grid_n):
     """
     Display random vignets from a SExtractor catalog
 
     data : data contained in the SExtractor catalog.
```

### Comparing `dja_sepp-0.1.7/src/dja_sepp/tiles.py` & `dja_sepp-0.1.8/src/dja_sepp/tiles.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp/utils.py` & `dja_sepp-0.1.8/src/dja_sepp/utils.py`

 * *Files identical despite different names*

### Comparing `dja_sepp-0.1.7/src/dja_sepp.egg-info/PKG-INFO` & `dja_sepp-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dja_sepp
-Version: 0.1.7
+Version: 0.1.8
 Summary: Package to run SourceXtractor++ on the DAWN JWST Archive
 Author-email: Aurélien Genin <aurelien.genin@polytechnique.org>
 Project-URL: Source, https://github.com/AstroAure/DJA-SEpp
 Project-URL: DJA, https://dawn-cph.github.io/dja/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,21 +20,28 @@
 
 # DJA x SourceXtractor++
 
 ## Introduction
 
 This project looks into implementing SourceXtractor++ on the [DAWN JWST Archive](https://dawn-cph.github.io/dja/) (DJA). The DJA is a repository of public JWST galaxy data reduced and ready for science. This project aims at expanding the DJA with model fitting and more precise measurements on the different sets of photometric images.
 
+[![PyPI - Version](https://img.shields.io/pypi/v/dja_sepp)](https://pypi.org/project/dja-sepp/)
+
+
+## Installation
+
+This code can be installed via PyPI: ```pip install dja_sepp --upgrade```
+
 ## Usage
 
-0. *(optional)* Cutouts in the image : [`00.2_Cutout.ipynb`](00.2_Cutout.ipynb)
-1. Detect point-like sources with the F200W band + create the PSF for every band : [`03.1_SingleBand-PSF.ipynb`](03.1_SingleBand-PSF.ipynb)
-2. Run SourceXtractor++ in detection mode : [`04_SE++.ipynb`](04_SE++.ipynb)
-3. Compare the results to the DJA : [`06_Validation.ipynb`](06_Validation.ipynb)
-4. View and analyse the results : [`05_Analysis.ipynb`](05_Analysis.ipynb)
+0. *(optional)* Cutouts in the image : [`00.2_Cutout.ipynb`](notebooks/00.2_Cutout.ipynb)
+1. Detect point-like sources with the F200W band + create the PSF for every band : [`03.1_SingleBand-PSF.ipynb`](notebooks/03.1_SingleBand-PSF.ipynb)
+2. Run SourceXtractor++ in detection mode : [`04_SE++.ipynb`](notebooks/04_SE++.ipynb)
+3. Compare the results to the DJA : [`06_Validation.ipynb`](notebooks/06_Validation.ipynb)
+4. View and analyse the results : [`05_Analysis.ipynb`](notebooks/05_Analysis.ipynb)
 
 ## Dependencies
 
 * [SExtractor](https://www.astromatic.net/software/sextractor/)
 * [PSFEx](https://www.astromatic.net/software/psfex/)
 * [SourceXtractor++](https://github.com/astrorama/SourceXtractorPlusPlus)
 * [Astropy](https://www.astropy.org/index.html)
```

### Comparing `dja_sepp-0.1.7/src/dja_sepp.egg-info/SOURCES.txt` & `dja_sepp-0.1.8/src/dja_sepp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

