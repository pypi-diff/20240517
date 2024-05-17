# Comparing `tmp/ricco-1.4.1.tar.gz` & `tmp/ricco-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricco-1.4.1.tar", last modified: Wed Mar  6 08:47:01 2024, max compression
+gzip compressed data, was "ricco-1.4.2.tar", last modified: Fri May 17 03:14:03 2024, max compression
```

## Comparing `ricco-1.4.1.tar` & `ricco-1.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.948798 ricco-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-06 08:46:48.000000 ricco-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-03-06 08:47:01.948798 ricco-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-03-06 08:46:48.000000 ricco-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 08:47:01.948798 ricco-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-06 08:46:48.000000 ricco-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.932798 ricco-1.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.932798 ricco-1.4.1/src/ricco/
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.936798 ricco-1.4.1/src/ricco/etl/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/data_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    10022 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/stat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/etl/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.936798 ricco-1.4.1/src/ricco/geocode/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geocode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geocode/amap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geocode/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geocode/geocode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geocode/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.936798 ricco-1.4.1/src/ricco/geometry/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geometry/coord_trans.py
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geometry/df.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geometry/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geometry/topology_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/geometry/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.940798 ricco-1.4.1/src/ricco/resource/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   161544 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/area_code.py
--rw-r--r--   0 runner    (1001) docker     (127)   639350 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/bd_region.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/bd_region.py
--rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/city_id.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/crs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23330 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/epsg_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/names.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/resource/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.944798 ricco-1.4.1/src/ricco/util/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/address_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/assertion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/building_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/district.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/docx.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/id_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/os.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-03-06 08:46:48.000000 ricco-1.4.1/src/ricco/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.948798 ricco-1.4.1/src/ricco.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-03-06 08:47:01.000000 ricco-1.4.1/src/ricco.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-03-06 08:47:01.000000 ricco-1.4.1/src/ricco.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 08:47:01.000000 ricco-1.4.1/src/ricco.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-06 08:47:01.000000 ricco-1.4.1/src/ricco.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-06 08:47:01.000000 ricco-1.4.1/src/ricco.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:47:01.944798 ricco-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_address_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_district.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_id_number.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_os.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_topology_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-03-06 08:46:48.000000 ricco-1.4.1/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.812071 ricco-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-17 03:13:54.000000 ricco-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-17 03:14:03.812071 ricco-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-05-17 03:13:54.000000 ricco-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 03:14:03.812071 ricco-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-17 03:13:54.000000 ricco-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.800071 ricco-1.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.800071 ricco-1.4.2/src/ricco/
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.804071 ricco-1.4.2/src/ricco/etl/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/data_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11298 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9989 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14589 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/etl/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.804071 ricco-1.4.2/src/ricco/geocode/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geocode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geocode/amap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geocode/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geocode/geocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geocode/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.804071 ricco-1.4.2/src/ricco/geometry/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7765 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geometry/coord_trans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25021 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geometry/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geometry/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geometry/topology_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12286 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/geometry/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.808071 ricco-1.4.2/src/ricco/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161544 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/area_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)   639350 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/bd_region.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/bd_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24671 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/city_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/crs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23330 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/epsg_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/resource/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.808071 ricco-1.4.2/src/ricco/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5971 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/address_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/building_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/district.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/docx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/id_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7575 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-05-17 03:13:54.000000 ricco-1.4.2/src/ricco/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.812071 ricco-1.4.2/src/ricco.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-17 03:14:03.000000 ricco-1.4.2/src/ricco.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-17 03:14:03.000000 ricco-1.4.2/src/ricco.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 03:14:03.000000 ricco-1.4.2/src/ricco.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 03:14:03.000000 ricco-1.4.2/src/ricco.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-17 03:14:03.000000 ricco-1.4.2/src/ricco.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 03:14:03.812071 ricco-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_address_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_district.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_id_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_topology_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-17 03:13:54.000000 ricco-1.4.2/tests/test_util.py
```

### Comparing `ricco-1.4.1/PKG-INFO` & `ricco-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.4.1
+Version: 1.4.2
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Requires-Dist: geojson<3.0.0
 Requires-Dist: numpy>=1.0.0
 Requires-Dist: pandas<2.0.0
 Requires-Dist: requests>=2.7
