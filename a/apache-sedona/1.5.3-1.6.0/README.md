# Comparing `tmp/apache_sedona-1.5.3.tar.gz` & `tmp/apache_sedona-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_sedona-1.5.3.tar", last modified: Fri May 10 06:44:30 2024, max compression
+gzip compressed data, was "apache_sedona-1.6.0.tar", last modified: Fri May 17 18:23:31 2024, max compression
```

## Comparing `apache_sedona-1.5.3.tar` & `apache_sedona-1.6.0.tar`

### file list

```diff
@@ -1,119 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.948583 apache_sedona-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-10 06:44:30.948583 apache_sedona-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.948583 apache_sedona-1.5.3/apache_sedona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-10 06:44:30.000000 apache_sedona-1.5.3/apache_sedona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-10 06:44:30.000000 apache_sedona-1.5.3/apache_sedona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:44:30.000000 apache_sedona-1.5.3/apache_sedona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-10 06:44:30.000000 apache_sedona-1.5.3/apache_sedona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 06:44:30.000000 apache_sedona-1.5.3/apache_sedona.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.932583 apache_sedona-1.5.3/sedona/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.932583 apache_sedona-1.5.3/sedona/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.936583 apache_sedona-1.5.3/sedona/core/SpatialRDD/
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/circle_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/linestring_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/point_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/polygon_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/rectangle_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/spatial_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/SpatialRDD/spatial_rdd_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.936583 apache_sedona-1.5.3/sedona/core/enums/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/enums/file_data_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/enums/grid_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/enums/index_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/enums/join_build_side.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/enums/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.936583 apache_sedona-1.5.3/sedona/core/formatMapper/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/disc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/geo_json_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/geo_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.936583 apache_sedona-1.5.3/sedona/core/formatMapper/shapefileParser/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/shapefileParser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/shapefileParser/shape_file_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/wkb_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/formatMapper/wkt_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.936583 apache_sedona-1.5.3/sedona/core/geom/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/geom/circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3864 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/geom/envelope.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.936583 apache_sedona-1.5.3/sedona/core/jvm/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/jvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/jvm/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/jvm/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/jvm/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.940583 apache_sedona-1.5.3/sedona/core/spatialOperator/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/join_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/join_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/join_query_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/knn_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/range_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/range_query_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/spatialOperator/rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.940583 apache_sedona-1.5.3/sedona/maps/
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/maps/SedonaKepler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/maps/SedonaMapUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/maps/SedonaPyDeck.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/maps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.940583 apache_sedona-1.5.3/sedona/raster_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/raster_utils/SedonaUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/raster_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.940583 apache_sedona-1.5.3/sedona/register/
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/register/geo_registrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/register/java_libs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.940583 apache_sedona-1.5.3/sedona/spark/
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/spark/SedonaContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.944583 apache_sedona-1.5.3/sedona/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/dataframe_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/st_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/st_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)    61309 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/st_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/st_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/sql/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.944583 apache_sedona-1.5.3/sedona/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/abstract_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/binary_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/geometry_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/geometry_serde.py
--rw-r--r--   0 runner    (1001) docker     (127)    19092 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/geometry_serde_general.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/serde.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/spatial_rdd_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/sedona/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:44:30.948583 apache_sedona-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.944583 apache_sedona-1.5.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geom_buf.c
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geom_buf.h
--rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geomserde.c
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geomserde.h
--rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geomserde_speedup_module.c
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geos_c_dyn.c
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geos_c_dyn.h
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/geos_c_dyn_funcs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.948583 apache_sedona-1.5.3/src/pygeos/
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/src/pygeos/c_api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:44:30.948583 apache_sedona-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/tests/test_assign_raw_spatial_rdd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/tests/test_circle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/tests/test_multiple_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-10 06:44:27.000000 apache_sedona-1.5.3/tests/test_scala_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.516154 apache_sedona-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-17 18:23:31.516154 apache_sedona-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.516154 apache_sedona-1.6.0/apache_sedona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-17 18:23:31.000000 apache_sedona-1.6.0/apache_sedona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-17 18:23:31.000000 apache_sedona-1.6.0/apache_sedona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 18:23:31.000000 apache_sedona-1.6.0/apache_sedona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-17 18:23:31.000000 apache_sedona-1.6.0/apache_sedona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 18:23:31.000000 apache_sedona-1.6.0/apache_sedona.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.500154 apache_sedona-1.6.0/sedona/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.500154 apache_sedona-1.6.0/sedona/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.500154 apache_sedona-1.6.0/sedona/core/SpatialRDD/
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/circle_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5723 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/linestring_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/point_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/polygon_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/rectangle_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15014 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/spatial_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/SpatialRDD/spatial_rdd_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.500154 apache_sedona-1.6.0/sedona/core/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/enums/file_data_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/enums/grid_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/enums/index_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/enums/join_build_side.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/enums/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.504154 apache_sedona-1.6.0/sedona/core/formatMapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/disc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/geo_json_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/geo_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.504154 apache_sedona-1.6.0/sedona/core/formatMapper/shapefileParser/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/shapefileParser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/shapefileParser/shape_file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/wkb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/formatMapper/wkt_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.504154 apache_sedona-1.6.0/sedona/core/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/envelope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.504154 apache_sedona-1.6.0/sedona/core/geom/shapely1/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/shapely1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/shapely1/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/shapely1/envelope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.504154 apache_sedona-1.6.0/sedona/core/geom/shapely2/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/shapely2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/shapely2/circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/geom/shapely2/envelope.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.504154 apache_sedona-1.6.0/sedona/core/jvm/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/jvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/jvm/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/jvm/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/jvm/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.508154 apache_sedona-1.6.0/sedona/core/spatialOperator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/join_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/join_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/join_query_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/knn_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/range_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/range_query_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/spatialOperator/rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.508154 apache_sedona-1.6.0/sedona/maps/
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/maps/SedonaKepler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/maps/SedonaMapUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11625 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/maps/SedonaPyDeck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/maps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.508154 apache_sedona-1.6.0/sedona/raster/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster/awt_raster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster/data_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster/raster_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster/sample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster/sedona_raster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.508154 apache_sedona-1.6.0/sedona/raster_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster_utils/SedonaUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/raster_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.508154 apache_sedona-1.6.0/sedona/register/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/register/geo_registrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/register/java_libs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.508154 apache_sedona-1.6.0/sedona/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/spark/SedonaContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.512154 apache_sedona-1.6.0/sedona/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/dataframe_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/st_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/st_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65451 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/st_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/st_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/sql/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.512154 apache_sedona-1.6.0/sedona/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/abstract_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/binary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/geometry_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/geometry_serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19104 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/geometry_serde_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6281 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/serde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/spatial_rdd_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/sedona/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 18:23:31.516154 apache_sedona-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.516154 apache_sedona-1.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    16382 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geom_buf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geom_buf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24131 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geomserde.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geomserde.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9326 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geomserde_speedup_module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geos_c_dyn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geos_c_dyn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/geos_c_dyn_funcs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.516154 apache_sedona-1.6.0/src/pygeos/
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/src/pygeos/c_api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 18:23:31.516154 apache_sedona-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/tests/test_assign_raw_spatial_rdd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7286 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/tests/test_circle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/tests/test_multiple_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-17 18:23:25.000000 apache_sedona-1.6.0/tests/test_scala_example.py
```

### Comparing `apache_sedona-1.5.3/PKG-INFO` & `apache_sedona-1.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-sedona
-Version: 1.5.3
+Version: 1.6.0
 Summary: Apache Sedona is a cluster computing system for processing large-scale spatial data
 Home-page: https://sedona.apache.org
 Author: Apache Sedona
 Author-email: dev@sedona.apache.org
 License: Apache License v2.0
 Project-URL: Documentation, https://sedona.apache.org
 Project-URL: Source code, https://github.com/apache/sedona
 Project-URL: Bug Reports, https://issues.apache.org/jira/projects/SEDONA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: shapely>=1.7.0
