# Comparing `tmp/REHO-1.0.2.tar.gz` & `tmp/reho-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REHO-1.0.2.tar", last modified: Wed Mar  6 08:55:09 2024, max compression
+gzip compressed data, was "reho-1.1.0.tar", last modified: Fri May 17 10:41:17 2024, max compression
```

## Comparing `REHO-1.0.2.tar` & `reho-1.1.0.tar`

### file list

```diff
@@ -1,125 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.251871 REHO-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-03-06 08:55:00.000000 REHO-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-06 08:55:00.000000 REHO-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-03-06 08:55:09.251871 REHO-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-06 08:55:00.000000 REHO-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.251871 REHO-1.0.2/REHO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-03-06 08:55:09.000000 REHO-1.0.2/REHO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-03-06 08:55:09.000000 REHO-1.0.2/REHO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 08:55:09.000000 REHO-1.0.2/REHO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-06 08:55:09.000000 REHO-1.0.2/REHO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-06 08:55:09.000000 REHO-1.0.2/REHO.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.219871 REHO-1.0.2/reho/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.215871 REHO-1.0.2/reho/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.219871 REHO-1.0.2/reho/data/QBuildings/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/QBuildings/Geneva.ini
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/QBuildings/Suisse.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.219871 REHO-1.0.2/reho/data/SIA/
--rw-r--r--   0 runner    (1001) docker     (127)   193707 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/SIA/sia2024_data.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/SIA/sia2024_rooms_sia380_1.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.219871 REHO-1.0.2/reho/data/elcom/
--rw-r--r--   0 runner    (1001) docker     (127)   179021 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/elcom/correspondance_table_municipality_operator.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.219871 REHO-1.0.2/reho/data/emissions/
--rw-r--r--   0 runner    (1001) docker     (127)  2099691 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/emissions/electricity_matrix_2019_reduced.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.223872 REHO-1.0.2/reho/data/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/infrastructure/AC_parameters.txt
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/infrastructure/HP_parameters.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/infrastructure/building_units.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/infrastructure/district_units.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/infrastructure/grids.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/infrastructure/storage_units.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.235871 REHO-1.0.2/reho/data/skydome/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/skydome/skyPatchesAreas.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/skydome/skyPatchesCenPts.txt
--rw-r--r--   0 runner    (1001) docker     (127)  7291033 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/skydome/total_irradiation.csv
--rw-r--r--   0 runner    (1001) docker     (127)   284250 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/skydome/typical_irradiation.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.235871 REHO-1.0.2/reho/data/weather/
--rw-r--r--   0 runner    (1001) docker     (127)    60210 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/weather/Weekday_2005.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.239872 REHO-1.0.2/reho/data/weather/hour/
--rwxr-xr-x   0 runner    (1001) docker     (127)   279325 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/weather/hour/Disentis-hour.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)   278555 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/weather/hour/Geneva-hour.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)   279681 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/weather/hour/Lugano-hour.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)   277148 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/weather/hour/Luzern-hour.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)   278755 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/weather/hour/Piotta-hour.dat
--rwxr-xr-x   0 runner    (1001) docker     (127)   277172 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/data/weather/hour/Zuerich-Kloten-hour.dat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.239872 REHO-1.0.2/reho/model/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.239872 REHO-1.0.2/reho/model/ampl_model/
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/data_stream.dat
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/data_stream_storage.dat
--rw-r--r--   0 runner    (1001) docker     (127)    21144 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/master_problem.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/master_problem_actors.mod
--rw-r--r--   0 runner    (1001) docker     (127)    35544 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/model.mod
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/scenario.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.243872 REHO-1.0.2/reho/model/ampl_model/units/
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/DHN.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/DHN_HEX.mod
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/DHN_pipes.mod
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/air_conditioner.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/data_heat.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.243872 REHO-1.0.2/reho/model/ampl_model/units/district_units/
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/district_units/evehicle.mod
--rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/district_units/heatpump_district.mod
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/district_units/heatstorage_district.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/district_units/ng_boiler_district.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/district_units/ng_cogeneration_district.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/electrical_heater.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.243872 REHO-1.0.2/reho/model/ampl_model/units/h2_units/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/h2_units/SOEFC.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/h2_units/electrolyser.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/h2_units/fuel_cell.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/h2_units/methanizer.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/heat_curtailment.mod
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/heatpump.mod
--rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/heatpump_anergy.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/ng_boiler.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/ng_cogeneration.mod
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/ng_cogeneration_partload.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/oil_boiler.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/pv.mod
--rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/pv_orientation.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.247871 REHO-1.0.2/reho/model/ampl_model/units/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/CH4_tank.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/LHS_storage.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/PTES_aggregated.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/PTES_split.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/battery.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/battery_interperiod.mod
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/dhwstorage.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/h2_storage.mod
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/heatstorage.mod
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/storage/heatstorage_interperiod.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/thermal_solar.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/ampl_model/units/wood_stove.mod
--rw-r--r--   0 runner    (1001) docker     (127)    37608 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/compact_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    58620 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/district_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)    25161 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/infrastructure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.247871 REHO-1.0.2/reho/model/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)    32706 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/postprocessing/KPIs.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/postprocessing/building_scale_network_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/postprocessing/write_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.251871 REHO-1.0.2/reho/model/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/EV_profile_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    31012 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/QBuildings.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/data_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35365 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/electricity_prices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/emissions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/sia_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14502 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/skydome.py
--rw-r--r--   0 runner    (1001) docker     (127)    20331 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/preprocessing/weather.py
--rw-r--r--   0 runner    (1001) docker     (127)    47602 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/model/reho.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 08:55:09.251871 REHO-1.0.2/reho/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/plotting/layout.csv
--rw-r--r--   0 runner    (1001) docker     (127)    77919 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/plotting/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)    15103 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/plotting/rainbow_plots.py
--rw-r--r--   0 runner    (1001) docker     (127)    13601 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/plotting/sankey.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/plotting/sia380_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-03-06 08:55:00.000000 REHO-1.0.2/reho/plotting/yearly_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 08:55:09.251871 REHO-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-06 08:55:00.000000 REHO-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.769704 reho-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11339 2024-05-17 10:41:12.000000 reho-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-17 10:41:12.000000 reho-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-17 10:41:17.769704 reho-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-17 10:41:12.000000 reho-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.769704 reho-1.1.0/REHO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-17 10:41:17.000000 reho-1.1.0/REHO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-17 10:41:17.000000 reho-1.1.0/REHO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:41:17.000000 reho-1.1.0/REHO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-17 10:41:17.000000 reho-1.1.0/REHO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 10:41:17.000000 reho-1.1.0/REHO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.741704 reho-1.1.0/reho/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-17 10:41:12.000000 reho-1.1.0/reho/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.741704 reho-1.1.0/reho/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.741704 reho-1.1.0/reho/data/QBuildings/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/QBuildings/Geneva.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/QBuildings/Suisse.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.745704 reho-1.1.0/reho/data/SIA/
+-rw-r--r--   0 runner    (1001) docker     (127)   193707 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/SIA/sia2024_data.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/SIA/sia2024_rooms_sia380_1.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.745704 reho-1.1.0/reho/data/elcom/
+-rw-r--r--   0 runner    (1001) docker     (127)   179021 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/elcom/correspondance_table_municipality_operator.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.745704 reho-1.1.0/reho/data/emissions/
+-rw-r--r--   0 runner    (1001) docker     (127)  2099691 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/emissions/electricity_matrix_2019_reduced.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.749704 reho-1.1.0/reho/data/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/infrastructure/AC_parameters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/infrastructure/HP_parameters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/infrastructure/building_units.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/infrastructure/district_units.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/infrastructure/grids.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/infrastructure/storage_units.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.757704 reho-1.1.0/reho/data/skydome/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/skydome/skyPatchesAreas.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/skydome/skyPatchesCenPts.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  7291033 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/skydome/total_irradiation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   284250 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/skydome/typical_irradiation.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.757704 reho-1.1.0/reho/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)    60210 2024-05-17 10:41:12.000000 reho-1.1.0/reho/data/weather/weekday.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.757704 reho-1.1.0/reho/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.761704 reho-1.1.0/reho/model/ampl_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/actors_problem.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/data_stream.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/data_stream_storage.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    21150 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/master_problem.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/scenario.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    35544 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/sub_problem.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.761704 reho-1.1.0/reho/model/ampl_model/units/
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/DHN.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/DHN_HEX.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/DHN_pipes.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/air_conditioner.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/data_heat.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.765704 reho-1.1.0/reho/model/ampl_model/units/district_units/
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/district_units/evehicle.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/district_units/heatpump_district.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/district_units/heatstorage_district.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/district_units/ng_boiler_district.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/district_units/ng_cogeneration_district.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/electrical_heater.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.765704 reho-1.1.0/reho/model/ampl_model/units/h2_units/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/h2_units/SOEFC.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/h2_units/electrolyser.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/h2_units/fuel_cell.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/h2_units/methanizer.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/heat_curtailment.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/heatpump.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/heatpump_anergy.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/ng_boiler.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/ng_cogeneration.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/ng_cogeneration_partload.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/oil_boiler.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/pv.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    11604 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/pv_orientation.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.765704 reho-1.1.0/reho/model/ampl_model/units/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/CH4_tank.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/LHS_storage.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/PTES_aggregated.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/PTES_split.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/battery.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/battery_interperiod.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/dhwstorage.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/h2_storage.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/heatstorage.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/storage/heatstorage_interperiod.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/thermal_solar.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/ampl_model/units/wood_stove.mod
+-rw-r--r--   0 runner    (1001) docker     (127)    25123 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60493 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/master_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.765704 reho-1.1.0/reho/model/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)    34531 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/postprocessing/KPIs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/postprocessing/building_scale_network_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/postprocessing/sensitivity_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28428 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/postprocessing/write_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.769704 reho-1.1.0/reho/model/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/EV_profile_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30835 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/QBuildings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14086 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/buildings_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12840 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35309 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/electricity_prices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/emissions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/local_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5162 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/sia_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13996 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/skydome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21488 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/preprocessing/weather.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40668 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/reho.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36355 2024-05-17 10:41:12.000000 reho-1.1.0/reho/model/sub_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-17 10:41:12.000000 reho-1.1.0/reho/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:41:17.769704 reho-1.1.0/reho/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 10:41:12.000000 reho-1.1.0/reho/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-17 10:41:12.000000 reho-1.1.0/reho/plotting/layout.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    83757 2024-05-17 10:41:12.000000 reho-1.1.0/reho/plotting/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-17 10:41:12.000000 reho-1.1.0/reho/plotting/rainbow_plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-05-17 10:41:12.000000 reho-1.1.0/reho/plotting/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-17 10:41:12.000000 reho-1.1.0/reho/plotting/sia380_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2024-05-17 10:41:12.000000 reho-1.1.0/reho/plotting/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:41:17.769704 reho-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-05-17 10:41:12.000000 reho-1.1.0/setup.py
```

### Comparing `REHO-1.0.2/LICENSE` & `reho-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/PKG-INFO` & `reho-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REHO
-Version: 1.0.2
+Version: 1.1.0
 Summary: Renewable Energy Hub Optimizer (REHO) - A Comprehensive Decision Support Tool for Sustainable Energy System Planning
 Home-page: https://github.com/IPESE/REHO
 Author: Dorsan Lepour
 Author-email: dorsan.lepour@epfl.ch
 Maintainer: IT team of IPESE Laboratory from EPFL
 Maintainer-email: joao.ferreiradasilva@epfl.ch
 Project-URL: Documentation, https://reho.readthedocs.io/en/main/
@@ -29,14 +29,18 @@
 Requires-Dist: sqlalchemy<2.0.0,>=1.4.42
 Requires-Dist: geopandas<1.0.0,>=0.12.2
 Requires-Dist: matplotlib<4.0.0,>=3.6.1
 Requires-Dist: plotly<6.0.0,>=5.10
 Requires-Dist: kaleido<1.0.0,>=0.2.1
 Requires-Dist: python-dotenv>=1.0
 Requires-Dist: requests<3.0.0,>=2.0.0
+Requires-Dist: coloredlogs>=15.0.1
+Requires-Dist: SALib>=1.4.8
+Requires-Dist: qmcpy>=1.4.5
+Requires-Dist: pvlib==0.10.*
 
 # REHO
 Renewable Energy Hub Optimizer (REHO) is a decision support tool for sustainable urban energy system planning.
 REHO simultaneously addresses the optimal design and operation of capacities, catering to multi-objective considerations
 across economic, environmental, and efficiency criteria.
 
 Key features:
@@ -49,35 +53,40 @@
 
 For more information about the model foundations and features, please refer to the [REHO documentation](https://reho.readthedocs.io/en/main/).
 
 ## Authors
 REHO is developed by EPFL (Switzerland), within the Industrial Process and Energy Systems Engineering (IPESE) group.
 
 Dorsan Lepour <dorsan.lepour@epfl.ch>  
-Cédric Terrier <cedric.terrier@epfl.ch>  
-Joseph Loustau <joseph.loustau@epfl.ch>
+Cédric Terrier <cedric.terrier@epfl.ch>
 
 ## Licence
 Copyright (C) <2021-2024> <Ecole Polytechnique Fédérale de Lausanne (EPFL), Switzerland>
 
-Licensed under the Apache License, Version0 (the "License");
+Licensed under the Apache License, (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Description and complete License: see LICENSE file.
 
 ## Installation
-1. Clone repository available at https://github.com/IPESE/REHO
-2. Create `venv` in the repository and install required libraries with
+
+REHO is available as a [PyPI package](https://pypi.org/project/REHO/) and can be installed via pip with:
+```
+pip install --extra-index-url https://pypi.ampl.com REHO
 ```
-pip install -r requirements.txt
+
+Full code can be accessed from the [REHO GitHub repository](https://github.com/IPESE/REHO) and cloned with:
 ```
-3. Please refer to "User guide" section of the documentation for step-by-step guidelines.
+git clone https://github.com/IPESE/REHO.git
+```
+
+Please refer to "[Getting started](https://reho.readthedocs.io/en/main/sections/5_Getting_started.html)" section of the documentation  for step-by-step guidelines.
 
 ## Suggestions and contributions
 All suggestions or implementation must be tracked with dedicated issues and reported in the project repository.
```

### Comparing `REHO-1.0.2/README.md` & `reho-1.1.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,35 +13,40 @@
 
 For more information about the model foundations and features, please refer to the [REHO documentation](https://reho.readthedocs.io/en/main/).
 
 ## Authors
 REHO is developed by EPFL (Switzerland), within the Industrial Process and Energy Systems Engineering (IPESE) group.
 
 Dorsan Lepour <dorsan.lepour@epfl.ch>  
-Cédric Terrier <cedric.terrier@epfl.ch>  
-Joseph Loustau <joseph.loustau@epfl.ch>
+Cédric Terrier <cedric.terrier@epfl.ch>
 
 ## Licence
 Copyright (C) <2021-2024> <Ecole Polytechnique Fédérale de Lausanne (EPFL), Switzerland>
 
-Licensed under the Apache License, Version0 (the "License");
+Licensed under the Apache License, (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Description and complete License: see LICENSE file.
 
 ## Installation
-1. Clone repository available at https://github.com/IPESE/REHO
-2. Create `venv` in the repository and install required libraries with
+
+REHO is available as a [PyPI package](https://pypi.org/project/REHO/) and can be installed via pip with:
+```
+pip install --extra-index-url https://pypi.ampl.com REHO
 ```
-pip install -r requirements.txt
+
+Full code can be accessed from the [REHO GitHub repository](https://github.com/IPESE/REHO) and cloned with:
 ```
-3. Please refer to "User guide" section of the documentation for step-by-step guidelines.
+git clone https://github.com/IPESE/REHO.git
+```
+
+Please refer to "[Getting started](https://reho.readthedocs.io/en/main/sections/5_Getting_started.html)" section of the documentation  for step-by-step guidelines.
 
 ## Suggestions and contributions
 All suggestions or implementation must be tracked with dedicated issues and reported in the project repository.
```

### Comparing `REHO-1.0.2/REHO.egg-info/PKG-INFO` & `reho-1.1.0/REHO.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REHO
-Version: 1.0.2
+Version: 1.1.0
 Summary: Renewable Energy Hub Optimizer (REHO) - A Comprehensive Decision Support Tool for Sustainable Energy System Planning
 Home-page: https://github.com/IPESE/REHO
 Author: Dorsan Lepour
 Author-email: dorsan.lepour@epfl.ch
 Maintainer: IT team of IPESE Laboratory from EPFL
 Maintainer-email: joao.ferreiradasilva@epfl.ch
 Project-URL: Documentation, https://reho.readthedocs.io/en/main/
@@ -29,14 +29,18 @@
 Requires-Dist: sqlalchemy<2.0.0,>=1.4.42
 Requires-Dist: geopandas<1.0.0,>=0.12.2
 Requires-Dist: matplotlib<4.0.0,>=3.6.1
 Requires-Dist: plotly<6.0.0,>=5.10
 Requires-Dist: kaleido<1.0.0,>=0.2.1
 Requires-Dist: python-dotenv>=1.0
 Requires-Dist: requests<3.0.0,>=2.0.0
+Requires-Dist: coloredlogs>=15.0.1
+Requires-Dist: SALib>=1.4.8
+Requires-Dist: qmcpy>=1.4.5
+Requires-Dist: pvlib==0.10.*
 
 # REHO
 Renewable Energy Hub Optimizer (REHO) is a decision support tool for sustainable urban energy system planning.
 REHO simultaneously addresses the optimal design and operation of capacities, catering to multi-objective considerations
 across economic, environmental, and efficiency criteria.
 
 Key features:
@@ -49,35 +53,40 @@
 
 For more information about the model foundations and features, please refer to the [REHO documentation](https://reho.readthedocs.io/en/main/).
 
 ## Authors
 REHO is developed by EPFL (Switzerland), within the Industrial Process and Energy Systems Engineering (IPESE) group.
 
 Dorsan Lepour <dorsan.lepour@epfl.ch>  
-Cédric Terrier <cedric.terrier@epfl.ch>  
-Joseph Loustau <joseph.loustau@epfl.ch>
+Cédric Terrier <cedric.terrier@epfl.ch>
 
 ## Licence
 Copyright (C) <2021-2024> <Ecole Polytechnique Fédérale de Lausanne (EPFL), Switzerland>
 
-Licensed under the Apache License, Version0 (the "License");
+Licensed under the Apache License, (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at http://www.apache.org/licenses/LICENSE-2.0
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 Description and complete License: see LICENSE file.
 
 ## Installation
-1. Clone repository available at https://github.com/IPESE/REHO
-2. Create `venv` in the repository and install required libraries with
+
+REHO is available as a [PyPI package](https://pypi.org/project/REHO/) and can be installed via pip with:
+```
+pip install --extra-index-url https://pypi.ampl.com REHO
 ```
-pip install -r requirements.txt
+
+Full code can be accessed from the [REHO GitHub repository](https://github.com/IPESE/REHO) and cloned with:
 ```
-3. Please refer to "User guide" section of the documentation for step-by-step guidelines.
+git clone https://github.com/IPESE/REHO.git
+```
+
+Please refer to "[Getting started](https://reho.readthedocs.io/en/main/sections/5_Getting_started.html)" section of the documentation  for step-by-step guidelines.
 
 ## Suggestions and contributions
 All suggestions or implementation must be tracked with dedicated issues and reported in the project repository.
```

### Comparing `REHO-1.0.2/REHO.egg-info/SOURCES.txt` & `reho-1.1.0/REHO.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,32 +21,26 @@
 reho/data/infrastructure/district_units.csv
 reho/data/infrastructure/grids.csv
 reho/data/infrastructure/storage_units.csv
 reho/data/skydome/skyPatchesAreas.txt
 reho/data/skydome/skyPatchesCenPts.txt
 reho/data/skydome/total_irradiation.csv
 reho/data/skydome/typical_irradiation.csv
-reho/data/weather/Weekday_2005.txt
-reho/data/weather/hour/Disentis-hour.dat
-reho/data/weather/hour/Geneva-hour.dat
-reho/data/weather/hour/Lugano-hour.dat
-reho/data/weather/hour/Luzern-hour.dat
-reho/data/weather/hour/Piotta-hour.dat
-reho/data/weather/hour/Zuerich-Kloten-hour.dat
+reho/data/weather/weekday.txt
 reho/model/__init__.py
-reho/model/compact_optimization.py
-reho/model/district_decomposition.py
 reho/model/infrastructure.py
+reho/model/master_problem.py
 reho/model/reho.py
+reho/model/sub_problem.py
+reho/model/ampl_model/actors_problem.mod
 reho/model/ampl_model/data_stream.dat
 reho/model/ampl_model/data_stream_storage.dat
 reho/model/ampl_model/master_problem.mod
-reho/model/ampl_model/master_problem_actors.mod
-reho/model/ampl_model/model.mod
 reho/model/ampl_model/scenario.mod
+reho/model/ampl_model/sub_problem.mod
 reho/model/ampl_model/units/DHN.mod
 reho/model/ampl_model/units/DHN_HEX.mod
 reho/model/ampl_model/units/DHN_pipes.mod
 reho/model/ampl_model/units/air_conditioner.mod
 reho/model/ampl_model/units/data_heat.mod
 reho/model/ampl_model/units/electrical_heater.mod
 reho/model/ampl_model/units/heat_curtailment.mod
@@ -78,25 +72,27 @@
 reho/model/ampl_model/units/storage/dhwstorage.mod
 reho/model/ampl_model/units/storage/h2_storage.mod
 reho/model/ampl_model/units/storage/heatstorage.mod
 reho/model/ampl_model/units/storage/heatstorage_interperiod.mod
 reho/model/postprocessing/KPIs.py
 reho/model/postprocessing/__init__.py
 reho/model/postprocessing/building_scale_network_builder.py
+reho/model/postprocessing/sensitivity_analysis.py
 reho/model/postprocessing/write_results.py
 reho/model/preprocessing/EV_profile_generator.py
 reho/model/preprocessing/QBuildings.py
 reho/model/preprocessing/__init__.py
+reho/model/preprocessing/buildings_profiles.py
 reho/model/preprocessing/clustering.py
-reho/model/preprocessing/data_generation.py
 reho/model/preprocessing/electricity_prices.py
 reho/model/preprocessing/emissions_parser.py
+reho/model/preprocessing/local_data.py
 reho/model/preprocessing/sia_parser.py
 reho/model/preprocessing/skydome.py
 reho/model/preprocessing/weather.py
 reho/plotting/__init__.py
 reho/plotting/layout.csv
 reho/plotting/plotting.py
 reho/plotting/rainbow_plots.py
 reho/plotting/sankey.py
 reho/plotting/sia380_1.csv
-reho/plotting/yearly_profile_builder.py
+reho/plotting/utils.py
```

### Comparing `REHO-1.0.2/reho/data/SIA/sia2024_data.xlsx` & `reho-1.1.0/reho/data/SIA/sia2024_data.xlsx`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/SIA/sia2024_rooms_sia380_1.csv` & `reho-1.1.0/reho/data/SIA/sia2024_rooms_sia380_1.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/elcom/correspondance_table_municipality_operator.csv` & `reho-1.1.0/reho/data/elcom/correspondance_table_municipality_operator.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/emissions/electricity_matrix_2019_reduced.csv` & `reho-1.1.0/reho/data/emissions/electricity_matrix_2019_reduced.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/infrastructure/HP_parameters.txt` & `reho-1.1.0/reho/data/infrastructure/HP_parameters.txt`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/infrastructure/building_units.csv` & `reho-1.1.0/reho/data/infrastructure/building_units.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/infrastructure/district_units.csv` & `reho-1.1.0/reho/data/infrastructure/district_units.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/infrastructure/grids.csv` & `reho-1.1.0/reho/data/infrastructure/grids.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/infrastructure/storage_units.csv` & `reho-1.1.0/reho/data/infrastructure/storage_units.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/skydome/skyPatchesAreas.txt` & `reho-1.1.0/reho/data/skydome/skyPatchesAreas.txt`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/skydome/skyPatchesCenPts.txt` & `reho-1.1.0/reho/data/skydome/skyPatchesCenPts.txt`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/skydome/total_irradiation.csv` & `reho-1.1.0/reho/data/skydome/total_irradiation.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/skydome/typical_irradiation.csv` & `reho-1.1.0/reho/data/skydome/typical_irradiation.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/data/weather/Weekday_2005.txt` & `reho-1.1.0/reho/data/weather/weekday.txt`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/data_stream.dat` & `reho-1.1.0/reho/model/ampl_model/data_stream.dat`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/data_stream_storage.dat` & `reho-1.1.0/reho/model/ampl_model/data_stream_storage.dat`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/master_problem.mod` & `reho-1.1.0/reho/model/ampl_model/master_problem.mod`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 set UnitsOfLayer{Layers} within Units;
 
 set House;
 set HousesOfLayer{Layers} within House;
 set FeasibleSolutions ordered;
 
 set Period;				# Set of periods (days)
-set PeriodStandard; # TODO set time as function of period as in model.mod
+set PeriodStandard; # TODO set time as function of period as in sub_problem.mod
 set PeriodExtrem := {Period diff PeriodStandard};
 
 param TimeStart default 1;
 param TimeEnd{p in Period};
 set Time{p in Period} := {TimeStart .. TimeEnd[p]} ordered;
 
 param dt{p in Period} default 1;		#h
```

### Comparing `REHO-1.0.2/reho/model/ampl_model/master_problem_actors.mod` & `reho-1.1.0/reho/model/ampl_model/actors_problem.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/model.mod` & `reho-1.1.0/reho/model/ampl_model/sub_problem.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/scenario.mod` & `reho-1.1.0/reho/model/ampl_model/scenario.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/DHN.mod` & `reho-1.1.0/reho/model/ampl_model/units/DHN.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/DHN_HEX.mod` & `reho-1.1.0/reho/model/ampl_model/units/DHN_HEX.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/air_conditioner.mod` & `reho-1.1.0/reho/model/ampl_model/units/air_conditioner.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/data_heat.mod` & `reho-1.1.0/reho/model/ampl_model/units/data_heat.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/district_units/evehicle.mod` & `reho-1.1.0/reho/model/ampl_model/units/district_units/evehicle.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/district_units/heatpump_district.mod` & `reho-1.1.0/reho/model/ampl_model/units/district_units/heatpump_district.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/district_units/heatstorage_district.mod` & `reho-1.1.0/reho/model/ampl_model/units/district_units/heatstorage_district.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/district_units/ng_boiler_district.mod` & `reho-1.1.0/reho/model/ampl_model/units/district_units/ng_boiler_district.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/district_units/ng_cogeneration_district.mod` & `reho-1.1.0/reho/model/ampl_model/units/district_units/ng_cogeneration_district.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/electrical_heater.mod` & `reho-1.1.0/reho/model/ampl_model/units/electrical_heater.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/h2_units/SOEFC.mod` & `reho-1.1.0/reho/model/ampl_model/units/h2_units/SOEFC.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/h2_units/electrolyser.mod` & `reho-1.1.0/reho/model/ampl_model/units/h2_units/electrolyser.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/h2_units/fuel_cell.mod` & `reho-1.1.0/reho/model/ampl_model/units/h2_units/fuel_cell.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/h2_units/methanizer.mod` & `reho-1.1.0/reho/model/ampl_model/units/h2_units/methanizer.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/heat_curtailment.mod` & `reho-1.1.0/reho/model/ampl_model/units/heat_curtailment.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/heatpump.mod` & `reho-1.1.0/reho/model/ampl_model/units/heatpump.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/heatpump_anergy.mod` & `reho-1.1.0/reho/model/ampl_model/units/heatpump_anergy.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/ng_boiler.mod` & `reho-1.1.0/reho/model/ampl_model/units/ng_boiler.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/ng_cogeneration.mod` & `reho-1.1.0/reho/model/ampl_model/units/ng_cogeneration.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/ng_cogeneration_partload.mod` & `reho-1.1.0/reho/model/ampl_model/units/ng_cogeneration_partload.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/oil_boiler.mod` & `reho-1.1.0/reho/model/ampl_model/units/oil_boiler.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/pv.mod` & `reho-1.1.0/reho/model/ampl_model/units/pv.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/pv_orientation.mod` & `reho-1.1.0/reho/model/ampl_model/units/pv_orientation.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/CH4_tank.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/CH4_tank.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/LHS_storage.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/LHS_storage.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/PTES_aggregated.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/PTES_aggregated.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/PTES_split.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/PTES_split.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/battery.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/battery.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/battery_interperiod.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/battery_interperiod.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/dhwstorage.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/dhwstorage.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/h2_storage.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/h2_storage.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/heatstorage.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/heatstorage.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/storage/heatstorage_interperiod.mod` & `reho-1.1.0/reho/model/ampl_model/units/storage/heatstorage_interperiod.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/thermal_solar.mod` & `reho-1.1.0/reho/model/ampl_model/units/thermal_solar.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/ampl_model/units/wood_stove.mod` & `reho-1.1.0/reho/model/ampl_model/units/wood_stove.mod`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/model/compact_optimization.py` & `reho-1.1.0/reho/model/sub_problem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,220 +1,202 @@
-import os
-from amplpy import AMPL, Environment
 import itertools as itertools
-import reho.model.preprocessing.data_generation as DGF
-import reho.model.preprocessing.weather as WD
-import reho.model.preprocessing.skydome as SkyDome
-import reho.model.preprocessing.emissions_parser as emissions
+import logging
+
+from amplpy import AMPL, Environment
+
 import reho.model.preprocessing.EV_profile_generator as EV_gen
+import reho.model.preprocessing.buildings_profiles as buildings_profiles
+import reho.model.preprocessing.emissions_parser as emissions
+import reho.model.preprocessing.weather as weather
 from reho.model.preprocessing.QBuildings import *
 
 
-class compact_optimization:
+__doc__ = """
+File for handling data and optimization for an AMPL sub-problem.
+"""
+
+
+class SubProblem:
     """
-            Collects all the data input and sends it an AMPL model, solves the optimization.
+    Collects all the data input and sends it an AMPL model, solves the optimization.
 
-            Parameters
-            ----------
-            district : district
-                Instance of the class district, contains relevant structure in the district such as Units or grids.
-            buildings_data : dict
-                Dictionary containing relevant Building data.
-            parameters : dict, optional
-                Dictionary containing 'new' parameters for the AMPL model. If incomplete, uses data from buildings_data.
-            set_indexed : dict, optional
-                Dictionary containing new data which are indexed sets in the AMPL model.
-            cluster : dict, optional
-                Dictionary containing information about clustering.
-            scenario : dict, optional
-                Dictionary containing the objective function, EMOO constraints, and additional constraints.
-            method : dict, optional
-                Dictionary containing different options for methodology choices.
-            solver : str, optional
-                Chosen solver for AMPL (gurobi, cplex, highs, cbc...).
-            qbuildings_data : dict, optional
-                Dictionary containing input data for the buildings.
-
-            See also
-            --------
-            reho.model.reho.reho
-            reho.model.district_decomposition.district_decomposition
+    Parameters
+    ----------
+    district : district
+        Instance of the class district, contains relevant structure in the district such as Units or grids.
+    buildings_data : dict
+        Building-specific data.
+    local_data : dict
+        Location-specific data.
+    parameters : dict, optional
+        Dictionary containing 'new' parameters for the AMPL model. If incomplete, uses data from buildings_data.
+    set_indexed : dict, optional
+        Dictionary containing new data which are indexed sets in the AMPL model.
+    cluster : dict, optional
+        Dictionary containing information about clustering.
+    scenario : dict, optional
+        Dictionary containing the objective function, EMOO constraints, and additional constraints.
+    method : dict, optional
+        Dictionary containing different options for methodology choices.
+    solver : str, optional
+        Chosen solver for AMPL (gurobi, cplex, HiGHS, cbc...).
+    qbuildings_data : dict, optional
+        Input data for the buildings.
+
+    See also
+    --------
+    reho.model.reho.reho
+    reho.model.master_problem.MasterProblem
 
-            """
-    def __init__(self, district, buildings_data, parameters, set_indexed, cluster, scenario, method, solver, qbuildings_data=None):
+    """
+
+    def __init__(self, district, buildings_data, local_data, parameters, set_indexed, cluster, scenario, method, solver, qbuildings_data=None):
 
-        self.buildings_data_compact = buildings_data
+        self.buildings_data_sp = buildings_data
         if method['use_facades']:
-            self.facades_compact = qbuildings_data['facades_data']
-            self.shadows_compact = qbuildings_data['shadows_data']
+            self.facades_sp = qbuildings_data['facades_data']
+            self.shadows_sp = qbuildings_data['shadows_data']
         if method['use_pv_orientation']:
-           self.roofs_compact = qbuildings_data['roofs_data']
-        self.infrastructure_compact = district
-        self.parameters_compact = parameters
-        self.set_indexed_compact = set_indexed
-        self.cluster_compact = cluster
+            self.roofs_sp = qbuildings_data['roofs_data']
+        self.infrastructure_sp = district
+        self.local_data = local_data
+        self.parameters_sp = parameters
+        self.set_indexed_sp = set_indexed
+        self.cluster_sp = cluster
         if 'exclude_units' not in scenario:
             scenario['exclude_units'] = []
         if 'enforce_units' not in scenario:
             scenario['enforce_units'] = []
-        self.scenario_compact = scenario
-        self.method_compact = method
+        self.scenario_sp = scenario
+        self.method_sp = method
         self.solver = solver
         self.parameters_to_ampl = dict()
 
-        # print('Execute for building:', self.buildings_data_compact)
-        # print('With parameters and sets:', self.parameters_compact, self.set_indexed_compact)
-        # print('Cluster settings are:', self.cluster_compact)
-
-    def solve_model(self):
-        ampl = self.build_model_without_solving()
-
-        debugging = False
-        if debugging:
-            # ampl.exportData('loaded_data.dat')
-            # ampl.expotModel('loaded_model.mod')
-            ampl.eval('suffix iis symbolic OUT;')
-            ampl.setOption('presolve', 1)
-
-        # ampl evaluation to speed up the optimization in case we have cogeneration units (since it has many integer variables)
-        #ampl.eval("suffix priority IN, integer, >= 0, <= 9999; let {u in Units} Units_Use[u].priority := 9999; "
-        #          "let {u in UnitsOfType['NG_Cogeneration'],p in Period,t in Time[p]} Units_Use_t[u,p,t].priority := "
-        #          "200*round(max{i in Period,j in Time[i]}(T_ext[i,j])-T_ext[p,t],0);")
-        ampl.solve()
-
-        if debugging:
-            ampl.eval('display {i in 1.._ncons: _con[i].iis <> "0"} (_conname[i], _con[i].iis);')
-            ampl.eval('for {i in 1.._ncons: _con[i].iis <> "0"} expand _con[i]; ')
-            ampl.eval('display{j in 1.._nvars: _var[j].iis <> "0"}(_varname[j], _var[j].iis);')
-
-        exitcode = exitcode_from_ampl(ampl)
-        return ampl, exitcode
-
     def build_model_without_solving(self):
-        File_ID = WD.get_cluster_file_ID(self.cluster_compact)
+        File_ID = weather.get_cluster_file_ID(self.cluster_sp)
 
         self.initialize_parameters_for_ampl_and_python()
         ampl = self.init_ampl_model()
         ampl = self.set_weather_data(ampl)
         ampl = self.set_ampl_sets(ampl)
         self.set_emissions_profiles(File_ID)
-        self.set_gains_and_demands_profiles(ampl, File_ID)
+        self.set_temperature_and_EVs_profiles()
         self.set_HP_parameters(ampl)
         self.set_streams_temperature(ampl)
-        if self.method_compact['use_pv_orientation']:
-            self.set_PV_models(ampl, File_ID)
+        if self.method_sp['use_pv_orientation']:
+            self.set_PV_models(ampl)
         ampl = self.send_parameters_and_sets_to_ampl(ampl)
         ampl = self.set_scenario(ampl)
 
         return ampl
 
     def initialize_parameters_for_ampl_and_python(self):
         # -----------------------------------------------------------------------------------------------------#
         # Default methods
         # -----------------------------------------------------------------------------------------------------#
-        self.method_compact = initialize_default_methods(self.method_compact)
+        self.method_sp = initialize_default_methods(self.method_sp)
         # -----------------------------------------------------------------------------------------------------#
         # Input Parameter Preparation
         # -----------------------------------------------------------------------------------------------------#
 
         # prepare input parameter which are used in AMPL model
 
-        buildings_to_ampl = ['ERA', 'SolarRoofArea',  'U_h', 'HeatCapacity',
+        buildings_to_ampl = ['ERA', 'SolarRoofArea', 'U_h', 'HeatCapacity',
                              'T_comfort_min_0', 'Th_supply_0', 'Th_return_0', 'Tc_supply_0', 'Tc_return_0']
 
         for parameter in buildings_to_ampl:
             self.parameters_to_ampl[parameter] = {}
-            for i, b in enumerate(self.buildings_data_compact):
-                if parameter not in self.parameters_compact:
-                    self.parameters_to_ampl[parameter][b] = self.buildings_data_compact[b][parameter]
+            for i, b in enumerate(self.buildings_data_sp):
+                if parameter not in self.parameters_sp:
+                    self.parameters_to_ampl[parameter][b] = self.buildings_data_sp[b][parameter]
                 else:
-                    self.parameters_to_ampl[parameter][b] = self.parameters_compact[parameter]
-
+                    self.parameters_to_ampl[parameter][b] = self.parameters_sp[parameter]
 
     def init_ampl_model(self):
         if os.getenv('USE_AMPL_MODULES', False):
             from amplpy import modules
             modules.load()
             ampl = AMPL()
         else:
             try:
                 ampl = AMPL(Environment(os.environ["AMPL_PATH"]))
             except:
                 raise Exception("AMPL_PATH is not defined. Please include a .env file at the project root (e.g., AMPL_PATH='C:/AMPL')")
-        # print(ampl.getOption('version'))
 
         # -AMPL (GNU) OPTIONS
         ampl.setOption('solution_round', 11)
 
         ampl.setOption('presolve_eps', 1e-4)  # -ignore difference between upper and lower bound by this tolerance
         ampl.setOption('presolve_inteps', 1e-6)  # -tolerance added/substracted to each upper/lower bound
         ampl.setOption('presolve_fixeps', 1e-9)
-        ampl.setOption('show_stats', 0)
+        if not self.method_sp['print_logs']:
+            ampl.setOption('show_stats', 0)
+            ampl.setOption('solver_msg', 0)
 
         # -SOLVER OPTIONS
         ampl.setOption('solver', self.solver)
         if self.solver == "gurobi":
             ampl.eval("option gurobi_options 'NodeFileStart=0.5';")
         if self.solver == "cplex":
             ampl.eval("option cplex_options 'bestbound mipgap=5e-7 integrality=1e-09 timing=1 timelimit=3000';")
 
         # -----------------------------------------------------------------------------------------------------#
         #  MODEL FILES
         # -----------------------------------------------------------------------------------------------------#
         ampl.cd(path_to_ampl_model)
-        ampl.read('model.mod')
+        ampl.read('sub_problem.mod')
 
         # Energy conversion Units
         ampl.cd(path_to_units)
-        if 'ElectricalHeater' in self.infrastructure_compact.UnitTypes:
+        if 'ElectricalHeater' in self.infrastructure_sp.UnitTypes:
             ampl.read('electrical_heater.mod')
-        if 'NG_Boiler' in self.infrastructure_compact.UnitTypes:
+        if 'NG_Boiler' in self.infrastructure_sp.UnitTypes:
             ampl.read('ng_boiler.mod')
-        if 'OIL_Boiler' in self.infrastructure_compact.UnitTypes:
+        if 'OIL_Boiler' in self.infrastructure_sp.UnitTypes:
             ampl.read('oil_boiler.mod')
-        if 'WOOD_Stove' in self.infrastructure_compact.UnitTypes:
+        if 'WOOD_Stove' in self.infrastructure_sp.UnitTypes:
             ampl.read('wood_stove.mod')
-        if 'HeatPump' in self.infrastructure_compact.UnitTypes:
+        if 'HeatPump' in self.infrastructure_sp.UnitTypes:
             ampl.read('heatpump.mod')
-        if 'Air_Conditioner' in self.infrastructure_compact.UnitTypes:
+        if 'Air_Conditioner' in self.infrastructure_sp.UnitTypes:
             ampl.read('air_conditioner.mod')
-        if 'ThermalSolar' in self.infrastructure_compact.UnitTypes:
+        if 'ThermalSolar' in self.infrastructure_sp.UnitTypes:
             ampl.read('thermal_solar.mod')
-        if 'DataHeat' in self.infrastructure_compact.UnitTypes:
+        if 'DataHeat' in self.infrastructure_sp.UnitTypes:
             ampl.read('data_heat.mod')
-        if 'NG_Cogeneration' in self.infrastructure_compact.UnitTypes:
+        if 'NG_Cogeneration' in self.infrastructure_sp.UnitTypes:
             ampl.read('ng_cogeneration.mod')
-        if 'DHN_hex' in self.infrastructure_compact.UnitTypes:
+        if 'DHN_hex' in self.infrastructure_sp.UnitTypes:
             ampl.read('DHN_HEX.mod')
             ampl.read('DHN_pipes.mod')
-        if 'PV' in self.infrastructure_compact.UnitTypes:
-            if self.method_compact['use_pv_orientation']:  # Choose the photovoltaics model if PV orientation - give hourly PV electricity profiles
+        if 'PV' in self.infrastructure_sp.UnitTypes:
+            if self.method_sp['use_pv_orientation']:
                 ampl.read('pv_orientation.mod')
             else:
                 ampl.read('pv.mod')
 
         # district Units
-        if 'EV' in self.infrastructure_compact.UnitTypes:
+        if 'EV' in self.infrastructure_sp.UnitTypes:
             ampl.cd(path_to_district_units)
             ampl.read('evehicle.mod')
         # Storage Units
         ampl.cd(path_to_units_storage)
-        if 'WaterTankSH' in self.infrastructure_compact.UnitTypes:
+        if 'WaterTankSH' in self.infrastructure_sp.UnitTypes:
             ampl.read('heatstorage.mod')
-        if 'WaterTankDHW' in self.infrastructure_compact.UnitTypes:
+        if 'WaterTankDHW' in self.infrastructure_sp.UnitTypes:
             ampl.read('dhwstorage.mod')
-        if 'Battery' in self.infrastructure_compact.UnitTypes:
+        if 'Battery' in self.infrastructure_sp.UnitTypes:
             ampl.read('battery.mod')
         ampl.cd(path_to_ampl_model)
 
         # Objectives, epsilon constraints and specific constraints
         ampl.read('scenario.mod')
 
         # TODO: integrate Jules units into district structure (avoid using ampl eval)
-        if self.method_compact['use_Storage_Interperiod']:
+        if self.method_sp['use_Storage_Interperiod']:
             ampl.eval(
                 'set UnitsOfStorage := setof{u in UnitsOfType["Battery_interperiod"] union UnitsOfType["PTES_storage"]'
                 'union UnitsOfType["PTES_conversion"] union UnitsOfType["CH4storage"]'
                 'union UnitsOfType["H2storage"] union UnitsOfType["SOEFC"]'
                 'union UnitsOfType["Methanizer"] union UnitsOfType["FuelCell"]'
                 'union UnitsOfType["Electrolyzer"] union UnitsOfType["WaterTankSH_interperiod"]'
                 'union UnitsOfType["SolidLiquidLHS"]'
@@ -246,205 +228,202 @@
     def set_weather_data(self, ampl):
         # -----------------------------------------------------------------------------------------------------#
         # -Setting DATA
         # -----------------------------------------------------------------------------------------------------#
 
         ampl.cd(path_to_clustering)
 
-        File_ID = WD.get_cluster_file_ID(self.cluster_compact)
+        File_ID = weather.get_cluster_file_ID(self.cluster_sp)
 
         ampl.readData('frequency_' + File_ID + '.dat')
         ampl.readData('index_' + File_ID + '.dat')
         self.parameters_to_ampl['T_ext'] = np.loadtxt(os.path.join(path_to_clustering, 'T_' + File_ID + '.dat'))
-        self.parameters_to_ampl['I_global'] = np.loadtxt(os.path.join(path_to_clustering, 'GHI_' + File_ID + '.dat'))
+        self.parameters_to_ampl['I_global'] = np.loadtxt(os.path.join(path_to_clustering, 'Irr_' + File_ID + '.dat'))
 
         ampl.cd(path_to_ampl_model)
+
         return ampl
 
     def set_ampl_sets(self, ampl):
         # -----------------------------------------------------------------------------------------------------#
         # Design Structure: Building Cluster, Units and Layers
         # -----------------------------------------------------------------------------------------------------#
 
-        if self.method_compact['use_discrete_units']:
-            self.infrastructure_compact.set_discretize_unit_size()
+        if self.method_sp['use_discrete_units']:
+            self.infrastructure_sp.set_discretize_unit_size()
 
-        self.parameters_to_ampl['Units_flowrate'] = self.infrastructure_compact.Units_flowrate
-        self.parameters_to_ampl['Grids_flowrate'] = self.infrastructure_compact.Grids_flowrate
-        self.parameters_to_ampl['Grids_Parameters'] = self.infrastructure_compact.Grids_Parameters
-        self.parameters_to_ampl['Grids_Parameters_lca'] = self.infrastructure_compact.Grids_Parameters_lca
-        self.parameters_to_ampl['Units_Parameters'] = self.infrastructure_compact.Units_Parameters
-        self.parameters_to_ampl['Units_Parameters_lca'] = self.infrastructure_compact.Units_Parameters_lca
-        self.parameters_to_ampl['Streams_H'] = self.infrastructure_compact.Streams_H
-
-        for key in self.infrastructure_compact.HP_parameters:
-            self.parameters_to_ampl[key] = self.infrastructure_compact.HP_parameters[key]
-
-        for s in self.infrastructure_compact.Set:
-            if isinstance(self.infrastructure_compact.Set[s], np.ndarray):
-                ampl.getSet(str(s)).setValues(self.infrastructure_compact.Set[s])
-            elif isinstance(self.infrastructure_compact.Set[s], dict):
+        self.parameters_to_ampl['Units_flowrate'] = self.infrastructure_sp.Units_flowrate
+        self.parameters_to_ampl['Grids_flowrate'] = self.infrastructure_sp.Grids_flowrate
+        self.parameters_to_ampl['Grids_Parameters'] = self.infrastructure_sp.Grids_Parameters
+        self.parameters_to_ampl['Grids_Parameters_lca'] = self.infrastructure_sp.Grids_Parameters_lca
+        self.parameters_to_ampl['Units_Parameters'] = self.infrastructure_sp.Units_Parameters
+        self.parameters_to_ampl['Units_Parameters_lca'] = self.infrastructure_sp.Units_Parameters_lca
+        self.parameters_to_ampl['Streams_H'] = self.infrastructure_sp.Streams_H
+
+        for key in self.infrastructure_sp.HP_parameters:
+            self.parameters_to_ampl[key] = self.infrastructure_sp.HP_parameters[key]
+
+        for s in self.infrastructure_sp.Set:
+            if isinstance(self.infrastructure_sp.Set[s], np.ndarray):
+                ampl.getSet(str(s)).setValues(self.infrastructure_sp.Set[s])
+            elif isinstance(self.infrastructure_sp.Set[s], dict):
                 for i, instance in ampl.getSet(str(s)):
-                    instance.setValues(self.infrastructure_compact.Set[s][i])
+                    instance.setValues(self.infrastructure_sp.Set[s][i])
             else:
                 raise ValueError('Type Error setting AMPLPY Set', s)
 
         all_units = [unit for unit, value in ampl.getVariable('Units_Use').instances()]
         for i in all_units:
-            for u in self.scenario_compact['exclude_units']:
+            for u in self.scenario_sp['exclude_units']:
                 if 'district' not in i and u in i:  # unit at the building scale
-                        ampl.getVariable('Units_Use').get(str(i)).fix(0)
+                    ampl.getVariable('Units_Use').get(str(i)).fix(0)
                 elif u in all_units:  # unit at the district scale with problem definition at the district scale
                     ampl.getVariable('Units_Use').get(str(u)).fix(0)
 
-            for u in self.scenario_compact['enforce_units']:
+            for u in self.scenario_sp['enforce_units']:
                 if 'district' not in i and u in i:  # unit at the building scale
-                        ampl.getVariable('Units_Use').get(str(i)).fix(1)  # !!Fmin = 0, leaves the option to exclude unit
+                    ampl.getVariable('Units_Use').get(str(i)).fix(1)  # !!Fmin = 0, leaves the option to exclude unit
                 elif u in all_units:  # unit at the district scale with problem definition at the district scale
                     ampl.getVariable('Units_Use').get(str(u)).fix(1)
 
         return ampl
 
     def set_emissions_profiles(self, File_ID):
 
-        df_em = emissions.return_typical_emission_profiles(self.cluster_compact, File_ID, 'GWP100a')
-        if self.method_compact['use_dynamic_emission_profiles']:
+        df_em = emissions.return_typical_emission_profiles(self.cluster_sp, File_ID, 'GWP100a', self.local_data["df_Timestamp"],
+                                                           self.local_data["df_Emissions"])
+        if self.method_sp['use_dynamic_emission_profiles']:
             self.parameters_to_ampl['GWP_supply'] = df_em
             self.parameters_to_ampl['GWP_demand'] = df_em.rename(columns={'GWP_supply': 'GWP_demand'})
-            self.parameters_to_ampl['Gas_emission'] = self.infrastructure_compact.Grids_Parameters.drop('Electricity').drop(
+            self.parameters_to_ampl['Gas_emission'] = self.infrastructure_sp.Grids_Parameters.drop('Electricity').drop(
                 columns=['Cost_demand_cst', 'Cost_supply_cst'])
 
-    def set_gains_and_demands_profiles(self, ampl, File_ID):
+    def set_temperature_and_EVs_profiles(self):
 
         # Reference temperature
-        #self.parameters_to_ampl['T_comfort_min'] = DGF.profile_reference_temperature(self.parameters_to_ampl, self.cluster_compact)
-
-        # Heat gains from solar
-        self.parameters_to_ampl['SolarGains'] = DGF.solar_gains_profile(ampl, self.buildings_data_compact, File_ID)
+        self.parameters_to_ampl['T_comfort_min'] = buildings_profiles.reference_temperature_profile(self.parameters_to_ampl, self.cluster_sp)
 
         # Set default EV plug out profile if EVs are allowed
         if "EV_plugged_out" not in self.parameters_to_ampl:
-            if len(self.infrastructure_compact.UnitsOfDistrict) != 0:
-                if "EV_district" in self.infrastructure_compact.UnitsOfDistrict:
-                    self.parameters_to_ampl["EV_plugged_out"], self.parameters_to_ampl["EV_plugging_in"] = EV_gen.generate_EV_plugged_out_profiles_district(self.cluster_compact)
+            if len(self.infrastructure_sp.UnitsOfDistrict) != 0:
+                if "EV_district" in self.infrastructure_sp.UnitsOfDistrict:
+                    self.parameters_to_ampl["EV_plugged_out"], self.parameters_to_ampl["EV_plugging_in"] = EV_gen.generate_EV_plugged_out_profiles_district(
+                        self.cluster_sp, self.local_data["df_Timestamp"])
 
     def set_HP_parameters(self, ampl):
         # --------------- Heat Pump ---------------------------------------------------------------------------#
         # T = 7.5C for Lake, T = 12C for underground, T = 16C for CO2
 
         df_end = ampl.getParameter('TimeEnd').getValues().toPandas()
         timesteps = int(df_end['TimeEnd'].sum())  # total number of timesteps
         sources = []
-        if 'T_source' in self.parameters_compact:
-            sources = self.parameters_compact['T_source'].keys()
+        if 'T_source' in self.parameters_sp:
+            sources = self.parameters_sp['T_source'].keys()
 
         T_source = []
-        if 'HeatPump' in self.infrastructure_compact.UnitsOfType:
-            for unit in self.infrastructure_compact.UnitsOfType['HeatPump']:
-                if any([i in unit for i in sources]):   # if T_source defined from script
+        if 'HeatPump' in self.infrastructure_sp.UnitsOfType:
+            for unit in self.infrastructure_sp.UnitsOfType['HeatPump']:
+                if any([i in unit for i in sources]):  # if T_source defined from script
                     source = list(itertools.compress(sources, [i in unit for i in sources]))[0]
-                    T_source = np.concatenate([T_source, np.repeat(self.parameters_compact['T_source'][source], timesteps)])
+                    T_source = np.concatenate([T_source, np.repeat(self.parameters_sp['T_source'][source], timesteps)])
                 elif 'Air' in unit:
                     T_source = np.concatenate([T_source, self.parameters_to_ampl['T_ext']])
                 elif 'Lake' in unit:
                     T_source = np.concatenate([T_source, np.repeat(7.5, timesteps)])
                 elif 'Geothermal' in unit:
                     T_source = np.concatenate([T_source, np.repeat(8, timesteps)])
                 elif 'Anergy' in unit:
                     T_source = np.concatenate([T_source, np.repeat(16, timesteps)])
                 elif 'DHN' in unit:
-                    if 'T_DHN_supply' and 'T_DHN_return' in self.parameters_compact:
-                        T_DHN_mean = (self.parameters_compact["T_DHN_supply"] + self.parameters_compact["T_DHN_return"]) / 2
-                    elif 'T_DHN_supply_cst' and 'T_DHN_return_cst' in self.parameters_compact:
-                        T_DHN_mean = (self.parameters_compact["T_DHN_supply_cst"] + self.parameters_compact["T_DHN_return_cst"]) / 2
+                    if 'T_DHN_supply' and 'T_DHN_return' in self.parameters_sp:
+                        T_DHN_mean = (self.parameters_sp["T_DHN_supply"] + self.parameters_sp["T_DHN_return"]) / 2
+                    elif 'T_DHN_supply_cst' and 'T_DHN_return_cst' in self.parameters_sp:
+                        T_DHN_mean = (self.parameters_sp["T_DHN_supply_cst"] + self.parameters_sp["T_DHN_return_cst"]) / 2
                         T_DHN_mean = np.repeat(T_DHN_mean, timesteps)
                     else:
                         T_DHN_mean = np.repeat(16, timesteps)
                     T_source = np.concatenate([T_source, T_DHN_mean])
                 else:
                     raise Exception('HP source undefined')
 
             self.parameters_to_ampl['T_source'] = T_source
-            if 'T_source' in self.parameters_compact:
-                del self.parameters_compact["T_source"]
+            if 'T_source' in self.parameters_sp:
+                del self.parameters_sp["T_source"]
 
         sources = []
-        if 'T_source_cool' in self.parameters_compact:
-            sources = self.parameters_compact['T_source_cool'].keys()
+        if 'T_source_cool' in self.parameters_sp:
+            sources = self.parameters_sp['T_source_cool'].keys()
 
         T_source_cool = np.array([])
-        if 'Air_Conditioner' in self.infrastructure_compact.UnitsOfType:
-            for unit in self.infrastructure_compact.UnitsOfType['Air_Conditioner']:
+        if 'Air_Conditioner' in self.infrastructure_sp.UnitsOfType:
+            for unit in self.infrastructure_sp.UnitsOfType['Air_Conditioner']:
                 # if T_source_cool defined from script
                 if any([i in unit for i in sources]):
                     source = list(itertools.compress(sources, [i in unit for i in sources]))[0]
-                    T_source_cool = np.concatenate([T_source_cool, np.repeat(self.parameters_compact['T_source_cool'][source], timesteps)])
+                    T_source_cool = np.concatenate([T_source_cool, np.repeat(self.parameters_sp['T_source_cool'][source], timesteps)])
 
                 elif "DHN" in unit:
-                    if 'T_DHN_supply' and 'T_DHN_return' in self.parameters_compact:
-                        T_DHN_mean = (self.parameters_compact["T_DHN_supply"] + self.parameters_compact["T_DHN_return"]) / 2
-                    elif 'T_DHN_supply_cst' and 'T_DHN_return_cst' in self.parameters_compact:
-                        T_DHN_mean = (self.parameters_compact["T_DHN_supply_cst"] + self.parameters_compact["T_DHN_return_cst"]) / 2
+                    if 'T_DHN_supply' and 'T_DHN_return' in self.parameters_sp:
+                        T_DHN_mean = (self.parameters_sp["T_DHN_supply"] + self.parameters_sp["T_DHN_return"]) / 2
+                    elif 'T_DHN_supply_cst' and 'T_DHN_return_cst' in self.parameters_sp:
+                        T_DHN_mean = (self.parameters_sp["T_DHN_supply_cst"] + self.parameters_sp["T_DHN_return_cst"]) / 2
                         T_DHN_mean = np.repeat(T_DHN_mean, timesteps)
                     else:
                         T_DHN_mean = np.repeat(16, timesteps)
                     T_source_cool = np.concatenate([T_source_cool, T_DHN_mean])
 
                 elif "Air" in unit:
                     T_source_cool = np.concatenate([T_source_cool, self.parameters_to_ampl['T_ext']])
 
                 else:
                     raise Exception('AC sink undefined')
 
             self.parameters_to_ampl['T_source_cool'] = T_source_cool
-            if 'T_source_cool' in self.parameters_compact:
-                del self.parameters_compact["T_source_cool"]
+            if 'T_source_cool' in self.parameters_sp:
+                del self.parameters_sp["T_source_cool"]
 
     def set_streams_temperature(self, ampl):
 
         df_end = ampl.getParameter('TimeEnd').getValues().toPandas()
         timesteps = int(df_end['TimeEnd'].sum())
         df_Streams_T = pd.DataFrame(columns=["Period", "Time", "Streams", "Streams_Tout", "Streams_Tin"])
         df_Streams_T = df_Streams_T.set_index(["Period", "Time", "Streams"])
 
-        index = [[(i, j+1) for j in list(range(int(df_end["TimeEnd"][i])))] for i in df_end.index]
+        index = [[(i, j + 1) for j in list(range(int(df_end["TimeEnd"][i])))] for i in df_end.index]
         index = [j for i in index for j in i]
         index = pd.MultiIndex.from_tuples(index, names=["Period", "Time"])
 
-        for bui in self.infrastructure_compact.houses:
-            for unit_data in self.infrastructure_compact.houses[bui]["units"]:
+        for bui in self.infrastructure_sp.houses:
+            for unit_data in self.infrastructure_sp.houses[bui]["units"]:
                 for i, T_level in enumerate(unit_data["StreamsOfUnit"]):
                     stream = unit_data["name"] + '_' + bui + '_' + T_level
                     df = pd.DataFrame(np.repeat(stream, timesteps), index=index, columns=["Streams"])
                     df["Streams_Tout"] = unit_data["stream_Tout"][i]
                     df["Streams_Tin"] = unit_data["stream_Tin"][i]
                     df.set_index("Streams", append=True, inplace=True)
                     df_Streams_T = pd.concat([df_Streams_T, df])
-            for stream in self.infrastructure_compact.StreamsOfBuilding[bui]:
+            for stream in self.infrastructure_sp.StreamsOfBuilding[bui]:
                 df = pd.DataFrame(np.repeat(stream, timesteps), index=index, columns=["Streams"])
-                df["Streams_Tout"] = 40 # default value that is changed in data_stream.dat
+                df["Streams_Tout"] = 40  # default value that is changed in data_stream.dat
                 df["Streams_Tin"] = 50  # default value that is changed in data_stream.dat
                 df.set_index("Streams", append=True, inplace=True)
                 df_Streams_T = pd.concat([df_Streams_T, df])
 
         self.parameters_to_ampl['streams_T'] = df_Streams_T.reorder_levels([2, 0, 1])
 
-
-
-    def set_PV_models(self, ampl, File_ID):
+    def set_PV_models(self, ampl):
         # --------------- PV Panels ---------------------------------------------------------------------------#
 
-        df_dome = SkyDome.skydome_to_df()
+        df_dome = skydome.skydome_to_df(self.local_data)
         self.parameters_to_ampl['Sin_a'] = df_dome.Sin_a.values
         self.parameters_to_ampl['Cos_a'] = df_dome.Cos_a.values
         self.parameters_to_ampl['Sin_e'] = df_dome.Sin_e.values
         self.parameters_to_ampl['Cos_e'] = df_dome.Cos_e.values
 
-        total_irradiation = os.path.join(path_to_skydome, 'total_irradiation.csv')
-        df_irr = SkyDome.irradiation_to_df(ampl, total_irradiation, File_ID)
+        df_irr = skydome.irradiation_to_df(ampl, self.local_data["df_Irradiation"], self.local_data["df_Timestamp"])
         self.parameters_to_ampl['Irr'] = df_irr
         # On Flat Roofs optimal Orientation of PV panel is chosen by the solver, Construction of possible Configurations
         # Azimuth = np.array([])
         # Tilt = np.array([])
         Azimuth = np.array(range(160, 210, 10))
         Tilt = np.array([5, 10, 20, 30, 40])
 
@@ -459,19 +438,19 @@
 
         np_surface = np.array([])
         np_flat_roof = np.array([])
         np_tilted_roof = np.array([])
         dict_SurfaceofHouse = {}
         dict_config = {}
         df_SurfaceArea = pd.DataFrame()
-        self.set_indexed_compact['Surface'] = np.array([])
+        self.set_indexed_sp['Surface'] = np.array([])
 
-        for b in self.buildings_data_compact:
+        for b in self.buildings_data_sp:
 
-            df_roofs = self.roofs_compact[self.roofs_compact['id_building'] == self.buildings_data_compact[b]['id_building']]
+            df_roofs = self.roofs_sp[self.roofs_sp['id_building'] == self.buildings_data_sp[b]['id_building']]
             # df_profiles is not used, but precalculated by the ampl model
             #  Surface/ Roof Area Values are selected matching to egid
             np_surface = np.append(np_surface, df_roofs['ROOF_ID'].values)
             dict_SurfaceofHouse[b] = df_roofs['ROOF_ID'].values
 
             # Flat roof if Tilt of Roof is either 1 or 0/ Tilted Roofs are all opposite to flat roofs
             Flat_roofs = df_roofs.ROOF_ID.loc[(df_roofs['TILT'] == 1) | (df_roofs['TILT'] == 0)].values
@@ -490,208 +469,224 @@
 
             # get area of surface
             index = pd.MultiIndex.from_tuples([(b, s) for s in df_roofs['ROOF_ID'].values])
             df = pd.DataFrame(df_roofs['AREA'].values, index=index, columns=['HouseSurfaceArea'])
             df_SurfaceArea = pd.concat([df_SurfaceArea, df])
 
         self.parameters_to_ampl['HouseSurfaceArea'] = df_SurfaceArea
-        self.set_indexed_compact['Surface'] = np.append(self.set_indexed_compact['Surface'], np_surface)
-        self.set_indexed_compact['SurfaceOfHouse'] = dict_SurfaceofHouse
+        self.set_indexed_sp['Surface'] = np.append(self.set_indexed_sp['Surface'], np_surface)
+        self.set_indexed_sp['SurfaceOfHouse'] = dict_SurfaceofHouse
 
-        self.set_indexed_compact['SurfaceTypes'] = np.array(['Flat_roof', 'Tilted_roof', 'Facades'])
-        self.set_indexed_compact['SurfaceOfType'] = {'Flat_roof': np_flat_roof, 'Tilted_roof': np_tilted_roof, 'Facades': []}
-        self.set_indexed_compact['ConfigOfSurface'] = dict_config
+        self.set_indexed_sp['SurfaceTypes'] = np.array(['Flat_roof', 'Tilted_roof', 'Facades'])
+        self.set_indexed_sp['SurfaceOfType'] = {'Flat_roof': np_flat_roof, 'Tilted_roof': np_tilted_roof, 'Facades': []}
+        self.set_indexed_sp['ConfigOfSurface'] = dict_config
 
         np_facades = np.array([])
         df_limit_angle = pd.DataFrame()
 
-        if self.method_compact['use_facades']:
-            for b in self.buildings_data_compact:
-                df_facades = self.facades_compact[self.facades_compact['id_building'] == self.buildings_data_compact[b]['id_building']]
-                df_shadows = self.shadows_compact[self.shadows_compact['id_building'] == self.buildings_data_compact[b]['id_building']]
+        if self.method_sp['use_facades']:
+            for b in self.buildings_data_sp:
+                df_facades = self.facades_sp[self.facades_sp['id_building'] == self.buildings_data_sp[b]['id_building']]
+                df_shadows = self.shadows_sp[self.shadows_sp['id_building'] == self.buildings_data_sp[b]['id_building']]
                 facades = df_facades['Facades_ID']
                 np_facades = np.append(np_facades, facades)
-                df_shadow = return_shadows_id_building(self.buildings_data_compact[b]['id_building'], df_shadows)
+                df_shadow = return_shadows_id_building(self.buildings_data_sp[b]['id_building'], df_shadows, self.local_data)
                 df_shadow = pd.concat([df_shadow], keys=[b], names=['House'])
                 df_limit_angle = pd.concat([df_limit_angle, df_shadow])
                 for fc in facades:
                     az = df_facades.AZIMUTH.loc[(df_facades['Facades_ID'] == fc)].values
                     # Tilt is not available for facades
                     # ti = df_facades.TILT.loc[(df_facades['Facades_ID'] == fc)].values
                     ti = 0
-                    self.set_indexed_compact['ConfigOfSurface'][fc] = [az[0], ti]
-                self.set_indexed_compact['SurfaceOfHouse'][b] = np.append(
-                    self.set_indexed_compact['SurfaceOfHouse'][b],
+                    self.set_indexed_sp['ConfigOfSurface'][fc] = [az[0], ti]
+                self.set_indexed_sp['SurfaceOfHouse'][b] = np.append(
+                    self.set_indexed_sp['SurfaceOfHouse'][b],
                     df_facades['Facades_ID'].values)
                 index = pd.MultiIndex.from_tuples([(b, f) for f in facades])
-                df = pd.DataFrame(df_facades['AREA'].values, index=index, columns=['HouseSurfaceArea'])  # Pq attribuer ici HouseSurfaceArea comme l'aire des facades?
+                df = pd.DataFrame(df_facades['AREA'].values, index=index,
+                                  columns=['HouseSurfaceArea'])  # Pq attribuer ici HouseSurfaceArea comme l'aire des facades?
                 self.parameters_to_ampl['HouseSurfaceArea'] = pd.concat(
                     [self.parameters_to_ampl['HouseSurfaceArea'], df])
                 # self.parameters_to_ampl['HouseSurfaceArea'].sort_index(inplace = True)
 
             if not df_limit_angle.empty:
                 # self.parameters_to_ampl['Limiting_angle_shadow'] = df_limit_angle.rename(columns={0:'Limiting_angle_shadow'})
                 self.parameters_to_ampl['Limiting_angle_shadow'] = df_limit_angle
-                self.set_indexed_compact['SurfaceOfType']['Facades'] = np_facades
-                self.set_indexed_compact['Surface'] = np.append(self.set_indexed_compact['Surface'], np_facades)
+                self.set_indexed_sp['SurfaceOfType']['Facades'] = np_facades
+                self.set_indexed_sp['Surface'] = np.append(self.set_indexed_sp['Surface'], np_facades)
 
     def send_parameters_and_sets_to_ampl(self, ampl):
         # -----------------------------------------------------------------------------------------------------#
         # Load data to AMPLPY depending on their type
         # -----------------------------------------------------------------------------------------------------#
 
-        for key in self.parameters_compact:
-            self.parameters_to_ampl[key] = self.parameters_compact[key]
+        for key in self.parameters_sp:
+            self.parameters_to_ampl[key] = self.parameters_sp[key]
 
         # set new indexed sets
-        for s in self.set_indexed_compact:
-            if isinstance(self.set_indexed_compact[s], np.ndarray):
-                ampl.getSet(str(s)).setValues(self.set_indexed_compact[s])
-            elif isinstance(self.set_indexed_compact[s], dict):
+        for s in self.set_indexed_sp:
+            if isinstance(self.set_indexed_sp[s], np.ndarray):
+                ampl.getSet(str(s)).setValues(self.set_indexed_sp[s])
+            elif isinstance(self.set_indexed_sp[s], dict):
                 for i, instance in ampl.getSet(str(s)):
                     try:
-                        instance.setValues(self.set_indexed_compact[s][i])
+                        instance.setValues(self.set_indexed_sp[s][i])
                     except ValueError:
-                        instance.setValues([self.set_indexed_compact[s][i]])
+                        instance.setValues([self.set_indexed_sp[s][i]])
             else:
                 raise ValueError('Type Error setting AMPLPY Set', s)
 
         # set new input Parameter
         for i in self.parameters_to_ampl:
 
             if isinstance(self.parameters_to_ampl[i], np.ndarray):
                 Para = ampl.getParameter(i)
-                # print('Set Values for ' + str(Para))
                 Para.setValues(self.parameters_to_ampl[i])
 
             elif isinstance(self.parameters_to_ampl[i], list):
                 Para = ampl.getParameter(i)
-                # print('Set Values for ' + str(Para))
                 Para.setValues(np.array(self.parameters_to_ampl[i]))
 
             elif isinstance(self.parameters_to_ampl[i], pd.DataFrame):
-                # print(self.parameters_to_ampl[i].columns)
                 ampl.setData(self.parameters_to_ampl[i])
 
             elif isinstance(self.parameters_to_ampl[i], pd.Series):
-                # print('Set values for : '+ i)
                 self.parameters_to_ampl[i].name = i
                 df = pd.DataFrame(self.parameters_to_ampl[i])
                 ampl.setData(df)
 
             elif isinstance(self.parameters_to_ampl[i], dict):
-                # print('Set Values for ' + str(i))
                 Para = ampl.getParameter(i)
-                # print('Set Values for ' + str(Para))
                 Para.setValues(self.parameters_to_ampl[i])
 
             elif isinstance(self.parameters_to_ampl[i], float):
                 Para = ampl.getParameter(i)
-                # print('Set Values for ' + str(Para))
                 Para.setValues([self.parameters_to_ampl[i]])
 
             elif isinstance(self.parameters_to_ampl[i], int):
                 Para = ampl.getParameter(i)
-                # print('Set Values for ' + str(Para))
                 Para.setValues([self.parameters_to_ampl[i]])
 
             else:
                 raise ValueError('Type Error setting AMPLPY Parameter', i)
 
         # TODO remove data_stream.dat
         ampl.readData('data_stream.dat')
-        if self.method_compact['use_Storage_Interperiod']:
+        if self.method_sp['use_Storage_Interperiod']:
             ampl.readData('data_stream_storage.dat')
 
         return ampl
 
     def set_scenario(self, ampl):
 
         # Set objective function
         for objective_name, objective_formulation in ampl.getObjectives():
             objective_formulation.drop()
 
-        if 'Objective' in self.scenario_compact:
+        if 'Objective' in self.scenario_sp:
             try:
-                ampl.getObjective(self.scenario_compact['Objective']).restore()
+                ampl.getObjective(self.scenario_sp['Objective']).restore()
             except KeyError:
                 ampl.getObjective('TOTEX').restore()
-                print('Objective function "', self.scenario_compact['Objective'],
-                      '" was not found in ampl model, TOTEX minimization was set instead.')
+                logging.warning('Objective function "' + str(self.scenario_sp['Objective']) +
+                                '" was not found in ampl model, TOTEX minimization was set instead.')
         else:
             ampl.getObjective('TOTEX').restore()
-            print('No objective function was found in scenario dictionary, TOTEX minimization was set instead.')
+            logging.warning('No objective function was found in scenario dictionary, TOTEX minimization was set instead.')
 
         # Set epsilon constraints
         ampl.getConstraint('EMOO_CAPEX_constraint').drop()
         ampl.getConstraint('EMOO_OPEX_constraint').drop()
         ampl.getConstraint('EMOO_TOTEX_constraint').drop()
         ampl.getConstraint('EMOO_GWP_constraint').drop()
         ampl.getConstraint('EMOO_lca_constraint').drop()
 
         ampl.getConstraint('EMOO_GU_demand_constraint').drop()
         ampl.getConstraint('EMOO_GU_supply_constraint').drop()
         ampl.getConstraint('EMOO_grid_constraint').drop()
         ampl.getConstraint('EMOO_network_constraint').drop()
 
-        if 'EMOO' in self.scenario_compact:
-            for epsilon_constraint in self.scenario_compact['EMOO']:
+        if 'EMOO' in self.scenario_sp:
+            for epsilon_constraint in self.scenario_sp['EMOO']:
                 try:
                     ampl.getConstraint(epsilon_constraint + '_constraint').restore()
-                    if isinstance(self.scenario_compact['EMOO'][epsilon_constraint], dict):
+                    if isinstance(self.scenario_sp['EMOO'][epsilon_constraint], dict):
                         epsilon_parameter = ampl.getParameter(epsilon_constraint)
-                        epsilon_parameter.setValues(self.scenario_compact['EMOO'][epsilon_constraint])
+                        epsilon_parameter.setValues(self.scenario_sp['EMOO'][epsilon_constraint])
                     else:
                         epsilon_parameter = ampl.getParameter(epsilon_constraint)
-                        epsilon_parameter.setValues([self.scenario_compact['EMOO'][epsilon_constraint]])
+                        epsilon_parameter.setValues([self.scenario_sp['EMOO'][epsilon_constraint]])
                 except:
-                    print('EMOO constraint ', epsilon_constraint, ' was not found in ampl model and was thus ignored.')
+                    logging.warning('EMOO constraint ' + str(epsilon_constraint) + ' was not found in ampl model and was thus ignored.')
 
         # Set specific constraints
         ampl.getConstraint('disallow_exchanges_1').drop()
         ampl.getConstraint('disallow_exchanges_2').drop()
         ampl.getConstraint('no_ElectricalHeater_without_HP').drop()
 
-        if 'PV' in self.infrastructure_compact.UnitsOfType:
+        if 'PV' in self.infrastructure_sp.UnitsOfType:
             ampl.getConstraint('enforce_PV_max').drop()
-        if 'HeatPump' in self.infrastructure_compact.UnitsOfType:
+        if 'HeatPump' in self.infrastructure_sp.UnitsOfType:
             ampl.getConstraint('enforce_DHN').drop()
-            if not any("DHN" in unit for unit in self.infrastructure_compact.UnitsOfType['HeatPump']):
+            if not any("DHN" in unit for unit in self.infrastructure_sp.UnitsOfType['HeatPump']):
                 ampl.getConstraint('DHN_heat').drop()
-        if 'Air_Conditioner' in self.infrastructure_compact.UnitsOfType and "Air_Conditioner_DHN" not in [unit["name"] for unit in self.infrastructure_compact.units]:
+        if 'Air_Conditioner' in self.infrastructure_sp.UnitsOfType and "Air_Conditioner_DHN" not in [unit["name"] for unit in self.infrastructure_sp.units]:
             ampl.getConstraint('AC_c3').drop()
-        if 'EV' in self.infrastructure_compact.UnitTypes:
+        if 'EV' in self.infrastructure_sp.UnitTypes:
             ampl.getConstraint('unidirectional_service').drop()
 
-        if self.method_compact['use_pv_orientation']:
+        if self.method_sp['use_pv_orientation']:
             ampl.getConstraint('enforce_PV_max_fac').drop()
-            if not self.method_compact['use_facades']:
+            if not self.method_sp['use_facades']:
                 ampl.getConstraint('limits_maximal_PV_to_fac').drop()
 
-        if 'specific' in self.scenario_compact:
-            for specific_constraint in self.scenario_compact['specific']:
+        if 'specific' in self.scenario_sp:
+            for specific_constraint in self.scenario_sp['specific']:
                 try:
                     ampl.getConstraint(specific_constraint).restore()
                 except:
-                    print('Specific constraint "', specific_constraint,
-                          '" was not found in ampl model and was thus ignored.')
+                    logging.warning('Specific constraint "' + str(specific_constraint) + '" was not found in ampl model and was thus ignored.')
 
         return ampl
 
+    def solve_model(self):
+        ampl = self.build_model_without_solving()
+
+        debugging = False
+        if debugging:
+            # ampl.exportData('loaded_data.dat')
+            # ampl.expotModel('loaded_model.mod')
+            ampl.eval('suffix iis symbolic OUT;')
+            ampl.setOption('presolve', 1)
+
+        # ampl evaluation to speed up the optimization in case we have cogeneration units (since it has many integer variables)
+        # ampl.eval("suffix priority IN, integer, >= 0, <= 9999; let {u in Units} Units_Use[u].priority := 9999; "
+        #          "let {u in UnitsOfType['NG_Cogeneration'],p in Period,t in Time[p]} Units_Use_t[u,p,t].priority := "
+        #          "200*round(max{i in Period,j in Time[i]}(T_ext[i,j])-T_ext[p,t],0);")
+        ampl.solve()
+
+        if debugging:
+            ampl.eval('display {i in 1.._ncons: _con[i].iis <> "0"} (_conname[i], _con[i].iis);')
+            ampl.eval('for {i in 1.._ncons: _con[i].iis <> "0"} expand _con[i]; ')
+            ampl.eval('display{j in 1.._nvars: _var[j].iis <> "0"}(_varname[j], _var[j].iis);')
+
+        exitcode = exitcode_from_ampl(ampl)
+        return ampl, exitcode
+
 
 def initialize_default_methods(method):
     if method is None:
         method = {}
 
     if 'use_facades' not in method:
         method['use_facades'] = False
     if 'use_pv_orientation' not in method:
         method['use_pv_orientation'] = False
 
-    if 'include_stochasticity' not in method:  # https://ipese-web.epfl.ch/lepour/lacorte_pds/index.html
+    if 'include_stochasticity' not in method:
         method['include_stochasticity'] = False
     if 'sd_stochasticity' not in method:
         method['sd_stochasticity'] = [0.1, 1]
 
     if 'building-scale' not in method:
         method['building-scale'] = False
     if 'district-scale' not in method:
@@ -709,34 +704,41 @@
     if 'use_dynamic_emission_profiles' not in method:
         method['use_dynamic_emission_profiles'] = False
     if 'use_custom_profiles' not in method:
         method['use_custom_profiles'] = False
 
     if 'include_all_solutions' not in method:
         method['include_all_solutions'] = False
-    if 'save_stream_t' not in method:
-        method['save_stream_t'] = False
+    if 'save_data_input' not in method:
+        method['save_data_input'] = True
+    if 'save_timeseries' not in method:
+        method['save_timeseries'] = True
+    if 'save_streams' not in method:
+        method['save_streams'] = False
     if 'save_lca' not in method:
         method['save_lca'] = False
     if 'extract_parameters' not in method:
         method['extract_parameters'] = False
+    if 'print_logs' not in method:
+        method['print_logs'] = True
 
-    if 'actors_cost' not in method:
-        method['actors_cost'] = False
-    if method['actors_cost']:
+    if 'actors_problem' not in method:
+        method['actors_problem'] = False
+    if method['actors_problem']:
         method["include_all_solutions"] = True
     if 'DHN_CO2' not in method:
         method['DHN_CO2'] = False
 
     if 'use_Storage_Interperiod' not in method:
         method['use_Storage_Interperiod'] = False
 
     if method['building-scale']:
-        method['include_all_solutions'] = False # avoid interactions between optimization scenarios
-        method['district-scale'] = True  # building-scale approach is also using the decomposition algorithm, but with only 1 MP optimization (DW_params['max_iter'] = 1)
+        method['include_all_solutions'] = False  # avoid interactions between optimization scenarios
+        method[
+            'district-scale'] = True  # building-scale approach is also using the decomposition algorithm, but with only 1 MP optimization (DW_params['max_iter'] = 1)
 
     return method
 
 
 def exitcode_from_ampl(ampl):
     solve_result = ampl.getData('solve_result').toList()[0]
     return 0 if solve_result == 'solved' else solve_result
```

### Comparing `REHO-1.0.2/reho/model/district_decomposition.py` & `reho-1.1.0/reho/model/master_problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-import reho.model.infrastructure as infrastructure
-from reho.model.compact_optimization import *
-import reho.model.postprocessing.write_results as WR
-from itertools import groupby
-import warnings
-import time
 import gc
+import time
+import warnings
+from itertools import groupby
+
+import coloredlogs
 import pandas as pd
 
+import reho.model.infrastructure as infrastructure
+import reho.model.postprocessing.write_results as write_results
+from reho.model.preprocessing.local_data import *
+from reho.model.sub_problem import *
+
 
-class district_decomposition:
+__doc__ = """
+File for handling data and optimization for an AMPL master problem.
+"""
+
+
+class MasterProblem:
     """
     Applies the decomposition method.
 
-    Store district attributes, scenario, method, attributes for the decomposition, and initiate an attribute
+    Stores district attributes, scenario, method, attributes for the decomposition, and initiate an attribute
     that will store results.
 
     Parameters
     ----------
     qbuildings_data : dict
         Contains 3 layers: A dictionary of the buildings characteristics such as surface area, class, egid, a DataFrame for Roofs characteristics and a DataFrame for Facades characteristics.
     units : dict
@@ -25,58 +34,77 @@
         Grids characteristics.
     parameters : dict, optional
         Parameters set in the script (usually energy tariffs).
     set_indexed : dict, optional
         The indexes used in the model.
     cluster : dict, optional
         Define location district, number of periods, and number of timesteps.
+        To use your own weather file, you can add a key ``custom_weather`` with the corresponding path.
     method : dict, optional
         The different methods to run the optimization (refer to :ref:`tbl-methods`).
     solver : str, optional
         Chosen solver for AMPL (gurobi, cplex, highs, cbc, etc.).
     DW_params : dict, optional
         Hyperparameters of the decomposition and other useful information.
 
     Notes
     -----
     - The REHO class inherits this class, so the inputs are similar.
-    - ``qbuildings_data`` contains by default only the buildings data. The roofs and facades are added solely with the use of methods: *use_pv_orientation* and *use_facades*.
+    - ``qbuildings_data`` contains by default only the buildings' data. The roofs and facades are added solely with the use of methods: *use_pv_orientation* and *use_facades*.
     """
 
     def __init__(self, qbuildings_data, units, grids, parameters=None, set_indexed=None,
                  cluster=None, method=None, solver=None, DW_params=None):
 
         # ampl solver
         self.solver = solver
 
         # methods
         self.method = initialize_default_methods(method)
+        self.logger = logging.getLogger(__name__)
+        if method['print_logs']:
+            coloredlogs.install(level=logging.INFO, logger=self.logger, isatty=True,
+                                fmt="%(message)s", stream=sys.stdout)
 
-        # District attributes / used also in REHO
+        # infrastructure
         if method['use_facades'] or method['use_pv_orientation']:
             self.qbuildings_data = qbuildings_data
         self.buildings_data = qbuildings_data['buildings_data']
         self.ERA = sum([self.buildings_data[house]['ERA'] for house in self.buildings_data.keys()])
-        self.infrastructure = infrastructure.infrastructure(qbuildings_data, units, grids)
+
+        self.infrastructure = infrastructure.Infrastructure(qbuildings_data, units, grids)
+        self.infrastructure_SP = dict()
+        self.build_infrastructure_SP()
 
         if cluster is None:
-            self.cluster = {'Location': 'Geneva', 'Attributes': ['I', 'T', 'W'], 'Periods': 10, 'PeriodDuration': 24}
+            self.cluster = {'Location': 'Geneva', 'Attributes': ['T', 'I', 'W'], 'Periods': 10, 'PeriodDuration': 24}
         else:
             self.cluster = cluster
-        self.File_ID = WD.get_cluster_file_ID(self.cluster)
+
+        # load SIA norms
+        sia_data = dict()
+        sia_data["df_SIA_380"] = pd.read_csv(path_to_sia_equivalence, sep=';', index_col=[0], header=[0])
+        sia_data["df_SIA_2024"] = pd.read_excel(path_to_sia_norms, sheet_name=['profiles', 'calculs', 'data'],
+                                                engine='openpyxl', index_col=[0], skiprows=[0, 2, 3, 4], header=[0])
+
+        # retrieve location data
+        self.local_data = return_local_data(cluster, qbuildings_data)
 
         if parameters is None:
             self.parameters = {}
         else:
             self.parameters = parameters
 
-        # Heat gains from electricity and people, domestic hot water demand, domestic electricity demand
+        # build end use demands profile
         self.parameters['HeatGains'], self.parameters['DHW_flowrate'], self.parameters['Domestic_electricity'] = \
-            DGF.build_eud_profiles(self.buildings_data, self.File_ID, self.cluster, self.method['include_stochasticity'],
-                                   self.method['sd_stochasticity'], self.method['use_custom_profiles'])
+            buildings_profiles.eud_profiles(self.buildings_data, self.cluster, sia_data["df_SIA_380"], sia_data["df_SIA_2024"], self.local_data["df_Timestamp"],
+                                            self.method['include_stochasticity'], self.method['sd_stochasticity'], self.method['use_custom_profiles'])
+
+        # build solar gains profile
+        self.parameters['SolarGains'] = buildings_profiles.solar_gains_profile(self.buildings_data, sia_data, self.local_data)
 
         if set_indexed is None:
             self.set_indexed = {}
         else:
             self.set_indexed = set_indexed
 
         # attributes for the decomposition algorithm
@@ -91,22 +119,21 @@
                                                 "area_district", "velocity", "density", "delta_enthalpy", "cinv1_dhn", "cinv2_dhn"],
                          "list_constraints_MP": []
                          }
 
         self.df_fix_Units = pd.DataFrame()
         self.fix_units_list = []
 
-
     def initialize_optimization_tracking_attributes(self):
         # internal IT parameter
         self.pool = None
         self.iter = 0  # keeps track of iterations, takes value of last iteration circle
         self.feasible_solutions = 0  # keeps track how many sets of SP solutions are proposed to the MP eg '2' means two per building
         list_obj = list(self.infrastructure.lca_kpis) + ["TOTEX", "CAPEX", "OPEX", "GWP"]
-        self.flags = {obj: 0 for obj in list_obj} # keep track if the initialization has already been done
+        self.flags = {obj: 0 for obj in list_obj}  # keep track if the initialization has already been done
 
         # output attributes
         self.stopping_criteria = pd.DataFrame()
 
         # result attributes
         self.number_SP_solutions = pd.DataFrame()  # records number of solutions per iteration circle
         self.number_MP_solutions = pd.DataFrame()  # records number of solutions per iteration circle
@@ -125,136 +152,138 @@
         return self_dict
 
     def __setstate__(self, state):
         self.__dict__.update(state)
 
     def select_SP_obj_decomposition(self, scenario):
         """
-        Description
-        -----------
-        the SPs in decomposition have another objective than in the compact formulation because their
-        objective function is formulated as a reduced cost
+        The SPs in decomposition have another objective than in the compact formulation because their objective function is formulated as a reduced cost.
         Also adding global linking constraints, like Epsilon, changes the scenario to choose.
-        3: min OPEX,epsilon_CAPEX -> 12
-        8: min CAPEx, epsilon_OPEX -> 13
-        10: min OPEX,epsilon_CAPEX -> 14
-        11: min CAPEx, epsilon_OPEX -> 15
-        for CAPEX (1), OPEX (2), TOTEX (4) and CO2 emissions (9) the same objective is taken
 
-        Inputs
+        Parameters
         ------
-        scenario: dictionary, objective function
+        scenario : dictionary
+            objective function
 
-        Outputs
+        Returns
         -------
-        SP_scenario: dictionary, scenario for the SP (iterations)
-        SP_scenario_init: dictionary, scenario for the SP (initiation)
+        SP_scenario : dictionary
+            scenario for the SP (iterations)
+        SP_scenario_init : dictionary
+            scenario for the SP (initiation)
 
         """
         SP_scenario = scenario.copy()
-        SP_scenario['EMOO'] = scenario['EMOO'].copy()
+        SP_scenario['EMOO'] = {}
         SP_scenario['specific'] = scenario['specific'].copy()
 
         SP_scenario_init = scenario.copy()
         SP_scenario_init['EMOO'] = scenario['EMOO'].copy()
         SP_scenario_init['specific'] = scenario['specific'].copy()
 
         # use GM or GU only for initialization. Then pi dictates when to restrict power exchanges
         SP_scenario_init['EMOO']['EMOO_grid'] = SP_scenario_init['EMOO']['EMOO_grid'] * 0.999
-        SP_scenario['EMOO']['EMOO_grid'] = 0.0
 
         if "TransformerCapacity" in self.parameters:
             nb_buildings = round(self.parameters["Domestic_electricity"].shape[0] / self.DW_params['timesteps'])
             profile_building_x = self.parameters["Domestic_electricity"].reshape(nb_buildings, self.DW_params['timesteps'])
             max_DEL = profile_building_x.max(axis=1).sum()
-            SP_scenario_init['EMOO']['EMOO_GU_demand'] = self.parameters["TransformerCapacity"][0] * 0.999/max_DEL
-            SP_scenario_init['EMOO']['EMOO_GU_supply'] = self.parameters["TransformerCapacity"][0] * 0.999/max_DEL
+            SP_scenario_init['EMOO']['EMOO_GU_demand'] = self.parameters["TransformerCapacity"][0] * 0.999 / max_DEL
+            SP_scenario_init['EMOO']['EMOO_GU_supply'] = self.parameters["TransformerCapacity"][0] * 0.999 / max_DEL
 
         for scenario_cst in scenario['specific']:
             if scenario_cst in self.lists_MP['list_constraints_MP']:
                 SP_scenario['specific'].remove(scenario_cst)
                 SP_scenario_init['specific'].remove(scenario_cst)
 
         return scenario, SP_scenario, SP_scenario_init
 
     def initiate_decomposition(self, scenario, Scn_ID=0, Pareto_ID=1, epsilon_init=None):
         """
-        Description
-        -----------
         The SPs are initialized for the given objective.
         In case the optimization includes an epsilon constraint, there are two ways to initialize.
         Either the epsilon constraint is applied on the SPs, or the initialization is done with beta.
         The former has the risk to be infeasible for certain SPs, therefore the latter is preferred.
         Three beta values are given to mark the extreme points and an average point.
-        Set up the parallel optimization if needed
+        Sets up the parallel optimization if needed
 
-        Inputs
-        ------
-        scenario : dictionary, Which objective function to optimize and the value of epsilon constraints to apply
-        Scn_ID : int, ID of the optimization scenario
-        Pareto_ID : int,  Id of the pareto point. For single objective optimization it is 1 by default
-        epsilon_init : array, Epsilon constraints to apply for the initialization
+        Parameters
+        ----------
+        scenario : dictionary
+            Which objective function to optimize and the value of epsilon constraints to apply
+        Scn_ID : int
+            ID of the optimization scenario
+        Pareto_ID : int
+            Id of the pareto point. For single objective optimization it is 1 by default
+        epsilon_init : array
+            Epsilon constraints to apply for the initialization
         """
         # check if TOTEX, OPEX or multi-objective optimization -> init with beta
         if self.method['building-scale']:
             init_beta = [None]  # keep same objective function
         elif not self.method['include_all_solutions'] or self.flags[scenario['Objective']] == 0 or scenario['EMOO']['EMOO_grid'] != 0:
             self.flags[scenario['Objective']] = 1  # never been optimized with this objective previously
             init_beta = [1000.0, 10, 1, 0.1, 0.001]
         else:
             init_beta = []  # skip the initialization
 
-        for beta in init_beta: # execute SP for MP initialization
+        for beta in init_beta:  # execute SP for MP initialization
             if self.method['parallel_computation']:
 
                 # to run multiprocesses, a copy of the model is performed with pickles -> make sure there are no ampl libraries
-                results = {h: self.pool.apply_async(self.SP_initiation_execution, args=(scenario, Scn_ID, Pareto_ID, h, epsilon_init, beta)) for h in self.infrastructure.houses}
+                results = {h: self.pool.apply_async(self.SP_initiation_execution, args=(scenario, Scn_ID, Pareto_ID, h, epsilon_init, beta)) for h in
+                           self.infrastructure.houses}
 
                 # sometimes, python goes to fast and extract the results before calculating them. This step makes python wait finishing the calculations
                 while len(results[list(self.buildings_data.keys())[-1]].get()) != 2:
                     time.sleep(1)
 
                 # the memory to write and share results is not parallel -> results have to be stored outside calculation
                 for h in self.infrastructure.houses:
                     (df_Results, attr) = results[h].get()
                     self.add_df_Results_SP(Scn_ID, Pareto_ID, self.iter, h, df_Results, attr)
-
             else:
                 for id, h in enumerate(self.infrastructure.houses):
                     df_Results, attr = self.SP_initiation_execution(scenario, Scn_ID=Scn_ID, Pareto_ID=Pareto_ID, h=h, epsilon_init=epsilon_init, beta=beta)
                     self.add_df_Results_SP(Scn_ID, Pareto_ID, self.iter, h, df_Results, attr)
 
             self.feasible_solutions += 1  # after each 'round' of SP execution the number of feasible solutions increase
         return
 
     def SP_initiation_execution(self, scenario, Scn_ID=0, Pareto_ID=1, h=None, epsilon_init=None, beta=None):
         """
-        Description
-        -----------
-        Adapt the model depending on the method, execute the optimization and get the results
+        Adapts the model depending on the method, execute the optimization and get the results
 
-        Inputs
-        ------
-        scenario : dictionary, Which objective function to optimize and the value of epsilon constraints to apply
-        Scn_ID : int, scenario ID
-        Pareto_ID : int, Id of the pareto point. For single objective optimization it is 1 by default
-        h : string,House id
-        epsilon_init : float, Epsilon constraint to apply for the initialization
-        beta : float, Beta initial value used for initialization
+        Parameters
+        ----------
+        scenario : dictionary
+            Which objective function to optimize and the value of epsilon constraints to apply
+        Scn_ID : int
+            scenario ID
+        Pareto_ID : int
+            Id of the pareto point. For single objective optimization it is 0 by default.
+        h : string
+            House id
+        epsilon_init : float
+            Epsilon constraint to apply for the initialization
+        beta : float
+            Beta initial value used for initialization
 
-        Outputs
+        Returns
         -------
-        df_Results : results of the optimization (unit installed, power exchanged, costs, GWP emissions, ...)
-        attr : results of the optimization process (CPU time, objective value, nb variables or constraints, ...)
+        df_Results :
+            results of the optimization (unit installed, power exchanged, costs, GWP emissions, ...)
+        attr :
+            results of the optimization process (CPU time, objective value, nb variables or constraints, ...)
         """
-
-        print('INITIATE HOUSE: ', h)
+        if self.method["print_logs"]:
+            print('INITIATE HOUSE: ' + h)
 
         # find district structure and parameter for one single building
-        buildings_data_SP, parameters_SP, infrastructure_SP = self.__split_parameter_sets_per_building(h)
+        buildings_data_SP, parameters_SP = self.split_parameter_sets_per_building(h)
 
         # epsilon constraints on districts may lead to infeasibilities on building level -> apply them in MP only
         if epsilon_init is not None and self.method['building-scale']:
             emoo = scenario["EMOO"].copy()
             emoo.pop("EMOO_grid")
             if len(emoo) == 1:
                 if 'EMOO_lca' in emoo:
@@ -264,103 +293,108 @@
             else:
                 raise warnings.warn("Multiple epsilon constraints")
         elif not self.method['building-scale']:
             scenario, beta_list = self.get_beta_values(scenario, beta)
             parameters_SP['beta_duals'] = beta_list
 
         if self.method['use_facades'] or self.method['use_pv_orientation']:
-            REHO = compact_optimization(infrastructure_SP, buildings_data_SP, parameters_SP, self.set_indexed, self.cluster, scenario, self.method, self.solver, self.qbuildings_data)
+            REHO = SubProblem(self.infrastructure_SP[h], buildings_data_SP, self.local_data, parameters_SP, self.set_indexed, self.cluster, scenario,
+                              self.method, self.solver, self.qbuildings_data)
         else:
-            REHO = compact_optimization(infrastructure_SP, buildings_data_SP, parameters_SP, self.set_indexed, self.cluster, scenario, self.method, self.solver)
+            REHO = SubProblem(self.infrastructure_SP[h], buildings_data_SP, self.local_data, parameters_SP, self.set_indexed, self.cluster, scenario,
+                              self.method, self.solver)
         ampl = REHO.build_model_without_solving()
 
         if self.method['fix_units']:
             for unit in self.fix_units_list:
                 if unit == 'PV':
                     ampl.getVariable('Units_Mult').get('PV_' + h).fix(self.df_fix_Units.Units_Mult.loc['PV_' + h] * 0.999)
                     ampl.getVariable('Units_Use').get('PV_' + h).fix(float(self.df_fix_Units.Units_Use.loc['PV_' + h]))
                 else:
-                    ampl.getVariable('Units_Mult').get(unit + '_' + h).fix( self.df_fix_Units.Units_Mult.loc[unit + '_' + h])
-                    ampl.getVariable('Units_Use').get(unit + '_' + h).fix( float(self.df_fix_Units.Units_Use.loc[unit + '_' + h]))
+                    ampl.getVariable('Units_Mult').get(unit + '_' + h).fix(self.df_fix_Units.Units_Mult.loc[unit + '_' + h])
+                    ampl.getVariable('Units_Use').get(unit + '_' + h).fix(float(self.df_fix_Units.Units_Use.loc[unit + '_' + h]))
 
         ampl.solve()
         exitcode = exitcode_from_ampl(ampl)
 
-        df_Results = WR.get_df_Results_from_SP(ampl, scenario, self.method, self.buildings_data)
+        df_Results = write_results.get_df_Results_from_SP(ampl, scenario, self.method, self.buildings_data)
         attr = self.get_solver_attributes(Scn_ID, Pareto_ID, ampl)
 
         del ampl
         gc.collect()  # free memory
         if exitcode != 0:
             # It might be that the solution is optimal with unscaled infeasibilities. So we check if we really found a solution (via its cost value)
             if exitcode != 'solved?' or df_Results["df_Performance"]['Costs_op'][0] + df_Results["df_Performance"]['Costs_inv'][0] == 0:
                 raise Exception('Sub problem did not converge')
 
         return df_Results, attr
 
     def MP_iteration(self, scenario, binary, Scn_ID=0, Pareto_ID=1, read_DHN=False):
         """
-        Description
-        -----------
-        Run the optimisation of the Master Problem (MP):
-        - Create the ampl_MP master problem
-        - Set the sets and the parameters in ampl
-        - Actualise the grid exchanges and the costs of each sub problem (house) without the grid costs
-        - Run the optimisation
-        - Extract the results (lambda, dual variables pi and mu, objective value of the MP (TOTEX, grid exchanges, ...)
-        - Delete the ampl_MP model
 
-        Inputs
-        ------
-        scenario: dictionary
-        binary: bool, if the decision variable 'lambda' is binary or continuous
-        Scn_ID: scenario ID
-        Pareto_ID: int, pareto ID
+        Runs the optimization of the Master Problem (MP):
+
+        - Creates the ampl_MP master problem
+        - Sets the sets and the parameters in ampl
+        - Actualises the grid exchanges and the costs of each sub problem (house) without the grid costs
+        - Runs the optimization
+        - Extracts the results (lambda, dual variables pi and mu, objective value of the MP (TOTEX, grid exchanges, ...)
+        - Deletes the ampl_MP model
+
+        Parameters
+        -----------
+        scenario : dictionary
+        binary : boolean
+            if the decision variable 'lambda' is binary or continuous
+        Scn_ID : int
+        Pareto_ID: int
+        read_DHN : bool
 
         Raises
         ------
-        ValueError: If the sets are not arrays or if the parameters are not arrays or floats or dataframes.
-        If the MP optimization did not converge
+        ValueError: If the sets are not arrays or if the parameters are not arrays or floats or dataframes. Or if the MP optimization did not converge
         """
 
-        ### Create the ampl Master Problem (MP)
+        # Create the ampl Master Problem (MP)
         if os.getenv('USE_AMPL_MODULES', False):
             from amplpy import modules
             modules.load()
             ampl_MP = AMPL()
         else:
             try:
                 ampl_MP = AMPL(Environment(os.environ["AMPL_PATH"]))
             except:
                 raise Exception("AMPL_PATH is not defined. Please include a .env file at the project root (e.g., AMPL_PATH='C:/AMPL')")
 
         # AMPL (GNU) OPTIONS
-        ampl_MP.setOption('show_stats', 2)
         ampl_MP.setOption('solution_round', 11)
         ampl_MP.setOption('rel_boundtol', 1e-12)
         ampl_MP.setOption('presolve_eps', 1e-4)  # -ignore difference between upper and lower bound by this tolerance
         ampl_MP.setOption('presolve_inteps', 1e-6)  # -tolerance added/substracted to each upper/lower bound
         ampl_MP.setOption('presolve_fixeps', 1e-9)
-        ampl_MP.setOption('show_stats', 1)
+        if not self.method['print_logs']:
+            ampl_MP.setOption('show_stats', 0)
+            ampl_MP.setOption('solver_msg', 0)
 
         # -SOLVER OPTIONS
         ampl_MP.setOption('solver', self.solver)
         if self.solver == "gurobi":
             ampl_MP.eval("option gurobi_options 'NodeFileStart=0.5';")
         if self.solver == "cplex":
             ampl_MP.eval("option cplex_options 'bestbound mipgap=5e-7 integrality=1e-09 timing=1 timelimit=120';")
 
         ampl_MP.eval('option show_boundtol 0;')
         ampl_MP.eval('option abs_boundtol 1e-10;')
 
         # Load Master Problem (MP) Formulation
         ampl_MP.cd(path_to_ampl_model)
         ampl_MP.read('master_problem.mod')
-        if self.method["actors_cost"]:
-            ampl_MP.read('master_problem_actors.mod')
+
+        if self.method["actors_problem"]:
+            ampl_MP.read('actors_problem.mod')
 
         if len(self.infrastructure.UnitsOfDistrict) > 0:
             ampl_MP.cd(path_to_district_units)
             if "EV_district" in self.infrastructure.UnitsOfDistrict:
                 ampl_MP.read('evehicle.mod')
                 self.lists_MP["list_constraints_MP"] = self.lists_MP["list_constraints_MP"] + ['unidirectional_service', 'unidirectional_service2']
             if "NG_Boiler_district" in self.infrastructure.UnitsOfDistrict:
@@ -374,73 +408,77 @@
         ampl_MP.read('battery.mod')
 
         if read_DHN:
             ampl_MP.cd(path_to_units)
             ampl_MP.read('DHN.mod')
 
         ampl_MP.cd(path_to_clustering)
-        ampl_MP.readData('frequency_' + self.File_ID + '.dat')
+        ampl_MP.readData('frequency_' + self.local_data['File_ID'] + '.dat')
         ampl_MP.cd(path_to_ampl_model)
 
         # -------------------------------------------------------------------------------------------------------------
         # Set Parameters, only bool to choose if including all solutions found also from other Pareto_IDs
         # ------------------------------------------------------------------------------------------------------------
         # collect data
         df_Performance = self.return_combined_SP_results(self.results_SP, 'df_Performance')
-        df_Performance = df_Performance.drop(index='Network', level='Hub').groupby(level=['Scn_ID', 'Pareto_ID', 'FeasibleSolution', 'Hub']).head(1).droplevel('Hub')  # select current Scn_ID and Pareto_ID
+        df_Performance = df_Performance.drop(index='Network', level='Hub').groupby(level=['Scn_ID', 'Pareto_ID', 'FeasibleSolution', 'Hub']).head(1).droplevel(
+            'Hub')  # select current Scn_ID and Pareto_ID
         df_Grid_t = np.round(self.return_combined_SP_results(self.results_SP, 'df_Grid_t'), 6)
 
         # prepare df to have the same index as AMPL model
         if not self.method['include_all_solutions']:
             df_Performance = df_Performance.xs((Scn_ID, Pareto_ID), level=('Scn_ID', 'Pareto_ID'))
-            df_Grid_t = df_Grid_t.xs((Scn_ID, Pareto_ID, 'Network'), level=('Scn_ID', 'Pareto_ID', 'Hub'))
+            df_Grid_t = df_Grid_t.xs((Scn_ID, Pareto_ID), level=('Scn_ID', 'Pareto_ID'))
         else:
             df_Performance = df_Performance.droplevel(['Scn_ID', 'Pareto_ID'])
-            df_Grid_t = df_Grid_t.droplevel(['Scn_ID', 'Pareto_ID']).xs('Network', level='Hub')
+            df_Grid_t = df_Grid_t.droplevel(['Scn_ID', 'Pareto_ID'])
 
         df_Performance = df_Performance.droplevel(level='Iter')
-        df_Grid_t = df_Grid_t.droplevel(level='Iter').reorder_levels(['Layer', 'FeasibleSolution', 'house', 'Period', 'Time'])
+        df_Grid_t = df_Grid_t.droplevel(level=['Iter', 'Hub']).reorder_levels(['Layer', 'FeasibleSolution', 'house', 'Period', 'Time'])
 
         # assign data
-        MP_parameters = {}
-        MP_parameters['Costs_inv_rep_SPs'] = df_Performance.Costs_inv + df_Performance.Costs_rep
-        MP_parameters['Costs_ft_SPs'] = pd.DataFrame(np.round(df_Performance.Costs_ft, 6)).set_axis(['Costs_ft_SPs'], axis=1)
-        MP_parameters['GWP_house_constr_SPs'] = pd.DataFrame(df_Performance.GWP_constr).set_axis(['GWP_house_constr_SPs'], axis=1)
+        MP_parameters = {'Costs_inv_rep_SPs': df_Performance.Costs_inv + df_Performance.Costs_rep,
+                         'Costs_ft_SPs': pd.DataFrame(np.round(df_Performance.Costs_ft, 6)).set_axis(['Costs_ft_SPs'], axis=1),
+                         'GWP_house_constr_SPs': pd.DataFrame(df_Performance.GWP_constr).set_axis(['GWP_house_constr_SPs'], axis=1)
+                         }
 
         if self.method['save_lca']:
             df_lca_Units = self.return_combined_SP_results(self.results_SP, 'df_lca_Units')
             df_lca_Units = df_lca_Units.groupby(level=['Scn_ID', 'Pareto_ID', 'FeasibleSolution', 'house']).sum()
             MP_parameters['lca_house_units_SPs'] = df_lca_Units.droplevel(["Scn_ID", "Pareto_ID"]).stack().swaplevel(1, 2)
             if not self.method['include_all_solutions']:
-                MP_parameters['lca_house_units_SPs'] = MP_parameters['lca_house_units_SPs'].xs(self.feasible_solutions - 1, level="FeasibleSolution", drop_level=False)
+                MP_parameters['lca_house_units_SPs'] = MP_parameters['lca_house_units_SPs'].xs(self.feasible_solutions - 1, level="FeasibleSolution",
+                                                                                               drop_level=False)
 
         MP_parameters['Grids_Parameters'] = self.infrastructure.Grids_Parameters
         MP_parameters['Grids_Parameters_lca'] = self.infrastructure.Grids_Parameters_lca
         MP_parameters['Units_flowrate'] = self.infrastructure.Units_flowrate.query('Unit.str.contains("district")')
         MP_parameters['Units_Parameters'] = self.infrastructure.Units_Parameters.query('index.str.contains("district")')
         MP_parameters['Units_Parameters_lca'] = self.infrastructure.Units_Parameters_lca.query('index.get_level_values("Units").str.contains("district")')
 
         if self.method['use_dynamic_emission_profiles']:
             ids = self.number_SP_solutions.iloc[-1]
             df = df_Grid_t[['GWP_supply']].xs("Electricity", level="Layer", drop_level=False)
             MP_parameters['GWP_supply'] = df.xs((ids["FeasibleSolution"], ids["House"]), level=("FeasibleSolution", "house"))
-
+            MP_parameters['GWP_demand'] = MP_parameters['GWP_supply'].rename(columns={"GWP_supply": "GWP_demand"}) * (1-1e-9)
 
         for key in self.lists_MP['list_parameters_MP']:
             if key in self.parameters.keys():
                 MP_parameters[key] = self.parameters[key]
 
         MP_parameters['df_grid'] = df_Grid_t[['Grid_demand', 'Grid_supply']]
         MP_parameters['ERA'] = np.asarray([self.buildings_data[house]['ERA'] for house in self.buildings_data.keys()])
         MP_parameters['Area_tot'] = self.ERA
 
         if 'EV_plugged_out' not in MP_parameters:
             if len(self.infrastructure.UnitsOfDistrict) != 0:
                 if 'EV_district' in self.infrastructure.UnitsOfDistrict:
-                    MP_parameters['EV_plugged_out'], MP_parameters['EV_plugging_in'] = EV_gen.generate_EV_plugged_out_profiles_district(self.cluster)
+                    MP_parameters['EV_plugged_out'], MP_parameters['EV_plugging_in'] = EV_gen.generate_EV_plugged_out_profiles_district(self.cluster,
+                                                                                                                                        self.local_data[
+                                                                                                                                            "df_Timestamp"])
 
         if read_DHN:
             if 'T_DHN_supply_cst' and 'T_DHN_return_cst' in self.parameters:
                 if not self.method["DHN_CO2"]:
                     dT = np.array(self.parameters["T_DHN_supply_cst"] - self.parameters["T_DHN_return_cst"])
                     MP_parameters['delta_enthalpy'] = dT.mean() * 4.18
                     MP_parameters['density'] = 1000
@@ -458,21 +496,21 @@
         MP_set_indexed = {}
         for sets in ['House', 'Layers', 'LayerTypes', 'LayersOfType', 'HousesOfLayer', 'Lca_kpi']:
             MP_set_indexed[sets] = self.infrastructure.Set[sets]
         MP_set_indexed['LayersOfType']['ResourceBalance'].sort()
 
         MP_set_indexed['UnitsOfLayer'] = dict()
         for layer in self.infrastructure.Set['UnitsOfLayer']:
-            lst =  self.infrastructure.Set['UnitsOfLayer'][layer]
+            lst = self.infrastructure.Set['UnitsOfLayer'][layer]
             MP_set_indexed['UnitsOfLayer'][layer] = np.array(list(filter(lambda k: 'district' in k, lst)))
 
         MP_set_indexed['FeasibleSolutions'] = df_Performance.index.unique('FeasibleSolution').to_numpy()  # index to array as set
 
-        if self.method['actors_cost']:
-            #MP_parameters['Costs_tot_actors_min'] = df_Performance[["Costs_op", "Costs_inv", "Costs_rep"]].sum(axis=1).groupby("house").min()
+        if self.method['actors_problem']:
+            # MP_parameters['Costs_tot_actors_min'] = df_Performance[["Costs_op", "Costs_inv", "Costs_rep"]].sum(axis=1).groupby("house").min()
             MP_set_indexed['ActorObjective'] = self.set_indexed["ActorObjective"]
 
             df_Unit_t = self.return_combined_SP_results(self.results_SP, 'df_Unit_t').xs("Electricity", level="Layer")
             df_PV_t = pd.DataFrame()
             for bui in self.infrastructure.houses:
                 dummy = df_Unit_t.xs("PV_" + bui, level="Unit")
                 df_PV_t = pd.concat([df_PV_t, dummy])
@@ -481,30 +519,30 @@
         if "Heat" in self.infrastructure.grids.keys():
             if 'T_DHN_supply_cst' and 'T_DHN_return_cst' in self.parameters:
                 T_DHN_mean = (self.parameters["T_DHN_supply_cst"] + self.parameters["T_DHN_return_cst"]) / 2
                 if "HeatPump_Geothermal_district" in self.infrastructure.UnitsOfDistrict:
                     MP_set_indexed["HP_Tsupply"] = np.array([T_DHN_mean.mean()])
                     MP_set_indexed["HP_Tsink"] = np.array([T_DHN_mean.mean()])
         if read_DHN:
-            MP_set_indexed["House_ID"] = np.array(range(0, len(self.infrastructure.houses)))+1
+            MP_set_indexed["House_ID"] = np.array(range(0, len(self.infrastructure.houses))) + 1
 
         # ---------------------------------------------------------------------------------------------------------------
         # CENTRAL UNITS
         # ---------------------------------------------------------------------------------------------------------------
         if len(self.infrastructure.district_units) > 0:
             MP_set_indexed['Units'] = np.array([])
             MP_set_indexed['UnitTypes'] = np.array([])
             MP_set_indexed['UnitsOfType'] = {}
             for u in self.infrastructure.district_units:
                 name = u['name']
                 MP_set_indexed['Units'] = np.append(MP_set_indexed['Units'], [name])
                 if not u['UnitOfType'] in MP_set_indexed['UnitTypes']:
                     MP_set_indexed['UnitTypes'] = np.append(MP_set_indexed['UnitTypes'], u['UnitOfType'])
                     MP_set_indexed['UnitsOfType'][u['UnitOfType']] = np.array([])
-                MP_set_indexed['UnitsOfType'][u['UnitOfType']] = np.append( MP_set_indexed['UnitsOfType'][u['UnitOfType']], [name])
+                MP_set_indexed['UnitsOfType'][u['UnitOfType']] = np.append(MP_set_indexed['UnitsOfType'][u['UnitOfType']], [name])
 
         # ---------------------------------------------------------------------------------------------------------------
         # give values to ampl
         # ---------------------------------------------------------------------------------------------------------------
 
         for s in MP_set_indexed:
             if isinstance(MP_set_indexed[s], np.ndarray):
@@ -540,16 +578,14 @@
             elif isinstance(MP_parameters[i], int):
                 Para = ampl_MP.getParameter(i)
                 Para.setValues([MP_parameters[i]])
 
             elif isinstance(MP_parameters[i], pd.DataFrame):
                 if not MP_parameters[i].empty:
                     ampl_MP.setData(MP_parameters[i])
-                else:
-                    print("DataFrame", i,"is empty.")
 
             elif isinstance(MP_parameters[i], pd.Series):
                 MP_parameters[i].name = i
                 df = pd.DataFrame(MP_parameters[i])
                 ampl_MP.setData(df)
 
             elif isinstance(MP_parameters[i], list):
@@ -562,41 +598,44 @@
         # Set scenario and Pareto_IDs
         # ------------------------------------------------------------------------------------------------------------
         if self.method['building-scale']:
             scenario = self.remove_emoo_constraints(scenario)
 
         ampl_MP = self.select_MP_objective(ampl_MP, scenario)
 
-        if not binary: ampl_MP.getConstraint('convexity_binary').drop()
+        if not binary:
+            ampl_MP.getConstraint('convexity_binary').drop()
 
         # Solve ampl_MP
         ampl_MP.solve()
 
-        df_Results_MP = WR.get_df_Results_from_MP(ampl_MP, binary, self.method, self.infrastructure, read_DHN=read_DHN)
-        print(ampl_MP.getCurrentObjective().getValues().toPandas())
+        df_Results_MP = write_results.get_df_Results_from_MP(ampl_MP, binary, self.method, self.infrastructure, read_DHN=read_DHN, scenario=scenario)
+        self.logger.info(str(ampl_MP.getCurrentObjective().getValues().toPandas()))
 
         df = self.get_solver_attributes(Scn_ID, Pareto_ID, ampl_MP)
         self.add_df_Results_MP(Scn_ID, Pareto_ID, self.iter, df_Results_MP, df)
         exitcode = exitcode_from_ampl(ampl_MP)
 
         del ampl_MP
         gc.collect()
-        if exitcode != 0: raise Exception('Master problem did not converge')
+        if exitcode != 0:
+            raise Exception('Master problem did not converge')
 
     def SP_iteration(self, scenario, Scn_ID=0, Pareto_ID=1):
         """
-        Description
-        -----------
-        Set up the parallel optimization if needed
+        Sets up the parallel optimization if needed.
 
-        Inputs
-        ------
-        scenario: dictionary
-        Scn_ID: scenario ID
-        Pareto_ID: int, pareto ID
+        Parameters
+        ----------
+        scenario : dictionary
+
+        Scn_ID : int
+            scenario ID
+        Pareto_ID: int
+            pareto ID
         """
 
         if self.method['parallel_computation']:
             # to run multiprocesses, a copy of the model is performed with pickles -> make sure ampl libraries are removed
             results = {h: self.pool.apply_async(self.SP_execution, args=(scenario, Scn_ID, Pareto_ID, h)) for h in self.infrastructure.houses}
 
             while len(results[list(self.buildings_data.keys())[-1]].get()) != 2:
@@ -608,111 +647,110 @@
         else:
             for h in self.infrastructure.houses:
                 df_Results, attr = self.SP_execution(scenario, Scn_ID, Pareto_ID, h)
                 self.add_df_Results_SP(Scn_ID, Pareto_ID, self.iter, h, df_Results, attr)
 
         self.feasible_solutions += 1  # after each 'round' of SP execution-> increase
 
-    def SP_execution(self, scenario, Scn_ID, Pareto_ID, House):
+    def SP_execution(self, scenario, Scn_ID, Pareto_ID, h):
         """
-        Description
-        -----------
-        Insert dual variables in ampl model, apply scenario, adapt model depending on the methods and get results
+        Inserts dual variables in ampl model, apply scenario, adapt model depending on the methods and get results.
 
-        Inputs
-        ------
+        Parameters
+        ----------
         scenario: dictionary
-        Scn_ID: scenario ID
-        Pareto_ID: int, pareto ID
-        House: string, house ID
 
-        Outputs
+        Scn_ID : int
+            scenario ID
+        Pareto_ID : int
+            pareto ID
+        h : string
+            house ID
+
+        Returns
         -------
-        df_Results : results of the optimization (unit installed, power exchanged, costs, GWP emissions, ...)
-        attr : results of the optimization process (CPU time, objective value, nb variables or constraints, ...)
+        df_Results :
+            results of the optimization (unit installed, power exchanged, costs, GWP emissions, ...)
+        attr :
+            results of the optimization process (CPU time, objective value, nb variables or constraints, ...)
 
         Raises
         ------
-        If the SP optimization did not converge
+        ValueError: If the SP optimization did not converge
         """
-        print('iterate HOUSE: ', House, 'iteration: ', self.iter)
+        self.logger.info('iterate HOUSE: ' + h + 'iteration: ' + str(self.iter))
 
         # Give dual variables to Subproblem
-        pi = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, House, 'pi').reorder_levels(['Layer', 'Period', 'Time'])
-        pi_GWP = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, House, 'pi_GWP').reorder_levels(['Layer', 'Period', 'Time'])
-        pi_lca = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, House, 'pi_lca')
-        pi_h = pd.concat([pi], keys=[House], names=['House']).reorder_levels(['House', 'Layer', 'Period', 'Time'])
-
-        parameters_SP = {}
-        parameters_SP['Cost_supply_network'] = pi
-        parameters_SP['Cost_demand_network'] = pi * (1-1e-9)
-        parameters_SP['Cost_supply'] = pi_h
-        parameters_SP['Cost_demand'] = pi_h * (1-1e-9)
-        parameters_SP['GWP_supply'] = pi_GWP
-        # set emissions of feed in to 0 -> changed in  postcompute
-        parameters_SP['GWP_demand'] = pi_GWP.mul(0)
-        parameters_SP['lca_kpi_demand'] = pi_lca
-        parameters_SP['lca_kpi_demand'] = pi_lca.mul(0)
+        pi = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, h, 'pi').reorder_levels(['Layer', 'Period', 'Time'])
+        pi_GWP = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, h, 'pi_GWP').reorder_levels(['Layer', 'Period', 'Time'])
+        pi_lca = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, h, 'pi_lca')
+        pi_h = pd.concat([pi], keys=[h], names=['Building']).reorder_levels(['Building', 'Layer', 'Period', 'Time'])
+
+        parameters_SP = {'Cost_supply_network': pi,
+                         'Cost_demand_network': pi * (1 - 1e-9),
+                         'Cost_supply': pi_h,
+                         'Cost_demand': pi_h * (1 - 1e-9),
+                         'GWP_supply': pi_GWP,
+                         'GWP_demand': pi_GWP.mul(0),  # set emissions of feed in to 0 -> changed in  postcompute
+                         'lca_kpi_demand': pi_lca.mul(0)
+                         }
 
         # find district structure, objective, beta and parameter for one single building
-        buildings_data_SP, parameters_SP, infrastructure_SP = self.__split_parameter_sets_per_building(House, parameters_SP)
-        beta = - self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, House, 'beta')
+        buildings_data_SP, parameters_SP = self.split_parameter_sets_per_building(h, parameters_SP)
+        beta = - self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter - 1, h, 'beta')
         scenario, beta_list = self.get_beta_values(scenario, beta)
         parameters_SP['beta_duals'] = beta_list
 
         # Execute optimization
         if self.method['use_facades'] or self.method['use_pv_orientation']:
-            REHO = compact_optimization(infrastructure_SP, buildings_data_SP, parameters_SP, self.set_indexed, self.cluster, scenario, self.method, self.solver, self.qbuildings_data)
+            REHO = SubProblem(self.infrastructure_SP[h], buildings_data_SP, self.local_data, parameters_SP, self.set_indexed, self.cluster,
+                              scenario, self.method, self.solver, self.qbuildings_data)
         else:
-            REHO = compact_optimization(infrastructure_SP, buildings_data_SP, parameters_SP, self.set_indexed, self.cluster, scenario, self.method, self.solver)
+            REHO = SubProblem(self.infrastructure_SP[h], buildings_data_SP, self.local_data, parameters_SP, self.set_indexed, self.cluster,
+                              scenario, self.method, self.solver)
 
         ampl = REHO.build_model_without_solving()
 
         if self.method['fix_units']:
             for unit in self.fix_units_list:
                 if unit == 'PV':
-                    ampl.getVariable('Units_Mult').get('PV_' + House).fix(self.df_fix_Units.Units_Mult.loc['PV_' + House] * 0.999)
-                    ampl.getVariable('Units_Use').get('PV_' + House).fix(float(self.df_fix_Units.Units_Use.loc['PV_' + House]))
+                    ampl.getVariable('Units_Mult').get('PV_' + h).fix(self.df_fix_Units.Units_Mult.loc['PV_' + h] * 0.999)
+                    ampl.getVariable('Units_Use').get('PV_' + h).fix(float(self.df_fix_Units.Units_Use.loc['PV_' + h]))
                 else:
-                    ampl.getVariable('Units_Mult').get(unit + '_' + House).fix( self.df_fix_Units.Units_Mult.loc[unit + '_' + House])
-                    ampl.getVariable('Units_Use').get(unit + '_' + House).fix( float(self.df_fix_Units.Units_Use.loc[unit + '_' + House]))
+                    ampl.getVariable('Units_Mult').get(unit + '_' + h).fix(self.df_fix_Units.Units_Mult.loc[unit + '_' + h])
+                    ampl.getVariable('Units_Use').get(unit + '_' + h).fix(float(self.df_fix_Units.Units_Use.loc[unit + '_' + h]))
 
         ampl.solve()
         exitcode = exitcode_from_ampl(ampl)
 
-        df_Results = WR.get_df_Results_from_SP(ampl, scenario, self.method, self.buildings_data)
+        df_Results = write_results.get_df_Results_from_SP(ampl, scenario, self.method, self.buildings_data)
         attr = self.get_solver_attributes(Scn_ID, Pareto_ID, ampl)
 
         del ampl
         gc.collect()  # free memory
 
         if exitcode != 0:
             # It might be that the solution is optimal with unscaled infeasibilities. So we check if we really found a solution (via its cost value)
             if exitcode != 'solved?' or df_Results["df_Performance"]['Costs_op'][0] + df_Results["df_Performance"]['Costs_inv'][0] == 0:
                 raise Exception('Sub problem did not converge')
 
         return df_Results, attr
 
     def check_Termination_criteria(self, scenario, Scn_ID=0, Pareto_ID=1):
         """
-        Description
-        -----------
-        Verify a number of termination criteria:
-            - optimal solution found based on reduced costs -> last solutions proposed by the SPs did not improve the MP
-            - no improvements
+        Verifies a number of termination criteria:
+
+        - Optimal solution found based on reduced costs -> last solutions proposed by the SPs did not improve the MP
+        - No improvements
 
-        Inputs
-        ------
-        scenario: dictionary, scenario of the optimization
-        Scn_ID: scenario ID
-        Pareto_ID: int, pareto ID
 
-        Outputs
+        Returns
         -------
-        df.any(axis=None): bool, if one of the stopping criteria is reached
+        df.any(axis=None) : boolean
+            If one of the stopping criteria is reached
 
         """
         # --------------------------------------------------------------
         # termination criteria based on no improvements
         # --------------------------------------------------------------
         solving_attributes = self.solver_attributes_MP.xs((Scn_ID, Pareto_ID), level=('Scn_ID', 'Pareto_ID'))
         delta = solving_attributes.val_objective.pct_change()  # .abs()
@@ -733,16 +771,17 @@
         # optimal solution found based on reduced costs
         # --------------------------------------------------------------
         last_SP_results = self.results_SP[Scn_ID][Pareto_ID][self.iter][self.feasible_solutions - 1]
         Cop = pd.DataFrame(dtype='float')
         Cinv = pd.DataFrame(dtype='float')
 
         for h in last_SP_results:
-            df_Grid_t = pd.concat([last_SP_results[h]["df_Grid_t"]], keys=[(self.iter, self.feasible_solutions - 1, h)], names=['Iter', 'FeasibleSolution', 'house'])
-            df_Grid_t = df_Grid_t.xs('Network', level='Hub')
+            df_Grid_t = pd.concat([last_SP_results[h]["df_Grid_t"]], keys=[(self.iter, self.feasible_solutions - 1, h)],
+                                  names=['Iter', 'FeasibleSolution', 'house'])
+            df_Grid_t = df_Grid_t.xs(h, level='Hub')
             pi = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter, h, 'pi')
             pi_GWP = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter, h, 'pi_GWP')
             pi_lca = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter, h, 'pi_lca')
 
             # Operation impact
             Cop_h = self.get_annual_grid_opex(df_Grid_t, cost_demand=pi, cost_supply=pi)
             Cop_h_GWP = self.get_annual_grid_opex(df_Grid_t, cost_demand=pi_GWP, cost_supply=pi_GWP)
@@ -767,15 +806,16 @@
         # calculate objective function for each Pareto_ID with latest dual values
         reduced_cost = pd.DataFrame()
         for h in last_SP_results:
             mu = self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter, h, 'mu')
             Cop_house = Cop.xs((self.iter, self.feasible_solutions - 1, h))
             Cinv_house = Cinv.xs((self.iter, self.feasible_solutions - 1, h))
             obj_fct = pd.Series( [Cinv_house["TOTEX"], Cop_house["TOTEX"]], index=["CAPEX", "OPEX"])
-            obj_fct = pd.concat([obj_fct, Cop_house + Cinv_house])
+            impacts = Cop_house + Cinv_house
+            obj_fct = pd.concat([obj_fct, impacts.replace(np.nan, 0)])
 
             beta = - self.get_dual_values_SPs(Scn_ID, Pareto_ID, self.iter, h, "beta")
             if beta.sum() == 0 and len(scenario["EMOO"].keys()) > 1:
                 warnings.warn('beta value = 0')
             beta_penalty = sum(beta * obj_fct)
 
             Costs_ft = last_SP_results[h]["df_Performance"].iloc[0].Costs_ft
@@ -806,32 +846,38 @@
     ####################################################################################################################
     #
     # THE FOLLOWING ATTRIBUTES ARE DOING DATA PROCESSING
     #
     ####################################################################################################################
 
     def initialise_DW_params(self, DW_params, cluster, buildings_datas):
-        if 'timesteps' not in DW_params: DW_params['timesteps'] = cluster['Periods'] * cluster['PeriodDuration'] + 2
-        if 'max_iter' not in DW_params: DW_params['max_iter'] = 15
-        if 'n_houses' not in DW_params: DW_params['n_houses'] = len(buildings_datas.keys())
-        if 'iter_no_improv' not in DW_params: DW_params['iter_no_improv'] = 5
-        if 'threshold_subP_value' not in DW_params: DW_params['threshold_subP_value'] = 0
-        if 'threshold_no_improv' not in DW_params: DW_params['threshold_no_improv'] = 0.00005
-        if 'grid_cost_exchange' not in DW_params: DW_params['grid_cost_exchange'] = 0.0
-        if 'weight_lagrange_cst' not in DW_params: DW_params['weight_lagrange_cst'] = 2.0
-        if self.method['building-scale']: DW_params['max_iter'] = 1
+        if 'timesteps' not in DW_params:
+            DW_params['timesteps'] = cluster['Periods'] * cluster['PeriodDuration'] + 2
+        if 'max_iter' not in DW_params:
+            DW_params['max_iter'] = 15
+        if 'n_houses' not in DW_params:
+            DW_params['n_houses'] = len(buildings_datas.keys())
+        if 'iter_no_improv' not in DW_params:
+            DW_params['iter_no_improv'] = 5
+        if 'threshold_subP_value' not in DW_params:
+            DW_params['threshold_subP_value'] = 0
+        if 'threshold_no_improv' not in DW_params:
+            DW_params['threshold_no_improv'] = 0.00005
+        if 'grid_cost_exchange' not in DW_params:
+            DW_params['grid_cost_exchange'] = 0.0
+        if 'weight_lagrange_cst' not in DW_params:
+            DW_params['weight_lagrange_cst'] = 2.0
+        if self.method['building-scale']:
+            DW_params['max_iter'] = 1
+
         return DW_params
 
     def get_final_MP_results(self, Pareto_ID=1, Scn_ID=0):
         """
-        Build the final design and operating results based on the optimal set of lambdas.
-
-        Attributes
-        ----------
-        result_object_of_REHO,  List of dataframes
+        Builds the final design and operating results based on the optimal set of lambdas.
         """
 
         # select the result chosen by the MP
         last_results = self.results_MP[Scn_ID][Pareto_ID][self.iter]
         lambdas = last_results["df_DW"]['lambda']
         MP_selection = lambdas[lambdas >= 0.999].index
 
@@ -851,23 +897,27 @@
             df_U_District = pd.concat([last_results["df_Unit"]], keys=[(self.iter, 'District')], names=['FeasibleSolution', 'house'])
             df_Unit = pd.concat([df_Unit, df_U_District])
         df_Unit = df_Unit.set_index(df_Unit.index.rename('Hub', level='house'))
         return df_Unit
 
     def get_annual_grid_opex(self, df_Grid_t, cost_supply=pd.Series(dtype='float'), cost_demand=pd.Series(dtype='float')):
         """
-        Inputs
-        ------
-        df_Grid_t: pandas dataframe, from result object REHO
-        Cost_supply_cst: optional, cost profile of supply
-        Cost_demand_cst: optional, cost profile of demand
+        Parameters
+        ----------
+        df_Grid_t : pd.DataFrame
+            from result object REHO
+        cost_supply : series
+            cost profile of supply
+        cost_demand : series
+            cost profile of demand
 
-        Outputs
+        Returns
         -------
-        annual_grid_costs: possibility to set tariffs/dual value pi. default: use costs from model
+        annual_grid_costs :
+            possibility to set tariffs/dual value pi. default: use costs from model
         """
         if cost_supply.empty:
             tariff_supply = df_Grid_t.Cost_supply
         else:
             tariff_supply = cost_supply.values
 
         if cost_demand.empty:
@@ -881,15 +931,15 @@
         ids = self.number_SP_solutions.iloc[0]
         df_Time = self.results_SP[ids['Scn_ID']][ids['Pareto_ID']][ids['Iter']][ids['FeasibleSolution']][ids['House']]["df_Time"]
         dp = df_Time.dp
         dp.iloc[-1] = 0  # exclude typical periods
         dp.iloc[-2] = 0
 
         # Transform profiles to annual values
-        df_costs = df_costs.groupby(level=['Iter', 'FeasibleSolution', 'house', 'Period'],  sort=False).sum()  # 'daily' sum
+        df_costs = df_costs.groupby(level=['Iter', 'FeasibleSolution', 'house', 'Period'], sort=False).sum()  # 'daily' sum
         df_costs = df_costs.mul(df_Time.dp, level='Period', axis=0)  # mul frequency of typical days
         annual_grid_costs = df_costs.groupby(level=['Iter', 'FeasibleSolution', 'house'], sort=False).sum()  # 'annual' sum
         return annual_grid_costs
 
     def select_MP_objective(self, ampl, scenario):
         list_constraints = ['EMOO_CAPEX_constraint', 'EMOO_OPEX_constraint', 'EMOO_GWP_constraint', 'EMOO_TOTEX_constraint',
                             'EMOO_lca_constraint', 'disallow_exchanges_1', 'disallow_exchanges_2'] + self.lists_MP["list_constraints_MP"]
@@ -913,18 +963,18 @@
 
         for i, o in ampl.getObjectives():
             o.drop()
         ampl.getObjective(scenario['Objective']).restore()
         return ampl
 
     def get_beta_values(self, scenario, beta=None):
-
+        scenario = scenario.copy()
         if isinstance(beta, (float, int, type(None))):
-            index = list(self.flags.keys()) # list of objective function
-            beta_list = pd.Series(np.zeros(len(index)), index=index) + 1e-6 # default penalty on other objectives
+            index = list(self.flags.keys())  # list of objective function
+            beta_list = pd.Series(np.zeros(len(index)), index=index) + 1e-6  # default penalty on other objectives
         elif isinstance(beta, pd.Series):
             beta_list = beta
             beta_list = beta_list.replace(0, 1e-6)
         else:
             raise warnings.warn("Wrong type beta")
 
         # select objective using beta values
@@ -933,15 +983,15 @@
         else:
             beta_list[scenario['Objective']] = 1
         scenario['Objective'] = 'SP_obj_fct'
 
         # add beta values on emoo constraint
         if isinstance(beta, (float, int)) and not self.method['building-scale']:
             emoo = scenario["EMOO"].copy()
-            for cst in ["EMOO_grid", "EMOO_GU_supply", "EMOO_GU_demand"]:
+            for cst in [k for k in scenario["EMOO"].keys() if k not in ['EMOO_TOTEX', 'EMOO_CAPEX', 'EMOO_OPEX','EMOO_GWP','EMOO_lca']]:
                 emoo.pop(cst, None)
             if 'EMOO_lca' in scenario["EMOO"].keys():
                 key = list(emoo['EMOO_lca'].keys())[0].replace("EMOO_", "")
                 beta_list[key] = beta
             elif len(emoo) == 1:
                 key = list(emoo.keys())[0].replace("EMOO_", "")
                 beta_list[key] = beta
@@ -949,46 +999,48 @@
                 if scenario["Objective"] == "OPEX":
                     beta_list["CAPEX"] = beta
                 else:
                     beta_list["OPEX"] = beta
             elif len(emoo) > 1:
                 raise warnings.warn("Multiple epsilon constraints")
 
-
         scenario = self.remove_emoo_constraints(scenario)
         return scenario, beta_list
 
+    @staticmethod
+    def remove_emoo_constraints(scenario):
 
-    def remove_emoo_constraints(self, scenario):
-        # remove emoo constraints
         EMOOs = list(scenario['EMOO'].keys())
         keys_to_remove = ['EMOO_CAPEX', 'EMOO_OPEX', 'EMOO_GWP', 'EMOO_TOTEX', 'EMOO_lca']
         if 'EMOO' in scenario:
             for key in list(set(EMOOs).intersection(keys_to_remove)):
                 scenario['EMOO'].pop(key, None)
         return scenario
 
-
     def get_dual_values_SPs(self, Scn_ID, Pareto_ID, iter, House, dual_variable):
         """
-        Description
-        -----------
-        Select the right dual variables for the given Scn_ID, Pareto_ID, iter and house IDs
+        Selects the right dual variables for the given Scn_ID, Pareto_ID, iter and house IDs.
 
-        Inputs
-        ------
-        Scn_ID: scenario ID
-        Pareto_ID: int, pareto ID
-        iter: int, iter ID
-        House: string, house ID
-        dual_variable: string, dual variable to get
+        Parameters
+        ----------
+        Scn_ID : int
+            scenario ID
+        Pareto_ID: int
+            pareto ID
+        iter : int
+            iter ID
+        House : string
+            house ID
+        dual_variable : string
+            dual variable to get
 
-        Outputs
+        Returns
         -------
-        dual_value : array, dual variables
+        dual_value : array
+            dual variables
         """
         attribute = None
         if dual_variable in ['pi', 'pi_GWP', 'pi_lca']:
             attribute = 'df_Dual_t'
         elif dual_variable in ['beta_cap', 'beta_op', 'beta_tot', 'beta_gwp']:
             attribute = 'df_District'
         elif dual_variable in ['beta']:
@@ -1002,29 +1054,30 @@
         elif dual_variable == 'pi_lca':
             dual_value = df[self.infrastructure.Set["Lca_kpi"]].stack()
             dual_value.index = dual_value.index.reorder_levels((3, 0, 1, 2))
         else:
             dual_value = df[dual_variable]  # dual variable from previous iteration
         return dual_value  # dual value for one BES only
 
-
     def get_solver_attributes(self, Scn_ID, Pareto_ID, ampl):
         """
-        Description
-        -----------
 
-        Inputs
-        ------
-        Scn_ID: scenario ID
-        Pareto_ID: int, ID of the pareto point, default is 1
-        ampl: ampl model with results concerning one SP
+        Parameters
+        ----------
+        Scn_ID: int
+            scenario ID
+        Pareto_ID: int
+            ID of the pareto point, default is 1
+        ampl: ampl model
+            results concerning one SP
 
-        Outputs
+        Returns
         -------
-        df: Dataframe with information on the optimization (CPU time, nb constraints, ...)
+        df : pd.DataFrame
+            Information on the optimization (CPU time, nb constraints, ...)
         """
         time = ampl.getValue('_total_solve_time')
         constr = ampl.getValue('_ncons')
         pres_constr = ampl.getValue('_sncons')  # after presolve
         var = ampl.getValue('_nvars')
         pres_var = ampl.getValue('_snvars')  # after presolve
         binaries = ampl.getValue('_snbvars')  # after presolve
@@ -1055,15 +1108,14 @@
         self.number_SP_solutions = self.number_SP_solutions.sort_values(['Pareto_ID', 'FeasibleSolution'])
         self.number_MP_solutions = self.number_MP_solutions.sort_values(['Pareto_ID', 'FeasibleSolution'])
         self.solver_attributes_SP = self.solver_attributes_SP.sort_values(['Pareto_ID', 'FeasibleSolution'])
         self.solver_attributes_MP = self.solver_attributes_MP.sort_values(['Pareto_ID', 'Iter'])
         if not self.method['building-scale']:
             self.reduced_costs = self.reduced_costs.sort_values(['Pareto_ID', 'Iter'])
 
-
     def add_df_Results_SP(self, Scn_ID, Pareto_ID, iter, house, df_Results, attr):
 
         if Scn_ID not in self.results_SP:
             self.results_SP[Scn_ID] = {}
         if Pareto_ID not in self.results_SP[Scn_ID]:
             self.results_SP[Scn_ID][Pareto_ID] = {}
         if iter not in self.results_SP[Scn_ID][Pareto_ID]:
@@ -1073,22 +1125,22 @@
         if house not in self.results_SP[Scn_ID][Pareto_ID][iter][self.feasible_solutions]:
             self.results_SP[Scn_ID][Pareto_ID][iter][self.feasible_solutions][house] = {}
 
         self.results_SP[Scn_ID][Pareto_ID][iter][self.feasible_solutions][house] = df_Results
         attr = pd.concat([attr], keys=[(house, iter, self.feasible_solutions)], names=['House', 'Iter', 'FeasibleSolution'])
         self.solver_attributes_SP = pd.concat([self.solver_attributes_SP, attr])
 
-        df = pd.DataFrame([[Scn_ID, Pareto_ID, iter, house, self.feasible_solutions]],  columns=['Scn_ID', 'Pareto_ID', 'Iter', 'House', 'FeasibleSolution'])
+        df = pd.DataFrame([[Scn_ID, Pareto_ID, iter, house, self.feasible_solutions]], columns=['Scn_ID', 'Pareto_ID', 'Iter', 'House', 'FeasibleSolution'])
         self.number_SP_solutions = pd.concat([self.number_SP_solutions, df], ignore_index=True)
 
         number_iter_global = int((len(self.number_SP_solutions) - 1) / len(self.buildings_data))
-        if 'MP_solution' not in self.number_SP_solutions.columns: self.number_SP_solutions['MP_solution'] = 0
+        if 'MP_solution' not in self.number_SP_solutions.columns:
+            self.number_SP_solutions['MP_solution'] = 0
         self.number_SP_solutions.iloc[-1, self.number_SP_solutions.columns.get_loc('MP_solution')] = number_iter_global
 
-
     def add_df_Results_MP(self, Scn_ID, Pareto_ID, iter, df_Results, attr):
 
         if Scn_ID not in self.results_MP:
             self.results_MP[Scn_ID] = {}
         if Pareto_ID not in self.results_MP[Scn_ID]:
             self.results_MP[Scn_ID][Pareto_ID] = {}
         if iter not in self.results_MP[Scn_ID][Pareto_ID]:
@@ -1096,58 +1148,65 @@
 
         self.results_MP[Scn_ID][Pareto_ID][iter] = df_Results
         attr = pd.concat([attr], keys=[iter], names=['Iter'])
         self.solver_attributes_MP = pd.concat([self.solver_attributes_MP, attr])
         col = self.number_SP_solutions.columns.difference(["House"])
         self.number_MP_solutions = self.number_SP_solutions[col].groupby('MP_solution').mean(numeric_only=True)
 
-    def __split_parameter_sets_per_building(self, h, parameters_SP=dict({})):
+    def split_parameter_sets_per_building(self, h, parameters_SP=dict({})):
         """
-        Description
-        -----------
         Some inputs are for the district and some other for the houses. This function fuses the two
         and gives the parameters per house. This is important to run an optimization on a single building
-        Inputs
-        ------
-        h : string,  House ID
-        parameters_SP: dictionary, Parameters of the house
 
-        Outputs
+        Parameters
+        ----------
+        h : string
+            House ID
+        parameters_SP : dict
+            Parameters of the house
+
+        Returns
         -------
-        buildings_data_SP: dictionary, egid, surface area, class of the building, ...
-        parameters_SP: dictionary, Parameters from the script for a single house (f.e. tariffs)
-        infrastructure_SP: dictionary, The district structure for a single house
+        buildings_data_SP : dict
+            egid, surface area, class of the building, ...
+        parameters_SP : dict
+            Parameters from the script for a single house (f.e. tariffs)
+        infrastructure_SP : dict
+            The district structure for a single house
         """
         ID = np.where(h == self.infrastructure.House)[0][0]
-
-        single_building_data = {"buildings_data": {h: self.buildings_data[h]}}
         buildings_data_SP = {h: self.buildings_data[h]}
-        building_units = {"building_units": self.infrastructure.units}
 
         for key in self.parameters:
             if key not in self.lists_MP["list_parameters_MP"]:
                 if isinstance(self.parameters[key], (int, float)):
                     parameters_SP[key] = self.parameters[key]
-                elif self.parameters[key].shape[0] >= self.DW_params['timesteps']:  # if demands profiles (heat gains / DHW / electricity) are set for more than 1 building
+                elif self.parameters[key].shape[0] >= self.DW_params['timesteps']:  # if demands profiles are set for more than 1 building
                     if len(self.infrastructure.houses) < self.DW_params['timesteps']:
-                        nb_buildings = round(self.parameters[key].shape[0]/self.DW_params['timesteps'])
+                        nb_buildings = round(self.parameters[key].shape[0] / self.DW_params['timesteps'])
                         profile_building_x = self.parameters[key].reshape(nb_buildings, self.DW_params['timesteps'])
                         parameters_SP[key] = profile_building_x[ID]
                 else:
                     parameters_SP[key] = self.parameters[key][ID]
+        return buildings_data_SP, parameters_SP
 
-        infrastructure_SP = infrastructure.infrastructure(single_building_data, building_units, self.infrastructure.grids)  # initialize District
-
-        # TODO: better integration Units_Parameters specific to each house
-        unit_param = self.infrastructure.Units_Parameters.loc[[string.endswith(h) for string in self.infrastructure.Units_Parameters.index]]
-        infrastructure_SP.Units_Parameters[["Units_Fmax", "Cost_inv2"]] = unit_param[["Units_Fmax", "Cost_inv2"]]
-
-        return buildings_data_SP, parameters_SP, infrastructure_SP
+    def build_infrastructure_SP(self):
+        for h in self.buildings_data:
+            single_building_data = {"buildings_data": {h: self.buildings_data[h]}}
+            building_units = {"building_units": self.infrastructure.units}
+            infrastructure_SP = infrastructure.Infrastructure(single_building_data, building_units, self.infrastructure.grids)
+
+            # TODO: better integration Units_Parameters specific to each house
+            unit_param = self.infrastructure.Units_Parameters.loc[[string.endswith(h) for string in self.infrastructure.Units_Parameters.index]]
+            infrastructure_SP.Units_Parameters[["Units_Fmax", "Cost_inv2"]] = unit_param[["Units_Fmax", "Cost_inv2"]]
+            self.infrastructure_SP[h] = infrastructure_SP
+        return
 
-    def return_combined_SP_results(self, df_Results, df_name):
+    @staticmethod
+    def return_combined_SP_results(df_Results, df_name):
 
         t = {(i, j, k, l, m): df_Results[i][j][k][l][m][df_name]
              for i in df_Results.keys()
              for j in df_Results[i].keys()
              for k in df_Results[i][j].keys()
              for l in df_Results[i][j][k].keys()
              for m in df_Results[i][j][k][l].keys()
```

### Comparing `REHO-1.0.2/reho/model/infrastructure.py` & `reho-1.1.0/reho/model/infrastructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 import os.path
-import math
+
 import numpy as np
 import pandas as pd
+
 from reho.paths import *
 
 
-class infrastructure:
+__doc__ = """
+File for handling infrastructure parameters.
+"""
+
+
+class Infrastructure:
     """
-    This class characterizes all the sets and parameters which are connected to buildings, units and grids.
+    Characterizes all the sets and parameters which are connected to buildings, units and grids.
 
     Parameters
     ----------
     qbuildings_data : dict
         Buildings characterization
     units : dict
         Units characterization
     grids : dict
         Grids characterization
     """
+
     def __init__(self, qbuildings_data, units, grids):
 
         self.units = units["building_units"]
         self.houses = {h: {'units': self.units, 'layers': grids} for h in qbuildings_data['buildings_data'].keys()}
         self.grids = grids
         if "district_units" in units:
             self.district_units = units["district_units"]
@@ -80,22 +87,19 @@
         self.Units_Parameters_lca = pd.DataFrame()
         self.Streams_H = pd.DataFrame()
 
         self.HP_parameters = {}
 
         self.generate_structure()
         self.generate_parameter()
-    
 
     def generate_structure(self):
-        """
-        The indexes h_ht, h_mt, h_lt, c_ht state for the discretization of the streams. They are connected to the heat cascade.
-        h_ht: hotstream_hightemperature. h_mt: hotstream_mediumtemperature. h_lt: hotstream_lowtemperature. c_ht: coldstream_hightemperature
-        :return:
-        """
+
+        # The indexes h_ht, h_mt, h_lt, c_ht state for the discretization of the streams. They are connected to the heat cascade.
+        # h_ht: hotstream_hightemperature. h_mt: hotstream_mediumtemperature. h_lt: hotstream_lowtemperature. c_ht: coldstream_hightemperature
 
         for h in self.House:
             # Units------------------------------------------------------------
             for u in self.houses[h]['units']:
                 complete_name = u['name'] + '_' + h
 
                 self.Units = np.append(self.Units, [complete_name])
@@ -103,15 +107,16 @@
                 for l in u['UnitOfLayer']:
                     self.UnitsOfLayer[l] = np.append(self.UnitsOfLayer[l], [complete_name])
                 self.UnitsOfHouse[h] = np.append(self.UnitsOfHouse[h], [complete_name])
                 for s in u['UnitOfService']:
                     self.UnitsOfService[s] = np.append(self.UnitsOfService[s], [complete_name])
 
                 # Streams---------------------------------------------------------
-                self.StreamsOfBuilding[h] = np.array([h + '_c_lt', h + '_c_mt', h + '_h_lt'])  # c_mt  c_lt - space heat demand discretized in 2 streams, _- h_lt for cooling
+                self.StreamsOfBuilding[h] = np.array(
+                    [h + '_c_lt', h + '_c_mt', h + '_h_lt'])  # c_mt  c_lt - space heat demand discretized in 2 streams, _- h_lt for cooling
                 self.StreamsOfUnit[complete_name] = np.array([])
                 for s in u['StreamsOfUnit']:
                     stream = u['name'] + '_' + h + '_' + s
                     self.StreamsOfUnit[complete_name] = np.append(self.StreamsOfUnit[complete_name], stream)
 
             # Layers------------------------------------------------------------
             for l in self.houses[h]['layers']:
@@ -250,27 +255,27 @@
                     else:
                         self.HP_parameters[u['HP_parameters']] = df
 
         for key in self.TemperatureSets:  # add additional sets from units to total set
             self.Set[key] = self.TemperatureSets[key]
 
         # TODO select the AC and HP units without number place in the self.units array
-        #self.Set['AC_Tsupply'] = np.array(self.units[2]['stream_Tin'])
-        #self.Set['HP_Tsupply'] = np.array(self.units[0]['stream_Tin'])
+        # self.Set['AC_Tsupply'] = np.array(self.units[2]['stream_Tin'])
+        # self.Set['HP_Tsupply'] = np.array(self.units[0]['stream_Tin'])
 
         # Streams------------------------------------------------------------
 
         Hin = {}
         Hout = {}
         for unitstreams in dict(self.StreamsOfUnit, **self.StreamsOfBuilding).values():  # union of dict
             for s in unitstreams:
-                if s.count('_h_') == 1:  # check if its a hot stream
+                if s.count('_h_') == 1:  # check if it's a hot stream
                     Hin[s] = 1
                     Hout[s] = 0
-                elif s.count('_c_') == 1:  # check if its a cold stream
+                elif s.count('_c_') == 1:  # check if it's a cold stream
                     Hin[s] = 0
                     Hout[s] = 1
                 else:
                     raise ('Stream ' + str(s) + ' cannot be classified as cold or hot')
 
         dfin = pd.DataFrame.from_dict(Hin, orient='index', columns=['Streams_Hin'])
         dfout = pd.DataFrame.from_dict(Hout, orient='index', columns=['Streams_Hout'])
@@ -295,27 +300,25 @@
         df_lca.index.names = ["Lca_kpi"]
         df_lca["Units"] = complete_name
         df_lca = df_lca.set_index("Units", append=True)
         self.Units_Parameters_lca = pd.concat([self.Units_Parameters_lca, df_lca])
 
     def set_discretize_unit_size(self):
 
-        sizes = {}
-        sizes['Air_Conditioner'] = [0]
-        sizes['HeatPump'] = [0, 2.7, 3.4, 5.5]
-        sizes['WaterTankDHW'] = [0, 0.07, 0.125, 0.20, 0.8]
-        sizes['WaterTankSH'] = [0, 0.20, 0.40, 0.60, 0.75]
-        sizes['ElectricalHeater'] = [0, 3.0, 6.0, 9.0, 12.0, 15, 20, 22]
-        sizes['ElectricalHeater'] = [0, 3.0, 6.0, 9.0, 12.0, 15, 20, 22]
-        sizes['NG_Boiler'] = [0, 11.8]
-        sizes['Battery'] = [0, 2.5, 5, 10]
-        sizes['NG_Cogeneration'] = [0, 0.7]
-        sizes['EV'] = []
-        sizes['PV'] = []
-        sizes['ThermalSolar'] = []
+        sizes = {'Air_Conditioner': [0],
+                 'HeatPump': [0, 2.7, 3.4, 5.5],
+                 'WaterTankDHW': [0, 0.07, 0.125, 0.20, 0.8],
+                 'WaterTankSH': [0, 0.20, 0.40, 0.60, 0.75],
+                 'ElectricalHeater': [0, 3.0, 6.0, 9.0, 12.0, 15, 20, 22],
+                 'NG_Boiler': [0, 11.8],
+                 'Battery': [0, 2.5, 5, 10],
+                 'NG_Cogeneration': [0, 0.7],
+                 'EV': [],
+                 'PV': [],
+                 'ThermalSolar': []}
 
         for h in self.House:
             for u in self.houses[h]['units']:
                 complete_name = u['name'] + '_' + h
                 self.UnitSizes[complete_name] = np.array(sizes[u['UnitOfType']])
 
         self.Set['UnitSizes'] = self.UnitSizes  # add to all sets
@@ -333,27 +336,28 @@
         The units you want to exclude, given through ``initialize_units``.
     grids : dict
         Grids given through ``initialize_units``.
 
     Returns
     -------
     np.array
-        Array that contains the one dictionary by cell, containing the units information.
+        Array that contains the one dictionary by cell, containing the units' information.
 
     See also
     --------
     initialize_units
 
     Notes
     -----
     - Make sure the name of the columns you are using are the same as the one from the default files, that can be found
       in *data/infrastructure*.
     - The name of the units, which will be used as keys, do not matter but the *UnitOfType* must be along a defined
       list of possibilities.
     """
+
     def transform_into_list(column):
         for idx, row in column.items():
             try:
                 new_value = [float(el) for el in row.split('/') if el != '']
             except:
                 new_value = [el.strip() for el in row.split('/') if el != '']
             if unit_data.index.get_loc(idx) == 0 and new_value == []:
@@ -412,15 +416,15 @@
 
     return units
 
 
 def initialize_units(scenario, grids=None, building_data=os.path.join(path_to_infrastructure, "building_units.csv"),
                      district_data=None, storage_data=None):
     """
-    Initialize the available units for the energy system.
+    Initializes the available units for the energy system.
 
     Parameters
     ----------
     scenario : dict or None
         A dictionary containing information about the scenario.
     grids : dict or None, optional
         Information about the energy layers considered. If None, ``['Electricity', 'NaturalGas', 'Oil', 'Wood', 'Data', 'Heat']``.
@@ -482,15 +486,15 @@
 
     return units
 
 
 def initialize_grids(available_grids={'Electricity': {}, 'NaturalGas': {}},
                      file=os.path.join(path_to_infrastructure, "grids.csv")):
     """
-    Initialize grid information for the energy system.
+    Initializes grid information for the energy system.
 
     Parameters
     ----------
     available_grids : dict, optional
         A dictionary specifying the available grids and their parameters. The keys represent grid names,
         and the values are dictionaries containing optional parameters ['Cost_demand_cst',
         'Cost_supply_cst', 'GWP_demand_cst', 'GWP_supply_cst'].
@@ -537,8 +541,7 @@
             if 'GWP_supply_cst' in available_grids[idx]:
                 grid_dict['GWP_supply_cst'] = available_grids[idx]['GWP_supply_cst']
             if 'Cost_connection' in available_grids[idx]:
                 grid_dict['Cost_connection'] = available_grids[idx]['Cost_connection']
             grids[idx] = grid_dict
 
     return grids
-
```

### Comparing `REHO-1.0.2/reho/model/postprocessing/KPIs.py` & `reho-1.1.0/reho/model/postprocessing/KPIs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import pandas as pd
 import numpy as np
 import reho.model.preprocessing.emissions_parser as emissions
-import reho.model.preprocessing.weather as WD
+import reho.model.preprocessing.weather as weather
 
 __doc__ = """
-*Calculates the KPIs resulting from the optimization.*
+Calculates the KPIs resulting from the optimization.
 """
 
-def postcompute_efficiency(df_unit, buildings_data, df_annual, df_annual_network, df_profiles, df_external, df_Time):
+
+def postcompute_efficiency(df_unit, buildings_data, df_annual, df_annual_network, df_profiles, df_Weather, df_Time):
     # --------------------------------------------------------------------
     # energy
     # --------------------------------------------------------------------
 
     demand = df_annual['MWh_el_domestic'] + df_annual['MWh_Qsh'] + df_annual['MWh_Qdhw']
     demand_net = demand.sum()
     supply = df_annual['MWh_imp_el'] - df_annual['MWh_exp'] + df_annual['MWh_resources'] + df_annual['MWh_PV']
@@ -19,15 +20,15 @@
         'MWh_resources'] + df_annual['MWh_PV'].sum()
 
     eta_I = demand / supply
     eta_I_net = demand_net / supply_net
 
     # -----------------------------eta_I including PV
     # annual irradiation density
-    irr_p = df_external['I_global'].groupby(level='Period').sum() / 1000  # kWh /m2
+    irr_p = df_Weather['I_global'].groupby(level='Period').sum() / 1000  # kWh /m2
     irr_a = irr_p.mul(df_Time.dp, axis=0)
     irr_a = irr_a.sum() / 1000  # MWh/m2
     # reference efficiency PV panel - default 0.14 if no value as input
 
     PV_IRR = pd.DataFrame()
     np_m2_PV = np.array([])
     for i, h in enumerate(buildings_data):
@@ -56,25 +57,25 @@
     LHV_ng = 50.018 / 3600  # MJ/kg -> MWh/kg [Favrat book, chapter 11, page 494 (English version)]
     ex_ng = 51.757 / 3600  # MJ/kg -> MWh/kg
 
     Ex_ng = (df_annual['MWh_resources'] / LHV_ng) * ex_ng
 
     # domestic hot water
     T_dhw = 55 + 273.15
-    eta_carnot_dhw = (1 - ((df_external['T_ext'] + 273.15) / (T_dhw + 273.15)))
+    eta_carnot_dhw = (1 - ((df_Weather['T_ext'] + 273.15) / (T_dhw + 273.15)))
     E_dhw = df_profiles['Q_DHW'] * eta_carnot_dhw
 
     E_dhw_p = E_dhw.groupby(level=['Hub', 'Period']).sum()
     E_dhw_a = E_dhw_p.mul(df_Time.dp, level='Period', axis=0)
     E_dhw_a = E_dhw_a.groupby(level='Hub').sum() / 1000
 
     # space heating
     df_E_sh_a = pd.DataFrame()
     for house in df_profiles.index.unique(level=0):
-        eta_carnot_sh = (1 - ((df_external['T_ext'] + 273.15) / (df_profiles['T_in'].xs(house, level=0) + 273.15)))
+        eta_carnot_sh = (1 - ((df_Weather['T_ext'] + 273.15) / (df_profiles['T_in'].xs(house, level=0) + 273.15)))
 
         E_sh = df_profiles['House_Q_heating'].xs(house, level=0) * eta_carnot_sh
 
         E_sh_p = E_sh.groupby(level='Period').sum()
         E_sh_a = E_sh_p.mul(df_Time.dp, axis=0)
         E_sh_a = E_sh_a.sum() / 1000
         df = pd.DataFrame(E_sh_a, index=[house], columns=['E_sh'])
@@ -91,17 +92,17 @@
         'MWh_PV'].sum() + Ex_ng.sum()
 
     eta_II = exergie_demand / exergie_supply
     eta_II_net = exergie_demand_net / exergie_supply_net
 
     # -----------------------------eta_II including PV
 
-    eta_carnot_irr = (1 - ((df_external['T_ext'] + 273.15) / (
+    eta_carnot_irr = (1 - ((df_Weather['T_ext'] + 273.15) / (
         6000)))  # Temperature sun 6000k - source: book: McEnvoy: Practical Handbook of Photovoltaics 2nd edition page 64
-    E_irr = eta_carnot_irr * df_external['I_global'] / 1000  # kW/m2
+    E_irr = eta_carnot_irr * df_Weather['I_global'] / 1000  # kW/m2
     E_irr_p = E_irr.groupby(level='Period').sum()
     E_irr_a = E_irr_p.mul(df_Time.dp, axis=0)
     E_irr_a = E_irr_a.sum() / 1000  # MWh
     E_irr_a = E_irr_a * df_m2
 
     exergie_supply_pv = df_annual['MWh_imp_el'] - df_annual['MWh_exp'] + E_irr_a['PV'] + Ex_ng
     exergie_supply_pv_net = df_annual_network['MWh_el_imp'] - df_annual_network['MWh_el_exp'] + E_irr_a[
@@ -131,15 +132,15 @@
         df_SC.iloc[df_SC == 0] = 1
         df_SC_net.iloc[df_SC_net == 0] = 1
 
         if (df_gen == 0).all():
             SC = df_SC / 1
             SC_net = df_SC_net / 1
         else:
-            # one building has PV -> district has a SC neq 1
+            # one building has PV -> district has SC neq 1
             SC_net = df_SC_net / df_gen.sum()
             # make sure to set SC 1 for buildings without PV
             df_gen[df_gen == 0] = 1
             SC = df_SC / df_gen
     else:
         SC = df_SC / df_gen
         SC_net = df_SC_net / df_gen.sum()
@@ -241,16 +242,16 @@
 
         kWh_PV = df_annual.loc[house]['MWh_PV'] * 1000
         kWh_house = df_annual.loc[house]['MWh_el_domestic'] * 1000
 
         if kWh_PV == 0:
             LCoE1 = np.nan
         else:
-            LCoE1 = (C_PV + C_BAT + C_el1[house]) / (kWh_PV)  # CHF/kWh
-        LCoE2 = (C_PV + C_BAT + C_el2[house]) / (kWh_house)
+            LCoE1 = (C_PV + C_BAT + C_el1[house]) / kWh_PV  # CHF/kWh
+        LCoE2 = (C_PV + C_BAT + C_el2[house]) / kWh_house
 
         df_LCoE.at[house, 'LCoE1'] = LCoE1
         df_LCoE.at[house, 'LCoE2'] = LCoE2
 
     # KPI on network
     kWh_house_net = df_annual.MWh_el_domestic.sum() * 1000
     kWh_PV_net = df_annual.MWh_PV.sum() * 1000
@@ -263,20 +264,17 @@
 
     df_LCoE.at['Network', 'LCoE1'] = LCoE1_net
     df_LCoE.at['Network', 'LCoE2'] = LCoE2_net
 
     return df_LCoE
 
 
-def postcompute_average_emission(df_annual, df_annual_net, df_profiles, df_profiles_net, df_Time, cluster,
-                                 infrastructure):
-    # --------------------------------------------------------------------
-    # emissions
-    # --------------------------------------------------------------------
+def postcompute_average_emission(df_annual, df_annual_net, df_profiles, df_profiles_net, df_Time, cluster, timestamp_file, emissions_matrix):
 
+    # Emissions
     em_supply_dy = df_profiles_net.GWP_supply.xs('Electricity')
     em_demand_dy = df_profiles_net.GWP_demand.xs('Electricity')
 
     # Buildings
     em_el_av_bui = em_supply_dy.mean() * df_profiles.Grid_supply - em_demand_dy.mean() * df_profiles.Grid_demand
     em_el_av_bui = em_el_av_bui.mul(df_Time.dp, level='Period', axis=0).groupby('Hub').sum()
 
@@ -304,17 +302,17 @@
     em_el_av = pd.concat([em_el_av_bui, em_el_av_net])
 
     # --------------------------------------------------------------------
     # Renewable energy share
     # --------------------------------------------------------------------
     df_el_net = df_profiles_net.xs('Electricity', level=0)
 
-    File_ID = WD.get_cluster_file_ID(cluster)
-    res_profile = emissions.return_typical_emission_profiles(df_Time, File_ID, 'method 1')
-    res_av = emissions.find_average_value('CH', 'method 1')
+    File_ID = weather.get_cluster_file_ID(cluster)
+    res_profile = emissions.return_typical_emission_profiles(df_Time, File_ID, 'method 1', timestamp_file, emissions_matrix)
+    res_av = emissions.find_average_value('CH', 'method 1', emissions_matrix)
     s_RES_dy = pd.Series(dtype='float')
     s_RES_av = pd.Series(dtype='float')
 
     for h in df_annual.index.get_level_values(level='Hub'):
         res_e = res_profile['GWP_supply'].values * df_profiles.Grid_supply.xs(h, level='Hub', drop_level=False)
         res_e = res_e.groupby(level=['Hub', 'Period']).sum()
         res_e = res_e.mul(df_Time.dp, axis=0).groupby(
@@ -400,32 +398,32 @@
         df.at['Network', 'COP'] = total_heat_network / total_HP_el
 
     return df
 
 
 def build_df_profiles_house(df_Results, infrastructure):
     """
-    Build hourly profiles for demand and consumption of units and buildings
+    Builds hourly profiles for demand and consumption of units and buildings.
     """
 
     df_PV = units_power_profiles_per_building(df_Results, infrastructure, 'PV')
     df_BAT = units_power_profiles_per_building(df_Results, infrastructure, 'Battery')
 
-    df_grid_profile = df_Results["df_Grid_t"].xs(('Electricity'), level=('Layer'))
+    df_grid_profile = df_Results["df_Grid_t"].xs('Electricity', level='Layer')
 
     df_profiles_house = df_grid_profile.drop('Network', level='Hub')
     df_profiles_house['PV'] = df_PV['Units_supply']
     df_profiles_house['PVC'] = df_PV['Units_curtailment']
     df_profiles_house['BA_in'] = df_BAT['Units_demand']
     df_profiles_house['BA_out'] = df_BAT['Units_supply']
     df_profiles_house['House_Q_heating'] = df_Results["df_Buildings_t"]['House_Q_heating']
     df_profiles_house['T_in'] = df_Results["df_Buildings_t"]['T_in']
     df_profiles_house['Q_DHW'] = df_Results["df_Buildings_t"]['House_Q_DHW']
 
-    if 'NG_Cogeneration' in infrastructure.UnitTypes and not infrastructure.UnitsOfType["NG_Cogeneration"] == 'NG_Cogeneration_district':
+    if 'NG_Cogeneration' in infrastructure.UnitTypes and not any(infrastructure.UnitsOfType["NG_Cogeneration"] == 'NG_Cogeneration_district'):
         df_NG_Cogeneration = units_power_profiles_per_building(df_Results, infrastructure, 'NG_Cogeneration')
         df_profiles_house['NG_Cogeneration'] = df_NG_Cogeneration['Units_supply']
         df_profiles_house['onsite_el'] = df_profiles_house['PV'] + df_profiles_house['NG_Cogeneration']
         PV_sell = df_profiles_house['Grid_demand'] - df_profiles_house['NG_Cogeneration']
         PV_sell[PV_sell < 0] = 0
         df_profiles_house['PV_SC'] = df_profiles_house['PV'] - PV_sell
     else:
@@ -434,16 +432,24 @@
     df_profiles_house['SC'] = df_profiles_house['onsite_el'] - df_profiles_house['Grid_demand']
 
     return df_profiles_house
 
 
 def build_df_annual(df_Results, df_profiles_house, infrastructure, df_Time):
     """
-    Transform profiles to annual values, convert to MWh and insert additional values (costs, net resource exchanges)
-    Outputs: Annual parameter for each building and for the network
+    Transforms profiles to annual values, convert to MWh and insert additional values (costs, net resource exchanges).
+
+    Parameters:
+        df_Results (df) : results of a scenario
+        df_profiles_house (df)
+        infrastructure (df)
+        df_Time (df)
+
+    Returns:
+        Annual parameters for each building and for the network.
     """
 
     df_period = df_profiles_house.groupby(level=['Hub', 'Period']).sum()  # 'daily' sum
     df_period = df_period.mul(df_Time.dp, level='Period', axis=0)  # multiply by frequency
 
     df_annual = df_period.groupby(level=['Hub']).sum()  # annuals
     df_annual['Cost_supply'] = df_annual['Cost_supply'] / 8760  # average price
@@ -491,15 +497,15 @@
 
     for key in ['Costs_op', 'Costs_inv', 'Costs_rep']:
         df_annual_network[key] = df_Results["df_Performance"].iloc[0][key]
 
     return df_annual, df_annual_network
 
 
-def calculate_KPIs(df_Results, infrastructure, buildings_data, cluster):
+def calculate_KPIs(df_Results, infrastructure, buildings_data, cluster, timestamp_file, emissions_matrix):
     df_profiles = build_df_profiles_house(df_Results, infrastructure)
     df_profiles_network = df_Results["df_Grid_t"].xs('Network', level='Hub').copy()
 
     df_Time = df_Results["df_Time"]
     df_Time.dp.iloc[-1] = 0  # exclude extreme periods
     df_Time.dp.iloc[-2] = 0
 
@@ -552,26 +558,25 @@
     # ------------------------------------------------------------------------------------------------------
     # GWP
     # ------------------------------------------------------------------------------------------------------
     df_KPI['gwp_op_m2'] = df_Results["df_Performance"]['GWP_op'].div(df_hsA.ERA)
     df_KPI['gwp_constr_m2'] = df_Results["df_Performance"]['GWP_constr'].div(df_hsA.ERA)
     df_KPI['gwp_tot_m2'] = df_KPI['gwp_op_m2'] + df_KPI['gwp_constr_m2']  # [kgCO2-eq/m2/yr]
 
-    df_G_RES = postcompute_average_emission(df_annual, df_annual_network, df_profiles, df_profiles_network, df_Time,
-                                            cluster, infrastructure)
+    df_G_RES = postcompute_average_emission(df_annual, df_annual_network, df_profiles, df_profiles_network, df_Time, cluster, timestamp_file, emissions_matrix)
     df_KPI = pd.concat([df_KPI, df_G_RES[['gwp_elec_av', 'gwp_elec_dy']].div(df_hsA.ERA, axis=0)], axis=1)
     df_KPI = df_KPI.rename(
         columns={'gwp_elec_av': 'gwp_elec_av_m2', 'gwp_elec_dy': 'gwp_elec_dy_m2'})  # gwp_elec_av_m2    gwp_elec_dy_m2
     df_KPI = pd.concat([df_KPI, df_G_RES[['RES_dy', 'RES_av']]], axis=1)  # RES_dy    RES_av
 
     # ------------------------------------------------------------------------------------------------------
     # Technical KPIs
     # ------------------------------------------------------------------------------------------------------
     df_eta = postcompute_efficiency(df_Results["df_Unit"], buildings_data, df_annual, df_annual_network, df_profiles,
-                                    df_Results["df_External"], df_Time)
+                                    df_Results["df_Weather"], df_Time)
     df_KPI = pd.concat([df_KPI, df_eta], axis=1)  # eta_I    eta_II   eta_Ipv  eta_IIpv
 
     if 'HeatPump' in infrastructure.UnitsOfType:  # Check if HP DHN is used
         df_COP = postcompute_annual_COP(df_Results["df_Annuals"], infrastructure)
         df_KPI = pd.concat([df_KPI, df_COP], axis=1)
 
     df_KPI.index.names = ['Hub']
@@ -692,10 +697,63 @@
 
     # Final dfs
     df_op = pd.concat([df_cost.merge(pivot_df_grid_cost, on='Hub')], keys=['costs'], names=['Perf_type'])
     df_op_impact = pd.concat([df_impact.merge(pivot_df_grid_impact, on='Hub')], keys=['impact'], names=['Perf_type'])
     df_op = pd.concat([df_op, df_op_impact])
     df_inv = pd.concat([df_unit_cost, df_unit_impact], keys=['costs', 'impact'], names=['Perf_type'])
 
-    df_eco = pd.concat([df_op, df_inv], keys=['operation', 'investment'], names=['Category'], axis=1)
+    df_Economics = pd.concat([df_op, df_inv], keys=['operation', 'investment'], names=['Category'], axis=1)
+
+    return df_Economics
+
+
+def temperature_profile(df_Results, daily_averaging=False):
+    """
+    Returns a pd.Series of the indoor temperature profile, one column per building.
+    TODO : check if multi-buildings works fine
+
+    Parameters:
+        df_Results (df) : pd.DataFrame of a scenario
+        daily_averaging (bool) : to average over days
+
+    Returns:
+        df_Tin
+    """
+    # Extract the data
+    buildings_list = list(df_Results['df_Buildings'].index)
+    df_buildings_t = df_Results['df_Buildings_t']
+
+    # Prepare the df to store the Tin
+    df_Tin = pd.DataFrame()
+
+    # list of the two last periods used for design purpose to drop later
+    period_to_drop = list(df_buildings_t.xs('Building1').index.get_level_values('Period').unique()[-2:])
+
+    # For each building: calculation of the Tin series
+    for b in buildings_list:
+        # Take Tin for the building in df_buildings_t
+        df_Tin_building = pd.DataFrame()
+        df_Tin_building['T_in'] = df_buildings_t.xs(b)['T_in']
+
+        # drop the last two periods for design
+        for i in period_to_drop:
+            df_Tin_building = df_Tin_building.drop(i, level='Period')
+
+        # array to work for a building
+        Tin_building = np.array([])
+
+        for j in range(1, 366):
+            id = df_Results['df_Index'].PeriodOfYear[j * 24]
+            data_id = df_Tin_building.xs(id)
+            Tin_building = np.concatenate((Tin_building, data_id['T_in']))
+
+        if daily_averaging:
+            items_average = 24
+            Tin_building = np.mean(Tin_building.reshape(-1, items_average), axis=1)
+
+        # Store the data in df_Tin (one col per building)
+        df_Tin['T_in_' + str(b)] = Tin_building
+
+    # create idx
+    idx = list(df_Tin.index + 1)
 
-    return df_eco
+    return df_Tin.to_numpy(), idx
```

### Comparing `REHO-1.0.2/reho/model/postprocessing/building_scale_network_builder.py` & `reho-1.1.0/reho/model/postprocessing/building_scale_network_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pandas as pd
 import numpy as np
 
 __doc__ = """
-*Manipulates results to have consistency between the building-scale and district-scale optimizations.*
+Manipulates results to have consistency between the building-scale and district-scale optimizations.
 """
 
+
 def correct_network_values(reho, scn_id=0, pareto_id=0):
     """
     This function is only useful to find KPIs from the district perspective with a building scale optimization.
-    It takes results from the reho object and correct df_KPI, df_Annuals and df_Performance
+    It takes results from the reho object and correct df_KPI, df_Annuals and df_Performance.
     """
     df_grid = reho.results[scn_id][pareto_id]["df_Grid_t"].xs(("Electricity", "Network"), level=("Layer", "Hub"))
     df_export, df_import = get_transformer_import_exports(df_grid)
     nb_periods = reho.cluster["Periods"]
 
     df = reho.results[scn_id][pareto_id]["df_Grid_t"].sort_index()
     df.loc[("Electricity", "Network"), 'Grid_demand'] = df_export['Grid_profile'].values
@@ -21,51 +22,51 @@
 
     df_grid = reho.results[scn_id][pareto_id]["df_Grid_t"]
     df_time = reho.results[scn_id][pareto_id]["df_Time"]
     surface = reho.ERA
     df_unit_t = reho.results[scn_id][pareto_id]["df_Unit_t"]
     df_KPI = reho.results[scn_id][pareto_id]["df_KPIs"]
 
-    OPEX_m2 = return_correct_OPEX(df_grid,  df_time, surface)
+    OPEX_m2 = return_correct_OPEX(df_grid, df_time, surface)
     SS_SC = correct_SS_SC(df_grid, df_unit_t, df_time, nb_periods)
     GWP = return_BUI_GWPop(df_grid, surface, df_time, df_KPI)
     GM_GU = correct_grid_param(df_grid)
     results = correct_data_in_reho(reho.results[scn_id][pareto_id], OPEX_m2, SS_SC, GWP, GM_GU, surface)
     return results
 
 
 def get_transformer_import_exports(df_grid):
-    typical_profile = df_grid.Grid_demand - df_grid.Grid_supply #attention! Supply is negative, feed in is positive
+    typical_profile = df_grid.Grid_demand - df_grid.Grid_supply  # attention! Supply is negative, feed in is positive
     df = pd.DataFrame(typical_profile, columns=['Grid_profile'])
     df_export = df.copy()
     df_import = df.copy()
     df_export[df_export.Grid_profile < 0] = 0
     df_import[df_import.Grid_profile > 0] = 0
     df_import = -df_import
     return df_export, df_import
 
 
 def return_annual_exports_imports(df_el, df_t):
     df_aim = {}
     df_export = df_el.Grid_demand.mul(df_t.dp, level='Period', axis=0)
     df_import = df_el.Grid_supply.mul(df_t.dp, level='Period', axis=0)
-    df_aim['MWh_imp_el'] = df_import.sum() /1000 #MWh
-    df_aim['MWh_exp'] = df_export.sum() /1000 #MWh
+    df_aim['MWh_imp_el'] = df_import.sum() / 1000  # MWh
+    df_aim['MWh_exp'] = df_export.sum() / 1000  # MWh
     return df_aim['MWh_imp_el'], df_aim['MWh_exp']
 
 
 def get_unit_use_annual_profile(df_unit, df_t, unit, nb_periods):
     df_PV = df_unit[df_unit.index.get_level_values('Unit').str.contains(unit)]
     df_PV = df_PV.groupby('Period').sum()
     df_PV = df_PV.mul(df_t.dp, level='Period', axis=0)
     df_PV = df_PV.loc[0:nb_periods].sum()
     return df_PV
 
 
-def return_correct_OPEX(df_grid,  df_time, total_area):
+def return_correct_OPEX(df_grid, df_time, total_area):
     opex = 0
     for layer in df_grid.groupby(level=[0]).nunique().index:
         df = df_grid.xs((layer, 'Network'), level=('Layer', 'Hub'))
         df_imp, df_exp = return_annual_exports_imports(df, df_time)
         opex = opex + 1000 * (df.Cost_supply.mean() * df_imp - df.Cost_demand.mean() * df_exp)
 
     OPEX_m2 = {'opex_m2': opex / total_area}
@@ -73,20 +74,20 @@
 
 
 def correct_grid_param(df_Grid):
     GM_GU = {}
     df_grid = df_Grid.xs(('Electricity', "Network"), level=('Layer', 'Hub'))[:-2]
     uncontrollable_load = df_Grid.xs("Electricity", level="Layer")["Uncontrollable_load"].drop("Network", level="Hub")
     uncontrollable_load = uncontrollable_load.groupby(level=["Period", "Time"]).sum().max()
-    GM_GU['GUd'] = np.round(np.max(df_grid['Grid_demand'] - df_grid['Grid_supply'])/uncontrollable_load, 2)
-    GM_GU['GUs'] = np.round(np.max(df_grid['Grid_supply'] - df_grid['Grid_demand'])/uncontrollable_load, 2)
+    GM_GU['GUd'] = np.round(np.max(df_grid['Grid_demand'] - df_grid['Grid_supply']) / uncontrollable_load, 2)
+    GM_GU['GUs'] = np.round(np.max(df_grid['Grid_supply'] - df_grid['Grid_demand']) / uncontrollable_load, 2)
 
     df = df_Grid.xs('Electricity', level=0)[['Grid_demand', 'Grid_supply']].xs("Network", level="Hub", drop_level=False)
     df_max = df.groupby(level=['Hub', 'Period']).max()
-    df_mean = df.groupby(level=['Hub', 'Period']).mean().replace(0, 1) # replace 0 with 1 to avoid div by 0,  profiles >0, in case av = 0- whole profile is 0
+    df_mean = df.groupby(level=['Hub', 'Period']).mean().replace(0, 1)  # replace 0 with 1 to avoid div by 0,  profiles >0, in case av = 0- whole profile is 0
     GM = df_max.div(df_mean, level='Hub').max()
 
     GM_GU['GMd'] = np.round(GM["Grid_demand"], 2)
     GM_GU['GMs'] = np.round(GM["Grid_supply"], 2)
 
     return GM_GU
 
@@ -95,44 +96,44 @@
     df_PV = get_unit_use_annual_profile(df_unit, df_t, "PV", nb_periods)
     df_cogen = get_unit_use_annual_profile(df_unit, df_t, "Cogeneration", nb_periods)
     onsite_elec = df_cogen.Units_supply + df_PV.Units_supply
 
     df_el = df_grid.xs(('Electricity', 'Network'), level=('Layer', 'Hub'))
     df_imp, df_exp = return_annual_exports_imports(df_el, df_t)
 
-    df_aim = {}
-    df_aim['SC'] = (onsite_elec - df_exp * 1000) / onsite_elec
-    df_aim['SS'] = (onsite_elec - df_exp * 1000) / (onsite_elec - df_exp * 1000 + df_imp * 1000)
-    df_aim["PVP"] = df_PV.Units_supply / (df_PV.Units_supply - df_exp * 1000 + df_imp * 1000)
-    df_aim["MWh_imp_el"] = df_imp
-    df_aim["MWh_exp"] = df_exp
+    df_aim = {'SC': (onsite_elec - df_exp * 1000) / onsite_elec,
+              'SS': (onsite_elec - df_exp * 1000) / (onsite_elec - df_exp * 1000 + df_imp * 1000),
+              "PVP": df_PV.Units_supply / (df_PV.Units_supply - df_exp * 1000 + df_imp * 1000),
+              "MWh_imp_el": df_imp,
+              "MWh_exp": df_exp}
+
     return df_aim
 
 
 def return_BUI_GWPop(df_grid, surface, df_time, df_KPI):
     df_el = df_grid.xs(('Electricity', 'Network'), level=('Layer', 'Hub'))
     emissions_el_dy = df_el.GWP_supply * df_el.Grid_supply - df_el.GWP_demand * df_el.Grid_demand
-    emissions_el_dy = emissions_el_dy.mul(df_time.dp, level='Period', axis=0).sum()/surface
+    emissions_el_dy = emissions_el_dy.mul(df_time.dp, level='Period', axis=0).sum() / surface
     emissions_el_av = df_el.GWP_supply.mean() * df_el.Grid_supply - df_el.GWP_demand.mean() * df_el.Grid_demand
-    emissions_el_av = emissions_el_av.mul(df_time.dp, level='Period', axis=0).sum()/surface
+    emissions_el_av = emissions_el_av.mul(df_time.dp, level='Period', axis=0).sum() / surface
 
     df_resource = df_grid.xs("Network", level="Hub")
     emissions = df_resource.GWP_supply * df_resource.Grid_supply - df_resource.GWP_demand * df_resource.Grid_demand
     emissions = emissions.mul(df_time.dp, level='Period', axis=0).sum()
 
     gwp_op_m2 = emissions / surface
     gwp_constr_m2 = df_KPI["gwp_constr_m2"].xs("Network")
     gwp_tot_m2 = gwp_op_m2 + gwp_constr_m2
 
-    df_aim = {}
-    df_aim['gwp_elec_av'] = emissions_el_av
-    df_aim['gwp_elec_dy'] = emissions_el_dy
-    df_aim['gwp_op_m2'] = gwp_op_m2
-    df_aim['gwp_constr_m2'] = gwp_constr_m2
-    df_aim['gwp_tot_m2'] = gwp_tot_m2
+    df_aim = {'gwp_elec_av': emissions_el_av,
+              'gwp_elec_dy': emissions_el_dy,
+              'gwp_op_m2': gwp_op_m2,
+              'gwp_constr_m2': gwp_constr_m2,
+              'gwp_tot_m2': gwp_tot_m2}
+
     return df_aim
 
 
 def correct_data_in_reho(results, OPEX_m2, SS_SC, GWP, GM_GU, surface):
     df_KPI = results["df_KPIs"]
     df_KPI.at["Network", "SS"] = SS_SC["SS"]
     df_KPI.at["Network", "SC"] = SS_SC["SC"]
@@ -154,8 +155,8 @@
     df_perf = results["df_Performance"]
     df_perf.at["Network", "Costs_op"] = OPEX_m2["opex_m2"] * surface
     df_perf.at["Network", "GWP_op"] = GWP["gwp_op_m2"] * surface
 
     results["df_Annuals"].at[("Electricity", "Network"), "Demand_MWh"] = SS_SC["MWh_exp"]
     results["df_Annuals"].at[("Electricity", "Network"), "Supply_MWh"] = SS_SC["MWh_imp_el"]
 
-    return results
+    return results
```

### Comparing `REHO-1.0.2/reho/model/postprocessing/write_results.py` & `reho-1.1.0/reho/model/postprocessing/write_results.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,462 +1,491 @@
 import pandas as pd
 import numpy as np
+import logging
 
 __doc__ = """
-*Extracts the results from the AMPL model and converts it to Python dictionary and pandas dataframes.*
+Extracts the results from the AMPL model and converts it to Python dictionary and pandas dataframes.
 """
 
-def get_df_Results_from_SP(ampl, scenario, method, buildings_data, filter=True):
 
-    def set_df_performance(df, ampl, scenario):
-        df1 = get_variable_in_pandas(df, 'Costs_House_op')  # without the comfort penalty costs
+def get_df_Results_from_SP(ampl, scenario, method, buildings_data, filter=True):
+    def set_df_performance(ampl, scenario):
+        df1 = get_ampl_data(ampl, 'Costs_House_op')  # without the comfort penalty costs
         df1 = df1.rename(columns={'Costs_House_op': 'Costs_op'})
 
-        df2 = get_variable_in_pandas(df, 'Costs_House_inv')
+        df2 = get_ampl_data(ampl, 'Costs_House_inv')
         df2 = df2.rename(columns={'Costs_House_inv': 'Costs_inv'})
         tau = ampl.getParameter('tau').getValues().toList()
         df2['Costs_inv'] = df2['Costs_inv'] * tau[0]
         df2['ANN_factor'] = tau[0]
-        df2['Costs_grid_connection'] = get_variable_in_pandas(df, 'Costs_grid_connection_House').groupby(level=1).sum()  # yearly cost for grid connection
 
-        df3 = get_variable_in_pandas(df, 'Costs_House_rep')
+        df2['Costs_grid_connection'] = get_ampl_data(ampl, 'Costs_grid_connection_House', multi_index=True).groupby(
+            level=1).sum()  # yearly cost for grid connection
+
+        df3 = get_ampl_data(ampl, 'Costs_House_rep')
         df3['Costs_House_rep'] = df3['Costs_House_rep'] * tau[0]
         df3 = df3.rename(columns={'Costs_House_rep': 'Costs_rep'})
 
-        df4 = get_variable_in_pandas(df, 'Costs_House_cft')
+        df4 = get_ampl_data(ampl, 'Costs_House_cft')
         df4 = df4.rename(columns={'Costs_House_cft': 'Costs_ft'})
 
-        df5 = get_variable_in_pandas(df, 'GWP_house_op')
+        df5 = get_ampl_data(ampl, 'GWP_house_op')
         df5 = df5.rename(columns={'GWP_house_op': 'GWP_op'})
 
-        df6 = get_variable_in_pandas(df, 'GWP_house_constr')
+        df6 = get_ampl_data(ampl, 'GWP_house_constr')
         df6 = df6.rename(columns={'GWP_house_constr': 'GWP_constr'})
 
-        df71 = get_parameter_in_pandas(ampl, 'EMOO_CAPEX', multi_index=False)
-        df72 = get_parameter_in_pandas(ampl, 'EMOO_OPEX', multi_index=False)
-        df73 = get_parameter_in_pandas(ampl, 'EMOO_TOTEX', multi_index=False)
-        df75 = get_parameter_in_pandas(ampl, 'EMOO_GWP', multi_index=False)
-        df76 = get_parameter_in_pandas(ampl, 'EMOO_grid', multi_index=False)
+        df71 = get_ampl_data(ampl, 'EMOO_CAPEX')
+        df72 = get_ampl_data(ampl, 'EMOO_OPEX')
+        df73 = get_ampl_data(ampl, 'EMOO_TOTEX')
+        df75 = get_ampl_data(ampl, 'EMOO_GWP')
+        df76 = get_ampl_data(ampl, 'EMOO_grid')
 
-        df_N1 = get_variable_in_pandas(df, 'Costs_op')  # without the comfort penalty costs
-        df_N2 = get_variable_in_pandas(df, 'Costs_inv')
+        df_N1 = get_ampl_data(ampl, 'Costs_op')  # without the comfort penalty costs
+        df_N2 = get_ampl_data(ampl, 'Costs_inv')
         df_N2['Costs_inv'] = df_N2['Costs_inv'] * tau[0]
         df_N2['ANN_factor'] = tau[0]
-        df_N2['Costs_grid_connection'] = get_variable_in_pandas(df, 'Costs_grid_connection').sum().values/2  # TODO enhance
-        df_N3 = get_variable_in_pandas(df, 'Costs_rep')
+        df_N2['Costs_grid_connection'] = get_ampl_data(ampl, 'Costs_grid_connection').sum().values / 2  # TODO enhance
+        df_N3 = get_ampl_data(ampl, 'Costs_rep')
         df_N3['Costs_rep'] = df_N3['Costs_rep'] * tau[0]
         df_N4 = pd.DataFrame({'Costs_ft': [df4.sum()['Costs_ft']]})
-        df_N5 = get_variable_in_pandas(df, 'GWP_op')
-        df_N6 = get_variable_in_pandas(df, 'GWP_constr')
+        df_N5 = get_ampl_data(ampl, 'GWP_op')
+        df_N6 = get_ampl_data(ampl, 'GWP_constr')
 
         df_PerformanceBuilding = pd.concat([df1, df2, df3, df4, df5, df6], axis=1)
         df_PerformanceNetwork = pd.concat([df_N1, df_N2, df_N3, df_N4, df_N5, df_N6], axis=1)
         df_PerformanceNetwork = df_PerformanceNetwork.rename(index={0: 'Network'})
 
         df_Performance = pd.concat([df_PerformanceBuilding, df_PerformanceNetwork], axis=0)
 
         df_Epsilon = pd.concat([df71, df72, df73, df75, df76], axis=1)
-        df_Epsilon['Objective'] = get_parameter_in_pandas(ampl, scenario["Objective"], multi_index=False).values[0][0]- df_N4.values[0][0]
+        df_Epsilon['Objective'] = get_ampl_data(ampl, scenario["Objective"]).values[0][0] - df_N4.values[0][0]
         df_Epsilon = df_Epsilon.rename(index={0: 'Network'})
 
         df_Performance = pd.concat([df_Performance, df_Epsilon], axis=1)
         df_Performance.index.names = ['Hub']
-        print(df_Performance)
+        if method['print_logs']:
+            print(df_Performance)
 
         return df_Performance.sort_index()
 
-    def set_df_annuals(df, ampl):
+    def set_df_annuals(ampl):
         # Annuals
-        df1 = get_variable_in_pandas(df, 'AnnualNetwork_demand')
+        df1 = get_ampl_data(ampl, 'AnnualNetwork_demand')
         df1.columns = ['Demand_MWh']
         df1 = pd.concat([df1], keys=['Network'])
         df1.index = df1.index.reorder_levels([1, 0])
-        df2 = get_variable_in_pandas(df, 'AnnualNetwork_supply')
+        df2 = get_ampl_data(ampl, 'AnnualNetwork_supply')
         df2.columns = ['Supply_MWh']
         df2 = pd.concat([df2], keys=['Network'])
         df2.index = df2.index.reorder_levels([1, 0])
         df12 = pd.concat([df1, df2], axis=1, sort=False)
 
-        df3 = get_variable_in_pandas(df, 'AnnualDomestic_electricity')
-        df3 = df3.set_index([pd.Index(["Electricity"]*df3.index.size), df3.index])
+        df3 = get_ampl_data(ampl, 'AnnualDomestic_electricity')
+        df3 = df3.set_index([pd.Index(["Electricity"] * df3.index.size), df3.index])
         df3.columns = ['Demand_MWh']
-        df4 = get_variable_in_pandas(df, 'AnnualHouse_Q')
+        df4 = get_ampl_data(ampl, 'AnnualHouse_Q')
         df4.columns = ['Demand_MWh']
-        df5 = get_variable_in_pandas(df, 'AnnualHeatGainHouse')
+        df5 = get_ampl_data(ampl, 'AnnualHeatGainHouse')
         df5.columns = ['Supply_MWh']
         df5 = pd.concat([df5], keys=['HeatGains'])
-        df6 = get_variable_in_pandas(df, 'AnnualSolarGainHouse')
+        df6 = get_ampl_data(ampl, 'AnnualSolarGainHouse')
         df6.columns = ['Supply_MWh']
         df6 = pd.concat([df6], keys=['SolarGains'])
         df3456 = pd.concat([df3, df4, df5, df6], sort=False)
 
-        df7 = get_variable_in_pandas(df, 'AnnualUnit_in')
+        df7 = get_ampl_data(ampl, 'AnnualUnit_in')
         df7.columns = ['Demand_MWh']
-        df8 = get_variable_in_pandas(df, 'AnnualUnit_out')
+        df8 = get_ampl_data(ampl, 'AnnualUnit_out')
         df8.columns = ['Supply_MWh']
         df78 = pd.concat([df7, df8], axis=1, sort=False)
-        df9 = get_variable_in_pandas(df, 'AnnualUnit_Q')
+        df9 = get_ampl_data(ampl, 'AnnualUnit_Q')
         df9.columns = ['Supply_MWh']
         df789 = pd.concat([df78, df9], sort=False)
 
         df_Annuals = pd.concat([df12, df3456, df789], sort=False)
         df_Annuals.index.names = ['Layer', 'Hub']
 
         # Correction of DHW layer
         hubs = [s for s in df_Annuals.index.levels[1] if s.startswith("Building")]
         for h in hubs:
             df_Annuals.loc[('DHW', h), 'Demand_MWh'] = df_Annuals.loc[('DHW', 'WaterTankDHW_' + h), 'Supply_MWh']
 
         return df_Annuals
 
-    def set_df_buildings(buildings_data, df, ampl):
+    def set_df_buildings(buildings_data):
         # Building
         df_Buildings = pd.DataFrame.from_dict(buildings_data, orient='index')
         df_Buildings.index.names = ['Hub']
         for item in ['x', 'y', 'z', 'geometry']:
             if item in df_Buildings.columns:
                 df_Buildings.drop([item], axis=1)
 
         return df_Buildings.sort_index()
 
-    def set_df_unit(df, ampl):
+    def set_df_unit(ampl):
         # Unit
         tau = ampl.getParameter('tau').getValues().toList()
-        df1 = get_variable_in_pandas(df, 'Units_Use')
-        df2 = get_variable_in_pandas(df, 'Units_Mult')
+        df1 = get_ampl_data(ampl, 'Units_Use')
+        df2 = get_ampl_data(ampl, 'Units_Mult')
 
-        df3 = tau[0] * get_variable_in_pandas(df, 'Costs_Unit_inv')
-        df4 = get_variable_in_pandas(df, 'GWP_Unit_constr') # per year! For total- multiply with lifetime
-        df5 = get_parameter_in_pandas(ampl, 'lifetime', multi_index=False)
+        df3 = tau[0] * get_ampl_data(ampl, 'Costs_Unit_inv')
+        df4 = get_ampl_data(ampl, 'GWP_Unit_constr')  # per year! For total, multiply with lifetime
+        df5 = get_ampl_data(ampl, 'lifetime')
         df_Unit = pd.concat([df1, df2, df3, df4, df5], axis=1)
         df_Unit.index.names = ['Unit']
         df_Unit = df_Unit.sort_index()
-        print(df_Unit)
+        if method['print_logs']:
+            print(df_Unit)
 
         # Unit_t
-        df1 = get_variable_in_pandas(df, 'Units_demand')
-        df2 = get_variable_in_pandas(df, 'Units_supply')
-        df3 = get_variable_in_pandas(df, 'Units_curtailment')
-        df4 = get_variable_in_pandas(df, 'BAT_E_stored')
+        df1 = get_ampl_data(ampl, 'Units_demand', multi_index=True)
+        df2 = get_ampl_data(ampl, 'Units_supply', multi_index=True)
+        df3 = get_ampl_data(ampl, 'Units_curtailment', multi_index=True)
+        df4 = get_ampl_data(ampl, 'BAT_E_stored', multi_index=True)
         df4 = pd.concat([df4], keys=['Electricity'], names=['Layer'])
         if "EV_district" in [unit for unit, value in ampl.getVariable('Units_Use').instances()]:
-            df5 = get_variable_in_pandas(df, 'EV_E_stored')
+            df5 = get_ampl_data(ampl, 'EV_E_stored', multi_index=True)
             df5 = pd.concat([df5], keys=['Electricity'], names=['Layer'])
-            df6 = get_parameter_in_pandas(ampl, "EV_displacement", multi_index=True)
+            df6 = get_ampl_data(ampl, "EV_displacement", multi_index=True)
             df6 = pd.concat([df6], keys=['Electricity'], names=['Layer'])
             df_Unit_t = pd.concat([df1, df2, df3, df4, df5, df6], axis=1)
         else:
             df_Unit_t = pd.concat([df1, df2, df3, df4], axis=1)
         df_Unit_t.index.names = ['Layer', 'Unit', 'Period', 'Time']
         df_Unit_t = df_Unit_t.sort_index()
 
         return df_Unit, df_Unit_t
 
-    def set_df_grid(df, ampl):
+    def set_df_grid(ampl, method):
         # Grid_t
-        df1 = get_variable_in_pandas(df, 'Grid_demand')
-        df2 = get_variable_in_pandas(df, 'Grid_supply')
-        df_cs = get_parameter_in_pandas(ampl, 'Cost_supply', multi_index=True)
+        df1 = get_ampl_data(ampl, 'Grid_demand', multi_index=True)
+        df2 = get_ampl_data(ampl, 'Grid_supply', multi_index=True)
+
+        df_cs = get_ampl_data(ampl, 'Cost_supply', multi_index=True)
         df_cs = df_cs.reorder_levels((1, 0, 2, 3))
-        df_cd = get_parameter_in_pandas(ampl, 'Cost_demand', multi_index=True)
+        df_cd = get_ampl_data(ampl, 'Cost_demand', multi_index=True)
         df_cd = df_cd.reorder_levels((1, 0, 2, 3))
-        df_electricity = get_parameter_in_pandas(ampl, 'Domestic_electricity', multi_index=True)
+
+        df_electricity = get_ampl_data(ampl, 'Domestic_electricity', multi_index=True)
         df_electricity.columns = ['Uncontrollable_load']
-        df_electricity = df_electricity.set_index([pd.Index(["Electricity"]*df_electricity.index.size), df_electricity.index])
-        df12 = pd.concat([df1, df2, df_cs, df_cd, df_electricity], axis=1)
+        df_electricity = df_electricity.set_index([pd.Index(["Electricity"] * df_electricity.index.size), df_electricity.index])
 
-        df3 = get_variable_in_pandas(df, 'Network_demand')
-        df4 = get_variable_in_pandas(df, 'Network_supply')
-        df_cs = get_parameter_in_pandas(ampl, 'Cost_supply_network', multi_index=True)
-        df_cd = get_parameter_in_pandas(ampl, 'Cost_demand_network', multi_index=True)
-        df_es = get_parameter_in_pandas(ampl, 'GWP_supply', multi_index=True)
-        df_ed = get_parameter_in_pandas(ampl, 'GWP_demand', multi_index=True)
-
-        # Rename Network to Grid and therefore add Level 'Hub' = Network
-        df3.columns = ['Grid_demand']
-        df4.columns = ['Grid_supply']
-        df_cs.columns = ['Cost_supply']
-        df_cd.columns = ['Cost_demand']
-
-        df34 = pd.concat([df3, df4, df_cs, df_cd, df_es, df_ed], axis=1)
-
-        df34['Hub'] = 'Network'
-        df34.set_index('Hub', append=True, inplace=True)
-        df34 = df34.reorder_levels((0, 3, 1, 2))
-        # combine Network & Grid dataframe
-        df_Grid_t = pd.concat([df12, df34], sort=True)
-        df_Grid_t.index.names = ['Layer', 'Hub', 'Period', 'Time']
+        df_es = get_ampl_data(ampl, 'GWP_supply', multi_index=True)
+        df_ed = get_ampl_data(ampl, 'GWP_demand', multi_index=True)
+        df_em = pd.concat([df_es, df_ed], axis=1)
+        df_em_tot = pd.DataFrame()
+        for bui in df1.index.get_level_values(1).unique():
+            df = df_em
+            df["Hub"] = bui
+            df_em_tot = pd.concat([df_em_tot, df])
+        df_em_tot.set_index('Hub', append=True, inplace=True)
+        df_em_tot = df_em_tot.reorder_levels((0, 3, 1, 2))
+
+        df_Grid_t = pd.concat([df1, df2, df_cs, df_cd, df_em_tot, df_electricity], axis=1)
+
+        if not method["district-scale"] or not method["district-scale"]:
+            df3 = get_ampl_data(ampl, 'Network_demand', multi_index=True)
+            df3.columns = ['Grid_demand']
+            df4 = get_ampl_data(ampl, 'Network_supply', multi_index=True)
+            df4.columns = ['Grid_supply']
+            df_cs_net = get_ampl_data(ampl, 'Cost_supply_network', multi_index=True)
+            df_cs_net.columns = ['Cost_supply']
+            df_cd_net = get_ampl_data(ampl, 'Cost_demand_network', multi_index=True)
+            df_cd_net.columns = ['Cost_demand']
+
+            df_electricity_net = df_electricity.groupby(level=(0, 2, 3)).sum()
+            df34 = pd.concat([df3, df4, df_cs_net, df_cd_net, df_es, df_ed, df_electricity_net], axis=1)
+            df34['Hub'] = 'Network'
+            df34.set_index('Hub', append=True, inplace=True)
+            df34 = df34.reorder_levels((0, 3, 1, 2))
+            df_Grid_t = pd.concat([df_Grid_t, df34])
 
+        df_Grid_t.index.names = ['Layer', 'Hub', 'Period', 'Time']
         return df_Grid_t.sort_index()
 
-    def set_df_buildings_t(df, ampl):
+    def set_df_buildings_t(ampl):
         # Building_t
-        df1 = get_parameter_in_pandas(ampl, 'Domestic_electricity', multi_index=True)
+        df1 = get_ampl_data(ampl, 'Domestic_electricity', multi_index=True)
 
-        m_DWH = get_parameter_in_pandas(ampl, 'DHW_flowrate', multi_index=True)
-        delta_T = get_parameter_in_pandas(ampl, 'DHW_dT', multi_index=False).iloc[0,0]
-        df2 = 4.18*m_DWH*delta_T/3600
+        m_DWH = get_ampl_data(ampl, 'DHW_flowrate', multi_index=True)
+        delta_T = get_ampl_data(ampl, 'DHW_dT').iloc[0, 0]
+        df2 = 4.18 * m_DWH * delta_T / 3600
         df2 = df2.rename(columns={'DHW_flowrate': 'House_Q_DHW'})
 
-        df31 = get_parameter_in_pandas(ampl, 'T_in', multi_index=True)
-        df32 = get_variable_in_pandas(df, 'House_Q_heating')
-        df33 = get_variable_in_pandas(df, 'House_Q_cooling')
-        df34 = get_parameter_in_pandas(ampl, 'Th_supply', multi_index=True)
-        df35 = get_parameter_in_pandas(ampl, 'Th_return', multi_index=True)
+        df31 = get_ampl_data(ampl, 'T_in', multi_index=True)
+        df32 = get_ampl_data(ampl, 'House_Q_heating')
+        df33 = get_ampl_data(ampl, 'House_Q_cooling')
+        df34 = get_ampl_data(ampl, 'Th_supply', multi_index=True)
+        df35 = get_ampl_data(ampl, 'Th_return', multi_index=True)
 
-        df4 = get_parameter_in_pandas(ampl, 'HeatGains', multi_index=True)
-        df5 = get_parameter_in_pandas(ampl, 'SolarGains', multi_index=True)
+        df4 = get_ampl_data(ampl, 'HeatGains', multi_index=True)
+        df5 = get_ampl_data(ampl, 'SolarGains', multi_index=True)
 
         df_Buildings_t = pd.concat([df1, df2, df31, df32, df33, df34, df35, df4, df5], axis=1)
         df_Buildings_t.index.names = ['Hub', 'Period', 'Time']
 
         return df_Buildings_t.sort_index()
 
-    def set_df_stream_t(df, ampl):
+    def set_df_streams_t(ampl):
 
-        df_Q = get_variable_in_pandas(df, 'Streams_Q')
+        df_Q = get_ampl_data(ampl, 'Streams_Q', multi_index=True)
         df_Q.index.set_names(['Service', 'Stream', 'Period', 'Time'], inplace=True)
 
-        df1 = get_variable_in_pandas(df, 'HC_Streams_Mult')
+        df1 = get_ampl_data(ampl, 'HC_Streams_Mult', multi_index=True)
         df1.index.set_names(['Service', 'Stream', 'Period', 'Time'], inplace=True)
-        df2 = get_parameter_in_pandas(ampl, 'Streams_Mcp', multi_index=True)
+        df2 = get_ampl_data(ampl, 'Streams_Mcp', multi_index=True)
         df2.index.set_names(['Stream', 'Period', 'Time'], inplace=True)
         df_mcp = df1['HC_Streams_Mult'].mul(df2['Streams_Mcp'])
         df_mcp = pd.DataFrame(df_mcp, columns=['Streams_Mcp_kW/K']).sort_index()
 
         dict = {}
         for a, b in ampl.getSet('StreamsOfUnit').instances():
             dict[a] = b.getValues().toPandas().index.to_list()
         df_dict = pd.DataFrame.from_dict(dict, orient='index')
 
-        df_Tin = get_parameter_in_pandas(ampl, 'Streams_Tin', multi_index=True)
-        df_Tout = get_parameter_in_pandas(ampl, 'Streams_Tout', multi_index=True)
+        df_Tin = get_ampl_data(ampl, 'Streams_Tin', multi_index=True)
+        df_Tout = get_ampl_data(ampl, 'Streams_Tout', multi_index=True)
 
         df_Tin.index.set_names(['Stream', 'Period', 'Time'], inplace=True)
         df_Tout.index.set_names(['Stream', 'Period', 'Time'], inplace=True)
 
-        df_Tmin = get_parameter_in_pandas(ampl, 'dTmin', multi_index=False)
+        df_Tmin = get_ampl_data(ampl, 'dTmin')
         df_Tmin.index.set_names('Stream', inplace=True)
 
         df_Q = df_Q.reset_index('Service', drop=False)
         df_Q = df_Q.join([df_Tin, df_Tout]).set_index('Service', append=True)
         df_Q = df_Q.merge(df_mcp, left_index=True, right_on=['Stream', 'Period', 'Time', 'Service'])
         df_Q = df_Q.reorder_levels([3, 0, 1, 2]).sort_index()
 
         df_dict = df_dict.unstack()
         df_dict.dropna(inplace=True)
         df_dict = df_dict.reset_index().set_index(0)
         df_dict.drop(columns='level_0', inplace=True)
         df_dict.index.set_names(['Stream'], inplace=True)
         df_dict.rename(columns={'level_1': 'Unit'}, inplace=True)
 
-        df_Stream_t = df_Q.reset_index().set_index('Stream')
-        df_Stream_t = df_Stream_t.join([df_dict, df_Tmin]).set_index(['Service', 'Unit', 'Period', 'Time'], append=True)
+        df_Streams_t = df_Q.reset_index().set_index('Stream')
+        df_Streams_t = df_Streams_t.join([df_dict, df_Tmin]).set_index(['Service', 'Unit', 'Period', 'Time'], append=True)
 
-        return df_Stream_t.sort_index()
+        return df_Streams_t.sort_index()
 
-    def set_dfs_lca(df, ampl):
+    def set_dfs_lca(ampl):
 
-        LCA_units = get_variable_in_pandas(df, 'lca_units')
+        LCA_units = get_ampl_data(ampl, 'lca_units')
         LCA_units = LCA_units.stack().unstack(level=0).droplevel(level=1)
 
-        LCA_tot = get_variable_in_pandas(df, 'lca_tot')
+        LCA_tot = get_ampl_data(ampl, 'lca_tot')
         LCA_tot = LCA_tot.stack().unstack(level=0)
         LCA_tot.index = ["Network"]
-        LCA_tot_house = get_variable_in_pandas(df, 'lca_tot_house')
+        LCA_tot_house = get_ampl_data(ampl, 'lca_tot_house')
         LCA_tot_house = LCA_tot_house.stack().unstack(level=0).droplevel(1)
         LCA_tot = pd.concat([LCA_tot_house, LCA_tot], axis=0)
         LCA_tot.index.names = ['Hub']
 
-        LCA_op = get_variable_in_pandas(df, 'lca_op')
+        LCA_op = get_ampl_data(ampl, 'lca_op')
         LCA_op = LCA_op.stack().unstack(level=0).droplevel(level=1)
 
         return LCA_units, LCA_tot, LCA_op
 
-    def set_dfs_pv(df, ampl):
+    def set_dfs_pv(ampl):
 
         # PV_Surface
-        df_PV_Surface = get_parameter_in_pandas(ampl, "HouseSurfaceArea", multi_index=True)
+        df_PV_Surface = get_ampl_data(ampl, "HouseSurfaceArea", multi_index=True)
         df_PV_Surface.index.names = ['Hub', 'Surface']
         df_PV_Surface.rename(columns={'HouseSurfaceArea': 'Area'})
         df_PV_Surface = df_PV_Surface.sort_index()
 
         # ["df_PV_orientation"]
-        df_PVA_module_nbr = get_variable_in_pandas(df, 'PVA_module_nbr')
+        df_PVA_module_nbr = get_ampl_data(ampl, 'PVA_module_nbr', multi_index=True)
         df_PVA_module_nbr = df_PVA_module_nbr.droplevel(4)
         df_PVA_module_nbr.index.names = ['Hub', 'Surface', 'Azimuth', 'Tilt']
-        #int_index = df_PVA_module_nbr.index.get_level_values('Surface').astype(int)
-        #df_PVA_module_nbr.index.set_levels(int_index, level="Surface", inplace=True)
+        # int_index = df_PVA_module_nbr.index.get_level_values('Surface').astype(int)
+        # df_PVA_module_nbr.index.set_levels(int_index, level="Surface", inplace=True)
 
-        df_PVA_module_coverage = get_parameter_in_pandas(ampl, "PVA_module_coverage", multi_index=True)
+        df_PVA_module_coverage = get_ampl_data(ampl, "PVA_module_coverage", multi_index=True)
         df_PVA_module_coverage = df_PVA_module_coverage.droplevel(1)
         df_PVA_module_coverage.index.names = ['Hub', 'Surface', 'Azimuth', 'Tilt']
 
         pd.concat([df_PVA_module_coverage, df_PVA_module_nbr], axis=1)
 
-
-        df_unshaded_share = get_parameter_in_pandas(ampl, 'unshaded_share', multi_index=True)
+        df_unshaded_share = get_ampl_data(ampl, 'unshaded_share', multi_index=True)
         df_unshaded_share = df_unshaded_share.groupby(level=[0, 1, 2, 3]).sum()
         df_unshaded_share = df_unshaded_share.div(145)  # 145 patches in skydome
         df_unshaded_share.index.names = ['Hub', 'Surface', 'Azimuth', 'Tilt']
 
         df_PV_orientation = pd.concat([df_PVA_module_coverage, df_unshaded_share, df_PVA_module_nbr], axis=1)
         # df_PV_Surface_profiles
         # centralized optimization PV_electricity takes a lot of memory -> TODO move to annuals profiles are not needed
-        # df_PV_Surface_profiles = get_variable_in_pandas(df, "PV_electricity")
-        # df_PV_Surface_loss = get_variable_in_pandas(df, "PV_electricity_without_loss")
+        # df_PV_Surface_profiles = get_ampl_data(ampl, "PV_electricity")
+        # df_PV_Surface_loss = get_ampl_data(ampl, "PV_electricity_without_loss")
         # df_PV_Surface_profiles = pd.concat([df_PV_Surface_profiles, df_PV_Surface_loss], axis=1)
         # df_PV_Surface_profiles.index.names = ['Hub','Unit','Surface', 'Azimuth','Tilt', 'Period', 'Time']
         # df_Results["df_PV_Surface"]_profiles = df_PV_Surface_profiles.sort_index()
 
         return df_PV_Surface, df_PV_orientation
 
-    def set_dfs_other(df, ampl):
+    def set_dfs_other(ampl):
         # Time
-        df1 = get_parameter_in_pandas(ampl, 'dp', multi_index=False)
-        df2 = get_parameter_in_pandas(ampl, 'TimeEnd', multi_index=False)
-        df3 = get_parameter_in_pandas(ampl, 'dt', multi_index=False)
+        df1 = get_ampl_data(ampl, 'dp')
+        df2 = get_ampl_data(ampl, 'TimeEnd')
+        df3 = get_ampl_data(ampl, 'dt')
         df_Time = pd.concat([df1, df2, df3], axis=1)
         df_Time.index.names = ['Period']
         df_Time = df_Time.sort_index()
 
         # External
-        df1 = get_parameter_in_pandas(ampl, 'T_ext', multi_index=True)
-        df2 = get_parameter_in_pandas(ampl, 'I_global', multi_index=True)
-        df_External = pd.concat([df1, df2], axis=1)
-        df_External.index.names = ['Period', 'Time']
-        df_External = df_External.sort_index()
+        df1 = get_ampl_data(ampl, 'T_ext', multi_index=True)
+        df2 = get_ampl_data(ampl, 'I_global', multi_index=True)
+        df_Weather = pd.concat([df1, df2], axis=1)
+        df_Weather.index.names = ['Period', 'Time']
+        df_Weather = df_Weather.sort_index()
 
         # Index
-        df_Index = get_parameter_in_pandas(ampl, 'PeriodOfYear', multi_index=False)
+        df_Index = get_ampl_data(ampl, 'PeriodOfYear')
         df_Index.index.names = ['HourOfYear']
         df_Index = df_Index.sort_index()
 
-        return df_Time, df_External, df_Index
+        return df_Time, df_Weather, df_Index
 
     df_Results = dict()
-    df = ampl.getData("{j in 1.._nvars} (_varname[j],_var[j])").toPandas()
-    df.columns = ["Varname", "Value"]
-    df_Results["df_Performance"] = set_df_performance(df, ampl, scenario)
-    df_Results["df_Annuals"] = set_df_annuals(df, ampl)
-    df_Results["df_Buildings"] = set_df_buildings(buildings_data, df, ampl)
-    df_Results["df_Unit"], df_Results["df_Unit_t"] = set_df_unit(df, ampl)
-    df_Results["df_Grid_t"] = set_df_grid(df, ampl)
-    df_Results["df_Buildings_t"] = set_df_buildings_t(df, ampl)
-    df_Results["df_Time"], df_Results["df_External"], df_Results["df_Index"] = set_dfs_other(df, ampl)
-    if method['save_stream_t']:
-        df_Results["df_Stream_t"] = set_df_stream_t(df, ampl)
+    df_Results["df_Performance"] = set_df_performance(ampl, scenario)
+    df_Results["df_Annuals"] = set_df_annuals(ampl)
+    df_Results["df_Unit"], df_Unit_t = set_df_unit(ampl)
+    df_Results["df_Grid_t"] = set_df_grid(ampl, method)
+    df_Results["df_Time"], df_Weather, df_Index = set_dfs_other(ampl)
+
+    if method['save_data_input']:
+        df_Results["df_Buildings"] = set_df_buildings(buildings_data)
+        df_Results["df_Weather"] = df_Weather
+        df_Results["df_Index"] = df_Index
+
+    if method["save_timeseries"]:
+        df_Results["df_Buildings_t"] = set_df_buildings_t(ampl)
+        df_Results["df_Unit_t"] = df_Unit_t
+    else:
+        for i in ['Cost_demand', 'Cost_supply', 'GWP_demand', 'GWP_supply', "Uncontrollable_load"]:
+            del df_Results["df_Grid_t"][i]
+
+    if method["save_streams"]:
+        df_Results["df_Streams_t"] = set_df_streams_t(ampl)
+
     if method['save_lca']:
-        df_Results["df_lca_Units"], df_Results["df_lca_Performance"], df_Results["df_lca_operation"] = set_dfs_lca(df, ampl)
+        df_Results["df_lca_Units"], df_Results["df_lca_Performance"], df_Results["df_lca_operation"] = set_dfs_lca(ampl)
     if method['use_pv_orientation'] or method['use_facades']:
-        df_Results["df_PV_Surface"], df_Results["df_PV_orientation"] = set_dfs_pv(df, ampl)
+        df_Results["df_PV_Surface"], df_Results["df_PV_orientation"] = set_dfs_pv(ampl)
     if method["extract_parameters"]:
         parameters_record = {}
         for p, ampl_obj in ampl.getParameters():
             try:
                 parameters_record[p] = ampl.getData(p).toPandas()
             except:
-                print(p)
+                logging.info(p)
 
     if filter:
         for df_name, df in df_Results.items():
             df = df.fillna(0)  # replace all NaN with zeros
             df = df.loc[~(df == 0).all(axis=1)]  # drop all lines with only zeros
 
     return df_Results
 
 
-def get_df_Results_from_MP(ampl, binary=False, method=None, district=None, read_DHN=False):
-
+def get_df_Results_from_MP(ampl, binary=False, method=None, district=None, read_DHN=False, scenario={}):
     df_Results = dict()
-    df = ampl.getData("{j in 1.._nvars} (_varname[j],_var[j])").toPandas()
-    df.columns = ["Varname", "Value"]
 
     # Dantzig Wolfe algorithm
-    df1 = get_variable_in_pandas(df, 'lambda')
+    df1 = get_ampl_data(ampl, 'lambda', multi_index=True)
     df_DW = pd.concat([df1], axis=1)
     df_DW.index.names = ['FeasibleSolution', 'Hub']
     df_Results["df_DW"] = df_DW.sort_index()
 
-    # Building_t
-    df1 = get_parameter_in_pandas(ampl, 'Grid_supply', multi_index=True)
-    df2 = get_parameter_in_pandas(ampl, 'Grid_demand', multi_index=True)
-    df_Buildings_t = pd.concat([df1, df2], axis=1)
-    if read_DHN:
-        df3 = get_parameter_in_pandas(ampl, 'flowrate_out', multi_index=True)
-        df3 = pd.concat({'Heat': df3})
-        df4 = get_parameter_in_pandas(ampl, 'flowrate_in', multi_index=True)
-        df4 = pd.concat({'Heat': df4})
-        df_Buildings_t = pd.concat([df_Buildings_t, df3, df4], axis=1)
-    df_Buildings_t.index.names = ['Layer', 'FeasibleSolution', 'Hub', 'Period', 'Time']
-    df_Results["df_Buildings_t"] = df_Buildings_t.sort_index()
-
-    # Building
-    df1 = get_parameter_in_pandas(ampl, 'Costs_inv_rep_SPs', multi_index=True)
-    df2 = get_parameter_in_pandas(ampl, 'Costs_ft_SPs', multi_index=True)
-    df_Buildings = pd.concat([df1, df2], axis=1)
-    df_Buildings.index.names = ['FeasibleSolution', 'Hub']
-    df_Results["df_Buildings"] = df_Buildings.sort_index()
+    if method["save_data_input"] or binary:
+        # Building_t
+        df1 = get_ampl_data(ampl, 'Grid_supply', multi_index=True)
+        df2 = get_ampl_data(ampl, 'Grid_demand', multi_index=True)
+        df_Buildings_t = pd.concat([df1, df2], axis=1)
+        if read_DHN:
+            df3 = get_ampl_data(ampl, 'flowrate_out', multi_index=True)
+            df3 = pd.concat({'Heat': df3})
+            df4 = get_ampl_data(ampl, 'flowrate_in', multi_index=True)
+            df4 = pd.concat({'Heat': df4})
+            df_Buildings_t = pd.concat([df_Buildings_t, df3, df4], axis=1)
+        df_Buildings_t.index.names = ['Layer', 'FeasibleSolution', 'Hub', 'Period', 'Time']
+        df_Results["df_Buildings_t"] = df_Buildings_t.sort_index()
+
+        # Building
+        df1 = get_ampl_data(ampl, 'Costs_inv_rep_SPs', multi_index=True)
+        df2 = get_ampl_data(ampl, 'Costs_ft_SPs', multi_index=True)
+        df_Buildings = pd.concat([df1, df2], axis=1)
+        df_Buildings.index.names = ['FeasibleSolution', 'Hub']
+        df_Results["df_Buildings"] = df_Buildings.sort_index()
 
     # District
-    df1 = get_variable_in_pandas(df, 'Costs_House_op')
-    df2 = get_variable_in_pandas(df, 'Costs_House_inv')
-    df3 = get_variable_in_pandas(df, 'Costs_House_cft')
+    df1 = get_ampl_data(ampl, 'Costs_House_op')
+    df2 = get_ampl_data(ampl, 'Costs_House_inv')
+    df3 = get_ampl_data(ampl, 'Costs_House_cft')
     df4 = df1.values + df2
     df4.columns = ["Costs_House_tot"]
-    df5 = get_variable_in_pandas(df, 'GWP_House_op')
-    df6 = get_variable_in_pandas(df, 'GWP_House_constr')
+    df5 = get_ampl_data(ampl, 'GWP_House_op')
+    df6 = get_ampl_data(ampl, 'GWP_House_constr')
     df_House = pd.concat([df1, df2, df3, df4, df5, df6], axis=1)
     df_House.columns = ["Costs_op", "Costs_inv", "Costs_cft", "Costs_tot", "GWP_op", "GWP_constr"]
     if read_DHN:
-        df7 = get_variable_in_pandas(df, 'diameter_max')
-        df8 = get_variable_in_pandas(df, 'DHN_inv_house')
+        df7 = get_ampl_data(ampl, 'diameter_max')
+        df8 = get_ampl_data(ampl, 'DHN_inv_house')
         df8.columns = ["DHN_inv"]
-        df9 = get_variable_in_pandas(df, 'flowrate_max')
+        df9 = get_ampl_data(ampl, 'flowrate_max')
         df_House = pd.concat([df_House, df7, df8, df9], axis=1)
 
-
-    df1 = get_variable_in_pandas(df, 'Costs_op')
-    df2 = get_variable_in_pandas(df, 'Costs_inv')  # with comfort costs
-    df3 = get_variable_in_pandas(df, 'Costs_cft')  # with comfort costs
-    df4 = get_variable_in_pandas(df, 'Costs_tot')  # with comfort costs
-    df5 = get_variable_in_pandas(df, 'GWP_op')
-    df6 = get_variable_in_pandas(df, 'GWP_constr')
+    df1 = get_ampl_data(ampl, 'Costs_op')
+    df2 = get_ampl_data(ampl, 'Costs_inv')  # with comfort costs
+    df3 = get_ampl_data(ampl, 'Costs_cft')  # with comfort costs
+    df4 = get_ampl_data(ampl, 'Costs_tot')  # with comfort costs
+    df5 = get_ampl_data(ampl, 'GWP_op')
+    df6 = get_ampl_data(ampl, 'GWP_constr')
     df_District = pd.concat([df1, df2, df3, df4, df5, df6], axis=1)
     if read_DHN:
-        df7 = np.sqrt(np.sum(df_House[["diameter_max"]]**2)).to_frame().transpose()
-        df8 = get_variable_in_pandas(df, 'DHN_inv')
+        df7 = np.sqrt(np.sum(df_House[["diameter_max"]] ** 2)).to_frame().transpose()
+        df8 = get_ampl_data(ampl, 'DHN_inv')
         df_District = pd.concat([df_District, df7, df8], axis=1)
     df_District = df_District.set_index(pd.Index(["Network"]))
     df_District = pd.concat([df_House, df_District], axis=0)
     df_District.index.names = ['Hub']
     df_Results["df_District"] = df_District.sort_index()
 
     # df_beta
-    df1 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_CAPEX_constraint', False)
-    df1.columns = ['CAPEX']
-    df2 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_OPEX_constraint', False)
-    df2.columns = ['OPEX']
-    df3 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_GWP_constraint', False)
-    df3.columns = ['GWP']
-    df4 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_TOTEX_constraint', False)
-    df4.columns = ['TOTEX']
-    df_beta = pd.concat([df1, df2, df3, df4], axis=1).stack().droplevel(0)
-    df_beta = pd.DataFrame(df_beta, columns=['beta'])
-    df5 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_lca_constraint', False)
-    df5.columns = ['beta']
-    df_Results["df_beta"] = pd.concat([df_beta, df5])
+    emoo_keys = ["EMOO_CAPEX", "EMOO_OPEX", "EMOO_GWP", "EMOO_TOTEX", "EMOO_lca"]
+    list_keys = [i for i in scenario["EMOO"].keys() if i in emoo_keys]
+    if not list_keys:
+        df = pd.DataFrame([0.0] * 16)
+        df.index = ['CAPEX', 'OPEX', 'GWP', 'TOTEX'] + list(get_ampl_data(ampl, 'Lca_kpi').index)
+        df.columns = ["beta"]
+        df_Results["df_beta"] = df
+    else:
+        df1 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_CAPEX_constraint', False)
+        df1.columns = ['CAPEX']
+        df2 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_OPEX_constraint', False)
+        df2.columns = ['OPEX']
+        df3 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_GWP_constraint', False)
+        df3.columns = ['GWP']
+        df4 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_TOTEX_constraint', False)
+        df4.columns = ['TOTEX']
+        df_beta = pd.concat([df1, df2, df3, df4], axis=1).stack().droplevel(0)
+        df_beta = pd.DataFrame(df_beta, columns=['beta'])
+        df5 = get_ampl_dual_values_in_pandas(ampl, 'EMOO_lca_constraint', False)
+        df5.columns = ['beta']
+        df_Results["df_beta"] = pd.concat([df_beta, df5])
 
     # District_t
-    df1 = get_parameter_in_pandas(ampl, 'Cost_demand_network', multi_index=True)
-    df2 = get_parameter_in_pandas(ampl, 'Cost_supply_network', multi_index=True)
-    df3 = get_parameter_in_pandas(ampl, 'GWP_demand', multi_index=True)
-    df4 = get_parameter_in_pandas(ampl, 'GWP_supply', multi_index=True)
-    df5 = get_variable_in_pandas(df, 'Network_supply')
-    df6 = get_variable_in_pandas(df, 'Network_demand')
+    df1 = get_ampl_data(ampl, 'Cost_demand_network', multi_index=True)
+    df2 = get_ampl_data(ampl, 'Cost_supply_network', multi_index=True)
+    df3 = get_ampl_data(ampl, 'GWP_demand', multi_index=True)
+    df4 = get_ampl_data(ampl, 'GWP_supply', multi_index=True)
+    df5 = get_ampl_data(ampl, 'Network_supply', multi_index=True)
+    df6 = get_ampl_data(ampl, 'Network_demand', multi_index=True)
 
     if binary:
         df_District_t = pd.concat([df1, df2, df3, df4, df5, df6], axis=1).sort_index()
     else:
         df_District_t = pd.concat([df5, df6], axis=1)
     df_District_t.index.names = ['Layer', 'Period', 'Time']
     df_Results["df_District_t"] = df_District_t.sort_index()
@@ -478,130 +507,104 @@
     df4.columns = ['gamma_supply']
     df_Dual_t = pd.concat([df1, df2, df3, df4], axis=1)
     df_Dual_t.index.names = ['Layer', 'Period', 'Time']
     df_Results["df_Dual_t"] = df_Dual_t.sort_index()
 
     # Unit
     tau = ampl.getParameter('tau').getValues().toList()  # annuality factor
-    df1 = get_variable_in_pandas(df, 'Units_Use')
-    df2 = get_variable_in_pandas(df, 'Units_Mult')
-    df3 = tau[0] * get_variable_in_pandas(df, 'Costs_Unit_inv')
-    df4 = get_variable_in_pandas(df, 'GWP_Unit_constr')  # per year! For total - multiply with lifetime
-    df5 = get_parameter_in_pandas(ampl, 'lifetime', multi_index=False)
+    df1 = get_ampl_data(ampl, 'Units_Use')
+    df2 = get_ampl_data(ampl, 'Units_Mult')
+    df3 = tau[0] * get_ampl_data(ampl, 'Costs_Unit_inv')
+    df4 = get_ampl_data(ampl, 'GWP_Unit_constr')  # per year! For total - multiply with lifetime
+    df5 = get_ampl_data(ampl, 'lifetime')
     df_Unit = pd.concat([df1, df2, df3, df4, df5], axis=1)
     if read_DHN:
-        df_DHN = pd.DataFrame([[1, 1, get_variable_in_pandas(df, 'DHN_inv')["DHN_inv"][0], 0, 0]], index=["DHN"], columns=df_Unit.columns)
+        df_DHN = pd.DataFrame([[1, 1, get_ampl_data(ampl, 'DHN_inv')["DHN_inv"][0], 0, 0]], index=["DHN"], columns=df_Unit.columns)
         df_Unit = pd.concat([df_Unit, df_DHN], axis=0)
     df_Unit.index.names = ['Unit']
     df_Results["df_Unit"] = df_Unit.sort_index()
-    print(df_Results["df_Unit"])
 
     # Unit_t
-    df1 = get_variable_in_pandas(df, 'Units_demand')
-    df2 = get_variable_in_pandas(df, 'Units_supply')
-    df3 = get_variable_in_pandas(df, 'BAT_E_stored')
+    df1 = get_ampl_data(ampl, 'Units_demand', multi_index=True)
+    df2 = get_ampl_data(ampl, 'Units_supply', multi_index=True)
+    df3 = get_ampl_data(ampl, 'BAT_E_stored', multi_index=True)
     df3 = pd.concat([df3], keys=['Electricity'], names=['Layer'])
     df_Unit_t = pd.concat([df1, df2, df3], axis=1)
 
     if len(district.UnitsOfDistrict) > 0:
         if "EV_district" in district.UnitsOfDistrict:
-            df4 = get_variable_in_pandas(df, 'EV_E_stored')
+            df4 = get_ampl_data(ampl, 'EV_E_stored', multi_index=True)
             df4 = pd.concat([df4], keys=['Electricity'], names=['Layer'])
-            df5 = get_parameter_in_pandas(ampl, 'EV_displacement', multi_index=True)
+            df5 = get_ampl_data(ampl, 'EV_displacement', multi_index=True)
             df5 = pd.concat([df5], keys=['Electricity'], names=['Layer'])
-            df6 = get_parameter_in_pandas(ampl, 'EV_V2V', multi_index=True)
+            df6 = get_ampl_data(ampl, 'EV_V2V', multi_index=True)
             df6 = pd.concat([df6], keys=['Electricity'], names=['Layer'])
             df_Unit_t = pd.concat([df_Unit_t, df4, df5, df6], axis=1)
     df_Unit_t.index.names = ['Layer', 'Unit', 'Period', 'Time']
 
     units_districts = district.UnitsOfDistrict
     district_l_u = []
-    for l, units in district.UnitsOfLayer.items():
-        [district_l_u.append((l, unit)) for unit in units if unit in units_districts]
+    for layer, units in district.UnitsOfLayer.items():
+        [district_l_u.append((layer, unit)) for unit in units if unit in units_districts]
     df_Unit_t = df_Unit_t.reset_index(level=['Period', 'Time']).loc[district_l_u, :]
     df_Results["df_Unit_t"] = df_Unit_t.reset_index().set_index(['Layer', 'Unit', 'Period', 'Time']).sort_index()
 
     # df_lca
     if method["save_lca"]:
-        LCA_units = get_variable_in_pandas(df, 'lca_units')
+        LCA_units = get_ampl_data(ampl, 'lca_units', multi_index=True)
         LCA_units = LCA_units.stack().unstack(level=0).droplevel(level=1)
         df_Results["df_lca_Units"] = LCA_units
 
-        LCA_tot = get_variable_in_pandas(df, 'lca_tot')
+        LCA_tot = get_ampl_data(ampl, 'lca_tot')
         LCA_tot = LCA_tot.stack().unstack(level=0)
         LCA_tot.index = ["Network"]
-        LCA_tot_house = get_variable_in_pandas(df, 'lca_tot_house')
+        LCA_tot_house = get_ampl_data(ampl, 'lca_tot_house', multi_index=True)
         LCA_tot_house = LCA_tot_house.stack().unstack(level=0).droplevel(1)
         df_Results["df_lca_Performance"] = pd.concat([LCA_tot_house, LCA_tot], axis=0)
         df_Results["df_lca_Performance"].index.names = ['Hub']
 
-        LCA_op = get_variable_in_pandas(df, 'lca_op')
+        LCA_op = get_ampl_data(ampl, 'lca_op', multi_index=True)
         LCA_op = LCA_op.stack().unstack(level=0).droplevel(level=1)
         df_Results["df_lca_operation"] = LCA_op
 
-    if method["actors_cost"]:
-        df1 = get_variable_in_pandas(df, 'Cost_demand_district').groupby(level=(0,2)).sum()
-        df2 = get_variable_in_pandas(df, 'Cost_supply_district').groupby(level=(0,2)).sum()
-        df3 = get_variable_in_pandas(df, 'Cost_self_consumption').groupby(level=1).sum()
+    if method["actors_problem"]:
+        df1 = get_ampl_data(ampl, 'Cost_demand_district', multi_index=True).groupby(level=(0, 2)).sum()
+        df2 = get_ampl_data(ampl, 'Cost_supply_district', multi_index=True).groupby(level=(0, 2)).sum()
+        df3 = get_ampl_data(ampl, 'Cost_self_consumption', multi_index=True).groupby(level=1).sum()
         df3 = pd.concat({'Electricity': df3})
         df_Results["df_Actors_tariff"] = pd.concat([df1, df2, df3], axis=1)
 
-        df_Results["df_Actors"] = get_variable_in_pandas(df, 'objective_functions')
+        df_Results["df_Actors"] = get_ampl_data(ampl, 'objective_functions')
 
-        df1 = get_variable_in_pandas(df, 'C_op_renters_to_utility')
-        df2 = get_variable_in_pandas(df, 'C_op_renters_to_owners')
-        df3 = get_variable_in_pandas(df, 'C_op_utility_to_owners')
-        df4 = get_variable_in_pandas(df, 'Costs_House_inv')
+        df1 = get_ampl_data(ampl, 'C_op_renters_to_utility')
+        df2 = get_ampl_data(ampl, 'C_op_renters_to_owners')
+        df3 = get_ampl_data(ampl, 'C_op_utility_to_owners')
+        df4 = get_ampl_data(ampl, 'Costs_House_inv')
         df4.columns = ["owner_inv"]
-        df5 = get_variable_in_pandas(df, 'owner_portfolio')
+        df5 = get_ampl_data(ampl, 'owner_portfolio')
         df_Actors = pd.concat([df1, df2, df3, df4, df5], axis=1)
         df_6 = df_Actors.sum(axis=0).to_frame().T.set_index(pd.Index(["Network"]))
         df_Actors = pd.concat([df_Actors, df_6], axis=0)
         df_Results["df_District"] = pd.concat([df_Results["df_District"], df_Actors], axis=1)
         df_Results["df_District"].loc["Network", "Objective"] = ampl.getObjective("TOTEX_bui").getValues().toList()[0]
 
     return df_Results
 
-def get_parameter_in_pandas(ampl, ampl_name, multi_index):
+
+def get_ampl_data(ampl, ampl_name, multi_index=False):
     # AMPl data in AMPLPY Dataframe
     df = ampl.getData(ampl_name)
     # transform to Pandas Dataframe
     df = df.toPandas()
     # Change index from tuple to multi index
     if multi_index:
         df.index = pd.MultiIndex.from_tuples(df.index)
 
     return df
 
-def get_variable_in_pandas(df, ampl_name):
-    # get values
-    df_filtered = df[df["Varname"].str.contains(r'\b' + ampl_name + "\[")] # search the name of the variable
-    if len(df_filtered) == 0:
-        df_filtered = df[df["Varname"] == ampl_name] # if the variable has no sets (single value)
-
-    df_clean = pd.DataFrame(df_filtered["Value"])
-    df_clean.columns = [ampl_name]
-
-    # indexing
-    idx = df_filtered["Varname"]
-    id = [idx[i].replace(ampl_name, "").replace("'", "").replace("]", "").replace("[", "").split(",") for i in idx.index] # get set values for indexing
-    if len(id[0]) > 1:
-        df_clean.index = pd.MultiIndex.from_tuples(id)
-
-        # try to convert indexes from strings to floats
-        for i in range(len(id[0])):
-            try:
-                df_clean.index = df_clean.index.set_levels(df_clean.index.levels[i].astype(float), level=i)
-            except:
-                pass
-    else:
-        if id[0][0] == '': # single variable independant of any set are indexed to 0
-            id = [[0]]
-        df_clean.index = pd.Index(np.concatenate(id))
-    return df_clean
 
 def get_ampl_dual_values_in_pandas(ampl, ampl_name, multi_index):
     # AMPl data in AMPLPY Dataframe
     df = ampl.getConstraint(ampl_name).getValues().toPandas()
     # Change index from tuple to multi index
     if multi_index:
         df.index = pd.MultiIndex.from_tuples(df.index)
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/EV_profile_generator.py` & `reho-1.1.0/reho/model/preprocessing/EV_profile_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 from reho.paths import *
-import reho.model.preprocessing.weather as WD
+import reho.model.preprocessing.weather as weather
 import pandas as pd
 import numpy as np
 
-
-def generate_EV_plugged_out_profiles_district(cluster):
-    """
-    Computes hourly electric vehicle (EV) profiles for each typical day considering weekdays and weekends. Data are taken from
-    `UK Department for Transport 2013 <https://www.gov.uk/government/collections/energy-and-environment-statistics#publications>`_
-    and `SFSO 2015 <https://www.bfs.admin.ch/asset/fr/1840478>`_. The EV occupancy profiles are used to
-    optimize EV electricity demand profiles with the evehicle.mod ampl model.
+__doc__ = """
+Generates electric vehicle (EV) demand profiles.
+"""
 
 
+def generate_EV_plugged_out_profiles_district(cluster, df_Timestamp):
+    """
+    Computes hourly electric vehicle profiles for each typical day considering weekdays and weekends.
+    The EV demand profiles are used to optimize EV electricity demand profiles with the `evehicle.mod` ampl model.
 
     Parameters
     ----------
     cluster : dict
         Define location district, number of periods, and number of timesteps.
+    df_Timestamp : pd.DataFrame
+        Information for clustering results, used to know the periods and period duration.
 
     Returns
     -------
     EV_plugged_out : array
         Hourly profile of the share of vehicles being plugged out of the district LV grid.
     EV_plugging_in : array
         Hourly profile of the share of vehicles connecting to the district LV grid.
 
     Notes
-    -----
-    - EV_plugged_out, EV_plugging_in
+    ------
+    Data are taken from `UK Department for Transport 2013
+    <https://www.gov.uk/government/collections/energy-and-environment-statistics#publications>`_ and `Swiss Federal Statistical Office 2015
+    <https://www.bfs.admin.ch/asset/fr/1840478>`_.
 
     """
     # TODO IMPLEMENTATION of flexible period duration
-    File_ID = WD.get_cluster_file_ID(cluster)
+    File_ID = weather.get_cluster_file_ID(cluster)
 
     if 'W' in File_ID.split('_'):
         use_weekdays = True
     else:
         use_weekdays = False
 
     if use_weekdays:
         timestamp = np.loadtxt(os.path.join(path_to_clustering, 'timestamp_' + File_ID + '.dat'), usecols=(1, 2, 3),
                                skiprows=1)
         timestamp = pd.DataFrame(timestamp, columns=("Day", "Frequency", "Weekday"))
     else:
-        df = pd.read_csv(os.path.join(path_to_clustering, 'timestamp_' + File_ID + '.dat'), delimiter='\t')
+        df = df_Timestamp
         timestamp = df.fillna(1)  # only weekdays
 
     # Federal Office of Statistic, Comportement de la population en matiere de transports, 2015
-    profiles_weekday = [0.01, 0.0, 0.0, 0.0, 0.0, 0.03, 0.1, 0.12, 0.11, 0.12, 0.12, 0.14, 0.13, 0.14, 0.13, 0.13, 0.18,
-                        0.2, 0.15, 0.1, 0.07, 0.06, 0.05, 0.03]
-    profiles_weekend = [0.01, 0.0, 0.0, 0.0, 0.0, 0.00, 0.0, 0.00, 0.03, 0.10, 0.12, 0.11, 0.12, 0.12, 0.14, 0.13, 0.14,
-                        0.13, 0.15, 0.1, 0.07, 0.06, 0.05, 0.03]
+    # profiles_weekday_CH = [0.01, 0.0, 0.0, 0.0, 0.0, 0.03, 0.1, 0.12, 0.11, 0.12, 0.12, 0.14, 0.13, 0.14, 0.13, 0.13, 0.18,
+    #                        0.2, 0.15, 0.1, 0.07, 0.06, 0.05, 0.03]
+    # profiles_weekend_CH = [0.01, 0.0, 0.0, 0.0, 0.0, 0.00, 0.0, 0.00, 0.03, 0.10, 0.12, 0.11, 0.12, 0.12, 0.14, 0.13, 0.14,
+    #                        0.13, 0.15, 0.1, 0.07, 0.06, 0.05, 0.03]
 
     # UK department for transport Electric Chargepoint Analysis 2017: Domestics
     profiles_weekday = [0.0, 0.0, 0.0, 0.0, 0.01, 0.02, 0.08, 0.2, 0.31, 0.35, 0.38, 0.39, 0.39, 0.38, 0.38, 0.36, 0.31,
                         0.24, 0.18, 0.13, 0.09, 0.05, 0.03, 0.01]
     profiles_weekend = [0.0, 0.0, 0.0, 0.0, 0.01, 0.02, 0.08, 0.2, 0.31, 0.35, 0.38, 0.39, 0.39, 0.38, 0.38, 0.36, 0.31,
                         0.24, 0.18, 0.13, 0.09, 0.05, 0.03, 0.01]
 
@@ -71,15 +75,15 @@
             profile = profiles_weekend
             profile_plug_in = plugging_in_weekend
         elif day == 1:
             profile = profiles_weekday
             profile_plug_in = plugging_in_weekday
             # profile = np.tile(profiles_weekday, 365).tolist() # workaround -  whole year profile
         else:
-            raise ("day type not possible")
+            raise "day type not possible"
 
         EV_plugged_out = EV_plugged_out + profile
         EV_plugging_in = EV_plugging_in + profile_plug_in
 
     EV_plugged_out = EV_plugged_out + [0.0, 0.0]  # extreme hours
     EV_plugged_out = np.array(EV_plugged_out)
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/QBuildings.py` & `reho-1.1.0/reho/model/preprocessing/QBuildings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import configparser
+import csv
+import math
 import os.path
+import re
+
+import geopandas as gpd
+import numpy as np
+import pandas as pd
 from sqlalchemy import create_engine, MetaData, select
 from sqlalchemy.dialects import postgresql
-import geopandas as gpd
-import re
-import csv
+
+import reho.model.preprocessing.skydome as skydome
 from reho.paths import *
-import reho.model.preprocessing.skydome as skd
-import pandas as pd
-import numpy as np
-import math
 
 
 class QBuildingsReader:
     """
     This class is used to handle and prepare the data related to buildings.
 
     There usually come from `GBuildings <https://ipese-web.epfl.ch/lepour/qbuildings/index.html>`_ database. However,
@@ -23,25 +25,30 @@
     Parameters
     ----------
     load_facades : bool
         Whether the facades data should be added.
     load_roofs : bool
         Whether the roofs data should be added.
     """
+
     def __init__(self, load_facades=False, load_roofs=False):
 
         self.db = None
         self.tables = None
         self.db_schema = None
         self.db_engine = None
         self.connection = None
         self.data = {}
         self.load_facades = load_facades
         self.load_roofs = load_roofs
 
+        self.local_data = dict()
+        self.local_data["df_Area"] = pd.read_csv(path_to_areas, header=None)
+        self.local_data["df_Cenpts"] = pd.read_csv(path_to_cenpts, header=None)
+
     def establish_connection(self, db):
         """
         Allows to establish the connection with one of the QBuildings database.
 
         Parameters
         ----------
         db : str
@@ -65,16 +72,16 @@
                                                                           project['database']['host'],
                                                                           project['database']['port'],
                                                                           project['database']['database'])
             self.db_engine = create_engine(db_engine_str)
             self.connection = self.db_engine.connect()  # test connection
             print('Connected to database')
 
-        except:
-            print('Cannot connect to database engine')
+        except Exception as e:
+            print(f'Cannot connect to database engine: {e}')
 
         if 'database' in project:
             print('\thost: {}\n\tport: {}\n\tdatabase: {}\n\tusername: {}'.format(
                 project['database']['host'],
                 project['database']['port'],
                 project['database']['database'],
                 project['database']['username']))
@@ -83,18 +90,17 @@
         metadata = MetaData(bind=self.db_engine)
         metadata.reflect(schema=self.db_schema)
         self.tables = metadata.tables
         self.db = db
 
         return
 
-    def read_csv(self, buildings_filename='buildings.csv', nb_buildings=None,
-                 roofs_filename='roofs.csv', facades_filename='facades.csv'):
+    def read_csv(self, buildings_filename='buildings.csv', nb_buildings=None, roofs_filename='roofs.csv', facades_filename='facades.csv'):
         """
-        Read buildings-related data from CSV files and prepare it for the REHO model.
+        Reads buildings-related data from CSV files and prepare it for the REHO model.
 
         If not all the buildings from the file should be extracted, one can give a number of buildings.
         The fields from the files are translated to the corresponding ones used in REHO.
 
         Parameters
         ----------
         buildings_filename : str
@@ -133,39 +139,40 @@
 
         >>> qbuildings_data['buildings_data']['Building1'].keys()
         dict_keys(['id_class', 'ratio', 'status', 'ERA', 'SolarRoofArea', 'area_facade_m2', 'height_m', 'U_h', 'HeatCapacity', 'T_comfort_min_0', 'Th_supply_0', 'Th_return_0', 'Tc_supply_0', 'Tc_return_0', 'x', 'y', 'z', 'geometry', 'transformer', 'id_building', 'egid', 'period', 'n_p', 'energy_heating_signature_kWh_y', 'energy_cooling_signature_kWh_y', 'energy_hotwater_signature_kWh_y', 'energy_el_kWh_y'])
         """
         self.data['buildings'] = file_reader(buildings_filename)
         self.data['buildings'] = translate_buildings_to_REHO(self.data['buildings'])
         # self.data['buildings'] = add_geometry(self.data['buildings'])
+
         if nb_buildings is None:
             nb_buildings = self.data['buildings'].shape[0]
         buildings = self.select_buildings_data(nb_buildings, None)
         # buildings = add_geometry(buildings)
         qbuildings = {'buildings_data': buildings}
         if self.load_facades:
             self.data['facades'] = file_reader(path_handler(facades_filename))
             selected_facades = self.select_roofs_or_facades_data(roof=False)
             self.data['facades'] = self.data['facades'][self.data['facades'].index.isin(selected_facades)]
             self.data['facades'] = add_geometry(self.data['facades'])
             self.data['facades'] = translate_facades_to_REHO(self.data['facades'], self.data['buildings'])
             qbuildings['facades_data'] = self.data['facades']
-            qbuildings['shadows_data'] = return_shadows_district(qbuildings['buildings_data'], self.data['facades'])
+            qbuildings['shadows_data'] = return_shadows_district(qbuildings['buildings_data'], self.data['facades'], self.local_data)
 
         if self.load_roofs:
             self.data['roofs'] = file_reader(path_handler(roofs_filename))
             selected_roofs = self.select_roofs_or_facades_data(roof=True)
             self.data['roofs'] = self.data['roofs'][self.data['roofs'].index.isin(selected_roofs)]
             self.data['roofs'] = add_geometry(self.data['roofs'])
             self.data['roofs'] = translate_roofs_to_REHO(self.data['roofs'])
             qbuildings['roofs_data'] = self.data['roofs']
 
         return qbuildings
 
-    def read_db(self, transformer=None, nb_buildings=None, egid=None, to_csv=False, return_location=False):
+    def read_db(self, transformer=None, nb_buildings=None, egid=None, to_csv=False):
         """
         Reads the database and extract from it the buildings required, by the LV transformer's ID.
 
         If not all the buildings from the transformer should be extracted, one can give a number of buildings or if
         the EGIDs are known, pass a list of EGIDs.
         The fields from the database are translated to the corresponding ones used in REHO.
 
@@ -175,21 +182,19 @@
             ID of the transformer on which we want to optimize
         nb_buildings : int
             Number of buildings to select
         egid : list
             To specify a list of buildings to optimize with their EGIDs
         to_csv : bool
             To export the data into csv
-        return_location : bool
-            To obtain the corresponding meteo cluster
 
         Returns
         -------
         dict
-            A Dictionary that contains the qbuildings data. The default has only one key ``buildings_data``
+            A dictionary that contains the qbuildings data. The default has only one key ``buildings_data``
             with a dictionary of buildings, with their fields and corresponding values.
 
 
         Notes
         -----
         - The use of this function requires the previous creation of a ``QBuildingsReader`` and the use of ``establish_connection('Suisse')``.
         - EGIDs are the postal address unique identifier used in Switzerland. One can find the EGIDs of a given address at the `RegBL <https://www.housing-stat.ch/fr/query/adrtoegid.html>`_.
@@ -226,18 +231,14 @@
         # TODO: SQL query to select only buildings, roofs and facades of interest
 
         # Select the right transformer
         sqlQuery = select([self.tables[self.db_schema + '.' + 'transformers']]) \
             .where(self.tables[self.db_schema + '.' + 'transformers'].columns.id == transformer)
         self.data['transformers'] = gpd.read_postgis(sqlQuery.compile(dialect=postgresql.dialect()), con=self.db_engine,
                                                      geom_col='geometry').fillna(np.nan)
-        if return_location:
-            meteo_cluster = translate_meteo_to_period_cluster(self.data['transformers']['meteo'][0])
-        else:
-            meteo_cluster = None
 
         # Select buildings
         sqlQuery = select([self.tables[self.db_schema + '.' + 'buildings']]) \
             .where(self.tables[self.db_schema + '.' + 'buildings'].columns.transformer == transformer)
         self.data['buildings'] = gpd.read_postgis(sqlQuery.compile(dialect=postgresql.dialect()), con=self.db_engine,
                                                   geom_col='geometry').fillna(np.nan)
         mask = (self.data['buildings']['egid'].isnull())
@@ -269,15 +270,15 @@
                 self.data['facades'] = pd.concat(
                     (self.data['facades'], gpd.read_postgis(sqlQuery.compile(dialect=postgresql.dialect()),
                                                             con=self.db_engine, geom_col='geometry').fillna(np.nan)))
             if to_csv:
                 self.data['facades'].to_csv('facades.csv', index=False)
             self.data['facades'] = translate_facades_to_REHO(self.data['facades'], self.data['buildings'])
             qbuildings['facades_data'] = self.data['facades']
-            qbuildings['shadows_data'] = return_shadows_district(qbuildings["buildings_data"], self.data['facades'])
+            qbuildings['shadows_data'] = return_shadows_district(qbuildings["buildings_data"], self.data['facades'], self.local_data)
         if self.load_roofs:
             self.data['roofs'] = gpd.GeoDataFrame()
             for id in self.data['buildings'].id_building:
                 sqlQuery = select([self.tables[self.db_schema + '.' + 'roofs']]) \
                     .where(self.tables[self.db_schema + '.' + 'roofs'].columns.id_building == id)
                 self.data['roofs'] = pd.concat(
                     (self.data['roofs'], gpd.read_postgis(sqlQuery.compile(dialect=postgresql.dialect()),
@@ -346,23 +347,34 @@
     dict_QBuildings_REHO = {
 
         #################################################
         # Data strictly necessary for a REHO optimization
         #################################################
 
         # Data for EUD profiles
+        'id_building': 'id_building',
+        'egid': 'egid',
         'id_class': 'id_class',
+        'class': 'class',
         'ratio': 'ratio',
         'status': 'status',
+        'period': 'period',
+        'capita_cap': 'n_p',
+        # 'NOMSECTEUR': 'NOMSECTEUR',
 
         # Area
         'area_era_m2': 'ERA',
         'area_roof_solar_m2': 'SolarRoofArea',
         'area_facade_m2': 'area_facade_m2',
         'height_m': 'height_m',  # only for use facades
+        'count_floor': 'count_floor',
+
+        # Heating source
+        'source_heating': 'source_heating',
+        'source_hotwater': 'source_hotwater',
 
         # Thermal envelope
         'thermal_transmittance_signature_kW_m2_K': 'U_h',
         'thermal_specific_capacity_Wh_m2_K': 'HeatCapacity',
 
         # Temperature requirements
         'temperature_interior_C': 'T_comfort_min_0',
@@ -378,60 +390,56 @@
         # Geographic information
         'x': 'x',
         'y': 'y',
         'z': 'z',
         'geometry': 'geometry',
         'transformer': 'transformer',
 
-        # Additional information
-        'id_building': 'id_building',
-        'egid': 'egid',
-        'period': 'period',
-        'capita_cap': 'n_p',
-
         # Annual energy
         'energy_heating_signature_kWh_y': 'energy_heating_signature_kWh_y',
         'energy_cooling_signature_kWh_y': 'energy_cooling_signature_kWh_y',
         'energy_hotwater_signature_kWh_y': 'energy_hotwater_signature_kWh_y',
         'energy_el_kWh_y': 'energy_el_kWh_y',
+
+        # Annual roof and facade irradiance
+        'roof_annual_irr_kWh_y': 'roof_annual_irr_kWh_y',
+        'facade_annual_irr_kWh_y': 'facade_annual_irr_kWh_y'
     }
 
     # TODO: correct heat source dictionary
-    dict_translate_heat_source = {
-        'Gas': 'gas',
-        'Oil': 'oil',
-        'Wood (beech)': 'wood',
-        'Electricity': 'electricity',
-        'Heat pump': 'Heat pump',
-        'District heat': 'District heat',
-        'Other': 'gas',
-        'Other/Oil': 'oil',
-        'Electricity/Other': 'electricity',
-        'Oil/Gas': 'oil',
-        'Oil/Other': 'oil',
-        'Electricity/Oil': 'electricity',
-        'Heat pump/Electricity': 'Heat pump',
-        'Solar collector': 'solar',
-        'Solar (thermal)': 'solar',
-        'No energy source/Oil': 'oil',
-        'No energy source': 'gas',
-        'Electricity/No energy source': 'electricity',
-        'Oil/No energy source': 'oil',
-        'Gas/Solar collector': 'gas',
-        'Not determined': 'unknown'
-    }
+    # dict_translate_heat_source = {
+    #     'Gas': 'gas',
+    #     'Oil': 'oil',
+    #     'Wood (beech)': 'wood',
+    #     'Electricity': 'electricity',
+    #     'Heat pump': 'Heat pump',
+    #     'District heat': 'District heat',
+    #     'Other': 'gas',
+    #     'Other/Oil': 'oil',
+    #     'Electricity/Other': 'electricity',
+    #     'Oil/Gas': 'oil',
+    #     'Oil/Other': 'oil',
+    #     'Electricity/Oil': 'electricity',
+    #     'Heat pump/Electricity': 'Heat pump',
+    #     'Solar collector': 'solar',
+    #     'Solar (thermal)': 'solar',
+    #     'No energy source/Oil': 'oil',
+    #     'No energy source': 'gas',
+    #     'Electricity/No energy source': 'electricity',
+    #     'Oil/No energy source': 'oil',
+    #     'Gas/Solar collector': 'gas',
+    #     'Not determined': 'unknown'
+    # }
 
     for key in dict_QBuildings_REHO.keys():
         REHO_index = dict_QBuildings_REHO[key]
         try:
             new_buildings_data[REHO_index] = df_buildings[key]
         except KeyError:
             print('Key %s not in the dictionary' % key)
-        except:
-            print('Missing key in loaded data %s' % key)
 
     # for i, building in new_buildings_data.iterrows():
     #     try:
     #         sources_translated = dict_translate_heat_source[building['source_heating']]
     #         sources_translated_w = dict_translate_heat_source[building['source_hotwater']]
     #         building['source_heating'] = sources_translated
     #         building['source_hotwater'] = sources_translated_w
@@ -480,16 +488,15 @@
 
     for key in dict_facades.keys():
         REHO_index = dict_facades[key]
         try:
             new_facades_data[REHO_index] = df_facades[key]
         except KeyError:
             print('Key %s not in the dictionary' % key)
-        except:
-            print('Missing key in loaded data %s' % key)
+            
     df_facades = new_facades_data
     df_facades['CX'] = df_facades['geometry'].centroid.x
     df_facades['CY'] = df_facades['geometry'].centroid.y
     df_facades['coord_Z0'] = None
 
     for i, b in df_buildings.iterrows():
         concerned_facades = df_facades[df_facades['id_building'] == b['id_building']]
@@ -511,31 +518,20 @@
 
     for key in dict_roofs.keys():
         REHO_index = dict_roofs[key]
         try:
             new_roofs_data[REHO_index] = df_roofs[key]
         except KeyError:
             print('Key %s not in the dictionary' % key)
-        except:
-            print('Missing key in loaded data %s' % key)
+        
     df_roofs = new_roofs_data
 
     return df_roofs
 
 
-def translate_meteo_to_period_cluster(location):
-    dict_meteo = {'Zermatt': 'Disentis',
-                  'Geneva': 'Geneva',
-                  'Berne': 'Bern-Liebefeld',
-                  'CHDF': 'Piotta',
-                  'Zurich': 'Zuerich-SMA',
-                  'Gruyères': 'Lugano'}  # TODO set real cluster
-    return dict_meteo[location]
-
-
 def get_roofs(self, buildings):
     selected_roofs = []
     for i, building in buildings.iterrows():
         selected_roofs += \
             self.data['roofs'].index[self.data['roofs']['id_building'] == building['id_building']].to_list()
     self.data['roofs'] = self.data['roofs'][self.data['roofs'].index.isin(selected_roofs)]
 
@@ -548,30 +544,30 @@
         selected_facades += \
             self.data['facades'].index[self.data['facades']['id_building'] == building['id_building']].to_list()
     self.data['facades'] = self.data['facades'][self.data['facades'].index.isin(selected_facades)]
 
     return self.data['facades']
 
 
-def calculate_id_building_shadows(df_angles, id_building):
+def calculate_id_building_shadows(df_angles, id_building, local_data):
     df_angles['to_id_building'] = pd.to_numeric(df_angles['to_id_building'])
     df_angles = df_angles.set_index('to_id_building')
     df_angles = df_angles.xs(id_building)
 
-    df_dome = skd.skydome_to_df()
+    df_dome = skydome.skydome_to_df(local_data)
 
     df_shadow = pd.DataFrame()
 
     for az in df_dome.azimuth.unique():
-        df_angles.loc[:, 'cosa2'] = df_angles.apply(lambda x: skd.f_cos([x['azimuth'], az]), axis=1)
-        # df_cosa2 = df_id_building.apply(lambda x: skd.f_cos([x['azimuth'], az]), axis=1)
+        df_angles.loc[:, 'cosa2'] = df_angles.apply(lambda x: skydome.f_cos([x['azimuth'], az]), axis=1)
+        # df_cosa2 = df_id_building.apply(lambda x: skydome.f_cos([x['azimuth'], az]), axis=1)
         df = df_angles.loc[(df_angles['cosa2'] > 0)].copy()
         # filter buildings which are more than 180 degree apart from patch with az
         df.loc[:, 'tanba'] = df.tanb * df.cosa2
-        # calculate tan(beta) for all buildings. Assumption: dxy is shortest distance and buildings infinite wide
+        # calculate tan(beta) for all buildings. Assumption: dxy is the shortest distance and buildings infinite wide
 
         max_tanba = df['tanba'].max()  # get max obscurance tan(beta, alpha)
         max_b = math.degrees(math.atan(max_tanba))  # get angle
 
         if math.isnan(max_b):  # if no shadow, set everything to 0
             id_building = 0
             max_b = 0
@@ -594,98 +590,95 @@
         df_BUI = pd.DataFrame()
         df_district = {buildings: bui for buildings, bui in buildings.items() if bui['id_building'] != id_building}
         df_district = pd.DataFrame.from_dict(df_district, orient='index')
         df_district = df_district.set_index('id_building')
         # exclude current building to avoid division with zero
         facades_build = facades[facades.id_building == id_building]  # facades of building
         for f in facades_build.index:
-            df_c = pd.DataFrame(index=df_district.index)  # df for calculating values for each facades
+            df_c = pd.DataFrame(index=df_district.index)  # df for calculating values for each facade
             df_c['dx'] = df_district.x.values - facades_build.loc[f]['CX']
             df_c['dy'] = df_district.y.values - facades_build.loc[f]['CY']
             df_c['dxy'] = (df_c.dx * df_c.dx + df_c.dy * df_c.dy) ** 0.5
             heights = df_district.height_m.values
             if facades_build.loc[f]['coord_Z0'] is None:
                 print('Missing value coord_Z0, not possible to use_facades')
                 continue
             df_c['dz'] = df_district.z.values + heights - facades_build.loc[f]['coord_Z0']
             # facades.loc[f]['HEIGHT_Z'] + facades.loc[f]['HEIGHT'] #take foot of facades/ HEIGHT_Z is upperbound
             df_c['tanb'] = df_c.dz / df_c.dxy
             df_c['cosa'] = df_c.dy / df_c.dxy
-            df_c['azimuth'] = df_c[['dx', 'dy']].apply(skd.f_atan, axis=1)
-            df_c['beta'] = df_c[['dz', 'dxy']].apply(skd.f_atan, axis=1)
+            df_c['azimuth'] = df_c[['dx', 'dy']].apply(skydome.f_atan, axis=1)
+            df_c['beta'] = df_c[['dz', 'dxy']].apply(skydome.f_atan, axis=1)
             df_c = pd.concat([df_c], keys=[f], names=['UID'])
             df_BUI = pd.concat((df_BUI, df_c))
 
         df_BUI = df_BUI.reset_index()
         df_BUI = df_BUI.rename(columns={'id_building': 'to_id_building'})
         df_BUI['id_building'] = int(id_building)
 
         df_angles = pd.concat((df_angles, df_BUI))
 
     df_angles.to_csv('data/angles.csv')
 
     return df_angles
 
 
-def return_shadows_district(buildings, facades):
+def return_shadows_district(buildings, facades, local_data):
     df_shadows = pd.DataFrame()
 
     if os.path.exists('data/angles.csv'):
         df_angles = pd.read_csv('data/angles.csv')
     else:
         df_angles = neighbourhood_angles(buildings, facades)
 
     for b in buildings:
         id_building = int(buildings[b]['id_building'])
         if id_building in df_angles['id_building'].values:  # check if angle calculation for id_building exists
-            df_id_building = calculate_id_building_shadows(df_angles, id_building)
+            df_id_building = calculate_id_building_shadows(df_angles, id_building, local_data)
             idx = np.repeat(id_building, len(df_id_building))
             df_id_building = df_id_building.set_index(idx)
         else:
             print('NO DATA AVAILABLE FOR id_building ' + str(id_building))
             df_id_building = pd.DataFrame(index=[id_building],
                                           columns=['tanb', 'beta', 'azimuth', 'id_building'])  # pass NaN instead
         df_shadows = pd.concat((df_shadows, df_id_building))
 
     df_shadows["id_building"] = df_shadows["id_building"].astype(str)
     df_shadows.to_csv('data/shadows.csv')
 
     return df_shadows
 
 
-def return_shadows_id_building(id_building, df_district):
+def return_shadows_id_building(id_building, df_district, local_data):
     id_building = int(id_building)
 
     if os.path.isfile('data/shadows.csv'):
         df = file_reader('data/shadows.csv', index_col=0)
     else:
         df = df_district
     df = df.xs(id_building)
-    df_dome = skd.skydome_to_df()
+    df_dome = skydome.skydome_to_df(local_data)
 
     df_beta_dome = pd.DataFrame()
     for az in df_dome.azimuth:
         df_beta_dome = pd.concat((df_beta_dome, df.beta[df.azimuth == az]), ignore_index=True)
 
     df_beta_dome = df_beta_dome.rename(columns={0: 'Limiting_angle_shadow'})
 
     return df_beta_dome
 
 
 def add_geometry(df):
-    """
-    Avoid issues with geometry when read from a csv
-    """
+    # Avoid issues with geometry when reading data from a csv
     try:
         geom = gpd.GeoSeries.from_wkb(df['geometry'])
     except KeyError:
         print("No geometry in the dataframe")
         return df
     except:
         try:
             geom = gpd.GeoSeries.from_wkt(df['geometry'])
         except TypeError:
-            print("Geometry passed is neither of format wkb or wkt so neither from PostGIS, neither from QBuildings\n"
-                  "I wonder what you are trying to do here...")
+            print("Geometry passed is neither of format wkb or wkt so neither from PostGIS, neither from QBuildings")
             return df
 
     return gpd.GeoDataFrame(df, geometry=geom)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/clustering.py` & `reho-1.1.0/reho/model/preprocessing/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,92 +1,96 @@
 import pandas as pd
 import numpy as np
 import scipy.spatial
 from sklearn_extra.cluster import KMedoids
 from sklearn.metrics import pairwise_distances
 
+
 class ClusterClass:
     """
     This class executes the data reduction for meteorological data.
+    It will execute a clustering for each number of clusters desired among an interval (nb_clusters), and select the optimal one according to the MAPE criterion (Maximum Average Pairwise Euclidean distance).
 
     Parameters
     ----------
     data : pd.DataFrame
-        Input data (.dat file)
+        Annual weather data
+    nb_clusters : list
+        Interval for the number of clusters tested.
 
     """
 
-    def __init__(self, data, Iter=None,  option=None, pd=None, outliers=None):
+    def __init__(self, data, nb_clusters=None, option=None, pd=None, outliers=None):
         super().__init__()
-        if Iter == None:
-            self.Iter = [3]
+        if nb_clusters is None:
+            self.nb_clusters = [8]
         else:
-            self.Iter = Iter
+            self.nb_clusters = nb_clusters
 
-        #org - original, nor-normalized, clu-clustered
+        # org - original, nor - normalized, clu - clustered
 
         self.outlier_removal = outliers
 
         self.data_org = data  # input data- df: attribute vectors as columns
         self.data_nor = None
-        self.attr_org = []  # matrix or attributes, arrays:  len(attr_org) = total number of periods per year , len(attr_org[0])= number of attributes x period duration
+        self.attr_org = []  # matrix or attributes, arrays:  len(attr_org) = total number of periods per year, len(attr_org[0])= number of attributes x period duration
         self.attr_nor = []
         self.attr_clu = None
         self.modula = None
-        self.mod_org =[]  # modulo data, f.e. last day of year (24hrs) for  pd = 7*24
-        self.mod_nor =[]
-        if option == None:
+        self.mod_org = []  # modulo data, f.e. last day of year (24hrs) for  pd = 7*24
+        self.mod_nor = []
+        if option is None:
             self.option = {"year-to-day": True, "extreme": [(1, "min"), (2, "max")]}
         else:
-            self.option= option
+            self.option = option
 
         self.results = {"idx": None}  # pd.DataFrame()
 
         self.kpis_clu = None
         self.nbr_opt = None
 
-        if pd == None:              # period duration, f.e. 1 period = 1 day => pd =  24 (default)
+        if pd is None:  # period duration, f.e. 1 period = 1 day => pd =  24 (default)
             self.pd = 24
         else:
             self.pd = pd
 
-
     def run_clustering(self):
         self.__do_normalization()
         self.__execute_clustering()
         self.__compute_kpis()
         self.__select_optimal()
 
-
     def __do_normalization(self):
         # - Load data set
         self.data_nor = pd.DataFrame([], index=self.data_org.index, columns=self.data_org.columns)
         # - Create dissimilarity matrix
         for id, col in enumerate(self.data_org):
-            self.data_nor.loc[:, col] = ((self.data_org.loc[:, col] - self.data_org.loc[:, col].min()) / (self.data_org.loc[:, col].max() - self.data_org.loc[:, col].min())) #normalize
+            self.data_nor.loc[:, col] = ((self.data_org.loc[:, col] - self.data_org.loc[:, col].min()) / (
+                        self.data_org.loc[:, col].max() - self.data_org.loc[:, col].min()))  # normalize
             # - OPTION : re-arrange dataframe
             if self.option["year-to-day"]:
-                nbr_p = int(self.data_nor.shape[0] // self.pd) #! integer division / number of periods default: 365
+                nbr_p = int(self.data_nor.shape[0] // self.pd)  # ! integer division / number of periods default: 365
                 self.modulo = int(self.data_nor.shape[0] % self.pd)
-                stop = self.data_nor.shape[0] -self.modulo
-                self.attr_org.append(np.reshape(self.data_org.loc[: (stop -1), col].tolist(), (nbr_p, self.pd)))
-                self.attr_nor.append(np.reshape(self.data_nor.loc[: (stop -1), col].tolist(), (nbr_p, self.pd)))
-                self.mod_org.append(self.data_org.loc[ stop :, col].tolist())
+                stop = self.data_nor.shape[0] - self.modulo
+                self.attr_org.append(np.reshape(self.data_org.loc[: (stop - 1), col].tolist(), (nbr_p, self.pd)))
+                self.attr_nor.append(np.reshape(self.data_nor.loc[: (stop - 1), col].tolist(), (nbr_p, self.pd)))
+                self.mod_org.append(self.data_org.loc[stop:, col].tolist())
                 self.mod_nor.append(self.data_nor.loc[stop:, col].tolist())
             else:
                 self.attr_org.append(np.reshape(self.data_org.loc[:, col].tolist(), (self.data_org.shape[0], 1)))
                 self.attr_nor.append(np.reshape(self.data_nor.loc[:, col].tolist(), (self.data_org.shape[0], 1)))
 
         self.attr_org = np.hstack(self.attr_org)
         self.attr_nor = np.hstack(self.attr_nor)
 
-    def __run_KMedoids(self, matrix, n_clusters):
+    @staticmethod
+    def __run_KMedoids(matrix, n_clusters):
 
-        if len(matrix) == 1: #check for trivial solution
-            df_res = pd.DataFrame([1], columns= ['1'])
+        if len(matrix) == 1:  # check for trivial solution
+            df_res = pd.DataFrame([1], columns=['1'])
 
         else:
 
             print('Applying algorithm for', n_clusters, 'clusters')
 
             dist_a = pairwise_distances(matrix, metric='sqeuclidean')
             kmedoids = KMedoids(n_clusters=n_clusters, method='pam', random_state=42)
@@ -99,25 +103,24 @@
             mapped_cluster_assignments = np.vectorize(label_to_medoid.get)(cluster_assignments)
 
             df_res = pd.DataFrame()
             df_res[str(n_clusters)] = mapped_cluster_assignments
 
         return df_res
 
-
     def __execute_clustering(self):
 
         df_res = pd.DataFrame()  # initialize df for results
 
-        for i, c in enumerate(self.Iter):
+        for i, c in enumerate(self.nb_clusters):
             df = self.__run_KMedoids(self.attr_nor, c)
             df_res[str(c)] = df[str(c)]
 
         if self.outlier_removal:
-            for i, c in enumerate(self.Iter):
+            for i, c in enumerate(self.nb_clusters):
                 ncluster = c
 
                 medoids = df_res[str(ncluster)].unique()  # Warning periods start with 1, python with 0
 
                 df_distance = pd.DataFrame()
 
                 for med in medoids:
@@ -132,77 +135,74 @@
 
                     dist = scipy.spatial.distance.cdist(np_group_vector, np_group_matrix)  # calculate distance to medoid
 
                     df_med = pd.DataFrame(dist[0], index=group_matrix.index)
 
                     df_distance = df_distance.append(df_med)
 
-
                 if 'nlargest' in self.outlier_removal.keys():
                     outliers = df_distance.nlargest(self.outlier_removal['nlargest'], 0)
                 elif 'distance' in self.outlier_removal.keys():
                     outliers = df_distance[df_distance[0] > self.outlier_removal['distance']]
 
                 else:
-                    raise("outlier removal not specified use for example {'nlargest': 3} or {'distance':1}")
-
-                without_outliers = np.delete(self.attr_nor, (outliers.index), axis=0)
-                df = self.__run_KMedoids( without_outliers, ncluster)
+                    raise "outlier removal not specified use for example {'nlargest': 3} or {'distance':1}"
 
+                without_outliers = np.delete(self.attr_nor, outliers.index, axis=0)
+                df = self.__run_KMedoids(without_outliers, ncluster)
 
-                s = df.apply(lambda x: self.__return_typical_periods_outliers(x, x[str(ncluster)], outliers.index), axis = 1)
+                s = df.apply(lambda x: self.__return_typical_periods_outliers(x, x[str(ncluster)], outliers.index), axis=1)
                 s = s.set_index(0)
                 for o in outliers.index:
-                    s.at[o,1] = o
+                    s.at[o, 1] = o
                 df_res[str(c)] = s[1].sort_index()
 
         df_res.columns.name = "iteration"
         for col in df_res.columns:
             # - Rename extreme day index
             df_res.loc[df_res.loc[:, col] == 0, col] = df_res.loc[df_res.loc[:, col] == 0, col].index
         self.results["idx"] = df_res
 
-
-    def __return_typical_periods_outliers(self, idx, clusters, outliers):
+    @staticmethod
+    def __return_typical_periods_outliers(idx, clusters, outliers):
         index = idx.name
         outliers = outliers.sort_values()
-        outlier_position = [] #find outlier position in new index
+        outlier_position = []  # find outlier position in new index
         for c, id in enumerate(outliers):
-             outlier_position.append(id - c)
+            outlier_position.append(id - c)
         outlier_position = np.array(outlier_position)
 
-        outliers_before_period = outlier_position[outlier_position<=clusters]
-        outliers_before_index = outlier_position[outlier_position<= index]
+        outliers_before_period = outlier_position[outlier_position <= clusters]
+        outliers_before_index = outlier_position[outlier_position <= index]
 
         if len(outliers_before_period) == 0:
             cluster = clusters
             if len(outliers_before_index) == 0:
                 period = index
             else:
                 period = index + len(outliers_before_index)
         else:
-             cluster = clusters +len(outliers_before_period)
-             if len(outliers_before_index) == 0:
-                 period = index
-             else:
-                 period = index + len(outliers_before_index)
-
-        return pd.Series ([period, cluster])
+            cluster = clusters + len(outliers_before_period)
+            if len(outliers_before_index) == 0:
+                period = index
+            else:
+                period = index + len(outliers_before_index)
 
+        return pd.Series([period, cluster])
 
     def __compute_kpis(self):
         frm_kpis = []
         frm_clus = []
         # - Iterate through solutions
         for sol in self.results["idx"]:
             # - Assess extreme periods
             self.__compute_extreme(sol)
             # - Assess clustered year
             attr_clu, data_clu = self.__do_attr_clu(sol)
-            #data_clu annual dataframe, build with clustered periods to reach 8760 rows
+            # data_clu annual dataframe, build with clustered periods to reach 8760 rows
             # attr_clu matrix, same size as attr_org but with clustered attributes
             # - Assess KPIs
             pi = pd.DataFrame(index=pd.Index(["LDC", "MAE", "RMSD", "MAPE"], name="kpi"), columns=pd.Index(self.data_org.columns, name="dimension"))
             # - LDC error
             pi.loc["LDC", :] = sum(abs(np.sort(data_clu.values, axis=0) - np.sort(self.data_nor.values, axis=0))) / sum(self.data_nor.values)
             # - MAE
             pi.loc["MAE", :] = (1 / data_clu.shape[0]) * abs(self.data_nor - data_clu).sum()
@@ -214,59 +214,56 @@
             # - Append
             frm_kpis.append(pi)
             frm_clus.append(data_clu)
         # - Assign
         self.kpis_clu = pd.concat(frm_kpis, keys=self.results["idx"].columns, names=["iteration"], axis=1)
         self.attr_clu = pd.concat(frm_clus, keys=self.results["idx"].columns, names=["iteration"], axis=1)
 
-
     def __do_attr_clu(self, sol):
         # - Create clustered data
         idx = [x - 1 for x in self.results["idx"].loc[:, sol].tolist()]  # - Warning python index starts with 0!
         attr_clu = []
         for id in idx:
             id = int(id)
             attr_clu.append(self.attr_nor[id, :])
 
-        #attr_clu.append(np.hstack(self.mod_nor))
+        # attr_clu.append(np.hstack(self.mod_nor))
         attr_clu = np.array(attr_clu)
 
         # - OPTION : re-arrange dataframe
         if self.option["year-to-day"]:
             df = pd.DataFrame(columns=self.data_org.columns)
-            #nbr_t = int(self.data_nor.shape[0] / 365)
+            # nbr_t = int(self.data_nor.shape[0] / 365)
             for num, id_col in enumerate(df):
-                df[id_col] = np.reshape(attr_clu[:, int(self.pd * num):int(self.pd * (num + 1))], (self.data_org.shape[0]-self.modulo, 1)).flatten()
+                df[id_col] = np.reshape(attr_clu[:, int(self.pd * num):int(self.pd * (num + 1))], (self.data_org.shape[0] - self.modulo, 1)).flatten()
         else:
             df = pd.DataFrame(data=attr_clu, index=self.data_org.index, columns=self.data_org.columns)
 
-        #create df from the modulo data and append to cluster
-        df_mod = pd.DataFrame.from_dict(dict(zip( self.data_org.columns,self.mod_nor)))
-        df = df.append(df_mod, ignore_index = True)
+        # create df from the modulo data and append to cluster
+        df_mod = pd.DataFrame.from_dict(dict(zip(self.data_org.columns, self.mod_nor)))
+        df = df.append(df_mod, ignore_index=True)
 
         return attr_clu, df
 
-
     def __select_optimal(self):
         # - Define local variables
         kpis = self.kpis_clu.stack(["dimension"])
         diff = pd.DataFrame(index=kpis.index, columns=kpis.columns)
-        self.nbr_opt = max(self.Iter)
+        self.nbr_opt = max(self.nb_clusters)
         # - Iterate over solutions
         for id, n_k in enumerate(kpis):
             if id < kpis.shape[1] - 1:
                 diff.iloc[:, id] = (kpis.iloc[:, id + 1] - kpis.iloc[:, id])
-                condition = (diff.loc[("MAPE", slice(None)), n_k] > -0.01).all()  # optimum condition: MAPE doesnt improve more than 1%
+                condition = (diff.loc[("MAPE", slice(None)), n_k] > -0.01).all()  # optimum condition: MAPE doesn't improve more than 1%
                 if condition:
                     self.nbr_opt = n_k
                     break
         # print(diff)
         print("N_k optimal: " + str(self.nbr_opt))
 
-
     def __compute_extreme(self, sol):
 
         def find_nearests(array, value):
             array = np.asarray(array)
             dif = array - value
             if array.ndim > 1:
                 dif[dif < 0] = 1e3
@@ -279,20 +276,20 @@
                 val = array[idx]
             return val, id
 
         # - Iterate over extreme options
         for id_dim in self.option["extreme"]:
             # - OPTION : re-arrange dataframe
             if self.option["year-to-day"]:
-                nbr_t = self.pd #int(self.data_nor.shape[0] / 365)
+                nbr_t = self.pd  # int(self.data_nor.shape[0] / 365)
                 id_str = int((id_dim[0] - 1) * nbr_t)
                 id_end = int(id_dim[0] * nbr_t)
             else:
                 id_str = int(id_dim[0])
                 id_end = int(id_dim[0])
             # - Alter index
             if id_dim[1] == "max":
                 _, max_id = find_nearests(self.attr_org[:, id_str:id_end], np.percentile(self.attr_org[:, id_str:id_end], 99))
-                self.results["idx"].loc[max_id, sol] = max_id + 1       # - Warning -> index starts from 1!
+                self.results["idx"].loc[max_id, sol] = max_id + 1  # - Warning -> index starts from 1!
             else:
                 _, min_id = find_nearests(self.attr_org[:, id_str:id_end], np.percentile(self.attr_org[:, id_str:id_end], 1))
-                self.results["idx"].loc[min_id, sol] = min_id + 1       # - Warning -> index starts from 1!
+                self.results["idx"].loc[min_id, sol] = min_id + 1  # - Warning -> index starts from 1!
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/data_generation.py` & `reho-1.1.0/reho/model/preprocessing/buildings_profiles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,78 +1,47 @@
-import numpy as np
-import pandas as pd
 from datetime import timedelta
-from reho.model.preprocessing.weather import get_cluster_file_ID
 from reho.model.preprocessing.sia_parser import *
 from reho.model.preprocessing.QBuildings import *
 
 __doc__ = """
-*Generates the buildings profiles : 1) Domestic hot water (DHW), 2) Domestic electricity, 3) Heat gains, 4) Solar gains.*
+Generates the buildings profiles for domestic hot water (DHW) demand, domestic electricity demand, internal heat gains, and solar gains.
 """
 
-def annual_to_typical(cluster, annual_file, typical_file=None):
-    """
-    From an annual profile, with 8760 values, extracts the values corresponding to the typical days.
-    """
-
-    # Get which days are the typical ones
-    File_ID = get_cluster_file_ID(cluster)
-    timestamp_file = os.path.join(path_to_clustering, 'timestamp_' + File_ID + '.dat')
-    df_time = pd.read_csv(timestamp_file, delimiter='\t')
-    typical_days = df_time.Date.apply(lambda date: date[0:-3]).values
-
-    df_annual = file_reader(annual_file)
-    t1 = pd.to_datetime('1/1/2005', dayfirst=True, infer_datetime_format=True)
 
-    # hour 1 is between 0:00 - 1:00 and is indexed with starting hour so 0:00
-    for h in df_annual.index.values:
-        df_annual.loc[h, 'h'] = t1 + timedelta(hours=(int(h) - 1))
-
-    df_annual = df_annual.set_index('h')
-    df_typical = pd.DataFrame()
-    for i, td in enumerate(typical_days):
-        df_typical = pd.concat([df_typical, df_annual.loc[td]], sort=True)
-    periods = list(range(1, len(typical_days) + 1))
-    hours = list(range(1, cluster['PeriodDuration'] + 1))
-    df_typical = df_typical.reset_index(drop=True)
-    df_typical = df_typical.set_index(pd.MultiIndex.from_product([periods, hours], names=['Period', 'Hour']))
-    if typical_file:
-        df_typical.to_csv(typical_file)
-
-    return df_typical
-
-
-def profile_reference_temperature(parameters_to_ampl, cluster):
+def reference_temperature_profile(parameters_to_ampl, cluster):
     # TODO: time dependent indoor temperature f.e. lower at night
 
     total_timesteps = cluster['Periods'] * cluster['PeriodDuration'] + 2
     T_comfort_min_0 = parameters_to_ampl['T_comfort_min_0']
 
     np_temperature = np.array([])
     for key in parameters_to_ampl['T_comfort_min_0']:
         np_temperature = np.append(np_temperature, np.tile(T_comfort_min_0[key], total_timesteps))
 
     return np_temperature
 
 
-def build_eud_profiles(buildings_data, File_ID, cluster,
-                       include_stochasticity=False, sd_stochasticity=None, use_custom_profiles=False):
+def eud_profiles(buildings_data, cluster, df_SIA_380, df_SIA_2024, df_Timestamp, include_stochasticity=False, sd_stochasticity=None, use_custom_profiles=False):
     """
-    Except if electricity, SH and DHW profiles are given by the user, REHO computes the End Use Demands from
-    `SIA 2024 <https://shop.sia.ch/collection%20des%20normes/architecte/2024_2021_f/F/Product>`_.
+    Generates building-specific profiles for internal heat gains, DHW demand, and domestic electricity demand based on
+    `SIA 2024 norms <https://shop.sia.ch/collection%20des%20normes/architecte/2024_2021_f/F/Product>`_.
 
     The SIA profiles are daily profiles with coefficient attributed to each month.
-    This function extends the profiles to the periods used, according the building's affectation.
+    This function extends the profiles to the periods used, according to the building's affectation.
 
     Parameters
     ----------
     buildings_data : dict
         Dictionary of buildings data from QBuildingsReader class.
-    File_ID : str
-        File ID of the clustering results, used to know the periods and period duration.
+    df_SIA_380 : pd.DataFrame
+        SIA norms.
+    df_SIA_2024 : pd.DataFrame
+        SIA norms.
+    df_Timestamp : pd.DataFrame
+        Information for clustering results, used to know the periods and period duration.
     cluster : dict
         cluster parameter from the reho.model.reho.reho class
     include_stochasticity : bool
         Activate the method `include_stochasticity`, from the reho.model.reho.reho class, that includes variability
         in the values given by the SIA profiles.
     sd_stochasticity : dict
         Dictionary, from the reho.model.reho.reho class, that precises the parameters of the stochasticity (see :ref:`tbl-methods`).
@@ -85,84 +54,76 @@
     the electricity demand.
 
     See also
     --------
     reho.model.preprocessing.QBuildings.QBuildingsReader :
         Class used to handle the buildings' data.
     reho.model.reho.reho :
-        Wrapper Class that manages the optimization.
+        Wrapper class that manages the optimization.
 
     Notes
     -----
     - One building can have several affectations. In that case, the building is divided by the share of ERA by
       affectations and the profiles are summed.
     - To use custom profiles, use csv files with 8760 rows. The name of the columns should be the same as the buildings keys in `buildings_data`.
-    -
 
     .. caution::
 
         When using custom electricity profiles, the heat gains from electricity appliances are estimated through a conversion
         factor ``conv_heat_factor`` (default value = 70%).
 
     Examples
     --------
     >>> my_profiles = {'electricity': 'my_folder/electricity.csv'}
     >>> file_id = 'Geneva_10_24_T_I_W'
-    >>> cluster = {'Location': 'Bruxelles', 'Attributes': ['I', 'T', 'W'], 'Periods': 10, 'PeriodDuration': 24}
-    >>> people_gain, eud_dhw, eud_elec =
-    >>>     build_eud_profiles(buildings_data, file_id, cluster, use_custom_profiles=my_profiles)
+    >>> cluster = {'Location': 'Bruxelles', 'Attributes': ['T', 'I', 'W'], 'Periods': 10, 'PeriodDuration': 24}
+    >>> people_gain, eud_dhw, eud_elec = eud_profiles(buildings_data, cluster, use_custom_profiles=my_profiles)
     """
     # get cluster information
-    timestamp_file = os.path.join(path_to_clustering, 'timestamp_' + File_ID + '.dat')
-    df = pd.read_csv(timestamp_file, delimiter='\t')
-    df.Date = pd.to_datetime(df['Date'], format="%m/%d/%Y/%H")
-
-    path_norms = os.path.join(path_to_sia, 'sia2024_data.xlsx')
-    df_SIA = pd.read_excel(path_norms, sheet_name=['profiles', 'calculs', 'data'], engine='openpyxl',
-                           index_col=[0], skiprows=[0, 2, 3, 4], header=[0])
+    df_Timestamp.Date = pd.to_datetime(df_Timestamp['Date'], format="%m/%d/%Y/%H")
 
     np_gain_all = np.array([])
     np_dhw_all = np.array([])
     np_el_all = np.array([])
 
     if use_custom_profiles:
         # Replace filepath in dictionary to typical profiles
         for key, val in use_custom_profiles.items():
-            use_custom_profiles[key] = annual_to_typical(cluster, annual_file=val)
+            use_custom_profiles[key] = annual_to_typical(cluster, annual_file=val, df_Timestamp=df_Timestamp)
 
     for b in buildings_data:  # iterate over buildings
         # get SIA Profiles
         classes = buildings_data[b]['id_class'].split('/')
         if isinstance(buildings_data[b]['ratio'], float):
             ratios = str(buildings_data[b]['ratio'])
         else:
             ratios = buildings_data[b]['ratio'].split('/')
         status_buildings = buildings_data[b]['status'].split(',')
         np_gain_class = np.zeros(cluster['Periods'] * cluster['PeriodDuration'] + 2)
         np_dhw_class = np.zeros(cluster['Periods'] * cluster['PeriodDuration'] + 2)
         np_el_class = np.zeros(cluster['Periods'] * cluster['PeriodDuration'] + 2)
         for i, class_380 in enumerate(classes):
             # share of rooms for building type
-            rooms = read_sia2024_rooms_sia380_1(class_380)
+            rooms = read_sia2024_rooms_sia380_1(class_380, df_SIA_380)
             status = ''.join(filter(str.isalnum, status_buildings[i]))
             if class_380 == 'I' or class_380 == 'II':
                 area_net_floor = buildings_data[b]['ERA'] / 1.245
             else:
                 area_net_floor = buildings_data[b]['ERA']
             area_net_floor = area_net_floor * float(ratios[i])
             np_gain = np.array([])
             np_dhw = np.array([])
             np_el = np.array([])
 
             if include_stochasticity:
                 [RV_scaling, SF] = create_random_var(sd_stochasticity[0], sd_stochasticity[1])
 
-            for p in df.index:  # get profiles for each typical day
+            for p in df_Timestamp.index:  # get profiles for each typical day
 
-                df_profiles = daily_profiles_with_monthly_deviation(status, rooms, df.xs(p).Date, df_SIA)
+                df_profiles = daily_profiles_with_monthly_deviation(status, rooms, df_Timestamp.xs(p).Date, df_SIA_2024)
                 if include_stochasticity:
                     df_profiles = apply_stochasticity(df_profiles, RV_scaling, SF)
 
                 df_custom_profiles = pd.DataFrame()
                 if use_custom_profiles:
                     for key, df_key in use_custom_profiles.items():
                         df_custom_profiles[key] = df_key.xs(i + 1, level='Period').loc[:, b]
@@ -187,29 +148,29 @@
                 else:
                     hotwater = df_profiles['hotwater_l/m2'] * area_net_floor
 
                 heatgain_day = (people_gain + elec_gain) / 1000  # kW profiles for each typical day
                 hot_water_day = hotwater  # L profiles for each typical day
                 electric_day = elec / 1000  # kW profiles for each typical day
 
-                if p not in df.index.tolist()[-2:]:
+                if p not in df_Timestamp.index.tolist()[-2:]:
                     # sort it correctly (if first hour is not 12:00)
-                    begin = df.xs(p).Date.hour
+                    begin = df_Timestamp.xs(p).Date.hour
 
                     # Size = 24 hours
                     heat_day = np.concatenate((heatgain_day.iloc[begin:].values, heatgain_day.iloc[:begin].values))
                     dhw_day = np.concatenate((hot_water_day.iloc[begin:].values, hot_water_day.iloc[:begin].values))
                     el_day = np.concatenate((electric_day.iloc[begin:].values, electric_day.iloc[:begin].values))
 
                     # Size = PeriodDuration (= TimeEnd in ampl)
                     heat_period = np.tile(heat_day, round(cluster['PeriodDuration'] / 24))
                     dhw_period = np.tile(dhw_day, round(cluster['PeriodDuration'] / 24))
                     el_period = np.tile(el_day, round(cluster['PeriodDuration'] / 24))
 
-                elif p == df.index.tolist()[-2:][0]:  # Minimum period
+                elif p == df_Timestamp.index.tolist()[-2:][0]:  # Minimum period
                     heat_period = np.array([min(heatgain_day)])
                     dhw_period = np.array([max(dhw_day)])
                     el_period = np.array([max(el_day)])
                 else:  # Maximum period
                     heat_period = np.array([max(heatgain_day)])
                     dhw_period = np.array([max(dhw_day)])
                     el_period = np.array([max(el_day)])
@@ -258,89 +219,99 @@
       one should adapt the function.
 
     See also
     --------
     apply_stochasticity
     """
     # constraints
-    if sd_amplitude < 0: sd_amplitude = 0
-    if sd_timeshift < 0: sd_timeshift = 0
+    if sd_amplitude < 0:
+        sd_amplitude = 0
+    if sd_timeshift < 0:
+        sd_timeshift = 0
 
     # create the random variable for the intensity variation
     mu = 1
     RV_scaling = np.random.normal(mu, sd_amplitude, 5)
-    if RV_scaling.argmin() < 0: print("-------------- Negative value in the intensity variation --------------")
+    if RV_scaling.argmin() < 0:
+        print("-------------- Negative value in the intensity variation --------------")
 
     # create the random variable for time-shift in standard profiles
     mu = 0
     SF = np.random.normal(mu, sd_timeshift, 5)
 
     return RV_scaling, SF
 
 
-def solar_gains_profile(ampl, buildings_data, File_ID):
+def annual_to_typical(cluster, annual_file, df_Timestamp, typical_file=None):
+    """
+    From an annual profile (8760 values), extracts the values corresponding to the typical days.
+    """
+
+    # Get which days are the typical ones
+    typical_days = pd.Series([i.strftime("%m/%d/%Y") for i in df_Timestamp.Date]).values
+    df_annual = file_reader(annual_file)
+    t1 = pd.to_datetime('1/1/2005', dayfirst=True, infer_datetime_format=True)
+
+    # hour 1 is between 0:00 - 1:00 and is indexed with starting hour so 0:00
+    for h in df_annual.index.values:
+        df_annual.loc[h, 'h'] = t1 + timedelta(hours=(int(h) - 1))
+
+    df_annual = df_annual.set_index('h')
+    df_typical = pd.DataFrame()
+    for i, td in enumerate(typical_days):
+        df_typical = pd.concat([df_typical, df_annual.loc[td]], sort=True)
+    periods = list(range(1, len(typical_days) + 1))
+    hours = list(range(1, cluster['PeriodDuration'] + 1))
+    df_typical = df_typical.reset_index(drop=True)
+    df_typical = df_typical.set_index(pd.MultiIndex.from_product([periods, hours], names=['Period', 'Hour']))
+    if typical_file:
+        df_typical.to_csv(typical_file)
+
+    return df_typical
+
+
+def solar_gains_profile(buildings_data, sia_data, local_data):
     """
     Computes the solar heat gains from the irradiance.
 
     It uses a typical irradiation file and uses `calc_orientation_profiles` to obtain the irradiation on the west
     facades. Additionally, the solar gains depends on the facades and on a window fraction (obtained from SIA 2024).
 
     Parameters
     ----------
-    ampl : AMPL
-        The AMPL object created in the reho.model.reho.reho class.
     buildings_data : dict
-        Dictionary of buildings data from QBuildingsReader class.
-    File_ID : str
-        File ID of the clustering results, used to know the periods and period duration.
+        Building-specific data.
+    sia_data : dict
+        SIA norms.
+    local_data : dict
+        Location-specific data.
 
     Returns
     -------
-    A Numpy array of shape (242,) with the solar gains for each timesteps.
+    A Numpy array with the solar gains for each timesteps.
     """
-    # Number of days computation
-    PeriodDuration = ampl.getParameter('TimeEnd').getValues().toPandas()
-    timestamp_file = os.path.join(path_to_clustering, 'timestamp_' + File_ID + '.dat')
-    df = pd.read_csv(timestamp_file, delimiter='\t')
-    df.Date = pd.to_datetime(df['Date'], format="%m/%d/%Y/%H")
-
-    frequency_dict = pd.Series(df.Frequency.values, index=df.Date).to_dict()
-    frequency_dict['PeriodDuration'] = {}
-    for p in ampl.getSet('PeriodStandard').getValues().toList():
-        frequency_dict['PeriodDuration'][p] = PeriodDuration.loc[p].TimeEnd
-
-    # get west_facades irradiation
-    # check if irradiation already exists:
-    filename = os.path.join(path_to_clustering, 'westfacades_irr_' + File_ID + '.txt')
-    if not os.path.exists(filename):
-        total_irradiation = os.path.join(path_to_skydome, 'total_irradiation.csv')
-        df_annual, irr_west = skd.calc_orientation_profiles(270, 90, 0, total_irradiation, frequency_dict)
-        np.savetxt(filename, irr_west)
-    else:
-        irr_west = pd.read_csv(filename, header=None)[0].values
+
+    irr_west = local_data["df_Westfacades_irr"]
 
     g = np.repeat(0.5, len(irr_west))  # g-value SIA 2024
     g[irr_west > 0.2] = 0.1  # assumption that if irradiation exceeds 200 W/m2, we use sunblinds
 
     np_gains = np.array([])
     for b in buildings_data:
         A_facades = buildings_data[b]['area_facade_m2']
         classes = buildings_data[b]['id_class'].split('/')
         if isinstance(buildings_data[b]['ratio'], float):
             ratios = str(buildings_data[b]['ratio'])
         else:
             ratios = buildings_data[b]['ratio'].split('/')
-        status_buildings = buildings_data[b]['status'].split(',')
         glass_fraction_building = 0
         for i, class_380 in enumerate(classes):
             # share of rooms for building type
-            rooms = read_sia2024_rooms_sia380_1(class_380)
-            path_norms = os.path.join(path_to_sia, 'sia2024_data.xlsx')
-            df = pd.read_excel(path_norms, sheet_name='data', engine='openpyxl', index_col=[0],
-                               skiprows=[0, 2, 3, 4], header=[0])
+            rooms = read_sia2024_rooms_sia380_1(class_380, sia_data["df_SIA_380"])
+            df = sia_data["df_SIA_2024"]['data']
             glass_fraction_2024 = df['Taux de surface vitrée']
             glass_fraction_rooms = (glass_fraction_2024 * rooms).sum()
             glass_fraction_building += glass_fraction_rooms * float(ratios[i])
         gains = irr_west / 1000 * g * 0.9 * glass_fraction_building / 100 * A_facades
         # glass fraction on facades from SIA 2024, 0.9 SIA 2024: acknowledge perpendicular rays
         np_gains = np.append(np_gains, gains)
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/electricity_prices.py` & `reho-1.1.0/reho/model/preprocessing/electricity_prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,51 +15,43 @@
     "http://www.w3.org/2001/XMLSchema#float": float,
     "http://www.w3.org/2001/XMLSchema#double": float,
     "http://www.w3.org/2001/XMLSchema#decimal": float,
     "http://www.w3.org/2001/XMLSchema#date": date.fromisoformat,
     "http://www.w3.org/2001/XMLSchema#dateTime": (
         lambda x: datetime.strptime(x.rstrip("Z"), "%Y-%m-%dT%H:%M:%S")
     ),
-    "http://www.opengis.net/ont/geosparql#wktLiteral": wkt.loads,
-    "http://www.openlinksw.com/schemas/virtrdf#Geometry": wkt.loads,
+    "https://www.opengis.net/ont/geosparql#wktLiteral": wkt.loads,
+    "https://www.openlinksw.com/schemas/virtrdf#Geometry": wkt.loads,
     "https://www.w3.org/2001/XMLSchema#integer": int,
     "https://www.w3.org/2001/XMLSchema#float": float,
     "https://www.w3.org/2001/XMLSchema#double": float,
     "https://www.w3.org/2001/XMLSchema#decimal": float,
     "https://www.w3.org/2001/XMLSchema#date": date.fromisoformat,
     "https://www.w3.org/2001/XMLSchema#dateTime": (
         lambda x: datetime.strptime(x.rstrip("Z"), "%Y-%m-%dT%H:%M:%S")
     ),
-    "https://www.opengis.net/ont/geosparql#wktLiteral": wkt.loads,
-    "https://www.openlinksw.com/schemas/virtrdf#Geometry": wkt.loads,
 }
 
-GEODATA_TYPES = set(
-    [
-        "http://www.opengis.net/ont/geosparql#wktLiteral",
-        "http://www.openlinksw.com/schemas/virtrdf#Geometry",
-        "https://www.opengis.net/ont/geosparql#wktLiteral",
-        "https://www.openlinksw.com/schemas/virtrdf#Geometry",
-    ]
-)
+GEODATA_TYPES = {"https://www.opengis.net/ont/geosparql#wktLiteral", "https://www.openlinksw.com/schemas/virtrdf#Geometry",
+                 "https://www.opengis.net/ont/geosparql#wktLiteral", "https://www.openlinksw.com/schemas/virtrdf#Geometry"}
 
 
 def requests_retry_session(
         retries=3, backoff_factor=0.3, status_forcelist=(500, 502, 504), session=None
 ):
     session = session or rq.Session()
     retry = urllib3.util.Retry(
         total=retries,
         read=retries,
         connect=retries,
         backoff_factor=backoff_factor,
         status_forcelist=status_forcelist,
     )
     adapter = rq.adapters.HTTPAdapter(max_retries=retry)
-    session.mount("http://", adapter)
+    session.mount("https://", adapter)
     session.mount("https://", adapter)
 
     return session
 
 
 class SparqlClient:
     def __init__(
@@ -99,42 +91,42 @@
         if normalized_prefixes:
             normalized_prefixes += "\n"
         return normalized_prefixes
 
     def add_prefixes(self, prefixes: Dict) -> None:
         """Define prefixes to be added to every query
         Args:
-            prefixes: 		prefixes to be added to every query
+            prefixes: prefixes to be added to every query
 
         Returns
             None
         """
 
         self.prefixes = {**self.prefixes, **prefixes}
 
     def remove_prefixes(self, prefixes: Dict) -> None:
         """Remove prefixes from the prefixes are added to every query
         Args:
-            prefixes: 		prefixes to be removed from self.prefixes
+            prefixes: prefixes to be removed from self.prefixes
 
         Returns
             None
         """
 
         for prefix in prefixes:
             self.prefixes.pop(prefix, None)
 
     def _format_query(self, query: str) -> str:
         """Format SPARQL query to include in-memory prefixes.
         Prefixes already defined in the query have precedence, and are not overwritten.
             Args:
-                query: 				user-defined SPARQL query
+                query: user-defined SPARQL query
 
             Returns
-                str:	            SPARQL query with predefined prefixes
+                str: SPARQL query with predefined prefixes
         """
 
         prefixes_in_query = dict(
             [
                 re.split(SPLIT_PATTERN, prefix, 1)
                 for prefix in re.findall(FIND_PATTERN, query)
             ]
@@ -198,15 +190,15 @@
             self, response: Dict
     ) -> Union[pd.DataFrame, gpd.GeoDataFrame]:
         """Normalize response from SPARQL endpoint. Transform json structure to table. Convert observations to python data types.
         Args:
             response: 			raw response from SPARQL endpoint
 
         Returns
-            pd.DataFrame	    response from SPARQL endpoint in a tabular form, with python data types
+            pd.DataFrame: response from SPARQL endpoint in a tabular form, with python data types
         """
 
         cols = response["head"]["vars"]
         data = dict(zip(cols, [[] for i in range(len(cols))]))
 
         has_geo_data = False
         for row in response["results"]["bindings"]:
@@ -264,25 +256,25 @@
                        'Thurgau', 'Tessin', 'Vaud', 'Valais', 'Neuchâtel', 'Geneva', 'Jura']}
 cantons = pd.DataFrame.from_dict(cantons).set_index('id')
 
 sparql = SparqlClient("https://lindas.admin.ch/query")
 geosparql = SparqlClient("https://ld.geo.admin.ch/query")
 
 sparql.add_prefixes({
-    "schema": "<http://schema.org/>",
+    "schema": "<https://schema.org/>",
     "cube": "<https://cube.link/>",
     "elcom": "<https://energy.ld.admin.ch/elcom/electricityprice/dimension/>",
     "admin": "<https://schema.ld.admin.ch/>",
 })
 
 geosparql.add_prefixes({
-    "dct": "<http://purl.org/dc/terms/>",
-    "geonames": "<http://www.geonames.org/ontology#>",
-    "schema": "<http://schema.org/>",
-    "geosparql": "<http://www.opengis.net/ont/geosparql#>",
+    "dct": "<https://purl.org/dc/terms/>",
+    "geonames": "<https://www.geonames.org/ontology#>",
+    "schema": "<https://schema.org/>",
+    "geosparql": "<https://www.opengis.net/ont/geosparql#>",
 })
 
 
 def get_providers_by_municipality_id(city=None, from_csv=False):
     """
     Gives the electricity providers for a given municipality.
 
@@ -335,71 +327,71 @@
             SELECT DISTINCT ?id_city ?commune ?id_operator ?operator WHERE {
                 <https://energy.ld.admin.ch/elcom/electricityprice> <https://cube.link/observationSet> ?observationSet0 .
                 ?observationSet0 <https://cube.link/observation> ?source0 .
             ?source0 <https://energy.ld.admin.ch/elcom/electricityprice/dimension/municipality> city_to_replace .
             ?source0 <https://energy.ld.admin.ch/elcom/electricityprice/dimension/operator> ?id_operator .
             
             OPTIONAL {
-                city_to_replace <http://schema.org/name> ?commune_0 .
+                city_to_replace <https://schema.org/name> ?commune_0 .
                 FILTER (
                   LANGMATCHES(LANG(?commune_0), "fr")
                 )
               }
               OPTIONAL {
-                city_to_replace <http://schema.org/name> ?commune_1 .
+                city_to_replace <https://schema.org/name> ?commune_1 .
                 FILTER (
                   LANGMATCHES(LANG(?commune_1), "de")
                 )
               }
               OPTIONAL {
-                city_to_replace <http://schema.org/name> ?commune_2 .
+                city_to_replace <https://schema.org/name> ?commune_2 .
                 FILTER (
                   LANGMATCHES(LANG(?commune_2), "it")
                 )
               }
               OPTIONAL {
-                city_to_replace <http://schema.org/name> ?commune_3 .
+                city_to_replace <https://schema.org/name> ?commune_3 .
                 FILTER (
                   LANGMATCHES(LANG(?commune_3), "en")
                 )
               }
               OPTIONAL {
-                city_to_replace <http://schema.org/name> ?commune_4 .
+                city_to_replace <https://schema.org/name> ?commune_4 .
                 FILTER (
                   (LANG(?commune_4) = "")
                 )
               }
             BIND(COALESCE(?commune_0, ?commune_1, ?commune_2, ?commune_3, ?commune_4) AS ?commune)    
             
             OPTIONAL {
-                ?id_operator <http://schema.org/name> ?operator_0 .
+                ?id_operator <https://schema.org/name> ?operator_0 .
                 FILTER (
                   LANGMATCHES(LANG(?operator_0), "fr")
                 )
               }
               OPTIONAL {
-                ?id_operator <http://schema.org/name> ?operator_1 .
+                ?id_operator <https://schema.org/name> ?operator_1 .
                 FILTER (
                   LANGMATCHES(LANG(?operator_1), "de")
                 )
               }
               OPTIONAL {
-                ?id_operator <http://schema.org/name> ?operator_2 .
+                ?id_operator <https://schema.org/name> ?operator_2 .
                 FILTER (
                   LANGMATCHES(LANG(?operator_2), "it")
                 )
               }
               OPTIONAL {
-                ?id_operator <http://schema.org/name> ?operator_3 .
+                ?id_operator <https://schema.org/name> ?operator_3 .
                 FILTER (
                   LANGMATCHES(LANG(?operator_3), "en")
                 )
               }
               OPTIONAL {
-                ?id_operator <http://schema.org/name> ?operator_4 .
+                ?id_operator <https://schema.org/name> ?operator_4 .
                 FILTER (
                   (LANG(?operator_4) = "")
                 )
               }
               BIND(COALESCE(?operator_0, ?operator_1, ?operator_2, ?operator_3, ?operator_4) AS ?operator)
             }
             """
@@ -590,19 +582,21 @@
     [1 rows x 9 columns]
     """
 
     city_link = 'https://ld.admin.ch/municipality/'
     cat_link = 'https://energy.ld.admin.ch/elcom/electricityprice/category/'
 
     if isinstance(city, QBuildingsReader):
-        city = city.data['transformers']['id_city'][0]
+        try:
+            city = city.data['transformers']['id_city'][0]
+        except KeyError:
+            city = 6621  # if id_city is missing from database, set Geneva by default
         city_query = '<' + city_link + str(city) + '>'
     elif isinstance(city, str):
-        cities = pd.read_csv(os.path.join(path_to_elcom, 'correspondance_table_municipality_operator.csv'),
-                             index_col=0)
+        cities = pd.read_csv(os.path.join(path_to_elcom, 'correspondance_table_municipality_operator.csv'), index_col=0)
         mask = (cities['id_city'] == city) + (cities['commune'] == city)
         cities = cities[mask]
         if cities.empty:
             print('No corresponding city with that name')
         city = cities.iloc[0]['id_city']
         city_query = '<' + city_link + str(city) + '>'
     elif isinstance(city, int):
@@ -634,71 +628,71 @@
           elcom:total ?totalcosts;
           elcom:gridusage ?grid;
           elcom:energy ?energy;
           elcom:charge ?community_fees;
           elcom:aidfee ?aidfee.
           
       OPTIONAL {
-        city_to_replace <http://schema.org/name> ?commune_0 .
+        city_to_replace <https://schema.org/name> ?commune_0 .
         FILTER (
           LANGMATCHES(LANG(?commune_0), "fr")
         )
       }
       OPTIONAL {
-        city_to_replace <http://schema.org/name> ?commune_1 .
+        city_to_replace <https://schema.org/name> ?commune_1 .
         FILTER (
           LANGMATCHES(LANG(?commune_1), "de")
         )
       }
       OPTIONAL {
-        city_to_replace <http://schema.org/name> ?commune_2 .
+        city_to_replace <https://schema.org/name> ?commune_2 .
         FILTER (
           LANGMATCHES(LANG(?commune_2), "it")
         )
       }
       OPTIONAL {
-        city_to_replace <http://schema.org/name> ?commune_3 .
+        city_to_replace <https://schema.org/name> ?commune_3 .
         FILTER (
           LANGMATCHES(LANG(?commune_3), "en")
         )
       }
       OPTIONAL {
-        city_to_replace <http://schema.org/name> ?commune_4 .
+        city_to_replace <https://schema.org/name> ?commune_4 .
         FILTER (
           (LANG(?commune_4) = "")
         )
       }
     BIND(COALESCE(?commune_0, ?commune_1, ?commune_2, ?commune_3, ?commune_4) AS ?City)
           
       OPTIONAL {
-        ?operator <http://schema.org/name> ?operator_0 .
+        ?operator <https://schema.org/name> ?operator_0 .
         FILTER (
           LANGMATCHES(LANG(?operator_0), "fr")
         )
       }
       OPTIONAL {
-        ?operator <http://schema.org/name> ?operator_1 .
+        ?operator <https://schema.org/name> ?operator_1 .
         FILTER (
           LANGMATCHES(LANG(?operator_1), "de")
         )
       }
       OPTIONAL {
-        ?operator <http://schema.org/name> ?operator_2 .
+        ?operator <https://schema.org/name> ?operator_2 .
         FILTER (
           LANGMATCHES(LANG(?operator_2), "it")
         )
       }
       OPTIONAL {
-        ?operator <http://schema.org/name> ?operator_3 .
+        ?operator <https://schema.org/name> ?operator_3 .
         FILTER (
           LANGMATCHES(LANG(?operator_3), "en")
         )
       }
       OPTIONAL {
-        ?operator <http://schema.org/name> ?operator_4 .
+        ?operator <https://schema.org/name> ?operator_4 .
         FILTER (
           (LANG(?operator_4) = "")
         )
       }
       BIND(COALESCE(?operator_0, ?operator_1, ?operator_2, ?operator_3, ?operator_4) AS ?Provider)
             
     }
@@ -734,29 +728,31 @@
     prices['finalcosts'] = tva * prices['totalcosts']
 
     if isinstance(export_path, str):
         prices.to_csv(os.path.realpath(export_path))
 
     return prices
 
+
 def get_vese_key():
     try:
         response = rq.get("https://ipese-lectures.epfl.ch/static/reho.json", timeout=1)
         if response.status_code == 200:
             json_data = response.json()
             api_key_value = json_data.get("API_VESE_KEY")
             return api_key_value
         else:
             return f"Error: {response.status_code}"
     except Exception:
         return False
-    
+
+
 def get_injection_prices(city=None, year=2024, category=None, tva=None):
     """
-    Retrieve injection prices from the `pvtarif.ch <https://www.vese.ch/fr/pvtarif/>`_  API.
+    Retrieves injection prices from the `pvtarif.ch <https://www.vese.ch/fr/pvtarif/>`_  API.
 
     The year, municipality and consumer category can be given to query at a more precise level.
     TVA is applied by default or can be adapted as a scaling factor.
 
     Parameters
     ----------
     city : str or None, optional
@@ -800,15 +796,15 @@
         id_city municipality  id_operator  ... origin_bonus  totalcosts  finalcosts
     1914     2701        Basel          624  ...          0.0        13.0        14.0
     [1 rows x 8 columns]
     """
     # Retrieve license key
     load_dotenv()
     if 'API_VESE_KEY' not in os.environ:
-        license_key=get_vese_key()
+        license_key = get_vese_key()
         if not license_key:
             raise UserWarning("You need a key from VESE to access the injection prices")
     else:
         license_key = os.environ["API_VESE_KEY"]
     if len(str(year)) == 4:
         year = year % 100
 
@@ -825,15 +821,15 @@
             if not json_data['valid']:
                 print(f'{json_data["code"]}: {json_data["details"]}')
                 continue
         else:
             raise ExecutionError(f"{response.status_code}")
 
         try:
-        # TODO: add a code to adapt the prices to the category given, as a function of what is defined
+            # TODO: add a code to adapt the prices to the category given, as a function of what is defined
             commune_price = {'id_city': commune.id_city, 'municipality': commune.commune,
                              'id_operator': int(json_data['nrElcom']), 'operator': json_data['nomEw'],
                              'federal_tariff': float(json_data['energy1']), 'origin_bonus': float(json_data['eco1']),
                              'totalcosts': float(json_data['energy1']) + float(json_data['eco1'])
                              }
         except:
             continue
@@ -906,13 +902,13 @@
     electricity_prices['Elec_demand_cts_kWh'] = demand_prices['finalcosts']
     electricity_prices.loc[:, 'Elec_supply_cts_kWh'] = supply_prices['finalcosts'].iloc[0]
 
     return electricity_prices
 
 
 if __name__ == '__main__':
-    injection = get_injection_prices(year=2023, city='Basel')
-    communes = get_electricity_prices(city='Genève', category=None, year=2017)
-    # prices = get_prices_from_elcom(year=2023, canton='Geneva', category=None, export_path='../../elec_prices_2024.csv')
+    injection = get_injection_prices(city='Basel', year=2023)
+    communes = get_electricity_prices(city='Geneva', year=2017, category=None)
+    prices = get_prices_from_elcom_by_city(year=2023, city='Geneva', category=None, export_path='../../elec_prices_2024.csv')
     id_commune = 177
     get_injection_prices(692)
     # url_commune = f'https://opendata.vese.ch/pvtarif/api/ClientService.php?mode=muni&idofs={id_commune}&licenseKey={license_key}'
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/sia_parser.py` & `reho-1.1.0/reho/model/preprocessing/sia_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 import pandas as pd
-from reho.paths import *
 import numpy as np
 
 __doc__ = """
-*Collects data from "SIA" Swiss Norms, which are used to distinguish between eight different building types in their usage and behavior.*
+Collects data from the `SIA Swiss norms <https://www.sia.ch/fr/services/sia-norm/>`_ , which are used to distinguish between eight different building types in their usage and behavior.
 """
 
-def read_sia2024_rooms_sia380_1(digit):
-
-    path_sia = os.path.join(path_to_sia, 'sia2024_rooms_sia380_1.csv')
 
+def read_sia2024_rooms_sia380_1(digit, df_SIA_380):
     dict_affiliation2digit = {'collective housing': 'I',
                               'individual housing': 'II',
                               'administrative': 'III',
                               'school': 'IV',
                               'commercial': 'V',
                               'restaurant': 'VI',
                               'gathering places': 'VII',
                               'hospital': 'VIII',
                               'industry': 'IX',
                               'shed, warehouse': 'X',
                               'sports facilities': 'XI',
                               'covered swimming-pool': 'XII',
                               'other': 'XIII'}
 
-    df = pd.read_csv(path_sia, sep=';', index_col=[0], header=[0])
-    df = df.rename(columns=dict_affiliation2digit)
+    df_SIA_380 = df_SIA_380.rename(columns=dict_affiliation2digit)
 
-    return df[digit]
+    return df_SIA_380[digit]
 
 
 def read_sia_2024_profiles(status, df):
-
     df_el_appliance = df["calculs"].iloc[:, 1:25]
     df_el_ap_norm = df_el_appliance.div(df_el_appliance.max(axis=1), axis=0)  # normalize profile
     df_el_ap_norm = df_el_ap_norm.fillna(0)
 
     # status allows to scale the domestic electricity consumption
     if status == 'existing':  # high electricity consumption
         df_existing = df["data"].iloc[:, 38]
@@ -43,65 +38,64 @@
     elif status == 'standard':  # medium electricity consumption
         df_standard = df["data"].iloc[:, 36]
         df_el_appliance = df_el_ap_norm.mul(df_standard, axis=0)
     elif (status == 'aim') or (status == 'target'):  # low electricity consumption
         df_aim = df["data"].iloc[:, 37]
         df_el_appliance = df_el_ap_norm.mul(df_aim, axis=0)
     else:
-        raise ('Building status unknown')
+        raise 'Building status unknown'
 
     df_el_light = df["calculs"].iloc[:, 26:50]
     df_el_light.columns = df_el_appliance.columns  # columns 1-24 - hours of the day
 
-    df_el_add = df["calculs"].iloc[:, 52:76] #additional light profile f.e. for "showrooms"
+    df_el_add = df["calculs"].iloc[:, 52:76]  # additional light profile f.e. for "showrooms"
     df_el_add.columns = df_el_appliance.columns  # columns 1-24 - hours of the day
 
-    df_heat_gain = df["calculs"].iloc[:, 102:126] # heatgain by people
+    df_heat_gain = df["calculs"].iloc[:, 102:126]  # heatgain by people
     df_heat_gain.columns = df_el_appliance.columns  # columns 1-24 - hours of the day
 
     df_dhw = df["calculs"].iloc[:, 127:151]
     df_dhw.columns = df_el_appliance.columns  # columns 1-24 - hours of the day
 
     df_occupancy = df["calculs"].iloc[:, 208:232]
     df_occupancy.columns = df_el_appliance.columns  # columns 1-24 - hours of the day
 
     return df_el_add, df_el_light, df_el_appliance, df_dhw, df_occupancy, df_heat_gain
 
 
 def daily_profiles_with_monthly_deviation(status, rooms, date, df):
-
     # get monthly deviation
     df_months = df['profiles'].iloc[:, 49:61]
 
     # rename to match python timestamp
     dict_months = {'Janvier': 1, 'Fevrier': 2, 'Mars': 3, 'Avril': 4, 'Mai': 5, 'Juin': 6,
                    'Juillet': 7, 'Aout': 8, 'Septembre': 9, 'Octobre': 10, 'Novembre': 11, 'Decembre': 12}
-    df_months = df_months.rename(columns = dict_months)
+    df_months = df_months.rename(columns=dict_months)
 
     monthly_factor = df_months[date.month]
 
     # get weekly deviation
     df_free = df['profiles'].iloc[:, 61]  # 0 no days unused, 2 = weekend unused, 1 = Sundays unused
 
     weekly_factor = np.repeat(1, len(rooms))
     if date.weekday() == 6:  # 6 = Sunday
         weekly_factor[(df_free == 1) | (df_free == 2)] = 0  # rooms which are not used on a Sunday
     if date.weekday() == 5:  # 5 = Saturday
-        weekly_factor[ df_free == 2] = 0  # rooms which are not used on a Saturday
+        weekly_factor[df_free == 2] = 0  # rooms which are not used on a Saturday
 
     # get 2024 profiles
     df_el_appliance, df_el_light, df_el_add, df_dhw, df_occupancy, df_heat_gain = read_sia_2024_profiles(status, df)
     df_el = df_el_appliance + df_el_light + df_el_add  # W/m2
     df_el_gain = df_el_appliance + df_el_light
     # adjust for current day of the year
-    df_el = df_el.multiply(weekly_factor*monthly_factor, axis=0)
+    df_el = df_el.multiply(weekly_factor * monthly_factor, axis=0)
     df_el_gain = df_el_gain.multiply(weekly_factor * monthly_factor, axis=0)
-    df_dhw = df_dhw.multiply(weekly_factor*monthly_factor, axis=0)
-    df_occupancy = df_occupancy.multiply(weekly_factor*monthly_factor, axis=0)
-    df_heat_gain = df_heat_gain.multiply(weekly_factor*monthly_factor, axis=0)
+    df_dhw = df_dhw.multiply(weekly_factor * monthly_factor, axis=0)
+    df_occupancy = df_occupancy.multiply(weekly_factor * monthly_factor, axis=0)
+    df_heat_gain = df_heat_gain.multiply(weekly_factor * monthly_factor, axis=0)
 
     # get profiles for each room. multiply by usage. nan if not appearing in building
     df_el = df_el.multiply(rooms.values, axis=0).dropna()
     df_el_gain = df_el_gain.multiply(rooms.values, axis=0).dropna()
     df_dhw = df_dhw.multiply(rooms.values, axis=0).dropna()
     df_occupancy = df_occupancy.multiply(rooms.values, axis=0).dropna()
     df_heat_gain = df_heat_gain.multiply(rooms.values, axis=0).dropna()
@@ -111,8 +105,7 @@
     df_profiles['electricity_W/m2'] = df_el.sum(axis=0)
     df_profiles['hotwater_l/m2'] = df_dhw.sum(axis=0)
     df_profiles['occupancy'] = df_occupancy.sum(axis=0)
     df_profiles['elecgain_W/m2'] = df_el_gain.sum(axis=0)
     df_profiles['heatgainpeople_W/m2'] = df_heat_gain.sum(axis=0)
 
     return df_profiles
-
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/skydome.py` & `reho-1.1.0/reho/model/preprocessing/skydome.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import math
 from datetime import timedelta
 from reho.paths import *
 import itertools as it
 import matplotlib.pyplot as plt
 
 __doc__ = """
-*Used for PV orientation.*
+Used for PV orientation.
 """
 
+
 def convert_results_txt_to_csv(load_timesteps):
     """ load one txt file for each hour/timestep in "load_timesteps".
     txt file contains oriented irradiation of each 145 skypatches. Combines all hours to one df
 
     :param load_timesteps:
     :return: df:
     """
@@ -28,157 +29,135 @@
         df_hour = pd.DataFrame(gh_result, index=[int(ts)])
         df = df.append(df_hour)
 
     t1 = pd.to_datetime('1/1/2005', dayfirst=True, infer_datetime_format=True)
 
     # hour 1 is between 0:00 - 1:00 and is indexed with starting hour so 0:00
     for h in df.index.values:
-        df.loc[h, 'time'] = t1 + timedelta(hours=(int(h)-1))
+        df.loc[h, 'time'] = t1 + timedelta(hours=(int(h) - 1))
 
     df = df.set_index('time')
     output_file = os.path.join(path_to_skydome, 'total_irradiation.csv')
     df.to_csv(output_file)
     print(df)
 
 
-def skydome_to_df():
-    """ reads two txt files: one containing the area and one the position of the center point of the 145 patches,
-     which define the skydome. Calculates basic additional values and returns all data in one single df
-
-    :return:   df
+def skydome_to_df(local_data):
     """
-    areas = os.path.join(path_to_skydome, 'skyPatchesAreas.txt')  # area of patches
-    cenpts = os.path.join(path_to_skydome, 'skyPatchesCenPts.txt')  # location of centre points
+    Reads two txt files: one containing the area and one the position of the center point of the 145 patches,
+    which define the skydome. Calculates basic additional values and returns all data in one single df
 
-    # create one df for all skydome data
-    df_area = pd.read_csv(areas, header=None)
-    df_cenpts = pd.read_csv(cenpts, header=None)
+    The irradiation dome is defined as a composition of patches, defined by their area and their centroids. Those
+    patches do not depend on the location. The sky is always decomposed the same way, as done by
+    `Lady Bug tool <https://www.ladybug.tools/ladybug/docs/index.html>`_.
+
+    Returns
+    -------
+       pd.DataFrame
+    """
+    df_area = local_data["df_Area"]  # area of patches
+    df_cenpts = local_data["df_Cenpts"]  # location of centre points
 
     df_dome = pd.DataFrame()
     df_dome['Area'] = df_area[0]
     df_dome['X'] = df_cenpts[0]
     df_dome['Y'] = df_cenpts[1]
     df_dome['Z'] = df_cenpts[2]
 
     # Add basic caluclations
     df_dome['XY'] = df_dome[['X', 'Y']].apply(f_sqrt, axis=1)
     df_dome['XYZ'] = df_dome[['XY', 'Z']].apply(f_sqrt, axis=1)
-    df_dome['Sin_e'] = round(df_dome['Z']/df_dome['XYZ'],4)
-    df_dome['Cos_e'] = round(df_dome['XY']/df_dome['XYZ'],4)
-    df_dome['Cos_a'] = round(df_dome['Y']/df_dome['XY'],4)
-    df_dome['Sin_a'] = round(df_dome['X']/df_dome['XY'],4)
+    df_dome['Sin_e'] = round(df_dome['Z'] / df_dome['XYZ'], 4)
+    df_dome['Cos_e'] = round(df_dome['XY'] / df_dome['XYZ'], 4)
+    df_dome['Cos_a'] = round(df_dome['Y'] / df_dome['XY'], 4)
+    df_dome['Sin_a'] = round(df_dome['X'] / df_dome['XY'], 4)
     df_dome['azimuth'] = df_dome[['X', 'Y']].apply(f_atan, axis=1)
-    df_dome['elavation'] = df_dome[['Z', 'XY']].apply(f_atan, axis=1)
+    df_dome['elevation'] = df_dome[['Z', 'XY']].apply(f_atan, axis=1)
 
     return df_dome
 
 
-def irradiation_to_df(ampl, irradiation_csv, File_ID):
+def irradiation_to_df(ampl, df_irradiation, df_time):
     """reads Irradiation values of all 145 for the timesteps given in the csv file.
      Converts them to float and returns them as df"""
 
-
-    df_IRR = pd.read_csv(irradiation_csv, index_col=[0])
-
-    #change column name from string to int
-    df_IRR.columns = df_IRR.columns.astype(int)
-    #change values from string to float
-    df_IRR = df_IRR.infer_objects()
+    # change column name from string to int
+    df_irradiation.columns = df_irradiation.columns.astype(int)
+    # change values from string to float
+    df_irradiation = df_irradiation.infer_objects()
 
     # parse index as datetime
-    df_IRR.index = pd.to_datetime(df_IRR.index)
+    df_irradiation.index = pd.to_datetime(df_irradiation.index)
 
     # get relevant cluster information
-    thisfile = os.path.join(path_to_clustering, 'timestamp_'+ File_ID +'.dat')
-    df = pd.read_csv(thisfile, delimiter='\t', parse_dates=[0])
-    PeriodDuration  = ampl.getParameter('TimeEnd').getValues().toPandas()
+    PeriodDuration = ampl.getParameter('TimeEnd').getValues().toPandas()
 
     # construct Multiindex
     df_p = pd.DataFrame()
     list_timesteps = []
 
-    for p in df.index:
-        date1 = df.xs(p).Date
-        end = PeriodDuration.xs(p+1).TimeEnd  # ampl starts at 1
+    for p in df_time.index:
+        date1 = df_time.xs(p).Date
+        end = PeriodDuration.xs(p + 1).TimeEnd  # ampl starts at 1
 
-        date2 = date1 + timedelta(hours=int(end)-1)
-        df_period = df_IRR.loc[date1:date2]
+        date2 = date1 + timedelta(hours=int(end) - 1)
+        df_period = df_irradiation.loc[date1:date2]
 
-        for t in np.arange(1, int(end)+1):  # ampl starts at 1
-            list_timesteps.append((p +1, t))  # create ample index
+        for t in np.arange(1, int(end) + 1):  # ampl starts at 1
+            list_timesteps.append((p + 1, t))  # create ampl index
 
         df_p = pd.concat([df_p, df_period])
 
     idx = pd.MultiIndex.from_tuples(list_timesteps)
 
     # marry index and data
-    df_IRR = df_p.set_index(idx)
+    df_irradiation = df_p.set_index(idx)
 
-    #df_IRR = pd.concat([df_IRR], axis=1, keys=['Patches'])
-    df = df_IRR.stack()
+    df = df_irradiation.stack()
     df = df.reorder_levels([2, 0, 1])
     df = pd.DataFrame(df)
-    df = df.rename(columns = {0 : 'Irr'})
+    df = df.rename(columns={0: 'Irr'})
     return df
 
 
-def irradiation_to_df_general(irradiation_csv):
+def irradiation_to_df_general(df_irradiation):
     """reads Irradiation values of all 145 for the timesteps given in the csv file.
      Converts them to float and returns them as df"""
 
-    df_IRR = pd.read_csv(irradiation_csv, index_col=[0])
-
-    #change column name from string to int
-    df_IRR.columns = df_IRR.columns.astype(int)
+    # change column name from string to int
+    df_irradiation.columns = df_irradiation.columns.astype(int)
     # change values from string to float
-    df_IRR = df_IRR.infer_objects()
+    df_irradiation = df_irradiation.infer_objects()
 
-    return df_IRR
+    return df_irradiation
 
 
-def irradiation_to_typical_df(typical_days_string):
+def irradiation_to_typical_df(typical_days_string, df_profiles):
     """reads Irradiation values of all 145 for the timesteps given in the csv file.
      Converts them to float and returns them as df"""
 
-    filename = os.path.join(path_to_skydome, 'total_irradiation.csv')
-    df_profiles = pd.read_csv(filename, sep=",", parse_dates=[1])
     df_profiles.set_index('time', inplace=True)
-
     df_profiles.index = pd.to_datetime(df_profiles.index)
 
-    # print(df_profiles[df_profiles.index.isin(typical_days_string)])
-    # print(df_profiles.loc['20160921'])
-    # print(df_profiles['20160921'])
-
     # select typical days, keep typday index as reference
     df_typical = pd.DataFrame()
     for i, td in enumerate(typical_days_string):
-        df_typical = pd.concat([df_typical, df_profiles[td]],  sort = True)
-        # df_typical.loc[td,'TypdayID'] = int(i)
+        df_typical = pd.concat([df_typical, df_profiles[td]], sort=True)
 
     # save profiles in csv
     df_typical.to_csv(os.path.join(path_to_skydome, 'typical_irradiation.csv'))
 
     return df_typical
 
 
-    #df_IRR = pd.read_csv(irradiation_csv, index_col=[0], dtype=float)
-
-    #change column name from string to int
-    #df_IRR.columns = df_IRR.columns.astype(int)
-    #change values from string to float
-    #df_IRR = df_IRR.infer_objects()
-
-    #return df_IRR
-
 def f_sqrt(x):
     """
     Calculates the square root of a vector with two elements
     """
-    return math.hypot(x[0],x[1])
+    return math.hypot(x[0], x[1])
 
 
 def f_atan(x):
     """
     math.atan2(y, x) : Returns atan(y / x), in radians. The result is between -pi and pi. The vector in the plane from
     the origin to point (x, y) makes this angle with the positive X axis. The point of atan2() is that the signs of both
     inputs are known to it, so it can compute the correct quadrant for the angle. For example, atan(1) and atan2(1, 1)
@@ -196,132 +175,127 @@
 
     return int(round(azimuth))
 
 
 def f_cos(x):
     a1 = math.radians(x[0])
     a2 = math.radians(x[1])  # cos(-a) = cos(a)
-    return math.cos(a1-a2)
+    return math.cos(a1 - a2)
 
 
-def calc_orientation_profiles(azimuth, tilt, design_lim_angle, irradiation_file, typical_frequency):
+def calc_orientation_profiles(azimuth, tilt, design_lim_angle, local_data, typical_frequency):
     cos_a = round(math.cos(math.radians(azimuth)), 8)
     sin_a = round(math.sin(math.radians(azimuth)), 8)
     sin_y = round(math.sin(math.radians(tilt)), 8)
     cos_y = round(math.cos(math.radians(tilt)), 8)
     print('PANEL ORIENTATION: azimuth ', azimuth, ', tilt ', tilt)
 
-    df_dome = skydome_to_df()
-    df_IRR = irradiation_to_df_general(irradiation_file)
+    df_dome = skydome_to_df(local_data)
+    df_irradiation = irradiation_to_df_general(local_data["df_Irradiation"])
 
-    df_irr_pos = pd.DataFrame()
-    df_irr_neg = pd.DataFrame()
-    for pt in df_IRR.columns.values:
+    df_irradiation_pos = pd.DataFrame()
+    df_irradiation_neg = pd.DataFrame()
+    for pt in df_irradiation.columns.values:
 
         azi_pt = df_dome.xs(pt)['azimuth']
-        ele_pt = df_dome.xs(pt)['elavation']
+        ele_pt = df_dome.xs(pt)['elevation']
         # ------------------------------
         # piecewise linerization skydome
         # ------------------------------
         delta_azi = np.cos(np.radians(azi_pt - azimuth))
         if delta_azi > 0:
-
             lim_angle = np.rad2deg(np.arctan(delta_azi * np.tan(np.radians(design_lim_angle))))
         else:
-
             lim_angle = -1
 
         if (lim_angle > (ele_pt - 6)) & (lim_angle < (ele_pt + 6)):
-
             linear_factor = 1 - ((lim_angle - (ele_pt - 6)) / 12)
 
         elif lim_angle >= (ele_pt + 6):
             linear_factor = 0
 
         elif lim_angle <= (ele_pt - 6):
             linear_factor = 1
 
         else:
             linear_factor = 'here is a problem linearization of skydome'
         if linear_factor < 0:
             raise 'linear factor negative, changes irradiation direction'
 
         # calculation orientation in skydome, rotation
-
         rotation = - sin_a * sin_y * df_dome.xs(pt)['Sin_a'] * df_dome.xs(pt)['Cos_e'] \
                    - sin_y * cos_a * df_dome.xs(pt)['Cos_a'] * df_dome.xs(pt)['Cos_e'] - cos_y * df_dome.xs(pt)['Sin_e']
-        irradiation_patch = round(df_IRR[pt] * rotation * linear_factor, 10)
+        irradiation_patch = round(df_irradiation[pt] * rotation * linear_factor, 10)
         if irradiation_patch.min() < 0:
-            df_irr_neg[pt] = irradiation_patch
+            df_irradiation_neg[pt] = irradiation_patch
         else:
-            df_irr_pos[pt] = irradiation_patch
+            df_irradiation_pos[pt] = irradiation_patch
     print('Limiting angle design', design_lim_angle)
-    print(len(df_irr_pos.columns), 'patches can NOT be seen')
-    print(len(df_irr_neg.columns), 'patches can be seen')
+    print(len(df_irradiation_pos.columns), 'patches can NOT be seen')
+    print(len(df_irradiation_neg.columns), 'patches can be seen')
 
-    df_irr_panel_t = df_irr_neg.sum(axis=1)
+    df_irradiation_panel_t = df_irradiation_neg.sum(axis=1)
 
-    df_irr_panel_t.index = pd.to_datetime(df_irr_panel_t.index)  # convert index to datetime
-    df_irr_panel_t = df_irr_panel_t.sort_index()
+    df_irradiation_panel_t.index = pd.to_datetime(df_irradiation_panel_t.index)  # convert index to datetime
+    df_irradiation_panel_t = df_irradiation_panel_t.sort_index()
 
     # construct annual sum
     df_period = np.array([])
 
     period_duration = typical_frequency.pop('PeriodDuration')
 
     for number, key in enumerate(list(typical_frequency.keys())[:-2]):
         hours_component = int(period_duration[number + 1])
         end = key + timedelta(hours=hours_component - 1)
-        irr_day = -1 * df_irr_panel_t.loc[key: end]
+        irr_day = -1 * df_irradiation_panel_t.loc[key: end]
         df_period = np.append(df_period, irr_day.values)
 
     df_period = np.append(df_period, [df_period.min(), df_period.max()])
 
-    return df_irr_panel_t, df_period
+    return df_irradiation_panel_t, df_period
 
 
-def calc_orientated_surface(azimuth, tilt, design_lim_angle, irradiation_file, typical_frequency):
-    df_irr_panel_t, df_typical = calc_orientation_profiles(azimuth, tilt, design_lim_angle, irradiation_file, typical_frequency)
+def calc_orientated_surface(azimuth, tilt, design_lim_angle, local_data, irradiation_file, typical_frequency):
+
+    df_irradiation_panel_t, df_typical = calc_orientation_profiles(azimuth, tilt, design_lim_angle, local_data, irradiation_file, typical_frequency)
 
     # construct annual sum
     df_period = pd.DataFrame()
 
     for key, value in typical_frequency.items():
-        irr_day = df_irr_panel_t.xs(key).sum() * (-value)
+        irr_day = df_irradiation_panel_t.xs(key).sum() * (-value)
         df_period = df_period.append([irr_day])
 
     annual_irr = round(df_period.sum().values[0] / 1000, 2)
 
     print('Sum of typical days is', annual_irr, 'kWh/m2')
 
     return azimuth, tilt, annual_irr
 
 
-def construct_annual_orientation_df(limiting_angle):
-
+def construct_annual_orientation_df(limiting_angle, local_data):
     azimuth = np.array(range(0, 360))
     tilt = np.array(range(0, 90, 5))
 
     df = pd.DataFrame()
     for (a, t) in it.product(azimuth, tilt):
-        azimuth, tilt, annual_irr = calc_orientated_surface(a, t, limiting_angle)
+        azimuth, tilt, annual_irr = calc_orientated_surface(a, t, limiting_angle, local_data)
         d = {'azimuth': azimuth, 'tilt': tilt, 'irr': annual_irr}
         df = df.append(d, ignore_index=True)
     print(df)
     filename = 'orientated_irr_linearized' + str(limiting_angle) + '.csv'
     df.to_csv(filename)
     print('Data saved in: ' + filename)
 
 
 def limiting_angle_for_tilt():
-
     a = 180
-    limit_angle = np.array(range(0,21,1))
-    tilt_1 = np.array(range(1,5,1))
-    tilt_2 = np.array(range(5,95,5))
+    limit_angle = np.array(range(0, 21, 1))
+    tilt_1 = np.array(range(1, 5, 1))
+    tilt_2 = np.array(range(5, 95, 5))
     tilt = np.append(tilt_1, tilt_2)
 
     df = pd.DataFrame()
 
     for (l, t) in it.product(limit_angle, tilt):
         azimuth, tilt, annual_irr = calc_orientated_surface(a, t, l)
 
@@ -332,18 +306,18 @@
     df.to_csv(filename)
     print('Data saved in: ' + filename)
 
 
 def plot_irr(save_fig):
     cm = plt.cm.get_cmap('Spectral_r')
 
-    #cm = plt.cm.get_cmap('cividis')
-    #cm = plt.cm.get_cmap('tab20c')
+    # cm = plt.cm.get_cmap('cividis')
+    # cm = plt.cm.get_cmap('tab20c')
 
-    #cm = plt.cm.get_cmap('GnBu')
+    # cm = plt.cm.get_cmap('GnBu')
 
     filename = os.path.join(path_to_skydome, 'orientated_irr.csv')
 
     df = pd.read_csv(filename, index_col=0)
 
     df_2 = df[(df['azimuth'] >= 80) & (df['azimuth'] <= 280)]
     df_3 = df_2[(df_2['irr'] >= 950) & (df_2['irr'] <= 1200)]
@@ -351,24 +325,23 @@
     condition = np.array(range(0, 90, 5))
     df_3 = df_3.loc[df_3.tilt.isin(condition)]
 
     #################################################################################################################
     # plotting: for all: plot df, for only tip plot df_3 (next line ax = df_3.plot....) change ax_xlim([])
     ###############################################################################################################
 
-    ax = df.plot.scatter(x='azimuth', y ='irr', c='tilt', cmap=cm, alpha=1, edgecolors='none', vmin=0, vmax=90)
+    ax = df.plot.scatter(x='azimuth', y='irr', c='tilt', cmap=cm, alpha=1, edgecolors='none', vmin=0, vmax=90)
 
-    #az_max = df_3.xs(df_3['irr'].idxmax())['azimuth']
-    #irr_max = df_3.xs(df_3['irr'].idxmax())['irr']
-    #tilt_max = df_3.xs(df_3['irr'].idxmax())['tilt']
+    # az_max = df_3.xs(df_3['irr'].idxmax())['azimuth']
+    # irr_max = df_3.xs(df_3['irr'].idxmax())['irr']
+    # tilt_max = df_3.xs(df_3['irr'].idxmax())['tilt']
 
-    #plt.scatter(az_max, irr_max, color='black')
+    # plt.scatter(az_max, irr_max, color='black')
 
-
-    #plt.text((az_max+5), irr_max, 'azimuth: '+str(int(az_max))+', ' + 'tilt: '+ str(int(tilt_max)))
+    # plt.text((az_max+5), irr_max, 'azimuth: '+str(int(az_max))+', ' + 'tilt: '+ str(int(tilt_max)))
     ax.set_xlim([90, 280])
     ax.set_xlim([0, 360])
     ax.set_xlabel('Azimuth angle [degree]')
     f = plt.gcf()
 
     cax = f.get_axes()[1]
     xax = f.get_axes()[0]
@@ -387,37 +360,33 @@
 
 if __name__ == '__main__':
 
     irradiation_file = os.path.join(path_to_skydome, 'typical_irradiation.csv')
     typical_days_string = ['20050921', '20050228', '20050810', '20050313', '20050725',
                            '20050107', '20050911',
                            '20050618']
-    typical_frequency = {'20050921':    54, '20050228':   46, '20050810':    17, '20050313':    49, '20050725':    52,
-                           '20050107':    68, '20050911':    49, '20050618':    30}
+    typical_frequency = {'20050921': 54, '20050228': 46, '20050810': 17, '20050313': 49, '20050725': 52,
+                         '20050107': 68, '20050911': 49, '20050618': 30}
 
-    #thisfile = os.path.join(path_to_clustering, 'timestamp.dat')
-    #df = pd.read_csv(thisfile, delimiter='\t')
+    # thisfile = os.path.join(path_to_clustering, 'timestamp.dat')
+    # df = pd.read_csv(thisfile, delimiter='\t')
 
-    #typical_days_string = df.Date.values
+    # typical_days_string = df.Date.values
 
-    #load_timesteps = np.array(range(1,8760))
-    #convert_results_txt_to_csv(load_timesteps)
-    #irradiation_to_typical_df(typical_days_string)
-    #skydome_to_tilt(tilt = 30)
-
-    #limiting_angle = 10  # = 0 for no irradiation losses
-    #construct_annual_orientation_df(limiting_angle)
-    #df_good = irradiation_to_df_general(irradiation_csv)
-    #df_wrong = irradiation_to_df(irradiation_csv)
-    save_fig = False
-    plt.rcParams.update({'font.size': 12})
-    plot_irr(save_fig)
-
-    #azimuth = 175
-    #tilt = 20
-    #design_lim_angle = 20
-    #print('design limiting angle:', design_lim_angle)
+    # load_timesteps = np.array(range(1,8760))
+    # convert_results_txt_to_csv(load_timesteps)
+    # irradiation_to_typical_df(typical_days_string)
+    # skydome_to_tilt(tilt = 30)
+
+    # limiting_angle = 10  # = 0 for no irradiation losses
+    # construct_annual_orientation_df(limiting_angle)
+    # df_good = irradiation_to_df_general(irradiation_csv)
+    # df_wrong = irradiation_to_df(irradiation_csv)
+
+    # azimuth = 175
+    # tilt = 20
+    # design_lim_angle = 20
+    # print('design limiting angle:', design_lim_angle)
     calc_orientated_surface(270, 90, 0, irradiation_file, typical_frequency)
-    #limiting_angle_for_tilt()
-    #df = skydome_to_df()
-    #print(df)
-
+    # limiting_angle_for_tilt()
+    # df = skydome_to_df()
+    # print(df)
```

### Comparing `REHO-1.0.2/reho/model/preprocessing/weather.py` & `reho-1.1.0/reho/model/preprocessing/weather.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,95 +2,125 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import calendar
 import datetime as dt
 from reho.paths import *
 from reho.model.preprocessing.clustering import ClusterClass
+import pvlib
+from pyproj import Transformer
+
 
 __doc__ = """
-*Generates the meteorological data (temperature and solar irradiance).*
+Generates the meteorological data (temperature and solar irradiance).
 """
 
+
 def get_cluster_file_ID(cluster):
     """
-    Gets the weather file ID that corresponds to what was given in the reho initalization:
-    ``cluster = {'Location': 'Geneva', 'Attributes': ['I', 'T', 'W'], 'Periods': 10, 'PeriodDuration': 24}``
+    Gets the weather file ID that corresponds to the specifications provided in the reho initalization.
 
-    Looks at data/weather/clustering results.
-    If that file does not exist yet, run the ClusterClass to create the required file.
+    The file ID is built by concatenating Location_Periods_PeriodDuration_Attributes.
+    ``cluster = {'Location': 'Geneva', 'Attributes': ['T', 'I', 'W'], 'Periods': 10, 'PeriodDuration': 24}``
+    Will yield to:
+    ``File_ID = 'Geneva_10_24_T_I_W'``
 
     Parameters
     ----------
     cluster : dict
-        Dictionary that contains a 'Location' (str), some 'Attributes' (list, among 'I', 'T', 'W'), a number of periods
-        'Periods' (int) and a 'PeriodDuration' (int)
+        Dictionary that contains a 'Location' (str), some 'Attributes' (list, among 'T' (temperature), 'I' (irradiance), 'W' (weekday) and 'E' (emissions)),
+        a number of periods 'Periods' (int) and a 'PeriodDuration' (int)
 
     Returns
     -------
-    A string that is the file ID
-
-    Notes
-    -----
-    - The file ID is built by concatenating Location_Periods_PeriodDuration_Attributes.
-    - The weather file is search using the Location
-    - If one wants to use his own meteo file, he can add to the cluster dictionary a key ``weather_file`` with the path
-      to the meteo. Should be a *.dat* with the same structure as the other weather_file.
+    A string that is the file ID.
     """
-    # get correct file ID for weather file
-    attributes = []
-
-    if 'I' in cluster['Attributes']:
-        I = '_I'
-        attributes.append('Irr')
-    else:
-        I = ''
     if 'T' in cluster['Attributes']:
         T = '_T'
-        attributes.append('Text')
     else:
         T = ''
+    if 'I' in cluster['Attributes']:
+        I = '_I'
+    else:
+        I = ''
     if 'W' in cluster['Attributes']:
         W = '_W'
-        attributes.append('Weekday')
     else:
         W = ''
     if 'E' in cluster['Attributes']:
         E = '_E'
     else:
         E = ''
 
-    File_ID = cluster['Location'] + '_' + str(cluster['Periods']) + '_' + str(cluster['PeriodDuration']) + \
-              T + I + W + E
-
-    among_cl_results = os.path.exists(os.path.join(path_to_clustering, 'timestamp_' + File_ID + '.dat'))
-    if not among_cl_results or 'weather_file' in cluster.keys():
-        if 'weather_file' in cluster.keys():
-            df = read_hourly_dat(cluster['weather_file'])
-        else:
-            df = read_hourly_dat(cluster['Location'])
-        df = df[attributes]
-        cl = ClusterClass(data=df, Iter=[cluster['Periods']], option={"year-to-day": True, "extreme": []}, pd=cluster['PeriodDuration'])
-        cl.run_clustering()
-
-        generate_output_data(cl, attributes, cluster['Location'])
+    File_ID = cluster['Location'] + '_' + str(cluster['Periods']) + '_' + str(cluster['PeriodDuration']) + T + I + W + E
 
     return File_ID
 
 
-def read_hourly_dat(location):
+def generate_weather_data(cluster, qbuildings_data):
+    """
+    This function is called if the clustered weather data specified by File_ID do not exist yet.
+    Runs the ClusterClass and create the required files.
+    """
 
-    if location.endswith('.dat'):
-        df = np.loadtxt(path_handler(location), unpack=True, skiprows=1)
+    if 'custom_weather' in cluster.keys():
+        df = read_custom_weather(cluster['custom_weather'])
     else:
-        df = np.loadtxt(os.path.join(path_to_weather, 'hour', location + '-hour.dat'), unpack=True, skiprows=1)
-    df = pd.DataFrame(df).transpose()
-    df = df.drop([5,6,7,8], axis=1)
-    df.columns = ['id', 'Month', 'Day', 'Hour', 'Irr', 'Text']
-    df2 = pd.read_csv(os.path.join(path_to_weather, 'Weekday_2005.txt'), index_col=[0], header=None)
+        df = get_weather_data(qbuildings_data).reset_index(drop=True)
+
+    attributes = []
+    if 'T' in cluster['Attributes']:
+        attributes.append('Text')
+    if 'I' in cluster['Attributes']:
+        attributes.append('Irr')
+    if 'W' in cluster['Attributes']:
+        attributes.append('Weekday')
+    if 'E' in cluster['Attributes']:
+        attributes.append('Emissions')
+
+    df = df[attributes]
+    cl = ClusterClass(data=df, nb_clusters=[cluster['Periods']], option={"year-to-day": True, "extreme": []}, pd=cluster['PeriodDuration'])
+    cl.run_clustering()
+
+    generate_output_data(cl, attributes, cluster['Location'])
+
+
+def get_weather_data(qbuildings_data):
+    """
+    Using the pvlib library, connects to the PVGIS dabatase to extract the weather data based on the building's coordinates.
+    """
+    lat, long = Transformer.from_crs("EPSG:2056", "EPSG:4326").transform(qbuildings_data['buildings_data']['Building1']['x'],
+                                                                         qbuildings_data['buildings_data']['Building1']['y'])
+
+    pvgis_data = pvlib.iotools.get_pvgis_tmy(lat, long, outputformat='csv', startyear=2005, endyear=2016)
+    location = pvgis_data[2]
+    weather_data = pvgis_data[0]
+    weather_data = weather_data.rename(columns={'temp_air': 'Text', 'ghi': 'Irr'})
+    weather_data['Month'] = weather_data.index.month
+    weather_data['Day'] = weather_data.index.day
+    weather_data['Hour'] = weather_data.index.hour + 1
+    weather_data['id'] = (weather_data.reset_index().index + 1).to_list()
+    weekday = pd.read_csv(os.path.join(path_to_weather, 'weekday.txt'), index_col=[0], header=None)
+    weather_data['Weekday'] = weekday[1].tolist()
+
+    print(f'The weather data have been loaded from the PVGIS database for a location with coordinates {location}.')
+
+    return weather_data
+
+
+def read_custom_weather(path_to_weather_file):
+    """
+    From the current directory, looks for a custom weather file.
+    This file should be a *.csv* with the same structure as the template provided in reho/scripts/template/data/profiles/.
+    """
+
+    df = file_reader(path_handler(path_to_weather_file))
+    print(f'The weather data have been loaded from {path_handler(path_to_weather_file)}.')
+
+    df2 = pd.read_csv(os.path.join(path_to_weather, 'weekday.txt'), index_col=[0], header=None)
     df['Weekday'] = df2
 
     return df
 
 
 def generate_output_data(cl, attributes, location):
     """
@@ -114,15 +144,15 @@
         The extreme temperatures and irradiance are estimated by adding 10% to the extreme found in the yearly weather data.
 
     See also
     --------
     reho.model.preprocessing.clustering.ClusterClass.run_clustering
     write_dat_files
     """
-    
+
     data_idx = cl.results["idx"]
     # - construct : cluster data
     frame = []
     cl.nbr_opt = str(cl.nbr_opt)
     for idx in data_idx.loc[:, cl.nbr_opt].unique():  # get unique typical periods from index vector
         idx = int(idx)
         df = pd.DataFrame(
@@ -153,15 +183,15 @@
     T_max = cl.data_org.iloc[[T_idx[1]]].copy()
     T_max['Irr'] = cl.data_org.loc[T_day[1] * 24: T_day[1] * 24 + 24, 'Irr'].max()
     T_min.loc[:, ['time.dd', 'time.hh', 'dt']] = [T_day[0], 1, 1]
     T_max.loc[:, ['time.dd', 'time.hh', 'dt']] = [T_day[1], 1, 1]
     data_cls = pd.concat([data_cls, T_min.rename({T_idx[0]: 240}), T_max.rename({T_idx[1]: 241})])
     # Add a 10% margin for the extreme over 20 years
     data_cls.loc[[240, 241], ['Text', 'Irr']] = data_cls.loc[[240, 241], ['Text', 'Irr']] * 1.1
-   
+
     # - construct : model data
     # - ** inter-period
     data_idy = pd.DataFrame(
         np.stack((np.arange(1, data_idx.loc[:, cl.nbr_opt].shape[0] + 1, 1), data_idx.loc[:, cl.nbr_opt].values),
                  axis=1), columns=["IndexYr", "inter_t"])
     if cl.modulo != 0:
         max_time_dd = len(cl.attr_org)
@@ -169,30 +199,30 @@
                              ignore_index=True)
 
     # - ** intra-period
     data_idp = pd.DataFrame(
         np.stack((np.arange(1, data_cls.shape[0] + 1, 1), np.arange(1, data_cls.shape[0] + 1, 1)), axis=1),
         columns=["IndexDy", "intra_t"])
     data_idp["intra_end"] = [id + cl.pd if (id % cl.pd) == 0 else 0 for id in data_idp.index]
-    
+
     # Call for the write_dat_files function
     write_dat_files(attributes, location, data_cls, data_idy)
-    
+
     return print(f'The data have been computed and saved in {path_to_clustering}.')
 
 
 def write_dat_files(attributes, location, values_cluster, index_inter):
     """
     Writes the clustering results computed from `generate_output_data` as .dat file
 
     Parameters
     ----------
     attributes : list
         List that contains string among 'Irr', 'Text', 'Weekday'.
-        If 'Irr' is in the list, writes a file named 'GHI' + '_File_ID.dat'
+        If 'Irr' is in the list, writes a file named 'Irr' + '_File_ID.dat'
         If 'Text' is in the list, writes a file named 'T' + '_File_ID.dat'
     location : str
         Location of the corresponding weather data.
     values_cluster : pd.DataFrame
         Produced by the *generate_output_data* function.
     index_inter : pd.DataFrame
         Produced by the *generate_output_data* function.
@@ -244,19 +274,19 @@
     # T
     # -------------------------------------------------------------------------------------
     df_T = values_cluster['Text']
     filename = os.path.join(path_to_clustering, 'T_' + File_ID + '.dat')
     df_T.to_csv(filename, index=False, header=False)
 
     # -------------------------------------------------------------------------------------
-    # GHI
+    # Irr
     # -------------------------------------------------------------------------------------
-    df_GHI = values_cluster['Irr']
-    filename = os.path.join(path_to_clustering, 'GHI_' + File_ID + '.dat')
-    df_GHI.to_csv(filename, index=False, header=False)
+    df_Irr = values_cluster['Irr']
+    filename = os.path.join(path_to_clustering, 'Irr_' + File_ID + '.dat')
+    df_Irr.to_csv(filename, index=False, header=False)
 
     # -------------------------------------------------------------------------------------
     # frequency
     # -------------------------------------------------------------------------------------
     if 'Weekday' in attributes:
         Weekday = np.array([])
         for dd in df_dd:
@@ -292,15 +322,16 @@
     # index
     # -------------------------------------------------------------------------------------
     df_time = pd.DataFrame()
     df_time['originalday'] = df_dd
     df_time['frequency'] = dp
     df_time['timesteps'] = pt
     dict_index = {}
-    for i, dd in enumerate(df_dd): dict_index[dd] = i + 1
+    for i, dd in enumerate(df_dd):
+        dict_index[dd] = i + 1
     index_inter['index_r'] = index_inter.inter_t.map(dict_index)
     df_time.index = df_time.index + 1
 
     df_aim = pd.DataFrame()
     for d in index_inter['index_r']:
         nt = int(df_time['timesteps'].xs(d))  # number of timesteps
         df_d = pd.DataFrame([np.repeat(d, nt), np.array(range(1, (nt + 1)))])
@@ -344,17 +375,17 @@
     df.columns.names = ['KPI']
     df.rename({'Irr': 'Global Irradiation', 'Text': 'Ambient Temperature'}, inplace=True)
     df_irr = df.xs('Global Irradiation', level=1)
     df_T = df.xs('Ambient Temperature', level=1)
 
     fig, ax = plt.subplots()
     fig.set_size_inches(4, 8)
-    df_irr['RMSD'].plot(linestyle='--', color='black', label='RMSD (GHI)', ax=ax)
+    df_irr['RMSD'].plot(linestyle='--', color='black', label='RMSD (Irr)', ax=ax)
     df_T['RMSD'].plot(linestyle='-', color='black', label='RMSD (T)', ax=ax)
-    df_irr['LDC'].plot(linestyle='--', color="red", label='LDC (GHI)', ax=ax)
+    df_irr['LDC'].plot(linestyle='--', color="red", label='LDC (Irr)', ax=ax)
     df_T['LDC'].plot(linestyle='-', color="red", label='LDC (T)', ax=ax)
 
     plt.xlabel('number of clusters [-]')
     plt.ylabel('key performance indicator (KPI) [-]')
     # plt.title('KPI for $ \u2B27 $ =  Global Irradiation, $\u00D7$ = Ambient Temperature', size = 14)
     plt.legend(title="KPI")
 
@@ -364,15 +395,15 @@
         export_format = 'pdf'
         plt.savefig(('Cluster_KPIs' + '.' + export_format), format=export_format, dpi=300)
     else:
         plt.show()
 
     fig, ax = plt.subplots()
     fig.set_size_inches(4, 8)
-    df_irr['MAE'].plot(linestyle='--', color='black', label='MAE (GHI)', ax=ax)
+    df_irr['MAE'].plot(linestyle='--', color='black', label='MAE (Irr)', ax=ax)
     df_T['MAE'].plot(linestyle='-', color='black', label='MAE (T)', ax=ax)
 
     plt.xlabel('number of clusters [-]')
     plt.ylabel('mean average error (MAE)  [-]')
     # plt.title('KPI for $ \u2B27 $ =  Global Irradiation, $\u00D7$ = Ambient Temperature', size = 14)
     plt.legend(title="KPI")
     # plt.ylim([0,0.40])
@@ -381,15 +412,15 @@
         export_format = 'pdf'
         plt.savefig(('MAE_KPIs' + '.' + export_format), format=export_format, dpi=300)
     else:
         plt.show()
 
     fig, ax = plt.subplots()
     fig.set_size_inches(4, 8)
-    df_irr['MAPE'].plot(linestyle='--', color='black', label='MAPE  (GHI)', ax=ax)
+    df_irr['MAPE'].plot(linestyle='--', color='black', label='MAPE  (Irr)', ax=ax)
     df_T['MAPE'].plot(linestyle='-', color='black', label='MAPE  (T)', ax=ax)
 
     plt.xlabel('number of clusters [-]')
     plt.ylabel('mean average percentage error  [-]')
     # plt.title('KPI for $ \u2B27 $ =  Global Irradiation, $\u00D7$ = Ambient Temperature', size = 14)
     plt.legend(title="KPI")
     # plt.ylim([0,0.40])
@@ -397,62 +428,60 @@
         plt.tight_layout()
         export_format = 'pdf'
         plt.savefig(('MAPE_KPIs' + '.' + export_format), format=export_format, dpi=300)
     else:
         plt.show()
 
 
-def plot_LDC(cl, location, save_fig):
+def plot_LDC(cl, save_fig):
     nbr_plot = cl.nbr_opt
     print('plotting for number of typical days: ', nbr_plot)
 
     # get original, not clustered data
     T_org = cl.data_org['Text']
     IRR_org = cl.data_org['Irr']
-   # E_org= cl.data_org['Emissions']
+    # E_org= cl.data_org['Emissions']
 
     # get clustered data and undo normalization
     df_clu = cl.attr_clu.xs(str(nbr_plot), axis=1)
     T_clu = df_clu['Text'] * (T_org.max() - T_org.min()) + T_org.min()
     IRR_clu = df_clu['Irr'] * (IRR_org.max() - IRR_org.min()) + IRR_org.min()
-  #  E_clu= df_clu['Emissions']* (E_org.max() - E_org.min()) + E_org.min()
-
+    #  E_clu= df_clu['Emissions']* (E_org.max() - E_org.min()) + E_org.min()
 
     # get assigned typical period
     res = cl.results['idx'][str(nbr_plot)]
     # instead of typical period (f.e. day 340) get index (1)
-    for i, d in enumerate(res.unique()): res = np.where(res == d, i + 1, res)
+    for i, d in enumerate(res.unique()):
+        res = np.where(res == d, i + 1, res)
     # get array of 8760 -modulo timesteps
     res = np.repeat(res, cl.pd)
 
     # add modulo
     modulo = cl.data_org.shape[0] % cl.pd
     res = np.append(res, np.repeat(int(nbr_plot) + 1, modulo))  # add modulo as extra period
 
     # ----------------------------------------------------------------------------
     # Plotting
     # ------------------------------------------------------------------------
 
     fig, ax = plt.subplots(2, 1, sharex=True, figsize=(10, 8))
 
-
     ax[0].plot(T_org, color='grey', alpha=0.5)
     sc = ax[0].scatter(T_clu.index, T_clu.values, s=10, c=res, cmap=cm)
     ax[1].plot(IRR_org, color='grey', alpha=0.5)
     ax[1].scatter(IRR_clu.index, IRR_clu.values, s=10, c=res, cmap=cm)
-    #ax[2].plot(E_org, color='grey', alpha=0.5)
-    #ax[2].scatter(E_clu.index, E_clu.values, s=10, c=res, cmap=cm)
-
+    # ax[2].plot(E_org, color='grey', alpha=0.5)
+    # ax[2].scatter(E_clu.index, E_clu.values, s=10, c=res, cmap=cm)
 
     # set months instead of timestep as xticks
-    plt.xticks(np.arange(8760, step=730), calendar.month_name[1:13], rotation=20)
+    plt.xticks(np.arange(8760, step=730), calendar.month_name[1:13], rotation=30, fontsize=16)
 
     ax[0].set_ylabel('temperature [C]')
     ax[1].set_ylabel('global irradiation [W/m$^2$]')
-  #  ax[2].set_ylabel('global warming potential [gCO2/kWh]')
+    # ax[2].set_ylabel('global warming potential [gCO2/kWh]')
     # plt.subplots_adjust(bottom=0.1, right=0.8, top=0.9)
 
     legend1 = ax[0].legend(*sc.legend_elements(),
                            loc='upper right', bbox_to_anchor=(1.0, 1.0), title="Period", ncol=2)
     ax[0].add_artist(legend1)
 
     if save_fig:
@@ -466,60 +495,60 @@
     df_T['Period'] = res
     df_T = df_T.sort_values(by=['Text'], ignore_index=True, ascending=False)
 
     df_Irr = pd.DataFrame(IRR_clu)
     df_Irr['Period'] = res
     df_Irr = df_Irr.sort_values(by=['Irr'], ignore_index=True, ascending=False)
 
-   # df_E = pd.DataFrame(E_clu)
-   # df_E['Period'] = res
-   # df_E = df_E.sort_values(by=['Emissions'], ignore_index=True, ascending=False)
+    # df_E = pd.DataFrame(E_clu)
+    # df_E['Period'] = res
+    # df_E = df_E.sort_values(by=['Emissions'], ignore_index=True, ascending=False)
 
     T_sort = T_org.sort_values(ascending=False, ignore_index=True)
     IRR_sort = IRR_org.sort_values(ascending=False, ignore_index=True)
-  #  E_sort =  E_org.sort_values(ascending=False, ignore_index=True)
-
+    # E_sort =  E_org.sort_values(ascending=False, ignore_index=True)
 
     fig, ax = plt.subplots(2, 1, sharex=True, figsize=(10, 8))
     ax[0].scatter(T_sort.index, T_sort.values, color='grey', alpha=0.5)
     ax[0].scatter(df_T.index, df_T['Text'], c=df_T['Period'], cmap=cm, s=20)
 
     ax[1].scatter(IRR_sort.index, IRR_sort.values, color='grey', alpha=0.5)
     ax[1].scatter(df_Irr.index, df_Irr['Irr'], c=df_Irr['Period'], cmap=cm, s=20)
 
-  #  ax[2].scatter(E_sort.index, E_sort.values, color='grey', alpha=0.5)
-   # ax[2].scatter(df_E.index, df_E['Emissions'], c=df_Irr['Period'], cmap=cm, s=20)
+    #  ax[2].scatter(E_sort.index, E_sort.values, color='grey', alpha=0.5)
+    # ax[2].scatter(df_E.index, df_E['Emissions'], c=df_Irr['Period'], cmap=cm, s=20)
 
     ax[0].set_ylabel('temperature [C]')
     ax[1].set_ylabel('global irradiation [W/m$^2$]')
-   # ax[2].set_ylabel('global warming potential [gCO2/kWh]')
+    # ax[2].set_ylabel('global warming potential [gCO2/kWh]')
 
     plt.xlabel('Hours [h]')
 
     legend1 = ax[0].legend(*sc.legend_elements(),
                            loc='upper right', bbox_to_anchor=(1.0, 1.0), title="Period", ncol=2)
     ax[0].add_artist(legend1)
 
     if save_fig:
         plt.tight_layout()
         format = 'pdf'
         plt.savefig(('LDC' + '.' + format), format=format, dpi=300)
     else:
         plt.show()
 
+
 if __name__ == '__main__':
     cm = plt.cm.get_cmap('Spectral_r')
 
-    # Location = ['Bern-Liebefeld', 'Geneve-Cointrin', 'La_Chaux-de-Fonds', 'Moleson', 'Zermatt', 'Zuerich-SMA'][4]
-    Location = 'Pully'
+    weather_file = '../../../scripts/template/data/profiles/Sion.csv'
     Attributes = ['Text', 'Irr']
-    Iter = [10]
+    nb_clusters = [2, 4, 6, 8, 10, 12]
 
-    df = read_hourly_dat(Location)
-    df = df[Attributes]
+    df_annual = read_custom_weather(weather_file)
+    df_annual = df_annual[Attributes]
 
-    cl = ClusterClass(data=df, Iter=Iter, option={"year-to-day": True, "extreme": []}, pd=24)
+    cl = ClusterClass(data=df_annual, nb_clusters=nb_clusters, option={"year-to-day": True, "extreme": []}, pd=24)
     cl.run_clustering()
 
     plot_cluster_KPI_separate(cl.kpis_clu, save_fig=False)
-    plot_LDC(cl, Location, save_fig=False)
-    generate_output_data(cl, Attributes, Location)
+    plot_LDC(cl, save_fig=False)
+
+    generate_output_data(cl, Attributes, "Sion")
```

### Comparing `REHO-1.0.2/reho/paths.py` & `reho-1.1.0/reho/paths.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from csv import Sniffer
 from pathlib import Path
 from pandas import read_csv, read_table, read_excel
 import sys
 from dotenv import load_dotenv
 
 __doc__ = """
-*File for managing file paths and configurations.*
+File for managing file paths and configurations.
 """
 
-
 load_dotenv()
 if "AMPL_PATH" not in os.environ:
     print("AMPL_PATH is not defined. Please include a .env file at the project root (e.g., AMPL_PATH='C:/AMPL')")
 
 path_to_reho = os.path.dirname(__file__)
 path_to_data = os.path.join(path_to_reho, 'data')
 path_to_model = os.path.join(path_to_reho, 'model')
@@ -28,34 +27,39 @@
 
 # data
 
 # elcom
 path_to_elcom = os.path.join(path_to_data, 'elcom')
 
 # emissions
-path_to_emissions_matrix = os.path.join(path_to_data, 'emissions', 'electricity_matrix_2019_reduced.csv')
+path_to_emissions = os.path.join(path_to_data, 'emissions', 'electricity_matrix_2019_reduced.csv')
 
 # infrastructure
 path_to_infrastructure = os.path.join(path_to_data, 'infrastructure')
 
 # QBuildings
 path_to_qbuildings = os.path.join(path_to_data, 'QBuildings')
 
 # SIA
 path_to_sia = os.path.join(path_to_data, 'SIA')
+path_to_sia_equivalence = os.path.join(path_to_sia, 'sia2024_rooms_sia380_1.csv')
+path_to_sia_norms = os.path.join(path_to_sia, 'sia2024_data.xlsx')
 
 # skydome
 path_to_skydome = os.path.join(path_to_data, 'skydome')
+path_to_irradiation = os.path.join(path_to_skydome, 'total_irradiation.csv')
+path_to_areas = os.path.join(path_to_skydome, 'skyPatchesAreas.txt')  # area of patches
+path_to_cenpts = os.path.join(path_to_skydome, 'skyPatchesCenPts.txt')  # location of centre points
 
 # weather
 path_to_weather = os.path.join(path_to_data, 'weather')
 
 # scripts specific paths
 path_to_clustering = os.path.join(os.getcwd(), 'data', 'clustering')
-path_to_configurations = os.path.join(os.getcwd(), 'configurations')
+path_to_configurations = os.path.join(os.getcwd(), 'results', 'configurations')
 
 
 def path_handler(path_given):
     """To handle the path to csv file, absolute path or not"""
 
     if os.path.isabs(path_given):
         if os.path.isfile(path_given):
@@ -81,8 +85,8 @@
             return read_csv(file, sep=delim.delimiter, index_col=index_col)
         elif file.suffix == '.xlsx':
             return read_excel(file)
         else:
             return read_table(file)
     except:
         print('It seems there is a problem when reading the file...\n')
-        print("%s" % sys.exc_info()[1])
+        print("%s" % sys.exc_info()[1])
```

### Comparing `REHO-1.0.2/reho/plotting/layout.csv` & `reho-1.1.0/reho/plotting/layout.csv`

 * *Files identical despite different names*

### Comparing `REHO-1.0.2/reho/plotting/plotting.py` & `reho-1.1.0/reho/plotting/plotting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,476 +1,599 @@
-import re
-import pandas as pd
-import numpy as np
-from reho.paths import *
-from reho.plotting import sankey
+import locale
+
+import matplotlib.patches as mpatches
 import plotly.graph_objects as go
-from plotly.subplots import make_subplots
 from matplotlib import pyplot as plt
-import matplotlib.patches as mpatches
-from matplotlib.lines import Line2D
 from matplotlib.legend_handler import HandlerTuple
-import locale, calendar
-from reho.model.compact_optimization import *
+from matplotlib.lines import Line2D
+from plotly.subplots import make_subplots
+
+from reho.model.sub_problem import *
+from reho.plotting.utils import *
+from reho.plotting import sankey
 
 
 __doc__ = """
-*Contains ready-to-use representations for results generated by REHO.*
+Contains ready-to-use representations for results generated by REHO.
 """
-# ---------------------------------------------------------------------------------------------
-# Definition of colors and labels
-cm = dict({'ardoise': '#413D3A', 'perle': '#CAC7C7', 'rouge': '#FF0000', 'groseille': '#B51F1F',
-           'canard': '#007480', 'leman': '#00A79F', 'salmon': '#FEA993', 'green': '#69B58A', 'yellow': '#FFB100',
-           'darkblue': '#1246B5', 'lightblue': '#8bacf4', 'perle_light': '#dad8d8',
-           'canard_light': '#4d9ea6', 'leman_light': '#4dc2bc', 'salmon_light': '#fec3b4',
-           'groseille_light': "#ff6666", 'darkyellow': '#A57300', 'dark': '#000000',
-           'yellow_light': '#FECC93'})
-
-# Colors and labels for units and layers
-layout = pd.read_csv(os.path.join(path_to_plotting, 'layout.csv'), index_col='Name').dropna(how='all')
-
-
-# ---------------------------------------------------------------------------------------------
-
-def dict_to_df(results, df):
-    t = {(Scn_ID, Pareto_ID): results[Scn_ID][Pareto_ID][df]
-         for Scn_ID in results.keys()
-         for Pareto_ID in results[Scn_ID].keys()}
-
-    df_merged = pd.concat(t.values(), keys=t.keys(), names=['Scn_ID', 'Pareto_ID'], axis=0)
 
-    return df_merged
 
+################################################################################################################################################################
+# Plotly
+################################################################################################################################################################
 
-def moving_average(data, n):
-    return np.convolve(data, np.ones(n), 'valid') / n
 
-
-def handle_zero_rows(df):
-    is_zero_row = (df == 0).all(axis=1)
-
-    return df.loc[~is_zero_row]
-
-
-def prepare_dfs(df_eco, indexed_on='Scn_ID', neg=False, premium_version=False,
-                additional_costs={}, scaling_factor=1):
+def plot_performance(results, plot='costs', indexed_on='Scn_ID', label='EN_long', add_annotation=True, per_m2=False, additional_costs=None, additional_gwp=None,
+                     scc=0.177,
+                     filename=None, export_format='html', scaling_factor=1, return_df=False):
     """
-    This function prepares the dataframes that will be needed for the plot_performance and plot_actors
-    """
-    df_eco = df_eco.xs('Network', level='Hub', axis=0)
-    df_eco = df_eco.groupby(level=indexed_on, sort=False).sum() * scaling_factor
-    indexes = df_eco.index.tolist()
-
-    data_capex = df_eco.xs('investment', level='Category', axis=1).transpose()
-    data_capex.index.names = ['Unit']
-
-    if 'isolation' in additional_costs:
-        data_capex.loc[('Isolation'), :] = additional_costs['isolation']
-
-    data_capex = data_capex.reset_index().merge(layout, left_on="Unit", right_on='Name').set_index("Unit").fillna(0)
-
-    data_opex = df_eco.xs('operation', level='Category', axis=1).transpose()
-    indices = data_opex.index.get_level_values(0)
-    new_indices = []
-    [new_indices.append(tuple(idx.split("_", 1))) for idx in indices]
-    for i, tup in enumerate(new_indices):
-        if tup == ('costs', 'Electricity'):
-            new_indices[i] = ('costs', 'Electrical_grid')
-        elif tup == ('revenues', 'Electricity'):
-            new_indices[i] = ('revenues', 'Electrical_grid_feed_in')
-    data_opex.index = pd.MultiIndex.from_tuples(new_indices, names=['type', 'Layer'])
-
-    if premium_version:
-        data_opex.loc[('avoided', 'solar_premium'), :] = data_opex.loc[('avoided', 'PV_SC')] * (0.279 - 0.1645) / 0.279
-        data_opex.loc[('revenues', 'solar_value'), :] = data_opex.loc[('revenues', 'Electrical_grid_feed_in')] + \
-                                                        data_opex.loc[('avoided', 'PV_SC')] - data_opex.loc[
-                                                            ('avoided', 'solar_premium')]
-        data_opex = data_opex.drop("PV_SC", level='Layer')
-        data_opex = data_opex.drop("Electrical_grid_feed_in", level='Layer')
-
-    data_opex = data_opex.drop("PV", level='Layer')
-
-    if 'mobility' in additional_costs:
-        data_opex.loc[('costs', 'Gasoline'), :] = additional_costs['mobility']
-
-    if 'ict' in additional_costs:
-        data_opex.loc[('costs', 'ict'), :] = additional_costs['ict']
-
-    if neg:
-        indices = data_opex.index.get_level_values(0)
-        neg_indices = indices.str.contains('avoided')
-        neg_indices = neg_indices + indices.str.contains('revenues')
-        data_opex.loc[neg_indices] = - data_opex.loc[neg_indices]
-    data_opex = data_opex.reset_index().merge(layout, left_on='Layer', right_on='Name').set_index(['type', 'Layer'])
-
-    return indexes, data_capex, data_opex
+    Plots performance based on REHO results.
 
-
-def remove_building_from_index(df):
-    """
-    Removes the Building_[123] appended to the name of the units in the index
-    """
-
-    def filter_building_str(str):
-        str_split = str.split("_")
-        if len(str_split) > 2:
-            new_idx = "_".join(str.split("_", 2)[:2])
-        else:
-            new_idx = str_split[0]
-        return new_idx
-
-    new_index = []
-    index_frame = df.index.to_frame()
-    if 'Unit' in index_frame.columns:
-        for idx in index_frame['Unit']:
-            new_index.append(filter_building_str(idx))
-        index_frame['Unit'] = new_index
-    if 'Hub' in index_frame.columns:
-        for idx in index_frame['Hub']:
-            new_index.append(filter_building_str(idx))
-        index_frame['Hub'] = new_index
-
-    index_modified = pd.MultiIndex.from_frame(index_frame)
-
-    return df.set_index(index_modified)
-
-
-def plot_performance(results, plot='costs', indexed_on='Scn_ID', label='EN_long', add_annotation=True, per_m2=False,
-                     additional_costs={}, filename=None,
-                     export_format='html', scaling_factor=1, return_df=False):
-    """
-    Plot performance based on REHO results.
-
-    :param results: Dictionary of REHO results.
-    :type results: dict
-    :param plot: Choose among 'costs' and 'gwp'.
-    :type plot: str
-    :param label: Indicates the language to use for the plot. Pick among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
-    :type label: str
-    :param indexed_on: Whether the results should be grouped on Scn_ID or Pareto_ID.
-    :type indexed_on: str
-    :param add_annotation: Adds the numerical values along the bar plots.
-    :type add_annotation: bool
-    :param per_m2: Set to True to obtain the results divided by the total ERA.
-    :type per_m2: bool
-    :param additional_costs: Dictionary of additional costs to include (choose between 'isolation', 'mobility', and 'ict') and scaling values.
-    :type additional_costs: dict
-    :param filename: Name of the file to be saved.
-    :type filename: str
-    :param export_format: Can be either 'html', 'png', or 'plotly_plot'.
-    :type export_format: str
-    :param scaling_factor: Scaling factor for the plot if a linear assumption is made.
-    :type scaling_factor: int or float
-    :param return_df: A dataframe can be returned for further post-processing or reporting purposes.
-    :type return_df: bool
-
-    :return: (Optional) A dataframe for further post-processing or reporting purposes.
-    :rtype: pd.DataFrame or None
+    Parameters
+    ----------
+    results: dict
+        Dictionary of REHO results.
+    plot: str
+        Choose among those three possibilities:
+
+        - 'costs' for the economic performance indicators,
+        - 'gwp' for the global warming potential indicators,
+        - 'combined' for a combination of the two indicators, where the emissions are converted into costs using the ``scc`` parameter.
+    indexed_on: str
+        Whether the results should be grouped on *Scn_ID* or *Pareto_ID*.
+    label: str
+        Indicates the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
+    add_annotation: bool
+        Adds the numerical values along the bar plots.
+    per_m2: bool
+        Set to True to obtain the results divided by the total ERA.
+    additional_costs: dict
+        Additional costs to include (choose between 'isolation', 'mobility', and 'ict') and scaling values.
+    additional_gwp: dict
+        Additional gwp to include (choose between 'isolation', 'mobility', and 'ict') and scaling values.
+    scc: float
+        Carbon externalities, expressed in *CHF/kgCO2*. Default value is the *Social Cost of Carbon*, from `Rennert, 2022 <https://www.nature.com/articles/s41586-022-05224-9>`_.
+    filename: str
+        Name of the file to be saved.
+    export_format: str
+        Can be either 'html', 'png', or 'pdf'.
+    scaling_factor: int/float
+        Scales linearly the REHO results for the plot.
+    return_df: bool
+        A dataframe can be returned for further post-processing or reporting purposes.
+
+    Returns
+    ----------
+    plotly.graph_objs.Figure
+        The generated plotly figure.
+    pd.DataFrame
+        (Optional) A dataframe for further post-processing or reporting purposes.
     """
 
+    if additional_gwp is None:
+        additional_gwp = {}
+    if additional_costs is None:
+        additional_costs = {}
     sc = list(results.keys())[0]
     id = list(results[sc].keys())[0]
     era = results[sc][id]['df_Buildings'].ERA
 
-    df_eco = dict_to_df(results, 'df_Economics')
+    df_Economics = dict_to_df(results, 'df_Economics')
 
     change_data = pd.DataFrame()
-    change_data.index = ['col_1', 'col_2', 'x_axis_1', 'x_axis_2', 'y_axis', 'keyword', 'total', 'unites']
+    change_data.index = ['x_axis_1', 'x_axis_2', 'y_axis', 'keyword', 'total', 'unites', 'scc_legend']
+    decimal = 0
     lang = re.split('_', label)[0]
+
     if plot == 'costs':
-        change_data['FR'] = ['Costs_Unit_inv', 'price', 'CAPEX', 'OPEX', 'Coûts [CHF/an]', 'Coûts', 'TOTEX', 'CHF']
-        change_data['EN'] = ['Costs_Unit_inv', 'price', 'CAPEX', 'OPEX', 'Costs [CHF/y]', 'Costs', 'TOTEX', 'CHF']
-        df_eco = df_eco.xs('costs', level='Perf_type')
-    elif plot == 'gwp':
-        change_data['FR'] = ['GWP_Unit_constr', 'gwp', 'Construction', 'Réseau', 'GWP [kgCO2/an]', 'Émissions', 'Total',
-                             'kgCO2']
-        change_data['EN'] = ['GWP_Unit_constr', 'gwp', 'Construction', 'Grid', 'GWP [kgCO2/y]', 'Emissions', 'Total',
-                             'kgCO2']
-        df_eco = df_eco.xs('impact', level='Perf_type')
-
-    if per_m2:
-        df_eco = df_eco / era.sum()
-        change_data.loc['y_axis']['FR'] = "Coûts [CHF/m2/an]"
-        change_data.loc['y_axis']['EN'] = "Costs [CHF/m2/y]"
+        change_data['FR'] = ['CAPEX', 'OPEX', 'Coûts [CHF/an]', 'Coûts', 'TOTEX', ' CHF', '']
+        change_data['EN'] = ['CAPEX', 'OPEX', 'Costs [CHF/y]', 'Costs', 'TOTEX', ' CHF', '']
+        df_costs = df_Economics.xs('costs', level='Perf_type')
+        if per_m2:
+            df_costs = df_costs / era.sum()
+            change_data.loc['y_axis']['FR'] = "Coûts [CHF/m2/an]"
+            change_data.loc['y_axis']['EN'] = "Costs [CHF/m2/y]"
+            decimal = 1
+        indexes, data_capacities, data_resources = prepare_dfs(df_costs, indexed_on, neg=True, additional_data=additional_costs, scaling_factor=scaling_factor)
+
+        data_resources = data_resources.drop("avoided", level='type')
 
-    indexes, data_capex, data_opex = prepare_dfs(df_eco, indexed_on, neg=True, additional_costs=additional_costs,
-                                                 scaling_factor=scaling_factor)
+        data_scc_resources = pd.DataFrame(0, columns=[indexes], index=data_resources.index)
+        data_scc_capacities = pd.DataFrame(0, columns=[indexes], index=data_capacities.index)
 
-    data_opex = data_opex.drop("avoided", level='type')
+        showlegend = False
+
+    elif plot == 'gwp':
+        change_data['FR'] = ['Capacités', 'Ressources', 'Émissions [kgCO2/an]', 'Émissions', 'Total', ' kgCO2', '']
+        change_data['EN'] = ['Capacities', 'Resources', 'Emissions [kgCO2/y]', 'Emissions', 'Total', ' kgCO2', '']
+        df_impact = df_Economics.xs('impact', level='Perf_type')
+        if per_m2:
+            df_impact = df_impact / era.sum()
+            change_data.loc['y_axis']['FR'] = "Émissions [kgCO2/m2/an]"
+            change_data.loc['y_axis']['EN'] = "Emissions [kgCO2/m2/y]"
+            decimal = 1
+        indexes, data_capacities, data_resources = prepare_dfs(df_impact, indexed_on, neg=True, additional_data=additional_gwp, scaling_factor=scaling_factor)
+
+        data_resources = data_resources.drop("avoided", level='type')
+
+        data_scc_resources = pd.DataFrame(0, columns=[indexes], index=data_resources.index)
+        data_scc_capacities = pd.DataFrame(0, columns=[indexes], index=data_capacities.index)
+
+        showlegend = False
+
+    elif plot == 'combined':
+        change_data['FR'] = ['Capacités', 'Ressources', 'Coûts [CHF/an]', 'Coûts', 'TOTEX', ' CHF', 'Impact carbone']
+        change_data['EN'] = ['Capacities', 'Resources', 'Costs [CHF/y]', 'Costs', 'TOTEX', ' CHF', 'Carbon impact']
+
+        df_costs = df_Economics.xs('costs', level='Perf_type')
+        df_impact = df_Economics.xs('impact', level='Perf_type')
+        if per_m2:
+            df_costs = df_costs / era.sum()
+            df_impact = df_impact / era.sum()
+            change_data.loc['y_axis']['FR'] = "Coûts [CHF/m2/an]"
+            change_data.loc['y_axis']['EN'] = "Costs [CHF/m2/y]"
+            decimal = 1
+        indexes, data_capacities, data_resources = prepare_dfs(df_costs, indexed_on, neg=True,
+                                                               additional_data=additional_costs,
+                                                               scaling_factor=scaling_factor)
+        indexes, data_scc_capacities, data_scc_resources = prepare_dfs(df_impact, indexed_on, neg=True,
+                                                                       additional_data=additional_gwp,
+                                                                       scaling_factor=scaling_factor)
+
+        data_resources = data_resources.drop("avoided", level='type')
+        data_scc_resources = data_scc_resources.drop("avoided", level='type')
+
+        data_scc_resources[indexes] = data_scc_resources[indexes] * scc
+        data_scc_capacities[indexes] = data_scc_capacities[indexes] * scc
+
+        showlegend = True
+
+    sum_resources = data_resources[indexes].sum(axis=0).reset_index(drop=True)
+    sum_capacities = data_capacities[indexes].sum(axis=0).reset_index(drop=True)
+    sum_scc_resources = data_scc_resources[indexes].sum(axis=0).reset_index(drop=True)
+    sum_scc_capacities = data_scc_capacities[indexes].sum(axis=0).reset_index(drop=True)
+    combined_resources = sum_resources + sum_scc_resources
+    combined_capacities = sum_capacities + sum_scc_capacities
 
     x1 = list(range(len(indexes)))
     x2 = [x + 1 / 3 for x in x1]
     xtick = [x + 1 / 6 for x in x1]
-    capex = data_capex[indexes].sum(axis=0).astype(int).reset_index(drop=True)
-    capex_text = ["<b>" + change_data.loc['x_axis_1', lang] + "</b><br>" + str(cp) + change_data.loc['unites', lang]
-                  for cp in capex]
-    opex = data_opex[indexes].sum(axis=0).astype(int).reset_index(drop=True)
-    pos_opex = data_opex[indexes][data_opex[indexes] > 0].sum(axis=0).astype(int).reset_index(drop=True)
-    opex_text = ["<b>" + change_data.loc['x_axis_2', lang] + "</b><br>" + str(op) + change_data.loc['unites', lang]
-                 for op in opex]
+
+    text_capacities = ["<b>" + change_data.loc['x_axis_1', lang] + "</b><br>" + str(custom_round(cp, decimal))
+                       for cp in combined_capacities]
+    text_resources = ["<b>" + change_data.loc['x_axis_2', lang] + "</b><br>" + str(custom_round(op, decimal))
+                      for op in combined_resources]
+    pos_resources = data_resources[indexes][data_resources[indexes] > 0].sum(axis=0).astype(int).reset_index(drop=True) + data_scc_resources[indexes][
+        data_scc_resources[indexes] > 0].sum(axis=0).astype(int).reset_index(drop=True)
 
     fig = go.Figure()
-    neg_opex = opex - pos_opex
-    text_placeholder = 0.04 * max(max(capex - neg_opex), max(capex + pos_opex), max(pos_opex - neg_opex))
+    neg_resources = combined_resources - pos_resources
+    text_placeholder = 0.04 * max(max(combined_capacities - neg_resources + combined_resources),
+                                  max(combined_capacities + combined_resources + neg_resources),
+                                  max(combined_resources))
 
     if add_annotation:
         for i in range(len(indexes)):
             fig.add_annotation(x=x2[i], y=-text_placeholder,
-                               text=opex_text[i], font=dict(size=10),
+                               text=text_resources[i], font=dict(size=10),
                                textangle=0, align='center', valign='top',
                                showarrow=False)
             fig.add_annotation(x=x1[i], y=-text_placeholder,
-                               text=capex_text[i], font=dict(size=9),
+                               text=text_capacities[i], font=dict(size=10),
                                textangle=0, align='center', valign='top',
                                showarrow=False
                                )
-            fig.add_annotation(x=xtick[i], y=max(capex[i], pos_opex[i], capex[i] + opex[i]) + text_placeholder,
-                               text="<b>" + change_data.loc['total', lang] + "</b><br>" + str(capex[i] + opex[i]) +
-                                    change_data.loc['unites', lang],
-                               font=dict(size=9, color=cm['darkblue']),
+            fig.add_annotation(x=xtick[i], y=max(combined_capacities[i], pos_resources[i],
+                                                 combined_capacities[i] + combined_resources[i]) + text_placeholder,
+                               text="<b>Total</b><br>" + str(custom_round(combined_capacities[i] + combined_resources[i], decimal)) + change_data.loc[
+                                   'unites', lang],
+                               font=dict(size=10, color=cm['darkblue']),
                                textangle=0, align='center', valign='top',
                                showarrow=False
                                )
-    for line, tech in data_capex.iterrows():
+    for line, tech in data_capacities.iterrows():
         if tech.loc[indexes].sum() > 0:
             fig.add_trace(
-                go.Bar(name=tech[label], x=x1,
-                       y=tech[indexes], width=1 / 3,
+                go.Bar(name=tech[label],
+                       x=x1,
+                       y=tech[indexes],
                        marker_color=tech["ColorPastel"],
-                       hovertemplate='<b>' + tech[label] + '</b>' +
-                                     '<br>' + change_data.loc['keyword', lang] + ': %{y:.0f}' +
-                                     change_data.loc['unites', lang],
-                       # text=unit_to_plot[label],
+                       width=1 / 3,
+                       hovertemplate=f'<b>{tech[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
                        legendgroup='group1',
                        legendgrouptitle_text=change_data.loc['x_axis_1', lang],
-                       showlegend=True))
-    for line, layer in data_opex.iterrows():
+                       showlegend=True)
+            )
+        if data_scc_capacities.loc[line, indexes].sum() > 0:
+            fig.add_trace(
+                go.Bar(name='Impact - ' + data_scc_capacities.loc[line, label],
+                       x=x1,
+                       y=data_scc_capacities.loc[line, indexes],
+                       marker_color=tech["ColorPastel"],
+                       marker_pattern_shape="x",
+                       width=1 / 3,
+                       hovertemplate=f'<b>{tech[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
+                       legendgroup='group1',
+                       showlegend=False)
+            )
+    for line, layer in data_resources.iterrows():
         if abs(layer.loc[indexes].sum()) > 0:
             fig.add_trace(
                 go.Bar(name=layer[label],
                        x=x2,
                        y=layer[indexes],
-                       marker=dict(color=layer["ColorPastel"]),
+                       marker_color=layer["ColorPastel"],
+                       width=1 / 3,
+                       hovertemplate=f'<b>{layer[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
                        legendgroup='group2',
                        legendgrouptitle_text=change_data.loc['x_axis_2', lang],
-                       # text=data_opex[label],
-                       showlegend=True,
+                       showlegend=True)
+            )
+        if abs(data_scc_resources.loc[line, indexes].sum()) > 0:
+            fig.add_trace(
+                go.Bar(name='Impact - ' + data_scc_resources.loc[line, label],
+                       x=x2,
+                       y=data_scc_resources.loc[line, indexes],
+                       marker_color=layer["ColorPastel"],
+                       marker_pattern_shape="x",
                        width=1 / 3,
-                       hovertemplate='<b>' + layer[label] + '</b>' +
-                                     '<br>' + change_data.loc['keyword', lang] + ': %{y:.0f}' + change_data.loc[
-                                         'unites', lang])
+                       hovertemplate=f'<b>{layer[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
+                       legendgroup='group2',
+                       showlegend=False)
             )
+
     fig.add_trace(
         go.Bar(
             name=change_data.loc['total', lang],
-            x=xtick, y=capex + opex,
-            width=1 / 6, showlegend=False,
-            hovertemplate="<b>" + change_data.loc['total', lang] + "</b><br>%{y:.0f}" + change_data.loc['unites', lang],
-            marker=dict(color=cm['lightblue'], opacity=1)
-        )
+            x=xtick,
+            y=sum_capacities + sum_resources,
+            marker_color=cm['lightblue'],
+            width=1 / 6,
+            hovertemplate=f'<b>Total</b><br>%{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
+            legendgroup='group3',
+            legendgrouptitle_text='Total',
+            showlegend=showlegend)
+    )
+
+    fig.add_trace(
+        go.Bar(
+            name=change_data.loc['scc_legend', lang],
+            x=xtick,
+            y=sum_scc_capacities + sum_scc_resources,
+            marker_color=cm['lightblue'],
+            marker_pattern_shape="x",
+            width=1 / 6,
+            hovertemplate=f'<b>Total</b><br>%{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
+            legendgroup='group3',
+            legendgrouptitle_text='Total',
+            showlegend=showlegend)
     )
+
     fig.update_layout(barmode="relative",
                       bargap=0,
                       template='plotly_white',
                       margin=dict(l=50, r=50, t=50, b=50),
                       xaxis=dict(
                           tickmode='array',
                           tickvals=xtick,
                           ticktext=indexes),
                       yaxis=dict(title=change_data.loc['y_axis', lang])
                       )
+
     if filename is not None:
         if not os.path.isdir(os.path.dirname(filename)):
             os.makedirs(os.path.dirname(filename))
-        if 'html' == export_format:
+        if export_format == 'html':
             fig.write_html(filename + '.' + export_format)
-        if 'png' == export_format:
-            fig.write_image(filename + '.' + export_format)
-        if 'pdf' == export_format:
+        if export_format == 'png' or export_format == 'pdf':
             fig.write_image(filename + '.' + export_format)
 
     if return_df:
-        return fig, pd.concat([data_capex, data_opex])
+        return fig, pd.concat([data_capacities, data_resources])
     else:
         return fig
 
 
-def plot_actors(results, plot='costs', indexed_on='Scn_ID', label='EN_long', premium_version=False, per_m2=False, additional_costs={},
-                filename=None, export_format='html', scaling_factor=1, return_df=False):
+def plot_expenses(results, plot='costs', indexed_on='Scn_ID', label='EN_long', premium_version=None, per_m2=False, additional_costs={}, additional_gwp={},
+                  scc=0.177,
+                  filename=None, export_format='html', scaling_factor=1, return_df=False):
+    """
+    Plots expenses based on REHO results.
+
+    Parameters
+    ----------
+    results: dict
+        Dictionary of REHO results.
+    plot: str
+        Choose among those three possibilities:
+
+        - 'costs' for the economic performance indicators,
+        - 'gwp' for the global warming potential indicators,
+        - 'combined' for a combination of the two indicators, where the emissions are converted into costs using the ``scc`` parameter.
+    indexed_on: str
+        Whether the results should be grouped on *Scn_ID* or *Pareto_ID*.
+    label: str
+        Indicates the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
+    premium_version : list
+        If enabled, it should be an array containing the retail price and feed-in price of electricity.
+    per_m2: bool
+        Set to True to obtain the results divided by the total ERA.
+    additional_costs: dict
+        Additional costs to include (choose between 'isolation', 'mobility', and 'ict') and scaling values.
+    additional_gwp: dict
+        Additional gwp to include (choose between 'isolation', 'mobility', and 'ict') and scaling values.
+    scc: float
+        Carbon externalities, expressed in *CHF/kgCO2*. Default value is the *Social Cost of Carbon*, from `Rennert, 2022 <https://www.nature.com/articles/s41586-022-05224-9>`_.
+    filename: str
+        Name of the file to be saved.
+    export_format: str
+        Can be either 'html', 'png', or 'pdf'.
+    scaling_factor: int/float
+        Scales linearly the REHO results for the plot.
+    return_df: bool
+        A dataframe can be returned for further post-processing or reporting purposes.
+
+    Returns
+    ----------
+    plotly.graph_objs.Figure
+        The generated plotly figure.
+    pd.DataFrame
+        (Optional) A dataframe for further post-processing or reporting purposes.
+    """
+
     sc = list(results.keys())[0]
     id = list(results[sc].keys())[0]
     era = results[sc][id]['df_Buildings'].ERA
 
-    df_eco = dict_to_df(results, 'df_Economics')
+    df_Economics = dict_to_df(results, 'df_Economics')
 
     change_data = pd.DataFrame()
-    change_data.index = ['col_1', 'col_2', 'x_axis_1', 'x_axis_2', 'y_axis', 'keyword', 'total', 'unites', 'leg_1',
-                         'leg_2']
+    change_data.index = ['x_axis_1', 'x_axis_2', 'y_axis', 'keyword', 'total', 'unites', 'leg_1', 'leg_2', 'scc_legend']
+    decimal = 0
     lang = re.split('_', label)[0]
+
     if plot == 'costs':
-        change_data['FR'] = ['Costs_Unit_inv', 'price', 'Coûts', 'Revenus', '[CHF/an]', 'Coûts', 'TOTEX', 'CHF', 'OPEX',
-                             'CAPEX']
-        change_data['EN'] = ['Costs_Unit_inv', 'price', 'Costs', 'Income', '[CHF/m2/y]', 'Costs', 'TOTEX', 'CHF',
-                             'OPEX', 'CAPEX']
-        df_eco = df_eco.xs('costs', level='Perf_type')
+        change_data['FR'] = ['Coûts', 'Revenus', '[CHF/an]', 'Coûts', 'Total', ' CHF', 'Capacités', 'Ressources', '']
+        change_data['EN'] = ['Costs', 'Revenues', '[CHF/y]', 'Costs', 'Total', ' CHF', 'Capacities', 'Resources', '']
+        df_costs = df_Economics.xs('costs', level='Perf_type')
+        if per_m2:
+            df_costs = df_costs / era.sum()
+            change_data.loc['y_axis']['FR'] = "Coûts [CHF/m2/an]"
+            change_data.loc['y_axis']['EN'] = "Costs [CHF/m2/y]"
+            decimal = 1
+        indexes, data_capacities, data_resources = prepare_dfs(df_costs, indexed_on, neg=False,
+                                                               premium_version=premium_version, additional_data=additional_costs, scaling_factor=scaling_factor)
+
+        data_scc_resources = pd.DataFrame(0, columns=[indexes], index=data_resources.index)
+        data_scc_capacities = pd.DataFrame(0, columns=[indexes], index=data_capacities.index)
+
     elif plot == 'gwp':
-        change_data['FR'] = ['GWP_Unit_constr', 'gwp', 'Emissions', 'Evitées', 'GWP [kgCO2/an]', 'Émissions', 'Total',
-                             'kgCO2', 'Réseau', 'Constr']
-        change_data['EN'] = ['GWP_Unit_constr', 'gwp', 'Emissions', 'Avoided', 'GWP [kgCO2/y]', 'Emissions', 'Total',
-                             'kgCO2', 'Grid', 'Constr']
-        df_eco = df_eco.xs('impact', level='Perf_type')
-
-    if per_m2:
-        df_eco = df_eco / era.sum()
-        change_data.loc['y_axis']['FR'] = "Coûts [CHF/m2/an]"
-        change_data.loc['y_axis']['EN'] = "Costs [CHF/m2/y]"
-
-    indexes, data_capex, data_opex = prepare_dfs(df_eco, indexed_on, neg=False, premium_version=premium_version, additional_costs=additional_costs,
-                                                 scaling_factor=scaling_factor)
-
-    costs = pd.concat([data_capex, data_opex.xs('costs', level='type')],
-                      keys=['investment', 'operation'], names=['Category'])
-    revenues = data_opex.loc[['avoided', 'revenues'], :]
+        change_data['FR'] = ['Émissions', 'Évitées', 'Émissions [kgCO2/an]', 'Émissions', 'Total', ' kgCO2', 'Capacités', 'Ressources', '']
+        change_data['EN'] = ['Emissions', 'Avoided', 'Emissions [kgCO2/y]', 'Emissions', 'Total', ' kgCO2', 'Capacities', 'Resources', '']
+        df_impact = df_Economics.xs('impact', level='Perf_type')
+        if per_m2:
+            df_impact = df_impact / era.sum()
+            change_data.loc['y_axis']['FR'] = "Émissions [kgCO2/m2/an]"
+            change_data.loc['y_axis']['EN'] = "Emissions [kgCO2/m2/y]"
+            decimal = 1
+        indexes, data_capacities, data_resources = prepare_dfs(df_impact, indexed_on, neg=False,
+                                                               premium_version=premium_version, additional_data=additional_gwp, scaling_factor=scaling_factor)
+
+        data_scc_resources = pd.DataFrame(0, columns=[indexes], index=data_resources.index)
+        data_scc_capacities = pd.DataFrame(0, columns=[indexes], index=data_capacities.index)
+
+    elif plot == 'combined':
+        change_data['FR'] = ['Coûts', 'Revenus', 'Coûts [CHF/an]', 'Coûts', 'Total', ' CHF', 'Capacités', 'Ressources', 'Impact carbone']
+        change_data['EN'] = ['Costs', 'Revenues', 'Costs [CHF/y]', 'Costs', 'Total', ' CHF', 'Capacities', 'Resources', 'Carbon impact']
+
+        df_costs = df_Economics.xs('costs', level='Perf_type')
+        df_impact = df_Economics.xs('impact', level='Perf_type')
+        if per_m2:
+            df_costs = df_costs / era.sum()
+            df_impact = df_impact / era.sum()
+            change_data.loc['y_axis']['FR'] = "Coûts [CHF/m2/an]"
+            change_data.loc['y_axis']['EN'] = "Costs [CHF/m2/y]"
+            decimal = 1
+        indexes, data_capacities, data_resources = prepare_dfs(df_costs, indexed_on, neg=False,
+                                                               additional_data=additional_costs,
+                                                               scaling_factor=scaling_factor)
+        indexes, data_scc_capacities, data_scc_resources = prepare_dfs(df_impact, indexed_on, neg=False,
+                                                                       additional_data=additional_gwp,
+                                                                       scaling_factor=scaling_factor)
+        data_scc_resources[indexes] = data_scc_resources[indexes] * scc
+        data_scc_capacities[indexes] = data_scc_capacities[indexes] * scc
+
+    costs = pd.concat([data_capacities, data_resources.xs('costs', level='type')], keys=['investment', 'operation'], names=['Category'])
+    revenues = data_resources.loc[['avoided', 'revenues'], :]
     costs = costs[costs[indexes].sum(axis=1) > 0]
     revenues = revenues[revenues[indexes].sum(axis=1) > 0]
     totex = costs[indexes].sum(axis=0) - revenues[indexes].sum(axis=0)
     revenues = revenues.reindex(columns=costs.columns.tolist())
 
+    costs_scc = pd.concat([data_scc_capacities, data_scc_resources.xs('costs', level='type')], keys=['investment', 'operation'], names=['Category'])
+    revenues_scc = data_scc_resources.loc[['avoided', 'revenues'], :]
+    totex_scc = costs_scc[indexes].sum(axis=0) - revenues_scc[indexes].sum(axis=0)
+    revenues_scc = revenues_scc.reindex(columns=costs_scc.columns.tolist())
+
+    sum_costs = costs[indexes].sum(axis=0).reset_index(drop=True)
+    sum_revenues = revenues[indexes].sum(axis=0).reset_index(drop=True)
+    sum_scc_costs = costs_scc[indexes].sum(axis=0).reset_index(drop=True)
+    sum_scc_revenues = revenues_scc[indexes].sum(axis=0).reset_index(drop=True)
+
     x1 = list(range(len(indexes)))
     x2 = [x + 1 / 3 for x in x1]
     xtick = [x + 1 / 6 for x in x1]
-    revenues_sum = revenues[indexes].sum(axis=0).astype(int).reset_index(drop=True)
-    costs_sum = costs[indexes].sum(axis=0).astype(int).reset_index(drop=True)
-    revenues_text = ["<b>" + change_data.loc['x_axis_2', lang] + "</b><br>" + str(cp) + change_data.loc['unites', lang]
-                     for cp in revenues_sum]
-    costs_text = ["<b>" + change_data.loc['x_axis_1', lang] + "</b><br>" + str(op) + change_data.loc['unites', lang]
-                  for op in costs_sum]
-    totex_text = ["<b>" + change_data.loc['total', lang] + "</b><br>" + str(tot) + change_data.loc['unites', lang]
-                  for tot in totex.astype(int)]
+    combined_costs = sum_costs + sum_scc_costs
+    combined_revenues = sum_revenues + sum_scc_revenues
+    combined_totex = totex.values + totex_scc.values
+    text_revenues = ["<b>" + change_data.loc['x_axis_2', lang] + "</b><br>" + str(custom_round(cp, decimal)) + change_data.loc['unites', lang]
+                     for cp in combined_revenues]
+    text_costs = ["<b>" + change_data.loc['x_axis_1', lang] + "</b><br>" + str(custom_round(op, decimal)) + change_data.loc['unites', lang]
+                  for op in combined_costs]
+    text_totex = ["<b>" + change_data.loc['total', lang] + "</b><br>" + str(custom_round(tot, decimal)) + change_data.loc['unites', lang]
+                  for tot in combined_totex]
 
     fig = go.Figure()
     for i in range(len(indexes)):
-        fig.add_annotation(x=x2[i], y=-0.04 * max(max(revenues_sum), max(costs_sum)),
-                           text=revenues_text[i], font=dict(size=10),
+        fig.add_annotation(x=x2[i], y=-0.04 * max(max(combined_revenues), max(combined_costs)),
+                           text=text_revenues[i], font=dict(size=10),
                            textangle=0, align='center', valign='top',
                            showarrow=False)
-        fig.add_annotation(x=x1[i], y=-0.04 * max(max(revenues_sum), max(costs_sum)),
-                           text=costs_text[i], font=dict(size=9),
+        fig.add_annotation(x=x1[i], y=-0.04 * max(max(combined_revenues), max(combined_costs)),
+                           text=text_costs[i], font=dict(size=10),
                            textangle=0, align='center', valign='top',
                            showarrow=False
                            )
-        fig.add_annotation(x=xtick[i], y=costs_sum[i] + 0.04 * max(max(revenues_sum), max(costs_sum)),
-                           text=totex_text[i],
-                           font=dict(size=9, color=cm['darkblue']),
+        fig.add_annotation(x=xtick[i], y=combined_costs[i] + 0.04 * max(max(combined_revenues), max(combined_costs)),
+                           text=text_totex[i],
+                           font=dict(size=10, color=cm['darkblue']),
                            textangle=0, align='center', valign='top',
                            showarrow=False
                            )
 
-    fig.add_trace(
-        go.Bar(name=change_data.loc['total', lang], x=x2,
-               y=totex,
-               legendgroup='group3',
-               legendgrouptitle_text=change_data.loc['total', lang],
-               marker=dict(color=cm['darkblue'], opacity=0),
-               showlegend=False,
-               # texttemplate=totex_text,
-               hovertemplate=None,
-               # textposition='inside',
-               # textfont=dict(size=9, color=cm['darkblue']),
-               width=1 / 6
-               )
-    )
+    df_scc = costs_scc.xs('investment', level='Category')
     for line, tech in costs.xs('investment', level='Category').iterrows():
         if tech.loc[indexes].sum() > 0:
             fig.add_trace(
-                go.Bar(name=tech[label], x=x1,
-                       y=tech[indexes], width=1 / 3,
+                go.Bar(name=tech[label],
+                       x=x1,
+                       y=tech[indexes],
+                       marker_color=tech["ColorPastel"],
+                       width=1 / 3,
+                       hovertemplate=f'<b>{tech[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
+                       legendgroup='group1',
+                       legendgrouptitle_text=change_data.loc['leg_1', lang],
+                       showlegend=True)
+            )
+        if line in df_scc.index and df_scc.loc[line, indexes].sum() > 0:
+            fig.add_trace(
+                go.Bar(name='Impact - ' + df_scc.loc[line, label],
+                       x=x1,
+                       y=df_scc.loc[line, indexes],
                        marker_color=tech["ColorPastel"],
-                       hovertemplate='<b>' + tech[label] + '</b>' +
-                                     '<br>' + change_data.loc['keyword', lang] + ': %{y:.1f}' +
-                                     change_data.loc['unites', lang],
+                       marker_pattern_shape="x",
+                       width=1 / 3,
+                       hovertemplate=f'<b>{tech[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
                        legendgroup='group1',
-                       legendgrouptitle_text=change_data.loc['leg_2', lang],
-                       showlegend=True))
-    for line, tech in costs.xs('operation', level='Category').iterrows():
+                       showlegend=False)
+            )
+    df_scc = costs_scc.xs('operation', level='Category')
+    for line, layer in costs.xs('operation', level='Category').iterrows():
         fig.add_trace(
-            go.Bar(name=tech[label], x=x1,
-                   y=tech[indexes], width=1 / 3,
-                   marker_color=tech["ColorPastel"],
-                   hovertemplate='<b>' + tech[label] + '</b>' +
-                                 '<br>' + change_data.loc['keyword', lang] + ': %{y:.1f}' +
-                                 change_data.loc['unites', lang],
+            go.Bar(name=layer[label],
+                   x=x1,
+                   y=layer[indexes],
+                   marker_color=layer["ColorPastel"],
+                   width=1 / 3,
+                   hovertemplate=f'<b>{layer[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
                    legendgroup='group2',
-                   legendgrouptitle_text=change_data.loc['leg_1', lang],
-                   showlegend=True))
+                   legendgrouptitle_text=change_data.loc['leg_2', lang],
+                   showlegend=True)
+        )
+        if line in df_scc.index and df_scc.loc[line, indexes].sum() > 0:
+            fig.add_trace(
+                go.Bar(name='Impact - ' + df_scc.loc[line, label],
+                       x=x1,
+                       y=df_scc.loc[line, indexes],
+                       marker_color=layer["ColorPastel"],
+                       marker_pattern_shape="x",
+                       width=1 / 3,
+                       hovertemplate=f'<b>{layer[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
+                       legendgroup='group1',
+                       showlegend=False)
+            )
+
+    fig.add_trace(
+        go.Bar(name=change_data.loc['total', lang],
+               x=x2,
+               y=combined_totex,
+               opacity=0,
+               width=1 / 6,
+               showlegend=False)
+    )
+
+    df_scc = revenues_scc
     for line, layer in revenues.iterrows():
         fig.add_trace(
             go.Bar(name=layer[label],
                    x=x2,
                    y=layer[indexes],
                    marker=dict(color=layer["ColorPastel"]),
+                   width=1 / 3,
+                   hovertemplate=f'<b>{layer[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
                    legendgroup='group2',
                    legendgrouptitle_text=change_data.loc['x_axis_2', lang],
-                   showlegend=True,
-                   width=1 / 3,
-                   hovertemplate='<b>' + layer[label] + '</b>' +
-                                 '<br>' + change_data.loc['keyword', lang] + ': %{y:.1f}' + change_data.loc[
-                                     'unites', lang])
+                   showlegend=True)
         )
-    # fig.add_trace(
-    #     go.Bar(
-    #         name=change_data.loc['total', lang],
-    #         x=xtick, y=totex,
-    #         width=1 / 6, showlegend=False,
-    #         hovertemplate=totex_text,
-    #         marker=dict(color=cm['darkblue'], opacity=0.7)
-    #     )
-    # )
+        if line in df_scc.index and df_scc.loc[line, indexes].sum() > 0:
+            fig.add_trace(
+                go.Bar(name='Impact - ' + df_scc.loc[line, label],
+                       x=x2,
+                       y=df_scc.loc[line, indexes],
+                       marker_color=layer["ColorPastel"],
+                       marker_pattern_shape="x",
+                       width=1 / 3,
+                       hovertemplate=f'<b>{layer[label]}</b><br>{change_data.loc["keyword", lang]}: %{{y:.{decimal}f}}{change_data.loc["unites", lang]}',
+                       legendgroup='group1',
+                       showlegend=False)
+            )
 
     fig.update_layout(barmode="relative",
                       bargap=0,
                       template='plotly_white',
                       margin=dict(l=50, r=50, t=50, b=50),
                       xaxis=dict(
                           tickmode='array',
                           tickvals=xtick,
                           ticktext=indexes),
                       yaxis=dict(title=change_data.loc['y_axis', lang])
                       )
+
     if filename is not None:
         if not os.path.isdir(os.path.dirname(filename)):
             os.makedirs(os.path.dirname(filename))
-        if 'html' == export_format:
+        if export_format == 'html':
             fig.write_html(filename + '.' + export_format)
-        if 'png' == export_format:
+        if export_format == 'png' or export_format == 'pdf':
             fig.write_image(filename + '.' + export_format)
 
     if return_df:
         return fig, pd.concat([costs, revenues])
     else:
         return fig
 
 
-def plot_sankey(df_Results, label='EN_long', color='ColorPastel', scaling_factor=1, return_df=False):
+def plot_sankey(df_Results, label='EN_long', color='ColorPastel', filename=None, export_format='html', scaling_factor=1, return_df=False):
     """
-    Generate a Sankey plot based on the results DataFrame.
+    Plots a Sankey plot based on the results DataFrame.
 
-    :param df_Results: DataFrame containing results for the Sankey plot.
-    :type df_Results: pandas.DataFrame
-    :param label: Indicates the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
-    :type label: str
-    :param color: Color scheme for the Sankey plot. Default is 'ColorPastel'.
-    :type color: str
-    :param scaling_factor: Scaling factor for the plot to adapt the results by a linear assumption. Default is 1.
-    :type scaling_factor: int or float
-    :param return_df: If True, return a dataframe for further post-processing or reporting purposes. Default is False.
-    :type return_df: bool
-
-    :return: If return_df is False, returns the Sankey plot. If True, returns a tuple containing the plot and a dataframe.
-    :rtype: plotly.graph_objects.Figure or tuple
+    Parameters
+    ----------
+    df_Results: pd.DataFrame
+        DataFrame coming from REHO results (already extracted from the desired *Scn_ID* or *Pareto_ID*).
+    label: str
+        Indicate the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
+    color: str
+        Indicate the color set to use for the plot. Choose among 'ColorPastel', 'ColorFlash'.
+    filename: str
+        Name of the file to be saved.
+    export_format: str
+        Can be either 'html', 'png', or 'pdf'.
+    scaling_factor: int/float
+        Scales linearly the REHO results for the plot.
+    return_df: bool
+        A dataframe can be returned for further post-processing or reporting purposes.
+
+    Returns
+    ----------
+    plotly.graph_objs.Figure
+        The generated plotly figure.
+    pd.DataFrame
+        (Optional) A dataframe for further post-processing or reporting purposes.
+    
     """
     source, target, value, label_, color_ = sankey.df_sankey(df_Results, label=label, color=color, precision=2,
                                                              units='MWh', display_label_value=True,
                                                              scaling_factor=scaling_factor)
 
     fig = go.Figure(data=[go.Sankey(
         orientation="h",
@@ -485,28 +608,615 @@
         ),
         link=dict(
             source=source,
             target=target,
             value=value
         ))])
 
+    if filename is not None:
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'html':
+            fig.write_html(filename + '.' + export_format)
+        if export_format == 'png' or export_format == 'pdf':
+            fig.write_image(filename + '.' + export_format)
+
     if return_df:
         df = pd.DataFrame()
         df["source"] = [label_[int(s)].split("\n")[0] for s in source]
         df["target"] = [label_[int(t)].split("\n")[0] for t in target]
         df["Energy [MWh/yr]"] = value
         return fig, df
     else:
         return fig
 
 
+def plot_profiles(df_Results, units_to_plot, style='plotly', label='EN_long', color='ColorPastel', resolution='weekly', plot_curtailment=False,
+                  filename=None, export_format='html', return_df=False):
+    """
+    Plots an hourly profile for an entire year of operation.
+
+    Parameters
+    ----------
+    df_Results: pd.DataFrame
+        DataFrame coming from REHO results (already extracted from the desired *Scn_ID* or *Pareto_ID*).
+    units_to_plot: list
+        Units to be plotted.
+    style: str
+        Choose between 'plotly' or 'matplotlib'.
+    label: str
+        Indicate the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
+    color: str
+        Indicate the color set to use for the plot. Choose among 'ColorPastel', 'ColorFlash'.
+    resolution: str
+        Moving average possible, choose between 'monthly', 'weekly', and 'daily'.
+    plot_curtailment: bool
+        PV curtailment can optionally be plotted.
+    filename: str
+        Name of the file to be saved.
+    export_format: str
+        Can be either 'html', 'png', or 'pdf'.
+    return_df: bool
+        A dataframe can be returned for further post-processing or reporting purposes.
+
+    Returns
+    ----------
+    plotly.graph_objs.Figure
+        The generated plotly figure.
+    pd.DataFrame
+        (Optional) A dataframe for further post-processing or reporting purposes.
+
+    """
+    if resolution == 'monthly':
+        items_average = 730
+    elif resolution == 'weekly':
+        items_average = 168
+    elif resolution == 'daily':
+        items_average = 24
+    else:
+        items_average = 1
+
+    units_demand = []
+    units_supply = []
+    for unit in units_to_plot:
+        if unit == "PV":
+            units_supply.append(unit)
+        elif unit in ["Battery", "EV_district"]:
+            units_demand.append(unit)
+            units_supply.append(unit)
+        else:
+            units_demand.append(unit)
+
+    # Grids
+    import_elec = df_Results['df_Grid_t'].xs(('Electricity', 'Network'), level=('Layer', 'Hub')).Grid_supply[:-2]
+    export_elec = df_Results['df_Grid_t'].xs(('Electricity', 'Network'), level=('Layer', 'Hub')).Grid_demand[:-2]
+    ng = df_Results['df_Grid_t'].xs(('NaturalGas', 'Network'), level=('Layer', 'Hub')).Grid_supply[:-2]
+
+    import_profile = np.array([])
+    export_profile = np.array([])
+    ng_profile = np.array([])
+    for i in range(1, 366):
+        id = df_Results['df_Index'].PeriodOfYear[i * 24]
+        import_profile = np.concatenate((import_profile, import_elec.xs(id)))
+        export_profile = np.concatenate((export_profile, export_elec.xs(id)))
+        ng_profile = np.concatenate((ng_profile, ng.xs(id)))
+
+    import_profile = moving_average(import_profile, items_average)
+    export_profile = moving_average(export_profile, items_average)
+    ng_profile = moving_average(ng_profile, items_average)
+
+    # Units
+    demands = dict()
+    supplies = dict()
+    curtailments = dict()
+    for unit in units_to_plot:
+        df_aggregated = df_Results['df_Unit_t'][df_Results['df_Unit_t'].index.get_level_values('Unit').str.contains(unit)]
+        if unit in units_demand:
+            demand = df_aggregated.droplevel('Layer').Units_demand[:-2].groupby(['Period', 'Time']).sum()
+            demands[unit] = np.array([])
+            for i in range(1, 366):
+                t = df_Results['df_Index'].PeriodOfYear[i * 24]
+                demands[unit] = np.concatenate((demands[unit], demand.xs(t)))
+        if unit in units_supply:
+            supply = df_aggregated.droplevel('Layer').Units_supply[:-2].groupby(['Period', 'Time']).sum()
+            supplies[unit] = np.array([])
+            for i in range(1, 366):
+                t = df_Results['df_Index'].PeriodOfYear[i * 24]
+                supplies[unit] = np.concatenate((supplies[unit], supply.xs(t)))
+        if unit == 'PV' and plot_curtailment:
+            curtailment = df_aggregated.droplevel('Layer').Units_curtailment[:-2].groupby(['Period', 'Time']).sum()
+            curtailments[unit] = np.array([])
+            for i in range(1, 366):
+                t = df_Results['df_Index'].PeriodOfYear[i * 24]
+                curtailments[unit] = np.concatenate((curtailments[unit], curtailment.xs(t)))
+
+    for unit in units_demand:
+        demands[unit] = moving_average(demands[unit], items_average)
+    for unit in units_supply:
+        supplies[unit] = moving_average(supplies[unit], items_average)
+    if plot_curtailment:
+        curtailments['PV'] = moving_average(curtailments['PV'], items_average)
+
+    idx = list(range(1, len(import_profile) + 1))
+
+    title = 'Energy profiles with a ' + resolution + ' moving average'
+    obj_x = 'Time [hours]'
+    obj_y = '[kWh]'
+
+    if style == 'matplotlib':
+        fig, ax = plt.subplots()
+        ax.plot(idx, import_profile, color=layout.loc['Electrical_grid', color],
+                label=layout.loc['Electrical_grid', label])
+        ax.plot(idx, -export_profile, color=layout.loc['Electrical_grid_feed_in', color],
+                label=layout.loc['Electrical_grid_feed_in', label])
+        ax.plot(idx, ng_profile, color=layout.loc['NaturalGas', color], label=layout.loc['NaturalGas', label],
+                alpha=0.5)
+        for unit in units_demand:
+            ax.plot(idx, demands[unit], linestyle='--', label=layout.loc[unit, label], color=layout.loc[unit, color])
+        for unit in units_supply:
+            ax.plot(idx, -supplies[unit], label=layout.loc[unit, label], color=layout.loc[unit, color])
+        if plot_curtailment:
+            ax.plot(idx, -curtailments['PV'], linestyle='.', label=layout.loc['Curtailment', label],
+                    color=layout.loc['Curtailment', color])
+
+        ax.set_title(title)
+        ax.set_xlabel(obj_x)
+        ax.set_ylabel(obj_y)
+        ax.legend(loc='best')
+
+        if filename is not None:
+            if not os.path.isdir(os.path.dirname(filename)):
+                os.makedirs(os.path.dirname(filename))
+            if export_format == 'png' or export_format == 'pdf':
+                plt.tight_layout()
+                plt.savefig((filename + '.' + export_format), format=export_format, dpi=300)
+
+        return plt
+
+    else:
+        fig = go.Figure()
+
+        fig.add_trace(go.Scatter(
+            x=idx,
+            y=import_profile,
+            mode="lines",
+            name=layout.loc['Electrical_grid', label],
+            line=dict(color=layout.loc['Electrical_grid', color])
+        ))
+
+        if export_profile.any() > 0:
+            fig.add_trace(go.Scatter(
+                x=idx,
+                y=-export_profile,
+                mode="lines",
+                name=layout.loc['Electrical_grid_feed_in', label],
+                line=dict(color=layout.loc['Electrical_grid_feed_in', color], dash='dash')
+            ))
+
+        if ng_profile.any() > 0:
+            fig.add_trace(go.Scatter(
+                x=idx,
+                y=ng_profile,
+                mode="lines",
+                name=layout.loc['NaturalGas', label],
+                line=dict(color=layout.loc['NaturalGas', color])
+            ))
+
+        for unit in units_demand:
+            if demands[unit].any() > 0:
+                fig.add_trace(go.Scatter(
+                    x=idx,
+                    y=demands[unit],
+                    mode="lines",
+                    name=layout.loc[unit, label],
+                    line=dict(color=layout.loc[unit, color])
+                ))
+        for unit in units_supply:
+            if supplies[unit].any() > 0:
+                fig.add_trace(go.Scatter(
+                    x=idx,
+                    y=-supplies[unit],
+                    mode="lines",
+                    name=layout.loc[unit, label],
+                    line=dict(color=layout.loc[unit, color], dash='dash')
+                ))
+        if plot_curtailment:
+            fig.add_trace(go.Scatter(
+                x=idx,
+                y=-curtailments['PV'],
+                mode="lines",
+                name=layout.loc['Curtailment', label],
+                line=dict(color=layout.loc['Curtailment', color], dash='dot')
+            ))
+
+        fig.update_layout(
+            title_text=title,
+            xaxis_title=obj_x,
+            yaxis_title=obj_y,
+            font=dict(
+                size=16,
+            )
+        )
+
+        if filename is not None:
+            if not os.path.isdir(os.path.dirname(filename)):
+                os.makedirs(os.path.dirname(filename))
+            if export_format == 'html':
+                fig.write_html(filename + '.' + export_format)
+            if export_format == 'png' or export_format == 'pdf':
+                fig.write_image(filename + '.' + export_format)
+
+        if return_df:
+            return fig, pd.DataFrame()
+        else:
+            return fig
+
+
+def plot_resources(results, label='EN_long', color='ColorPastel', filename=None, export_format='html'):
+    """
+    Under construction.
+    """
+    
+    scenarios = list(results.keys())
+    df_annuals = dict_to_df(results, 'df_Annuals')
+    pareto_id = list(results[scenarios[0]].keys())[0]
+    df_annuals = df_annuals.loc[(slice(None), pareto_id, slice(None), 'Network')]
+    idx = df_annuals.index.levels[1].tolist()
+    layers = ['NaturalGas', 'Oil', 'Electricity', 'Wood', 'Data']
+    df_resources = pd.DataFrame(0, index=['NaturalGas', 'Oil', 'Electrical_grid', 'Wood', ],
+                                columns=['scenario', 'Supply'])
+    df_resources = df_resources.merge(layout, left_index=True, right_on='Name')
+    df_resources = df_resources.rename({'Electrical_grid': 'Electricity'})
+    for scn in scenarios:
+        df_resources.loc[:, ['scenario', 'Supply']] = ([scn, df_annuals.loc[scn]['Supply_MWh']])
+    df_resources.fillna(0, inplace=True)
+    df_resources.reset_index(inplace=True)
+    fig = go.Figure()
+    for i, layer in enumerate(layers):
+        df_to_plot = df_resources[df_resources['Name'] == layer]
+        if ~df_to_plot.empty:
+            fig.add_trace(
+                go.Bar(x=df_to_plot['scenario'], y=df_to_plot['Supply'], name=df_to_plot.iloc[0][label],
+                       marker=dict(color=df_to_plot[color]),
+                       hovertemplate='<b>' + df_to_plot[label] + '</b>' +
+                                     '<br>%{y:.2f} MWh'
+                       )
+            )
+    fig.update_layout(
+        barmode="group",
+        template='plotly_white',
+        yaxis=dict(title="MWh"),
+    )
+
+    if filename is not None:
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'html':
+            fig.write_html(filename + '.' + export_format)
+        if export_format == 'png' or export_format == 'pdf':
+            fig.write_image(filename + '.' + export_format)
+
+    return fig
+
+
+def plot_sunburst_eud(results, label='EN_long', filename=None, export_format='html', scaling_factor=1, return_df=False):
+    """
+    Plots a Sunburst for End Use Demand (EUD) based on REHO results, grouped by buildings' class.
+
+    Parameters
+    ----------
+    results: dict
+        Dictionary of REHO results.
+    label: str
+        Indicate the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
+    filename: str
+        Name of the file to be saved.
+    export_format: str
+        Can be either 'html', 'png', or 'pdf'.
+    scaling_factor: int/float
+        Scales linearly the REHO results for the plot.
+    return_df: bool
+        A dataframe can be returned for further post-processing or reporting purposes.
+
+    Returns
+    ----------
+    plotly.graph_objs.Figure
+        The generated plotly figure.
+    pd.DataFrame
+        (Optional) A dataframe for further post-processing or reporting purposes.
+
+    """
+
+    def add_class(row):
+        ratio = [float(s) for s in str(row['ratio']).split("/")]
+        class_ = row['id_class'].split("/")
+        serie = pd.Series(ratio, index=class_).groupby(level=0).sum()
+        for key, value in correspondance_dict.items():
+            data_to_plot[value].update(data_to_plot[value] + serie * row[key])
+
+    correspondance_dict = {'ERA': 'area_per_class',
+                           'SH': 'sh_per_class',
+                           'DHW': 'dhw_per_class',
+                           'Electricity': 'elec_per_class'}
+    classes = ['I', 'II', 'III', 'IV', 'V', 'VI', 'VII', 'VIII', 'IX', 'X', 'XI', 'XII', 'XIII']
+    df_buildings = dict_to_df(results, 'df_Buildings')
+    df_annuals = dict_to_df(results, 'df_Annuals').reset_index().pivot(index=['Scn_ID', 'Pareto_ID', 'Hub'],
+                                                                       columns='Layer', values='Demand_MWh')
+    df_buildings = df_buildings.reset_index().merge(df_annuals, on=['Scn_ID', 'Pareto_ID', 'Hub']).set_index(
+        ['Scn_ID', 'Pareto_ID', 'Hub'])
+    data_to_plot = pd.DataFrame(0, index=classes, columns=['area_per_class', 'sh_per_class', 'dhw_per_class',
+                                                           'elec_per_class'])
+    class_names = pd.read_csv(os.path.join(path_to_plotting, 'sia380_1.csv'), index_col='id_class', sep=";")
+    data_to_plot = data_to_plot.merge(class_names, left_index=True, right_on='id_class')
+
+    if 'FR' in label.upper().split("_"):
+        hover_text = 'Demande en énergie'
+        liaison = ' du '
+    else:
+        hover_text = 'End Use Demand'
+        liaison = ' of '
+
+    scenarios = list(results.keys())
+    paretos = list(results[scenarios[0]].keys())
+
+    df_buildings.loc[(scenarios[0], paretos[0])].apply(add_class, axis=1)
+    child_name = []
+    parents_name = []
+    text_template = []
+    hover_template = []
+    values_sun = []
+    for i in range(len(classes)):
+        [child_name.append(element) for element in [data_to_plot.iloc[i]['class_' + label], "SH", "DHW", "Elec"]]
+        [parents_name.append(element) for element in
+         ["Total", data_to_plot.iloc[i]['class_' + label], data_to_plot.iloc[i]['class_' + label],
+          data_to_plot.iloc[i]['class_' + label]]]
+        [values_sun.append(element) for element in [
+            data_to_plot.iloc[i]['sh_per_class'] + data_to_plot.iloc[i]['dhw_per_class'] +
+            data_to_plot.iloc[i]['elec_per_class'],
+            data_to_plot.iloc[i]['sh_per_class'], data_to_plot.iloc[i]['dhw_per_class'],
+            data_to_plot.iloc[i]['elec_per_class']]]
+        [text_template.append(element) for element in ['%{label}<br>%{percentParent:.2%}',
+                                                       '%{label}<br>%{percentParent:.2%}',
+                                                       '%{label}<br>%{percentParent:.2%}',
+                                                       '%{label}<br>%{percentParent:.2%}']]
+        [hover_template.append(element) for element in
+         ['<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentParent:.2%}' + liaison + '%{parent}',
+          '<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentRoot:.2%}' + liaison + '%{root}',
+          '<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentRoot:.2%}' + liaison + '%{root}',
+          '<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentRoot:.2%}' + liaison + '%{root}']]
+
+    values_sun = [round(val * scaling_factor, 2) for val in values_sun]
+    fig = go.Figure(go.Sunburst(
+        labels=child_name,
+        parents=parents_name,
+        values=values_sun,
+        branchvalues='total',
+        name=hover_text,
+        hovertemplate=hover_template,
+        texttemplate=text_template,
+    ))
+
+    fig.update_layout(
+        sunburstcolorway=["#413D3A", "#CAC7C7", "#B51F1F", "#007480", "#00A79F", "#FEA993"],
+        extendsunburstcolors=True)
+
+    if filename is not None:
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'html':
+            fig.write_html(filename + '.' + export_format)
+        if export_format == 'png' or export_format == 'pdf':
+            fig.write_image(filename + '.' + export_format)
+
+    if return_df:
+        df = pd.DataFrame()
+        df["Energy Use"] = child_name
+        df["Building Type"] = parents_name
+        df["Energy Demand"] = values_sun
+        return fig, df
+
+    return fig
+
+
+def plot_unit_monthly(results, unit_to_plot, label='EN_short', filename=None, export_format='html'):
+    """
+    Generates a monthly bar plot showing the mean energy produced per hour and the installed power for a specific unit.
+
+    Parameters
+    ----------
+    results: dict
+        Dictionary of REHO results.
+    unit_to_plot: dict
+        Specify the unit to plot and Scn_ID / Pareto_ID from which it should be found.
+    label: str
+        Indicates the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
+    filename: str
+        Name of the file to be saved.
+    export_format: str
+        Can be either 'html', 'png', or 'pdf'.
+
+    Returns
+    ----------
+    plotly.graph_objs.Figure
+        The generated plotly figure.
+    pd.DataFrame
+        (Optional) A dataframe for further post-processing or reporting purposes.
+
+    Examples
+    --------
+    >>> reho_results = pd.read_pickle('results/progressive_scenario.pickle')
+    >>> unit_to_plot = {'Unit': 'NG_Boiler', 'Scn_ID': 'fossil', 'Pareto_ID': False}
+    >>> plot_unit_monthly(reho_results, unit_to_plot, label='FR_long', filename="my_plot", export_format='png').show()
+
+    """
+
+    def monthly_average_balance(results, unit_to_plot):
+        """
+        Return data to plot a monthly heat balance.
+
+        :return: pd.Series of House_Q_heating, -House_Q_cooling, House_Q_convection, HeatGains, SolarGains
+
+        """
+
+        df_Unit_t_t = remove_building_from_index(results['df_Unit_t'])
+        pos_units = df_Unit_t_t.index.get_level_values('Unit').unique()
+        pos_columns_bui = ['House_Q_heating', 'House_Q_cooling', 'House_Q_convection', 'HeatGains', 'SolarGains']
+
+        df_period_time = df_Unit_t_t.index.to_frame()[['Period', 'Time']].reset_index(drop=True)
+
+        df_type = ''
+        if unit_to_plot in pos_units:
+            df_type = 'unit'
+        elif unit_to_plot in pos_columns_bui:
+            df_type = 'building'
+
+        # For unit
+        if df_type == 'unit':
+            if unit_to_plot == 'PV':
+                column_to_plot = 'Units_supply'
+            else:
+                column_to_plot = 'Units_demand'
+            df_to_extract = df_Unit_t_t.xs(unit_to_plot, level='Unit').droplevel('Layer')[column_to_plot][:-2]
+
+        elif df_type == 'building':
+            # Extract the data
+            df_Weather = results['df_Weather']
+            df_buildings_th_feature = results['df_Buildings'][['U_h', 'ERA']]
+
+            if unit_to_plot == 'House_Q_convection':
+                df_to_extract = pd.DataFrame(0, index=df_period_time, columns=[unit_to_plot])
+                # For each building: calculation of the heat flux
+                # and addition of the flux of each building in df_heat_building_t
+                for b in list(df_buildings_th_feature.index):
+                    df_to_extract['House_Q_convection'] = df_buildings_th_feature.loc[b, 'U_h'] * \
+                                                          df_buildings_th_feature.loc[b, 'ERA'] * \
+                                                          (df_Weather.T_ext - df_Weather.T_in)
+                df_to_extract = df_to_extract[:-2]
+            else:
+                df_to_extract = results['df_Buildings_t'][unit_to_plot][:-2]
+        else:
+            # Case where the unit is not referenced in df_Unit_t such as for WaterTank
+            if 'df_Streams_t' in results.dict_config.keys():
+                df_Streams_t = remove_building_from_index(results['df_Streams_t'])
+                df_to_extract = df_Streams_t.xs(unit_to_plot, level='Unit')['Streams_Q'][:-2]
+            else:
+                idx = pd.MultiIndex.from_frame(df_period_time)
+                units_mult = remove_building_from_index(results['df_Unit']).reset_index().groupby('Unit').sum()[
+                    'Units_Mult']
+                df_to_extract = pd.Series(units_mult, index=idx)
+
+        month_values = monthly_average(results, df_to_extract)
+
+        return month_values
+
+    design = layout.loc[unit_to_plot['Unit']]
+
+    # Filter the right results dictionary from the REHO results dictionary
+    if 'Scn_ID' not in unit_to_plot.keys() or not unit_to_plot['Scn_ID']:
+        scn_id = list(results.keys())[0]
+        if 'Pareto_ID' not in unit_to_plot.keys() or not unit_to_plot['Pareto_ID']:
+            pareto_id = list(results[scn_id].keys())[0]
+        else:
+            pareto_id = unit_to_plot['Pareto_ID']
+    else:
+        scn_id = unit_to_plot['Scn_ID']
+        pareto_id = 0
+    unit_to_plot = unit_to_plot['Unit']
+    df_Results = results[scn_id][pareto_id]
+
+    month_values = monthly_average_balance(df_Results, unit_to_plot)
+    sized = remove_building_from_index(df_Results['df_Unit']).loc[unit_to_plot]['Units_Mult']
+
+    title_y = 'Energy [kWh/h]'
+    power = 'Power installed [kW]'
+    energy = 'Mean energy produced per hour [kWh/h]'
+    title = 'Power installed and energy produced for {}'.format(design.loc[label])
+
+    if 'FR' in label:
+        locale.setlocale(locale.LC_TIME, 'fr_FR.UTF-8')
+        title_y = 'Energie [kWh/h]'
+        power = 'Puissance installée [kW]'
+        energy = 'Energie moyenne produite par heure [kWh/h]'
+        title = 'Puissance installée et énergie produite pour {}'.format(design.loc[label])
+    if 'short' in label:
+        month_ticks = list(calendar.month_abbr)[1:]
+    else:
+        month_ticks = list(calendar.month_name)[1:]
+
+    # month_ticks = [month.encode('latin1').decode('utf-8') for month in month_ticks]
+
+    fig = go.Figure(
+        go.Bar(
+            name=energy,
+            x=list(range(1, 13)), y=month_values,
+            width=1, showlegend=False,
+            hovertemplate="<b>" + design.loc[label] + "</b><br>%{y:.0f} kWh/h",
+            marker=dict(color=design.loc['ColorPastel']),
+        ),
+        go.Layout(
+            template='plotly_white',
+            bargap=0,
+            xaxis=dict(
+                tickmode='array',
+                tickvals=list(range(1, 13)),
+                ticktext=month_ticks
+            ),
+            yaxis=dict(title=title_y),
+            title=title
+        )
+    )
+    if sized is not None:
+        max_y = sized
+        fig.add_trace(
+            go.Bar(
+                name=power,
+                x=[6.5], y=[max_y],
+                width=12, showlegend=False,
+                hovertemplate="<b>" + design.loc[label] + "</b><br>%{y:.0f} kW",
+                marker=dict(color=design.loc['ColorPastel'], opacity=0.3),
+            )
+        )
+        fig.update_layout(yaxis=dict(range=[0, max_y]))
+
+    if filename is not None:
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'html':
+            fig.write_html(filename + '.' + export_format)
+        if export_format == 'png' or export_format == 'pdf':
+            fig.write_image(filename + '.' + export_format)
+
+    return fig
+
+
 def plot_pareto(results, label='EN_long', color='ColorPastel', return_df=False):
+    """
+    Plots a Pareto front based on REHO results.
+
+    Parameters
+    ----------
+    results: dict
+        Dictionary of REHO results.
+    label: str
+        Indicates the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
+    color: str
+    Indicate the color set to use for the plot. Choose among 'ColorPastel', 'ColorFlash'.
+    return_df: bool
+        A dataframe can be returned for further post-processing or reporting purposes.
+
+    Returns
+    ----------
+    plotly.graph_objs.Figure
+        The generated plotly figure.
+    pd.DataFrame
+        (Optional) A dataframe for further post-processing or reporting purposes.
+    """
+
     df_performance = dict_to_df(results, 'df_Performance').loc[
-        (slice(None), slice(None), 'Network'),
-        ["Costs_op", "Costs_inv", "Costs_grid_connection", "Costs_rep", "GWP_op", "GWP_constr"]].reset_index(
+        (slice(None), slice(None), 'Network'), ["Costs_op", "Costs_inv", "Costs_grid_connection", "Costs_rep", "GWP_op", "GWP_constr"]].reset_index(
         ['Scn_ID', 'Hub'])
     era = dict_to_df(results, 'df_Buildings').loc[(slice(None), 1, slice(None))].ERA.sum()
     df_performance["CAPEX"] = df_performance["Costs_inv"] + df_performance["Costs_rep"]
     df_performance["OPEX"] = df_performance["Costs_op"] + df_performance["Costs_grid_connection"]
     df_performance["TOTEX"] = df_performance["CAPEX"] + df_performance["OPEX"]
     df_performance["GWP"] = df_performance["GWP_op"] + df_performance["GWP_constr"]
 
@@ -578,29 +1288,30 @@
         df = df_performance[['CAPEX', 'OPEX', 'TOTEX', 'GWP']].round(2)
         df["Scenario"] = np.arange(1, len(df) + 1)
         return fig, df[["Scenario", 'CAPEX', 'OPEX', 'TOTEX', 'GWP']]
     else:
         return fig
 
 
-def plot_pareto_old(results, name_list=None, objectives=["CAPEX", "OPEX"], style='plotly', annotation="TOTEX",
-                    annot_offset=0, legend=True, save_fig=False, name_fig='pareto', format_fig='png'):
+def plot_pareto_by_objectives(results, name_list=None, objectives=["CAPEX", "OPEX"], style='plotly', annotation="TOTEX", annot_offset=0, legend=True,
+                              filename=None, export_format='png'):
+    """
+    # TO DO
+    """
     df_performance_dict = {}
     # for results in results_list:
     df_performance = dict_to_df(results, 'df_Performance').loc[
         (slice(None), slice(None), 'Network'), ["Costs_op", "Costs_inv", "Costs_grid_connection", "Costs_rep",
                                                 "GWP_op", "GWP_constr"]].reset_index(['Scn_ID', 'Hub'])
     era = dict_to_df(results, 'df_Buildings').loc[(slice(None), 1, slice(None))].ERA.sum()
     df_performance["CAPEX"] = df_performance["Costs_inv"] + df_performance["Costs_rep"]
     df_performance["OPEX"] = df_performance["Costs_op"] + df_performance["Costs_grid_connection"]
     df_performance["TOTEX"] = df_performance["CAPEX"] + df_performance["OPEX"]
     df_performance["GWP"] = df_performance["GWP_op"] + df_performance["GWP_constr"]
-    df_performance_dict[df_performance.loc[1, "Scn_ID"]] = df_performance[
-                                                               ["CAPEX", "OPEX", "TOTEX", "GWP"]].sort_values(
-        by=objectives[0]) / era
+    df_performance_dict[df_performance.loc[1, "Scn_ID"]] = df_performance[["CAPEX", "OPEX", "TOTEX", "GWP"]].sort_values(by=objectives[0]) / era
 
     if name_list is None:
         name_list = list(df_performance_dict.keys())
 
     if objectives[0] == "CAPEX":
         obj_x = "CAPEX [CHF/m$^2$yr]"
     elif objectives[0] == "TOTEX":
@@ -629,17 +1340,20 @@
         plt.title(objectives[0] + "-" + objectives[1] + " Pareto")
         plt.xlabel(obj_x)
         plt.ylabel(obj_y)
 
         if legend:
             plt.legend(labels=name_list, loc='upper right', fancybox=True, shadow=True)
 
-        if save_fig:
-            plt.tight_layout()
-            plt.savefig((name_fig + '.' + format_fig), format=format_fig, dpi=300)
+        if filename is not None:
+            if not os.path.isdir(os.path.dirname(filename)):
+                os.makedirs(os.path.dirname(filename))
+            if export_format == 'png' or export_format == 'pdf':
+                plt.tight_layout()
+                plt.savefig((filename + '.' + export_format), format=export_format, dpi=300)
 
         return plt
 
     else:
 
         fig = go.Figure()
 
@@ -668,19 +1382,35 @@
             xaxis_title=obj_x,
             yaxis_title=obj_y,
             font=dict(
                 size=16,
             )
         )
 
+        if filename is not None:
+            if not os.path.isdir(os.path.dirname(filename)):
+                os.makedirs(os.path.dirname(filename))
+            if export_format == 'html':
+                fig.write_html(filename + '.' + export_format)
+            if export_format == 'png' or export_format == 'pdf':
+                fig.write_image(filename + '.' + export_format)
+
         return fig
 
 
-def plot_pareto_units(results, objectives=["CAPEX", "OPEX"], label='EN_long', color='ColorPastel',
-                      save_fig=False, name_fig='pareto_units', format_fig='png', opex_line=False, title=None):
+################################################################################################################################################################
+# Matplotlib
+################################################################################################################################################################
+
+
+def plot_pareto_units(results, objectives=["CAPEX", "OPEX"], label='EN_long', color='ColorPastel', opex_line=False, title=None, filename=None,
+                      export_format='png'):
+    """
+    TO DO
+    """
     fig, ax = plt.subplots()
     fig.set_size_inches(10, 5)
 
     if not isinstance(results, list):
         results = [results]
     nb_pareto = len(results)
 
@@ -776,15 +1506,15 @@
             ax.plot(idx, df_performance[grid_stack] / era, label="Resources", color=cm['salmon'],
                     linestyle=linestyle[id_res])
             ax.plot(idx, (df_performance[grid_stack] + df_performance.Costs_inv) / era, label="TOTEX", color="red",
                     linestyle=linestyle[id_res])
     ax.axhline(0, color='black', linewidth=0.8)
 
     ax.set_xticks(idx)
-    ax.set_xticklabels(round((df_performance.Costs_inv) / era, 1).values)
+    ax.set_xticklabels(round(df_performance.Costs_inv / era, 1).values)
 
     if title:
         plt.title(title)
     else:
         plt.title(objectives[0] + "-" + objectives[1] + " Pareto : " + str(scenario))
 
     if objectives[0] == "CAPEX":
@@ -811,38 +1541,27 @@
         circ = []
         for i in range(nb_pareto):
             circ = circ + [(mpatches.Patch(facecolor='white', edgecolor='black', hatch=hatch_pareto[i]),
                             Line2D([0], [0], color="black", linestyle=linestyle[i]))]
         ax1.legend(circ, label_pareto, loc='lower left', frameon=False, ncol=nb_pareto,
                    handler_map={tuple: HandlerTuple(ndivide=None)}, handlelength=5)
 
-    if save_fig:
-        plt.tight_layout()
-        plt.savefig((name_fig + '_' + scenario + '.' + format_fig), format=format_fig, dpi=300)
+    if filename is not None:
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'png' or export_format == 'pdf':
+            plt.tight_layout()
+            plt.savefig((filename + '.' + export_format), format=export_format, dpi=300)
 
     return plt
 
 
-def merge_handles_labels(ax):
-    handles = []
-    labels = []
-    for axis in ax:
-        handle, label = axis.get_legend_handles_labels()
-        handles = handles + handle
-        labels = labels + label
-
-    handles.reverse()
-    labels.reverse()
-    by_label = dict(zip(labels, handles))
-    return by_label
-
-
-def plot_gwp_KPIs(results, save_fig=False, name='GWP', format='png'):
+def plot_gwp_KPIs(results, filename=None, export_format='png'):
     """
-        Plot the GWP_Op, GWP_Constr and GWP_Tot
+    TO DO
     """
     scenario = list(results.keys())[0]
     ids = list(results[scenario].keys())
 
     dict_df_perf = {}
     GWP_OP_list = []
     GWP_CONSTR_list = []
@@ -861,22 +1580,28 @@
     df.plot('scenario', y=['GWP_Op', 'GWP_Constr', 'GWP_Tot'], marker='.', linestyle='--')
 
     plt.xlabel('Scenario')
     plt.ylabel('GWP')
     # plt.legend(loc='upper center', bbox_to_anchor=(0.5, -0.20),
     #          fancybox=True, shadow=True, ncol=3)
 
-    if save_fig:
-        plt.tight_layout()
-        plt.savefig((name + '.' + format), format=format, dpi=300)
+    if filename is not None:
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'png' or export_format == 'pdf':
+            plt.tight_layout()
+            plt.savefig((filename + '.' + export_format), format=export_format, dpi=300)
 
     return plt
 
 
 def plot_LCOE(results, KPI_list, era, idx=None):
+    """
+    TO DO
+    """
     fig, ax = plt.subplots(2, figsize=(5.5, 7))
     ax2 = ax[0].twinx()
 
     for id_res, res in enumerate(results):
         style = ["-", "--", ":"][id_res]
         if idx is None:
             idx = np.array([res[0][i]["df_Performance"].xs("Network")["Costs_inv"] for i in res[0]]) / era
@@ -886,23 +1611,20 @@
         EPFL_canard = '#007480'
         Salmon = '#FEA993'
         colors = {"SC": EPFL_light_grey, "PVP": EPFL_red, "LCoE1": Salmon, "SS": EPFL_canard,
                   "gwp_tot_m2": "black", "gwp_constr_m2": "black", "gwp_op_m2": "black",
                   "Import max": "black", "Export max": EPFL_red, "electricity import": EPFL_light_grey,
                   "electricity export": Salmon, "natural gas import": "black"}
 
-        data_annual = {}
-        # data_annual["Import max"] = [res[0][i]["df_Grid_t"].xs(("Electricity", "Network"), level=(0, 1))["Grid_supply"][0:-2].max() for i in res[0]]
-        # data_annual["Export max"] = [res[0][i]["df_Grid_t"].xs(("Electricity", "Network"), level=(0, 1))["Grid_demand"][0:-2].max() for i in res[0]]
-        data_annual["electricity import"] = [
-            res[0][i]["df_Annuals"].xs(("Electricity", "Network"), level=(0, 1))["Supply_MWh"][0] for i in res[0]]
-        data_annual["electricity export"] = [
-            res[0][i]["df_Annuals"].xs(("Electricity", "Network"), level=(0, 1))["Demand_MWh"][0] for i in res[0]]
-        data_annual["natural gas import"] = [
-            res[0][i]["df_Annuals"].xs(("NaturalGas", "Network"), level=(0, 1))["Supply_MWh"][0] for i in res[0]]
+        data_annual = {"Import max": [res[0][i]["df_Grid_t"].xs(("Electricity", "Network"), level=(0, 1))["Grid_supply"][0:-2].max() for i in res[0]],
+                       "Export max": [res[0][i]["df_Grid_t"].xs(("Electricity", "Network"), level=(0, 1))["Grid_demand"][0:-2].max() for i in res[0]],
+                       "electricity import": [res[0][i]["df_Annuals"].xs(("Electricity", "Network"), level=(0, 1))["Supply_MWh"][0] for i in res[0]],
+                       "electricity export": [res[0][i]["df_Annuals"].xs(("Electricity", "Network"), level=(0, 1))["Demand_MWh"][0] for i in res[0]],
+                       "natural gas import": [res[0][i]["df_Annuals"].xs(("NaturalGas", "Network"), level=(0, 1))["Supply_MWh"][0] for i in res[0]]
+                       }
 
         for kpi in KPI_list:
             kpi_res = [res[0][i]["df_KPI"].xs("Network")[kpi] for i in res[0]]
             ax[0].plot(idx, kpi_res, marker='.', linestyle=style, color=colors[kpi], label=kpi)
         ax[0].set_ylabel('performance [kWh/kWh]', color="black")
         lcoe = np.array([res[0][i]["df_KPI"].xs("Network")["LCoE1"] for i in res[0]]) * 100
         ax2.plot(idx, lcoe, marker='.', linestyle=style, color=colors["LCoE1"], label="LCoE1")
@@ -929,224 +1651,29 @@
                title='system design')
     axx.set_axis_off()
     plt.tight_layout()
 
     return plt
 
 
-def plot_unit_size(results, units_to_plot):
-    scenario = list(results.keys())[0]
-    ids = list(results[scenario].keys())
-
-    unit_dict = dict()
-    for unit in units_to_plot:
-        unit_dict[unit] = dict()
-        for id in ids:
-            idx = [unit in string for string in results[scenario][id]['df_Unit'].index]
-            unit_dict[unit][id] = results[scenario][id]['df_Unit'][idx]['Units_Mult'].sum()
-        unit_dict[unit] = pd.DataFrame.from_dict(unit_dict[unit], orient='index')
-
-    fig, ax = plt.subplots()
-    for key in unit_dict:
-        ax.plot(ids, unit_dict[key].to_numpy(), marker='.', linestyle='-')
-
-    plt.xlabel('Scenario [-]')
-    plt.ylabel('Unit size [ref size]')
-
-    return plt
-
-
-def plot_profiles(df, units_to_plot, style='plotly', label='EN_long', color='ColorPastel', resolution='weekly',
-                  save_fig=False, name='plot_profiles', format='png', plot_curtailment=False, return_df=False):
-    if resolution == 'monthly':
-        items_average = 730
-    elif resolution == 'weekly':
-        items_average = 168
-    elif resolution == 'daily':
-        items_average = 24
-    else:
-        items_average = 1
-
-    units_demand = []
-    units_supply = []
-    for unit in units_to_plot:
-        if unit == "PV":
-            units_supply.append(unit)
-        elif unit in ["Battery", "EV_district"]:
-            units_demand.append(unit)
-            units_supply.append(unit)
-        else:
-            units_demand.append(unit)
-
-    # Grids
-    import_elec = df['df_Grid_t'].xs(('Electricity', 'Network'), level=('Layer', 'Hub')).Grid_supply[:-2]
-    export_elec = df['df_Grid_t'].xs(('Electricity', 'Network'), level=('Layer', 'Hub')).Grid_demand[:-2]
-    ng = df['df_Grid_t'].xs(('NaturalGas', 'Network'), level=('Layer', 'Hub')).Grid_supply[:-2]
-
-    import_profile = np.array([])
-    export_profile = np.array([])
-    ng_profile = np.array([])
-    for i in range(1, 366):
-        id = df['df_Index'].PeriodOfYear[i * 24]
-        import_profile = np.concatenate((import_profile, import_elec.xs(id)))
-        export_profile = np.concatenate((export_profile, export_elec.xs(id)))
-        ng_profile = np.concatenate((ng_profile, ng.xs(id)))
-
-    import_profile = moving_average(import_profile, items_average)
-    export_profile = moving_average(export_profile, items_average)
-    ng_profile = moving_average(ng_profile, items_average)
-
-    # Units
-    demands = dict()
-    supplies = dict()
-    curtailments = dict()
-    for unit in units_to_plot:
-        df_aggregated = df['df_Unit_t'][df['df_Unit_t'].index.get_level_values('Unit').str.contains(unit)]
-        if unit in units_demand:
-            demand = df_aggregated.droplevel('Layer').Units_demand[:-2].groupby(['Period', 'Time']).sum()
-            demands[unit] = np.array([])
-            for i in range(1, 366):
-                t = df['df_Index'].PeriodOfYear[i * 24]
-                demands[unit] = np.concatenate((demands[unit], demand.xs(t)))
-        if unit in units_supply:
-            supply = df_aggregated.droplevel('Layer').Units_supply[:-2].groupby(['Period', 'Time']).sum()
-            supplies[unit] = np.array([])
-            for i in range(1, 366):
-                t = df['df_Index'].PeriodOfYear[i * 24]
-                supplies[unit] = np.concatenate((supplies[unit], supply.xs(t)))
-        if unit == 'PV' and plot_curtailment:
-            curtailment = df_aggregated.droplevel('Layer').Units_curtailment[:-2].groupby(['Period', 'Time']).sum()
-            curtailments[unit] = np.array([])
-            for i in range(1, 366):
-                t = df['df_Index'].PeriodOfYear[i * 24]
-                curtailments[unit] = np.concatenate((curtailments[unit], curtailment.xs(t)))
-
-    for unit in units_demand:
-        demands[unit] = moving_average(demands[unit], items_average)
-    for unit in units_supply:
-        supplies[unit] = moving_average(supplies[unit], items_average)
-    if plot_curtailment:
-        curtailments['PV'] = moving_average(curtailments['PV'], items_average)
-
-    idx = list(range(1, len(list(demands.values())[0]) + 1))
-
-    title = 'Energy profiles with a ' + resolution + ' moving average'
-    obj_x = 'Time [hours]'
-    obj_y = '[kWh]'
-
-    if style == 'matplotlib':
-        fig, ax = plt.subplots()
-        ax.plot(idx, import_profile, color=layout.loc['Electrical_grid', color],
-                label=layout.loc['Electrical_grid', label])
-        ax.plot(idx, -export_profile, color=layout.loc['Electrical_grid_feed_in', color],
-                label=layout.loc['Electrical_grid_feed_in', label])
-        ax.plot(idx, ng_profile, color=layout.loc['NaturalGas', color], label=layout.loc['NaturalGas', label],
-                alpha=0.5)
-        for unit in units_demand:
-            ax.plot(idx, demands[unit], linestyle='--', label=layout.loc[unit, label], color=layout.loc[unit, color])
-        for unit in units_supply:
-            ax.plot(idx, -supplies[unit], label=layout.loc[unit, label], color=layout.loc[unit, color])
-        if plot_curtailment:
-            ax.plot(idx, -curtailments['PV'], linestyle='.', label=layout.loc['Curtailment', label],
-                    color=layout.loc['Curtailment', color])
-
-        ax.set_title(title)
-        ax.set_xlabel(obj_x)
-        ax.set_ylabel(obj_y)
-        ax.legend(loc='best')
-
-        if save_fig:
-            plt.tight_layout()
-            plt.savefig((name + '.' + format), format=format, dpi=300)
-
-        return plt
-
-    else:
-        fig = go.Figure()
-
-        fig.add_trace(go.Scatter(
-            x=idx,
-            y=import_profile,
-            mode="lines",
-            name=layout.loc['Electrical_grid', label],
-            line=dict(color=layout.loc['Electrical_grid', color])
-        ))
-
-        if export_profile.any() > 0:
-            fig.add_trace(go.Scatter(
-                x=idx,
-                y=-export_profile,
-                mode="lines",
-                name=layout.loc['Electrical_grid_feed_in', label],
-                line=dict(color=layout.loc['Electrical_grid_feed_in', color], dash='dash')
-            ))
-
-        if ng_profile.any() > 0:
-            fig.add_trace(go.Scatter(
-                x=idx,
-                y=ng_profile,
-                mode="lines",
-                name=layout.loc['NaturalGas', label],
-                line=dict(color=layout.loc['NaturalGas', color])
-            ))
-
-        for unit in units_demand:
-            if demands[unit].any() > 0:
-                fig.add_trace(go.Scatter(
-                    x=idx,
-                    y=demands[unit],
-                    mode="lines",
-                    name=layout.loc[unit, label],
-                    line=dict(color=layout.loc[unit, color])
-                ))
-        for unit in units_supply:
-            if supplies[unit].any() > 0:
-                fig.add_trace(go.Scatter(
-                    x=idx,
-                    y=-supplies[unit],
-                    mode="lines",
-                    name=layout.loc[unit, label],
-                    line=dict(color=layout.loc[unit, color], dash='dash')
-                ))
-        if plot_curtailment:
-            fig.add_trace(go.Scatter(
-                x=idx,
-                y=-curtailments['PV'],
-                mode="lines",
-                name=layout.loc['Curtailment', label],
-                line=dict(color=layout.loc['Curtailment', color], dash='dot')
-            ))
-
-        fig.update_layout(
-            title_text=title,
-            xaxis_title=obj_x,
-            yaxis_title=obj_y,
-            font=dict(
-                size=16,
-            )
-        )
-
-        if return_df:
-            return fig, pd.DataFrame()
-        else:
-            return fig
-
-
-def plot_composite_curve(results, cluster, plot=True, periods=["Yearly"]):
+def plot_composite_curve(results, cluster, periods=["Yearly"], filename=None, export_format='png'):
+    """
+    TO DO
+    """
     # process results data
     df_heat = results["df_Buildings_t"][["House_Q_heating", "House_Q_cooling", "Th_supply"]]
     df_heat_T = pd.DataFrame(np.round(df_heat['Th_supply'], 1).values, columns=["temperature"])
     df_heat_T.index = df_heat.index
     df_heat = pd.concat([df_heat, df_heat_T], axis=1)
     df_heat = df_heat.set_index("temperature", append=True)
     df_heat = df_heat.drop(columns="Th_supply")
     df_heat = df_heat.groupby(["Period", "temperature"], level=[1, 3]).sum()
 
     # get index typical periods
-    file_ID = WD.get_cluster_file_ID(cluster)
+    file_ID = weather.get_cluster_file_ID(cluster)
     file_name = "index_" + file_ID + ".dat"
     thisfile = os.path.join(path_to_clustering, file_name)
     df = np.loadtxt(thisfile, skiprows=1, max_rows=8760)
     df = pd.DataFrame(df).set_index(0)
 
     # calculate monthly heat load profile, raw data
     t = [1, 744, 672, 744, 720, 744, 720, 744, 744, 720, 744, 720, 744]
@@ -1169,278 +1696,31 @@
         profile = monthly_profile[i].assign(sum=monthly_profile[i].House_Q_heating.values.cumsum())
         profile.columns = ["Heat", "Cooling", "Heat_stacked"]
         profile = profile.assign(sum=profile.Cooling.values.cumsum())
         profile.columns = ["Heat", "Cooling", "Heat_stacked", "Cooling_stacked"]
         data_month = profile.Heat_stacked / duration[i] / 1000
         data[month[i]] = data_month
 
-    # create Figures folder
-    try:
-        os.makedirs('Figures')
-    except:
-        pass
-
-    if plot:
-        for i in periods:
-            fig, ax = plt.subplots(figsize=(9, 6))
-            ax.plot(data[i] , data[i].index, color="indianred", label="Space heating")
-            plt.ylabel("Temperature [°C]", fontsize=18)
-            plt.xlabel("Heat [MW]", fontsize=18)
-            plt.title("Composite curve for the city of Sierre: " + i, fontsize=20)
-            plt.legend(fontsize=16)
-            plt.xticks(fontsize=16)
-            plt.yticks(fontsize=16)
-            plt.savefig("Figures//" + i + ".png")
-            plt.show()
-    data = data.fillna(0)
-    return data
-
-
-
-
-def plot_resources(results, label='EN_long', color='ColorPastel',
-                   save_path="", filename=None, export_format='html'):
-    scenarios = list(results.keys())
-    df_annuals = dict_to_df(results, 'df_Annuals')
-    pareto_id = list(results[scenarios[0]].keys())[0]
-    df_annuals = df_annuals.loc[(slice(None), pareto_id, slice(None), 'Network')]
-    idx = df_annuals.index.levels[1].tolist()
-    layers = ['NaturalGas', 'Oil', 'Electricity', 'Wood', 'Data']
-    df_resources = pd.DataFrame(0, index=['NaturalGas', 'Oil', 'Electrical_grid', 'Wood', ],
-                                columns=['scenario', 'Supply'])
-    df_resources = df_resources.merge(layout, left_index=True, right_on='Name')
-    df_resources = df_resources.rename({'Electrical_grid': 'Electricity'})
-    for scn in scenarios:
-        df_resources.loc[:, ['scenario', 'Supply']] = [scn, df_annuals.loc[scn]['Supply_MWh']]
-    df_resources.fillna(0, inplace=True)
-    df_resources.reset_index(inplace=True)
-    fig = go.Figure()
-    for i, layer in enumerate(layers):
-        df_to_plot = df_resources[df_resources['Name'] == layer]
-        if ~df_to_plot.empty:
-            fig.add_trace(
-                go.Bar(x=df_to_plot['scenario'], y=df_to_plot['Supply'], name=df_to_plot.iloc[0][label],
-                       marker=dict(color=df_to_plot[color]),
-                       hovertemplate='<b>' + df_to_plot[label] + '</b>' +
-                                     '<br>%{y:.2f} MWh'
-                       )
-            )
-    fig.update_layout(
-        barmode="group",
-        template='plotly_white',
-        yaxis=dict(title="MWh"),
-    )
-
-    if filename is not None:
-        filename = os.path.join(save_path, str(filename + '.' + export_format))
-        if export_format == 'html':
-            fig.to_html(filename)
-        elif export_format == 'png':
-            fig.to_image(filename)
-
-    return fig
-
-
-def sunburst_eud(results, label='EN_long', save_path="", filename=None, export_format='html', scaling_factor=1,
-                 return_df=False):
-    """
-    Generate a Sunburst plot for End Use Demand (EUD) based on REHO results, by buildings' class.
-
-    :param results: Dictionary of REHO results.
-    :type results: dict
-    :param label: Indicates the language to use for the plot. Choose among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
-    :type label: str
-    :param save_path: Path to save the plot file. Default is an empty string.
-    :type save_path: str
-    :param filename: Name of the file to be saved. Default is None.
-    :type filename: str or None
-    :param export_format: Format for exporting the plot. Can be 'html' or 'png'. Default is 'html'.
-    :type export_format: str
-    :param scaling_factor: Scaling factor for the plot to adapt the results by a linear assumption. Default is 1.
-    :type scaling_factor: int or float
-    :param return_df: If True, return a dataframe for further post-processing or reporting purposes. Default is False.
-    :type return_df: bool
-
-    :return: If return_df is False, returns the Sunburst plot. If True, returns a tuple containing the plot and a dataframe.
-    :rtype: plotly.graph_objects.Figure or tuple
-    """
-
-    def add_class(row):
-        ratio = [float(s) for s in str(row['ratio']).split("/")]
-        class_ = row['id_class'].split("/")
-        serie = pd.Series(ratio, index=class_).groupby(level=0).sum()
-        for key, value in correspondance_dict.items():
-            data_to_plot[value].update(data_to_plot[value] + serie * row[key])
-
-    correspondance_dict = {'ERA': 'area_per_class',
-                           'SH': 'sh_per_class',
-                           'DHW': 'dhw_per_class',
-                           'Electricity': 'elec_per_class'}
-    classes = ['I', 'II', 'III', 'IV', 'V', 'VI', 'VII', 'VIII', 'IX', 'X', 'XI', 'XII', 'XIII']
-    df_buildings = dict_to_df(results, 'df_Buildings')
-    df_annuals = dict_to_df(results, 'df_Annuals').reset_index().pivot(index=['Scn_ID', 'Pareto_ID', 'Hub'],
-                                                                       columns='Layer', values='Demand_MWh')
-    df_buildings = df_buildings.reset_index().merge(df_annuals, on=['Scn_ID', 'Pareto_ID', 'Hub']).set_index(
-        ['Scn_ID', 'Pareto_ID', 'Hub'])
-    data_to_plot = pd.DataFrame(0, index=classes, columns=['area_per_class', 'sh_per_class', 'dhw_per_class',
-                                                           'elec_per_class'])
-    class_names = pd.read_csv(os.path.join(path_to_plotting, 'sia380_1.csv'), index_col='id_class', sep=";")
-    data_to_plot = data_to_plot.merge(class_names, left_index=True, right_on='id_class')
-
-    if 'FR' in label.upper().split("_"):
-        hover_text = 'Demande en énergie'
-        liaison = ' du '
-    else:
-        hover_text = 'End Use Demand'
-        liaison = ' of '
-
-    scenarios = list(results.keys())
-    paretos = list(results[scenarios[0]].keys())
-
-    df_buildings.loc[(scenarios[0], paretos[0])].apply(add_class, axis=1)
-    child_name = []
-    parents_name = []
-    text_template = []
-    hover_template = []
-    values_sun = []
-    for i in range(len(classes)):
-        [child_name.append(element) for element in [data_to_plot.iloc[i]['class_' + label], "SH", "DHW", "Elec"]]
-        [parents_name.append(element) for element in
-         ["Total", data_to_plot.iloc[i]['class_' + label], data_to_plot.iloc[i]['class_' + label],
-          data_to_plot.iloc[i]['class_' + label]]]
-        [values_sun.append(element) for element in [
-            data_to_plot.iloc[i]['sh_per_class'] + data_to_plot.iloc[i]['dhw_per_class'] +
-            data_to_plot.iloc[i]['elec_per_class'],
-            data_to_plot.iloc[i]['sh_per_class'], data_to_plot.iloc[i]['dhw_per_class'],
-            data_to_plot.iloc[i]['elec_per_class']]]
-        [text_template.append(element) for element in ['%{label}<br>%{percentParent:.2%}',
-                                                       '%{label}<br>%{percentParent:.2%}',
-                                                       '%{label}<br>%{percentParent:.2%}',
-                                                       '%{label}<br>%{percentParent:.2%}']]
-        [hover_template.append(element) for element in
-         ['<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentParent:.2%}' + liaison + '%{parent}',
-          '<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentRoot:.2%}' + liaison + '%{root}',
-          '<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentRoot:.2%}' + liaison + '%{root}',
-          '<i>%{label}</i><br><b>' + hover_text + ': </b>%{value} MWh<br>%{percentRoot:.2%}' + liaison + '%{root}']]
-
-    values_sun = [round(val * scaling_factor, 2) for val in values_sun]
-    fig = go.Figure(go.Sunburst(
-        labels=child_name,
-        parents=parents_name,
-        values=values_sun,
-        branchvalues='total',
-        name=hover_text,
-        hovertemplate=hover_template,
-        texttemplate=text_template,
-    ))
-
-    fig.update_layout(
-        sunburstcolorway=["#413D3A", "#CAC7C7", "#B51F1F", "#007480", "#00A79F", "#FEA993"],
-        extendsunburstcolors=True)
     if filename is not None:
-        filename = os.path.join(save_path, filename + '_sunburst.')
-        if export_format == 'png':
-            fig.write_image(filename + export_format)
-        elif export_format == 'html':
-            fig.write_html(filename + export_format)
-        return print("Sunburst printed at " + filename + export_format)
-
-    if return_df:
-        df = pd.DataFrame()
-        df["Energy Use"] = child_name
-        df["Building Type"] = parents_name
-        df["Energy Demand"] = values_sun
-        return fig, df
-    else:
-        return fig
-
-
-def temperature_profile(df_results):
-    """
-        return a df series of the Tin temperature profile
-        one column per building
-        TODO : check if multi-building is okay
-
-        Author : Florent
-
-        Parameters:
-            df_results (df): dataframe of a scenario
-
-        Returns:
-            df_Tin
-    """
-    # Extract the data
-    buildings_list = list(df_results['df_Buildings'].index)
-    df_buildings_t = df_results['df_Buildings_t']
-
-    # Prepare the df to store the Tin
-    df_Tin = pd.DataFrame()
-
-    # list of the two last periods used for design purpose to drop later
-    period_to_drop = list(df_buildings_t.xs('Building1').index.get_level_values('Period').unique()[-2:])
-
-    # For each building: calculation of the Tin series
-    for b in buildings_list:
-        # Take Tin for the building in df_buildings_t
-        df_Tin_building = pd.DataFrame()
-        df_Tin_building['T_in'] = df_buildings_t.xs(b)['T_in']
-
-        # drop the last two periods for design
-        for i in period_to_drop:
-            df_Tin_building = df_Tin_building.drop(i, level='Period')
-
-        # to averaging over days if wanted
-        items_average = 24  # daily
-        # array to work for a building
-        Tin_building = np.array([])
-
-        for j in range(1, 366):
-            id = df_results['df_Index'].PeriodOfYear[j * 24]
-            data_id = df_Tin_building.xs(id)
-            Tin_building = np.concatenate((Tin_building, data_id['T_in']))
-
-        # to averaging over days if wanted
-        # Tin_building = np.mean(Tin_building.reshape(-1, items_average), axis=1)
-
-        # Store the data in df_Tin (one col per building)
-        df_Tin['T_in_' + str(b)] = Tin_building
-
-    # create idx
-    idx = list(df_Tin.index + 1)
-    return df_Tin.to_numpy(), idx
-
-
-def plot_EUD_FES(results):
-    scenario = list(results.keys())[0]
-
-    df_annuals = results[scenario][0]['df_Annuals']
-
-    # service end use
-    df_EUD_FEC = pd.DataFrame(0,
-                              index=['Electricity_EUD', 'Electricity_FEC', 'SH_EUD', 'SH_FEC', 'DHW_EUD', 'DHW_FEC'],
-                              columns=['Electrical grid', 'Electrical appliances', 'Oil boiler (oil)',
-                                       'Oil boiler (heat)'])
-
-    # Oil per service
-    oil_for_oil_boiler = df_annuals.loc[('Oil', 'OIL_Boiler_Building1'), 'Demand_MWh']
-    DHW_from_oil_boiler = df_annuals.loc[('DHW', 'OIL_Boiler_Building1'), 'Supply_MWh']
-    SH_from_oil_boiler = df_annuals.loc[('SH', 'OIL_Boiler_Building1'), 'Supply_MWh']
-    ratio_SHonDHW_oil_boiler = SH_from_oil_boiler / (DHW_from_oil_boiler + SH_from_oil_boiler)
-
-    df_EUD_FEC.loc['Electricity_EUD', 'Electrical grid'] = df_annuals.loc[('Electricity', 'Network'), 'Supply_MWh']
-    df_EUD_FEC.loc['Electricity_FEC', 'Electrical appliances'] = df_annuals.loc[
-        ('Electricity', 'Building1'), 'Demand_MWh']
-    df_EUD_FEC.loc['SH_EUD', 'Oil boiler (heat)'] = df_annuals.loc[('SH', 'OIL_Boiler_Building1'), 'Supply_MWh']
-    df_EUD_FEC.loc['SH_FEC', 'Oil boiler (oil)'] = ratio_SHonDHW_oil_boiler * df_annuals.loc[
-        ('Oil', 'OIL_Boiler_Building1'), 'Demand_MWh']
-    df_EUD_FEC.loc['DHW_EUD', 'Oil boiler (heat)'] = df_annuals.loc[('DHW', 'OIL_Boiler_Building1'), 'Supply_MWh']
-    df_EUD_FEC.loc['DHW_FEC', 'Oil boiler (oil)'] = (1 - ratio_SHonDHW_oil_boiler) * df_annuals.loc[
-        ('Oil', 'OIL_Boiler_Building1'), 'Demand_MWh']
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'png' or export_format == 'pdf':
+            for i in periods:
+                fig, ax = plt.subplots(figsize=(9, 6))
+                ax.plot(data[i], data[i].index, color="indianred", label="Space heating")
+                plt.ylabel("Temperature [°C]", fontsize=18)
+                plt.xlabel("Heat [MW]", fontsize=18)
+                plt.title("Composite curve: " + i, fontsize=20)
+                plt.legend(fontsize=16)
+                plt.xticks(fontsize=16)
+                plt.yticks(fontsize=16)
+                plt.tight_layout()
+                plt.savefig((filename + i + '.' + export_format), format=export_format, dpi=300)
 
-    print(df_EUD_FEC)
+    return data.fillna(0)
 
 
 def plot_EVs(results, era, label='EN_long', color='ColorPastel'):
     fig, ax = plt.subplots(1, figsize=(5.5, 4.2))
     ax2 = ax.twinx()
     data = {}
     for id_res, res in enumerate(results):
@@ -1482,22 +1762,22 @@
         data["E_dem"] = E_dem / E_dem[0]
         data["E_sup"] = E_sup / E_sup[0]
         data["NG_sup"] = NG_sup / NG_sup[0]
         data["NG_sup"][2] = 1.12
 
         style = ["-", "--", ":"][id_res]
         idx = list(data["EVs"]["Units_Mult"] / data["EVs"]["Units_Mult"].max() * 100)
-        ax2.plot(idx, data["SC"], marker='.', linestyle=style, color=layout.loc['Electricity', color],
+        ax2.plot(idx, data["SC"], linestyle=style, color=layout.loc['Electricity', color],
                  label="Self-consumption")
-        ax.plot(idx, data["C_tot"], marker='.', linestyle=style, color="red", label=layout.loc['TOTEX', label])
-        ax.plot(idx, data["E_sup"], marker='.', linestyle=style, color=layout.loc['self_cons', color],
+        ax.plot(idx, data["C_tot"], linestyle=style, color="red", label=layout.loc['TOTEX', label])
+        ax.plot(idx, data["E_sup"], linestyle=style, color=layout.loc['PV_SC', color],
                 label="Electricity retail")
-        ax.plot(idx, data["NG_sup"], marker='.', linestyle=style, color=layout.loc['NaturalGas', color],
-                label="Gas retail")
-        ax.plot(idx, data["E_dem"], marker='.', linestyle=style, color=layout.loc['Heat', color],
+        # ax.plot(idx, data["NG_sup"], linestyle=style, color=layout.loc['NaturalGas', color],
+        #        label="Gas retail")
+        ax.plot(idx, data["E_dem"], linestyle=style, color=layout.loc['Heat', color],
                 label="Electricity feed-in")
 
     # legend system design
     ax.set_ylabel('relative variation [-]', color="black")
     ax.set_xlabel('share of electric mobility [%]', color="black")
     ax2.spines["right"].set_color(layout.loc['Electricity', color])
     ax2.tick_params(axis='y', colors=layout.loc['Electricity', color])
@@ -1513,15 +1793,18 @@
     #            ncol=2, title='system design')
     # axx.set_axis_off()
     plt.tight_layout()
 
     return plt
 
 
-def plot_load_duration_curve(results, ids, save_fig=False, label='EN_long', color='ColorPastel'):
+def plot_load_duration_curve(results, ids, color='ColorPastel', filename=None, export_format='pdf'):
+    """
+    TO DO
+    """
     fig, ax = plt.subplots(figsize=(9, 6))
     axx = ax.twinx()
     linstyles = ["-", ":"]
     idx = list(range(1, 8761))
     col = 0.2
     for res in results:
         for id in ids:
@@ -1553,223 +1836,15 @@
 
     custom_lines = [Line2D([0], [0], color='black', linewidth=1.5, ),
                     Line2D([0], [0], color='black', linewidth=1.5, linestyle=':')]
     axx.legend(custom_lines, ['centralized', 'decentralized'], bbox_to_anchor=(0.86, -0.12), frameon=False, ncol=2,
                title='design strategy', fontsize=18, title_fontsize=18)
     axx.set_axis_off()
 
-    if save_fig:
-        plt.tight_layout()
-        format = 'pdf'
-        plt.savefig(('figures\\load_duration_curves' + '.' + format), format=format, dpi=300)
-
-    return plt
-
-
-def monthly_average_balance(results, to_plot):
-    """
-        return data to plot a monthly heat balance of the df_results, from REHO
-        TODO : check if multi-building is okay
-
-        Author : Florent, Joseph
-
-        Parameters:
-            results (dict): dict from pickle of REHO
-
-        Returns:
-            df series of House_Q_heating, -House_Q_cooling, House_Q_convection, HeatGains, SolarGains
-    """
-
-    def monthly_average(results, df_to_extract):
-        np_to_extract = np.array([])
-        np_month = np.array([])
-        ranges = divide_hours_into_months()
-        for i in range(1, 366):
-            hour = i * 24
-            month = len(np_to_extract)
-            id_period = results['df_Index'].PeriodOfYear[hour]
-            data_id = df_to_extract.xs(id_period)
-            np_month = np.concatenate((np_month, data_id))
-            if ranges[month][1] == hour:
-                np_to_extract = np.append(np_to_extract, np.sum(np_month) / (ranges[month][1] - ranges[month][0]))
-                np_month = np.array([])
-
-        return np_to_extract
-
-    def divide_hours_into_months():
-        num_months = 12
-
-        month_ranges = []
-        start_hour = 1
-        for month in range(num_months):
-            days = calendar.monthrange(2023, month + 1)
-            end_hour = start_hour + days[1] * 24 - 1
-            month_ranges.append((start_hour, end_hour))
-            start_hour = end_hour + 1
-
-        return month_ranges
-
-    df_units_t = remove_building_from_index(results['df_Unit_t'])
-    pos_units = df_units_t.index.get_level_values('Unit').unique()
-    pos_columns_bui = ['House_Q_heating', 'House_Q_cooling', 'House_Q_convection', 'HeatGains', 'SolarGains']
-
-    # Df of time period
-    df_period_time = df_units_t.index.to_frame()[['Period', 'Time']].reset_index(drop=True)
-
-    df_type = ''
-    if to_plot in pos_units:
-        df_type = 'unit'
-    elif to_plot in pos_columns_bui:
-        df_type = 'building'
-
-    # For unit
-    if df_type == 'unit':
-        if to_plot == 'PV':
-            column_to_plot = 'Units_supply'
-        else:
-            column_to_plot = 'Units_demand'
-        df_to_extract = df_units_t.xs(to_plot, level='Unit').droplevel('Layer')[column_to_plot][:-2]
-
-    elif df_type == 'building':
-        # Extract the data
-        df_external = results['df_External']
-        df_buildings_th_feature = results['df_Buildings'][['U_h', 'ERA']]
-
-        if to_plot == 'House_Q_convection':
-            df_to_extract = pd.DataFrame(0, index=df_period_time, columns=[to_plot])
-            # For each building: calculation of the heat flux
-            # and addition of the flux of each building in df_heat_building_t
-            for b in list(df_buildings_th_feature.index):
-                df_to_extract['House_Q_convection'] = df_buildings_th_feature.loc[b, 'U_h'] * \
-                                                      df_buildings_th_feature.loc[b, 'ERA'] * \
-                                                      (df_external.T_ext - df_external.T_in)
-            df_to_extract = df_to_extract[:-2]
-        else:
-            df_to_extract = results['df_Buildings_t'][to_plot][:-2]
-    else:
-        # Case where the unit is not referenced in df_Unit_t such as for WaterTank
-        if 'df_Stream_t' in results.dict_config.keys():
-            df_stream = remove_building_from_index(results['df_Stream_t'])
-            df_to_extract = df_stream.xs(to_plot, level='Unit')['Streams_Q'][:-2]
-        else:
-            idx = pd.MultiIndex.from_frame(df_period_time)
-            units_mult = remove_building_from_index(results['df_Unit']).reset_index().groupby('Unit').sum()['Units_Mult']
-            df_to_extract = pd.Series(units_mult, index=idx)
-    month_values = monthly_average(results, df_to_extract)
-
-    return month_values
-
-
-def unit_monthly_plot(results, to_plot, label='EN_short', save_path="", filename=None, export_format='html'):
-    """
-    Generate a monthly bar plot showing the mean energy produced per hour
-    and the installed power for a specific unit.
-
-    :param results: Dictionary containing REHO results.
-    :type results: dict
-
-    :param to_plot: Dictionary specifying the unit to plot and scenario/pareto id from which it should be found.
-    :type to_plot: dict
-
-    :param label: Indicates the language to use for the plot. Pick among 'FR_long', 'FR_short', 'EN_long', 'EN_short'.
-    :type label: str
-
-    :param save_path: Path where the plot should be saved.
-    :type save_path: str
-
-    :param filename: Name of the file to be saved.
-    :type filename: str
-
-    :param export_format: Format for exporting the plot ('html' or 'png', default: 'html').
-    :type export_format: str
-
-    :return: The generated plotly.graph_objs.Figure.
-
-    :example:
-
-     In a fossil scenario, plot the use of gas boiler throughout the year::
-
-        from reho.plotting.plotting import unit_monthly_plot
-
-        reho_results = pd.read_pickle('results/progressive_scenario.pickle')
-        to_plot = {'Unit': 'NG_Boiler', 'Scn_ID': 'fossil', 'Pareto_ID': False}
-        fig = unit_monthly_plot(reho_results, to_plot, label='FR_long',
-                                save_path="plots", filename="", export_format='png')
-        fig.show()
-
-    """
-    design = layout.loc[to_plot['Unit']]
-    # Filter the right results dictionary from the REHO results dictionary
-    if 'Scn_ID' not in to_plot.keys() or not to_plot['Scn_ID']:
-        scn_id = list(results.keys())[0]
-        if 'Pareto_ID' not in to_plot.keys() or not to_plot['Pareto_ID']:
-            pareto_id = list(results[scn_id].keys())[0]
-        else:
-            pareto_id = to_plot['Pareto_ID']
-    else:
-        scn_id = to_plot['Scn_ID']
-        pareto_id = 0
-    to_plot = to_plot['Unit']
-    df_results = results[scn_id][pareto_id]
-
-    month_values = monthly_average_balance(df_results, to_plot)
-    sized = remove_building_from_index(df_results['df_Unit']).loc[to_plot]['Units_Mult']
-
-    title_y = 'Energy [kWh/h]'
-    power = 'Power installed [kW]'
-    energy = 'Mean energy produced per hour [kWh/h]'
-    title = 'Power installed and energy produced for {}'.format(design.loc[label])
-
-    if 'FR' in label:
-        locale.setlocale(locale.LC_TIME, 'fr_FR.UTF-8')
-        title_y = 'Energie [kWh/h]'
-        power = 'Puissance installée [kW]'
-        energy = 'Energie moyenne produite par heure [kWh/h]'
-        title = 'Puissance installée et énergie produite pour {}'.format(design.loc[label])
-    if 'short' in label:
-        month_ticks = list(calendar.month_abbr)[1:]
-    else:
-        month_ticks = list(calendar.month_name)[1:]
-
-    # month_ticks = [month.encode('latin1').decode('utf-8') for month in month_ticks]
-
-    fig = go.Figure(
-        go.Bar(
-            name=energy,
-            x=list(range(1, 13)), y=month_values,
-            width=1, showlegend=False,
-            hovertemplate="<b>" + design.loc[label] + "</b><br>%{y:.0f} kWh/h",
-            marker=dict(color=design.loc['ColorPastel']),
-        ),
-        go.Layout(
-            template='plotly_white',
-            bargap=0,
-            xaxis=dict(
-                tickmode='array',
-                tickvals=list(range(1, 13)),
-                ticktext=month_ticks
-            ),
-            yaxis=dict(title=title_y),
-            title=title
-        )
-    )
-    if sized is not None:
-        max_y = sized
-        fig.add_trace(
-            go.Bar(
-                name=power,
-                x=[6.5], y=[max_y],
-                width=12, showlegend=False,
-                hovertemplate="<b>" + design.loc[label] + "</b><br>%{y:.0f} kW",
-                marker=dict(color=design.loc['ColorPastel'], opacity=0.3),
-            )
-        )
-        fig.update_layout(yaxis=dict(range=[0, max_y]))
-
     if filename is not None:
-        filename = os.path.join(save_path, filename + '_monthly_' + to_plot + '.')
-        if export_format == 'png':
-            fig.write_image(filename + export_format)
-        elif export_format == 'html':
-            fig.write_html(filename + export_format)
+        if not os.path.isdir(os.path.dirname(filename)):
+            os.makedirs(os.path.dirname(filename))
+        if export_format == 'png' or export_format == 'pdf':
+            plt.tight_layout()
+            plt.savefig((filename + '.' + export_format), format=export_format, dpi=300)
 
-    return fig
+    return plt
```

### Comparing `REHO-1.0.2/reho/plotting/rainbow_plots.py` & `reho-1.1.0/reho/plotting/rainbow_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,95 +1,98 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.interpolate import interp1d
 import math
 import scipy as sp
 
+__doc__ = """
+Reconstructs data from a Pareto optimization to produce a rainbow plot.
+"""
 
-def linerize_equal_steps (x, y):
+
+def linerize_equal_steps(x, y):
     x.name = 'x'
     y.name = 'y'
     step = (x.max() - x.min()) / len(x)
-    df = pd.concat([x, y], names =['x','y'], axis=1)
+    df = pd.concat([x, y], names=['x', 'y'], axis=1)
 
     df_new = pd.DataFrame(columns=['y'])
-    for s in  np.arange(1,  len(x)+1 ):
-        x_new = s*step
+    for s in np.arange(1, len(x) + 1):
+        x_new = s * step
         ub = df[df.x >= x_new].x.min()
         lb = df[df.x < x_new].x.max()
-        if math.isnan(ub) == True: # happens in case x_new == to last x in array
-            y_new = df[df.x == lb].iloc[0].y # just return last point
+        if math.isnan(ub):  # happens in case x_new == to last x in array
+            y_new = df[df.x == lb].iloc[0].y  # just return last point
         else:
             upper_bound = df[df.x == ub].iloc[0]
             lower_bound = df[df.x == lb].iloc[0]
 
             m = ((upper_bound.y - lower_bound.y) / (upper_bound.x - lower_bound.x))
-            b = lower_bound.y- m * lower_bound.x
+            b = lower_bound.y - m * lower_bound.x
 
-            y_new = m*x_new + b
+            y_new = m * x_new + b
         df_new.at[x_new, 'y'] = y_new
     return df_new
 
-def split_orientation(az):
 
-    if (az < 45) or  (az > 315):
+def split_orientation(az):
+    if (az < 45) or (az > 315):
         orientation = 'North'
-    elif  (az >= 45) and (az < 135):
+    elif (az >= 45) and (az < 135):
         orientation = 'East'
     elif (az >= 135) and (az < 225):
         orientation = 'South'
     elif (az >= 225) and (az <= 315):
         orientation = 'West'
     else:
         orientation = 'Other'
 
     return orientation
 
-def get_roof_max(df_nbr, hs_A):
 
+def get_roof_max(df_nbr, hs_A):
     df_n = df_nbr.groupby(['Pareto_ID', 'Surface', 'Azimuth', 'Tilt']).sum()
     roofs = df_n[df_n.index.get_level_values(level='Tilt') != 90]
 
-    #get total m2 PV
+    # get total m2 PV
     total_roofs = roofs.groupby('Pareto_ID').sum()
-    total_roofs['PV_m2'] = total_roofs.PVA_module_nbr*1.6
+    total_roofs['PV_m2'] = total_roofs.PVA_module_nbr * 1.6
     # get occupation based on azimuth orientation
-    roofs = roofs.reset_index(level = ['Azimuth'])
+    roofs = roofs.reset_index(level=['Azimuth'])
     roofs['Orientation'] = roofs.apply(lambda x: split_orientation(x['Azimuth']), axis=1)
     roofs = roofs.set_index('Orientation', append='True')
     roofs = roofs.groupby(['Pareto_ID', 'Orientation']).sum()
     max = roofs.PVA_module_nbr.groupby(level="Orientation").max()
     roofs['occupancy'] = roofs.PVA_module_nbr / max
 
     roofs_max = total_roofs.PV_m2.max()
-    roofs_max_m2 = roofs_max /hs_A
+    roofs_max_m2 = roofs_max / hs_A
 
     facades = df_n[df_n.index.get_level_values(level='Tilt') == 90]
     if not facades.empty:
         # get total m2 facades
         total_facades = facades.groupby('Pareto').sum()
-        total_facades['PV_m2'] = total_facades.PVA_module_nbr*1.6
+        total_facades['PV_m2'] = total_facades.PVA_module_nbr * 1.6
         # get occupation based on azimuth orientation
         facades = facades.reset_index(level=['Azimuth'])
         facades['Orientation'] = facades.apply(lambda x: split_orientation(x['Azimuth']), axis=1)
         facades = facades.set_index('Orientation', append='True')
         facades = facades.groupby(['Pareto', 'Orientation']).sum()
         max = facades.PVA_module_nbr.max(level=1)
         facades['occupancy'] = facades.PVA_module_nbr / max
         total_surface = total_facades['PV_m2'] + total_roofs['PV_m2']
     else:
         total_surface = total_roofs['PV_m2']
-    total_surface_m2 = total_surface/hs_A
+    total_surface_m2 = total_surface / hs_A
 
     return total_surface_m2, roofs_max_m2
 
 
 def plot_economical_feedin_price(bounds, resolution, Pareto):
-
     df_unit = return_district_result_object_dataframe(Pareto, 'df_Unit')
     df_KPIs = return_district_result_object_dataframe(Pareto, 'df_KPIs')
     hs_A = return_district_result_object_dataframe(Pareto, 'df_Buildings')["ERA"].xs(1, level=1).sum()
 
     df_nbr = return_district_result_object_dataframe(Pareto, 'df_PV_orientation')  # df_PVA_module_nbr, ["df_PV_orientation"]
     total_surface_m2, roof_max_m2 = get_roof_max(df_nbr, hs_A)
     # some data processing
@@ -102,15 +105,15 @@
             id = ["PV" in id for id in Pareto[0][i].df_Annuals.xs("Electricity")["Supply_MWh"].index]
             MWh_PV[i] = Pareto[0][i].df_Annuals.xs("Electricity")["Supply_MWh"][id].sum()
     MWh_PV = pd.DataFrame.from_dict(MWh_PV, orient="Index")[0]
     total_surface_m2.index.name = "Pareto"
 
     df_K = df_KPIs.xs((0, 'Network'), level=('Scn_ID', 'Hub'))
     SC = df_K.SC
-    MWh_PV.index=SC.index
+    MWh_PV.index = SC.index
 
     MWh_SC = MWh_PV.mul(SC)
     MWh_SC = MWh_SC.fillna(0)
     MWh_exp = MWh_PV - MWh_SC
     MWh_exp = MWh_exp.fillna(0)
 
     PV_kWyr = MWh_PV
@@ -183,33 +186,38 @@
             y_last = np.append(y_last, last_economic_point)
             y_inv_induced = np.append(y_inv_induced, inv_induced)
             y_first = np.append(y_first, first_economic_point)
         df_plot_last[d] = y_last
         df_plot_inv_induced[d] = y_inv_induced
         df_plot_first[d] = y_first
 
-    df_plot_first = df_plot_first.set_index(feed_in_prices)
+    # df_plot_first = df_plot_first.set_index(feed_in_prices)
     df_plot_last = df_plot_last.set_index(feed_in_prices)
     df_plot_inv_induced = df_plot_inv_induced.set_index(feed_in_prices)
+
     return df_plot_last, feed_in_prices, No_feed_in, df_plot_inv_induced
 
+
 def plot_rainbow(df_plot_last, feed_in_prices, No_feed_in, df_plot_inv_induced, bounds, save_fig, plot_type):
-    # plotting
+
     fig, ax = plt.subplots()
     for demand_price in df_plot_last.columns:
         if plot_type == "demand_feed_in_E_gen_pv":
             if all(pd.isnull(df_plot_last[demand_price].values)):
                 c_list = ["white"] * No_feed_in
             else:
                 c_list = df_plot_last[demand_price].values
-            cs = ax.scatter(feed_in_prices, np.repeat(demand_price, No_feed_in), c=c_list, s=5, cmap=cm, vmin = df_plot_last.min().min(), vmax = df_plot_last.max().max() )
+            cs = ax.scatter(feed_in_prices, np.repeat(demand_price, No_feed_in), c=c_list, s=5, cmap=cm, vmin=df_plot_last.min().min(),
+                            vmax=df_plot_last.max().max())
         elif plot_type == "E_gen_pv_demand_feed_in":
-            cs = ax.scatter(np.repeat(demand_price, No_feed_in), df_plot_last[demand_price].values, c=feed_in_prices, s=5, cmap=cm, vmin=bounds["feed_in"][0], vmax=bounds["feed_in"][1])
+            cs = ax.scatter(np.repeat(demand_price, No_feed_in), df_plot_last[demand_price].values, c=feed_in_prices, s=5, cmap=cm, vmin=bounds["feed_in"][0],
+                            vmax=bounds["feed_in"][1])
         elif plot_type == "invest_demand_feed_in":
-            cs = ax.scatter(np.repeat(demand_price, No_feed_in), df_plot_inv_induced[demand_price].values, c=feed_in_prices, s=5, cmap=cm, vmin=bounds["feed_in"][0], vmax=bounds["feed_in"][1])
+            cs = ax.scatter(np.repeat(demand_price, No_feed_in), df_plot_inv_induced[demand_price].values, c=feed_in_prices, s=5, cmap=cm,
+                            vmin=bounds["feed_in"][0], vmax=bounds["feed_in"][1])
 
     ax.annotate(' all PV investments \n economic feasible', (0.08, 0.22), zorder=10)
     cbar = fig.colorbar(cs)
 
     if plot_type == "demand_feed_in_E_gen_pv":
         ax.set_xlim(bounds["feed_in"][0], bounds["feed_in"][1])
         ax.set_ylim(bounds["retail"][0], bounds["retail"][1])
@@ -222,56 +230,56 @@
         ax.set_ylim(df_plot_last.min().min(), df_plot_last.max().max())
         ax.set_xlabel('retail tariff [CHF/kWh]')
         ax.set_ylabel('PV electricity generated [TWh/yr]')
         cbar.ax.set_ylabel('feed-in tariff  [CHF/kWh]')
 
     elif plot_type == "invest_demand_feed_in":
         ax.set_xlim(bounds["retail"][0], bounds["retail"][1])
-        ax.set_ylim(df_plot_inv_induced.min().min(),  df_plot_inv_induced.max().max())
+        ax.set_ylim(df_plot_inv_induced.min().min(), df_plot_inv_induced.max().max())
         ax.set_xlabel('retail tariff [CHF/kWh]')
         ax.set_ylabel('investment [CHF/yr]')
         cbar.ax.set_ylabel('feed-in tariff  [CHF/kWh]')
 
-    #ax.legend(loc='upper center', bbox_to_anchor=(0.5, -0.2), frameon=False, ncol=2)
+    # ax.legend(loc='upper center', bbox_to_anchor=(0.5, -0.2), frameon=False, ncol=2)
 
-    if save_fig == True:
+    if save_fig:
         plt.tight_layout()
         format = 'png'
         plt.savefig(('PV_rainbow_CH' + '.' + format), format=format, dpi=300)
     plt.show()
     return
 
 
-
 def return_district_result_object_dataframe(dict_results, result_dataframe):
     if result_dataframe in dir(dict_results[0][1]):
         t = {(j, k): getattr(dict_results[j][k], result_dataframe)
-                for j in dict_results.keys()
-                for k in dict_results[j].keys()}
+             for j in dict_results.keys()
+             for k in dict_results[j].keys()}
     else:
         t = {(j, k): dict_results[j][k][result_dataframe]
              for j in dict_results.keys()
              for k in dict_results[j].keys()}
 
     df_district_results = pd.concat(t.values(), keys=t.keys(), names=['Scn_ID', 'Pareto_ID'], axis=0)
     df_district_results = df_district_results.sort_index()
 
     return df_district_results
 
-def plot_rainbow_CH(Pareto_list, surface_district, surface_CH, CH_roof_area=None, bounds=None, resolution=100, std_filter=1.5, plot_type="demand_feed_in_E_gen_pv", filter=0):
 
+def plot_rainbow_CH(Pareto_list, surface_district, surface_CH, CH_roof_area=None, bounds=None, resolution=100, std_filter=1.5,
+                    plot_type="demand_feed_in_E_gen_pv", filter=0):
     if bounds is None:
         bounds = {"feed_in": [0.0, 0.15], "retail": [0.0, 0.30]}
 
     df_plot_last = {}
     df_plot_inv_induced = {}
 
     # get data
     for n, tr_id in enumerate(Pareto_list):
-        pareto = Pareto_list[tr_id]
+
         print("district:", n, " processed")
         df_plot_last[n], feed_in_prices, No_feed_in, df_plot_inv_induced[n] = plot_economical_feedin_price(bounds, resolution, Pareto_list)
 
         # get last economic retail tariffs
         last_id = []
         for idx, col in enumerate(df_plot_last[n]):
             if any(df_plot_last[n][col].notnull()):
@@ -282,24 +290,23 @@
                 else:
                     last_id = np.concatenate([last_id, [df_not_nan.index[0]]])
             else:
                 last_id = np.concatenate([last_id, [np.nan]])
         last_id = pd.DataFrame(last_id)
         last_id[0] = last_id[0].interpolate()
 
-
         for idx, col in enumerate(df_plot_last[n]):
             df_plot_last[n][col] = df_plot_last[n][col].replace(np.nan, 0)
             index_max_PV = df_plot_last[n][col].loc[last_id.loc[idx][0]:].index[1:]
             df_plot_last[n][col].loc[index_max_PV] = df_plot_last[n].max().max()
 
     # aggregate data and extrapolate to CH
     df_plot_last_CH = df_plot_last[0] * 0
     for n, tr_id in enumerate(Pareto_list):
-        if CH_roof_area != None:
+        if CH_roof_area is not None:
             ratio = list(surface_CH.values()) / np.sum(list(surface_CH.values()))
             df_plot_last_CH = df_plot_last_CH + df_plot_last[n] / surface_district[tr_id] * ratio[n] * CH_roof_area
         else:
             df_plot_last_CH = df_plot_last_CH + df_plot_last[n] / surface_district[tr_id] * surface_CH[tr_id]
 
     for col in df_plot_last_CH:
         df_plot_last_CH[col][df_plot_last_CH[col] < filter] = 0.0
@@ -316,22 +323,19 @@
     for col in df_plot_last_CH:
         df_plot_last_CH[col].mask(df_plot_last_CH[col] < 0.03, np.nan, inplace=True)
         df_plot_last_CH[col].mask(df_plot_last_CH[col] > max_value - 0.1, np.nan, inplace=True)
 
     plot_rainbow(df_plot_last_CH, feed_in_prices, No_feed_in, df_plot_inv_induced, bounds, save_fig=True, plot_type=plot_type)
 
 
-
 if __name__ == '__main__':
-
     plt.rcParams.update({'font.size': 14})
     cm = plt.cm.get_cmap('Spectral')
 
     Pareto = pd.read_pickle("results.pickle")
 
     surfaces_districts = {0: 100, 1: 200, 2: 300, 3: 400, 4: 500}  # surface of the typical districts in m2
     surfaces_country = {0: 1, 1: 2, 2: 3, 3: 4, 4: 5}  # representative surface of the typical districts at the national scale in 10e6 m2
     data = {i: Pareto[n] for i, n in enumerate(Pareto)}
 
     plot_rainbow_CH(data, surface_district=surfaces_districts, surface_CH=surfaces_country,
                     resolution=140, std_filter=1.5, plot_type="demand_feed_in_E_gen_pv", filter=6)
-
```

### Comparing `REHO-1.0.2/reho/plotting/sankey.py` & `reho-1.1.0/reho/plotting/sankey.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 import re
 import pandas as pd
 import numpy as np
 from reho.paths import *
 
 __doc__ = """
-*Builds the dataframe for the visualization of annual flows from REHO results in the form of a Sankey diagram.*
+Builds the dataframe for the visualization of annual flows from REHO results in the form of a Sankey diagram.
 """
 
 # Colors and labels for units and layers
 layout = pd.read_csv(os.path.join(path_to_plotting, 'layout.csv'), index_col='Name').dropna(how='all')
 
+
 def update_label(source_name, target_name, df_label):
     """
         update labels of df_label if source_name or target_name not in index of df_label
 
         Parameters:
             source_name (string) : first name to update
             target_name (string) : second name to update
-            df_label (df): dataframe with labels
+            df_label (df) : pd.DataFrame with labels
 
         Returns:
             df_label (df) updated
     """
     if not (source_name in df_label.index):  # create label 'source' if not existing yet
         df_label.loc[source_name, 'pos'] = len(df_label)
     if not (target_name in df_label.index):  # create label 'target' if not existing yet
         df_label.loc[target_name, 'pos'] = len(df_label)
     return df_label
 
+
 def add_label_value(df_label, df_stv, precision, units):
     """
         add the values from df_stv to the labels of df_labels
         The value of the nodes are thus available in the nodes name for the sankey diagram
 
         Parameters:
-            df_label (df): dataframe of labels
-            df_stv (df): dataframe of source, target and value
+            df_label (df) : pd.DataFrame of labels
+            df_stv (df) : pd.DataFrame of source, target and value
             precision (int): precision of the displayed numbers (default = 2)
             units (string): unit of the values (default MWh)
 
         Returns:
             df label updated with the label values
     """
     df_source_value = pd.DataFrame()
@@ -48,17 +50,18 @@
     for i in list(df_source_value.index):
         source_val = df_stv.loc['value', df_stv.loc['source', :] == i].sum()
         target_val = df_stv.loc['value', df_stv.loc['target', :] == i].sum()
         # higher value on the node is displayed, (i.e. size of the box node on the sankey)
         df_source_value.loc[i, 'value'] = max(source_val, target_val)
 
     df_label = df_label.merge(df_source_value, left_on='pos', right_index=True)
-    df_label.label = df_label.label+"\n"+df_label.value.round(precision).astype(str)+units
+    df_label.label = df_label.label + "\n" + df_label.value.round(precision).astype(str) + units
     return df_label
 
+
 def add_flow(source, dest, layer, hub, dem_sup, df_annuals, df_label, df_stv, check_dest_2=False, dest_2=None, adjustment=0, fact=1):
     """
         Add an energy flow for the sankey diagramm for 'sankey_plot' according (a) cell(s) of df_annuals if cell not null
 
         Parameters:
             source (string) : name of the source
             dest (string) : name of the destination
@@ -72,68 +75,68 @@
             dest_2 (string) : second possible destination (default none)
             adjustment (float) : offset added to the cell value (default 0)
             fact (float) : factor multiplied to the cell value (default 1)
 
         Returns:
             df_label updated (df), df_stv updated (df), value added (float, 0 if nothing added)
     """
-    source_to_dest = df_annuals.loc[(df_annuals['Layer'] == layer) & (df_annuals['Hub'] == hub)][dem_sup].sum() # .sum() to add all the values of the buildings if multiple buildings
-    if source_to_dest != 0:                                                     # if data available
-        if check_dest_2:                                                        # if True apply the second dest
+    source_to_dest = df_annuals.loc[(df_annuals['Layer'] == layer) & (df_annuals['Hub'] == hub)][
+        dem_sup].sum()  # .sum() to add all the values of the buildings if multiple buildings
+    if source_to_dest != 0:  # if data available
+        if check_dest_2:  # if True apply the second dest
             dest = dest_2
-        df_label = update_label(source, dest, df_label)                         # update label list
-        df_stv[source+'_to_'+dest] = [df_label.loc[source, 'pos'],              # source, create a source to target column
-                                      df_label.loc[dest, 'pos'],                # target
-                                      float(fact*source_to_dest+adjustment)]    # value
+        df_label = update_label(source, dest, df_label)  # update label list
+        df_stv[source + '_to_' + dest] = [df_label.loc[source, 'pos'],  # source, create a source to target column
+                                          df_label.loc[dest, 'pos'],  # target
+                                          float(fact * source_to_dest + adjustment)]  # value
+
+    return df_label, df_stv, fact * source_to_dest + adjustment
 
-    return df_label, df_stv, fact*source_to_dest+adjustment
 
 def df_sankey(df_results, label='FR_long', color='ColorPastel', precision=2, units='MWh', display_label_value=True, scaling_factor=1):
-    # Hypothèses :
+    # Hypotheses :
     # 1. DHW demand taken as the supply of the watertank DHW
     # 2. no flow: electrical storage system to grid feed in, all to 'feed in electrical grid ' is from PV
     # 3. Small losses of NG, heat, wood,... between network and devices not accounted
     # 4. Electricity for 'Data heat' fully accounted as electricity consumption (Layer Data: not in sankey)
-    # 5. Electricity produced by technologies can be stored (eg. NG_cogen elec -> battery)
+    # 5. Electricity produced by technologies can be stored (e.g. NG_cogen elec -> battery)
 
     # Multi building :
     # supported
 
     # !! MAKE SURE : all the possible technologies/sources/demands are in the list below (if not, risk that sth will be
     # not displayed, there is no check provided by this function for that)
     # List of supported technologies/sources/demands
     # Electrical storage device
     elec_storage_list = ['Battery', 'EV_district']
     # Manual handled devices (list below not used, just here for the information)
-    manual_device     = ['PV', 'WaterTankSH']
+    # manual_device = ['PV', 'WaterTankSH']
     # Semi automatic handled devices
-    semi_auto_device  = ['HeatPump_Air', 'HeatPump_DHN', 'NG_Boiler', 'ThermalSolar', 'OIL_Boiler',
-                         'ElectricalHeater_DHW', 'ElectricalHeater_SH', 'NG_Cogeneration', 'DHN_in',
-                         'HeatPump_Lake', 'WOOD_Stove', 'HeatPump_Geothermal', 'Air_Conditioner',
-                         'DataHeat_DHW'] # name must be the same as used by REHO
+    semi_auto_device = ['HeatPump_Air', 'HeatPump_DHN', 'NG_Boiler', 'ThermalSolar', 'OIL_Boiler',
+                        'ElectricalHeater_DHW', 'ElectricalHeater_SH', 'NG_Cogeneration', 'DHN_in',
+                        'HeatPump_Lake', 'WOOD_Stove', 'HeatPump_Geothermal', 'Air_Conditioner',
+                        'DataHeat_DHW']  # name must be the same as used by REHO
     # Network (electrical grid, oil network...) and end use demand (DHW, SH, elec appliances) handled automatically
 
-
-
     # Select only not null lines in df_annuals
-    df_annuals = scaling_factor*df_results['df_Annuals']
+    df_annuals = scaling_factor * df_results['df_Annuals']
     df_annuals = df_annuals.replace(0, np.nan)
     df_annuals = df_annuals.loc[df_annuals['Demand_MWh'].notnull() | df_annuals['Supply_MWh'].notnull()]
     df_annuals = df_annuals.replace(np.nan, 0).reset_index()
 
     # "Building" string management in data to deal with data uniformly regarding buildings
     for x in list(df_annuals.index):
-        if df_annuals.loc[x, "Hub"].startswith('Building'): #all Buildingx -> Building
+        if df_annuals.loc[x, "Hub"].startswith('Building'):  # all Buildingx -> Building
             df_annuals.loc[x, "Hub"] = "Building"
-        else:                                               #else remove '_Buildingx' of the hub name
+        else:  # else remove '_Buildingx' of the hub name
             df_annuals.loc[x, "Hub"] = re.sub("_Building\d+", "", df_annuals.loc[x, "Hub"])
 
     # Creating the dataframe for the following
-    df_label = pd.DataFrame(columns=['pos'])                      # df for labels, position number (pos) and colors
-    df_stv   = pd.DataFrame(index=['source', 'target', 'value'])  # df for source,target,value
+    df_label = pd.DataFrame(columns=['pos'])  # df for labels, position number (pos) and colors
+    df_stv = pd.DataFrame(index=['source', 'target', 'value'])  # df for source,target,value
 
     # check if electricity storage
     elec_storage_use = False
     for elec_storage in elec_storage_list:
         if len(df_annuals.loc[(df_annuals['Layer'] == 'Electricity') & (df_annuals['Hub'] == elec_storage)]) != 0:
             elec_storage_use = True
 
@@ -160,27 +163,27 @@
                                    -pv_to_egf)
 
     # 5 WaterTankSH to SH
     df_label, df_stv, wtsh_to_sh = add_flow('WaterTankSH', 'SH', 'SH', 'WaterTankSH', 'Supply_MWh',
                                             df_annuals, df_label, df_stv)
 
     # Calculation of Losses in the watertank
-    heat_tot_sh  = df_annuals.loc[(df_annuals['Layer'] == 'SH') & (df_annuals['Hub'] == 'Building')].Demand_MWh.sum()
+    heat_tot_sh = df_annuals.loc[(df_annuals['Layer'] == 'SH') & (df_annuals['Hub'] == 'Building')].Demand_MWh.sum()
     heat_tot_sup = df_annuals.loc[(df_annuals['Layer'] == 'SH')].Supply_MWh.sum() - wtsh_to_sh
     heat_loss_wt = heat_tot_sup - heat_tot_sh
 
     # 6 SH Heat to Watertank SH if watertank
     df_label, df_stv, _ = add_flow('SH_heat', 'WaterTankSH', 'SH', 'WaterTankSH', 'Supply_MWh',
                                    df_annuals, df_label, df_stv, adjustment=heat_loss_wt)
 
     # 7 SH Heat to SH if watertank
     df_label, df_stv, _ = add_flow('SH_heat', 'SH', 'SH', 'WaterTankSH', 'Supply_MWh',
-                                   df_annuals, df_label, df_stv, adjustment=heat_tot_sup-heat_loss_wt, fact=-1)
+                                   df_annuals, df_label, df_stv, adjustment=heat_tot_sup - heat_loss_wt, fact=-1)
 
-    elec_storage_energy_in  = 0
+    elec_storage_energy_in = 0
     elec_storage_energy_out = 0
     for elec_storage in elec_storage_list:
         # 8 Electrical cons before elec storage to storage device
         df_label, df_stv, dev_flow_in = add_flow('Electrical_consumption_bp', elec_storage, 'Electricity', elec_storage,
                                                  'Demand_MWh', df_annuals, df_label, df_stv)
         elec_storage_energy_in += dev_flow_in
 
@@ -188,23 +191,23 @@
         df_label, df_stv, dev_flow_out = add_flow(elec_storage, 'Electrical_consumption', 'Electricity', elec_storage,
                                                   'Supply_MWh', df_annuals, df_label, df_stv)
         elec_storage_energy_out += dev_flow_out
 
     # 10 Electrical cons before elec storage to Electr cons
     if elec_storage_use:
         df_label = update_label('Electrical_consumption_bp', 'Electrical_consumption', df_label)
-        Ec_after_bp =  df_annuals.loc[(df_annuals['Layer'] == 'Electricity') & (df_annuals['Hub'] != 'Network')].Demand_MWh.sum()
+        Ec_after_bp = df_annuals.loc[(df_annuals['Layer'] == 'Electricity') & (df_annuals['Hub'] != 'Network')].Demand_MWh.sum()
         Ec_after_bp -= elec_storage_energy_out
         df_stv['Electrical_consumption_bp_to_Electrical_consumption'] = [df_label.loc['Electrical_consumption_bp', 'pos'],
                                                                          df_label.loc['Electrical_consumption', 'pos'],
-                                                                         float(Ec_after_bp-elec_storage_energy_in)]
+                                                                         float(Ec_after_bp - elec_storage_energy_in)]
 
     # Semi-Auto for the followings devices
     for device in semi_auto_device:
-        abr_hp = device
+        
         # 1 Ele Cons to Device
         df_label, df_stv, _ = add_flow('Electrical_consumption', device, 'Electricity', device, 'Demand_MWh',
                                        df_annuals, df_label, df_stv)
 
         # 2 Heat to Device
         df_label, df_stv, _ = add_flow('Heat', device, 'Heat', device, 'Demand_MWh',
                                        df_annuals, df_label, df_stv)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `REHO-1.0.2/setup.py` & `reho-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 # All rights reserved. ECOLE POLYTECHNIQUE FEDERALE DE LAUSANNE, Switzerland,
 # IPESE Laboratory, Copyright 2021
 # This work can be distributed under the Apache Software License.
 # See the LICENSE file for more details.
 
-import subprocess
-import sys
 from setuptools import setup, find_packages
 
 
 def read_file(file_path):
     with open(file_path, 'r', encoding='utf-8') as file:
         return file.read()
-    
-def install_dependencies():
-    try:
-        subprocess.run([sys.executable, '-m', 'pip', 'install', 'psycopg2'])
-    except subprocess.CalledProcessError:
-        subprocess.run([sys.executable, '-m', 'pip', 'install', 'psycopg2-binary'])
 
 
 setup(
 
     name='REHO',
-    version='1.0.2',
+    version='1.1.0',
     packages=find_packages(),
     include_package_data=True,
     install_requires=['amplpy>=0.12.0,<0.13.0',
                       'ampl_module_base',
                       'ampl_module_highs',
                       'pandas>=1.5.3,<2.0.0',
                       'openpyxl>=3.1.2,<4.0.0',
@@ -37,14 +29,18 @@
                       'sqlalchemy>=1.4.42,<2.0.0',
                       'geopandas>=0.12.2,<1.0.0',
                       'matplotlib>=3.6.1,<4.0.0',
                       'plotly>=5.10,<6.0.0',
                       'kaleido>=0.2.1,<1.0.0',
                       'python-dotenv>=1.0',
                       'requests>=2.0.0,<3.0.0',
+                      'coloredlogs>=15.0.1',
+                      'SALib>=1.4.8',
+                      'qmcpy>=1.4.5',
+                      'pvlib==0.10.*'
                       ],
     package_data={
           '': ['*.csv', '*.xlsx', '*.dat', '*.txt' '*.mod', '*.ini'],
       },
     author='Dorsan Lepour',
     author_email='dorsan.lepour@epfl.ch',
     maintainer="IT team of IPESE Laboratory from EPFL",
```

