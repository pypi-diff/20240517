# Comparing `tmp/pylibs_ocean-1.0.0.tar.gz` & `tmp/pylibs_ocean-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibs_ocean-1.0.0.tar", last modified: Fri Jan 19 22:40:26 2024, max compression
+gzip compressed data, was "pylibs_ocean-1.0.1.tar", last modified: Fri May 17 19:59:05 2024, max compression
```

## Comparing `pylibs_ocean-1.0.0.tar` & `pylibs_ocean-1.0.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-01-19 22:40:26.015060 pylibs_ocean-1.0.0/
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)    11342 2022-12-02 23:28:43.000000 pylibs_ocean-1.0.0/LICENSE
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      482 2024-01-19 22:40:26.017060 pylibs_ocean-1.0.0/PKG-INFO
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1149 2024-01-19 22:34:24.000000 pylibs_ocean-1.0.0/README.md
-drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-01-19 22:40:23.414136 pylibs_ocean-1.0.0/pyScripts/
-drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-01-19 22:40:24.133115 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)      680 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/compile.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)    16205 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/nrutil.c
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     3330 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/nrutil.h
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)       99 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/readme.txt
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     4430 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/tidal_analysis.c
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)    22928 2022-08-22 20:54:50.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/tidal_analyze
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      138 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/tidal_const.dat
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     2470 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/tide_fac_const.npz
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)        0 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/__init__.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     2292 2022-08-17 14:08:04.000000 pylibs_ocean-1.0.0/pyScripts/change_ssh_hotstart.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1150 2022-08-16 19:51:43.000000 pylibs_ocean-1.0.0/pyScripts/download_AVISO.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     4517 2023-08-18 19:09:10.000000 pylibs_ocean-1.0.0/pyScripts/download_CMEMS.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      846 2023-05-19 18:52:26.000000 pylibs_ocean-1.0.0/pyScripts/download_HFRadar.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     2248 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/download_hycom.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     6141 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/gen_bctides.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     1476 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/gen_fluxflag.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1637 2023-04-03 21:21:21.000000 pylibs_ocean-1.0.0/pyScripts/gen_fluxth_USGS.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     9239 2023-03-15 01:31:54.000000 pylibs_ocean-1.0.0/pyScripts/gen_hycom_3Dth_nudge.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     5048 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/gen_hycom_hotstart.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     3652 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/gen_narr_sflux.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     4754 2022-08-25 18:55:27.000000 pylibs_ocean-1.0.0/pyScripts/gen_shapiro.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     4116 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/gen_vqs.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)    28148 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/hotstart_proc.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     1397 2022-09-20 16:21:52.000000 pylibs_ocean-1.0.0/pyScripts/make_sflux_links.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     3661 2023-01-10 04:10:47.000000 pylibs_ocean-1.0.0/pyScripts/make_sflux_subdomain.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)    10836 2022-08-16 18:34:49.000000 pylibs_ocean-1.0.0/pyScripts/pextract_OLDIO_schism_fabm_xyz.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     6511 2022-05-24 20:35:00.000000 pylibs_ocean-1.0.0/pyScripts/pextract_OLDIO_schism_tide.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     5770 2024-01-16 20:15:53.000000 pylibs_ocean-1.0.0/pyScripts/pextract_schism.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     6809 2024-01-16 20:17:57.000000 pylibs_ocean-1.0.0/pyScripts/pextract_schism_flux.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     4751 2023-08-08 16:48:03.000000 pylibs_ocean-1.0.0/pyScripts/pextract_schism_slab.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     7264 2023-08-08 16:47:54.000000 pylibs_ocean-1.0.0/pyScripts/pload_depth.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)    36837 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/prj.npz
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     4053 2023-08-08 16:48:18.000000 pylibs_ocean-1.0.0/pyScripts/pschism_output_subset.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     2810 2023-08-08 16:48:23.000000 pylibs_ocean-1.0.0/pyScripts/run_mpi_template.py
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)      124 2023-09-01 21:03:58.000000 pylibs_ocean-1.0.0/pyScripts/schismcheck
--rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)      123 2023-03-14 19:25:27.000000 pylibs_ocean-1.0.0/pyScripts/schismview
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     3318 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyScripts/sflux_template.npz
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     5751 2023-05-19 18:52:26.000000 pylibs_ocean-1.0.0/pyScripts/subset_outputs_parallel.py
-drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-01-19 22:40:24.188114 pylibs_ocean-1.0.0/pyUtility/
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)        0 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.0/pyUtility/__init__.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)   105309 2023-12-11 22:13:09.000000 pylibs_ocean-1.0.0/pyUtility/mylib.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)   208749 2024-01-19 21:51:52.000000 pylibs_ocean-1.0.0/pyUtility/schism_file.py
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     5742 2024-01-19 21:51:52.000000 pylibs_ocean-1.0.0/pylib.py
-drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-01-19 22:40:25.221083 pylibs_ocean-1.0.0/pylibs_ocean.egg-info/
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      482 2024-01-19 22:40:18.000000 pylibs_ocean-1.0.0/pylibs_ocean.egg-info/PKG-INFO
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1498 2024-01-19 22:40:18.000000 pylibs_ocean-1.0.0/pylibs_ocean.egg-info/SOURCES.txt
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)        1 2024-01-19 22:40:18.000000 pylibs_ocean-1.0.0/pylibs_ocean.egg-info/dependency_links.txt
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      191 2024-01-19 22:40:18.000000 pylibs_ocean-1.0.0/pylibs_ocean.egg-info/requires.txt
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)       26 2024-01-19 22:40:18.000000 pylibs_ocean-1.0.0/pylibs_ocean.egg-info/top_level.txt
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)       79 2024-01-19 22:40:26.046059 pylibs_ocean-1.0.0/setup.cfg
--rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1217 2024-01-19 22:34:24.000000 pylibs_ocean-1.0.0/setup.py
+drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-05-17 19:59:05.130622 pylibs_ocean-1.0.1/
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)    11342 2022-12-02 23:28:43.000000 pylibs_ocean-1.0.1/LICENSE
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      482 2024-05-17 19:59:05.130622 pylibs_ocean-1.0.1/PKG-INFO
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1149 2024-01-19 22:34:24.000000 pylibs_ocean-1.0.1/README.md
+drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-05-17 19:59:04.950626 pylibs_ocean-1.0.1/pyScripts/
+drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-05-17 19:59:05.053624 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)      680 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/compile.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)    16205 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/nrutil.c
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     3330 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/nrutil.h
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)       99 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/readme.txt
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     4430 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/tidal_analysis.c
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)    22928 2022-08-22 20:54:50.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/tidal_analyze
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      138 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/tidal_const.dat
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     2470 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/tide_fac_const.npz
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)        0 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/__init__.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     2292 2022-08-17 14:08:04.000000 pylibs_ocean-1.0.1/pyScripts/change_ssh_hotstart.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1150 2022-08-16 19:51:43.000000 pylibs_ocean-1.0.1/pyScripts/download_AVISO.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     4517 2023-08-18 19:09:10.000000 pylibs_ocean-1.0.1/pyScripts/download_CMEMS.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      846 2023-05-19 18:52:26.000000 pylibs_ocean-1.0.1/pyScripts/download_HFRadar.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     2248 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/download_hycom.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     6141 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/gen_bctides.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     1476 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/gen_fluxflag.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1637 2023-04-03 21:21:21.000000 pylibs_ocean-1.0.1/pyScripts/gen_fluxth_USGS.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     9239 2023-03-15 01:31:54.000000 pylibs_ocean-1.0.1/pyScripts/gen_hycom_3Dth_nudge.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     5048 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/gen_hycom_hotstart.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     3652 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/gen_narr_sflux.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     4754 2022-08-25 18:55:27.000000 pylibs_ocean-1.0.1/pyScripts/gen_shapiro.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     4116 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/gen_vqs.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)    28148 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/hotstart_proc.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     1397 2022-09-20 16:21:52.000000 pylibs_ocean-1.0.1/pyScripts/make_sflux_links.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     2241 2024-04-17 19:44:11.000000 pylibs_ocean-1.0.1/pyScripts/make_sflux_subdomain.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)    10677 2024-01-29 04:40:24.000000 pylibs_ocean-1.0.1/pyScripts/pextract_OLDIO_schism_fabm_xyz.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     6511 2022-05-24 20:35:00.000000 pylibs_ocean-1.0.1/pyScripts/pextract_OLDIO_schism_tide.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     5659 2024-02-15 15:59:35.000000 pylibs_ocean-1.0.1/pyScripts/pextract_schism.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     6592 2024-01-29 04:39:07.000000 pylibs_ocean-1.0.1/pyScripts/pextract_schism_flux.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     4668 2024-02-15 21:34:32.000000 pylibs_ocean-1.0.1/pyScripts/pextract_schism_slab.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     7026 2024-01-29 04:42:47.000000 pylibs_ocean-1.0.1/pyScripts/pload_depth.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)   227571 2024-04-30 23:15:35.000000 pylibs_ocean-1.0.1/pyScripts/prj.npz
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     3812 2024-01-29 04:43:46.000000 pylibs_ocean-1.0.1/pyScripts/pschism_output_subset.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)     2548 2024-01-29 04:37:48.000000 pylibs_ocean-1.0.1/pyScripts/run_mpi_template.py
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)      124 2023-09-01 21:03:58.000000 pylibs_ocean-1.0.1/pyScripts/schismcheck
+-rwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)      123 2023-03-14 19:25:27.000000 pylibs_ocean-1.0.1/pyScripts/schismview
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     3318 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyScripts/sflux_template.npz
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     5751 2023-05-19 18:52:26.000000 pylibs_ocean-1.0.1/pyScripts/subset_outputs_parallel.py
+drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-05-17 19:59:05.090623 pylibs_ocean-1.0.1/pyUtility/
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)        0 2022-05-24 20:11:17.000000 pylibs_ocean-1.0.1/pyUtility/__init__.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)   113418 2024-05-01 14:12:40.000000 pylibs_ocean-1.0.1/pyUtility/mylib.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)   219776 2024-04-26 15:41:12.000000 pylibs_ocean-1.0.1/pyUtility/schism_file.py
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     6011 2024-04-29 21:27:32.000000 pylibs_ocean-1.0.1/pylib.py
+drwxr-xr-x   0 wangzg   (49925) vimsyz    (1513)        0 2024-05-17 19:59:05.124622 pylibs_ocean-1.0.1/pylibs_ocean.egg-info/
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      482 2024-05-17 19:59:03.000000 pylibs_ocean-1.0.1/pylibs_ocean.egg-info/PKG-INFO
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1498 2024-05-17 19:59:03.000000 pylibs_ocean-1.0.1/pylibs_ocean.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)        1 2024-05-17 19:59:03.000000 pylibs_ocean-1.0.1/pylibs_ocean.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)      191 2024-05-17 19:59:03.000000 pylibs_ocean-1.0.1/pylibs_ocean.egg-info/requires.txt
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)       26 2024-05-17 19:59:03.000000 pylibs_ocean-1.0.1/pylibs_ocean.egg-info/top_level.txt
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)       79 2024-05-17 19:59:05.132621 pylibs_ocean-1.0.1/setup.cfg
+-rw-r--r--   0 wangzg   (49925) vimsyz    (1513)     1217 2024-05-17 19:57:55.000000 pylibs_ocean-1.0.1/setup.py
```

### Comparing `pylibs_ocean-1.0.0/LICENSE` & `pylibs_ocean-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/README.md` & `pylibs_ocean-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/compile.py` & `pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/compile.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/nrutil.c` & `pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/nrutil.c`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/nrutil.h` & `pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/nrutil.h`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/tidal_analysis.c` & `pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/tidal_analysis.c`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/tidal_analyze` & `pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/tidal_analyze`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/Harmonic_Analysis/tide_fac_const.npz` & `pylibs_ocean-1.0.1/pyScripts/Harmonic_Analysis/tide_fac_const.npz`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/change_ssh_hotstart.py` & `pylibs_ocean-1.0.1/pyScripts/change_ssh_hotstart.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/download_AVISO.py` & `pylibs_ocean-1.0.1/pyScripts/download_AVISO.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/download_CMEMS.py` & `pylibs_ocean-1.0.1/pyScripts/download_CMEMS.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/download_HFRadar.py` & `pylibs_ocean-1.0.1/pyScripts/download_HFRadar.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/download_hycom.py` & `pylibs_ocean-1.0.1/pyScripts/download_hycom.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_bctides.py` & `pylibs_ocean-1.0.1/pyScripts/gen_bctides.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_fluxflag.py` & `pylibs_ocean-1.0.1/pyScripts/gen_fluxflag.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_fluxth_USGS.py` & `pylibs_ocean-1.0.1/pyScripts/gen_fluxth_USGS.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_hycom_3Dth_nudge.py` & `pylibs_ocean-1.0.1/pyScripts/gen_hycom_3Dth_nudge.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_hycom_hotstart.py` & `pylibs_ocean-1.0.1/pyScripts/gen_hycom_hotstart.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_narr_sflux.py` & `pylibs_ocean-1.0.1/pyScripts/gen_narr_sflux.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_shapiro.py` & `pylibs_ocean-1.0.1/pyScripts/gen_shapiro.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/gen_vqs.py` & `pylibs_ocean-1.0.1/pyScripts/gen_vqs.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/hotstart_proc.py` & `pylibs_ocean-1.0.1/pyScripts/hotstart_proc.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/make_sflux_links.py` & `pylibs_ocean-1.0.1/pyScripts/make_sflux_links.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/pextract_OLDIO_schism_fabm_xyz.py` & `pylibs_ocean-1.0.1/pyScripts/pextract_OLDIO_schism_fabm_xyz.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,36 +21,31 @@
 fmt=0                   #fmt=0: output as *.npz format; fmt=1: output as ASCII
 
 #optional
 grid=run+'/grid.npz'  #saved grid info, to speed up; use hgrid.gr3 and vgrid.in if not exist
 igather=1             #igather=1: save data on each rank,then combine; igather=0: use MPI  
 
 #resource requst 
-walltime='00:10:00'
-qnode='x5672'; nnode=2; ppn=8       #hurricane, ppn=8
-#qnode='bora'; nnode=2; ppn=20      #bora, ppn=20
-#qnode='vortex'; nnode=2; ppn=12    #vortex, ppn=12
-#qnode='femto'; nnode=2; ppn=12     #femto,ppn=32
-#qnode='potomac'; nnode=4; ppn=8    #ches, ppn=12
-#qnode='james'; nnode=5; ppn=20     #james, ppn=20
-#qnode='frontera'; nnode=1; ppn=56  #frontera, ppn=56 (flex,normal)
-#qnode='stampede2'; nnode=1; ppn=48 #stampede2, ppn=48 (skx-normal,skx-dev,normal,etc)
+walltime='00:10:00'; nnode=1;  ppn=4
+#hpc: femto, hurricane, bora, vortex, potomac, james, frontera, levante, stampede2
+#ppn:   32,       8,     8,    12,       12,     20,     56,      128,      48
 
-#additional information:  frontera,stampede2
-qname='flex'                        #partition name
-account='TG-OCE140024'              #stampede2: NOAA_CSDL_NWI,TG-OCE140024
+#optional: (frontera,levante,stampede2)
+qname   ='compute'         #partition name
+account ='TG-OCE140024'    #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028 
+qnode   =None              #specify node name, or default qnode based on HOST will be used
 
 jname='Rd_{}'.format(os.path.basename(run)) #job name
 ibatch=1; scrout='screen.out'; bdir=os.path.abspath(os.path.curdir)
 #-----------------------------------------------------------------------------
 #on front node: 1). submit jobs first (qsub), 2) running parallel jobs (mpirun) 
 #-----------------------------------------------------------------------------
 if ibatch==0: os.environ['job_on_node']='1'; os.environ['bdir']=bdir #run locally
 if os.getenv('job_on_node')==None:
-   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]
+   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]; os.environ['qnode']=get_qnode(qnode)
    if os.getenv('param')!=None: fmt=1; bdir,bcode=os.getenv('param').split(); os.chdir(bdir)
    scode=get_hpc_command(bcode,bdir,jname,qnode,nnode,ppn,walltime,scrout,fmt=fmt,qname=qname)
    print(scode); os.system(scode); os._exit(0)
 
 #-----------------------------------------------------------------------------
 #on computation node
 #-----------------------------------------------------------------------------
```

### Comparing `pylibs_ocean-1.0.0/pyScripts/pextract_OLDIO_schism_tide.py` & `pylibs_ocean-1.0.1/pyScripts/pextract_OLDIO_schism_tide.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/pextract_schism.py` & `pylibs_ocean-1.0.1/pyScripts/pextract_schism.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 #!/usr/bin/env python3
 '''
   extract time series of points@xyz or transects@xy from SCHISM outputs
 '''
 from pylib import *
-import time
 
 #-----------------------------------------------------------------------------
 #Input
 #-----------------------------------------------------------------------------
 run='/sciclone/data10/wangzg/CBP/RUN04a'
 svars=('elev','salt','hvel','NO3') #variables to be extracted
 bpfile='./station.bp'  #station file
 sname='./icm'
 
 #optional
 #itype=1         #0: time series of points @xyz;  1: time series of trasects @xy
 #ifs=0           #0: refer to free surface; 1: fixed depth
 #stacks=[1,3]    #outputs stacks to be extracted
 #nspool=12       #sub-sampling frequency within each stack (1 means all)
+#mdt=1           #time window (day) for averaging output
 #rvars=['elev','salt','hvel','NO3'] #rname the varibles 
 #prj=['epsg:26918','epsg:4326']  #projections used to transform coord. in station.bp
 
-#resource requst 
-walltime='00:10:00' 
-#qnode='x5672'; nnode=2; ppn=8       #hurricane, ppn=8
-#qnode='bora'; nnode=2; ppn=20      #bora, ppn=20
-#qnode='vortex'; nnode=2; ppn=12    #vortex, ppn=12
-qnode='femto'; nnode=1; ppn=32     #femto,ppn=32
-#qnode='potomac'; nnode=4; ppn=8    #ches, ppn=12
-#qnode='james'; nnode=5; ppn=20     #james, ppn=20
-#qnode='frontera'; nnode=1; ppn=56  #frontera, ppn=56 (flex,normal)
-#qnode='levante'; nnode=1; ppn=36   #levante, ppn=128
-#qnode='stampede2'; nnode=1; ppn=48 #stampede2, ppn=48 (skx-normal,skx-dev,normal,etc)
-
-#additional information:  frontera,levante,stampede2
-qname='flex'                        #partition name
-account='TG-OCE140024'              #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028 
+#hpc resource requst
+walltime='00:10:00'; nnode=1;  ppn=4
+#hpc: femto, hurricane, bora, vortex, potomac, james, frontera, levante, stampede2
+#ppn:   32,       8,     8,    12,       12,     20,     56,      128,      48
+
+#optional: (frontera,levante,stampede2)
+qname   ='compute'         #partition name
+account ='TG-OCE140024'    #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028
+qnode   =None              #specify node name, or default qnode based on HOST will be used
 
 brun=os.path.basename(run); jname='Rd_'+brun #job name
 ibatch=1; scrout='screen_{}.out'.format(brun); bdir=os.path.abspath(os.path.curdir)
 #-----------------------------------------------------------------------------
 #on front node: 1). submit jobs first (qsub), 2) running parallel jobs (mpirun) 
 #-----------------------------------------------------------------------------
 if ibatch==0: os.environ['job_on_node']='1'; os.environ['bdir']=bdir #run locally
 if os.getenv('job_on_node')==None:
-   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]
+   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]; os.environ['qnode']=get_qnode(qnode)
    if os.getenv('param')!=None: fmt=1; bdir,bcode=os.getenv('param').split(); os.chdir(bdir)
    scode=get_hpc_command(bcode,bdir,jname,qnode,nnode,ppn,walltime,scrout,fmt=fmt,qname=qname)
    print(scode); os.system(scode); os._exit(0)
 
 #-----------------------------------------------------------------------------
 #on computation node
 #-----------------------------------------------------------------------------
@@ -63,14 +57,15 @@
 #-----------------------------------------------------------------------------
 sdir=run+'/outputs'                                              #output directory
 if 'itype' not in locals(): itype=0                              #time series or transect
 if 'ifs' not in locals(): ifs=0                                  #refer to free surface
 if 'nspool' not in locals(): nspool=1                            #subsample
 if 'rvars' not in locals(): rvars=svars                          #rename variables
 if 'prj' not in locals(): prj=None                               #projections
+if 'mdt' not in locals(): mdt=None                               #average
 modules, outfmt, dstacks, dvars, dvars_2d = get_schism_output_info(sdir,1)     #schism outputs information
 stacks=arange(stacks[0],stacks[1]+1) if ('stacks' in locals()) else dstacks #check stacks
 
 #read model grid
 fgz=run+'/grid.npz'; fgd=run+'/hgrid.gr3'; fvd=run+'/vgrid.in'
 gd=loadz(fgz,'hgrid') if fexist(fgz) else read_schism_hgrid(fgd); gd.compute_bnd()
 vd=loadz(fgz,'vgrid') if fexist(fgz) else read_schism_vgrid(fvd); sys.stdout.flush()
@@ -80,15 +75,15 @@
 for svar in svars: 
    ovars=get_schism_var_info(svar,modules,fmt=outfmt)
    if ovars[0][1] not in dvars: continue 
    for istack in stacks:
        fname='{}_{}_{}'.format(oname,svar,istack); irec=irec+1; t00=time.time()
        if irec%nproc==myrank: 
           try:
-             read_schism_output(run,svar,bpfile,istack,ifs,nspool,fname=fname,hgrid=gd,vgrid=vd,fmt=itype,prj=prj)
+             read_schism_output(run,svar,bpfile,istack,ifs,nspool,fname=fname,hgrid=gd,vgrid=vd,fmt=itype,prj=prj,mdt=mdt)
              dt=time.time()-t00; print('finishing reading {}_{}.nc on myrank={}: {:.2f}s'.format(svar,istack,myrank,dt)); sys.stdout.flush()
           except:
              pass
 
 #combine results
 comm.Barrier()
 if myrank==0:
```

### Comparing `pylibs_ocean-1.0.0/pyScripts/pextract_schism_flux.py` & `pylibs_ocean-1.0.1/pyScripts/pextract_schism_flux.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 '''
 Compute fluxes based on SCHISM node information
 '''
 from pylib import *