+Requires-Dist: rasterio>=1.2.10
 Provides-Extra: spark
 Requires-Dist: pyspark>=2.3.0; extra == "spark"
 Provides-Extra: pydeck-map
-Requires-Dist: pandas<=1.3.5; extra == "pydeck-map"
-Requires-Dist: geopandas<=0.10.2; extra == "pydeck-map"
+Requires-Dist: geopandas; extra == "pydeck-map"
 Requires-Dist: pydeck==0.8.0; extra == "pydeck-map"
 Provides-Extra: kepler-map
-Requires-Dist: pandas<=1.3.5; extra == "kepler-map"
-Requires-Dist: geopandas<=0.10.2; extra == "kepler-map"
+Requires-Dist: geopandas; extra == "kepler-map"
 Requires-Dist: keplergl==0.3.2; extra == "kepler-map"
 Provides-Extra: all
 Requires-Dist: pyspark>=2.3.0; extra == "all"
-Requires-Dist: pandas<=1.3.5; extra == "all"
-Requires-Dist: geopandas<=0.10.2; extra == "all"
+Requires-Dist: geopandas; extra == "all"
 Requires-Dist: pydeck==0.8.0; extra == "all"
 Requires-Dist: keplergl==0.3.2; extra == "all"
 
 # Apache Sedona
 
 <img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=acc24e73-991b-4e92-8a6d-e33f333a645d" />
```

### Comparing `apache_sedona-1.5.3/README.md` & `apache_sedona-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/apache_sedona.egg-info/PKG-INFO` & `apache_sedona-1.6.0/apache_sedona.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: apache-sedona
-Version: 1.5.3
+Version: 1.6.0
 Summary: Apache Sedona is a cluster computing system for processing large-scale spatial data
 Home-page: https://sedona.apache.org
 Author: Apache Sedona
 Author-email: dev@sedona.apache.org
 License: Apache License v2.0
 Project-URL: Documentation, https://sedona.apache.org
 Project-URL: Source code, https://github.com/apache/sedona
 Project-URL: Bug Reports, https://issues.apache.org/jira/projects/SEDONA
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: shapely>=1.7.0
+Requires-Dist: rasterio>=1.2.10
 Provides-Extra: spark
 Requires-Dist: pyspark>=2.3.0; extra == "spark"
 Provides-Extra: pydeck-map
-Requires-Dist: pandas<=1.3.5; extra == "pydeck-map"
-Requires-Dist: geopandas<=0.10.2; extra == "pydeck-map"
+Requires-Dist: geopandas; extra == "pydeck-map"
 Requires-Dist: pydeck==0.8.0; extra == "pydeck-map"
 Provides-Extra: kepler-map