+Requires-Dist: shapely<2.0.0
 Requires-Dist: tqdm>=4.62.0
 
 # 安装与更新
 
 ```shell
 pip install ricco
 pip install ricco -U # 或
```

### Comparing `ricco-1.4.1/README.md` & `ricco-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/setup.py` & `ricco-1.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     include_package_data=True,
     platforms='any',
     install_requires=[
       'geojson<3.0.0',
       'numpy>=1.0.0',
       'pandas<2.0.0',
       'requests>=2.7',
+      'shapely<2.0.0',
       'tqdm>=4.62.0',
     ],
     classifiers=[
       'Development Status :: 3 - Alpha',
       'Intended Audience :: Developers',
       'Natural Language :: English',
       'Operating System :: OS Independent',
```

### Comparing `ricco-1.4.1/src/ricco/__init__.py` & `ricco-1.4.2/src/ricco/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.4.1'
+__version__ = '1.4.2'
 
 from .base import ensure_list
 from .base import is_empty
 from .base import not_empty
 from .etl.extract import rdf
 from .etl.extract import rdf_by_dir
 from .etl.extract import read_all_sheets
```

### Comparing `ricco-1.4.1/src/ricco/base.py` & `ricco-1.4.2/src/ricco/base.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/etl/data_reporter.py` & `ricco-1.4.2/src/ricco/etl/data_reporter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import os
-
 import pandas as pd
 
 from ..base import ensure_list
 from ..util.decorator import print_doc
 from ..util.docx import Docx
 from .extract import rdf
 from .stat import describe_auto
@@ -22,24 +20,19 @@
 
   def __init__(
       self, data: (str, pd.DataFrame),
       only: list = None,
       exclude: list = None):
     self.set_default_style()
     self.doc.add_heading('数据检测报告', 0)
-    if isinstance(data, str):
-      if os.path.exists(data):
-        self.add_intense_quote(f'Data：{data}')
-        self.df = rdf(data, info=True)
-      else:
-        raise FileNotFoundError(f'未找到文件{data}')
-    elif isinstance(data, pd.DataFrame):
+    if isinstance(data, pd.DataFrame):
       self.df = data
     else:
-      raise ValueError('请输入Dataframe或路径')
+      self.add_intense_quote(f'Data：{data}')
+      self.df = rdf(data, info=True)
 
     columns = list(self.df.columns)
     if not only:
       only = columns
     elif exclude:
       only = [c for c in columns if c not in exclude]
```

### Comparing `ricco-1.4.1/src/ricco/etl/entropy.py` & `ricco-1.4.2/src/ricco/etl/entropy.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/etl/extract.py` & `ricco-1.4.2/src/ricco/etl/extract.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/etl/file.py` & `ricco-1.4.2/src/ricco/etl/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,22 +217,18 @@
   to_file(df, os.path.join(to_dir, f'part_{str(n).zfill(6)}{to_ext}'),
           log=log,
           **kwargs)
   print(f'输入文件总数: {len(path_list)}, 输入数据量: {total_lines}')
   print(f'输出文件总数: {n}, 输出数据量: {after_lines}')
 
 
-def df_iter_by_column(df: pd.DataFrame, by):
+def df_iter_by_column(df: pd.DataFrame, by, na='null'):
   """按列的值分组迭代df"""
-  if df[by].isna().any():
-    yield 'null', df[df[by].isna()]
-
-  df = df[df[by].notna()]
-  for enum in df[by].unique():
-    yield enum, df[df[by] == enum]
+  for enum, _df in df.groupby(by, as_index=False, dropna=False):
+    yield enum if pd.notna(enum) else na, _df
 
 
 def split_csv_by_column(
     filepath: str, by: str,
     *,
     to_dir: str = None,
     to_ext: str = '.csv',
```

### Comparing `ricco-1.4.1/src/ricco/etl/graph.py` & `ricco-1.4.2/src/ricco/etl/graph.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/etl/load.py` & `ricco-1.4.2/src/ricco/etl/load.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/etl/stat.py` & `ricco-1.4.2/src/ricco/etl/stat.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/etl/transformer.py` & `ricco-1.4.2/src/ricco/etl/transformer.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geocode/amap.py` & `ricco-1.4.2/src/ricco/geocode/amap.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geocode/baidu.py` & `ricco-1.4.2/src/ricco/geocode/baidu.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geocode/geocode.py` & `ricco-1.4.2/src/ricco/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geocode/util.py` & `ricco-1.4.2/src/ricco/geocode/util.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geometry/__init__.py` & `ricco-1.4.2/src/ricco/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geometry/coord_trans.py` & `ricco-1.4.2/src/ricco/geometry/coord_trans.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geometry/df.py` & `ricco-1.4.2/src/ricco/geometry/df.py`

 * *Files 4% similar despite different names*

```diff
@@ -436,34 +436,41 @@
     geometry_format='wkb',
     warning=True,
     point_lng='lng',
     point_lat='lat',
     point_geometry='geometry',
     polygon_geometry='geometry',
     warning_message=None,
+    ensure_point=True
 ):
   """
   使用面数据通过空间关联（sjoin）给数据打标签
 
   Args:
     point_df: 点数据
     polygon_df: 面数据
     col_list: 面数据中要关联到结果中的列，若为空则全部关联
     predicate: 关联方法，默认 'intersects'
-    drop_geometry: 结果是否删除geometry，默认删除
+    drop_geometry: 结果是否删除geometry，默认不删除
     geometry_format: 输出的geometry格式，支持wkb,wkt,shapely,geojson，默认wkb
     warning: 是否输出警告信息
     point_lng: 指定点数据的经度列名
     point_lat: 指定点数据的经度列名
     point_geometry: 指定点数据的geometry列名
     polygon_geometry: 指定面数据的geometry列名
     warning_message: 是否输出警告信息，已弃用
+    ensure_point: point_df是否强制转换为点数据
   """
   if warning_message is not None:
     warn_('参数"warning_message"已弃用，请使用参数"warning"')
+
+  if point_df.empty or point_df.empty:
+    warn_('存在空的数据集，请检查', warning)
+    return point_df
+
   point_df = point_df.copy()
   assert point_df.index.is_unique, 'point_df索引列必须唯一'
   if not col_list:
     col_list = polygon_df.columns.to_list()
   else:
     col_list = ensure_list(col_list)
     polygon_df = polygon_df[[*col_list, polygon_geometry]]
@@ -472,35 +479,30 @@
     c: f'{c}_origin' for c in col_list
     if c in point_df and c not in [point_lng, point_lat, point_geometry]
   }:
     warn_(f'同名字段重命名：{cols_mapping}', warning)
     point_df.rename(columns=cols_mapping, inplace=True)
 
   # 转换为shapely格式
