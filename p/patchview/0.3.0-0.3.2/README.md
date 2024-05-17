# Comparing `tmp/patchview-0.3.0.tar.gz` & `tmp/patchview-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patchview-0.3.0.tar", last modified: Fri Feb 16 20:31:30 2024, max compression
+gzip compressed data, was "patchview-0.3.2.tar", last modified: Fri May 17 21:37:49 2024, max compression
```

## Comparing `patchview-0.3.0.tar` & `patchview-0.3.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1307 2024-02-16 19:25:02.000000 patchview-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)       25 2024-02-16 19:25:02.000000 patchview-0.3.0/HISTORY.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1555 2024-02-16 19:25:02.000000 patchview-0.3.0/LICENSE
--rw-r--r--   0 mhu       (1000) mhu       (1000)      473 2024-02-16 19:25:02.000000 patchview-0.3.0/MANIFEST.in
--rw-r--r--   0 mhu       (1000) mhu       (1000)     4500 2024-02-16 20:31:30.617516 patchview-0.3.0/PKG-INFO
--rw-r--r--   0 mhu       (1000) mhu       (1000)     2520 2024-02-16 19:25:02.000000 patchview-0.3.0/README.rst
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.607516 patchview-0.3.0/docs/
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1766 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/APIs.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)      630 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/Makefile
--rw-r--r--   0 mhu       (1000) mhu       (1000)     6341 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/conf.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)       34 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/contributing.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)       29 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/credits.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)      346 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/index.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)     7037 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/installation.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)     5218 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/introduction.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)      807 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/make.bat
--rw-r--r--   0 mhu       (1000) mhu       (1000)       28 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/readme.rst
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.607516 patchview-0.3.0/docs/resources/
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.607516 patchview-0.3.0/docs/resources/icons/
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1146 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/icons/GP1.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      732 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/icons/GPcorr.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      383 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/icons/navigation.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    42415 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/icons/neuron.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      999 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/icons/rectangle.png
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/docs/resources/images/
--rw-r--r--   0 mhu       (1000) mhu       (1000)   263017 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/FP_stats.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   235641 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/FP_trace.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    11902 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/PatchViewer.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    12435 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/connectionTraces_loaded2.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   102223 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/connections.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    78021 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/couplingRatio.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   139763 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/density.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)  1312222 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/event_curate.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   212714 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/event_detec.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   890804 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/event_histExport.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)  1783491 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/event_sweep.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)  1140759 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/event_template.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    31835 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/fp.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   927525 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/measurePiaToSomas.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    62169 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/morphor_polar.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    64865 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/morphor_tree.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    86547 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/pasedavian_001_trace.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    95936 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/pasedavian_002_multTraces.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   211264 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/pasedavian_003_series.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   152373 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/pasedavian_004_morphology.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)   123755 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/pasedavian_004_morphology_soma.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)  1460027 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/patchview_ads.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    96533 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/shollAna1.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    78834 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources/images/test_CR.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1806 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/resources.rst
--rw-r--r--   0 mhu       (1000) mhu       (1000)    10657 2024-02-16 19:25:02.000000 patchview-0.3.0/docs/tutorials.rst
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/Data/
--rw-r--r--   0 mhu       (1000) mhu       (1000)      508 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/JiangLab_protocols.yaml
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1535 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/LICENSE.txt
--rw-r--r--   0 mhu       (1000) mhu       (1000)      229 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/NDX_files
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1586 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/Navigator.ui
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/Data/icons/
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1146 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/GP1.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      732 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/GP2.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      732 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/GPcorr.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    16958 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/PatchViewer.ico
--rw-r--r--   0 mhu       (1000) mhu       (1000)    47689 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/connection.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    17889 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/connection2.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      383 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/navigation.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    42415 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/neuron.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      999 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/rectangle.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)     4565 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/settings.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1257 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/spikes.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)    12832 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/icons/tree.png
--rw-r--r--   0 mhu       (1000) mhu       (1000)      973 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/Data/patchview.yaml
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/HekaIO/
--rw-r--r--   0 mhu       (1000) mhu       (1000)    46768 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/HekaIO/HEKA_Reader_MAIN.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)     7116 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/HekaIO/HekaHelpers.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)        0 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/HekaIO/__init__.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    16958 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/PatchViewer.ico
--rw-r--r--   0 mhu       (1000) mhu       (1000)      338 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/__init__.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)       17 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/__version__.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)      483 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/enviroment-dev.yml
--rw-r--r--   0 mhu       (1000) mhu       (1000)      486 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/enviroment.yml
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/ephys/
--rw-r--r--   0 mhu       (1000) mhu       (1000)        0 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/ephys/__init__.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    55305 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/ephys/ephys_extractor.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    60946 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/ephys/ephys_features.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)   110619 2024-02-16 20:16:10.000000 patchview-0.3.0/patchview/ephys/extraEhpys_PV.py
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/examples/
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1348 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/examples/load_spike_list.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)       37 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/main.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)   358161 2024-02-16 20:14:41.000000 patchview-0.3.0/patchview/patchview.py
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/utilitis/
--rw-r--r--   0 mhu       (1000) mhu       (1000)    39404 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/AllMyParsHere.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)     9135 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/AnalysisMethods.py
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview/utilitis/NDX_files/
--rw-r--r--   0 mhu       (1000) mhu       (1000)     1766 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/NDX_files/XiaolongJiangLab.extensions.yaml
--rw-r--r--   0 mhu       (1000) mhu       (1000)      229 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/NDX_files/XiaolongJiangLab.namespace.yaml
--rw-r--r--   0 mhu       (1000) mhu       (1000)    14476 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/PVdat2NWB.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)        0 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/__init__.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)     4925 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/dandi2pvNWB.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)      342 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/debugHelpers.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    10281 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/emfDraw.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    11238 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/fitFuncs.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)      749 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/graphictools.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)     2827 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/linecollection_update.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    29249 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/morphorFeatureExtrator.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    55429 2024-02-16 20:28:21.000000 patchview-0.3.0/patchview/utilitis/patchviewObjects.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)     6781 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/patchview_ndx.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)    25164 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/pvEphy.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)     7536 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/pvNDX_class.py
--rw-r--r--   0 mhu       (1000) mhu       (1000)      432 2024-02-16 19:25:02.000000 patchview-0.3.0/patchview/utilitis/pyqtgraph_helpers.py
-drwxr-xr-x   0 mhu       (1000) mhu       (1000)        0 2024-02-16 20:31:30.617516 patchview-0.3.0/patchview.egg-info/
--rw-r--r--   0 mhu       (1000) mhu       (1000)     4500 2024-02-16 20:31:30.000000 patchview-0.3.0/patchview.egg-info/PKG-INFO
--rw-r--r--   0 mhu       (1000) mhu       (1000)     3360 2024-02-16 20:31:30.000000 patchview-0.3.0/patchview.egg-info/SOURCES.txt
--rw-r--r--   0 mhu       (1000) mhu       (1000)        1 2024-02-16 20:31:30.000000 patchview-0.3.0/patchview.egg-info/dependency_links.txt
--rw-r--r--   0 mhu       (1000) mhu       (1000)       42 2024-02-16 20:31:30.000000 patchview-0.3.0/patchview.egg-info/entry_points.txt
--rw-r--r--   0 mhu       (1000) mhu       (1000)        1 2024-02-16 19:53:15.000000 patchview-0.3.0/patchview.egg-info/not-zip-safe
--rw-r--r--   0 mhu       (1000) mhu       (1000)      354 2024-02-16 20:31:30.000000 patchview-0.3.0/patchview.egg-info/requires.txt
--rw-r--r--   0 mhu       (1000) mhu       (1000)       10 2024-02-16 20:31:30.000000 patchview-0.3.0/patchview.egg-info/top_level.txt
--rw-r--r--   0 mhu       (1000) mhu       (1000)      377 2024-02-16 19:25:02.000000 patchview-0.3.0/requirements.txt
--rw-r--r--   0 mhu       (1000) mhu       (1000)      603 2024-02-16 20:31:30.617516 patchview-0.3.0/setup.cfg
--rw-r--r--   0 mhu       (1000) mhu       (1000)     2595 2024-02-16 19:58:28.000000 patchview-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.104212 patchview-0.3.2/
+-rw-rw-rw-   0        0        0     1307 2024-05-17 19:09:33.000000 patchview-0.3.2/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0       25 2024-05-17 19:09:33.000000 patchview-0.3.2/HISTORY.rst
+-rw-rw-rw-   0        0        0     1555 2024-05-17 19:09:33.000000 patchview-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      473 2024-05-17 19:09:33.000000 patchview-0.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4607 2024-05-17 21:37:49.103212 patchview-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2520 2024-05-17 19:09:33.000000 patchview-0.3.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.017211 patchview-0.3.2/docs/
+-rw-rw-rw-   0        0        0     1766 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/APIs.rst
+-rw-rw-rw-   0        0        0      630 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/Makefile
+-rw-rw-rw-   0        0        0     6341 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/contributing.rst
+-rw-rw-rw-   0        0        0       29 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/credits.rst
+-rw-rw-rw-   0        0        0      346 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/index.rst
+-rw-rw-rw-   0        0        0     7037 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/installation.rst
+-rw-rw-rw-   0        0        0     5218 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/introduction.rst
+-rwxrwxrwx   0        0        0      807 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/make.bat
+-rw-rw-rw-   0        0        0       28 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/readme.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:48.996210 patchview-0.3.2/docs/resources/
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.022211 patchview-0.3.2/docs/resources/icons/
+-rw-rw-rw-   0        0        0     1146 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/icons/GP1.png
+-rw-rw-rw-   0        0        0      732 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/icons/GPcorr.png
+-rw-rw-rw-   0        0        0      383 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/icons/navigation.png
+-rw-rw-rw-   0        0        0    42415 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/icons/neuron.png
+-rw-rw-rw-   0        0        0      999 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/icons/rectangle.png
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.046211 patchview-0.3.2/docs/resources/images/
+-rw-rw-rw-   0        0        0   263017 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/FP_stats.png
+-rw-rw-rw-   0        0        0   235641 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/FP_trace.png
+-rw-rw-rw-   0        0        0    11902 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/PatchViewer.png
+-rw-rw-rw-   0        0        0    12435 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/connectionTraces_loaded2.png
+-rw-rw-rw-   0        0        0   102223 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/connections.png
+-rw-rw-rw-   0        0        0    78021 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/couplingRatio.png
+-rw-rw-rw-   0        0        0   139763 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/density.png
+-rw-rw-rw-   0        0        0  1312222 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/event_curate.png
+-rw-rw-rw-   0        0        0   212714 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/event_detec.png
+-rw-rw-rw-   0        0        0   890804 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/event_histExport.png
+-rw-rw-rw-   0        0        0  1783491 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/event_sweep.png
+-rw-rw-rw-   0        0        0  1140759 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/event_template.png
+-rw-rw-rw-   0        0        0    31835 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/fp.png
+-rw-rw-rw-   0        0        0   927525 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/measurePiaToSomas.png
+-rw-rw-rw-   0        0        0    62169 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/morphor_polar.png
+-rw-rw-rw-   0        0        0    64865 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/morphor_tree.png
+-rw-rw-rw-   0        0        0    86547 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/pasedavian_001_trace.png
+-rw-rw-rw-   0        0        0    95936 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/pasedavian_002_multTraces.png
+-rw-rw-rw-   0        0        0   211264 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/pasedavian_003_series.png
+-rw-rw-rw-   0        0        0   152373 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/pasedavian_004_morphology.png
+-rw-rw-rw-   0        0        0   123755 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/pasedavian_004_morphology_soma.png
+-rw-rw-rw-   0        0        0  1460027 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/patchview_ads.png
+-rw-rw-rw-   0        0        0    96533 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/shollAna1.png
+-rw-rw-rw-   0        0        0    78834 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources/images/test_CR.png
+-rw-rw-rw-   0        0        0     1806 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/resources.rst
+-rw-rw-rw-   0        0        0    10657 2024-05-17 19:09:33.000000 patchview-0.3.2/docs/tutorials.rst
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.061211 patchview-0.3.2/patchview/
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.078212 patchview-0.3.2/patchview/Data/
+-rw-rw-rw-   0        0        0      508 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/JiangLab_protocols.yaml
+-rw-rw-rw-   0        0        0     1535 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/LICENSE.txt
+-rw-rw-rw-   0        0        0      229 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/NDX_files
+-rw-rw-rw-   0        0        0     1586 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/Navigator.ui
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.085213 patchview-0.3.2/patchview/Data/icons/
+-rw-rw-rw-   0        0        0     1146 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/GP1.png
+-rw-rw-rw-   0        0        0      732 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/GP2.png
+-rw-rw-rw-   0        0        0      732 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/GPcorr.png
+-rw-rw-rw-   0        0        0    16958 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/PatchViewer.ico
+-rw-rw-rw-   0        0        0    47689 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/connection.png
+-rw-rw-rw-   0        0        0    17889 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/connection2.png
+-rw-rw-rw-   0        0        0      383 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/navigation.png
+-rw-rw-rw-   0        0        0    42415 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/neuron.png
+-rw-rw-rw-   0        0        0      999 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/rectangle.png
+-rw-rw-rw-   0        0        0     4565 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/settings.png
+-rw-rw-rw-   0        0        0     1257 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/spikes.png
+-rw-rw-rw-   0        0        0    12832 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/icons/tree.png
+-rw-rw-rw-   0        0        0      973 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/Data/patchview.yaml
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.087212 patchview-0.3.2/patchview/HekaIO/
+-rw-rw-rw-   0        0        0    46768 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/HekaIO/HEKA_Reader_MAIN.py
+-rw-rw-rw-   0        0        0     7116 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/HekaIO/HekaHelpers.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/HekaIO/__init__.py
+-rw-rw-rw-   0        0        0    16958 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/PatchViewer.ico
+-rw-rw-rw-   0        0        0      338 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/__init__.py
+-rw-rw-rw-   0        0        0       17 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/__version__.py
+-rw-rw-rw-   0        0        0      483 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/enviroment-dev.yml
+-rw-rw-rw-   0        0        0      486 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/enviroment.yml
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.090212 patchview-0.3.2/patchview/ephys/
+-rw-rw-rw-   0        0        0        0 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/ephys/__init__.py
+-rw-rw-rw-   0        0        0    55305 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/ephys/ephys_extractor.py
+-rw-rw-rw-   0        0        0    60946 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/ephys/ephys_features.py
+-rw-rw-rw-   0        0        0   110619 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/ephys/extraEhpys_PV.py
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.091212 patchview-0.3.2/patchview/examples/
+-rw-rw-rw-   0        0        0     1348 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/examples/load_spike_list.py
+-rw-rw-rw-   0        0        0       37 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/main.py
+-rw-rw-rw-   0        0        0   358771 2024-05-17 21:36:59.000000 patchview-0.3.2/patchview/patchview.py
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.101213 patchview-0.3.2/patchview/utilitis/
+-rw-rw-rw-   0        0        0    39404 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/AllMyParsHere.py
+-rw-rw-rw-   0        0        0     9135 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/AnalysisMethods.py
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.102212 patchview-0.3.2/patchview/utilitis/NDX_files/
+-rw-rw-rw-   0        0        0     1766 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/NDX_files/XiaolongJiangLab.extensions.yaml
+-rw-rw-rw-   0        0        0      229 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/NDX_files/XiaolongJiangLab.namespace.yaml
+-rw-rw-rw-   0        0        0    14476 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/PVdat2NWB.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/__init__.py
+-rw-rw-rw-   0        0        0     4925 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/dandi2pvNWB.py
+-rw-rw-rw-   0        0        0      342 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/debugHelpers.py
+-rw-rw-rw-   0        0        0    10281 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/emfDraw.py
+-rw-rw-rw-   0        0        0    11238 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/fitFuncs.py
+-rw-rw-rw-   0        0        0      749 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/graphictools.py
+-rw-rw-rw-   0        0        0     2827 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/linecollection_update.py
+-rw-rw-rw-   0        0        0    29249 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/morphorFeatureExtrator.py
+-rw-rw-rw-   0        0        0    55429 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/patchviewObjects.py
+-rw-rw-rw-   0        0        0     6781 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/patchview_ndx.py
+-rw-rw-rw-   0        0        0    25164 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/pvEphy.py
+-rw-rw-rw-   0        0        0     7536 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/pvNDX_class.py
+-rw-rw-rw-   0        0        0      432 2024-05-17 19:09:33.000000 patchview-0.3.2/patchview/utilitis/pyqtgraph_helpers.py
+drwxrwxrwx   0        0        0        0 2024-05-17 21:37:49.103212 patchview-0.3.2/patchview.egg-info/
+-rw-rw-rw-   0        0        0     4607 2024-05-17 21:37:48.000000 patchview-0.3.2/patchview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3360 2024-05-17 21:37:48.000000 patchview-0.3.2/patchview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 21:37:48.000000 patchview-0.3.2/patchview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 21:37:48.000000 patchview-0.3.2/patchview.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-17 19:10:10.000000 patchview-0.3.2/patchview.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      347 2024-05-17 21:37:48.000000 patchview-0.3.2/patchview.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-17 21:37:48.000000 patchview-0.3.2/patchview.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      370 2024-05-17 19:09:33.000000 patchview-0.3.2/requirements.txt
+-rw-rw-rw-   0        0        0      639 2024-05-17 21:37:49.105212 patchview-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2595 2024-05-17 21:36:54.000000 patchview-0.3.2/setup.py
```

### Comparing `patchview-0.3.0/CONTRIBUTING.rst` & `patchview-0.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/LICENSE` & `patchview-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/PKG-INFO` & `patchview-0.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-Metadata-Version: 2.1
-Name: patchview
-Version: 0.3.0
-Summary: Patchview perform data analysis and visualization on whole-cell recording data, including firing pattern analysis, event analysis, synatpic connection detection, morphorlocial analysis and more.
-Home-page: https://github.com/zeitgeberH/patchview
-Author: Ming Hu
-Author-email: hi@gmail.com
-License: BSD-3-Clause
-Keywords: patchview
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: furo
-Requires-Dist: morphopy
-Requires-Dist: colorcet
-Requires-Dist: appdirs
-Requires-Dist: Pillow
-Requires-Dist: pynwb
-Requires-Dist: tqdm
-Requires-Dist: PySide2
-Requires-Dist: pyqt5
-Requires-Dist: pyqtwebengine
-Requires-Dist: pyqt5-sip
-Requires-Dist: pyqtgraph==0.13.1
-Requires-Dist: PyOpenGL
-Requires-Dist: PyOpenGL_accelerate>=3.1.6; sys_platform == "win32"
-Requires-Dist: cython
-Requires-Dist: neo
-Requires-Dist: pylru==1.2.1
-Requires-Dist: h5py==3.7.0
-Requires-Dist: joblib
-Requires-Dist: future>=0.18.3
-Requires-Dist: pyYAML
-Requires-Dist: python-dateutil
-Requires-Dist: seaborn
-Requires-Dist: pytz
-Requires-Dist: scipy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: pycairo
-Requires-Dist: scikit-image
-Requires-Dist: morphio
-Requires-Dist: scikit-learn
-Requires-Dist: numpy<1.24,>=1.22
-Provides-Extra: dev
-
-===============
-PatchView
-===============
-.. image:: https://img.shields.io/pypi/v/patchview.svg 
-        :target: https://pypi.python.org/pypi/patchview
-      
-.. image:: https://img.shields.io/badge/python-3.10%2B-blue
-        :target: https://www.python.org/downloads/release/python
-        :alt: Python3.8
-
-.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
-        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-        :target: https://opensource.org/licenses/BSD-3-Clause
-        :alt: BSD-3-Clause    
-
-.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
-   :target: https://doi.org/10.21105/joss.04706
-.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
-           
-
-.. image:: docs/resources/images/patchview_ads.png
-    :width: 800
-
-PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
-synaptic connection detection, morphological analysis and more.
-
-* Free software: BSD 3-Clause license
-* Documentation: https://patchview.readthedocs.io.
-
-
-Features
---------
-PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
-Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
-these tools or writing any Python scripts.
-
-* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
-* Visualizing single and multiple traces with zoom, pan operations.
-* Automatically sorting experiments data according to predefined labels.
-* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
-* Synaptic connection analysis.
-* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
-
-
-Citation
----------
-If you find our work useful for your research, please cite:
-
-    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
+Metadata-Version: 2.1
+Name: patchview
+Version: 0.3.2
+Summary: Patchview perform data analysis and visualization on whole-cell recording data, including firing pattern analysis, event analysis, synatpic connection detection, morphorlocial analysis and more.
+Home-page: https://github.com/zeitgeberH/patchview
+Author: Ming Hu
+Author-email: hi@gmail.com
+License: BSD-3-Clause
+Keywords: patchview
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: furo
+Requires-Dist: morphopy
+Requires-Dist: colorcet
+Requires-Dist: appdirs
+Requires-Dist: Pillow
+Requires-Dist: pynwb
+Requires-Dist: tqdm
+Requires-Dist: PySide2
+Requires-Dist: pyqt5
+Requires-Dist: pyqtwebengine
+Requires-Dist: pyqt5-sip
+Requires-Dist: pyqtgraph==0.13.1
+Requires-Dist: PyOpenGL
+Requires-Dist: PyOpenGL_accelerate>=3.1.6; sys_platform == "win32"
+Requires-Dist: cython
+Requires-Dist: neo
+Requires-Dist: pylru==1.2.1
+Requires-Dist: h5py
+Requires-Dist: joblib
+Requires-Dist: future>=0.18.3
+Requires-Dist: pyYAML
+Requires-Dist: python-dateutil
+Requires-Dist: seaborn
+Requires-Dist: pytz
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: pycairo
+Requires-Dist: scikit-image
+Requires-Dist: morphio
+Requires-Dist: scikit-learn
+Requires-Dist: numpy<1.24,>=1.22
+Provides-Extra: dev
+
+===============
+PatchView
+===============
+.. image:: https://img.shields.io/pypi/v/patchview.svg 
+        :target: https://pypi.python.org/pypi/patchview
+      
+.. image:: https://img.shields.io/badge/python-3.10%2B-blue
+        :target: https://www.python.org/downloads/release/python
+        :alt: Python3.8
+
+.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
+        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+        :target: https://opensource.org/licenses/BSD-3-Clause
+        :alt: BSD-3-Clause    
+
+.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
+   :target: https://doi.org/10.21105/joss.04706
+.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
+           
+
+.. image:: docs/resources/images/patchview_ads.png
+    :width: 800
+
+PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
+synaptic connection detection, morphological analysis and more.
+
+* Free software: BSD 3-Clause license
+* Documentation: https://patchview.readthedocs.io.
+
+
+Features
+--------
+PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
+Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
+these tools or writing any Python scripts.
+
+* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
+* Visualizing single and multiple traces with zoom, pan operations.
+* Automatically sorting experiments data according to predefined labels.
+* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
+* Synaptic connection analysis.
+* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
+
+
+Citation
+---------
+If you find our work useful for your research, please cite:
+
+    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
```

### Comparing `patchview-0.3.0/README.rst` & `patchview-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/APIs.rst` & `patchview-0.3.2/docs/APIs.rst`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/Makefile` & `patchview-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/conf.py` & `patchview-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/installation.rst` & `patchview-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/introduction.rst` & `patchview-0.3.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/make.bat` & `patchview-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/icons/GP1.png` & `patchview-0.3.2/docs/resources/icons/GP1.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/icons/GPcorr.png` & `patchview-0.3.2/docs/resources/icons/GPcorr.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/icons/neuron.png` & `patchview-0.3.2/docs/resources/icons/neuron.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/icons/rectangle.png` & `patchview-0.3.2/docs/resources/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/FP_stats.png` & `patchview-0.3.2/docs/resources/images/FP_stats.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/FP_trace.png` & `patchview-0.3.2/docs/resources/images/FP_trace.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/PatchViewer.png` & `patchview-0.3.2/docs/resources/images/PatchViewer.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/connectionTraces_loaded2.png` & `patchview-0.3.2/docs/resources/images/connectionTraces_loaded2.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/connections.png` & `patchview-0.3.2/docs/resources/images/connections.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/couplingRatio.png` & `patchview-0.3.2/docs/resources/images/couplingRatio.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/density.png` & `patchview-0.3.2/docs/resources/images/density.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/event_curate.png` & `patchview-0.3.2/docs/resources/images/event_curate.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/event_detec.png` & `patchview-0.3.2/docs/resources/images/event_detec.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/event_histExport.png` & `patchview-0.3.2/docs/resources/images/event_histExport.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/event_sweep.png` & `patchview-0.3.2/docs/resources/images/event_sweep.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/event_template.png` & `patchview-0.3.2/docs/resources/images/event_template.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/fp.png` & `patchview-0.3.2/docs/resources/images/fp.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/measurePiaToSomas.png` & `patchview-0.3.2/docs/resources/images/measurePiaToSomas.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/morphor_polar.png` & `patchview-0.3.2/docs/resources/images/morphor_polar.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/morphor_tree.png` & `patchview-0.3.2/docs/resources/images/morphor_tree.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/pasedavian_001_trace.png` & `patchview-0.3.2/docs/resources/images/pasedavian_001_trace.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/pasedavian_002_multTraces.png` & `patchview-0.3.2/docs/resources/images/pasedavian_002_multTraces.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/pasedavian_003_series.png` & `patchview-0.3.2/docs/resources/images/pasedavian_003_series.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/pasedavian_004_morphology.png` & `patchview-0.3.2/docs/resources/images/pasedavian_004_morphology.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/pasedavian_004_morphology_soma.png` & `patchview-0.3.2/docs/resources/images/pasedavian_004_morphology_soma.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/patchview_ads.png` & `patchview-0.3.2/docs/resources/images/patchview_ads.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/shollAna1.png` & `patchview-0.3.2/docs/resources/images/shollAna1.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources/images/test_CR.png` & `patchview-0.3.2/docs/resources/images/test_CR.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/resources.rst` & `patchview-0.3.2/docs/resources.rst`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/docs/tutorials.rst` & `patchview-0.3.2/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/LICENSE.txt` & `patchview-0.3.2/patchview/Data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/Navigator.ui` & `patchview-0.3.2/patchview/Data/Navigator.ui`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/GP1.png` & `patchview-0.3.2/patchview/Data/icons/GP1.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/GP2.png` & `patchview-0.3.2/patchview/Data/icons/GP2.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/GPcorr.png` & `patchview-0.3.2/patchview/Data/icons/GPcorr.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/PatchViewer.ico` & `patchview-0.3.2/patchview/Data/icons/PatchViewer.ico`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/connection.png` & `patchview-0.3.2/patchview/Data/icons/connection.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/connection2.png` & `patchview-0.3.2/patchview/Data/icons/connection2.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/neuron.png` & `patchview-0.3.2/patchview/Data/icons/neuron.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/rectangle.png` & `patchview-0.3.2/patchview/Data/icons/rectangle.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/settings.png` & `patchview-0.3.2/patchview/Data/icons/settings.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/spikes.png` & `patchview-0.3.2/patchview/Data/icons/spikes.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/icons/tree.png` & `patchview-0.3.2/patchview/Data/icons/tree.png`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/Data/patchview.yaml` & `patchview-0.3.2/patchview/Data/patchview.yaml`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/HekaIO/HEKA_Reader_MAIN.py` & `patchview-0.3.2/patchview/HekaIO/HEKA_Reader_MAIN.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/HekaIO/HekaHelpers.py` & `patchview-0.3.2/patchview/HekaIO/HekaHelpers.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/PatchViewer.ico` & `patchview-0.3.2/patchview/PatchViewer.ico`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/ephys/ephys_extractor.py` & `patchview-0.3.2/patchview/ephys/ephys_extractor.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/ephys/ephys_features.py` & `patchview-0.3.2/patchview/ephys/ephys_features.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/ephys/extraEhpys_PV.py` & `patchview-0.3.2/patchview/ephys/extraEhpys_PV.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/examples/load_spike_list.py` & `patchview-0.3.2/patchview/examples/load_spike_list.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/patchview.py` & `patchview-0.3.2/patchview/patchview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Patchviewer by M.H.
 """
+import PyQt5
 from PyQt5 import QtGui, QtWidgets, QtCore
 from PyQt5.QtWidgets import QMessageBox, QTableWidgetItem
 from PyQt5.QtWidgets import QSplitter
 import pyqtgraph as pg
 import pyqtgraph.opengl as gl
 from pyqtgraph.parametertree import Parameter, ParameterTree
 from patchview.utilitis import AllMyParsHere as AllMyPars
@@ -97,15 +98,15 @@
 from patchview.utilitis.pvNDX_class import PatchviewSweepGroup, PatchviewSweep
 warnings.filterwarnings("ignore")
 import gc as GCollector
 from appdirs import *
 
 patchview_dir, this_filename = os.path.split(__file__)
 appname = "Patchview"
-__version__ = "0.3.0.0"
+__version__ = "0.3.2"
 
 class MainWindow(QtWidgets.QMainWindow):
     """
     Main frame.
     """
 
     def __init__(self, app, parent=None):
@@ -620,24 +621,22 @@
                 self.switchStateLine(lauto[lineIdx], manul="False")
             else:
                 self.switchStateLine(lman[lineIdx], manul="False")
         else:
             if self.events.eventMarker != None:
                 scatterPlot = self.events.eventMarker
                 penColor = (
-                    scatterPlot.getSpotOpts(scatterPlot.data[lineIdx])[2]
-                    .color()
-                    .getRgb()
+                    scatterPlot.data[lineIdx][-2].pen().color().getRgb()
                 )
                 if penColor[0] > 0:
                     pc = "g"  ## change r to g
                 else:
                     pc = "r"  ## change g to r
-                spotsPen = [scatterPlot.getSpotOpts(yy)[2] for yy in scatterPlot.data]
-                spotsBrush = [scatterPlot.getSpotOpts(yy)[3] for yy in scatterPlot.data]
+                spotsPen = [yy[-2].pen() for yy in scatterPlot.data]
+                spotsBrush = [yy[-2].brush() for yy in scatterPlot.data]
                 spotsPen[lineIdx] = pg.mkPen(pc)
                 spotsBrush[lineIdx] = pg.mkBrush(pc)
                 scatterPlot.setPen(spotsPen)
                 scatterPlot.setBrush(spotsBrush)
 
     def updateROI_table(self):
         data = np.array(
@@ -2053,17 +2052,20 @@
 
         ss = self.events.datFile
         if self.events.eventMarker == None:
             print("No events are marked!")
             return
         eventMarkers = self.events.eventMarker
         eventPenRvalue = [
-            eventMarkers.getSpotOpts(yy)[2].color().getRgb()[0]
+            # eventMarkers.getSpotOpts(yy)[2].color().getRgb()[0]
+            # eventMarkers.opts[idx]["pen"].color().getRgb()[0]
+            yy[-2].pen.color().getRgb()[0] if yy[-2] else 0
             for yy in eventMarkers.data
         ]  # red is for disabled one
+
         autoType = [
             True if eventPenRvalue[idx] == 0 else False
             for idx, index in enumerate(self.events.peakIndex)
         ]
         # autoIdx = [index for idx, index in enumerate(self.events.peakIndex) if eventStatus[idx]==0] ## only grab green ones
         autoIdx = self.events.peakIndex  ## only grab green ones
 
@@ -2701,69 +2703,71 @@
             return
         pv = self.eventParTree_data_view.p.getValues()  ##
         lfcut = pv["Data selection"][1]["Low frequency cutoff"][0]
         hfcut = pv["Data selection"][1]["High frequency cutoff"][0]
 
         self.events.isConcat = True
         self.events.traceYUnit = self.currentPulseTree.abf.yUnits
-        if self.events.traceYUnit == "V" or self.events.traceYUnit == "mV":
+        if 'v' in self.events.traceYUnit.lower():
             outlierCutoff_LV = pv["PSP Outliers"][1][
                 "Outlier voltage (mV) - lower bound"
             ][0]
             outlierCutoff_UV = pv["PSP Outliers"][1][
                 "Outlier voltage (mV) - upper bound"
             ][0]
             outlierCutoff_rv = pv["PSP Outliers"][1]["replacement value"][0]
+            rmSpks = True
         else:
             outlierCutoff_LV = pv["PSC Outliers"][1][
                 "Outlier voltage (pA) - lower bound"
             ][0]
             outlierCutoff_UV = pv["PSC Outliers"][1][
                 "Outlier voltage (pA) - upper bound"
             ][0]
             outlierCutoff_rv = pv["PSC Outliers"][1]["replacement value"][0]
+            rmSpks = False
 
         ## read data
         time, data = self.extractSingleSeries_ABF(series_index)
         nSweep = data.shape[1]
         data = data.reshape(
             (np.product(data.shape),), order="F"
         )  ## flatten from 2D to 1D concatenated
         self.events.data_raw = data  ## save a copy of raw data
         data = self.bandPass_signal(
             data, highCutOff=hfcut, lowCutOff=lfcut, useButter=True
         )
         time = np.arange(len(data)) / self.parameters["fs"]
-
+        baseline_ = np.mean(data)
         ## remove spiking and/or stimuli artifacts
-        data_ = data.copy()
-        baseline_ = np.mean(data_)
-        std_ = np.std(data_)
-        data_[data > baseline_ + 3 * std_] = baseline_
-        data_[data < baseline_ - 3 * std_] = baseline_
-        baseline_ = np.mean(data_)  ## iterative estamtion of baseline
-        if pv["Spikes"][1]["Removing spikes"][0]:
-            dvdt_th = pv["Spikes"][1]["dv/dt (V/s) - threhold"][0]
-            peaks_lv = self.removeStimulationArtifacts(data.copy(), dvdt_th)
-            for p in peaks_lv:
-                data[p - 20 : p + 20] = baseline_
+        if rmSpks:
+            data_ = data.copy()
+            std_ = np.std(data_)
+            data_[data > baseline_ + 3 * std_] = baseline_
+            data_[data < baseline_ - 3 * std_] = baseline_
+            baseline_ = np.mean(data_)  ## iterative estamtion of baseline
+            if  pv["Spikes"][1]["Removing spikes"][0]:
+                dvdt_th = pv["Spikes"][1]["dv/dt (V/s) - threhold"][0]
+                peaks_lv = self.removeStimulationArtifacts(data.copy(), dvdt_th)
+                for p in peaks_lv:
+                    data[p - 20 : p + 20] = baseline_
 
         currentTrace = pv["Data selection"][1]["Trace"][0] - 1
         self.events.node = []
         self.events.nSweep = nSweep
         self.events.seriesName = series_index[1] + 1
         self.events.traceName = currentTrace + 1
         self.events.datFile = datName  # self.currentPulseTree.dat_file
         self.events.setSeriesSampleRate(self.parameters["fs"])  ## series sampling rate
         self.events.globalBaseline = baseline_
         self.events.time = time
         self.events.data = data
         mean_data = np.mean(data)
         median_data = np.median(data)
-
+        print(f"mean: {mean_data}, median: {median_data}")
         if outlierCutoff_rv == "bound":
             data[data <= outlierCutoff_LV] = outlierCutoff_LV
             data[data >= outlierCutoff_UV] = outlierCutoff_UV
         elif outlierCutoff_rv == "median":
             data[data <= outlierCutoff_LV] = median_data
             data[data >= outlierCutoff_UV] = median_data
         elif outlierCutoff_rv == "mean":
@@ -3070,16 +3074,17 @@
 
             def marker_mouseClicked(scatterPlot, spots):
                 penColor = spots[0].pen().color().getRgb()
                 if penColor[0] > 0:
                     pc = "g"  # change r to g
                 else:
                     pc = invalidColor  ## change g to r
-                spotsPen = [scatterPlot.getSpotOpts(yy)[2] for yy in scatterPlot.data]
-                spotsBrush = [scatterPlot.getSpotOpts(yy)[3] for yy in scatterPlot.data]
+                print(f"pc, {pc}")
+                spotsPen = [yy[-2].pen() for yy in scatterPlot.data]
+                spotsBrush = [yy[-2].brush() for yy in scatterPlot.data]
                 spotsPen[spots[0].index()] = pg.mkPen(pc)
                 spotsBrush[spots[0].index()] = pg.mkBrush(pc)
                 scatterPlot.setPen(spotsPen)
                 scatterPlot.setBrush(spotsBrush)
 
             def marker_mouseHovered(scatterPlot, spot):  # update wave plot
                 if len(spot) > 0:
@@ -3762,14 +3767,15 @@
         )
         self.parameter_Tab.setData(data)
 
     #        self.parameter_Tab.show()
 
     def extractStimData_ABF(self):
         rawP = self.currentPulseTree.abf.read_raw_protocol()
+        print(self.currentPulseTree.abf.yUnits)
         nProtocol = len(rawP[0])  ## should be the same as nSegments for firing pattern.
         stimChanIdx = 0  ## channel index where stimuli is applied to
         stimUnit = rawP[2][stimChanIdx]  ## 'pA'
         stimData = rawP[0]
         self.currentPulseTree.stimUnit = stimUnit
         stimInfo = []
         for stim in stimData:
@@ -3802,15 +3808,19 @@
         ## loops through all the sweeps.
         nSweep = len(block.segments)
         nSamples = self.currentPulseTree.abf.get_signal_size(0, 0)
         data = np.zeros((nSamples, nSweep))
         for idx, seg in enumerate(block.segments):  # enumerate(block.segments):
             data[:, idx] = seg.analogsignals[0].transpose()[0]
         time = np.arange(nSamples) / self.parameters["fs"]
-        return time, data / 1000.0  ## convert it back to Volt for downstream analaysis
+        if 'm' in self.currentPulseTree.abf.yUnits.lower():
+            sfactor = 1e3
+        elif 'p' in self.currentPulseTree.abf.yUnits.lower():
+            sfactor = 1e12
+        return time, data/sfactor  ## convert it back to Volt for downstream analaysis
 
     def extractSingleSeries(self, sel):
         """Extract single series (multiple sweep) data"""
         print(self.parameters["Protocols"]["This serie"]["Type"])
         if self.parameters["Protocols"]["This serie"]["Type"] == "Firing pattern":
             stimChanIndex = self.parameters["Protocols"]["This serie"]["StimChanID"]
             traceID = self.getCellTraceID(sel, stimChanIndex)
@@ -5984,21 +5994,25 @@
                     segmentIdx = [sel.index[1], sel.index[2]]
                     trace = (
                         self.currentPulseTree.abfBlocks[segmentIdx[0]]
                         .segments[segmentIdx[1]]
                         .analogsignals[0]
                         .transpose()[0]
                     )
+                    if 'v' in self.currentPulseTree.abf.yUnits.lower():
+                        getSpikes = True
+                    else:
+                        getSpikes = False  ## skip analysing spikes if not voltage
                     self.plotSingleTrace_ABF(
                         plotHandle,
                         segmentIdx,
                         trace,
                         None,
                         highCutOff=None,
-                        analaysisSpike=True,
+                        analaysisSpike=getSpikes,
                     )
                 elif self.currentPulseTree.filetype == ".nwb": # sweep level
                     if len(selected) == 1: # if one sweep is slected.
                         sel  =selected[0]
                         children = getAllSiblings(sel)
                         # sel.setExpanded(True)
                         for c in children: # shrink all siblings
@@ -6942,15 +6956,15 @@
         )
         EphysObject.process_spikes()
         spike_df, sweep_df = extract_sweep_feature(t, v, curr, start, end, EphysObject)
         v_filtered = ephys_ft.calculate_v_filter(v, t, filterHighCutFreq_signal / 1000)
         dvdt = ephys_ft.calculate_dvdt(v, t, filterHighCutFreq_signal / 1000)
         dvdt1 = np.insert(dvdt, 0, 0)
         if EphysObject._spikes_df.size:
-            peaks = spike_df["peak_index"].to_list()  ## list of peak index
+            peaks = [int(p_) for p_ in spike_df["peak_index"].to_list()]  ## list of peak index
             try:
                 maxSPwidth = int(spike_df["width"].max(skipna=True) * sampleRate * 2.5)
             except:
                 maxSPwidth = int(
                     (spike_df["peak_index"] - spike_df["threshold_index"]).max() * 5
                 )
                 if not self.OptionAction5.isChecked():  ## that's OK for non-spike type
@@ -6970,15 +6984,14 @@
 
             waves = np.zeros((after_ + before_, len(peaks)))
             waves_dvdt = np.zeros((after_ + before_, len(peaks)))
             waveTime = np.arange(-before_, after_) / sampleRate * 1e3
             for j, p in enumerate(peaks):
                 start_index = p - before_
                 end_index = p + after_
-                # print(start_index, end_index, sweepCount)
                 waves[:, j] = v_filtered[start_index:end_index]
                 waves_dvdt[:, j] = dvdt1[start_index:end_index]
         else:
             peaks = []
             waves = []
             waves_dvdt = []
             waveTime = []
```