-Requires-Dist: pandas<=1.3.5; extra == "kepler-map"
-Requires-Dist: geopandas<=0.10.2; extra == "kepler-map"
+Requires-Dist: geopandas; extra == "kepler-map"
 Requires-Dist: keplergl==0.3.2; extra == "kepler-map"
 Provides-Extra: all
 Requires-Dist: pyspark>=2.3.0; extra == "all"
-Requires-Dist: pandas<=1.3.5; extra == "all"
-Requires-Dist: geopandas<=0.10.2; extra == "all"
+Requires-Dist: geopandas; extra == "all"
 Requires-Dist: pydeck==0.8.0; extra == "all"
 Requires-Dist: keplergl==0.3.2; extra == "all"
 
 # Apache Sedona
 
 <img referrerpolicy="no-referrer-when-downgrade" src="https://static.scarf.sh/a.png?x-pxid=acc24e73-991b-4e92-8a6d-e33f333a645d" />
```

### Comparing `apache_sedona-1.5.3/apache_sedona.egg-info/SOURCES.txt` & `apache_sedona-1.6.0/apache_sedona.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 sedona/core/formatMapper/wkb_reader.py
 sedona/core/formatMapper/wkt_reader.py
 sedona/core/formatMapper/shapefileParser/__init__.py
 sedona/core/formatMapper/shapefileParser/shape_file_reader.py
 sedona/core/geom/__init__.py
 sedona/core/geom/circle.py
 sedona/core/geom/envelope.py
+sedona/core/geom/shapely1/__init__.py
+sedona/core/geom/shapely1/circle.py
+sedona/core/geom/shapely1/envelope.py
+sedona/core/geom/shapely2/__init__.py
+sedona/core/geom/shapely2/circle.py
+sedona/core/geom/shapely2/envelope.py
 sedona/core/jvm/__init__.py
 sedona/core/jvm/abstract.py
 sedona/core/jvm/config.py
 sedona/core/jvm/translate.py
 sedona/core/spatialOperator/__init__.py
 sedona/core/spatialOperator/join_params.py
 sedona/core/spatialOperator/join_query.py
@@ -48,14 +54,21 @@
 sedona/core/spatialOperator/range_query.py
 sedona/core/spatialOperator/range_query_raw.py
 sedona/core/spatialOperator/rdd.py
 sedona/maps/SedonaKepler.py
 sedona/maps/SedonaMapUtils.py
 sedona/maps/SedonaPyDeck.py
 sedona/maps/__init__.py
+sedona/raster/__init__.py
+sedona/raster/awt_raster.py
+sedona/raster/data_buffer.py
+sedona/raster/meta.py
+sedona/raster/raster_serde.py
+sedona/raster/sample_model.py
+sedona/raster/sedona_raster.py
 sedona/raster_utils/SedonaUtils.py
 sedona/raster_utils/__init__.py
 sedona/register/__init__.py
 sedona/register/geo_registrator.py
 sedona/register/java_libs.py
 sedona/spark/SedonaContext.py
 sedona/spark/__init__.py
```

### Comparing `apache_sedona-1.5.3/sedona/__init__.py` & `apache_sedona-1.6.0/sedona/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/__init__.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/circle_rdd.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/circle_rdd.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/linestring_rdd.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/linestring_rdd.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/point_rdd.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/point_rdd.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/polygon_rdd.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/polygon_rdd.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/rectangle_rdd.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/rectangle_rdd.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/spatial_rdd.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/spatial_rdd.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
             grid = GridTypeJvm(self._jvm, GridType.from_str(partitioning)).jvm_instance
         elif type(partitioning) == GridType:
             grid = GridTypeJvm(self._jvm, partitioning).jvm_instance
         elif type(partitioning) == SpatialPartitioner:
             grid = partitioning.jvm_partitioner
         elif type(partitioning) == list:
             if isinstance(partitioning[0], Envelope):
-                bytes_data = pickle.dumps(partitioning)
+                bytes_data = Envelope.serialize_for_java(partitioning)
                 jvm_envelopes = self._jvm.EnvelopeAdapter.getFromPython(bytes_data)
                 grid = jvm_envelopes
             else:
                 raise AttributeError("List should consists of Envelopes")
         else:
             raise TypeError("Grid does not have correct type")