-import time
 
 #-----------------------------------------------------------------------------
 #Input
 #-----------------------------------------------------------------------------
 run='/home/g/g260135/work/wangzg/DSP/RUN08a'
 svars=['GEN_1','GEN_2','GEN_3',]
 txy=[[[630597.229,630752.001], [4257510.76,4257544.77]],      #1st transect: [xi,yi]
@@ -18,38 +17,32 @@
 #optional
 #stacks=[1,9]    #output stacks
 #nspool=12       #sub-sampling frequency within each stack (1 means all)
 #dx=10          #interval of sub-section, used to divide transect
 #prj='cpp'      #projection that convert lon&lat to local project when ics=2
 #rvars=['g1','g2','g3',] #rname the varibles
 
-#resource requst 
-walltime='01:00:00'
-#qnode='x5672'; nnode=2; ppn=8      #hurricane, ppn=8
-#qnode='bora'; nnode=2; ppn=20      #bora, ppn=20
-#qnode='vortex'; nnode=2; ppn=12    #vortex, ppn=12
-#qnode='femto'; nnode=1; ppn=5      #femto,ppn=32
-#qnode='potomac'; nnode=4; ppn=8    #ches, ppn=12
-#qnode='james'; nnode=5; ppn=20     #james, ppn=20
-#qnode='frontera'; nnode=1; ppn=56  #frontera, ppn=56 (flex,normal)
-qnode='levante'; nnode=3; ppn=3   #levante, ppn=128
-#qnode='stampede2'; nnode=1; ppn=48 #stampede2, ppn=48 (skx-normal,skx-dev,normal,etc)
-
-#additional information:  frontera,levante,stampede2
-qname='compute'    #partition name
-account='gg0028'   #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028
+#resource requst
+walltime='00:10:00'; nnode=1;  ppn=4
+#hpc: femto, hurricane, bora, vortex, potomac, james, frontera, levante, stampede2
+#ppn:   32,       8,     8,    12,       12,     20,     56,      128,      48
+
+#optional: (frontera,levante,stampede2)
+qname   ='compute'         #partition name
+account ='TG-OCE140024'    #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028
+qnode   =None              #specify node name, or default qnode based on HOST will be used
 
-brun=os.path.basename(run); jname='Rd_'+brun #job name 
+brun=os.path.basename(run); jname='Rd_'+brun #job name
 ibatch=1; scrout='screen.out'; bdir=os.path.abspath(os.path.curdir)
 #-----------------------------------------------------------------------------
 #on front node: 1). submit jobs first (qsub), 2) running parallel jobs (mpirun) 
 #-----------------------------------------------------------------------------
 if ibatch==0: os.environ['job_on_node']='1'; os.environ['bdir']=bdir #run locally
 if os.getenv('job_on_node')==None:
-   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]
+   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]; os.environ['qnode']=get_qnode(qnode)
    if os.getenv('param')!=None: fmt=1; bdir,bcode=os.getenv('param').split(); os.chdir(bdir)
    scode=get_hpc_command(bcode,bdir,jname,qnode,nnode,ppn,walltime,scrout,fmt=fmt,qname=qname)
    print(scode); os.system(scode); os._exit(0)
 
 #-----------------------------------------------------------------------------
 #on computation node
 #-----------------------------------------------------------------------------
```

### Comparing `pylibs_ocean-1.0.0/pyScripts/pextract_schism_slab.py` & `pylibs_ocean-1.0.1/pyScripts/pextract_schism_slab.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 #!/usr/bin/env python3
 '''
   extract SCHISM slab outputs
 '''
 from pylib import *
-import time
 
 #-----------------------------------------------------------------------------
 #Input
 #-----------------------------------------------------------------------------
 run='/home/g/g260135/work/wangzg/DSP/RUN08a'  #run dir containing outputs
 svars=('elev','hvel','GEN_1')                 #variables to be extracted
 levels=[1,3,]        #schism level indices (1-nvrt: surface-bottom; (>nvrt): kbp level)
 sname='RUN08a/slab'  #name for saving the resutls
 
 #optional
 #stacks=[1,5]   #outputs stacks to be extracted
 #nspool=12      #sub-sampling frequency within each stack (1 means all)
 #mdt=1          #time window (day) for averaging output
 #rvars=['elev','hvel','G1'] #rname the varibles 
+#reg=None       #region for subsetting reslts (*.reg, or *.bp, or gd_subgrid)
 
 #resource requst 
-walltime='01:10:00' 
-#qnode='x5672'; nnode=2; ppn=8       #hurricane, ppn=8
-#qnode='bora'; nnode=2; ppn=20      #bora, ppn=20
-#qnode='vortex'; nnode=2; ppn=12    #vortex, ppn=12
-#qnode='femto'; nnode=1; ppn=32     #femto,ppn=32
-#qnode='potomac'; nnode=4; ppn=8    #ches, ppn=12
-#qnode='james'; nnode=5; ppn=20     #james, ppn=20
-#qnode='frontera'; nnode=1; ppn=56  #frontera, ppn=56 (flex,normal)
-qnode='levante'; nnode=1; ppn=36   #levante, ppn=128
-#qnode='stampede2'; nnode=1; ppn=48 #stampede2, ppn=48 (skx-normal,skx-dev,normal,etc)
-
-#additional information:  frontera,levante,stampede2
-qname='compute'    #partition name
-account='gg0028'   #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028
+walltime='00:10:00'; nnode=1;  ppn=4
+#hpc: femto, hurricane, bora, vortex, potomac, james, frontera, levante, stampede2
+#ppn:   32,       8,     8,    12,       12,     20,     56,      128,      48
+
+#optional: (frontera,levante,stampede2)
+qname   ='compute'         #partition name
+account ='TG-OCE140024'    #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028 
+qnode   =None              #specify node name, or default qnode based on HOST will be used
 
 brun=os.path.basename(run); jname='Rd_'+brun #job name
 ibatch=1; scrout='screen_{}.out'.format(brun); bdir=os.path.abspath(os.path.curdir)
 #-----------------------------------------------------------------------------
 #on front node: 1). submit jobs first (qsub), 2) running parallel jobs (mpirun) 
 #-----------------------------------------------------------------------------
 if ibatch==0: os.environ['job_on_node']='1'; os.environ['bdir']=bdir #run locally
 if os.getenv('job_on_node')==None:
-   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]
+   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]; os.environ['qnode']=get_qnode(qnode)
    if os.getenv('param')!=None: fmt=1; bdir,bcode=os.getenv('param').split(); os.chdir(bdir)
    scode=get_hpc_command(bcode,bdir,jname,qnode,nnode,ppn,walltime,scrout,fmt=fmt,qname=qname)
    print(scode); os.system(scode); os._exit(0)
 
 #-----------------------------------------------------------------------------
 #on computation node
 #-----------------------------------------------------------------------------
@@ -58,27 +52,28 @@
 
 #-----------------------------------------------------------------------------
 #do MPI work on each core
 #-----------------------------------------------------------------------------
 sdir=run+'/outputs'                            #output directory
 if 'nspool' not in locals(): nspool=1          #subsample
 if 'rvars' not in locals(): rvars=svars        #rename variables
-if 'mdt' not in locals(): mdt=None             #rename variables
+if 'mdt' not in locals(): mdt=None             #averaging
+if 'reg' not in locals(): reg=None             #region
 modules, outfmt, dstacks, dvars, dvars_2d = get_schism_output_info(sdir,1)  #schism outputs information
 stacks=arange(stacks[0],stacks[1]+1) if ('stacks' in locals()) else dstacks #check stacks
 
 #extract results
 irec=0; oname=odir+'/.schout'
 for svar in svars: 
    ovars=get_schism_var_info(svar,modules,fmt=outfmt)
    if ovars[0][1] not in dvars: continue 
    for istack in stacks:
        fname='{}_{}_{}_slab'.format(oname,svar,istack); irec=irec+1; t00=time.time()
        if irec%nproc==myrank: 
-          read_schism_slab(run,svar,levels,istack,nspool,mdt,fname=fname)
+          read_schism_slab(run,svar,levels,istack,nspool,mdt,fname=fname,reg=reg)
           dt=time.time()-t00; print('finishing reading {}_{}.nc on myrank={}: {:.2f}s'.format(svar,istack,myrank,dt)); sys.stdout.flush()
 
 #combine results
 comm.Barrier()
 if myrank==0:
    S=zdata(); S.time=[]; fnames=[]
    for i,[k,m] in enumerate(zip(svars,rvars)):
```

### Comparing `pylibs_ocean-1.0.0/pyScripts/pload_depth.py` & `pylibs_ocean-1.0.1/pyScripts/pload_depth.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,37 +24,31 @@
          "al_ll","nc_ll","fl_ll","gulf_1_dem_usgs","gulf_3_demcombined_ll","ge_ll","sc_ll",
          "cb_ll","db_ll","new_england_topobathy_dem_3m_dd","Tile3_R3_DEMv2","cb_bay_dem_v3.1_ll")
 
 sdir=r'/sciclone/data10/wangzg/DEM/npz'  #directory of DEM data
 reverse_sign=1  #invert depth sign
 
 #resource requst 
-walltime='00:10:00'
-qnode='x5672'; nnode=8; ppn=4       #hurricane, ppn=8
-#qnode='bora'; nnode=2; ppn=20      #bora, ppn=20
-#qnode='vortex'; nnode=2; ppn=12    #vortex, ppn=12
-#qnode='femto'; nnode=2; ppn=12     #femto,ppn=32
-#qnode='potomac'; nnode=4; ppn=8    #ches, ppn=12
-#qnode='james'; nnode=5; ppn=20     #james, ppn=20
-#qnode='frontera'; nnode=1; ppn=56  #frontera, ppn=56 (flex,normal)
-#qnode='levante'; nnode=1; ppn=36   #levante, ppn=128
-#qnode='stampede2'; nnode=1; ppn=48 #stampede2, ppn=48 (skx-normal,skx-dev,normal,etc)
+walltime='00:10:00'; nnode=1;  ppn=4
+#hpc: femto, hurricane, bora, vortex, potomac, james, frontera, levante, stampede2
+#ppn:   32,       8,     8,    12,       12,     20,     56,      128,      48
 
-#additional information:  frontera,levante,stampede2
-qname='flex'                        #partition name
-account='TG-OCE140024'              #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028
+#optional: (frontera,levante,stampede2)
+qname   ='compute'         #partition name
+account ='TG-OCE140024'    #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028 
+qnode   =None              #specify node name, or default qnode based on HOST will be used
 
 jname='load_dem' #job name
 ibatch=1; scrout='screen.out'; bdir=os.path.abspath(os.path.curdir)
 #-----------------------------------------------------------------------------
 #on front node: 1). submit jobs first (qsub), 2) running parallel jobs (mpirun) 
 #-----------------------------------------------------------------------------
 if ibatch==0: os.environ['job_on_node']='1'; os.environ['bdir']=bdir #run locally
 if os.getenv('job_on_node')==None:
-   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]
+   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]; os.environ['qnode']=get_qnode(qnode)
    if os.getenv('param')!=None: fmt=1; bdir,bcode=os.getenv('param').split(); os.chdir(bdir)
    scode=get_hpc_command(bcode,bdir,jname,qnode,nnode,ppn,walltime,scrout,fmt=fmt,qname=qname,account=account)
    print(scode); os.system(scode); os._exit(0)
 
 #-----------------------------------------------------------------------------
 #on computation node
 #-----------------------------------------------------------------------------
```

### Comparing `pylibs_ocean-1.0.0/pyScripts/run_mpi_template.py` & `pylibs_ocean-1.0.1/pyScripts/run_mpi_template.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 #!/usr/bin/env python3
 '''
 Template for running MPI job on sciclone/ches 
 Note: For MPI jobs demanding large memory, use small ppn
 '''
 from pylib import *
-import time
 
 #-----------------------------------------------------------------------------
 #Input
 #-----------------------------------------------------------------------------
-jname='mpi4py' #job name
+walltime='00:10:00'; nnode=1;  ppn=4
+#hpc: femto, hurricane, bora, vortex, potomac, james, frontera, levante, stampede2
+#ppn:   32,       8,     8,    12,       12,     20,     56,      128,      48
 
-#resource requst 
-walltime='00:10:00' 
-#qnode='x5672'; nnode=2; ppn=8      #hurricane, ppn=8
-#qnode='bora'; nnode=2; ppn=20      #bora, ppn=20
-#qnode='vortex'; nnode=2; ppn=12    #vortex, ppn=12
-#qnode='femto'; nnode=2; ppn=12     #femto,ppn=32
-#qnode='potomac'; nnode=4; ppn=8    #ches, ppn=12
-#qnode='james'; nnode=5; ppn=20     #james, ppn=20
-#qnode='frontera'; nnode=1; ppn=56  #frontera, ppn=56 (flex,normal)
-qnode='levante'; nnode=1; ppn=48   #levante, ppn=128
-#qnode='stampede2'; nnode=1; ppn=48 #stampede2, ppn=48 (skx-normal,skx-dev,normal,etc)
-
-#additional information:  frontera,levante,stampede2
-qname='compute'                        #partition name
-account='TG-OCE140024'              #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028 
+#optional: (frontera,levante,stampede2)
+qname   ='compute'         #partition name
+account ='TG-OCE140024'    #stampede2: NOAA_CSDL_NWI,TG-OCE140024; levante: gg0028
+qnode   =None              #specify node name, or default qnode based on HOST will be used
+jname   ='mpi4py'          #job name
 
 ibatch=1; scrout='screen.out'; bdir=os.path.abspath(os.path.curdir)
 #-----------------------------------------------------------------------------
 #on front node: 1). submit jobs first (qsub), 2) running parallel jobs (mpirun) 
 #-----------------------------------------------------------------------------
 if ibatch==0: os.environ['job_on_node']='1'; os.environ['bdir']=bdir #run locally
 if os.getenv('job_on_node')==None:
-   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]
+   if os.getenv('param')==None: fmt=0; bcode=sys.argv[0]; os.environ['qnode']=get_qnode(qnode)
    if os.getenv('param')!=None: fmt=1; bdir,bcode=os.getenv('param').split(); os.chdir(bdir)
    scode=get_hpc_command(bcode,bdir,jname,qnode,nnode,ppn,walltime,scrout,fmt=fmt,qname=qname,account=account)
    print(scode); os.system(scode); os._exit(0)
 
 #-----------------------------------------------------------------------------
 #on computation node
 #-----------------------------------------------------------------------------
```

### Comparing `pylibs_ocean-1.0.0/pyScripts/sflux_template.npz` & `pylibs_ocean-1.0.1/pyScripts/sflux_template.npz`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyScripts/subset_outputs_parallel.py` & `pylibs_ocean-1.0.1/pyScripts/subset_outputs_parallel.py`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/pyUtility/mylib.py` & `pylibs_ocean-1.0.1/pyUtility/mylib.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,50 @@
 
     def update(self):
         self.hf.canvas.restore_region(self.bg)
         for hg in self.hgs: self.hf.draw_artist(hg)
         self.hf.canvas.blit(self.hf.bbox)
         self.hf.canvas.flush_events()
 
+class _COMM_WORLD:
+      def __init__(self):
+          self.pid=os.getpid()
+          self.myrank=None
+
+      def Get_size(self):
+          self.nproc=1 if os.getenv('nproc') is None else int(os.getenv('nproc'))
+          return self.nproc
+
+      def Get_rank(self):
+          header='.pylib_pjob_id_'; open(header+str(self.pid),'w+').close()
+          if not hasattr(self,'nproc'): self.Get_size()
+          while len(glob(header+'*'))<self.nproc: time.sleep(0.1)
+          fnames=glob(header+'*'); pids=[*sort([int(i.split('_')[-1]) for i in fnames])]
+          self.myrank=pids.index(self.pid); self.delete(header,0.2)
+          return self.myrank
+
+      def Barrier(self):
+          header='.pylib_pjob_lock_'; open(header+str(self.pid),'w+').close()
+          while len(glob(header+'*'))<self.nproc: time.sleep(0.1)
+          self.delete(header,dt=0.2)
+
+      def delete(self,header=None,dt=0):
+          if self.myrank==0:
+             time.sleep(dt); [os.remove(i) for i in glob(header+'*')]
+          else:
+             time.sleep(2*dt)
+
+class parallel_jobs:
+      '''
+      compute nproc and myrank by dumping pid information on disk, when mpi4py fails.
+      Note: this is not MPI, but only for the purpose in distributing parallel jobs
+      '''
+      def __init__(self):
+          self.COMM_WORLD=_COMM_WORLD()
+
 def resize(data,shape,fill=0):
     '''
     re-define the shape of an data array; The added data are filled with value='fill argument'
     '''
     ds=data.shape; fdata=zeros(shape).astype(data.dtype); fdata[:]=fill
     exec('fdata[{}]=data'.format(':'+',:'.join([str(i) for i in ds])+',0'*(len(shape)-len(ds))))
     return fdata
@@ -262,74 +298,96 @@
         key=sline[0].strip(); value=sline[1].strip()
         if value=='': continue
         value=value.split()[0]
         param[key]=value
 
     return param
 
-def get_hpc_command(code,bdir,jname='mpi4py',qnode='x5672',nnode=1,ppn=1,wtime='01:00:00',
-                    scrout='screen.out',fmt=0,ename='param',qname='flex',account='gg0028',mem='4G'):
+def get_qnode(qnode=None):
+    '''
+    return hpc node name based on system's environment variable $HOST
+    '''
+    if qnode is not None: return qnode  #used other node names
+
+    host=os.getenv('HOST')
+    if host is None: sys.exit('set HOST environment variable HOST')
+    if host in ['femto.sciclone.wm.edu','viz']: qnode='femto'
+    if host in ['kuro.sciclone.wm.edu']: qnode='kuro'
+    if host in ['hurricane.sciclone.wm.edu']: qnode='x5672'
+    if host in ['bora.sciclone.wm.edu']: qnode='bora'
+    if host in ['vortex.sciclone.wm.edu']: qnode='vortex'
+    if host in ['chesapeake.sciclone.wm.edu']: qnode='potomac'
+    return qnode
+
+def get_hpc_command(code,bdir,jname='mpi4py',qnode=None,nnode=1,ppn=1,wtime='01:00:00',
+                    scrout='screen.out',fmt=0,ename='param',qname='flex',account=None,mem='4G',reservation=None):
     '''
     get command for batch jobs on sciclone/ches/viz3
        code: job script
        bdir: current working directory
        jname: job name
        qname: partition name (needed on some cluster/project)
        qnode: hpc node name
        nnode,ppn,wtime: request node number, core per node, and walltime
        mem: meomory; needed on cluster grace
+       reservation: get request debug node on kuro
        fmt=0: command for submitting batch jobs; fmt=1: command for run parallel jobs
     '''
-
-    nproc=nnode*ppn
+  
+    qnode0=qnode; qnode=os.getenv('qnode') if qnode is None else qnode; nproc=nnode*ppn
     if fmt==0:
        os.environ[ename]='{} {}'.format(bdir,os.path.abspath(code))
        #for submit jobs
-       if qnode in ['femto','cyclops']:
+       if qnode in ['femto','cyclops','kuro']:
           #scmd='sbatch --export=ALL --constraint=femto --exclusive -J {} -N {} -n {} -t {} {}'.format(jname,nnode,nproc,wtime,code)
           scmd='sbatch --export=ALL -J {} -N {} --ntasks-per-node {} -t {} {}'.format(jname,nnode,ppn,wtime,code)
+          if qnode=='kuro' and (reservation is not None): scmd='sbatch --reservation=debug --export=ALL -J {} -N {} --ntasks-per-node {} -t {} {}'.format(jname,nnode,ppn,wtime,code)
        elif qnode in ['grace',]:
           scmd='sbatch --export=ALL -J {} -N {} --mem={} --ntasks-per-node {} -t {} {}'.format(jname,nnode,mem,ppn,wtime,code)
        elif qnode in ['frontera',]:
           #scmd='sbatch --export=ALL,{}="{} {}" -J {} -p {} -N {} -n {} -t {} {}'.format(ename,bdir,code,jname,qname,nnode,nproc,wtime,code)
           scmd='sbatch --export=ALL -J {} -p {} -N {} --ntasks-per-node {} -t {} {}'.format(jname,qname,nnode,ppn,wtime,code)
-       elif qnode in ['levante',]:
+       elif qnode in ['levante','hercules']:
           scmd='sbatch --export=ALL --exclusive -J {} -p {} --account={} -N {} --ntasks-per-node {} -t {} {}'.format(jname,qname,account,nnode,ppn,wtime,code)
        elif qnode in ['stampede2',]:
           scmd='sbatch "--export=ALL" -J {} -p {} -A {} -N {} -n {} -t {} {}'.format(jname,qname,account,nnode,nproc,wtime,code)
        elif qnode in ['x5672','vortex','vortexa','c18x','potomac','james','bora']:
-          scmd='qsub {} -v {}="{} {}", -N {} -j oe -l nodes={}:{}:ppn={} -l walltime={}'.format(code,ename,bdir,code,jname,nnode,qnode,ppn,wtime)
+          scmd='qsub {} {} -v {}="{} {}", -N {} -j oe -l nodes={}:{}:ppn={} -l walltime={}'.format(code,'-V' if qnode0 is None else '', ename,bdir,code,jname,nnode,qnode,ppn,wtime)
           if qnode=='james': scmd='qsub {} -V -v {}="{} {}", -N {} -j oe -l nodes={}:{}:ppn={} -l walltime={}'.format(code,ename,bdir,code,jname,nnode,qnode,ppn,wtime)
        elif qnode in ['eagle','deception']:
           scmd='sbatch --export=ALL -A {} -J {} -p {} -N {} --ntasks-per-node {} -t {} {}'.format(account,jname,qname,nnode,ppn,wtime,code)
        else:
           sys.exit('unknow qnode: {},tag=1'.format(qnode))
     elif fmt==1:
        #for run parallel jobs
-       if qnode in ['femto','cyclops']:
-          scmd="srun --export=ALL,job_on_node=1,bdir={} {} >& {}".format(bdir,code,scrout)
+       if qnode in ['femto','cyclops','kuro',]:
+          scmd="srun --export=ALL,job_on_node=1,bdir={},nproc={} {} >& {}".format(bdir,nproc,code,scrout)
+          if qnode=='kuro' and ename!='run_schism': scmd='srun --export=PATH={},job_on_node=1,bdir={},nproc={} {} >& {}'.format('/sciclone/data10/wangzg/mambaforge/envs/kuro/bin/',bdir,nproc,code,scrout)
        elif qnode in ['grace',]:
           scmd="mpirun --env job_on_node 1 --env bdir='{}' -np {} {} >& {}".format(bdir,nproc,code,scrout) 
           if ename=='run_schism': scmd="mpirun -np {} ./{} >& {}".format(nproc,code,scrout)
        elif qnode in ['frontera']:
-          scmd="mpirun --env job_on_node 1 --env bdir='{}' -np {} {} >& {}".format(bdir,nproc,code,scrout)
+          scmd="mpirun --env job_on_node 1 --env bdir='{}' --env nproc {} -np {} {} >& {}".format(bdir,nproc,nproc,code,scrout)
           if ename=='run_schism': scmd="ibrun {} >& {}".format(code,scrout)
        elif qnode in ['stampede2',]:
-          scmd="mpiexec -envall -genv job_on_node 1 -genv bdir '{}' -n {} {} >& {}".format(bdir,nproc,code,scrout)
+          scmd="mpiexec -envall -genv job_on_node 1 -genv bdir '{}' -genv nproc {} -n {} {} >& {}".format(bdir,nproc,nproc,code,scrout)
           if ename=='run_schism': scmd="ibrun {} >& {}".format(code,scrout)
