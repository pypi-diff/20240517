# Comparing `tmp/UnitMatchPy-1.2.tar.gz` & `tmp/UnitMatchPy-1.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnitMatchPy-1.2.tar", last modified: Thu May  2 10:53:14 2024, max compression
+gzip compressed data, was "UnitMatchPy-1.5b0.tar", last modified: Fri May 17 15:35:29 2024, max compression
```

## Comparing `UnitMatchPy-1.2.tar` & `UnitMatchPy-1.5b0.tar`

### file list

```diff
@@ -1,23 +1,378 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 10:53:14.138713 UnitMatchPy-1.2/
--rw-rw-rw-   0        0        0    21281 2023-12-13 15:09:14.000000 UnitMatchPy-1.2/LICENSE
--rw-rw-rw-   0        0        0     2325 2024-05-02 10:53:14.138713 UnitMatchPy-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2053 2024-05-01 10:16:34.000000 UnitMatchPy-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 10:53:14.120740 UnitMatchPy-1.2/UnitMatchPy/
--rw-rw-rw-   0        0        0     7092 2024-05-01 13:35:29.000000 UnitMatchPy-1.2/UnitMatchPy/AssignUniqueID.py
--rw-rw-rw-   0        0        0     2600 2024-05-01 13:35:22.000000 UnitMatchPy-1.2/UnitMatchPy/Bayes_fun.py
--rw-rw-rw-   0        0        0     8209 2024-05-01 13:35:20.000000 UnitMatchPy-1.2/UnitMatchPy/Extract_raw_data.py
--rw-rw-rw-   0        0        0    50594 2024-05-01 13:35:16.000000 UnitMatchPy-1.2/UnitMatchPy/GUI.py
--rw-rw-rw-   0        0        0    23396 2024-05-01 13:35:11.000000 UnitMatchPy-1.2/UnitMatchPy/Metrics_fun.py
--rw-rw-rw-   0        0        0     5258 2024-05-01 13:35:07.000000 UnitMatchPy-1.2/UnitMatchPy/Overlord.py
--rw-rw-rw-   0        0        0    13809 2024-05-01 13:35:03.000000 UnitMatchPy-1.2/UnitMatchPy/Param_fun.py
--rw-rw-rw-   0        0        0    13419 2024-05-01 13:34:57.000000 UnitMatchPy-1.2/UnitMatchPy/Save_utils.py
--rw-rw-rw-   0        0        0      228 2024-05-01 13:35:33.000000 UnitMatchPy-1.2/UnitMatchPy/__init__.py
--rw-rw-rw-   0        0        0    20911 2024-05-02 10:52:32.000000 UnitMatchPy-1.2/UnitMatchPy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 10:53:14.138713 UnitMatchPy-1.2/UnitMatchPy.egg-info/
--rw-rw-rw-   0        0        0     2325 2024-05-02 10:53:13.000000 UnitMatchPy-1.2/UnitMatchPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-02 10:53:13.000000 UnitMatchPy-1.2/UnitMatchPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 10:53:13.000000 UnitMatchPy-1.2/UnitMatchPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-02 10:53:13.000000 UnitMatchPy-1.2/UnitMatchPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-02 10:53:13.000000 UnitMatchPy-1.2/UnitMatchPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 10:53:14.138713 UnitMatchPy-1.2/setup.cfg
--rw-rw-rw-   0        0        0      644 2024-05-02 10:52:29.000000 UnitMatchPy-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.840255 UnitMatchPy-1.5b0/
+-rw-rw-rw-   0        0        0    21281 2023-12-13 15:09:14.000000 UnitMatchPy-1.5b0/LICENSE
+-rw-rw-rw-   0        0        0       31 2024-05-17 15:23:47.000000 UnitMatchPy-1.5b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2327 2024-05-17 15:35:29.839219 UnitMatchPy-1.5b0/PKG-INFO
+-rw-rw-rw-   0        0        0     2053 2024-05-01 10:16:34.000000 UnitMatchPy-1.5b0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.350176 UnitMatchPy-1.5b0/UnitMatchPy/
+-rw-rw-rw-   0        0        0     7288 2024-05-17 14:46:04.000000 UnitMatchPy-1.5b0/UnitMatchPy/AssignUniqueID.py
+-rw-rw-rw-   0        0        0     2600 2024-05-01 13:35:22.000000 UnitMatchPy-1.5b0/UnitMatchPy/Bayes_fun.py
+-rw-rw-rw-   0        0        0     8209 2024-05-01 13:35:20.000000 UnitMatchPy-1.5b0/UnitMatchPy/Extract_raw_data.py
+-rw-rw-rw-   0        0        0    50507 2024-05-17 15:28:42.000000 UnitMatchPy-1.5b0/UnitMatchPy/GUI.py
+-rw-rw-rw-   0        0        0    23396 2024-05-01 13:35:11.000000 UnitMatchPy-1.5b0/UnitMatchPy/Metrics_fun.py
+-rw-rw-rw-   0        0        0     5258 2024-05-01 13:35:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/Overlord.py
+-rw-rw-rw-   0        0        0    13809 2024-05-01 13:35:03.000000 UnitMatchPy-1.5b0/UnitMatchPy/Param_fun.py
+-rw-rw-rw-   0        0        0    13419 2024-05-01 13:34:57.000000 UnitMatchPy-1.5b0/UnitMatchPy/Save_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.294785 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.390803 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/LICENSE
+-rw-rw-rw-   0        0        0    15818 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/README.txt
+-rw-rw-rw-   0        0        0     2097 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awdark.tcl
+-rw-rw-rw-   0        0        0     1881 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awlight.tcl
+-rw-rw-rw-   0        0        0     6815 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awtemplate.tcl
+-rw-rw-rw-   0        0        0     5137 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.n7
+-rw-rw-rw-   0        0        0   170232 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awthemes.tcl
+-rw-rw-rw-   0        0        0     3562 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/awwinxpblue.tcl
+-rw-rw-rw-   0        0        0    10425 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/colorutils.tcl
+-rw-rw-rw-   0        0        0     7022 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaled.tcl
+-rw-rw-rw-   0        0        0     5311 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demoscaledb.tcl
+-rw-rw-rw-   0        0        0    42639 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/demottk.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.294785 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.392802 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/
+-rw-rw-rw-   0        0        0     3066 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/README.txt
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.297370 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.400831 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/
+-rw-rw-rw-   0        0        0     2614 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2596 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2608 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2608 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2699 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2703 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2704 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     2711 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-d.svg
+-rw-rw-rw-   0        0        0     2703 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/chevron/arrow-up-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.414919 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/
+-rw-rw-rw-   0        0        0     2593 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2686 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2687 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2755 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2757 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2757 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     2755 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/open/arrow-up-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.425084 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/
+-rw-rw-rw-   0        0        0     2506 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2590 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2590 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2660 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2662 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2636 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     2636 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid/arrow-up-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.438429 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/
+-rw-rw-rw-   0        0        0     2972 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2966 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2964 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2969 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-d.svg
+-rw-rw-rw-   0        0        0     2961 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-left-n.svg
+-rw-rw-rw-   0        0        0     2968 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-d.svg
+-rw-rw-rw-   0        0        0     2960 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2967 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-d.svg
+-rw-rw-rw-   0        0        0     2959 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/arrow-up-n.svg
+-rw-rw-rw-   0        0        0       77 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/arrow/solid-bg/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.302149 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.446768 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/
+-rw-rw-rw-   0        0        0     4016 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-a.svg
+-rw-rw-rw-   0        0        0     2984 2024-04-23 13:37:49.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-d.svg
+-rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-n.svg
+-rw-rw-rw-   0        0        0     3013 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/button-p.svg
+-rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-accent-gradient/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.459028 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/
+-rw-rw-rw-   0        0        0     2161 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-a.svg
+-rw-rw-rw-   0        0        0     2195 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af-base.svg
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-af.svg
+-rw-rw-rw-   0        0        0     2169 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-d.svg
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-f.svg
+-rw-rw-rw-   0        0        0     2197 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-n.svg
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/button-p.svg
+-rw-rw-rw-   0        0        0      117 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-flat/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.460603 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/
+-rw-rw-rw-   0        0        0     3596 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-d.svg
+-rw-rw-rw-   0        0        0     3573 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n-base.svg
+-rw-rw-rw-   0        0        0     3590 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/button-n.svg
+-rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/button/roundedrect-gradient/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.305204 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.472602 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/
+-rw-rw-rw-   0        0        0     3260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa-base.svg
+-rw-rw-rw-   0        0        0     3244 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sa.svg
+-rw-rw-rw-   0        0        0     3198 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sd.svg
+-rw-rw-rw-   0        0        0     2772 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3203 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-sn.svg
+-rw-rw-rw-   0        0        0     2199 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ua.svg
+-rw-rw-rw-   0        0        0     2200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-ud.svg
+-rw-rw-rw-   0        0        0     2202 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.488618 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/
+-rw-rw-rw-   0        0        0     3260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa-base.svg
+-rw-rw-rw-   0        0        0     3243 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sa.svg
+-rw-rw-rw-   0        0        0     3195 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sd.svg
+-rw-rw-rw-   0        0        0     2772 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-sn.svg
+-rw-rw-rw-   0        0        0     2199 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ua.svg
+-rw-rw-rw-   0        0        0     2200 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-ud.svg
+-rw-rw-rw-   0        0        0     2202 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-check-rev/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.500285 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/
+-rw-rw-rw-   0        0        0     2460 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sa.svg
+-rw-rw-rw-   0        0        0     2458 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sd.svg
+-rw-rw-rw-   0        0        0     2443 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     2457 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-sn.svg
+-rw-rw-rw-   0        0        0     2187 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ua.svg
+-rw-rw-rw-   0        0        0     2190 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-ud.svg
+-rw-rw-rw-   0        0        0     2186 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/roundedrect-square/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.506920 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/
+-rw-rw-rw-   0        0        0     3929 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sd.svg
+-rw-rw-rw-   0        0        0     3531 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3930 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-sn.svg
+-rw-rw-rw-   0        0        0     2963 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-ud.svg
+-rw-rw-rw-   0        0        0     2957 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-check-gradient/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.514869 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/
+-rw-rw-rw-   0        0        0     3079 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sd.svg
+-rw-rw-rw-   0        0        0     2965 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn-base.svg
+-rw-rw-rw-   0        0        0     3073 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-sn.svg
+-rw-rw-rw-   0        0        0     2169 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-ud.svg
+-rw-rw-rw-   0        0        0     2165 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/checkbutton/square-x/cb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.307197 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.527780 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/
+-rw-rw-rw-   0        0        0     3113 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     3109 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     3107 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2754 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-a.svg
+-rw-rw-rw-   0        0        0     2756 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-d.svg
+-rw-rw-rw-   0        0        0     2753 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-f.svg
+-rw-rw-rw-   0        0        0     2760 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n-base.svg
+-rw-rw-rw-   0        0        0     2752 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/combo-entry-n.svg
+-rw-rw-rw-   0        0        0       95 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/rounded/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.535587 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/
+-rw-rw-rw-   0        0        0     2861 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-a.svg
+-rw-rw-rw-   0        0        0     2796 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d-base.svg
+-rw-rw-rw-   0        0        0     2882 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2890 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2870 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/combo-arrow-down-n.svg
+-rw-rw-rw-   0        0        0       79 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/combobox/solid-bg/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.308404 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.536587 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/
+-rw-rw-rw-   0        0        0     1898 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/empty/empty/empty.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.309424 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.545294 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-a.svg
+-rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-d.svg
+-rw-rw-rw-   0        0        0     2253 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-f.svg
+-rw-rw-rw-   0        0        0     2283 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n-base.svg
+-rw-rw-rw-   0        0        0     2252 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/entry-n.svg
+-rw-rw-rw-   0        0        0       38 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/entry/roundedrect/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.309424 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.547294 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/
+-rw-rw-rw-   0        0        0     2083 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-d.svg
+-rw-rw-rw-   0        0        0     2081 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/labelframe/square/labelframe-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.309424 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.554620 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/
+-rw-rw-rw-   0        0        0     2938 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-a.svg
+-rw-rw-rw-   0        0        0     2933 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2930 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2923 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/chevron/mb-arrow-down-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.559407 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/
+-rw-rw-rw-   0        0        0     2486 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d-base.svg
+-rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-d.svg
+-rw-rw-rw-   0        0        0     2480 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2567 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/menubutton/solid/mb-arrow-down-n.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.313812 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.569079 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/
+-rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-a.svg
+-rw-rw-rw-   0        0        0     2768 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-d.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-h.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i-base.svg
+-rw-rw-rw-   0        0        0     2768 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/notebook-tab-i.svg
+-rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-dark/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.578172 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/
+-rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-a.svg
+-rw-rw-rw-   0        0        0     2771 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-d.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-h.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i-base.svg
+-rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/notebook-tab-i.svg
+-rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.590002 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/
+-rw-rw-rw-   0        0        0     2762 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-a.svg
+-rw-rw-rw-   0        0        0     2771 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-d.svg
+-rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-h.svg
+-rw-rw-rw-   0        0        0     2773 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i-base.svg
+-rw-rw-rw-   0        0        0     2764 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/notebook-tab-i.svg
+-rw-rw-rw-   0        0        0       71 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/notebook/roundedtop-light-accent/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.592412 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.612642 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/settings.tcl
+-rw-rw-rw-   0        0        0     2252 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hd.svg
+-rw-rw-rw-   0        0        0     2249 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn-base.svg
+-rw-rw-rw-   0        0        0     2250 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-hn.svg
+-rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vd.svg
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/slider-vn.svg
+-rw-rw-rw-   0        0        0     2256 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hd.svg
+-rw-rw-rw-   0        0        0     2249 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn-base.svg
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-hn.svg
+-rw-rw-rw-   0        0        0     2260 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vd.svg
+-rw-rw-rw-   0        0        0     2258 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect/trough-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.624306 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/settings.tcl
+-rw-rw-rw-   0        0        0     2268 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hd.svg
+-rw-rw-rw-   0        0        0     2309 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn-base.svg
+-rw-rw-rw-   0        0        0     2264 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-hn.svg
+-rw-rw-rw-   0        0        0     2267 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vd.svg
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-bord/slider-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.639226 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/
+-rw-rw-rw-   0        0        0    16071 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/diag-mask.svg
+-rw-rw-rw-   0        0        0       41 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/settings.tcl
+-rw-rw-rw-   0        0        0    16122 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hd.svg
+-rw-rw-rw-   0        0        0    16122 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn-base.svg
+-rw-rw-rw-   0        0        0    16118 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-hn.svg
+-rw-rw-rw-   0        0        0    16147 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vd.svg
+-rw-rw-rw-   0        0        0    16147 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn-base.svg
+-rw-rw-rw-   0        0        0    16143 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rect-diag/slider-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.659700 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/settings.tcl
+-rw-rw-rw-   0        0        0     2264 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hd.svg
+-rw-rw-rw-   0        0        0     2262 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-hn.svg
+-rw-rw-rw-   0        0        0     2257 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vd.svg
+-rw-rw-rw-   0        0        0     2255 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/slider-vn.svg
+-rw-rw-rw-   0        0        0     2268 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hd.svg
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn-base.svg
+-rw-rw-rw-   0        0        0     2266 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-hn.svg
+-rw-rw-rw-   0        0        0     2261 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vd.svg
+-rw-rw-rw-   0        0        0     2263 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn-base.svg
+-rw-rw-rw-   0        0        0     2259 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/rounded-line/trough-vn.svg
+-rw-rw-rw-   0        0        0       78 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/progressbar/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.319584 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.676540 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/
+-rw-rw-rw-   0        0        0     2300 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sa.svg
+-rw-rw-rw-   0        0        0     2297 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sd.svg
+-rw-rw-rw-   0        0        0     2340 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2311 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-sn.svg
+-rw-rw-rw-   0        0        0     2139 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ua.svg
+-rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-ud.svg
+-rw-rw-rw-   0        0        0     2152 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.686216 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/
+-rw-rw-rw-   0        0        0     3198 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sd.svg
+-rw-rw-rw-   0        0        0     3178 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     3204 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-sn.svg
+-rw-rw-rw-   0        0        0     2950 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-ud.svg
+-rw-rw-rw-   0        0        0     2960 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-gradient/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.697323 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/
+-rw-rw-rw-   0        0        0     2313 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sa.svg
+-rw-rw-rw-   0        0        0     2321 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sd.svg
+-rw-rw-rw-   0        0        0     2288 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2306 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-sn.svg
+-rw-rw-rw-   0        0        0     2120 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ua.svg
+-rw-rw-rw-   0        0        0     2126 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-ud.svg
+-rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-hlbg/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.708715 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/
+-rw-rw-rw-   0        0        0     2336 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sa.svg
+-rw-rw-rw-   0        0        0     2333 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sd.svg
+-rw-rw-rw-   0        0        0     2342 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2327 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-sn.svg
+-rw-rw-rw-   0        0        0     2155 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ua.svg
+-rw-rw-rw-   0        0        0     2138 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-ud.svg
+-rw-rw-rw-   0        0        0     2152 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/circle-circle-rev/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.717938 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/
+-rw-rw-rw-   0        0        0     2796 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sd.svg
+-rw-rw-rw-   0        0        0     3133 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn-base.svg
+-rw-rw-rw-   0        0        0     2806 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-sn.svg
+-rw-rw-rw-   0        0        0     2543 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-ud.svg
+-rw-rw-rw-   0        0        0     2557 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/radiobutton/octagon-circle/rb-un.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.323027 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.722620 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/
+-rw-rw-rw-   0        0        0     2163 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-ha.svg
+-rw-rw-rw-   0        0        0     2164 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hd.svg
+-rw-rw-rw-   0        0        0     2162 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle/scale-hn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.727376 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/
+-rw-rw-rw-   0        0        0     2160 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-ha.svg
+-rw-rw-rw-   0        0        0     2164 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hd.svg
+-rw-rw-rw-   0        0        0     2162 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/circle-rev/scale-hn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.733581 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/
+-rw-rw-rw-   0        0        0     7806 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hd.svg
+-rw-rw-rw-   0        0        0     7808 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn-base.svg
+-rw-rw-rw-   0        0        0     7778 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-hn.svg
+-rw-rw-rw-   0        0        0     7812 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vd.svg
+-rw-rw-rw-   0        0        0     7784 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-bord-grip/scale-vn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.760189 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/
+-rw-rw-rw-   0        0        0     3369 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hd.svg
+-rw-rw-rw-   0        0        0     3364 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn-base.svg
+-rw-rw-rw-   0        0        0     3359 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-hn.svg
+-rw-rw-rw-   0        0        0     2258 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hd.svg
+-rw-rw-rw-   0        0        0     2269 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn-base.svg
+-rw-rw-rw-   0        0        0     2254 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-hn.svg
+-rw-rw-rw-   0        0        0     2246 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vd.svg
+-rw-rw-rw-   0        0        0     2257 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn-base.svg
+-rw-rw-rw-   0        0        0     2242 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-trough-vn.svg
+-rw-rw-rw-   0        0        0     3423 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vd.svg
+-rw-rw-rw-   0        0        0     3413 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/scale-vn.svg
+-rw-rw-rw-   0        0        0       90 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scale/rect-narrow/settings.tcl
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.324028 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.766416 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/
+-rw-rw-rw-   0        0        0     7495 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip-base.svg
+-rw-rw-rw-   0        0        0     7453 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-h-grip.svg
+-rw-rw-rw-   0        0        0     7520 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip-base.svg
+-rw-rw-rw-   0        0        0     7500 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/scrollbar-grip/circle/sb-slider-v-grip.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.325029 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.769298 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/
+-rw-rw-rw-   0        0        0     5046 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip-base.svg
+-rw-rw-rw-   0        0        0     5058 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/sizegrip/circle/sizegrip.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.327030 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.776263 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/
+-rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-base.svg
+-rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     3000 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2993 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/chevron/tree-arrow-right-sn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.785959 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/
+-rw-rw-rw-   0        0        0     2593 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2685 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2685 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2627 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n-base.svg
+-rw-rw-rw-   0        0        0     2716 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2716 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/open/tree-arrow-right-sn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.791381 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/
+-rw-rw-rw-   0        0        0     3068 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     3005 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     3005 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     3035 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n-base.svg
+-rw-rw-rw-   0        0        0     3055 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     3056 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/plusminus-box/tree-arrow-right-sn.svg
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.801470 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/
+-rw-rw-rw-   0        0        0     2475 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n-base.svg
+-rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-n.svg
+-rw-rw-rw-   0        0        0     2578 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-down-sn.svg
+-rw-rw-rw-   0        0        0     2461 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n-base.svg
+-rw-rw-rw-   0        0        0     2570 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-n.svg
+-rw-rw-rw-   0        0        0     2570 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/i/awthemes/treeview/solid/tree-arrow-right-sn.svg
+-rw-rw-rw-   0        0        0     1811 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/TkinterTheme/awthemes-10.4.0/pkgIndex.tcl
+-rw-rw-rw-   0        0        0    14872 2024-04-23 13:36:45.000000 UnitMatchPy-1.5b0/UnitMatchPy/UM Logo.ico
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.806128 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/
+-rw-rw-rw-   0        0        0     2325 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 15:16:39.000000 UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      228 2024-05-01 13:35:33.000000 UnitMatchPy-1.5b0/UnitMatchPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.838222 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/
+-rw-rw-rw-   0        0        0     9564 2024-04-30 12:55:34.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/AssignUniqueID.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4322 2024-04-23 13:42:01.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Bayes_fun.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4066 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Bayes_fun.cpython-312.pyc
+-rw-rw-rw-   0        0        0     9387 2024-04-23 13:42:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8483 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Extract_raw_data.cpython-312.pyc
+-rw-rw-rw-   0        0        0    81032 2024-04-30 12:42:43.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/GUI.cpython-311.pyc
+-rw-rw-rw-   0        0        0    68574 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/GUI.cpython-312.pyc
+-rw-rw-rw-   0        0        0    32875 2024-04-23 13:42:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Metrics_fun.cpython-311.pyc
+-rw-rw-rw-   0        0        0    29945 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Metrics_fun.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5735 2024-04-23 13:42:07.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Overlord.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5433 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Overlord.cpython-312.pyc
+-rw-rw-rw-   0        0        0    17495 2024-04-23 13:42:01.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Param_fun.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16071 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Param_fun.cpython-312.pyc
+-rw-rw-rw-   0        0        0    16462 2024-04-30 12:57:43.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Save_utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0    13859 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/Save_utils.cpython-312.pyc
+-rw-rw-rw-   0        0        0      558 2024-04-23 13:42:01.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      431 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0    17825 2024-04-30 09:18:28.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/utils.cpython-311.pyc
+-rw-rw-rw-   0        0        0    14691 2024-04-23 13:37:50.000000 UnitMatchPy-1.5b0/UnitMatchPy/__pycache__/utils.cpython-312.pyc
+-rw-rw-rw-   0        0        0    20911 2024-05-02 10:52:32.000000 UnitMatchPy-1.5b0/UnitMatchPy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-17 15:35:29.371899 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/
+-rw-rw-rw-   0        0        0     2327 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    25269 2024-05-17 15:35:29.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-17 15:35:28.000000 UnitMatchPy-1.5b0/UnitMatchPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-17 15:35:29.840255 UnitMatchPy-1.5b0/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-05-17 15:35:16.000000 UnitMatchPy-1.5b0/setup.py
```

### Comparing `UnitMatchPy-1.2/LICENSE` & `UnitMatchPy-1.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/PKG-INFO` & `UnitMatchPy-1.5b0/UnitMatchPy/UnitMatchPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnitMatchPy
-Version: 1.2
+Version: 1.5
 Summary: Description of the package
 Author: Enny van Beest, Celian Bimbard and Sam Dodgson
 Author-email: e.beest@ucl.ac.uk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `UnitMatchPy-1.2/README.md` & `UnitMatchPy-1.5b0/README.md`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy/AssignUniqueID.py` & `UnitMatchPy-1.5b0/UnitMatchPy/AssignUniqueID.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,23 +9,24 @@
 
     Returns:
         IsIn -- ndarray (N) dtype - bool
     """    
     IsIn = (TestArray[:, None] == ParentArray).all(-1).any(-1)
     return IsIn
 
+
 def AssignUID(Output, param, ClusInfo):
 
     AllClusterIDs = ClusInfo['OriginalID'] # each units has unique ID
 
     #create arrays for the uniwue ids
     UniqueIDLiberal = np.arange(AllClusterIDs.shape[0])
     OriUniqueID = np.arange(AllClusterIDs.shape[0])
     UniqueIDConservative = np.arange(AllClusterIDs.shape[0])
-    UniqueID = np.arange(AllClusterIDs.shape[0])
+    UniqueID = np.arange(AllClusterIDs.shape[0]) #Intermediate Case
 
     GoodRecSesID = ClusInfo['SessionID']
     RecOpt = np.unique(ClusInfo['SessionID'])
     nRec = RecOpt.shape[0]
 
     #data Driven Threshold?
     if param.get('UseDataDrivenProbThrs', False):
@@ -84,60 +85,62 @@
         # delete the potential self-matches 
         CheckPairsA = np.delete(CheckPairsA, np.argwhere(CheckPairsA[:,0] == CheckPairsA[:,1]), axis =0)
         CheckPairsB = np.delete(CheckPairsB, np.argwhere(CheckPairsB[:,0] == CheckPairsB[:,1]), axis =0)
 
         if (np.logical_and(np.all(check_is_in(CheckPairsA, PairsAll)), np.all(check_is_in(CheckPairsB, PairsAll)))):
             #If each pairs matches with every unit in the other pairs group
             #can add as match to all classes
-            UniqueIDConservative[pair[0]] = min(UniqueIDConservative[pair])
-            UniqueIDConservative[pair[1]] = min(UniqueIDConservative[pair])
+            AllPairs = np.vstack((CheckPairsA, CheckPairsB))
+            AllGoupsIdxs = np.unique(AllPairs)
+            UniqueIDConservative[AllGoupsIdxs] = np.min(UniqueIDConservative[AllGoupsIdxs])
             nMatchesConservative +=1
 
-            UniqueID[pair[0]] = min(UniqueID[pair])
-            UniqueID[pair[1]] = min(UniqueID[pair])
+        ##Intermediate matches
+        #Now test to see if each pairs match with every unit in the other pair IF they are in the same/adjacent sessions 
+        UnitAID = UniqueID[pair[0]]
+        UnitBID = UniqueID[pair[1]]
+
+        SameGroupIdA = np.argwhere(UniqueID == UnitAID).squeeze()
+        SameGroupIdB = np.argwhere(UniqueID == UnitBID).squeeze()
+        if len(SameGroupIdA.shape) == 0:
+            SameGroupIdA = SameGroupIdA[np.newaxis]
+        if len(SameGroupIdB.shape) == 0:
+            SameGroupIdB = SameGroupIdB[np.newaxis]
+
+        CheckPairsA = np.stack((SameGroupIdB, np.broadcast_to(np.array(pair[0]), SameGroupIdB.shape)), axis = -1)
+        CheckPairsB = np.stack((SameGroupIdA, np.broadcast_to(np.array(pair[1]), SameGroupIdA.shape)), axis = -1)
+        #delte potential self-matches
+        CheckPairsA = np.delete(CheckPairsA, np.argwhere(CheckPairsA[:,0] == CheckPairsA[:,1]), axis =0)
+        CheckPairsB = np.delete(CheckPairsB, np.argwhere(CheckPairsB[:,0] == CheckPairsB[:,1]), axis =0)
+
+        #check to see if they are in the same or adjacent sessions
+        InNearSessionA = np.abs(np.diff(ClusInfo['SessionID'][CheckPairsA])) <= 1
+        InNearSessionB = np.abs(np.diff(ClusInfo['SessionID'][CheckPairsB])) <= 1
+
+        CheckPairsNearA = CheckPairsA[InNearSessionA.squeeze()]
+        CheckPairsNearB = CheckPairsB[InNearSessionB.squeeze()]
+
+        #Catch the csae where the units ARE NOT in adjacent session, so CheckPairsNear is empty
+        if np.logical_and(CheckPairsNearA.size == 0, CheckPairsNearB.size == 0):
+            AllPairs = np.vstack((CheckPairsA, CheckPairsB))
+            AllGoupsIdxs = np.unique(AllPairs)
+            UniqueID[AllGoupsIdxs] = np.min(UniqueID[AllGoupsIdxs])
+            nMatches +=1
+        elif (np.logical_and(np.all(check_is_in(CheckPairsNearA, PairsAll)), np.all(check_is_in(CheckPairsNearB, PairsAll)))):
+            AllPairs = np.vstack((CheckPairsA, CheckPairsB))
+            AllGoupsIdxs = np.unique(AllPairs)
+            UniqueID[AllGoupsIdxs] = np.min(UniqueID[AllGoupsIdxs])
             nMatches +=1
 
-            UniqueIDLiberal[pair[0]] = min(UniqueIDLiberal[pair])
-            UniqueIDLiberal[pair[0]] = min(UniqueIDLiberal[pair])
-            nMatchesLiberal +=1
-        else:
-            #Now test to see if each pairs match with every unit in the other pair IF they are in the same/adjacent sessions 
-            UnitAID = UniqueID[pair[0]]
-            UnitBID = UniqueID[pair[1]]
-
-            SameGroupIdA = np.argwhere(UniqueID == UnitAID).squeeze()
-            SameGroupIdB = np.argwhere(UniqueID == UnitBID).squeeze()
-            if len(SameGroupIdA.shape) == 0:
-                SameGroupIdA = SameGroupIdA[np.newaxis]
-            if len(SameGroupIdB.shape) == 0:
-                SameGroupIdB = SameGroupIdB[np.newaxis]
-
-            CheckPairsA = np.stack((SameGroupIdB, np.broadcast_to(np.array(pair[0]), SameGroupIdB.shape)), axis = -1)
-            CheckPairsB = np.stack((SameGroupIdA, np.broadcast_to(np.array(pair[1]), SameGroupIdA.shape)), axis = -1)
-            #delte potential self-matches
-            CheckPairsA = np.delete(CheckPairsA, np.argwhere(CheckPairsA[:,0] == CheckPairsA[:,1]), axis =0)
-            CheckPairsB = np.delete(CheckPairsB, np.argwhere(CheckPairsB[:,0] == CheckPairsB[:,1]), axis =0)
-
-            #check to see if they are in the same or adjacent sessions
-            InNearSessionA = np.abs(np.diff(ClusInfo['SessionID'][CheckPairsA])) <= 1
-            InNearSessionB = np.abs(np.diff(ClusInfo['SessionID'][CheckPairsB])) <= 1
-
-            CheckPairsNearA = CheckPairsA[InNearSessionA.squeeze()]
-            CheckPairsNearB = CheckPairsB[InNearSessionB.squeeze()]
-
-            if (np.logical_and(np.all(check_is_in(CheckPairsNearA, PairsAll)), np.all(check_is_in(CheckPairsNearB, PairsAll)))):
-                UniqueID[pair[0]] = min(UniqueID[pair])
-                UniqueID[pair[1]] = min(UniqueID[pair])
-                nMatches +=1
-
-                UniqueIDLiberal[pair[0]] = min(UniqueIDLiberal[pair])
-                UniqueIDLiberal[pair[1]] = min(UniqueIDLiberal[pair])
-                nMatchesLiberal +=1
-            else:
-                UniqueIDLiberal[pair[0]] = min(UniqueIDLiberal[pair])
-                UniqueIDLiberal[pair[1]] = min(UniqueIDLiberal[pair])
-                nMatchesLiberal +=1
-                
+        ## Liberal Matches
+        SameGroupIdA = np.argwhere(UniqueIDLiberal == UniqueIDLiberal[pair[0]]).squeeze()
+        SameGroupIdB = np.argwhere(UniqueIDLiberal == UniqueIDLiberal[pair[1]]).squeeze()
+
+        AllPairs = np.hstack((SameGroupIdA, SameGroupIdB))
+        AllGoupsIdxs = np.unique(AllPairs)
+        UniqueIDLiberal[AllGoupsIdxs] = np.min(UniqueIDLiberal[AllGoupsIdxs])
+        nMatchesLiberal +=1
+            
     print(f'Number of Liberal Matches: {nMatchesLiberal}')
     print(f'Number of Intermediate Matches: {nMatches}')
     print(f'Number of Conservative Matches: {nMatchesConservative}')
     return [UniqueIDLiberal, UniqueID, UniqueIDConservative, OriUniqueID]
```

### Comparing `UnitMatchPy-1.2/UnitMatchPy/Bayes_fun.py` & `UnitMatchPy-1.5b0/UnitMatchPy/Bayes_fun.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy/Extract_raw_data.py` & `UnitMatchPy-1.5b0/UnitMatchPy/Extract_raw_data.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy/GUI.py` & `UnitMatchPy-1.5b0/UnitMatchPy/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,17 @@
     rcParams['xtick.color'] = Color
     rcParams['ytick.color'] = Color
 
     
     np.set_printoptions(suppress = True)
     IsMatch = []
     NotMatch = []
-
     root = Tk()
-    #C:\Users\Experiment\Documents\temp\UnitMatch\UMPy\UMPy\TkinterTheme\awthemes-10.4.0\awdark.tcl
     # downloaded theme from https://sourceforge.net/projects/tcl-awthemes/
-    theme_path = os.path.join(os.path.dirname(os.path.abspath(__file__)) , r'TkinterTheme')
+    theme_path = os.path.join(os.path.dirname(os.path.abspath(__file__)) , r'TkinterTheme\awthemes-10.4.0')
     root.tk.call('lappend', 'auto_path', theme_path)
     root.tk.call('package', 'require', 'awdark')
     s = ttk.Style(root)
     s.theme_use('awdark')
     root.title('UMPy - Manual Curation')
     #root.geometry('800x800')
     root.iconbitmap(os.path.join(os.path.dirname(os.path.abspath(__file__)) , r'UM Logo.ico'))
```

### Comparing `UnitMatchPy-1.2/UnitMatchPy/Metrics_fun.py` & `UnitMatchPy-1.5b0/UnitMatchPy/Metrics_fun.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy/Overlord.py` & `UnitMatchPy-1.5b0/UnitMatchPy/Overlord.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy/Param_fun.py` & `UnitMatchPy-1.5b0/UnitMatchPy/Param_fun.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy/Save_utils.py` & `UnitMatchPy-1.5b0/UnitMatchPy/Save_utils.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy/utils.py` & `UnitMatchPy-1.5b0/UnitMatchPy/utils.py`

 * *Files identical despite different names*

### Comparing `UnitMatchPy-1.2/UnitMatchPy.egg-info/PKG-INFO` & `UnitMatchPy-1.5b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UnitMatchPy
-Version: 1.2
+Version: 1.5b0
 Summary: Description of the package
 Author: Enny van Beest, Celian Bimbard and Sam Dodgson
 Author-email: e.beest@ucl.ac.uk
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `UnitMatchPy-1.2/setup.py` & `UnitMatchPy-1.5b0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     description = f.read()
 
 setup(
     name="UnitMatchPy",
-    version="1.2",
+    version="1.5b",
     description="Description of the package",
     author="Enny van Beest, Celian Bimbard and Sam Dodgson",
     author_email="e.beest@ucl.ac.uk",
     packages=find_packages(),  
+    include_package_data=True,
     python_requires=">=3.7",
     install_requires=[
         "numpy",
         "scipy",
         "pandas",
         "matplotlib",
         "mtscomp",
```