```

### Comparing `apache_sedona-1.5.3/sedona/core/SpatialRDD/spatial_rdd_factory.py` & `apache_sedona-1.6.0/sedona/core/SpatialRDD/spatial_rdd_factory.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/__init__.py` & `apache_sedona-1.6.0/sedona/core/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/enums/__init__.py` & `apache_sedona-1.6.0/sedona/core/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/enums/file_data_splitter.py` & `apache_sedona-1.6.0/sedona/core/enums/file_data_splitter.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/enums/grid_type.py` & `apache_sedona-1.6.0/sedona/core/enums/grid_type.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/enums/index_type.py` & `apache_sedona-1.6.0/sedona/core/enums/index_type.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/enums/join_build_side.py` & `apache_sedona-1.6.0/sedona/core/enums/join_build_side.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/enums/spatial.py` & `apache_sedona-1.6.0/sedona/core/enums/spatial.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/__init__.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/disc_utils.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/disc_utils.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/geo_json_reader.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/geo_json_reader.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/geo_reader.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/geo_reader.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/shapefileParser/__init__.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/shapefileParser/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/shapefileParser/shape_file_reader.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/shapefileParser/shape_file_reader.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/wkb_reader.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/wkb_reader.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/formatMapper/wkt_reader.py` & `apache_sedona-1.6.0/sedona/core/formatMapper/wkt_reader.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/geom/__init__.py` & `apache_sedona-1.6.0/sedona/core/geom/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/geom/circle.py` & `apache_sedona-1.6.0/sedona/core/geom/shapely1/circle.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/geom/envelope.py` & `apache_sedona-1.6.0/sedona/core/geom/shapely1/envelope.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 #  under the License.
 
 from shapely.geometry import Polygon, Point
 from shapely.geometry.base import BaseGeometry
 
 from sedona.utils.decorators import require
 import math
+import pickle
 
 class Envelope(Polygon):
 
     def __init__(self, minx=0, maxx=1, miny=0, maxy=1):
         self.minx = minx
         self.maxx = maxx
         self.miny = miny
@@ -96,18 +97,19 @@
             maxx=self.maxx,
             miny=self.miny,
             maxy=self.maxy,
 
         )
 
     def __setstate__(self, state):
-        self.minx = state.get("minx", 0)
-        self.minx = state.get("maxx", 1)
-        self.minx = state.get("miny", 0)
-        self.minx = state.get("maxy", 1)
+        minx = state.get("minx", 0)
+        maxx = state.get("maxx", 1)
+        miny = state.get("miny", 0)
+        maxy = state.get("maxy", 1)
+        self.__init__(minx, maxx, miny, maxy)
 
     @property
     def __array_interface__(self):
         raise NotImplementedError()
 
     def _get_coords(self):
         raise NotImplementedError()
@@ -117,7 +119,11 @@
 
     @property
     def coords(self):
         raise NotImplementedError()
 
     def __repr__(self):
         return f"Envelope({self.minx}, {self.maxx}, {self.miny}, {self.maxy})"
+
+    @classmethod
+    def serialize_for_java(cls, envelopes):
+        return pickle.dumps(envelopes)
```

### Comparing `apache_sedona-1.5.3/sedona/core/jvm/__init__.py` & `apache_sedona-1.6.0/sedona/core/geom/shapely1/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/jvm/abstract.py` & `apache_sedona-1.6.0/sedona/core/jvm/abstract.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/jvm/config.py` & `apache_sedona-1.6.0/sedona/core/jvm/config.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/jvm/translate.py` & `apache_sedona-1.6.0/sedona/core/jvm/translate.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/__init__.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/join_params.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/join_params.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/join_query.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/join_query.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/join_query_raw.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/join_query_raw.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/knn_query.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/knn_query.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/range_query.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/range_query.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/range_query_raw.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/range_query_raw.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/spatialOperator/rdd.py` & `apache_sedona-1.6.0/sedona/core/spatialOperator/rdd.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/core/utils.py` & `apache_sedona-1.6.0/sedona/core/utils.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/exceptions.py` & `apache_sedona-1.6.0/sedona/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/maps/SedonaKepler.py` & `apache_sedona-1.6.0/sedona/maps/SedonaKepler.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/maps/SedonaMapUtils.py` & `apache_sedona-1.6.0/sedona/maps/SedonaMapUtils.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/maps/SedonaPyDeck.py` & `apache_sedona-1.6.0/sedona/maps/SedonaPyDeck.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/maps/__init__.py` & `apache_sedona-1.6.0/sedona/core/geom/shapely2/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/raster_utils/SedonaUtils.py` & `apache_sedona-1.6.0/sedona/raster_utils/SedonaUtils.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/raster_utils/__init__.py` & `apache_sedona-1.6.0/sedona/core/jvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/register/__init__.py` & `apache_sedona-1.6.0/sedona/register/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/register/geo_registrator.py` & `apache_sedona-1.6.0/sedona/register/geo_registrator.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/register/java_libs.py` & `apache_sedona-1.6.0/sedona/register/java_libs.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/spark/SedonaContext.py` & `apache_sedona-1.6.0/sedona/spark/SedonaContext.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/spark/__init__.py` & `apache_sedona-1.6.0/sedona/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/sql/__init__.py` & `apache_sedona-1.6.0/sedona/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/sql/dataframe_api.py` & `apache_sedona-1.6.0/sedona/sql/dataframe_api.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/sql/exceptions.py` & `apache_sedona-1.6.0/sedona/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/sql/st_aggregates.py` & `apache_sedona-1.6.0/sedona/sql/st_aggregates.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/sql/st_constructors.py` & `apache_sedona-1.6.0/sedona/sql/st_constructors.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/sql/st_functions.py` & `apache_sedona-1.6.0/sedona/sql/st_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,41 +197,65 @@
     :return: Azimuth for point_a and point_b in radians as a double column.
     :rtype: Column
     """
     return _call_st_function("ST_Azimuth", (point_a, point_b))
 
 
 @validate_argument_types
+def ST_BestSRID(geometry: ColumnOrName) -> Column:
+    """Estimates the best SRID (EPSG code) of the geometry.
+
+    :param geometry: Geometry column to calculate the boundary for.
+    :type geometry: ColumnOrName
+    :return: SRID as an Integer
+    :rtype: Column
+    """
+    return _call_st_function("ST_BestSRID", geometry)
+
+@validate_argument_types
+def ST_ShiftLongitude(geometry: ColumnOrName) -> Column:
+    """Shifts longitudes between -180..0 degrees to 180..360 degrees and vice versa.
+
+    :param geometry: Geometry column.
+    :type geometry: ColumnOrName
+    :return: Shifted geometry
+    :rtype: Column
+    """
+    return _call_st_function("ST_ShiftLongitude", geometry)
+
+@validate_argument_types
 def ST_Boundary(geometry: ColumnOrName) -> Column:
     """Calculate the closure of the combinatorial boundary of a geometry column.
 
     :param geometry: Geometry column to calculate the boundary for.
     :type geometry: ColumnOrName
     :return: Boundary of the input geometry as a geometry column.
     :rtype: Column
     """
     return _call_st_function("ST_Boundary", geometry)
 
 
 @validate_argument_types
-def ST_Buffer(geometry: ColumnOrName, buffer: ColumnOrNameOrNumber, parameters: Optional[Union[ColumnOrName, str]] = None) -> Column:
+def ST_Buffer(geometry: ColumnOrName, buffer: ColumnOrNameOrNumber, useSpheroid: Optional[Union[ColumnOrName, bool]] = None, parameters: Optional[Union[ColumnOrName, str]] = None) -> Column:
     """Calculate a geometry that represents all points whose distance from the
     input geometry column is equal to or less than a given amount.
 
     :param geometry: Input geometry column to buffer.
     :type geometry: ColumnOrName
     :param buffer: Either a column or value for the amount to buffer the input geometry by.
     :type buffer: ColumnOrNameOrNumber
     :return: Buffered geometry as a geometry column.
     :rtype: Column
     """
-    if parameters is None:
+    if parameters is None and useSpheroid is None:
         args = (geometry, buffer)
+    elif parameters is None:
+        args = (geometry, buffer, useSpheroid)
     else:
-        args = (geometry, buffer, parameters)
+        args = (geometry, buffer, useSpheroid, parameters)
 
     return _call_st_function("ST_Buffer", args)
 
 
 @validate_argument_types
 def ST_BuildArea(geometry: ColumnOrName) -> Column:
     """Generate a geometry described by the constituent linework of the input