-       elif qnode in ['levante',]:
-          scmd="mpiexec -envall -genv job_on_node 1 -genv bdir '{}' -n {} {} >& {}".format(bdir,nproc,code,scrout)
+       elif qnode in ['levante','hercules']:
+          scmd="mpiexec -envall -genv job_on_node 1 -genv bdir '{}' -genv nproc {} -n {} {} >& {}".format(bdir,nproc,nproc,code,scrout)
           if ename=='run_schism':
              scmd="ulimit -s unlimited; ulimit -c 0; source /home/g/g260135/intel_tool; export UCX_UNIFIED_MODE=y;"
              scmd=scmd+"srun --export=ALL,job_on_node=1,bdir={} -l --cpu_bind=verbose --hint=nomultithread --distribution=block:cyclic {} >& {}".format(bdir,code,scrout)
+          if qnode=='hercules' and ename=='run_schism':
+             scmd="set -e; ulimit -s unlimited; source /home/yjzhang/modules.hercules;"
+             scmd=scmd+"srun --export=ALL,job_on_node=1,bdir={},nproc={} {} >& {}".format(bdir,nproc,code,scrout)
        elif qnode in ['x5672','vortex','vortexa','c18x','potomac','james','bora']:
           code=os.path.abspath(code)
-          scmd="mvp2run -v -e job_on_node=1 -e bdir='{}' {} >& {}".format(bdir,code,scrout)
-          if qnode=='bora': scmd="mvp2run -v -a -e job_on_node=1 -e bdir='{}' {} >& {}".format(bdir,code,scrout)
-          if qnode=='james': scmd="mvp2run -v -C 0.05 -a -e job_on_node=1 -e bdir='{}' {} >& {}".format(bdir,code,scrout)
+          scmd="mvp2run -v -e job_on_node=1 -e bdir='{}' -e nproc={} {} >& {}".format(bdir,nproc,code,scrout)
+          if qnode=='bora': scmd="mvp2run -v -a -e job_on_node=1 -e bdir='{}' -e nproc={} {} >& {}".format(bdir,nproc,code,scrout)
+          if qnode=='james': scmd="mvp2run -v -C 0.05 -a -e job_on_node=1 -e bdir='{}' -e nproc={} {} >& {}".format(bdir,nproc,code,scrout)
           #if qnode=='james' and ename=='run_schism': scmd='mpiexec -np {} --bind-to socket {}/{} >& {}'.format(nproc,bdir,code,scrout)
        elif qnode in ['eagle','deception']:
           scmd="mpirun --env job_on_node 1 --env bdir='{}' -{} {} {} >& {}".format(bdir,'n' if qnode=='eagle' else 'np',nproc,code,scrout)
        else:
           sys.exit('unknow qnode: {},tag=2'.format(qnode))
 
     return scmd
@@ -1662,14 +1720,40 @@
     elif backend == 'WXAgg':
         f.canvas.manager.window.SetPosition((x, y))
     else:
         # This works for QT and GTK
         # You can also use window.setGeometry
         f.canvas.manager.window.move(x, y)
 
+def modify_figure(fmt=0,hf=None):
+    '''
+    todo: not working yet !!
+    alias for "gcf().tight_layout(); mvfig(); show(block=False)"
+    '''
+    if hf is None: hf=gcf()
+    try:
+       hf.tight_layout(); mvfig(f=hf)
+       plt.ion(); show()
+       #if fmt==0: hf.show(block=False)
+       #if fmt==1: hf.show()
+    except:
+       pass
+
+def fig_IFNO(hf=None,ax=None):
+    '''
+    get figure information
+    '''
+    if hf is None: hf=gcf()
+    if ax is None: ax=gca()
+    f='figure(figsize=[{},{}])'.format(hf.get_figwidth(),hf.get_figheight())
+    a='xm={}; ym={}'.format(ax.get_xlim(),ax.get_ylim())
+    b='setp(gca(),xticks=[],yticks=[],xlim=xm,ylim=ym)'
+    c='gcf().tight_layout()'; d='show(block=False); mvfig()'
+    print('\n'.join([f,a,b,c,d]))
+
 def proj(fname0=None,fmt0=None,prj0=None,fname1=None,fmt1=None,prj1=None,x=None,y=None,lon0=None,lat0=None,order0=0,order1=0):
     '''
     tranfrom projection of files: proj(fname0,fmt0,prj0,fname1,fmt1,prj1,x,y,lon0,lat0,order0,order1)
        fname: file name
        fmt: 0: SCHISM gr3 file; 1: SCHISM bp file; 2: xyz file; 3: xyz file with line number
        prj: projection name (e.g. 'epsg:26918', 'epsg:4326','cpp'), or projection string (e.g. prj0=get_prj_file('epsg:4326'))
        lon0,lat0: center for transformation between lon&lat and x&y; if lon0=None or lat0=None, then x0=mean(lon), and y0=mean(lat)
@@ -1757,15 +1841,15 @@
       prj1: name of original projection
       prj2: name of target projection
       when 'cpp' projection exists, lon0, and lat0 arguments can be provided
     '''
     px,py=proj(prj0=prj1,prj1=prj2,x=x,y=y,**args)
     return [px,py]
 
-def get_prj_file(prjname='epsg:4326',fmt=0,prj_dir=r'D:\Work\Database\projection\prj_files'):
+def get_prj_file(prjname='epsg:4326',fmt=0,prj_dir=r'D:\Work\Database\projection\prj_files',fname=None):
     '''
     return projection name or entire database (dict)
         fmt=0: get one projection
         fmt=1: return dict of projection database
         fmt=-1: process *.prj files from prj_dir
 
     #-------online method-----------------
@@ -1787,35 +1871,22 @@
     if fmt==0:
         S=loadz('{}/../pyScripts/prj.npz'.format(bdir))
         return S.prj[prjname]
     elif fmt==1:
         S=loadz('{}/../pyScripts/prj.npz'.format(bdir))
         return S.prj
     elif fmt==-1:
-        #dir of *.prj files
-        #prj_dir=r'D:\Work\Database\projection\prj_files'
-
-        #---processing all prj files-------------------------------------------
-        fnames=os.listdir(prj_dir)
-
-        prj=dict()
-        for fname in fnames:
-            import re
-            R=re.match('epsg.(\d+).prj',fname);
-            if not R: continue
-            prj_num=int(R.groups()[0])
-            with open('{}/{}'.format(prj_dir,fname),'r') as fid:
-                line=fid.readline().strip();
-                prj['epsg:{}'.format(prj_num)]=line
-
-        # #save prj file as a database
-        # S=zdata();
-        # S.prj=prj
-        # savez('{}/prj'.format(bdir),S)
-        return prj
+         if not os.path.exists(prj_dir): return
+         pnames=glob('{}/*.prj'.format(prj_dir)); prj={}
+         for pname in pnames:
+             line=open(pname,'r').readline().strip()
+             pn=os.path.basename(pname)[:-4].replace('.',':').lower()
+             prj[pn]=line
+         if fname is not None: C=zdata(); C.prj=prj; C.save(fname)
+         return prj
     else:
         sys.exit('unknow fmt')
 
 #----------------convert_matfile_format----------------------------------------
 #def convert_matfile_format(file):
 #    '''
 #    convert a matlab data to self-defined python format
@@ -1961,14 +2032,49 @@
     S.std=std(dx)
     S.ms=1-sum(dx**2)/sum((abs(x1-mx2)+abs(x2-mx2))**2)
     if fmt==1: a,S.pvalue=sp.stats.pearsonr(x1,x2)
     S.std1=std1; S.std2=std2; S.npt=npt
     S.taylor=array([sqrt(mean((x1-x1.mean())**2))/S.std2,sqrt(((x1-x1.mean()-x2+x2.mean())**2).mean())/S.std2,S.R]) if (npt>=3 and std2!=0) else [0,0,0]
     return S
 
+def interp_vertical(data0,zcor0,zcor):
+    '''
+    interpolate data in the vertical dimension; works for multi-dimensional data.
+    format:
+      data0([nz0,...]: can be mutli-dimensional, but the 1st dim must be vertical
+      zcor0[nz0,...]:    z-coordiantes of data; it can have fewer dimenions of data
+      zcor[nz,...]:   target z-coordiantes.
+    where nz0 and nz are number of vertical layers
+
+    Note: zs and zcor can have different number of dimensions, can be different from data.
+          However, their dimensions should be consistent with data if ndim>1.
+    '''
+
+    #collect dimension info
+    v0=data0; z0=zcor0; z=zcor; nz0=len(z0); nz=len(z); ds=[nz,*v0.shape[1:]]; ndim=v0.ndim
+
+    #check zcor order and dimension
+    dz=array(z0[0]-z0[-1])
+    if dz.min()*dz.max()<0: sys.exit('zcor should be either decreasing or increasing for all pts')
+    if dz.max()>0: v0=v0[::-1]; z0=z0[::-1]
+
+    #interpolate in the vertical
+    v=zeros(ds)*nan; sfp=ones(ds)==1
+    for i in arange(ndim-z0.ndim): z0=z0[...,None] #z0=expand_dims(z0,axis=-1) expand z dims
+    for i in arange(ndim-z.ndim):  z=z[...,None]   #z=expand_dims(z,axis=-1)
+    fp=z<=z0[0][None,...];  afp=sfp*fp; v[afp]=(v0[0][None,...]*sfp)[afp]  #extend bottom
+    fp=z>=z0[-1][None,...]; afp=sfp*fp; v[afp]=(v0[-1][None,...]*sfp)[afp] #extend surface
+    for k in arange(nz0-1):
+        z1,z2=z0[k][None,...],z0[k+1][None,...]; dz=z2-z1; fpz=dz==0; dz[fpz]=1 #exclude z1=z2
+        if sum(~fpz)==0: continue
+        rat=(z-z1)/dz; fp=(rat>=0)*(rat<=1); fp=fp*(~fpz)
+        if sum(fp)==0: continue
+        afp=fp*sfp; v[afp]=((1-rat)*v0[k][None,...]+rat*v0[k+1][None,...])[afp]
+    return v
+
 def read_shapefile_data(fname):
     '''
     read shapefile (*.shp) and return its content
 
     note:  works for pts and polygon only, may not work for other geomerties (need update in these cases)
     '''
 
@@ -2488,14 +2594,92 @@
     S.freq=r_[0,array([i.strip() for i in open(tidal_names,'r').readlines()[2::2]]).astype('float')]
 
     #clean temporaray files--------
     os.remove(fname); os.remove(sname)
     if os.path.exists(tname): os.remove(tname)
     return S
 
+def ceqstate(T,S,P=0):
+    '''
+    calculate seawater density (Millero and Poisson 1981, Gill, 1982); Input:
+      T: temperature in [C]
+      S: salinity in [PSU]
+      P: pressure [bars] (P=0: at 1 atm. pressure)
+    '''
+
+    npt=len(T)
+    #pre_calculation
+    T2=T*T; T3=T**3; T4=T**4; T5=T**5
+    S05=sqrt(S); S15=S*S05; S2=S*S; P2=P*P
+
+    #pure water S=0,at 1 atm.
+    rho_pw=999.842594+6.793952e-2*T-9.095290e-3*T2+1.001685e-4*T3-1.120083e-6*T4+6.536332e-9*T5
+
+    #density with Salinity
+    A=8.24493e-1-4.0899e-3*T+7.6438e-5*T2-8.2467e-7*T3+5.3875e-9*T4
+    B=-5.72466e-3+1.0227e-4*T-1.6546e-6*T2
+    C=4.8314e-4
+    rho_st=rho_pw+A*S+B*S15+C*S2
+
+    #pressure not zero
+    if P==0:
+      rho=rho_st
+    else:
+      K_pw=19652.21+148.4206*T-2.327105*T2+1.360477e-2*T3-5.155288e-5*T4; K_st=K_pw
+      K_st=K_st+S*(54.6746-0.603459*T+1.09987e-2*T2-6.1670e-5*T3)+S15*(7.944e-2+1.6483e-2*T-5.3009e-4*T2);
+      K_stp=K_st+P*(3.239908+1.43713e-3*T+1.16092e-4*T2-5.77905e-7*T3)+P*S*(2.2838e-3-1.0981e-5*T-1.6078e-6*T2)+1.91075e-4*P*S15 \
+            +P2*(8.50935e-5-6.12293e-6*T+5.2787e-8*T2)+P2*S*(-9.9348e-7+2.0816e-8*T+9.1697e-10*T2)
+      rho=rho_st/(1-P/K_stp)
+    return rho
+
+def subdomain_index(x,y,xm,ym):
+    '''
+    get subdomain indice (e.g. for subsetting purpose)
+    Inputs:
+       x(ny,nx): x coordinate
+       y(ny,nx): y coordinate
+       xm:  x-range: [-75, -70],  or x-array (eg. gd.x)
+       ym:  y-range: [35, 40],    or y-array (eg. gd.y)
+    Output:  ix1,ix2,iy1,iy2
+    '''
+    #pre-proc
+    if len(xm)==2: xm=array([*xm,xm[1],xm[0]]); ym=array([ym[0],ym[0],ym[1],ym[1]])
+    xc=xm.mean(); yc=xm.mean(); x1,x2,y1,y2=xm.min(),xm.max(),ym.min(),ym.max()
+    ny,nx=x.shape; sind=near_pts(c_[xc,yc],c_[x.ravel(),y.ravel()])
+    iy,ix=[i[0] for i in unravel_index(sind,[ny,nx])]; ix1,ix2,iy1,iy2=ix,ix+1,iy,iy+1
+
+    #find initial box
+    while True:
+        ix1i=ix1; ix2i=ix2; iy1i=iy1; iy2i=iy2
+        if x[iy1:iy2,ix1].max()>x1: ix1=max(0,ix1-1)
+        if x[iy1:iy2,ix2-1].min()<x2: ix2=min(nx,ix2+1)
+        if y[iy1,ix1:ix2].max()>y1: iy1=max(0,iy1-1)
+        if y[iy2-1,ix1:ix2].min()<y2: iy2=min(ny,iy2+1)
+        if (ix1i==ix1)*(ix2i==ix2)*(iy1i==iy1)*(iy2i==iy2): break
+
+    #shrink the box
+    for m in arange(2):
+        if m==1 and len(xm)==2: continue
+        pxy=c_[array([x1,x2,x2,x1]),array([y1,y1,y2,y2])] if m==0 else c_[xm,ym]
+        for n in arange(4):
+            while True:
+                if n==0: ix1=ix1+1
+                if n==1: ix2=ix2-1
+                if n==2: iy1=iy1+1
+                if n==3: iy2=iy2-1
+                xs=r_[x[iy1:iy2,ix1],x[iy2-1,(ix1+1):(ix2-1)],x[iy1:iy2,ix2-1][::-1],x[iy1,(ix1+1):(ix2-1)][::-1]]
+                ys=r_[y[iy1:iy2,ix1],y[iy2-1,(ix1+1):(ix2-1)],y[iy1:iy2,ix2-1][::-1],y[iy1,(ix1+1):(ix2-1)][::-1]]
+                if inside_polygon(pxy,xs,ys).min()==0:
+                   if n==0: ix1=ix1-1
+                   if n==1: ix2=ix2+1
+                   if n==2: iy1=iy1-1
+                   if n==3: iy2=iy2+1
+                   break
+    return ix1,ix2,iy1,iy2
+
 def get_hycom(Time,xyz,vind,hdir='./HYCOM',method=0):
     '''
     extract Hycom time series at stations
     ti: time seires; xyz=c_[loni,lati,depi];
     vind: list of index for variables to be extracted. [0,1,2,3] for ['elev','temp','salt','uv']
     hdir: directory for hycom data
     method=0: linear interpolation; method=1: nearest interpolation
```

### Comparing `pylibs_ocean-1.0.0/pyUtility/schism_file.py` & `pylibs_ocean-1.0.1/pyUtility/schism_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         if not hasattr(self,'zcj'): self.compute_side(2)
         return self.dps
 
     def plot(self,ax=None,fmt=0,value=None,ec=None,fc=None,lw=0.1,levels=None,shading='gouraud',xy=0,
              ticks=None,xlim=None,ylim=None,clim=None,extend='both',method=0,cb=True,cb_aspect=30,cb_pad=0.02,**args):
         '''
         plot grid with default color value (grid depth)
-        fmt=0: plot grid only; fmt=1: plot filled contours; fmt=2: plot contour lines
+        fmt=0: plot grid only; fmt=1: plot filled contours
+        fmt=2: plot contour lines at levels; colors and linewidths can be provided for each contour
         value: color value size(np,or ne)
         ec: color of grid line;  fc: element color; lw: grid line width
         levels=100: number of colors for depths; levels=array([v1,v2,...]): depths for plot
         ticks=[v1,v2,...]: colorbar ticks; ticks=10: number of ticks
         clim=[vmin,vmax]: value range for plot/colorbar
         method=0: using tricontourf/tricontouf; method=1: using tripcolor
         cb=False: not add colorbar
@@ -75,14 +76,15 @@
               if value.size==self.ne+sum(fp4) and sum(fp4)!=0: hg=tripcolor(x,y,trs,facecolors=value,vmin=vm[0],vmax=vm[1],**args)
            else:  #contourf or contour
               if sum(isnan(value))!=0: trs=trs[~isnan(value[trs].sum(axis=1))] #set mask
               if value.size==self.ne: value=self.interp_elem_to_node(value=value) #elem value to node value
               if not hasattr(levels,'__len__'): levels=linspace(*vm,int(levels)) #detemine levels
               if fmt==1: hg=tricontourf(x,y,trs,value,levels=levels,vmin=vm[0],vmax=vm[1],extend=extend,**args)
               if fmt==2: hg=tricontour(x,y,trs,value,levels=levels, vmin=vm[0],vmax=vm[1],extend=extend,**args)
+           self.data=value
 
            #add colobar
            cm.ScalarMappable.set_clim(hg,vmin=vm[0],vmax=vm[1])
            if cb==True:
               hc=colorbar(hg,aspect=cb_aspect,pad=cb_pad); self.hc=hc
               if ticks is not None:
                  if not hasattr(ticks,'__len__'):
@@ -100,14 +102,15 @@
 
         hg=hg0 if fmt==0 else hg if ec=='None' else [*hg0,hg]; self.hg=hg
         if xlim is not None: setp(ax,xlim=xlim)
         if ylim is not None: setp(ax,ylim=ylim)
         if mpl.get_backend().lower() in ['qt5agg','qtagg']:
            acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs])
            if 'bp' not in ats: self.bp=schism_bpfile()
+           if 'reg' not in ats: self.reg=schism_bpfile(fmt=1)
            if 'query' not in ats: self.query_pt()
            if 'bnd' not in ats: self.create_bnd()
            if 'node' not in ats: self.show_node()
         return hg
 
         #-------------------------------------------------
         #for reference: old grid plot method
@@ -212,14 +215,15 @@
         if len(c)==1:
            hb=plot(r_[bx1,nan,bx2],r_[by1,nan,by2],c,lw=lw,**args); self.hb=hb
         else:
           hb1=plot(bx1,by1,c[0],lw=lw,**args); hb2=plot(bx2,by2,c[-1],lw=lw,**args); self.hb=[hb1,hb2]
         if mpl.get_backend().lower() in ['qt5agg','qtagg']:
            acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs])
            if 'bp' not in ats: self.bp=schism_bpfile()
+           if 'reg' not in ats: self.reg=schism_bpfile(fmt=1)
            if 'query' not in ats: self.query_pt()
            if 'bnd' not in ats: self.create_bnd()
            if 'node' not in ats: self.show_node()
         return self.hb
 
     def read_hgrid(self,fname,*args):
         #attribute tracking the file originally read, mainly used for savez and save_pkl
@@ -270,50 +274,58 @@
         '''
         evi=read_schism_prop(fname)
         if len(evi)!=self.ne: sys.exit("check dimension: ne={}, prop={}".format(self.ne,len(evi)))
         return evi
 
     def interp_node_to_elem(self,value=None):
         '''
-        interpolate node values to element values
+        interpolate node values to element values (works for multi-dimensional data)
             default is self.dp => self.dpe
         '''
         #interpolate
         dp=self.dp if (value is None) else value
-        fp3=self.i34==3; fp4=~fp3; dpe=zeros(self.ne)
-        dpe[fp3]=dp[self.elnode[fp3,:3]].mean(axis=1)
-        dpe[fp4]=dp[self.elnode[fp4]].mean(axis=1)
-        return dpe
+        dms=[*dp.shape]; ip=dms.index(self.np); idm=arange(len(dms)); dms[ip]=self.ne
+        if len(dms)>1:  idm[0],idm[ip]=ip,0; dms[0],dms[ip]=dms[ip],dms[0] #put dim=np 1st for multi-dimensional data
+        fp3=self.i34==3; fp4=~fp3; dp=dp.transpose(idm); dpe=zeros(dms)
+        dpe[fp3]=dp[self.elnode[fp3,:3]].mean(axis=1); dpe[fp4]=dp[self.elnode[fp4]].mean(axis=1)
+        return dpe.transpose(idm)
 
     def interp_elem_to_node(self,value=None,fmt=0,p=1):
         '''
         interpolate element values to nodes
         if value not given, dpe is used
-        fmt=0: simple avarage; fmt=1: inverse distance (power=p)
+        fmt=0: element area weighted avarage in nodal ball
+        fmt=1: inverse distance (power=p)
         fmt=2: maximum of surrounding nodal values
         fmt=3: minimum of surrounding nodal values
+        fmt=4: simple avarage in nodal ball
         '''
         #element values
         if not hasattr(self,'nne'): self.compute_nne()
         if (value is None) and (not hasattr(self,'dpe')): self.compute_ctr()
         v0=self.dpe if (value is None) else value
 
         #interpolation
         vs=v0[self.ine]
         if fmt==0:
+           if not hasattr(self,'area'): self.compute_area()
+           fpn=self.ine!=-1; a=self.area[self.ine]
+           ta=sum(a*fpn,axis=1); tv=sum(a*vs*fpn,axis=1)
+           fpz=ta!=0; v=zeros(self.np)*nan; v[fpz]=tv[fpz]/ta[fpz]
+        if fmt==1:
+              dist=abs((self.xctr[self.ine]+1j*self.yctr[self.ine])-(self.x+1j*self.y)[:,None])
+              w=1/(dist**p); w[self.ine==-1]=0; tw=w.sum(axis=1); v=(w*vs).sum(axis=1)/tw
+        if fmt==2: vs[self.ine==-1]=v0.min()-1; v=vs.max(axis=1)
+        if fmt==3: vs[self.ine==-1]=v0.max()+1; v=vs.min(axis=1)
+        if fmt==4:
            w=self.ine!=-1; tw=w.sum(axis=1)
-           if sum(isnan(value))!=0:
+           if sum(isnan(v0))!=0:
               vs[~w]=0; v=vs.sum(axis=1)/tw
            else:
               v=(w*vs).sum(axis=1)/tw
-        if fmt==2: vs[self.ine==-1]=v0.min()-1; v=vs.max(axis=1)
-        if fmt==3: vs[self.ine==-1]=v0.max()+1; v=vs.min(axis=1)
-        if fmt==1:
-              dist=abs((self.xctr[self.ine]+1j*self.yctr[self.ine])-(self.x+1j*self.y)[:,None])
-              w=1/(dist**p); w[self.ine==-1]=0; tw=w.sum(axis=1); v=(w*vs).sum(axis=1)/tw
         return v
 
     def compute_all(self,fmt=0):
         '''
         compute all geometry information of hgrid by invoking:
            functions: compute_ctr(),compute_area(),compute_side(fmt=2),compute_nne(),compute_ic3()
            attrs: (xctr,yctr,dpe),(area),(ns,isidenode,isdel,xcj,ycj,dps,distj),(nne,mnei,indel,ine),(ic3,elside)