### Comparing `patchview-0.3.0/patchview/utilitis/AllMyParsHere.py` & `patchview-0.3.2/patchview/utilitis/AllMyParsHere.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/AnalysisMethods.py` & `patchview-0.3.2/patchview/utilitis/AnalysisMethods.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/NDX_files/XiaolongJiangLab.extensions.yaml` & `patchview-0.3.2/patchview/utilitis/NDX_files/XiaolongJiangLab.extensions.yaml`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/PVdat2NWB.py` & `patchview-0.3.2/patchview/utilitis/PVdat2NWB.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/dandi2pvNWB.py` & `patchview-0.3.2/patchview/utilitis/dandi2pvNWB.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/emfDraw.py` & `patchview-0.3.2/patchview/utilitis/emfDraw.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/fitFuncs.py` & `patchview-0.3.2/patchview/utilitis/fitFuncs.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/graphictools.py` & `patchview-0.3.2/patchview/utilitis/graphictools.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/linecollection_update.py` & `patchview-0.3.2/patchview/utilitis/linecollection_update.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/morphorFeatureExtrator.py` & `patchview-0.3.2/patchview/utilitis/morphorFeatureExtrator.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/patchviewObjects.py` & `patchview-0.3.2/patchview/utilitis/patchviewObjects.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/patchview_ndx.py` & `patchview-0.3.2/patchview/utilitis/patchview_ndx.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/pvEphy.py` & `patchview-0.3.2/patchview/utilitis/pvEphy.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview/utilitis/pvNDX_class.py` & `patchview-0.3.2/patchview/utilitis/pvNDX_class.py`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/patchview.egg-info/PKG-INFO` & `patchview-0.3.2/patchview.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-Metadata-Version: 2.1
-Name: patchview
-Version: 0.3.0
-Summary: Patchview perform data analysis and visualization on whole-cell recording data, including firing pattern analysis, event analysis, synatpic connection detection, morphorlocial analysis and more.
-Home-page: https://github.com/zeitgeberH/patchview
-Author: Ming Hu
-Author-email: hi@gmail.com
-License: BSD-3-Clause
-Keywords: patchview
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: furo
-Requires-Dist: morphopy
-Requires-Dist: colorcet
-Requires-Dist: appdirs
-Requires-Dist: Pillow
-Requires-Dist: pynwb
-Requires-Dist: tqdm
-Requires-Dist: PySide2
-Requires-Dist: pyqt5
-Requires-Dist: pyqtwebengine
-Requires-Dist: pyqt5-sip
-Requires-Dist: pyqtgraph==0.13.1
-Requires-Dist: PyOpenGL
-Requires-Dist: PyOpenGL_accelerate>=3.1.6; sys_platform == "win32"
-Requires-Dist: cython
-Requires-Dist: neo
-Requires-Dist: pylru==1.2.1
-Requires-Dist: h5py==3.7.0
-Requires-Dist: joblib
-Requires-Dist: future>=0.18.3
-Requires-Dist: pyYAML
-Requires-Dist: python-dateutil
-Requires-Dist: seaborn
-Requires-Dist: pytz
-Requires-Dist: scipy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: pycairo
-Requires-Dist: scikit-image
-Requires-Dist: morphio
-Requires-Dist: scikit-learn
-Requires-Dist: numpy<1.24,>=1.22
-Provides-Extra: dev
-
-===============
-PatchView
-===============
-.. image:: https://img.shields.io/pypi/v/patchview.svg 
-        :target: https://pypi.python.org/pypi/patchview
-      
-.. image:: https://img.shields.io/badge/python-3.10%2B-blue
-        :target: https://www.python.org/downloads/release/python
-        :alt: Python3.8
-
-.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
-        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
-        :alt: Documentation Status
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-
-.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
-        :target: https://opensource.org/licenses/BSD-3-Clause
-        :alt: BSD-3-Clause    
-
-.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
-   :target: https://doi.org/10.21105/joss.04706
-.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
-           
-
-.. image:: docs/resources/images/patchview_ads.png
-    :width: 800
-
-PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
-synaptic connection detection, morphological analysis and more.
-
-* Free software: BSD 3-Clause license
-* Documentation: https://patchview.readthedocs.io.
-
-
-Features
---------
-PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
-Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
-these tools or writing any Python scripts.
-
-* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
-* Visualizing single and multiple traces with zoom, pan operations.
-* Automatically sorting experiments data according to predefined labels.
-* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
-* Synaptic connection analysis.
-* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
-
-
-Citation
----------
-If you find our work useful for your research, please cite:
-
-    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
+Metadata-Version: 2.1
+Name: patchview
+Version: 0.3.2
+Summary: Patchview perform data analysis and visualization on whole-cell recording data, including firing pattern analysis, event analysis, synatpic connection detection, morphorlocial analysis and more.
+Home-page: https://github.com/zeitgeberH/patchview
+Author: Ming Hu
+Author-email: hi@gmail.com
+License: BSD-3-Clause
+Keywords: patchview
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: furo
+Requires-Dist: morphopy
+Requires-Dist: colorcet
+Requires-Dist: appdirs
+Requires-Dist: Pillow
+Requires-Dist: pynwb
+Requires-Dist: tqdm
+Requires-Dist: PySide2
+Requires-Dist: pyqt5
+Requires-Dist: pyqtwebengine
+Requires-Dist: pyqt5-sip
+Requires-Dist: pyqtgraph==0.13.1
+Requires-Dist: PyOpenGL
+Requires-Dist: PyOpenGL_accelerate>=3.1.6; sys_platform == "win32"
+Requires-Dist: cython
+Requires-Dist: neo
+Requires-Dist: pylru==1.2.1
+Requires-Dist: h5py
+Requires-Dist: joblib
+Requires-Dist: future>=0.18.3
+Requires-Dist: pyYAML
+Requires-Dist: python-dateutil
+Requires-Dist: seaborn
+Requires-Dist: pytz
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: pycairo
+Requires-Dist: scikit-image
+Requires-Dist: morphio
+Requires-Dist: scikit-learn
+Requires-Dist: numpy<1.24,>=1.22
+Provides-Extra: dev
+
+===============
+PatchView
+===============
+.. image:: https://img.shields.io/pypi/v/patchview.svg 
+        :target: https://pypi.python.org/pypi/patchview
+      
+.. image:: https://img.shields.io/badge/python-3.10%2B-blue
+        :target: https://www.python.org/downloads/release/python
+        :alt: Python3.8
+
+.. image:: https://readthedocs.org/projects/patchview/badge/?version=latest
+        :target: https://patchview.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+
+.. image:: https://img.shields.io/badge/License-BSD%203--Clause-blue.svg
+        :target: https://opensource.org/licenses/BSD-3-Clause
+        :alt: BSD-3-Clause    
+
+.. image:: https://joss.theoj.org/papers/10.21105/joss.04706/status.svg
+   :target: https://doi.org/10.21105/joss.04706
+.. image:: https://img.shields.io/pypi/dm/patchview?label=pypi%20downloads
+           
+
+.. image:: docs/resources/images/patchview_ads.png
+    :width: 800
+
+PatchView perform data analysis and visualization on multi channel whole-cell recording (multi-patch) data, including firing pattern analysis, event analysis,
+synaptic connection detection, morphological analysis and more.
+
+* Free software: BSD 3-Clause license
+* Documentation: https://patchview.readthedocs.io.
+
+
+Features
+--------
+PatchView integrates multiple open-source tools (see credit page) and wrap them using an intuitive graphic user interface (GUI).
+Thus users can perform most analysis quickly for the data collected in a typical patch-clamp experiment without installing Python and 
+these tools or writing any Python scripts.
+
+* Importing both Heka data and Axon Instruments data. Exporting to Python pickle file or NWB (Neurodata Without Borders) file format.
+* Visualizing single and multiple traces with zoom, pan operations.
+* Automatically sorting experiments data according to predefined labels.
+* Performing analysis on intrinsic membrane properties, action potential detection, firing pattern analysis.
+* Synaptic connection analysis.
+* Visualizing and quantification of neuron's morphological reconstruction from Neurolucida
+
+
+Citation
+---------
+If you find our work useful for your research, please cite:
+
+    Hu et al., (2022). PatchView: A Python Package for Patch-clamp Data Analysis and Visualization. Journal of Open Source Software, 7(78), 4706, https://doi.org/10.21105/joss.04706
```

### Comparing `patchview-0.3.0/patchview.egg-info/SOURCES.txt` & `patchview-0.3.2/patchview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patchview-0.3.0/setup.py` & `patchview-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     name='patchview',
     packages=find_packages(include=['patchview','patchview/Data',\
         'patchview/HekaIO','patchview/utilitis']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/zeitgeberH/patchview',
-    version = "0.3.0",
+    version = "0.3.2",
     zip_safe=False,
     entry_points={
         'gui_scripts': [
             'patchview=patchview:pvGUI'
         ],
     },
 )
```