@@ -327,14 +351,25 @@
     :type geometry: ColumnOrName
     :return: Convex hull of geometry as a geometry column.
     :rtype: Column
     """
     return _call_st_function("ST_ConvexHull", geometry)
 
 @validate_argument_types
+def ST_CrossesDateLine(a: ColumnOrName) -> Column:
+    """Check whether geometry a crosses the International Date Line.
+
+    :param a: Geometry to check crossing with.
+    :type a: ColumnOrName
+    :return: True if geometry a cross the dateline.
+    :rtype: Column
+    """
+    return _call_st_function("ST_CrossesDateLine", (a))
+
+@validate_argument_types
 def ST_Dimension(geometry: ColumnOrName):
     """Calculate the inherent dimension of a geometry column.
 
     :param geometry: Geometry column to calculate the dimension for.
     :type geometry: ColumnOrName
     :return: Dimension of geometry as an integer column.
     :rtype: Column
@@ -662,14 +697,27 @@
     :return: True if the geometry is empty and False otherwise as a boolean column.
     :rtype: Column
     """
     return _call_st_function("ST_IsEmpty", geometry)
 
 
 @validate_argument_types
+def ST_IsPolygonCW(geometry: ColumnOrName) -> Column:
+    """Check if the Polygon or MultiPolygon use a clockwise orientation for exterior ring and counter-clockwise
+    orientation for interior ring.
+
+    :param geometry: Geometry column to check.
+    :type geometry: ColumnOrName
+    :return: True if the geometry is empty and False otherwise as a boolean column.
+    :rtype: Column
+    """
+    return _call_st_function("ST_IsPolygonCW", geometry)
+
+
+@validate_argument_types
 def ST_IsRing(line_string: ColumnOrName) -> Column:
     """Check if a linestring geometry is both closed and simple.
 
     :param line_string: Linestring geometry column to check.
     :type line_string: ColumnOrName
     :return: True if the linestring is both closed and simple and False otherwise as a boolean column.
     :rtype: Column
@@ -834,14 +882,25 @@
     :type srid: ColumnOrNameOrNumber
     :return: Polygon geometry column created from the input linestring.
     :rtype: Column
     """
     return _call_st_function("ST_Polygon", (line_string, srid))
 
 @validate_argument_types
+def ST_Polygonize(geometry: ColumnOrName) -> Column:
+    """Generates a GeometryCollection composed of polygons that are formed from the linework of a set of input geometries.
+
+    :param geometry: input geometry of type GeometryCollection
+    :type geometry: ColumnOrName
+    :return: GeometryCollection geometry column created from the input geometry.
+    :rtype: Column
+    """
+    return _call_st_function("ST_Polygonize", (geometry))
+
+@validate_argument_types
 def ST_MakePolygon(line_string: ColumnOrName, holes: Optional[ColumnOrName] = None) -> Column:
     """Create a polygon geometry from a linestring describing the exterior ring as well as an array of linestrings describing holes.
 
     :param line_string: Closed linestring geometry column that describes the exterior ring of the polygon.
     :type line_string: ColumnOrName
     :param holes: Optional column for an array of closed geometry columns that describe holes in the polygon, defaults to None.
     :type holes: Optional[ColumnOrName], optional