@@ -327,30 +339,29 @@
 
     def compute_ctr(self):
         '''
         compute element center information: (xctr,yctr,dpe)
         '''
         if not hasattr(self,'xctr'):
            fp3=self.i34==3; fp4=~fp3; self.xctr,self.yctr,self.dpe=zeros([3,self.ne])
-           self.xctr[fp3]=self.x[self.elnode[fp3,:3]].mean(axis=1)
-           self.xctr[fp4]=self.x[self.elnode[fp4,:]].mean(axis=1)
-           self.yctr[fp3]=self.y[self.elnode[fp3,:3]].mean(axis=1)
-           self.yctr[fp4]=self.y[self.elnode[fp4,:]].mean(axis=1)
-           self.dpe[fp3]=self.dp[self.elnode[fp3,:3]].mean(axis=1)
-           self.dpe[fp4]=self.dp[self.elnode[fp4,:]].mean(axis=1)
+           self.xctr[fp3],self.yctr[fp3],self.dpe[fp3]=c_[self.x,self.y,self.dp][self.elnode[fp3,:3]].mean(axis=1).T
+           self.xctr[fp4],self.yctr[fp4],self.dpe[fp4]=c_[self.x,self.y,self.dp][self.elnode[fp4]].mean(axis=1).T
         return self.dpe
 
-    def compute_area(self):
-        fp=self.elnode[:,-1]<0;
-        x1=self.x[self.elnode[:,0]]; y1=self.y[self.elnode[:,0]];
-        x2=self.x[self.elnode[:,1]]; y2=self.y[self.elnode[:,1]];
-        x3=self.x[self.elnode[:,2]]; y3=self.y[self.elnode[:,2]];
-        x4=self.x[self.elnode[:,3]]; y4=self.y[self.elnode[:,3]]; x4[fp]=x1[fp]; y4[fp]=y1[fp]
-        self.area=((x2-x1)*(y3-y1)-(x3-x1)*(y2-y1)+(x3-x1)*(y4-y1)-(x4-x1)*(y3-y1))/2
-        return self.area
+    def compute_area(self,fmt=0):
+        '''
+        compute element area
+        fmt=0: return element area
+        fmt=1: return element area, 1st triangle area, and 2nd triangle area
+        '''
+        x1,x2,x3,x4=self.x[self.elnode].T; y1,y2,y3,y4=self.y[self.elnode].T
+        #fp=self.elnode[:,-1]<0; x4[fp]=x1[fp]; y4[fp]=y1[fp]
+        fp=self.i34==3; x4[fp]=x1[fp]; y4[fp]=y1[fp]
+        a1=((x2-x1)*(y3-y1)-(x3-x1)*(y2-y1))/2; a2=((x3-x1)*(y4-y1)-(x4-x1)*(y3-y1))/2;  self.area=a1+a2
+        return self.area if fmt==0 else [self.area, a1, a2]
 
     def compute_gradient(self,fmt=0,value=None,outfmt=0,cpp=None,lon0=None,lat0=None):
         '''
         Compute gradient on each element first, then convert to node value
           fmt: interploation method (see details in interp_elem_to_node())
               (0: simple avarage; fmt=1: inverse distance; fmt=2: maximum of surrounding nodal values)
           value=None: gd.dp is used;    value: array of [np,] or [ne]
@@ -367,32 +378,24 @@
         else:
             x=self.x; y=self.y
 
         #get node value
         v0=self.dp if value is None else value
         if len(v0)==self.ne: v0=self.interp_elem_to_node(value=v0)
 
-        #get pts
-        fp=self.elnode[:,-1]<0; fpn=~fp;
-        x1=x[self.elnode[:,0]]; y1=y[self.elnode[:,0]]; v1=v0[self.elnode[:,0]]
-        x2=x[self.elnode[:,1]]; y2=y[self.elnode[:,1]]; v2=v0[self.elnode[:,1]]
-        x3=x[self.elnode[:,2]]; y3=y[self.elnode[:,2]]; v3=v0[self.elnode[:,2]]
-        x4=x[self.elnode[:,3]]; y4=y[self.elnode[:,3]]; v4=v0[self.elnode[:,3]]
-        x4[fp]=x1[fp]; y4[fp]=y1[fp]; v4[fp]=v1[fp]
-        a1=((x2-x1)*(y3-y1)-(x3-x1)*(y2-y1))/2
-        a2=((x3-x1)*(y4-y1)-(x4-x1)*(y3-y1))/2
-
         #compute gradients
-        dpedx=(v1*(y2-y3)+v2*(y3-y1)+v3*(y1-y2))/(2*a1)
-        dpedy=((x3-x2)*v1+(x1-x3)*v2+(x2-x1)*v3)/(2*a1)
-
-        #for quads
-        dpedx2=(v1[fpn]*(y3[fpn]-y4[fpn])+v3[fpn]*(y4[fpn]-y1[fpn])+v4[fpn]*(y1[fpn]-y3[fpn]))/(2*a2[fpn])
-        dpedy2=((x4[fpn]-x3[fpn])*v1[fpn]+(x1[fpn]-x4[fpn])*v3[fpn]+(x3[fpn]-x1[fpn])*v4[fpn])/(2*a2[fpn])
-        dpedx[fpn]=(dpedx[fpn]+dpedx2)/2;  dpedy[fpn]=(dpedy[fpn]+dpedy2)/2
+        x1,x2,x3,x4=x[self.elnode].T; y1,y2,y3,y4=y[self.elnode].T; v1,v2,v3,v4=v0[self.elnode].T
+        a1, a2=self.compute_area(fmt=1)[1:]
+        dpedx=(v1*(y2-y3)+v2*(y3-y1)+v3*(y1-y2))/(2*a1); dpedy=((x3-x2)*v1+(x1-x3)*v2+(x2-x1)*v3)/(2*a1)
+
+        #for quads, average 2 triangles
+        fpn=self.i34==4
+        if sum(fpn)!=0:
+           dpedx[fpn]=(dpedx[fpn]+(v1*(y3-y4)+v3*(y4-y1)+v4*(y1-y3))[fpn]/(2*a2[fpn]))/2
+           dpedy[fpn]=(dpedy[fpn]+((x4-x3)*v1+(x1-x4)*v3+(x3-x1)*v4)[fpn]/(2*a2[fpn]))/2
 
         #interp to node
         dpedxy=sqrt(dpedx**2+dpedy**2)
         dpdx=self.interp_elem_to_node(value=dpedx,fmt=fmt)
         dpdy=self.interp_elem_to_node(value=dpedy,fmt=fmt)
         dpdxy=self.interp_elem_to_node(value=dpedxy,fmt=fmt)
 
@@ -439,65 +442,146 @@
               inode=self.isidenode.ravel(); iside=tile(arange(self.ns),2) #node-side table
               sind=argsort(inode); inode=inode[sind]; iside=iside[sind]
               self.nns=unique(inode,return_counts=True)[1]; self.ins=-ones([self.np,self.nns.max()]).astype('int'); n=0
               for i in arange(self.np): self.ins[i,:self.nns[i]]=iside[n:(n+self.nns[i])]; n=n+self.nns[i]
 
            return self.ns,self.isidenode,self.isdel
 
-    def compute_bnd(self,bxy=None,nb_max=500000):
+    def compute_bnd(self,bxy=None,nb_max=500000,method=0):
         '''
         compute boundary information. If bxy is provided, define open/land boundries
 
         bxy: endpoint coordinates of open boundaries. Examples:
             1). bxy=[x1,x2,y1,y2]  #only one open boundary
             2). bxy=[[x1,x2,y1,y2],[x1,x2,y1,y2],...]  #multiple open boundaries
             3). bxy="bpfile", with paired build points sequentially defining each boundaries
 
         nb_max: maximum boundary nodes allowed for each bnd segments
+        method=0: latest method in computing bnd; method=1: old method
         '''
-        print('computing grid boundaries')
         if not hasattr(self,'isdel') or not hasattr(self,'isidenode'): self.compute_side(fmt=1)
+        if self.ns>1e6: print('computing grid boundaries')
 
-        #find boundary side and element
-        fpn=self.isdel[:,-1]==-1;  isn=self.isidenode[fpn]; be=self.isdel[fpn][:,0]; nbs=len(be)
+        if method==0:
+           #find boundary side and element, and sort it
+           fpn=self.isdel[:,-1]==-1; be=self.isdel[fpn][:,0]; n1,n2=self.isidenode[fpn].T; i34=self.i34[be]; nbs=len(be)
+           for i in arange(4): fp=(n1==self.elnode[be,(i+1)%i34])*(n2==self.elnode[be,i%i34]); n1[fp],n2[fp]=n2[fp],n1[fp]
+           sinds=dict(zip(n1,[[i] for i in n2]))
+
+           #---------------------------------------------------------------------------
+           #this part is used to dealing with illegal mesh
+           #---------------------------------------------------------------------------
+           #find the nodes connecting to more than 2 sides,and build the side dict
+           ibnx,nbnx=unique(n1,return_counts=True); ibnx=ibnx[nbnx>1]
+           for i in ibnx:
+               #find all nodes in the nodal ball, and compute the angles
+               if not hasattr(self,'xctr'): self.compute_ctr()
+               ips=unique(self.elnode[self.indel[i]]); ips=setdiff1d(ips[1:] if ips[0]<0 else ips,i); nps=len(ips)
+               A=angle((self.x[ips]-self.x[i])+1j*(self.y[ips]-self.y[i])); iA=argsort(A); A,ips=A[iA],ips[iA]
+               cA=angle((self.xctr[self.indel[i]]-self.x[i])+1j*(self.yctr[self.indel[i]]-self.y[i])) #angle for element center
+
+               #get all boundary nodes
+               ib1=nonzero(n1==i)[0]; ip1=n2[ib1];  ib2=nonzero(n2==i)[0]; ip2=n1[ib2]; sinds[i]=[]
+               for n in arange(nps):
+                   i1=ips[n]; i2=ips[(n+1)%nps]; A1=A[n]; A2=A[(n+1)%nps]
+                   if A2<A1: A2=A2%(2*pi); cA=cA%(2*pi)
+                   if sum((cA>A1)*(cA<A2))!=0: continue #element center between i1 and i2
+                   if (i1 in ip1) and (i2 in ip2):  #find a pair
+                       sinds[i].append([i2,i,i1])
+                   elif (i2 in ip1) and (i1 in ip2):
+                       sinds[i].append([i1,i,i2])
+                   else:
+                       sys.exit('wrong in connect side pairs')
+
+           #reconnect sides, but skip the nodes connecting to more than 2 sides
+           while True:#append sides to their downstream sides
+               iflag=0
+               for i in ibnx:
+                   for n, side in enumerate(sinds[i]):
+                       if side is None: continue
+                       if side[-1] in ibnx:
+                           iflag=1
+                           for m,dside in enumerate(sinds[side[-1]]):
+                               if dside is None: continue
+                               nsd=dside.index(side[-1])
+                               if array_equal(side[-(nsd+1):],dside[:(nsd+1)]):
+                                   sinds[i][n]=[*side,*dside[(nsd+1):]]
+                                   sinds[side[-1]][m]=None; break
+               if iflag==0: break
+
+           while True: #append all sides to their upstream ordinary sides
+               iflag=0
+               for i in ibnx:
+                   for n, side in enumerate(sinds[i]):
+                       if side is None: continue
+                       sinds[i][n]=None; iflag=1
+                       if side[0] in ibnx: #append to upstream side
+                           for m,uside in enumerate(sinds[side[0]]):
+                               if uside is None: continue
+                               isd=uside.index(side[0]); nsd=len(uside)-isd
+                               if array_equal(uside[isd:],side[:nsd]):
+                                   sinds[side[0]][m]=[*uside,*side[nsd:]]
+                                   sinds[i][n]=None; break
+                       else: #append to other side
+                           sinds[side[0]]=side[1:]
+               if iflag==0: break
+           for i in ibnx: del sinds[i]
+           #---------------------------------------------------------------------------
+
+           #search boundary from other nodes
+           ids=list(sinds.keys()); ns=len(ids); sindf=dict(zip(ids,arange(ns))); ifb=ones(ns).astype('int'); nb=0; nbn=[]; ibn=[]
+           while(sum(ifb)!=0):
+               #start points
+               ib=nonzero(ifb==1)[0][0]; id0=ids[ib]; id=sinds[id0][-1]; ifb[sindf[id0]]=0; ibni=[id0,*sinds[id0]]; iloop=0
+
+               #search each segments
+               while True:
+                   idp=id; id=sinds[id][-1]; ifb[sindf[idp]]=0
+                   if(id==id0): ibni.extend(sinds[idp][:-1]); break
+                   ibni.extend(sinds[idp]); iloop=iloop+1
+                   if iloop>nb_max: print('grid boundary search failed: check your grid'); return array(ibni)
+               nb=nb+1; nbn.append(len(ibni)); ibn.append(array(ibni))
+        else:
+            #find boundary side and element
+            fpn=self.isdel[:,-1]==-1;  isn=self.isidenode[fpn]; be=self.isdel[fpn][:,0]; nbs=len(be)
 
-        #sort isn
-        i2=ones(nbs).astype('int'); fp3=nonzero(self.i34[be]==3)[0]; fp4=nonzero(self.i34[be]==4)[0]
-        for i in arange(4):
-            if i==3:
-                i1=self.elnode[be[fp4],3]; i2=self.elnode[be[fp4],0]
-                fp=(isn[fp4,0]==i2)*(isn[fp4,1]==i1); isn[fp4[fp]]=fliplr(isn[fp4[fp]])
-            else:
-                i1=self.elnode[be,i]; i2[fp3]=self.elnode[be[fp3],(i+1)%3]; i2[fp4]=self.elnode[be[fp4],i+1]
-                fp=(isn[:,0]==i2)*(isn[:,1]==i1); isn[fp]=fliplr(isn[fp])
+            #sort isn
+            i2=ones(nbs).astype('int'); fp3=nonzero(self.i34[be]==3)[0]; fp4=nonzero(self.i34[be]==4)[0]
+            for i in arange(4):
+                if i==3:
+                    i1=self.elnode[be[fp4],3]; i2=self.elnode[be[fp4],0]
+                    fp=(isn[fp4,0]==i2)*(isn[fp4,1]==i1); isn[fp4[fp]]=fliplr(isn[fp4[fp]])
+                else:
+                    i1=self.elnode[be,i]; i2[fp3]=self.elnode[be[fp3],(i+1)%3]; i2[fp4]=self.elnode[be[fp4],i+1]
+                    fp=(isn[:,0]==i2)*(isn[:,1]==i1); isn[fp]=fliplr(isn[fp])
 
-        #compute all boundaries
-        ifb=ones(nbs).astype('int'); nb=0; nbn=[]; ibn=[]
-        sinds=dict(zip(isn[:,0],arange(nbs))) #dict for sides
-
-        #find the nodes connecting to more than 2 sides
-        ibnx,nbnx=unique(isn[:,0],return_counts=True); idx=[]; nbx=0
-        for i in ibnx[nbnx>1]: k=nonzero(isn[:,0]==i)[0]; idx.extend(k); nbx=nbx+len(k)
-
-        #search boundary from other nodes
-        while(sum(ifb)!=0):
-            #start points
-            if nbx>0:
-                nbx=nbx-1; id0,id=isn[idx[nbx]]; ifb[idx[nbx]]=0
-            else:
-                id0=isn[nonzero(ifb==1)[0][0],0]; id=isn[sinds[id0],1]; ifb[sinds[id0]]=0
-            ibni=[id0,id]; ifb[sinds[id]]=0; iloop=0
+            #compute all boundaries
+            ifb=ones(nbs).astype('int'); nb=0; nbn=[]; ibn=[]
+            sinds=dict(zip(isn[:,0],arange(nbs))) #dict for sides
+
+            #find the nodes connecting to more than 2 sides
+            ibnx,nbnx=unique(isn[:,0],return_counts=True); idx=[]; nbx=0
+            for i in ibnx[nbnx>1]: k=nonzero(isn[:,0]==i)[0]; idx.extend(k); nbx=nbx+len(k)
+
+            #search boundary from other nodes
+            while(sum(ifb)!=0):
+                #start points
+                if nbx>0:
+                    nbx=nbx-1; id0,id=isn[idx[nbx]]; ifb[idx[nbx]]=0
+                else:
+                    id0=isn[nonzero(ifb==1)[0][0],0]; id=isn[sinds[id0],1]; ifb[sinds[id0]]=0
+                ibni=[id0,id]; ifb[sinds[id]]=0; iloop=0
 
-            #search each segments
-            while True:
-                id=isn[sinds[id],1]; ifb[sinds[id]]=0
-                if(id==id0): break
-                ibni.append(id); iloop=iloop+1
-                if iloop>nb_max: print('grid boundary search failed: check your grid'); return array(ibni)
-            nb=nb+1; nbn.append(len(ibni)); ibn.append(array(ibni))
+                #search each segments
+                while True:
+                    id=isn[sinds[id],1]; ifb[sinds[id]]=0
+                    if(id==id0): break
+                    ibni.append(id); iloop=iloop+1
+                    if iloop>nb_max: print('grid boundary search failed: check your grid'); return array(ibni)
+                nb=nb+1; nbn.append(len(ibni)); ibn.append(array(ibni))
 
         #sort bnd
         nbn=array(nbn); ibn=array(ibn,dtype='O'); fps=flipud(argsort(nbn)); nbn,ibn=nbn[fps],ibn[fps]
         if ibn.shape[0]==1: ibn=ibn.astype('int')
 
         #find the outline
         island=ones(nb).astype('int'); bid=[]
@@ -521,15 +605,17 @@
 
         #add to grid bnd info
         if (not hasattr(self,'nob')) and (bxy is None):
            self.nob=0; self.nobn=array([]); self.iobn=array([[]])
            self.nlb=S.nb+1; self.nlbn=array([2,*S.nbn]); self.island=array([0,*S.island])
            self.ilbn=array([array([S.ibn[0][-1],S.ibn[0][0]]).astype('int'), *S.ibn],dtype='O')
 
+        #----------------------------------------------------------------------------
         #define open/land/island boundaries
+        #----------------------------------------------------------------------------
         if bxy is not None:
            if isinstance(bxy,str): #bxy is a bpfile
               bp=read_schism_bpfile(bxy); bxy=[]
               if bp.nsta%2!=0: sys.exit('even number of points are required')
               for i in arange(int(bp.nsta/2)): bxy.append([bp.x[2*i],bp.x[2*i+1],bp.y[2*i],bp.y[2*i+1]])
 
            S=self.bndinfo; bf=array([zeros(i) for i in S.nbn],dtype='O')
@@ -701,15 +787,16 @@
                fps=pie2!=-1; pie[sind2[fps]]=sind4[pie2[fps]]; pip[sind2[fps]]=sindn.T[pie2[fps]]
 
             #compute acor
             fpn=pie!=-1
             if sum(fpn)!=0:
                x1,x2,x3=self.x[pip[fpn]].T; y1,y2,y3=self.y[pip[fpn]].T; x,y=pxy[fpn].T
                A1=signa(c_[x,x2,x3],c_[y,y2,y3]); A2=signa(c_[x1,x,x3],c_[y1,y,y3])
-               A=signa(c_[x1,x2,x3],c_[y1,y2,y3]); pacor[fpn]=c_[A1/A,A2/A,1-(A1+A2)/A]
+               A=signa(c_[x1,x2,x3],c_[y1,y2,y3]); fp=(A1+A2-A)>0; A[fp]=A1[fp]+A2[fp]
+               pacor[fpn]=c_[A1/A,A2/A,1-(A1+A2)/A]
             if sum(~fpn)!=0:
                sindn=near_pts(pxy[~fpn],c_[self.x,self.y]); pip[~fpn]=sindn[:,None]; pacor[~fpn,0]=1
 
         return pie,pip,pacor
 
     def compute_kb(self,kbp,fmt=0):
         '''
@@ -718,31 +805,79 @@
         '''
         if fmt==0: kb=kbp[self.elnode]; kb[self.i34==3,-1]=-1; kb=kb.max(axis=1)
         if fmt==1:
            if not hasattr(self,'isidenode'): self.compute_side(fmt=1)
            kb=kbp[self.isidenode].max(axis=1)
         return kb
 
+    def compute_angle(self):
+        '''
+        compute internal angles
+        '''
+        ie=arange(self.ne); angles=[]
+        for i in arange(4):
+            i1=(i-1)%self.i34; i2=i%self.i34; i3=(i+1)%self.i34
+            id=self.elnode[ie[:,None],c_[i1,i2,i3]]; x1,x2,x3=self.x[id].T; y1,y2,y3=self.y[id].T
+            a=(angle((x1-x2)+1j*(y1-y2))-angle((x3-x2)+1j*(y3-y2)))%(2*pi); angles.append(a*180/pi)
+        self.angles=array(angles).T
+        return self.angles
+
     def interp(self,pxy,value=None,fmt=0):
         '''
         interpolate to get value at pxy
           pxy: c_[x,y]
           value=None: gd.dp is used; value: array of [np,] or [ne,]
           fmt=0: (default) faster method by searching the neighbors of elements and nodes
           fmt=1: slower method using point-wise comparison
 
           Note: for interpolation of few pts on a large grid, fmt=1 can be faster than fmt=0
         '''
-        #get node value
-        vi=self.dp if value is None else value
-        if len(vi)==self.ne: vi=self.interp_elem_to_node(value=vi)
+
+        vi=self.dp if value is None else value; npt=len(vi) #get value
+        pie,pip,pacor=self.compute_acor(pxy,fmt=fmt)        #get interp coeff
 
         #interp
-        pip,pacor=self.compute_acor(pxy,fmt=fmt)[1:]
-        return (vi[pip]*pacor).sum(axis=1)
+        if npt==self.np:
+           return (vi[pip]*pacor).sum(axis=1)
+        elif npt==self.ne:
+           return vi[pie]
+        else:
+           sys.exit('unknown data size: {}'.format(npt))
+
+    def scatter_to_grid(self,fmt=0,reg_in=1,reg_out=1,**args):
+        '''
+        construct a new schism grid based on:
+           fmt=0:  node
+           fmt=1:  element center
+           fmt=2:  side center
+
+        reg_in=1:  delete elements inside islands;      reg_in=0: not delete
+        reg_out=1: delete elements outside grid domain; reg_out=0: not delete
+
+        '''
+        #get regions
+        if reg_in==1 or reg_out==1:
+           if not hasattr(self,'bndinfo'): self.compute_bnd()
+           if reg_in==1:  reg_in=[c_[self.x[i],self.y[i]] for i in self.bndinfo.ibn[1:]]
+           if reg_out==1: reg_out=[c_[self.x[i],self.y[i]] for i in self.bndinfo.ibn[:1]]
+        if reg_in==0:  reg_in=None
+        if reg_out==0: reg_out=None
+
+        #get scatter
+        if fmt==0: xyz=c_[self.x,self.y,self.z]
+        if fmt==1:
+           if not hasattr(self,'dpe'): self.compute_ctr()
+           xyz=c_[self.xctr,self.yctr,self.dpe]
+        if fmt==2:
+           if not hasattr(self,'dps'): self.compute_side(fmt=2)
+           xyz=c_[self.xcj,self.ycj,self.dps]
+
+        #build grid
+        gdn=scatter_to_schism_grid(xyz,reg_out=reg_out,reg_in=reg_in,**args)
+        return gdn
 
     def smooth(self,dist,value=None,fmt=0,ms=1e8):
         '''
         smooth field by averaging values within radius of dist
           dist: averaging radius
           value=None: gd.dp is used; value: array of [np,] or [ne,]
           fmt=0: return smoothed nodal values; fmt=1: return smoothed elem. values