-  df = ensure_geometry(point_df, True, warning,
-                       lng=point_lng, lat=point_lat, geometry=point_geometry)
+  _df = ensure_geometry(point_df, ensure_point, warning,
+                        lng=point_lng, lat=point_lat, geometry=point_geometry)
   polygon_df = auto2shapely(polygon_df, geometry=polygon_geometry)
   # 空间关联
-  df = df.sjoin(
+  _df = _df.sjoin(
       polygon_df, how='left', predicate=predicate,
   ).drop(['index_right'], axis=1)
+  del _df[point_geometry]
   # 统一geometry输出格式、删除geometry、避免多次转换
   if point_geometry in point_df:
-    if geometry_format != 'shapely':
-      del df[point_geometry]
-    if geometry_format == 'shapely' or drop_geometry:
+    if drop_geometry:
       del point_df[point_geometry]
     else:
       point_df = auto2x(point_df, geometry_format, geometry=point_geometry)
-  elif drop_geometry:
-    del df[point_geometry]
-  else:
-    df = shapely2x(df, geometry_format, geometry=point_geometry)
   # 将空间关联后的数据关联到原来的Dataframe上
-  return point_df.join(df, how='left')
+  return point_df.join(_df, how='left')
 
 
 def nearest_neighbor(
     df: pd.DataFrame,
     df_target: pd.DataFrame,
     c_dst: str = 'min_distance',
     epsg: int = None) -> pd.DataFrame:
```

### Comparing `ricco-1.4.1/src/ricco/geometry/topology.py` & `ricco-1.4.2/src/ricco/geometry/topology.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/geometry/util.py` & `ricco-1.4.2/src/ricco/geometry/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,14 +354,36 @@
   for p in points:
     lnglat = p.split(lnglat_sep)
     lnglat = [float(i) for i in lnglat if i != '']
     res.append(lnglat)
   return [i for i, _ in groupby(res)]
 
 
+def deg_to_decimal(x: (str, list, tuple)):
+  """
+  将度分秒格式的经纬度转为小数
+
+  Args:
+    x: 字符串或列表，
+      - 字符串格式为 123°5'6.77"（分和秒分别为单双引号）
+      - 列表长度为3，分别是度分秒，数值型
+  """
+  if isinstance(x, str):
+    x = x.strip('"')
+    d, m_s = x.split('°', 1)
+    m, s = m_s.split("'")
+  elif isinstance(x, (tuple, list)):
+    assert len(x) == 3, '长度必须为3'
+    d, m, s = x
+  else:
+    raise TypeError('类型错误，必须为字符串或列表')
+  d, m, s = [float(i) for i in (d, m, s)]
+  return d + m / 60 + s / 3600
+
+
 def text2shapely(
     text: str,
     geometry_type: str,
     point_sep: str = ';',
     lnglat_sep: str = ',',
     ensure_multi: bool = True):
   """
```

### Comparing `ricco-1.4.1/src/ricco/local.py` & `ricco-1.4.2/src/ricco/local.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/area_code.py` & `ricco-1.4.2/src/ricco/resource/area_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/bd_region.csv` & `ricco-1.4.2/src/ricco/resource/bd_region.csv`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/bd_region.py` & `ricco-1.4.2/src/ricco/resource/bd_region.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/city_id.py` & `ricco-1.4.2/src/ricco/resource/city_id.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/epsg_code.py` & `ricco-1.4.2/src/ricco/resource/epsg_code.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/names.py` & `ricco-1.4.2/src/ricco/resource/names.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/patterns.py` & `ricco-1.4.2/src/ricco/resource/patterns.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/resource/phone_number.py` & `ricco-1.4.2/src/ricco/resource/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/address_tools.py` & `ricco-1.4.2/src/ricco/util/address_tools.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/assertion.py` & `ricco-1.4.2/src/ricco/util/assertion.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/base.py` & `ricco-1.4.2/src/ricco/util/base.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/building_address.py` & `ricco-1.4.2/src/ricco/util/building_address.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/decorator.py` & `ricco-1.4.2/src/ricco/util/decorator.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/district.py` & `ricco-1.4.2/src/ricco/util/district.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/docx.py` & `ricco-1.4.2/src/ricco/util/docx.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/dt.py` & `ricco-1.4.2/src/ricco/util/dt.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/id_generator.py` & `ricco-1.4.2/src/ricco/util/id_generator.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/id_number.py` & `ricco-1.4.2/src/ricco/util/id_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/kdtree.py` & `ricco-1.4.2/src/ricco/util/kdtree.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/media.py` & `ricco-1.4.2/src/ricco/util/media.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/os.py` & `ricco-1.4.2/src/ricco/util/os.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/phone_number.py` & `ricco-1.4.2/src/ricco/util/phone_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/random.py` & `ricco-1.4.2/src/ricco/util/random.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/strings.py` & `ricco-1.4.2/src/ricco/util/strings.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco/util/util.py` & `ricco-1.4.2/src/ricco/util/util.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/src/ricco.egg-info/PKG-INFO` & `ricco-1.4.2/src/ricco.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ricco
-Version: 1.4.1
+Version: 1.4.2
 Summary: A handy ETL&GEOM kit
 Home-page: https://github.com/Ricco1010/ricco
 Author: Ricco Wang
 Author-email: wyk_0610@163.com
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Requires-Dist: geojson<3.0.0
 Requires-Dist: numpy>=1.0.0
 Requires-Dist: pandas<2.0.0
 Requires-Dist: requests>=2.7
+Requires-Dist: shapely<2.0.0
 Requires-Dist: tqdm>=4.62.0
 
 # 安装与更新
 
 ```shell
 pip install ricco
 pip install ricco -U # 或
```

### Comparing `ricco-1.4.1/src/ricco.egg-info/SOURCES.txt` & `ricco-1.4.2/src/ricco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/tests/test_address_tools.py` & `ricco-1.4.2/tests/test_address_tools.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/tests/test_entropy.py` & `ricco-1.4.2/tests/test_entropy.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/tests/test_geometry.py` & `ricco-1.4.2/tests/test_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,15 @@
 def test_mark_tags_v2():
   """测试空间连接打标签的方法"""
 
   # lnglat -- wkb
   df1 = pd.DataFrame(point_df[['name', 'lng', 'lat']])
   df2 = pd.DataFrame(polygon_df[[
     '板块', 'geometry_wkb']].rename(columns={'geometry_wkb': 'geometry'}))
-  df3 = pd.DataFrame(res_df[[
-    'name', 'lng', 'lat', 'geometry_wkb', '板块'
-  ]].rename(columns={'geometry_wkb': 'geometry'}))
+  df3 = pd.DataFrame(res_df[['name', 'lng', 'lat', '板块']])
   assert_frame_equal(mark_tags_v2(df1, df2, '板块'), df3)
 
   # wkb -- wkb, with lnglat
   assert_frame_equal(
       mark_tags_v2(
           point_df[['name', 'lng', 'lat', 'geometry_wkb']].rename(
               columns={'geometry_wkb': 'geometry'}),
@@ -159,16 +157,15 @@
               columns={'geometry_wkb2': 'geometry2'}),
           col_list=['板块'],
           point_lng='lng2',
           point_lat='lat2',
           point_geometry='geometry2',
           polygon_geometry='geometry2',
       ),
-      res[['name', 'lng2', 'lat2', 'geometry_wkb2', '板块']].rename(
-          columns={'geometry_wkb2': 'geometry2'})
+      res[['name', 'lng2', 'lat2', '板块']]
   )
 
   # wkb -- wkb, with lnglat
   assert_frame_equal(
       mark_tags_v2(
           point[['name', 'lng2', 'lat2', 'geometry_wkb2']].rename(
               columns={'geometry_wkb2': 'geometry2'}),
```

### Comparing `ricco-1.4.1/tests/test_id_number.py` & `ricco-1.4.2/tests/test_id_number.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/tests/test_strings.py` & `ricco-1.4.2/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/tests/test_topology_check.py` & `ricco-1.4.2/tests/test_topology_check.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/tests/test_transformer.py` & `ricco-1.4.2/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `ricco-1.4.1/tests/test_util.py` & `ricco-1.4.2/tests/test_util.py`

 * *Files identical despite different names*