@@ -1043,14 +1102,26 @@
     :rtype: List[long]
     """
     args = (geometry, level)
     return _call_st_function("ST_S2CellIDs", args)
 
 
 @validate_argument_types
+def ST_S2ToGeom(cells: Union[ColumnOrName, list]) -> Column:
+    """Create a polygon from the S2 cells
+
+    :param cells: S2 cells
+    :type cells: List[long]
+    :return: the Polygon for all S2 cells
+    :rtype: Geometry
+    """
+    return _call_st_function("ST_S2ToGeom", cells)
+
+
+@validate_argument_types
 def ST_SetPoint(line_string: ColumnOrName, index: Union[ColumnOrName, int], point: ColumnOrName) -> Column:
     """Replace a point in a linestring.
 
     :param line_string: Linestring geometry column which contains the point to be replaced.
     :type line_string: ColumnOrName
     :param index: Index for the point to be replaced, 0-based, negative values start from the end so -1 is the last point.
     :type index: Union[ColumnOrName, int]
@@ -1071,14 +1142,47 @@
     :param srid: SRID to set as either an integer or an integer column.
     :type srid: Union[ColumnOrName, int]
     :return: Geometry column with SRID set to srid.
     :rtype: Column
     """
     return _call_st_function("ST_SetSRID", (geometry, srid))
 
+@validate_argument_types
+def ST_Snap(input: ColumnOrName, reference: ColumnOrName, tolerance: Union[ColumnOrName, float]) -> Column:
+    """Snaps input Geometry to reference Geometry controlled by distance tolerance.
+
+    :param input: Geometry
+    :param reference: Geometry to snap to
+    :param tolerance: Distance to control snapping
+    :return: Snapped Geometry
+    """
+    return _call_st_function("ST_Snap", (input, reference, tolerance))
+
+
+@validate_argument_types
+def ST_IsPolygonCCW(geometry: ColumnOrName) -> Column:
+    """Check if the Polygon or MultiPolygon use a counter-clockwise orientation for exterior ring and clockwise
+    orientation for interior ring.
+    :param geometry: Geometry column to check.
+    :type geometry: ColumnOrName
+    :return: True if the geometry is empty and False otherwise as a boolean column.
+    :rtype: Column
+    """
+    return _call_st_function("ST_IsPolygonCCW", geometry)
+
+
+@validate_argument_types
+def ST_ForcePolygonCCW(geometry: ColumnOrName) -> Column:
+    """
+    Returns a geometry with counter-clockwise oriented exterior ring and clockwise oriented interior rings
+    :param geometry: Geometry column to change orientation
+    :return: counter-clockwise oriented geometry
+    """
+    return _call_st_function("ST_ForcePolygonCCW", geometry)
+
 
 @validate_argument_types
 def ST_SRID(geometry: ColumnOrName) -> Column:
     """Get the SRID of geometry.
 
     :param geometry: Geometry column to get SRID from.
     :type geometry: ColumnOrName
@@ -1197,25 +1301,31 @@
             args = (geometry, source_crs)
     else:
         args = (geometry, source_crs, target_crs, disable_error)
     return _call_st_function("ST_Transform", args)
 
 
 @validate_argument_types
-def ST_Union(a: ColumnOrName, b: ColumnOrName) -> Column:
+def ST_Union(a: ColumnOrName, b: Optional[ColumnOrName] = None) -> Column:
     """Calculate the union of two geometries.
 
     :param a: One geometry column to use.
     :type a: ColumnOrName
     :param b: Other geometry column to use.
     :type b: ColumnOrName
     :return: Geometry representing the union of a and b as a geometry column.
     :rtype: Column
     """
-    return _call_st_function("ST_Union", (a, b))
+
+    if b is None:
+        args = a
+    else:
+        args = (a, b)
+
+    return _call_st_function("ST_Union", args)
 
 
 @validate_argument_types
 def ST_X(point: ColumnOrName) -> Column:
     """Return the X coordinate of a point geometry.
 
     :param point: Point geometry column to get the coordinate for.
@@ -1336,14 +1446,23 @@
     :param geometry: Geometry column to make 3D
     :return: 3D geometry with either already present z coordinate if any, or zcoordinate with given zValue
     """
     args = (geometry, zValue)
     return _call_st_function("ST_Force3D", args)
 
 @validate_argument_types
+def ST_ForcePolygonCW(geometry: ColumnOrName) -> Column:
+    """
+    Returns
+    :param geometry: Geometry column to change orientation
+    :return: Clockwise oriented geometry
+    """
+    return _call_st_function("ST_ForcePolygonCW", geometry)
+
+@validate_argument_types
 def ST_NRings(geometry: ColumnOrName) -> Column:
     """
     Returns the total number of rings in a Polygon or MultiPolygon. Compared to ST_NumInteriorRings, ST_NRings takes exterior rings into account as well.
     :param geometry: Geometry column to calculate rings for
     :return: Number of exterior rings + interior rings (if any) for the given Polygon or MultiPolygon
     """
     return _call_st_function("ST_NRings", geometry)