@@ -773,14 +908,104 @@
                 pv[pidi]=ev.sum(axis=1)/ew.sum(axis=1)
             sindp,pxy=sindp[~fpc],pxy[~fpc] #update remaining nodes
         if fmt==1:
            return pv
         else:
            return self.interp_elem_to_node(pv)
 
+    def compute_zcor(self,vgrid,eta=None):
+        ''' 
+        compute zcor @ each nodes; need inputs:
+           vgrid: read_schism_vgrid('vgrid.in')
+           eta (optional): surface elevation (dim=[np] or [1])
+        ''' 
+        if eta is None:
+           zcor=self.zcor if hasattr(self,'zcor') else vgrid.compute_zcor(self.dp)
+           if not hasattr(self,'zcor'): self.zcor=zcor #save zcor
+        else:
+           zcor=vgrid.compute_zcor(self.dp,eta=eta)
+        return zcor
+
+    def compute_volume(self,vgrid,fmt=0,value=None,eta=None): 
+        '''
+        compute volume or volume*value for schism grid
+        Inputs:
+           vgrid: read_schism_vgrid('vgrid.in')
+           eta   (optional): surface elevation (dim=[np] or [1])
+           value (optional): tracer concentration with dimension size (ne, nvrt) or (np, nvrt).
+        Outputs:
+          fmt=0: each prism   (ne,nvrt-1)
+          fmt=1: each column  (ne,)
+          fmt=2: total volumn (1,)
+        '''
+        #compute prism volume
+        if not hasattr(self,'area'): self.compute_area()
+        zcor=self.compute_zcor(vgrid,eta=eta); ze=zeros([self.ne,vgrid.nvrt]); fp3=self.i34==3; fp4=~fp3
+        ze[fp3]=zcor[self.elnode[fp3,:3]].mean(axis=1); ze[fp4]=zcor[self.elnode[fp4]].mean(axis=1)
+        v=(ze[:,1:]-ze[:,:-1])*self.area[:,None]
+
+        #multiplee value
+        if value is not None:
+           if value.shape[0]==self.np: value=self.interp_node_to_elem(value); value[:,1:]=(value[:,:-1]+value[:,1:])/2
+           v=v*value[:,1:]
+        
+        return v if fmt==0 else v.sum(axis=1) if fmt==1 else v.sum()
+
+    def compute_CFL(self,dt=120, u=0):
+        '''
+        compute CFL number
+        dt: time step (second);  u: flow velocity (m/s)
+        '''
+        if not hasattr(self,'area'): self.compute_area()
+        if not hasattr(self,'dpe'): self.compute_ctr()
+        self.cfl=0.5*dt*(abs(u)+sqrt(9.81*self.dpe))/sqrt(self.area/pi); fp4=self.i34==4
+        self.cfl[fp4]=self.cfl[fp4]*sqrt(2)
+        return self.cfl
+
+    def compute_curl(self,u,v):
+        '''
+        compute curl of vector filed (u, v):  curl=dv/dx-du/dy
+        note: the rotation rate of eddy flow field is: omiga=0.5*curl (radian/second)
+        '''
+        #pre-proc
+        if u.shape[0]==self.ne: u=self.interp_elem_to_node(u); v=self.interp_elem_to_node(v)
+        x1,x2,x3,x4=self.x[self.elnode].T; y1,y2,y3,y4=self.y[self.elnode].T
+        u1,u2,u3,u4=u[self.elnode].T; v1,v2,v3,v4=v[self.elnode].T;  a1, a2=self.compute_area(fmt=1)[1:]
+
+        #compute gradient
+        dvdx=(v1*(y2-y3)+v2*(y3-y1)+v3*(y1-y2))/(2*a1)
+        dudy=((x3-x2)*u1+(x1-x3)*u2+(x2-x1)*u3)/(2*a1)
+
+        #for quads, average 2 triangles
+        fpn=self.i34==4
+        if sum(fpn)!=0:
+           dvdx[fpn]=(dvdx[fpn]+(v1*(y3-y4)+v3*(y4-y1)+v4*(y1-y3))[fpn]/(2*a2[fpn]))/2
+           dudy[fpn]=(dudy[fpn]+((x4-x3)*u1+(x1-x4)*u3+(x3-x1)*u4)[fpn]/(2*a2[fpn]))/2
+        return dvdx-dudy
+
+    def compute_contour(self,levels,value=None):
+        '''
+        compute contour lines
+        '''
+        value=self.dp if value is None else value
+        if value.size==self.ne: value=self.interp_elem_to_node(value)
+
+        #plot contour and extract the lines
+        fp4=self.i34==4; trs=r_[self.elnode[:,:3],c_[self.elnode[fp4,0],self.elnode[fp4,2:]]]
+        hf=figure(); hf.set_visible(False)
+        P=tricontour(self.x,self.y,trs,value,levels=levels); close(hf); cxy=[]
+        for k in arange(len(P.collections)):
+            p=P.collections[k].get_paths()
+            for i in arange(len(p)):
+                xii,yii=p[i].vertices.T
+                xi=r_[xii,NaN] if i==0 else r_[xi,xii,NaN]
+                yi=r_[yii,NaN] if i==0 else r_[yi,yii,NaN]
+            cxy.append(c_[xi,yi])
+        return array(cxy) if len(cxy)==1 else array(cxy,dtype='O')
+
     def write(self, fname=None,**args):
         '''
         generic function to save grid as different format
         format: (*.gr3, *.ll, *.ic, *.prop, *.npz, *.pkl, *.shp, *.bnd), (exceptions are in *.gr3 format)
         examples:
            1). gd.write('grid.npz')  or gd.write('grid')
            2). gd.write('grid.pkl')
@@ -924,50 +1149,31 @@
             c. internal angle >= angle_max,
             if no parameters are provided, angle_ratio=0.5 will be use
         2). fname: output a new grid "fname" if fname!=None
         '''
         if not hasattr(self,'index_bad_quad'): self.check_quads(angle_ratio,angle_min,angle_max)
 
         #compute (angle_max-angle_min) in splitted triangle
-        qind=self.index_bad_quad;
-        x=self.x[self.elnode[qind,:]]; y=self.y[self.elnode[qind,:]];
+        qind=self.index_bad_quad; x=self.x[self.elnode[qind,:]]; y=self.y[self.elnode[qind,:]]
 
         #compute difference between internal angles
         for i in arange(4):
-            id1=mod(i-1+4,4); id2=i; id3=mod(i+1,4)
-            x1=x[:,id1]; x2=x[:,id2]; x3=x[:,id3]
-            y1=y[:,id1]; y2=y[:,id2]; y3=y[:,id3]
-
-            a1=angle((x1-x2)+1j*(y1-y2))-angle((x3-x2)+1j*(y3-y2))
-            a2=angle((x2-x3)+1j*(y2-y3))-angle((x1-x3)+1j*(y1-y3))
-            a3=angle((x3-x1)+1j*(y3-y1))-angle((x2-x1)+1j*(y2-y1))
-            a1=mod(a1*180/pi+360,360);a2=mod(a2*180/pi+360,360);a3=mod(a3*180/pi+360,360)
-
-            #compute amax-amin
-            a=c_[a1,a2,a3]; Ai=a.max(axis=1)-a.min(axis=1)
-            A=Ai if i==0 else c_[A,Ai]
+            nid=r_[(i-1)%4,i,(i+1)%4]; x1,x2,x3=x[:,nid].T; y1,y2,y3=y[:,nid].T
+            a1=(angle((x1-x2)+1j*(y1-y2))-angle((x3-x2)+1j*(y3-y2)))%(2*pi)
+            a2=(angle((x2-x3)+1j*(y2-y3))-angle((x1-x3)+1j*(y1-y3)))%(2*pi)
+            a3=(angle((x3-x1)+1j*(y3-y1))-angle((x2-x1)+1j*(y2-y1)))%(2*pi)
+            a=c_[a1,a2,a3]*180/pi; da=a.max(axis=1)-a.min(axis=1) #compute amax-amin
+            A=da if i==0 else c_[A,da]
+        flag=sign(A[:,0]+A[:,2]-A[:,1]-A[:,3]) #flag for spliting quads
 
         #split quads
-        flag=sign(A[:,0]+A[:,2]-A[:,1]-A[:,3])
-
-        ne=self.ne; nea=len(self.index_bad_quad);
-        self.elnode=r_[self.elnode,ones([nea,4])-3].astype('int');
-        for i in arange(nea):
-            ind=self.index_bad_quad[i]
-            nds=self.elnode[ind,:].copy();
-            if flag[i]>=0:
-                self.elnode[ind,:]=r_[nds[[0,1,2]],-2]; self.i34[ind]=3
-                self.elnode[ne+i,:]=r_[nds[[2,3,0]],-2]
-            else:
-                self.elnode[ind,:]=r_[nds[[1,2,3]],-2]; self.i34[ind]=3
-                self.elnode[ne+i,:]=r_[nds[[3,0,1]],-2]
-
-        self.ne=ne+nea
-        self.i34=r_[self.i34,ones(nea)*3].astype('int');
-        self.elnode=self.elnode.astype('int')
+        nea=len(self.index_bad_quad); elnode=tile(-2,[nea,4]); nds=self.elnode[qind]; self.i34[qind]=3
+        fp=flag>=0; ie=qind[fp]; self.elnode[ie,:3]=nds[fp,:3]; self.elnode[ie,-1]=-2; elnode[fp,:3]=nds[fp][:,array([2,3,0])]
+        fp=flag<0;  ie=qind[fp]; self.elnode[ie,:3]=nds[fp][:,array([1,2,3])]; self.elnode[ie,-1]=-2; elnode[fp,:3]=nds[fp][:,array([3,0,1])]
+        self.ne=self.ne+nea; self.i34=r_[self.i34,tile(3,nea)]; self.elnode=r_[self.elnode,elnode]
 
         #write new grids
         if fname is not None: self.write_hgrid(fname)
 
     def check_quads(self,angle_ratio=None,angle_min=None,angle_max=None,fname='bad_quad.bp'):
         '''
         1). check the quality of quads, violations can be:
@@ -975,40 +1181,26 @@
             b. internal angle <= angle_min,
             c. internal angle >= angle_max,
             if no parameters are provided, angle_ratio=0.5 will be used
         2). the locations of bad quads are saved in file "fname"
         '''
 
         if angle_ratio is None and angle_min is None and angle_max is None: angle_ratio=0.5
-        qind=nonzero(self.i34==4)[0];
-        x=self.x[self.elnode[qind,:]]; y=self.y[self.elnode[qind,:]];
-
-        #compute internal angle
-        a=[];
-        for i in arange(4):
-            id1=mod(i-1+4,4); id2=i; id3=mod(i+1,4)
-            x1=x[:,id1]; x2=x[:,id2]; x3=x[:,id3];
-            y1=y[:,id1]; y2=y[:,id2]; y3=y[:,id3];
-
-            ai=angle((x1-x2)+1j*(y1-y2))-angle((x3-x2)+1j*(y3-y2))
-            a.append(ai*180/pi);
-        a=array(a).T; a=mod(a+360,360)
+        if not hasattr(self,'angles'): self.compute_angle()
+        if not hasattr(self,'xctr'): self.compute_ctr()
 
         #check violation
-        fp=a[:,0]==-999
-        if angle_ratio is not None: fp=fp|((a.min(axis=1)/a.max(axis=1))<angle_ratio)
-        for i in arange(4):
-            if angle_min is not None: fp=fp|(a[:,i]<=angle_min)
-            if angle_max is not None: fp=fp|(a[:,i]>=angle_max)
+        qind=nonzero(self.i34==4)[0]; A=self.angles[qind]; fp=qind==-999
+        if angle_ratio is not None: fp=fp|((A.min(axis=1)/A.max(axis=1))<angle_ratio)
+        if angle_min is not None: fp=fp|(A.min(axis=1)<=angle_min)
+        if angle_max is not None: fp=fp|(A.max(axis=1)>=angle_max)
         self.index_bad_quad=qind[nonzero(fp)[0]]
 
         #output bad_quad location as bp file
-        if not hasattr(self,'xctr'): self.compute_ctr()
-        qxi=self.xctr[self.index_bad_quad]; qyi=self.yctr[self.index_bad_quad]
-        sbp=schism_bpfile(); sbp.nsta=len(qxi); sbp.x=qxi; sbp.y=qyi; sbp.z=zeros(sbp.nsta); sbp.write_bpfile(fname)
+        sbp=schism_bpfile(); sbp.x,sbp.y=c_[self.xctr,self.yctr][self.index_bad_quad].T; sbp.save(fname)
         return self.index_bad_quad
 
     def plot_bad_quads(self,color='r',ms=12,*args):
         #plot grid with bad quads
         if not hasattr(self,'index_bad_quad'): self.check_quads()
         if not hasattr(self,'xctr'): self.compute_ctr()
 
@@ -1060,39 +1252,25 @@
         Examples:
             1). gd.check_skew_elems(), or gd.check_skew_elems(threshold=30)
             2). gd.check_skew_elems(15,10), or gd.check_skew_elems(threshold=15,angle_min=10)
         '''
         if threshold is None and angle_min is None: threshold=30
         if not hasattr(self,'dpe'): self.compute_ctr()
 
-        sindw=[]
         if threshold is not None: #check length ratio
            if not hasattr(self,'distj'):  self.compute_side(fmt=2)
            if not hasattr(self,'elside'): self.compute_ic3()
            if not hasattr(self,'area'):   self.compute_area()
            distj=self.distj[self.elside]; distj[self.elside==-1]=0  #side length
            srat=distj.max(axis=1)/sqrt(maximum(self.area/pi,sys.float_info.epsilon)) #ratio
-           sindw.extend(nonzero(srat>threshold)[0])
+           sindw=nonzero(srat>threshold)[0]
 
         if angle_min is not None: #check minimum angle
-           #for triangles
-           fp=nonzero(self.i34==3)[0]; x=self.x[self.elnode[fp,:3]]; y=self.y[self.elnode[fp,:3]]; sind=[]
-           for i in arange(3):
-               x1=x[:,i]; x2=x[:,(i+1)%3]; x3=x[:,(i+2)%3]; y1=y[:,i]; y2=y[:,(i+1)%3]; y3=y[:,(i+2)%3]
-               ai=abs(angle((x1-x2)+1j*(y1-y2))-angle((x3-x2)+1j*(y3-y2)))*180/pi
-               sind.extend(nonzero(ai<=angle_min)[0])
-           sind3=fp[unique(sind).astype('int')]
-
-           #for quads
-           fp=nonzero(self.i34==4)[0]; x=self.x[self.elnode[fp,:]]; y=self.y[self.elnode[fp,:]]; sind=[]
-           for i in arange(4):
-               x1=x[:,i]; x2=x[:,(i+1)%4]; x3=x[:,(i+2)%4]; y1=y[:,i]; y2=y[:,(i+1)%4]; y3=y[:,(i+2)%4]
-               ai=abs(angle((x1-x2)+1j*(y1-y2))-angle((x3-x2)+1j*(y3-y2)))*180/pi
-               sind.extend(nonzero(ai<=angle_min)[0])
-           sind4=fp[unique(sind).astype('int')]; sindw.extend(r_[sind3,sind4])
+           if not hasattr(self,'angles'): self.compute_angle()
+           a=self.angles; a[a<0]=999; sindw=nonzero(a.min(axis=1)<=angle_min)[0]
 
         #combine and save
         sindw=array(sindw)
         if fname is not None: C=schism_bpfile(); C.x,C.y,C.z=self.xctr[sindw],self.yctr[sindw],self.dpe[sindw]; C.save(fname)
         return sindw
 
     def inside_elem(self,pxy,ie):
@@ -1114,15 +1292,16 @@
             A2=signa(c_[x1,xi,x3],c_[y1,yi,y3]); A3=signa(c_[x1,x2,xi],c_[y1,y2,yi])
             fps=(A1>=0)*(A2>=0)*(A3>=0); ac1=A1[fps]/A0[fps]; ac2=A2[fps]/A0[fps]
             if not isinstance(fps,np.ndarray): fps=array([fps])
 
             #get index of pts
             if i==0: sind.extend(nonzero(fps)[0])
             if i==1: sind.extend(sindr[fps])
-            pip.extend(ip[fps]); pacor.extend(c_[ac1,ac2,1-ac1-ac2])
+            ac3=1-ac1-ac2; fpn=ac3<0; ac2[fpn]=1-ac1[fpn]; ac3[fpn]=0
+            pip.extend(ip[fps]); pacor.extend(c_[ac1,ac2,ac3])
         return array(sind),array(pip),array(pacor)
 
     def inside_grid(self,pxy):
         '''
         check whether pts are inside grid
         usage:
             sind=gd.inside_grid(pxy)
@@ -1309,30 +1488,40 @@
         '''
         add function for querying depth
         '''
         def connect_actions():
             self.cidquery=gcf().canvas.mpl_connect('button_press_event', onclick)
 
         def onclick(sp):
-            dlk=int(sp.dblclick); btn=int(sp.button); bx=sp.xdata; by=sp.ydata
-            if dlk==0 and btn==1:
+            dlk=int(sp.dblclick); btn=int(sp.button); bx=sp.xdata; by=sp.ydata; pz=0
+            if dlk==0 and btn==3:
                acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs]);ac=acs[nonzero(ats=='bp')[0][0]]
                if hasattr(ac,'bp'):
                   if ac.bp.nsta==0: return
                   distp=squeeze(abs((ac.bp.x-bx)+1j*(ac.bp.y-by))); sid=nonzero(distp==distp.min())[0][0]
-                  pie,pip,pacor=self.compute_acor(c_[ac.bp.x[sid],ac.bp.y[sid]]); pzi=(self.dp[pip]*pacor).sum()
-                  print('query: bp depth= {}'.format(pzi))
-            elif dlk==0 and btn==3:
-               pie,pip,pacor=self.compute_acor(c_[bx,by]); pzi=(self.dp[pip]*pacor).sum()
-               print('query: depth= {}'.format(pzi))
+                  px=ac.bp.x[sid]; py=ac.bp.y[sid]; pz=1
+            elif dlk==0 and btn==1:
+               px=bx; py=by; pz=1
             elif dlk==0 and btn==2:
+               self.hqt.remove(); self.hqp.remove(); delattr(self,'hqt'); delattr(self,'hqp'); gcf().canvas.draw()
                gcf().canvas.mpl_disconnect(self.cidquery)
 
+            #annotate text
+            if dlk==0 and (btn in [1,3]) and pz==1:
+               pz=self.interp(c_[px,py],value=self.data if hasattr(self,'data') else self.dp)
+               if not hasattr(self,'hqp'):
+                  self.hqp=plot(px,py,'g^',ms=6,alpha=1)[0]
+                  self.hqt=text(px,py,'',color='orangered',fontsize=12,bbox=dict(facecolor='w',alpha=0.75))
+               self.hqt.set_x(px); self.hqt.set_y(py); self.hqt.set_text(' {}'.format(pz[0]))
+               self.hqp.set_xdata(px); self.hqp.set_ydata(py); gcf().canvas.draw()
+
         acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs])
         abp=acs[nonzero(ats=='query')[0][0]] if 'query' in ats else gcf().canvas.toolbar.addAction('query')
+        if hasattr(self,'hqt'): delattr(self,'hqt')
+        if hasattr(self,'hqp'): delattr(self,'hqp')
         #if not abp.isCheckable(): abp.setCheckable(True)
         abp.triggered.connect(connect_actions)
 
     def show_node(self):
         '''
         show node/element number
         '''
@@ -1348,61 +1537,55 @@
                for i in arange(len(self.hts)): self.hts.pop().remove()
             gcf().canvas.draw()
         acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs]); self.hts=[]
         abp=acs[nonzero(ats=='node')[0][0]] if 'node' in ats else gcf().canvas.toolbar.addAction('node')
         abp.triggered.connect(_show_node)
 
 class schism_bpfile:
-    def __init__(self,x=None,y=None,z=None,station=None):
+    def __init__(self,x=None,y=None,z=None,station=None,fmt=0):
         self.nsta=0; self.x=array([]); self.y=array([]); self.z=array([])
-        self.station=[]; self.hp=[]; self.ht=[]
+        self.station=[]; self.hp=[]; self.ht=[]; self.fmt=fmt
         if x is not None: self.x=x
         if y is not None: self.y=y
         if z is not None: self.z=z
         if station is not None: self.station=station
-        self.edit()
+        self.check(); self.edit()
 
     @property
     def INFO(self):
         return get_INFO(self)
     @property
     def VINFO(self):
         return get_INFO(self)
 
-    def read_reg(self,fname):
-        self.read_bpfile(fname,fmt=1)
-
-    def read_bpfile(self,fname,fmt=0):
-        #read file content
-        lines=[i.strip().split() for i in open(fname,'r').readlines()]
-        stations=[i.strip().split('!')[-1] for i in open(fname,'r').readlines()[2:] if ('!' in i)]
-        if fmt==0:
-            self.nsta=int(lines[1][0])
-            if self.nsta==0: return
-            fc=lambda x: x if len(x)==4 else [*x[:4],x[4][1:]]
-            data=array([fc(line) for line in lines[2:(2+self.nsta)]])
+    def read_reg(self,*args0,**args):
+        self.read(fname,*args0,**args)
 
-            self.x=data[:,1].astype(float)
-            self.y=data[:,2].astype(float)
-            self.z=data[:,3].astype(float)
-        elif fmt==1:
-            self.nsta=int(lines[2][0])
-            if self.nsta==0: return
-            data=squeeze(array([lines[3:]])).astype('float')
-            self.x=data[:,0]
-            self.y=data[:,1]
-            self.z=zeros(self.nsta)
-        else:
-            sys.exit('unknow format')
+    def read_bpfile(self,*args0,**args):
+        self.read(fname,*args0,**args)
 
-        #get unique station data.
-        if len(stations)==self.nsta:
-           self.station=array(stations)
-        else:
-           self.station=array(['{}'.format(i) for i in arange(self.nsta)])
+    def read(self,fname,delimiter='!',fmt=None):
+        '''
+        read SCHISM bpfile or reg file
+        fmt=0: bpfile;  fmt=1: regfile
+        '''
+        #pre-proc
+        lines=[i.strip() for i in open(fname,'r').readlines()]
+        self.fmt=1 if len(lines[2].split())==2 else 0 #check file format
+        if (fmt is not None) and self.fmt!=fmt: sys.exit('fmt is wrong; fmt is not need anymore!')
+
+        if self.fmt==0: #bpfile
+           self.nsta=int(lines[1].split()[0])
+           snames=[i.split(delimiter)[-1] if (delimiter in i) else ''  for i in lines[2:]] #read stations
+           self.station=[] if (len(unique(snames))==1 and snames[0]=='') else array(snames,dtype='U')
+           self.x,self.y,self.z=array([i.split()[1:4] for i in lines[2:(2+self.nsta)]]).astype('float').T
+        else: #regfile
+            self.nsta=int(lines[2].split()[0])
+            self.x,self.y=array([i.split()[:2] for i in lines[3:(3+self.nsta)]]).astype('float').T
+        self.check() 
 
     def write(self,fname,**args):
         '''
         generic fun in saving file in different format (*.bp, *.reg, *.shp)
         when other format is provided, output as *.bp
         '''
         F=None
@@ -1423,67 +1606,69 @@
 
     def write_bpfile(self,fname,fmt=0):
         '''
         fmt=0: write ACE/gredit *.bp file
         fmt=1: write ACE/gredit *.reg file
         '''
 
-        #check data
-        if (not hasattr(self,'nsta')) or (self.nsta==0 and len(self.x)!=0): self.nsta=len(self.x)
-        if (not hasattr(self,'z')) or (len(self.z)==0 and self.nsta!=0): self.z=zeros(self.nsta)
-        if (not hasattr(self,'station')) or (len(self.station)==0 and self.nsta!=0): self.station=array([str(i+1) for i in arange(self.nsta)])
-        self.np=self.nsta
-
-        fid=open(fname,'w+')
+        self.check(); fid=open(fname,'w+')
         #write header
         if hasattr(self,'note'): fid.write('ACE/gredit: {}'.format(self.note))
         if fmt==0: fid.write('bpfile in ACE/gredit format\n{}\n'.format(self.nsta))
         if fmt==1: fid.write('Region in ACE/gredit format\n1\n{} 1\n'.format(self.nsta))
 
         #write pts
         for i in arange(self.nsta):
             if fmt==0: fid.write('{:<d} {:<.8f} {:<.8f} {:<.8f} !{}\n'.format(i+1,self.x[i],self.y[i],self.z[i],self.station[i]))
             if fmt==1: fid.write('{:<.8f} {:<.8f}\n'.format(self.x[i],self.y[i]))
         fid.close()
 
+    def check(self):
+        '''
+        fill up missing field in bpfile based on self.x
+        '''
+        npt=len(self.x); self.nsta=npt; self.npt=npt; nz0=len(self.z); nsta0=len(self.station)
+        if nz0<npt: self.z=r_[array(self.z),zeros(npt-nz0)]
+        if nsta0<npt: self.station=r_[array(self.station,dtype='U'),arange(nsta0+1,npt+1).astype('U')]
+
     def get_unique_pts(self,fmt=0):
         '''
         compute unique pts
-            fmt=0: compute ux,uy,uz,ustation of the point
-            fmt=1: replace (x,y,z,station) by (ux,uy,uz,ustation)
+          fmt=0: unique xy; fmt=1: unique xyz
         '''
-        #get unique locations
-        upxy,sind=unique(self.x+1j*self.y,return_index=True); sind=sort(sind)
-        self.ux=self.x[sind]; self.uy=self.y[sind]
-        self.uz=self.z[sind]; self.ustation=self.station[sind]
-        if fmt==1: self.x,self.y,self.z,self.station,self.nsta=self.ux,self.uy,self.uz,self.ustation,len(self.ux)
+        sind=sort(unique(c_[self.x,self.y] if fmt==0 else c_[self.x,self.y,self.z],axis=0,return_index=True)[1])
+        self.ux,self.uy,self.uz,self.ustation=self.x[sind],self.y[sind],self.z[sind],self.station[sind]
+        self.unsta=self.unpt=len(sind)
         return [self.ux,self.uy,self.uz,self.ustation]
 
     def proj(self,prj0,prj1='epsg:4326',fmt=0,lon0=None,lat0=None):
         '''
         transform the projection of bpfile points' coordinates
         Inputs:
             prj0: projection name of bpfile
             prj1: target projection name; default is 'epsg:4326'
             fmt=0: change bp.x,bp.y to transform xy; fmt=1: only return transformed xy
             lon0,lat0: lon&lat of cpp projection center; needed only if 'cpp' in [prj0,prj1]
                        if ("ll"=>"cpp") and (lon0 or lat0 is not provided): lon0=mean(x); lat0=mean(y)
         '''
-        px,py=proj(prj0=prj0,prj1=prj1,x=self.x,y=self.y,lon0=lon0,lat0=lat0)
+        self.check(); px,py=proj(prj0=prj0,prj1=prj1,x=self.x,y=self.y,lon0=lon0,lat0=lat0)
         if fmt==0: self.x,self.y=px,py
         return [px,py]
 
     def inside(self,xy,fmt=0):
         '''
         check whether pts c_[x,y] are inside the polygon of bp points.
         fmt=0: return indices of pts inside; fmt=1: return boolean flag
+        fmt=2: return indices of pts outside region; fmt=3: return boolean flag outside
         '''
 
         fp=inside_polygon(xy,self.x,self.y)==1
-        return nonzero(fp)[0] if fmt==0 else fp
+        return nonzero(fp)[0] if fmt==0 else fp if fmt==1 else nonzero(~fp)[0] if fmt==2 else ~fp
+    def outside(self,xy,fmt=2):
+        return self.inside(xy,fmt=fmt)
 
     def write_shapefile(self,fname,prj='epsg:4326'):
         self.shp_bp=zdata()
         self.shp_bp.type='POINT'
         self.shp_bp.xy=c_[self.x,self.y]
         self.shp_bp.prj=get_prj_file(prj)
 
@@ -1491,118 +1676,101 @@
             self.shp_bp.attname=['station']
             self.shp_bp.attvalue=self.station
         write_shapefile_data(fname,self.shp_bp)
 
     def plot_station(self,**args):
         return self.plot(**args)
 
-    def plot(self,ax=None,color='r',marker='.',ls=None,label=True,fmt=0,**args):
+    def plot(self,ax=None,color=None,ls=None,label=None,marker='.',markersize=6,fmt=0,connect_mpl=1,**args):
         '''
         plot points on current figure
-          fmt=0: plot all points
-          fmt=1: plot unique points
+          fmt=0: plot all points; fmt=1: plot unique points
         '''
-
-        self.edit()
         #pre-processing
-        if ls is None: ls='None'
-        lc=color if label else 'None'
-        if not None: ax=gca()
-        if fmt==0: sx,sy,sz,stations=self.x,self.y,self.z,self.station
-        if fmt==1: sx,sy,sz,stations=self.get_unique_pts()
+        if connect_mpl==1: self.edit()
+        if color is None: color='r'
+        if ls is None: ls='None' if self.fmt==0 else '-'
+        if label is None: label=1 
+        if ax is None: ax=gca()
+
+        #get pts
+        self.check(); npt,xs,ys,zs,stations=self.npt,self.x,self.y,self.z,self.station
+        if fmt==1: xs,ys,zs,stations=self.get_unique_pts(); npt=len(xs)
+
+        #label
+        if label==1:
+           [i.remove() for i in self.ht]; self.ht=[]
+           for xi,yi,ti in zip(xs,ys,stations): hti=text(xi,yi,ti,color=color,fontsize=10); self.ht.append(hti)
 
         #plot
-        self.hp=[]; self.ht=[]
-        for i,station in enumerate(stations):
-            hpi=plot(sx[i],sy[i],marker=marker,color=color,linestyle=ls,**args); self.hp.append(hpi)
-            hti=text(sx[i],sy[i],station,color=lc); self.ht.append(hti)
-        #show(block=False)
-        return [self.hp,self.ht]
+        if self.fmt==1: #for region file
+           if hasattr(self,'hp2'): self.hp2.remove(); delattr(self,'hp2')
+           if npt>=3: [self.hp2]=fill(xs,ys,facecolor='m',alpha=0.15)
+           if npt!=0: xs=r_[xs,xs[0]]; ys=r_[ys,ys[0]] #close polygon
+        if len(self.hp)!=0: self.hp[0].set_xdata(xs); self.hp[0].set_ydata(ys)
+        if len(self.hp)==0: self.hp=plot(xs,ys,marker=marker,markersize=markersize,color=color,linestyle=ls,**args)
+        gcf().canvas.draw()
 
     def compute_acor(self,gd):
         #compute areal coordinates, and gd is the schism grid
         self.ie,self.ip,self.acor=gd.compute_acor(c_[self.x,self.y])
         return self.ie,self.ip,self.acor
 
+    def disconnect_edit(self):
+        if hasattr(self,'cidpress'): gcf().canvas.mpl_disconnect(self.cidpress)
+        if hasattr(self,'cidmove'):  gcf().canvas.mpl_disconnect(self.cidmove)
+        acs=gcf().canvas.toolbar.actions(); ats=[i.iconText() for i in acs]; ap=acs[ats.index('Pan')]
+        if ap.isChecked(): ap.trigger()
+        gcf().canvas.draw()
+
     def edit(self):
         def connect_actions():
             self.cidmove=gcf().canvas.mpl_connect('motion_notify_event', onmove)
             self.cidpress=gcf().canvas.mpl_connect('button_press_event', onclick)
             if self.nsta!=0 and len(self.hp)==0: self.plot_station()
-            acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs]); ac=acs[nonzero(ats=='Pan')[0][0]]
-            if not ac.isChecked(): ac.trigger()
+            acs=gcf().canvas.toolbar.actions(); ats=[i.iconText() for i in acs]
+            ap=acs[ats.index('Pan')]; ab=acs[ats.index('reg' if self.fmt==0 else 'bp')]
+            if not ap.isChecked(): ap.trigger()
+            if hasattr(ab,'bp'): ab.bp.disconnect_edit()
             gcf().canvas.draw()
             print('double click: left=add pt, right=remove pt; middle=finish edit')
             print('single click: middle=move pt')
 
         def onmove(sp):
             if sp.button is not None:
                dlk=int(sp.dblclick); btn=int(sp.button); bx=sp.xdata; by=sp.ydata
                if dlk==0 and btn==2: move_pt(bx,by)
 
         def onclick(sp):
             dlk=int(sp.dblclick); btn=int(sp.button); bx=sp.xdata; by=sp.ydata
             #double click
             if dlk==1 and btn==1: add_pt(bx,by)
             if dlk==1 and btn==3: remove_pt(bx,by)
-            if dlk==1 and btn==2:
-               gcf().canvas.mpl_disconnect(self.cidpress)
-               gcf().canvas.mpl_disconnect(self.cidmove)
-               acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs]); ac=acs[nonzero(ats=='Pan')[0][0]]
-               if ac.isChecked(): ac.trigger()
-               gcf().canvas.draw()
+            if dlk==1 and btn==2: self.disconnect_edit()
+            if dlk==1 and btn in [1,3]: self.station=(arange(len(self.x))+1).astype('U'); self.plot(connect_mpl=0)
 
         def add_pt(x,y):
-            self.nsta=self.nsta+1; self.station=[*self.station,'{}'.format(self.nsta)]
-            self.x=r_[self.x,x]; self.y=r_[self.y,y]; self.z=r_[self.z,0.0]
-
-            #plot point
-            if len(self.hp)!=0:
-                hp=self.hp[-1][0]; ht=self.ht[-1]
-                color=hp.get_color(); mk=hp.get_marker(); ms=hp.get_markersize(); ls=hp.get_linestyle()
-                fs=ht.get_fontsize(); fw=ht.get_fontweight(); fc=ht.get_color()
-            else:
-                color='r'; mk='.'; ms=6.0; ls='None'; fs=10; fw='normal'; fc='r'
-            hpi=plot(x,y,marker=mk,markersize=ms,color=color,linestyle=ls); self.hp.append(hpi)
-            hti=text(x,y,self.station[-1],color=fc,fontsize=fs,fontweight=fw); self.ht.append(hti)
-            gcf().canvas.draw()
+            self.x=r_[self.x,x]; self.y=r_[self.y,y]; self.plot(connect_mpl=0)
 
         def remove_pt(x,y):
             if self.nsta==0: return
             distp=squeeze(abs((self.x-x)+1j*(self.y-y))); sid=nonzero(distp==distp.min())[0][0]
-            color='r'; mk='.'; ms=6.0; ls='None'; fs=10; fw='normal'; fc='r'
-            for i in arange(sid,self.nsta):
-                if i==self.nsta-1:
-                   self.hp[-1][0].remove(); self.ht[-1].remove()
-                   del self.hp[-1]; del self.ht[-1]
-                else:
-                   xi=self.x[i+1]; yi=self.y[i+1]
-                   self.x[i]=xi; self.y[i]=yi; self.station[i]='{}'.format(i+1)
-                   self.hp[i][0].remove(); self.ht[i].remove()
-                   hpi=plot(xi,yi,marker=mk,markersize=ms,color=color,linestyle=ls); self.hp[i]=hpi
-                   hti=text(xi,yi,self.station[i],color=fc,fontsize=fs,fontweight=fw); self.ht[i]=hti
-            self.x=self.x[:-1]; self.y=self.y[:-1]; self.z=self.z[:-1]; self.station=self.station[:-1]; self.nsta=self.nsta-1
-            gcf().canvas.draw()
+            self.x=r_[self.x[:sid],self.x[(sid+1):]]; self.y=r_[self.y[:sid],self.y[(sid+1):]]; self.plot()
 
         def move_pt(xi,yi):
             distp=squeeze(abs((self.x-xi)+1j*(self.y-yi))); sid=nonzero(distp==distp.min())[0][0]
-            color='r'; mk='.'; ms=6.0; ls='None'; fs=10; fw='normal'; fc='r'
-            self.x[sid]=xi; self.y[sid]=yi
-            self.hp[sid][0].remove(); self.ht[sid].remove()
-            hpi=plot(xi,yi,marker=mk,markersize=ms,color=color,linestyle=ls); self.hp[sid]=hpi
-            hti=text(xi,yi,self.station[sid],color=fc,fontsize=fs,fontweight=fw); self.ht[sid]=hti
-            gcf().canvas.draw()
+            self.x[sid]=xi; self.y[sid]=yi; self.plot()
 
         if mpl._pylab_helpers.Gcf.get_active() is not None:
-            acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs])
-            abp=acs[nonzero(ats=='bp')[0][0]] if 'bp' in ats else gcf().canvas.toolbar.addAction('bp')
+            acs=gcf().canvas.toolbar.actions(); ats=array([i.iconText() for i in acs]); at='bp' if self.fmt==0 else 'reg'
+            abp=acs[nonzero(ats==at)[0][0]] if at in ats else gcf().canvas.toolbar.addAction(at)
             #if not abp.isCheckable(): abp.setCheckable(True)
 
             #disconnect and clean previous bpfile
-            if hasattr(abp,'bp'):
+            if hasattr(abp,at):
                if self is not abp.bp:
                   nhp=len(abp.bp.hp)
                   for i in arange(nhp):
                       abp.bp.hp[-1][0].remove(); abp.bp.ht[-1].remove()
                       del abp.bp.hp[-1],abp.bp.ht[-1]
                abp.triggered.disconnect()
 
@@ -1614,34 +1782,35 @@
     gd=schism_grid(); gd.read_hgrid(fname)
     return gd
 
 def read_schism_bpfile(fname,fmt=0):
     '''
     read schism *bp (fmt=0) or *.reg (fmt=1) file created by ACE/gredit
     '''
-    bp=schism_bpfile(); bp.read_bpfile(fname,fmt=fmt)
+    bp=schism_bpfile(); bp.read(fname); bp.edit()
+    return bp
+
+def read_schism_reg(fname):
+    '''
+    read schism *bp (fmt=0) or *.reg (fmt=1) file created by ACE/gredit
+    '''
+    bp=schism_bpfile(); bp.read(fname); bp.edit()
     return bp
 
 def read_schism_prop(fname):
     '''
     read schism *.prop file (element based), and return the values
     '''
     try:
       pdata=loadtxt(fname)
     except:
       pdata=array([i.strip().split() for i in open(fname,'r').readlines() if len(i.split())==2]).astype('float')
     pvalue=pdata[:,1] if pdata.ndim==2 else pdata[None,:][:,1]
     return pvalue
 
-def read_schism_reg(fname):
-    '''
-    read schism *.reg file created by ACE/gredit
-    '''
-    return read_schism_bpfile(fname,fmt=1)
-
 def save_schism_grid(fmt=0,path='.',method=0):
     '''
     save schism grid information in *.npz format (hgrid.gr3,hgrid.ll,vgrid.in}
        path:  directory of grids
        fmt=0: save as grid.npz (include hgrid and vgrid); fmt=1: save as hgrid.npz and vgrid.npz
        method=1: save hgrid full geometry information
     '''
@@ -2199,17 +2368,25 @@
     elnode=array([ip[:-1,:-1],ip[:-1,1:],ip[1:,1:],ip[1:,:-1]]).reshape([4,(nvrt-1)*(npt-1)]).T #all quads
     y=ys.ravel()[elnode]; fp=(y[:,0]==y[:,3])*(y[:,1]==y[:,2]); elnode=elnode[~fp]; p=elnode #valid quads
     sindp,sindv=unique(elnode,return_inverse=True) #get unique points
     gd.x,gd.y,gd.dp=xs.ravel()[sindp],ys.ravel()[sindp],vs.ravel()[sindp]
     elnode=arange(sindp.size)[sindv].reshape(elnode.shape) #renumber node index
     p=elnode; p[p[:,3]==p[:,0],3]=-2; p[p[:,2]==p[:,1],2]=-2; fp=p[:,2]==-2; p[fp]=p[fp][:,array([3,0,1,2])] #for triangle
     gd.elnode=elnode; gd.np,gd.ne=len(gd.x),len(gd.elnode); gd.i34=sum(gd.elnode!=-2,axis=1)
+    gd.compute_area(); fp3=(gd.i34==3)*(gd.area<0); fp4=(gd.i34==4)*(gd.area<0)
+    gd.elnode[fp3,:3]=gd.elnode[fp3,2::-1]; gd.elnode[fp4,:]=gd.elnode[fp4,::-1]; gd.compute_area()
 
     return gd
 
+def compute_schism_volume(hgrid,vgrid,fmt=0,value=None,eta=None):
+    '''
+    compute volume or volume*value for schism grid; see help from gd.compute_volume
+    '''
+    return hgrid.compute_volume(vgrid,fmt,value,eta)
+
 def scatter_to_schism_grid(xyz,angle_min=None,area_max=None,side_min=None,side_max=None,reg_in=None,reg_out=None):
     '''
     create schism grid from scatter pts
         xyz: c_[x,y] or c_[x,y,z]
         angle_min: remove element with internal_angle < angle_min
         area_max:  remove element with element_area   > area_max
         side_min:  remove element with side_length    < side_min
@@ -2219,17 +2396,18 @@
     '''
 
     #get xyz
     x,y=xyz.T[:2]; np=len(x)
     z=xyz[:,2] if xyz.shape[1]>=3 else zeros(np)
 
     #triangulate scatter
-    tr=mpl.tri.Triangulation(x,y); gd=schism_grid()
-    gd.np,gd.ne=np,len(tr.triangles); gd.x,gd.y,gd.dp=x,y,z
-    gd.elnode=c_[tr.triangles,-2*ones([gd.ne,1])].astype('int'); gd.i34=3*ones(gd.ne).astype('int')
+    gd=schism_grid(); gd.x,gd.y,gd.dp=x,y,z; gd.np=len(gd.x)
+    #tr=sp.spatial.Delaunay(c_[x,y]); gd.elnode=tr.simplices #method 1
+    tr=mpl.tri.Triangulation(x,y); gd.elnode=unique(tr.triangles,axis=0) #method 2
+    gd.ne=len(gd.elnode); gd.elnode=resize(gd.elnode,[gd.ne,4],-2); gd.i34=tile(3,gd.ne)
 
     #clean mesh
     gd=delete_schism_grid_element(gd,angle_min=angle_min,area_max=area_max,side_min=side_min,side_max=side_max,reg_in=reg_in,reg_out=reg_out)
     return gd
 
 def delete_schism_grid_element(gd,angle_min=5,area_max=None,side_min=None,side_max=None,reg_in=None,reg_out=None,method=0):
     '''
@@ -2240,74 +2418,68 @@
         side_min:  remove element with side_length    < side_min
         side_max:  remove element with side_length    > side_max
         reg_in:    ACE/xgredit region file. remove elements in region if reg_in is provided
         reg_out:   ACE/xgredit region file. remove elements outside of region if reg_out is provided
         method=0: use side_max for dangling pts; method=1: use angle_min for dangling pts
     '''
 