```

### Comparing `apache_sedona-1.5.3/sedona/sql/st_predicates.py` & `apache_sedona-1.6.0/sedona/sql/st_predicates.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #  under the License.
 import inspect
 import sys
 
 from functools import partial
 
 from pyspark.sql import Column
-from typing import Union
+from typing import Union, Optional
 
 from sedona.sql.dataframe_api import ColumnOrName, call_sedona_function, validate_argument_types
 
 
 # Automatically populate __all__
 __all__ = [name for name, obj in inspect.getmembers(sys.modules[__name__])
            if inspect.isfunction(obj)]
@@ -56,15 +56,14 @@
     :param b: Geometry to check crossing of.
     :type b: ColumnOrName
     :return: True if geometry a cross geometry b and False otherwise as a boolean column.
     :rtype: Column
     """
     return _call_predicate_function("ST_Crosses", (a, b))
 
-
 @validate_argument_types
 def ST_Disjoint(a: ColumnOrName, b: ColumnOrName) -> Column:
     """Check whether two geometries are disjoint.
 
     :param a: One geometry column to check.
     :type a: ColumnOrName
     :param b: Other geometry column to check.
@@ -183,17 +182,18 @@
     :type b: ColumnOrName
     :return: True if a is covered by b and False otherwise, as a boolean column.
     :rtype: Column
     """
     return _call_predicate_function("ST_CoveredBy", (a, b))
 
 @validate_argument_types
-def ST_DWithin(a: ColumnOrName, b: ColumnOrName, distance: Union[ColumnOrName, float]):
+def ST_DWithin(a: ColumnOrName, b: ColumnOrName, distance: Union[ColumnOrName, float], use_sphere: Optional[Union[ColumnOrName, bool]] = None):
     """
     Check if geometry a is within 'distance' units of geometry b
     :param a: Geometry column to check
     :param b: Geometry column to check
     :param distance: distance units to check the within predicate