-    #find max/min side or angle values
-    angles,sides=[],[];  fp3=gd.i34==3; fp4=gd.i34==4
-    id1,id2,id3=ones([3,gd.ne]).astype('int'); sid=arange(gd.ne)
-    for i in arange(4):
-        id1[fp3]=i%3; id2[fp3]=(i+1)%3; id3[fp3]=(i+2)%3
-        id1[fp4]=i%4; id2[fp4]=(i+1)%4; id3[fp4]=(i+2)%4
-        x1=gd.x[gd.elnode[sid,id1]]; x2=gd.x[gd.elnode[sid,id2]]; x3=gd.x[gd.elnode[sid,id3]]
-        y1=gd.y[gd.elnode[sid,id1]]; y2=gd.y[gd.elnode[sid,id2]]; y3=gd.y[gd.elnode[sid,id3]]
-        ai=abs(angle((x1-x2)+1j*(y1-y2))-angle((x3-x2)+1j*(y3-y2)))*180/pi; angles.append(ai)
-        si=abs((x1+1j*y1)-(x2+1j*y2)); sides.append(si)
-    angles=array(angles).T; sides=array(sides)
-    mangle=angles.min(axis=1); sidemin=sides.min(axis=0); sidemax=sides.max(axis=0)
-
-    #filter illegal elements
-    gd.compute_area(); gd.compute_ctr()
-    fangle=nonzero(mangle<angle_min)[0] if (angle_min is not None) else array([])
-    farea=nonzero(gd.area>area_max)[0] if (area_max is not None) else array([])
-    fside_max=nonzero(sidemax>side_max)[0] if (side_max is not None) else array([])
-    fside_min=nonzero(sidemin<side_min)[0] if (side_min is not None) else array([])
-    sindp=r_[fangle,farea,fside_max,fside_min].astype('int')
-
-    #filter elements inside region
-    if (reg_in is not None) and len(sindp)!=0:
-        if isinstance(reg_in,str): bp=read_schism_bpfile(reg_in,fmt=1); reg_in=c_[bp.x,bp.y]
-        print(reg_in.shape); sys.exit()
-        fpr=inside_polygon(c_[gd.xctr[sindp],gd.yctr[sindp]],reg_in[:,0],reg_in[:,1])==1; sindp=sindp[fpr]
-
-    #filter elements outside region
-    if reg_out is not None:
-        if isinstance(reg_out,str): bp=read_schism_bpfile(reg_out,fmt=1); reg_out=c_[bp.x,bp.y]
-        sindo=nonzero(inside_polygon(c_[gd.xctr,gd.yctr],reg_out[:,0],reg_out[:,1])==0)[0]; sindp=r_[sindp,sindo]
-
-    sind=setdiff1d(arange(gd.ne),sindp)
-
-    #add back elements with dangling pts
-    ips=setdiff1d(arange(gd.np),unique(gd.elnode[sind].ravel()))
-    if len(ips)!=0:
-        gd.compute_nne(); sinde=[]
-        for ip in ips:
-            ies=gd.indel[ip]
-            if method==0: ai=sidemax[ies]; sinde.append(ies[nonzero(ai==min(ai))[0][0]])
-            if method==1: ai=mangle[ies]; sinde.append(ies[nonzero(ai==max(ai))[0][0]])
-        sind=sort(r_[sind,array(sinde)])
-
-    #delete elements
-    gd.ne,gd.i34,gd.elnode=len(sind),gd.i34[sind],gd.elnode[sind]
-    gd.area,gd.xctr,gd.yctr,gd.dpe=gd.area[sind],gd.xctr[sind],gd.yctr[sind],gd.dpe[sind]
+    fpe=tile(True,gd.ne)
+    if angle_min is not None: #check min angle
+        if not hasattr(gd,'angles'): gd.compute_angle()
+        fpe=fpe*(gd.angles.min(axis=1)>=angle_min)
+
+    if area_max is not None: #check maximum area
+        if not hasattr(gd,'area'): gd.compute_area()
+        fpe=fpe*(gd.area<=area_max)
+
+    if (side_min is not None) or (side_max is not None): #check side length
+        slen=[]; ie=arange(gd.ne)
+        for n in arange(4):
+            i1=gd.elnode[ie,n%gd.i34]; i2=gd.elnode[ie,(n+1)%gd.i34]
+            slen.append(abs((gd.x[i2]-gd.x[i1])+1j*(gd.y[i2]-gd.y[i1])))
+        slen=array(slen).T
+        if side_min is not None: fpe=fpe*(slen.min(axis=1)>=side_min)
+        if side_max is not None: fpe=fpe*(slen.max(axis=1)<=side_max)
+
+    for m in arange(2): #check region inside and outside
+        regs=reg_in if m==0 else reg_out
+        if regs is not None:
+            if not hasattr(gd,'xctr'): gd.compute_ctr()
+            if isinstance(regs,str) or array(regs[0]).ndim==1: regs=[regs]
+            for n,rxy in enumerate(regs):
+                if isinstance(rxy,str): bp=read(rxy); rxy=c_[bp.x,bp.y]
+                fpe=fpe*(inside_polygon(c_[gd.xctr,gd.yctr], rxy[:,0],rxy[:,1])==(0 if m==0 else 1))
+
+    #add back one element if nodal is zero
+    ip=unique(gd.elnode[fpe])[1:]
+    if ip.size<gd.np:
+       if not hasattr(gd, 'ine'): gd.compute_nne()
+       if not hasattr(gd,'angles'): gd.compute_angle()
+       sindp=setdiff1d(arange(gd.np),ip); sinde=gd.ine[sindp]; fpn=sinde==-1
+       A=gd.angles[sinde]; dA=A.max(axis=2)-A.min(axis=2); dA[fpn]=1e3
+       ie=sinde[arange(len(sinde)),dA.argmin(axis=1)]; fpe[ie]=True
+
+    #delete elements and update grid
+    gd.ne=sum(fpe); gd.i34=gd.i34[fpe]; gd.elnode=gd.elnode[fpe]
+    if hasattr(gd,'angles'): gd.angles=gd.angles[fpe]
+    if hasattr(gd,'area'): gd.angles=gd.area[fpe]
+    if hasattr(gd,'xctr'): gd.xctr=gd.xctr[fpe]; gd.yctr=gd.yctr[fpe]; gd.dpe=gd.dpe[fpe]
+    gd.compute_nne()
     return gd
 
 def combine_icm_output(rundir='.',sname='icm.nc',fmt=0,outfmt=0):
     '''
     combine schism-icm station outputs
       rundir: run directory
       sname: save name for combined output
       fmt=1: copy subdomain output file, and then read
       outfmt=0: float32;  outfmt=1: float64
     '''
     from time import time as gettime
     from shutil import copyfile
-    from glob import glob
     from netCDF4 import Dataset
 
     outdir=rundir+'/outputs/'
     bp=read_schism_bpfile(rundir+'/istation.in')
     fid=Dataset(outdir+sname,'w',format='NETCDF4'); fvar=fid.variables; fdim=fid.dimensions
 
     #get fnames information
@@ -2355,15 +2527,15 @@
         if fmt==1: os.remove(fname)
     fid.close()
 
 def combine_schism_hotstart(outdir='.',fmt=0,irec=None):
     '''
     combine schism hotstart
        outdir: schism output directory
-       fmt=0: combine the last hotstart; fmt=1: combine all hotstart
+       fmt=0: combine the last hotstart; fmt=1: combine all hotstart, skip combined; fmt=2: re-combine all
        irec: step number of hotstrat (fmt is disabled when irec is set)
     '''
     from netCDF4 import Dataset
 
     #get all hotstart records
     irecs=sort([int(i[:-3].split('_')[-1]) for i in os.listdir(outdir) if i.startswith('hotstart_000000_')])
     if fmt==0: irecs=irecs[-1:]
@@ -2372,15 +2544,17 @@
     #get subdomain information
     S=get_schism_output_info(outdir,fmt=2); dname=['nResident_node','nResident_elem','nResident_side']
     dnn=['node','elem','side']; dsn=[S.npg,S.neg,S.nsg] #global dim
 
     fnames=[]
     for m,irec in enumerate(irecs):
         fname='hotstart.nc_{}'.format(irec); fnames.append(fname)
+        if fmt==1 and os.path.exists(outdir+'/'+fname): continue
         fid=Dataset(outdir+'/'+fname,'w',format='NETCDF4');  #open file
+        print('combining '+fname)
         for n in arange(S.nproc):  #assemble subdomain information
             C=ReadNC('{}/hotstart_{:06}_{}.nc'.format(outdir,n,irec),1)
             cvar=C.variables; cdim=C.dimensions
 
             #def dimension and variables
             if n==0:
                dn=[*cdim]; ds=[cdim[i].size for i in dn]                    #dim. name and size
@@ -2476,31 +2650,33 @@
           if vd[0]=='time' and len(vd)>1:
              for n,k in enumerate(cvar[i][:]): fid.variables[i][n]=_subset(vd[1],k,1)
           else:
              fid.variables[i][:]=_subset(vd[0],cvar[i][:],1)
    fid.close(); C.close()
    return gd
 
-def read_schism_output(run,varname,xyz,stacks=None,ifs=0,nspool=1,sname=None,fname=None,hgrid=None,vgrid=None,fmt=0,extend=0,prj=None,zcor=0):
+def read_schism_output(run,varname,xyz,stacks=None,ifs=0,nspool=1,sname=None,fname=None,hgrid=None,vgrid=None,fmt=0,mdt=None,extend=0,prj=None,zcor=0,sgrid=None):
     '''
     extract time series of SCHISM results @xyz or transects @xy (works for scribe IO and combined oldIO)
        run:     run directory where (grid.npz or hgrid.gr3) and outputs are located
        varname: variables to be extracted; accept shortname(s) or fullname(s) (elev, hvel, horizontalVelX, NO3, ICM_NO3, etc. )
        xyz:     c_[x,y,z], or bpfile, or c_[x,y]
        fmt:     (optional) 0: read time series @xyz;     1: read transect @xy
        stacks:  (optional) output stacks to be extract; all avaiable stacks will be extracted if not specified
        ifs=0:   (optional) extract results @xyz refers to free surface (default); ifs=1: refer to fixed levels
        nspool:  (optional) sub-sampling frequency within each stack (npsool=1 means all records)
+       mdt:     (optional) time window (day) for averaging output
        sname:   (optional) variable name for save
        fname:   (optional) save the results as fname.npz
        hgrid:   (optional) hgrid=read_schism_hgrid('hgrid.gr3'); hgrid.compute_all(); used to speed up
        vgrid:   (optional) vgrid=read_schism_vgrid('vgrid.in'); used to speed up
        extend:  (optional) 0: extend bottom value beyond;  1: assign nan for value beyond bottom
        prj:     (optional) used to tranform xy (e.g. prj=['epsg:26918','epsg:4326'])
        zcor:    (optional) 0: zcoordinate computed from elev;  1: read from outputs
+       sgrid:   (optional) side-based grid used to extract side values (FEM method); see gd.scatter_to_grid(fmt=2)
     '''
 
     #get schism outputs information
     bdir=run+'/outputs'; modules,outfmt,dstacks,dvars,dvars_2d =get_schism_output_info(bdir,1)
 
     #variables
     if isinstance(varname,str): varname=[varname]
@@ -2513,20 +2689,24 @@
 
     #read station coordinates (xyz)
     if isinstance(xyz,str): bp=read_schism_bpfile(xyz); xyz=c_[bp.x,bp.y,bp.z]
     if array(xyz).ndim==1: xyz=array(xyz)[None,:]
     lx,ly=xyz.T[:2]; npt=len(lx); lz=xyz.T[2] if xyz.shape[1]==3 else zeros(npt)
     if prj is not None: lx,ly=proj_pts(lx,ly,prj[0],prj[1])
     pie,pip,pacor=gd.compute_acor(c_[lx,ly]); pip,pacor=pip.T,pacor.T; P=zdata()
-    def _sindex(): #for output@side
-        if not hasattr(gd,'nns'): gd.compute_side(fmt=2)
-        if not hasattr(P,'nns'): P.nns,P.ins=gd.nns[pip],gd.ins[pip]; P.ds=P.ins.shape; P.fp=P.ins!=0
+    def _sindex(sgrid,P): #for output@side
+        if sgrid is None:
+           if not hasattr(gd,'nns'): gd.compute_side(fmt=2)
+           if not hasattr(P,'nns'): P.nns,P.ins=gd.nns[pip],gd.ins[pip]; P.ds=P.ins.shape; P.fp=P.ins!=0
+        else:
+           if isinstance(sgrid,int): sgrid=gd.scatter_to_grid(fmt=2)
+           if not hasattr(P,'pie'): P.pie,P.pip,P.pacor=sgrid.compute_acor(c_[lx,ly])
 
-    #extract time series@xyz
-    S=zdata(); mtime=[]; mdata=[[] for i in varname]
+    #extract time series@xyz or transect@xy
+    mtime=[]; mdata=[[] for i in varname]
     stacks=dstacks if (stacks is None) else [*array(stacks).ravel()] #check outputs stacks
     for istack in stacks:
         print('reading stack: {}'.format(istack))
         C0=ReadNC('{}/{}_{}.nc'.format(bdir,'out2d' if outfmt==0 else 'schout',istack),1)
         if fmt==0 and zcor==1: #open zcoordinates channel
             if outfmt==0:
               Z0=ReadNC('{}/zCoordinates_{}.nc'.format(bdir,istack),1); Z=Z0.variables['zCoordinates']
@@ -2536,17 +2716,19 @@
         if istack==stacks[0]: nvrt=C0.dimensions['nSCHISM_vgrid_layers'].size
 
         for m,varnamei in enumerate(varname):
             vs=[]; svars=get_schism_var_info(varnamei,modules,fmt=outfmt) #get variable information
             for n,[vari,svar] in enumerate(svars):
                 if svar in dvars_2d: #2D
                     C=C0.variables[svar]; np=C.shape[1]
+                    if np==gd.ns: _sindex(sgrid,P)
                     if np==gd.np: vi=array([(array([C[i,j] for j in pip])*pacor).sum(axis=0) for i in arange(0,nt,nspool)])
                     if np==gd.ne: vi=array([C[i,pie] for i in arange(0,nt,nspool)])
-                    if np==gd.ns: _sindex(); vi=array([(sum(array(C[i,P.ins.ravel()]).reshape(P.ds)*P.fp,axis=2)*pacor/P.nns).sum(axis=0) for i in arange(0,nt,nspool)])
+                    if (np==gd.ns) and (sgrid is None): vi=array([(sum(array(C[i,P.ins.ravel()]).reshape(P.ds)*P.fp,axis=2)*pacor/P.nns).sum(axis=0) for i in arange(0,nt,nspool)])
+                    if (np==gd.ns) and (sgrid is not None): vi=array([sum(array(C[i][P.pip]*P.pacor),axis=1) for i in arange(0,nt,nspool)])
                     vs.append(vi)
                 else: #3D
                     #read zcoor,and extend zcoor downward
                     if (zii is None) and fmt==0:
                        if n==0:
                           if zcor==0:
                              eta=array([C0['elevation'][i][pip] for i in arange(0,nt,nspool)]).ravel(); sindp=tile(pip,[ntime,1,1]).ravel()
@@ -2556,127 +2738,122 @@
                              zii=(array([array(Z[i])[pip] for i in arange(0,nt,nspool)])*pacor[None,...,None]).sum(axis=1).transpose([2,0,1])
                        for k in arange(nvrt-1): z1=zii[nvrt-k-2]; z2=zii[nvrt-k-1]; z1[abs(z1)>1e8]=z2[abs(z1)>1e8]
                        if ifs==0: zii=zii-zii[-1][None,...]
 
                     #read data for the whole vertical
                     C1=ReadNC('{}/{}_{}.nc'.format(bdir,svar,istack),1) if outfmt==0 else C0
                     C=C1.variables[svar]; np=C.shape[1]; nd=C.ndim
-                    if np==gd.np and nd==3: vii=(array([array(C[i])[pip] for i in arange(0,nt,nspool)])*pacor[None,...,None]).sum(axis=1).transpose([2,0,1])
-                    if np==gd.np and nd==4: vii=(array([array(C[i])[pip] for i in arange(0,nt,nspool)])*pacor[None,...,None,None]).sum(axis=1).transpose([2,0,1,3])
-                    if np==gd.ne: vii=array([C[i][pie] for i in arange(0,nt,nspool)]).transpose([2,0,1])
-                    if np==gd.ns: _sindex(); vii=array([[(sum(array(C[i,P.ins.ravel(),k]).reshape(P.ds)*P.fp,axis=2)*pacor/P.nns).sum(axis=0) for k in arange(nvrt)] for i in arange(0,nt,nspool)]).transpose([1,0,2])
+                    if np==gd.ns: _sindex(sgrid,P)
+                    if np==gd.np and nd==3: vii=(array([array(C[i])[pip] for i in arange(0,nt,nspool)])*pacor[None,...,None]).sum(axis=1)
+                    if np==gd.np and nd==4: vii=(array([array(C[i])[pip] for i in arange(0,nt,nspool)])*pacor[None,...,None,None]).sum(axis=1)
+                    if np==gd.ne: vii=array([C[i][pie] for i in arange(0,nt,nspool)])
+                    if (np==gd.ns) and (sgrid is None): vii=array([(sum(C[i][P.ins]*P.fp[...,None],axis=2)*pacor[...,None]/P.nns[...,None]).sum(axis=0) for i in arange(0,nt,nspool)])
+                    if (np==gd.ns) and (sgrid is not None): vii=array([sum(C[i][P.pip]*P.pacor[...,None],axis=1) for i in arange(0,nt,nspool)])
+                    vii=vii.transpose([2,0,1]) if nd==3 else vii.tranpose([2,0,1,3]) #from (nt,npt,nvrt) to (nvrt,nt,npt)
                     if extend==0:
-                       for k in arange(nvrt-1): z1=vii[nvrt-k-2]; z2=vii[nvrt-k-1]; z1[abs(z1)>1e8]=z2[abs(z1)>1e8] #extend value at bottom
+                       for k in arange(nvrt-1)[::-1]: z1=vii[k]; z2=vii[k+1]; fpn=abs(z1)>1e8; z1[fpn]=z2[fpn] #extend value at bottom
                     else:
                        fpn=abs(vii)>1e8; vii[fpn]=nan
                     if outfmt==0: C1.close()
 
                     #interp in the vertical
                     if fmt==0: #time series
-                       for ivs in arange(2):
-                           if ivs==1 and nd==3: continue
-                           viii=vii if nd==3 else vii[:,:,:,ivs]
-                           vi=ones([nrec,npt]); zm=-tile(lz,[nrec,1]); dz=1e-10
-                           ziii=zii[-1]-dz; fpz=zm>ziii; zm[fpz]=ziii[fpz]
-                           ziii=zii[0] +dz; fpz=zm<ziii; zm[fpz]=ziii[fpz]
-                           for k in arange(nvrt-1):
-                               z1=zii[k]; z2=zii[k+1]; v1=viii[k]; v2=viii[k+1]; fpz=(zm>z1)*(zm<=z2)
-                               if sum(fpz)!=0: vi[fpz]=v1[fpz]+(v2[fpz]-v1[fpz])*(zm[fpz]-z1[fpz])/(z2[fpz]-z1[fpz])
-                           vs.append(vi)
+                       vii=interp_vertical(vii,zii,-lz[None,None,:]); vs.append(vii)
+                       if nd==4: vs=vs[0].transpose([2,0,1])
                     else: #transect
                        if nd==3: vs.append(vii)
                        if nd==4: vs.append(vii[...,0]); vs.append(vii[...,1])
-            mdata[m].extend(array(vs).transpose([1,2,0])) if (fmt==0 or (svar in dvars_2d)) else mdata[m].extend(array(vs).transpose([2,3,1,0]))
+            mdata[m].extend(array(vs).transpose([1,2,0])) if (fmt==0 or (svar in dvars_2d))*(array(vs).ndim==3) else mdata[m].extend(array(vs).transpose([2,3,1,0]))
         C0.close()
         if fmt==0 and outfmt==0 and zcor==1: Z0.close()
 
     #save data
-    if sname is None: sname=varname
-    for m,k in enumerate(sname):
-        if array(mdata[m]).ndim==3: S.__dict__[k]=squeeze(array(mdata[m]).transpose([1,0,2]))
-        if array(mdata[m]).ndim==4: S.__dict__[k]=squeeze(array(mdata[m]).transpose([1,0,2,3]))
-    S.time=array(mtime)
-    if fname is not None: savez(fname,S)
+    S=zdata(); sdict=S.__dict__; mt=array(mtime); mdata=[array(i) for i in mdata]
+    for m,k in enumerate(varname if sname is None else sname):
+        vi=mdata[m] if (mdt is None) else array([mdata[m][(mt>=i)*(mt<(i+mdt))].mean(axis=0) for i in arange(mt[0],mt[-1],mdt)]) #average
+        sdict[k]=squeeze(vi.transpose([1,0,2] if vi.ndim==3 else [1,0,2,3]))
+    S.time=mt if (mdt is None) else array([mt[(mt>=i)*(mt<(i+mdt))].mean() for i in arange(mt[0],mt[-1],mdt)]) #average
+    if fname is not None: S.save(fname)
     return S
 
-def read_schism_slab(run,varname,levels,stacks=None,nspool=1,mdt=None,sname=None,fname=None):
+def read_schism_slab(run,varname,levels,stacks=None,nspool=1,mdt=None,sname=None,fname=None,reg=None):
     '''
     extract slabs of SCHISM results (works for scribe IO and combined oldIO)
        run:     run directory where (grid.npz or hgrid.gr3,vgrid.in) and outputs are located
        varname: variables to be extracted; accept shortname(s) or fullname(s) (elev, hvel, horizontalVelX, NO3, ICM_NO3, etc. )
-       levels:  schism level indices (1-nvrt: surface-bottom; (>nvrt): kbp level)
+       levels:  schism level indices (1-nvrt: surface-bottom; (>nvrt): kbp level; "all": all layers)
        stacks:  (optional) output stacks to be extract; all avaiable stacks will be extracted if not specified
        nspool:  (optional) sub-sampling frequency within each stack (npsool=1 means all records)
        mdt:     (optional) time window (day) for averaging output
        sname:   (optional) variable name for save
        fname:   (optional) save the results as fname.npz
+       reg:     (optional) subsetting reslts inside region (*.reg, or *.bp, or gd_subgrid)
     '''
     #proc
+    fgz=run+'/grid.npz'; fgd=run+'/hgrid.gr3'; fvd=run+'/vgrid.in'; fexist=os.path.exists; P=zdata()
     bdir=run+'/outputs'; modules,outfmt,dstacks,dvars,dvars_2d =get_schism_output_info(bdir,1)
+    gd=read(fgz,'hgrid') if fexist(fgz) else read(fgd); np,ne,ns=gd.np,gd.ne,gd.ns
     if isinstance(varname,str): varname=[varname]
     if sname is None: sname=varname
     if stacks is None: stacks=dstacks
     if outfmt==1: sys.exit('OLDIO not supported yet')
+    if reg is not None: #build subgrid
+       sgd=gd.subset(reg) if isinstance(reg,str) else reg; sindp,sinde,sinds=sgd.sindp,sgd.sinde,sgd.sinds
 
     #read output
-    S=zdata(); sdict=S.__dict__; sdict['time']=[]; S.levels=array(levels)
-    for i in sname: sdict[i]=[]
+    mtime=[]; mdata=[[] for i in varname]
     for istack in [*unique(stacks).ravel()]:
         if outfmt==0:
            C0=ReadNC('{}/out2d_{}.nc'.format(bdir,istack),1); nvrt=C0.dimensions['nSCHISM_vgrid_layers'].size
-           #np=C0.dimensions['nSCHISM_hgrid_node'].size; ne=C0.dimensions['nSCHISM_hgrid_face'].size
-           mt=array(C0.variables['time'][:])/86400; nt=len(mt); sdict['time'].extend(mt[::nspool])
+           mt=array(C0.variables['time'][:])/86400; nt=len(mt); mtime.extend(mt[::nspool])
+           zs=arange(nvrt,0,-1) if levels=='all' else array(levels)
 
-        for snamei,varnamei in zip(sname,varname):
-            svars=get_schism_var_info(varnamei,modules,fmt=outfmt); nvar=len(svars)
+        for ivar, varnamei in enumerate(varname):
+            svars=get_schism_var_info(varnamei,modules,fmt=outfmt)
             for m,[vari,svar] in enumerate(svars):
+                C=C0 if (svar in dvars_2d) else read('{}/{}_{}.nc'.format(bdir,svar,istack),1); cvar=C.variables[svar]; vi=[]
                 if svar in dvars_2d:  #2D
-                   A=array([array(C0.variables[svar][i]).astype('float32') for i in arange(nt) if i%nspool==0])
+                   vi=array([array(cvar[i]).astype('float32') for i in arange(nt) if i%nspool==0])
+                   if reg is not None: npt=cvar.shape[1]; vi=vi[:,sindp if npt==np else sinde if npt==ne else sinds] #subset
                 else:   #3D
-                   C=ReadNC('{}/{}_{}.nc'.format(bdir,svar,istack),1); A=[]
-                   for n,k in enumerate(levels):
-                       if ('kbp' not in locals()) and (k>nvrt): #get bottom index
-                          grd=run+'grid.npz'; vd=loadz(grd,['vgrid']).vgrid if os.path.exists(grd) else read_schism_vgrid(run+'/vgrid.in')
-                          sindp=arange(vd.np); kbp=vd.kbp
+                   for n,k in enumerate(zs):
                        if k>nvrt:
-                          a=array([array(C.variables[svar][i][sindp,kbp]).astype('float32') for i in arange(nt) if i%nspool==0])
+                          if not hasattr(P,'kbp'): vd=read(fgz,'vgrid') if fexist(fgz) else read(fvd); P.sindp,P.kbp=arange(np),vd.kbp
+                          vii=array([array(cvar[i][P.sindp,P.kbp]).astype('float32') for i in arange(nt) if i%nspool==0])
                        else:
-                          a=array([array(C.variables[svar][i,:,nvrt-k]).astype('float32') for i in arange(nt) if i%nspool==0])
-                       A.append(a)
-                   A=A[0] if len(levels)==1 else array(A).transpose([1,0,2]); C.close()
-                datai=A if m==0 else c_[datai[...,None],A[...,None]]
-            S.__dict__[snamei].extend(datai)
+                          vii=array([array(cvar[i,:,nvrt-k]).astype('float32') for i in arange(nt) if i%nspool==0])
+                       if reg is not None: npt=cvar.shape[1]; vii=vii[:,sindp if npt==np else sinde if npt==ne else sinds] #subset
+                       vi.append(vii)
+                   vi=vi[0] if len(zs)==1 else array(vi).transpose([1,0,2]); C.close()
+                vs=vi if m==0 else c_[vs[...,None],vi[...,None]]
+            mdata[ivar].extend(vs)
         C0.close()
-    sind=argsort(array(S.time))
-    for i in ['time',*sname]: sdict[i]=array(sdict[i])[sind]
-
-    #average data
-    if mdt is not None:
-       M=zdata(); mdict=M.__dict__
-       for i in ['time',*sname]: mdict[i]=[]
-       for ti in arange(S.time[0],S.time[-1],mdt):
-           fpt=(S.time>=ti)*(S.time<(ti+mdt))
-           for i in ['time',*sname]: mdict[i].append(sdict[i][fpt].mean(axis=0))
-       for i in ['time',*sname]: mdict[i]=array(mdict[i])
-       S=M
 
     #save data
-    if fname is not None: savez(fname,S)
+    S=zdata(); sdict=S.__dict__; S.zs=array(zs); mt=array(mtime); mdata=[array(i) for i in mdata]
+    for m, k in enumerate(sname):
+        sdict[k]=mdata[m] if (mdt is None) else array([mdata[m][(mt>=i)*(mt<(i+mdt))].mean(axis=0) for i in arange(mt[0],mt[-1],mdt)])
+    sdict['time']=mt if (mdt is None) else array([mt[(mt>=i)*(mt<(i+mdt))].mean() for i in arange(mt[0],mt[-1],mdt)])
+    if reg is not None: S.gd=sgd
+    if fname is not None: S.save(fname)
     return S
 
 def get_schism_output_info(run,fmt=0):
     '''
     get info. about SCHISM ["modules", "output format", "stacks", "output variables", "output 2D variables"]
     Inputs:
         run:  SCHISM outputs directory
         fmt=0: remove schsim default variables related to grid; fmt=1: not remove
 
     Outputs:
         fmt=0/1: [modules,outfmt,stacks,svars,svars_2d]
         fmt=2: information about domain-decomposition
+        fmt=3: gather run information
+        fmt=4: return reconstructed SCHISM hgrid
+        (Note: fmt=3/4 works for new schism outputs)
     '''
 
     if fmt in [0,1]:
        #default variables to be excluded
        dvars=('out2d','schout','time','minimum_depth','SCHISM_hgrid','crs','SCHISM_hgrid_node_x','SCHISM_hgrid_node_y',
               'depth','bottom_index_node','SCHISM_hgrid_face_x','SCHISM_hgrid_face_y','SCHISM_hgrid_edge_x',
               'SCHISM_hgrid_edge_y','SCHISM_hgrid_face_nodes','SCHISM_hgrid_edge_nodes','dryFlagNode','Cs',
@@ -2688,40 +2865,53 @@
        #get SCHISM variables
        ovars=unique([i[:i.rfind('_')] for i in os.listdir(run) if (i.endswith('.nc') \
              and (not i.startswith('hotstart_')) and i.rfind('_')!=-1)])
        outfmt=0 if ('out2d' in ovars) else 1 #output format: newIO or oldIO
 
        #get additional SCHISM variables
        if outfmt==0:
-          stacks=unique([int(i[:-3].split('_')[-1]) for i in os.listdir(run) if (i.startswith('out2d_') and i.endswith('.nc'))])
+          stacks=unique([int(i[:-3].split('_')[-1]) for i in glob(run+'/out2d_*.nc')])
           C=ReadNC(run+'/out2d_{}.nc'.format(stacks[0]),1); svars_2d=setdiff1d(array([*C.variables]),dvars); C.close()
           svars=setdiff1d(r_[ovars,svars_2d],dvars)
        else:
-          stacks=unique([int(i[:-3].split('_')[-1]) for i in os.listdir(run) if (i.startswith('schout_') and i.endswith('.nc'))])
+          stacks=unique([int(i[:-3].split('_')[-1]) for i in glob(run+'/schout_*.nc')])
           fname=[i for i in os.listdir(run) if (i.startswith('schout_') and i.endswith('_{}.nc'.format(stacks[0])))][0]
           C=ReadNC(run+'/{}'.format(fname),1); svars=setdiff1d(array([*C.variables]),dvars)
           svars_2d=array([i for i in svars if C.variables[i].ndim==2]); C.close()
 
        #get SCHISM modules
        M=get_schism_var_info(fmt=outfmt).__dict__
        modules=array([k for k in M if len(intersect1d([*M[k].values()],svars))!=0])
        return [modules,outfmt,stacks,svars,svars_2d]
-    else:
+    elif fmt==2:
        nes=[]; nps=[]; nss=[]; ies=[]; ips=[]; iss=[]
        nsg,neg,npg,nvrt,nproc,ntr=[int(i) for i in open(run+'/local_to_global_000000','r').readline().split()[:6]]
        for n in arange(nproc):
            lines=open('{}/local_to_global_{:06}'.format(run,n),'r').readlines()[2:]
            ne=int(lines[0].strip()); np=int(lines[ne+1].strip()); ns=int(lines[ne+np+2].strip())
            iei=array([i.split()[1] for i in lines[1:(ne+1)]]).astype('int')-1
            ipi=array([i.split()[1] for i in lines[(ne+2):(ne+np+2)]]).astype('int')-1
            isi=array([i.split()[1] for i in lines[(ne+np+3):(ne+np+ns+3)]]).astype('int')-1
            nes.append(ne); nps.append(np); nss.append(ns); ies.append(iei); ips.append(ipi); iss.append(isi)
        S=zdata(); S.nsg,S.neg,S.npg,S.nvrt,S.nproc,S.ntr=nsg,neg,npg,nvrt,nproc,ntr
        S.nes,S.nps,S.nss,S.ies,S.ips,S.iss=array(nes),array(nps),array(nss),ies,ips,iss
        return S
+    elif fmt==3:
+       fns=array(glob(run+'/out2d_*.nc')); ifs=array([int(i.replace('_','.').split('.')[-2]) for i in fns]); idx=argsort(ifs); ifs,fns=ifs[idx],fns[idx] #files
+       f=ReadNC(fns[0],1); v=f.variables['time']; StartT=datenum(*[int(i.split('.')[0]) for i in v.base_date.split()]); dt=(v[1]-v[0])/86400; ns=len(v); f.close() #StartT
+       mis=array([arange(ns)+(i-1)*ns for i in ifs]).ravel(); mts=dt*mis+StartT; EndT=mts[-1] #time
+       irec=mod(mis,ns); istack=array([tile(i,ns) for i in ifs]).ravel(); f=ReadNC(fns[-1],1); nm=len(f.variables['time'])-ns; f.close() #stack and record
+       if nm!=0: mts,istack,irec=mts[:nm],istack[:nm],irec[:nm]
+       S=zdata(); S.outdir,S.StartT, S.EndT, S.dt, S.nrec, S.ifs, S.fns, S.istack, S.irec, S.mts=run,StartT,EndT,dt,ns,ifs,fns,istack,irec,mts
+       return S
+    elif fmt==4:
+       sinfo=get_schism_output_info(run,3); f=ReadNC(sinfo.fns[0],1); cvar=f.variables; gd=schism_grid()
+       gd.x=array(cvar['SCHISM_hgrid_node_x']); gd.y=array(cvar['SCHISM_hgrid_node_y']); gd.dp=array(cvar['depth']); gd.elnode=array(cvar['SCHISM_hgrid_face_nodes'])-1
+       gd.np,gd.ne=gd.dp.size,len(gd.elnode); gd.elnode[(gd.elnode<0)|(abs(gd.elnode)>1e8)]=-2; gd.i34=sum(gd.elnode!=-2,axis=1); gd.ns=cvar['SCHISM_hgrid_edge_x'].size; f.close()
+       return gd
 
 def get_schism_var_info(svar=None,modules=None,fmt=0):
     '''
       usage:
          svar: variable name (either short and long names)
          modules: modules that svar may belong to
          fmt=0: scribe IO;   fmt=1: OLDIO (schout_*.nc)
@@ -3174,15 +3364,14 @@
     def INFO(self):
         return get_INFO(self)
     @property
     def VINFO(self):
         return get_INFO(self)
 
     def run_info(self,run):
-        from glob import glob
         import threading,time
 
         #check output
         print('reading grid and output info.')
         fns=glob(run+'/out2d_*.nc'); fns2=glob(run+'/outputs/out2d_*.nc'); self.gr3=[os.path.basename(i) for i in glob(run+'/*.gr3')]; iout=1
         self.outputs,fnames=[run,fns] if len(fns)!=0 else [run+'/outputs',fns2]; self.runpath=os.path.abspath(run); self.run=os.path.basename(self.runpath)
         if len(fnames)!=0:
@@ -3197,16 +3386,15 @@
         grd=run+'/grid.npz'; gr3=run+'/hgrid.gr3'; vrd=run+'/vgrid.in'; par=run+'/param.nml'
         if os.path.exists(par): p=read_schism_param(par,3); self.param=p; self.StartT=datenum(p.start_year,p.start_month,p.start_day,p.start_hour)
         def _read_grid():
            gd=loadz(grd).hgrid if os.path.exists(grd) else read_schism_hgrid(gr3) if os.path.exists(gr3) else None
            vd=loadz(grd).vgrid if os.path.exists(grd) else read_schism_vgrid(vrd) if os.path.exists(vrd) else None
            if gd==None: #create hgrid
               if cvar==None: return
-              gd=schism_grid(); gd.x=array(cvar['SCHISM_hgrid_node_x']); gd.y=array(cvar['SCHISM_hgrid_node_y']); gd.dp=array(cvar['depth'])
-              gd.elnode=array(cvar['SCHISM_hgrid_face_nodes'])-1; gd.np,gd.ne=gd.dp.size,len(gd.elnode); gd.i34=sum(gd.elnode!=-2,axis=1); gd.ns=cvar['SCHISM_hgrid_edge_x'].size
+              gd=get_schism_output_info(self.outputs,4)
            self.hgrid=gd; self.xm=[gd.x.min(),gd.x.max()]; self.ym=[gd.y.min(),gd.y.max()]; self.vm=[gd.dp.min(),gd.dp.max()]; self.fp3=nonzero(gd.i34==3)[0]; self.fp4=nonzero(gd.i34==4)[0]
            self.kbp, self.nvrt=[vd.kbp, vd.nvrt] if vd!=None else [array(cvar['bottom_index_node']), cdim['nSCHISM_vgrid_layers'].size]; self.kbe=gd.compute_kb(self.kbp)
            while not hasattr(self,'wp'): time.sleep(0.01)
            w=self.wp; w._layer['values']=['surface','bottom',*arange(2,self.nvrt+1)]; print('schismview ready')
            w.vmin.set(self.vm[0]); w.vmax.set(self.vm[1]); w.xmin.set(self.xm[0]); w.xmax.set(self.xm[1]); w.ymin.set(self.ym[0]); w.ymax.set(self.ym[1])
         self.nvrt=2; self.xm=[0,1]; self.ym=[0,1]; self.vm=[0,1]
         threading.Thread(target=_read_grid).start()
@@ -3517,15 +3705,15 @@
           #add gd.plot for *_nu.nc
           if fname.endswith('_nu.nc') or fname=='uv3D.th.nc':
              sfm=ttk.Frame(master=fm); sfm.grid(row=2,column=0,sticky='W')
              ttk.Label(master=sfm,text='  ').grid(row=0,column=0,sticky='W')
              tk.Checkbutton(master=sfm,text='grid',variable=p.grid,onvalue=1,offvalue=0).grid(row=0,column=1,sticky='W')
              tk.Checkbutton(master=sfm,text='bnd',variable=p.bnd,onvalue=1,offvalue=0).grid(row=0,column=2,sticky='W')
              if fname.endswith('_nu.nc'):
-                tk.Checkbutton(master=sfm,text='ctr',variable=p.ctr,onvalue=1,offvalue=0).grid(row=0,column=3,sticky='W')
+                tk.Checkbutton(master=sfm,text='dispaly on mesh',variable=p.ctr,onvalue=1,offvalue=0).grid(row=0,column=3,sticky='W')
              else:
                 ttk.Label(master=sfm,text='   zoom').grid(row=0,column=3,sticky='W')
                 ttk.Entry(sfm,textvariable=p.scale,width=5).grid(row=0,column=4,sticky='W')
        elif self.fmt in [2,3]:  #hotstart.nc or source.nc
           if p.init==1 and option==1: #save parameter
              p0=zdata(); p0.dvars=[i.get() for i in p.dvars]; p0.vmin=p.vmin.get(); p0.vmax=p.vmax.get(); p0.scale=p.scale.get()
              p0.transpose=p.transpose.get(); p0.grid=p.grid.get(); p0.bnd=p.bnd.get(); p0.dims=[*p.dims]
@@ -3590,15 +3778,15 @@
           if self.fmt==3:
              sfm=ttk.Frame(master=fm); sfm.grid(row=2,column=0,sticky='W',pady=5)
              tk.Checkbutton(master=sfm,text='scatter',variable=p.sctr,onvalue=1,offvalue=0).grid(row=0,column=0,sticky='W')
              ttk.Label(master=sfm,text='  zoom').grid(row=0,column=1,sticky='W')
              ttk.Entry(sfm,textvariable=p.srat,width=10).grid(row=0,column=2,sticky='W',padx=2)
              tk.Checkbutton(master=sfm,text='grid',variable=p.grid,onvalue=1,offvalue=0).grid(row=0,column=3)
              tk.Checkbutton(master=sfm,text='bnd',variable=p.bnd,onvalue=1,offvalue=0).grid(row=0,column=4,sticky='W')
-             tk.Checkbutton(master=sfm,text='ctr',variable=p.ctr,onvalue=1,offvalue=0).grid(row=0,column=5,sticky='W')
+             tk.Checkbutton(master=sfm,text='color',variable=p.ctr,onvalue=1,offvalue=0).grid(row=0,column=5,sticky='W')
              tk.Checkbutton(master=sfm,text='id',variable=p.id,onvalue=1,offvalue=0).grid(row=0,column=6,sticky='W')
              wd.geometry('400x185')
 
           #restore parameters if dims are the same
           if p.init==1 and option==1 and array_equal(array(p0.dims),array(p.dims)):
              [i.set(k) for i,k in zip(p.dvars,p0.dvars)]; p.vmin.set(p0.vmin); p.vmax.set(p0.vmax); p.scale.set(p0.scale)
              p.transpose.set(p0.transpose); p.grid.set(p0.grid); p.bnd.set(p0.bnd)
@@ -3771,20 +3959,17 @@
                cm.ScalarMappable.set_clim(hg,vmin=vm[0],vmax=vm[1])
                hc=colorbar(fraction=0.05,aspect=50,spacing='proportional',pad=0.02); hc.set_ticks(linspace(*vm,11)); hc.ax.set_ylim(vm)
        elif self.fmt in [1,2,3,4]: # bnd, nudge, hotstart, source.nc
           vm=[p.vmin.get(),p.vmax.get()]
           if p.data.ndim==1:
               i0=p.ax[0]; xi,xn=p.xs[i0], p.dnames[i0]
               if not hasattr(self,'hgrid'):self.read_hgrid()
-              flag_nu=0; fn=self.run+fname.split('_')[0]+'_nudge.gr3'; fexist=os.path.exists
-              if fname.endswith('_nu.nc') and xn=='node' and fexist(fn) and p.ctr.get()==1: flag_nu=1
-              if flag_nu==1:  #plot nudge value on grid
+              if fname.endswith('_nu.nc') and xn=='node' and p.ctr.get()==1:
                   gd=self.hgrid
-                  if fn not in fids: fids[fn]=read(fn).z #read *_nudge.gr3
-                  if not hasattr(p,'sindn'): p.sindn=nonzero(fids[fn]!=0)[0]
+                  if not hasattr(p,'sindn'): p.sindn=array(read(self.run+os.path.sep+fname,1).variables['map_to_global_node'])-1
                   vi=zeros(gd.np); vi[p.sindn]=p.data
                   gd.plot(fmt=1,value=vi,clim=[p.vmin.get(),p.vmax.get()],ticks=11,cmap='jet',method=1); p.hp=gca()
                   if p.grid.get()==1: gd.plot()
                   if p.bnd.get()==1:  gd.plot_bnd(c='rg',lw=1)
                   pfmt=6; slimit(gd.x,gd.y,p.data)
               elif self.fmt==2 and (xn in ['node', 'elem','node/elem','dim_{}'.format(self.hgrid.np),'dim_{}'.format(self.hgrid.ne)]): #schism grid plot
                   gd=self.hgrid
```

### Comparing `pylibs_ocean-1.0.0/pylib.py` & `pylibs_ocean-1.0.1/pylib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #---------------------------------------------------------------------
 #import system lib
 #---------------------------------------------------------------------
 import os,sys
+from glob import glob
 
 Libs=['pylib','mylib','schism_file']
 if not set(Libs).issubset(set(sys.modules.keys())):
    pversion=sys.version.split(' ')[0] #print(pversion)
 
    #---------------------------------------------------------------------
    #load pylib libraries of packages
@@ -42,15 +43,17 @@
    from scipy import interpolate
    from scipy.fftpack import fft, ifft
 
    #mpi4py
    try:
       from mpi4py import MPI
    except:
-       pass
+      pass
+      #from pyUtility.mylib import parallel_jobs
+      #MPI=parallel_jobs()
 
    #url download
    try:
       import urllib
       from urllib.request import urlretrieve as urlsave
       import ssl
       try:
@@ -92,30 +95,31 @@
    #---------------------------------------------------------------------
    import pyUtility.mylib as mylib
    sys.modules['mylib'] = mylib
    from pyUtility.mylib import (get_xtick,close_data_loop,datenum,quickdatenum,
         get_INFO,loadz,zdata,savez,find_cs,npz2mat,convert_matfile,
         smooth,daytime_length,move_figure,bpfilt,lpfilt,mdivide,signa,
         inside_polygon,mdist,command_outputs,near_pts,proj,proj_pts,rewrite,rewrite_input,
-        get_prj_file,mfft,read_shapefile_data,write_shapefile_data,
+        get_prj_file,mfft,interp_vertical,read_shapefile_data,write_shapefile_data,
         ReadNC,WriteNC,harmonic_fit,harmonic_analysis,get_hycom,compute_contour,EOF,
         get_stat,get_subplot_position,get_subplot_position2,load_bathymetry,plot_taylor_diagram,
         convert_dem_format,get_hpc_command,least_square_fit,read_yaml,read_excel,
-        write_excel,rtext,mklink,cindex,resize,savefig,pplot,blit_manager,read,add_xtick)
+        write_excel,rtext,mklink,cindex,resize,savefig,pplot,blit_manager,read,add_xtick,
+        get_qnode,modify_figure,parallel_jobs,fig_IFNO,ceqstate,subdomain_index)
 
    import pyUtility.schism_file as schism_file
    sys.modules['schism_file'] = schism_file
    from pyUtility.schism_file import (read_schism_hgrid, read_schism_bpfile,getglob,
         schism_grid,schism_vgrid,schism_bpfile,sms2grd,read_schism_vgrid,save_schism_grid,
         compute_zcor,read_schism_param,write_schism_param,read_schism_local_to_global,
         create_schism_vgrid,srank,grd2sms,scatter_to_schism_grid,delete_schism_grid_element,
         read_schism_prop,read_schism_reg,interp_schism_3d,get_schism_var_info,
         read_schism_output,change_schism_param,get_schism_output_info,get_schism_grid_subdomain,
         get_schism_output_subset,combine_schism_hotstart,combine_icm_output,read_schism_slab,
-        convert_schism_source,schism_view,schism_check,zcor_to_schism_grid)
+        convert_schism_source,schism_view,schism_check,zcor_to_schism_grid,compute_schism_volume)
 
    if os.getenv('HOME')!=None:
        sys.path.append(os.getenv('HOME'))
 
    #sys.modules['loadz'] = mylib #in case oldmodule name used
    #sys.modules['read_schism_file'] = schism_file #in case oldmodule name used
 
@@ -126,14 +130,15 @@
    #alias
    #---------------------------------------------------------------------
    from os.path import exists as fexist
    from pyUtility.mylib import savez as save_npz; mylib.save_npz=savez
    from pyUtility.mylib import zdata as npz_data; mylib.npz_data=zdata
    from pyUtility.mylib import least_square_fit as lsq; mylib.least_square_fit=lsq
    from pyUtility.mylib import move_figure as mvfig
+   from pyUtility.mylib import modify_figure as mfig
    from pyUtility.mylib import find_cs as find_continuous_sections; mylib.find_continuous_sections=find_cs
    from pyUtility.mylib import convert_matfile as mat2npz
    from pyUtility.mylib import convert_matfile as loadm
    from pyUtility.mylib import convert_dem_format as read_dem
    from pyUtility.mylib import read_shapefile_data as read_shp
    from pyUtility.mylib import write_shapefile_data as write_shp
    from pyUtility.schism_file import read_schism_hgrid as read_grd
```

### Comparing `pylibs_ocean-1.0.0/pylibs_ocean.egg-info/SOURCES.txt` & `pylibs_ocean-1.0.1/pylibs_ocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylibs_ocean-1.0.0/setup.py` & `pylibs_ocean-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     setup(
         name='pylibs_ocean',
         packages=[
           'pyUtility',
     	  'pyScripts',
         ],
         py_modules=['pylib'],
-        version='1.0.0',  # Ideally should be same as your GitHub release tag varsion
+        version='1.0.1',  # Ideally should be same as your GitHub release tag varsion
         package_data={'pyScripts': ['prj.npz','sflux_template.npz','Harmonic_Analysis/*','schismcheck','schismview']},
         description='python tools for ocean reserach',
         long_description='python libraries and utilities for data processing including the pre/post-processing about SCHISM models',
         author='Zhengui Wang',
         author_email='wzhengui@gmail.com',
         url='https://github.com/wzhengui/pylibs',
         classifiers=[],
```