+    :param use_sphere: whether to use spheroid distance or euclidean distance
     :return: True if a is within distance units of Geometry b
     """
-
-    return _call_predicate_function("ST_DWithin", (a, b, distance))
+    args = (a, b, distance, use_sphere) if use_sphere is not None else (a, b, distance,)
+    return _call_predicate_function("ST_DWithin", args)
```

### Comparing `apache_sedona-1.5.3/sedona/sql/types.py` & `apache_sedona-1.6.0/sedona/sql/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 from pyspark.sql.types import UserDefinedType, BinaryType
 
 from ..utils import geometry_serde
+from ..raster import raster_serde
+from ..raster.sedona_raster import SedonaRaster
 
 
 class GeometryType(UserDefinedType):
 
     @classmethod
     def sqlType(cls):
         return BinaryType()
@@ -51,19 +53,22 @@
     def sqlType(cls):
         return BinaryType()
 
     def serialize(self, obj):
         raise NotImplementedError("RasterType.serialize is not implemented yet")
 
     def deserialize(self, datum):
-        raise NotImplementedError("RasterType.deserialize is not implemented yet")
+        return raster_serde.deserialize(datum)
 
     @classmethod
     def module(cls):
         return "sedona.sql.types"
 
     def needConversion(self):
         return True
 
     @classmethod
     def scalaUDT(cls):
         return "org.apache.spark.sql.sedona_sql.UDT.RasterUDT"
+
+
+SedonaRaster.__UDT__ = RasterType()
```

### Comparing `apache_sedona-1.5.3/sedona/utils/__init__.py` & `apache_sedona-1.6.0/sedona/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/abstract_parser.py` & `apache_sedona-1.6.0/sedona/utils/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/adapter.py` & `apache_sedona-1.6.0/sedona/utils/adapter.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/binary_parser.py` & `apache_sedona-1.6.0/sedona/utils/binary_parser.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/decorators.py` & `apache_sedona-1.6.0/sedona/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/geometry_adapter.py` & `apache_sedona-1.6.0/sedona/utils/geometry_adapter.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/geometry_serde.py` & `apache_sedona-1.6.0/sedona/utils/geometry_serde.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/geometry_serde_general.py` & `apache_sedona-1.6.0/sedona/utils/geometry_serde_general.py`

 * *Files 0% similar despite different names*

```diff
@@ -375,19 +375,19 @@
 
 
 def serialize_multi_linestring(geom: MultiLineString) -> bytes:
     linestrings = list(geom.geoms)
 
     coord_type = CoordinateType.type_of(geom)
     lines = [[list(coord) for coord in ls.coords] for ls in linestrings]
-    line_lengths = [len(l) for l in lines]
+    line_lengths = [len(line) for line in lines]
     num_coords = sum(line_lengths)
 
     header = generate_header_bytes(GeometryTypeID.MULTILINESTRING, coord_type, num_coords)
-    coord_data = array.array('d', [c for l in lines for coord in l for c in coord]).tobytes()
+    coord_data = array.array('d', [c for line in lines for coord in line for c in coord]).tobytes()
     num_lines = struct.pack('i', len(lines))
     structure_data = array.array('i', line_lengths).tobytes()
 
     result = header + coord_data + num_lines + structure_data
 
     return result
```

### Comparing `apache_sedona-1.5.3/sedona/utils/jvm.py` & `apache_sedona-1.6.0/sedona/utils/jvm.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/meta.py` & `apache_sedona-1.6.0/sedona/utils/meta.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/prep.py` & `apache_sedona-1.6.0/sedona/utils/prep.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/serde.py` & `apache_sedona-1.6.0/sedona/utils/serde.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/spatial_rdd_parser.py` & `apache_sedona-1.6.0/sedona/utils/spatial_rdd_parser.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/utils/types.py` & `apache_sedona-1.6.0/sedona/utils/types.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/sedona/version.py` & `apache_sedona-1.6.0/sedona/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  Unless required by applicable law or agreed to in writing,
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
-version = "1.5.3"
+version = "1.6.0"
```

### Comparing `apache_sedona-1.5.3/setup.py` & `apache_sedona-1.6.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,20 +48,20 @@
     author='Apache Sedona',
     author_email='dev@sedona.apache.org',
     packages=find_packages(exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
     ext_modules=ext_modules,
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
-    install_requires=['attrs', "shapely>=1.7.0"],
+    install_requires=['attrs', "shapely>=1.7.0", "rasterio>=1.2.10"],
     extras_require={
         "spark": ["pyspark>=2.3.0"],
-        "pydeck-map": ["pandas<=1.3.5", "geopandas<=0.10.2", "pydeck==0.8.0"],
-        "kepler-map": ["pandas<=1.3.5", "geopandas<=0.10.2", "keplergl==0.3.2"],
-        "all": ["pyspark>=2.3.0", "pandas<=1.3.5", "geopandas<=0.10.2","pydeck==0.8.0", "keplergl==0.3.2"],
+        "pydeck-map": ["geopandas", "pydeck==0.8.0"],
+        "kepler-map": ["geopandas", "keplergl==0.3.2"],
+        "all": ["pyspark>=2.3.0", "geopandas","pydeck==0.8.0", "keplergl==0.3.2"],
     },
     project_urls={
         'Documentation': 'https://sedona.apache.org',
         'Source code': 'https://github.com/apache/sedona',
         'Bug Reports': 'https://issues.apache.org/jira/projects/SEDONA'
     },
     classifiers=[
```

### Comparing `apache_sedona-1.5.3/src/geom_buf.c` & `apache_sedona-1.6.0/src/geom_buf.c`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/geom_buf.h` & `apache_sedona-1.6.0/src/geom_buf.h`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/geomserde.c` & `apache_sedona-1.6.0/src/geomserde.c`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/geomserde.h` & `apache_sedona-1.6.0/src/geomserde.h`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/geomserde_speedup_module.c` & `apache_sedona-1.6.0/src/geomserde_speedup_module.c`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/geos_c_dyn.c` & `apache_sedona-1.6.0/src/geos_c_dyn.c`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/geos_c_dyn.h` & `apache_sedona-1.6.0/src/geos_c_dyn.h`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/geos_c_dyn_funcs.h` & `apache_sedona-1.6.0/src/geos_c_dyn_funcs.h`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/src/pygeos/c_api.h` & `apache_sedona-1.6.0/src/pygeos/c_api.h`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/tests/test_assign_raw_spatial_rdd.py` & `apache_sedona-1.6.0/tests/test_assign_raw_spatial_rdd.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/tests/test_base.py` & `apache_sedona-1.6.0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/tests/test_circle.py` & `apache_sedona-1.6.0/tests/test_circle.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,33 +12,36 @@
 #  software distributed under the License is distributed on an
 #  "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 #  KIND, either express or implied.  See the License for the
 #  specific language governing permissions and limitations
 #  under the License.
 
 import pytest
+
+import shapely
 from shapely import wkt
 from shapely.geometry import Point
 
 from sedona.core.geom.circle import Circle
 from sedona.core.geom.envelope import Envelope
 
 
 class TestCircle:
 
     def test_get_center(self):
         point = Point(0.0, 0.0)
         circle = Circle(point, 0.1)
-        assert circle.centerGeometry.x == point.x and circle.centerGeometry.y == point.y
+        assert circle.centerGeometry.x == pytest.approx(point.x, 1e-6) and circle.centerGeometry.y == pytest.approx(point.y, 1e-6)
 
     def test_get_radius(self):
         point = Point(0.0, 0.0)
         circle = Circle(point, 0.1)
         assert circle.getRadius() == pytest.approx(0.1, 0.01)
 
+    @pytest.mark.skipif(shapely.__version__.startswith('2.'), reason="Circle is immutable when working with Shapely 2.0")
     def test_set_radius(self):
         point = Point(0.0, 0.0)
         circle = Circle(point, 0.1)
         circle.setRadius(0.1)
         assert circle.getRadius() == pytest.approx(0.1, 0.01)
 
     def test_get_envelope_internal(self):
```

### Comparing `apache_sedona-1.5.3/tests/test_multiple_meta.py` & `apache_sedona-1.6.0/tests/test_multiple_meta.py`

 * *Files identical despite different names*

### Comparing `apache_sedona-1.5.3/tests/test_scala_example.py` & `apache_sedona-1.6.0/tests/test_scala_example.py`

 * *Files identical despite different names*

